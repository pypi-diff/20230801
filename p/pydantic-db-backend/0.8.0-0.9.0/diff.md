# Comparing `tmp/pydantic_db_backend-0.8.0.tar.gz` & `tmp/pydantic_db_backend-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.8.0.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.9.0.tar", max compression
```

## Comparing `pydantic_db_backend-0.8.0.tar` & `pydantic_db_backend-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0       87 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     7337 2023-08-01 08:11:56.032146 pydantic_db_backend-0.8.0/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0    10066 2023-08-01 08:06:34.796194 pydantic_db_backend-0.8.0/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0        0 2023-08-01 08:06:34.812194 pydantic_db_backend-0.8.0/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      768 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/indexes.py
--rw-r--r--   0        0        0     1192 2023-08-01 07:56:20.200003 pydantic_db_backend-0.8.0/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0     1038 2023-08-01 08:16:59.340250 pydantic_db_backend-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 pydantic_db_backend-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-08-01 07:56:20.200003 pydantic_db_backend-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 07:56:20.200003 pydantic_db_backend-0.9.0/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     6852 2023-08-01 11:29:15.007159 pydantic_db_backend-0.9.0/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-08-01 07:56:20.200003 pydantic_db_backend-0.9.0/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0    10120 2023-08-01 11:30:31.106487 pydantic_db_backend-0.9.0/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-08-01 07:56:20.200003 pydantic_db_backend-0.9.0/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      768 2023-08-01 07:56:20.200003 pydantic_db_backend-0.9.0/pydantic_db_backend/indexes.py
+-rw-r--r--   0        0        0     1192 2023-08-01 07:56:20.200003 pydantic_db_backend-0.9.0/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0     1034 2023-08-01 11:35:46.340490 pydantic_db_backend-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 pydantic_db_backend-0.9.0/PKG-INFO
```

### Comparing `pydantic_db_backend-0.8.0/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.9.0/pydantic_db_backend/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,30 @@
 from __future__ import annotations
 
 import contextlib
-import datetime
 import json
 import logging
 import re
 from contextvars import ContextVar
 from typing import Type, Dict, List, Tuple
 
 from dotenv import load_dotenv
-from pydantic import BaseModel, Field
+from pydantic import BaseModel
 
-from pydantic_db_backend_exceptions import IndexNotExisting
 from pydantic_db_backend.indexes import Index
-from pydantic_db_backend.utils import uid, utcnow, str_to_datetime_if_parseable
+from pydantic_db_backend.utils import uid, utcnow
+from pydantic_db_backend_common.exceptions import IndexNotExisting
+from pydantic_db_backend_common.pydantic import BackendModel
 
 log = logging.getLogger(__name__)
 
 backend_context_var = ContextVar('backend_context_var')
 backend_alias_context_var = ContextVar('backend_alias_context_var', default='default')
 
 
-class BackendModel(BaseModel):
-    uid: str | None = Field(default_factory=uid)
-    revision: str | None = None
-    version: int | None = 1
-    created_time: datetime.datetime | None = Field(default_factory=utcnow)
-    updated_time: datetime.datetime | None = Field(default_factory=utcnow)
-
-    class Config:
-        json_encoders = {
-            datetime.datetime: lambda x: x.isoformat(),
-        }
-        json_decoders = {
-            datetime.datetime: str_to_datetime_if_parseable,
-        }
-
-
 class Backend(object):
     @staticmethod
     @contextlib.contextmanager
     def provider(backend: Type[BackendBase]):
         token = backend_context_var.set(backend)
         yield backend
         backend_context_var.reset(token)
```

### Comparing `pydantic_db_backend-0.8.0/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.9.0/pydantic_db_backend/backends/couchdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from typing import Dict, Type, List, Tuple, Callable, Any
 
 import pydash
 from couchdb import ResourceConflict, ServerError
 from pydantic import BaseModel, Field
 
 import couchdb
-from pydantic_db_backend.backend import BackendBase, BackendModel
-from pydantic_db_backend_exceptions import RevisionConflict, NotFound, AlreadyExists
+from pydantic_db_backend.backend import BackendBase
+from pydantic_db_backend_common.exceptions import NotFound, AlreadyExists, RevisionConflict
+from pydantic_db_backend_common.pydantic import BackendModel
 from pydantic_db_backend.indexes import Index, SortingIndex, AggregationIndex
 from pydantic_db_backend.utils import CustomJSONEncoder
 
 log = logging.getLogger(__name__)
 
 
 class CouchDbBackend(BackendBase):
```

### Comparing `pydantic_db_backend-0.8.0/pydantic_db_backend/indexes.py` & `pydantic_db_backend-0.9.0/pydantic_db_backend/indexes.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.8.0/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.9.0/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.8.0/pyproject.toml` & `pydantic_db_backend-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.8.0"
+version = "0.9.0"
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
-pydantic-db-backend-exceptions = "^1.0.0"
+pydantic-db-backend-common = "^1.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.7"
 pytest = "^7.3.1"
 freezegun = "^1.2.2"
 couchdb = "^1.2"
```

### Comparing `pydantic_db_backend-0.8.0/PKG-INFO` & `pydantic_db_backend-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.8.0
+Version: 0.9.0
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
-Requires-Dist: pydantic-db-backend-exceptions (>=1.0.0,<2.0.0)
+Requires-Dist: pydantic-db-backend-common (>=1.0.1,<2.0.0)
 Requires-Dist: pydash
 Requires-Dist: pymongo (>=3.13.0,<4.0.0) ; extra == "mongodb"
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: webexception (>=1.0.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Testing
```

