# Comparing `tmp/selenium_axe_python-2.1.12.tar.gz` & `tmp/selenium_axe_python-2.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_axe_python-2.1.12.tar", max compression
+gzip compressed data, was "selenium_axe_python-2.1.13.tar", max compression
```

## Comparing `selenium_axe_python-2.1.12.tar` & `selenium_axe_python-2.1.13.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    16725 2023-08-01 17:36:19.940023 selenium_axe_python-2.1.12/LICENSE.txt
--rwxr-xr-x   0        0        0     6892 2023-08-01 17:36:19.940023 selenium_axe_python-2.1.12/README.md
--rw-r--r--   0        0        0     5318 2023-08-01 17:36:19.944023 selenium_axe_python-2.1.12/pyproject.toml
--rw-r--r--   0        0        0      255 2023-08-01 17:36:19.944023 selenium_axe_python-2.1.12/selenium_axe_python/__init__.py
--rw-r--r--   0        0        0   519419 2023-08-01 17:36:19.944023 selenium_axe_python-2.1.12/selenium_axe_python/axe-core/axe.min.js
--rwxr-xr-x   0        0        0     3899 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/axe.py
--rw-r--r--   0        0        0      199 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/__init__.py
--rw-r--r--   0        0        0     1124 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/conftest.py
--rw-r--r--   0        0        0     2318 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/pytest.ini
--rwxr-xr-x   0        0        0    13523 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/test_axe.py
--rw-r--r--   0        0        0      379 2023-08-01 17:36:19.948023 selenium_axe_python-2.1.12/selenium_axe_python/tests/test_page.html
--rw-r--r--   0        0        0     8612 1970-01-01 00:00:00.000000 selenium_axe_python-2.1.12/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-08-01 20:54:52.025870 selenium_axe_python-2.1.13/LICENSE.txt
+-rwxr-xr-x   0        0        0     6928 2023-08-01 20:54:52.025870 selenium_axe_python-2.1.13/README.md
+-rw-r--r--   0        0        0     5282 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/pyproject.toml
+-rw-r--r--   0        0        0      255 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/selenium_axe_python/__init__.py
+-rw-r--r--   0        0        0   519419 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/selenium_axe_python/axe-core/axe.min.js
+-rwxr-xr-x   0        0        0     3899 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/selenium_axe_python/axe.py
+-rw-r--r--   0        0        0      199 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/selenium_axe_python/tests/__init__.py
+-rw-r--r--   0        0        0     1124 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/selenium_axe_python/tests/conftest.py
+-rw-r--r--   0        0        0     2318 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/selenium_axe_python/tests/pytest.ini
+-rwxr-xr-x   0        0        0    13523 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/selenium_axe_python/tests/test_axe.py
+-rw-r--r--   0        0        0      379 2023-08-01 20:54:52.029870 selenium_axe_python-2.1.13/selenium_axe_python/tests/test_page.html
+-rw-r--r--   0        0        0     8618 1970-01-01 00:00:00.000000 selenium_axe_python-2.1.13/PKG-INFO
```

### Comparing `selenium_axe_python-2.1.12/LICENSE.txt` & `selenium_axe_python-2.1.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.12/README.md` & `selenium_axe_python-2.1.13/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 selenium-axe-python integrates aXe and selenium to enable automated web accessibility testing.
 
 Originally created as [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/) by [Kimberly Sereduck](https://github.com/kimberlythegeek).
 Unfortunately she is no longer assigned to the project which means the original project has gone stale.
 This is a fork of that project with some updates.
 
-**This version of selenium-axe-python is using axe-core@4.7.2.**
+**This version of selenium-axe-python is using axe-core@4.7.2**
+
 
 [![License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://github.com/bandophahita/selenium-axe-python/blob/master/LICENSE.txt)
 [![PyPI](https://img.shields.io/pypi/v/selenium-axe-python.svg)](https://pypi.org/project/selenium-axe-python/)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/screenpy.svg)](https://pypi.org/project/screenpy)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -55,15 +56,15 @@
     driver = webdriver.Firefox()
     driver.get("http://www.google.com")
     axe = Axe(driver)
     # Inject axe-core javascript into page.
     axe.inject()
     # Run axe accessibility checks.
     results = axe.run()
-    # Write results to file
+    # Write results to jsfile
     axe.write_results(results, 'a11y.json')
     driver.close()
     # Assert no violations are found
     assert len(results["violations"]) == 0, axe.report(results["violations"])
 ```
 
 The method `axe.run()` accepts two parameters: `context` and `options`.
@@ -111,14 +112,15 @@
 CHANGELOG
 ---------
 
 ## version 2.1.12
 
 - forked from original repo [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/)
 - updated to work with python >=3.7
+- Updated axe to `axe-core@4.7.2`
 
 
 ### version 2.1.5
 
 **Breaks backwards compatibility**:
 
 - The Axe class method `execute` has been renamed to `run` to mirror the method in the axe-core API.
```

### Comparing `selenium_axe_python-2.1.12/pyproject.toml` & `selenium_axe_python-2.1.13/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 # Poetry:
 #   poetry install --extras dev
 # PIP:
 #   pip install -e .[dev]
 
 [tool.poetry]
 name = "selenium-axe-python"
-version = "2.1.12"
+version = "2.1.13"
 description = "Python library to integrate axe and selenium for web accessibility testing."
-authors = ["Kimberly Sereduck"]
-maintainers = ["Marcel Wilson"]
+authors = ["Marcel Wilson"]
 license = "Mozilla Public License 2.0 (MPL 2.0)"
 repository = "https://github.com/bandophahita/selenium-axe-python"
 #documentation = ""
 readme = "README.md"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `selenium_axe_python-2.1.12/selenium_axe_python/axe-core/axe.min.js` & `selenium_axe_python-2.1.13/selenium_axe_python/axe-core/axe.min.js`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.12/selenium_axe_python/axe.py` & `selenium_axe_python-2.1.13/selenium_axe_python/axe.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.12/selenium_axe_python/tests/conftest.py` & `selenium_axe_python-2.1.13/selenium_axe_python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.12/selenium_axe_python/tests/pytest.ini` & `selenium_axe_python-2.1.13/selenium_axe_python/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.12/selenium_axe_python/tests/test_axe.py` & `selenium_axe_python-2.1.13/selenium_axe_python/tests/test_axe.py`

 * *Files identical despite different names*

### Comparing `selenium_axe_python-2.1.12/PKG-INFO` & `selenium_axe_python-2.1.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: selenium-axe-python
-Version: 2.1.12
+Version: 2.1.13
 Summary: Python library to integrate axe and selenium for web accessibility testing.
 Home-page: https://github.com/bandophahita/selenium-axe-python
 License: Mozilla Public License 2.0 (MPL 2.0)
-Author: Kimberly Sereduck
-Maintainer: Marcel Wilson
+Author: Marcel Wilson
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -43,15 +42,16 @@
 
 selenium-axe-python integrates aXe and selenium to enable automated web accessibility testing.
 
 Originally created as [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/) by [Kimberly Sereduck](https://github.com/kimberlythegeek).
 Unfortunately she is no longer assigned to the project which means the original project has gone stale.
 This is a fork of that project with some updates.
 
-**This version of selenium-axe-python is using axe-core@4.7.2.**
+**This version of selenium-axe-python is using axe-core@4.7.2**
+
 
 [![License](https://img.shields.io/badge/license-MPL%202.0-blue.svg)](https://github.com/bandophahita/selenium-axe-python/blob/master/LICENSE.txt)
 [![PyPI](https://img.shields.io/pypi/v/selenium-axe-python.svg)](https://pypi.org/project/selenium-axe-python/)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/screenpy.svg)](https://pypi.org/project/screenpy)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -95,15 +95,15 @@
     driver = webdriver.Firefox()
     driver.get("http://www.google.com")
     axe = Axe(driver)
     # Inject axe-core javascript into page.
     axe.inject()
     # Run axe accessibility checks.
     results = axe.run()
-    # Write results to file
+    # Write results to jsfile
     axe.write_results(results, 'a11y.json')
     driver.close()
     # Assert no violations are found
     assert len(results["violations"]) == 0, axe.report(results["violations"])
 ```
 
 The method `axe.run()` accepts two parameters: `context` and `options`.
@@ -151,14 +151,15 @@
 CHANGELOG
 ---------
 
 ## version 2.1.12
 
 - forked from original repo [axe-selenium-python](http://github.com/mozilla-services/axe-selenium-python/)
 - updated to work with python >=3.7
+- Updated axe to `axe-core@4.7.2`
 
 
 ### version 2.1.5
 
 **Breaks backwards compatibility**:
 
 - The Axe class method `execute` has been renamed to `run` to mirror the method in the axe-core API.
```

