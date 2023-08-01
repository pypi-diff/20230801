# Comparing `tmp/shell_whiz-0.2.5rc1.tar.gz` & `tmp/shell_whiz-0.2.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.2.5rc1.tar", max compression
+gzip compressed data, was "shell_whiz-0.2.5rc2.tar", max compression
```

## Comparing `shell_whiz-0.2.5rc1.tar` & `shell_whiz-0.2.5rc2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-08-01 18:42:49.046074 shell_whiz-0.2.5rc1/LICENSE
--rw-r--r--   0        0        0     3141 2023-08-01 18:42:49.046074 shell_whiz-0.2.5rc1/README.md
--rw-r--r--   0        0        0      539 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/pyproject.toml
--rw-r--r--   0        0        0      510 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/argparse.py
--rw-r--r--   0        0        0     6761 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/cli.py
--rw-r--r--   0        0        0     1686 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/config.py
--rw-r--r--   0        0        0       54 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/console.py
--rw-r--r--   0        0        0      207 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/constants.py
--rw-r--r--   0        0        0      152 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/exceptions.py
--rw-r--r--   0        0        0    10011 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/openai.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 shell_whiz-0.2.5rc1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-01 19:19:52.554443 shell_whiz-0.2.5rc2/LICENSE
+-rw-r--r--   0        0        0     3141 2023-08-01 19:19:52.554443 shell_whiz-0.2.5rc2/README.md
+-rw-r--r--   0        0        0      542 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/argparse.py
+-rw-r--r--   0        0        0     6761 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/cli.py
+-rw-r--r--   0        0        0     1686 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/config.py
+-rw-r--r--   0        0        0       54 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/console.py
+-rw-r--r--   0        0        0      207 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/constants.py
+-rw-r--r--   0        0        0      152 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0    10011 2023-08-01 19:19:52.558443 shell_whiz-0.2.5rc2/shell_whiz/openai.py
+-rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 shell_whiz-0.2.5rc2/PKG-INFO
```

### Comparing `shell_whiz-0.2.5rc1/LICENSE` & `shell_whiz-0.2.5rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc1/README.md` & `shell_whiz-0.2.5rc2/README.md`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc1/pyproject.toml` & `shell_whiz-0.2.5rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.2.5rc1"
+version = "0.2.5rc2"
 description = "Shell Whiz: AI assistant right in your terminal"
 license = "GPL-3.0-only"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.8 <4"
 openai = "^0.27.8"
 inquirer = "^3.1.3"
 yaspin = "^2.3.0"
 jsonschema = "^4.18.4"
 rich = "^13.4.2"
 
 [tool.poetry.scripts]
```

### Comparing `shell_whiz-0.2.5rc1/shell_whiz/cli.py` & `shell_whiz-0.2.5rc2/shell_whiz/cli.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc1/shell_whiz/config.py` & `shell_whiz-0.2.5rc2/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc1/shell_whiz/openai.py` & `shell_whiz-0.2.5rc2/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.5rc1/PKG-INFO` & `shell_whiz-0.2.5rc2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.2.5rc1
+Version: 0.2.5rc2
 Summary: Shell Whiz: AI assistant right in your terminal
 License: GPL-3.0-only
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: jsonschema (>=4.18.4,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
```

