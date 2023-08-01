# Comparing `tmp/openlineage-integration-common-0.9.0.tar.gz` & `tmp/openlineage-integration-common-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-integration-common-0.9.0.tar", last modified: Fri Jun  3 23:03:13 2022, max compression
+gzip compressed data, was "openlineage-integration-common-1.0.0.tar", last modified: Tue Aug  1 19:46:03 2023, max compression
```

## Comparing `openlineage-integration-common-0.9.0.tar` & `openlineage-integration-common-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      594 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6491 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/dataset.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1325 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/models.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9724 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/bigquery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25202 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/dbt.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16564 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/action.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1774 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/facets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7666 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/results.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/schema/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      166 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/schema/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage/common/sql/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/sql/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9904 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/sql/parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3851 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1898 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/openlineage/common/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      594 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      907 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      978 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      553 2022-06-03 23:03:13.000000 openlineage-integration-common-0.9.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1686 2022-06-03 23:03:12.000000 openlineage-integration-common-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.796534 openlineage-integration-common-1.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      462 2023-08-01 19:46:03.796534 openlineage-integration-common-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.788534 openlineage-integration-common-1.0.0/openlineage/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.792534 openlineage-integration-common-1.0.0/openlineage/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6857 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1735 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.792534 openlineage-integration-common-1.0.0/openlineage/common/provider/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10235 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/bigquery.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.792534 openlineage-integration-common-1.0.0/openlineage/common/provider/dbt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/dbt/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2579 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/dbt/cloud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6955 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/dbt/local.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22039 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/dbt/processor.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.792534 openlineage-integration-common-1.0.0/openlineage/common/provider/great_expectations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/great_expectations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20759 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/great_expectations/action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1991 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/great_expectations/facets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7769 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/great_expectations/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/redshift_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1816 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/provider/snowflake.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.792534 openlineage-integration-common-1.0.0/openlineage/common/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/schema/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.792534 openlineage-integration-common-1.0.0/openlineage/common/sql/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/sql/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4762 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1965 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage/common/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.796534 openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      462 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1198 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1205 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2023-08-01 19:46:03.796534 openlineage-integration-common-1.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1865 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:03.796534 openlineage-integration-common-1.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2792 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/tests/test_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/tests/test_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1378 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/tests/test_snowflake.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1627 2023-08-01 19:46:03.000000 openlineage-integration-common-1.0.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openlineage-integration-common-0.9.0/openlineage/common/dataset.py` & `openlineage-integration-common-1.0.0/openlineage/common/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,28 @@
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 
-from typing import List, Optional, Dict
+from typing import Dict, List, Optional
 
-from openlineage.common.models import DbTableSchema, DbColumn
-from openlineage.client.facet import BaseFacet, DataSourceDatasetFacet, \
-    DocumentationDatasetFacet, SchemaDatasetFacet, SchemaField
-from openlineage.client.run import Dataset as OpenLineageDataset, InputDataset, OutputDataset
+from openlineage.client.facet import (
+    BaseFacet,
+    DataSourceDatasetFacet,
+    DocumentationDatasetFacet,
+    SchemaDatasetFacet,
+    SchemaField,
+)
+from openlineage.client.run import Dataset as OpenLineageDataset
+from openlineage.client.run import InputDataset, OutputDataset
+from openlineage.client.utils import RedactMixin
+from openlineage.common.models import DbColumn, DbTableSchema
 
 
-class Source:
+class Source(RedactMixin):
+    _skip_redact: List[str] = ['scheme', 'name']
+
     def __init__(
             self,
             scheme: Optional[str] = None,
             authority: Optional[str] = None,
             connection_url: Optional[str] = None,
             name: Optional[str] = None
     ):
@@ -37,17 +47,19 @@
         if self._name:
             return self._name
         if self.authority:
             return f'{self.scheme}://{self.authority}'
         return f'{self.scheme}'
 
 
-class Field:
+class Field(RedactMixin):
+    _skip_redact: List[str] = ['name', 'type', 'tags']
+
     def __init__(self, name: str, type: str,
-                 tags: List[str] = None, description: str = None):
+                 tags: Optional[List[str]] = None, description: Optional[str] = None):
         self.name = name
         self.type = type
         self.tags = tags
         self.description = description
 
         if self.tags is None:
             self.tags = []
@@ -67,23 +79,25 @@
                self.description == other.description
 
     def __repr__(self):
         return f"Field({self.name!r},{self.type!r}, \
                        {self.tags!r},{self.description!r})"
 
 
-class Dataset:
+class Dataset(RedactMixin):
+    _skip_redact: List[str] = ['name']
+
     def __init__(
             self,
             source: Source,
-            name: str, fields: List[Field] = None,
+            name: str, fields: Optional[List[Field]] = None,
             description: Optional[str] = None,
-            custom_facets: Dict[str, BaseFacet] = None,
-            input_facets: Dict[str, BaseFacet] = None,
-            output_facets: Dict[str, BaseFacet] = None
+            custom_facets: Optional[Dict[str, BaseFacet]] = None,
+            input_facets: Optional[Dict[str, BaseFacet]] = None,
+            output_facets: Optional[Dict[str, BaseFacet]] = None
     ):
         if fields is None:
             fields = []
         if custom_facets is None:
             custom_facets = {}
         if input_facets is None:
             input_facets = {}
@@ -96,30 +110,30 @@
         self.custom_facets = custom_facets
         self.input_facets = input_facets
         self.output_facets = output_facets
 
     @staticmethod
     def from_table(source: Source,
                    table_name: str,
-                   schema_name: str = None,
-                   database_name: str = None):
+                   schema_name: Optional[str] = None,
+                   database_name: Optional[str] = None):
         return Dataset(
             name=Dataset._to_name(
                 schema_name=schema_name,
                 table_name=table_name,
                 database_name=database_name
             ),
             source=source
         )
 
     @staticmethod
     def from_table_schema(
             source: Source,
             table_schema: DbTableSchema,
-            database_name: str = None
+            database_name: Optional[str] = None
     ):
         return Dataset(
             name=Dataset._to_name(
                 schema_name=table_schema.schema_name,
                 table_name=table_schema.table_name.name,
                 database_name=database_name
             ),
@@ -129,15 +143,15 @@
                 Field.from_column(column) for column in sorted(
                     table_schema.columns, key=lambda x: x.ordinal_position
                 )
             ]
         )
 
     @staticmethod
-    def _to_name(table_name: str, schema_name: str = None, database_name: str = None):
+    def _to_name(table_name: str, schema_name: Optional[str] = None, database_name: Optional[str] = None):  # noqa
         # Prefix the table name with database and schema name using
         # the format: {database_name}.{table_schema}.{table_name}.
         name = [table_name]
         if schema_name is not None:
             name = [schema_name] + name
         if database_name is not None:
             name = [database_name] + name
@@ -151,36 +165,30 @@
                self.description == other.description
 
     def __repr__(self):
         return f"Dataset({self.source!r},{self.name!r}, \
                          {self.fields!r},{self.description!r})"
 
     def to_openlineage_dataset(self) -> OpenLineageDataset:
-        facets = {
-            "dataSource": DataSourceDatasetFacet(
-                self.source.name,
-                self.source.connection_url
-            )
-        }
+        facets: Dict[str, BaseFacet] = {"dataSource": DataSourceDatasetFacet(
+            name=self.source.name,
+            uri=self.source.connection_url or "",
+        )}
         if self.description:
-            facets.update({
-                "documentation": DocumentationDatasetFacet(
-                    description=self.description
-                )
-            })
+            facets["documentation"] = DocumentationDatasetFacet(
+                description=self.description
+            )
 
         if self.fields is not None and len(self.fields):
-            facets.update({
-                "schema": SchemaDatasetFacet(
-                    fields=[
-                        SchemaField(field.name, field.type, field.description)
-                        for field in self.fields
-                    ]
-                )
-            })
+            facets["schema"] = SchemaDatasetFacet(
+                fields=[
+                    SchemaField(field.name, field.type, field.description)
+                    for field in self.fields
+                ]
+            )
 
         if self.custom_facets:
             facets.update(self.custom_facets)
 
         if len(self.input_facets):
             return InputDataset(
                 namespace=self.source.name,
```

### Comparing `openlineage-integration-common-0.9.0/openlineage/common/provider/bigquery.py` & `openlineage-integration-common-1.0.0/openlineage/common/provider/bigquery.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,38 @@
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 
 import json
 import logging
 import traceback
-import attr
-
-from typing import Tuple, Optional, Dict, List
-
-from google.cloud.bigquery import Client
+from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
 
+import attr
+from openlineage.client.facet import (
+    BaseFacet,
+    ExternalQueryRunFacet,
+    OutputStatisticsOutputDatasetFacet,
+)
 from openlineage.common.dataset import Dataset, Source
-from openlineage.common.models import DbTableSchema, DbColumn
+from openlineage.common.models import DbColumn, DbTableSchema
 from openlineage.common.schema import GITHUB_LOCATION
 from openlineage.common.sql import DbTableMeta
 from openlineage.common.utils import get_from_nullable_chain
-from openlineage.client.facet import BaseFacet, OutputStatisticsOutputDatasetFacet, \
-    ExternalQueryRunFacet
 
 _BIGQUERY_CONN_URL = 'bigquery'
 
+# we lazy-load bigquery Client in BigQueryDatasetsProvider if not type-checking
+if TYPE_CHECKING:
+    from google.cloud.bigquery import Client
+
+
+def get_bq_client():
+    from google.cloud.bigquery import Client
+    return Client
+
 
 @attr.s
 class BigQueryErrorRunFacet(BaseFacet):
     """
     Represents errors that can happen during execution of BigqueryExtractor
     :param clientError: represents errors originating in bigquery client
     :param parserError: represents errors that happened during parsing SQL provided to bigquery
@@ -41,16 +51,16 @@
     Facet that represents relevant statistics of bigquery run.
     :param cached: bigquery caches query results. Rest of the statistics will not be provided
         for cached queries.
     :param billedBytes: how many bytes bigquery bills for.
     :param properties: full property tree of bigquery run.
     """
     cached: bool = attr.ib()
-    billedBytes: int = attr.ib(default=None)
-    properties: str = attr.ib(default=None)
+    billedBytes: Optional[int] = attr.ib(default=None)
+    properties: Optional[str] = attr.ib(default=None)
 
     @staticmethod
     def _get_schema() -> str:
         return GITHUB_LOCATION + "bq-statistics-run-facet.json"
 
 
 @attr.s
@@ -80,31 +90,34 @@
     inputs: List[Dataset] = attr.ib()
     output: Optional[Dataset] = attr.ib(default=None)
 
 
 class BigQueryDatasetsProvider:
     def __init__(
         self,
-        client: Optional[Client] = None,
+        client: Optional["Client"] = None,
         logger: Optional[logging.Logger] = None
     ):
-        self.client = client
         if client is None:
-            self.client = Client()
-        self.logger = logger
+            # lazy-load bigquery client since its slow to import (primarily due to pandas)
+            self.client = get_bq_client()
+        else:
+            self.client = client
         if logger is None:
-            self.logger = logging.getLogger(__name__)
+            self.logger: logging.Logger = logging.getLogger(__name__)
+        else:
+            self.logger = logger
 
     def get_facets(self, job_id: str) -> BigQueryFacets:
         inputs = []
         output = None
         run_facets = {}
         try:
             try:
-                job = self.client.get_job(job_id=job_id)
+                job = self.client.get_job(job_id=job_id)        # type: ignore
                 props = job._properties
 
                 run_stat_facet, dataset_stat_facet = self._get_output_statistics(props)
 
                 run_facets.update({
                     "bigQuery_job": run_stat_facet,
                     "externalQuery": ExternalQueryRunFacet(
@@ -225,44 +238,44 @@
     def _get_table_safely(self, output_table_name):
         try:
             return self._get_table(output_table_name)
         except Exception as e:
             self.logger.warning(f'Could not extract output schema from bigquery. {e}')
         return None
 
-    def _get_table_schemas(self, tables: [str]) \
-            -> [DbTableSchema]:
+    def _get_table_schemas(self, tables: List[str]) \
+            -> List[DbTableSchema]:
         # Avoid querying BigQuery by returning an empty array
         # if no tables have been provided.
         if not tables:
             return []
 
         return [self._get_table(table) for table in tables]
 
     def _get_table(self, table: str) -> Optional[DbTableSchema]:
         bq_table = self.client.get_table(table)
         if not bq_table._properties:
-            return
-        table = bq_table._properties
+            return None
+        table_prop = bq_table._properties
 
-        fields = get_from_nullable_chain(table, ['schema', 'fields'])
+        fields = get_from_nullable_chain(table_prop, ['schema', 'fields'])
         if not fields:
-            return
+            return None
 
         columns = [DbColumn(
             name=fields[i].get('name'),
             type=fields[i].get('type'),
             description=fields[i].get('description'),
             ordinal_position=i
         ) for i in range(len(fields))]
 
         return DbTableSchema(
-            schema_name=table.get('tableReference').get('projectId') + '.' +
-            table.get('tableReference').get('datasetId'),
-            table_name=DbTableMeta(table.get('tableReference').get('tableId')),
+            schema_name=table_prop.get('tableReference').get('projectId') + '.' +
+            table_prop.get('tableReference').get('datasetId'),
+            table_name=DbTableMeta(table_prop.get('tableReference').get('tableId')),
             columns=columns
         )
 
     def _source(self) -> Source:
         return Source(
             scheme='bigquery',
             connection_url='bigquery'
```

### Comparing `openlineage-integration-common-0.9.0/openlineage/common/provider/dbt.py` & `openlineage-integration-common-1.0.0/openlineage/common/provider/dbt/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,63 @@
+# Copyright 2018-2023 contributors to the OpenLineage project
 # SPDX-License-Identifier: Apache-2.0
 
 import collections
 import datetime
-import json
 import logging
-import os
 import uuid
+from abc import abstractmethod
 from enum import Enum
-from typing import Dict, List, Optional, Tuple, TypeVar
+from typing import Dict, List, Optional, Tuple
 
 import attr
-import yaml
-from jinja2 import Environment, Undefined
-from openlineage.client.facet import (Assertion, BaseFacet,
-                                      DataQualityAssertionsDatasetFacet,
-                                      DataSourceDatasetFacet,
-                                      OutputStatisticsOutputDatasetFacet,
-                                      ParentRunFacet, SchemaDatasetFacet,
-                                      SchemaField, SqlJobFacet)
-from openlineage.client.run import (Dataset, Job, OutputDataset, Run, RunEvent,
-                                    RunState)
-
+from openlineage.client.facet import (
+    Assertion,
+    BaseFacet,
+    DataQualityAssertionsDatasetFacet,
+    DataSourceDatasetFacet,
+    OutputStatisticsOutputDatasetFacet,
+    ParentRunFacet,
+    SchemaDatasetFacet,
+    SchemaField,
+    SqlJobFacet,
+)
+from openlineage.client.run import Dataset, Job, OutputDataset, Run, RunEvent, RunState
+from openlineage.common.provider.snowflake import fix_account_name
 from openlineage.common.schema import GITHUB_LOCATION
-from openlineage.common.utils import (get_from_multiple_chains,
-                                      get_from_nullable_chain)
+from openlineage.common.utils import get_from_multiple_chains, get_from_nullable_chain
 
 
 class Adapter(Enum):
     # This class represents supported adapters.
-    BIGQUERY = 'bigquery'
-    SNOWFLAKE = 'snowflake'
-    REDSHIFT = 'redshift'
-    SPARK = 'spark'
+    BIGQUERY = "bigquery"
+    SNOWFLAKE = "snowflake"
+    REDSHIFT = "redshift"
+    SPARK = "spark"
+    POSTGRES = "postgres"
+    DATABRICKS = "databricks"
 
     @staticmethod
     def adapters() -> str:
         # String representation of all supported adapter names
-        return ','.join([f"`{x.value}`" for x in list(Adapter)])
+        return ",".join([f"`{x.value}`" for x in list(Adapter)])
 
 
 class SparkConnectionMethod(Enum):
-    THRIFT = 'thrift'
-    ODBC = 'odbc'
-    HTTP = 'http'
+    THRIFT = "thrift"
+    ODBC = "odbc"
+    HTTP = "http"
 
     @staticmethod
     def methods():
         return [x.value for x in SparkConnectionMethod]
 
 
-class SkipUndefined(Undefined):
-    def __getattr__(self, name):
-        return SkipUndefined(name=f"{self._undefined_name}.{name}")
-
-    def __str__(self):
-        return f"{{{{ {self._undefined_name} }}}}"
-
-    def _fail_with_undefined_error(self, *args, **kwargs):
-        pass
-
-    def __call__(self, *args, **kwargs):
-        arguments = ', '.join([
-            arg._undefined_name if isinstance(arg, SkipUndefined) else str(arg) for arg in args
-        ])
-        return f"{{{{ {self._undefined_name}({arguments}) }}}}"
+class UnsupportedDbtCommand(Exception):
+    pass
 
 
 @attr.s
 class ModelNode:
     metadata_node: Dict = attr.ib()
     catalog_node: Optional[Dict] = attr.ib(default=None)
 
@@ -129,354 +119,268 @@
 class ParentRunMetadata:
     run_id: str = attr.ib()
     job_name: str = attr.ib()
     job_namespace: str = attr.ib()
 
     def to_openlineage(self) -> ParentRunFacet:
         return ParentRunFacet.create(
-            runId=self.run_id,
-            name=self.job_name,
-            namespace=self.job_namespace
+            runId=self.run_id, name=self.job_name, namespace=self.job_namespace
         )
 
 
 @attr.s
 class DbtVersionRunFacet(BaseFacet):
     version: str = attr.ib()
 
     @staticmethod
     def _get_schema() -> str:
         return GITHUB_LOCATION + "dbt-version-run-facet.json"
 
 
-T = TypeVar('T')
-
-logging.getLogger('null').addHandler(logging.NullHandler())
-
 
 class DbtArtifactProcessor:
+    should_raise_on_unsupported_command = True
+
     def __init__(
         self,
         producer: str,
-        project_dir: str,
         job_namespace: str,
-        profile_name: Optional[str] = None,
-        target: Optional[str] = None,
         skip_errors: bool = False,
-        logger: logging.Logger = logging.getLogger("null")
+        logger: Optional[logging.Logger] = None,
     ):
         self.producer = producer
-        self.dir = os.path.abspath(project_dir)
-        self._dbt_run_metadata = None
-        self.profile_name = profile_name
-        self.target = target
-        self.jinja_environment = None
-        self.logger = logger
+        self._dbt_run_metadata: Optional[ParentRunMetadata] = None
+        self.logger = logger or logging.getLogger(
+            f"{self.__class__.__module__}.{self.__class__.__name__}"
+        )
 
         self.job_namespace = job_namespace
         self.dataset_namespace = ""
         self.skip_errors = skip_errors
-        self.project = self.load_yaml_with_jinja(os.path.join(project_dir, 'dbt_project.yml'))
         self.run_metadata = None
         self.command = None
 
-        self.manifest_path = os.path.join(self.dir, self.project['target-path'], 'manifest.json')
-        self.run_result_path = os.path.join(
-            self.dir, self.project['target-path'], 'run_results.json'
-        )
-        self.catalog_path = os.path.join(self.dir, self.project['target-path'], 'catalog.json')
-
     @property
     def dbt_run_metadata(self):
         return self._dbt_run_metadata
 
     @dbt_run_metadata.setter
     def dbt_run_metadata(self, metadata: ParentRunMetadata):
         self._dbt_run_metadata = metadata
 
+    @abstractmethod
+    def get_dbt_metadata(self):
+        ...
+
     def parse(self) -> DbtEvents:
         """
-            Parse dbt manifest and run_result and produce OpenLineage events.
+        Parse dbt manifest and run_result and produce OpenLineage events.
         """
-        manifest = self.load_metadata(self.manifest_path, [2, 3, 4], self.logger)
-        run_result = self.load_metadata(self.run_result_path, [2, 3, 4], self.logger)
-        self.run_metadata = run_result['metadata']
-        self.command = run_result['args']['which']
-
-        try:
-            catalog = self.load_metadata(self.catalog_path, [1], self.logger)
-        except FileNotFoundError:
-            catalog = None
+        manifest, run_result, profile, catalog = self.get_dbt_metadata()
+        self.manifest_version = self.get_schema_version(manifest)
 
-        profile_dir = run_result['args']['profiles_dir']
-
-        if not self.profile_name:
-            self.profile_name = self.project['profile']
-
-        profile = self.load_yaml_with_jinja(
-            os.path.join(profile_dir, 'profiles.yml')
-        )[self.profile_name]
-
-        if not self.target:
-            self.target = profile['target']
-
-        profile = profile['outputs'][self.target]
+        self.run_metadata = run_result["metadata"]
+        self.command = run_result["args"]["which"]
 
         self.extract_adapter_type(profile)
         self.extract_dataset_namespace(profile)
 
         nodes = {}
-        # Filter non-model or test nodes
-        for name, node in manifest['nodes'].items():
-            if name.startswith('model.') or name.startswith('test.'):
+        # Filter nodes
+        for name, node in manifest["nodes"].items():
+            if any(
+                name.startswith(prefix) for prefix in ("model.", "test.", "snapshot.")
+            ):
                 nodes[name] = node
 
         context = DbtRunContext(manifest, run_result, catalog)
 
-        if self.command not in ['run', 'build', 'test']:
-            raise ValueError(
-                f"Not recognized run command "
-                f"{self.command} - should be run, test or build"
-            )
-
         events = DbtEvents()
-        if self.command in ['run', 'build']:
+
+        if self.command not in ["run", "build", "test", "seed", "snapshot"]:
+            if self.should_raise_on_unsupported_command:
+                raise UnsupportedDbtCommand(
+                    f"Not recognized run command "
+                    f"{self.command} - should be run, test, seed or build"
+                )
+            else:
+                return events
+
+        if self.command in ["run", "build", "seed", "snapshot"]:
             events += self.parse_execution(context, nodes)
-        if self.command in ['test', 'build']:
+        if self.command in ["test", "build"]:
             events += self.parse_test(context, nodes)
         return events
 
     @classmethod
-    def load_metadata(
-        cls,
-        path: str,
-        desired_schema_versions: List[int],
-        logger: logging.Logger
-    ) -> Dict:
-        with open(path, 'r') as f:
-            metadata = json.load(f)
-            str_schema_version = get_from_nullable_chain(
-                metadata,
-                ['metadata', 'dbt_schema_version']
-            )
-            schema_version = cls.get_version_number(str_schema_version)
-            if schema_version not in desired_schema_versions:
-                if schema_version > max(desired_schema_versions):
-                    logger.warning(
-                        f"Artifact schema version: {str_schema_version} is above dbt-ol "
-                        f"supported version {max(desired_schema_versions)}. "
-                        f"This might cause errors."
-                    )
-                else:
-                    raise ValueError(f"Wrong version of dbt metadata: {schema_version}, "
-                                     f"should be in {desired_schema_versions}")
-            return metadata
+    def get_schema_version(cls, metadata):
+        str_schema_version = get_from_nullable_chain(
+            metadata, ["metadata", "dbt_schema_version"]
+        )
+        return cls.get_version_number(str_schema_version)
 
     @staticmethod
     def get_version_number(version: str) -> int:
         # "https://schemas.getdbt.com/dbt/manifest/v2.json" -> "v2.json"
-        file = version.split('/')[-1]
+        file = version.split("/")[-1]
         # "v2.json" -> 2
-        return int(file.split('.')[0][1:])
-
-    @staticmethod
-    def env_var(var: str, default: Optional[str] = None) -> str:
-        """The env_var() function. Return the environment variable named 'var'.
-        If there is no such environment variable set, return the default.
-
-        If the default is None, raise an exception for an undefined variable.
-        """
-        if var in os.environ:
-            return os.environ[var]
-        elif default is not None:
-            return default
-        else:
-            msg = f"Env var required but not provided: '{var}'"
-            raise Exception(msg)
-
-    @staticmethod
-    def load_yaml(path: str) -> Dict:
-        with open(path, 'r') as f:
-            return yaml.load(f, Loader=yaml.FullLoader)
+        return int(file.split(".")[0][1:])
 
-    @staticmethod
-    def setup_jinja() -> Environment:
-        env = Environment(
-            extensions=["jinja2.ext.do"],
-            undefined=SkipUndefined
-        )
-        # When using env vars for Redshift port, it must be "{{ env_var('PORT') | as_number }}"
-        # otherwise Redshift driver will complain, hence the need to add the "as_number" filter
-        env.filters.update({"as_number": lambda x: x})
-        env.globals["env_var"] = DbtArtifactProcessor.env_var
-        return env
-
-    def load_yaml_with_jinja(self, path: str) -> Dict:
-        loaded = self.load_yaml(path)
-        if not self.jinja_environment:
-            self.jinja_environment = self.setup_jinja()
-        return self.render_values_jinja(environment=self.jinja_environment, value=loaded)
-
-    @classmethod
-    def render_values_jinja(cls, environment: Environment, value: T) -> T:
-        """
-        Traverses passed dictionary and render any string value using jinja.
-        Returns copy of the dict with parsed values.
-        """
-        if isinstance(value, dict):
-            parsed = {}
-            for key, val in value.items():
-                parsed[key] = cls.render_values_jinja(environment, val)
-            return parsed
-        elif isinstance(value, list):
-            parsed = []
-            for elem in value:
-                parsed.append(cls.render_values_jinja(environment, elem))
-            return parsed
-        elif isinstance(value, str):
-            return environment.from_string(value).render()
-        else:
-            return value
-
-    def parse_execution(
-        self,
-        context: DbtRunContext,
-        nodes: Dict
-    ) -> DbtEvents:
+    def parse_execution(self, context: DbtRunContext, nodes: Dict) -> DbtEvents:
         events = DbtEvents()
-        for run in context.run_results['results']:
-            name = run['unique_id']
-            if not name.startswith('model.') and not name.startswith('source.'):
+        for run in context.run_results["results"]:
+            name = run["unique_id"]
+            if not any(
+                name.startswith(prefix) for prefix in ("model.", "source.", "snapshot.")
+            ):
                 continue
-            if run['status'] == 'skipped':
+            if run["status"] == "skipped":
                 continue
 
             output_node = nodes[name]
-            started_at, completed_at = self.get_timings(run['timing'])
-            namespace, name, _ = self.extract_dataset_data(
-                ModelNode(output_node), None, has_facets=False
-            )
+            started_at, completed_at = self.get_timings(run["timing"])
 
             inputs = []
-            for node in context.manifest['parent_map'][run['unique_id']]:
-                if node.startswith('model.'):
-                    inputs.append(ModelNode(
-                        nodes[node],
-                        get_from_nullable_chain(context.catalog, ['nodes', node])
-                    ))
-                elif node.startswith('source.'):
-                    inputs.append(ModelNode(
-                        context.manifest['sources'][node],
-                        get_from_nullable_chain(context.catalog, ['sources', node])
-                    ))
+            for node in context.manifest["parent_map"][run["unique_id"]]:
+                if node.startswith("model."):
+                    inputs.append(
+                        ModelNode(
+                            nodes[node],
+                            get_from_nullable_chain(context.catalog, ["nodes", node]),
+                        )
+                    )
+                elif node.startswith("source."):
+                    inputs.append(
+                        ModelNode(
+                            context.manifest["sources"][node],
+                            get_from_nullable_chain(context.catalog, ["sources", node]),
+                        )
+                    )
 
             run_id = str(uuid.uuid4())
-            job_name = f"{output_node['database']}.{output_node['schema']}" \
-                f".{self.removeprefix(run['unique_id'], 'model.')}" \
-                + (".build.run" if self.command == 'build' else "")
-            events.add(self.to_openlineage_events(
-                run['status'],
-                started_at,
-                completed_at,
-                self.get_run(run_id),
-                Job(
-                    namespace=self.job_namespace,
-                    name=job_name,
-                    facets={
-                        'sql': SqlJobFacet(output_node['compiled_sql'])
-                    }
-                ),
-                [self.node_to_dataset(node, has_facets=True) for node in inputs],
-                self.node_to_output_dataset(
-                    ModelNode(
-                        output_node,
-                        get_from_nullable_chain(context.catalog, ['nodes', run['unique_id']])
+            if name.startswith("snapshot."):
+                job_name = (
+                    f"{output_node['database']}.{output_node['schema']}"
+                    f".{self.removeprefix(run['unique_id'], 'snapshot.')}"
+                    + (".build.snapshot" if self.command == "build" else ".snapshot")
+                )
+            else:
+                job_name = (
+                    f"{output_node['database']}.{output_node['schema']}"
+                    f".{self.removeprefix(run['unique_id'], 'model.')}"
+                    + (".build.run" if self.command == "build" else "")
+                )
+
+            if self.manifest_version >= 7:
+                sql = output_node.get("compiled_code", None)
+            else:
+                sql = output_node["compiled_sql"]
+
+            job_facets = {}
+            if sql:
+                job_facets["sql"] = SqlJobFacet(sql)
+
+            events.add(
+                self.to_openlineage_events(
+                    run["status"],
+                    started_at,
+                    completed_at,
+                    self.get_run(run_id),
+                    Job(namespace=self.job_namespace, name=job_name, facets=job_facets),
+                    [self.node_to_dataset(node, has_facets=True) for node in inputs],
+                    self.node_to_output_dataset(
+                        ModelNode(
+                            output_node,
+                            get_from_nullable_chain(
+                                context.catalog, ["nodes", run["unique_id"]]
+                            ),
+                        ),
+                        has_facets=True,
                     ),
-                    has_facets=True
                 )
-            ))
+            )
         return events
 
-    def parse_test(
-        self,
-        context: DbtRunContext,
-        nodes: Dict
-    ) -> DbtEvents:
-
+    def parse_test(self, context: DbtRunContext, nodes: Dict) -> DbtEvents:
         # The tests can have different timings, so just take current time
         started_at = datetime.datetime.now(datetime.timezone.utc).isoformat()
         completed_at = datetime.datetime.now(datetime.timezone.utc).isoformat()
 
         assertions = self.parse_assertions(context, nodes)
 
         events = DbtEvents()
-        for name, node in context.manifest['nodes'].items():
-            if not name.startswith('model.') and not name.startswith('source.'):
+        for name, node in context.manifest["nodes"].items():
+            if not name.startswith("model.") and not name.startswith("source."):
                 continue
             if len(assertions[name]) == 0:
                 continue
 
             assertion_facet = DataQualityAssertionsDatasetFacet(
                 assertions=assertions[name]
             )
 
             namespace, name, _ = self.extract_dataset_data(
-                ModelNode(node),
-                assertion_facet,
-                has_facets=False
+                ModelNode(node), assertion_facet, has_facets=False
             )
 
-            job_name = f"{node['database']}.{node['schema']}." \
-                f"{self.removeprefix(node['unique_id'], 'model.')}" \
-                + (".build.test" if self.command == 'build' else "")
+            job_name = (
+                f"{node['database']}.{node['schema']}."
+                f"{self.removeprefix(node['unique_id'], 'model.')}"
+                + (".build.test" if self.command == "build" else ".test")
+            )
 
             run_id = str(uuid.uuid4())
-            events.add(self.to_openlineage_events(
-                "success",
-                started_at,
-                completed_at,
-                self.get_run(run_id),
-                Job(self.job_namespace, job_name),
-                [Dataset(namespace, name, facets={
-                    "dataQualityAssertions": assertion_facet
-                })],
-                None
-            ))
+            events.add(
+                self.to_openlineage_events(
+                    "success",
+                    started_at,
+                    completed_at,
+                    self.get_run(run_id),
+                    Job(self.job_namespace, job_name),
+                    [
+                        Dataset(
+                            namespace,
+                            name,
+                            facets={"dataQualityAssertions": assertion_facet},
+                        )
+                    ],
+                    None,
+                )
+            )
         return events
 
     def parse_assertions(
-        self,
-        context: DbtRunContext,
-        nodes: Dict
+        self, context: DbtRunContext, nodes: Dict
     ) -> Dict[str, List[Assertion]]:
         assertions = collections.defaultdict(list)
-        for run in context.run_results['results']:
-            if not run['unique_id'].startswith('test.'):
+        for run in context.run_results["results"]:
+            if not run["unique_id"].startswith("test."):
                 continue
-            test_node = nodes[run['unique_id']]
+            test_node = nodes[run["unique_id"]]
 
             model_node = None
-            for node in context.manifest['parent_map'][run['unique_id']]:
-                if node.startswith('model.') or node.startswith('source.'):
+            for node in context.manifest["parent_map"][run["unique_id"]]:
+                if node.startswith("model.") or node.startswith("source."):
                     model_node = node
 
-            assertions[model_node].append(Assertion(
-                assertion=test_node['test_metadata']['name'],
-                success=True if run['status'] == 'pass' else False,
-                column=get_from_nullable_chain(
-                    test_node['test_metadata'],
-                    ['kwargs', 'column_name']
+            assertions[model_node].append(
+                Assertion(
+                    assertion=test_node["test_metadata"]["name"],
+                    success=True if run["status"] == "pass" else False,
+                    column=get_from_nullable_chain(
+                        test_node["test_metadata"], ["kwargs", "column_name"]
+                    ),
                 )
-            ))
+            )
 
             if not model_node:
                 raise ValueError(
                     f"Model node connected to test {nodes[run['unique_id']]} not found"
                 )
-        return assertions
+        return assertions  # type: ignore
 
     def to_openlineage_events(self, *args, **kwargs) -> Optional[DbtRunResult]:
         try:
             return self._to_openlineage_events(*args, **kwargs)
         except Exception as e:
             if self.skip_errors:
                 return None
@@ -486,206 +390,223 @@
         self,
         status: str,
         started_at: str,
         completed_at: str,
         run: Run,
         job: Job,
         inputs: List[Dataset],
-        output: Optional[Dataset]
+        output: Optional[Dataset],
     ) -> Optional[DbtRunResult]:
         start = RunEvent(
             eventType=RunState.START,
             eventTime=started_at,
             run=run,
             job=job,
             producer=self.producer,
             inputs=inputs,
-            outputs=[output] if output else []
+            outputs=[output] if output else [],
         )
-        if status == 'success':
+        if status == "success":
             return DbtRunResult(
                 start,
                 complete=RunEvent(
                     eventType=RunState.COMPLETE,
                     eventTime=completed_at,
                     run=run,
                     job=job,
                     producer=self.producer,
                     inputs=inputs,
-                    outputs=[output] if output else []
-                )
+                    outputs=[output] if output else [],
+                ),
             )
-        elif status == 'error':
+        elif status == "error":
             return DbtRunResult(
                 start,
                 fail=RunEvent(
                     eventType=RunState.FAIL,
                     eventTime=completed_at,
                     run=run,
                     job=job,
                     producer=self.producer,
                     inputs=inputs,
-                    outputs=[]
-                )
+                    outputs=[],
+                ),
             )
         else:
             # Should not happen?
-            raise ValueError(f"Run status was {status}, "
-                             f"should be in ['success', 'skipped', 'error']")
+            raise ValueError(
+                f"Run status was {status}, "
+                f"should be in ['success', 'skipped', 'error']"
+            )
 
     def node_to_dataset(
         self,
         node: ModelNode,
         assertions: Optional[DataQualityAssertionsDatasetFacet] = None,
-        has_facets: bool = False
+        has_facets: bool = False,
     ) -> Dataset:
-        name, namespace, facets = self.extract_dataset_data(node, assertions, has_facets)
+        name, namespace, facets = self.extract_dataset_data(
+            node, assertions, has_facets
+        )
         return Dataset(name, namespace, facets)
 
     def node_to_output_dataset(
-        self,
-        node: ModelNode,
-        has_facets: bool = False
+        self, node: ModelNode, has_facets: bool = False
     ) -> OutputDataset:
         name, namespace, facets = self.extract_dataset_data(node, None, has_facets)
         output_facets = {}
         if has_facets and node.catalog_node:
             bytes = get_from_multiple_chains(
                 node.catalog_node,
                 [
-                    ['stats', 'num_bytes', 'value'],  # bigquery
-                    ['stats', 'bytes', 'value'],  # snowflake
-                    ['stats', 'size', 'value']  # redshift (Note: size = count of 1MB blocks)
-                ]
+                    ["stats", "num_bytes", "value"],  # bigquery
+                    ["stats", "bytes", "value"],  # snowflake
+                    [
+                        "stats",
+                        "size",
+                        "value",
+                    ],  # redshift (Note: size = count of 1MB blocks)
+                ],
             )
             rows = get_from_multiple_chains(
                 node.catalog_node,
                 [
-                    ['stats', 'num_rows', 'value'],  # bigquery
-                    ['stats', 'row_count', 'value'],  # snowflake
-                    ['stats', 'rows', 'value']  # redshift
-                ]
+                    ["stats", "num_rows", "value"],  # bigquery
+                    ["stats", "row_count", "value"],  # snowflake
+                    ["stats", "rows", "value"],  # redshift
+                ],
             )
 
             if bytes:
-                bytes = int(bytes) if self.adapter_type != Adapter.REDSHIFT \
-                    else int(rows) * (2 ** 20)
+                bytes = (
+                    int(bytes)
+                    if self.adapter_type != Adapter.REDSHIFT
+                    else int(rows) * (2**20)
+                )
             if rows:
                 rows = int(rows)
 
-                output_facets['outputStatistics'] = OutputStatisticsOutputDatasetFacet(
-                    rowCount=rows,
-                    size=bytes
+                output_facets["outputStatistics"] = OutputStatisticsOutputDatasetFacet(
+                    rowCount=rows, size=bytes
                 )
-        return OutputDataset(
-            name, namespace, facets, output_facets
-        )
+        return OutputDataset(name, namespace, facets, output_facets)
 
     def extract_dataset_data(
         self,
         node: ModelNode,
         assertions: Optional[DataQualityAssertionsDatasetFacet],
-        has_facets: bool = False
+        has_facets: bool = False,
     ) -> Tuple[str, str, Dict]:
         if has_facets:
             facets = {
-                'dataSource': DataSourceDatasetFacet(
-                    name=self.dataset_namespace,
-                    uri=self.dataset_namespace
+                "dataSource": DataSourceDatasetFacet(
+                    name=self.dataset_namespace, uri=self.dataset_namespace
+                ),
+                "schema": SchemaDatasetFacet(
+                    fields=self.extract_metadata_fields(
+                        node.metadata_node["columns"].values()
+                    )
                 ),
-                'schema': SchemaDatasetFacet(
-                    fields=self.extract_metadata_fields(node.metadata_node['columns'].values())
-                )
             }
             if assertions:
-                facets['dataQualityAssertions'] = assertions
+                facets["dataQualityAssertions"] = assertions
             if node.catalog_node:
-                facets['schema'] = SchemaDatasetFacet(
+                facets["schema"] = SchemaDatasetFacet(
                     fields=self.extract_catalog_fields(
-                        node.catalog_node['columns'].values(),
-                        node.metadata_node['columns']
+                        node.catalog_node["columns"].values(),
+                        node.metadata_node["columns"],
                     )
                 )
         else:
             facets = {}
         return (
             self.dataset_namespace,
             f"{node.metadata_node['database']}."
             f"{node.metadata_node['schema']}."
             f"{node.metadata_node['name']}",
-            facets
+            facets,
         )
 
     @staticmethod
     def extract_metadata_fields(columns: List[Dict]) -> List[SchemaField]:
         """
         Extract table field info from metadata's node column info
         Should be used only in the lack of catalog's presence, as there's less
         information in metadata file than in catalog.
         """
         fields = []
         for field in columns:
-            type, description = None, None
-            if 'data_type' in field and field['data_type'] is not None:
-                type = field['data_type']
-            if 'description' in field and field['description'] is not None:
-                description = field['description']
-            fields.append(SchemaField(
-                name=field['name'], type=type, description=description
-            ))
+            of_type, description = None, None
+            if "data_type" in field and field["data_type"] is not None:
+                of_type = field["data_type"]
+            if "description" in field and field["description"] is not None:
+                description = field["description"]
+            fields.append(
+                SchemaField(
+                    name=field["name"], type=of_type or "", description=description
+                )
+            )
         return fields
 
     @staticmethod
-    def extract_catalog_fields(columns: List[Dict], metadata_columns: Dict) -> List[SchemaField]:
+    def extract_catalog_fields(
+        columns: List[Dict], metadata_columns: Dict
+    ) -> List[SchemaField]:
         """Extract table field info from catalog's node column info"""
         fields = []
         for field in columns:
-            name = field['name']
+            name = field["name"]
             type = None
-            if 'type' in field and field['type'] is not None:
-                type = field['type']
-            description = get_from_nullable_chain(metadata_columns, [name, 'description'])
-            fields.append(SchemaField(
-                name=name, type=type, description=description
-            ))
+            if "type" in field and field["type"] is not None:
+                type = field["type"]
+            description = get_from_nullable_chain(
+                metadata_columns, [name, "description"]
+            )
+            assert isinstance(type, str)
+            fields.append(SchemaField(name=name, type=type, description=description))
         return fields
 
     def extract_adapter_type(self, profile: Dict):
         try:
-            self.adapter_type = Adapter[profile['type'].upper()]
+            self.adapter_type = Adapter[profile["type"].upper()]
         except KeyError:
             raise NotImplementedError(
                 f"Only {Adapter.adapters()} adapters are supported right now. "
                 f"Passed {profile['type']}"
             )
 
     def extract_dataset_namespace(self, profile: Dict):
         self.dataset_namespace = self.extract_namespace(profile)
 
     def extract_namespace(self, profile: Dict) -> str:
         """Extract namespace from profile's type"""
         if self.adapter_type == Adapter.SNOWFLAKE:
-            return f"snowflake://{profile['account']}"
+            return f"snowflake://{fix_account_name(profile['account'])}"
         elif self.adapter_type == Adapter.BIGQUERY:
             return "bigquery"
         elif self.adapter_type == Adapter.REDSHIFT:
             return f"redshift://{profile['host']}:{profile['port']}"
+        elif self.adapter_type == Adapter.POSTGRES:
+            return f"postgres://{profile['host']}:{profile['port']}"
+        elif self.adapter_type == Adapter.DATABRICKS:
+            return f"databricks://{profile['host']}"
         elif self.adapter_type == Adapter.SPARK:
             port = ""
 
-            if 'port' in profile:
+            if "port" in profile:
                 port = f":{profile['port']}"
-            elif profile['method'] in [
-                SparkConnectionMethod.HTTP.value, SparkConnectionMethod.ODBC.value
+            elif profile["method"] in [
+                SparkConnectionMethod.HTTP.value,
+                SparkConnectionMethod.ODBC.value,
             ]:
-                port = '443'
-            elif profile['method'] == SparkConnectionMethod.THRIFT.value:
-                port = '10001'
+                port = "443"
+            elif profile["method"] == SparkConnectionMethod.THRIFT.value:
+                port = "10001"
 
-            if profile['method'] in SparkConnectionMethod.methods():
+            if profile["method"] in SparkConnectionMethod.methods():
                 return f"spark://{profile['host']}{port}"
             else:
                 raise NotImplementedError(
                     f"Connection method `{profile['method']}` is not "
                     f"supported for spark adapter."
                 )
         else:
@@ -694,34 +615,34 @@
                 f"Passed {profile['type']}"
             )
 
     def get_run(self, run_id: str) -> Run:
         return Run(
             runId=run_id,
             facets={
-                "parent": self._dbt_run_metadata.to_openlineage(),
-                "dbt_version": self.dbt_version_facet()
-            }
+                "parent": self._dbt_run_metadata.to_openlineage()
+                if self._dbt_run_metadata
+                else None,
+                "dbt_version": self.dbt_version_facet(),
+            },
         )
 
     def dbt_version_facet(self):
-        return DbtVersionRunFacet(
-            version=self.run_metadata['dbt_version']
-        )
+        return DbtVersionRunFacet(version=self.run_metadata["dbt_version"])
 
     @staticmethod
     def get_timings(timings: List[Dict]) -> Tuple[str, str]:
         """Extract timing info from run_result's timing dict"""
         try:
-            timing = list(filter(lambda x: x['name'] == 'execute', timings))[0]
-            return timing['started_at'], timing['completed_at']
+            timing = list(filter(lambda x: x["name"] == "execute", timings))[0]
+            return timing["started_at"], timing["completed_at"]
         except IndexError:
             # Run failed: there is no timing data
-            timing = datetime.datetime.now(datetime.timezone.utc).isoformat()
-            return timing, timing
+            timing_str = datetime.datetime.now(datetime.timezone.utc).isoformat()
+            return timing_str, timing_str
 
     @staticmethod
     def removeprefix(string: str, prefix: str) -> str:
         if string.startswith(prefix):
-            return string[len(prefix):]
+            return string[len(prefix) :]
         else:
             return string[:]
```

### Comparing `openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/action.py` & `openlineage-integration-common-1.0.0/openlineage/common/provider/great_expectations/action.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,74 @@
+# Copyright 2018-2023 contributors to the OpenLineage project
 # SPDX-License-Identifier: Apache-2.0
+
 import copy
 import logging
 import os
 from collections import defaultdict
 from datetime import datetime
-from typing import Optional, List
+from typing import Dict, List, Optional, Union
 from urllib.parse import urlparse
 from uuid import uuid4
 
+from openlineage.client import OpenLineageClient, OpenLineageClientOptions
+from openlineage.client.facet import (
+    BaseFacet,
+    ColumnMetric,
+    DataQualityMetricsInputDatasetFacet,
+    DocumentationJobFacet,
+    ParentRunFacet,
+    SourceCodeLocationJobFacet,
+)
+from openlineage.client.run import Job, Run, RunEvent, RunState
+from openlineage.client.serde import Serde
+from openlineage.common.dataset import Dataset, Field, Source
+from openlineage.common.dataset import Dataset as OLDataset
+from openlineage.common.provider.great_expectations.facets import (
+    GreatExpectationsAssertionsDatasetFacet,
+    GreatExpectationsRunFacet,
+)
+from openlineage.common.provider.great_expectations.results import (
+    COLUMN_EXPECTATIONS_PARSER,
+    EXPECTATIONS_PARSERS,
+    GreatExpectationsAssertion,
+)
+from openlineage.common.provider.snowflake import fix_snowflake_sqlalchemy_uri
+from openlineage.common.sql import parse
+
 from great_expectations.checkpoint import ValidationAction
 from great_expectations.core import ExpectationSuiteValidationResult
-from great_expectations.data_context.types.resource_identifiers import \
-    ValidationResultIdentifier
-from great_expectations.dataset import SqlAlchemyDataset, PandasDataset, \
-    Dataset as GEDataset
+from great_expectations.data_context.types.resource_identifiers import (
+    ValidationResultIdentifier,
+)
+from great_expectations.dataset import Dataset as GEDataset
+from great_expectations.dataset import (
+    PandasDataset,
+    SqlAlchemyDataset,
+)
 from great_expectations.execution_engine import (
-    SqlAlchemyExecutionEngine, PandasExecutionEngine,
+    PandasExecutionEngine,
+    SqlAlchemyExecutionEngine,
+)
+from great_expectations.execution_engine.sqlalchemy_batch_data import (
+    SqlAlchemyBatchData,
 )
-from great_expectations.execution_engine.sqlalchemy_batch_data import \
-    SqlAlchemyBatchData
 from great_expectations.validator.validator import Validator
-from openlineage.client import OpenLineageClient, OpenLineageClientOptions
-from openlineage.client.facet import ParentRunFacet, DocumentationJobFacet, \
-    SourceCodeLocationJobFacet, DataQualityMetricsInputDatasetFacet, \
-    ColumnMetric
-from openlineage.client.run import RunEvent, RunState, Run, Job
-from openlineage.client.serde import Serde
-from openlineage.common.dataset import Dataset, Source, Field
-from openlineage.common.dataset import Dataset as OLDataset
-from openlineage.common.provider.great_expectations.facets import \
-    GreatExpectationsAssertionsDatasetFacet, \
-    GreatExpectationsRunFacet
-from openlineage.common.provider.great_expectations.results import \
-    EXPECTATIONS_PARSERS, \
-    COLUMN_EXPECTATIONS_PARSER, \
-    GreatExpectationsAssertion
-from openlineage.common.sql import parse
-from sqlalchemy import MetaData, Table
-from sqlalchemy.engine import Connection
+
+# There is no guarantee that SqlAlchemy is available with Great Expectations.
+# Especially, it could be used only with Pandas datasets, in which case
+# we shouldn't try to import it.
+# Great Expectations itself tries hard to not import SqlAlchemy if not needed.
+try:
+    from sqlalchemy import MetaData, Table
+    from sqlalchemy.engine import Connection
+except ImportError:
+    MetaData = None  # type: ignore
+    Table = None  # type: ignore
+    Connection = None  # type: ignore
 
 
 class OpenLineageValidationAction(ValidationAction):
     """
     ValidationAction implementation which posts RunEvents for a GreatExpectations validation job.
 
     Openlineage host parameters can be passed in as constructor arguments or environment variables
@@ -61,238 +88,360 @@
     argument). The DataQualityDatasetFacet is also posted as the more standard OpenLineage
     DataQualityMetricsInputDatasetFacet.
 
     The resulting RunEvent is returned from the _run method, so it can be seen in the
     actions_results field of the validation results.
     """
 
-    def __init__(self, data_context,
-                 openlineage_host=None,
-                 openlineage_namespace=None,
-                 openlineage_apiKey=None,
-                 openlineage_parent_run_id=None,
-                 openlineage_parent_job_namespace=None,
-                 openlineage_parent_job_name=None,
-                 job_name=None,
-                 job_description=None,
-                 code_location=None,
-                 openlineage_run_id=None,
-                 do_publish=True):
+    def __init__(
+        self,
+        data_context,
+        openlineage_host=None,
+        openlineage_namespace=None,
+        openlineage_apiKey=None,
+        openlineage_parent_run_id=None,
+        openlineage_parent_job_namespace=None,
+        openlineage_parent_job_name=None,
+        job_name=None,
+        job_description=None,
+        code_location=None,
+        openlineage_run_id=None,
+        do_publish=True,
+    ):
         super().__init__(data_context)
         if openlineage_host is not None:
-            self.openlineage_client = OpenLineageClient(openlineage_host,
-                                                        OpenLineageClientOptions(
-                                                            api_key=openlineage_apiKey))
+            self.openlineage_client = OpenLineageClient(
+                openlineage_host, OpenLineageClientOptions(api_key=openlineage_apiKey)
+            )
         else:
             self.openlineage_client = OpenLineageClient.from_environment()
         if openlineage_namespace is not None:
             self.namespace = openlineage_namespace
         else:
-            self.namespace = os.getenv('OPENLINEAGE_NAMESPACE', 'default')
+            self.namespace = os.getenv("OPENLINEAGE_NAMESPACE", "default")
         if openlineage_run_id is not None:
             self.run_id = openlineage_run_id
         else:
             self.run_id = uuid4()
         self.parent_run_id = openlineage_parent_run_id
         self.parent_job_namespace = openlineage_parent_job_namespace
         self.parent_job_name = openlineage_parent_job_name
         self.job_name = job_name
         self.job_description = job_description
         self.code_location = code_location
         self.do_publish = do_publish
 
-    def _run(self,
-             validation_result_suite: ExpectationSuiteValidationResult,
-             validation_result_suite_identifier: ValidationResultIdentifier,
-             data_asset: [GEDataset, Validator],
-             expectation_suite_identifier=None,
-             checkpoint_identifier=None,
-             payload=None):
+    def _run(
+        self,
+        validation_result_suite: ExpectationSuiteValidationResult,
+        validation_result_suite_identifier: ValidationResultIdentifier,
+        data_asset: Union[GEDataset, Validator],
+        expectation_suite_identifier=None,
+        checkpoint_identifier=None,
+        payload=None,
+    ):
         # Initialize logger here so that the action is serializable until it actually runs
-        self.log = logging.getLogger(self.__class__.__module__ + '.' + self.__class__.__name__)
+        self.log = logging.getLogger(
+            self.__class__.__module__ + "." + self.__class__.__name__
+        )
 
         datasets = []
         if isinstance(data_asset, SqlAlchemyDataset):
-            datasets = self._fetch_datasets_from_sql_source(data_asset, validation_result_suite)
+            datasets = self._fetch_datasets_from_sql_source(
+                data_asset, validation_result_suite
+            )
         elif isinstance(data_asset, PandasDataset):
-            datasets = self._fetch_datasets_from_pandas_source(data_asset, validation_result_suite)
+            datasets = self._fetch_datasets_from_pandas_source(
+                data_asset, validation_result_suite
+            )
         elif isinstance(data_asset.execution_engine, SqlAlchemyExecutionEngine):
-            datasets = self._fetch_datasets_from_sql_source(data_asset, validation_result_suite)
+            datasets = self._fetch_datasets_from_sql_source(
+                data_asset, validation_result_suite
+            )
         elif isinstance(data_asset.execution_engine, PandasExecutionEngine):
-            datasets = self._fetch_datasets_from_pandas_source(data_asset, validation_result_suite)
+            datasets = self._fetch_datasets_from_pandas_source(
+                data_asset, validation_result_suite
+            )
         run_facets = {}
         if self.parent_run_id is not None:
-            run_facets.update({"parentRun": ParentRunFacet.create(
-                self.parent_run_id,
-                self.parent_job_namespace,
-                self.parent_job_name
-            )})
+            run_facets.update(
+                {
+                    "parentRun": ParentRunFacet.create(
+                        self.parent_run_id,
+                        self.parent_job_namespace,
+                        self.parent_job_name,
+                    )
+                }
+            )
 
         # workaround for GE v2 and v3 API difference
-        suite_meta = copy.deepcopy(validation_result_suite.meta)
-        if 'expectation_suite_meta' not in suite_meta:
-            suite_meta['expectation_suite_meta'] = validation_result_suite.meta
+        suite_meta = dict(
+            {
+                key: self._ser(value)
+                for key, value in copy.deepcopy(validation_result_suite.meta).items()
+            }
+        )
+        if "expectation_suite_meta" not in suite_meta:
+            suite_meta["expectation_suite_meta"] = dict(
+                {
+                    key: self._ser(value)
+                    for key, value in copy.deepcopy(
+                        validation_result_suite.meta
+                    ).items()
+                }
+            )
         run_facets.update(
-            {"great_expectations_meta": GreatExpectationsRunFacet(
-                **suite_meta,
-            )})
-        job_facets = {}
+            {
+                "great_expectations_meta": GreatExpectationsRunFacet(
+                    **suite_meta,
+                )
+            }
+        )
+        job_facets: Dict[str, BaseFacet] = {}
         if self.job_description:
-            job_facets.update({
-                "documentation": DocumentationJobFacet(self.job_description)
-            })
+            job_facets["documentation"] = DocumentationJobFacet(self.job_description)
         if self.code_location:
-            job_facets.update({
-                "sourceCodeLocation": SourceCodeLocationJobFacet("", self.code_location)
-            })
+            job_facets["sourceCodeLocation"] = SourceCodeLocationJobFacet(
+                type="", url=self.code_location
+            )
 
         job_name = self.job_name
         if self.job_name is None:
-            job_name = validation_result_suite.meta["expectation_suite_name"] + '.' \
-                       + validation_result_suite_identifier.batch_identifier
+            job_name = (
+                validation_result_suite.meta["expectation_suite_name"]
+                + "."
+                + validation_result_suite_identifier.batch_identifier
+            )
         run_event = RunEvent(
             eventType=RunState.COMPLETE,
             eventTime=datetime.now().isoformat(),
             run=Run(runId=str(self.run_id), facets=run_facets),
             job=Job(self.namespace, job_name, facets=job_facets),
             inputs=datasets,
             outputs=[],
-            producer="https://github.com/OpenLineage/OpenLineage/tree/$VERSION/integration/common/openlineage/provider/great_expectations"  # noqa
+            producer="https://github.com/OpenLineage/OpenLineage/tree/$VERSION/integration/common/openlineage/provider/great_expectations",  # noqa
         )
         if self.do_publish:
             self.openlineage_client.emit(run_event)
         # Great expectations tries to append stuff here, so we need to make it a dict
         return Serde.to_dict(run_event)
 
-    def _fetch_datasets_from_pandas_source(self, data_asset: PandasDataset,
-                                           validation_result_suite: ExpectationSuiteValidationResult) -> List[OLDataset]:  # noqa
+    def _ser(self, obj):
+        if hasattr(obj, "to_json_dict"):
+            return obj.to_json_dict()
+        else:
+            return obj
+
+    def _fetch_datasets_from_pandas_source(
+        self,
+        data_asset: Union[PandasDataset, Validator],
+        validation_result_suite: ExpectationSuiteValidationResult,
+    ) -> List[OLDataset]:  # noqa
         """
         Generate a list of OpenLineage Datasets from a PandasDataset
         :param data_asset:
         :param validation_result_suite:
         :return:
         """
-        if data_asset.batch_kwargs.__contains__("path"):
-            path = data_asset.batch_kwargs.get("path")
+        if isinstance(data_asset, PandasDataset):
+            if data_asset.batch_kwargs.__contains__("path"):
+                path = data_asset.batch_kwargs.get("path")
+                if path.startswith("/"):
+                    path = "file://{}".format(path)
+                parsed_url = urlparse(path)
+                columns = [
+                    Field(
+                        name=col,
+                        type=str(data_asset[col].dtype)
+                        if data_asset[col].dtype is not None
+                        else "UNKNOWN",
+                    )
+                    for col in data_asset.columns
+                ]
+                return [
+                    Dataset(
+                        source=self._source(parsed_url._replace(path="")),
+                        name=parsed_url.path,
+                        fields=columns,
+                        input_facets=self.results_facet(validation_result_suite),
+                    ).to_openlineage_dataset()
+                ]
+            return []
+        else:
+            batch = data_asset.active_batch
+            batch_data = batch.data
+            path = (
+                batch.batch_request.runtime_parameters.get("path", None)
+                if batch.batch_request.runtime_parameters is not None
+                else None
+            )
+            if path is None:
+                return []
             if path.startswith("/"):
                 path = "file://{}".format(path)
             parsed_url = urlparse(path)
-            columns = [Field(
-                name=col,
-                type=str(data_asset[col].dtype) if data_asset[col].dtype is not None else 'UNKNOWN'
-            ) for col in data_asset.columns]
+            columns = [
+                Field(
+                    name=col,
+                    type=str(data_asset[col].dtype)
+                    if data_asset[col].dtype is not None
+                    else "UNKNOWN",
+                )
+                for col in batch_data.columns
+            ]
             return [
                 Dataset(
-                    source=self._source(parsed_url._replace(path='')),
+                    source=self._source(parsed_url._replace(path="")),
                     name=parsed_url.path,
                     fields=columns,
-                    input_facets=self.results_facet(validation_result_suite)
+                    input_facets=self.results_facet(validation_result_suite),
                 ).to_openlineage_dataset()
             ]
 
-    def _fetch_datasets_from_sql_source(self, data_asset: [SqlAlchemyDataset, Validator],
-                                        validation_result_suite: ExpectationSuiteValidationResult) -> List[OLDataset]:  # noqa
+    def _fetch_datasets_from_sql_source(
+        self,
+        data_asset: Union[SqlAlchemyDataset, Validator],
+        validation_result_suite: ExpectationSuiteValidationResult,
+    ) -> List[OLDataset]:  # noqa
         """
         Generate a list of OpenLineage Datasets from a SqlAlchemyDataset.
         :param data_asset:
         :param validation_result_suite:
         :return:
         """
         metadata = MetaData()
         if isinstance(data_asset, SqlAlchemyDataset):
             if data_asset.generated_table_name is not None:
-                custom_sql = data_asset.batch_kwargs.get('query')
-                parsed_sql = parse(custom_sql)
+                custom_sql = data_asset.batch_kwargs.get("query")
+                parsed_sql = parse(
+                    custom_sql, dialect=data_asset.engine.dialect.name.lower()
+                )
                 return [
-                    self._get_sql_table(data_asset, metadata, t.schema, t.name,
-                                        validation_result_suite) for t in
-                    parsed_sql.in_tables
+                    self._get_sql_table(
+                        data_asset, metadata, t.schema, t.name, validation_result_suite
+                    )
+                    for t in parsed_sql.in_tables
                 ]
-            return [self._get_sql_table(data_asset, metadata, data_asset._table.schema,
-                                        data_asset._table.name,
-                                        validation_result_suite)]
+            return [
+                self._get_sql_table(
+                    data_asset,
+                    metadata,
+                    data_asset._table.schema,
+                    data_asset._table.name,
+                    validation_result_suite,
+                )
+            ]
         else:
             batch = data_asset.active_batch
             batch_data = batch["data"]
+            custom_sql = (
+                batch.batch_request.runtime_parameters.get("query", None)
+                if batch.batch_request.runtime_parameters is not None
+                else None
+            )
+            if custom_sql:
+                parsed_sql = parse(
+                    custom_sql, dialect=data_asset.execution_engine.dialect_name
+                )
+                return [
+                    self._get_sql_table(
+                        batch_data, metadata, t.schema, t.name, validation_result_suite
+                    )
+                    for t in parsed_sql.in_tables
+                ]
             table_name = batch["batch_spec"]["table_name"]
             try:
                 schema_name = batch["batch_spec"]["schema_name"]
             except KeyError:
                 schema_name = None
             return [
                 self._get_sql_table(
                     batch_data,
                     metadata,
                     schema_name,
                     table_name,
-                    validation_result_suite
+                    validation_result_suite,
                 )
             ]
 
     def _get_sql_table(
         self,
-        data_asset: [SqlAlchemyDataset, SqlAlchemyBatchData],
+        data_asset: Union[SqlAlchemyDataset, SqlAlchemyBatchData],
         meta: MetaData,
         schema: Optional[str],
         table_name: str,
-        validation_result_suite: ExpectationSuiteValidationResult
+        validation_result_suite: ExpectationSuiteValidationResult,
     ) -> Optional[OLDataset]:
         """
         Construct a Dataset from the connection url and the columns returned from the
         SqlAlchemyDataset
         :param data_asset:
         :return:
         """
-        engine = data_asset.engine if isinstance(data_asset, SqlAlchemyDataset)\
+        engine = (
+            data_asset.engine
+            if isinstance(data_asset, SqlAlchemyDataset)
             else data_asset._engine
+        )
         if isinstance(engine, Connection):
             engine = engine.engine
         datasource_url = engine.url
+
+        if engine.dialect.name.lower() == "snowflake":
+            if engine.connection_string:
+                datasource_url = engine.connection_string
+            else:
+                datasource_url = engine.url
+            datasource_url = fix_snowflake_sqlalchemy_uri(datasource_url)
+
+        # bug in sql parser doesn't strip ` character from bigquery tables
+        if table_name.endswith("`") or table_name.startswith("`"):
+            table_name = table_name.replace("`", "")
         if engine.dialect.name.lower() == "bigquery":
-            schema = '{}.{}'.format(datasource_url.host, datasource_url.database)
+            schema = "{}.{}".format(datasource_url.host, datasource_url.database)
 
         table = Table(table_name, meta, autoload_with=engine)
 
-        fields = [Field(
-            name=key,
-            type=str(col.type) if col.type is not None else 'UNKNOWN',
-            description=col.doc
-        ) for key, col in table.columns.items()]
-
-        name = table_name \
-            if schema is None \
-            else "{}.{}".format(schema, table_name)
+        fields = [
+            Field(
+                name=key,
+                type=str(col.type) if col.type is not None else "UNKNOWN",
+                description=col.doc,
+            )
+            for key, col in table.columns.items()
+        ]
+
+        name = table_name if schema is None else "{}.{}".format(schema, table_name)
 
         results_facet = self.results_facet(validation_result_suite)
         return Dataset(
             source=self._source(urlparse(str(datasource_url))),
             fields=fields,
             name=name,
-            input_facets=results_facet
+            input_facets=results_facet,
         ).to_openlineage_dataset()
 
     def _source(self, url) -> Source:
         """
         Construct a Source from the connection url. Special handling for BigQuery is included.
         We attempt to strip credentials from the connection url, if present.
         :param url: a parsed url, as returned from urlparse()
         :return:
         """
 
         if url.scheme == "bigquery":
-            return Source(
-                scheme='bigquery',
-                connection_url='bigquery'
-            )
+            return Source(scheme="bigquery", connection_url="bigquery")
 
         return Source(
             scheme=url.scheme,
             authority=url.hostname,
             # Remove credentials from the URL if present
-            connection_url=url._replace(netloc=url.hostname, query=None, fragment=None).geturl()
+            connection_url=url._replace(
+                netloc=url.hostname, query=None, fragment=None
+            ).geturl(),
         )
 
     def results_facet(self, validation_result: ExpectationSuiteValidationResult):
         """
         Parse the validation result and extract input facets based on the results. We'll return a
         DataQualityDatasetFacet, a GreatExpectationsAssertionsDatasetFacet, and a
         (openlineage standard) DataQualityMetricsInputDatasetFacet
@@ -304,70 +453,79 @@
             if not data_quality_facet:
                 return None
 
             assertions_facet = self.parse_assertions(validation_result)
             if not assertions_facet:
                 return None
             return {
-                'dataQuality': data_quality_facet,
-                'greatExpectations_assertions': assertions_facet,
-                'dataQualityMetrics': data_quality_facet
+                "dataQuality": data_quality_facet,
+                "greatExpectations_assertions": assertions_facet,
+                "dataQualityMetrics": data_quality_facet,
             }
 
         except ValueError:
             self.log.exception("Exception while retrieving great expectations dataset")
         return None
 
-    def parse_data_quality_facet(self, validation_result: ExpectationSuiteValidationResult) \
-            -> Optional[DataQualityMetricsInputDatasetFacet]:
+    def parse_data_quality_facet(
+        self, validation_result: ExpectationSuiteValidationResult
+    ) -> Optional[DataQualityMetricsInputDatasetFacet]:
         """
         Parse the validation result and extract a DataQualityDatasetFacet
         :param validation_result:
         :return:
         """
-        facet_data = {
-            "columnMetrics": defaultdict(dict)
-        }
+        facet_data: Dict[str, defaultdict] = {"columnMetrics": defaultdict(dict)}
 
         # try to get to actual expectations results
         try:
-            expectations_results = validation_result['results']
+            expectations_results = validation_result["results"]
             for expectation in expectations_results:
                 for parser in EXPECTATIONS_PARSERS:
 
                     # accept possible duplication, should have no difference in results
                     if parser.can_accept(expectation):
                         result = parser.parse_expectation_result(expectation)
                         facet_data[result.facet_key] = result.value
                 for parser in COLUMN_EXPECTATIONS_PARSER:
                     if parser.can_accept(expectation):
                         result = parser.parse_expectation_result(expectation)
-                        facet_data['columnMetrics'][result.column_id][result.facet_key] \
-                            = result.value
-
-            for key in facet_data['columnMetrics'].keys():
-                facet_data['columnMetrics'][key] = ColumnMetric(**facet_data['columnMetrics'][key])
-            return DataQualityMetricsInputDatasetFacet(**facet_data)
+                        facet_data["columnMetrics"][result.column_id][
+                            result.facet_key
+                        ] = result.value
+
+            for key in facet_data["columnMetrics"].keys():
+                facet_data["columnMetrics"][key] = ColumnMetric(
+                    **facet_data["columnMetrics"][key]
+                )
+            return DataQualityMetricsInputDatasetFacet(**facet_data)  # type: ignore[arg-type]
         except ValueError:
             self.log.exception(
                 "Great Expectations's CheckpointResult object does not have expected key"
             )
         return None
 
-    def parse_assertions(self, validation_result: ExpectationSuiteValidationResult) -> \
-            Optional[GreatExpectationsAssertionsDatasetFacet]:
+    def parse_assertions(
+        self, validation_result: ExpectationSuiteValidationResult
+    ) -> Optional[GreatExpectationsAssertionsDatasetFacet]:
         assertions = []
 
         try:
             for expectation in validation_result.results:
-                assertions.append(GreatExpectationsAssertion(
-                    expectationType=expectation['expectation_config']['expectation_type'],
-                    success=expectation['success'],
-                    column=expectation['expectation_config']['kwargs'].get('column', None)
-                ))
+                assertions.append(
+                    GreatExpectationsAssertion(
+                        expectationType=expectation["expectation_config"][
+                            "expectation_type"
+                        ],
+                        success=expectation["success"],
+                        column=expectation["expectation_config"]["kwargs"].get(
+                            "column", None
+                        ),
+                    )
+                )
 
             return GreatExpectationsAssertionsDatasetFacet(assertions)
         except ValueError:
             self.log.exception(
                 "Great Expectations's CheckpointResult object does not have expected key"
             )
         return None
```

### Comparing `openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/facets.py` & `openlineage-integration-common-1.0.0/openlineage/common/provider/great_expectations/facets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,39 @@
+# Copyright 2018-2023 contributors to the OpenLineage project
 # SPDX-License-Identifier: Apache-2.0
 
-from typing import List, Optional, Union, Dict
+from typing import Dict, List, Optional, Union
 
 import attr
-from great_expectations.core import IDDict
-from great_expectations.core.batch import BatchMarkers, BatchDefinition
-from great_expectations.core.id_dict import BatchSpec, BatchKwargs
 from openlineage.client.facet import BaseFacet
-
 from openlineage.common.provider.great_expectations.results import GreatExpectationsAssertion
 
+from great_expectations.core import IDDict
+from great_expectations.core.batch import BatchDefinition, BatchMarkers
+from great_expectations.core.id_dict import BatchKwargs, BatchSpec
+
 
 @attr.s
 class GreatExpectationsRunFacet(BaseFacet):
     """
     Custom facet which describes the instance of GreatExpectations and the suite configuration
     """
     great_expectations_version = attr.ib()
     expectation_suite_name: str = attr.ib()
-    run_id: Dict = attr.ib(converter=lambda x: x.to_json_dict())
+    run_id: Dict = attr.ib()    # type: ignore
     expectation_suite_meta: Dict = attr.ib()
     validation_time: str = attr.ib()
     batch_spec: Optional[BatchSpec] = attr.ib(default=None)
     batch_markers: Optional[BatchMarkers] = attr.ib(default=None)
     batch_kwargs: Optional[BatchKwargs] = attr.ib(default=None)
     active_batch_definition: Union[None, IDDict, BatchDefinition] = attr.ib(default=None)
     batch_parameters = attr.ib(default=None)
+    checkpoint_name: Optional[str] = attr.ib(default=None)
+    validation_id: Optional[str] = attr.ib(default=None)
+    checkpoint_id: Optional[str] = attr.ib(default=None)
 
     @staticmethod
     def _get_schema() -> str:
         return "https://github.com/OpenLineage/OpenLineage/tree/main/integration/common/openlineage/common/provider/ge-run-facet.json"  # noqa
 
 
 @attr.s
```

### Comparing `openlineage-integration-common-0.9.0/openlineage/common/provider/great_expectations/results.py` & `openlineage-integration-common-1.0.0/openlineage/common/provider/great_expectations/results.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+# Copyright 2018-2023 contributors to the OpenLineage project
 # SPDX-License-Identifier: Apache-2.0
 
-from typing import Optional, Any
+from typing import Any, Optional
 
 import attr
-from great_expectations.core import ExpectationValidationResult
-
 from openlineage.common.utils import get_from_nullable_chain
 
+from great_expectations.core import ExpectationValidationResult
+
 
 @attr.s
 class ExpectationsParserResult:
     """
     Internal class to represent actual expectation values, per table and optionally per column
     """
     facet_key: str = attr.ib()
@@ -30,15 +31,15 @@
     Base expectation parser. Dispatches parser looking at expectation type.
     Implementations should extract result from result dictionary.
     """
     expectation_key: str = ''
     facet_key: str = ''
 
     @classmethod
-    def can_accept(cls, expectation_result: ExpectationValidationResult) -> bool:
+    def can_accept(cls, expectation_result: ExpectationValidationResult) -> Optional[Any]:
         expectation_type = get_from_nullable_chain(expectation_result,
                                                    ['expectation_config', 'expectation_type'])
         return expectation_type and expectation_type == cls.expectation_key
 
     @staticmethod
     def parse_expectation_result(
             expectation_result: ExpectationValidationResult) -> ExpectationsParserResult:
@@ -62,26 +63,26 @@
     expectation_key = 'expect_table_row_count_to_equal'
 
 
 class FileSizeExpectationsParser(ExpectationsParser):
     expectation_key = 'expect_file_size_to_be_between'
 
     @staticmethod
-    def parse_expectation_result(expectation_result: dict) -> ExpectationsParserResult:
+    def parse_expectation_result(expectation_result: dict) -> ExpectationsParserResult:  # type: ignore # noqa
         pass  # TODO: file asset validation
 
 
 class ColumnExpectationsParser(ExpectationsParser):
     """
     Extractor for column-based expectations. Looks at column name in addition to expectation type
     """
     column = ''
 
     @classmethod
-    def can_accept(cls, expectation_result: ExpectationValidationResult) -> bool:
+    def can_accept(cls, expectation_result: ExpectationValidationResult) -> Optional[Any]:
         expectation_type = get_from_nullable_chain(expectation_result,
                                                    ['expectation_config', 'expectation_type'])
         extracted_column = get_from_nullable_chain(
             expectation_result,
             ['expectation_config', 'kwargs', 'column']
         )
         return expectation_type and extracted_column and expectation_type == cls.expectation_key
```

### Comparing `openlineage-integration-common-0.9.0/openlineage/common/sql/__init__.py` & `openlineage-integration-common-1.0.0/openlineage/common/sql/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import logging
-from typing import Optional, Union, List
+from typing import List, Optional, Union
 
+from openlineage_sql import (
+    ColumnLineage,  # noqa: F401
+    ColumnMeta,  # noqa: F401
+    DbTableMeta,  # noqa: F401
+    ExtractionError,  # noqa: F401
+    SqlMeta,  # noqa: F401
+    provider,  # noqa: F401
+)
+from openlineage_sql import parse as parse_sql  # noqa: F401  # noqa: F401
 
 log = logging.getLogger(__name__)
 
 
-try:
-    from openlineage_sql import parse as parse_sql, SqlMeta, DbTableMeta, provider  # noqa: F401
-except ImportError:
-    from openlineage.common.sql.parser import parse as parse_sql, SqlMeta, DbTableMeta, provider  # noqa: F401,E501
-
-
 def parse(
     sql: Union[List[str], str],
     dialect: Optional[str] = None,
-    default_schema: Optional[str] = None
+    default_schema: Optional[str] = None,
 ) -> Optional[SqlMeta]:
     if isinstance(sql, str):
         sql = [sql]
     try:
         return parse_sql(sql, dialect=dialect, default_schema=default_schema)
     except Exception as e:
         log.error(f"SQL parser failed: {e}")
```

### Comparing `openlineage-integration-common-0.9.0/openlineage/common/utils.py` & `openlineage-integration-common-1.0.0/openlineage/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# SPDX-License-Identifier: Apache-2.0.
-from typing import Dict, Any, List, Optional
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
+from typing import Any, Dict, List, Optional
 
 
 def get_from_nullable_chain(source: Any, chain: List[str]) -> Optional[Any]:
     """
     Get object from nested structure of objects, where it's not guaranteed that
     all keys in the nested structure exist.
     Intended to replace chain of `dict.get()` statements.
@@ -26,15 +28,15 @@
             next_key = chain.pop()
             if isinstance(source, dict):
                 source = source.get(next_key)
             else:
                 source = getattr(source, next_key)
         return source
     except AttributeError:
-        return
+        return None
 
 
 def get_from_multiple_chains(source: Dict[str, Any], chains: List[List[str]]) -> Optional[Any]:
     for chain in chains:
         result = get_from_nullable_chain(source, chain)
         if result:
             return result
```

### Comparing `openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/SOURCES.txt` & `openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 openlineage/common/__init__.py
 openlineage/common/dataset.py
 openlineage/common/models.py
 openlineage/common/test.py
 openlineage/common/utils.py
 openlineage/common/provider/bigquery.py
-openlineage/common/provider/dbt.py
+openlineage/common/provider/redshift_data.py
+openlineage/common/provider/snowflake.py
+openlineage/common/provider/dbt/__init__.py
+openlineage/common/provider/dbt/cloud.py
+openlineage/common/provider/dbt/local.py
+openlineage/common/provider/dbt/processor.py
 openlineage/common/provider/great_expectations/__init__.py
 openlineage/common/provider/great_expectations/action.py
 openlineage/common/provider/great_expectations/facets.py
 openlineage/common/provider/great_expectations/results.py
 openlineage/common/schema/__init__.py
 openlineage/common/sql/__init__.py
-openlineage/common/sql/parser.py
 openlineage_integration_common.egg-info/PKG-INFO
 openlineage_integration_common.egg-info/SOURCES.txt
 openlineage_integration_common.egg-info/dependency_links.txt
 openlineage_integration_common.egg-info/not-zip-safe
 openlineage_integration_common.egg-info/requires.txt
-openlineage_integration_common.egg-info/top_level.txt
+openlineage_integration_common.egg-info/top_level.txt
+tests/test_dataset.py
+tests/test_models.py
+tests/test_snowflake.py
+tests/test_utils.py
```

### Comparing `openlineage-integration-common-0.9.0/openlineage_integration_common.egg-info/requires.txt` & `openlineage-integration-common-1.0.0/openlineage_integration_common.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,80 @@
 attrs>=19.3.0
-openlineage-python==0.9.0
-sqlparse>=0.3.1
+openlineage-python==1.0.0
+openlineage_sql==1.0.0
 
 [bigquery]
 google-api-core>=1.26.3
 google-auth>=1.30.0
-google-cloud-bigquery<3.0.0,>=2.15.0
+google-cloud-bigquery<4.0.0,>=2.15.0
 google-cloud-core>=1.6.0
 google-crc32c>=1.1.2
 
 [dbt]
 dbt-core>=0.20.0
 pyyaml>=5.3.1
 
 [dev]
-jinja2
 google-api-core>=1.26.3
-google-auth>=1.30.0
-dbt-core>=0.20.0
-google-crc32c>=1.1.2
-sqlalchemy>=1.3.24
-pyyaml>=5.3.1
-google-cloud-bigquery<3.0.0,>=2.15.0
-mock
-flake8
-pandas
-python-dateutil
 pytest-cov
-openlineage_sql==0.9.0
 pytest
-great_expectations>=0.13.26
+mypy>=0.960
+boto3>=1.15.0
+types-python-dateutil
+dbt-core>=0.20.0
+google-cloud-bigquery<4.0.0,>=2.15.0
+jinja2
+python-dateutil
+google-auth>=1.30.0
+sqlalchemy<2.0.0,>=1.3.24
+pandas
+great_expectations<0.15.35,>=0.13.26
+ruff
+mock
 google-cloud-core>=1.6.0
+types-PyYAML
+pyyaml>=5.3.1
+google-crc32c>=1.1.2
+pytest-mock
 
 [dev_no_parser]
-jinja2
 google-api-core>=1.26.3
-google-auth>=1.30.0
-dbt-core>=0.20.0
-google-crc32c>=1.1.2
-sqlalchemy>=1.3.24
-pyyaml>=5.3.1
-google-cloud-bigquery<3.0.0,>=2.15.0
-mock
-flake8
-pandas
-python-dateutil
 pytest-cov
 pytest
-great_expectations>=0.13.26
+mypy>=0.960
+boto3>=1.15.0
+types-python-dateutil
+dbt-core>=0.20.0
+google-cloud-bigquery<4.0.0,>=2.15.0
+jinja2
+python-dateutil
+google-auth>=1.30.0
+sqlalchemy<2.0.0,>=1.3.24
+pandas
+great_expectations<0.15.35,>=0.13.26
+ruff
+mock
 google-cloud-core>=1.6.0
+types-PyYAML
+pyyaml>=5.3.1
+google-crc32c>=1.1.2
+pytest-mock
 
 [great_expectations]
-great_expectations>=0.13.26
-sqlalchemy>=1.3.24
+great_expectations<0.15.35,>=0.13.26
+sqlalchemy<2.0.0,>=1.3.24
 
-[sql]
-openlineage_sql==0.9.0
+[redshift]
+boto3>=1.15.0
 
 [tests]
 pytest
 pytest-cov
+pytest-mock
 mock
-flake8
+ruff
 pandas
 jinja2
 python-dateutil
+mypy>=0.960
+types-python-dateutil
+types-PyYAML
```

### Comparing `openlineage-integration-common-0.9.0/setup.py` & `openlineage-integration-common-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 #!/usr/bin/env python
 #
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 #
 # -*- coding: utf-8 -*-
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "0.9.0"
+__version__ = "1.0.0"
 
 requirements = [
     "attrs>=19.3.0",
     f"openlineage-python=={__version__}",
-    "sqlparse>=0.3.1",
+    f"openlineage_sql=={__version__}"
 ]
 
 extras_require = {
-    "sql": [
-        f"openlineage_sql=={__version__}"
-    ],
     "bigquery": [
         "google-api-core>=1.26.3",
         "google-auth>=1.30.0",
-        "google-cloud-bigquery>=2.15.0,<3.0.0",
+        "google-cloud-bigquery>=2.15.0,<4.0.0",
         "google-cloud-core>=1.6.0",
         "google-crc32c>=1.1.2"
     ],
     "dbt": [
         "dbt-core>=0.20.0",
         "pyyaml>=5.3.1"
     ],
     "great_expectations": [
-        "great_expectations>=0.13.26",
-        "sqlalchemy>=1.3.24"
+        "great_expectations>=0.13.26,<0.15.35",
+        "sqlalchemy>=1.3.24,<2.0.0"
+    ],
+    "redshift": [
+        "boto3>=1.15.0"
     ],
     "tests": [
         "pytest",
         "pytest-cov",
+        "pytest-mock",
         "mock",
-        "flake8",
+        "ruff",
         "pandas",
         "jinja2",
         "python-dateutil",
+        "mypy>=0.960",
+        "types-python-dateutil",
+        "types-PyYAML"
     ],
 }
 extras_require["dev"] = set(sum(extras_require.values(), []))
 extras_require["dev_no_parser"] = set(
     sum({
         k: extras_require[k] for k in extras_require.keys() if k not in ["sql", "dev"]
     }.values(), [])
@@ -60,11 +65,11 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     author="OpenLineage",
     packages=find_namespace_packages(include=["openlineage.*"]),
     include_package_data=True,
     install_requires=requirements,
     extras_require=extras_require,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
     keywords="openlineage",
 )
```

