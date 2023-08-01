# Comparing `tmp/JSONSki-0.1.6.tar.gz` & `tmp/JSONSki-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JSONSki-0.1.6.tar", last modified: Tue Aug  1 04:58:19 2023, max compression
+gzip compressed data, was "JSONSki-0.1.7.tar", last modified: Tue Aug  1 05:03:55 2023, max compression
```

## Comparing `JSONSki-0.1.6.tar` & `JSONSki-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 04:58:19.512331 JSONSki-0.1.6/
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 04:58:19.511322 JSONSki-0.1.6/JSONSki.egg-info/
--rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 04:58:19.000000 JSONSki-0.1.6/JSONSki.egg-info/PKG-INFO
--rw-r--r--   0 work       (503) staff       (20)      213 2023-08-01 04:58:19.000000 JSONSki-0.1.6/JSONSki.egg-info/SOURCES.txt
--rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 04:58:19.000000 JSONSki-0.1.6/JSONSki.egg-info/dependency_links.txt
--rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 04:58:19.000000 JSONSki-0.1.6/JSONSki.egg-info/not-zip-safe
--rw-r--r--   0 work       (503) staff       (20)        8 2023-08-01 04:58:19.000000 JSONSki-0.1.6/JSONSki.egg-info/top_level.txt
--rw-r--r--   0 work       (503) staff       (20)     1068 2023-07-28 00:30:06.000000 JSONSki-0.1.6/LICENSE.md
--rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 04:58:19.511981 JSONSki-0.1.6/PKG-INFO
--rw-r--r--   0 work       (503) staff       (20)     5242 2023-08-01 01:42:14.000000 JSONSki-0.1.6/README.md
-drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 04:58:19.505722 JSONSki-0.1.6/example_python/
--rw-r--r--   0 work       (503) staff       (20)     1375 2023-08-01 04:51:25.000000 JSONSki-0.1.6/example_python/example1.cpp
--rw-r--r--   0 work       (503) staff       (20)       38 2023-08-01 04:58:19.512480 JSONSki-0.1.6/setup.cfg
--rw-r--r--   0 work       (503) staff       (20)     1197 2023-08-01 04:56:40.000000 JSONSki-0.1.6/setup.py
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 05:03:55.602711 JSONSki-0.1.7/
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 05:03:55.601683 JSONSki-0.1.7/JSONSki.egg-info/
+-rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 05:03:55.000000 JSONSki-0.1.7/JSONSki.egg-info/PKG-INFO
+-rw-r--r--   0 work       (503) staff       (20)      213 2023-08-01 05:03:55.000000 JSONSki-0.1.7/JSONSki.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 05:03:55.000000 JSONSki-0.1.7/JSONSki.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (503) staff       (20)        1 2023-08-01 05:03:55.000000 JSONSki-0.1.7/JSONSki.egg-info/not-zip-safe
+-rw-r--r--   0 work       (503) staff       (20)        8 2023-08-01 05:03:55.000000 JSONSki-0.1.7/JSONSki.egg-info/top_level.txt
+-rw-r--r--   0 work       (503) staff       (20)     1068 2023-07-28 00:30:06.000000 JSONSki-0.1.7/LICENSE.md
+-rw-r--r--   0 work       (503) staff       (20)     5571 2023-08-01 05:03:55.602338 JSONSki-0.1.7/PKG-INFO
+-rw-r--r--   0 work       (503) staff       (20)     5242 2023-08-01 01:42:14.000000 JSONSki-0.1.7/README.md
+drwxr-xr-x   0 work       (503) staff       (20)        0 2023-08-01 05:03:55.596323 JSONSki-0.1.7/example_python/
+-rw-r--r--   0 work       (503) staff       (20)     1375 2023-08-01 04:51:25.000000 JSONSki-0.1.7/example_python/example1.cpp
+-rw-r--r--   0 work       (503) staff       (20)       38 2023-08-01 05:03:55.602848 JSONSki-0.1.7/setup.cfg
+-rw-r--r--   0 work       (503) staff       (20)     1178 2023-08-01 05:03:07.000000 JSONSki-0.1.7/setup.py
```

### Comparing `JSONSki-0.1.6/JSONSki.egg-info/PKG-INFO` & `JSONSki-0.1.7/JSONSki.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JSONSki
-Version: 0.1.6
+Version: 0.1.7
 Summary: JSONSki_Python is the Python binding port for JSONSki
 Home-page: https://github.com/your_username/your_repository
 Author: AutomataLab
 Author-email: zhijia@cs.ucr.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `JSONSki-0.1.6/LICENSE.md` & `JSONSki-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `JSONSki-0.1.6/PKG-INFO` & `JSONSki-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JSONSki
-Version: 0.1.6
+Version: 0.1.7
 Summary: JSONSki_Python is the Python binding port for JSONSki
 Home-page: https://github.com/your_username/your_repository
 Author: AutomataLab
 Author-email: zhijia@cs.ucr.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `JSONSki-0.1.6/README.md` & `JSONSki-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `JSONSki-0.1.6/example_python/example1.cpp` & `JSONSki-0.1.7/example_python/example1.cpp`

 * *Files identical despite different names*

### Comparing `JSONSki-0.1.6/setup.py` & `JSONSki-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, Extension
 
 # Extension module
 JSONSKi_module = Extension(
     'JSONSki',
     sources=['./example_python/example1.cpp','/example_python',],
-    include_dirs=['./example_python/pybind11-master/include','./src','../src', '../src/..','/src','src','example_python','/example_python','./example_python'],
+    include_dirs=['./example_python/pybind11-master/include','./src','../src', '../src/..','/src','src','example_python','/example_python'],
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
-    version='0.1.06',
+    version='0.1.07',
     author= AUTHOR,
     author_email= AUTHOR_EMAILS,
     description='JSONSki_Python is the Python binding port for JSONSki',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/your_repository',
     ext_modules=[JSONSKi_module],
```

