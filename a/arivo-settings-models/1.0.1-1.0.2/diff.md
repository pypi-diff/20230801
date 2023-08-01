# Comparing `tmp/arivo-settings_models-1.0.1.tar.gz` & `tmp/arivo-settings_models-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arivo-settings_models-1.0.1.tar", last modified: Mon Jul 31 09:04:36 2023, max compression
+gzip compressed data, was "dist/arivo-settings_models-1.0.2.tar", last modified: Tue Aug  1 07:19:08 2023, max compression
```

## Comparing `arivo-settings_models-1.0.1.tar` & `arivo-settings_models-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/docs/migrations.md
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/test-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/tools/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/tools/pages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/.coveragerc
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1440 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)    39686 2023-07-31 09:04:25.000000 arivo-settings_models-1.0.1/tests/test_validation.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11501 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/tests/test_serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/settings_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 09:04:25.000000 arivo-settings_models-1.0.1/settings_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6344 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/_combat.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/doc.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/settings_models/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 09:04:25.000000 arivo-settings_models-1.0.1/settings_models/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/settings/enforcement.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/settings/device_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    21017 2023-07-31 09:04:25.000000 arivo-settings_models-1.0.1/settings_models/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/settings/intercom.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/settings/gate_control.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/tox.ini
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)      704 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11501 2023-08-01 07:18:53.000000 arivo-settings_models-1.0.2/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/tests/test_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)    40248 2023-08-01 07:18:53.000000 arivo-settings_models-1.0.2/tests/test_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/docs/migrations.md
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/test-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/arivo_settings_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/arivo_settings_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/arivo_settings_models.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      704 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/arivo_settings_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/arivo_settings_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/arivo_settings_models.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/arivo_settings_models.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      922 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/arivo_settings_models.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/tools/pages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/settings_models/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/settings_models/_combat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/settings_models/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/settings_models/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/settings_models/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/settings_models/settings/gate_control.py
+-rw-rw-rw-   0 root         (0) root         (0)    21017 2023-08-01 07:18:53.000000 arivo-settings_models-1.0.2/settings_models/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/settings_models/settings/device_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-08-01 07:18:53.000000 arivo-settings_models-1.0.2/settings_models/settings/intercom.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 07:18:53.000000 arivo-settings_models-1.0.2/settings_models/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-14 09:15:36.000000 arivo-settings_models-1.0.2/settings_models/settings/enforcement.py
+-rw-rw-rw-   0 root         (0) root         (0)     6344 2023-08-01 07:18:53.000000 arivo-settings_models-1.0.2/settings_models/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 07:18:53.000000 arivo-settings_models-1.0.2/settings_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-08-01 07:19:08.000000 arivo-settings_models-1.0.2/AUTHORS
```

### Comparing `arivo-settings_models-1.0.1/.gitlab-ci.yml` & `arivo-settings_models-1.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/PKG-INFO` & `arivo-settings_models-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings_models
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-1.0.1/arivo_settings_models.egg-info/PKG-INFO` & `arivo-settings_models-1.0.2/arivo_settings_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings-models
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-1.0.1/arivo_settings_models.egg-info/SOURCES.txt` & `arivo-settings_models-1.0.2/arivo_settings_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/ChangeLog` & `arivo-settings_models-1.0.2/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v1.0.2
+------
+
+* intercom number nullable if not enabled
+
 v1.0.1
 ------
 
 * changes in support setting
 
 v1.0.0
 ------
@@ -67,8 +72,7 @@
 
 v0.0.0rc0
 ---------
 
 * added testcase for refs
 * coverage fix
 * removing pages stage because no documentation yet
-* settings models and parsing/serializing
```

### Comparing `arivo-settings_models-1.0.1/setup.cfg` & `arivo-settings_models-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/tests/test_validation.py` & `arivo-settings_models-1.0.2/tests/test_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -670,7 +670,18 @@
         gt = {"9999a7e2-be78-488e-8d1a-1486f7da9999": {
             "id": "0000a7e2-be78-488e-8d1a-1486f7da0000",
             "name": "Dauerparker ohne Kosten",
             "gates": ["gate1"],
             "default_cost_entries": []}}
         res = parse_setting("common/parksettings2", dump_setting(gt), custom_type=Parksettings)
         self.assert_result(res, gt)
+
+    def test_intercom(self):
+        setting_str = '{"enabled": false, "phone_number": null}'
+        res = parse_setting("intercom/basic_settings", setting_str)
+        self.assert_result(setting_str, dump_setting(res))
+
+        setting_str = '{"enabled": true, "phone_number": null}'
+        with self.assertRaises(ValidationError) as e:
+            res = parse_setting("intercom/basic_settings", setting_str)
+        self.assertEqual(str(e.exception).count("\n"), 2)
+        self.assertIn("phone_number must be set if intercom is enabled", str(e.exception))
```

### Comparing `arivo-settings_models-1.0.1/tests/utils.py` & `arivo-settings_models-1.0.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/tests/test_models.py` & `arivo-settings_models-1.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/tests/test_serialization.py` & `arivo-settings_models-1.0.2/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/settings_models/serialization.py` & `arivo-settings_models-1.0.2/settings_models/serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/settings_models/validators.py` & `arivo-settings_models-1.0.2/settings_models/validators.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/settings_models/settings/device_keys.py` & `arivo-settings_models-1.0.2/settings_models/settings/device_keys.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/settings_models/settings/common.py` & `arivo-settings_models-1.0.2/settings_models/settings/common.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.1/settings_models/settings/gate_control.py` & `arivo-settings_models-1.0.2/settings_models/settings/gate_control.py`

 * *Files identical despite different names*

