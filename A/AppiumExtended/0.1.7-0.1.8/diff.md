# Comparing `tmp/AppiumExtended-0.1.7.tar.gz` & `tmp/AppiumExtended-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppiumExtended-0.1.7.tar", last modified: Tue Aug  1 12:18:04 2023, max compression
+gzip compressed data, was "AppiumExtended-0.1.8.tar", last modified: Tue Aug  1 12:56:01 2023, max compression
```

## Comparing `AppiumExtended-0.1.7.tar` & `AppiumExtended-0.1.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.557603 AppiumExtended-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28049 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_is.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_swipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumExtended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumGraph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumGraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumGraph/appium_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumHelpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumHelpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumHelpers/appium_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31739 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumHelpers/appium_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumHelpers/helpers_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumNavigator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumNavigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumNavigator/appium_navigator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumServer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumServer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumServer/appium_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumWebElementExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_adb_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_click.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_dom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_scroll.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_tap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumWebElementsExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementsExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementsExtended/web_elements_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 12:18:04.557603 AppiumExtended-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   246568 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:18:04.557603 AppiumExtended-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/terminal/aapt.py
--rw-r--r--   0 runner    (1001) docker     (123)    41664 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/terminal/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26266 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/terminal/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.557603 AppiumExtended-0.1.7/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/utils/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.216432 AppiumExtended-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.204432 AppiumExtended-0.1.8/AppiumExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28049 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_is.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_swipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumExtended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumGraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumGraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumGraph/appium_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumHelpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumHelpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumHelpers/appium_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31739 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumHelpers/appium_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumHelpers/helpers_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumNavigator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumNavigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumNavigator/appium_navigator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumServer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumServer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumServer/appium_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/AppiumWebElementExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_adb_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_dom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_scroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/AppiumWebElementsExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementsExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementsExtended/web_elements_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   246568 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:56:01.216432 AppiumExtended-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/terminal/aapt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41664 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/terminal/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26266 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/terminal/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/utils/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/utils/utils.py
```

### Comparing `AppiumExtended-0.1.7/AppiumExtended/appium_base.py` & `AppiumExtended-0.1.8/AppiumExtended/appium_base.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumExtended/appium_extended.py` & `AppiumExtended-0.1.8/AppiumExtended/appium_extended.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumExtended/appium_get.py` & `AppiumExtended-0.1.8/AppiumExtended/appium_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumExtended/appium_is.py` & `AppiumExtended-0.1.8/AppiumExtended/appium_is.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumExtended/appium_swipe.py` & `AppiumExtended-0.1.8/AppiumExtended/appium_swipe.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumExtended/appium_tap.py` & `AppiumExtended-0.1.8/AppiumExtended/appium_tap.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumExtended/appium_wait.py` & `AppiumExtended-0.1.8/AppiumExtended/appium_wait.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumExtended.egg-info/PKG-INFO` & `AppiumExtended-0.1.8/AppiumExtended.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppiumExtended
-Version: 0.1.7
+Version: 0.1.8
 Summary: An extension library for adding ease of use Appium-Python-Client
 Home-page: https://github.com/molokov-klim/appium_extended
 Author: molokov-klim
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `AppiumExtended-0.1.7/AppiumExtended.egg-info/SOURCES.txt` & `AppiumExtended-0.1.8/AppiumExtended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumHelpers/appium_helpers.py` & `AppiumExtended-0.1.8/AppiumHelpers/appium_helpers.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumHelpers/appium_image.py` & `AppiumExtended-0.1.8/AppiumHelpers/appium_image.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumHelpers/helpers_decorators.py` & `AppiumExtended-0.1.8/AppiumHelpers/helpers_decorators.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumNavigator/appium_navigator.py` & `AppiumExtended-0.1.8/AppiumNavigator/appium_navigator.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumServer/appium_server.py` & `AppiumExtended-0.1.8/AppiumServer/appium_server.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_adb_actions.py` & `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_adb_actions.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_click.py` & `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_click.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_dom.py` & `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_dom.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_extended.py` & `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_extended.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_get.py` & `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_scroll.py` & `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_scroll.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_tap.py` & `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_tap.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/LICENSE` & `AppiumExtended-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/PKG-INFO` & `AppiumExtended-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppiumExtended
-Version: 0.1.7
+Version: 0.1.8
 Summary: An extension library for adding ease of use Appium-Python-Client
 Home-page: https://github.com/molokov-klim/appium_extended
 Author: molokov-klim
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `AppiumExtended-0.1.7/README.md` & `AppiumExtended-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/setup.py` & `AppiumExtended-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 An extension library for adding ease of use to Appium-Python-Client.
 
 AppiumExtended is a collection of utilities and convenience functions designed to enhance the usage of Appium-Python-Client for mobile app automation testing. It provides additional functionalities and abstractions to simplify the testing process.
 '''
 
 setup(
     name='AppiumExtended',
-    version='0.1.7',
+    version='0.1.8',
     description='An extension library for adding ease of use Appium-Python-Client',
     author='molokov-klim',
     packages=find_packages(),
     install_requires=[
         'Appium-Python-Client==2.11.1',
         'allure-pytest==2.13.2',
         'zlib-compress==0.0.1',
```

### Comparing `AppiumExtended-0.1.7/terminal/aapt.py` & `AppiumExtended-0.1.8/terminal/aapt.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,23 +16,32 @@
         Возвращает название пакета.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.info(f"get_package_name() < {path_to_apk}")
 
         command = ["aapt", "dump", "badging", os.path.join(path_to_apk)]
 
-        # Выполнение команды и получение вывода
-        output: str = str(subprocess.check_output(command)).strip()
-
-        # Извлечение строки, содержащей информацию о пакете
-        start_index = output.index("package: name='") + len("package: name='")
-        end_index = output.index("'", start_index)
-
-        # Извлекаем название пакета
-        package_name = output[start_index:end_index]
+        try:
+            # Выполнение команды и получение вывода
+            output: str = str(subprocess.check_output(command)).strip()
+
+            # Извлечение строки, содержащей информацию о пакете
+            start_index = output.index("package: name='") + len("package: name='")
+            end_index = output.index("'", start_index)
+
+            # Извлекаем название пакета
+            package_name = output[start_index:end_index]
+
+        except subprocess.CalledProcessError as e:
+            logger.error(f"Could not extract package name. Error: {str(e)}")
+            raise  # Выбрасываем исключение дальше
+
+        except ValueError:
+            logger.error(f"Could not find package name in the output.")
+            raise  # Выбрасываем исключение дальше
 
         logger.info(f"get_package_name() > {package_name}")
         # Возвращение названия пакета в виде строки
         return package_name
 
     @staticmethod
     def get_launchable_activity_from_apk(path_to_apk: str) -> str:
@@ -41,20 +50,27 @@
         Возвращает название активности в виде строки.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.info(f"get_launchable_activity_from_apk() < {path_to_apk}")
 
         command = ["aapt", "dump", "badging", path_to_apk]
 
-        # Выполнение команды и получение вывода
-        output = str(subprocess.check_output(command)).strip()
-
-        # Извлечение строки, содержащей информацию о запускаемой активности
-        package_line = [line for line in output.splitlines() if line.startswith("launchable-activity")][0]
-
-        # Извлечение названия активности из строки
-        launchable_activity = package_line.split("'")[1]
+        try:
+            # Выполнение команды и получение вывода
+            output = subprocess.check_output(command, universal_newlines=True).strip()
+
+            # Извлечение строки, содержащей информацию о запускаемой активности
+            package_line = next(line for line in output.splitlines() if line.startswith("launchable-activity"))
+
+            # Извлечение названия активности из строки
+            launchable_activity = package_line.split("'")[1]
+
+            # Возвращение названия активности в виде строки
+            logger.info(f"get_launchable_activity_from_apk() > {launchable_activity}")
+            return launchable_activity
+        except subprocess.CalledProcessError as e:
+            logger.error(f"Could not extract launchable activity. Error: {str(e)}")
+        except StopIteration:
+            logger.error("Could not find 'launchable-activity' line in aapt output.")
 
-        # Возвращение названия активности в виде строки
+        return ""
 
-        logger.info(f"get_launchable_activity_from_apk() > {launchable_activity}")
-        return launchable_activity
```

### Comparing `AppiumExtended-0.1.7/terminal/adb.py` & `AppiumExtended-0.1.8/terminal/adb.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/terminal/terminal.py` & `AppiumExtended-0.1.8/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/utils/operations.py` & `AppiumExtended-0.1.8/utils/operations.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.7/utils/utils.py` & `AppiumExtended-0.1.8/utils/utils.py`

 * *Files identical despite different names*

