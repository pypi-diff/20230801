# Comparing `tmp/streaminghub-pydfds-0.1.19.tar.gz` & `tmp/streaminghub-pydfds-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaminghub-pydfds-0.1.19.tar", last modified: Mon Jul 31 20:58:25 2023, max compression
+gzip compressed data, was "streaminghub-pydfds-0.1.20.tar", last modified: Tue Aug  1 05:02:52 2023, max compression
```

## Comparing `streaminghub-pydfds-0.1.19.tar` & `streaminghub-pydfds-0.1.20.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.658470 streaminghub-pydfds-0.1.19/
--rw-r--r--   0 yasith     (501) staff       (20)     2110 2023-07-31 20:58:25.658335 streaminghub-pydfds-0.1.19/PKG-INFO
--rw-r--r--   0 yasith     (501) staff       (20)     1583 2023-07-31 20:58:11.000000 streaminghub-pydfds-0.1.19/README.md
--rwxr-xr-x   0 yasith     (501) staff       (20)     1258 2023-07-31 20:58:11.000000 streaminghub-pydfds-0.1.19/pyproject.toml
--rw-r--r--   0 yasith     (501) staff       (20)       38 2023-07-31 20:58:25.658509 streaminghub-pydfds-0.1.19/setup.cfg
-drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.656634 streaminghub-pydfds-0.1.19/src/
-drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.657391 streaminghub-pydfds-0.1.19/src/dfds/
--rw-r--r--   0 yasith     (501) staff       (20)       58 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/src/dfds/__init__.py
--rw-r--r--   0 yasith     (501) staff       (20)     2692 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/src/dfds/lsl.py
--rw-r--r--   0 yasith     (501) staff       (20)     5752 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/src/dfds/parser.py
--rwxr-xr-x   0 yasith     (501) staff       (20)     4670 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/src/dfds/typing.py
-drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.658003 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/
--rw-r--r--   0 yasith     (501) staff       (20)     2110 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/PKG-INFO
--rw-r--r--   0 yasith     (501) staff       (20)      354 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/SOURCES.txt
--rw-r--r--   0 yasith     (501) staff       (20)        1 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/dependency_links.txt
--rw-r--r--   0 yasith     (501) staff       (20)      145 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/requires.txt
--rw-r--r--   0 yasith     (501) staff       (20)        5 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/top_level.txt
-drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.658145 streaminghub-pydfds-0.1.19/tests/
--rwxr-xr-x   0 yasith     (501) staff       (20)      596 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/tests/test_parser.py
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-08-01 05:02:52.980630 streaminghub-pydfds-0.1.20/
+-rw-r--r--   0 yasith     (501) staff       (20)     2110 2023-08-01 05:02:52.980494 streaminghub-pydfds-0.1.20/PKG-INFO
+-rw-r--r--   0 yasith     (501) staff       (20)     1583 2023-08-01 05:02:49.000000 streaminghub-pydfds-0.1.20/README.md
+-rwxr-xr-x   0 yasith     (501) staff       (20)     1258 2023-08-01 05:02:49.000000 streaminghub-pydfds-0.1.20/pyproject.toml
+-rw-r--r--   0 yasith     (501) staff       (20)       38 2023-08-01 05:02:52.980671 streaminghub-pydfds-0.1.20/setup.cfg
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-08-01 05:02:52.977342 streaminghub-pydfds-0.1.20/src/
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-08-01 05:02:52.979183 streaminghub-pydfds-0.1.20/src/dfds/
+-rw-r--r--   0 yasith     (501) staff       (20)       58 2023-07-31 22:58:21.000000 streaminghub-pydfds-0.1.20/src/dfds/__init__.py
+-rw-r--r--   0 yasith     (501) staff       (20)      993 2023-08-01 04:46:31.000000 streaminghub-pydfds-0.1.20/src/dfds/loader.py
+-rw-r--r--   0 yasith     (501) staff       (20)     2692 2023-07-31 22:59:32.000000 streaminghub-pydfds-0.1.20/src/dfds/lsl.py
+-rw-r--r--   0 yasith     (501) staff       (20)     3651 2023-08-01 04:49:46.000000 streaminghub-pydfds-0.1.20/src/dfds/parser.py
+-rwxr-xr-x   0 yasith     (501) staff       (20)     4678 2023-08-01 04:58:40.000000 streaminghub-pydfds-0.1.20/src/dfds/typing.py
+-rw-r--r--   0 yasith     (501) staff       (20)     2627 2023-08-01 04:52:37.000000 streaminghub-pydfds-0.1.20/src/dfds/url.py
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-08-01 05:02:52.979960 streaminghub-pydfds-0.1.20/src/streaminghub_pydfds.egg-info/
+-rw-r--r--   0 yasith     (501) staff       (20)     2110 2023-08-01 05:02:52.000000 streaminghub-pydfds-0.1.20/src/streaminghub_pydfds.egg-info/PKG-INFO
+-rw-r--r--   0 yasith     (501) staff       (20)      408 2023-08-01 05:02:52.000000 streaminghub-pydfds-0.1.20/src/streaminghub_pydfds.egg-info/SOURCES.txt
+-rw-r--r--   0 yasith     (501) staff       (20)        1 2023-08-01 05:02:52.000000 streaminghub-pydfds-0.1.20/src/streaminghub_pydfds.egg-info/dependency_links.txt
+-rw-r--r--   0 yasith     (501) staff       (20)      145 2023-08-01 05:02:52.000000 streaminghub-pydfds-0.1.20/src/streaminghub_pydfds.egg-info/requires.txt
+-rw-r--r--   0 yasith     (501) staff       (20)        5 2023-08-01 05:02:52.000000 streaminghub-pydfds-0.1.20/src/streaminghub_pydfds.egg-info/top_level.txt
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-08-01 05:02:52.980260 streaminghub-pydfds-0.1.20/tests/
+-rwxr-xr-x   0 yasith     (501) staff       (20)      596 2023-08-01 04:53:00.000000 streaminghub-pydfds-0.1.20/tests/test_parser.py
+-rw-r--r--   0 yasith     (501) staff       (20)     1449 2023-08-01 04:53:06.000000 streaminghub-pydfds-0.1.20/tests/test_path.py
```

### Comparing `streaminghub-pydfds-0.1.19/PKG-INFO` & `streaminghub-pydfds-0.1.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaminghub-pydfds
-Version: 0.1.19
+Version: 0.1.20
 Summary: Parser for Data Flow Description Schema (DFDS) metadata
 Author-email: Yasith Jayawardana <yasith@cs.odu.edu>
 Project-URL: homepage, https://github.com/nirdslab/streaminghub/tree/master/pydfds
 Keywords: dfds,metadata,parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 PyDFDS is a parser for Data Flow Description Schema (DFDS) metadata, written using Python.
 
 ## Installation
 
 ```bash
 
-pip install streaminghub-pydfds==0.1.19
+pip install streaminghub-pydfds==0.1.20
 
 ```
 
 ## Usage
 
 ```python
```

### Comparing `streaminghub-pydfds-0.1.19/README.md` & `streaminghub-pydfds-0.1.20/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 PyDFDS is a parser for Data Flow Description Schema (DFDS) metadata, written using Python.
 
 ## Installation
 
 ```bash
 
-pip install streaminghub-pydfds==0.1.19
+pip install streaminghub-pydfds==0.1.20
 
 ```
 
 ## Usage
 
 ```python
```

### Comparing `streaminghub-pydfds-0.1.19/pyproject.toml` & `streaminghub-pydfds-0.1.20/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streaminghub-pydfds"
-version = "0.1.19"
+version = "0.1.20"
 authors = [{ name = "Yasith Jayawardana", email = "yasith@cs.odu.edu" }]
 description = "Parser for Data Flow Description Schema (DFDS) metadata"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["dfds", "metadata", "parser"]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -27,15 +27,15 @@
 [project.urls]
 homepage = "https://github.com/nirdslab/streaminghub/tree/master/pydfds"
 
 [project.optional-dependencies]
 dev = ["black", "build", "twine", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.1.19"
+current_version = "0.1.20"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump pydfds version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
```

### Comparing `streaminghub-pydfds-0.1.19/src/dfds/lsl.py` & `streaminghub-pydfds-0.1.20/src/dfds/lsl.py`

 * *Files identical despite different names*

### Comparing `streaminghub-pydfds-0.1.19/src/dfds/typing.py` & `streaminghub-pydfds-0.1.20/src/dfds/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import itertools
-import os
 from collections import OrderedDict
 from typing import List, Optional, Tuple
 
 import h5py
 import numpy as np
 import parse
 import pydantic as p
@@ -69,15 +68,15 @@
 class Node(p.BaseModel):
     device: Optional[Device] = p.Field(default=None)
     uri: Optional[str] = p.Field(default=None)
     inputs: OrderedDict[str, Stream] = p.Field(default=OrderedDict())
     outputs: OrderedDict[str, Stream] = p.Field(default=OrderedDict())
 
 
-Stream.update_forward_refs()
+Stream.model_rebuild()
 
 
 class Author(p.BaseModel):
     name: str
     affiliation: str
     email: str
 
@@ -120,15 +119,17 @@
     def __init__(
         self,
         collection: Collection,
     ) -> None:
         super().__init__()
         self.__collection = collection
         self.__parser = parse.compile(self.__collection.pattern)
-        base_dir = os.getenv("DATA_DIR")
+
+        import os
+        base_dir = os.getenv("SHUB_DATA_DIR")
         assert base_dir
         self.__fpath = os.path.join(base_dir, self.__collection.name, "data.h5")
         assert os.path.isfile(self.__fpath)
 
     def ls(
         self,
     ) -> List[OrderedDict[str, str]]:
```

### Comparing `streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/PKG-INFO` & `streaminghub-pydfds-0.1.20/src/streaminghub_pydfds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaminghub-pydfds
-Version: 0.1.19
+Version: 0.1.20
 Summary: Parser for Data Flow Description Schema (DFDS) metadata
 Author-email: Yasith Jayawardana <yasith@cs.odu.edu>
 Project-URL: homepage, https://github.com/nirdslab/streaminghub/tree/master/pydfds
 Keywords: dfds,metadata,parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 PyDFDS is a parser for Data Flow Description Schema (DFDS) metadata, written using Python.
 
 ## Installation
 
 ```bash
 
-pip install streaminghub-pydfds==0.1.19
+pip install streaminghub-pydfds==0.1.20
 
 ```
 
 ## Usage
 
 ```python
```

### Comparing `streaminghub-pydfds-0.1.19/tests/test_parser.py` & `streaminghub-pydfds-0.1.20/tests/test_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 import dfds
 
 if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
+    logging.basicConfig(level=logging.INFO)
+
     parser = dfds.Parser()
     collection = parser.get_collection_metadata("repository/adhd_sin.collection.json")
 
     for group in collection.iterate_groups():
         for stream_id, stream in collection.streams.items():
             print(stream_id, dict(group))
```

