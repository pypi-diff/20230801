# Comparing `tmp/datapipe_app-0.3.2.dev2.tar.gz` & `tmp/datapipe_app-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_app-0.3.2.dev2.tar", max compression
+gzip compressed data, was "datapipe_app-0.4.0a1.tar", max compression
```

## Comparing `datapipe_app-0.3.2.dev2.tar` & `datapipe_app-0.4.0a1.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0     1174 2022-12-26 14:31:04.420758 datapipe_app-0.3.2.dev2/README.md
--rw-r--r--   0        0        0     1481 2023-02-17 19:42:56.902361 datapipe_app-0.3.2.dev2/datapipe_app/__init__.py
--rw-r--r--   0        0        0     8259 2023-02-17 19:42:56.902361 datapipe_app-0.3.2.dev2/datapipe_app/api_v1alpha1.py
--rw-r--r--   0        0        0    10501 2023-02-17 19:42:56.902361 datapipe_app-0.3.2.dev2/datapipe_app/cli.py
--rw-r--r--   0        0        0      533 2022-12-26 14:31:04.420758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/asset-manifest.json
--rw-r--r--   0        0        0     1150 2022-12-26 14:31:04.420758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/favicon.ico
--rw-r--r--   0        0        0      523 2022-12-26 14:31:04.430758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/index.html
--rw-r--r--   0        0        0      302 2022-12-26 14:31:04.430758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/manifest.json
--rw-r--r--   0        0        0       67 2022-12-26 14:31:04.430758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/robots.txt
--rw-r--r--   0        0        0   563144 2022-12-26 14:31:04.430758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/css/main.f1c7d66b.css
--rw-r--r--   0        0        0  1543694 2022-12-26 14:31:04.440758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/css/main.f1c7d66b.css.map
--rw-r--r--   0        0        0  1277098 2022-12-26 14:31:04.460758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/js/main.e9d707b4.js
--rw-r--r--   0        0        0     2462 2022-12-26 14:31:04.460758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/js/main.e9d707b4.js.LICENSE.txt
--rw-r--r--   0        0        0  5556874 2022-12-26 14:31:04.530758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/js/main.e9d707b4.js.map
--rw-r--r--   0        0        0     1309 2022-12-26 14:31:04.530758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/media/db-icon.9befcb0d4eeb44fd922f.svg
--rw-r--r--   0        0        0     2868 2022-12-26 14:31:04.530758 datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/media/fn-icon.947c4ec9c8f529970e90.svg
--rw-r--r--   0        0        0     4197 2023-02-06 17:55:29.928492 datapipe_app-0.3.2.dev2/datapipe_app/lints.py
--rw-r--r--   0        0        0     1091 2023-02-17 19:42:56.902361 datapipe_app-0.3.2.dev2/pyproject.toml
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 datapipe_app-0.3.2.dev2/setup.py
--rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 datapipe_app-0.3.2.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1174 2022-12-26 14:31:04.420758 datapipe_app-0.4.0a1/README.md
+-rw-r--r--   0        0        0     1885 2023-05-25 18:50:52.292956 datapipe_app-0.4.0a1/datapipe_app/__init__.py
+-rw-r--r--   0        0        0     9611 2023-08-01 07:38:43.686010 datapipe_app-0.4.0a1/datapipe_app/api_v1alpha1.py
+-rw-r--r--   0        0        0      569 2023-05-25 18:57:06.830333 datapipe_app-0.4.0a1/datapipe_app/cli.py
+-rw-r--r--   0        0        0      533 2022-12-26 14:31:04.420758 datapipe_app-0.4.0a1/datapipe_app/frontend/asset-manifest.json
+-rw-r--r--   0        0        0     1150 2022-12-26 14:31:04.420758 datapipe_app-0.4.0a1/datapipe_app/frontend/favicon.ico
+-rw-r--r--   0        0        0      523 2022-12-26 14:31:04.430758 datapipe_app-0.4.0a1/datapipe_app/frontend/index.html
+-rw-r--r--   0        0        0      302 2022-12-26 14:31:04.430758 datapipe_app-0.4.0a1/datapipe_app/frontend/manifest.json
+-rw-r--r--   0        0        0       67 2022-12-26 14:31:04.430758 datapipe_app-0.4.0a1/datapipe_app/frontend/robots.txt
+-rw-r--r--   0        0        0   563144 2022-12-26 14:31:04.430758 datapipe_app-0.4.0a1/datapipe_app/frontend/static/css/main.f1c7d66b.css
+-rw-r--r--   0        0        0  1543694 2022-12-26 14:31:04.440758 datapipe_app-0.4.0a1/datapipe_app/frontend/static/css/main.f1c7d66b.css.map
+-rw-r--r--   0        0        0  1277098 2022-12-26 14:31:04.460758 datapipe_app-0.4.0a1/datapipe_app/frontend/static/js/main.e9d707b4.js
+-rw-r--r--   0        0        0     2462 2022-12-26 14:31:04.460758 datapipe_app-0.4.0a1/datapipe_app/frontend/static/js/main.e9d707b4.js.LICENSE.txt
+-rw-r--r--   0        0        0  5556874 2022-12-26 14:31:04.530758 datapipe_app-0.4.0a1/datapipe_app/frontend/static/js/main.e9d707b4.js.map
+-rw-r--r--   0        0        0     1309 2022-12-26 14:31:04.530758 datapipe_app-0.4.0a1/datapipe_app/frontend/static/media/db-icon.9befcb0d4eeb44fd922f.svg
+-rw-r--r--   0        0        0     2868 2022-12-26 14:31:04.530758 datapipe_app-0.4.0a1/datapipe_app/frontend/static/media/fn-icon.947c4ec9c8f529970e90.svg
+-rw-r--r--   0        0        0     1249 2023-08-01 07:40:30.576016 datapipe_app-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 datapipe_app-0.4.0a1/PKG-INFO
```

### Comparing `datapipe_app-0.3.2.dev2/README.md` & `datapipe_app-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/__init__.py` & `datapipe_app-0.4.0a1/datapipe_app/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,56 @@
-import sys
-import os.path
 import logging
+import os.path
+import sys
+from typing import Optional
 
+from datapipe.compute import Catalog, DatapipeApp, Pipeline
+from datapipe.datatable import DataStore
 from fastapi import FastAPI
-from fastapi.staticfiles import StaticFiles
 from fastapi.middleware.cors import CORSMiddleware
-
-from datapipe.datatable import DataStore
-from datapipe.compute import build_compute, Catalog, Pipeline
+from fastapi.staticfiles import StaticFiles
 
 import datapipe_app.api_v1alpha1 as api_v1alpha1
 
 
-class DatapipeApp(FastAPI):
-    def __init__(self, ds: DataStore, catalog: Catalog, pipeline: Pipeline):
-        FastAPI.__init__(self)
-
-        self.ds = ds
-        self.catalog = catalog
-        self.pipeline = pipeline
+class DatapipeAPI(FastAPI, DatapipeApp):
+    def __init__(
+        self,
+        ds: Optional[DataStore] = None,
+        catalog: Optional[Catalog] = None,
+        pipeline: Optional[Pipeline] = None,
+        app: Optional[DatapipeApp] = None,
+    ):
+        if app is not None:
+            self.ds = app.ds
+            self.catalog = app.catalog
+            self.pipeline = app.pipeline
+            self.steps = app.steps
+        else:
+            assert ds is not None
+            assert catalog is not None
+            assert pipeline is not None
+            DatapipeApp.__init__(self, ds, catalog, pipeline)
 
-        self.steps = build_compute(ds, catalog, pipeline)
+        FastAPI.__init__(self)
 
         self.add_middleware(
             CORSMiddleware,
             allow_origins=["*"],
             allow_credentials=True,
             allow_methods=["*"],
             allow_headers=["*"],
         )
 
         self.api = FastAPI()
 
         self.api.mount(
             "/v1alpha1",
-            api_v1alpha1.DatpipeAPIv1(ds, catalog, pipeline, self.steps),
-            name="v1alpha1"
+            api_v1alpha1.DatpipeAPIv1(self.ds, self.catalog, self.pipeline, self.steps),
+            name="v1alpha1",
         )
 
         self.mount("/api", self.api, name="api")
         self.mount(
             "/",
             StaticFiles(
                 directory=os.path.join(os.path.dirname(__file__), "frontend/"),
```

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/api_v1alpha1.py` & `datapipe_app-0.4.0a1/datapipe_app/api_v1alpha1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Literal, Optional
 
 import pandas as pd
 from datapipe.compute import (
     Catalog,
     ComputeStep,
     DataStore,
     Pipeline,
     run_steps,
     run_steps_changelist,
 )
 from datapipe.store.database import TableStoreDB
 from datapipe.types import ChangeList
-from fastapi import FastAPI, Response, Query
+from fastapi import BackgroundTasks, FastAPI, Query, Response
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 from pydantic import BaseModel, Field
-from sqlalchemy.sql.expression import select
+from sqlalchemy.sql.expression import select, text
 from sqlalchemy.sql.functions import count
 
 
 class PipelineStepResponse(BaseModel):
     id_: str = Field(alias="id")
     type_: str = Field(alias="type")
     name: str
@@ -39,17 +39,145 @@
     catalog: Dict[str, TableResponse]
     pipeline: List[PipelineStepResponse]
 
 
 class UpdateDataRequest(BaseModel):
     table_name: str
     upsert: Optional[List[Dict]] = None
+    enable_changelist: bool = True
     # delete: List[Dict] = None
 
 
+class UpdateDataResponse(BaseModel):
+    result: str
+
+
+class GetDataRequest(BaseModel):
+    table: str
+    filters: Dict[str, Any] = {}
+    page: int = 0
+    page_size: int = 20
+    order_by: Optional[str] = None
+    order: Literal["asc", "desc"] = "asc"
+
+
+class GetDataResponse(BaseModel):
+    page: int
+    page_size: int
+    total: int
+    data: List[Dict]
+
+
+def update_data(
+    ds: DataStore,
+    catalog: Catalog,
+    steps: List[ComputeStep],
+    req: UpdateDataRequest,
+) -> UpdateDataResponse:
+    dt = catalog.get_datatable(ds, req.table_name)
+
+    cl = ChangeList()
+
+    if req.upsert is not None and len(req.upsert) > 0:
+        idx = dt.store_chunk(pd.DataFrame.from_records(req.upsert))
+
+        cl.append(dt.name, idx)
+
+    # if req.delete is not None and len(req.delete) > 0:
+    #     idx = dt.delete_by_idx(
+    #         pd.DataFrame.from_records(req.delete)
+    #     )
+
+    #     cl.append(dt.name, idx)
+    if req.enable_changelist:
+        run_steps_changelist(ds, steps, cl)
+
+    return UpdateDataResponse(result="ok")
+
+
+def get_data_get(
+    ds: DataStore,
+    catalog: Catalog,
+    table: str,
+    page: int = 0,
+    page_size: int = 20,
+) -> GetDataResponse:
+    dt = catalog.get_datatable(ds, table)
+
+    meta_schema = dt.meta_table.sql_schema
+    meta_tbl = dt.meta_table.sql_table
+
+    sql = select(*meta_schema)
+    sql = sql.where(meta_tbl.c.delete_ts.is_(None))
+    sql = sql.offset(page * page_size).limit(page_size)
+
+    meta_df = pd.read_sql_query(
+        sql,
+        con=ds.meta_dbconn.con,
+    )
+
+    if not meta_df.empty:
+        data_df = dt.get_data(meta_df)
+    else:
+        data_df = pd.DataFrame()
+
+    return GetDataResponse(
+        page=page,
+        page_size=page_size,
+        total=len(meta_df),
+        data=data_df.fillna("").to_dict(orient="records"),
+    )
+
+
+def get_data_post(
+    ds: DataStore, catalog: Catalog, req: GetDataRequest
+) -> GetDataResponse:
+    dt = catalog.get_datatable(ds, req.table)
+
+    assert isinstance(dt.table_store, TableStoreDB)
+
+    sql_schema = dt.table_store.data_sql_schema
+    sql_table = dt.table_store.data_table
+
+    sql = select(*sql_schema).select_from(sql_table)
+    # Data table has no delete_ts
+    # sql = sql.where(sql_table.c.delete_ts.is_(None))
+    if req.order_by:
+        sql = sql.where(text(f"{req.order_by} is not null"))
+        sql = sql.order_by(text(f"{req.order_by} {req.order}"))
+    sql = sql.offset(req.page * req.page_size).limit(req.page_size)
+
+    for col, val in req.filters.items():
+        sql = sql.where(sql_table.c[col] == val)
+
+    sql_count = select(count()).select_from(sql_table)
+    for col, val in req.filters.items():
+        sql_count = sql_count.where(sql_table.c[col] == val)
+
+    meta_df = pd.read_sql_query(
+        sql,
+        con=ds.meta_dbconn.con,
+    )
+
+    if not meta_df.empty:
+        data_df = dt.get_data(meta_df)
+        if req.order_by is not None:
+            ascending = req.order == "asc"
+            data_df.sort_values(by=req.order_by, ascending=ascending, inplace=True)
+    else:
+        data_df = pd.DataFrame()
+
+    return GetDataResponse(
+        page=req.page,
+        page_size=req.page_size,
+        total=dt.table_store.dbconn.con.execute(sql_count).fetchone()[0],
+        data=data_df.fillna("").to_dict(orient="records"),
+    )
+
+
 def DatpipeAPIv1(
     ds: DataStore, catalog: Catalog, pipeline: Pipeline, steps: List[ComputeStep]
 ) -> FastAPI:
     app = FastAPI()
 
     @app.get("/graph", response_model=GraphResponse)
     def get_graph() -> GraphResponse:
@@ -60,16 +188,16 @@
                 name=tbl.name,
                 indexes=tbl.primary_keys,
                 size=tbl.get_size(),
                 store_class=tbl.table_store.__class__.__name__,
             )
 
         def pipeline_step_response(step):
-            inputs = [i.name for i in step.get_input_dts()]
-            outputs = [i.name for i in step.get_output_dts()]
+            inputs = [i.name for i in step.input_dts]
+            outputs = [i.name for i in step.output_dts]
             inputs_join = ",".join(inputs)
             outputs_join = ",".join(outputs)
             id_ = f"{step.name}({inputs_join})->({outputs_join})"
 
             return PipelineStepResponse(
                 id=id_,
                 type="transform",
@@ -82,114 +210,30 @@
             catalog={
                 table_name: table_response(table_name)
                 for table_name in catalog.catalog.keys()
             },
             pipeline=[pipeline_step_response(step) for step in steps],
         )
 
-    @app.post("/update-data")
-    def update_data(req: UpdateDataRequest):
-        dt = catalog.get_datatable(ds, req.table_name)
-
-        cl = ChangeList()
-
-        if req.upsert is not None and len(req.upsert) > 0:
-            idx = dt.store_chunk(pd.DataFrame.from_records(req.upsert))
-
-            cl.append(dt.name, idx)
-
-        # if req.delete is not None and len(req.delete) > 0:
-        #     idx = dt.delete_by_idx(
-        #         pd.DataFrame.from_records(req.delete)
-        #     )
-
-        #     cl.append(dt.name, idx)
-
-        run_steps_changelist(ds, steps, cl)
-
-        return {"result": "ok"}
-
-    class GetDataRequest(BaseModel):
-        table: str
-        filters: Dict[str, Any] = {}
-        page: int = 0
-        page_size: int = 20
-
-    class GetDataResponse(BaseModel):
-        page: int
-        page_size: int
-        total: int
-        data: List[Dict]
+    @app.post("/update-data", response_model=UpdateDataResponse)
+    def update_data_api(req: UpdateDataRequest) -> UpdateDataResponse:
+        return update_data(ds, catalog, steps, req)
 
     # /table/<table_name>?page=1&id=111&another_filter=value&sort=<+|->column_name
     @app.get("/get-data", response_model=GetDataResponse)
-    def get_data_get(table: str, page: int = 0, page_size: int = 20) -> GetDataResponse:
-        dt = catalog.get_datatable(ds, table)
-
-        meta_schema = dt.meta_table.sql_schema
-        meta_tbl = dt.meta_table.sql_table
-
-        sql = select(*meta_schema)
-        sql = sql.where(meta_tbl.c.delete_ts.is_(None))
-        sql = sql.offset(page * page_size).limit(page_size)
-
-        meta_df = pd.read_sql_query(
-            sql,
-            con=ds.meta_dbconn.con,
-        )
-
-        if not meta_df.empty:
-            data_df = dt.get_data(meta_df)
-        else:
-            data_df = pd.DataFrame()
-
-        return GetDataResponse(
-            page=page,
-            page_size=page_size,
-            total=len(meta_df),
-            data=data_df.fillna("").to_dict(orient="records"),
-        )
+    def get_data_get_api(
+        table: str,
+        page: int = 0,
+        page_size: int = 20,
+    ) -> GetDataResponse:
+        return get_data_get(ds, catalog, table, page, page_size)
 
     @app.post("/get-data", response_model=GetDataResponse)
-    def get_data_post(req: GetDataRequest) -> GetDataResponse:
-        dt = catalog.get_datatable(ds, req.table)
-
-        assert isinstance(dt.table_store, TableStoreDB)
-
-        sql_schema = dt.table_store.data_sql_schema
-        sql_table = dt.table_store.data_table
-
-        sql = select(*sql_schema).select_from(sql_table)
-        # Data table has no delete_ts
-        # sql = sql.where(sql_table.c.delete_ts.is_(None))
-        sql = sql.offset(req.page * req.page_size).limit(req.page_size)
-
-        for col, val in req.filters.items():
-            sql = sql.where(sql_table.c[col] == val)
-
-        sql_count = select(count()).select_from(sql_table)
-        for col, val in req.filters.items():
-            sql_count = sql_count.where(sql_table.c[col] == val)
-
-        meta_df = pd.read_sql_query(
-            sql,
-            con=ds.meta_dbconn.con,
-        )
-
-        if not meta_df.empty:
-            data_df = dt.get_data(meta_df)
-        else:
-            data_df = pd.DataFrame()
-
-        return GetDataResponse(
-            page=req.page,
-            page_size=req.page_size,
-            total=dt.table_store.dbconn.con.execute(sql_count).fetchone()[0],
-            data=data_df.fillna("").to_dict(orient="records"),
-        )
+    def get_data_post_api(req: GetDataRequest) -> GetDataResponse:
+        return get_data_post(ds, catalog, req)
 
     class FocusFilter(BaseModel):
         table_name: str
         items_idx: List[Dict]
 
     class GetDataWithFocusRequest(BaseModel):
         table_name: str
@@ -217,15 +261,15 @@
 
         return GetDataResponse(
             page=req.page,
             page_size=req.page_size,
             total=len(existing_idx),
             data=dt.get_data(
                 existing_idx.iloc[
-                    req.page * req.page_size : (req.page + 1) * req.page_size
+                    req.page * req.page_size : (req.page + 1) * req.page_size  # noqa: E203
                 ]
             ).to_dict(orient="records"),
         )
 
     class GetDataByIdxRequest(BaseModel):
         table_name: str
         idx: List[Dict]
@@ -243,38 +287,52 @@
         run_steps(ds=ds, steps=steps)
 
     # TODO refactor out to component based extension system
     # TODO automatic setup of webhook on project creation
     @app.post("/labelstudio-webhook")
     def labelstudio_webhook(
         request: Dict,
+        background_tasks: BackgroundTasks,
         table_name: str = Query(..., title="Input table name"),
         data_field: List = Query(..., title="Fields to get from data"),
+        background: bool = Query(False, title="Run as Background Task (default = False)")
     ) -> None:
-        update_data(
-            req=UpdateDataRequest(
-                table_name=table_name,
-                upsert=[
-                    {
-                        **{
-                            k: v for k, v in request["task"]["data"].items()
-                            if k in data_field
-                        },
-                        "annotations": [request["annotation"]],
-                    }
-                ],
-            )
-        )
+
+        upsert = [
+            {
+                **{
+                    k: v
+                    for k, v in request["task"]["data"].items()
+                    if k in data_field
+                },
+                "annotations": [request["annotation"]],
+            }
+        ]
+
+        dt = catalog.get_datatable(ds, table_name)
+
+        cl = ChangeList()
+
+        if len(upsert) > 0:
+            idx = dt.store_chunk(pd.DataFrame.from_records(upsert))
+
+            cl.append(dt.name, idx)
+
+        if background:
+            background_tasks.add_task(run_steps_changelist, ds=ds, steps=steps, changelist=cl)
+        else:
+            run_steps_changelist(ds=ds, steps=steps, changelist=cl)
 
     @app.get("/get-file")
     def get_file(filepath: str):
         import mimetypes
 
         import fsspec
 
         with fsspec.open(filepath) as f:
             mime = mimetypes.guess_type(filepath)
+            assert mime[0] is not None
             return Response(content=f.read(), media_type=mime[0])
 
     FastAPIInstrumentor.instrument_app(app, excluded_urls="docs")
 
     return app
```

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/asset-manifest.json` & `datapipe_app-0.4.0a1/datapipe_app/frontend/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/favicon.ico` & `datapipe_app-0.4.0a1/datapipe_app/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/index.html` & `datapipe_app-0.4.0a1/datapipe_app/frontend/index.html`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/css/main.f1c7d66b.css` & `datapipe_app-0.4.0a1/datapipe_app/frontend/static/css/main.f1c7d66b.css`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/css/main.f1c7d66b.css.map` & `datapipe_app-0.4.0a1/datapipe_app/frontend/static/css/main.f1c7d66b.css.map`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/js/main.e9d707b4.js` & `datapipe_app-0.4.0a1/datapipe_app/frontend/static/js/main.e9d707b4.js`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/js/main.e9d707b4.js.LICENSE.txt` & `datapipe_app-0.4.0a1/datapipe_app/frontend/static/js/main.e9d707b4.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/js/main.e9d707b4.js.map` & `datapipe_app-0.4.0a1/datapipe_app/frontend/static/js/main.e9d707b4.js.map`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/media/db-icon.9befcb0d4eeb44fd922f.svg` & `datapipe_app-0.4.0a1/datapipe_app/frontend/static/media/db-icon.9befcb0d4eeb44fd922f.svg`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/datapipe_app/frontend/static/media/fn-icon.947c4ec9c8f529970e90.svg` & `datapipe_app-0.4.0a1/datapipe_app/frontend/static/media/fn-icon.947c4ec9c8f529970e90.svg`

 * *Files identical despite different names*

### Comparing `datapipe_app-0.3.2.dev2/pyproject.toml` & `datapipe_app-0.4.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 [tool.poetry]
 name = "datapipe-app"
-version = "0.3.2-dev.2"
+version = "0.4.0-alpha.1"
 description = ""
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 
 readme = "README.md"
 
 packages = [
     { include = "datapipe_app" },
 ]
 
 include = [
     "datapipe_app/frontend/**/*"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8.1,<3.11"
 fastapi = ">=0.69.0"
 uvicorn = {extras = ["standard"], version = ">= 0.17.0"}
 click = ">=7.1.2"
-termcolor = "^2.1.0"
+rich = "^13.3.2"
 
-datapipe-core = {version=">=0.11.12-dev.1, <0.12", allow-prereleases = true}
+datapipe-core = {version=">=0.12.0-alpha.1", allow-prereleases = true}
+# datapipe-core = {version=">=0.12.0, <0.13", allow-prereleases = true}
 # datapipe-core = {path="../datapipe"}
 
+prometheus-client = ">= 0.8.0, < 1.0.0"
+
 opentelemetry-instrumentation-fastapi = "0.35b0"
 
 opentelemetry-exporter-gcp-trace = {version="^1.3.0", optional=true}
 opentelemetry-exporter-jaeger = {version="^1.8.0", optional=true}
 
 [tool.poetry.extras]
 gcp = ["opentelemetry-exporter-gcp-trace"]
 jaeger = ["opentelemetry-exporter-jaeger"]
 
-[tool.poetry.scripts]
-datapipe = 'datapipe_app.cli:main'
+[tool.poetry.plugins."datapipe.cli"]
+datapipe_app = "datapipe_app.cli:register_commands"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 mypy = "*"
 sqlalchemy = {extras = ["mypy"], version = "*"}
 alembic = "*"
 black = "*"
+flake8 = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datapipe_app-0.3.2.dev2/PKG-INFO` & `datapipe_app-0.4.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: datapipe-app
-Version: 0.3.2.dev2
+Version: 0.4.0a1
 Summary: 
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8.1,<3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: gcp
 Provides-Extra: jaeger
 Requires-Dist: click (>=7.1.2)
-Requires-Dist: datapipe-core (>=0.11.12-dev.1,<0.12)
+Requires-Dist: datapipe-core (>=0.12.0-alpha.1)
 Requires-Dist: fastapi (>=0.69.0)
 Requires-Dist: opentelemetry-exporter-gcp-trace (>=1.3.0,<2.0.0) ; extra == "gcp"
 Requires-Dist: opentelemetry-exporter-jaeger (>=1.8.0,<2.0.0) ; extra == "jaeger"
 Requires-Dist: opentelemetry-instrumentation-fastapi (==0.35b0)
-Requires-Dist: termcolor (>=2.1.0,<3.0.0)
+Requires-Dist: prometheus-client (>=0.8.0,<1.0.0)
+Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: uvicorn[standard] (>=0.17.0)
 Description-Content-Type: text/markdown
 
 # datapipe-app
 
 `datapipe-app` implements two aspects to make every [datapipe](https://github.com/epoch8/datapipe) pipeline to work as
 an application:
```

