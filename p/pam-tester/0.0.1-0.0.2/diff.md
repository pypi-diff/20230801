# Comparing `tmp/pam_tester-0.0.1.tar.gz` & `tmp/pam_tester-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pam_tester-0.0.1.tar", max compression
+gzip compressed data, was "pam_tester-0.0.2.tar", max compression
```

## Comparing `pam_tester-0.0.1.tar` & `pam_tester-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2479 2023-07-31 17:55:18.170495 pam_tester-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-31 17:55:18.170495 pam_tester-0.0.1/pam_tester/__init__.py
--rw-r--r--   0        0        0     1221 2023-07-31 17:55:18.170495 pam_tester-0.0.1/pam_tester/pam_tester.py
--rw-r--r--   0        0        0      854 2023-07-31 17:55:18.170495 pam_tester-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3434 1970-01-01 00:00:00.000000 pam_tester-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-08-01 16:04:09.646705 pam_tester-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 16:04:09.646705 pam_tester-0.0.2/pam_tester/__init__.py
+-rw-r--r--   0        0        0     1221 2023-08-01 16:04:09.646705 pam_tester-0.0.2/pam_tester/pam_tester.py
+-rw-r--r--   0        0        0      854 2023-08-01 16:04:09.646705 pam_tester-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 pam_tester-0.0.2/PKG-INFO
```

### Comparing `pam_tester-0.0.1/README.md` & `pam_tester-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pam_tester-0.0.1/pam_tester/pam_tester.py` & `pam_tester-0.0.2/pam_tester/pam_tester.py`

 * *Files identical despite different names*

### Comparing `pam_tester-0.0.1/pyproject.toml` & `pam_tester-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pam-tester"
-version = "0.0.1"
+version = "0.0.2"
 description = "Tool for testing PAM configurations"
 readme = "README.md"
 authors = ["Martin Schurz <Martin.Schurz@telekom.de>"]
 license = "GPL-3.0-only"
 homepage = "https://github.com/dev-sec/pam-tester"
 repository = "https://github.com/dev-sec/pam-tester"
 documentation = "https://github.com/dev-sec/pam-tester"
@@ -12,23 +12,23 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/dev-sec/pam-tester/blob/master/CHANGELOG.md"
 
 [tool.poetry.scripts]
 pam-tester = "pam_tester.pam_tester:pam_auth"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-click = "^8.1.6"
+python = "^3.6"
+click = "^8.0.4"
 pam = "^0.2.0"
 six = "^1.16.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.6.4"
-ruff = "^0.0.280"
+ruff = "^0.0.282"
 isort = "^5.12.0"
 black = "^23.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pam_tester-0.0.1/PKG-INFO` & `pam_tester-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pam-tester
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool for testing PAM configurations
 Home-page: https://github.com/dev-sec/pam-tester
 License: GPL-3.0-only
 Author: Martin Schurz
 Author-email: Martin.Schurz@telekom.de
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.6,<9.0.0)
+Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: pam (>=0.2.0,<0.3.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Project-URL: Changelog, https://github.com/dev-sec/pam-tester/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/dev-sec/pam-tester
 Project-URL: Repository, https://github.com/dev-sec/pam-tester
 Description-Content-Type: text/markdown
```

