# Comparing `tmp/python-hole-0.0.6.tar.gz` & `tmp/python-hole-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-hole-0.0.6.tar", last modified: Mon Jul 31 14:37:51 2023, max compression
+gzip compressed data, was "python-hole-0.0.7.tar", last modified: Tue Aug  1 12:37:09 2023, max compression
```

## Comparing `python-hole-0.0.6.tar` & `python-hole-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.764876 python-hole-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 14:37:45.000000 python-hole-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-31 14:37:51.764876 python-hole-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-31 14:37:45.000000 python-hole-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:37:51.764876 python-hole-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-31 14:37:45.000000 python-hole-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.756876 python-hole-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.760877 python-hole-0.0.6/src/pyhole/
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/AstWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/HoleAST.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/Matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/PatternMatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/PyHoleErrorListener.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/PyHoleParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    40290 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/PyHoleVisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.764876 python-hole-0.0.6/src/pyhole/antlr/
--rw-r--r--   0 runner    (1001) docker     (123)    52568 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/Python3Lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27385 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/Python3Listener.py
--rw-r--r--   0 runner    (1001) docker     (123)   339487 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/Python3Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/Python3Visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.764876 python-hole-0.0.6/src/pyhole/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/visualizer/Visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/visualizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.764876 python-hole-0.0.6/src/python_hole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.781131 python-hole-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 12:37:05.000000 python-hole-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-01 12:37:09.781131 python-hole-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-01 12:37:05.000000 python-hole-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:37:09.781131 python-hole-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-01 12:37:05.000000 python-hole-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.777131 python-hole-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.777131 python-hole-0.0.7/src/pyhole/
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/AstWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/HoleAST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/Matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/PatternMatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/PyHoleErrorListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/PyHoleParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40290 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/PyHoleVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.777131 python-hole-0.0.7/src/pyhole/antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)    52568 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/Python3Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27385 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/Python3Listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   339487 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/Python3Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/Python3Visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.777131 python-hole-0.0.7/src/pyhole/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/visualizer/Visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/visualizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.781131 python-hole-0.0.7/src/python_hole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/top_level.txt
```

### Comparing `python-hole-0.0.6/LICENSE` & `python-hole-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/PKG-INFO` & `python-hole-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hole
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package to build code patterns
 Home-page: https://github.com/JulienLie/python-hole
 Author: Julien Lienard
 Author-email: julien.lienard@uclouvain.be
 License: MIT
 Description: # Python Hole
```

### Comparing `python-hole-0.0.6/README.md` & `python-hole-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/setup.py` & `python-hole-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='python-hole',
-    version='0.0.6',
+    version='0.0.7',
     packages=['pyhole', 'pyhole.antlr', 'pyhole.visualizer'],
     package_dir={'': 'src'},
     url='https://github.com/JulienLie/python-hole',
     license='MIT',
     author='Julien Lienard',
     author_email='julien.lienard@uclouvain.be',
     description="Python package to build code patterns",
```

### Comparing `python-hole-0.0.6/src/pyhole/AstWalker.py` & `python-hole-0.0.7/src/pyhole/AstWalker.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/HoleAST.py` & `python-hole-0.0.7/src/pyhole/HoleAST.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/Matcher.py` & `python-hole-0.0.7/src/pyhole/Matcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,29 @@
+import glob
 from copy import deepcopy
 
 from .AstWalker import AstWalker
 from .HoleAST import *
 from .PatternMatch import PatternMatch
 from .PyHoleParser import parse_pyhole
 
 
+def match_wildcards(path_pattern_with_wildcards, path_python_with_wildcard, strict_match=False, match_details=False):
+    ret = {}
+    patterns_filespath = glob.glob(str(path_pattern_with_wildcards))
+    pythons_filespath = glob.glob(str(path_python_with_wildcard))
+    for python_filepath in pythons_filespath:
+        for pattern_filepath in patterns_filespath:
+            result = match_files(pattern_filepath, python_filepath, strict_match, match_details)
+            if python_filepath not in ret:
+                ret[python_filepath] = {}
+            ret[python_filepath][pattern_filepath] = result
+    return ret
+
+
 def match_files(path_pattern, path_python, strict_match=False, match_details=False):
     pattern = parse_pyhole(path_pattern)
     with open(path_python) as file:
         source = file.read()
         python = ast.parse(source, path_python)
 
     matcher = Matcher()
```

### Comparing `python-hole-0.0.6/src/pyhole/PatternMatch.py` & `python-hole-0.0.7/src/pyhole/PatternMatch.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/PyHoleErrorListener.py` & `python-hole-0.0.7/src/pyhole/PyHoleErrorListener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/PyHoleParser.py` & `python-hole-0.0.7/src/pyhole/PyHoleParser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/PyHoleVisitor.py` & `python-hole-0.0.7/src/pyhole/PyHoleVisitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/antlr/Python3Lexer.py` & `python-hole-0.0.7/src/pyhole/antlr/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/antlr/Python3Listener.py` & `python-hole-0.0.7/src/pyhole/antlr/Python3Listener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/antlr/Python3Parser.py` & `python-hole-0.0.7/src/pyhole/antlr/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/antlr/Python3Visitor.py` & `python-hole-0.0.7/src/pyhole/antlr/Python3Visitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/pyhole/visualizer/Visualizer.py` & `python-hole-0.0.7/src/pyhole/visualizer/Visualizer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.6/src/python_hole.egg-info/PKG-INFO` & `python-hole-0.0.7/src/python_hole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hole
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package to build code patterns
 Home-page: https://github.com/JulienLie/python-hole
 Author: Julien Lienard
 Author-email: julien.lienard@uclouvain.be
 License: MIT
 Description: # Python Hole
```

### Comparing `python-hole-0.0.6/src/python_hole.egg-info/SOURCES.txt` & `python-hole-0.0.7/src/python_hole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

