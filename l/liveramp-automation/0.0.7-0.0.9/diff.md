# Comparing `tmp/liveramp_automation-0.0.7.tar.gz` & `tmp/liveramp_automation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-0.0.7.tar", last modified: Tue Aug  1 08:41:27 2023, max compression
+gzip compressed data, was "liveramp_automation-0.0.9.tar", last modified: Tue Aug  1 08:46:07 2023, max compression
```

## Comparing `liveramp_automation-0.0.7.tar` & `liveramp_automation-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-01 08:41:27.002400 liveramp_automation-0.0.7/
--rw-r--r--   0 jasqia     (502) staff       (20)     1675 2023-08-01 08:41:27.001688 liveramp_automation-0.0.7/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)     1398 2023-07-19 08:48:17.000000 liveramp_automation-0.0.7/README.md
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-01 08:41:27.000700 liveramp_automation-0.0.7/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     1675 2023-08-01 08:41:26.000000 liveramp_automation-0.0.7/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      232 2023-08-01 08:41:26.000000 liveramp_automation-0.0.7/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-01 08:41:26.000000 liveramp_automation-0.0.7/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-01 08:41:26.000000 liveramp_automation-0.0.7/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-08-01 08:41:26.000000 liveramp_automation-0.0.7/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-01 08:41:27.002631 liveramp_automation-0.0.7/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1159 2023-08-01 08:41:24.000000 liveramp_automation-0.0.7/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-01 08:46:07.920454 liveramp_automation-0.0.9/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1675 2023-08-01 08:46:07.919978 liveramp_automation-0.0.9/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1398 2023-07-19 08:48:17.000000 liveramp_automation-0.0.9/README.md
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-01 08:46:07.914440 liveramp_automation-0.0.9/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.0.9/liveramp_automation/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-01 08:46:07.919029 liveramp_automation-0.0.9/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1675 2023-08-01 08:46:07.000000 liveramp_automation-0.0.9/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      264 2023-08-01 08:46:07.000000 liveramp_automation-0.0.9/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-01 08:46:07.000000 liveramp_automation-0.0.9/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-01 08:46:07.000000 liveramp_automation-0.0.9/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-08-01 08:46:07.000000 liveramp_automation-0.0.9/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-01 08:46:07.920634 liveramp_automation-0.0.9/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1159 2023-08-01 08:46:04.000000 liveramp_automation-0.0.9/setup.py
```

### Comparing `liveramp_automation-0.0.7/PKG-INFO` & `liveramp_automation-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 0.0.7
+Version: 0.0.9
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 # liveramp-automation
```

### Comparing `liveramp_automation-0.0.7/README.md` & `liveramp_automation-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.0.7/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-0.0.9/liveramp_automation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 0.0.7
+Version: 0.0.9
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 # liveramp-automation
```

### Comparing `liveramp_automation-0.0.7/setup.py` & `liveramp_automation-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation',
-    version='0.0.7',
+    version='0.0.9',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
     packages=['liveramp_automation'],
```

