# Comparing `tmp/pywemo-1.2.0.tar.gz` & `tmp/pywemo-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywemo-1.2.0.tar", max compression
+gzip compressed data, was "pywemo-1.2.1.tar", max compression
```

## Comparing `pywemo-1.2.0.tar` & `pywemo-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     2831 2023-07-31 02:36:23.986254 pywemo-1.2.0/LICENSE
--rw-r--r--   0        0        0     8322 2023-07-31 02:36:23.986254 pywemo-1.2.0/README.rst
--rw-r--r--   0        0        0     3196 2023-07-31 02:36:23.986254 pywemo-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2889 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/README.md
--rw-r--r--   0        0        0     1254 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/__init__.py
--rw-r--r--   0        0        0     2762 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/color.py
--rw-r--r--   0        0        0     6806 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/discovery.py
--rw-r--r--   0        0        0     2753 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/exceptions.py
--rw-r--r--   0        0        0     1468 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/LICENSE
--rw-r--r--   0        0        0    26370 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/__init__.py
--rw-r--r--   0        0        0       23 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/__init__.py
--rw-r--r--   0        0        0     4843 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/attributes.py
--rw-r--r--   0        0        0     6733 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/db_orm.py
--rw-r--r--   0        0        0     6059 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/long_press.py
--rw-r--r--   0        0        0    14976 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/rules_db.py
--rw-r--r--   0        0        0    12705 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/service.py
--rw-r--r--   0        0        0      912 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/wemo_services.py
--rw-r--r--   0        0        0     6838 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/wemo_services.pyi
--rw-r--r--   0        0        0       60 2023-07-31 02:36:23.986254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/__init__.py
--rw-r--r--   0        0        0   126828 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/device.py
--rw-r--r--   0        0        0     4305 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/device.xsd
--rw-r--r--   0        0        0   122520 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/service.py
--rw-r--r--   0        0        0     3526 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/service.xsd
--rw-r--r--   0        0        0     7275 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd_types.py
--rw-r--r--   0        0        0    18975 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/bridge.py
--rw-r--r--   0        0        0     3345 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/coffeemaker.py
--rw-r--r--   0        0        0     5035 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/crockpot.py
--rw-r--r--   0        0        0     2250 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/dimmer.py
--rw-r--r--   0        0        0     7162 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/humidifier.py
--rw-r--r--   0        0        0     6125 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/insight.py
--rw-r--r--   0        0        0      328 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/lightswitch.py
--rw-r--r--   0        0        0     1645 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/maker.py
--rw-r--r--   0        0        0      141 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/motion.py
--rw-r--r--   0        0        0      157 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/outdoor_plug.py
--rw-r--r--   0        0        0     1023 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ouimeaux_device/switch.py
--rw-r--r--   0        0        0        0 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/py.typed
--rw-r--r--   0        0        0    12531 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/ssdp.py
--rw-r--r--   0        0        0    28315 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/subscribe.py
--rw-r--r--   0        0        0     4417 2023-07-31 02:36:23.990254 pywemo-1.2.0/pywemo/util.py
--rw-r--r--   0        0        0     9084 1970-01-01 00:00:00.000000 pywemo-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-08-01 05:46:07.880125 pywemo-1.2.1/LICENSE
+-rw-r--r--   0        0        0     8322 2023-08-01 05:46:07.880125 pywemo-1.2.1/README.rst
+-rw-r--r--   0        0        0     3196 2023-08-01 05:46:07.884125 pywemo-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2889 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/README.md
+-rw-r--r--   0        0        0     1254 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/__init__.py
+-rw-r--r--   0        0        0     2762 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/color.py
+-rw-r--r--   0        0        0     6806 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/discovery.py
+-rw-r--r--   0        0        0     2759 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/exceptions.py
+-rw-r--r--   0        0        0     1468 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/LICENSE
+-rw-r--r--   0        0        0    26370 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/__init__.py
+-rw-r--r--   0        0        0       23 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/__init__.py
+-rw-r--r--   0        0        0     4843 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/attributes.py
+-rw-r--r--   0        0        0     6733 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/db_orm.py
+-rw-r--r--   0        0        0     6059 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/long_press.py
+-rw-r--r--   0        0        0    14976 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/rules_db.py
+-rw-r--r--   0        0        0    12705 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/service.py
+-rw-r--r--   0        0        0      912 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/wemo_services.py
+-rw-r--r--   0        0        0     6838 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/wemo_services.pyi
+-rw-r--r--   0        0        0       60 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/__init__.py
+-rw-r--r--   0        0        0   126828 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/device.py
+-rw-r--r--   0        0        0     4305 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/device.xsd
+-rw-r--r--   0        0        0   122520 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/service.py
+-rw-r--r--   0        0        0     3526 2023-08-01 05:46:07.884125 pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/service.xsd
+-rw-r--r--   0        0        0     7275 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd_types.py
+-rw-r--r--   0        0        0    18975 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/bridge.py
+-rw-r--r--   0        0        0     3345 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/coffeemaker.py
+-rw-r--r--   0        0        0     5035 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/crockpot.py
+-rw-r--r--   0        0        0     2250 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/dimmer.py
+-rw-r--r--   0        0        0     7162 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/humidifier.py
+-rw-r--r--   0        0        0     6125 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/insight.py
+-rw-r--r--   0        0        0      328 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/lightswitch.py
+-rw-r--r--   0        0        0     1645 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/maker.py
+-rw-r--r--   0        0        0      141 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/motion.py
+-rw-r--r--   0        0        0      157 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/outdoor_plug.py
+-rw-r--r--   0        0        0     1023 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ouimeaux_device/switch.py
+-rw-r--r--   0        0        0        0 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/py.typed
+-rw-r--r--   0        0        0    12531 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/ssdp.py
+-rw-r--r--   0        0        0    28315 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/subscribe.py
+-rw-r--r--   0        0        0     4417 2023-08-01 05:46:07.888125 pywemo-1.2.1/pywemo/util.py
+-rw-r--r--   0        0        0     9084 1970-01-01 00:00:00.000000 pywemo-1.2.1/PKG-INFO
```

### Comparing `pywemo-1.2.0/LICENSE` & `pywemo-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/README.rst` & `pywemo-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pyproject.toml` & `pywemo-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pywemo"
-version = "1.2.0"
+version = "1.2.1"
 description = "Lightweight Python module to discover and control WeMo devices"
 authors = ["Eric Severance <pywemo@esev.com>"]
 license = "MIT"
 
 readme = 'README.rst'
 
 repository = "https://github.com/pywemo/pywemo"
```

### Comparing `pywemo-1.2.0/pywemo/README.md` & `pywemo-1.2.1/pywemo/README.md`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/__init__.py` & `pywemo-1.2.1/pywemo/__init__.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/color.py` & `pywemo-1.2.1/pywemo/color.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/discovery.py` & `pywemo-1.2.1/pywemo/discovery.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/exceptions.py` & `pywemo-1.2.1/pywemo/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     """HTTP request to the device failed."""
 
 
 class HTTPNotOkException(HTTPException):
     """Raised when a non-200 status is returned."""
 
 
-class RulesDbError(Exception):
+class RulesDbError(PyWeMoException):
     """Base class for errors related to the Rules database."""
 
 
 class RulesDbQueryError(RulesDbError):
     """Exception when querying the rules database."""
```

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/LICENSE` & `pywemo-1.2.1/pywemo/ouimeaux_device/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/__init__.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/__init__.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/attributes.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/attributes.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/db_orm.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/db_orm.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/long_press.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/long_press.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/rules_db.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/rules_db.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/service.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/service.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/wemo_services.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/wemo_services.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/wemo_services.pyi` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/wemo_services.pyi`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/device.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/device.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/device.xsd` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/device.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/service.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/service.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd/service.xsd` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd/service.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/api/xsd_types.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/api/xsd_types.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/bridge.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/bridge.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/coffeemaker.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/coffeemaker.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/crockpot.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/crockpot.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/dimmer.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/dimmer.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/humidifier.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/humidifier.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/insight.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/insight.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/maker.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/maker.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ouimeaux_device/switch.py` & `pywemo-1.2.1/pywemo/ouimeaux_device/switch.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/ssdp.py` & `pywemo-1.2.1/pywemo/ssdp.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/subscribe.py` & `pywemo-1.2.1/pywemo/subscribe.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/pywemo/util.py` & `pywemo-1.2.1/pywemo/util.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.2.0/PKG-INFO` & `pywemo-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywemo
-Version: 1.2.0
+Version: 1.2.1
 Summary: Lightweight Python module to discover and control WeMo devices
 Home-page: https://github.com/pywemo/pywemo
 License: MIT
 Keywords: wemo,api
 Author: Eric Severance
 Author-email: pywemo@esev.com
 Requires-Python: >=3.8.1,<4.0.0
```

