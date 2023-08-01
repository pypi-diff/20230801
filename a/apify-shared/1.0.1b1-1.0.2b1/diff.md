# Comparing `tmp/apify_shared-1.0.1b1.tar.gz` & `tmp/apify_shared-1.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_shared-1.0.1b1.tar", last modified: Tue Aug  1 08:29:58 2023, max compression
+gzip compressed data, was "apify_shared-1.0.2b1.tar", last modified: Tue Aug  1 21:55:24 2023, max compression
```

## Comparing `apify_shared-1.0.1b1.tar` & `apify_shared-1.0.2b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:58.832959 apify_shared-1.0.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 08:29:58.828958 apify_shared-1.0.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 08:29:55.000000 apify_shared-1.0.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:29:58.832959 apify_shared-1.0.1b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:58.828958 apify_shared-1.0.1b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:58.828958 apify_shared-1.0.1b1/src/apify_shared/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:58.828958 apify_shared-1.0.1b1/src/apify_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:24.263535 apify_shared-1.0.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 21:55:24.263535 apify_shared-1.0.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 21:55:19.000000 apify_shared-1.0.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:55:24.263535 apify_shared-1.0.2b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:24.259535 apify_shared-1.0.2b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:24.259535 apify_shared-1.0.2b1/src/apify_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-01 21:54:52.000000 apify_shared-1.0.2b1/src/apify_shared/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:55:24.263535 apify_shared-1.0.2b1/src/apify_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 21:55:24.000000 apify_shared-1.0.2b1/src/apify_shared.egg-info/top_level.txt
```

### Comparing `apify_shared-1.0.1b1/LICENSE` & `apify_shared-1.0.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.1b1/PKG-INFO` & `apify_shared-1.0.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_shared
-Version: 1.0.1b1
+Version: 1.0.2b1
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.1b1/README.md` & `apify_shared-1.0.2b1/README.md`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.1b1/pyproject.toml` & `apify_shared-1.0.2b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dependencies = []
 description = "Tools and constants shared across Apify projects."
 keywords = ["apify", "api", "shared", "scraping", "automation"]
 license = {text = "Apache Software License"}
 name = "apify_shared"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.0.1b1"
+version = "1.0.2b1"
 
 [project.optional-dependencies]
 dev = [
   "autopep8 ~= 2.0.2",
   "build ~= 0.10.0",
   "flake8 ~= 6.0.0",
   "flake8-bugbear ~= 23.5.9",
@@ -31,14 +31,15 @@
   "flake8-datetimez ~= 20.10.0",
   "flake8-docstrings ~= 1.7.0",
   "flake8-encodings ~= 0.5.0",
   "flake8-isort ~= 6.0.0",
   "flake8-noqa ~= 1.3.1",
   "flake8-pytest-style ~= 1.7.2",
   "flake8-quotes ~= 3.3.2",
+  "flake8-simplify ~= 0.20.0",
   "flake8-unused-arguments ~= 0.0.13",
   "isort ~= 5.12.0",
   "mypy ~= 1.4.0",
   "pep8-naming ~= 0.13.3",
   "pre-commit ~= 3.3.2",
   "pytest ~= 7.3.1",
   "pytest-asyncio ~= 0.21.0",
```

### Comparing `apify_shared-1.0.1b1/src/apify_shared/consts.py` & `apify_shared-1.0.2b1/src/apify_shared/consts.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,117 +50,158 @@
     MIGRATING = 'migrating'
     #: Sent when the actor should persist its state (every minute or when migrating)
     PERSIST_STATE = 'persistState'
     #: Sent when the actor is aborting
     ABORTING = 'aborting'
 
 
+class ActorEnvVars(str, Enum):
+    """Possible Apify-specific environment variables prefixed with "ACTOR_"."""
+
+    # TODO: document these
+
+    #: BUILD_ID
+    BUILD_ID = 'ACTOR_BUILD_ID'
+    #: BUILD_NUMBER
+    BUILD_NUMBER = 'ACTOR_BUILD_NUMBER'
+    #: DEFAULT_DATASET_ID
+    DEFAULT_DATASET_ID = 'ACTOR_DEFAULT_DATASET_ID'
+    #: DEFAULT_KEY_VALUE_STORE_ID
+    DEFAULT_KEY_VALUE_STORE_ID = 'ACTOR_DEFAULT_KEY_VALUE_STORE_ID'
+    #: DEFAULT_REQUEST_QUEUE_ID
+    DEFAULT_REQUEST_QUEUE_ID = 'ACTOR_DEFAULT_REQUEST_QUEUE_ID'
+    #: EVENTS_WEBSOCKET_URL
+    EVENTS_WEBSOCKET_URL = 'ACTOR_EVENTS_WEBSOCKET_URL'
+    #: ID
+    ID = 'ACTOR_ID'
+    #: INPUT_KEY
+    INPUT_KEY = 'ACTOR_INPUT_KEY'
+    #: MAX_PAID_DATASET_ITEMS
+    MAX_PAID_DATASET_ITEMS = 'ACTOR_MAX_PAID_DATASET_ITEMS'
+    #: MEMORY_MBYTES
+    MEMORY_MBYTES = 'ACTOR_MEMORY_MBYTES'
+    #: RUN_ID
+    RUN_ID = 'ACTOR_RUN_ID'
+    #: STARTED_AT
+    STARTED_AT = 'ACTOR_STARTED_AT'
+    #: TASK_ID
+    TASK_ID = 'ACTOR_TASK_ID'
+    #: TIMEOUT_AT
+    TIMEOUT_AT = 'ACTOR_TIMEOUT_AT'
+    #: WEB_SERVER_PORT
+    WEB_SERVER_PORT = 'ACTOR_WEB_SERVER_PORT'
+    #: WEB_SERVER_URL
+    WEB_SERVER_URL = 'ACTOR_WEB_SERVER_URL'
+
+
 class ApifyEnvVars(str, Enum):
-    """Possible Apify-specific environment variables."""
+    """Possible Apify-specific environment variables prefixed with "APIFY_"."""
 
     # TODO: document these
 
-    #: ACT_ID
-    ACT_ID = 'APIFY_ACT_ID'
-    #: ACT_RUN_ID
-    ACT_RUN_ID = 'APIFY_ACT_RUN_ID'
-    #: ACTOR_BUILD_ID
-    ACTOR_BUILD_ID = 'APIFY_ACTOR_BUILD_ID'
-    #: ACTOR_BUILD_NUMBER
-    ACTOR_BUILD_NUMBER = 'APIFY_ACTOR_BUILD_NUMBER'
-    #: ACTOR_EVENTS_WS_URL
-    ACTOR_EVENTS_WS_URL = 'APIFY_ACTOR_EVENTS_WS_URL'
-    #: ACTOR_ID
-    ACTOR_ID = 'APIFY_ACTOR_ID'
-    #: ACTOR_RUN_ID
-    ACTOR_RUN_ID = 'APIFY_ACTOR_RUN_ID'
-    #: ACTOR_TASK_ID
-    ACTOR_TASK_ID = 'APIFY_ACTOR_TASK_ID'
     #: API_BASE_URL
     API_BASE_URL = 'APIFY_API_BASE_URL'
     #: API_PUBLIC_BASE_URL
     API_PUBLIC_BASE_URL = 'APIFY_API_PUBLIC_BASE_URL'
     #: CHROME_EXECUTABLE_PATH
     CHROME_EXECUTABLE_PATH = 'APIFY_CHROME_EXECUTABLE_PATH'
-    #: CONTAINER_PORT
-    CONTAINER_PORT = 'APIFY_CONTAINER_PORT'
-    #: CONTAINER_URL
-    CONTAINER_URL = 'APIFY_CONTAINER_URL'
     #: DEDICATED_CPUS
     DEDICATED_CPUS = 'APIFY_DEDICATED_CPUS'
     #: DEFAULT_BROWSER_PATH
     DEFAULT_BROWSER_PATH = 'APIFY_DEFAULT_BROWSER_PATH'
-    #: DEFAULT_DATASET_ID
-    DEFAULT_DATASET_ID = 'APIFY_DEFAULT_DATASET_ID'
-    #: DEFAULT_KEY_VALUE_STORE_ID
-    DEFAULT_KEY_VALUE_STORE_ID = 'APIFY_DEFAULT_KEY_VALUE_STORE_ID'
-    #: DEFAULT_REQUEST_QUEUE_ID
-    DEFAULT_REQUEST_QUEUE_ID = 'APIFY_DEFAULT_REQUEST_QUEUE_ID'
     #: DISABLE_BROWSER_SANDBOX
     DISABLE_BROWSER_SANDBOX = 'APIFY_DISABLE_BROWSER_SANDBOX'
     #: DISABLE_OUTDATED_WARNING
     DISABLE_OUTDATED_WARNING = 'APIFY_DISABLE_OUTDATED_WARNING'
     #: FACT
     FACT = 'APIFY_FACT'
     #: HEADLESS
     HEADLESS = 'APIFY_HEADLESS'
-    #: INPUT_KEY
-    INPUT_KEY = 'APIFY_INPUT_KEY'
     #: INPUT_SECRETS_PRIVATE_KEY_FILE
     INPUT_SECRETS_PRIVATE_KEY_FILE = 'APIFY_INPUT_SECRETS_PRIVATE_KEY_FILE'
     #: INPUT_SECRETS_PRIVATE_KEY_PASSPHRASE
     INPUT_SECRETS_PRIVATE_KEY_PASSPHRASE = 'APIFY_INPUT_SECRETS_PRIVATE_KEY_PASSPHRASE'
     #: IS_AT_HOME
     IS_AT_HOME = 'APIFY_IS_AT_HOME'
     #: LOCAL_STORAGE_DIR
     LOCAL_STORAGE_DIR = 'APIFY_LOCAL_STORAGE_DIR'
     #: LOG_FORMAT
     LOG_FORMAT = 'APIFY_LOG_FORMAT'
     #: LOG_LEVEL
     LOG_LEVEL = 'APIFY_LOG_LEVEL'
     #: MAX_USED_CPU_RATIO
     MAX_USED_CPU_RATIO = 'APIFY_MAX_USED_CPU_RATIO'
-    #: MEMORY_MBYTES
-    MEMORY_MBYTES = 'APIFY_MEMORY_MBYTES'
     #: META_ORIGIN
     META_ORIGIN = 'APIFY_META_ORIGIN'
+    #: METAMORPH_AFTER_SLEEP_MILLIS
+    METAMORPH_AFTER_SLEEP_MILLIS = 'APIFY_METAMORPH_AFTER_SLEEP_MILLIS'
+    #: PERSIST_STATE_INTERVAL_MILLIS
+    PERSIST_STATE_INTERVAL_MILLIS = 'APIFY_PERSIST_STATE_INTERVAL_MILLIS'
     #: PERSIST_STORAGE
     PERSIST_STORAGE = 'APIFY_PERSIST_STORAGE'
     #: PROXY_HOSTNAME
     PROXY_HOSTNAME = 'APIFY_PROXY_HOSTNAME'
     #: PROXY_PASSWORD
     PROXY_PASSWORD = 'APIFY_PROXY_PASSWORD'
     #: PROXY_PORT
     PROXY_PORT = 'APIFY_PROXY_PORT'
     #: PROXY_STATUS_URL
     PROXY_STATUS_URL = 'APIFY_PROXY_STATUS_URL'
+    #: PURGE_ON_START
+    PURGE_ON_START = 'APIFY_PURGE_ON_START'
     #: SDK_LATEST_VERSION
     SDK_LATEST_VERSION = 'APIFY_SDK_LATEST_VERSION'
-    #: STARTED_AT
-    STARTED_AT = 'APIFY_STARTED_AT'
-    #: TIMEOUT_AT
-    TIMEOUT_AT = 'APIFY_TIMEOUT_AT'
+    #: SYSTEM_INFO_INTERVAL_MILLIS
+    SYSTEM_INFO_INTERVAL_MILLIS = 'APIFY_SYSTEM_INFO_INTERVAL_MILLIS'
     #: TOKEN
     TOKEN = 'APIFY_TOKEN'
     #: USER_ID
     USER_ID = 'APIFY_USER_ID'
     #: WORKFLOW_KEY
     WORKFLOW_KEY = 'APIFY_WORKFLOW_KEY'
     #: XVFB
     XVFB = 'APIFY_XVFB'
 
-    # Extra ones not in @apify/consts:
-    #: METAMORPH_AFTER_SLEEP_MILLIS
-    METAMORPH_AFTER_SLEEP_MILLIS = 'APIFY_METAMORPH_AFTER_SLEEP_MILLIS'
-    #: PERSIST_STATE_INTERVAL_MILLIS
-    PERSIST_STATE_INTERVAL_MILLIS = 'APIFY_PERSIST_STATE_INTERVAL_MILLIS'
-    #: PURGE_ON_START
-    PURGE_ON_START = 'APIFY_PURGE_ON_START'
-    #: SYSTEM_INFO_INTERVAL_MILLIS
-    SYSTEM_INFO_INTERVAL_MILLIS = 'APIFY_SYSTEM_INFO_INTERVAL_MILLIS'
+    # Replaced by ActorEnvVars, kept for backward compatibility:
+    #: ACTOR_BUILD_ID
+    ACTOR_BUILD_ID = 'APIFY_ACTOR_BUILD_ID'
+    #: ACTOR_BUILD_NUMBER
+    ACTOR_BUILD_NUMBER = 'APIFY_ACTOR_BUILD_NUMBER'
+    #: ACTOR_EVENTS_WS_URL
+    ACTOR_EVENTS_WS_URL = 'APIFY_ACTOR_EVENTS_WS_URL'
+    #: ACTOR_ID
+    ACTOR_ID = 'APIFY_ACTOR_ID'
+    #: ACTOR_RUN_ID
+    ACTOR_RUN_ID = 'APIFY_ACTOR_RUN_ID'
+    #: ACTOR_TASK_ID
+    ACTOR_TASK_ID = 'APIFY_ACTOR_TASK_ID'
+    #: CONTAINER_PORT
+    CONTAINER_PORT = 'APIFY_CONTAINER_PORT'
+    #: CONTAINER_URL
+    CONTAINER_URL = 'APIFY_CONTAINER_URL'
+    #: DEFAULT_DATASET_ID
+    DEFAULT_DATASET_ID = 'APIFY_DEFAULT_DATASET_ID'
+    #: DEFAULT_KEY_VALUE_STORE_ID
+    DEFAULT_KEY_VALUE_STORE_ID = 'APIFY_DEFAULT_KEY_VALUE_STORE_ID'
+    #: DEFAULT_REQUEST_QUEUE_ID
+    DEFAULT_REQUEST_QUEUE_ID = 'APIFY_DEFAULT_REQUEST_QUEUE_ID'
+    #: INPUT_KEY
+    INPUT_KEY = 'APIFY_INPUT_KEY'
+    #: MEMORY_MBYTES
+    MEMORY_MBYTES = 'APIFY_MEMORY_MBYTES'
+    #: STARTED_AT
+    STARTED_AT = 'APIFY_STARTED_AT'
+    #: TIMEOUT_AT
+    TIMEOUT_AT = 'APIFY_TIMEOUT_AT'
+
+    # Deprecated, kept for backward compatibility:
+    #: ACT_ID
+    ACT_ID = 'APIFY_ACT_ID'
+    #: ACT_RUN_ID
+    ACT_RUN_ID = 'APIFY_ACT_RUN_ID'
 
 
 class ActorExitCodes(int, Enum):
     """Usual actor exit codes."""
 
     #: The actor finished successfully
     SUCCESS = 0
@@ -213,14 +254,19 @@
     #: Job started by the webhook
     WEBHOOK = 'WEBHOOK'
     #: Job started by another actor run
     ACTOR = 'ACTOR'
 
 
 INTEGER_ENV_VARS_TYPE = Literal[
+    # Actor env vars
+    ActorEnvVars.MAX_PAID_DATASET_ITEMS,
+    ActorEnvVars.MEMORY_MBYTES,
+    ActorEnvVars.WEB_SERVER_PORT,
+    # Apify env vars
     ApifyEnvVars.CONTAINER_PORT,
     ApifyEnvVars.DEDICATED_CPUS,
     ApifyEnvVars.LOG_LEVEL,
     ApifyEnvVars.MEMORY_MBYTES,
     ApifyEnvVars.METAMORPH_AFTER_SLEEP_MILLIS,
     ApifyEnvVars.PERSIST_STATE_INTERVAL_MILLIS,
     ApifyEnvVars.PROXY_PORT,
@@ -244,21 +290,38 @@
     ApifyEnvVars.PURGE_ON_START,
     ApifyEnvVars.XVFB,
 ]
 
 BOOL_ENV_VARS: List[BOOL_ENV_VARS_TYPE] = list(get_args(BOOL_ENV_VARS_TYPE))
 
 DATETIME_ENV_VARS_TYPE = Literal[
+    # Actor env vars
+    ActorEnvVars.STARTED_AT,
+    ActorEnvVars.TIMEOUT_AT,
+    # Apify env vars
     ApifyEnvVars.STARTED_AT,
     ApifyEnvVars.TIMEOUT_AT,
 ]
 
 DATETIME_ENV_VARS: List[DATETIME_ENV_VARS_TYPE] = list(get_args(DATETIME_ENV_VARS_TYPE))
 
 STRING_ENV_VARS_TYPE = Literal[
+    # Actor env vars
+    ActorEnvVars.BUILD_ID,
+    ActorEnvVars.BUILD_NUMBER,
+    ActorEnvVars.DEFAULT_DATASET_ID,
+    ActorEnvVars.DEFAULT_KEY_VALUE_STORE_ID,
+    ActorEnvVars.DEFAULT_REQUEST_QUEUE_ID,
+    ActorEnvVars.EVENTS_WEBSOCKET_URL,
+    ActorEnvVars.ID,
+    ActorEnvVars.INPUT_KEY,
+    ActorEnvVars.RUN_ID,
+    ActorEnvVars.TASK_ID,
+    ActorEnvVars.WEB_SERVER_URL,
+    # Apify env vars
     ApifyEnvVars.ACT_ID,
     ApifyEnvVars.ACT_RUN_ID,
     ApifyEnvVars.ACTOR_BUILD_ID,
     ApifyEnvVars.ACTOR_BUILD_NUMBER,
     ApifyEnvVars.ACTOR_EVENTS_WS_URL,
     ApifyEnvVars.ACTOR_ID,
     ApifyEnvVars.ACTOR_RUN_ID,
```

### Comparing `apify_shared-1.0.1b1/src/apify_shared/models.py` & `apify_shared-1.0.2b1/src/apify_shared/models.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.1b1/src/apify_shared/utils.py` & `apify_shared-1.0.2b1/src/apify_shared/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import io
 import json
 import re
 from datetime import datetime, timezone
 from enum import Enum
 from typing import Any, Dict, List, Optional, TypeVar, cast
 
@@ -96,18 +97,16 @@
     if isinstance(data, list):
         return [parse_date_fields(item, max_depth - 1) for item in data]
 
     if isinstance(data, dict):
         def parse(key: str, value: object) -> object:
             parsed_value = value
             if key.endswith(PARSE_DATE_FIELDS_KEY_SUFFIX) and isinstance(value, str):
-                try:
+                with contextlib.suppress(ValueError):
                     parsed_value = datetime.strptime(value, '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc)
-                except ValueError:
-                    pass
             elif isinstance(value, dict):
                 parsed_value = parse_date_fields(value, max_depth - 1)
             elif isinstance(value, list):
                 parsed_value = parse_date_fields(value, max_depth)  # type: ignore # mypy doesn't work with decorators and recursive calls well
             return parsed_value
 
         return {key: parse(key, value) for (key, value) in data.items()}
```

### Comparing `apify_shared-1.0.1b1/src/apify_shared.egg-info/PKG-INFO` & `apify_shared-1.0.2b1/src/apify_shared.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-shared
-Version: 1.0.1b1
+Version: 1.0.2b1
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.1b1/src/apify_shared.egg-info/requires.txt` & `apify_shared-1.0.2b1/src/apify_shared.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 flake8-datetimez~=20.10.0
 flake8-docstrings~=1.7.0
 flake8-encodings~=0.5.0
 flake8-isort~=6.0.0
 flake8-noqa~=1.3.1
 flake8-pytest-style~=1.7.2
 flake8-quotes~=3.3.2
+flake8-simplify~=0.20.0
 flake8-unused-arguments~=0.0.13
 isort~=5.12.0
 mypy~=1.4.0
 pep8-naming~=0.13.3
 pre-commit~=3.3.2
 pytest~=7.3.1
 pytest-asyncio~=0.21.0
```

