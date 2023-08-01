# Comparing `tmp/aws-step-functions-pydantic-0.0.2.tar.gz` & `tmp/aws-step-functions-pydantic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-step-functions-pydantic-0.0.2.tar", last modified: Tue Aug  1 15:22:06 2023, max compression
+gzip compressed data, was "aws-step-functions-pydantic-0.0.3.tar", last modified: Tue Aug  1 15:29:10 2023, max compression
```

## Comparing `aws-step-functions-pydantic-0.0.2.tar` & `aws-step-functions-pydantic-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.436711 aws-step-functions-pydantic-0.0.2/.github/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3226 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/.github/CONTRIBUTING.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.436711 aws-step-functions-pydantic-0.0.2/.github/workflows/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3587 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/.github/workflows/master.yml
--rw-rw-r--   0 louis     (1000) louis     (1000)      203 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/.gitignore
--rw-rw-r--   0 louis     (1000) louis     (1000)      749 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 louis     (1000) louis     (1000)      327 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/.readthedocs.yml
--rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)     2899 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)     1692 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)      187 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/codecov.yml
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.436711 aws-step-functions-pydantic-0.0.2/codegen/
--rwxrwxr-x   0 louis     (1000) louis     (1000)     1060 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/codegen/generate_pydantic_models.sh
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/docs/
--rw-rw-r--   0 louis     (1000) louis     (1000)      634 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/docs/Makefile
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.436711 aws-step-functions-pydantic-0.0.2/docs/_static/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/docs/_static/css/
--rw-rw-r--   0 louis     (1000) louis     (1000)       70 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/docs/_static/css/style.css
--rw-rw-r--   0 louis     (1000) louis     (1000)      122 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/docs/api.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)     3799 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/docs/conf.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      485 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/docs/index.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)      795 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/docs/make.bat
--rw-rw-r--   0 louis     (1000) louis     (1000)      354 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/mypy.ini
--rw-rw-r--   0 louis     (1000) louis     (1000)      355 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/pyproject.toml
--rw-rw-r--   0 louis     (1000) louis     (1000)       25 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/requirements-generate.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       19 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     3155 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/setup.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.436711 aws-step-functions-pydantic-0.0.2/src/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/
--rw-rw-r--   0 louis     (1000) louis     (1000)      471 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/__init__.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/api/
--rw-rw-r--   0 louis     (1000) louis     (1000)       58 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/api/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      510 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/api/define.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      919 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/api/sfn.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/generated/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/generated/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    10298 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/generated/base_state_machine.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/utils/
--rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/utils/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      113 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/utils/boto.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     2899 2023-08-01 15:22:06.000000 aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)     1056 2023-08-01 15:22:06.000000 aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-08-01 15:22:06.000000 aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-08-01 15:22:06.000000 aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      227 2023-08-01 15:22:06.000000 aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       17 2023-08-01 15:22:06.000000 aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/tests/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/tests/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      108 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/tests/core_test.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.436711 aws-step-functions-pydantic-0.0.2/tools/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:22:06.440711 aws-step-functions-pydantic-0.0.2/tools/github/
--rw-rw-r--   0 louis     (1000) louis     (1000)      353 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/tools/github/install_miniconda.sh
--rw-rw-r--   0 louis     (1000) louis     (1000)     1194 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.2/tox.ini
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/.github/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3226 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.github/CONTRIBUTING.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/.github/workflows/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3587 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.github/workflows/master.yml
+-rw-rw-r--   0 louis     (1000) louis     (1000)      203 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.gitignore
+-rw-rw-r--   0 louis     (1000) louis     (1000)      749 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.pre-commit-config.yaml
+-rw-rw-r--   0 louis     (1000) louis     (1000)      327 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.readthedocs.yml
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2899 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1692 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)      187 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/codecov.yml
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/codegen/
+-rwxrwxr-x   0 louis     (1000) louis     (1000)     1060 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/codegen/generate_pydantic_models.sh
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/docs/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      634 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/Makefile
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.445027 aws-step-functions-pydantic-0.0.3/docs/_static/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/docs/_static/css/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       70 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/_static/css/style.css
+-rw-rw-r--   0 louis     (1000) louis     (1000)      122 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/api.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3799 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/conf.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      485 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/index.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)      795 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/make.bat
+-rw-rw-r--   0 louis     (1000) louis     (1000)      354 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/mypy.ini
+-rw-rw-r--   0 louis     (1000) louis     (1000)      355 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/pyproject.toml
+-rw-rw-r--   0 louis     (1000) louis     (1000)       25 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/requirements-generate.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       19 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3155 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.445027 aws-step-functions-pydantic-0.0.3/src/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      471 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/__init__.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       58 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      510 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/define.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      916 2023-08-01 15:28:39.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/sfn.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/generated/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/generated/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    10298 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/generated/base_state_machine.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/utils/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/utils/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      113 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/utils/boto.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2899 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1056 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      227 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       17 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/tests/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/tests/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      108 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/tests/core_test.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.445027 aws-step-functions-pydantic-0.0.3/tools/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/tools/github/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      353 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/tools/github/install_miniconda.sh
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1194 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/tox.ini
```

### Comparing `aws-step-functions-pydantic-0.0.2/.github/CONTRIBUTING.md` & `aws-step-functions-pydantic-0.0.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/.github/workflows/master.yml` & `aws-step-functions-pydantic-0.0.3/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/.pre-commit-config.yaml` & `aws-step-functions-pydantic-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/LICENSE` & `aws-step-functions-pydantic-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/PKG-INFO` & `aws-step-functions-pydantic-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-step-functions-pydantic
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pydantic models for AWS step functions
 Home-page: https://github.com/lmmx/aws-step-functions-pydantic
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
```

### Comparing `aws-step-functions-pydantic-0.0.2/README.md` & `aws-step-functions-pydantic-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/codegen/generate_pydantic_models.sh` & `aws-step-functions-pydantic-0.0.3/codegen/generate_pydantic_models.sh`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/docs/Makefile` & `aws-step-functions-pydantic-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/docs/conf.py` & `aws-step-functions-pydantic-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/docs/make.bat` & `aws-step-functions-pydantic-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/setup.py` & `aws-step-functions-pydantic-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/api/sfn.py` & `aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/sfn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from textwrap import indent
+import textwrap
 
 import yaml
 
 from ..generated.base_state_machine import StateMachine as BaseStateMachine
 from .define import get_sfn_defn
 
 __all__ = ["StateMachine"]
@@ -22,8 +22,8 @@
 
         - `indent` can be 2, 4, or 8. (default: 2)
         - `level` how many levels of indentation to prefix each line by (default: 0).
         """
         sfn = self.model_dump(exclude_unset=True)
         prefix = " " * indent * level
         yml = yaml.dump(sfn, indent=indent, sort_keys=False)
-        return indent(yml, prefix=prefix)
+        return textwrap.indent(yml, prefix=prefix)
```

### Comparing `aws-step-functions-pydantic-0.0.2/src/aws_sfn_pydantic/generated/base_state_machine.py` & `aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/generated/base_state_machine.py`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/PKG-INFO` & `aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-step-functions-pydantic
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pydantic models for AWS step functions
 Home-page: https://github.com/lmmx/aws-step-functions-pydantic
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
```

### Comparing `aws-step-functions-pydantic-0.0.2/src/aws_step_functions_pydantic.egg-info/SOURCES.txt` & `aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.2/tox.ini` & `aws-step-functions-pydantic-0.0.3/tox.ini`

 * *Files identical despite different names*

