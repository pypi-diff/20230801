# Comparing `tmp/repo-loader-0.2.1.tar.gz` & `tmp/repo-loader-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-loader-0.2.1.tar", last modified: Tue Aug  1 10:40:24 2023, max compression
+gzip compressed data, was "repo-loader-0.2.2.tar", last modified: Tue Aug  1 10:58:05 2023, max compression
```

## Comparing `repo-loader-0.2.1.tar` & `repo-loader-0.2.2.tar`

### file list

```diff
@@ -1,52 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.584610 repo-loader-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/push_macos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/push_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/push_win.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.gptignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 10:40:17.000000 repo-loader-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 10:40:17.000000 repo-loader-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-01 10:40:24.584610 repo-loader-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-08-01 10:40:17.000000 repo-loader-0.2.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-08-01 10:40:17.000000 repo-loader-0.2.1/activate.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-08-01 10:40:17.000000 repo-loader-0.2.1/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-01 10:40:17.000000 repo-loader-0.2.1/make_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 10:40:17.000000 repo-loader-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:40:17.000000 repo-loader-0.2.1/requirements.testing.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:40:24.584610 repo-loader-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 10:40:17.000000 repo-loader-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.576610 repo-loader-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/src/repo_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/.gptignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/repo_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/src/repo_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/tests/test_data/example_repo/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/.gptignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/file2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.584610 repo-loader-0.2.1/tests/test_data/example_repo/folder1/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/folder1/file3.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/folder1/file4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/expected_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_gpt_repository_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-08-01 10:40:17.000000 repo-loader-0.2.1/upload_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.864326 repo-loader-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.856326 repo-loader-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.860326 repo-loader-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.github/workflows/push_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.github/workflows/push_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.github/workflows/push_win.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.gptignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.860326 repo-loader-0.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 10:57:57.000000 repo-loader-0.2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 10:57:57.000000 repo-loader-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 10:57:57.000000 repo-loader-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-01 10:58:05.864326 repo-loader-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-08-01 10:57:57.000000 repo-loader-0.2.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-08-01 10:57:57.000000 repo-loader-0.2.2/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 10:57:57.000000 repo-loader-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:57:57.000000 repo-loader-0.2.2/requirements.testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:58:05.864326 repo-loader-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 10:57:57.000000 repo-loader-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.856326 repo-loader-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.860326 repo-loader-0.2.2/src/repo_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 10:57:57.000000 repo-loader-0.2.2/src/repo_loader/.gptignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:57:57.000000 repo-loader-0.2.2/src/repo_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 10:57:57.000000 repo-loader-0.2.2/src/repo_loader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-08-01 10:57:57.000000 repo-loader-0.2.2/src/repo_loader/repo_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-01 10:57:57.000000 repo-loader-0.2.2/src/repo_loader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.860326 repo-loader-0.2.2/src/repo_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-01 10:58:05.000000 repo-loader-0.2.2/src/repo_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-01 10:58:05.000000 repo-loader-0.2.2/src/repo_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:58:05.000000 repo-loader-0.2.2/src/repo_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 10:58:05.000000 repo-loader-0.2.2/src/repo_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:58:05.000000 repo-loader-0.2.2/src/repo_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 10:58:05.000000 repo-loader-0.2.2/src/repo_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.860326 repo-loader-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.860326 repo-loader-0.2.2/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.864326 repo-loader-0.2.2/tests/test_data/example_repo/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tests/test_data/example_repo/.gptignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tests/test_data/example_repo/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tests/test_data/example_repo/file2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:58:05.864326 repo-loader-0.2.2/tests/test_data/example_repo/folder1/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tests/test_data/example_repo/folder1/file3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tests/test_data/example_repo/folder1/file4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tests/test_data/expected_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tests/test_gpt_repository_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 10:57:57.000000 repo-loader-0.2.2/tox.ini
```

### Comparing `repo-loader-0.2.1/.github/workflows/lint.yml` & `repo-loader-0.2.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/.github/workflows/push_macos.yml` & `repo-loader-0.2.2/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/.github/workflows/push_ubuntu.yml` & `repo-loader-0.2.2/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/.github/workflows/push_win.yml` & `repo-loader-0.2.2/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/.github/workflows/release_pypi.yml` & `repo-loader-0.2.2/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/.gitignore` & `repo-loader-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/.vscode/settings.json` & `repo-loader-0.2.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/LICENSE` & `repo-loader-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/PKG-INFO` & `repo-loader-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-loader
-Version: 0.2.1
+Version: 0.2.2
 Summary: repository loader for github and chatgpt
 Home-page: https://github.com/cachho/repo-loader
 Maintainer: cachho
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -51,15 +51,15 @@
 ### Options
 
 | Argument                     | Type | Default                                                                                                                         | Description                                                             |
 | ---------------------------- | ---- | ------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
 | `repo_path`                  | str  | Current directory                                                                                                               | The path to the git repository to be processed.                         |
 | `out_path`                   | str  | 'output.txt'                                                                                                                    | The path to the output file.                                            |
 | `preamble_file`              | str  | None                                                                                                                            | The path to a preamble file. Contents are written to output first.      |
-| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/9801bbe6e879455376a337cf207db2dcc30d8225/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
+| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/f2be8ff244e85b6df640b8cd5539ed7b1b3661e0/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
 | `clipboard`                  | bool | False                                                                                                                           | If True, output is copied to the clipboard instead of a file.           |
 | `quiet`                      | bool | False                                                                                                                           | If True, the script will not print to stdout or auto-open the file.     |
 | `progress`                   | bool | False                                                                                                                           | If True, the script will display a progress bar during processing.      |
 | `open_file_after_processing` | bool | False                                                                                                                           | If True, the output file will be automatically opened after processing. |
 
 ## Description
```

### Comparing `repo-loader-0.2.1/README.md` & `repo-loader-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ### Options
 
 | Argument                     | Type | Default                                                                                                                         | Description                                                             |
 | ---------------------------- | ---- | ------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
 | `repo_path`                  | str  | Current directory                                                                                                               | The path to the git repository to be processed.                         |
 | `out_path`                   | str  | 'output.txt'                                                                                                                    | The path to the output file.                                            |
 | `preamble_file`              | str  | None                                                                                                                            | The path to a preamble file. Contents are written to output first.      |
-| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/9801bbe6e879455376a337cf207db2dcc30d8225/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
+| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/f2be8ff244e85b6df640b8cd5539ed7b1b3661e0/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
 | `clipboard`                  | bool | False                                                                                                                           | If True, output is copied to the clipboard instead of a file.           |
 | `quiet`                      | bool | False                                                                                                                           | If True, the script will not print to stdout or auto-open the file.     |
 | `progress`                   | bool | False                                                                                                                           | If True, the script will display a progress bar during processing.      |
 | `open_file_after_processing` | bool | False                                                                                                                           | If True, the output file will be automatically opened after processing. |
 
 ## Description
```

### Comparing `repo-loader-0.2.1/pyproject.toml` & `repo-loader-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "pyperclip",
     "pathspec==0.11.1",
     "tqdm==4.65.0"
 ]
 
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
     "i",
     "ok",
     "id",
```

### Comparing `repo-loader-0.2.1/setup.py` & `repo-loader-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.1/src/repo_loader/repo_loader.py` & `repo-loader-0.2.2/src/repo_loader/repo_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,17 @@
                 continue
 
             if not is_quiet and not use_progress_bar:
                 print(f"Processing directory: {content}")
 
             pbar = (
                 tqdm(
-                    total=num_files, bar_format="{l_bar}{bar:50}{r_bar}", desc=f"{content[:17]:<20}"
+                    total=num_files,
+                    bar_format="{l_bar}{bar:50}{r_bar}",
+                    desc=f"{content[:17]:<20}",
                 )
                 if use_progress_bar
                 else None
             )
 
             for root, _, files in os.walk(content_path):
                 for file in files:
@@ -244,24 +246,36 @@
                         If no directory is specified, the config file will be written
                         to the current working directory.
     """
     # copy this but using argparse
     parser = argparse.ArgumentParser(
         description="Process a git repository into a single file for chat gpt."
     )
-    parser.add_argument("repo_path", help="path to the git repository", type=str, nargs="?")
+    parser.add_argument(
+        "repo_path", help="path to the git repository", type=str, nargs="?"
+    )
     parser.add_argument("-o", "--output", help="output file path", type=str, nargs="?")
     parser.add_argument(
         "-p", "--preamble_file", help="path to the preamble file", type=str, nargs="?"
     )
-    parser.add_argument("--preamble", help="preamble text as raw string", type=str, nargs="?")
-    parser.add_argument("--clipboard", help="copy the output to the clipboard", action="store_true")
-    parser.add_argument("-q", "--quiet", help="no stdout, file not opened", action="store_true")
-    parser.add_argument("-pg", "--progress", help="display a progress bar", action="store_true")
-    parser.add_argument("--open", help="open file after processing", action="store_true")
+    parser.add_argument(
+        "--preamble", help="preamble text as raw string", type=str, nargs="?"
+    )
+    parser.add_argument(
+        "--clipboard", help="copy the output to the clipboard", action="store_true"
+    )
+    parser.add_argument(
+        "-q", "--quiet", help="no stdout, file not opened", action="store_true"
+    )
+    parser.add_argument(
+        "-pg", "--progress", help="display a progress bar", action="store_true"
+    )
+    parser.add_argument(
+        "--open", help="open file after processing", action="store_true"
+    )
     parser.add_argument(
         "--write-config",
         help="Write a default config file to the target directory.",
         type=str,
         nargs="?",
     )
     args = parser.parse_args()
```

### Comparing `repo-loader-0.2.1/src/repo_loader.egg-info/PKG-INFO` & `repo-loader-0.2.2/src/repo_loader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-loader
-Version: 0.2.1
+Version: 0.2.2
 Summary: repository loader for github and chatgpt
 Home-page: https://github.com/cachho/repo-loader
 Maintainer: cachho
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -51,15 +51,15 @@
 ### Options
 
 | Argument                     | Type | Default                                                                                                                         | Description                                                             |
 | ---------------------------- | ---- | ------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
 | `repo_path`                  | str  | Current directory                                                                                                               | The path to the git repository to be processed.                         |
 | `out_path`                   | str  | 'output.txt'                                                                                                                    | The path to the output file.                                            |
 | `preamble_file`              | str  | None                                                                                                                            | The path to a preamble file. Contents are written to output first.      |
-| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/9801bbe6e879455376a337cf207db2dcc30d8225/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
+| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/f2be8ff244e85b6df640b8cd5539ed7b1b3661e0/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
 | `clipboard`                  | bool | False                                                                                                                           | If True, output is copied to the clipboard instead of a file.           |
 | `quiet`                      | bool | False                                                                                                                           | If True, the script will not print to stdout or auto-open the file.     |
 | `progress`                   | bool | False                                                                                                                           | If True, the script will display a progress bar during processing.      |
 | `open_file_after_processing` | bool | False                                                                                                                           | If True, the output file will be automatically opened after processing. |
 
 ## Description
```

### Comparing `repo-loader-0.2.1/src/repo_loader.egg-info/SOURCES.txt` & `repo-loader-0.2.2/src/repo_loader.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 .gitignore
 .gptignore
 LICENSE
 MANIFEST.in
 README.md
-activate.sh
 lint.sh
-make_venv.py
 pyproject.toml
 requirements.testing.txt
 setup.py
 tox.ini
-upload_package.sh
 .github/CODEOWNERS
 .github/workflows/lint.yml
 .github/workflows/push_macos.yml
 .github/workflows/push_ubuntu.yml
 .github/workflows/push_win.yml
 .github/workflows/release_pypi.yml
 .vscode/settings.json
```

### Comparing `repo-loader-0.2.1/tests/test_gpt_repository_loader.py` & `repo-loader-0.2.2/tests/test_gpt_repository_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import os
 import shutil
 import tempfile
 import unittest
 
-from repo_loader.repo_loader import (
-    build_ignore_list,
-    process_repository,
-)
+from repo_loader.repo_loader import build_ignore_list, process_repository
 
 PROJECT_ROOT = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 GPT_IGNORE_PATH = os.path.join(PROJECT_ROOT, "src", "repo_loader", ".gptignore")
 
 
 class TestGPTRepositoryLoader(unittest.TestCase):
     def setUp(self):
         self.test_data_path = os.path.join(os.path.dirname(__file__), "test_data")
         self.example_repo_path = os.path.join(self.test_data_path, "example_repo")
 
     def test_end_to_end(self):
         # Set up the output file and the expected output file paths
         output_file_path = os.path.join(tempfile.mkdtemp(), "output.txt")
-        expected_output_file_path = os.path.join(self.test_data_path, "expected_output.txt")
+        expected_output_file_path = os.path.join(
+            self.test_data_path, "expected_output.txt"
+        )
 
         # Create an ignore list for the example repository
         ignore_file_path = os.path.join(self.example_repo_path, ".gptignore")
         if os.path.exists(ignore_file_path):
             ignore_list = build_ignore_list(self.example_repo_path, ".gptignore")
         else:
             ignore_list = []
```

