# Comparing `tmp/alertmanagermeshtastic-2023.8.1.5.tar.gz` & `tmp/alertmanagermeshtastic-2023.8.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.8.1.5.tar", last modified: Tue Aug  1 13:24:12 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.8.1.6.tar", last modified: Tue Aug  1 13:46:27 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.8.1.5.tar` & `alertmanagermeshtastic-2023.8.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.550733 alertmanagermeshtastic-2023.8.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.554733 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 13:24:12.000000 alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:24:12.558733 alertmanagermeshtastic-2023.8.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 13:24:03.000000 alertmanagermeshtastic-2023.8.1.5/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.262514 alertmanagermeshtastic-2023.8.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-01 13:46:27.262514 alertmanagermeshtastic-2023.8.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 13:46:27.262514 alertmanagermeshtastic-2023.8.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.254513 alertmanagermeshtastic-2023.8.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.258514 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:46:18.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.258514 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 13:46:27.000000 alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:46:27.262514 alertmanagermeshtastic-2023.8.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 13:46:17.000000 alertmanagermeshtastic-2023.8.1.6/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.8.1.5/Dockerfile` & `alertmanagermeshtastic-2023.8.1.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/LICENSE` & `alertmanagermeshtastic-2023.8.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.5
+Version: 2023.8.1.6
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Project-URL: // Changelog, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/blob/main/CHANGES.rst
@@ -33,53 +33,68 @@
 License-File: LICENSE
 
 # Alertmanager webhook for meshtastic
 
 [![linux/amd64](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/actions/workflows/build-linux-image.yml/badge.svg)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/actions/workflows/build-linux-image.yml)
 [![dockerhub](https://img.shields.io/badge/dockerhub-images-important.svg?logo=Docker)](https://hub.docker.com/r/apfelwurm/alertmanager-webhook-meshtastic-python)
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python)
+[![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
-This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID. (currently not working and docs not updated!)
+This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
+
+> **Warning**
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at [Contribution](#Contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
+
+```
 	receivers:
 	- name: 'meshtastic-webhook'
 	  webhook_configs:
-	  - url: http://ipFlaskAlert:9119/alert
+	  - url: http://alertmanager-meshtastic:9119/alert
 	    send_resolved: true
-	    http_config:
-	      basic_auth:
-		username: 'XXXUSERNAME'
-		password: 'XXXPASSWORD'
+```
+
+## config.toml example
+
+This is an example config, that shows all of the config options.
+
+```
+log_level = "debug"
+
+[http]
+host = "0.0.0.0"
+port = 9119
+
+[meshtastic.connection]
+tty = "/tmp/vcom0"
+nodeid = 631724152
+maxsendingattempts = 30
+timeout = 60
+```
+
 
 ##  docker compose service example - Hardware Serial (default)
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanager-webhook-meshtastic-python
       ports:
         - 9119:9119
       volumes:
         - /tmp/vcom0:/tmp/vcom0
-      environment:
-        - meshtty=/tmp/vcom0
-        - nodeID=631724152
-        - maxsendingattempts=5
-        - auth=true
-        - username=XXXUSERNAME
-        - password=XXXPASSWORD
-        - loglevel=WARNING
+        - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 ##  docker compose service example - Virtual Serial
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
@@ -87,60 +102,43 @@
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanager-webhook-meshtastic-python
       ports:
         - 9119:9119
       volumes:
         - /tmp/vcom0:/tmp/vcom0
-      environment:
-        - meshtty=/tmp/vcom0
-        - nodeID=631724152
-        - maxsendingattempts=5
-        - auth=true
-        - username=XXXUSERNAME
-        - password=XXXPASSWORD
-        - loglevel=WARNING
+        - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 
 ##  Running on docker example - Hardware Serial (default)
 
 ```
     docker run -d --name alertmanager-webhook-meshtastic-python \
 		--device=/dev/ttyACM0 \
-		-e "meshtty=/dev/ttyACM0" \
-      -e "maxsendingattempts=5" \
-    	-e "nodeID=123456789" \
-    	-e "auth=true" \
-    	-e "username=XXXUSERNAME" \
-    	-e "password=XXXPASSWORD" \
-    	-e "loglevel=WARNING" \
-    	-p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
+		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
+    -p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
 ```
 
 ##  Running on docker example - Virtual Serial
 
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     docker run -d --name alertmanager-webhook-meshtastic-python \
 		-v /tmp/vcom0:/tmp/vcom0 \
-		-e "meshtty=/tmp/vcom0" \
-    	-e "nodeID=123456789" \
-      -e "maxsendingattempts=5" \
-    	-e "auth=true" \
-    	-e "username=XXXUSERNAME" \
-    	-e "password=XXXPASSWORD" \
-    	-e "loglevel=WARNING" \
-    	-p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
+		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
+    -p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
 ```
 
 ## Contribution
 
-This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. I would appreciate any help.
+This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. You can also take a look on the opened Issues, where i have opened some for planned features and work on them if you want. I would appreciate any help.
 
 
 ## Example to test
+
+You can use the test.sh or the test single.sh or the following curl command to test alertmanager-meshtastic
 ```
-	curl -XPOST --data '{"status":"resolved","groupLabels":{"alertname":"instance_down"},"commonAnnotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"},"alerts":[{"status":"resolved","labels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"},"endsAt":"2019-07-01T16:16:19.376244942-03:00","generatorURL":"http://pmts.io:9090","startsAt":"2019-07-01T16:02:19.376245319-03:00","annotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"}}],"version":"4","receiver":"infra-alert","externalURL":"http://alm.io:9093","commonLabels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"}}' http://XXXUSERNAME:XXXPASSWORD@flaskAlert:9119/alert
+	curl -XPOST --data '{"status":"resolved","groupLabels":{"alertname":"instance_down"},"commonAnnotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"},"alerts":[{"status":"resolved","labels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"},"endsAt":"2019-07-01T16:16:19.376244942-03:00","generatorURL":"http://pmts.io:9090","startsAt":"2019-07-01T16:02:19.376245319-03:00","annotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"}}],"version":"4","receiver":"infra-alert","externalURL":"http://alm.io:9093","commonLabels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"}}' http://alertmanager-meshtastic:9119/alert
 ```
```

### Comparing `alertmanagermeshtastic-2023.8.1.5/README.md` & `alertmanagermeshtastic-2023.8.1.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 # Alertmanager webhook for meshtastic
 
 [![linux/amd64](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/actions/workflows/build-linux-image.yml/badge.svg)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/actions/workflows/build-linux-image.yml)
 [![dockerhub](https://img.shields.io/badge/dockerhub-images-important.svg?logo=Docker)](https://hub.docker.com/r/apfelwurm/alertmanager-webhook-meshtastic-python)
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python)
+[![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
-This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID. (currently not working and docs not updated!)
+This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
+
+> **Warning**
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at [Contribution](#Contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
+
+```
 	receivers:
 	- name: 'meshtastic-webhook'
 	  webhook_configs:
-	  - url: http://ipFlaskAlert:9119/alert
+	  - url: http://alertmanager-meshtastic:9119/alert
 	    send_resolved: true
-	    http_config:
-	      basic_auth:
-		username: 'XXXUSERNAME'
-		password: 'XXXPASSWORD'
+```
+
+## config.toml example
+
+This is an example config, that shows all of the config options.
+
+```
+log_level = "debug"
+
+[http]
+host = "0.0.0.0"
+port = 9119
+
+[meshtastic.connection]
+tty = "/tmp/vcom0"
+nodeid = 631724152
+maxsendingattempts = 30
+timeout = 60
+```
+
 
 ##  docker compose service example - Hardware Serial (default)
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanager-webhook-meshtastic-python
       ports:
         - 9119:9119
       volumes:
         - /tmp/vcom0:/tmp/vcom0
-      environment:
-        - meshtty=/tmp/vcom0
-        - nodeID=631724152
-        - maxsendingattempts=5
-        - auth=true
-        - username=XXXUSERNAME
-        - password=XXXPASSWORD
-        - loglevel=WARNING
+        - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 ##  docker compose service example - Virtual Serial
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
@@ -53,60 +68,43 @@
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanager-webhook-meshtastic-python
       ports:
         - 9119:9119
       volumes:
         - /tmp/vcom0:/tmp/vcom0
-      environment:
-        - meshtty=/tmp/vcom0
-        - nodeID=631724152
-        - maxsendingattempts=5
-        - auth=true
-        - username=XXXUSERNAME
-        - password=XXXPASSWORD
-        - loglevel=WARNING
+        - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 
 ##  Running on docker example - Hardware Serial (default)
 
 ```
     docker run -d --name alertmanager-webhook-meshtastic-python \
 		--device=/dev/ttyACM0 \
-		-e "meshtty=/dev/ttyACM0" \
-      -e "maxsendingattempts=5" \
-    	-e "nodeID=123456789" \
-    	-e "auth=true" \
-    	-e "username=XXXUSERNAME" \
-    	-e "password=XXXPASSWORD" \
-    	-e "loglevel=WARNING" \
-    	-p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
+		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
+    -p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
 ```
 
 ##  Running on docker example - Virtual Serial
 
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     docker run -d --name alertmanager-webhook-meshtastic-python \
 		-v /tmp/vcom0:/tmp/vcom0 \
-		-e "meshtty=/tmp/vcom0" \
-    	-e "nodeID=123456789" \
-      -e "maxsendingattempts=5" \
-    	-e "auth=true" \
-    	-e "username=XXXUSERNAME" \
-    	-e "password=XXXPASSWORD" \
-    	-e "loglevel=WARNING" \
-    	-p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
+		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
+    -p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
 ```
 
 ## Contribution
 
-This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. I would appreciate any help.
+This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. You can also take a look on the opened Issues, where i have opened some for planned features and work on them if you want. I would appreciate any help.
 
 
 ## Example to test
+
+You can use the test.sh or the test single.sh or the following curl command to test alertmanager-meshtastic
 ```
-	curl -XPOST --data '{"status":"resolved","groupLabels":{"alertname":"instance_down"},"commonAnnotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"},"alerts":[{"status":"resolved","labels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"},"endsAt":"2019-07-01T16:16:19.376244942-03:00","generatorURL":"http://pmts.io:9090","startsAt":"2019-07-01T16:02:19.376245319-03:00","annotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"}}],"version":"4","receiver":"infra-alert","externalURL":"http://alm.io:9093","commonLabels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"}}' http://XXXUSERNAME:XXXPASSWORD@flaskAlert:9119/alert
+	curl -XPOST --data '{"status":"resolved","groupLabels":{"alertname":"instance_down"},"commonAnnotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"},"alerts":[{"status":"resolved","labels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"},"endsAt":"2019-07-01T16:16:19.376244942-03:00","generatorURL":"http://pmts.io:9090","startsAt":"2019-07-01T16:02:19.376245319-03:00","annotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"}}],"version":"4","receiver":"infra-alert","externalURL":"http://alm.io:9093","commonLabels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"}}' http://alertmanager-meshtastic:9119/alert
 ```
```

### Comparing `alertmanagermeshtastic-2023.8.1.5/setup.cfg` & `alertmanagermeshtastic-2023.8.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/cli.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import rtoml
 
 DEFAULT_HTTP_HOST = '127.0.0.1'
 DEFAULT_HTTP_PORT = 9119
 DEFAULT_MESHTASTIC_NODEID = 123456789
 DEFAULT_MESHTASTIC_MAXSENDINGATTEMPTS = 5
+DEFAULT_MESHTASTIC_TIMEOUT = 60
 
 
 class ConfigurationError(Exception):
     """Indicates a configuration error."""
 
 
 @dataclass(frozen=True)
@@ -44,14 +45,15 @@
 @dataclass(frozen=True)
 class MeshtasticConnection:
     """An MESHTASTIC connection."""
 
     tty: str
     nodeid: int = DEFAULT_MESHTASTIC_NODEID
     maxsendingattempts: int = DEFAULT_MESHTASTIC_MAXSENDINGATTEMPTS
+    timeout: int = DEFAULT_MESHTASTIC_TIMEOUT
 
 
 @dataclass(frozen=True)
 class MeshtasticConfig:
     """An MESHTASTIC Interface configuration."""
 
     connection: Optional[MeshtasticConnection]
@@ -104,16 +106,20 @@
     data_meshtastic: Any,
 ) -> Optional[MeshtasticConnection]:
     data_connection = data_meshtastic.get('connection')
     if data_connection is None:
         return None
 
     maxsendingattempts = data_connection.get('maxsendingattempts')
+    timeout = data_connection.get('timeout')
     tty = data_connection.get('tty')
     if not tty:
         return None
 
     nodeid = int(data_connection.get('nodeid', DEFAULT_MESHTASTIC_NODEID))
 
     return MeshtasticConnection(
-        tty=tty, nodeid=nodeid, maxsendingattempts=maxsendingattempts
+        tty=tty,
+        nodeid=nodeid,
+        maxsendingattempts=maxsendingattempts,
+        timeout=timeout,
     )
```

### Comparing `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/http.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/meshtastic.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,18 +44,19 @@
         self.connection = connection
 
         self.meshtasticinterface = _create_meshtasticinterface(connection)
 
     def start(self) -> None:
         """Connect to the connection, in a separate thread."""
         logger.info(
-            '\t Connecting to MESHTASTIC connection %s, the node is %d and messages will be sent %d times before failing',
+            '\t Connecting to MESHTASTIC connection %s, the node is %d and messages will be sent %d times with timeout %d before failing',
             self.connection.tty,
             self.connection.nodeid,
             self.connection.maxsendingattempts,
+            self.connection.timeout,
         )
 
         # start_thread(self.meshtasticinterface.start)
 
     def announce(self, alert: str) -> None:
         """Announce a message."""
         try:
@@ -112,18 +113,15 @@
                             True,
                             False,
                             self.meshtasticinterface.getNode(
                                 self.connection.nodeid, False
                             ).onAckNak,
                         )
                         self.meshtasticinterface.waitForAckNak()
-
                         start_time = time.time()
-                        timeout = 60
-
                         while True:
                             # Check if value is True
                             if (
                                 self.meshtasticinterface._acknowledgment.receivedAck
                             ):
                                 logger.debug(
                                     "\t [%s][%d][%d] got ack received from meshtastic on attempt %d",
@@ -131,15 +129,18 @@
                                     alert["qn"],
                                     index,
                                     attempt,
                                 )
                                 break
 
                             # Check if timeout has been reached
-                            if time.time() - start_time > timeout:
+                            if (
+                                time.time() - start_time
+                                > self.connection.timeout
+                            ):
                                 logger.debug(
                                     "\t [%s][%d][%d] Timeout reached on attempt %d!",
                                     alert["fingerprint"],
                                     alert["qn"],
                                     index,
                                     attempt,
                                 )
```

### Comparing `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/processor.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.5
+Version: 2023.8.1.6
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python
 Project-URL: // Changelog, https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/blob/main/CHANGES.rst
@@ -33,53 +33,68 @@
 License-File: LICENSE
 
 # Alertmanager webhook for meshtastic
 
 [![linux/amd64](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/actions/workflows/build-linux-image.yml/badge.svg)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python/actions/workflows/build-linux-image.yml)
 [![dockerhub](https://img.shields.io/badge/dockerhub-images-important.svg?logo=Docker)](https://hub.docker.com/r/apfelwurm/alertmanager-webhook-meshtastic-python)
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanager-webhook-meshtastic-python)
+[![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
-This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID. (currently not working and docs not updated!)
+This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
+
+> **Warning**
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at [Contribution](#Contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
+
+```
 	receivers:
 	- name: 'meshtastic-webhook'
 	  webhook_configs:
-	  - url: http://ipFlaskAlert:9119/alert
+	  - url: http://alertmanager-meshtastic:9119/alert
 	    send_resolved: true
-	    http_config:
-	      basic_auth:
-		username: 'XXXUSERNAME'
-		password: 'XXXPASSWORD'
+```
+
+## config.toml example
+
+This is an example config, that shows all of the config options.
+
+```
+log_level = "debug"
+
+[http]
+host = "0.0.0.0"
+port = 9119
+
+[meshtastic.connection]
+tty = "/tmp/vcom0"
+nodeid = 631724152
+maxsendingattempts = 30
+timeout = 60
+```
+
 
 ##  docker compose service example - Hardware Serial (default)
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanager-webhook-meshtastic-python
       ports:
         - 9119:9119
       volumes:
         - /tmp/vcom0:/tmp/vcom0
-      environment:
-        - meshtty=/tmp/vcom0
-        - nodeID=631724152
-        - maxsendingattempts=5
-        - auth=true
-        - username=XXXUSERNAME
-        - password=XXXPASSWORD
-        - loglevel=WARNING
+        - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 ##  docker compose service example - Virtual Serial
 
 To integrate this bridge into your composed prometheus/alertmanager cluster, this is a good startingpoint.
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
@@ -87,60 +102,43 @@
 ```
     alertmanagermeshtastic:
       image: apfelwurm/alertmanager-webhook-meshtastic-python
       ports:
         - 9119:9119
       volumes:
         - /tmp/vcom0:/tmp/vcom0
-      environment:
-        - meshtty=/tmp/vcom0
-        - nodeID=631724152
-        - maxsendingattempts=5
-        - auth=true
-        - username=XXXUSERNAME
-        - password=XXXPASSWORD
-        - loglevel=WARNING
+        - ./alertmanager-meshtastic/config.toml:/app/config.toml
       restart: always
 ```
 
 
 ##  Running on docker example - Hardware Serial (default)
 
 ```
     docker run -d --name alertmanager-webhook-meshtastic-python \
 		--device=/dev/ttyACM0 \
-		-e "meshtty=/dev/ttyACM0" \
-      -e "maxsendingattempts=5" \
-    	-e "nodeID=123456789" \
-    	-e "auth=true" \
-    	-e "username=XXXUSERNAME" \
-    	-e "password=XXXPASSWORD" \
-    	-e "loglevel=WARNING" \
-    	-p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
+		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
+    -p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
 ```
 
 ##  Running on docker example - Virtual Serial
 
 If you plan to use a virtual serial port that is provided with socat (for example /tmp/vcom0), you have to use a volume mount instead of the device binding:
 
 ```
     docker run -d --name alertmanager-webhook-meshtastic-python \
 		-v /tmp/vcom0:/tmp/vcom0 \
-		-e "meshtty=/tmp/vcom0" \
-    	-e "nodeID=123456789" \
-      -e "maxsendingattempts=5" \
-    	-e "auth=true" \
-    	-e "username=XXXUSERNAME" \
-    	-e "password=XXXPASSWORD" \
-    	-e "loglevel=WARNING" \
-    	-p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
+		-v ./alertmanager-meshtastic/config.toml:/app/config.toml \
+    -p 9119:9119 apfelwurm/alertmanager-webhook-meshtastic-python:latest
 ```
 
 ## Contribution
 
-This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. I would appreciate any help.
+This is currently a minimal implementation that supports only a single node as a receiver. If you need additional features, you are welcome to open an issue, or even better, submit a pull request. You can also take a look on the opened Issues, where i have opened some for planned features and work on them if you want. I would appreciate any help.
 
 
 ## Example to test
+
+You can use the test.sh or the test single.sh or the following curl command to test alertmanager-meshtastic
 ```
-	curl -XPOST --data '{"status":"resolved","groupLabels":{"alertname":"instance_down"},"commonAnnotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"},"alerts":[{"status":"resolved","labels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"},"endsAt":"2019-07-01T16:16:19.376244942-03:00","generatorURL":"http://pmts.io:9090","startsAt":"2019-07-01T16:02:19.376245319-03:00","annotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"}}],"version":"4","receiver":"infra-alert","externalURL":"http://alm.io:9093","commonLabels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"}}' http://XXXUSERNAME:XXXPASSWORD@flaskAlert:9119/alert
+	curl -XPOST --data '{"status":"resolved","groupLabels":{"alertname":"instance_down"},"commonAnnotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"},"alerts":[{"status":"resolved","labels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"},"endsAt":"2019-07-01T16:16:19.376244942-03:00","generatorURL":"http://pmts.io:9090","startsAt":"2019-07-01T16:02:19.376245319-03:00","annotations":{"description":"i-0d7188fkl90bac100 of job ec2-sp-node_exporter has been down for more than 2 minutes.","summary":"Instance i-0d7188fkl90bac100 down"}}],"version":"4","receiver":"infra-alert","externalURL":"http://alm.io:9093","commonLabels":{"name":"olokinho01-prod","instance":"i-0d7188fkl90bac100","job":"ec2-sp-node_exporter","alertname":"instance_down","os":"linux","severity":"page"}}' http://alertmanager-meshtastic:9119/alert
 ```
```

### Comparing `alertmanagermeshtastic-2023.8.1.5/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.8.1.6/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.8.1.6/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.8.1.6/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/tests/test_load_config.py` & `alertmanagermeshtastic-2023.8.1.6/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.8.1.6/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.8.1.6/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.5/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.8.1.6/tests/test_token_cli.py`

 * *Files identical despite different names*

