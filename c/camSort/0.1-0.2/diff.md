# Comparing `tmp/camSort-0.1.tar.gz` & `tmp/camSort-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/camSort-0.1.tar", last modified: Tue Aug  1 07:31:55 2023, max compression
+gzip compressed data, was "dist/camSort-0.2.tar", last modified: Tue Aug  1 08:27:55 2023, max compression
```

## Comparing `camSort-0.1.tar` & `camSort-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 07:31:55.000000 camSort-0.1/
--rw-r--r--   0 macbook    (501) staff       (20)     2213 2023-08-01 07:31:55.000000 camSort-0.1/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1480 2023-08-01 07:18:27.000000 camSort-0.1/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 07:31:55.000000 camSort-0.1/camSort/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-08-01 06:50:14.000000 camSort-0.1/camSort/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   234571 2023-08-01 07:17:43.000000 camSort-0.1/camSort/camSort.c
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 07:31:55.000000 camSort-0.1/camSort.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2213 2023-08-01 07:31:55.000000 camSort-0.1/camSort.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      180 2023-08-01 07:31:55.000000 camSort-0.1/camSort.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-01 07:31:55.000000 camSort-0.1/camSort.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-01 07:31:55.000000 camSort-0.1/camSort.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-01 07:31:55.000000 camSort-0.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)      879 2023-08-01 07:31:53.000000 camSort-0.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:27:55.000000 camSort-0.2/
+-rw-r--r--   0 macbook    (501) staff       (20)     2459 2023-08-01 08:27:55.000000 camSort-0.2/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1529 2023-08-01 07:52:20.000000 camSort-0.2/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:27:55.000000 camSort-0.2/camSort/
+-rw-r--r--   0 macbook    (501) staff       (20)       14 2023-08-01 08:09:51.000000 camSort-0.2/camSort/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   234571 2023-08-01 07:17:43.000000 camSort-0.2/camSort/camSort.c
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 08:27:55.000000 camSort-0.2/camSort.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2459 2023-08-01 08:27:55.000000 camSort-0.2/camSort.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      180 2023-08-01 08:27:55.000000 camSort-0.2/camSort.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-01 08:27:55.000000 camSort-0.2/camSort.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-01 08:27:55.000000 camSort-0.2/camSort.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-01 08:27:55.000000 camSort-0.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1038 2023-08-01 08:27:51.000000 camSort-0.2/setup.py
```

### Comparing `camSort-0.1/PKG-INFO` & `camSort-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.1
+Version: 0.2
 Summary: make sorted() fast for strings
 Home-page: https://github.com/cameronbae/camSort
 Author: cameronbae / cameron jay
 Author-email: <contact@camjay.io>
 License: UNKNOWN
 Description: 
         # camSort
@@ -19,14 +19,16 @@
         
         The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
         
         The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
         
         ## Installation
         
+        ```pip install camSort``` or compile locally :)
+        
         ## Usage
         
         ```python
         import camSort
         # or
         from camSort import sortStrings
         
@@ -43,10 +45,14 @@
         Average output on my 2017 macbook pro:
             (1 million strings, with a random legnth of 1 to 1000 chararacters)
         
         Time taken by Python sorted(): 56.08621883392334 seconds
         Time taken by camSort: 6.356221914291382 seconds
 Keywords: python,sorted,sort,camSort
 Platform: UNKNOWN
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `camSort-0.1/README.md` & `camSort-0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
 
 The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
 
 ## Installation
 
+```pip install camSort``` or compile locally :)
+
 ## Usage
 
 ```python
 import camSort
 # or
 from camSort import sortStrings
```

### Comparing `camSort-0.1/camSort/camSort.c` & `camSort-0.2/camSort/camSort.c`

 * *Files identical despite different names*

### Comparing `camSort-0.1/camSort.egg-info/PKG-INFO` & `camSort-0.2/camSort.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.1
+Version: 0.2
 Summary: make sorted() fast for strings
 Home-page: https://github.com/cameronbae/camSort
 Author: cameronbae / cameron jay
 Author-email: <contact@camjay.io>
 License: UNKNOWN
 Description: 
         # camSort
@@ -19,14 +19,16 @@
         
         The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
         
         The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
         
         ## Installation
         
+        ```pip install camSort``` or compile locally :)
+        
         ## Usage
         
         ```python
         import camSort
         # or
         from camSort import sortStrings
         
@@ -43,10 +45,14 @@
         Average output on my 2017 macbook pro:
             (1 million strings, with a random legnth of 1 to 1000 chararacters)
         
         Time taken by Python sorted(): 56.08621883392334 seconds
         Time taken by camSort: 6.356221914291382 seconds
 Keywords: python,sorted,sort,camSort
 Platform: UNKNOWN
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `camSort-0.1/setup.py` & `camSort-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from setuptools import setup, find_packages
 from Cython.Build import cythonize
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.13'
 LONG_DESCRIPTION = ''
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name="camSort",
-    version="0.1",
+    version="0.2",
     packages=["camSort"], 
     ext_modules = cythonize('camSort/camSort.pyx'),
     author="cameronbae / cameron jay",
     author_email="<contact@camjay.io>",
     url="https://github.com/cameronbae/camSort",
     description="make sorted() fast for strings",
     long_description_content_type="text/markdown",
     long_description=long_description,
     keywords=['python', 'sorted', 'sort', 'camSort'],
     classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Operating System :: MacOS :: MacOS X"
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
     ]
 )
```

