# Comparing `tmp/JSONSki-0.1.2.tar.gz` & `tmp/JSONSki-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JSONSki-0.1.2.tar", last modified: Sun Jul 30 00:46:27 2023, max compression
+gzip compressed data, was "JSONSki-0.1.3.tar", last modified: Tue Aug  1 02:19:23 2023, max compression
```

## Comparing `JSONSki-0.1.2.tar` & `JSONSki-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-07-30 00:46:27.301441 JSONSki-0.1.2/
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-07-30 00:46:27.300458 JSONSki-0.1.2/JSONSki.egg-info/
--rw-r--r--   0 work       (503) staff       (20)     5618 2023-07-30 00:46:27.000000 JSONSki-0.1.2/JSONSki.egg-info/PKG-INFO
--rw-r--r--   0 work       (503) staff       (20)      213 2023-07-30 00:46:27.000000 JSONSki-0.1.2/JSONSki.egg-info/SOURCES.txt
--rw-r--r--   0 work       (503) staff       (20)        1 2023-07-30 00:46:27.000000 JSONSki-0.1.2/JSONSki.egg-info/dependency_links.txt
--rw-r--r--   0 work       (503) staff       (20)        1 2023-07-30 00:46:27.000000 JSONSki-0.1.2/JSONSki.egg-info/not-zip-safe
--rw-r--r--   0 work       (503) staff       (20)        8 2023-07-30 00:46:27.000000 JSONSki-0.1.2/JSONSki.egg-info/top_level.txt
--rw-r--r--   0 work       (503) staff       (20)     1068 2023-07-28 00:30:06.000000 JSONSki-0.1.2/LICENSE.md
--rw-r--r--   0 work       (503) staff       (20)     5618 2023-07-30 00:46:27.301097 JSONSki-0.1.2/PKG-INFO
--rw-r--r--   0 work       (503) staff       (20)     5251 2023-03-16 05:53:30.000000 JSONSki-0.1.2/README.md
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-07-30 00:46:27.295305 JSONSki-0.1.2/example_python/
--rw-r--r--   0 work       (503) staff       (20)     1431 2023-07-29 00:06:50.000000 JSONSki-0.1.2/example_python/example1.cpp
--rw-r--r--   0 work       (503) staff       (20)       38 2023-07-30 00:46:27.301572 JSONSki-0.1.2/setup.cfg
--rw-r--r--   0 work       (503) staff       (20)     1145 2023-07-30 00:29:54.000000 JSONSki-0.1.2/setup.py
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 02:19:23.501201 JSONSki-0.1.3/
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 02:19:23.500176 JSONSki-0.1.3/JSONSki.egg-info/
+-rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/PKG-INFO
+-rw-r--r--   0 work       (503) staff       (20)      213 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/not-zip-safe
+-rw-r--r--   0 work       (503) staff       (20)        8 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/top_level.txt
+-rw-r--r--   0 work       (503) staff       (20)     1068 2023-07-28 00:30:06.000000 JSONSki-0.1.3/LICENSE.md
+-rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 02:19:23.500849 JSONSki-0.1.3/PKG-INFO
+-rw-r--r--   0 work       (503) staff       (20)     5242 2023-08-01 01:42:14.000000 JSONSki-0.1.3/README.md
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 02:19:23.494941 JSONSki-0.1.3/example_python/
+-rw-r--r--   0 work       (503) staff       (20)     1407 2023-08-01 02:11:03.000000 JSONSki-0.1.3/example_python/example1.cpp
+-rw-r--r--   0 work       (503) staff       (20)       38 2023-08-01 02:19:23.501342 JSONSki-0.1.3/setup.cfg
+-rw-r--r--   0 work       (503) staff       (20)     1124 2023-08-01 02:11:37.000000 JSONSki-0.1.3/setup.py
```

### Comparing `JSONSki-0.1.2/JSONSki.egg-info/PKG-INFO` & `JSONSki-0.1.3/JSONSki.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: JSONSki
-Version: 0.1.2
+Version: 0.1.3
 Summary: JSONSki_Python is the Python binding port for JSONSki
 Home-page: https://github.com/your_username/your_repository
-Author: ('AutomataLab', 'Zhija Zhao', 'Kapilan Ramasamy')
+Author: AutomataLab
 Author-email: zhijia@cs.ucr.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 [![CircleCI](https://circleci.com/gh/AutomataLab/JSONSki_nodejs.svg?style=shield&circle-token=daf002fef2464bc57675d6a3dc072485f27b7bbc)](https://app.circleci.com/pipelines/github/AutomataLab/JSONSki_nodejs)  ![GitHub](https://img.shields.io/github/license/AutomataLab/JSONSki_nodejs)
 ![npm](https://img.shields.io/npm/dt/jsonski?label=npm%20downloads)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/AutomataLab/jsonski_nodejs)
 ![](https://img.shields.io/badge/linux-macos-green)
 
-# JSONSki_NodeJs
-JSONSki_Nodejs is the Node.Js (Javascript) binding port for JSONSki
+# JSONSki
+JSONSki is the Python binding port for JSONSki written in c++ found here here - https://github.com/AutomataLab/JSONSki
+
+# What is it?
 
 JSONSki is **a streaming JSONPath processor** with **fast-forward** functionality. During the streaming, it can automatically fast-forward over certain JSON substructures that are irrelavent to the query evaluation, without parsing them in detail. To make the fast-forward efficient, JSONSki features a highly bit-parallel solution that intensively utilizes bitwise and SIMD operations that are prevelent on modern CPUs to implement the fast-forward APIs. 
 
 ## NPM Package
 You can download the npm package from here - https://www.npmjs.com/package/jsonski
 
 ## Installation
 ```
-npm i jsonski
+pip install JSONSki
 ```
 
 ## Quick Start
 
 ```
 const JSki = require('jsonski')
 console.log(JSki.JSONSkiParser("$.features[150].actor.login", "datasets/test.json"));
@@ -49,16 +51,14 @@
 - C++ Compiler: g++ (7.4.0 or higher)
 
 
 ### Software requirements
 
 Before starting to use Node-API you need to assure you have the following prerequisites:
 
-- Node.JS (v14 and above) see: [Installing Node.js](https://nodejs.org/)
-
 - Python (v3.9) see: [Installing Python](https://www.python.org/downloads/release/python-3100/)
 
 - C++ : g++ (v7.4.0 and above) see: [Installing C++](https://gcc.gnu.org/install/)
 
 
 ## Getting Started with Querying using JSONSki
 ### JSONPath
```

### Comparing `JSONSki-0.1.2/LICENSE.md` & `JSONSki-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `JSONSki-0.1.2/PKG-INFO` & `JSONSki-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: JSONSki
-Version: 0.1.2
+Version: 0.1.3
 Summary: JSONSki_Python is the Python binding port for JSONSki
 Home-page: https://github.com/your_username/your_repository
-Author: ('AutomataLab', 'Zhija Zhao', 'Kapilan Ramasamy')
+Author: AutomataLab
 Author-email: zhijia@cs.ucr.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 [![CircleCI](https://circleci.com/gh/AutomataLab/JSONSki_nodejs.svg?style=shield&circle-token=daf002fef2464bc57675d6a3dc072485f27b7bbc)](https://app.circleci.com/pipelines/github/AutomataLab/JSONSki_nodejs)  ![GitHub](https://img.shields.io/github/license/AutomataLab/JSONSki_nodejs)
 ![npm](https://img.shields.io/npm/dt/jsonski?label=npm%20downloads)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/AutomataLab/jsonski_nodejs)
 ![](https://img.shields.io/badge/linux-macos-green)
 
-# JSONSki_NodeJs
-JSONSki_Nodejs is the Node.Js (Javascript) binding port for JSONSki
+# JSONSki
+JSONSki is the Python binding port for JSONSki written in c++ found here here - https://github.com/AutomataLab/JSONSki
+
+# What is it?
 
 JSONSki is **a streaming JSONPath processor** with **fast-forward** functionality. During the streaming, it can automatically fast-forward over certain JSON substructures that are irrelavent to the query evaluation, without parsing them in detail. To make the fast-forward efficient, JSONSki features a highly bit-parallel solution that intensively utilizes bitwise and SIMD operations that are prevelent on modern CPUs to implement the fast-forward APIs. 
 
 ## NPM Package
 You can download the npm package from here - https://www.npmjs.com/package/jsonski
 
 ## Installation
 ```
-npm i jsonski
+pip install JSONSki
 ```
 
 ## Quick Start
 
 ```
 const JSki = require('jsonski')
 console.log(JSki.JSONSkiParser("$.features[150].actor.login", "datasets/test.json"));
@@ -49,16 +51,14 @@
 - C++ Compiler: g++ (7.4.0 or higher)
 
 
 ### Software requirements
 
 Before starting to use Node-API you need to assure you have the following prerequisites:
 
-- Node.JS (v14 and above) see: [Installing Node.js](https://nodejs.org/)
-
 - Python (v3.9) see: [Installing Python](https://www.python.org/downloads/release/python-3100/)
 
 - C++ : g++ (v7.4.0 and above) see: [Installing C++](https://gcc.gnu.org/install/)
 
 
 ## Getting Started with Querying using JSONSki
 ### JSONPath
```

### Comparing `JSONSki-0.1.2/README.md` & `JSONSki-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [![CircleCI](https://circleci.com/gh/AutomataLab/JSONSki_nodejs.svg?style=shield&circle-token=daf002fef2464bc57675d6a3dc072485f27b7bbc)](https://app.circleci.com/pipelines/github/AutomataLab/JSONSki_nodejs)  ![GitHub](https://img.shields.io/github/license/AutomataLab/JSONSki_nodejs)
 ![npm](https://img.shields.io/npm/dt/jsonski?label=npm%20downloads)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/AutomataLab/jsonski_nodejs)
 ![](https://img.shields.io/badge/linux-macos-green)
 
-# JSONSki_NodeJs
-JSONSki_Nodejs is the Node.Js (Javascript) binding port for JSONSki
+# JSONSki
+JSONSki is the Python binding port for JSONSki written in c++ found here here - https://github.com/AutomataLab/JSONSki
+
+# What is it?
 
 JSONSki is **a streaming JSONPath processor** with **fast-forward** functionality. During the streaming, it can automatically fast-forward over certain JSON substructures that are irrelavent to the query evaluation, without parsing them in detail. To make the fast-forward efficient, JSONSki features a highly bit-parallel solution that intensively utilizes bitwise and SIMD operations that are prevelent on modern CPUs to implement the fast-forward APIs. 
 
 ## NPM Package
 You can download the npm package from here - https://www.npmjs.com/package/jsonski
 
 ## Installation
 ```
-npm i jsonski
+pip install JSONSki
 ```
 
 ## Quick Start
 
 ```
 const JSki = require('jsonski')
 console.log(JSki.JSONSkiParser("$.features[150].actor.login", "datasets/test.json"));
@@ -37,16 +39,14 @@
 - C++ Compiler: g++ (7.4.0 or higher)
 
 
 ### Software requirements
 
 Before starting to use Node-API you need to assure you have the following prerequisites:
 
-- Node.JS (v14 and above) see: [Installing Node.js](https://nodejs.org/)
-
 - Python (v3.9) see: [Installing Python](https://www.python.org/downloads/release/python-3100/)
 
 - C++ : g++ (v7.4.0 and above) see: [Installing C++](https://gcc.gnu.org/install/)
 
 
 ## Getting Started with Querying using JSONSki
 ### JSONPath
```

### Comparing `JSONSki-0.1.2/example_python/example1.cpp` & `JSONSki-0.1.3/example_python/example1.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 
-#include "../src/QueryAutomaton.h"
+#include "src/QueryAutomaton.h"
 
-#include "../src/JSONPathParser.h"
-#include "../src/JSONPathParser.cpp"
+#include "src/JSONPathParser.h"
+#include "src/JSONPathParser.cpp"
 
 
 
-#include "../src/Records.h"
+#include "src/Records.h"
 
-#include "../src/RecordLoader.h"
-#include "../src/RecordLoader.cpp"
+#include "src/RecordLoader.h"
+#include "src/RecordLoader.cpp"
 
 
-#include "../src/QueryProcessor.h"
-#include "../src/QueryProcessor.cpp"
+#include "src/QueryProcessor.h"
+#include "src/QueryProcessor.cpp"
 #include <pybind11/pybind11.h>
 
 
 
 
 std::string execute_query(const char* input) {
 // std::string execute_query(char* input) {
```

### Comparing `JSONSki-0.1.2/setup.py` & `JSONSki-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from setuptools import setup, Extension
 
 # Extension module
 JSONSKi_module = Extension(
     'JSONSki',
     sources=['./example_python/example1.cpp'],
-    include_dirs=['./example_python/pybind11-master/include','./src','../src', '../src/..'],
+    include_dirs=['./example_python/pybind11-master/include','./src','../src', '../src/..','/src','src'],
      extra_compile_args=['-mavx', '-mavx2', '-mpclmul','-std=c++11']  
 )
 
 # JSONSKi_module = Extension(
 #     'JSONSki',
 #     sources=['example1.cpp'],
 #     include_dirs=['../example_python/pybind11-master/include','../src', '../src/..'],
 #      extra_compile_args=['-mavx', '-mavx2', '-mpclmul','-std=c++11']  
 # )
 
-AUTHOR = 'AutomataLab', 'Zhija Zhao', 'Kapilan Ramasamy'
+AUTHOR = 'AutomataLab'
 
 AUTHOR_EMAILS = 'zhijia@cs.ucr.edu'
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 # Package information
 setup(
     name='JSONSki',
-    version='0.1.02',
+    version='0.1.03',
     author= AUTHOR,
     author_email= AUTHOR_EMAILS,
     description='JSONSki_Python is the Python binding port for JSONSki',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/your_repository',
     ext_modules=[JSONSKi_module],
```

