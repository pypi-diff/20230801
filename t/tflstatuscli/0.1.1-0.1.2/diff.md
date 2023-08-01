# Comparing `tmp/tflstatuscli-0.1.1.tar.gz` & `tmp/tflstatuscli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tflstatuscli-0.1.1.tar", max compression
+gzip compressed data, was "tflstatuscli-0.1.2.tar", max compression
```

## Comparing `tflstatuscli-0.1.1.tar` & `tflstatuscli-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      179 2023-08-01 18:28:17.345268 tflstatuscli-0.1.1/README.md
--rw-r--r--   0        0        0      461 2023-08-01 18:32:06.598386 tflstatuscli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 22:24:52.823601 tflstatuscli-0.1.1/tflstatuscli/__init__.py
--rwxr-xr-x   0        0        0     2363 2023-08-01 18:02:56.312839 tflstatuscli-0.1.1/tflstatuscli/tflstatuscli.py
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 tflstatuscli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-08-01 18:43:56.625056 tflstatuscli-0.1.2/README.md
+-rw-r--r--   0        0        0      461 2023-08-01 20:21:40.777857 tflstatuscli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 22:24:52.823601 tflstatuscli-0.1.2/tflstatuscli/__init__.py
+-rwxr-xr-x   0        0        0     2363 2023-08-01 18:02:56.312839 tflstatuscli-0.1.2/tflstatuscli/tflstatuscli.py
+-rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 tflstatuscli-0.1.2/PKG-INFO
```

### Comparing `tflstatuscli-0.1.1/tflstatuscli/tflstatuscli.py` & `tflstatuscli-0.1.2/tflstatuscli/tflstatuscli.py`

 * *Files identical despite different names*

### Comparing `tflstatuscli-0.1.1/PKG-INFO` & `tflstatuscli-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,52 @@
 Metadata-Version: 2.1
 Name: tflstatuscli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Query TFL tube line status
 Author: stevenb92
 Author-email: stevenb92@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.5.2,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-## tflstatuscli
+# tflstatuscli
 tflstatuscli is a Python CLI written using the Typer CLI framework for querying the TFL Tube line statuses
 
-# Installation
+## Installation
 ```bash
 pip install tflstatuscli
 ```
 
+## Usage
+### Show status of all tube lines
+```bash
+tflcli status   
+```
 
+### Show status of particular tube line
+```bash
+tflcli status --line <line_name>
+```
+NOTE: When searching a particular tube line, validity is checked against the TFL APIs list of tube lines which at the time of writing this includes;
+- Bakerloo 
+- Central            
+- Circle             
+- District           
+- Hammersmith & City 
+- Jubilee            
+- Metropolitan                                         
+- Northern           
+- Piccadilly         
+- Victoria           
+- Waterloo & City
 
+### Show all disruptions on TFL tube lines
+```bash
+tflcli disruptions
+```
```

