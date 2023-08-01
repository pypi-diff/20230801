# Comparing `tmp/hivecode-0.0.0.8.23.tar.gz` & `tmp/hivecode-0.0.0.8.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivecode-0.0.0.8.23.tar", last modified: Mon Jul 31 00:24:26 2023, max compression
+gzip compressed data, was "hivecode-0.0.0.8.24.tar", last modified: Tue Aug  1 04:38:39 2023, max compression
```

## Comparing `hivecode-0.0.0.8.23.tar` & `hivecode-0.0.0.8.24.tar`

### file list

```diff
@@ -1,40 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.850968 hivecode-0.0.0.8.23/
--rw-rw-rw-   0        0        0     3790 2023-07-31 00:24:26.851467 hivecode-0.0.0.8.23/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.23/README.rst
--rw-rw-rw-   0        0        0     1402 2023-07-31 00:24:05.000000 hivecode-0.0.0.8.23/pyproject.toml
--rw-rw-rw-   0        0        0      226 2023-07-20 05:57:35.000000 hivecode-0.0.0.8.23/requirements.txt
--rw-rw-rw-   0        0        0     1182 2023-07-31 00:24:26.852973 hivecode-0.0.0.8.23/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.794349 hivecode-0.0.0.8.23/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.811809 hivecode-0.0.0.8.23/src/hiveadb/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hiveadb/__init__.py
--rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.23/src/hiveadb/eda.py
--rw-rw-rw-   0        0        0    11930 2023-07-29 05:56:28.000000 hivecode-0.0.0.8.23/src/hiveadb/function.py
--rw-rw-rw-   0        0        0     3706 2023-07-30 23:57:54.000000 hivecode-0.0.0.8.23/src/hiveadb/functions.py
--rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.23/src/hiveadb/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hiveadb/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.828878 hivecode-0.0.0.8.23/src/hivecode.egg-info/
--rw-rw-rw-   0        0        0     3790 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      808 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      314 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.845456 hivecode-0.0.0.8.23/src/hivecore/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivecore/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.23/src/hivecore/constant.py
--rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.23/src/hivecore/decorator.py
--rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.23/src/hivecore/eda.py
--rw-rw-rw-   0        0        0    11298 2023-07-30 23:04:15.000000 hivecode-0.0.0.8.23/src/hivecore/functions.py
--rw-rw-rw-   0        0        0        0 2023-07-30 23:46:14.000000 hivecode-0.0.0.8.23/src/hivecore/legacy_preprocess.py
--rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.23/src/hivecore/patterns.py
--rw-rw-rw-   0        0        0    31989 2023-07-30 23:56:16.000000 hivecode-0.0.0.8.23/src/hivecore/preprocess.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivecore/py.typed
--rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.23/src/hivecore/visual.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.850466 hivecode-0.0.0.8.23/src/hivesignal/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/analysis.py
--rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/eda.py
--rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/py.typed
--rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/transform.py
+drwxrwxrwx   0        0        0        0 2023-08-01 04:38:39.116073 hivecode-0.0.0.8.24/
+-rw-rw-rw-   0        0        0     1103 2023-07-31 00:53:19.000000 hivecode-0.0.0.8.24/LICENSE
+-rw-rw-rw-   0        0        0     3683 2023-08-01 04:38:39.116573 hivecode-0.0.0.8.24/PKG-INFO
+-rw-rw-rw-   0        0        0     2818 2023-07-31 00:51:24.000000 hivecode-0.0.0.8.24/README.rst
+-rw-rw-rw-   0        0        0     1261 2023-08-01 04:38:24.000000 hivecode-0.0.0.8.24/pyproject.toml
+-rw-rw-rw-   0        0        0      249 2023-08-01 04:30:01.000000 hivecode-0.0.0.8.24/requirements.txt
+-rw-rw-rw-   0        0        0     1182 2023-08-01 04:38:39.118569 hivecode-0.0.0.8.24/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 04:38:39.068529 hivecode-0.0.0.8.24/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 04:38:39.081381 hivecode-0.0.0.8.24/src/hiveadb/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hiveadb/__init__.py
+-rw-rw-rw-   0        0        0    13883 2023-08-01 04:33:35.000000 hivecode-0.0.0.8.24/src/hiveadb/functions.py
+-rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.24/src/hiveadb/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hiveadb/py.typed
+drwxrwxrwx   0        0        0        0 2023-08-01 04:38:39.099467 hivecode-0.0.0.8.24/src/hivecode.egg-info/
+-rw-rw-rw-   0        0        0     3683 2023-08-01 04:38:39.000000 hivecode-0.0.0.8.24/src/hivecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2023-08-01 04:38:39.000000 hivecode-0.0.0.8.24/src/hivecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 04:38:39.000000 hivecode-0.0.0.8.24/src/hivecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.24/src/hivecode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      336 2023-08-01 04:38:39.000000 hivecode-0.0.0.8.24/src/hivecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-08-01 04:38:39.000000 hivecode-0.0.0.8.24/src/hivecode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 04:38:39.109562 hivecode-0.0.0.8.24/src/hivecore/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hivecore/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.24/src/hivecore/constant.py
+-rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.24/src/hivecore/decorator.py
+-rw-rw-rw-   0        0        0    11298 2023-07-30 23:04:15.000000 hivecode-0.0.0.8.24/src/hivecore/functions.py
+-rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.24/src/hivecore/patterns.py
+-rw-rw-rw-   0        0        0    31989 2023-07-30 23:56:16.000000 hivecode-0.0.0.8.24/src/hivecore/preprocess.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hivecore/py.typed
+drwxrwxrwx   0        0        0        0 2023-08-01 04:38:39.115563 hivecode-0.0.0.8.24/src/hivesignal/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hivesignal/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hivesignal/analysis.py
+-rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hivesignal/eda.py
+-rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hivesignal/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hivesignal/py.typed
+-rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.24/src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.23/PKG-INFO` & `hivecode-0.0.0.8.24/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.23
-Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
+Version: 0.0.0.8.24
+Summary: Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
 Platform: osx
@@ -13,14 +13,15 @@
 Platform: win32
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: dev
+License-File: LICENSE
 
 .. |PyPI version Hivecode| image:: https://img.shields.io/pypi/v/hivecode.svg
    :target: https://pypi.org/project/hivecode/
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/hivecode/badge/?version=latest
    :target: http://hivecode.readthedocs.io/?badge=latest
 
@@ -30,15 +31,15 @@
 .. |PyPI license| image:: https://img.shields.io/pypi/l/hivecode.svg
    :target: https://pypi.org/project/hivecode/
 
 Hivecode
 ========
 |PyPI version Hivecode| |Documentation Status| |MIT license|
 
-Hivecode is a Python library designed as a toolkit for data engineering and data science. The library includes a collection of useful functions and tools for reading, mounting, and storing data in Azure DataBricks. Hivecode also includes patterns, decorators, and analytics tools to help make your data processing workflow more efficient and streamlined. With Hivecode, you can simplify your data engineering and analysis tasks, freeing up your time to focus on more strategic work. Whether you're a data engineer, data analyst, or data scientist, Hivecode has something to offer.
+Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects. This library boasts a wide array of practical and innovative functions, ranging from seamless integration with Azure Databricks to implementing essential design patterns, data preprocessing, visualization, exploration, and more. Whether you're looking to supercharge your data analysis or accelerate your Python projects, Hivecode is the go-to toolkit for unlocking the full potential of your endeavors.
 
 Packages
 ========
 - Hivecore: A set of many vanilla python tools.
 - Hiveadb: A set of tools to work in Azure Databricks.
 - Hivesignal: A set of tools for signal analysis.
```

### Comparing `hivecode-0.0.0.8.23/README.rst` & `hivecode-0.0.0.8.24/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 .. |PyPI license| image:: https://img.shields.io/pypi/l/hivecode.svg
    :target: https://pypi.org/project/hivecode/
 
 Hivecode
 ========
 |PyPI version Hivecode| |Documentation Status| |MIT license|
 
-Hivecode is a Python library designed as a toolkit for data engineering and data science. The library includes a collection of useful functions and tools for reading, mounting, and storing data in Azure DataBricks. Hivecode also includes patterns, decorators, and analytics tools to help make your data processing workflow more efficient and streamlined. With Hivecode, you can simplify your data engineering and analysis tasks, freeing up your time to focus on more strategic work. Whether you're a data engineer, data analyst, or data scientist, Hivecode has something to offer.
+Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects. This library boasts a wide array of practical and innovative functions, ranging from seamless integration with Azure Databricks to implementing essential design patterns, data preprocessing, visualization, exploration, and more. Whether you're looking to supercharge your data analysis or accelerate your Python projects, Hivecode is the go-to toolkit for unlocking the full potential of your endeavors.
 
 Packages
 ========
 - Hivecore: A set of many vanilla python tools.
 - Hiveadb: A set of tools to work in Azure Databricks.
 - Hivesignal: A set of tools for signal analysis.
```

### Comparing `hivecode-0.0.0.8.23/pyproject.toml` & `hivecode-0.0.0.8.24/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "hivecode"
-description = "Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell."
-version = "0.0.0.8.23"
+description = "Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects."
+version = "0.0.0.8.24"
 requires-python = ">=3.8.0"
 readme = "README.rst"
 authors = [
     {name = "Juan Manuel Mejía Botero", email="juanmam941025@gmail.com"},
     {name = "Sebastian López Valencia", email="sebaslv12@hotmail.com"}
 ]
```

### Comparing `hivecode-0.0.0.8.23/setup.cfg` & `hivecode-0.0.0.8.24/setup.cfg`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hiveadb/io.py` & `hivecode-0.0.0.8.24/src/hiveadb/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hivecode.egg-info/PKG-INFO` & `hivecode-0.0.0.8.24/src/hivecode.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.23
-Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
+Version: 0.0.0.8.24
+Summary: Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
 Platform: osx
@@ -13,14 +13,15 @@
 Platform: win32
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: dev
+License-File: LICENSE
 
 .. |PyPI version Hivecode| image:: https://img.shields.io/pypi/v/hivecode.svg
    :target: https://pypi.org/project/hivecode/
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/hivecode/badge/?version=latest
    :target: http://hivecode.readthedocs.io/?badge=latest
 
@@ -30,15 +31,15 @@
 .. |PyPI license| image:: https://img.shields.io/pypi/l/hivecode.svg
    :target: https://pypi.org/project/hivecode/
 
 Hivecode
 ========
 |PyPI version Hivecode| |Documentation Status| |MIT license|
 
-Hivecode is a Python library designed as a toolkit for data engineering and data science. The library includes a collection of useful functions and tools for reading, mounting, and storing data in Azure DataBricks. Hivecode also includes patterns, decorators, and analytics tools to help make your data processing workflow more efficient and streamlined. With Hivecode, you can simplify your data engineering and analysis tasks, freeing up your time to focus on more strategic work. Whether you're a data engineer, data analyst, or data scientist, Hivecode has something to offer.
+Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects. This library boasts a wide array of practical and innovative functions, ranging from seamless integration with Azure Databricks to implementing essential design patterns, data preprocessing, visualization, exploration, and more. Whether you're looking to supercharge your data analysis or accelerate your Python projects, Hivecode is the go-to toolkit for unlocking the full potential of your endeavors.
 
 Packages
 ========
 - Hivecore: A set of many vanilla python tools.
 - Hiveadb: A set of tools to work in Azure Databricks.
 - Hivesignal: A set of tools for signal analysis.
```

### Comparing `hivecode-0.0.0.8.23/src/hivecode.egg-info/SOURCES.txt` & `hivecode-0.0.0.8.24/src/hivecode.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,29 @@
+LICENSE
 README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 src/hiveadb/__init__.py
-src/hiveadb/eda.py
-src/hiveadb/function.py
 src/hiveadb/functions.py
 src/hiveadb/io.py
 src/hiveadb/py.typed
 src/hivecode.egg-info/PKG-INFO
 src/hivecode.egg-info/SOURCES.txt
 src/hivecode.egg-info/dependency_links.txt
 src/hivecode.egg-info/not-zip-safe
 src/hivecode.egg-info/requires.txt
 src/hivecode.egg-info/top_level.txt
 src/hivecore/__init__.py
 src/hivecore/constant.py
 src/hivecore/decorator.py
-src/hivecore/eda.py
 src/hivecore/functions.py
-src/hivecore/legacy_preprocess.py
 src/hivecore/patterns.py
 src/hivecore/preprocess.py
 src/hivecore/py.typed
-src/hivecore/visual.py
 src/hivesignal/__init__.py
 src/hivesignal/analysis.py
 src/hivesignal/eda.py
 src/hivesignal/io.py
 src/hivesignal/py.typed
 src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.23/src/hivecore/constant.py` & `hivecode-0.0.0.8.24/src/hivecore/constant.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hivecore/decorator.py` & `hivecode-0.0.0.8.24/src/hivecore/decorator.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hivecore/functions.py` & `hivecode-0.0.0.8.24/src/hivecore/functions.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hivecore/patterns.py` & `hivecode-0.0.0.8.24/src/hivecore/patterns.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hivecore/preprocess.py` & `hivecode-0.0.0.8.24/src/hivecore/preprocess.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hivesignal/analysis.py` & `hivecode-0.0.0.8.24/src/hivesignal/analysis.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hivesignal/io.py` & `hivecode-0.0.0.8.24/src/hivesignal/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.23/src/hivesignal/transform.py` & `hivecode-0.0.0.8.24/src/hivesignal/transform.py`

 * *Files identical despite different names*

