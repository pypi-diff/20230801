# Comparing `tmp/datapipe_label_studio_lite-0.2.0.tar.gz` & `tmp/datapipe_label_studio_lite-0.3.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_label_studio_lite-0.2.0.tar", max compression
+gzip compressed data, was "datapipe_label_studio_lite-0.3.0a2.tar", max compression
```

## Comparing `datapipe_label_studio_lite-0.2.0.tar` & `datapipe_label_studio_lite-0.3.0a2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       22 2023-02-17 19:44:15.747201 datapipe_label_studio_lite-0.2.0/datapipe_label_studio_lite/__init__.py
--rw-r--r--   0        0        0    13931 2023-02-17 22:35:27.162092 datapipe_label_studio_lite-0.2.0/datapipe_label_studio_lite/pipeline.py
--rw-r--r--   0        0        0     4134 2023-02-17 19:44:15.747201 datapipe_label_studio_lite-0.2.0/datapipe_label_studio_lite/sdk_utils.py
--rw-r--r--   0        0        0      837 2023-02-17 22:35:27.162092 datapipe_label_studio_lite-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 datapipe_label_studio_lite-0.2.0/setup.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 datapipe_label_studio_lite-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-02-17 19:44:15.747201 datapipe_label_studio_lite-0.3.0a2/datapipe_label_studio_lite/__init__.py
+-rw-r--r--   0        0        0    15585 2023-08-01 07:38:45.976010 datapipe_label_studio_lite-0.3.0a2/datapipe_label_studio_lite/pipeline.py
+-rw-r--r--   0        0        0     3988 2023-07-22 18:38:48.120921 datapipe_label_studio_lite-0.3.0a2/datapipe_label_studio_lite/sdk_utils.py
+-rw-r--r--   0        0        0      862 2023-08-01 07:38:45.976010 datapipe_label_studio_lite-0.3.0a2/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 datapipe_label_studio_lite-0.3.0a2/PKG-INFO
```

### Comparing `datapipe_label_studio_lite-0.2.0/datapipe_label_studio_lite/pipeline.py` & `datapipe_label_studio_lite-0.3.0a2/datapipe_label_studio_lite/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 import numpy as np
 import pandas as pd
-from typing import Any, Union, List, Optional
+from typing import Any, Dict, Union, List, Optional
 from datetime import datetime, timezone
 from dataclasses import dataclass
 from datapipe.run_config import RunConfig
 from datapipe.store.database import TableStoreDB
 
 from sqlalchemy import Integer, Column, JSON, DateTime
 
-from datapipe.types import ChangeList, data_to_index, index_to_data
+from datapipe.types import IndexDF, data_to_index, index_difference, index_to_data
 from datapipe.compute import (
     PipelineStep,
     DataStore,
     Table,
     Catalog,
-    DatatableTransformStep,
 )
-from datapipe.core_steps import BatchTransformStep, DataTable
+from datapipe.core_steps import BatchTransformStep, DataTable, DatatableTransformStep
 from datapipe.store.database import DBConn
+from datapipe.core_steps import logger
 import label_studio_sdk
 from datapipe_label_studio_lite.sdk_utils import get_project_by_title, get_tasks_iter
 from label_studio_sdk.data_manager import Filters, Operator, Type, DATETIME_FORMAT
 
 
-class DatatableTransformStepNoChangeList(DatatableTransformStep):
-    def run_changelist(
-        self, ds: DataStore, changelist: ChangeList, run_config: RunConfig = None
-    ) -> ChangeList:
-        return ChangeList()
-
-
 @dataclass
 class LabelStudioStep(PipelineStep):
     input: str  # Input Table name
     output: str  # Output Table name
     sync_table: str
 
     ls_url: str
@@ -44,27 +37,22 @@
 
     name: Optional[str] = None
 
     project_label_config_at_create: str = ""
     project_description_at_create: str = ""
 
     create_table: bool = False
+    delete_unannotated_tasks_only_on_update: bool = False
 
     def __post_init__(self):
         assert self.dbconn is not None
         self.data_sql_schema: List[Column] = [column for column in self.data_sql_schema]
-        self.data_sql_schema_primary: List[Column] = [
-            column for column in self.data_sql_schema if column.primary_key
-        ]
-        self.data_columns: List[str] = [
-            column.name for column in self.data_sql_schema if not column.primary_key
-        ]
-        self.primary_keys = [
-            column.name for column in self.data_sql_schema if column.primary_key
-        ]
+        self.data_sql_schema_primary: List[Column] = [column for column in self.data_sql_schema if column.primary_key]
+        self.data_columns: List[str] = [column.name for column in self.data_sql_schema if not column.primary_key]
+        self.primary_keys = [column.name for column in self.data_sql_schema if column.primary_key]
         for column in ["task_id", "annotations"]:
             assert (
                 column not in self.data_columns and column not in self.primary_keys
             ), f'The column "{column}" is reserved for this PipelineStep.'
         if isinstance(self.project_identifier, str):
             assert len(self.project_identifier) <= 50
 
@@ -159,31 +147,26 @@
             response.raise_for_status()
 
     def _convert_data_if_need(self, value: Any):
         if isinstance(value, np.int64):
             return int(value)
         return value
 
-    def build_compute(
-        self, ds: DataStore, catalog: Catalog
-    ) -> List[DatatableTransformStep]:
+    def build_compute(self, ds: DataStore, catalog: Catalog) -> List[DatatableTransformStep]:
         input_dt = catalog.get_datatable(ds, self.input)
         input_uploader_dt = ds.get_or_create_table(
             f"{self.input}_upload",
             TableStoreDB(
                 dbconn=self.dbconn,
                 name=f"{self.input}_upload",
-                data_sql_schema=self.data_sql_schema_primary
-                + [Column("task_id", Integer)],
+                data_sql_schema=self.data_sql_schema_primary + [Column("task_id", Integer)],
                 create_table=self.create_table,
             ),
         )
-        catalog.add_datatable(
-            f"{self.input}_upload", Table(input_uploader_dt.table_store)
-        )
+        catalog.add_datatable(f"{self.input}_upload", Table(input_uploader_dt.table_store))
         sync_datetime_dt = ds.get_or_create_table(
             self.sync_table,
             TableStoreDB(
                 dbconn=self.dbconn,
                 name=self.sync_table,
                 data_sql_schema=[
                     Column("project_id", Integer, primary_key=True),
@@ -194,92 +177,124 @@
         )
         catalog.add_datatable(self.sync_table, Table(sync_datetime_dt.table_store))
         output_dt = ds.get_or_create_table(
             self.output,
             TableStoreDB(
                 dbconn=self.dbconn,
                 name=self.output,
-                data_sql_schema=self.data_sql_schema_primary
-                + [Column("annotations", JSON)],
+                data_sql_schema=self.data_sql_schema_primary + [Column("annotations", JSON)],
                 create_table=self.create_table,
             ),
         )
         catalog.add_datatable(self.output, Table(output_dt.table_store))
 
-        def upload_tasks(df: pd.DataFrame):
+        def upload_tasks(df: pd.DataFrame, idx: IndexDF):
             """
             Добавляет в LS новые задачи с заданными ключами.
             (Не поддерживает удаление задач, если в input они пропадают)
             """
-            if df.empty or len(df) == 0:
-                return
+            if df.empty and idx.empty:
+                return pd.DataFrame(columns=self.primary_keys + ["task_id"])
 
-            # Удаляем существующие задачи и перезаливаем их
-            df_idx = data_to_index(df, self.primary_keys)
-            existing_tasks_df_without_annotations = input_uploader_dt.get_data(
-                idx=df_idx
-            )
-            if len(existing_tasks_df_without_annotations) > 0:
-                existing_idx = data_to_index(
-                    existing_tasks_df_without_annotations, self.primary_keys
-                )
-                df_to_be_deleted = pd.merge(
-                    left=index_to_data(df, existing_idx),
-                    right=existing_tasks_df_without_annotations[
-                        self.primary_keys + ["task_id"]
+            idx = data_to_index(idx, self.primary_keys)
+            if self.delete_unannotated_tasks_only_on_update:
+                df_idx = data_to_index(df, self.primary_keys)
+                df_existing_tasks = input_uploader_dt.get_data(idx=idx)
+                df_existing_tasks_with_output = pd.merge(df_existing_tasks, output_dt.get_data(idx=idx), how="left")
+                deleted_idx = index_difference(df_idx, idx)
+                if len(df_existing_tasks_with_output) > 0:
+                    have_annotations = df_existing_tasks_with_output["annotations"].apply(
+                        lambda ann: not pd.isna(ann) and len(ann) > 0
+                    )
+                    df_existing_tasks_to_be_stayed = df_existing_tasks_with_output[have_annotations]
+                    df_existing_tasks_to_be_deleted = pd.merge(
+                        df_existing_tasks_with_output[~have_annotations], deleted_idx, how="outer"
+                    )
+                else:
+                    df_existing_tasks_to_be_stayed = pd.DataFrame(columns=self.primary_keys + ["task_id"])
+                    df_existing_tasks_to_be_deleted = pd.merge(
+                        pd.DataFrame(columns=self.primary_keys + ["task_id"]), deleted_idx, how="outer"
+                    )
+                df_to_be_uploaded = pd.concat(
+                    [
+                        pd.merge(df, df_existing_tasks_to_be_deleted, on=self.primary_keys),
+                        index_to_data(
+                            df,
+                            index_difference(
+                                index_difference(
+                                    df_idx, data_to_index(df_existing_tasks_to_be_stayed, self.primary_keys)
+                                ),
+                                data_to_index(df_existing_tasks_to_be_deleted, self.primary_keys),
+                            ),
+                        ),
                     ],
-                    on=self.primary_keys,
+                    ignore_index=True,
                 )
-                for task_id in df_to_be_deleted["task_id"]:
+            else:
+                df_existing_tasks_to_be_deleted = input_uploader_dt.get_data(idx=idx)
+                df_to_be_uploaded = df
+
+            if len(df_existing_tasks_to_be_deleted) > 0:
+                for task_id in df_existing_tasks_to_be_deleted["task_id"]:
                     self._delete_task_from_project(task_id)
+                output_dt.delete_by_idx(
+                    idx=data_to_index(df_existing_tasks_to_be_deleted, self.primary_keys)
+                )
 
-            # Добавляем новые задачи
-            data_to_be_added = [
-                {
-                    "data": {
-                        **{
-                            primary_key: self._convert_data_if_need(
-                                df.loc[idx, primary_key]
-                            )
-                            for primary_key in self.primary_keys + self.data_columns
+            if df.empty:
+                return pd.DataFrame(columns=self.primary_keys + ["task_id"])
+
+            if len(df_to_be_uploaded) > 0:
+                data_to_be_added = [
+                    {
+                        "data": {
+                            **{
+                                primary_key: self._convert_data_if_need(df_to_be_uploaded.loc[idx, primary_key])
+                                for primary_key in self.primary_keys + self.data_columns
+                            }
                         }
                     }
-                }
-                for idx in df.index
-            ]
-            tasks_added = self.project.import_tasks(tasks=data_to_be_added)
-            df["task_id"] = tasks_added
-            return df[self.primary_keys + ["task_id"]]
+                    for idx in df_to_be_uploaded.index
+                ]
+                tasks_added = self.project.import_tasks(tasks=data_to_be_added)
+                df_to_be_uploaded["task_id"] = tasks_added
+
+            if self.delete_unannotated_tasks_only_on_update:
+                df_res = pd.concat([df_existing_tasks_to_be_stayed, df_to_be_uploaded], ignore_index=True)
+            else:
+                df_res = df_to_be_uploaded
+            logger.debug(
+                f"Deleted {len(df_existing_tasks_to_be_deleted)} tasks, uploaded {len(df_to_be_uploaded)} tasks."
+            )
+            return df_res[self.primary_keys + ["task_id"]]
 
         def get_annotations_from_ls(
             ds: DataStore,
             input_dts: List[DataTable],
             output_dts: List[DataTable],
             run_config: RunConfig,
+            kwargs: Dict[str, Any],
         ):
             """
             Записывает в табличку задачи из сервера LS вместе с разметкой согласно
             дате последней синхронизации
             """
+
             # created_ago - очень плохой параметр, он меняется каждый раз, когда происходит запрос
             def _cleanup(values):
                 for ann in values:
                     if "created_ago" in ann:
                         del ann["created_ago"]
                 return values
 
-            sync_datetime_df = sync_datetime_dt.get_data(
-                idx=pd.DataFrame({"project_id": [self.project.id]})
-            )
+            sync_datetime_df = sync_datetime_dt.get_data(idx=pd.DataFrame({"project_id": [self.project.id]}))
 
             if sync_datetime_df.empty:
                 sync_datetime_df.loc[0, "project_id"] = self.project.id
-                sync_datetime_df.loc[0, "last_updated_at"] = datetime.fromtimestamp(
-                    0, tz=timezone.utc
-                )
+                sync_datetime_df.loc[0, "last_updated_at"] = datetime.fromtimestamp(0, tz=timezone.utc)
 
             last_sync = sync_datetime_df.loc[0, "last_updated_at"]
 
             filters = Filters.create(
                 conjunction="and",
                 items=[
                     Filters.item(
@@ -288,49 +303,41 @@
                         column_type=Type.Datetime,
                         value=Filters.value(value=Filters.datetime(last_sync)),
                     )
                 ],
             )
             updated_ats = []
             for tasks_page in get_tasks_iter(self.project, filters=filters):
-                updated_ats.extend(
-                    [
-                        datetime.strptime(task["updated_at"], DATETIME_FORMAT)
-                        for task in tasks_page
-                    ]
-                )
+                updated_ats.extend([datetime.strptime(task["updated_at"], DATETIME_FORMAT) for task in tasks_page])
                 output_df = pd.DataFrame.from_records(
                     {
                         **{
-                            primary_key: [
-                                task["data"][primary_key] for task in tasks_page
-                            ]
+                            primary_key: [task["data"][primary_key] for task in tasks_page]
                             for primary_key in self.primary_keys
                         },
-                        "annotations": [
-                            _cleanup(task["annotations"]) for task in tasks_page
-                        ],
+                        "annotations": [_cleanup(task["annotations"]) for task in tasks_page],
                     }
                 )
                 output_dts[0].store_chunk(output_df)
 
             if len(updated_ats) > 0:
                 sync_datetime_df.loc[0, "last_updated_at"] = max(updated_ats)
                 sync_datetime_dt.store_chunk(sync_datetime_df)
 
         return [
             BatchTransformStep(
+                ds=ds,
                 name=f"{self.name_prefix}upload_data_to_ls",
-                labels={"step": "upload_data_to_ls"},
+                labels=[("stage", "upload_data_to_ls")],
                 func=upload_tasks,
                 input_dts=[input_dt],
                 output_dts=[input_uploader_dt],
                 chunk_size=100,
             ),
-            DatatableTransformStepNoChangeList(
+            DatatableTransformStep(
                 name=f"{self.name_prefix}get_annotations_from_ls",
                 func=get_annotations_from_ls,
                 input_dts=[],
                 output_dts=[output_dt],
                 check_for_changes=False,
             ),
         ]
```

### Comparing `datapipe_label_studio_lite-0.2.0/datapipe_label_studio_lite/sdk_utils.py` & `datapipe_label_studio_lite-0.3.0a2/datapipe_label_studio_lite/sdk_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,60 +2,44 @@
 import label_studio_sdk
 from urllib.parse import urljoin
 from typing import Any, Dict, Iterator, List, Optional
 
 
 def sign_up(ls_url: str, email: str, password: str) -> Optional[str]:
     session = requests.Session()
-    response_first = session.get(
-        url=urljoin(ls_url, 'user/signup/')
-    )
+    response_first = session.get(url=urljoin(ls_url, "user/signup/"))
     response_signup = session.post(
-        url=urljoin(ls_url, 'user/signup/'),
-        data={
-            'csrfmiddlewaretoken': response_first.cookies['csrftoken'],
-            'email': email,
-            'password': password
-        }
+        url=urljoin(ls_url, "user/signup/"),
+        data={"csrfmiddlewaretoken": response_first.cookies["csrftoken"], "email": email, "password": password},
     )
     if not response_signup.ok:
-        raise ValueError('Signup failed.')
-    api_key = session.get(
-        url=urljoin(ls_url, 'api/current-user/token')
-    ).json()
-    if 'token' in api_key:
-        return api_key['token']
+        raise ValueError("Signup failed.")
+    api_key = session.get(url=urljoin(ls_url, "api/current-user/token")).json()
+    if "token" in api_key:
+        return api_key["token"]
     return None
 
 
 def login_and_get_token(ls_url: str, email: str, password: str) -> str:
     session = requests.Session()
-    response = session.get(
-        url=urljoin(ls_url, 'user/login/')
-    )
+    response = session.get(url=urljoin(ls_url, "user/login/"))
     session.post(
-        url=urljoin(ls_url, 'user/login/'),
-        data={
-            'csrfmiddlewaretoken': response.cookies['csrftoken'],
-            'email': email,
-            'password': password
-        }
+        url=urljoin(ls_url, "user/login/"),
+        data={"csrfmiddlewaretoken": response.cookies["csrftoken"], "email": email, "password": password},
     )
-    api_key = session.get(
-        url=urljoin(ls_url, 'api/current-user/token')
-    ).json()
-    if 'token' in api_key:
-        return api_key['token']
+    api_key = session.get(url=urljoin(ls_url, "api/current-user/token")).json()
+    if "token" in api_key:
+        return api_key["token"]
     else:
         raise ValueError("Login failed.")
 
 
 def get_project_by_title(ls: label_studio_sdk.Client, title: str) -> Optional[label_studio_sdk.Project]:
     projects: List[label_studio_sdk.Project] = ls.get_projects()
-    titles = [project.get_params()['title'] for project in projects]
+    titles = [project.get_params()["title"] for project in projects]
     if title in titles:
         assert titles.count(title) == 1, f'There are 2 or more projects with title="{title}"'
         return projects[titles.index(title)]
     return None
 
 
 def is_service_up(ls: label_studio_sdk.Client, raise_exception: bool = False) -> bool:
@@ -73,15 +57,15 @@
     project: label_studio_sdk.Project,
     filters=None,
     ordering=None,
     view_id=None,
     selected_ids=None,
     only_ids: bool = False,
 ) -> Iterator[List[Dict[str, Any]]]:
-    """ Retrieve a subset of tasks from the Data Manager based on a filter, ordering mechanism, or a
+    """Retrieve a subset of tasks from the Data Manager based on a filter, ordering mechanism, or a
     predefined view ID.
 
     Parameters
     ----------
     filters: label_studio_sdk.data_manager.Filters.create()
         JSON objects representing Data Manager filters. Use `label_studio_sdk.data_manager.Filters.create()`
         helper to create it.
@@ -124,14 +108,14 @@
             data = project.get_paginated_tasks(
                 filters=filters,
                 ordering=ordering,
                 view_id=view_id,
                 selected_ids=selected_ids,
                 only_ids=only_ids,
                 page=page,
-                page_size=100
+                page_size=100,
             )
-            yield data['tasks']
+            yield data["tasks"]
             page += 1
         # we'll get 404 from API on empty page
         except label_studio_sdk.project.LabelStudioException:
             break
```

### Comparing `datapipe_label_studio_lite-0.2.0/pyproject.toml` & `datapipe_label_studio_lite-0.3.0a2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [tool.poetry]
 name = "datapipe-label-studio-lite"
-version = "0.2.0"
+version = "0.3.0-alpha.2"
 description = ""
 authors = [
     "Alexander Kozlov <bobokvsky@epoch8.co>",
     "Andrey Tatarinov <a@tatarinov.co>",
 ]
 
-exclude = ["tests", "examples"]
+exclude = ["tests", "experiments"]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 pandas = "^1.2.0"
 numpy = "^1.21.0"
 SQLAlchemy = "^1.4.25"
-tqdm = "^4.60.0"
 requests = "^2.24.0"
-datapipe-core = {version=">=0.11.12-dev.1, <0.12", extras=["sqlite"], allow-prereleases = true}
-iteration-utilities = "^0.11.0"
+datapipe-core = {version=">=0.13.0-alpha.5, <0.14", allow-prereleases = true}
 label-studio-sdk = "^0.0.16"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-xdist = "*"
-flake8 = "^3.9.2"
-mypy = "^0.910"
-black = "^21.7b0"
+flake8 = "*"
+mypy = "*"
+black = "*"
 pandas-stubs = "^1.2.0"
 types-requests = "^2.25.6"
 pytest-cases = "^3.6.4"
 types-setuptools = "^57.4.7"
+datapipe-core = {version=">=0.13.0-alpha.5, <0.14", extras=["sqlite"], allow-prereleases = true}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datapipe_label_studio_lite-0.2.0/PKG-INFO` & `datapipe_label_studio_lite-0.3.0a2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: datapipe-label-studio-lite
-Version: 0.2.0
+Version: 0.3.0a2
 Summary: 
 Author: Alexander Kozlov
 Author-email: bobokvsky@epoch8.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: SQLAlchemy (>=1.4.25,<2.0.0)
-Requires-Dist: datapipe-core[sqlite] (>=0.11.12-dev.1,<0.12)
-Requires-Dist: iteration-utilities (>=0.11.0,<0.12.0)
+Requires-Dist: datapipe-core (>=0.13.0-alpha.5,<0.14)
 Requires-Dist: label-studio-sdk (>=0.0.16,<0.0.17)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pandas (>=1.2.0,<2.0.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
-Requires-Dist: tqdm (>=4.60.0,<5.0.0)
```

