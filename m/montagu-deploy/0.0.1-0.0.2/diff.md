# Comparing `tmp/montagu_deploy-0.0.1.tar.gz` & `tmp/montagu_deploy-0.0.2.tar.gz`

## Comparing `montagu_deploy-0.0.1.tar` & `montagu_deploy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,27 @@
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/config/basic/montagu.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/config/complete/montagu.yml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/src/montagu_deploy/__about__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/src/montagu_deploy/__init__.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/src/montagu_deploy/cli.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/src/montagu_deploy/config.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/src/montagu_deploy/montagu_constellation.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/tests/test_config.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/tests/test_constellation.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/tests/test_integration.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/README.md
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 montagu_deploy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/basic/diagnostic-reports.yml
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/basic/montagu.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/ci/diagnostic-reports.yml
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/ci/montagu.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/complete/diagnostic-reports.yml
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/config/complete/montagu.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/__about__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/admin.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/cli.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/config.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/database.py
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/src/montagu_deploy/montagu_constellation.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/orderly-web.yml
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/test_config.py
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/test_constellation.py
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/test_integration.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/tests/utils.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/README.md
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 montagu_deploy-0.0.2/PKG-INFO
```

### Comparing `montagu_deploy-0.0.1/.github/workflows/test.yml` & `montagu_deploy-0.0.2/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -31,13 +31,16 @@
         run: |
           python -m pip install --upgrade pip
           pip install hatch
       - name: Lint
         run: |
           hatch run lint:style
       - name: Test
+        env:
+          VAULT_TOKEN: ${{ secrets.VAULT_TOKEN }}
+          YOUTRACK_TOKEN: ${{ secrets.YOUTRACK_TOKEN }}
         run: |
           hatch run cov-ci
       - name: Upload to Codecov
         uses: codecov/codecov-action@v3
         with:
           fail_ci_if_error: true
```

### Comparing `montagu_deploy-0.0.1/src/montagu_deploy/cli.py` & `montagu_deploy-0.0.2/src/montagu_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `montagu_deploy-0.0.1/tests/test_cli.py` & `montagu_deploy-0.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `montagu_deploy-0.0.1/LICENSE.txt` & `montagu_deploy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `montagu_deploy-0.0.1/README.md` & `montagu_deploy-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 ## Dev requirements
 
 1. [Python3](https://www.python.org/downloads/) (>= 3.7)
 2. [Hatch](https://hatch.pypa.io/latest/install/)
 
 ## Test and lint
 
+For all integration tests to pass, you will need 2 environment variables:
+1. `YOUTRACK_TOKEN` - a token for accessing the YT API
+2. `VAULT_TOKEN` - a github PAT for a user in the vimc robots team.
+
 1. `hatch run test`
 2. `hatch run lint:fmt`
 
 To get coverage reported locally in the console, use `hatch run cov`. 
 On CI, use `hatch run cov-ci` to generate an xml report.
 
 ## Build
@@ -62,12 +66,17 @@
 ```
 
 ## Install from local sources
 
 1. `hatch build`
 2. `pip install dist/montagu_deploy-{version}.tar.gz`
 
+## Publish to PyPi
+
+```console
+hatch publish
+```
 
 ## License
 
 `montagu-deploy` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `montagu_deploy-0.0.1/pyproject.toml` & `montagu_deploy-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,17 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "constellation",
-  "docopt"
+  "constellation>=1.1.2",
+  "docopt",
+  "psycopg2"
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/montagu-deploy#readme"
 Issues = "https://github.com/unknown/montagu-deploy/issues"
 Source = "https://github.com/unknown/montagu-deploy"
 
@@ -38,16 +39,21 @@
 montagu = "montagu_deploy.cli:main"
 
 [tool.hatch.version]
 path = "src/montagu_deploy/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
+  "celery",
   "coverage[toml]>=6.5",
+  "orderly_web",
   "pytest",
+  "redis",
+  "vault_dev",
+  "YTClient"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `montagu_deploy-0.0.1/PKG-INFO` & `montagu_deploy-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: montagu-deploy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Deploy tool for the Montagu web app
 Project-URL: Documentation, https://github.com/unknown/montagu-deploy#readme
 Project-URL: Issues, https://github.com/unknown/montagu-deploy/issues
 Project-URL: Source, https://github.com/unknown/montagu-deploy
 Author-email: Alex <alex.hill@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,16 +14,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: constellation
+Requires-Dist: constellation>=1.1.2
 Requires-Dist: docopt
+Requires-Dist: psycopg2
 Description-Content-Type: text/markdown
 
 # montagu-deploy
 
 [![PyPI - Version](https://img.shields.io/pypi/v/montagu-deploy.svg)](https://pypi.org/project/montagu-deploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/montagu-deploy.svg)](https://pypi.org/project/montagu-deploy)
 
@@ -69,14 +70,18 @@
 ## Dev requirements
 
 1. [Python3](https://www.python.org/downloads/) (>= 3.7)
 2. [Hatch](https://hatch.pypa.io/latest/install/)
 
 ## Test and lint
 
+For all integration tests to pass, you will need 2 environment variables:
+1. `YOUTRACK_TOKEN` - a token for accessing the YT API
+2. `VAULT_TOKEN` - a github PAT for a user in the vimc robots team.
+
 1. `hatch run test`
 2. `hatch run lint:fmt`
 
 To get coverage reported locally in the console, use `hatch run cov`. 
 On CI, use `hatch run cov-ci` to generate an xml report.
 
 ## Build
@@ -86,12 +91,17 @@
 ```
 
 ## Install from local sources
 
 1. `hatch build`
 2. `pip install dist/montagu_deploy-{version}.tar.gz`
 
+## Publish to PyPi
+
+```console
+hatch publish
+```
 
 ## License
 
 `montagu-deploy` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

