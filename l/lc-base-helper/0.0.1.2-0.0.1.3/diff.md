# Comparing `tmp/lc_base_helper-0.0.1.2.tar.gz` & `tmp/lc_base_helper-0.0.1.3.tar.gz`

## Comparing `lc_base_helper-0.0.1.2.tar` & `lc_base_helper-0.0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/GetRequires.bat
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/setup.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/chineseLanguageHelper.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/ocrHelper.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/pathHelper.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/pdfHelper.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/stringHelper.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/src/lc-base-helper/terminalHelper.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/.gitignore
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/README.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/GetRequires.bat
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/setup.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/src/lc-base-helper/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/src/lc-base-helper/chineseLanguageHelper.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/src/lc-base-helper/ocrHelper.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/src/lc-base-helper/pathHelper.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/src/lc-base-helper/pdfHelper.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/src/lc-base-helper/stringHelper.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/src/lc-base-helper/terminalHelper.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/.gitignore
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/README.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 lc_base_helper-0.0.1.3/PKG-INFO
```

### Comparing `lc_base_helper-0.0.1.2/setup.py` & `lc_base_helper-0.0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/.github/workflows/python-publish.yml` & `lc_base_helper-0.0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/src/lc-base-helper/chineseLanguageHelper.py` & `lc_base_helper-0.0.1.3/src/lc-base-helper/chineseLanguageHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/src/lc-base-helper/ocrHelper.py` & `lc_base_helper-0.0.1.3/src/lc-base-helper/ocrHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/src/lc-base-helper/pathHelper.py` & `lc_base_helper-0.0.1.3/src/lc-base-helper/pathHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/src/lc-base-helper/pdfHelper.py` & `lc_base_helper-0.0.1.3/src/lc-base-helper/pdfHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/src/lc-base-helper/stringHelper.py` & `lc_base_helper-0.0.1.3/src/lc-base-helper/stringHelper.py`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/.gitignore` & `lc_base_helper-0.0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/LICENSE` & `lc_base_helper-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lc_base_helper-0.0.1.2/PKG-INFO` & `lc_base_helper-0.0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-base-helper
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Lc's python helper.
 Project-URL: Homepage, https://github.com/Diselorya/LCsPythonHelper/
 Author: Diselorya
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         
@@ -40,13 +40,13 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: opencv-python
 Requires-Dist: pangu
-Requires-Dist: pypdf2>3.0.1
-Requires-Dist: pytesseract>0.3.10
+Requires-Dist: pypdf2
+Requires-Dist: pytesseract
 Description-Content-Type: text/markdown
 
 # LCsPythonHelper
 # My Python Helper
```

