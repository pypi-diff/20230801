# Comparing `tmp/alertmanagermeshtastic-2023.8.1.6.tar.gz` & `tmp/alertmanagermeshtastic-2023.8.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.8.1.6.tar", last modified: Tue Aug  1 13:46:27 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.8.1.7.tar", last modified: Tue Aug  1 13:52:51 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.8.1.6.tar` & `alertmanagermeshtastic-2023.8.1.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.262514 alertmanagermeshtastic-2023.8.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-01 13:46:27.262514 alertmanagermeshtastic-2023.8.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 13:46:27.262514 alertmanagermeshtastic-2023.8.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.254513 alertmanagermeshtastic-2023.8.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.258514 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:46:18.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.258514 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.262514 alertmanagermeshtastic-2023.8.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:51.869368 alertmanagermeshtastic-2023.8.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-08-01 13:52:51.869368 alertmanagermeshtastic-2023.8.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 13:52:51.869368 alertmanagermeshtastic-2023.8.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:51.865367 alertmanagermeshtastic-2023.8.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:51.865367 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:51.869368 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-08-01 13:52:51.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 13:52:51.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:52:51.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 13:52:51.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:52:51.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:52:51.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 13:52:51.000000 alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:51.869368 alertmanagermeshtastic-2023.8.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 13:52:44.000000 alertmanagermeshtastic-2023.8.1.7/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.8.1.6/Dockerfile` & `alertmanagermeshtastic-2023.8.1.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/LICENSE` & `alertmanagermeshtastic-2023.8.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.6
+Version: 2023.8.1.7
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Project-URL: // Changelog, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/blob/main/CHANGES.rst
@@ -39,15 +39,15 @@
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python)
 [![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
 This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
 
 > **Warning**
-> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at [Contribution](#Contribution)
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
```

### Comparing `alertmanagermeshtastic-2023.8.1.6/README.md` & `alertmanagermeshtastic-2023.8.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python)
 [![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
 This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
 
 > **Warning**
-> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at [Contribution](#Contribution)
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
```

### Comparing `alertmanagermeshtastic-2023.8.1.6/setup.cfg` & `alertmanagermeshtastic-2023.8.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/cli.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/http.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/meshtastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,17 +129,16 @@
                                     alert["qn"],
                                     index,
                                     attempt,
                                 )
                                 break
 
                             # Check if timeout has been reached
-                            if (
-                                time.time() - start_time
-                                > self.connection.timeout
+                            if time.time() - start_time > int(
+                                self.connection.timeout
                             ):
                                 logger.debug(
                                     "\t [%s][%d][%d] Timeout reached on attempt %d!",
                                     alert["fingerprint"],
                                     alert["qn"],
                                     index,
                                     attempt,
```

### Comparing `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/processor.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.6
+Version: 2023.8.1.7
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Project-URL: // Changelog, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/blob/main/CHANGES.rst
@@ -39,15 +39,15 @@
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python)
 [![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
 This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
 
 > **Warning**
-> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at [Contribution](#Contribution)
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
```

### Comparing `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.8.1.7/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.8.1.7/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.8.1.7/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/tests/test_load_config.py` & `alertmanagermeshtastic-2023.8.1.7/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.8.1.7/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.8.1.7/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.6/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.8.1.7/tests/test_token_cli.py`

 * *Files identical despite different names*

