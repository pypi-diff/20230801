# Comparing `tmp/KKMeans-0.0.5.tar.gz` & `tmp/KKMeans-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KKMeans-0.0.5.tar", last modified: Mon Jul 31 12:15:23 2023, max compression
+gzip compressed data, was "KKMeans-0.0.6.tar", last modified: Mon Jul 31 23:17:10 2023, max compression
```

## Comparing `KKMeans-0.0.5.tar` & `KKMeans-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 12:15:23.253541 KKMeans-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-31 12:15:23.231119 KKMeans-0.0.5/KKMeans.egg-info/
--rw-rw-rw-   0        0        0      585 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      585 2023-07-31 12:15:23.253034 KKMeans-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-30 20:10:21.000000 KKMeans-0.0.5/README.md
--rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.5/license.txt
--rw-rw-rw-   0        0        0      521 2023-07-31 12:14:25.000000 KKMeans-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 12:15:23.253541 KKMeans-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1663 2023-07-31 12:13:21.000000 KKMeans-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:15:23.212752 KKMeans-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 12:15:23.252014 KKMeans-0.0.5/src/KKMeans/
--rw-rw-rw-   0        0        0   875796 2023-07-31 11:49:59.000000 KKMeans-0.0.5/src/KKMeans/KKMeans.c
--rw-rw-rw-   0        0        0    27233 2023-07-31 11:36:19.000000 KKMeans-0.0.5/src/KKMeans/KKMeans.py
--rw-rw-rw-   0        0        0       43 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/__init__.py
--rw-rw-rw-   0        0        0  1170842 2023-07-31 12:15:21.000000 KKMeans-0.0.5/src/KKMeans/elkan.c
--rw-rw-rw-   0        0        0     9984 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/elkan.pyx
--rw-rw-rw-   0        0        0  1182482 2023-07-31 12:15:22.000000 KKMeans-0.0.5/src/KKMeans/kernels.c
--rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/kernels.pyx
--rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.5/src/KKMeans/lloyd.c
--rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/lloyd.pyx
--rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.5/src/KKMeans/quality.c
--rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.5/src/KKMeans/quality.pyx
--rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.5/src/KKMeans/utils.c
--rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/utils.pyx
+drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.862546 KKMeans-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.837993 KKMeans-0.0.6/KKMeans.egg-info/
+-rw-rw-rw-   0        0        0      618 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 23:17:10.000000 KKMeans-0.0.6/KKMeans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      618 2023-07-31 23:17:10.862027 KKMeans-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-31 12:26:00.000000 KKMeans-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.6/license.txt
+-rw-rw-rw-   0        0        0      521 2023-07-31 23:16:26.000000 KKMeans-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 23:17:10.863053 KKMeans-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2023-07-31 12:13:21.000000 KKMeans-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.815519 KKMeans-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.859978 KKMeans-0.0.6/src/KKMeans/
+-rw-rw-rw-   0        0        0   875796 2023-07-31 11:49:59.000000 KKMeans-0.0.6/src/KKMeans/KKMeans.c
+-rw-rw-rw-   0        0        0    27233 2023-07-31 11:36:19.000000 KKMeans-0.0.6/src/KKMeans/KKMeans.py
+-rw-rw-rw-   0        0        0       28 2023-07-31 23:15:44.000000 KKMeans-0.0.6/src/KKMeans/__init__.py
+-rw-rw-rw-   0        0        0  1170842 2023-07-31 23:17:09.000000 KKMeans-0.0.6/src/KKMeans/elkan.c
+-rw-rw-rw-   0        0        0     9984 2023-07-31 16:04:53.000000 KKMeans-0.0.6/src/KKMeans/elkan.pyx
+-rw-rw-rw-   0        0        0  1182482 2023-07-31 23:17:09.000000 KKMeans-0.0.6/src/KKMeans/kernels.c
+-rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.6/src/KKMeans/kernels.pyx
+-rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.6/src/KKMeans/lloyd.c
+-rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.6/src/KKMeans/lloyd.pyx
+-rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.6/src/KKMeans/quality.c
+-rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.6/src/KKMeans/quality.pyx
+-rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.6/src/KKMeans/utils.c
+-rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.6/src/KKMeans/utils.pyx
+drwxrwxrwx   0        0        0        0 2023-07-31 23:17:10.861000 KKMeans-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1472 2023-07-31 17:53:20.000000 KKMeans-0.0.6/tests/test_pytest_utils.py
```

### Comparing `KKMeans-0.0.5/KKMeans.egg-info/SOURCES.txt` & `KKMeans-0.0.6/KKMeans.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 src/KKMeans/kernels.c
 src/KKMeans/kernels.pyx
 src/KKMeans/lloyd.c
 src/KKMeans/lloyd.pyx
 src/KKMeans/quality.c
 src/KKMeans/quality.pyx
 src/KKMeans/utils.c
-src/KKMeans/utils.pyx
+src/KKMeans/utils.pyx
+tests/test_pytest_utils.py
```

### Comparing `KKMeans-0.0.5/license.txt` & `KKMeans-0.0.6/license.txt`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/pyproject.toml` & `KKMeans-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=63", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "KKMeans"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Paul Theis", email="keymailt7@gmail.com" },
 ]
 dependencies = ["numpy>=1.25"]
 description = "https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `KKMeans-0.0.5/setup.py` & `KKMeans-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/KKMeans.c` & `KKMeans-0.0.6/src/KKMeans/KKMeans.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/KKMeans.py` & `KKMeans-0.0.6/src/KKMeans/KKMeans.py`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/elkan.c` & `KKMeans-0.0.6/src/KKMeans/elkan.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/elkan.pyx` & `KKMeans-0.0.6/src/KKMeans/elkan.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/kernels.c` & `KKMeans-0.0.6/src/KKMeans/kernels.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/kernels.pyx` & `KKMeans-0.0.6/src/KKMeans/kernels.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/lloyd.c` & `KKMeans-0.0.6/src/KKMeans/lloyd.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/lloyd.pyx` & `KKMeans-0.0.6/src/KKMeans/lloyd.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/quality.c` & `KKMeans-0.0.6/src/KKMeans/quality.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/quality.pyx` & `KKMeans-0.0.6/src/KKMeans/quality.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/utils.c` & `KKMeans-0.0.6/src/KKMeans/utils.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.5/src/KKMeans/utils.pyx` & `KKMeans-0.0.6/src/KKMeans/utils.pyx`

 * *Files identical despite different names*

