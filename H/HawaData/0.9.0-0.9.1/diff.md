# Comparing `tmp/HawaData-0.9.0.tar.gz` & `tmp/HawaData-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.9.0.tar", last modified: Thu Jul 27 05:28:38 2023, max compression
+gzip compressed data, was "HawaData-0.9.1.tar", last modified: Tue Aug  1 10:00:18 2023, max compression
```

## Comparing `HawaData-0.9.0.tar` & `HawaData-0.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.483112 HawaData-0.9.0/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.473611 HawaData-0.9.0/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3545 2023-07-27 05:28:38.000000 HawaData-0.9.0/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-27 05:28:38.000000 HawaData-0.9.0/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-27 05:28:38.000000 HawaData-0.9.0/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-27 05:28:38.000000 HawaData-0.9.0/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3545 2023-07-27 05:28:38.482816 HawaData-0.9.0/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.9.0/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.474063 HawaData-0.9.0/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.9.0/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.475861 HawaData-0.9.0/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.9.0/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2807 2023-07-27 02:46:27.000000 HawaData-0.9.0/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.9.0/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.9.0/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.9.0/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.477123 HawaData-0.9.0/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.9.0/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    17368 2023-07-27 05:22:54.000000 HawaData-0.9.0/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6517 2023-07-27 05:22:54.000000 HawaData-0.9.0/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.9.0/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.9.0/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.480781 HawaData-0.9.0/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.9.0/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.9.0/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.9.0/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.9.0/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.9.0/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.9.0/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.9.0/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.481947 HawaData-0.9.0/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.9.0/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.9.0/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.9.0/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-27 05:28:38.483192 HawaData-0.9.0/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.9.0/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.482191 HawaData-0.9.0/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.9.0/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-01 10:00:18.574087 HawaData-0.9.1/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-01 10:00:18.561226 HawaData-0.9.1/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3574 2023-08-01 10:00:18.000000 HawaData-0.9.1/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-08-01 10:00:18.000000 HawaData-0.9.1/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-08-01 10:00:18.000000 HawaData-0.9.1/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-08-01 10:00:18.000000 HawaData-0.9.1/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3574 2023-08-01 10:00:18.573695 HawaData-0.9.1/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.9.1/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-01 10:00:18.562056 HawaData-0.9.1/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.9.1/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-01 10:00:18.564733 HawaData-0.9.1/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.9.1/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2807 2023-07-27 02:46:27.000000 HawaData-0.9.1/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.9.1/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      142 2023-08-01 09:59:51.000000 HawaData-0.9.1/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.9.1/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-01 10:00:18.567000 HawaData-0.9.1/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.9.1/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    17368 2023-07-27 05:22:54.000000 HawaData-0.9.1/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6517 2023-07-27 05:22:54.000000 HawaData-0.9.1/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.9.1/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.9.1/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-01 10:00:18.570848 HawaData-0.9.1/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.9.1/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.9.1/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.9.1/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.9.1/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.9.1/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.9.1/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1181 2023-08-01 09:59:51.000000 HawaData-0.9.1/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-01 10:00:18.572335 HawaData-0.9.1/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.9.1/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.9.1/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.9.1/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-08-01 10:00:18.574178 HawaData-0.9.1/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.9.1/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-01 10:00:18.572980 HawaData-0.9.1/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.9.1/test/test_query.py
```

### Comparing `HawaData-0.9.0/HawaData.egg-info/PKG-INFO` & `HawaData-0.9.1/HawaData.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.9.0
+Version: 0.9.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -121,7 +121,8 @@
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
 - 0.8.5 load less data
 - 0.8.7 add mongo params
 - 0.8.8 fix
 - 0.8.9 log
 - 0.9.0 use less item codes to upper
+- 0.9.1 add no answers error
```

### Comparing `HawaData-0.9.0/HawaData.egg-info/SOURCES.txt` & `HawaData-0.9.1/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/PKG-INFO` & `HawaData-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.9.0
+Version: 0.9.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -121,7 +121,8 @@
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
 - 0.8.5 load less data
 - 0.8.7 add mongo params
 - 0.8.8 fix
 - 0.8.9 log
 - 0.9.0 use less item codes to upper
+- 0.9.1 add no answers error
```

### Comparing `HawaData-0.9.0/README.md` & `HawaData-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/base/db.py` & `HawaData-0.9.1/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/base/decos.py` & `HawaData-0.9.1/hawa/base/decos.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/base/init.py` & `HawaData-0.9.1/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/common/data.py` & `HawaData-0.9.1/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/common/query.py` & `HawaData-0.9.1/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/common/utils.py` & `HawaData-0.9.1/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/config.py` & `HawaData-0.9.1/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/data/klass.py` & `HawaData-0.9.1/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/data/province.py` & `HawaData-0.9.1/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/data/school.py` & `HawaData-0.9.1/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/paper/health.py` & `HawaData-0.9.1/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/hawa/paper/mht.py` & `HawaData-0.9.1/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/setup.py` & `HawaData-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.0/test/test_query.py` & `HawaData-0.9.1/test/test_query.py`

 * *Files identical despite different names*

