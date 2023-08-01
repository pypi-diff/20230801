# Comparing `tmp/jsonator-0.1.5.tar.gz` & `tmp/jsonator-0.1.6.tar.gz`

## Comparing `jsonator-0.1.5.tar` & `jsonator-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 jsonator-0.1.5/jsonator/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jsonator-0.1.5/jsonator/__main__.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 jsonator-0.1.5/jsonator/jsonator.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jsonator-0.1.5/jsonator/output.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jsonator-0.1.5/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 jsonator-0.1.5/LICENSE
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 jsonator-0.1.5/README.rst
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jsonator-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jsonator-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/__main__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/enum.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/jsonator.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/output.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 jsonator-0.1.6/jsonator/report.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jsonator-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 jsonator-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 jsonator-0.1.6/README.md
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jsonator-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 jsonator-0.1.6/PKG-INFO
```

### Comparing `jsonator-0.1.5/jsonator/__init__.py` & `jsonator-0.1.6/jsonator/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Main function"""
 import argparse
 import sys
 from pathlib import Path
 
-from jsonator.jsonator import ReturnCode, format_json_file
+from jsonator.enum import ReturnCode
+from jsonator.jsonator import format_json_file
+from jsonator.report import Report
 
 
 def main() -> int:
     """Main function"""
     arg_parser = argparse.ArgumentParser(
         prog="jsonator", formatter_class=argparse.RawTextHelpFormatter
     )
@@ -43,27 +45,20 @@
     if not args.path.exists():
         return ReturnCode.FILE_NOT_FOUND.value
 
     if args.sort_keys and sys.version_info < (3, 5):
         print("The `--sort-keys` option is only available on Python 3.5 and above", file=sys.stderr)
         return ReturnCode.INTERNAL_ERROR.value
 
+    report = Report(args.check, args.diff)
+
     if args.path.is_dir():
-        all_files_identical = True
         pattern = "**/*.json" if args.recursive else "*.json"
 
         for json_file in args.path.glob(pattern):
-            result = format_json_file(json_file, args.check, args.diff, args.color, args.sort_keys)
-
-            if result == ReturnCode.INTERNAL_ERROR:
-                return ReturnCode.INTERNAL_ERROR.value
-
-            if result == ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED and args.check:
-                all_files_identical = False
+            format_json_file(json_file, report, args.check, args.diff, args.color, args.sort_keys)
 
-        return (
-            ReturnCode.NOTHING_WOULD_CHANGE.value
-            if all_files_identical
-            else ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED.value
-        )
+    else:
+        format_json_file(args.path, report, args.check, args.diff, args.color, args.sort_keys)
 
-    return format_json_file(args.path, args.check, args.diff, args.color, args.sort_keys).value
+    print(report)
+    return report.status
```

### Comparing `jsonator-0.1.5/jsonator/jsonator.py` & `jsonator-0.1.6/jsonator/jsonator.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,33 +2,24 @@
 Format JSON using json tool
 """
 import filecmp
 import os
 import random
 import string
 import sys
-from enum import Enum
 from pathlib import Path
 from tempfile import gettempdir
 
 from jsonator import output
+from jsonator.report import Report
 
 INTERPRETER = Path(sys.executable).stem
 FILES_ENCODING = "utf-8"
 
 
-class ReturnCode(Enum):
-    """Set of possible return codes"""
-
-    NOTHING_WOULD_CHANGE = 0
-    SOME_FILES_WOULD_BE_REFORMATTED = 1
-    FILE_NOT_FOUND = 122
-    INTERNAL_ERROR = 123
-
-
 def random_str() -> str:
     """Generating a random alphanumeric string of 8 characters long"""
     return "".join(random.choices(string.ascii_letters + string.digits, k=8))
 
 
 def make_temp_file() -> Path:
     """Generate temp file path"""
@@ -37,58 +28,51 @@
 
     while temp_file.exists():
         temp_file = temp_dir / random_str()
 
     return temp_file
 
 
-def format_json_file(
-    json_file: Path, check: bool, diff: bool, color: bool, sort_keys: bool
-) -> ReturnCode:
+def format_json_file(  # pylint: disable=too-many-arguments
+    json_file: Path, report: Report, check: bool, diff: bool, color: bool, sort_keys: bool
+) -> None:
     """
     This function formats the file in JSON format.
     It uses the json.tool module, built into Python, to create a readable JSON format.
     """
-    if check or diff:
-        print(f"Comparing {json_file} - ", end="")
-    else:
-        print(f"Formatting {json_file}")
-
     tmp_file = make_temp_file()
 
-    cmd = [INTERPRETER, "-m", "json.tool", json_file, tmp_file]
+    cmd = [INTERPRETER, "-m", "json.tool", f'"{json_file}"', tmp_file]
     if sort_keys:
         cmd.append("--sort-keys")
 
     os.system(" ".join([str(command) for command in cmd]))
 
-    if check or diff:
+    try:
         is_identical = filecmp.cmp(json_file, tmp_file, shallow=False)
+    except FileNotFoundError:
+        report.failed(json_file, "Internal error")
+        return
 
-        if is_identical:
-            print("Ok")
-            os.unlink(tmp_file)
-            return ReturnCode.NOTHING_WOULD_CHANGE
+    report.done(json_file, not is_identical)
 
-        print("Need to format")
+    if diff:
         diff_contents = output.diff(
             json_file.read_text(encoding=FILES_ENCODING),
             tmp_file.read_text(encoding=FILES_ENCODING),
             json_file.name,
-            tmp_file.name,
+            "formatted file",
         )
 
         if color:
             diff_contents = output.color_diff(diff_contents)
 
         print(diff_contents)
 
-        os.unlink(tmp_file)
-        return ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED
-
     if tmp_file.exists():
-        os.unlink(json_file)
-        os.rename(tmp_file, json_file)
+        if check or diff:
+            os.unlink(tmp_file)
+        else:
+            os.unlink(json_file)
+            os.rename(tmp_file, json_file)
     else:
-        return ReturnCode.INTERNAL_ERROR
-
-    return ReturnCode.NOTHING_WOULD_CHANGE
+        report.failed(json_file, "Internal error")
```

### Comparing `jsonator-0.1.5/jsonator/output.py` & `jsonator-0.1.6/jsonator/output.py`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.5/LICENSE` & `jsonator-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.5/README.rst` & `jsonator-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 JSONator
 ========
 
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Downloads](https://static.pepy.tech/badge/jsonator)](https://pepy.tech/project/jsonator)
 
 Description
 -----------
 
 This module provides a command-line interface for formatting JSON files.
 It takes a path to either a JSON file or a directory containing JSON files
@@ -39,31 +40,31 @@
 
 * `122`: Indicates that the specified file or directory was not found.
 
 * `123`: Indicates that there was an internal error.
 
 Example usage:
 --------------
-::
 
+```
 $ jsonator /path/to/json/file.json --check
-
+```
 
 Dev:
 --------------
 Build package
 
-::
-
+```
 $ python -m build
+```
 
 Check package
 
-::
-
+```
 $ twine check dist/*
+```
 
 Publish package
 
-::
-
-$ twine upload dist/*
+```
+$ twine upload dist/*
+```
```

### Comparing `jsonator-0.1.5/pyproject.toml` & `jsonator-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = [
     "hatchling>=0.25.1",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonator"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Sergey Fomin", email="sergiusnn@gmail.com" },
 ]
 description = "JSON formatting and validating tool"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
 ]
 
 [project.urls]
@@ -31,14 +31,14 @@
     "/jsonator/*",
 ]
 
 [project.scripts]
 jsonator = "jsonator:main"
 
 [tool.poetry]
-readme = "README.rst"
+readme = "README.md"
 name = "jsonator"
-version = "0.1.5"
+version = "0.1.6"
 description = "JSON formatting and validating tool"
 authors = [
   "Sergey Fomin <sergiusnn@gmail.com>",
-]
+]
```

### Comparing `jsonator-0.1.5/PKG-INFO` & `jsonator-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: jsonator
-Version: 0.1.5
+Version: 0.1.6
 Summary: JSON formatting and validating tool
 Project-URL: Homepage, https://github.com/sfominx/jsonator
 Author-email: Sergey Fomin <sergiusnn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
 JSONator
 ========
 
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Downloads](https://static.pepy.tech/badge/jsonator)](https://pepy.tech/project/jsonator)
 
 Description
 -----------
 
 This module provides a command-line interface for formatting JSON files.
 It takes a path to either a JSON file or a directory containing JSON files
@@ -51,31 +52,31 @@
 
 * `122`: Indicates that the specified file or directory was not found.
 
 * `123`: Indicates that there was an internal error.
 
 Example usage:
 --------------
-::
 
+```
 $ jsonator /path/to/json/file.json --check
-
+```
 
 Dev:
 --------------
 Build package
 
-::
-
+```
 $ python -m build
+```
 
 Check package
 
-::
-
+```
 $ twine check dist/*
+```
 
 Publish package
 
-::
-
-$ twine upload dist/*
+```
+$ twine upload dist/*
+```
```

