# Comparing `tmp/kimariplot-1.1.1.tar.gz` & `tmp/kimariplot-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariplot-1.1.1.tar", last modified: Tue Aug  1 08:23:04 2023, max compression
+gzip compressed data, was "kimariplot-1.1.2.tar", last modified: Tue Aug  1 08:25:40 2023, max compression
```

## Comparing `kimariplot-1.1.1.tar` & `kimariplot-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:23:04.692707 kimariplot-1.1.1/
--rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3065 2023-08-01 08:23:04.691707 kimariplot-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2023-08-01 08:14:46.000000 kimariplot-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:23:04.678709 kimariplot-1.1.1/kimariplot/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.1.1/kimariplot/__init__.py
--rw-rw-rw-   0        0        0     5682 2023-08-01 08:22:58.000000 kimariplot-1.1.1/kimariplot/poltter.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:23:04.689709 kimariplot-1.1.1/kimariplot.egg-info/
--rw-rw-rw-   0        0        0     3065 2023-08-01 08:23:04.000000 kimariplot-1.1.1/kimariplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-01 08:23:04.000000 kimariplot-1.1.1/kimariplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:23:04.000000 kimariplot-1.1.1/kimariplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-01 08:23:04.000000 kimariplot-1.1.1/kimariplot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 08:23:04.000000 kimariplot-1.1.1/kimariplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:23:04.692707 kimariplot-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-08-01 08:22:58.000000 kimariplot-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:25:40.592654 kimariplot-1.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3065 2023-08-01 08:25:40.591654 kimariplot-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2620 2023-08-01 08:14:46.000000 kimariplot-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:25:40.578667 kimariplot-1.1.2/kimariplot/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.1.2/kimariplot/__init__.py
+-rw-rw-rw-   0        0        0     5682 2023-08-01 08:22:58.000000 kimariplot-1.1.2/kimariplot/poltter.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:25:40.588652 kimariplot-1.1.2/kimariplot.egg-info/
+-rw-rw-rw-   0        0        0     3065 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:25:40.592654 kimariplot-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-08-01 08:25:35.000000 kimariplot-1.1.2/setup.py
```

### Comparing `kimariplot-1.1.1/LICENSE` & `kimariplot-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.1/PKG-INFO` & `kimariplot-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.1.1/README.md` & `kimariplot-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.1/kimariplot/poltter.py` & `kimariplot-1.1.2/kimariplot/poltter.py`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.1/kimariplot.egg-info/PKG-INFO` & `kimariplot-1.1.2/kimariplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.1.1/setup.py` & `kimariplot-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kimariplot",
-    version="1.1.1",
+    version="1.1.2",
     author="Kimariyb",
     author_email="kimariyb@163.com",
     description="A tool for generating Kimari-plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimariyb/kimariPlot",
     packages=setuptools.find_packages(),
```

