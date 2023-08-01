# Comparing `tmp/plotagain-1.0.5.tar.gz` & `tmp/plotagain-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotagain-1.0.5.tar", last modified: Sun Jul 23 14:15:27 2023, max compression
+gzip compressed data, was "plotagain-1.0.6.tar", last modified: Tue Aug  1 16:56:47 2023, max compression
```

## Comparing `plotagain-1.0.5.tar` & `plotagain-1.0.6.tar`

### file list

```diff
@@ -1,75 +1,38 @@
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.277085 plotagain-1.0.5/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       49 2023-07-23 14:15:06.000000 plotagain-1.0.5/.gitignore
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3860 2023-07-23 14:15:27.276894 plotagain-1.0.5/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3267 2023-07-23 14:13:03.000000 plotagain-1.0.5/README.md
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2159 2023-07-20 18:09:45.000000 plotagain-1.0.5/bitbucket-pipelines.yml
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.265892 plotagain-1.0.5/docs/
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.266048 plotagain-1.0.5/docs/build/
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.268211 plotagain-1.0.5/docs/build/doctrees/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)    17067 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/doctrees/environment.pickle
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4971 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/doctrees/index.doctree
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.269640 plotagain-1.0.5/docs/build/html/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      230 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/.buildinfo
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.270259 plotagain-1.0.5/docs/build/html/.doctrees/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7208 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/.doctrees/api.doctree
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)   146512 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/.doctrees/environment.pickle
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.270992 plotagain-1.0.5/docs/build/html/.doctrees/generated/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4927 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/.doctrees/generated/plotagain.doctree
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)    78474 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/.doctrees/generated/plotagain.saveplotcontext.SavePlotContext.doctree
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     5033 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/.doctrees/generated/plotagain.saveplotcontext.doctree
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     5961 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/.doctrees/generated/plotagain.utils.doctree
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     6077 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/.doctrees/index.doctree
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.271339 plotagain-1.0.5/docs/build/html/_sources/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      155 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_sources/api.rst.txt
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.272003 plotagain-1.0.5/docs/build/html/_sources/generated/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      189 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_sources/generated/plotagain.rst.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      809 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_sources/generated/plotagain.saveplotcontext.SavePlotContext.rst.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      227 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_sources/generated/plotagain.saveplotcontext.rst.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      214 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_sources/generated/plotagain.utils.rst.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      770 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_sources/index.rst.txt
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.273888 plotagain-1.0.5/docs/build/html/_static/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)    11230 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/alabaster.css
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)    14813 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/basic.css
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       42 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/custom.css
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4472 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/doctools.js
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      420 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      286 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/file.png
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4758 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/language_data.js
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       90 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/minus.png
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       90 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/plus.png
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     5327 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/pygments.css
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)    18215 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/searchtools.js
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4712 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     5063 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/api.html
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.274560 plotagain-1.0.5/docs/build/html/generated/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4040 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/generated/plotagain.html
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)    22895 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/generated/plotagain.saveplotcontext.SavePlotContext.html
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4503 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/generated/plotagain.saveplotcontext.html
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4113 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/generated/plotagain.utils.html
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4619 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/genindex.html
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     4812 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/index.html
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      411 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/objects.inv
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3572 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/py-modindex.html
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2803 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/search.html
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     5155 2023-07-23 14:13:03.000000 plotagain-1.0.5/docs/build/html/searchindex.js
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      859 2023-07-20 18:21:23.000000 plotagain-1.0.5/pyproject.toml
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-23 14:15:06.000000 plotagain-1.0.5/requirements.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-07-23 14:15:27.277141 plotagain-1.0.5/setup.cfg
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.266854 plotagain-1.0.5/src/
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.275533 plotagain-1.0.5/src/plotagain/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      549 2023-07-23 14:15:06.000000 plotagain-1.0.5/src/plotagain/__init__.py
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.276490 plotagain-1.0.5/src/plotagain/data-save-dir/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      404 2023-07-23 08:24:22.000000 plotagain-1.0.5/src/plotagain/data-save-dir/make_plot.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2526 2023-07-20 18:00:09.000000 plotagain-1.0.5/src/plotagain/iddict.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7252 2023-07-23 14:15:06.000000 plotagain-1.0.5/src/plotagain/pyplotcall.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     8911 2023-07-23 14:15:06.000000 plotagain-1.0.5/src/plotagain/saveplotcontext.py
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)      124 2023-07-20 17:53:49.000000 plotagain-1.0.5/src/plotagain/script_template.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1930 2023-07-23 14:15:06.000000 plotagain-1.0.5/src/plotagain/utils.py
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.276330 plotagain-1.0.5/src/plotagain.egg-info/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3860 2023-07-23 14:15:27.000000 plotagain-1.0.5/src/plotagain.egg-info/PKG-INFO
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2199 2023-07-23 14:15:27.000000 plotagain-1.0.5/src/plotagain.egg-info/SOURCES.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-07-23 14:15:27.000000 plotagain-1.0.5/src/plotagain.egg-info/dependency_links.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-07-23 14:15:27.000000 plotagain-1.0.5/src/plotagain.egg-info/requires.txt
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-07-23 14:15:27.000000 plotagain-1.0.5/src/plotagain.egg-info/top_level.txt
-drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-07-23 14:15:27.276642 plotagain-1.0.5/tests/
--rw-r--r--   0 jeremywilkinson   (501) staff       (20)       30 2023-07-20 18:12:48.000000 plotagain-1.0.5/tests/test_nothing.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.632669 plotagain-1.0.6/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       60 2023-07-23 14:24:24.000000 plotagain-1.0.6/.gitignore
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3860 2023-08-01 16:56:47.632507 plotagain-1.0.6/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3267 2023-07-23 14:21:28.000000 plotagain-1.0.6/README.md
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2159 2023-07-20 18:09:45.000000 plotagain-1.0.6/bitbucket-pipelines.yml
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.627660 plotagain-1.0.6/docs/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      638 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/Makefile
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      804 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/make.bat
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.628101 plotagain-1.0.6/docs/source/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      155 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/source/api.rst
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1048 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/source/conf.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.628724 plotagain-1.0.6/docs/source/generated/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      189 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/source/generated/plotagain.rst
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      809 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/source/generated/plotagain.saveplotcontext.SavePlotContext.rst
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      227 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/source/generated/plotagain.saveplotcontext.rst
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      214 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/source/generated/plotagain.utils.rst
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      770 2023-07-23 14:24:24.000000 plotagain-1.0.6/docs/source/index.rst
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      859 2023-07-20 18:21:23.000000 plotagain-1.0.6/pyproject.toml
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       16 2023-07-23 14:20:54.000000 plotagain-1.0.6/requirements.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       38 2023-08-01 16:56:47.632713 plotagain-1.0.6/setup.cfg
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.626257 plotagain-1.0.6/src/
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.630515 plotagain-1.0.6/src/plotagain/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      556 2023-08-01 16:56:33.000000 plotagain-1.0.6/src/plotagain/__init__.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.631829 plotagain-1.0.6/src/plotagain/data-save-dir/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      404 2023-07-23 08:24:22.000000 plotagain-1.0.6/src/plotagain/data-save-dir/make_plot.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     2526 2023-07-20 18:00:09.000000 plotagain-1.0.6/src/plotagain/iddict.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     7252 2023-07-23 14:20:54.000000 plotagain-1.0.6/src/plotagain/pyplotcall.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     8911 2023-07-23 14:21:28.000000 plotagain-1.0.6/src/plotagain/saveplotcontext.py
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      124 2023-07-20 17:53:49.000000 plotagain-1.0.6/src/plotagain/script_template.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     1930 2023-07-23 14:20:54.000000 plotagain-1.0.6/src/plotagain/utils.py
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.631672 plotagain-1.0.6/src/plotagain.egg-info/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)     3860 2023-08-01 16:56:47.000000 plotagain-1.0.6/src/plotagain.egg-info/PKG-INFO
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)      779 2023-08-01 16:56:47.000000 plotagain-1.0.6/src/plotagain.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)        1 2023-08-01 16:56:47.000000 plotagain-1.0.6/src/plotagain.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       17 2023-08-01 16:56:47.000000 plotagain-1.0.6/src/plotagain.egg-info/requires.txt
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       10 2023-08-01 16:56:47.000000 plotagain-1.0.6/src/plotagain.egg-info/top_level.txt
+drwxr-xr-x   0 jeremywilkinson   (501) staff       (20)        0 2023-08-01 16:56:47.632139 plotagain-1.0.6/tests/
+-rw-r--r--   0 jeremywilkinson   (501) staff       (20)       30 2023-07-20 18:12:48.000000 plotagain-1.0.6/tests/test_nothing.py
```

### Comparing `plotagain-1.0.5/PKG-INFO` & `plotagain-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotagain
-Version: 1.0.5
+Version: 1.0.6
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://bitbucket.org/jjhw3/plotagain/
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `plotagain-1.0.5/README.md` & `plotagain-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/bitbucket-pipelines.yml` & `plotagain-1.0.6/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/docs/build/html/_sources/generated/plotagain.saveplotcontext.SavePlotContext.rst.txt` & `plotagain-1.0.6/docs/source/generated/plotagain.saveplotcontext.SavePlotContext.rst`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/docs/build/html/_sources/index.rst.txt` & `plotagain-1.0.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/pyproject.toml` & `plotagain-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/src/plotagain/__init__.py` & `plotagain-1.0.6/src/plotagain/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .saveplotcontext import SavePlotContext
 from .utils import load_pickle, write_pickle
-import saveplotcontext
+from . import saveplotcontext
 
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 
 
 def set_skip_all_show_plots(skip: bool) -> None:
     """
     A global version of SavePlotContext.skip_show_plots which applies to all SavePlotContext instances. If set to True,
     overrides the value of skip_show_plots passed into the constructor of a SavePlotContext object
```

### Comparing `plotagain-1.0.5/src/plotagain/iddict.py` & `plotagain-1.0.6/src/plotagain/iddict.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/src/plotagain/pyplotcall.py` & `plotagain-1.0.6/src/plotagain/pyplotcall.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/src/plotagain/saveplotcontext.py` & `plotagain-1.0.6/src/plotagain/saveplotcontext.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/src/plotagain/utils.py` & `plotagain-1.0.6/src/plotagain/utils.py`

 * *Files identical despite different names*

### Comparing `plotagain-1.0.5/src/plotagain.egg-info/PKG-INFO` & `plotagain-1.0.6/src/plotagain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotagain
-Version: 1.0.5
+Version: 1.0.6
 Summary: A helper tool for matplotlib. Provides a contextmanager which automatically saves data used to make plots and automatically generates a script to re-load and re-plot this data at a later stage.
 Author-email: Jeremy John Henry Wilkinson <jero.wilkinson@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://bitbucket.org/jjhw3/plotagain/
 Keywords: save data,matplotlib,plt
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
```

