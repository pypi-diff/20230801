# Comparing `tmp/cybrex-1.1.7.tar.gz` & `tmp/cybrex-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.1.7.tar", last modified: Tue Aug  1 20:46:17 2023, max compression
+gzip compressed data, was "cybrex-1.1.8.tar", last modified: Tue Aug  1 21:12:30 2023, max compression
```

## Comparing `cybrex-1.1.7.tar` & `cybrex-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:46:17.889213 cybrex-1.1.7/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.7/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:46:17.888766 cybrex-1.1.7/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.7/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:46:17.884742 cybrex-1.1.7/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.7/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5636 2023-08-01 20:40:01.000000 cybrex-1.1.7/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11974 2023-08-01 20:45:51.000000 cybrex-1.1.7/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.7/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:46:17.887691 cybrex-1.1.7/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 20:45:51.000000 cybrex-1.1.7/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:22:19.000000 cybrex-1.1.7/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 20:46:17.889380 cybrex-1.1.7/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 21:12:30.302073 cybrex-1.1.8/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.8/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 21:12:30.301526 cybrex-1.1.8/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.8/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 21:12:30.298789 cybrex-1.1.8/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.8/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 21:12:18.000000 cybrex-1.1.8/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    11975 2023-08-01 21:12:18.000000 cybrex-1.1.8/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.8/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 21:12:30.300902 cybrex-1.1.8/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 21:12:18.000000 cybrex-1.1.8/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:22:19.000000 cybrex-1.1.8/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 21:12:30.302282 cybrex-1.1.8/setup.cfg
```

### Comparing `cybrex-1.1.7/PKG-INFO` & `cybrex-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.7
+Version: 1.1.8
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.7/README.md` & `cybrex-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.7/cybrex/cli.py` & `cybrex-1.1.8/cybrex/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import sys
 import textwrap
 
 import fire
 from termcolor import colored
 
-from cybrex_ai import CybrexAI
+from .cybrex_ai import CybrexAI
 
 
 def create_snippet(document):
     return document['metadata']['doi'] + ': ' + document['text']
 
 
 class CybrexCli:
```

### Comparing `cybrex-1.1.7/cybrex/cybrex_ai.py` & `cybrex-1.1.8/cybrex/cybrex_ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from izihawa_utils.exceptions import BaseError
 from izihawa_utils.file import mkdir_p
 from langchain.chains.summarize import load_summarize_chain
 from langchain.schema import Document
 from stc_geck.advices import get_documents_on_topic
 from stc_geck.client import StcGeck
 
-from models import CybrexModel
+from .models import CybrexModel
 
 
 class DocumentNotFoundError(BaseError):
     pass
 
 
 def print_color(text, color):
```

### Comparing `cybrex-1.1.7/cybrex/models.py` & `cybrex-1.1.8/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.7/cybrex.egg-info/PKG-INFO` & `cybrex-1.1.8/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.7
+Version: 1.1.8
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.7/pyproject.toml` & `cybrex-1.1.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.1.7"
+version = "1.1.8"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

