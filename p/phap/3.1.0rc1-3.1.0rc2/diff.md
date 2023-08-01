# Comparing `tmp/phap-3.1.0rc1.tar.gz` & `tmp/phap-3.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phap-3.1.0rc1.tar", last modified: Mon Jul 31 04:31:18 2023, max compression
+gzip compressed data, was "phap-3.1.0rc2.tar", last modified: Tue Aug  1 14:11:02 2023, max compression
```

## Comparing `phap-3.1.0rc1.tar` & `phap-3.1.0rc2.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.032437 phap-3.1.0rc1/
--rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0rc1/LICENSE
--rw-rw-rw-   0        0        0     2502 2023-07-31 04:31:18.032437 phap-3.1.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0     1702 2023-07-31 04:30:14.000000 phap-3.1.0rc1/README.md
--rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0rc1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 04:31:18.033437 phap-3.1.0rc1/setup.cfg
--rw-rw-rw-   0        0        0     1686 2023-07-31 04:30:32.000000 phap-3.1.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:17.960915 phap-3.1.0rc1/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.006471 phap-3.1.0rc1/src/algo/
--rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0rc1/src/algo/__init__.py
--rw-rw-rw-   0        0        0      607 2023-07-25 04:12:52.000000 phap-3.1.0rc1/src/algo/arraylib.py
--rw-rw-rw-   0        0        0     4538 2023-07-31 04:28:39.000000 phap-3.1.0rc1/src/algo/treelib.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.008476 phap-3.1.0rc1/src/phap/
--rw-rw-rw-   0        0        0       72 2023-07-24 11:39:49.000000 phap-3.1.0rc1/src/phap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.015472 phap-3.1.0rc1/src/phap.egg-info/
--rw-rw-rw-   0        0        0     2502 2023-07-31 04:31:17.000000 phap-3.1.0rc1/src/phap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-07-31 04:31:17.000000 phap-3.1.0rc1/src/phap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 04:31:17.000000 phap-3.1.0rc1/src/phap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 04:31:17.000000 phap-3.1.0rc1/src/phap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.017440 phap-3.1.0rc1/src/phapbm/
--rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0rc1/src/phapbm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.022434 phap-3.1.0rc1/src/stralgo/
--rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/base.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.025435 phap-3.1.0rc1/src/stralgo/hash/
--rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/hash/__init__.py
--rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/hash/sha.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.029440 phap-3.1.0rc1/src/stralgo/hash/sm/
--rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/hash/sm/__init__.py
--rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0rc1/src/stralgo/hash/sm/sm3libs.py
--rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/json.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.467963 phap-3.1.0rc2/
+-rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0rc2/LICENSE
+-rw-rw-rw-   0        0        0     2502 2023-08-01 14:11:02.467963 phap-3.1.0rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     1702 2023-08-01 01:31:55.000000 phap-3.1.0rc2/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0rc2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 14:11:02.467963 phap-3.1.0rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2023-08-01 14:06:26.000000 phap-3.1.0rc2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.377099 phap-3.1.0rc2/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.441248 phap-3.1.0rc2/src/algo/
+-rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0rc2/src/algo/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-07-25 04:12:52.000000 phap-3.1.0rc2/src/algo/arraylib.py
+-rw-rw-rw-   0        0        0     4538 2023-07-31 04:28:39.000000 phap-3.1.0rc2/src/algo/treelib.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.443247 phap-3.1.0rc2/src/cahap/
+-rw-rw-rw-   0        0        0     1160 2023-08-01 14:05:58.000000 phap-3.1.0rc2/src/cahap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.444251 phap-3.1.0rc2/src/phap/
+-rw-rw-rw-   0        0        0      107 2023-08-01 13:59:56.000000 phap-3.1.0rc2/src/phap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.452354 phap-3.1.0rc2/src/phap.egg-info/
+-rw-rw-rw-   0        0        0     2502 2023-08-01 14:11:02.000000 phap-3.1.0rc2/src/phap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-08-01 14:11:02.000000 phap-3.1.0rc2/src/phap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 14:11:02.000000 phap-3.1.0rc2/src/phap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-01 14:11:02.000000 phap-3.1.0rc2/src/phap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.453861 phap-3.1.0rc2/src/phapbm/
+-rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0rc2/src/phapbm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.458867 phap-3.1.0rc2/src/stralgo/
+-rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/base.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.461866 phap-3.1.0rc2/src/stralgo/hash/
+-rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/hash/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/hash/sha.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.464964 phap-3.1.0rc2/src/stralgo/hash/sm/
+-rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/hash/sm/__init__.py
+-rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0rc2/src/stralgo/hash/sm/sm3libs.py
+-rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/json.py
```

### Comparing `phap-3.1.0rc1/LICENSE` & `phap-3.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc1/PKG-INFO` & `phap-3.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.1.0rc1
+Version: 3.1.0rc2
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-rc1
++ v3.1.0-rc2
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0rc1/README.md` & `phap-3.1.0rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-rc1
++ v3.1.0-rc2
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0rc1/setup.py` & `phap-3.1.0rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phap",
-    version="3.1.0rc1",  #版本
+    version="3.1.0rc2",  #版本
     author="DashBing",
     author_email="mcbbkf@outlook.com",
     description="Programing Helpful Algorithm Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #scripts=[],
     url="https://github.com/DashBing/phap/",
```

### Comparing `phap-3.1.0rc1/src/algo/arraylib.py` & `phap-3.1.0rc2/src/algo/arraylib.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc1/src/algo/treelib.py` & `phap-3.1.0rc2/src/algo/treelib.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc1/src/phap.egg-info/PKG-INFO` & `phap-3.1.0rc2/src/phap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.1.0rc1
+Version: 3.1.0rc2
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-rc1
++ v3.1.0-rc2
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0rc1/src/phapbm/__init__.py` & `phap-3.1.0rc2/src/phapbm/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc1/src/stralgo/__init__.py` & `phap-3.1.0rc2/src/stralgo/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc1/src/stralgo/base.py` & `phap-3.1.0rc2/src/stralgo/base.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc1/src/stralgo/hash/sm/sm3libs.py` & `phap-3.1.0rc2/src/stralgo/hash/sm/sm3libs.py`

 * *Files identical despite different names*

