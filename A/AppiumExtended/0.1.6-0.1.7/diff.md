# Comparing `tmp/AppiumExtended-0.1.6.tar.gz` & `tmp/AppiumExtended-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppiumExtended-0.1.6.tar", last modified: Fri Jul 28 13:00:51 2023, max compression
+gzip compressed data, was "AppiumExtended-0.1.7.tar", last modified: Tue Aug  1 12:18:04 2023, max compression
```

## Comparing `AppiumExtended-0.1.6.tar` & `AppiumExtended-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.636560 AppiumExtended-0.1.6/AppiumExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28026 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_is.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_swipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.636560 AppiumExtended-0.1.6/AppiumExtended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.636560 AppiumExtended-0.1.6/AppiumGraph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumGraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumGraph/appium_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumHelpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumHelpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumHelpers/appium_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31656 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumHelpers/appium_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumHelpers/helpers_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumNavigator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumNavigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumNavigator/appium_navigator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumServer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumServer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumServer/appium_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumWebElementExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_adb_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_click.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_dom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_scroll.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_tap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumWebElementsExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementsExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementsExtended/web_elements_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27562 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/adb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/adb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27272 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/adb/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/utils/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.557603 AppiumExtended-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28049 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_is.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_swipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumExtended/appium_wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumExtended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 12:18:04.000000 AppiumExtended-0.1.7/AppiumExtended.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumGraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumGraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumGraph/appium_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumHelpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumHelpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumHelpers/appium_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31739 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumHelpers/appium_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumHelpers/helpers_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumNavigator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumNavigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumNavigator/appium_navigator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumServer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumServer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumServer/appium_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumWebElementExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_adb_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_dom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_scroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/AppiumWebElementsExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementsExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/AppiumWebElementsExtended/web_elements_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 12:18:04.557603 AppiumExtended-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   246568 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:18:04.557603 AppiumExtended-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.553603 AppiumExtended-0.1.7/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/terminal/aapt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41664 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/terminal/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26266 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/terminal/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:18:04.557603 AppiumExtended-0.1.7/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/utils/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-01 12:17:54.000000 AppiumExtended-0.1.7/utils/utils.py
```

### Comparing `AppiumExtended-0.1.6/AppiumExtended/appium_base.py` & `AppiumExtended-0.1.7/AppiumExtended/appium_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # coding: utf-8
 import logging
 import json
 import time
 
 from appium import webdriver
 
-import config
 from AppiumServer.appium_server import AppiumServer
 from AppiumHelpers.appium_image import AppiumImage
+from terminal.terminal import Terminal
+from terminal.aapt import Aapt
+from terminal.adb import Adb
+import config
 
 
 class AppiumBase(object):
     """
     Класс работы с Appium.
     Обеспечивает подключение к устройству
     """
@@ -24,16 +27,19 @@
         # port = 4723,
 
         self.url = f"http://{config.APPIUM_IP}:{config.APPIUM_PORT}/wd/hub"
         self.capabilities = None
         self.keep_alive_server = True
         self.driver = None
         self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-        self.server = AppiumServer(port=config.APPIUM_IP, log_level=config.APPIUM_LOG_LEVEL)
+        self.server = AppiumServer(port=config.APPIUM_PORT, log_level=config.APPIUM_LOG_LEVEL)
         self.image = None
+        self.terminal = None
+        self.aapt = Aapt()
+        self.adb = Adb()
 
     def connect(self, capabilities: dict):
         """
         Подключение к устройству
         """
         self.capabilities = capabilities
         self.logger.debug(
@@ -50,14 +56,15 @@
                                        desired_capabilities=self.capabilities,
                                        keep_alive=True)
 
         app_capabilities = json.dumps(capabilities)
 
         # Инициализация объектов требующих драйвер
         self.image = AppiumImage(driver=self.driver)
+        self.terminal = Terminal(driver=self.driver)
 
         self.logger.info('Подключение установлено: '.format(app_capabilities))
         self.logger.info(f'Сессия №: {self.driver.session_id}')
 
     def disconnect(self):
         """
         Отключение от устройства
@@ -67,8 +74,7 @@
             self.driver.quit()
             self.driver = None
         if not self.keep_alive_server:
             self.server.stop()
 
     def is_running(self):
         return self.driver.is_running()
-
```

### Comparing `AppiumExtended-0.1.6/AppiumExtended/appium_extended.py` & `AppiumExtended-0.1.7/AppiumExtended/appium_extended.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,38 +3,32 @@
 from typing import Union, Tuple, Dict, List, Optional, cast, Any
 
 import numpy as np
 from PIL import Image
 from appium.webdriver import WebElement
 from appium.webdriver.common.appiumby import AppiumBy
 from appium.webdriver.common.mobileby import MobileBy
-from selenium.common import StaleElementReferenceException
+from selenium.common.exceptions import StaleElementReferenceException
 from selenium.webdriver.common.by import By
 
 from AppiumExtended.appium_is import AppiumIs
 from AppiumExtended.appium_swipe import AppiumSwipe
 from AppiumExtended.appium_tap import AppiumTap
 from AppiumExtended.appium_wait import AppiumWait
 from AppiumWebElementExtended.web_element_extended import WebElementExtended
-from adb import adb
+
 from utils import utils
 
 
 class AppiumExtended(AppiumIs, AppiumTap, AppiumSwipe, AppiumWait):
     """
     Класс работы с Appium.
     Обеспечивает работу с устройством
     """
 
-    def __init__(self):
-        super().__init__()
-
-    def __del__(self):
-        self.disconnect()
-
     def get_element(self,
                     locator: Union[Tuple, WebElementExtended, Dict[str, str], str] = None,
                     by: Union[MobileBy, AppiumBy, By, str] = None,
                     value: Union[str, Dict, None] = None,
                     timeout_elem: int = 10,
                     timeout_method: int = 600,
                     elements_range: Union[Tuple, List[WebElementExtended], Dict[str, str], None] = None,
@@ -153,16 +147,15 @@
                              ocr: Optional[bool] = True,
                              ) -> Union[Tuple[int, int, int, int], None]:  # TODO реализовать None
         """
         # TODO fill
         """
         if ocr:
             return self._get_text_coordinates(text=text, language=language, image=image)
-        else:
-            return self.get_element(locator={'text': text, 'displayed': 'true', 'enabled': 'true'}).get_coordinates()
+        return self.get_element(locator={'text': text, 'displayed': 'true', 'enabled': 'true'}).get_coordinates()
 
     # DOM
 
     def get_element_contains(self,
                              ) -> Any:
         """
         Возвращает элемент содержащий определенный элемент
@@ -234,16 +227,15 @@
         - language (str): Язык распознавания текста. Значение по умолчанию: 'rus'.
 
         Возвращает:
         - bool: True, если заданный текст найден на экране. False в противном случае.
         """
         if ocr:
             return self.image.is_text_on_ocr_screen(text=text, language=language)
-        else:
-            return self._is_element_within_screen(locator={'text': text})
+        return self._is_element_within_screen(locator={'text': text})
 
     def is_image_on_the_screen(self,
                                image: Union[bytes, np.ndarray, Image.Image, str],
                                threshold: float = 0.9,
                                ) -> bool:
         return self.image.is_image_on_the_screen(image=image,
                                                  threshold=threshold)
@@ -325,52 +317,53 @@
         start_x, start_y = self._extract_point_coordinates_by_typing(start_position)
 
         if end_position is not None:
             # Извлечение координат конечной точки свайпа
             end_x, end_y = self._extract_point_coordinates_by_typing(end_position)
         else:
             # Извлечение координат конечной точки свайпа на основе направления и расстояния
-            end_x, end_y = self._extract_point_coordinates_by_direction(direction, distance, start_x, start_y)
+            end_x, end_y = self._extract_point_coordinates_by_direction(direction, distance, start_x, start_y,
+                                                                        screen_resolution=self.terminal.get_screen_resolution())
 
         # Выполнение свайпа
         assert self._swipe(start_x=start_x, start_y=start_y,
                            end_x=end_x, end_y=end_y,
                            duration=duration)
 
         # Возвращаем экземпляр класса AppiumExtended
         return cast('AppiumExtended', self)
 
     def swipe_right_to_left(self):
-        window_size = adb.get_screen_resolution()
+        window_size = self.terminal.get_screen_resolution()
         width = window_size[0]
         height = window_size[1]
         left = int(width * 0.1)
         right = int(width * 0.9)
         self.swipe(start_position=(right, height // 2),
                    end_position=(left, height // 2))
 
     def swipe_left_to_right(self):
-        window_size = adb.get_screen_resolution()
+        window_size = self.terminal.get_screen_resolution()
         width = window_size[0]
         height = window_size[1]
         left = int(width * 0.1)
         right = int(width * 0.9)
         self.swipe(start_position=(left, height // 2),
                    end_position=(right, height // 2))
 
     def swipe_top_to_bottom(self):
-        window_size = adb.get_screen_resolution()
+        window_size = self.terminal.get_screen_resolution()
         height = window_size[1]
         top = int(height * 0.1)
         bottom = int(height * 0.9)
         self.swipe(start_position=(top, height // 2),
                    end_position=(bottom, height // 2))
 
     def swipe_bottom_to_top(self):
-        window_size = adb.get_screen_resolution()
+        window_size = self.terminal.get_screen_resolution()
         height = window_size[1]
         top = int(height * 0.1)
         bottom = int(height * 0.9)
         self.swipe(start_position=(bottom, height // 2),
                    end_position=(top, height // 2))
 
     # WAIT
@@ -468,30 +461,30 @@
         elif isinstance(position, (bytes, np.ndarray, Image.Image, str)):
             # Если position является строкой, байтами, массивом NumPy или объектом Image.Image,
             # то получаем координаты центра изображения
             x, y = utils.calculate_center_of_coordinates(
                 self.get_image_coordinates(image=position))
         return x, y
 
-    def _extract_point_coordinates_by_direction(self,
-                                                direction: int, distance: int,
-                                                start_x: int, start_y: int
+    @staticmethod
+    def _extract_point_coordinates_by_direction(direction: int, distance: int,
+                                                start_x: int, start_y: int,
+                                                screen_resolution: tuple
                                                 ) -> Tuple[int, int]:
         """
         Извлекает координаты точки на заданном расстоянии и в заданном направлении относительно начальных координат.
 
         Параметры:
             direction (str): Направление движения в пределах 360 градусов.
             distance (int): Расстояние, на которое нужно переместиться относительно начальных координат в пикселях.
             start_x (int): Начальная координата X.
             start_y (int): Начальная координата Y.
 
         Возвращает:
             Tuple[int, int]: Координаты конечной точки в формате (x, y).
         """
-        window_size = adb.get_screen_resolution()
-        width = window_size[0]
-        height = window_size[1]
+        width = screen_resolution[0]
+        height = screen_resolution[1]
         end_x, end_y = utils.find_coordinates_by_vector(width=width, height=height,
                                                         direction=direction, distance=distance,
                                                         start_x=start_x, start_y=start_y)
         return end_x, end_y
```

### Comparing `AppiumExtended-0.1.6/AppiumExtended/appium_get.py` & `AppiumExtended-0.1.7/AppiumExtended/appium_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.6/AppiumExtended/appium_is.py` & `AppiumExtended-0.1.7/AppiumExtended/appium_is.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # coding: utf-8
 from typing import Union, Dict, Tuple
 
 from appium.webdriver import WebElement
 
 from AppiumExtended.appium_get import AppiumGet
-from adb import adb
 
 
 class AppiumIs(AppiumGet):
     """
     Класс расширяющий Appium.
     Обеспечивает ....
     """
 
     def __init__(self):
         super().__init__()
         self.helper = None
 
-
     def _is_element_within_screen(
             self,
             locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
             timeout: int = 10
     ) -> bool:
         """
         Метод проверяет, находится ли заданный элемент на видимом экране.
@@ -30,15 +28,15 @@
         - locator (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str]):
             Локатор или элемент, который нужно проверить.
         - timeout (int): Время ожидания элемента. Значение по умолчанию: 10.
 
         Возвращает:
         - bool: True, если элемент находится на экране, False, если нет.
         """
-        screen_size = adb.get_screen_resolution()  # Получаем размеры экрана
+        screen_size = self.terminal.get_screen_resolution()  # Получаем размеры экрана
         screen_width = screen_size[0]  # Ширина экрана
         screen_height = screen_size[1]  # Высота экрана
         element = self._get_element(locator=locator, timeout_elem=timeout)  # Получаем элемент по локатору
         if element is None:
             return False
         if not element.get_attribute('displayed') == 'true':
             # Если элемент не отображается на экране
@@ -51,9 +49,7 @@
                 element_location['y'] < 0 or
                 element_location['x'] < 0
         ):
             # Если элемент находится за пределами экрана
             return False
         # Если элемент находится на экране
         return True
-
-
```

### Comparing `AppiumExtended-0.1.6/AppiumExtended/appium_swipe.py` & `AppiumExtended-0.1.7/AppiumExtended/appium_swipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-from selenium.common import WebDriverException
+from selenium.common.exceptions import WebDriverException
 from AppiumExtended.appium_get import AppiumGet
 
 
 class AppiumSwipe(AppiumGet):
     """
     Класс работы с Appium.
     Обеспечивает swipe
```

### Comparing `AppiumExtended-0.1.6/AppiumExtended/appium_tap.py` & `AppiumExtended-0.1.7/AppiumExtended/appium_tap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 from typing import Optional
 
-from selenium.common import WebDriverException
+from selenium.common.exceptions import WebDriverException
 
 from AppiumExtended.appium_get import AppiumGet
 
 
 class AppiumTap(AppiumGet):
     """
     Класс работы с Appium.
```

### Comparing `AppiumExtended-0.1.6/AppiumExtended/appium_wait.py` & `AppiumExtended-0.1.7/AppiumExtended/appium_wait.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.6/AppiumExtended.egg-info/PKG-INFO` & `AppiumExtended-0.1.7/AppiumExtended.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: AppiumExtended
-Version: 0.1.6
+Version: 0.1.7
 Summary: An extension library for adding ease of use Appium-Python-Client
+Home-page: https://github.com/molokov-klim/appium_extended
 Author: molokov-klim
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `AppiumExtended-0.1.6/AppiumExtended.egg-info/SOURCES.txt` & `AppiumExtended-0.1.7/AppiumExtended.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,12 +31,14 @@
 AppiumWebElementExtended/web_element_dom.py
 AppiumWebElementExtended/web_element_extended.py
 AppiumWebElementExtended/web_element_get.py
 AppiumWebElementExtended/web_element_scroll.py
 AppiumWebElementExtended/web_element_tap.py
 AppiumWebElementsExtended/__init__.py
 AppiumWebElementsExtended/web_elements_extended.py
-adb/__init__.py
-adb/adb.py
+terminal/__init__.py
+terminal/aapt.py
+terminal/adb.py
+terminal/terminal.py
 utils/__init__.py
 utils/operations.py
 utils/utils.py
```

### Comparing `AppiumExtended-0.1.6/AppiumHelpers/appium_helpers.py` & `AppiumExtended-0.1.7/AppiumHelpers/appium_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 import os
 from typing import Tuple, Dict, Union, List, Optional, Any
 
 from appium.webdriver import WebElement
-from selenium.common import WebDriverException
+from selenium.common.exceptions import WebDriverException
 
 from AppiumHelpers.appium_image import AppiumImage
 
 
 class AppiumHelpers(AppiumImage):
 
     def __init__(self, driver):
```

### Comparing `AppiumExtended-0.1.6/AppiumHelpers/appium_image.py` & `AppiumExtended-0.1.7/AppiumHelpers/appium_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 import numpy as np
 from PIL import Image
 from pytesseract import pytesseract
 
 from selenium.common.exceptions import WebDriverException
 
 import config
-from adb import adb
+
 from AppiumHelpers.helpers_decorators import retry
+from terminal.terminal import Terminal
 
 
 class AppiumImage(object):
     """
     Класс работы с Appium.
     Обеспечивает работу с изображениями
     """
 
     def __init__(self, driver=None):
         self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
         self.driver = driver
+        self.terminal = Terminal(driver=self.driver)
 
     def get_screenshot_as_base64_decoded(self):
         screenshot = self.driver.get_screenshot_as_base64().encode('utf-8')
         screenshot = base64.b64decode(screenshot)
         return screenshot
 
     @retry
@@ -96,15 +98,15 @@
             threshold (float, optional): Пороговое значение сходства для шаблонного сопоставления. По умолчанию 0.9.
 
         Возвращает:
             tuple: Координаты внутреннего изображения относительно экрана в формате ((x1, y1), (x2, y2)).
                    Если внутреннее изображение не найдено, возвращает None.
         """
         # Получаем разрешение экрана
-        screen_width, screen_height = adb.get_screen_resolution()
+        screen_width, screen_height = self.terminal.get_screen_resolution()
 
         # Захватываем скриншот
         screenshot = base64.b64decode(self.driver.get_screenshot_as_base64())
 
         # Читаем скриншот
         full_image = self.to_ndarray(image=screenshot, grayscale=True)
```

### Comparing `AppiumExtended-0.1.6/AppiumHelpers/helpers_decorators.py` & `AppiumExtended-0.1.7/AppiumHelpers/helpers_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,19 +218,59 @@
             ...
     """
 
     # Определяем декоратор функций
     def func_decorator(func):
         # Создаем обертку функции, сохраняющую метаданные исходной функции
         @allure.step(my_str)
-        def wrapper(*args, **kwargs):
+        def wrapper(self, *args, **kwargs):
+            result = None
             # Логируем информацию перед вызовом метода
             logger.info(my_str)
-            # Выполняем исходную функцию
-            result = func(*args, **kwargs)
+            # Получаем скриншот до вызова метода
+            screenshot = self.driver.get_screenshot_as_png()
+            # Генерируем временную метку для имени скриншота
+            timestamp = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+            # Устанавливаем имя скриншота до вызова метода
+            screenshot_name_begin = f"screenshot_begin_{timestamp}.png"
+            video_filename = 'screenrecord_{}.mp4'.format(timestamp)  # Имя файла видеозаписи с временной меткой
+            self.driver.start_recording_screen()
+
+            try:
+                # Выполняем исходную функцию
+                result = func(self, *args, **kwargs)
+            except AssertionError as e:
+                # Если произошло исключение, прикрепляем скриншот до вызова метода к отчету
+                allure.attach(screenshot, name=screenshot_name_begin, attachment_type=allure.attachment_type.PNG)
+                # Получаем скриншот после вызова метода
+                screenshot = self.driver.get_screenshot_as_png()
+                # Генерируем временную метку для имени скриншота
+                timestamp = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+                # Устанавливаем имя скриншота до вызова метода
+                screenshot_name_end = f"screenshot_end_{timestamp}.png"
+                # Если произошло исключение, прикрепляем скриншот после вызова метода к отчету
+                allure.attach(screenshot, name=screenshot_name_end, attachment_type=allure.attachment_type.PNG)
+
+                # Если произошло исключение, прикрепляем видеозапись выполнения метода к отчету
+                allure.attach(base64.b64decode(self.driver.stop_recording_screen()),
+                              name=video_filename,
+                              attachment_type=allure.attachment_type.MP4)
+
+                # Прикрепляем информацию об ошибке AssertionError к отчету
+                allure.attach(str(e), name="AssertionError", attachment_type=allure.attachment_type.TEXT)
+
+                # Выводим информацию в лог
+                logger.error(f"{my_str} [не выполнено]")
+                logger.error("AssertionError:")
+                traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
+                logger.error(traceback_info)
+
+                # Прокидываем исключение дальше
+                raise AssertionError(str(e)).with_traceback(sys.exc_info()[2])
+
             # Логируем информацию после успешного выполнения метода
             logger.info(f"{my_str} [выполнено успешно]")
             # Возвращаем результат выполнения исходной функции
             return result
 
         # Возвращаем обертку функции
         return wrapper
```

### Comparing `AppiumExtended-0.1.6/AppiumNavigator/appium_navigator.py` & `AppiumExtended-0.1.7/AppiumNavigator/appium_navigator.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.6/AppiumServer/appium_server.py` & `AppiumExtended-0.1.7/AppiumServer/appium_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     def __init__(self, port: int = 4723, log_level='error'):
         self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
         self.port = port
         self.log_level = log_level
 
     def start(self) -> bool:
         self.logger.info("Start Appium server")
-        cmd = f'appium server -ka 800 --log-level {self.log_level} --use-plugins=device-farm,appium-dashboard -p {self.port} -a 0.0.0.0 -pa /wd/hub --plugin-device-farm-platform=android'
+        cmd = f'appium server -ka 800 --log-level {self.log_level} --log logs/appium_log.txt --log-timestamp ' \
+              f'--use-plugins=device-farm,appium-dashboard -p {self.port} -a 0.0.0.0 -pa /wd/hub ' \
+              f'--plugin-device-farm-platform=android --allow-insecure=adb_shell'
         try:
             subprocess.Popen(cmd, shell=True)
             return True
         except subprocess.CalledProcessError:
             self.logger.error("Error starting Appium server: subprocess.CalledProcessError")
             return False
         except OSError:
@@ -46,15 +48,15 @@
         try:
             cmd = 'taskkill /F /IM node.exe'
             subprocess.check_output(cmd, shell=True)
             return True
         except subprocess.CalledProcessError:
             return False
 
-    def wait_until_alive(self, timeout: int = 60, poll: int = 2):
+    def wait_until_alive(self, timeout: int = 600, poll: int = 2):
         self.logger.info("Wait for Appium server")
         start_time = time.time()
         while time.time() < start_time + timeout:
             if self.is_alive():
                 return True
             time.sleep(poll)
         return False
```

### Comparing `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_adb_actions.py` & `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_click.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,182 +1,215 @@
 # coding: utf-8
 import logging
-import subprocess
+from typing import Union, Tuple, Dict
 
 from appium.webdriver import WebElement
+from selenium.webdriver.common.action_chains import ActionChains
+from selenium.common.exceptions import ElementNotInteractableException, StaleElementReferenceException, \
+    InvalidElementStateException
 
 import config
 
-from adb import adb
 from AppiumWebElementExtended.web_element_get import WebElementGet
+
 from AppiumHelpers.helpers_decorators import wait_for_window_change
 from utils.utils import find_coordinates_by_vector
 
 
-class WebElementAdbActions(WebElementGet):
+class WebElementClick(WebElementGet):
     """
-    Класс для выполнения adb-действий с элементами.
+    Класс для выполнения действий клика на элементе, двойного клика и клика с зажатием и перемещением курсора.
     Наследуется от класса WebElementGet.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.driver = args[0]
         self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
 
-    def _adb_tap(self,
-                 decorator_args: dict = None,
-                 wait: bool = False) -> bool:
+    def _click(self,
+               duration: int = 0,
+               decorator_args: dict = None,
+               wait: bool = False) -> bool:
         """
-        Выполняет нажатие на элемент с помощью adb.
+        Нажимает на элемент.
 
         Аргументы:
-            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
+            duration (int): Время в секундах для продолжительности нажатия (по умолчанию 0).
+            decorator_args (dict): Параметры для декоратора.
                 timeout_window (int): Время ожидания нового окна (умножается на количество попыток).
                 tries (int): Количество попыток нажатия (по умолчанию 3).
             wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна.
 
+        Использование:
+            decorator_args = {"timeout_window": 5,
+                              "tries": 5}
+            element._click(duration=0, wait=True, decorator_args=decorator_args)
+
         Возвращает:
             bool: True, если нажатие выполнено успешно; False в противном случае.
         """
         if wait:
-            # Если нужно ожидать изменения окна.
+            # Если нужно ожидать изменения окна после нажатия
             if not decorator_args:
+                # Декоратор по умолчанию
                 decorator_args = {"timeout_window": 5,
                                   "tries": 5}
-            return self._adb_tap_to_element_and_wait(decorator_args=decorator_args)
+            return self._click_to_element_and_wait(duration=duration, decorator_args=decorator_args)
         else:
-            # Если не нужно ожидать изменения окна.
-            return self._adb_tap_to_element()
+            # Если не нужно ожидать результата после нажатия
+            return self._click_to_element(duration=duration)
 
-    def _adb_tap_to_element(self) -> bool:
-        return self.__adb_tap()
+    def _click_to_element(self,
+                          duration: int = 0) -> bool:
+        return self.__click(duration=duration)
 
     @wait_for_window_change()
-    def _adb_tap_to_element_and_wait(self,
-                                     decorator_args: dict = None) -> bool:
-        return self.__adb_tap()
+    def _click_to_element_and_wait(self,
+                                   duration: int = 0,
+                                   decorator_args: dict = None) -> bool:
+        return self.__click(duration=duration)
 
-    def __adb_tap(self) -> bool:
+    def __click(self,
+                duration: int = 0) -> bool:
         """
-        Выполняет нажатие на элемент с помощью adb.
+        Выполняет клик на элементе.
+
+        Аргументы:
+            duration (int): Длительность удержания клика в секундах.
 
         Возвращает:
-            bool: True, если нажатие выполнено успешно, False в противном случае.
+            bool: True, если клик выполнен успешно; False в противном случае.
         """
         try:
-            x, y = self._get_center()
-            return adb.tap(x=x, y=y)
-        except Exception:
+            action = ActionChains(self.driver)
+            element = self
+
+            if duration > 0:
+                # Если указана длительность клика, выполняется клик с удержанием на заданную длительность
+                action.click_and_hold(element).pause(duration / 1000).release()
+                action.perform()
+            else:
+                # Если не указана длительность клика, выполняется обычный клик
+                action.click(element).perform()
+
+        except (ElementNotInteractableException, StaleElementReferenceException, InvalidElementStateException) as e:
+            self.logger.error(f"Не удалось кликнуть по элементу")
+            self.logger.error("{}".format(e))
             return False
+        return True
 
-    def _adb_multi_tap(self,
-                       decorator_args: dict = None,
-                       wait: bool = False) -> bool:
-        """
-        Выполняет несколько нажатий с помощью adb.
-
-        Args:
-            decorator_args (dict, optional): Дополнительные аргументы для декоратора.
-                По умолчанию None.
-                Если None то будут преобразованы в decorator_args = {"timeout_window": 5, "tries": 5}), где
-                    timeout_window: время ожидания изменения окна в секундах.
-                    tries: количество попыток (выполнения настоящего метода) для изменения окна.
-            wait (bool, optional): Флаг, указывающий, нужно ли ожидать изменение окна после нажатия.
-                По умолчанию False.
+    def _double_click(self,
+                      decorator_args: dict = None,
+                      wait: bool = False) -> bool:
+        """
+        Выполняет двойное нажатие (double click) на элементе.
 
-        Returns:
-            bool: True, если нажатие выполнено успешно, False в противном случае.
+        Аргументы:
+            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
+                Например:
+                    decorator_args = {"timeout_window": 5,
+                                      "tries": 5}, где
+                    timeout_window (int): время ожидания изменения окна
+                    tries (int): количество попыток для изменения окна
+            wait (bool): Флаг, указывающий, нужно ли ожидать выполнения двойного нажатия.
+
+        Возвращает:
+        - True, если двойное нажатие выполнено успешно; False в противном случае.
         """
+        decorator_args = {"timeout_window": 5,
+                          "tries": 5}
         if wait:
-            if not decorator_args:
-                decorator_args = {"timeout_window": 5,
-                                  "tries": 5}
-            return self._adb_multi_tap_to_element_and_wait(decorator_args=decorator_args)
+            return self._double_click_to_element_and_wait(decorator_args=decorator_args)
         else:
-            return self._adb_multi_tap_to_element()
+            return self._double_click_to_element()
 
-    def _adb_multi_tap_to_element(self) -> bool:
-        """
-        Выполняет три быстрых нажатия с помощью adb.
-        """
-        return self.__adb_multi_tap()
+    def _double_click_to_element(self) -> bool:
+        return self.__double_click()
 
     @wait_for_window_change()
-    def _adb_multi_tap_to_element_and_wait(self,
-                                           decorator_args: dict = None) -> bool:
-        """
-        Выполняет три быстрых нажатия с помощью adb и ожидает изменения окна.
-        """
-        return self.__adb_multi_tap()
+    def _double_click_to_element_and_wait(self, decorator_args: dict = None) -> bool:
+        return self.__double_click()
 
-    def __adb_multi_tap(self) -> bool:
+    def __double_click(self):
         """
-        Выполняет три быстрых нажатия с помощью adb.
-        Если подавать последовательно, через ";", то выполняются с задержкой в пару секунд.
-        Если подавать два тапа, то выполняются одновременно и сливаются.
-        С текущей конфигурацией команды - в 90% нажимает два раза. В 10% нажимает 3 раза.
-        Для выделения текста подходит.
+        Выполняет двойное нажатие (double click) на элементе.
+        Возвращает:
+        - True, если двойное нажатие выполнено успешно; False в противном случае.
         """
         try:
-            x, y = self._get_center()
-            # command = f'adb shell "input tap {x} {y} & input tap {x} {y} & input tap {x} {y}"'
-            command = ['adb', 'shell', f'input tap {x} {y} & input tap {x} {y} & input tap {x} {y}']
-
-            subprocess.run(command, check=True)
+            action = ActionChains(self.driver)
+            action.click(self).click(self).perform()
             return True
-        except Exception as e:
-            self.logger.error("__adb_multi_tap() ERROR:\n", e)
+        except InvalidElementStateException:
+            return True
+        except (ElementNotInteractableException, StaleElementReferenceException) as e:
+            self.logger.error(f"Не удалось тапнуть по элементу")
+            self.logger.error("{}".format(e))
             return False
 
-    def _adb_swipe(self,
-                   root,
-                   element: WebElement = None,
-                   x: int = None,
-                   y: int = None,
-                   direction: int = None,
-                   distance: int = None,
-                   duration: int = 1) -> bool:
-        """
-        Выполняет прокрутку с помощью adb.
-
-        Аргументы:
-            root: Корневой элемент на странице.
-            element (WebElement): Целевой элемент.
-            x (int): Координата X целевой позиции прокрутки.
-            y (int): Координата Y целевой позиции прокрутки.
-            direction (int): Направление прокрутки в градусах (от 0 до 360).
-            distance (int): Расстояние прокрутки в пикселях.
-            duration (int): Длительность прокрутки в секундах.
+    def _click_and_move(self,
+                        root=None,
+                        locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                        x: int = None,
+                        y: int = None,
+                        direction: int = None,
+                        distance: int = None,
+                        ) -> bool:
+        """
+        Нажимает левую кнопку мыши, перемещает курсор к указанной цели и отпускает кнопку.
+
+        Целью может быть WebElement, абсолютные координаты (x, y) или направление и расстояние.
+        Если предоставлены направление и расстояние, функция вычисляет целевую позицию
+        на основе вектора, определенного этими значениями.
+        Если предоставлены абсолютные координаты (x, y), курсор перемещается в указанные позиции.
+        Если предоставлен локатор, функция перемещается к найденному элементу на веб-странице.
+
+        Параметры:
+        - root: Первый элемент на странице.
+        - locator: Локатор для поиска целевого элемента на веб-странице.
+        - x: Абсолютная координата по оси X для перемещения курсора.
+        - y: Абсолютная координата по оси Y для перемещения курсора.
+        - direction: Направление в градусах для перемещения курсора, где 0/360 - вверх, 90 - вправо, 180 - вниз, 270 - влево.
+        - distance: Расстояние в пикселях для перемещения курсора.
 
         Возвращает:
-            bool: True, если прокрутка выполнена успешно; False в противном случае.
+        - True, если действие было успешно выполнено, в противном случае False.
+
+        Примечание: Если не предоставлены аргументы, функция возвращает False и регистрирует ошибку.
         """
-        # Проверка наличия входных данных
-        if element is None and (x is None or y is None) and (direction is None or distance is None):
-            return False
+        element = self
+        action = ActionChains(self.driver)
+        action.click_and_hold(element)
 
         # Получение координат центра начальной позиции прокрутки
         x1, y1 = self._get_center()
-        x2, y2 = self._get_center()
 
-        # Расчет целевой позиции прокрутки на основе предоставленных входных данных
-        if element is not None:
-            # Если предоставлен локатор, получаем координаты центра целевого элемента
-            x2, y2 = self._get_center(element)
+        if (x is None and y is None) and locator is None and (direction is None and distance is None):
+            # Если не предоставлены аргументы
+            self.logger.error(f"_click_and_move(): Нет аргументов")
+            return False
         elif x is not None and y is not None:
-            # Если предоставлены координаты x и y, используем их в качестве целевой позиции прокрутки
-            x2, y2 = x, y
+            # Если указаны абсолютные координаты (x, y) для перемещения курсора
+            action.move_by_offset(x-x1, y-y1)
+            action.release().perform()
+            return True
+        elif locator is not None and root is not None:
+            # Если указан локатор элемента и корневой элемент
+            target_element = root.get_element(locator)
+            action.move_to_element(target_element)
+            return True
         elif direction is not None and distance is not None:
             # Если предоставлены направление и расстояние, вычисляем целевую позицию прокрутки
-            window_size = adb.get_screen_resolution()
+            window_size = self.adb.get_screen_resolution()
             width = window_size[0]
             height = window_size[1]
+
             x2, y2 = find_coordinates_by_vector(width=width, height=height,
                                                 direction=direction, distance=distance,
                                                 start_x=x1, start_y=y1)
+            action.move_by_offset(x2-x1, y2-y1)
+            action.release().perform()
+            return True
 
-        # Выполнение adb-команды прокрутки с заданными координатами и длительностью
-        command = ['adb', 'shell', 'input', 'swipe', str(x1), str(y1), str(x2), str(y2), str(duration * 1000)]
-        subprocess.run(command, check=True)
+        return False
 
-        return True
```

### Comparing `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_click.py` & `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_tap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,215 +1,238 @@
 # coding: utf-8
 import logging
-from typing import Union, Tuple, Dict
+from typing import Union, Tuple, Dict, List, Optional
 
 from appium.webdriver import WebElement
 from selenium.webdriver.common.action_chains import ActionChains
-from selenium.common import ElementNotInteractableException, StaleElementReferenceException, \
-    InvalidElementStateException
+from selenium.webdriver.common.actions import interaction
+from selenium.webdriver.common.actions.action_builder import ActionBuilder
+from selenium.webdriver.common.actions.pointer_input import PointerInput
 
 import config
 
 from AppiumWebElementExtended.web_element_get import WebElementGet
-from adb import adb
+
 from AppiumHelpers.helpers_decorators import wait_for_window_change
 from utils.utils import find_coordinates_by_vector
 
 
-class WebElementClick(WebElementGet):
+class WebElementTap(WebElementGet):
     """
-    Класс для выполнения действий клика на элементе, двойного клика и клика с зажатием и перемещением курсора.
+    Класс для выполнения действий нажатия (Tap), а также нажатия и перемещения с использованием элементов веб-страницы.
     Наследуется от класса WebElementGet.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.driver = args[0]
         self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
 
-    def _click(self,
-               duration: int = 0,
-               decorator_args: dict = None,
-               wait: bool = False) -> bool:
+    def _tap(self,
+             positions: List[Tuple[int, int]],
+             duration: int = 0,
+             decorator_args: dict = None,
+             wait: bool = False) -> bool:
         """
-        Нажимает на элемент.
+        Выполняет нажатие на указанные координаты.
 
         Аргументы:
-            duration (int): Время в секундах для продолжительности нажатия (по умолчанию 0).
-            decorator_args (dict): Параметры для декоратора.
-                timeout_window (int): Время ожидания нового окна (умножается на количество попыток).
-                tries (int): Количество попыток нажатия (по умолчанию 3).
-            wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна.
-
-        Использование:
-            decorator_args = {"timeout_window": 5,
-                              "tries": 5}
-            element._click(duration=0, wait=True, decorator_args=decorator_args)
+            positions (List[Tuple[int, int]]): Список координат X и Y для нажатия.
+            duration (int): Длительность нажатия в миллисекундах.
+            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
+                    Например:
+                        decorator_args = {"timeout_window": 5,
+                                          "tries": 5}, где
+                        timeout_window (int): время ожидания изменения окна
+                        tries (int): количество попыток для изменения окна
+            wait (bool): Флаг, указывающий, нужно ли ожидать результата после нажатия.
 
         Возвращает:
             bool: True, если нажатие выполнено успешно; False в противном случае.
         """
+
         if wait:
-            # Если нужно ожидать изменения окна после нажатия
+            # Если нужно ожидать результата после нажатия
+
             if not decorator_args:
                 # Декоратор по умолчанию
                 decorator_args = {"timeout_window": 5,
                                   "tries": 5}
-            return self._click_to_element_and_wait(duration=duration, decorator_args=decorator_args)
+
+            return self._tap_to_element_and_wait(positions=positions, duration=duration, decorator_args=decorator_args)
         else:
             # Если не нужно ожидать результата после нажатия
-            return self._click_to_element(duration=duration)
-
-    def _click_to_element(self,
-                          duration: int = 0) -> bool:
-        return self.__click(duration=duration)
+            return self._tap_to_element(positions=positions, duration=duration)
 
     @wait_for_window_change()
-    def _click_to_element_and_wait(self,
-                                   duration: int = 0,
-                                   decorator_args: dict = None) -> bool:
-        return self.__click(duration=duration)
+    def _tap_to_element_and_wait(self,
+                                 positions: List[Tuple[int, int]],
+                                 duration: int = 0,
+                                 decorator_args: dict = None, ):
+        return self.__tap(positions=positions, duration=duration)
+
+    def _tap_to_element(self,
+                        positions: List[Tuple[int, int]],
+                        duration: int = 0, ):
+        return self.__tap(positions=positions, duration=duration)
 
-    def __click(self,
-                duration: int = 0) -> bool:
+    def __tap(self, positions: List[Tuple[int, int]], duration: Optional[int] = None):
         """
-        Выполняет клик на элементе.
+        Выполняет нажатие по указанным координатам.
 
         Аргументы:
-            duration (int): Длительность удержания клика в секундах.
+            positions (List[Tuple[int, int]]): Список координат X и Y для нажатия.
+            duration (Optional[int]): Длительность нажатия в миллисекундах.
 
         Возвращает:
-            bool: True, если клик выполнен успешно; False в противном случае.
+            bool: True, если нажатие выполнено успешно; False в противном случае.
         """
-        try:
-            action = ActionChains(self.driver)
-            element = self
 
-            if duration > 0:
-                # Если указана длительность клика, выполняется клик с удержанием на заданную длительность
-                action.click_and_hold(element).pause(duration / 1000).release()
-                action.perform()
-            else:
-                # Если не указана длительность клика, выполняется обычный клик
-                action.click(element).perform()
-
-        except (ElementNotInteractableException, StaleElementReferenceException, InvalidElementStateException) as e:
-            self.logger.error(f"Не удалось кликнуть по элементу")
-            self.logger.error("{}".format(e))
+        try:
+            self.driver.tap(positions=positions, duration=duration)
+            return True
+        except Exception as e:
+            self.logger.error("some exception with __tap(): {}".format(e))
             return False
-        return True
 
-    def _double_click(self,
-                      decorator_args: dict = None,
-                      wait: bool = False) -> bool:
+    def _double_tap(self,
+                    positions: Tuple[int, int],
+                    decorator_args: dict = None,
+                    wait: bool = False,
+                    pause: float = 0.2) -> bool:
         """
-        Выполняет двойное нажатие (double click) на элементе.
+        Выполняет двойное нажатие (double tap) на указанных координатах.
 
         Аргументы:
+            positions (Tuple[int, int]): Координаты X и Y для двойного нажатия.
             decorator_args (dict): Дополнительные аргументы для использования в декораторе.
                 Например:
                     decorator_args = {"timeout_window": 5,
                                       "tries": 5}, где
                     timeout_window (int): время ожидания изменения окна
                     tries (int): количество попыток для изменения окна
-            wait (bool): Флаг, указывающий, нужно ли ожидать выполнения двойного нажатия.
+            wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна после двойного нажатия.
+            pause (float): Пауза между двумя нажатиями в секундах.
 
         Возвращает:
-        - True, если двойное нажатие выполнено успешно; False в противном случае.
+            bool: True, если двойное нажатие выполнено успешно; False в противном случае.
         """
+
+        # Декоратор по умолчанию
         decorator_args = {"timeout_window": 5,
                           "tries": 5}
+
         if wait:
-            return self._double_click_to_element_and_wait(decorator_args=decorator_args)
+            # Если нужно ожидать результата после двойного нажатия
+            return self._double_tap_to_element_and_wait(positions=positions, decorator_args=decorator_args, pause=pause)
         else:
-            return self._double_click_to_element()
-
-    def _double_click_to_element(self) -> bool:
-        return self.__double_click()
+            # Если не нужно ожидать результата после двойного нажатия
+            return self._double_tap_to_element(positions=positions, pause=pause)
 
     @wait_for_window_change()
-    def _double_click_to_element_and_wait(self, decorator_args: dict = None) -> bool:
-        return self.__double_click()
+    def _double_tap_to_element_and_wait(self, positions: Tuple[int, int], decorator_args: dict = None,
+                                        pause: float = 0.2) -> bool:
+        return self.__double_tap(positions=positions, pause=pause)
 
-    def __double_click(self):
+    def _double_tap_to_element(self, positions: Tuple[int, int], pause: float = 0.2) -> bool:
+        return self.__double_tap(positions=positions, pause=pause)
+
+    def __double_tap(self, positions: Tuple[int, int], pause: float = 0.2) -> bool:
         """
-        Выполняет двойное нажатие (double click) на элементе.
+        Выполняет двойное нажатие (double tap) по указанным координатам.
+
+        Аргументы:
+            positions (Tuple[int, int]): Координаты X и Y для двойного нажатия.
+            pause (float): Пауза между двумя нажатиями в секундах.
+
         Возвращает:
-        - True, если двойное нажатие выполнено успешно; False в противном случае.
+            bool: True, если двойное нажатие выполнено успешно; False в противном случае.
         """
+        actions = ActionChains(self.driver)
+        actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
+        x = positions[0]
+        y = positions[1]
+
+        # Первое нажатие
+        actions.w3c_actions.pointer_action.move_to_location(x, y)
+        actions.w3c_actions.pointer_action.pointer_down()
+        actions.w3c_actions.pointer_action.pause(0.1)
+        actions.w3c_actions.pointer_action.pointer_up()
+        actions.w3c_actions.pointer_action.pause(pause)
+
+        # Второе нажатие
+        actions.w3c_actions.pointer_action.pointer_down()
+        actions.w3c_actions.pointer_action.pause(0.1)
+        actions.w3c_actions.pointer_action.release()
+
         try:
-            action = ActionChains(self.driver)
-            action.click(self).click(self).perform()
-            return True
-        except InvalidElementStateException:
+            actions.perform()
             return True
-        except (ElementNotInteractableException, StaleElementReferenceException) as e:
-            self.logger.error(f"Не удалось тапнуть по элементу")
-            self.logger.error("{}".format(e))
+        except Exception as e:
+            self.logger.error("some exception with __double_tap(): {}".format(e))
             return False
 
-    def _click_and_move(self,
-                        root=None,
-                        locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                        x: int = None,
-                        y: int = None,
-                        direction: int = None,
-                        distance: int = None,
-                        ) -> bool:
-        """
-        Нажимает левую кнопку мыши, перемещает курсор к указанной цели и отпускает кнопку.
-
-        Целью может быть WebElement, абсолютные координаты (x, y) или направление и расстояние.
-        Если предоставлены направление и расстояние, функция вычисляет целевую позицию
-        на основе вектора, определенного этими значениями.
-        Если предоставлены абсолютные координаты (x, y), курсор перемещается в указанные позиции.
-        Если предоставлен локатор, функция перемещается к найденному элементу на веб-странице.
-
-        Параметры:
-        - root: Первый элемент на странице.
-        - locator: Локатор для поиска целевого элемента на веб-странице.
-        - x: Абсолютная координата по оси X для перемещения курсора.
-        - y: Абсолютная координата по оси Y для перемещения курсора.
-        - direction: Направление в градусах для перемещения курсора, где 0/360 - вверх, 90 - вправо, 180 - вниз, 270 - влево.
-        - distance: Расстояние в пикселях для перемещения курсора.
+    def _tap_and_move(self,
+                      root=None,
+                      locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                      x: int = None,
+                      y: int = None,
+                      direction: int = None,
+                      distance: int = None,
+                      ) -> bool:
+        """
+        Выполняет операцию "нажать и переместить" на веб-элементе или на указанных координатах.
 
-        Возвращает:
-        - True, если действие было успешно выполнено, в противном случае False.
+        Аргументы:
+            root (WebElementExtended): Корневой элемент, относительно которого будет выполнено нажатие и перемещение.
+            locator (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str]): Локатор элемента,
+                на который будет выполнено нажатие и перемещение.
+            x (int): Координата X для нажатия и перемещения.
+            y (int): Координата Y для нажатия и перемещения.
+            direction (int): Направление прокрутки в градусах (0 - вверх, 90 - вправо, 180 - вниз, 270 - влево).
+            distance (int): Расстояние прокрутки в пикселях.
 
-        Примечание: Если не предоставлены аргументы, функция возвращает False и регистрирует ошибку.
+        Возвращает:
+            bool: True, если операция успешно выполнена; False в противном случае.
         """
-        element = self
-        action = ActionChains(self.driver)
-        action.click_and_hold(element)
-
         # Получение координат центра начальной позиции прокрутки
         x1, y1 = self._get_center()
 
+        actions = ActionChains(self.driver)
+        actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
+        actions.w3c_actions.pointer_action.move_to_location(x1, y1)
+        actions.w3c_actions.pointer_action.pointer_down()
+
+        # Проверка аргументов для определения типа операции
         if (x is None and y is None) and locator is None and (direction is None and distance is None):
             # Если не предоставлены аргументы
-            self.logger.error(f"_click_and_move(): Нет аргументов")
+            self.logger.error(f"_tap_and_move(): Нет аргументов")
             return False
         elif x is not None and y is not None:
-            # Если указаны абсолютные координаты (x, y) для перемещения курсора
-            action.move_by_offset(x-x1, y-y1)
-            action.release().perform()
+            # Если указаны координаты для нажатия и перемещения
+            actions.w3c_actions.pointer_action.move_to_location(x, y)
+            actions.w3c_actions.pointer_action.release()
+            actions.perform()
             return True
         elif locator is not None and root is not None:
             # Если указан локатор элемента и корневой элемент
             target_element = root.get_element(locator)
-            action.move_to_element(target_element)
+            x, y = target_element._get_center()
+            actions.w3c_actions.pointer_action.move_to_location(x, y)
+            actions.w3c_actions.pointer_action.release()
+            actions.perform()
             return True
         elif direction is not None and distance is not None:
             # Если предоставлены направление и расстояние, вычисляем целевую позицию прокрутки
-            window_size = adb.get_screen_resolution()
+            window_size = self.adb.get_screen_resolution()
             width = window_size[0]
             height = window_size[1]
 
             x2, y2 = find_coordinates_by_vector(width=width, height=height,
                                                 direction=direction, distance=distance,
                                                 start_x=x1, start_y=y1)
-            action.move_by_offset(x2-x1, y2-y1)
-            action.release().perform()
+            actions.w3c_actions.pointer_action.move_to_location(x2, y2)
+            actions.w3c_actions.pointer_action.release()
+            actions.perform()
             return True
 
         return False
-
```

### Comparing `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_dom.py` & `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_dom.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_extended.py` & `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,22 +126,14 @@
         tap by adb
         # TODO fill
         """
         assert self._adb_tap(wait=wait,
                              decorator_args=decorator_args)
         return cast('WebElementExtended', self)
 
-    def adb_multi_tap(self) -> 'WebElementExtended':
-        """
-        double tap by adb
-        # TODO fill
-        """
-        assert self._adb_multi_tap()
-        return cast('WebElementExtended', self)
-
     def adb_swipe(self,
                   locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
                   x: int = None,
                   y: int = None,
                   direction: int = None,
                   distance: int = None,
                   duration: int = 1,
```

### Comparing `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_get.py` & `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 import logging
 import time
 from typing import Union, Dict, List, Tuple
 
 import xml.etree.ElementTree as ET
 
 from appium.webdriver import WebElement
-from selenium.common import WebDriverException
+from selenium.common.exceptions import WebDriverException
 
 from appium.webdriver.common.mobileby import MobileBy
 from appium.webdriver.common.appiumby import AppiumBy
 from selenium.webdriver.common.by import By
 
 import config
 from AppiumHelpers.appium_helpers import AppiumHelpers
 from AppiumHelpers.appium_image import AppiumImage
+from terminal.terminal import Terminal
 
 
 class WebElementGet(WebElement):
     """
     Класс расширяющий Appium WebElement.
     Обеспечивает получение сущностей из элемента.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.driver = args[0]
         self.image = AppiumImage(driver=self.driver)
+        self.terminal = Terminal(driver=self.driver)
         self.helper = None
         self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
 
     def _get_element(self,
                      locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
                      by: Union[MobileBy, AppiumBy, By, str] = None,
                      value: Union[str, Dict, None] = None,
```

### Comparing `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_scroll.py` & `AppiumExtended-0.1.7/AppiumWebElementExtended/web_element_scroll.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 import logging
 import time
 from typing import Union, Tuple, Dict
 
 from appium.webdriver import WebElement
-from selenium.common import StaleElementReferenceException, NoSuchElementException, TimeoutException
+from selenium.common.exceptions import StaleElementReferenceException, NoSuchElementException, TimeoutException
 
 import config
 
 from AppiumWebElementExtended.web_element_get import WebElementGet
 
 
 class WebElementScroll(WebElementGet):
```

### Comparing `AppiumExtended-0.1.6/LICENSE` & `AppiumExtended-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.6/PKG-INFO` & `AppiumExtended-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: AppiumExtended
-Version: 0.1.6
+Version: 0.1.7
 Summary: An extension library for adding ease of use Appium-Python-Client
+Home-page: https://github.com/molokov-klim/appium_extended
 Author: molokov-klim
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `AppiumExtended-0.1.6/setup.py` & `AppiumExtended-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 An extension library for adding ease of use to Appium-Python-Client.
 
 AppiumExtended is a collection of utilities and convenience functions designed to enhance the usage of Appium-Python-Client for mobile app automation testing. It provides additional functionalities and abstractions to simplify the testing process.
 '''
 
 setup(
     name='AppiumExtended',
-    version='0.1.6',
+    version='0.1.7',
     description='An extension library for adding ease of use Appium-Python-Client',
     author='molokov-klim',
     packages=find_packages(),
     install_requires=[
         'Appium-Python-Client==2.11.1',
         'allure-pytest==2.13.2',
         'zlib-compress==0.0.1',
@@ -34,8 +34,9 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
+    url='https://github.com/molokov-klim/appium_extended',
 )
```

### Comparing `AppiumExtended-0.1.6/utils/utils.py` & `AppiumExtended-0.1.7/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,11 +172,7 @@
 
     # Вычисляем центр по оси y путем сложения y1 и y2, деленного на 2
     center_y = (y1 + y2) // 2
 
     # Возвращаем кортеж с центральными координатами (center_x, center_y)
     return center_x, center_y
 
-
-
-
-
```

