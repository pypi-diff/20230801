# Comparing `tmp/http-stream-xml-1.3.6.tar.gz` & `tmp/http-stream-xml-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http-stream-xml-1.3.6.tar", last modified: Tue Aug  1 08:32:08 2023, max compression
+gzip compressed data, was "http-stream-xml-1.3.7.tar", last modified: Tue Aug  1 08:45:42 2023, max compression
```

## Comparing `http-stream-xml-1.3.6.tar` & `http-stream-xml-1.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:08.654310 http-stream-xml-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 08:32:08.654310 http-stream-xml-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 08:32:08.654310 http-stream-xml-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:08.650310 http-stream-xml-1.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:08.654310 http-stream-xml-1.3.6/src/http_stream_xml/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/src/http_stream_xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/src/http_stream_xml/entrez.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/src/http_stream_xml/entrez_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/src/http_stream_xml/entrez_socket_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/src/http_stream_xml/socket_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/src/http_stream_xml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-01 08:31:54.000000 http-stream-xml-1.3.6/src/http_stream_xml/xml_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:32:08.654310 http-stream-xml-1.3.6/src/http_stream_xml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 08:32:08.000000 http-stream-xml-1.3.6/src/http_stream_xml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-01 08:32:08.000000 http-stream-xml-1.3.6/src/http_stream_xml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:32:08.000000 http-stream-xml-1.3.6/src/http_stream_xml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 08:32:08.000000 http-stream-xml-1.3.6/src/http_stream_xml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 08:32:08.000000 http-stream-xml-1.3.6/src/http_stream_xml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 08:32:08.000000 http-stream-xml-1.3.6/src/http_stream_xml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:42.509289 http-stream-xml-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 08:45:42.509289 http-stream-xml-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 08:45:42.513289 http-stream-xml-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:42.505289 http-stream-xml-1.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:42.509289 http-stream-xml-1.3.7/src/http_stream_xml/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/src/http_stream_xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/src/http_stream_xml/entrez.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/src/http_stream_xml/entrez_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/src/http_stream_xml/entrez_socket_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/src/http_stream_xml/socket_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/src/http_stream_xml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-01 08:45:30.000000 http-stream-xml-1.3.7/src/http_stream_xml/xml_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:45:42.509289 http-stream-xml-1.3.7/src/http_stream_xml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 08:45:42.000000 http-stream-xml-1.3.7/src/http_stream_xml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-01 08:45:42.000000 http-stream-xml-1.3.7/src/http_stream_xml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:45:42.000000 http-stream-xml-1.3.7/src/http_stream_xml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 08:45:42.000000 http-stream-xml-1.3.7/src/http_stream_xml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 08:45:42.000000 http-stream-xml-1.3.7/src/http_stream_xml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 08:45:42.000000 http-stream-xml-1.3.7/src/http_stream_xml.egg-info/top_level.txt
```

### Comparing `http-stream-xml-1.3.6/LICENSE.txt` & `http-stream-xml-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.6/PKG-INFO` & `http-stream-xml-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http-stream-xml
-Version: 1.3.6
+Version: 1.3.7
 Summary: Parse XML in HTTP response on the fly, by chunks.
 Home-page: https://http-stream-xml.readthedocs.io/en/latest/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: http stream xml chunked
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `http-stream-xml-1.3.6/README.rst` & `http-stream-xml-1.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.6/setup.py` & `http-stream-xml-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.6/src/http_stream_xml/entrez.py` & `http-stream-xml-1.3.7/src/http_stream_xml/entrez.py`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.6/src/http_stream_xml/entrez_example.py` & `http-stream-xml-1.3.7/src/http_stream_xml/entrez_example.py`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.6/src/http_stream_xml/entrez_socket_example.py` & `http-stream-xml-1.3.7/src/http_stream_xml/entrez_socket_example.py`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.6/src/http_stream_xml/socket_stream.py` & `http-stream-xml-1.3.7/src/http_stream_xml/socket_stream.py`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.6/src/http_stream_xml/xml_stream.py` & `http-stream-xml-1.3.7/src/http_stream_xml/xml_stream.py`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.6/src/http_stream_xml.egg-info/PKG-INFO` & `http-stream-xml-1.3.7/src/http_stream_xml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http-stream-xml
-Version: 1.3.6
+Version: 1.3.7
 Summary: Parse XML in HTTP response on the fly, by chunks.
 Home-page: https://http-stream-xml.readthedocs.io/en/latest/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: http stream xml chunked
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `http-stream-xml-1.3.6/src/http_stream_xml.egg-info/SOURCES.txt` & `http-stream-xml-1.3.7/src/http_stream_xml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

