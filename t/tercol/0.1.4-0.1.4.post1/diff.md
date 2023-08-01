# Comparing `tmp/tercol-0.1.4.tar.gz` & `tmp/tercol-0.1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tercol-0.1.4.tar", last modified: Sat Jun  3 23:52:20 2023, max compression
+gzip compressed data, was "tercol-0.1.4.post1.tar", last modified: Tue Aug  1 19:37:45 2023, max compression
```

## Comparing `tercol-0.1.4.tar` & `tercol-0.1.4.post1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 23:52:20.534211 tercol-0.1.4/
--rw-rw-rw-   0        0        0     1094 2023-06-03 22:41:35.000000 tercol-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       25 2023-06-01 22:00:38.000000 tercol-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1837 2023-06-03 23:52:20.534211 tercol-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-06-03 23:44:17.000000 tercol-0.1.4/README.md
--rw-rw-rw-   0        0        0      817 2023-06-03 22:46:49.000000 tercol-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 23:52:20.534211 tercol-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-03 23:52:20.528228 tercol-0.1.4/tercol/
--rw-rw-rw-   0        0        0    12136 2023-06-03 22:52:59.000000 tercol-0.1.4/tercol/__init__.py
--rw-rw-rw-   0        0        0      886 2023-06-03 23:51:18.000000 tercol-0.1.4/tercol/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 23:52:20.533213 tercol-0.1.4/tercol.egg-info/
--rw-rw-rw-   0        0        0     1837 2023-06-03 23:52:20.000000 tercol-0.1.4/tercol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-03 23:52:20.000000 tercol-0.1.4/tercol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 23:52:20.000000 tercol-0.1.4/tercol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-03 23:52:20.000000 tercol-0.1.4/tercol.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 19:37:45.024895 tercol-0.1.4.post1/
+-rw-rw-rw-   0        0        0     1094 2023-06-04 00:43:29.000000 tercol-0.1.4.post1/LICENSE
+-rw-rw-rw-   0        0        0     1832 2023-08-01 19:37:45.023898 tercol-0.1.4.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-08-01 19:23:28.000000 tercol-0.1.4.post1/README.md
+-rw-rw-rw-   0        0        0      815 2023-08-01 19:35:55.000000 tercol-0.1.4.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 19:37:45.024895 tercol-0.1.4.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 19:37:45.016917 tercol-0.1.4.post1/tercol/
+-rw-rw-rw-   0        0        0    12136 2023-06-04 00:43:29.000000 tercol-0.1.4.post1/tercol/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-06-04 00:43:29.000000 tercol-0.1.4.post1/tercol/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:37:45.021903 tercol-0.1.4.post1/tercol.egg-info/
+-rw-rw-rw-   0        0        0     1832 2023-08-01 19:37:44.000000 tercol-0.1.4.post1/tercol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-08-01 19:37:45.000000 tercol-0.1.4.post1/tercol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 19:37:44.000000 tercol-0.1.4.post1/tercol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 19:37:44.000000 tercol-0.1.4.post1/tercol.egg-info/top_level.txt
```

### Comparing `tercol-0.1.4/LICENSE` & `tercol-0.1.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `tercol-0.1.4/PKG-INFO` & `tercol-0.1.4.post1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: tercol
-Version: 0.1.4
-Summary: TerCol is a useless library that colors your text.
+Version: 0.1.4.post1
+Summary: TerCol is a library that colors your text.
 Author-email: Butterroach <epicnoobcontactemail@gmail.com>
 Project-URL: Homepage, https://butterroach.github.io/tercol
 Project-URL: Bug Tracker, https://github.com/butterroach/tercol/issues
 Project-URL: Source Code, https://github.com/butterroach/tercol
 Keywords: terminal styling,colors,style
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # **[TerCol](https://pypi.org/project/tercol/)**
 
-TerCol is a small, pure Python library that allows you to color and style text output. TerCol has no dependencies and only requires Python 3.6 or newer. It also supports true color. (i think please tell me if it doesn't)
+TerCol is a small, pure Python library that allows you to color and style text output. TerCol has no dependencies and only requires Python 3.7 or newer. It also supports true color.
 
 ## Usage
 
 ```python
 import tercol
 
 print(tercol.red('Red text'))
@@ -33,26 +33,26 @@
 print(tercol.hexa(0xffd700, 'Gold text using HEX'))
 print(tercol.hsv(51, 100, 100, 'Gold text using HSV'))
 print(tercol.rainbowtext('Rainbow text'))
 ```
 
 ## Requirements
 
-TerCol only requires Python 3.6 or newer. No additional dependencies are needed.
+TerCol only requires Python 3.7 or newer. No additional dependencies are needed.
 
 ## Pros
 
 - Small size
 - Pure Python
 - No dependencies
 - Simple automatic reset handling
 - IDE-autocomplete friendly
 - True color support
 
 ## Cons
 
 - Limited support of nested styles
-- Only supports Python 3.6+
+- Only supports Python 3.7+
 
 ## License
 
-TerCol is licensed under the MIT license.
+TerCol is licensed under the MIT license. See the LICENSE file for more info.
```

### Comparing `tercol-0.1.4/README.md` & `tercol-0.1.4.post1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # **[TerCol](https://pypi.org/project/tercol/)**
 
-TerCol is a small, pure Python library that allows you to color and style text output. TerCol has no dependencies and only requires Python 3.6 or newer. It also supports true color. (i think please tell me if it doesn't)
+TerCol is a small, pure Python library that allows you to color and style text output. TerCol has no dependencies and only requires Python 3.7 or newer. It also supports true color.
 
 ## Usage
 
 ```python
 import tercol
 
 print(tercol.red('Red text'))
@@ -15,26 +15,26 @@
 print(tercol.hexa(0xffd700, 'Gold text using HEX'))
 print(tercol.hsv(51, 100, 100, 'Gold text using HSV'))
 print(tercol.rainbowtext('Rainbow text'))
 ```
 
 ## Requirements
 
-TerCol only requires Python 3.6 or newer. No additional dependencies are needed.
+TerCol only requires Python 3.7 or newer. No additional dependencies are needed.
 
 ## Pros
 
 - Small size
 - Pure Python
 - No dependencies
 - Simple automatic reset handling
 - IDE-autocomplete friendly
 - True color support
 
 ## Cons
 
 - Limited support of nested styles
-- Only supports Python 3.6+
+- Only supports Python 3.7+
 
 ## License
 
-TerCol is licensed under the MIT license.
+TerCol is licensed under the MIT license. See the LICENSE file for more info.
```

### Comparing `tercol-0.1.4/pyproject.toml` & `tercol-0.1.4.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tercol"
-version = "0.1.4"
+version = "0.1.4.post1"
 authors = [
   { name="Butterroach", email="epicnoobcontactemail@gmail.com" },
 ]
-description = "TerCol is a useless library that colors your text."
+description = "TerCol is a library that colors your text."
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 keywords = ["terminal styling", "colors", "style"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `tercol-0.1.4/tercol/__init__.py` & `tercol-0.1.4.post1/tercol/__init__.py`

 * *Files identical despite different names*

### Comparing `tercol-0.1.4/tercol/__main__.py` & `tercol-0.1.4.post1/tercol/__main__.py`

 * *Files identical despite different names*

### Comparing `tercol-0.1.4/tercol.egg-info/PKG-INFO` & `tercol-0.1.4.post1/tercol.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: tercol
-Version: 0.1.4
-Summary: TerCol is a useless library that colors your text.
+Version: 0.1.4.post1
+Summary: TerCol is a library that colors your text.
 Author-email: Butterroach <epicnoobcontactemail@gmail.com>
 Project-URL: Homepage, https://butterroach.github.io/tercol
 Project-URL: Bug Tracker, https://github.com/butterroach/tercol/issues
 Project-URL: Source Code, https://github.com/butterroach/tercol
 Keywords: terminal styling,colors,style
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # **[TerCol](https://pypi.org/project/tercol/)**
 
-TerCol is a small, pure Python library that allows you to color and style text output. TerCol has no dependencies and only requires Python 3.6 or newer. It also supports true color. (i think please tell me if it doesn't)
+TerCol is a small, pure Python library that allows you to color and style text output. TerCol has no dependencies and only requires Python 3.7 or newer. It also supports true color.
 
 ## Usage
 
 ```python
 import tercol
 
 print(tercol.red('Red text'))
@@ -33,26 +33,26 @@
 print(tercol.hexa(0xffd700, 'Gold text using HEX'))
 print(tercol.hsv(51, 100, 100, 'Gold text using HSV'))
 print(tercol.rainbowtext('Rainbow text'))
 ```
 
 ## Requirements
 
-TerCol only requires Python 3.6 or newer. No additional dependencies are needed.
+TerCol only requires Python 3.7 or newer. No additional dependencies are needed.
 
 ## Pros
 
 - Small size
 - Pure Python
 - No dependencies
 - Simple automatic reset handling
 - IDE-autocomplete friendly
 - True color support
 
 ## Cons
 
 - Limited support of nested styles
-- Only supports Python 3.6+
+- Only supports Python 3.7+
 
 ## License
 
-TerCol is licensed under the MIT license.
+TerCol is licensed under the MIT license. See the LICENSE file for more info.
```

