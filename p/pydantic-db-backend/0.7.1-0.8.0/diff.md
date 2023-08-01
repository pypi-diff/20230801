# Comparing `tmp/pydantic_db_backend-0.7.1.tar.gz` & `tmp/pydantic_db_backend-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.7.1.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.8.0.tar", max compression
```

## Comparing `pydantic_db_backend-0.7.1.tar` & `pydantic_db_backend-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.7.1/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     7309 2023-07-19 14:38:49.532351 pydantic_db_backend-0.7.1/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.7.1/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0    10066 2023-07-20 07:18:52.099731 pydantic_db_backend-0.7.1/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.7.1/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      990 2023-07-14 09:23:03.448444 pydantic_db_backend-0.7.1/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      768 2023-07-12 13:44:19.743864 pydantic_db_backend-0.7.1/pydantic_db_backend/indexes.py
--rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.7.1/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      996 2023-07-20 07:27:29.379025 pydantic_db_backend-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     7337 2023-08-01 08:11:56.032146 pydantic_db_backend-0.8.0/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0    10066 2023-08-01 08:06:34.796194 pydantic_db_backend-0.8.0/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0        0 2023-08-01 08:06:34.812194 pydantic_db_backend-0.8.0/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      768 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/indexes.py
+-rw-r--r--   0        0        0     1192 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0     1038 2023-08-01 08:16:59.340250 pydantic_db_backend-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 pydantic_db_backend-0.8.0/PKG-INFO
```

### Comparing `pydantic_db_backend-0.7.1/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.8.0/pydantic_db_backend/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 from contextvars import ContextVar
 from typing import Type, Dict, List, Tuple
 
 from dotenv import load_dotenv
 from pydantic import BaseModel, Field
 
-from pydantic_db_backend.exceptions import IndexNotExisting
+from pydantic_db_backend_exceptions import IndexNotExisting
 from pydantic_db_backend.indexes import Index
 from pydantic_db_backend.utils import uid, utcnow, str_to_datetime_if_parseable
 
 log = logging.getLogger(__name__)
 
 backend_context_var = ContextVar('backend_context_var')
 backend_alias_context_var = ContextVar('backend_alias_context_var', default='default')
@@ -142,19 +142,19 @@
             indexes = cls.create_indexes(model, create_index_kwargs)
             cls._indexes[model] = indexes
         return cls._indexes[model]
 
     @classmethod
     def get_index_by_name(cls, model: Type[BaseModel], name: str) -> Index:
         if model not in cls._indexes:
-            raise IndexNotExisting(model=model, name=name)
+            raise IndexNotExisting(model_name=model.__name__, name=name)
         model_indexes = cls._indexes[model]
         index = next(filter(lambda x: x.name == name, model_indexes), None)
         if index is None:
-            raise IndexNotExisting(model=model, name=name)
+            raise IndexNotExisting(model_name=model.__name__, name=name)
         return index
 
     @classmethod
     def create_indexes(cls, model: Type[BaseModel], create_index_kwargs: dict | None) -> List[Index]:
 
         if not hasattr(model, "Config"):
             return True
```

### Comparing `pydantic_db_backend-0.7.1/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.8.0/pydantic_db_backend/backends/couchdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import pydash
 from couchdb import ResourceConflict, ServerError
 from pydantic import BaseModel, Field
 
 import couchdb
 from pydantic_db_backend.backend import BackendBase, BackendModel
-from pydantic_db_backend.exceptions import RevisionConflict, NotFound, AlreadyExists
+from pydantic_db_backend_exceptions import RevisionConflict, NotFound, AlreadyExists
 from pydantic_db_backend.indexes import Index, SortingIndex, AggregationIndex
 from pydantic_db_backend.utils import CustomJSONEncoder
 
 log = logging.getLogger(__name__)
 
 
 class CouchDbBackend(BackendBase):
```

### Comparing `pydantic_db_backend-0.7.1/pydantic_db_backend/indexes.py` & `pydantic_db_backend-0.8.0/pydantic_db_backend/indexes.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.7.1/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.8.0/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.7.1/pyproject.toml` & `pydantic_db_backend-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.7.1"
+version = "0.8.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.15.0"
 couchdb = { version = "^1.2", optional = true }
 pymongo = { version = "^3.13.0", optional = true }
 pydash = "*"
 iso8601 = "^1.1.0"
 pydantic = "^1.10.7"
 webexception = "^1.0.4"
+pydantic-db-backend-exceptions = "^1.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.7"
 pytest = "^7.3.1"
 freezegun = "^1.2.2"
 couchdb = "^1.2"
```

### Comparing `pydantic_db_backend-0.7.1/PKG-INFO` & `pydantic_db_backend-0.8.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.7.1
+Version: 0.8.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
 Provides-Extra: mongodb
 Requires-Dist: couchdb (>=1.2,<2.0) ; extra == "couchdb"
 Requires-Dist: iso8601 (>=1.1.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic-db-backend-exceptions (>=1.0.0,<2.0.0)
 Requires-Dist: pydash
 Requires-Dist: pymongo (>=3.13.0,<4.0.0) ; extra == "mongodb"
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: webexception (>=1.0.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Testing
```

