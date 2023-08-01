# Comparing `tmp/python-dotenv-vault-0.6.0.tar.gz` & `tmp/python-dotenv-vault-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dotenv-vault-0.6.0.tar", last modified: Tue May 16 04:39:03 2023, max compression
+gzip compressed data, was "python-dotenv-vault-0.6.1.tar", last modified: Tue Aug  1 00:45:06 2023, max compression
```

## Comparing `python-dotenv-vault-0.6.0.tar` & `python-dotenv-vault-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:39:03.167764 python-dotenv-vault-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-16 04:39:03.167764 python-dotenv-vault-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:39:03.167764 python-dotenv-vault-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:39:03.163764 python-dotenv-vault-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:39:03.163764 python-dotenv-vault-0.6.0/src/dotenv_vault/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/src/dotenv_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/src/dotenv_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/src/dotenv_vault/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-16 04:38:44.000000 python-dotenv-vault-0.6.0/src/dotenv_vault/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:39:03.163764 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 04:39:03.000000 python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:45:06.780162 python-dotenv-vault-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/src/dotenv_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/src/dotenv_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/src/dotenv_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/src/dotenv_vault/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/src/dotenv_vault/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/top_level.txt
```

### Comparing `python-dotenv-vault-0.6.0/CHANGELOG.md` & `python-dotenv-vault-0.6.1/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.1
+
+### Changed
+
+- Fix fallback issue with gunicorn not respecting the current working directory when attempting to call `find_dotenv`. [#17](https://github.com/dotenv-org/python-dotenv-vault/pull/17)
+
 ## 0.6.0
 
 ### Changed
 
 - Fix environment variable load [#12](https://github.com/dotenv-org/python-dotenv-vault/pull/12)
 
 ## 0.5.1
```

### Comparing `python-dotenv-vault-0.6.0/LICENSE` & `python-dotenv-vault-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.0/PKG-INFO` & `python-dotenv-vault-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.6.0
+Version: 0.6.1
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
@@ -41,25 +41,27 @@
 S3_BUCKET=YOURS3BUCKET
 SECRET_KEY=YOURSECRETKEYGOESHERE
 ```
 
 As early as possible in your application bootstrap process, load .env:
 
 ```python
+import os
 from dotenv_vault import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
 # Code of your application, which uses environment variables (e.g. from `os.environ` or
 # `os.getenv`) as if they came from the actual environment.
 ```
 
 When your application loads, these variables will be available in `os.environ` or `os.getenv`:
 
 ```python
+import os
 s3_bucket = os.getenv("S3_BUCKET")
 print(s3_bucket)
 ```
 
 ## 🚀 Deploying
 
 Encrypt your environment variables by doing:
@@ -170,14 +172,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.1
+
+### Changed
+
+- Fix fallback issue with gunicorn not respecting the current working directory when attempting to call `find_dotenv`. [#17](https://github.com/dotenv-org/python-dotenv-vault/pull/17)
+
 ## 0.6.0
 
 ### Changed
 
 - Fix environment variable load [#12](https://github.com/dotenv-org/python-dotenv-vault/pull/12)
 
 ## 0.5.1
```

### Comparing `python-dotenv-vault-0.6.0/README.md` & `python-dotenv-vault-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,25 +29,27 @@
 S3_BUCKET=YOURS3BUCKET
 SECRET_KEY=YOURSECRETKEYGOESHERE
 ```
 
 As early as possible in your application bootstrap process, load .env:
 
 ```python
+import os
 from dotenv_vault import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
 # Code of your application, which uses environment variables (e.g. from `os.environ` or
 # `os.getenv`) as if they came from the actual environment.
 ```
 
 When your application loads, these variables will be available in `os.environ` or `os.getenv`:
 
 ```python
+import os
 s3_bucket = os.getenv("S3_BUCKET")
 print(s3_bucket)
 ```
 
 ## 🚀 Deploying
 
 Encrypt your environment variables by doing:
```

### Comparing `python-dotenv-vault-0.6.0/setup.py` & `python-dotenv-vault-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.0/src/dotenv_vault/main.py` & `python-dotenv-vault-0.6.1/src/dotenv_vault/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,21 @@
     """
     if "DOTENV_KEY" in os.environ:
         vault_stream = parse_vault(open(".env.vault"))
         return dotenv.load_dotenv(
             stream=vault_stream,
             verbose=verbose,
             override=override,
-            interpolate=interpolate
+            interpolate=interpolate,
+            encoding=encoding
         )
     else:
+        dotenv_path = dotenv.find_dotenv(usecwd=True)
+        stream = open(dotenv_path) if not stream else stream
         return dotenv.load_dotenv(
-            dotenv_path=dotenv_path,
             stream=stream, 
             verbose=verbose, 
             override=override, 
             interpolate=interpolate, 
             encoding=encoding
         )
```

### Comparing `python-dotenv-vault-0.6.0/src/dotenv_vault/test_vault.py` & `python-dotenv-vault-0.6.1/src/dotenv_vault/test_vault.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.0/src/python_dotenv_vault.egg-info/PKG-INFO` & `python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.6.0
+Version: 0.6.1
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
@@ -41,25 +41,27 @@
 S3_BUCKET=YOURS3BUCKET
 SECRET_KEY=YOURSECRETKEYGOESHERE
 ```
 
 As early as possible in your application bootstrap process, load .env:
 
 ```python
+import os
 from dotenv_vault import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
 # Code of your application, which uses environment variables (e.g. from `os.environ` or
 # `os.getenv`) as if they came from the actual environment.
 ```
 
 When your application loads, these variables will be available in `os.environ` or `os.getenv`:
 
 ```python
+import os
 s3_bucket = os.getenv("S3_BUCKET")
 print(s3_bucket)
 ```
 
 ## 🚀 Deploying
 
 Encrypt your environment variables by doing:
@@ -170,14 +172,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.1
+
+### Changed
+
+- Fix fallback issue with gunicorn not respecting the current working directory when attempting to call `find_dotenv`. [#17](https://github.com/dotenv-org/python-dotenv-vault/pull/17)
+
 ## 0.6.0
 
 ### Changed
 
 - Fix environment variable load [#12](https://github.com/dotenv-org/python-dotenv-vault/pull/12)
 
 ## 0.5.1
```

