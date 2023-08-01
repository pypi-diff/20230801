# Comparing `tmp/sconce-0.0.28.tar.gz` & `tmp/sconce-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sconce-0.0.28.tar", last modified: Tue Aug  1 08:04:33 2023, max compression
+gzip compressed data, was "sconce-0.0.29.tar", last modified: Tue Aug  1 08:07:48 2023, max compression
```

## Comparing `sconce-0.0.28.tar` & `sconce-0.0.29.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-08-01 08:04:33.874133 sconce-0.0.28/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     1068 2023-07-21 20:40:44.000000 sconce-0.0.28/LICENSE.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     3517 2023-08-01 08:04:33.874133 sconce-0.0.28/PKG-INFO
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     3130 2023-07-27 08:03:42.000000 sconce-0.0.28/README.md
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      324 2023-08-01 08:04:01.000000 sconce-0.0.28/pyproject.toml
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      841 2023-07-21 20:40:44.000000 sconce-0.0.28/requirements.txt
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-08-01 08:04:33.874133 sconce-0.0.28/sconce/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      130 2023-08-01 07:59:42.000000 sconce-0.0.28/sconce/__init__.py
--rw-rw-r--   0 sathya    (1000) sathya    (1000)    15589 2023-08-01 08:03:10.000000 sconce-0.0.28/sconce/sconce.py
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-08-01 08:04:33.874133 sconce-0.0.28/sconce.egg-info/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     3517 2023-08-01 08:04:33.000000 sconce-0.0.28/sconce.egg-info/PKG-INFO
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      257 2023-08-01 08:04:33.000000 sconce-0.0.28/sconce.egg-info/SOURCES.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)        1 2023-08-01 08:04:33.000000 sconce-0.0.28/sconce.egg-info/dependency_links.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      841 2023-08-01 08:04:33.000000 sconce-0.0.28/sconce.egg-info/requires.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)        7 2023-08-01 08:04:33.000000 sconce-0.0.28/sconce.egg-info/top_level.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       79 2023-08-01 08:04:33.878133 sconce-0.0.28/setup.cfg
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      916 2023-08-01 08:02:56.000000 sconce-0.0.28/setup.py
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-08-01 08:07:48.284891 sconce-0.0.29/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1068 2023-07-21 20:40:44.000000 sconce-0.0.29/LICENSE.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     3517 2023-08-01 08:07:48.284891 sconce-0.0.29/PKG-INFO
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     3130 2023-07-27 08:03:42.000000 sconce-0.0.29/README.md
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      324 2023-08-01 08:07:15.000000 sconce-0.0.29/pyproject.toml
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      841 2023-07-21 20:40:44.000000 sconce-0.0.29/requirements.txt
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-08-01 08:07:48.284891 sconce-0.0.29/sconce/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      128 2023-08-01 08:06:41.000000 sconce-0.0.29/sconce/__init__.py
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)    15589 2023-08-01 08:03:10.000000 sconce-0.0.29/sconce/sconce.py
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-08-01 08:07:48.284891 sconce-0.0.29/sconce.egg-info/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     3517 2023-08-01 08:07:48.000000 sconce-0.0.29/sconce.egg-info/PKG-INFO
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      257 2023-08-01 08:07:48.000000 sconce-0.0.29/sconce.egg-info/SOURCES.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)        1 2023-08-01 08:07:48.000000 sconce-0.0.29/sconce.egg-info/dependency_links.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      841 2023-08-01 08:07:48.000000 sconce-0.0.29/sconce.egg-info/requires.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)        7 2023-08-01 08:07:48.000000 sconce-0.0.29/sconce.egg-info/top_level.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       79 2023-08-01 08:07:48.288891 sconce-0.0.29/setup.cfg
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      916 2023-08-01 08:07:21.000000 sconce-0.0.29/setup.py
```

### Comparing `sconce-0.0.28/LICENSE.txt` & `sconce-0.0.29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sconce-0.0.28/PKG-INFO` & `sconce-0.0.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sconce
-Version: 0.0.28
+Version: 0.0.29
 Summary: sconce: torch helper
 Home-page: https://github.com/satabios/sconce
 Download-URL: https://pypi.org/project/sconce/
 Author: Sathyaprakash Narayanan
 Author-email: Sathyaprakash Narayanan <snaray17@ucsc.edu>
 Project-URL: code, https://github.com/satabios/sconce
 Description-Content-Type: text/markdown
```

### Comparing `sconce-0.0.28/README.md` & `sconce-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `sconce-0.0.28/requirements.txt` & `sconce-0.0.29/requirements.txt`

 * *Files identical despite different names*

### Comparing `sconce-0.0.28/sconce/sconce.py` & `sconce-0.0.29/sconce/sconce.py`

 * *Files identical despite different names*

### Comparing `sconce-0.0.28/sconce.egg-info/PKG-INFO` & `sconce-0.0.29/sconce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sconce
-Version: 0.0.28
+Version: 0.0.29
 Summary: sconce: torch helper
 Home-page: https://github.com/satabios/sconce
 Download-URL: https://pypi.org/project/sconce/
 Author: Sathyaprakash Narayanan
 Author-email: Sathyaprakash Narayanan <snaray17@ucsc.edu>
 Project-URL: code, https://github.com/satabios/sconce
 Description-Content-Type: text/markdown
```

### Comparing `sconce-0.0.28/sconce.egg-info/requires.txt` & `sconce-0.0.29/sconce.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sconce-0.0.28/setup.py` & `sconce-0.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 import os
 setup_args = dict(
     name='sconce',
-    version='0.0.28',
+    version='0.0.29',
     description='sconce: torch helper',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     packages=['sconce'],
     author='Sathyaprakash Narayanan',
     author_email='snaray17@ucsc.edu',
     url='https://github.com/satabios/sconce',
```

