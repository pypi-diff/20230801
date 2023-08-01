# Comparing `tmp/valipy-0.2.2.tar.gz` & `tmp/valipy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valipy-0.2.2.tar", last modified: Sun Jul 30 09:21:07 2023, max compression
+gzip compressed data, was "valipy-0.2.3.tar", last modified: Tue Aug  1 06:55:08 2023, max compression
```

## Comparing `valipy-0.2.2.tar` & `valipy-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:21:07.478335 valipy-0.2.2/
--rw-r--r--   0 josevonchong   (501) staff       (20)     1463 2023-07-30 09:21:07.478452 valipy-0.2.2/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-07-30 09:21:07.478849 valipy-0.2.2/setup.cfg
--rw-r--r--   0 josevonchong   (501) staff       (20)     1311 2023-07-30 09:20:51.000000 valipy-0.2.2/setup.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:21:07.476366 valipy-0.2.2/test/
--rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.2.2/test/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      544 2023-07-30 08:51:40.000000 valipy-0.2.2/test/misc.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.2.2/test/test.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:21:07.477352 valipy-0.2.2/valipy/
--rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.2.2/valipy/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)    11818 2023-07-30 08:45:39.000000 valipy-0.2.2/valipy/exceptions.py
--rw-r--r--   0 josevonchong   (501) staff       (20)    11728 2023-07-30 08:35:33.000000 valipy-0.2.2/valipy/myFunctions.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-30 09:21:07.478175 valipy-0.2.2/valipy.egg-info/
--rw-r--r--   0 josevonchong   (501) staff       (20)     1463 2023-07-30 09:21:07.000000 valipy-0.2.2/valipy.egg-info/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)      243 2023-07-30 09:21:07.000000 valipy-0.2.2/valipy.egg-info/SOURCES.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-07-30 09:21:07.000000 valipy-0.2.2/valipy.egg-info/dependency_links.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-07-30 09:21:07.000000 valipy-0.2.2/valipy.egg-info/top_level.txt
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 06:55:08.730294 valipy-0.2.3/
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1604 2023-08-01 06:55:08.730364 valipy-0.2.3/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-08-01 06:55:08.730594 valipy-0.2.3/setup.cfg
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1367 2023-08-01 06:55:04.000000 valipy-0.2.3/setup.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 06:55:08.728495 valipy-0.2.3/test/
+-rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.2.3/test/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      544 2023-07-30 08:51:40.000000 valipy-0.2.3/test/misc.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.2.3/test/test.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 06:55:08.729345 valipy-0.2.3/valipy/
+-rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.2.3/valipy/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)    11818 2023-07-30 08:45:39.000000 valipy-0.2.3/valipy/exceptions.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)    11728 2023-07-30 08:35:33.000000 valipy-0.2.3/valipy/myFunctions.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-08-01 06:55:08.730166 valipy-0.2.3/valipy.egg-info/
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1604 2023-08-01 06:55:08.000000 valipy-0.2.3/valipy.egg-info/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)      272 2023-08-01 06:55:08.000000 valipy-0.2.3/valipy.egg-info/SOURCES.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-08-01 06:55:08.000000 valipy-0.2.3/valipy.egg-info/dependency_links.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)       23 2023-08-01 06:55:08.000000 valipy-0.2.3/valipy.egg-info/requires.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-08-01 06:55:08.000000 valipy-0.2.3/valipy.egg-info/top_level.txt
```

### Comparing `valipy-0.2.2/PKG-INFO` & `valipy-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
-Keywords: validation,data,schema,schema validation
+Keywords: validation,data,schema,schema validation,regex,patter matching
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
-## Valipy
+<div style="text-align:center">
+    <img src='docs/LOGO.png'/>
+    <p>Dead Simple Data Validation In Python</p>
+</div>
+
+# Valipy
 
 Valipy is a simple, chainable and composable data validation library that aims to be used in any place where you need to make sure data is schematized in a certain way.
 
 Valipy is heavily inspired on the js validation library [v8n.js](https://github.com/imbrn/v8n) and it tries it best to be an almost 1:1 python alternative.
 
 ## Python Version Support
```

### Comparing `valipy-0.2.2/setup.py` & `valipy-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import os
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 setup(
     name='valipy',
     packages=find_packages(),
-    version='0.2.2',
+    version='0.2.3',
     description='A chainable, fluent Python library for validating data',
     long_description_content_type='text/markdown',
     long_description=read_file('readme.md'),
 
     author='Joaquin Jose Von Chong',
     license='MIT',
     readme='readme.md',
     author_email = 'jjvonchong@outlook.com',      # Type in your E-Mail
     url = 'https://github.com/pimepan/valipy',   # Provide either the link to your github or to your website
-    keywords = ['validation', 'data', 'schema', 'schema validation'],   # Keywords that define your package best
-    install_requires=[],
+    keywords = ['validation', 'data', 'schema', 'schema validation', 'regex', 'patter matching'],   # Keywords that define your package best
+    install_requires=["twine","wheel","setuptools"],
     classifiers=[
         'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',      # Define that your audience are developers
         'Topic :: Software Development',
         'License :: OSI Approved :: MIT License',   # Again, pick a license
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
```

### Comparing `valipy-0.2.2/test/misc.py` & `valipy-0.2.3/test/misc.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.2/valipy/exceptions.py` & `valipy-0.2.3/valipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.2/valipy/myFunctions.py` & `valipy-0.2.3/valipy/myFunctions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.2.2/valipy.egg-info/PKG-INFO` & `valipy-0.2.3/valipy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
-Keywords: validation,data,schema,schema validation
+Keywords: validation,data,schema,schema validation,regex,patter matching
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
-## Valipy
+<div style="text-align:center">
+    <img src='docs/LOGO.png'/>
+    <p>Dead Simple Data Validation In Python</p>
+</div>
+
+# Valipy
 
 Valipy is a simple, chainable and composable data validation library that aims to be used in any place where you need to make sure data is schematized in a certain way.
 
 Valipy is heavily inspired on the js validation library [v8n.js](https://github.com/imbrn/v8n) and it tries it best to be an almost 1:1 python alternative.
 
 ## Python Version Support
```

