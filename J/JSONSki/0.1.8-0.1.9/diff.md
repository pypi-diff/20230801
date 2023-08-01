# Comparing `tmp/JSONSki-0.1.8.tar.gz` & `tmp/JSONSki-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JSONSki-0.1.8.tar", last modified: Tue Aug  1 05:12:05 2023, max compression
+gzip compressed data, was "JSONSki-0.1.9.tar", last modified: Tue Aug  1 16:12:39 2023, max compression
```

## Comparing `JSONSki-0.1.8.tar` & `JSONSki-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 05:12:05.372259 JSONSki-0.1.8/
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 05:12:05.371251 JSONSki-0.1.8/JSONSki.egg-info/
--rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 05:12:05.000000 JSONSki-0.1.8/JSONSki.egg-info/PKG-INFO
--rw-r--r--   0 work       (503) staff       (20)      213 2023-08-01 05:12:05.000000 JSONSki-0.1.8/JSONSki.egg-info/SOURCES.txt
--rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 05:12:05.000000 JSONSki-0.1.8/JSONSki.egg-info/dependency_links.txt
--rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 05:12:05.000000 JSONSki-0.1.8/JSONSki.egg-info/not-zip-safe
--rw-r--r--   0 work       (503) staff       (20)        8 2023-08-01 05:12:05.000000 JSONSki-0.1.8/JSONSki.egg-info/top_level.txt
--rw-r--r--   0 work       (503) staff       (20)     1068 2023-07-28 00:30:06.000000 JSONSki-0.1.8/LICENSE.md
--rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 05:12:05.371898 JSONSki-0.1.8/PKG-INFO
--rw-r--r--   0 work       (503) staff       (20)     5242 2023-08-01 01:42:14.000000 JSONSki-0.1.8/README.md
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 05:12:05.366052 JSONSki-0.1.8/example_python/
--rw-r--r--   0 work       (503) staff       (20)     1375 2023-08-01 04:51:25.000000 JSONSki-0.1.8/example_python/example1.cpp
--rw-r--r--   0 work       (503) staff       (20)       38 2023-08-01 05:12:05.372391 JSONSki-0.1.8/setup.cfg
--rw-r--r--   0 work       (503) staff       (20)     1142 2023-08-01 05:11:17.000000 JSONSki-0.1.8/setup.py
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 16:12:39.314098 JSONSki-0.1.9/
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 16:12:39.313240 JSONSki-0.1.9/JSONSki.egg-info/
+-rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 16:12:39.000000 JSONSki-0.1.9/JSONSki.egg-info/PKG-INFO
+-rw-r--r--   0 work       (503) staff       (20)      213 2023-08-01 16:12:39.000000 JSONSki-0.1.9/JSONSki.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 16:12:39.000000 JSONSki-0.1.9/JSONSki.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 16:12:39.000000 JSONSki-0.1.9/JSONSki.egg-info/not-zip-safe
+-rw-r--r--   0 work       (503) staff       (20)        8 2023-08-01 16:12:39.000000 JSONSki-0.1.9/JSONSki.egg-info/top_level.txt
+-rw-r--r--   0 work       (503) staff       (20)     1068 2023-07-28 00:30:06.000000 JSONSki-0.1.9/LICENSE.md
+-rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 16:12:39.313658 JSONSki-0.1.9/PKG-INFO
+-rw-r--r--   0 work       (503) staff       (20)     5242 2023-08-01 01:42:14.000000 JSONSki-0.1.9/README.md
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 16:12:39.307577 JSONSki-0.1.9/example_python/
+-rw-r--r--   0 work       (503) staff       (20)     1375 2023-08-01 05:53:09.000000 JSONSki-0.1.9/example_python/example1.cpp
+-rw-r--r--   0 work       (503) staff       (20)       38 2023-08-01 16:12:39.314221 JSONSki-0.1.9/setup.cfg
+-rw-r--r--   0 work       (503) staff       (20)     1177 2023-08-01 16:11:31.000000 JSONSki-0.1.9/setup.py
```

### Comparing `JSONSki-0.1.8/JSONSki.egg-info/PKG-INFO` & `JSONSki-0.1.9/JSONSki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JSONSki
-Version: 0.1.8
+Version: 0.1.9
 Summary: JSONSki_Python is the Python binding port for JSONSki
 Home-page: https://github.com/your_username/your_repository
 Author: AutomataLab
 Author-email: zhijia@cs.ucr.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `JSONSki-0.1.8/LICENSE.md` & `JSONSki-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `JSONSki-0.1.8/PKG-INFO` & `JSONSki-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JSONSki
-Version: 0.1.8
+Version: 0.1.9
 Summary: JSONSki_Python is the Python binding port for JSONSki
 Home-page: https://github.com/your_username/your_repository
 Author: AutomataLab
 Author-email: zhijia@cs.ucr.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `JSONSki-0.1.8/README.md` & `JSONSki-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `JSONSki-0.1.8/example_python/example1.cpp` & `JSONSki-0.1.9/example_python/example1.cpp`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-#include <pybind11/pybind11.h>
+
 #include "QueryAutomaton.h"
 
 #include "JSONPathParser.h"
 #include "JSONPathParser.cpp"
 
 
 
@@ -12,15 +12,15 @@
 #include "RecordLoader.h"
 #include "RecordLoader.cpp"
 
 
 #include "QueryProcessor.h"
 #include "QueryProcessor.cpp"
 
-
+#include <pybind11/pybind11.h>
 
 
 
 std::string execute_query(const char* input) {
 // std::string execute_query(char* input) {
 //int main(){
  // char* file_path = "../dataset/twitter_sample_large_record.json";
```

### Comparing `JSONSki-0.1.8/setup.py` & `JSONSki-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, Extension
 
 # Extension module
 JSONSKi_module = Extension(
     'JSONSki',
-    sources=['./example_python/example1.cpp',],
-    include_dirs=['./example_python/pybind11-master/include','./src','../src', '../src/..','/src','src','example_python'],
+    sources=['./example_python/example1.cpp'],
+    include_dirs=['./example_python/pybind11-master/include','./src','../src', '../src/..','/src','src','example_python','./example_python/QueryAutomaton.h'],
      extra_compile_args=['-mavx', '-mavx2', '-mpclmul','-std=c++11']  
 )
 
 # JSONSKi_module = Extension(
 #     'JSONSki',
 #     sources=['example1.cpp'],
 #     include_dirs=['../example_python/pybind11-master/include','../src', '../src/..'],
@@ -22,15 +22,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 # Package information
 setup(
     name='JSONSki',
-    version='0.1.08',
+    version='0.1.09',
     author= AUTHOR,
     author_email= AUTHOR_EMAILS,
     description='JSONSki_Python is the Python binding port for JSONSki',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/your_repository',
     ext_modules=[JSONSKi_module],
```

