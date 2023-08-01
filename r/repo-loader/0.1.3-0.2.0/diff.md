# Comparing `tmp/repo-loader-0.1.3.tar.gz` & `tmp/repo-loader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-loader-0.1.3.tar", last modified: Tue Aug  1 09:14:40 2023, max compression
+gzip compressed data, was "repo-loader-0.2.0.tar", last modified: Tue Aug  1 10:09:11 2023, max compression
```

## Comparing `repo-loader-0.1.3.tar` & `repo-loader-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.700940 repo-loader-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/push_macos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/push_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/push_win.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.gptignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 09:14:31.000000 repo-loader-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 09:14:31.000000 repo-loader-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-01 09:14:40.700940 repo-loader-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-01 09:14:31.000000 repo-loader-0.1.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-08-01 09:14:31.000000 repo-loader-0.1.3/activate.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-08-01 09:14:31.000000 repo-loader-0.1.3/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-01 09:14:31.000000 repo-loader-0.1.3/make_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 09:14:31.000000 repo-loader-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 09:14:31.000000 repo-loader-0.1.3/requirements.testing.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:14:40.700940 repo-loader-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 09:14:31.000000 repo-loader-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.692940 repo-loader-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/src/repo_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/.gptignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/repo_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/src/repo_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.700940 repo-loader-0.1.3/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.700940 repo-loader-0.1.3/tests/test_data/example_repo/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/.gptignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/file2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.700940 repo-loader-0.1.3/tests/test_data/example_repo/folder1/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/folder1/file3.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/folder1/file4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/expected_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_gpt_repository_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-08-01 09:14:31.000000 repo-loader-0.1.3/upload_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/push_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/push_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/push_win.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.gptignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 10:09:03.000000 repo-loader-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 10:09:03.000000 repo-loader-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-01 10:09:11.034613 repo-loader-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-01 10:09:03.000000 repo-loader-0.2.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-08-01 10:09:03.000000 repo-loader-0.2.0/activate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-08-01 10:09:03.000000 repo-loader-0.2.0/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-01 10:09:03.000000 repo-loader-0.2.0/make_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 10:09:03.000000 repo-loader-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:09:03.000000 repo-loader-0.2.0/requirements.testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:09:11.034613 repo-loader-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 10:09:03.000000 repo-loader-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.026612 repo-loader-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/src/repo_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/.gptignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/repo_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/src/repo_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 10:09:11.000000 repo-loader-0.2.0/src/repo_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/tests/test_data/example_repo/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/.gptignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/file2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/tests/test_data/example_repo/folder1/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/folder1/file3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/folder1/file4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/expected_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_gpt_repository_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tox.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-08-01 10:09:03.000000 repo-loader-0.2.0/upload_package.sh
```

### Comparing `repo-loader-0.1.3/.github/workflows/lint.yml` & `repo-loader-0.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/.github/workflows/push_macos.yml` & `repo-loader-0.2.0/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/.github/workflows/push_ubuntu.yml` & `repo-loader-0.2.0/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/.github/workflows/push_win.yml` & `repo-loader-0.2.0/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/.github/workflows/release_pypi.yml` & `repo-loader-0.2.0/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/.gitignore` & `repo-loader-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/.vscode/settings.json` & `repo-loader-0.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/LICENSE` & `repo-loader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/make_venv.py` & `repo-loader-0.2.0/make_venv.py`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/pyproject.toml` & `repo-loader-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "pyperclip",
     "pathspec==0.11.1",
     "tqdm==4.65.0"
 ]
 
-version = "0.1.3"
+version = "0.2.0"
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
     "i",
     "ok",
     "id",
```

### Comparing `repo-loader-0.1.3/setup.py` & `repo-loader-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/src/repo_loader/repo_loader.py` & `repo-loader-0.2.0/src/repo_loader/repo_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 import argparse
 import os
 import sys
+from typing import Optional
 
 import pyperclip
 from pathspec import PathSpec
 from pathspec.patterns import GitWildMatchPattern
 from tqdm import tqdm
 
 from .utils import is_readable
@@ -128,73 +129,148 @@
         # Add lines to ignore_list
         with open(ignore_file_path, "r") as ignore_file:
             for line in ignore_file:
                 ignore_list.append(line.strip())
     return ignore_list
 
 
-def main() -> int:  # pylint: disable=too-many-statements
-    # copy this but using argparse
-    parser = argparse.ArgumentParser(
-        description="Process a git repository into a single file for chat gpt."
-    )
-    parser.add_argument("repo_path", help="path to the git repository", type=str, nargs="?")
-    parser.add_argument("-o", "--output", help="output file path", type=str, nargs="?")
-    parser.add_argument("-p", "--preamble", help="path to the preamble file", type=str, nargs="?")
-    parser.add_argument("--clipboard", help="copy the output to the clipboard", action="store_true")
-    parser.add_argument("-q", "--quiet", help="no stdout, file not opened", action="store_true")
-    parser.add_argument("-pg", "--progress", help="display a progress bar", action="store_true")
-    parser.add_argument("--open", help="open file after processing", action="store_true")
-    parser.add_argument(
-        "--write-config",
-        help="Write a default config file to the target directory.",
-        type=str,
-        nargs="?",
-    )
-    args = parser.parse_args()
-
-    repo_path = args.repo_path or os.getcwd()
-    out_path = args.output or "output.txt"
+# pylint: disable=too-many-arguments, too-many-locals
+def load(
+    repo_path: Optional[str] = None,
+    out_path: Optional[str] = None,
+    preamble_file: Optional[str] = None,
+    preamble: Optional[str] = None,
+    clipboard: bool = False,
+    quiet: bool = False,
+    progress: bool = False,
+    open_file_after_processing: bool = False,
+):
+    """
+    Processes a git repository into a single text file.
+
+    Args:
+        repo_path (str, optional): The path to the git repository to be processed.
+                                   Defaults to the current working directory if None.
+        out_path (str, optional): The path to the output file.
+                                  Defaults to 'output.txt' if None.
+        preamble_file (str, optional): The path to a preamble file. The contents of this
+                                       file will be written to the output file before the
+                                       repository contents. If None, no preamble is used.
+        preamble (str, optional): Text that will be written to the output file before the
+                                  repository contents.
+                                  Cannot be used together with `--preamble-file`.
+        clipboard (bool, optional): If True, the contents of the output file will be
+                                     copied to the clipboard instead of written to a file.
+                                     Defaults to False.
+        quiet (bool, optional): If True, the script will not print to stdout
+                                and will not automatically open the output file.
+                                Defaults to False.
+        progress (bool, optional): If True, the script will display a progress
+                                   bar while processing the repository.
+                                   Defaults to False.
+        open_file_after_processing (bool, optional): If True, the output file will be
+                                                     automatically opened after processing.
+                                                     Defaults to False.
+    """
+
+    # Validate arguments
+    if preamble and preamble_file:
+        raise ValueError("Preamble and preamble file cannot be used together")
+
+    # Set defaults
+    repo_path = repo_path or os.getcwd()
+    out_path = out_path or "output.txt"
+    preamble = preamble or "The following text is a Git repository with code. ..."
 
     gpt_ignore_list = build_ignore_list(repo_path=repo_path, filename=".gptignore")
     git_ignore_list = build_ignore_list(repo_path=repo_path, filename=".gitignore")
 
-    # pylint: disable=fixme
-    # TODO: Added `output.txt` to gitignore, otherwise it keeps adding itself.
-    # There might be a better way to do this, in case there is a file with the same name you want to add.
     ignore_list = gpt_ignore_list + git_ignore_list + [out_path]
-    # Filter comments and empty lines
-    ignore_list = [x for x in ignore_list if len(x) > 0 and x[0] != "#"]
-    # Filter duplicats
+    ignore_list = [x for x in ignore_list if x and len(x) > 0 and x[0] != "#"]
     ignore_list = list(set(ignore_list))
 
-    preamble_file = args.preamble
-
     outfile = os.path.abspath(out_path)
     with open(outfile, "w") as output_file:
         if preamble_file:
             with open(preamble_file, "r") as pf:
                 preamble_text = pf.read()
                 output_file.write(f"{preamble_text}\n")
         else:
-            output_file.write(
-                "The following text is a Git repository with code. The structure of the text are sections that begin with ----!@#$----, followed by a single line containing the file path and file name, followed by a variable amount of lines containing the file contents. The text representing the Git repository ends when the symbols --END-- are encounted. Any further text beyond --END-- are meant to be interpreted as instructions using the aforementioned Git repository as context.\n"
-            )
-        process_repository(repo_path, ignore_list, output_file, args.progress, args.quiet)
+            output_file.write(f"{preamble}\n")
+        process_repository(repo_path, ignore_list, output_file, progress, quiet)
     with open(out_path, "a") as output_file:
         output_file.write("--END--")
 
-    # Post Processing
-    if not args.clipboard:
-        if not args.quiet:
+    if not clipboard:
+        if not quiet:
             print(f"Repository contents written to {out_path}")
-        if args.open:
+        if open_file_after_processing:
             open_file(filename=out_path)
-        return 0
-    if args.clipboard:
+    if clipboard:
         with open(out_path, "r") as output_file:
             contents = output_file.read()
         pyperclip.copy(contents)
         os.remove(out_path)
-        if not args.quiet:
+        if not quiet:
             print("Copied to clipboard")
+
+
+def main() -> int:
+    """
+    Processes a git repository into a single text file. The script is
+    intended to be used from the command line, and has several options
+    for customizing its behavior.
+
+    Command Line Arguments:
+        repo_path: The path to the git repository that should be processed.
+                   If this argument is omitted, the current working directory is used.
+        -o, --output: The path to the output file. If omitted, output.txt will be used.
+        -p, --preamble_file: The path to a preamble file. The contents of this file
+                        will be written to the output file before the repository contents.
+        --preamble: Text that will be written to the output file before the repository contents.
+                     Cannot be used together with `--preamble-file`.
+        --clipboard: If this flag is present, the contents of the output file
+                     will be copied to the clipboard instead of written to a file.
+        -q, --quiet: If this flag is present, the script will not print to stdout
+                     and will not automatically open the output file.
+        -pg, --progress: If this flag is present, the script will display a progress
+                         bar while processing the repository.
+        --open: If this flag is present, the output file will be automatically
+                opened after processing.
+        --write-config: Writes a default config file to the target directory.
+                        If a directory is specified, the config file will be written there.
+                        If no directory is specified, the config file will be written
+                        to the current working directory.
+    """
+    # copy this but using argparse
+    parser = argparse.ArgumentParser(
+        description="Process a git repository into a single file for chat gpt."
+    )
+    parser.add_argument("repo_path", help="path to the git repository", type=str, nargs="?")
+    parser.add_argument("-o", "--output", help="output file path", type=str, nargs="?")
+    parser.add_argument(
+        "-p", "--preamble_file", help="path to the preamble file", type=str, nargs="?"
+    )
+    parser.add_argument("--preamble", help="preamble text as raw string", type=str, nargs="?")
+    parser.add_argument("--clipboard", help="copy the output to the clipboard", action="store_true")
+    parser.add_argument("-q", "--quiet", help="no stdout, file not opened", action="store_true")
+    parser.add_argument("-pg", "--progress", help="display a progress bar", action="store_true")
+    parser.add_argument("--open", help="open file after processing", action="store_true")
+    parser.add_argument(
+        "--write-config",
+        help="Write a default config file to the target directory.",
+        type=str,
+        nargs="?",
+    )
+    args = parser.parse_args()
+
+    load(
+        repo_path=args.repo_path,
+        out_path=args.output,
+        preamble_file=args.preamble_file,
+        preamble=args.preamble,
+        clipboard=args.clipboard,
+        quiet=args.quiet,
+        progress=args.progress,
+        open_file_after_processing=args.open,
+    )
     return 0
```

### Comparing `repo-loader-0.1.3/src/repo_loader.egg-info/SOURCES.txt` & `repo-loader-0.2.0/src/repo_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.3/tests/test_gpt_repository_loader.py` & `repo-loader-0.2.0/tests/test_gpt_repository_loader.py`

 * *Files identical despite different names*

