# Comparing `tmp/mongoy-0.1.4.tar.gz` & `tmp/mongoy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoy-0.1.4.tar", last modified: Tue Aug  1 09:36:04 2023, max compression
+gzip compressed data, was "mongoy-0.1.5.tar", last modified: Tue Aug  1 09:39:11 2023, max compression
```

## Comparing `mongoy-0.1.4.tar` & `mongoy-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:36:04.758758 mongoy-0.1.4/
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1061 2023-07-18 15:58:12.000000 mongoy-0.1.4/LICENSE
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1939 2023-08-01 09:36:04.758633 mongoy-0.1.4/PKG-INFO
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1601 2023-07-19 08:24:07.000000 mongoy-0.1.4/README.md
-drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:36:04.757276 mongoy-0.1.4/mongoy/
-drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:36:04.758461 mongoy-0.1.4/mongoy/mongoy.egg-info/
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1939 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/PKG-INFO
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      210 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/SOURCES.txt
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        1 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/dependency_links.txt
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       16 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/requires.txt
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        7 2023-08-01 09:36:04.000000 mongoy-0.1.4/mongoy/mongoy.egg-info/top_level.txt
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       38 2023-08-01 09:36:04.758793 mongoy-0.1.4/setup.cfg
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1199 2023-08-01 09:36:00.000000 mongoy-0.1.4/setup.py
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:39:11.536337 mongoy-0.1.5/
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1061 2023-07-18 15:58:12.000000 mongoy-0.1.5/LICENSE
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1939 2023-08-01 09:39:11.536179 mongoy-0.1.5/PKG-INFO
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1601 2023-07-19 08:24:07.000000 mongoy-0.1.5/README.md
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:39:11.534964 mongoy-0.1.5/mongoy/
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:37:57.000000 mongoy-0.1.5/mongoy/__init__.py
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     3983 2023-08-01 09:38:03.000000 mongoy-0.1.5/mongoy/mongo.py
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-08-01 09:39:11.535923 mongoy-0.1.5/mongoy.egg-info/
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1939 2023-08-01 09:39:11.000000 mongoy-0.1.5/mongoy.egg-info/PKG-INFO
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      210 2023-08-01 09:39:11.000000 mongoy-0.1.5/mongoy.egg-info/SOURCES.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        1 2023-08-01 09:39:11.000000 mongoy-0.1.5/mongoy.egg-info/dependency_links.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       16 2023-08-01 09:39:11.000000 mongoy-0.1.5/mongoy.egg-info/requires.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        7 2023-08-01 09:39:11.000000 mongoy-0.1.5/mongoy.egg-info/top_level.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       38 2023-08-01 09:39:11.536375 mongoy-0.1.5/setup.cfg
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1201 2023-08-01 09:38:44.000000 mongoy-0.1.5/setup.py
```

### Comparing `mongoy-0.1.4/LICENSE` & `mongoy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoy-0.1.4/PKG-INFO` & `mongoy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoy
-Version: 0.1.4
+Version: 0.1.5
 Summary: wrapper utility for mongodb
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mongoy-0.1.4/README.md` & `mongoy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mongoy-0.1.4/mongoy/mongoy.egg-info/PKG-INFO` & `mongoy-0.1.5/mongoy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoy
-Version: 0.1.4
+Version: 0.1.5
 Summary: wrapper utility for mongodb
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mongoy-0.1.4/setup.py` & `mongoy-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mongoy",                     # This is the name of the package
-    version="0.1.4",                        # The initial release version
+    version="0.1.5",                        # The initial release version
     author="pavittarx",                     # Full name of the author
     description="wrapper utility for mongodb",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
     py_modules=["mongoy"],             # Name of the python package
-    package_dir={'':'mongoy'},     # Directory of the source code of the package
+    # package_dir={'':'mongoy'},     # Directory of the source code of the package
     install_requires=["pymongo", "certifi"]                     # Install other dependencies if any
 )
```

