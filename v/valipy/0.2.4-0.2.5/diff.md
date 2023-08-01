# Comparing `tmp/valipy-0.2.4.tar.gz` & `tmp/valipy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valipy-0.2.4.tar", last modified: Tue Aug  1 06:58:05 2023, max compression
+gzip compressed data, was "valipy-0.2.5.tar", last modified: Tue Aug  1 07:01:25 2023, max compression
```

## Comparing `valipy-0.2.4.tar` & `valipy-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 06:58:05.709766 valipy-0.2.4/
--rw-r--r--   0 josevonchong   (501) staff       (20)     1604 2023-08-01 06:58:05.709851 valipy-0.2.4/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-08-01 06:58:05.710078 valipy-0.2.4/setup.cfg
--rw-r--r--   0 josevonchong   (501) staff       (20)     1343 2023-08-01 06:58:01.000000 valipy-0.2.4/setup.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 06:58:05.707796 valipy-0.2.4/test/
--rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.2.4/test/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      544 2023-07-30 08:51:40.000000 valipy-0.2.4/test/misc.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.2.4/test/test.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 06:58:05.708773 valipy-0.2.4/valipy/
--rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.2.4/valipy/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)    11818 2023-07-30 08:45:39.000000 valipy-0.2.4/valipy/exceptions.py
--rw-r--r--   0 josevonchong   (501) staff       (20)    11728 2023-07-30 08:35:33.000000 valipy-0.2.4/valipy/myFunctions.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 06:58:05.709580 valipy-0.2.4/valipy.egg-info/
--rw-r--r--   0 josevonchong   (501) staff       (20)     1604 2023-08-01 06:58:05.000000 valipy-0.2.4/valipy.egg-info/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)      272 2023-08-01 06:58:05.000000 valipy-0.2.4/valipy.egg-info/SOURCES.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-08-01 06:58:05.000000 valipy-0.2.4/valipy.egg-info/dependency_links.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)       23 2023-08-01 06:58:05.000000 valipy-0.2.4/valipy.egg-info/requires.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-08-01 06:58:05.000000 valipy-0.2.4/valipy.egg-info/top_level.txt
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 07:01:25.737293 valipy-0.2.5/
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1605 2023-08-01 07:01:25.737373 valipy-0.2.5/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-08-01 07:01:25.737600 valipy-0.2.5/setup.cfg
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1322 2023-08-01 07:01:20.000000 valipy-0.2.5/setup.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 07:01:25.735396 valipy-0.2.5/test/
+-rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.2.5/test/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      544 2023-07-30 08:51:40.000000 valipy-0.2.5/test/misc.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.2.5/test/test.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 07:01:25.736171 valipy-0.2.5/valipy/
+-rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.2.5/valipy/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)    11818 2023-07-30 08:45:39.000000 valipy-0.2.5/valipy/exceptions.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)    11728 2023-07-30 08:35:33.000000 valipy-0.2.5/valipy/myFunctions.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 07:01:25.737162 valipy-0.2.5/valipy.egg-info/
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1605 2023-08-01 07:01:25.000000 valipy-0.2.5/valipy.egg-info/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)      272 2023-08-01 07:01:25.000000 valipy-0.2.5/valipy.egg-info/SOURCES.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-08-01 07:01:25.000000 valipy-0.2.5/valipy.egg-info/dependency_links.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)       23 2023-08-01 07:01:25.000000 valipy-0.2.5/valipy.egg-info/requires.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-08-01 07:01:25.000000 valipy-0.2.5/valipy.egg-info/top_level.txt
```

### Comparing `valipy-0.2.4/PKG-INFO` & `valipy-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.2.4
+Version: 0.2.5
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
-Keywords: validation,data,schema,schema validation,regex,patter matching
+Keywords: validation,data,schema,schema validation,regex,pattern matching
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

### Comparing `valipy-0.2.4/test/misc.py` & `valipy-0.2.5/test/misc.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.4/valipy/exceptions.py` & `valipy-0.2.5/valipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.4/valipy/myFunctions.py` & `valipy-0.2.5/valipy/myFunctions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.4/valipy.egg-info/PKG-INFO` & `valipy-0.2.5/valipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.2.4
+Version: 0.2.5
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
-Keywords: validation,data,schema,schema validation,regex,patter matching
+Keywords: validation,data,schema,schema validation,regex,pattern matching
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

