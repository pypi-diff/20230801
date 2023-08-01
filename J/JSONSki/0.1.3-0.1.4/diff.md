# Comparing `tmp/JSONSki-0.1.3.tar.gz` & `tmp/JSONSki-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JSONSki-0.1.3.tar", last modified: Tue Aug  1 02:19:23 2023, max compression
+gzip compressed data, was "JSONSki-0.1.4.tar", last modified: Tue Aug  1 03:43:58 2023, max compression
```

## Comparing `JSONSki-0.1.3.tar` & `JSONSki-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 02:19:23.501201 JSONSki-0.1.3/
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 02:19:23.500176 JSONSki-0.1.3/JSONSki.egg-info/
--rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/PKG-INFO
--rw-r--r--   0 work       (503) staff       (20)      213 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/SOURCES.txt
--rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/dependency_links.txt
--rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/not-zip-safe
--rw-r--r--   0 work       (503) staff       (20)        8 2023-08-01 02:19:23.000000 JSONSki-0.1.3/JSONSki.egg-info/top_level.txt
--rw-r--r--   0 work       (503) staff       (20)     1068 2023-07-28 00:30:06.000000 JSONSki-0.1.3/LICENSE.md
--rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 02:19:23.500849 JSONSki-0.1.3/PKG-INFO
--rw-r--r--   0 work       (503) staff       (20)     5242 2023-08-01 01:42:14.000000 JSONSki-0.1.3/README.md
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 02:19:23.494941 JSONSki-0.1.3/example_python/
--rw-r--r--   0 work       (503) staff       (20)     1407 2023-08-01 02:11:03.000000 JSONSki-0.1.3/example_python/example1.cpp
--rw-r--r--   0 work       (503) staff       (20)       38 2023-08-01 02:19:23.501342 JSONSki-0.1.3/setup.cfg
--rw-r--r--   0 work       (503) staff       (20)     1124 2023-08-01 02:11:37.000000 JSONSki-0.1.3/setup.py
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 03:43:58.597238 JSONSki-0.1.4/
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 03:43:58.596215 JSONSki-0.1.4/JSONSki.egg-info/
+-rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 03:43:58.000000 JSONSki-0.1.4/JSONSki.egg-info/PKG-INFO
+-rw-r--r--   0 work       (503) staff       (20)      213 2023-08-01 03:43:58.000000 JSONSki-0.1.4/JSONSki.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 03:43:58.000000 JSONSki-0.1.4/JSONSki.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 03:43:58.000000 JSONSki-0.1.4/JSONSki.egg-info/not-zip-safe
+-rw-r--r--   0 work       (503) staff       (20)        8 2023-08-01 03:43:58.000000 JSONSki-0.1.4/JSONSki.egg-info/top_level.txt
+-rw-r--r--   0 work       (503) staff       (20)     1068 2023-07-28 00:30:06.000000 JSONSki-0.1.4/LICENSE.md
+-rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 03:43:58.596871 JSONSki-0.1.4/PKG-INFO
+-rw-r--r--   0 work       (503) staff       (20)     5242 2023-08-01 01:42:14.000000 JSONSki-0.1.4/README.md
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 03:43:58.591094 JSONSki-0.1.4/example_python/
+-rw-r--r--   0 work       (503) staff       (20)     1375 2023-08-01 03:32:14.000000 JSONSki-0.1.4/example_python/example1.cpp
+-rw-r--r--   0 work       (503) staff       (20)       38 2023-08-01 03:43:58.597371 JSONSki-0.1.4/setup.cfg
+-rw-r--r--   0 work       (503) staff       (20)     1124 2023-08-01 03:38:56.000000 JSONSki-0.1.4/setup.py
```

### Comparing `JSONSki-0.1.3/JSONSki.egg-info/PKG-INFO` & `JSONSki-0.1.4/JSONSki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JSONSki
-Version: 0.1.3
+Version: 0.1.4
 Summary: JSONSki_Python is the Python binding port for JSONSki
 Home-page: https://github.com/your_username/your_repository
 Author: AutomataLab
 Author-email: zhijia@cs.ucr.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `JSONSki-0.1.3/LICENSE.md` & `JSONSki-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `JSONSki-0.1.3/PKG-INFO` & `JSONSki-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JSONSki
-Version: 0.1.3
+Version: 0.1.4
 Summary: JSONSki_Python is the Python binding port for JSONSki
 Home-page: https://github.com/your_username/your_repository
 Author: AutomataLab
 Author-email: zhijia@cs.ucr.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `JSONSki-0.1.3/README.md` & `JSONSki-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `JSONSki-0.1.3/example_python/example1.cpp` & `JSONSki-0.1.4/example_python/example1.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 
-#include "src/QueryAutomaton.h"
+#include "QueryAutomaton.h"
 
-#include "src/JSONPathParser.h"
-#include "src/JSONPathParser.cpp"
+#include "JSONPathParser.h"
+#include "JSONPathParser.cpp"
 
 
 
-#include "src/Records.h"
+#include "Records.h"
 
-#include "src/RecordLoader.h"
-#include "src/RecordLoader.cpp"
+#include "RecordLoader.h"
+#include "RecordLoader.cpp"
 
 
-#include "src/QueryProcessor.h"
-#include "src/QueryProcessor.cpp"
+#include "QueryProcessor.h"
+#include "QueryProcessor.cpp"
 #include <pybind11/pybind11.h>
 
 
 
 
 std::string execute_query(const char* input) {
 // std::string execute_query(char* input) {
```

### Comparing `JSONSki-0.1.3/setup.py` & `JSONSki-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 # Package information
 setup(
     name='JSONSki',
-    version='0.1.03',
+    version='0.1.04',
     author= AUTHOR,
     author_email= AUTHOR_EMAILS,
     description='JSONSki_Python is the Python binding port for JSONSki',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/your_repository',
     ext_modules=[JSONSKi_module],
```

