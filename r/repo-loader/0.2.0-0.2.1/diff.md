# Comparing `tmp/repo-loader-0.2.0.tar.gz` & `tmp/repo-loader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-loader-0.2.0.tar", last modified: Tue Aug  1 10:09:11 2023, max compression
+gzip compressed data, was "repo-loader-0.2.1.tar", last modified: Tue Aug  1 10:40:24 2023, max compression
```

## Comparing `repo-loader-0.2.0.tar` & `repo-loader-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/push_macos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/push_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/push_win.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.gptignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 10:09:03.000000 repo-loader-0.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 10:09:03.000000 repo-loader-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 10:09:03.000000 repo-loader-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-01 10:09:11.034613 repo-loader-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-01 10:09:03.000000 repo-loader-0.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-08-01 10:09:03.000000 repo-loader-0.2.0/activate.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-08-01 10:09:03.000000 repo-loader-0.2.0/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-01 10:09:03.000000 repo-loader-0.2.0/make_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 10:09:03.000000 repo-loader-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:09:03.000000 repo-loader-0.2.0/requirements.testing.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:09:11.034613 repo-loader-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 10:09:03.000000 repo-loader-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.026612 repo-loader-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/src/repo_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/.gptignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/repo_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-01 10:09:03.000000 repo-loader-0.2.0/src/repo_loader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.030612 repo-loader-0.2.0/src/repo_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 10:09:11.000000 repo-loader-0.2.0/src/repo_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 10:09:10.000000 repo-loader-0.2.0/src/repo_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/tests/test_data/example_repo/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/.gptignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/file2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:09:11.034613 repo-loader-0.2.0/tests/test_data/example_repo/folder1/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/folder1/file3.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/example_repo/folder1/file4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_data/expected_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tests/test_gpt_repository_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 10:09:03.000000 repo-loader-0.2.0/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-08-01 10:09:03.000000 repo-loader-0.2.0/upload_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.584610 repo-loader-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/push_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/push_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/push_win.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.gptignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 10:40:17.000000 repo-loader-0.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 10:40:17.000000 repo-loader-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 10:40:17.000000 repo-loader-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-01 10:40:24.584610 repo-loader-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-08-01 10:40:17.000000 repo-loader-0.2.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-08-01 10:40:17.000000 repo-loader-0.2.1/activate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-08-01 10:40:17.000000 repo-loader-0.2.1/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-01 10:40:17.000000 repo-loader-0.2.1/make_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 10:40:17.000000 repo-loader-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 10:40:17.000000 repo-loader-0.2.1/requirements.testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:40:24.584610 repo-loader-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 10:40:17.000000 repo-loader-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.576610 repo-loader-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/src/repo_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/.gptignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/repo_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-01 10:40:17.000000 repo-loader-0.2.1/src/repo_loader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/src/repo_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 10:40:24.000000 repo-loader-0.2.1/src/repo_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.580610 repo-loader-0.2.1/tests/test_data/example_repo/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/.gptignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/file2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:40:24.584610 repo-loader-0.2.1/tests/test_data/example_repo/folder1/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/folder1/file3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/example_repo/folder1/file4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_data/expected_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tests/test_gpt_repository_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 10:40:17.000000 repo-loader-0.2.1/tox.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-08-01 10:40:17.000000 repo-loader-0.2.1/upload_package.sh
```

### Comparing `repo-loader-0.2.0/.github/workflows/lint.yml` & `repo-loader-0.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/.github/workflows/push_macos.yml` & `repo-loader-0.2.1/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/.github/workflows/push_ubuntu.yml` & `repo-loader-0.2.1/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/.github/workflows/push_win.yml` & `repo-loader-0.2.1/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/.github/workflows/release_pypi.yml` & `repo-loader-0.2.1/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/.gitignore` & `repo-loader-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/.vscode/settings.json` & `repo-loader-0.2.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/LICENSE` & `repo-loader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/PKG-INFO` & `repo-loader-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-loader
-Version: 0.2.0
+Version: 0.2.1
 Summary: repository loader for github and chatgpt
 Home-page: https://github.com/cachho/repo-loader
 Maintainer: cachho
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -46,24 +46,24 @@
 ```python
 from repo_loader import repo_loader
 repo_loader.load("example_repo")
 ```
 
 ### Options
 
-| Argument                     | Type | Default                                               | Description                                                             |
-| ---------------------------- | ---- | ----------------------------------------------------- | ----------------------------------------------------------------------- |
-| `repo_path`                  | str  | Current directory                                     | The path to the git repository to be processed.                         |
-| `out_path`                   | str  | 'output.txt'                                          | The path to the output file.                                            |
-| `preamble_file`              | str  | None                                                  | The path to a preamble file. Contents are written to output first.      |
-| `preamble`                   | str  | The following text is a Git repository with code. ... | Text that will be written to the output file before the repo contents.  |
-| `clipboard`                  | bool | False                                                 | If True, output is copied to the clipboard instead of a file.           |
-| `quiet`                      | bool | False                                                 | If True, the script will not print to stdout or auto-open the file.     |
-| `progress`                   | bool | False                                                 | If True, the script will display a progress bar during processing.      |
-| `open_file_after_processing` | bool | False                                                 | If True, the output file will be automatically opened after processing. |
+| Argument                     | Type | Default                                                                                                                         | Description                                                             |
+| ---------------------------- | ---- | ------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
+| `repo_path`                  | str  | Current directory                                                                                                               | The path to the git repository to be processed.                         |
+| `out_path`                   | str  | 'output.txt'                                                                                                                    | The path to the output file.                                            |
+| `preamble_file`              | str  | None                                                                                                                            | The path to a preamble file. Contents are written to output first.      |
+| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/9801bbe6e879455376a337cf207db2dcc30d8225/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
+| `clipboard`                  | bool | False                                                                                                                           | If True, output is copied to the clipboard instead of a file.           |
+| `quiet`                      | bool | False                                                                                                                           | If True, the script will not print to stdout or auto-open the file.     |
+| `progress`                   | bool | False                                                                                                                           | If True, the script will display a progress bar during processing.      |
+| `open_file_after_processing` | bool | False                                                                                                                           | If True, the output file will be automatically opened after processing. |
 
 ## Description
 
 `repo-loader` is a command-line and script tool that converts the contents of a Git repository into a text format, preserving the structure of the files and file contents. The generated output can be interpreted by AI language models, allowing them to process the repository's contents for various tasks, such as code review or documentation generation.
 
 ## Contributing
```

### Comparing `repo-loader-0.2.0/README.md` & `repo-loader-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 ```python
 from repo_loader import repo_loader
 repo_loader.load("example_repo")
 ```
 
 ### Options
 
-| Argument                     | Type | Default                                               | Description                                                             |
-| ---------------------------- | ---- | ----------------------------------------------------- | ----------------------------------------------------------------------- |
-| `repo_path`                  | str  | Current directory                                     | The path to the git repository to be processed.                         |
-| `out_path`                   | str  | 'output.txt'                                          | The path to the output file.                                            |
-| `preamble_file`              | str  | None                                                  | The path to a preamble file. Contents are written to output first.      |
-| `preamble`                   | str  | The following text is a Git repository with code. ... | Text that will be written to the output file before the repo contents.  |
-| `clipboard`                  | bool | False                                                 | If True, output is copied to the clipboard instead of a file.           |
-| `quiet`                      | bool | False                                                 | If True, the script will not print to stdout or auto-open the file.     |
-| `progress`                   | bool | False                                                 | If True, the script will display a progress bar during processing.      |
-| `open_file_after_processing` | bool | False                                                 | If True, the output file will be automatically opened after processing. |
+| Argument                     | Type | Default                                                                                                                         | Description                                                             |
+| ---------------------------- | ---- | ------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
+| `repo_path`                  | str  | Current directory                                                                                                               | The path to the git repository to be processed.                         |
+| `out_path`                   | str  | 'output.txt'                                                                                                                    | The path to the output file.                                            |
+| `preamble_file`              | str  | None                                                                                                                            | The path to a preamble file. Contents are written to output first.      |
+| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/9801bbe6e879455376a337cf207db2dcc30d8225/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
+| `clipboard`                  | bool | False                                                                                                                           | If True, output is copied to the clipboard instead of a file.           |
+| `quiet`                      | bool | False                                                                                                                           | If True, the script will not print to stdout or auto-open the file.     |
+| `progress`                   | bool | False                                                                                                                           | If True, the script will display a progress bar during processing.      |
+| `open_file_after_processing` | bool | False                                                                                                                           | If True, the output file will be automatically opened after processing. |
 
 ## Description
 
 `repo-loader` is a command-line and script tool that converts the contents of a Git repository into a text format, preserving the structure of the files and file contents. The generated output can be interpreted by AI language models, allowing them to process the repository's contents for various tasks, such as code review or documentation generation.
 
 ## Contributing
```

### Comparing `repo-loader-0.2.0/make_venv.py` & `repo-loader-0.2.1/make_venv.py`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/pyproject.toml` & `repo-loader-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "pyperclip",
     "pathspec==0.11.1",
     "tqdm==4.65.0"
 ]
 
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
     "i",
     "ok",
     "id",
```

### Comparing `repo-loader-0.2.0/setup.py` & `repo-loader-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/src/repo_loader/repo_loader.py` & `repo-loader-0.2.1/src/repo_loader/repo_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,18 @@
     # Validate arguments
     if preamble and preamble_file:
         raise ValueError("Preamble and preamble file cannot be used together")
 
     # Set defaults
     repo_path = repo_path or os.getcwd()
     out_path = out_path or "output.txt"
-    preamble = preamble or "The following text is a Git repository with code. ..."
+    preamble = (
+        preamble
+        or "The following text is a Git repository with code. The structure of the text are sections that begin with ----!@#$----, followed by a single line containing the file path and file name, followed by a variable amount of lines containing the file contents. The text representing the Git repository ends when the symbols --END-- are encounted. Any further text beyond --END-- are meant to be interpreted as instructions using the aforementioned Git repository as context."
+    )
 
     gpt_ignore_list = build_ignore_list(repo_path=repo_path, filename=".gptignore")
     git_ignore_list = build_ignore_list(repo_path=repo_path, filename=".gitignore")
 
     ignore_list = gpt_ignore_list + git_ignore_list + [out_path]
     ignore_list = [x for x in ignore_list if x and len(x) > 0 and x[0] != "#"]
     ignore_list = list(set(ignore_list))
```

### Comparing `repo-loader-0.2.0/src/repo_loader.egg-info/PKG-INFO` & `repo-loader-0.2.1/src/repo_loader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-loader
-Version: 0.2.0
+Version: 0.2.1
 Summary: repository loader for github and chatgpt
 Home-page: https://github.com/cachho/repo-loader
 Maintainer: cachho
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -46,24 +46,24 @@
 ```python
 from repo_loader import repo_loader
 repo_loader.load("example_repo")
 ```
 
 ### Options
 
-| Argument                     | Type | Default                                               | Description                                                             |
-| ---------------------------- | ---- | ----------------------------------------------------- | ----------------------------------------------------------------------- |
-| `repo_path`                  | str  | Current directory                                     | The path to the git repository to be processed.                         |
-| `out_path`                   | str  | 'output.txt'                                          | The path to the output file.                                            |
-| `preamble_file`              | str  | None                                                  | The path to a preamble file. Contents are written to output first.      |
-| `preamble`                   | str  | The following text is a Git repository with code. ... | Text that will be written to the output file before the repo contents.  |
-| `clipboard`                  | bool | False                                                 | If True, output is copied to the clipboard instead of a file.           |
-| `quiet`                      | bool | False                                                 | If True, the script will not print to stdout or auto-open the file.     |
-| `progress`                   | bool | False                                                 | If True, the script will display a progress bar during processing.      |
-| `open_file_after_processing` | bool | False                                                 | If True, the output file will be automatically opened after processing. |
+| Argument                     | Type | Default                                                                                                                         | Description                                                             |
+| ---------------------------- | ---- | ------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
+| `repo_path`                  | str  | Current directory                                                                                                               | The path to the git repository to be processed.                         |
+| `out_path`                   | str  | 'output.txt'                                                                                                                    | The path to the output file.                                            |
+| `preamble_file`              | str  | None                                                                                                                            | The path to a preamble file. Contents are written to output first.      |
+| `preamble`                   | str  | [here](https://github.com/cachho/repo-loader/blob/9801bbe6e879455376a337cf207db2dcc30d8225/src/repo_loader/repo_loader.py#L184) | Text that will be written to the output file before the repo contents.  |
+| `clipboard`                  | bool | False                                                                                                                           | If True, output is copied to the clipboard instead of a file.           |
+| `quiet`                      | bool | False                                                                                                                           | If True, the script will not print to stdout or auto-open the file.     |
+| `progress`                   | bool | False                                                                                                                           | If True, the script will display a progress bar during processing.      |
+| `open_file_after_processing` | bool | False                                                                                                                           | If True, the output file will be automatically opened after processing. |
 
 ## Description
 
 `repo-loader` is a command-line and script tool that converts the contents of a Git repository into a text format, preserving the structure of the files and file contents. The generated output can be interpreted by AI language models, allowing them to process the repository's contents for various tasks, such as code review or documentation generation.
 
 ## Contributing
```

### Comparing `repo-loader-0.2.0/src/repo_loader.egg-info/SOURCES.txt` & `repo-loader-0.2.1/src/repo_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repo-loader-0.2.0/tests/test_gpt_repository_loader.py` & `repo-loader-0.2.1/tests/test_gpt_repository_loader.py`

 * *Files identical despite different names*

