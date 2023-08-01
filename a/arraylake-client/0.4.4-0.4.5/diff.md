# Comparing `tmp/arraylake_client-0.4.4.tar.gz` & `tmp/arraylake_client-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraylake_client-0.4.4.tar", max compression
+gzip compressed data, was "arraylake_client-0.4.5.tar", max compression
```

## Comparing `arraylake_client-0.4.4.tar` & `arraylake_client-0.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      613 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/README.md
--rw-r--r--   0        0        0      357 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/__init__.py
--rw-r--r--   0        0        0       70 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/__main__.py
--rw-r--r--   0        0        0    15553 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/api_utils.py
--rw-r--r--   0        0        0     2381 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/async_utils.py
--rw-r--r--   0        0        0      630 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/chunkstore/__init__.py
--rw-r--r--   0        0        0     1534 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/chunkstore/abc.py
--rw-r--r--   0        0        0     5201 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/chunkstore/s3chunkstore.py
--rw-r--r--   0        0        0        0 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/__init__.py
--rw-r--r--   0        0        0     3973 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/auth.py
--rw-r--r--   0        0        0     4762 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/config.py
--rw-r--r--   0        0        0     1155 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/main.py
--rw-r--r--   0        0        0     3568 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/repo.py
--rw-r--r--   0        0        0     3390 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/cli/utils.py
--rw-r--r--   0        0        0     7778 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/client.py
--rw-r--r--   0        0        0     7098 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/commits.py
--rw-r--r--   0        0        0      538 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/config.py
--rw-r--r--   0        0        0      105 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/config.yaml
--rw-r--r--   0        0        0      192 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/exceptions.py
--rw-r--r--   0        0        0     1110 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/log_util.py
--rw-r--r--   0        0        0      282 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/metastore/__init__.py
--rw-r--r--   0        0        0     8943 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/metastore/abc.py
--rw-r--r--   0        0        0    13035 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/metastore/http_metastore.py
--rw-r--r--   0        0        0    53388 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/repo.py
--rw-r--r--   0        0        0     1227 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/spec.py
--rw-r--r--   0        0        0     4550 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/token.py
--rw-r--r--   0        0        0     9753 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/types.py
--rw-r--r--   0        0        0    10315 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/virtual.py
--rw-r--r--   0        0        0      851 2023-07-19 00:27:10.899278 arraylake_client-0.4.4/arraylake_client/zarr_util.py
--rw-r--r--   0        0        0     2337 2023-07-19 00:27:47.453407 arraylake_client-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 arraylake_client-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      613 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/README.md
+-rw-r--r--   0        0        0      357 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/__main__.py
+-rw-r--r--   0        0        0    15553 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/api_utils.py
+-rw-r--r--   0        0        0     2381 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/async_utils.py
+-rw-r--r--   0        0        0      630 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/chunkstore/__init__.py
+-rw-r--r--   0        0        0     1534 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/chunkstore/abc.py
+-rw-r--r--   0        0        0     5201 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/chunkstore/s3chunkstore.py
+-rw-r--r--   0        0        0        0 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/cli/__init__.py
+-rw-r--r--   0        0        0     3973 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/cli/auth.py
+-rw-r--r--   0        0        0     4762 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/cli/config.py
+-rw-r--r--   0        0        0     1155 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/cli/main.py
+-rw-r--r--   0        0        0     3568 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/cli/repo.py
+-rw-r--r--   0        0        0     3390 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/cli/utils.py
+-rw-r--r--   0        0        0     7778 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/client.py
+-rw-r--r--   0        0        0     7199 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/commits.py
+-rw-r--r--   0        0        0      538 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/config.py
+-rw-r--r--   0        0        0      105 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/config.yaml
+-rw-r--r--   0        0        0      244 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/exceptions.py
+-rw-r--r--   0        0        0     1110 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/log_util.py
+-rw-r--r--   0        0        0      282 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/metastore/__init__.py
+-rw-r--r--   0        0        0     8943 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/metastore/abc.py
+-rw-r--r--   0        0        0    13035 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/metastore/http_metastore.py
+-rw-r--r--   0        0        0    53388 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/repo.py
+-rw-r--r--   0        0        0     1227 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/spec.py
+-rw-r--r--   0        0        0     4550 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/token.py
+-rw-r--r--   0        0        0     9768 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/types.py
+-rw-r--r--   0        0        0    10315 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/virtual.py
+-rw-r--r--   0        0        0      851 2023-08-01 02:11:28.070194 arraylake_client-0.4.5/arraylake_client/zarr_util.py
+-rw-r--r--   0        0        0     2362 2023-08-01 02:12:01.426288 arraylake_client-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1995 1970-01-01 00:00:00.000000 arraylake_client-0.4.5/PKG-INFO
```

### Comparing `arraylake_client-0.4.4/README.md` & `arraylake_client-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/api_utils.py` & `arraylake_client-0.4.5/arraylake_client/api_utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/async_utils.py` & `arraylake_client-0.4.5/arraylake_client/async_utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/chunkstore/__init__.py` & `arraylake_client-0.4.5/arraylake_client/chunkstore/__init__.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/chunkstore/abc.py` & `arraylake_client-0.4.5/arraylake_client/chunkstore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/chunkstore/s3chunkstore.py` & `arraylake_client-0.4.5/arraylake_client/chunkstore/s3chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/cli/auth.py` & `arraylake_client-0.4.5/arraylake_client/cli/auth.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/cli/config.py` & `arraylake_client-0.4.5/arraylake_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/cli/main.py` & `arraylake_client-0.4.5/arraylake_client/cli/main.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/cli/repo.py` & `arraylake_client-0.4.5/arraylake_client/cli/repo.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/cli/utils.py` & `arraylake_client-0.4.5/arraylake_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/client.py` & `arraylake_client-0.4.5/arraylake_client/client.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/commits.py` & `arraylake_client-0.4.5/arraylake_client/commits.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dataclasses import dataclass
 from html import escape
 from typing import Mapping, Optional, Sequence, Tuple, TypeVar
 
 from bson.errors import InvalidId
 
-from arraylake_client.exceptions import DocumentNotFoundError
+from arraylake_client.exceptions import CommitNotFoundException, DocumentNotFoundError
 from arraylake_client.types import (
     Branch,
     BranchName,
     Commit,
     CommitHistory,
     CommitID,
     DocResponse,
@@ -60,22 +60,24 @@
     all_commits: Mapping[CommitID, Commit]
 
     def walk(self) -> CommitHistory:
         "Construct the lineage for the provided commit_id over provided commits"
         try:
             commit = self.all_commits[self.commit_id]
         except KeyError:
-            raise KeyError(f"Error retrieving commit id {self.commit_id}, root does not exist in provided commits")
+            raise CommitNotFoundException(f"Error retrieving commit id {self.commit_id}, root does not exist in provided commits")
         while commit:
             yield (commit.id, commit.session_id)
             if commit.parent_commit:
                 try:
                     commit = self.all_commits[commit.parent_commit]
                 except KeyError:
-                    raise KeyError(f"Error retrieving commit id {commit.parent_commit}, parent does not exist in provided commits")
+                    raise CommitNotFoundException(
+                        f"Error retrieving commit id {commit.parent_commit}, parent does not exist in provided commits"
+                    )
             else:
                 commit = None
 
 
 class CommitData:
     """Data structure containing all the commit information for a session."""
```

### Comparing `arraylake_client-0.4.4/arraylake_client/config.py` & `arraylake_client-0.4.5/arraylake_client/config.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/log_util.py` & `arraylake_client-0.4.5/arraylake_client/log_util.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/metastore/abc.py` & `arraylake_client-0.4.5/arraylake_client/metastore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/metastore/http_metastore.py` & `arraylake_client-0.4.5/arraylake_client/metastore/http_metastore.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/repo.py` & `arraylake_client-0.4.5/arraylake_client/repo.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/spec.py` & `arraylake_client-0.4.5/arraylake_client/spec.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/token.py` & `arraylake_client-0.4.5/arraylake_client/token.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/types.py` & `arraylake_client-0.4.5/arraylake_client/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     total_chunk_bytes: int
 
 
 class Array(BaseModel):
     attributes: Dict[str, Any] = {}
     chunk_grid: Dict[str, Any] = {}
     chunk_memory_layout: str = None
-    compressor: Dict[str, Any] = {}
+    compressor: Union[Dict[str, Any], None] = None
     data_type: Union[str, Dict[str, Any]] = None
     fill_value: Any = None
     extensions: list = []
     shape: Tuple[int, ...] = None
 
 
 # Utility to coerce Array data types to string version
```

### Comparing `arraylake_client-0.4.4/arraylake_client/virtual.py` & `arraylake_client-0.4.5/arraylake_client/virtual.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/arraylake_client/zarr_util.py` & `arraylake_client-0.4.5/arraylake_client/zarr_util.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.4/pyproject.toml` & `arraylake_client-0.4.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "arraylake-client"
-version = "0.4.4"  # placeholder
+version = "0.4.5"  # placeholder
 description = "Python client for ArrayLake"
 authors = ["Joe Hamman <joe@earthmover.io>"]
 readme = "README.md"
 packages = [{include = "arraylake_client"}]
 
 [tool.poetry-dynamic-versioning]
 enable = false
@@ -16,15 +16,15 @@
 style = "pep440"
 strict = true
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 aiobotocore = { version = "^2.4.0", extras = ["boto3"]}
 types-aiobotocore = "^2.4.0"
-anyio = "^3.6.1"
+anyio = "3.7.0"
 zarr = ">=2.14,<2.15"
 numpy = "^1.20"
 donfig = ">=0.7,<1.0"
 pydantic = {extras = ["email"], version = "^1.10"}
 httpx = ">=0.23.0,<1.0"
 pymongo = { version = "^4.2.0"}
 ruamel-yaml = { version = ">=0.17,<1.0", optional = true }
@@ -48,14 +48,15 @@
 xarray = ">=2022.12.0"
 pandas = "^1.3"
 dask = "^2022.10.2"
 distributed = "^2022.10.2"
 respx = "^0.20.1"
 scipy = "^1.10.1"
 arraylake-mongo-metastore = {path = "../mongo-metastore", develop = true}
+pytest-timeout = "^2.1.0"
 
 [tool.poetry.scripts]
 arraylake = 'arraylake_client.cli.main:app'
 
 [tool.poetry.extras]
 cli = ["ruamel-yaml", "typer", "rich"]
 virtual = ["fsspec", "kerchunk", "h5py", "s3fs"]
```

### Comparing `arraylake_client-0.4.4/PKG-INFO` & `arraylake_client-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: arraylake-client
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python client for ArrayLake
 Author: Joe Hamman
 Author-email: joe@earthmover.io
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cli
 Provides-Extra: virtual
 Provides-Extra: widgets
 Requires-Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0)
-Requires-Dist: anyio (>=3.6.1,<4.0.0)
+Requires-Dist: anyio (==3.7.0)
 Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: donfig (>=0.7,<1.0)
 Requires-Dist: fsspec (>=2022.11.0) ; extra == "virtual"
 Requires-Dist: h5py (>=3.7.0,<4.0.0) ; extra == "virtual"
 Requires-Dist: httpx (>=0.23.0,<1.0)
 Requires-Dist: ipytree (>=0.2.2,<1.0) ; extra == "widgets"
 Requires-Dist: kerchunk (>=0.1,<1.0) ; extra == "virtual"
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: arraylake-client Version: 0.4.4 Summary: Python
+Metadata-Version: 2.1 Name: arraylake-client Version: 0.4.5 Summary: Python
 client for ArrayLake Author: Joe Hamman Author-email: joe@earthmover.io
 Requires-Python: >=3.8,<3.11 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cli Provides-Extra: virtual Provides-Extra: widgets Requires-
-Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist: anyio (>=3.6.1,<4.0.0)
+Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist: anyio (==3.7.0)
 Requires-Dist: cachetools (>=5.3.0,<6.0.0) Requires-Dist: donfig (>=0.7,<1.0)
 Requires-Dist: fsspec (>=2022.11.0) ; extra == "virtual" Requires-Dist: h5py
 (>=3.7.0,<4.0.0) ; extra == "virtual" Requires-Dist: httpx (>=0.23.0,<1.0)
 Requires-Dist: ipytree (>=0.2.2,<1.0) ; extra == "widgets" Requires-Dist:
 kerchunk (>=0.1,<1.0) ; extra == "virtual" Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: pydantic[email] (>=1.10,<2.0) Requires-Dist: pymongo
 (>=4.2.0,<5.0.0) Requires-Dist: rich (>=12.6,<14.0) ; extra == "cli" Requires-
```

