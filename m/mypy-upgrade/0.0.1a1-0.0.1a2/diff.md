# Comparing `tmp/mypy_upgrade-0.0.1a1.tar.gz` & `tmp/mypy_upgrade-0.0.1a2.tar.gz`

## Comparing `mypy_upgrade-0.0.1a1.tar` & `mypy_upgrade-0.0.1a2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/mypy_upgrade/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/mypy_upgrade/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/mypy_upgrade/__main__.py
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/mypy_upgrade/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/mypy_upgrade/py.typed
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/.gitignore
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/AUTHORS.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/LICENSE.txt
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/README.md
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/__main__.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/mypy_upgrade/py.typed
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/AUTHORS.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/LICENSE.txt
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/README.md
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a2/PKG-INFO
```

### Comparing `mypy_upgrade-0.0.1a1/mypy_upgrade/cli.py` & `mypy_upgrade-0.0.1a2/mypy_upgrade/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This defines a tool to silence mypy errors using in-line comments.
 """
 # remove when dropping Python 3.7-3.9 support
 from __future__ import annotations
 
 import argparse
 import importlib
+import importlib.abc
 import pathlib
 import re
 import sys
 import typing
 from importlib import util
 
 
@@ -149,35 +150,36 @@
     Args:
         line: a string containing the line.
         error_code: a string representing the mypy error code.
         description: a string representing a description of the error.
     Returns:
         The line with a type error suppression comment.
     """
-    # ! Use str.removesuffix when dropping Python 3.7-3.8 support
-    line = line.rstrip("\n")
+    line = line.rstrip()
     old_comment, old_code, old_description = extract_old_error(line)
 
     if old_comment is not None:
         line = line.replace(old_comment, "")
 
     if old_code and error_code:
         error_code = ",".join((old_code.strip(), error_code))
     else:
         error_code = old_code if old_code else error_code
 
     if old_description and description:
-        description = f"# {', '.join((old_description.strip(), description))}"
+        description = (
+            f" # {', '.join((old_description.strip(), description.strip()))}"
+        )
     else:
         description = (
-            f"# {old_description}" if old_description else description
+            f" # {old_description}" if old_description else f" # {description}"
         )
 
     error_code_annotation = f"[{error_code}]" if error_code else ""
-    comment = f"# type: ignore{error_code_annotation}  {description}"
+    comment = f"# type: ignore{error_code_annotation}{description}"
     return f"{line}  {comment}\n"
 
 
 def _parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="mypy-upgrade",
         description="""
```

### Comparing `mypy_upgrade-0.0.1a1/.gitignore` & `mypy_upgrade-0.0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a1/LICENSE.txt` & `mypy_upgrade-0.0.1a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a1/README.md` & `mypy_upgrade-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a1/pyproject.toml` & `mypy_upgrade-0.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a1/PKG-INFO` & `mypy_upgrade-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-upgrade
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: automatic error suppression for mypy
 Project-URL: Documentation, https://github.com/ugognw/mypy-upgrade#readme
 Project-URL: Issues, https://github.com/ugognw/mypy-upgrade/issues
 Project-URL: Source, https://github.com/ugognw/mypy-upgrade
 Author-email: Ugochukwu Nwosu <ugognw@gmail.com>
 License-Expression: MIT
 License-File: AUTHORS.md
```

