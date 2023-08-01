# Comparing `tmp/kimariplot-1.1.2.tar.gz` & `tmp/kimariplot-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariplot-1.1.2.tar", last modified: Tue Aug  1 08:25:40 2023, max compression
+gzip compressed data, was "kimariplot-1.1.3.tar", last modified: Tue Aug  1 08:26:55 2023, max compression
```

## Comparing `kimariplot-1.1.2.tar` & `kimariplot-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:25:40.592654 kimariplot-1.1.2/
--rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     3065 2023-08-01 08:25:40.591654 kimariplot-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2023-08-01 08:14:46.000000 kimariplot-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:25:40.578667 kimariplot-1.1.2/kimariplot/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.1.2/kimariplot/__init__.py
--rw-rw-rw-   0        0        0     5682 2023-08-01 08:22:58.000000 kimariplot-1.1.2/kimariplot/poltter.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:25:40.588652 kimariplot-1.1.2/kimariplot.egg-info/
--rw-rw-rw-   0        0        0     3065 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 08:25:40.000000 kimariplot-1.1.2/kimariplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:25:40.592654 kimariplot-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-08-01 08:25:35.000000 kimariplot-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:26:55.420193 kimariplot-1.1.3/
+-rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3065 2023-08-01 08:26:55.419192 kimariplot-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2620 2023-08-01 08:14:46.000000 kimariplot-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:26:55.408195 kimariplot-1.1.3/kimariplot/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.1.3/kimariplot/__init__.py
+-rw-rw-rw-   0        0        0     5682 2023-08-01 08:22:58.000000 kimariplot-1.1.3/kimariplot/poltter.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:26:55.417192 kimariplot-1.1.3/kimariplot.egg-info/
+-rw-rw-rw-   0        0        0     3065 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 08:26:55.000000 kimariplot-1.1.3/kimariplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:26:55.420193 kimariplot-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-08-01 08:26:52.000000 kimariplot-1.1.3/setup.py
```

### Comparing `kimariplot-1.1.2/LICENSE` & `kimariplot-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.2/PKG-INFO` & `kimariplot-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.1.2/README.md` & `kimariplot-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.2/kimariplot/poltter.py` & `kimariplot-1.1.3/kimariplot/poltter.py`

 * *Files identical despite different names*

### Comparing `kimariplot-1.1.2/kimariplot.egg-info/PKG-INFO` & `kimariplot-1.1.3/kimariplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.1.2/setup.py` & `kimariplot-1.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kimariplot",
-    version="1.1.2",
+    version="1.1.3",
     author="Kimariyb",
     author_email="kimariyb@163.com",
     description="A tool for generating Kimari-plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimariyb/kimariPlot",
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
-            'kimariplot=main:main',
+            'kimariplot=kimariPlot:main',
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

