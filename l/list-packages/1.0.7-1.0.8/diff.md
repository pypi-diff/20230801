# Comparing `tmp/list_packages-1.0.7.tar.gz` & `tmp/list_packages-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_packages-1.0.7.tar", last modified: Tue Aug  1 13:54:54 2023, max compression
+gzip compressed data, was "list_packages-1.0.8.tar", last modified: Tue Aug  1 14:23:59 2023, max compression
```

## Comparing `list_packages-1.0.7.tar` & `list_packages-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:54:54.194581 list_packages-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 13:54:45.000000 list_packages-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 13:54:45.000000 list_packages-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 13:54:54.194581 list_packages-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-01 13:54:45.000000 list_packages-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:54:54.194581 list_packages-1.0.7/list_packages/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 13:54:45.000000 list_packages-1.0.7/list_packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 13:54:45.000000 list_packages-1.0.7/list_packages/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:54:54.194581 list_packages-1.0.7/list_packages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:54:54.194581 list_packages-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 13:54:45.000000 list_packages-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:54:54.194581 list_packages-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 13:54:45.000000 list_packages-1.0.7/tests/test_list_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:23:59.559445 list_packages-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 14:23:50.000000 list_packages-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 14:23:50.000000 list_packages-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-01 14:23:59.559445 list_packages-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-01 14:23:50.000000 list_packages-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:23:59.559445 list_packages-1.0.8/list_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 14:23:50.000000 list_packages-1.0.8/list_packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 14:23:50.000000 list_packages-1.0.8/list_packages/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:23:59.559445 list_packages-1.0.8/list_packages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-01 14:23:59.000000 list_packages-1.0.8/list_packages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 14:23:59.000000 list_packages-1.0.8/list_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:23:59.000000 list_packages-1.0.8/list_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 14:23:59.000000 list_packages-1.0.8/list_packages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 14:23:59.000000 list_packages-1.0.8/list_packages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:23:59.559445 list_packages-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 14:23:50.000000 list_packages-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:23:59.559445 list_packages-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 14:23:50.000000 list_packages-1.0.8/tests/test_list_packages.py
```

### Comparing `list_packages-1.0.7/LICENSE` & `list_packages-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.7/PKG-INFO` & `list_packages-1.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list_packages
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package to list all the installed Python packages and their dependencies
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 # list_packages
 
 [![publish](https://github.com/maurya-anand/py-list-packages/actions/workflows/publish-pypi.yml/badge.svg)](https://pypi.org/project/list-packages)
 [![tests](https://github.com/maurya-anand/py-list-packages/actions/workflows/python-package.yml/badge.svg)]()
 
 A utility to retrieve a list of installed Python packages and their dependencies.
 
-- [Documentation](https://py-list-packages.readthedocs.io/)
+- [Technical Details](https://py-list-packages.readthedocs.io/)
 
 - [PyPI](https://pypi.org/project/list-packages)
 
 ## Installation
 
 ``` python
 pip install list-packages
@@ -36,41 +36,24 @@
 
 Alternative:
 
 ``` python
 pip install git+https://github.com/maurya-anand/py-list-packages.git
 ```
 
-## Usage
+## Example usage
 
 ### Terminal
 
 After installing the package, you can run the list-packages command in the terminal to list all installed Python packages and their dependencies:
 
 ``` bash
 list_packages
 ```
 
-### Python Script/Notebook
-
-To use list-packages in a Python notebook, you can import the list_packages module and call the list_installed_packages() function:
-
-``` python
-## import
-from list_packages import list_installed_packages
-```
-
-## Examples
-
-### Terminal
-
-``` bash
-list_packages
-```
-
 Output
 
 ``` bash
 Package                 Dependency
 setuptools==59.6.0      None
 Jinja2==3.1.2           markupsafe>=2.0
 requests==2.31.0        charset-normalizer<4,>=2,certifi>=2017.4.17,urllib3<3,>=1.21.1,idna<4,>=2.5
@@ -80,14 +63,16 @@
 
 ``` bash
 list_packages json
 ```
 
 ### Python script/Notebook
 
+To use list-packages in a Python notebook, you can import the list_packages module and call the list_installed_packages() function.
+
 By default, the function returns a list of dictionaries containing package information. Each dictionary has the following keys:
 
 - package: Package name (str)
 - version: Package version (str)
 - depends: List of dictionaries containing package information (list)
 
 ``` python
@@ -127,7 +112,12 @@
         "package": "markupsafe",
         "version": ">=2.0"
       }
     ]
   }
 ]
 ```
+
+### Links
+
+- [Changelog](./CHANGELOG.md)
+- [License](./LICENSE)
```

### Comparing `list_packages-1.0.7/README.md` & `list_packages-1.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # list_packages
 
 [![publish](https://github.com/maurya-anand/py-list-packages/actions/workflows/publish-pypi.yml/badge.svg)](https://pypi.org/project/list-packages)
 [![tests](https://github.com/maurya-anand/py-list-packages/actions/workflows/python-package.yml/badge.svg)]()
 
 A utility to retrieve a list of installed Python packages and their dependencies.
 
-- [Documentation](https://py-list-packages.readthedocs.io/)
+- [Technical Details](https://py-list-packages.readthedocs.io/)
 
 - [PyPI](https://pypi.org/project/list-packages)
 
 ## Installation
 
 ``` python
 pip install list-packages
@@ -17,41 +17,24 @@
 
 Alternative:
 
 ``` python
 pip install git+https://github.com/maurya-anand/py-list-packages.git
 ```
 
-## Usage
+## Example usage
 
 ### Terminal
 
 After installing the package, you can run the list-packages command in the terminal to list all installed Python packages and their dependencies:
 
 ``` bash
 list_packages
 ```
 
-### Python Script/Notebook
-
-To use list-packages in a Python notebook, you can import the list_packages module and call the list_installed_packages() function:
-
-``` python
-## import
-from list_packages import list_installed_packages
-```
-
-## Examples
-
-### Terminal
-
-``` bash
-list_packages
-```
-
 Output
 
 ``` bash
 Package                 Dependency
 setuptools==59.6.0      None
 Jinja2==3.1.2           markupsafe>=2.0
 requests==2.31.0        charset-normalizer<4,>=2,certifi>=2017.4.17,urllib3<3,>=1.21.1,idna<4,>=2.5
@@ -61,14 +44,16 @@
 
 ``` bash
 list_packages json
 ```
 
 ### Python script/Notebook
 
+To use list-packages in a Python notebook, you can import the list_packages module and call the list_installed_packages() function.
+
 By default, the function returns a list of dictionaries containing package information. Each dictionary has the following keys:
 
 - package: Package name (str)
 - version: Package version (str)
 - depends: List of dictionaries containing package information (list)
 
 ``` python
@@ -108,7 +93,12 @@
         "package": "markupsafe",
         "version": ">=2.0"
       }
     ]
   }
 ]
 ```
+
+### Links
+
+- [Changelog](./CHANGELOG.md)
+- [License](./LICENSE)
```

### Comparing `list_packages-1.0.7/list_packages/main.py` & `list_packages-1.0.8/list_packages/main.py`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.7/list_packages.egg-info/PKG-INFO` & `list_packages-1.0.8/list_packages.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-packages
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package to list all the installed Python packages and their dependencies
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 # list_packages
 
 [![publish](https://github.com/maurya-anand/py-list-packages/actions/workflows/publish-pypi.yml/badge.svg)](https://pypi.org/project/list-packages)
 [![tests](https://github.com/maurya-anand/py-list-packages/actions/workflows/python-package.yml/badge.svg)]()
 
 A utility to retrieve a list of installed Python packages and their dependencies.
 
-- [Documentation](https://py-list-packages.readthedocs.io/)
+- [Technical Details](https://py-list-packages.readthedocs.io/)
 
 - [PyPI](https://pypi.org/project/list-packages)
 
 ## Installation
 
 ``` python
 pip install list-packages
@@ -36,41 +36,24 @@
 
 Alternative:
 
 ``` python
 pip install git+https://github.com/maurya-anand/py-list-packages.git
 ```
 
-## Usage
+## Example usage
 
 ### Terminal
 
 After installing the package, you can run the list-packages command in the terminal to list all installed Python packages and their dependencies:
 
 ``` bash
 list_packages
 ```
 
-### Python Script/Notebook
-
-To use list-packages in a Python notebook, you can import the list_packages module and call the list_installed_packages() function:
-
-``` python
-## import
-from list_packages import list_installed_packages
-```
-
-## Examples
-
-### Terminal
-
-``` bash
-list_packages
-```
-
 Output
 
 ``` bash
 Package                 Dependency
 setuptools==59.6.0      None
 Jinja2==3.1.2           markupsafe>=2.0
 requests==2.31.0        charset-normalizer<4,>=2,certifi>=2017.4.17,urllib3<3,>=1.21.1,idna<4,>=2.5
@@ -80,14 +63,16 @@
 
 ``` bash
 list_packages json
 ```
 
 ### Python script/Notebook
 
+To use list-packages in a Python notebook, you can import the list_packages module and call the list_installed_packages() function.
+
 By default, the function returns a list of dictionaries containing package information. Each dictionary has the following keys:
 
 - package: Package name (str)
 - version: Package version (str)
 - depends: List of dictionaries containing package information (list)
 
 ``` python
@@ -127,7 +112,12 @@
         "package": "markupsafe",
         "version": ">=2.0"
       }
     ]
   }
 ]
 ```
+
+### Links
+
+- [Changelog](./CHANGELOG.md)
+- [License](./LICENSE)
```

### Comparing `list_packages-1.0.7/setup.py` & `list_packages-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='list_packages',
-    version='1.0.7',
+    version='1.0.8',
     description='A package to list all the installed Python packages and their dependencies',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Anand Maurya',
     author_email='anandmaurya@hotmail.com',
     platforms=['Any'],
     packages=find_packages(),
```

### Comparing `list_packages-1.0.7/tests/test_list_packages.py` & `list_packages-1.0.8/tests/test_list_packages.py`

 * *Files identical despite different names*

