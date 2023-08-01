# Comparing `tmp/datatable-faker-0.1.6.tar.gz` & `tmp/datatable-faker-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable-faker-0.1.6.tar", last modified: Thu Apr 27 07:32:30 2023, max compression
+gzip compressed data, was "datatable-faker-0.1.7.tar", last modified: Tue Aug  1 05:05:11 2023, max compression
```

## Comparing `datatable-faker-0.1.6.tar` & `datatable-faker-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:32:30.184568 datatable-faker-0.1.6/
--rw-rw-r--   0 root         (0) root         (0)     1070 2023-04-25 12:48:19.000000 datatable-faker-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2381 2023-04-27 07:32:30.184568 datatable-faker-0.1.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1751 2023-04-26 05:06:25.000000 datatable-faker-0.1.6/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 07:32:30.184568 datatable-faker-0.1.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      982 2023-04-27 07:32:20.000000 datatable-faker-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:32:30.184568 datatable-faker-0.1.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:32:30.184568 datatable-faker-0.1.6/src/datatable_faker/
--rw-rw-r--   0 root         (0) root         (0)     5049 2023-04-27 07:32:03.000000 datatable-faker-0.1.6/src/datatable_faker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    29616 2023-04-27 07:28:59.000000 datatable-faker-0.1.6/src/datatable_faker/check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:32:30.184568 datatable-faker-0.1.6/src/datatable_faker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2381 2023-04-27 07:32:30.000000 datatable-faker-0.1.6/src/datatable_faker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      302 2023-04-27 07:32:30.000000 datatable-faker-0.1.6/src/datatable_faker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 07:32:30.000000 datatable-faker-0.1.6/src/datatable_faker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 07:32:30.000000 datatable-faker-0.1.6/src/datatable_faker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 07:32:30.000000 datatable-faker-0.1.6/src/datatable_faker.egg-info/top_level.txt
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-08-01 05:05:11.290983 datatable-faker-0.1.7/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1070 2023-08-01 04:49:39.000000 datatable-faker-0.1.7/LICENSE
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     2418 2023-08-01 05:05:11.290983 datatable-faker-0.1.7/PKG-INFO
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1751 2023-08-01 04:49:39.000000 datatable-faker-0.1.7/README.rst
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)       38 2023-08-01 05:05:11.290983 datatable-faker-0.1.7/setup.cfg
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1030 2023-08-01 05:04:22.000000 datatable-faker-0.1.7/setup.py
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-08-01 05:05:11.290983 datatable-faker-0.1.7/src/
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-08-01 05:05:11.290983 datatable-faker-0.1.7/src/datatable_faker/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1881 2023-08-01 04:50:05.000000 datatable-faker-0.1.7/src/datatable_faker/__init__.py
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-08-01 05:05:11.290983 datatable-faker-0.1.7/src/datatable_faker.egg-info/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     2418 2023-08-01 05:05:11.000000 datatable-faker-0.1.7/src/datatable_faker.egg-info/PKG-INFO
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)      273 2023-08-01 05:05:11.000000 datatable-faker-0.1.7/src/datatable_faker.egg-info/SOURCES.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)        1 2023-08-01 05:05:11.000000 datatable-faker-0.1.7/src/datatable_faker.egg-info/dependency_links.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)        6 2023-08-01 05:05:11.000000 datatable-faker-0.1.7/src/datatable_faker.egg-info/requires.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)       16 2023-08-01 05:05:11.000000 datatable-faker-0.1.7/src/datatable_faker.egg-info/top_level.txt
```

### Comparing `datatable-faker-0.1.6/LICENSE` & `datatable-faker-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.6/PKG-INFO` & `datatable-faker-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: datatable-faker
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to generate fake datatable for unittest 
 Home-page: https://github.com/Agent-Hellboy/datatable-faker
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Keywords: faker,datatable-faker
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 datatable-faker
 ================
 
 Library to generate fake datatable for unittest
```

### Comparing `datatable-faker-0.1.6/README.rst` & `datatable-faker-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `datatable-faker-0.1.6/setup.py` & `datatable-faker-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="datatable-faker",
     author="Prince Roshan",
-    version='0.1.6',
+    version='0.1.7',
     author_email="princekrroshan01@gmail.com",
     url="https://github.com/Agent-Hellboy/datatable-faker",
     description="Library to generate fake datatable for unittest ",
+    long_description_content_type='text/x-rst',
     long_description=read("README.rst"),
     license="MIT",
     package_dir={'': 'src'},
     packages=['datatable_faker'],
     keywords=[
         "faker","datatable-faker"
     ],
```

### Comparing `datatable-faker-0.1.6/src/datatable_faker.egg-info/PKG-INFO` & `datatable-faker-0.1.7/src/datatable_faker.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: datatable-faker
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to generate fake datatable for unittest 
 Home-page: https://github.com/Agent-Hellboy/datatable-faker
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Keywords: faker,datatable-faker
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 datatable-faker
 ================
 
 Library to generate fake datatable for unittest
```

