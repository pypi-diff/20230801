# Comparing `tmp/azure-cli-telemetry-1.0.8.tar.gz` & `tmp/azure-cli-telemetry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-cli-telemetry-1.0.8.tar", last modified: Fri Sep  2 05:40:14 2022, max compression
+gzip compressed data, was "azure-cli-telemetry-1.1.0.tar", last modified: Thu Jul 27 07:10:37 2023, max compression
```

## Comparing `azure-cli-telemetry-1.0.8.tar` & `azure-cli-telemetry-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-09-02 05:40:14.638116 azure-cli-telemetry-1.0.8/
--rw-r--r--   0 vsts      (1001) docker     (121)      586 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1109 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       90 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     1641 2022-09-02 05:40:14.638116 azure-cli-telemetry-1.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      293 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-09-02 05:40:14.638116 azure-cli-telemetry-1.0.8/azure/
--rw-r--r--   0 vsts      (1001) docker     (121)      410 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-09-02 05:40:14.638116 azure-cli-telemetry-1.0.8/azure/cli/
--rw-r--r--   0 vsts      (1001) docker     (121)      410 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-09-02 05:40:14.638116 azure-cli-telemetry-1.0.8/azure/cli/telemetry/
--rw-r--r--   0 vsts      (1001) docker     (121)     5249 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/telemetry/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-09-02 05:40:14.638116 azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/
--rw-r--r--   0 vsts      (1001) docker     (121)      345 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4461 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/records_collection.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4829 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/telemetry_client.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2087 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/telemetry_logging.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2955 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/telemetry_note.py
--rw-r--r--   0 vsts      (1001) docker     (121)      561 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/telemetry/const.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3188 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/azure/cli/telemetry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-09-02 05:40:14.638116 azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     1641 2022-09-02 05:40:14.000000 azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      698 2022-09-02 05:40:14.000000 azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-09-02 05:40:14.000000 azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-09-02 05:40:14.000000 azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-09-02 05:40:14.000000 azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-09-02 05:40:14.000000 azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-09-02 05:40:14.638116 azure-cli-telemetry-1.0.8/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1620 2022-09-02 05:40:04.000000 azure-cli-telemetry-1.0.8/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-27 07:10:37.015299 azure-cli-telemetry-1.1.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      669 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/HISTORY.rst
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1109 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/LICENSE.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       90 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1674 2023-07-27 07:10:37.015299 azure-cli-telemetry-1.1.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      293 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/README.rst
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-27 07:10:37.015299 azure-cli-telemetry-1.1.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      410 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-27 07:10:37.015299 azure-cli-telemetry-1.1.0/azure/cli/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      410 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-27 07:10:37.015299 azure-cli-telemetry-1.1.0/azure/cli/telemetry/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4918 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/telemetry/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-27 07:10:37.015299 azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      345 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3803 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/records_collection.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4829 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/telemetry_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2087 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/telemetry_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2955 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/telemetry_note.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      561 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/telemetry/const.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1813 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/azure/cli/telemetry/util.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-27 07:10:37.015299 azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1674 2023-07-27 07:10:37.000000 azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      698 2023-07-27 07:10:37.000000 azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-07-27 07:10:37.000000 azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-07-27 07:10:36.000000 azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       54 2023-07-27 07:10:37.000000 azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-07-27 07:10:37.000000 azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-07-27 07:10:37.015299 azure-cli-telemetry-1.1.0/setup.cfg
+-rwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)     1575 2023-07-27 07:10:05.000000 azure-cli-telemetry-1.1.0/setup.py
```

### Comparing `azure-cli-telemetry-1.0.8/HISTORY.rst` & `azure-cli-telemetry-1.1.0/HISTORY.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 .. :changelog:
 
 Release History
 ===============
+1.1.0
++++++
+* Drop telemetry cache strategy. Records will be uploaded immediately
+
 1.0.8
 +++++
 * Keep storing telemetry to CLI AppInsights in local cache but send telemetry to other AppInsights immediately
 
 1.0.7
 +++++
 * Support specifying `telemetry.push_interval_in_hours` to force push telemetry cache file
```

### Comparing `azure-cli-telemetry-1.0.8/LICENSE.txt` & `azure-cli-telemetry-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `azure-cli-telemetry-1.0.8/PKG-INFO` & `azure-cli-telemetry-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: azure-cli-telemetry
-Version: 1.0.8
+Version: 1.1.0
 Summary: Microsoft Azure CLI Telemetry Package
 Home-page: https://github.com/Azure/azure-cli
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE.txt
 
 Microsoft Azure CLI Telemetry Package
@@ -29,14 +28,18 @@
 
 
 
 .. :changelog:
 
 Release History
 ===============
+1.1.0
++++++
+* Drop telemetry cache strategy. Records will be uploaded immediately
+
 1.0.8
 +++++
 * Keep storing telemetry to CLI AppInsights in local cache but send telemetry to other AppInsights immediately
 
 1.0.7
 +++++
 * Support specifying `telemetry.push_interval_in_hours` to force push telemetry cache file
```

### Comparing `azure-cli-telemetry-1.0.8/azure/cli/telemetry/__init__.py` & `azure-cli-telemetry-1.1.0/azure/cli/telemetry/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import os
 import subprocess
 import portalocker
 
 from azure.cli.telemetry.util import save_payload
 
-__version__ = "1.0.8"
+__version__ = "1.1.0"
 
 DEFAULT_INSTRUMENTATION_KEY = 'c4395b75-49cc-422c-bc95-c7d51aef5d46'
 
 
 def _start(config_dir):
     from azure.cli.telemetry.components.telemetry_logging import get_logger
 
@@ -43,23 +43,22 @@
             kwargs['stderr'] = subprocess.STDOUT
 
     subprocess.Popen(**kwargs)
     logger.info('Return from creating process')
 
 
 def save(config_dir, payload):
-    from azure.cli.telemetry.util import should_upload
     from azure.cli.telemetry.components.telemetry_client import CliTelemetryClient
     from azure.cli.telemetry.components.telemetry_logging import get_logger
 
     logger = get_logger('main')
     try:
         # Split payload to cli events and extra events by instrumentation key
-        # cli events should be stored in local cache and sent together
         # extra events can be sent immediately
+        # cli events will be handled in separate process
         import json
         events = json.loads(payload)
 
         logger.info('Begin splitting cli events and extra events, total events: %s', len(events))
         cli_events = {}
         client = CliTelemetryClient()
         for key, event in events.items():
@@ -71,38 +70,33 @@
         client.flush(force=True)
         cli_payload = json.dumps(cli_events) if cli_events else None
         logger.info('Finish splitting cli events and extra events, cli events: %s', len(cli_events))
     except Exception as ex:  # pylint: disable=broad-except
         logger.info("Split cli events and extra events failure: %s", str(ex))
         cli_payload = payload
 
-    if save_payload(config_dir, cli_payload) and should_upload(config_dir):
+    if save_payload(config_dir, cli_payload):
         logger.info('Begin creating telemetry upload process.')
         _start(config_dir)
         logger.info('Finish creating telemetry upload process.')
 
 
 def main():
-    from azure.cli.telemetry.util import should_upload
     from azure.cli.telemetry.components.telemetry_note import TelemetryNote
     from azure.cli.telemetry.components.records_collection import RecordsCollection
     from azure.cli.telemetry.components.telemetry_client import CliTelemetryClient
     from azure.cli.telemetry.components.telemetry_logging import config_logging_for_upload, get_logger
 
     try:
         config_dir = sys.argv[1]
         config_logging_for_upload(config_dir)
 
         logger = get_logger('main')
         logger.info('Attempt start. Configuration directory [%s].', sys.argv[1])
 
-        if not should_upload(config_dir):
-            logger.info('Exit early. The note file indicates it is not a suitable time to upload telemetry.')
-            sys.exit(0)
-
         try:
             with TelemetryNote(config_dir) as telemetry_note:
                 telemetry_note.touch()
 
                 collection = RecordsCollection(telemetry_note.get_last_sent(), config_dir)
                 collection.snapshot_and_read()
```

### Comparing `azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/records_collection.py` & `azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/records_collection.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # --------------------------------------------------------------------------------------------
 
 import datetime
 import os
 import shutil
 import stat
 import tempfile
-from knack.config import CLIConfig
 
 
 class RecordsCollection:
     def __init__(self, last_sent, config_dir):
         from azure.cli.telemetry.components.telemetry_logging import get_logger
 
         self._last_sent = last_sent
@@ -32,19 +31,16 @@
         """ Scan the telemetry cache files and move all the rotated files to a temp directory. """
         from azure.cli.telemetry.const import TELEMETRY_CACHE_DIR
 
         folder = os.path.join(self._config_dir, TELEMETRY_CACHE_DIR)
         if not os.path.isdir(folder):
             return
 
-        # Collect all cache.x files. If it has been a long time since last sent, also collect cache file itself.
-        push_interval = datetime.timedelta(hours=self._get_push_interval_config())
-        include_cache = datetime.datetime.now() - self._last_sent > push_interval
-        candidates = [(fn, os.stat(os.path.join(folder, fn))) for fn in os.listdir(folder)
-                      if include_cache or fn != 'cache']
+        # Collect all cache/cache.x files
+        candidates = [(fn, os.stat(os.path.join(folder, fn))) for fn in os.listdir(folder)]
 
         # sort the cache files base on their last modification time.
         candidates = [(fn, file_stat) for fn, file_stat in candidates if stat.S_ISREG(file_stat.st_mode)]
         candidates.sort(key=lambda pair: pair[1].st_mtime, reverse=True)  # move the newer cache file first
 
         if not candidates:
             self._logger.info('No cache to be uploaded.')
@@ -68,20 +64,14 @@
             self._read_file(os.path.join(tmp, each))
 
         shutil.rmtree(tmp,
                       ignore_errors=True,
                       onerror=lambda _, p, tr: self._logger.error('Fail to remove file %s', p))
         self._logger.info('Remove directory %s', tmp)
 
-    def _get_push_interval_config(self):
-        config = CLIConfig(config_dir=self._config_dir)
-        threshold = config.getint('telemetry', 'push_interval_in_hours', fallback=24)
-        # the threshold for push telemetry can't be less than 1 hour, default value is 24 hours
-        return threshold if threshold >= 1 else 24
-
     def _read_file(self, path):
         """ Read content of a telemetry cache file and parse them into records. """
         try:
             with open(path, mode='r') as fh:
                 for line in fh.readlines():
                     self._add_record(line)
```

### Comparing `azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/telemetry_client.py` & `azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/telemetry_client.py`

 * *Files identical despite different names*

### Comparing `azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/telemetry_logging.py` & `azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/telemetry_logging.py`

 * *Files identical despite different names*

### Comparing `azure-cli-telemetry-1.0.8/azure/cli/telemetry/components/telemetry_note.py` & `azure-cli-telemetry-1.1.0/azure/cli/telemetry/components/telemetry_note.py`

 * *Files identical despite different names*

### Comparing `azure-cli-telemetry-1.0.8/azure/cli/telemetry/const.py` & `azure-cli-telemetry-1.1.0/azure/cli/telemetry/const.py`

 * *Files identical despite different names*

### Comparing `azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/PKG-INFO` & `azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: azure-cli-telemetry
-Version: 1.0.8
+Version: 1.1.0
 Summary: Microsoft Azure CLI Telemetry Package
 Home-page: https://github.com/Azure/azure-cli
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE.txt
 
 Microsoft Azure CLI Telemetry Package
@@ -29,14 +28,18 @@
 
 
 
 .. :changelog:
 
 Release History
 ===============
+1.1.0
++++++
+* Drop telemetry cache strategy. Records will be uploaded immediately
+
 1.0.8
 +++++
 * Keep storing telemetry to CLI AppInsights in local cache but send telemetry to other AppInsights immediately
 
 1.0.7
 +++++
 * Support specifying `telemetry.push_interval_in_hours` to force push telemetry cache file
```

### Comparing `azure-cli-telemetry-1.0.8/azure_cli_telemetry.egg-info/SOURCES.txt` & `azure-cli-telemetry-1.1.0/azure_cli_telemetry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-cli-telemetry-1.0.8/setup.py` & `azure-cli-telemetry-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 from codecs import open
 from setuptools import setup
 
-VERSION = "1.0.8"
+VERSION = "1.1.0"
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Intended Audience :: System Administrators',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'License :: OSI Approved :: MIT License',
 ]
 
 with open('README.rst', 'r', encoding='utf-8') as f:
```

