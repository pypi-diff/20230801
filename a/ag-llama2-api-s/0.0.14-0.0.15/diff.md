# Comparing `tmp/ag_llama2_api_s-0.0.14.tar.gz` & `tmp/ag_llama2_api_s-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama2_api_s-0.0.14.tar", last modified: Tue Aug  1 15:09:06 2023, max compression
+gzip compressed data, was "dist\ag_llama2_api_s-0.0.15.tar", last modified: Tue Aug  1 15:10:38 2023, max compression
```

## Comparing `ag_llama2_api_s-0.0.14.tar` & `ag_llama2_api_s-0.0.15.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 15:09:06.740889 ag_llama2_api_s-0.0.14/
--rw-rw-rw-   0        0        0      771 2023-08-01 15:09:06.738894 ag_llama2_api_s-0.0.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 15:09:06.717950 ag_llama2_api_s-0.0.14/ag_llama2_api_s/
--rw-rw-rw-   0        0        0     2190 2023-08-01 15:06:03.000000 ag_llama2_api_s-0.0.14/ag_llama2_api_s/__init__.py
--rw-rw-rw-   0        0        0     8785 2023-07-27 11:11:47.000000 ag_llama2_api_s-0.0.14/ag_llama2_api_s/__main__.py
--rw-rw-rw-   0        0        0     5352 2023-08-01 15:03:22.000000 ag_llama2_api_s-0.0.14/ag_llama2_api_s/model.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:09:06.727923 ag_llama2_api_s-0.0.14/ag_llama2_api_s.egg-info/
--rw-rw-rw-   0        0        0      771 2023-08-01 15:09:06.000000 ag_llama2_api_s-0.0.14/ag_llama2_api_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-08-01 15:09:06.000000 ag_llama2_api_s-0.0.14/ag_llama2_api_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 15:09:06.000000 ag_llama2_api_s-0.0.14/ag_llama2_api_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      297 2023-08-01 15:09:06.000000 ag_llama2_api_s-0.0.14/ag_llama2_api_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-01 15:09:06.000000 ag_llama2_api_s-0.0.14/ag_llama2_api_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 15:09:06.740889 ag_llama2_api_s-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0     2573 2023-08-01 15:00:39.000000 ag_llama2_api_s-0.0.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:09:06.733908 ag_llama2_api_s-0.0.14/tests/
--rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama2_api_s-0.0.14/tests/test_choice.py
--rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama2_api_s-0.0.14/tests/test_model.py
--rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama2_api_s-0.0.14/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:09:06.736901 ag_llama2_api_s-0.0.14/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_api_s-0.0.14/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_api_s-0.0.14/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:10:38.065046 ag_llama2_api_s-0.0.15/
+-rw-rw-rw-   0        0        0      771 2023-08-01 15:10:38.063052 ag_llama2_api_s-0.0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 15:10:38.042010 ag_llama2_api_s-0.0.15/ag_llama2_api_s/
+-rw-rw-rw-   0        0        0     2190 2023-08-01 15:06:03.000000 ag_llama2_api_s-0.0.15/ag_llama2_api_s/__init__.py
+-rw-rw-rw-   0        0        0     8751 2023-08-01 15:10:27.000000 ag_llama2_api_s-0.0.15/ag_llama2_api_s/__main__.py
+-rw-rw-rw-   0        0        0     5352 2023-08-01 15:03:22.000000 ag_llama2_api_s-0.0.15/ag_llama2_api_s/model.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:10:38.050987 ag_llama2_api_s-0.0.15/ag_llama2_api_s.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-08-01 15:10:37.000000 ag_llama2_api_s-0.0.15/ag_llama2_api_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-08-01 15:10:37.000000 ag_llama2_api_s-0.0.15/ag_llama2_api_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 15:10:37.000000 ag_llama2_api_s-0.0.15/ag_llama2_api_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      297 2023-08-01 15:10:37.000000 ag_llama2_api_s-0.0.15/ag_llama2_api_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-01 15:10:37.000000 ag_llama2_api_s-0.0.15/ag_llama2_api_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 15:10:38.065046 ag_llama2_api_s-0.0.15/setup.cfg
+-rw-rw-rw-   0        0        0     2573 2023-08-01 15:00:39.000000 ag_llama2_api_s-0.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:10:38.056970 ag_llama2_api_s-0.0.15/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama2_api_s-0.0.15/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama2_api_s-0.0.15/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama2_api_s-0.0.15/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:10:38.062054 ag_llama2_api_s-0.0.15/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_api_s-0.0.15/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_api_s-0.0.15/utils/render.py
```

### Comparing `ag_llama2_api_s-0.0.14/PKG-INFO` & `ag_llama2_api_s-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama2_api_s
-Version: 0.0.14
+Version: 0.0.15
 Summary: ag_llama2_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama2_api_s-0.0.14/ag_llama2_api_s/__init__.py` & `ag_llama2_api_s-0.0.15/ag_llama2_api_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_api_s-0.0.14/ag_llama2_api_s/__main__.py` & `ag_llama2_api_s-0.0.15/ag_llama2_api_s/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 logger.level("INFO", color="<green>")
 
 import waitress
 from flask import Flask, Response, abort, jsonify, render_template, request
 from flask_cors import CORS
 
 from . import is_true
-from .choice import reduce_choice
 from .model import load_model
 
 # Configurations from environment variables.
 from . import MODEL
 from . import HOST
 from . import PORT
 from . import MODEL_REVISION
```

### Comparing `ag_llama2_api_s-0.0.14/ag_llama2_api_s/model.py` & `ag_llama2_api_s-0.0.15/ag_llama2_api_s/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_api_s-0.0.14/ag_llama2_api_s.egg-info/PKG-INFO` & `ag_llama2_api_s-0.0.15/ag_llama2_api_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama2-api-s
-Version: 0.0.14
+Version: 0.0.15
 Summary: ag_llama2_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama2_api_s-0.0.14/setup.py` & `ag_llama2_api_s-0.0.15/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_api_s-0.0.14/tests/test_choice.py` & `ag_llama2_api_s-0.0.15/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_api_s-0.0.14/tests/test_model.py` & `ag_llama2_api_s-0.0.15/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_api_s-0.0.14/tests/test_tokenizer.py` & `ag_llama2_api_s-0.0.15/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_api_s-0.0.14/utils/download.py` & `ag_llama2_api_s-0.0.15/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_api_s-0.0.14/utils/render.py` & `ag_llama2_api_s-0.0.15/utils/render.py`

 * *Files identical despite different names*

