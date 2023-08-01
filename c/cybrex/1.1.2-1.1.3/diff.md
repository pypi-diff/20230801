# Comparing `tmp/cybrex-1.1.2.tar.gz` & `tmp/cybrex-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.1.2.tar", last modified: Tue Aug  1 19:52:16 2023, max compression
+gzip compressed data, was "cybrex-1.1.3.tar", last modified: Tue Aug  1 19:58:06 2023, max compression
```

## Comparing `cybrex-1.1.2.tar` & `cybrex-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:52:16.888172 cybrex-1.1.2/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.2/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 19:52:16.887852 cybrex-1.1.2/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.2/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:52:16.885432 cybrex-1.1.2/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.2/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5636 2023-08-01 19:14:39.000000 cybrex-1.1.2/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11690 2023-08-01 19:12:09.000000 cybrex-1.1.2/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13594 2023-08-01 18:15:58.000000 cybrex-1.1.2/cybrex/models.py
--rw-r--r--   0 pasha      (501) staff       (20)    13911 2023-08-01 13:45:04.000000 cybrex-1.1.2/cybrex/test.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:52:16.887380 cybrex-1.1.2/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      320 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      204 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 19:51:49.000000 cybrex-1.1.2/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      204 2023-08-01 19:51:35.000000 cybrex-1.1.2/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 19:52:16.888273 cybrex-1.1.2/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:58:06.694486 cybrex-1.1.3/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.3/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 19:58:06.694137 cybrex-1.1.3/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.3/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:58:06.691311 cybrex-1.1.3/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.3/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 19:57:30.000000 cybrex-1.1.3/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    11678 2023-08-01 19:57:40.000000 cybrex-1.1.3/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.3/cybrex/models.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13911 2023-08-01 13:45:04.000000 cybrex-1.1.3/cybrex/test.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:58:06.693571 cybrex-1.1.3/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      320 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      204 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 19:58:06.000000 cybrex-1.1.3/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 19:57:48.000000 cybrex-1.1.3/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      204 2023-08-01 19:51:35.000000 cybrex-1.1.3/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 19:58:06.694630 cybrex-1.1.3/setup.cfg
```

### Comparing `cybrex-1.1.2/PKG-INFO` & `cybrex-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.2
+Version: 1.1.3
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.2/README.md` & `cybrex-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.2/cybrex/cli.py` & `cybrex-1.1.3/cybrex/cli.py`

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

### Comparing `cybrex-1.1.2/cybrex/cybrex_ai.py` & `cybrex-1.1.3/cybrex/cybrex_ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 import base64
 import io
 import json
 import logging
 import os.path
 import uuid
 from gzip import GzipFile
-from typing import (
-    List,
-    Optional,
-)
+from typing import List, Optional
 
 import chromadb
 import numpy as np
 import pypdf
 import yaml
 from aiokit import AioThing
 from bs4 import BeautifulSoup
@@ -21,15 +18,15 @@
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

### Comparing `cybrex-1.1.2/cybrex/models.py` & `cybrex-1.1.3/cybrex/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import logging
 from collections import OrderedDict
 from typing import List
 
 from ctransformers import AutoModelForCausalLM
 from keybert import KeyBERT
-from langchain import (
-    OpenAI,
-)
-from langchain.embeddings import (
-    OpenAIEmbeddings, HuggingFaceInstructEmbeddings,
-)
+from langchain import OpenAI
+from langchain.embeddings import HuggingFaceInstructEmbeddings, OpenAIEmbeddings
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from lazy import lazy
 
 
 class BasePrompter:
     @staticmethod
     def prompter_from_type(type_):
```

### Comparing `cybrex-1.1.2/cybrex/test.py` & `cybrex-1.1.3/cybrex/test.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.2/cybrex.egg-info/PKG-INFO` & `cybrex-1.1.3/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.2
+Version: 1.1.3
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.2/pyproject.toml` & `cybrex-1.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.1.2"
+version = "1.1.3"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

