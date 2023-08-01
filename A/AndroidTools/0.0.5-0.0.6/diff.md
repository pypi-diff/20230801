# Comparing `tmp/AndroidTools-0.0.5.tar.gz` & `tmp/AndroidTools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AndroidTools-0.0.5.tar", last modified: Mon Jul 17 09:00:07 2023, max compression
+gzip compressed data, was "AndroidTools-0.0.6.tar", last modified: Tue Aug  1 08:53:06 2023, max compression
```

## Comparing `AndroidTools-0.0.5.tar` & `AndroidTools-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 09:00:07.864993 AndroidTools-0.0.5/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 09:00:07.862204 AndroidTools-0.0.5/AndTools/
--rw-r--r--   0 1a         (501) staff       (20)     2562 2023-07-17 08:59:51.000000 AndroidTools-0.0.5/AndTools/Pack.py
--rw-r--r--   0 1a         (501) staff       (20)     9323 2023-06-29 11:17:00.000000 AndroidTools-0.0.5/AndTools/TEA.py
--rw-r--r--   0 1a         (501) staff       (20)       75 2023-07-16 08:46:39.000000 AndroidTools-0.0.5/AndTools/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      269 2023-07-17 08:24:35.000000 AndroidTools-0.0.5/AndTools/byte_.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 09:00:07.863030 AndroidTools-0.0.5/AndroidTools.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-17 09:00:07.000000 AndroidTools-0.0.5/AndroidTools.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)      330 2023-07-17 09:00:07.000000 AndroidTools-0.0.5/AndroidTools.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2023-07-17 09:00:07.000000 AndroidTools-0.0.5/AndroidTools.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)       13 2023-07-17 09:00:07.000000 AndroidTools-0.0.5/AndroidTools.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 09:00:07.864178 AndroidTools-0.0.5/Jce/
--rw-r--r--   0 1a         (501) staff       (20)      115 2023-07-10 08:50:41.000000 AndroidTools-0.0.5/Jce/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2191 2023-07-15 07:24:55.000000 AndroidTools-0.0.5/Jce/bytebuffer.py
--rw-r--r--   0 1a         (501) staff       (20)      193 2023-07-10 08:50:41.000000 AndroidTools-0.0.5/Jce/exception.py
--rw-r--r--   0 1a         (501) staff       (20)    11676 2023-07-16 08:28:14.000000 AndroidTools-0.0.5/Jce/stream.py
--rw-r--r--   0 1a         (501) staff       (20)     1725 2023-07-16 09:19:40.000000 AndroidTools-0.0.5/Jce/struct.py
--rw-r--r--   0 1a         (501) staff       (20)      639 2023-07-17 09:00:07.864774 AndroidTools-0.0.5/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)      267 2023-07-16 09:28:20.000000 AndroidTools-0.0.5/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2023-07-17 09:00:07.865054 AndroidTools-0.0.5/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      622 2023-07-17 09:00:02.000000 AndroidTools-0.0.5/setup.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-07-17 09:00:07.864432 AndroidTools-0.0.5/test/
--rw-r--r--   0 1a         (501) staff       (20)      693 2023-07-16 08:31:43.000000 AndroidTools-0.0.5/test/test_Jce.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 08:53:06.701292 AndroidTools-0.0.6/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 08:53:06.696623 AndroidTools-0.0.6/AndTools/
+-rw-r--r--   0 1a         (501) staff       (20)     2562 2023-07-17 08:59:51.000000 AndroidTools-0.0.6/AndTools/Pack.py
+-rw-r--r--   0 1a         (501) staff       (20)     9323 2023-06-29 11:17:00.000000 AndroidTools-0.0.6/AndTools/TEA.py
+-rw-r--r--   0 1a         (501) staff       (20)       75 2023-07-16 08:46:39.000000 AndroidTools-0.0.6/AndTools/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      269 2023-07-17 08:24:35.000000 AndroidTools-0.0.6/AndTools/byte_.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 08:53:06.697450 AndroidTools-0.0.6/AndroidTools.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      639 2023-08-01 08:53:06.000000 AndroidTools-0.0.6/AndroidTools.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)      460 2023-08-01 08:53:06.000000 AndroidTools-0.0.6/AndroidTools.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2023-08-01 08:53:06.000000 AndroidTools-0.0.6/AndroidTools.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)       19 2023-08-01 08:53:06.000000 AndroidTools-0.0.6/AndroidTools.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 08:53:06.698599 AndroidTools-0.0.6/Jce/
+-rw-r--r--   0 1a         (501) staff       (20)      115 2023-07-10 08:50:41.000000 AndroidTools-0.0.6/Jce/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2191 2023-07-15 07:24:55.000000 AndroidTools-0.0.6/Jce/bytebuffer.py
+-rw-r--r--   0 1a         (501) staff       (20)      193 2023-07-10 08:50:41.000000 AndroidTools-0.0.6/Jce/exception.py
+-rw-r--r--   0 1a         (501) staff       (20)    11676 2023-07-16 08:28:14.000000 AndroidTools-0.0.6/Jce/stream.py
+-rw-r--r--   0 1a         (501) staff       (20)     1746 2023-08-01 06:13:47.000000 AndroidTools-0.0.6/Jce/struct.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 08:53:06.700563 AndroidTools-0.0.6/Jce_b/
+-rw-r--r--   0 1a         (501) staff       (20)     1153 2023-08-01 06:18:45.000000 AndroidTools-0.0.6/Jce_b/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     5686 2023-08-01 05:44:52.000000 AndroidTools-0.0.6/Jce_b/buffer.py
+-rw-r--r--   0 1a         (501) staff       (20)     1035 2023-08-01 05:44:52.000000 AndroidTools-0.0.6/Jce_b/head.py
+-rw-r--r--   0 1a         (501) staff       (20)      203 2023-08-01 06:44:28.000000 AndroidTools-0.0.6/Jce_b/jcetypes.py
+-rw-r--r--   0 1a         (501) staff       (20)    12499 2023-08-01 05:44:52.000000 AndroidTools-0.0.6/Jce_b/reader.py
+-rw-r--r--   0 1a         (501) staff       (20)      426 2023-08-01 05:44:52.000000 AndroidTools-0.0.6/Jce_b/struct.py
+-rw-r--r--   0 1a         (501) staff       (20)      522 2023-08-01 05:44:52.000000 AndroidTools-0.0.6/Jce_b/typing.py
+-rw-r--r--   0 1a         (501) staff       (20)     6341 2023-08-01 06:18:45.000000 AndroidTools-0.0.6/Jce_b/writer.py
+-rw-r--r--   0 1a         (501) staff       (20)      639 2023-08-01 08:53:06.701166 AndroidTools-0.0.6/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)      267 2023-07-16 09:28:20.000000 AndroidTools-0.0.6/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2023-08-01 08:53:06.701338 AndroidTools-0.0.6/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      622 2023-08-01 08:53:06.000000 AndroidTools-0.0.6/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2023-08-01 08:53:06.700858 AndroidTools-0.0.6/test/
+-rw-r--r--   0 1a         (501) staff       (20)      693 2023-07-16 08:31:43.000000 AndroidTools-0.0.6/test/test_Jce.py
```

### Comparing `AndroidTools-0.0.5/AndTools/Pack.py` & `AndroidTools-0.0.6/AndTools/Pack.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.5/AndTools/TEA.py` & `AndroidTools-0.0.6/AndTools/TEA.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.5/AndroidTools.egg-info/PKG-INFO` & `AndroidTools-0.0.6/AndroidTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AndroidTools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Android Tools for Python
 Home-page: https://github.com/grayrail000/PyJce
 Author: 1a
 Author-email: grayrail1x3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AndroidTools-0.0.5/Jce/bytebuffer.py` & `AndroidTools-0.0.6/Jce/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.5/Jce/stream.py` & `AndroidTools-0.0.6/Jce/stream.py`

 * *Files identical despite different names*

### Comparing `AndroidTools-0.0.5/Jce/struct.py` & `AndroidTools-0.0.6/Jce/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     def __getitem__(self, key):
         return self.data[key]
 
     def __setitem__(self, key, value):
         self.data[key] = value
 
     def read_from(self, stream):
+        """读取"""
         self.data.clear()
         head_data, _ = stream.peak_head()
         while head_data.type != 11 and stream._bs.position < len(stream._bs.bytes):
             tag = head_data.tag
             value = stream.read_current(True)
             if isinstance(value, bytes) and len(value) > 0:
                 try:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AndroidTools-0.0.5/PKG-INFO` & `AndroidTools-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AndroidTools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Android Tools for Python
 Home-page: https://github.com/grayrail000/PyJce
 Author: 1a
 Author-email: grayrail1x3@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AndroidTools-0.0.5/setup.py` & `AndroidTools-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AndroidTools",
-    version="0.0.5",
+    version="0.0.6",
     author="1a",
     author_email="grayrail1x3@gmail.com",
     description="Android Tools for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/grayrail000/PyJce",
     packages=setuptools.find_packages(),
```

### Comparing `AndroidTools-0.0.5/test/test_Jce.py` & `AndroidTools-0.0.6/test/test_Jce.py`

 * *Files identical despite different names*

