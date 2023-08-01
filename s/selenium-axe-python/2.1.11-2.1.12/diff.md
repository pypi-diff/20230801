# Comparing `tmp/selenium_axe_python-2.1.11.tar.gz` & `tmp/selenium_axe_python-2.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_axe_python-2.1.11.tar", max compression
+gzip compressed data, was "selenium_axe_python-2.1.12.tar", max compression
```

## Comparing `selenium_axe_python-2.1.11.tar` & `selenium_axe_python-2.1.12.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0    16725 2023-07-28 14:37:27.211201 selenium_axe_python-2.1.11/LICENSE.txt
--rwxr-xr-x   0        0        0     5921 2023-08-01 15:47:06.671577 selenium_axe_python-2.1.11/README.md
--rw-r--r--   0        0        0     5318 2023-08-01 16:25:03.997193 selenium_axe_python-2.1.11/pyproject.toml
--rw-r--r--   0        0        0      255 2023-08-01 15:47:06.676738 selenium_axe_python-2.1.11/selenium_axe_python/__init__.py
--rw-r--r--   0        0        0   519419 2023-08-01 15:47:06.678705 selenium_axe_python-2.1.11/selenium_axe_python/axe-core/axe.min.js
--rwxr-xr-x   0        0        0     3899 2023-08-01 15:47:06.679227 selenium_axe_python-2.1.11/selenium_axe_python/axe.py
--rw-r--r--   0        0        0      372 2023-08-01 15:47:06.679563 selenium_axe_python-2.1.11/selenium_axe_python/package-lock.json
--rw-r--r--   0        0        0      606 2023-08-01 15:47:06.679626 selenium_axe_python-2.1.11/selenium_axe_python/package.json
--rw-r--r--   0        0        0      199 2023-08-01 15:47:06.679699 selenium_axe_python-2.1.11/selenium_axe_python/tests/__init__.py
--rw-r--r--   0        0        0     1124 2023-08-01 15:47:06.679980 selenium_axe_python-2.1.11/selenium_axe_python/tests/conftest.py
--rw-r--r--   0        0        0     2299 2023-08-01 15:47:06.680227 selenium_axe_python-2.1.11/selenium_axe_python/tests/pytest.ini
--rwxr-xr-x   0        0        0    13523 2023-08-01 15:47:06.680509 selenium_axe_python-2.1.11/selenium_axe_python/tests/test_axe.py
--rw-r--r--   0        0        0      379 2023-08-01 15:47:06.680570 selenium_axe_python-2.1.11/selenium_axe_python/tests/test_page.html
--rw-r--r--   0        0        0     7641 1970-01-01 00:00:00.000000 selenium_axe_python-2.1.11/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-08-01 17:36:19.940023 selenium_axe_python-2.1.12/LICENSE.txt
+-rwxr-xr-x   0        0        0     6892 2023-08-01 17:36:19.940023 selenium_axe_python-2.1.12/README.md
+-rw-r--r--   0        0        0     5318 2023-08-01 17:36:19.944023 selenium_axe_python-2.1.12/pyproject.toml
+-rw-r--r--   0        0        0      255 2023-08-01 17:36:19.944023 selenium_axe_python-2.1.12/selenium_axe_python/__init__.py
+-rw-r--r--   0        0        0   519419 2023-08-01 17:36:19.944023 selenium_axe_python-2.1.12/selenium_axe_python/axe-core/axe.min.js
+-rwxr-xr-x   0        0        0     3899 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/axe.py
+-rw-r--r--   0        0        0      199 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/__init__.py
+-rw-r--r--   0        0        0     1124 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/conftest.py
+-rw-r--r--   0        0        0     2318 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/pytest.ini
+-rwxr-xr-x   0        0        0    13523 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/test_axe.py
+-rw-r--r--   0        0        0      379 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/test_page.html
+-rw-r--r--   0        0        0     8612 1970-01-01 00:00:00.000000 selenium_axe_python-2.1.12/PKG-INFO
```

### Comparing `selenium_axe_python-2.1.11/LICENSE.txt` & `selenium_axe_python-2.1.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.11/README.md` & `selenium_axe_python-2.1.12/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 selenium-axe-python
 ===================
 
 selenium-axe-python integrates aXe and selenium to enable automated web accessibility testing.
 
-Originally created as [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/) by [Kimberly Sereduck](https://github.com/kimberlythegeek)
+Originally created as [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/) by [Kimberly Sereduck](https://github.com/kimberlythegeek).
 Unfortunately she is no longer assigned to the project which means the original project has gone stale.
-This is basically a fork of that project with some updates.
+This is a fork of that project with some updates.
 
 **This version of selenium-axe-python is using axe-core@4.7.2.**
 
-[![License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://github.com/mozilla-services/axe-selenium-python/blob/master/LICENSE.txt)
-[![PyPI](https://img.shields.io/pypi/v/axe-selenium-python.svg)](https://pypi.org/project/axe-selenium-python/)
-[![Travis](https://img.shields.io/travis/mozilla-services/axe-selenium-python.svg)](https://travis-ci.org/mozilla-services/axe-selenium-python)
+[![License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://github.com/bandophahita/selenium-axe-python/blob/master/LICENSE.txt)
+[![PyPI](https://img.shields.io/pypi/v/selenium-axe-python.svg)](https://pypi.org/project/selenium-axe-python/)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/screenpy.svg)](https://pypi.org/project/screenpy)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
 [![Issues](https://img.shields.io/github/issues-raw/bandophahita/selenium-axe-python.svg)](https://github.com/bandophahita/selenium-axe-python/issues)
 
+[![Build Status](https://github.com/bandophahita/selenium-axe-python/actions/workflows/tests.yml/badge.svg)](https://github.com/bandophahita/selenium-axe-python/actions/workflows/tests.yml)
+[![Build Status](https://github.com/bandophahita/selenium-axe-python/actions/workflows/lint.yml/badge.svg)](https://github.com/bandophahita/selenium-axe-python/actions/workflows/lint.yml)
 
 Requirements
 ------------
 
 You will need the following prerequisites in order to use selenium-axe-python:
 
 - selenium >= 3.0.2
@@ -28,16 +35,15 @@
 
 Installation
 ------------
 
 To install selenium-axe-python:
 
 ```bash
-$ pip install git+https://github.com/bandophahita/selenium-axe-python
-              git+ssh://git@github.com/bandophahita/selenium-axe-python.git@master
+$ pip install selenium-axe-python
 ```
 
 Usage
 -----
 
 ```python
 
@@ -63,40 +69,53 @@
 The method `axe.run()` accepts two parameters: `context` and `options`.
 
 For more information on `context` and `options`, view the [aXe documentation here](https://github.com/dequelabs/axe-core/blob/master/doc/API.md#parameters-axerun).
 
 Contributing
 ------------
 
-Fork the repository and submit PRs with bug fixes and enhancements;
-contributions are very welcome.
+You want to contribute? Great! Here are the things you should do before submitting your PR:
+
+
+1. Fork the repo and git clone your fork.
+1. `dev` install the project package:
+    1. `pip install -e .[dev]`
+    1. Optional (poetry users):
+        1. `poetry install --extras dev`
+1. Run `tox` to perform tests frequently.
+1. Create pull-request from your branch.
 
-~~Node dependencies must be installed by running `npm install` inside the selenium-axe-python directory~~
 
 The original project required you to run `npm install` (or in most cases did it at install for you) but this
 limited the use of the package to systems that have npm.  This fork includes the latest version of
 axe-core.
 
 You can run the tests using [tox](https://tox.readthedocs.io/en/latest/):
 
 ```bash
 $ tox
 ```
 
+Alternatively you can use the makefile in the root of the repo:
+
+```bash
+$ make pre-check-in
+```
+
 Resources
 ---------
 
 - [Issue Tracker](https://github.com/bandophahita/selenium-axe-python/issues)
 - [Code](https://github.com/bandophahita/selenium-axe-python/)
 - [pytest-axe](http://github.com/mozilla-services/pytest-axe/)
 
 CHANGELOG
 ---------
 
-## version 2.1.7
+## version 2.1.12
 
 - forked from original repo [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/)
 - updated to work with python >=3.7
 
 
 ### version 2.1.5
```

### Comparing `selenium_axe_python-2.1.11/pyproject.toml` & `selenium_axe_python-2.1.12/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Poetry:
 #   poetry install --extras dev
 # PIP:
 #   pip install -e .[dev]
 
 [tool.poetry]
 name = "selenium-axe-python"
-version = "2.1.11"
+version = "2.1.12"
 description = "Python library to integrate axe and selenium for web accessibility testing."
 authors = ["Kimberly Sereduck"]
 maintainers = ["Marcel Wilson"]
 license = "Mozilla Public License 2.0 (MPL 2.0)"
 repository = "https://github.com/bandophahita/selenium-axe-python"
 #documentation = ""
 readme = "README.md"
```

### Comparing `selenium_axe_python-2.1.11/selenium_axe_python/axe-core/axe.min.js` & `selenium_axe_python-2.1.12/selenium_axe_python/axe-core/axe.min.js`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.11/selenium_axe_python/axe.py` & `selenium_axe_python-2.1.12/selenium_axe_python/axe.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.11/selenium_axe_python/tests/conftest.py` & `selenium_axe_python-2.1.12/selenium_axe_python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.11/selenium_axe_python/tests/pytest.ini` & `selenium_axe_python-2.1.12/selenium_axe_python/tests/pytest.ini`

 * *Files 2% similar despite different names*

```diff
@@ -55,9 +55,10 @@
 ; verbosity 0 makes the mini results (i.e. the period or s) appear for each test
 ; I haven't figured out a way to disable that.
 ; verbosity 1 makes the mini result show PASSED/FAILED/SKIPPED
 
 
 markers = 
     xpass: Neato freato xpassing
+    nondestructive
```

### Comparing `selenium_axe_python-2.1.11/selenium_axe_python/tests/test_axe.py` & `selenium_axe_python-2.1.12/selenium_axe_python/tests/test_axe.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.11/PKG-INFO` & `selenium_axe_python-2.1.12/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-axe-python
-Version: 2.1.11
+Version: 2.1.12
 Summary: Python library to integrate axe and selenium for web accessibility testing.
 Home-page: https://github.com/bandophahita/selenium-axe-python
 License: Mozilla Public License 2.0 (MPL 2.0)
 Author: Kimberly Sereduck
 Maintainer: Marcel Wilson
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -39,25 +39,32 @@
 Description-Content-Type: text/markdown
 
 selenium-axe-python
 ===================
 
 selenium-axe-python integrates aXe and selenium to enable automated web accessibility testing.
 
-Originally created as [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/) by [Kimberly Sereduck](https://github.com/kimberlythegeek)
+Originally created as [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/) by [Kimberly Sereduck](https://github.com/kimberlythegeek).
 Unfortunately she is no longer assigned to the project which means the original project has gone stale.
-This is basically a fork of that project with some updates.
+This is a fork of that project with some updates.
 
 **This version of selenium-axe-python is using axe-core@4.7.2.**
 
-[![License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://github.com/mozilla-services/axe-selenium-python/blob/master/LICENSE.txt)
-[![PyPI](https://img.shields.io/pypi/v/axe-selenium-python.svg)](https://pypi.org/project/axe-selenium-python/)
-[![Travis](https://img.shields.io/travis/mozilla-services/axe-selenium-python.svg)](https://travis-ci.org/mozilla-services/axe-selenium-python)
+[![License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://github.com/bandophahita/selenium-axe-python/blob/master/LICENSE.txt)
+[![PyPI](https://img.shields.io/pypi/v/selenium-axe-python.svg)](https://pypi.org/project/selenium-axe-python/)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/screenpy.svg)](https://pypi.org/project/screenpy)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
 [![Issues](https://img.shields.io/github/issues-raw/bandophahita/selenium-axe-python.svg)](https://github.com/bandophahita/selenium-axe-python/issues)
 
+[![Build Status](https://github.com/bandophahita/selenium-axe-python/actions/workflows/tests.yml/badge.svg)](https://github.com/bandophahita/selenium-axe-python/actions/workflows/tests.yml)
+[![Build Status](https://github.com/bandophahita/selenium-axe-python/actions/workflows/lint.yml/badge.svg)](https://github.com/bandophahita/selenium-axe-python/actions/workflows/lint.yml)
 
 Requirements
 ------------
 
 You will need the following prerequisites in order to use selenium-axe-python:
 
 - selenium >= 3.0.2
@@ -68,16 +75,15 @@
 
 Installation
 ------------
 
 To install selenium-axe-python:
 
 ```bash
-$ pip install git+https://github.com/bandophahita/selenium-axe-python
-              git+ssh://git@github.com/bandophahita/selenium-axe-python.git@master
+$ pip install selenium-axe-python
 ```
 
 Usage
 -----
 
 ```python
 
@@ -103,40 +109,53 @@
 The method `axe.run()` accepts two parameters: `context` and `options`.
 
 For more information on `context` and `options`, view the [aXe documentation here](https://github.com/dequelabs/axe-core/blob/master/doc/API.md#parameters-axerun).
 
 Contributing
 ------------
 
-Fork the repository and submit PRs with bug fixes and enhancements;
-contributions are very welcome.
+You want to contribute? Great! Here are the things you should do before submitting your PR:
+
+
+1. Fork the repo and git clone your fork.
+1. `dev` install the project package:
+    1. `pip install -e .[dev]`
+    1. Optional (poetry users):
+        1. `poetry install --extras dev`
+1. Run `tox` to perform tests frequently.
+1. Create pull-request from your branch.
 
-~~Node dependencies must be installed by running `npm install` inside the selenium-axe-python directory~~
 
 The original project required you to run `npm install` (or in most cases did it at install for you) but this
 limited the use of the package to systems that have npm.  This fork includes the latest version of
 axe-core.
 
 You can run the tests using [tox](https://tox.readthedocs.io/en/latest/):
 
 ```bash
 $ tox
 ```
 
+Alternatively you can use the makefile in the root of the repo:
+
+```bash
+$ make pre-check-in
+```
+
 Resources
 ---------
 
 - [Issue Tracker](https://github.com/bandophahita/selenium-axe-python/issues)
 - [Code](https://github.com/bandophahita/selenium-axe-python/)
 - [pytest-axe](http://github.com/mozilla-services/pytest-axe/)
 
 CHANGELOG
 ---------
 
-## version 2.1.7
+## version 2.1.12
 
 - forked from original repo [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/)
 - updated to work with python >=3.7
 
 
 ### version 2.1.5
```

