# Comparing `tmp/alertmanagermeshtastic-2023.8.1.11.tar.gz` & `tmp/alertmanagermeshtastic-2023.8.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.8.1.11.tar", last modified: Tue Aug  1 20:20:05 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.8.1.12.tar", last modified: Tue Aug  1 20:24:27 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.8.1.11.tar` & `alertmanagermeshtastic-2023.8.1.12.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:05.685161 alertmanagermeshtastic-2023.8.1.11/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-01 20:20:05.685161 alertmanagermeshtastic-2023.8.1.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-01 20:20:05.685161 alertmanagermeshtastic-2023.8.1.11/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:05.677161 alertmanagermeshtastic-2023.8.1.11/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:05.681161 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:05.681161 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-01 20:20:05.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 20:20:05.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:20:05.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 20:20:05.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:20:05.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 20:20:05.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 20:20:05.000000 alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:05.685161 alertmanagermeshtastic-2023.8.1.11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 20:19:56.000000 alertmanagermeshtastic-2023.8.1.11/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:24:27.734417 alertmanagermeshtastic-2023.8.1.12/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-01 20:24:27.734417 alertmanagermeshtastic-2023.8.1.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-01 20:24:27.734417 alertmanagermeshtastic-2023.8.1.12/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:24:27.726416 alertmanagermeshtastic-2023.8.1.12/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:24:27.730416 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 20:24:20.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:24:27.734417 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-01 20:24:27.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 20:24:27.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:24:27.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 20:24:27.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:24:27.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 20:24:27.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 20:24:27.000000 alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:24:27.734417 alertmanagermeshtastic-2023.8.1.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 20:24:19.000000 alertmanagermeshtastic-2023.8.1.12/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.8.1.11/Dockerfile` & `alertmanagermeshtastic-2023.8.1.12/Dockerfile`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/LICENSE` & `alertmanagermeshtastic-2023.8.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.11
+Version: 2023.8.1.12
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
```

### Comparing `alertmanagermeshtastic-2023.8.1.11/README.md` & `alertmanagermeshtastic-2023.8.1.12/README.md`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/setup.cfg` & `alertmanagermeshtastic-2023.8.1.12/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/cli.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/http.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/meshtastic.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/processor.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.11
+Version: 2023.8.1.12
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
```

### Comparing `alertmanagermeshtastic-2023.8.1.11/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.8.1.12/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.8.1.12/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.8.1.12/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/tests/test_load_config.py` & `alertmanagermeshtastic-2023.8.1.12/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.8.1.12/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.8.1.12/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.11/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.8.1.12/tests/test_token_cli.py`

 * *Files identical despite different names*

