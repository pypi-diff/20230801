# Comparing `tmp/lc_base_helper-0.0.1.1.tar.gz` & `tmp/lc_base_helper-0.0.1.2.tar.gz`

## Comparing `lc_base_helper-0.0.1.1.tar` & `lc_base_helper-0.0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/GetRequires.bat
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/setup.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/src/lc-base-helper/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/src/lc-base-helper/chineseLanguageHelper.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/src/lc-base-helper/ocrHelper.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/src/lc-base-helper/pathHelper.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/src/lc-base-helper/pdfHelper.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/src/lc-base-helper/stringHelper.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/src/lc-base-helper/terminalHelper.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/.gitignore
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/README.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/GetRequires.bat
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/setup.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/chineseLanguageHelper.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/ocrHelper.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/pathHelper.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/pdfHelper.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/stringHelper.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/terminalHelper.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/.gitignore
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/README.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/PKG-INFO
```

### Comparing `lc_base_helper-0.0.1.1/setup.py` & `lc_base_helper-0.0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/.github/workflows/python-publish.yml` & `lc_base_helper-0.0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/src/lc-base-helper/chineseLanguageHelper.py` & `lc_base_helper-0.0.1.2/src/lc-base-helper/chineseLanguageHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/src/lc-base-helper/ocrHelper.py` & `lc_base_helper-0.0.1.2/src/lc-base-helper/ocrHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/src/lc-base-helper/pathHelper.py` & `lc_base_helper-0.0.1.2/src/lc-base-helper/pathHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/src/lc-base-helper/pdfHelper.py` & `lc_base_helper-0.0.1.2/src/lc-base-helper/pdfHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/src/lc-base-helper/stringHelper.py` & `lc_base_helper-0.0.1.2/src/lc-base-helper/stringHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/.gitignore` & `lc_base_helper-0.0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/LICENSE` & `lc_base_helper-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.1/pyproject.toml` & `lc_base_helper-0.0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lc-base-helper"
-version = "0.0.1.1"
+version = "0.0.1.2"
 description = "Lc's python helper."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Diselorya"},
 ]
 keywords=['python', 'lc-base-helper', 'diselorya']
 dependencies = [
     'PyPDF2>3.0.1',
     'pytesseract>0.3.10', 
     'pangu', 
-    'opencv-python>4.8.0.74'
+    'opencv-python'
 ]
 classifiers= [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Operating System :: Microsoft :: Windows"
 ]
```

### Comparing `lc_base_helper-0.0.1.1/PKG-INFO` & `lc_base_helper-0.0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-base-helper
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Lc's python helper.
 Project-URL: Homepage, https://github.com/Diselorya/LCsPythonHelper/
 Author: Diselorya
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         
@@ -38,15 +38,15 @@
 License-File: LICENSE
 Keywords: diselorya,lc-base-helper,python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: opencv-python>4.8.0.74
+Requires-Dist: opencv-python
 Requires-Dist: pangu
 Requires-Dist: pypdf2>3.0.1
 Requires-Dist: pytesseract>0.3.10
 Description-Content-Type: text/markdown
 
 # LCsPythonHelper
 # My Python Helper
```

