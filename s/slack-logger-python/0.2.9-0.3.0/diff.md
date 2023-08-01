# Comparing `tmp/slack-logger-python-0.2.9.tar.gz` & `tmp/slack-logger-python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-logger-python-0.2.9.tar", last modified: Sun Jul 30 15:36:39 2023, max compression
+gzip compressed data, was "slack-logger-python-0.3.0.tar", last modified: Tue Aug  1 00:57:44 2023, max compression
```

## Comparing `slack-logger-python-0.2.9.tar` & `slack-logger-python-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.821392 slack-logger-python-0.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.github/workflows/tagging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 15:36:31.000000 slack-logger-python-0.2.9/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/slack_logger/
--rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/slack_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/slack_logger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/slack_logger_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 15:36:39.000000 slack-logger-python-0.2.9/slack_logger_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:39.825392 slack-logger-python-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-30 15:36:28.000000 slack-logger-python-0.2.9/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.057858 slack-logger-python-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.057858 slack-logger-python-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.github/workflows/tagging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.057858 slack-logger-python-0.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 00:57:34.000000 slack-logger-python-0.3.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.057858 slack-logger-python-0.3.0/slack_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/slack_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/slack_logger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/slack_logger_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 00:57:44.000000 slack-logger-python-0.3.0/slack_logger_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:44.061858 slack-logger-python-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-01 00:57:25.000000 slack-logger-python-0.3.0/tests/test_basic.py
```

### Comparing `slack-logger-python-0.2.9/.github/workflows/deploy.yml` & `slack-logger-python-0.3.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.9/.github/workflows/format.yml` & `slack-logger-python-0.3.0/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.9/.github/workflows/tagging.yml` & `slack-logger-python-0.3.0/.github/workflows/tagging.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.9/.gitignore` & `slack-logger-python-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.9/LICENSE` & `slack-logger-python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.9/PKG-INFO` & `slack-logger-python-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-logger-python
-Version: 0.2.9
+Version: 0.3.0
 Summary: Slack logger utilizing python logging interface.
 Author-email: GRBurst <GRBurst@protonmail.com>
 Project-URL: Homepage, https://github.com/GRBurst/slack-python-logging
 Project-URL: Bug Tracker, https://github.com/GRBurst/slack-python-logging/issues
 Keywords: slack,python,logging,logger,log,python-logging,Handler,Formatter,logging.Handler,logging.Formatter,monitoring,alerting,slack-api,webhook,slack-logger,messaging,health-check,notification-service,notification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -226,24 +226,24 @@
 ```python
 from slack_logger import Configuration, SlackFilter, SlackHandler
 import os
 import logging 
 
 logger = logging.getLogger("ProdFilter")
 # Allow only logs from `prod` environment
-filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyWhitelist)
+filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyAllowList)
 slack_handler.addFilter(filter)
 logger.addHandler(slack_handler)
 
 
 # When the ENV enviroment variable is set to prod, the message will be send.
 # Otherwise, the message is filtered out and not send (e.g. if ENV is `dev`)
-logger.warning(f"{log_msg} in some environment and whitelisted prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
+logger.warning(f"{log_msg} in some environment and allow listed prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
 
 # Will be filtered
-logger.warning(f"{log_msg} in dev environment and whitelisted prod", extra={"filter": {"environment": "dev"}})
+logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "dev"}})
 
 # Will be send
-logger.warning(f"{log_msg} in dev environment and whitelisted prod", extra={"filter": {"environment": "prod"}})
+logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "prod"}})
 ```
 
 The composition of configurations, filters and dynamic extra fields allow for a flexible way of specifying your message content and filter unwanted messages.
```

### Comparing `slack-logger-python-0.2.9/README.md` & `slack-logger-python-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -204,24 +204,24 @@
 ```python
 from slack_logger import Configuration, SlackFilter, SlackHandler
 import os
 import logging 
 
 logger = logging.getLogger("ProdFilter")
 # Allow only logs from `prod` environment
-filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyWhitelist)
+filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyAllowList)
 slack_handler.addFilter(filter)
 logger.addHandler(slack_handler)
 
 
 # When the ENV enviroment variable is set to prod, the message will be send.
 # Otherwise, the message is filtered out and not send (e.g. if ENV is `dev`)
-logger.warning(f"{log_msg} in some environment and whitelisted prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
+logger.warning(f"{log_msg} in some environment and allow listed prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
 
 # Will be filtered
-logger.warning(f"{log_msg} in dev environment and whitelisted prod", extra={"filter": {"environment": "dev"}})
+logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "dev"}})
 
 # Will be send
-logger.warning(f"{log_msg} in dev environment and whitelisted prod", extra={"filter": {"environment": "prod"}})
+logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "prod"}})
 ```
 
 The composition of configurations, filters and dynamic extra fields allow for a flexible way of specifying your message content and filter unwanted messages.
```

### Comparing `slack-logger-python-0.2.9/pyproject.toml` & `slack-logger-python-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.9/shell.nix` & `slack-logger-python-0.3.0/shell.nix`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.9/slack_logger/__init__.py` & `slack-logger-python-0.3.0/slack_logger/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,58 +187,58 @@
 
     def format(self, record: LogRecord) -> str:
         super().format(record)
         return self.design.format(record)
 
 
 class FilterType(Enum):
-    AnyWhitelist = "AnyWhitelist"
-    AllWhitelist = "AllWhitelist"
-    AnyBlacklist = "AnyBlacklist"
-    AllBlacklist = "AllBlacklist"
+    AnyAllowList = "AnyAllowList"
+    AllAllowList = "AllAllowList"
+    AnyDenyList = "AnyDenyList"
+    AllDenyList = "AllDenyList"
 
 
 class SlackFilter(logging.Filter):
     config: Configuration
     tpe: FilterType
 
-    def __init__(self, config: Configuration, filterType: FilterType = FilterType.AnyWhitelist):
+    def __init__(self, config: Configuration, filterType: FilterType = FilterType.AnyAllowList):
         super(SlackFilter, self).__init__()
         self.config = config
         self.tpe = filterType
 
     @classmethod
     def filter_by_fields(
-        cls, fields: Dict[str, str], filterType: FilterType = FilterType.AnyWhitelist
+        cls, fields: Dict[str, str], filterType: FilterType = FilterType.AnyAllowList
     ) -> "SlackFilter":
         return cls(Configuration(extra_fields=fields), filterType=filterType)
 
     @classmethod
-    def hide_by_fields(cls, fields: Dict[str, str], filterType: FilterType = FilterType.AnyBlacklist) -> "SlackFilter":
+    def hide_by_fields(cls, fields: Dict[str, str], filterType: FilterType = FilterType.AnyDenyList) -> "SlackFilter":
         return cls(Configuration(extra_fields=fields), filterType=filterType)
 
     def filterConfig(self, serviceConfig: Configuration, record: LogRecord) -> bool:
         res_list = []
         if self.config.service is not None:
             res_list.append(serviceConfig.service == self.config.service)
         if self.config.environment is not None:
             res_list.append(serviceConfig.environment == self.config.environment)
         if self.config.extra_fields != {}:
             for f in self.config.extra_fields.items():
                 res_list.append(f in serviceConfig.extra_fields.items())
 
         res: bool
         match self.tpe:
-            case FilterType.AnyWhitelist:
+            case FilterType.AnyAllowList:
                 res = any(res_list)
-            case FilterType.AllWhitelist:
+            case FilterType.AllAllowList:
                 res = all(res_list)
-            case FilterType.AnyBlacklist:
+            case FilterType.AnyDenyList:
                 res = not all(res_list)
-            case FilterType.AllBlacklist:
+            case FilterType.AllDenyList:
                 res = not any(res_list)
 
         log.debug(f"final result ({self.tpe}): res({res}) = {res_list}")
         return res
 
     def filter(self, record: LogRecord) -> bool:
         log_filters = getattr(record, "filter", None)
```

### Comparing `slack-logger-python-0.2.9/slack_logger_python.egg-info/PKG-INFO` & `slack-logger-python-0.3.0/slack_logger_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-logger-python
-Version: 0.2.9
+Version: 0.3.0
 Summary: Slack logger utilizing python logging interface.
 Author-email: GRBurst <GRBurst@protonmail.com>
 Project-URL: Homepage, https://github.com/GRBurst/slack-python-logging
 Project-URL: Bug Tracker, https://github.com/GRBurst/slack-python-logging/issues
 Keywords: slack,python,logging,logger,log,python-logging,Handler,Formatter,logging.Handler,logging.Formatter,monitoring,alerting,slack-api,webhook,slack-logger,messaging,health-check,notification-service,notification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -226,24 +226,24 @@
 ```python
 from slack_logger import Configuration, SlackFilter, SlackHandler
 import os
 import logging 
 
 logger = logging.getLogger("ProdFilter")
 # Allow only logs from `prod` environment
-filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyWhitelist)
+filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyAllowList)
 slack_handler.addFilter(filter)
 logger.addHandler(slack_handler)
 
 
 # When the ENV enviroment variable is set to prod, the message will be send.
 # Otherwise, the message is filtered out and not send (e.g. if ENV is `dev`)
-logger.warning(f"{log_msg} in some environment and whitelisted prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
+logger.warning(f"{log_msg} in some environment and allow listed prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
 
 # Will be filtered
-logger.warning(f"{log_msg} in dev environment and whitelisted prod", extra={"filter": {"environment": "dev"}})
+logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "dev"}})
 
 # Will be send
-logger.warning(f"{log_msg} in dev environment and whitelisted prod", extra={"filter": {"environment": "prod"}})
+logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "prod"}})
 ```
 
 The composition of configurations, filters and dynamic extra fields allow for a flexible way of specifying your message content and filter unwanted messages.
```

### Comparing `slack-logger-python-0.2.9/slack_logger_python.egg-info/SOURCES.txt` & `slack-logger-python-0.3.0/slack_logger_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.2.9/tests/test_basic.py` & `slack-logger-python-0.3.0/tests/test_basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,89 +78,89 @@
         1 / 0
     except Exception as e:
         logger.exception(log_msg)
         raise e
 
 
 def basic_text_filter(log_msg: str) -> None:  # type: ignore
-    # Whitelist
+    # AllowList
     ## We allow logs from test environment
-    slackFilter10 = SlackFilter(config=Configuration(environment="test"), filterType=FilterType.AnyWhitelist)
+    slackFilter10 = SlackFilter(config=Configuration(environment="test"), filterType=FilterType.AnyAllowList)
     slack_handler.addFilter(slackFilter10)
 
     ### Log from test environment
-    logger.warning(f"{log_msg} in test and whitelisted test", extra={"filter": {"environment": "test"}})
+    logger.warning(f"{log_msg} in test and allow listed test", extra={"filter": {"environment": "test"}})
 
     ### Log from dev environment
-    logger.warning(f"{log_msg} in dev and whitelisted test", extra={"filter": {"environment": "dev"}})
+    logger.warning(f"{log_msg} in dev and allow listed test", extra={"filter": {"environment": "dev"}})
 
     # Cleanup
     slack_handler.removeFilter(slackFilter10)
     assert len(slack_handler.filters) == 0
 
     ## We allow logs in test environment with extra_field {"cow": "moo"}
     slackFilter11 = SlackFilter(
-        config=Configuration(environment="test", extra_fields={"cow": "moo"}), filterType=FilterType.AllWhitelist
+        config=Configuration(environment="test", extra_fields={"cow": "moo"}), filterType=FilterType.AllAllowList
     )
     slack_handler.addFilter(slackFilter11)
 
     ### Log from test environment
-    logger.warning(f"{log_msg} in test, whitelisted test, no cow", extra={"filter": {"environment": "test"}})
+    logger.warning(f"{log_msg} in test, allow listed test, no cow", extra={"filter": {"environment": "test"}})
     logger.warning(
-        f"{log_msg} in test, whitelisted test, english cow",
+        f"{log_msg} in test, allow listed test, english cow",
         extra={"filter": {"environment": "test", "extra_fields": {"cow": "moo"}}},
     )
     logger.warning(
-        f"{log_msg} in dev, whitelisted test, english cow",
+        f"{log_msg} in dev, allow listed test, english cow",
         extra={"filter": {"environment": "dev", "extra_fields": {"cow": "moo"}}},
     )
     logger.warning(
-        f"{log_msg} in test, whitelisted test, german cow",
+        f"{log_msg} in test, allow listed test, german cow",
         extra={"filter": {"environment": "test", "extra_fields": {"cow": "muh"}}},
     )
 
     # Cleanup
     slack_handler.removeFilter(slackFilter11)
     assert len(slack_handler.filters) == 0
 
-    # Blacklist
-    ## We blacklist logs from "test" environment
-    slackFilter20 = SlackFilter(config=Configuration(environment="test"), filterType=FilterType.AnyBlacklist)
+    # DenyList
+    ## We deny list logs from "test" environment
+    slackFilter20 = SlackFilter(config=Configuration(environment="test"), filterType=FilterType.AnyDenyList)
     slack_handler.addFilter(slackFilter20)
 
     ## Log from test environment
-    logger.warning(f"{log_msg} in test and blacklisted test", extra={"filter": {"environment": "test"}})
+    logger.warning(f"{log_msg} in test and deny listed test", extra={"filter": {"environment": "test"}})
 
     ## Log from dev environment
-    logger.warning(f"{log_msg} in dev and blacklisted test", extra={"filter": {"environment": "dev"}})
+    logger.warning(f"{log_msg} in dev and deny listed test", extra={"filter": {"environment": "dev"}})
 
     # Cleanup
     slack_handler.removeFilter(slackFilter20)
     assert len(slack_handler.filters) == 0
 
 
 def basic_blocks_filter(log_msg: str) -> None:  # type: ignore
     service_config = Configuration(
         service="testrunner", environment="test", extra_fields={"foo": "bar", "raven": "caw"}
     )
     formatter = SlackFormatter.default(service_config)
     slack_handler.setFormatter(formatter)
-    # Whitelist
+    # AllowList
     ## We allow logs from test environment
-    slackFilter10 = SlackFilter(config=Configuration(environment="test"), filterType=FilterType.AnyWhitelist)
+    slackFilter10 = SlackFilter(config=Configuration(environment="test"), filterType=FilterType.AnyAllowList)
     slack_handler.addFilter(slackFilter10)
 
     ### Log from test environment
-    logger.warning(f"{log_msg} in test and whitelisted test")
+    logger.warning(f"{log_msg} in test and allow listed test")
 
     ### Log from dev environment
     service_config = Configuration(service="testrunner", environment="dev", extra_fields={"foo": "bar", "raven": "caw"})
     formatter = SlackFormatter.default(service_config)
     slack_handler.setFormatter(formatter)
-    logger.warning(f"{log_msg} in dev and whitelisted test")
+    logger.warning(f"{log_msg} in dev and allow listed test")
 
     # Cleanup
     slack_handler.removeFilter(slackFilter10)
     assert len(slack_handler.filters) == 0
 
 
 DEFAULT_ADDITIONAL_FIELDS: Dict[str, Dict[str, str]] = {
@@ -301,29 +301,29 @@
 
     def test_filters(self, caplog) -> None:  # type: ignore
         slack_handler.setFormatter(None)
         caplog.clear()
 
         log_msg = "warning from basic_text_filter"
         basic_text_filter(log_msg)
-        assert text_msg(f"{log_msg} in test and whitelisted test") in caplog.messages
-        assert text_msg(f"{log_msg} in dev and whitelisted test") not in caplog.messages
-        assert text_msg(f"{log_msg} in test and blacklisted test") not in caplog.messages
-        assert text_msg(f"{log_msg} in dev and blacklisted test") in caplog.messages
-
-        assert text_msg(f"{log_msg} in test, whitelisted test, no cow") not in caplog.messages
-        assert text_msg(f"{log_msg} in test, whitelisted test, english cow") in caplog.messages
-        assert text_msg(f"{log_msg} in dev, whitelisted test, english cow") not in caplog.messages
-        assert text_msg(f"{log_msg} in test, whitelisted test, german cow") not in caplog.messages
+        assert text_msg(f"{log_msg} in test and allow listed test") in caplog.messages
+        assert text_msg(f"{log_msg} in dev and allow listed test") not in caplog.messages
+        assert text_msg(f"{log_msg} in test and deny listed test") not in caplog.messages
+        assert text_msg(f"{log_msg} in dev and deny listed test") in caplog.messages
+
+        assert text_msg(f"{log_msg} in test, allow listed test, no cow") not in caplog.messages
+        assert text_msg(f"{log_msg} in test, allow listed test, english cow") in caplog.messages
+        assert text_msg(f"{log_msg} in dev, allow listed test, english cow") not in caplog.messages
+        assert text_msg(f"{log_msg} in test, allow listed test, german cow") not in caplog.messages
 
         slack_handler.setFormatter(None)
         caplog.clear()
 
         log_msg = "warning from basic_blocks_filter"
         basic_blocks_filter(log_msg)
         assert (
-            default_msg(log_msg=f"{log_msg} in test and whitelisted test", levelno=logging.WARNING) in caplog.messages
+            default_msg(log_msg=f"{log_msg} in test and allow listed test", levelno=logging.WARNING) in caplog.messages
         )
         assert (
-            default_msg(log_msg=f"{log_msg} in dev and whitelisted test", levelno=logging.WARNING)
+            default_msg(log_msg=f"{log_msg} in dev and allow listed test", levelno=logging.WARNING)
             not in caplog.messages
         )
```

