# Comparing `tmp/create_pipenv_project-0.1.tar.gz` & `tmp/create_pipenv_project-0.2.tar.gz`

## Comparing `create_pipenv_project-0.1.tar` & `create_pipenv_project-0.2.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 create_pipenv_project-0.1/create_pipenv_project/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 create_pipenv_project-0.1/create_pipenv_project/__main__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 create_pipenv_project-0.1/create_pipenv_project/terminal.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 create_pipenv_project-0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 create_pipenv_project-0.1/LICENSE
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 create_pipenv_project-0.1/README.md
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 create_pipenv_project-0.1/pyproject.toml
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 create_pipenv_project-0.1/PKG-INFO
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/py.typed
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/terminal.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/user_files/.gitignore
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/user_files/__init__.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/user_files/_main_runner.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/user_files/env
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/user_files/logging.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/user_files/mypy.ini
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/user_files/run.py
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/create_pipenv_project/user_files/run_tests.sh
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/LICENSE
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/README.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 create_pipenv_project-0.2/PKG-INFO
```

### Comparing `create_pipenv_project-0.1/create_pipenv_project/__init__.py` & `create_pipenv_project-0.2/create_pipenv_project/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1"
+__version__ = "0.2"
 
 import os
 import shutil
 import create_pipenv_project
 from create_pipenv_project.terminal import ANSICodes as ansi, print_error
```

### Comparing `create_pipenv_project-0.1/create_pipenv_project/terminal.py` & `create_pipenv_project-0.2/create_pipenv_project/terminal.py`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.1/.gitignore` & `create_pipenv_project-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.1/LICENSE` & `create_pipenv_project-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.1/README.md` & `create_pipenv_project-0.2/README.md`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.1/pyproject.toml` & `create_pipenv_project-0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 "Repository" = "https://github.com/nietsuu/create_pipenv_project"
 
 [project.scripts]
 create_pipenv_project = "create_pipenv_project:main"
 
 [tool.hatch.build]
 include = [
-  "create_pipenv_project/*.py",
+  "create_pipenv_project/**",
 ]
 
 [tool.hatch.version]
 path = "create_pipenv_project/__init__.py"
```

### Comparing `create_pipenv_project-0.1/PKG-INFO` & `create_pipenv_project-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create_pipenv_project
-Version: 0.1
+Version: 0.2
 Summary: A CLI tool for creating Python projects with Pipenv workflow.
 Project-URL: Repository, https://github.com/nietsuu/create_pipenv_project
 Author-email: Nie Tsuu <nietsuu@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: pipenv
 Description-Content-Type: text/markdown
```

