# Comparing `tmp/pypeline-python-0.1.2.tar.gz` & `tmp/pypeline-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeline-python-0.1.2.tar", last modified: Tue Aug  1 16:49:22 2023, max compression
+gzip compressed data, was "pypeline-python-0.1.3.tar", last modified: Tue Aug  1 16:57:41 2023, max compression
```

## Comparing `pypeline-python-0.1.2.tar` & `pypeline-python-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/pypeline_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 16:49:22.000000 pypeline-python-0.1.2/pypeline_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/pypipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/item.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/items_container.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/pypipeline/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:49:22.378436 pypeline-python-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-01 16:49:13.000000 pypeline-python-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:57:41.418202 pypeline-python-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-01 16:57:41.418202 pypeline-python-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:57:41.414201 pypeline-python-0.1.3/pypeline_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-01 16:57:41.000000 pypeline-python-0.1.3/pypeline_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-01 16:57:41.000000 pypeline-python-0.1.3/pypeline_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:57:41.000000 pypeline-python-0.1.3/pypeline_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 16:57:41.000000 pypeline-python-0.1.3/pypeline_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 16:57:41.000000 pypeline-python-0.1.3/pypeline_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:57:41.414201 pypeline-python-0.1.3/pypipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/items_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/pypipeline/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:57:41.418202 pypeline-python-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-01 16:57:29.000000 pypeline-python-0.1.3/setup.py
```

### Comparing `pypeline-python-0.1.2/LICENSE` & `pypeline-python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.2/PKG-INFO` & `pypeline-python-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeline-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyPipeline is a simple Python framework for building data processing pipelines.
 Home-page: https://github.com/zigai/py-pipeline
 Author: Žiga Ivanšek
 Author-email: ziga.ivansek@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pypeline-python-0.1.2/README.md` & `pypeline-python-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.2/pypeline_python.egg-info/PKG-INFO` & `pypeline-python-0.1.3/pypeline_python.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeline-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyPipeline is a simple Python framework for building data processing pipelines.
 Home-page: https://github.com/zigai/py-pipeline
 Author: Žiga Ivanšek
 Author-email: ziga.ivansek@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pypeline-python-0.1.2/pypipeline/action.py` & `pypeline-python-0.1.3/pypipeline/action.py`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.2/pypipeline/cli.py` & `pypeline-python-0.1.3/pypipeline/cli.py`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.2/pypipeline/filter.py` & `pypeline-python-0.1.3/pypipeline/filter.py`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.2/pypipeline/items_container.py` & `pypeline-python-0.1.3/pypipeline/items_container.py`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.2/pypipeline/pipeline.py` & `pypeline-python-0.1.3/pypipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.2/pypipeline/util.py` & `pypeline-python-0.1.3/pypipeline/util.py`

 * *Files identical despite different names*

### Comparing `pypeline-python-0.1.2/setup.py` & `pypeline-python-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 REQUIREMENTS = (HERE / "requirements.txt").read_text()
 
 setup(
     name="pypeline-python",
-    version="0.1.2",
+    version="0.1.3",
     description="PyPipeline is a simple Python framework for building data processing pipelines.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Žiga Ivanšek",
     author_email="ziga.ivansek@gmail.com",
     url="https://github.com/zigai/py-pipeline",
     license="MIT",
```

