# Comparing `tmp/repo-loader-0.1.2.tar.gz` & `tmp/repo-loader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-loader-0.1.2.tar", last modified: Tue Aug  1 09:08:12 2023, max compression
+gzip compressed data, was "repo-loader-0.1.3.tar", last modified: Tue Aug  1 09:14:40 2023, max compression
```

## Comparing `repo-loader-0.1.2.tar` & `repo-loader-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.271109 repo-loader-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.267109 repo-loader-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.267109 repo-loader-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.github/workflows/push_macos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.github/workflows/push_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.github/workflows/push_win.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.gptignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.271109 repo-loader-0.1.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 09:08:06.000000 repo-loader-0.1.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 09:08:06.000000 repo-loader-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 09:08:06.000000 repo-loader-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-01 09:08:12.271109 repo-loader-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-01 09:08:06.000000 repo-loader-0.1.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-08-01 09:08:06.000000 repo-loader-0.1.2/activate.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-08-01 09:08:06.000000 repo-loader-0.1.2/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-01 09:08:06.000000 repo-loader-0.1.2/make_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 09:08:06.000000 repo-loader-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 09:08:06.000000 repo-loader-0.1.2/requirements.testing.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:08:12.271109 repo-loader-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 09:08:06.000000 repo-loader-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.267109 repo-loader-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.271109 repo-loader-0.1.2/src/repo_loader/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 09:08:06.000000 repo-loader-0.1.2/src/repo_loader/.gptignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:06.000000 repo-loader-0.1.2/src/repo_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-01 09:08:06.000000 repo-loader-0.1.2/src/repo_loader/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-08-01 09:08:06.000000 repo-loader-0.1.2/src/repo_loader/repo_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-01 09:08:06.000000 repo-loader-0.1.2/src/repo_loader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.271109 repo-loader-0.1.2/src/repo_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-01 09:08:12.000000 repo-loader-0.1.2/src/repo_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 09:08:12.000000 repo-loader-0.1.2/src/repo_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:08:12.000000 repo-loader-0.1.2/src/repo_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 09:08:12.000000 repo-loader-0.1.2/src/repo_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 09:08:12.000000 repo-loader-0.1.2/src/repo_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 09:08:12.000000 repo-loader-0.1.2/src/repo_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.271109 repo-loader-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.271109 repo-loader-0.1.2/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.271109 repo-loader-0.1.2/tests/test_data/example_repo/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tests/test_data/example_repo/.gptignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tests/test_data/example_repo/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tests/test_data/example_repo/file2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:08:12.271109 repo-loader-0.1.2/tests/test_data/example_repo/folder1/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tests/test_data/example_repo/folder1/file3.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tests/test_data/example_repo/folder1/file4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tests/test_data/expected_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tests/test_gpt_repository_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 09:08:06.000000 repo-loader-0.1.2/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-08-01 09:08:06.000000 repo-loader-0.1.2/upload_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.700940 repo-loader-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/push_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/push_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/push_win.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.gptignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 09:14:31.000000 repo-loader-0.1.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 09:14:31.000000 repo-loader-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 09:14:31.000000 repo-loader-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-01 09:14:40.700940 repo-loader-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-01 09:14:31.000000 repo-loader-0.1.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-08-01 09:14:31.000000 repo-loader-0.1.3/activate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-08-01 09:14:31.000000 repo-loader-0.1.3/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-01 09:14:31.000000 repo-loader-0.1.3/make_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 09:14:31.000000 repo-loader-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 09:14:31.000000 repo-loader-0.1.3/requirements.testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:14:40.700940 repo-loader-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 09:14:31.000000 repo-loader-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.692940 repo-loader-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/src/repo_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/.gptignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/repo_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-01 09:14:31.000000 repo-loader-0.1.3/src/repo_loader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/src/repo_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 09:14:40.000000 repo-loader-0.1.3/src/repo_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.696940 repo-loader-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.700940 repo-loader-0.1.3/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.700940 repo-loader-0.1.3/tests/test_data/example_repo/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/.gptignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/file2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:14:40.700940 repo-loader-0.1.3/tests/test_data/example_repo/folder1/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/folder1/file3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/example_repo/folder1/file4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_data/expected_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tests/test_gpt_repository_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 09:14:31.000000 repo-loader-0.1.3/tox.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-08-01 09:14:31.000000 repo-loader-0.1.3/upload_package.sh
```

### Comparing `repo-loader-0.1.2/.github/workflows/lint.yml` & `repo-loader-0.1.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/.github/workflows/push_macos.yml` & `repo-loader-0.1.3/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/.github/workflows/push_ubuntu.yml` & `repo-loader-0.1.3/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/.github/workflows/push_win.yml` & `repo-loader-0.1.3/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/.gitignore` & `repo-loader-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/.vscode/settings.json` & `repo-loader-0.1.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/LICENSE` & `repo-loader-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/PKG-INFO` & `repo-loader-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-loader
-Version: 0.1.2
+Version: 0.1.3
 Summary: repository loader for github and chatgpt
 Home-page: https://github.com/cachho/repo-loader
 Maintainer: cachho
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `repo-loader-0.1.2/README.md` & `repo-loader-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/make_venv.py` & `repo-loader-0.1.3/make_venv.py`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/pyproject.toml` & `repo-loader-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "pyperclip",
     "pathspec==0.11.1",
     "tqdm==4.65.0"
 ]
 
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
     "i",
     "ok",
     "id",
```

### Comparing `repo-loader-0.1.2/setup.py` & `repo-loader-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/src/repo_loader/repo_loader.py` & `repo-loader-0.1.3/src/repo_loader/repo_loader.py`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/src/repo_loader.egg-info/PKG-INFO` & `repo-loader-0.1.3/src/repo_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-loader
-Version: 0.1.2
+Version: 0.1.3
 Summary: repository loader for github and chatgpt
 Home-page: https://github.com/cachho/repo-loader
 Maintainer: cachho
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `repo-loader-0.1.2/src/repo_loader.egg-info/SOURCES.txt` & `repo-loader-0.1.3/src/repo_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repo-loader-0.1.2/tests/test_gpt_repository_loader.py` & `repo-loader-0.1.3/tests/test_gpt_repository_loader.py`

 * *Files identical despite different names*

