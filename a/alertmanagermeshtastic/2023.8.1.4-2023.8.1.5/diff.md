# Comparing `tmp/alertmanagermeshtastic-2023.8.1.4.tar.gz` & `tmp/alertmanagermeshtastic-2023.8.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.8.1.4.tar", last modified: Tue Aug  1 13:03:10 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.8.1.5.tar", last modified: Tue Aug  1 13:24:12 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.8.1.4.tar` & `alertmanagermeshtastic-2023.8.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:10.284635 alertmanagermeshtastic-2023.8.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-08-01 13:03:10.284635 alertmanagermeshtastic-2023.8.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 13:03:10.288635 alertmanagermeshtastic-2023.8.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:10.280635 alertmanagermeshtastic-2023.8.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:10.284635 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:10.284635 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-08-01 13:03:10.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 13:03:10.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:03:10.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 13:03:10.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:03:10.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:03:10.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 13:03:10.000000 alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:03:10.284635 alertmanagermeshtastic-2023.8.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 13:03:00.000000 alertmanagermeshtastic-2023.8.1.4/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.550733 alertmanagermeshtastic-2023.8.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.554733 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.8.1.4/Dockerfile` & `alertmanagermeshtastic-2023.8.1.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/LICENSE` & `alertmanagermeshtastic-2023.8.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.4
+Version: 2023.8.1.5
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Project-URL: // Changelog, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/blob/main/CHANGES.rst
```

### Comparing `alertmanagermeshtastic-2023.8.1.4/README.md` & `alertmanagermeshtastic-2023.8.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/setup.cfg` & `alertmanagermeshtastic-2023.8.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/cli.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/http.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/meshtastic.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,18 +214,18 @@
             message += "Instance: " + alert["labels"]["instance"] + "\n"
         elif "alertname" in alert["labels"]:
             message += "Alert: " + alert["labels"]["alertname"] + "\n"
         if "info" in alert["annotations"]:
             message += "Info: " + alert["annotations"]["info"] + "\n"
         if "summary" in alert["annotations"]:
             message += "Summary: " + alert["annotations"]["summary"] + "\n"
-        if 'description' in alert['annotations']:
-            message += (
-                "Description: " + alert['annotations']['description'] + "\n"
-            )
+        # if 'description' in alert['annotations']:
+        #     message += (
+        #         "Description: " + alert['annotations']['description'] + "\n"
+        #     )
         if alert["status"] == "resolved":
             correctdate = parser.parse(alert["endsAt"]).strftime(
                 "%Y-%m-%d %H:%M:%S"
             )
             message += "Resolved: " + correctdate
         elif alert["status"] == "firing":
             correctdate = parser.parse(alert["startsAt"]).strftime(
```

### Comparing `alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/processor.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.4
+Version: 2023.8.1.5
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Project-URL: // Changelog, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/blob/main/CHANGES.rst
```

### Comparing `alertmanagermeshtastic-2023.8.1.4/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.8.1.5/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.8.1.5/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/tests/test_load_config.py` & `alertmanagermeshtastic-2023.8.1.5/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.8.1.5/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.8.1.5/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.4/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.8.1.5/tests/test_token_cli.py`

 * *Files identical despite different names*

