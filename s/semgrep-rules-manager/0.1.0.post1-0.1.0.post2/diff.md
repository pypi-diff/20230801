# Comparing `tmp/semgrep_rules_manager-0.1.0.post1.tar.gz` & `tmp/semgrep_rules_manager-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semgrep_rules_manager-0.1.0.post1.tar", max compression
+gzip compressed data, was "semgrep_rules_manager-0.1.0.post2.tar", max compression
```

## Comparing `semgrep_rules_manager-0.1.0.post1.tar` & `semgrep_rules_manager-0.1.0.post2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-07-27 09:28:13.660884 semgrep_rules_manager-0.1.0.post1/LICENSE
--rw-r--r--   0        0        0     1710 2023-07-28 12:26:40.315877 semgrep_rules_manager-0.1.0.post1/README.pypi.md
--rw-r--r--   0        0        0     1440 2023-07-28 12:28:53.575978 semgrep_rules_manager-0.1.0.post1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 10:09:41.096768 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/__init__.py
--rw-r--r--   0        0        0     4994 2023-07-27 15:23:18.259554 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/cli.py
--rw-r--r--   0        0        0     1440 2023-07-27 15:12:22.885391 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/core.py
--rw-r--r--   0        0        0     1426 2023-07-28 07:44:40.423516 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/data/sources.yaml
--rw-r--r--   0        0        0      284 2023-07-27 13:50:03.352821 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/exception.py
--rw-r--r--   0        0        0     4902 2023-07-28 12:12:53.103670 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/sources.py
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 semgrep_rules_manager-0.1.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-27 09:28:13.660884 semgrep_rules_manager-0.1.0.post2/LICENSE
+-rw-r--r--   0        0        0     1711 2023-08-01 08:02:36.011149 semgrep_rules_manager-0.1.0.post2/README.pypi.md
+-rw-r--r--   0        0        0     1443 2023-08-01 08:00:26.082746 semgrep_rules_manager-0.1.0.post2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 10:09:41.096768 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/__init__.py
+-rw-r--r--   0        0        0     4994 2023-07-27 15:23:18.259554 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/cli.py
+-rw-r--r--   0        0        0     1440 2023-07-27 15:12:22.885391 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/core.py
+-rw-r--r--   0        0        0     1426 2023-07-28 07:44:40.423516 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/data/sources.yaml
+-rw-r--r--   0        0        0      284 2023-07-27 13:50:03.352821 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/exception.py
+-rw-r--r--   0        0        0     4902 2023-07-28 12:12:53.103670 semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/sources.py
+-rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 semgrep_rules_manager-0.1.0.post2/PKG-INFO
```

### Comparing `semgrep_rules_manager-0.1.0.post1/LICENSE` & `semgrep_rules_manager-0.1.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post1/README.pypi.md` & `semgrep_rules_manager-0.1.0.post2/README.pypi.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-    <img src="https://raw.githubusercontent.com/returntocorp/semgrep/develop/images/semgrep-logo-light.svg" height="100" alt="Semgrep logo"/>
+    <img src="https://raw.githubusercontent.com/iosifache/semgrep-rules-manager/main/logo.png" height="256" alt="semgrep-rules-manager logo"/>
 </p>
 
 ## Description
 
 Despite the fact that there is an open source repository containing community rules, some Semgrep users prefer to keep their custom rules in repositories that they manage.
 
 The goal of **`semgrep-rules-manager`** is to collect **high-quality Semgrep rules from third-party sources**. It allows you to examine information about a source, download it, and check for and retrieve remote updates. If a downloaded source no longer meets your requirements, `semgrep-rules-manager` can handle deletion procedures.
```

### Comparing `semgrep_rules_manager-0.1.0.post1/pyproject.toml` & `semgrep_rules_manager-0.1.0.post2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semgrep_rules_manager"
-version = "0.1.0.post1"
+version = "0.1.0.post2"
 description = "Manager of third-party Semgrep rules"
 keywords = ["semgrep", "semgrep-rules", "semgrep-rules-manager", "sast"]
 authors = ["George-Andrei Iosif <andrei.iosif@canonical.com>"]
 readme = "README.pypi.md"
 license = "MIT"
 packages = [{include = "semgrep_rules_manager"}]
 repository = "https://github.com/iosifache/semgrep-rules-manager"
@@ -20,26 +20,26 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.6"
 pyyaml = "^6.0.1"
 gitpython = "^3.1.32"
 rich = "^13.4.2"
 
-[tool.poetry.scripts]
-semgrep-rules-manager = 'semgrep_rules_manager.cli:main'
-generate-readme = 'actions.generate_readme.generate_readme:main'
-
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 black = "^23.7.0"
 isort = "^5.12.0"
 
 [tool.poetry.group.actions.dependencies]
 tabulate = "^0.9.0"
 
+[tool.poetry.scripts]
+semgrep-rules-manager = 'semgrep_rules_manager.cli:main'
+generate-readmes = 'actions.generate_readmes.generate_readmes:main'
+
 [tool.black]
 line-length = 79
 preview = true
 include = '\.pyi?$'
 extend-exclude = """
 (
     ^/.venv/*
```

### Comparing `semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/cli.py` & `semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/cli.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/core.py` & `semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/core.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/data/sources.yaml` & `semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/data/sources.yaml`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/sources.py` & `semgrep_rules_manager-0.1.0.post2/semgrep_rules_manager/sources.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0.post1/PKG-INFO` & `semgrep_rules_manager-0.1.0.post2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semgrep-rules-manager
-Version: 0.1.0.post1
+Version: 0.1.0.post2
 Summary: Manager of third-party Semgrep rules
 Home-page: https://github.com/iosifache/semgrep-rules-manager
 License: MIT
 Keywords: semgrep,semgrep-rules,semgrep-rules-manager,sast
 Author: George-Andrei Iosif
 Author-email: andrei.iosif@canonical.com
 Requires-Python: >=3.10,<4.0
@@ -22,15 +22,15 @@
 Requires-Dist: gitpython (>=3.1.32,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Repository, https://github.com/iosifache/semgrep-rules-manager
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/returntocorp/semgrep/develop/images/semgrep-logo-light.svg" height="100" alt="Semgrep logo"/>
+    <img src="https://raw.githubusercontent.com/iosifache/semgrep-rules-manager/main/logo.png" height="256" alt="semgrep-rules-manager logo"/>
 </p>
 
 ## Description
 
 Despite the fact that there is an open source repository containing community rules, some Semgrep users prefer to keep their custom rules in repositories that they manage.
 
 The goal of **`semgrep-rules-manager`** is to collect **high-quality Semgrep rules from third-party sources**. It allows you to examine information about a source, download it, and check for and retrieve remote updates. If a downloaded source no longer meets your requirements, `semgrep-rules-manager` can handle deletion procedures.
```

