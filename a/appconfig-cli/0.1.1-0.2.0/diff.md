# Comparing `tmp/appconfig_cli-0.1.1.tar.gz` & `tmp/appconfig_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appconfig_cli-0.1.1.tar", max compression
+gzip compressed data, was "appconfig_cli-0.2.0.tar", max compression
```

## Comparing `appconfig_cli-0.1.1.tar` & `appconfig_cli-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      139 2023-07-28 22:06:16.720517 appconfig_cli-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1061 2023-07-05 14:37:28.705062 appconfig_cli-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     1481 2023-07-28 22:06:12.256504 appconfig_cli-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-07-28 16:04:03.210700 appconfig_cli-0.1.1/appconf/__init__.py
--rw-r--r--   0        0        0     3397 2023-07-28 16:06:47.448450 appconfig_cli-0.1.1/appconf/api.py
--rw-r--r--   0        0        0       62 2023-07-28 15:56:01.799312 appconfig_cli-0.1.1/appconf/exceptions.py
--rw-r--r--   0        0        0     3230 2023-07-28 16:07:54.779836 appconfig_cli-0.1.1/appconf/main.py
--rw-r--r--   0        0        0      726 2023-07-28 16:06:47.438566 appconfig_cli-0.1.1/appconf/models.py
--rw-r--r--   0        0        0     1159 2023-07-28 22:09:00.784275 appconfig_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 appconfig_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      139 2023-07-28 22:06:16.720517 appconfig_cli-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1061 2023-07-05 14:37:28.705062 appconfig_cli-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1481 2023-07-28 22:06:12.256504 appconfig_cli-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-01 10:02:00.655933 appconfig_cli-0.2.0/appconf/__init__.py
+-rw-r--r--   0        0        0     4699 2023-07-31 19:21:06.065367 appconfig_cli-0.2.0/appconf/api.py
+-rw-r--r--   0        0        0       62 2023-07-28 15:56:01.799312 appconfig_cli-0.2.0/appconf/exceptions.py
+-rw-r--r--   0        0        0     5246 2023-08-01 10:17:42.735706 appconfig_cli-0.2.0/appconf/main.py
+-rw-r--r--   0        0        0     1277 2023-07-31 19:21:06.051442 appconfig_cli-0.2.0/appconf/models.py
+-rw-r--r--   0        0        0     1176 2023-08-01 10:05:16.536834 appconfig_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 appconfig_cli-0.2.0/PKG-INFO
```

### Comparing `appconfig_cli-0.1.1/LICENSE.md` & `appconfig_cli-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `appconfig_cli-0.1.1/README.md` & `appconfig_cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `appconfig_cli-0.1.1/pyproject.toml` & `appconfig_cli-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "appconfig-cli"
-version = "0.1.1"
+version = "0.2.0"
 description = "Unofficial CLI tool for working with AWS AppConfig"
 packages = [{include = "appconf"}]
 authors = ["Nick Snell <n@nicksnell.com>"]
 license = "MIT"
 readme = ["README.md", "CHANGELOG.md"]
 repository = "https://github.com/nicksnell/appconfig-cli"
 keywords = ["appconfig", "aws", "cli", "aws-appconfig", "appconfig-cli", "cli-tool"]
@@ -28,14 +28,15 @@
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 ruff = "^0.0.277"
 black = "^23.3.0"
 pre-commit = "^3.3.3"
+invoke = "2.2.0"
 
 
 [tool.poetry.scripts]
 appconf = "appconf.main:cli"
 
 
 [build-system]
```

### Comparing `appconfig_cli-0.1.1/PKG-INFO` & `appconfig_cli-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appconfig-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: Unofficial CLI tool for working with AWS AppConfig
 Home-page: https://github.com/nicksnell/appconfig-cli
 License: MIT
 Keywords: appconfig,aws,cli,aws-appconfig,appconfig-cli,cli-tool
 Author: Nick Snell
 Author-email: n@nicksnell.com
 Requires-Python: >=3.9,<4.0
```

