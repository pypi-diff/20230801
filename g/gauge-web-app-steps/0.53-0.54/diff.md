# Comparing `tmp/gauge-web-app-steps-0.53.tar.gz` & `tmp/gauge-web-app-steps-0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauge-web-app-steps-0.53.tar", last modified: Tue Aug  1 09:11:07 2023, max compression
+gzip compressed data, was "gauge-web-app-steps-0.54.tar", last modified: Tue Aug  1 11:27:07 2023, max compression
```

## Comparing `gauge-web-app-steps-0.53.tar` & `gauge-web-app-steps-0.54.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 09:11:07.886433 gauge-web-app-steps-0.53/
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1088 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/LICENCE
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     5415 2023-08-01 09:11:07.886310 gauge-web-app-steps-0.53/PKG-INFO
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     4807 2023-08-01 08:37:40.000000 gauge-web-app-steps-0.53/README.md
-drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 09:11:07.884180 gauge-web-app-steps-0.53/gauge_web_app_steps/
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       63 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/__init__.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     3033 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/app_context.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)      525 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/bymapper.py
-drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 09:11:07.885500 gauge-web-app-steps-0.53/gauge_web_app_steps/config/
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       63 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/config/__init__.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     2677 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/config/common_config.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)      631 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/config/local_config.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     2128 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/config/saucelabs_config.py
-drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 09:11:07.886113 gauge-web-app-steps-0.53/gauge_web_app_steps/driver/
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)      326 2023-08-01 08:37:41.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/driver/__init__.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1103 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/driver/browsers.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)    16737 2023-08-01 08:37:41.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/driver/driver_factory.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1735 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/driver/operating_system.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)      364 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/driver/platform.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     4594 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/imagepaths.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)    12496 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/images.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)      423 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/keymapper.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     2852 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/report.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     2874 2023-08-01 08:37:41.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/sauce_tunnel.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1287 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/selector.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)    44907 2023-08-01 08:37:41.000000 gauge-web-app-steps-0.53/gauge_web_app_steps/web_app_steps.py
-drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 09:11:07.884983 gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     5415 2023-08-01 09:11:07.000000 gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/PKG-INFO
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1010 2023-08-01 09:11:07.000000 gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/SOURCES.txt
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)        1 2023-08-01 09:11:07.000000 gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/dependency_links.txt
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)        1 2023-08-01 09:11:07.000000 gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/not-zip-safe
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)      132 2023-08-01 09:11:07.000000 gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/requires.txt
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       20 2023-08-01 09:11:07.000000 gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/top_level.txt
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       82 2023-08-01 08:37:41.000000 gauge-web-app-steps-0.53/pyproject.toml
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       38 2023-08-01 09:11:07.886473 gauge-web-app-steps-0.53/setup.cfg
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1068 2023-08-01 08:37:40.000000 gauge-web-app-steps-0.53/setup.py
+drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 11:27:07.681880 gauge-web-app-steps-0.54/
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1088 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/LICENCE
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     5415 2023-08-01 11:27:07.681757 gauge-web-app-steps-0.54/PKG-INFO
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     4807 2023-08-01 11:11:22.000000 gauge-web-app-steps-0.54/README.md
+drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 11:27:07.679556 gauge-web-app-steps-0.54/gauge_web_app_steps/
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       63 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/__init__.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     3033 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/app_context.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)      525 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/bymapper.py
+drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 11:27:07.680919 gauge-web-app-steps-0.54/gauge_web_app_steps/config/
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       63 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/config/__init__.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     2677 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/config/common_config.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)      631 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/config/local_config.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     2128 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/config/saucelabs_config.py
+drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 11:27:07.681577 gauge-web-app-steps-0.54/gauge_web_app_steps/driver/
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)      326 2023-08-01 11:11:22.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/driver/__init__.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1103 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/driver/browsers.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)    16737 2023-08-01 11:11:22.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/driver/driver_factory.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1735 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/driver/operating_system.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)      364 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/driver/platform.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     4594 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/imagepaths.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)    12496 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/images.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)      423 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/keymapper.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     2852 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/report.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     2874 2023-08-01 11:11:22.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/sauce_tunnel.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1287 2023-07-28 13:51:11.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/selector.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)    44907 2023-08-01 11:11:22.000000 gauge-web-app-steps-0.54/gauge_web_app_steps/web_app_steps.py
+drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-08-01 11:27:07.680380 gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     5415 2023-08-01 11:27:07.000000 gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/PKG-INFO
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1010 2023-08-01 11:27:07.000000 gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)        1 2023-08-01 11:27:07.000000 gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)        1 2023-08-01 11:27:07.000000 gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/not-zip-safe
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)      132 2023-08-01 11:27:07.000000 gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/requires.txt
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       20 2023-08-01 11:27:07.000000 gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/top_level.txt
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       82 2023-08-01 11:11:22.000000 gauge-web-app-steps-0.54/pyproject.toml
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       38 2023-08-01 11:27:07.681919 gauge-web-app-steps-0.54/setup.cfg
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1068 2023-08-01 11:12:49.000000 gauge-web-app-steps-0.54/setup.py
```

### Comparing `gauge-web-app-steps-0.53/LICENCE` & `gauge-web-app-steps-0.54/LICENCE`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/PKG-INFO` & `gauge-web-app-steps-0.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauge-web-app-steps
-Version: 0.53
+Version: 0.54
 Summary: Provides basic steps for a Gauge project, that runs tests with Selenium and Appium
 Home-page: https://github.com/IBM/gauge-web-app-steps
 Author: Tobias Lehmann
 Author-email: derdualist1@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `gauge-web-app-steps-0.53/README.md` & `gauge-web-app-steps-0.54/README.md`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/app_context.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/app_context.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/bymapper.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/bymapper.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/config/common_config.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/config/common_config.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/config/local_config.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/config/local_config.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/config/saucelabs_config.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/config/saucelabs_config.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/driver/browsers.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/driver/browsers.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/driver/driver_factory.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/driver/driver_factory.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/driver/operating_system.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/driver/operating_system.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/imagepaths.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/imagepaths.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/images.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/images.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/report.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/report.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/sauce_tunnel.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/sauce_tunnel.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/selector.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/selector.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps/web_app_steps.py` & `gauge-web-app-steps-0.54/gauge_web_app_steps/web_app_steps.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/PKG-INFO` & `gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauge-web-app-steps
-Version: 0.53
+Version: 0.54
 Summary: Provides basic steps for a Gauge project, that runs tests with Selenium and Appium
 Home-page: https://github.com/IBM/gauge-web-app-steps
 Author: Tobias Lehmann
 Author-email: derdualist1@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `gauge-web-app-steps-0.53/gauge_web_app_steps.egg-info/SOURCES.txt` & `gauge-web-app-steps-0.54/gauge_web_app_steps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.53/setup.py` & `gauge-web-app-steps-0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     long_description = long_description.replace('./docs/', 'https://github.com/IBM/gauge-web-app-steps/tree/master/docs/')
 
 setup(
     name='gauge-web-app-steps',
-    version='0.53',
+    version='0.54',
     description='Provides basic steps for a Gauge project, that runs tests with Selenium and Appium',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/IBM/gauge-web-app-steps',
     author='Tobias Lehmann',
     author_email='derdualist1@gmail.com',
     license='MIT',
```

