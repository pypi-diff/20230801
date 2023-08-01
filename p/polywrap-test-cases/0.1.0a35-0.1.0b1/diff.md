# Comparing `tmp/polywrap_test_cases-0.1.0a35.tar.gz` & `tmp/polywrap_test_cases-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_test_cases-0.1.0a35.tar", max compression
+gzip compressed data, was "polywrap_test_cases-0.1.0b1.tar", max compression
```

## Comparing `polywrap_test_cases-0.1.0a35.tar` & `polywrap_test_cases-0.1.0b1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       96 2023-06-28 13:05:20.152194 polywrap_test_cases-0.1.0a35/README.md
--rw-r--r--   0        0        0     1257 2023-06-28 13:05:20.152194 polywrap_test_cases-0.1.0a35/polywrap_test_cases/__init__.py
--rw-r--r--   0        0        0      142 2023-06-28 13:05:20.152194 polywrap_test_cases-0.1.0a35/polywrap_test_cases/__main__.py
--rw-r--r--   0        0        0        0 2023-06-28 13:05:20.152194 polywrap_test_cases-0.1.0a35/polywrap_test_cases/py.typed
--rw-r--r--   0        0        0      991 2023-06-28 13:06:52.061022 polywrap_test_cases-0.1.0a35/pyproject.toml
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 polywrap_test_cases-0.1.0a35/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-08-01 17:46:03.395536 polywrap_test_cases-0.1.0b1/README.md
+-rw-r--r--   0        0        0     1257 2023-08-01 17:46:03.395536 polywrap_test_cases-0.1.0b1/polywrap_test_cases/__init__.py
+-rw-r--r--   0        0        0      142 2023-08-01 17:46:03.395536 polywrap_test_cases-0.1.0b1/polywrap_test_cases/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:46:03.395536 polywrap_test_cases-0.1.0b1/polywrap_test_cases/py.typed
+-rw-r--r--   0        0        0      941 2023-08-01 17:49:08.772872 polywrap_test_cases-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 polywrap_test_cases-0.1.0b1/PKG-INFO
```

### Comparing `polywrap_test_cases-0.1.0a35/polywrap_test_cases/__init__.py` & `polywrap_test_cases-0.1.0b1/polywrap_test_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_test_cases-0.1.0a35/pyproject.toml` & `polywrap_test_cases-0.1.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-test-cases"
-version = "0.1.0a35"
+version = "0.1.0b1"
 description = "Plugin package"
 authors = ["Cesar <cesar@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
-pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
@@ -35,15 +34,14 @@
 target-version = ["py310"]
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportShadowedImports = false
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
 
 [tool.pylint]
 disable = [
 ]
```

