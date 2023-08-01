# Comparing `tmp/mt4forexparser-1.1.dev26.tar.gz` & `tmp/mt4forexparser-1.1.dev29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mt4forexparser-1.1.dev26.tar", last modified: Wed Mar 10 20:36:30 2021, max compression
+gzip compressed data, was "dist/mt4forexparser-1.1.dev29.tar", last modified: Wed Mar 10 22:34:42 2021, max compression
```

## Comparing `mt4forexparser-1.1.dev26.tar` & `mt4forexparser-1.1.dev29.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/
--rw-rw-r--   0 travis    (2000) travis    (2000)      898 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    10112 2021-03-10 20:35:13.000000 mt4forexparser-1.1.dev26/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6965 2021-03-10 20:35:13.000000 mt4forexparser-1.1.dev26/mt4forexparser/MT4ForexParser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3010 2021-03-10 20:35:13.000000 mt4forexparser-1.1.dev26/mt4forexparser/UniLogger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-10 20:35:13.000000 mt4forexparser-1.1.dev26/mt4forexparser/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2021-03-10 20:35:13.000000 mt4forexparser-1.1.dev26/mt4forexparser/__main__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      898 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      406 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/mt4forexparser.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2021-03-10 20:36:30.000000 mt4forexparser-1.1.dev26/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2435 2021-03-10 20:35:13.000000 mt4forexparser-1.1.dev26/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      898 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10112 2021-03-10 22:33:28.000000 mt4forexparser-1.1.dev29/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6965 2021-03-10 22:33:29.000000 mt4forexparser-1.1.dev29/mt4forexparser/MT4ForexParser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3010 2021-03-10 22:33:29.000000 mt4forexparser-1.1.dev29/mt4forexparser/UniLogger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-10 22:33:29.000000 mt4forexparser-1.1.dev29/mt4forexparser/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2021-03-10 22:33:29.000000 mt4forexparser-1.1.dev29/mt4forexparser/__main__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      898 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      406 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/mt4forexparser.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2021-03-10 22:34:42.000000 mt4forexparser-1.1.dev29/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2435 2021-03-10 22:33:29.000000 mt4forexparser-1.1.dev29/setup.py
```

### Comparing `mt4forexparser-1.1.dev26/PKG-INFO` & `mt4forexparser-1.1.dev29/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mt4forexparser
-Version: 1.1.dev26
+Version: 1.1.dev29
 Summary: Read forex data in MetaTrader 4 .hst-format and convert into .csv file and pandas dataframe. Also you can draw an interactive chart.
 Home-page: https://github.com/Tim55667757/MT4ForexParser/
 Author: Timur Gilmullin
 Author-email: tim55667757@gmail.com
 License: MIT
 Download-URL: https://github.com/Tim55667757/MT4ForexParser.git
 Description: GitHub Pages: https://tim55667757.github.io/MT4ForexParser
```

### Comparing `mt4forexparser-1.1.dev26/README.md` & `mt4forexparser-1.1.dev29/README.md`

 * *Files identical despite different names*

### Comparing `mt4forexparser-1.1.dev26/mt4forexparser/MT4ForexParser.py` & `mt4forexparser-1.1.dev29/mt4forexparser/MT4ForexParser.py`

 * *Files identical despite different names*

### Comparing `mt4forexparser-1.1.dev26/mt4forexparser/UniLogger.py` & `mt4forexparser-1.1.dev29/mt4forexparser/UniLogger.py`

 * *Files identical despite different names*

### Comparing `mt4forexparser-1.1.dev26/mt4forexparser.egg-info/PKG-INFO` & `mt4forexparser-1.1.dev29/mt4forexparser.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mt4forexparser
-Version: 1.1.dev26
+Version: 1.1.dev29
 Summary: Read forex data in MetaTrader 4 .hst-format and convert into .csv file and pandas dataframe. Also you can draw an interactive chart.
 Home-page: https://github.com/Tim55667757/MT4ForexParser/
 Author: Timur Gilmullin
 Author-email: tim55667757@gmail.com
 License: MIT
 Download-URL: https://github.com/Tim55667757/MT4ForexParser.git
 Description: GitHub Pages: https://tim55667757.github.io/MT4ForexParser
```

### Comparing `mt4forexparser-1.1.dev26/setup.py` & `mt4forexparser-1.1.dev29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,20 @@
         "MetaTrader",
         "MetaTrader4",
     ],
 
     tests_require=[
         "pytest>=6.2.2",
         "pandas>=1.2.2",
-        "pricegenerator>=1.2.36",
+        "pricegenerator>=1.2.46",
     ],
 
     install_requires=[
         "pandas>=1.2.2",
-        "pricegenerator>=1.2.36",
+        "pricegenerator>=1.2.46",
     ],
 
     packages=[
         "mt4forexparser",
     ],
 
     zip_safe=True,
```

