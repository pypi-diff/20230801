# Comparing `tmp/http-stream-xml-1.3.4.tar.gz` & `tmp/http-stream-xml-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http-stream-xml-1.3.4.tar", last modified: Wed Apr 26 04:50:41 2023, max compression
+gzip compressed data, was "http-stream-xml-1.3.5.tar", last modified: Tue Aug  1 04:31:25 2023, max compression
```

## Comparing `http-stream-xml-1.3.4.tar` & `http-stream-xml-1.3.5.tar`

### file list

```diff
@@ -1,11 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:50:41.182674 http-stream-xml-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 04:50:29.000000 http-stream-xml-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-26 04:50:41.182674 http-stream-xml-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-26 04:50:29.000000 http-stream-xml-1.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:50:41.182674 http-stream-xml-1.3.4/http_stream_xml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-26 04:50:41.000000 http-stream-xml-1.3.4/http_stream_xml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-26 04:50:41.000000 http-stream-xml-1.3.4/http_stream_xml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:50:41.000000 http-stream-xml-1.3.4/http_stream_xml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:50:41.000000 http-stream-xml-1.3.4/http_stream_xml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 04:50:41.182674 http-stream-xml-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-26 04:50:29.000000 http-stream-xml-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:31:25.939100 http-stream-xml-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-01 04:31:25.939100 http-stream-xml-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 04:31:25.939100 http-stream-xml-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:31:25.935100 http-stream-xml-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:31:25.939100 http-stream-xml-1.3.5/src/http_stream_xml/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/src/http_stream_xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/src/http_stream_xml/entrez.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/src/http_stream_xml/entrez_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/src/http_stream_xml/entrez_socket_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/src/http_stream_xml/socket_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/src/http_stream_xml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-01 04:31:16.000000 http-stream-xml-1.3.5/src/http_stream_xml/xml_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:31:25.939100 http-stream-xml-1.3.5/src/http_stream_xml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-01 04:31:25.000000 http-stream-xml-1.3.5/src/http_stream_xml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-01 04:31:25.000000 http-stream-xml-1.3.5/src/http_stream_xml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:31:25.000000 http-stream-xml-1.3.5/src/http_stream_xml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 04:31:25.000000 http-stream-xml-1.3.5/src/http_stream_xml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 04:31:25.000000 http-stream-xml-1.3.5/src/http_stream_xml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 04:31:25.000000 http-stream-xml-1.3.5/src/http_stream_xml.egg-info/top_level.txt
```

### Comparing `http-stream-xml-1.3.4/PKG-INFO` & `http-stream-xml-1.3.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: http-stream-xml
-Version: 1.3.4
-Summary: Parse XML in HTTP response on the fly, by chunks
+Version: 1.3.5
+Summary: Parse XML in HTTP response on the fly, by chunks.
 Home-page: https://http-stream-xml.readthedocs.io/en/latest/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: http stream xml chunked
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 
 http-stream-xml
 ===============
 
-|made_with_python| |build_status| |pypi_version| |pypi_license| |readthedocs|
+|made_with_python| |build_status| |coverage| |codecov| |pypi_version| |pypi_license| |readthedocs|
 
 Parse XML in HTTP response on the fly, by chunks.
 
 It could be `HTTP protocol chunks <https://en.wikipedia.org/wiki/Chunked_transfer_encoding>`_
 Or just partial download of big HTTP response.
 
 
@@ -32,15 +34,15 @@
     pip install http-stream-xml --upgrade
 
 Documentation
 -------------
 `Documentation <https://http-stream-xml.sorokin.engineer/en/latest/>`_
 
 .. |build_status| image:: https://github.com/andgineer/redis-redirect//workflows/ci/badge.svg
-    :target: (https://github.com/andgineer/redis-redirect//actions
+    :target: https://github.com/andgineer/redis-redirect//actions
     :alt: Latest release
 
 .. |pypi_version| image:: https://img.shields.io/pypi/v/http-stream-xml.svg?style=flat-square
     :target: https://pypi.org/p/http-stream-xml
     :alt: Latest release
 
 .. |pypi_license| image:: https://img.shields.io/pypi/l/http-stream-xml.svg?style=flat-square
@@ -50,7 +52,15 @@
 .. |readthedocs| image:: https://readthedocs.org/projects/http-stream-xml/badge/?version=latest
     :target: https://http-stream-xml.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |made_with_python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
     :target: https://www.python.org/
     :alt: Made with Python
+
+.. |codecov| image:: https://codecov.io/gh/andgineer/http-stream-xml/branch/master/graph/badge.svg
+    :target: https://app.codecov.io/gh/andgineer/http-stream-xml/tree/master/src%2Fhttp_stream_xml
+    :alt: Code coverage
+
+.. |coverage| image:: https://raw.githubusercontent.com/andgineer/http-stream-xml/python-coverage-comment-action-data/badge.svg
+    :target: https://htmlpreview.github.io/?https://github.com/andgineer/http-stream-xml/blob/python-coverage-comment-action-data/htmlcov/index.html
+    :alt: Coverage report
```

### Comparing `http-stream-xml-1.3.4/README.rst` & `http-stream-xml-1.3.5/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 http-stream-xml
 ===============
 
-|made_with_python| |build_status| |pypi_version| |pypi_license| |readthedocs|
+|made_with_python| |build_status| |coverage| |codecov| |pypi_version| |pypi_license| |readthedocs|
 
 Parse XML in HTTP response on the fly, by chunks.
 
 It could be `HTTP protocol chunks <https://en.wikipedia.org/wiki/Chunked_transfer_encoding>`_
 Or just partial download of big HTTP response.
 
 
@@ -19,15 +19,15 @@
     pip install http-stream-xml --upgrade
 
 Documentation
 -------------
 `Documentation <https://http-stream-xml.sorokin.engineer/en/latest/>`_
 
 .. |build_status| image:: https://github.com/andgineer/redis-redirect//workflows/ci/badge.svg
-    :target: (https://github.com/andgineer/redis-redirect//actions
+    :target: https://github.com/andgineer/redis-redirect//actions
     :alt: Latest release
 
 .. |pypi_version| image:: https://img.shields.io/pypi/v/http-stream-xml.svg?style=flat-square
     :target: https://pypi.org/p/http-stream-xml
     :alt: Latest release
 
 .. |pypi_license| image:: https://img.shields.io/pypi/l/http-stream-xml.svg?style=flat-square
@@ -37,7 +37,15 @@
 .. |readthedocs| image:: https://readthedocs.org/projects/http-stream-xml/badge/?version=latest
     :target: https://http-stream-xml.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |made_with_python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
     :target: https://www.python.org/
     :alt: Made with Python
+
+.. |codecov| image:: https://codecov.io/gh/andgineer/http-stream-xml/branch/master/graph/badge.svg
+    :target: https://app.codecov.io/gh/andgineer/http-stream-xml/tree/master/src%2Fhttp_stream_xml
+    :alt: Code coverage
+
+.. |coverage| image:: https://raw.githubusercontent.com/andgineer/http-stream-xml/python-coverage-comment-action-data/badge.svg
+    :target: https://htmlpreview.github.io/?https://github.com/andgineer/http-stream-xml/blob/python-coverage-comment-action-data/htmlcov/index.html
+    :alt: Coverage report
```

### Comparing `http-stream-xml-1.3.4/http_stream_xml.egg-info/PKG-INFO` & `http-stream-xml-1.3.5/src/http_stream_xml.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: http-stream-xml
-Version: 1.3.4
-Summary: Parse XML in HTTP response on the fly, by chunks
+Version: 1.3.5
+Summary: Parse XML in HTTP response on the fly, by chunks.
 Home-page: https://http-stream-xml.readthedocs.io/en/latest/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: http stream xml chunked
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 
 http-stream-xml
 ===============
 
-|made_with_python| |build_status| |pypi_version| |pypi_license| |readthedocs|
+|made_with_python| |build_status| |coverage| |codecov| |pypi_version| |pypi_license| |readthedocs|
 
 Parse XML in HTTP response on the fly, by chunks.
 
 It could be `HTTP protocol chunks <https://en.wikipedia.org/wiki/Chunked_transfer_encoding>`_
 Or just partial download of big HTTP response.
 
 
@@ -32,15 +34,15 @@
     pip install http-stream-xml --upgrade
 
 Documentation
 -------------
 `Documentation <https://http-stream-xml.sorokin.engineer/en/latest/>`_
 
 .. |build_status| image:: https://github.com/andgineer/redis-redirect//workflows/ci/badge.svg
-    :target: (https://github.com/andgineer/redis-redirect//actions
+    :target: https://github.com/andgineer/redis-redirect//actions
     :alt: Latest release
 
 .. |pypi_version| image:: https://img.shields.io/pypi/v/http-stream-xml.svg?style=flat-square
     :target: https://pypi.org/p/http-stream-xml
     :alt: Latest release
 
 .. |pypi_license| image:: https://img.shields.io/pypi/l/http-stream-xml.svg?style=flat-square
@@ -50,7 +52,15 @@
 .. |readthedocs| image:: https://readthedocs.org/projects/http-stream-xml/badge/?version=latest
     :target: https://http-stream-xml.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |made_with_python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
     :target: https://www.python.org/
     :alt: Made with Python
+
+.. |codecov| image:: https://codecov.io/gh/andgineer/http-stream-xml/branch/master/graph/badge.svg
+    :target: https://app.codecov.io/gh/andgineer/http-stream-xml/tree/master/src%2Fhttp_stream_xml
+    :alt: Code coverage
+
+.. |coverage| image:: https://raw.githubusercontent.com/andgineer/http-stream-xml/python-coverage-comment-action-data/badge.svg
+    :target: https://htmlpreview.github.io/?https://github.com/andgineer/http-stream-xml/blob/python-coverage-comment-action-data/htmlcov/index.html
+    :alt: Coverage report
```

