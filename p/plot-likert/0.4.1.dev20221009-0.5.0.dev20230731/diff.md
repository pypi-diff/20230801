# Comparing `tmp/plot-likert-0.4.1.dev20221009.tar.gz` & `tmp/plot-likert-0.5.0.dev20230731.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot-likert-0.4.1.dev20221009.tar", last modified: Sun Oct  9 21:40:17 2022, max compression
+gzip compressed data, was "plot-likert-0.5.0.dev20230731.tar", last modified: Tue Aug  1 05:24:32 2023, max compression
```

## Comparing `plot-likert-0.4.1.dev20221009.tar` & `plot-likert-0.5.0.dev20230731.tar`

### file list

```diff
@@ -1,31 +1,21 @@
-drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2022-10-09 21:40:17.576928 plot-likert-0.4.1.dev20221009/
-drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2022-10-09 21:40:17.559475 plot-likert-0.4.1.dev20221009/.github/
-drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2022-10-09 21:40:17.562217 plot-likert-0.4.1.dev20221009/.github/workflows/
--rw-r--r--   0 nmalkin    (501) staff       (20)     1195 2022-04-03 05:04:24.000000 plot-likert-0.4.1.dev20221009/.github/workflows/test.yml
--rw-r--r--   0 nmalkin    (501) staff       (20)     2107 2021-01-01 23:12:01.000000 plot-likert-0.4.1.dev20221009/.gitignore
--rw-r--r--   0 nmalkin    (501) staff       (20)     1454 2018-08-19 01:07:57.000000 plot-likert-0.4.1.dev20221009/LICENSE
--rw-r--r--   0 nmalkin    (501) staff       (20)     2824 2022-10-09 21:40:17.576558 plot-likert-0.4.1.dev20221009/PKG-INFO
--rw-r--r--   0 nmalkin    (501) staff       (20)     2225 2022-04-03 05:04:24.000000 plot-likert-0.4.1.dev20221009/README.md
-drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2022-10-09 21:40:17.571393 plot-likert-0.4.1.dev20221009/docs/
--rw-r--r--   0 nmalkin    (501) staff       (20)    68634 2022-09-08 03:46:35.000000 plot-likert-0.4.1.dev20221009/docs/example.ipynb
--rw-r--r--   0 nmalkin    (501) staff       (20)   178380 2022-09-08 03:46:35.000000 plot-likert-0.4.1.dev20221009/docs/guide.ipynb
--rw-r--r--   0 nmalkin    (501) staff       (20)  1916931 2022-09-08 03:46:35.000000 plot-likert-0.4.1.dev20221009/docs/lots_of_random_figures.ipynb
--rw-r--r--   0 nmalkin    (501) staff       (20)    14254 2021-02-18 18:41:35.000000 plot-likert-0.4.1.dev20221009/docs/sample_plot.png
-drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2022-10-09 21:40:17.573147 plot-likert-0.4.1.dev20221009/plot_likert/
--rw-r--r--   0 nmalkin    (501) staff       (20)      185 2022-04-03 05:04:24.000000 plot-likert-0.4.1.dev20221009/plot_likert/__init__.py
--rw-r--r--   0 nmalkin    (501) staff       (20)     1424 2022-04-03 05:04:24.000000 plot-likert-0.4.1.dev20221009/plot_likert/colors.py
--rw-r--r--   0 nmalkin    (501) staff       (20)     2010 2022-10-08 06:08:53.000000 plot-likert-0.4.1.dev20221009/plot_likert/interval.py
--rw-r--r--   0 nmalkin    (501) staff       (20)    15390 2022-10-09 21:38:59.000000 plot-likert-0.4.1.dev20221009/plot_likert/plot_likert.py
--rw-r--r--   0 nmalkin    (501) staff       (20)     2226 2022-04-03 05:04:24.000000 plot-likert-0.4.1.dev20221009/plot_likert/scales.py
-drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2022-10-09 21:40:17.575085 plot-likert-0.4.1.dev20221009/plot_likert.egg-info/
--rw-r--r--   0 nmalkin    (501) staff       (20)     2824 2022-10-09 21:40:17.000000 plot-likert-0.4.1.dev20221009/plot_likert.egg-info/PKG-INFO
--rw-r--r--   0 nmalkin    (501) staff       (20)      506 2022-10-09 21:40:17.000000 plot-likert-0.4.1.dev20221009/plot_likert.egg-info/SOURCES.txt
--rw-r--r--   0 nmalkin    (501) staff       (20)        1 2022-10-09 21:40:17.000000 plot-likert-0.4.1.dev20221009/plot_likert.egg-info/dependency_links.txt
--rw-r--r--   0 nmalkin    (501) staff       (20)       31 2022-10-09 21:40:17.000000 plot-likert-0.4.1.dev20221009/plot_likert.egg-info/requires.txt
--rw-r--r--   0 nmalkin    (501) staff       (20)       18 2022-10-09 21:40:17.000000 plot-likert-0.4.1.dev20221009/plot_likert.egg-info/top_level.txt
--rw-r--r--   0 nmalkin    (501) staff       (20)       31 2022-04-03 05:04:24.000000 plot-likert-0.4.1.dev20221009/requirements.txt
--rw-r--r--   0 nmalkin    (501) staff       (20)       38 2022-10-09 21:40:17.577044 plot-likert-0.4.1.dev20221009/setup.cfg
--rw-r--r--   0 nmalkin    (501) staff       (20)      930 2022-10-09 21:40:02.000000 plot-likert-0.4.1.dev20221009/setup.py
-drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2022-10-09 21:40:17.575712 plot-likert-0.4.1.dev20221009/tests/
--rw-r--r--   0 nmalkin    (501) staff       (20)        0 2020-12-28 02:04:44.000000 plot-likert-0.4.1.dev20221009/tests/__init__.py
--rw-r--r--   0 nmalkin    (501) staff       (20)     1531 2022-04-03 05:04:24.000000 plot-likert-0.4.1.dev20221009/tests/test_interval.py
+drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2023-08-01 05:24:32.276738 plot-likert-0.5.0.dev20230731/
+-rw-r--r--   0 nmalkin    (501) staff       (20)     1454 2023-08-01 05:22:36.000000 plot-likert-0.5.0.dev20230731/LICENSE
+-rw-r--r--   0 nmalkin    (501) staff       (20)     2824 2023-08-01 05:24:32.276425 plot-likert-0.5.0.dev20230731/PKG-INFO
+-rw-r--r--   0 nmalkin    (501) staff       (20)     2225 2022-04-03 05:04:24.000000 plot-likert-0.5.0.dev20230731/README.md
+drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2023-08-01 05:24:32.272784 plot-likert-0.5.0.dev20230731/plot_likert/
+-rw-r--r--   0 nmalkin    (501) staff       (20)      232 2023-07-31 17:33:37.000000 plot-likert-0.5.0.dev20230731/plot_likert/__init__.py
+-rw-r--r--   0 nmalkin    (501) staff       (20)     1424 2022-04-03 05:04:24.000000 plot-likert-0.5.0.dev20230731/plot_likert/colors.py
+-rw-r--r--   0 nmalkin    (501) staff       (20)     2010 2022-10-08 06:08:53.000000 plot-likert-0.5.0.dev20230731/plot_likert/interval.py
+-rw-r--r--   0 nmalkin    (501) staff       (20)    15390 2023-07-31 17:33:29.000000 plot-likert-0.5.0.dev20230731/plot_likert/plot_likert.py
+-rw-r--r--   0 nmalkin    (501) staff       (20)     2226 2022-04-03 05:04:24.000000 plot-likert-0.5.0.dev20230731/plot_likert/scales.py
+drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2023-08-01 05:24:32.275088 plot-likert-0.5.0.dev20230731/plot_likert.egg-info/
+-rw-r--r--   0 nmalkin    (501) staff       (20)     2824 2023-08-01 05:24:32.000000 plot-likert-0.5.0.dev20230731/plot_likert.egg-info/PKG-INFO
+-rw-r--r--   0 nmalkin    (501) staff       (20)      360 2023-08-01 05:24:32.000000 plot-likert-0.5.0.dev20230731/plot_likert.egg-info/SOURCES.txt
+-rw-r--r--   0 nmalkin    (501) staff       (20)        1 2023-08-01 05:24:32.000000 plot-likert-0.5.0.dev20230731/plot_likert.egg-info/dependency_links.txt
+-rw-r--r--   0 nmalkin    (501) staff       (20)       31 2023-08-01 05:24:32.000000 plot-likert-0.5.0.dev20230731/plot_likert.egg-info/requires.txt
+-rw-r--r--   0 nmalkin    (501) staff       (20)       18 2023-08-01 05:24:32.000000 plot-likert-0.5.0.dev20230731/plot_likert.egg-info/top_level.txt
+-rw-r--r--   0 nmalkin    (501) staff       (20)       38 2023-08-01 05:24:32.276853 plot-likert-0.5.0.dev20230731/setup.cfg
+-rw-r--r--   0 nmalkin    (501) staff       (20)      930 2023-08-01 05:20:34.000000 plot-likert-0.5.0.dev20230731/setup.py
+drwxr-xr-x   0 nmalkin    (501) staff       (20)        0 2023-08-01 05:24:32.275853 plot-likert-0.5.0.dev20230731/tests/
+-rw-r--r--   0 nmalkin    (501) staff       (20)        0 2020-12-28 02:04:44.000000 plot-likert-0.5.0.dev20230731/tests/__init__.py
+-rw-r--r--   0 nmalkin    (501) staff       (20)     1531 2022-04-03 05:04:24.000000 plot-likert-0.5.0.dev20230731/tests/test_interval.py
```

### Comparing `plot-likert-0.4.1.dev20221009/LICENSE` & `plot-likert-0.5.0.dev20230731/LICENSE`

 * *Files identical despite different names*

### Comparing `plot-likert-0.4.1.dev20221009/PKG-INFO` & `plot-likert-0.5.0.dev20230731/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-likert
-Version: 0.4.1.dev20221009
+Version: 0.5.0.dev20230731
 Summary: Library to visualize results from Likert-style survey questions
 Home-page: https://github.com/nmalkin/plot-likert
 Author: nmalkin
 Keywords: plot graph visualize likert survey matplotlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `plot-likert-0.4.1.dev20221009/README.md` & `plot-likert-0.5.0.dev20230731/README.md`

 * *Files identical despite different names*

### Comparing `plot-likert-0.4.1.dev20221009/plot_likert/colors.py` & `plot-likert-0.5.0.dev20230731/plot_likert/colors.py`

 * *Files identical despite different names*

### Comparing `plot-likert-0.4.1.dev20221009/plot_likert/interval.py` & `plot-likert-0.5.0.dev20230731/plot_likert/interval.py`

 * *Files identical despite different names*

### Comparing `plot-likert-0.4.1.dev20221009/plot_likert/plot_likert.py` & `plot-likert-0.5.0.dev20230731/plot_likert/plot_likert.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import plot_likert.colors as builtin_colors
 import plot_likert.interval as interval_helper
 
 HIDE_EXCESSIVE_TICK_LABELS = True
 PADDING_LEFT = 0.02  # fraction of the total width to use as padding
 PADDING_RIGHT = 0.04  # fraction of the total width to use as padding
 BAR_LABEL_FORMAT = (
-    "%d"  # if showing labels, how should the number be formatted? e.g., "%.2g"
+    "%g"  # if showing labels, how should the number be formatted? e.g., "%.2g"
 )
 BAR_LABEL_SIZE_CUTOFF = 0.05
 
 
 class PlotLikertError(ValueError):
     pass
```

### Comparing `plot-likert-0.4.1.dev20221009/plot_likert/scales.py` & `plot-likert-0.5.0.dev20230731/plot_likert/scales.py`

 * *Files identical despite different names*

### Comparing `plot-likert-0.4.1.dev20221009/plot_likert.egg-info/PKG-INFO` & `plot-likert-0.5.0.dev20230731/plot_likert.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-likert
-Version: 0.4.1.dev20221009
+Version: 0.5.0.dev20230731
 Summary: Library to visualize results from Likert-style survey questions
 Home-page: https://github.com/nmalkin/plot-likert
 Author: nmalkin
 Keywords: plot graph visualize likert survey matplotlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `plot-likert-0.4.1.dev20221009/setup.py` & `plot-likert-0.5.0.dev20230731/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="plot-likert",
-    version="0.4.1dev20221009",
+    version="0.5.0dev20230731",
     author="nmalkin",
     description="Library to visualize results from Likert-style survey questions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="plot graph visualize likert survey matplotlib",
     url="https://github.com/nmalkin/plot-likert",
     packages=setuptools.find_packages(),
```

### Comparing `plot-likert-0.4.1.dev20221009/tests/test_interval.py` & `plot-likert-0.5.0.dev20230731/tests/test_interval.py`

 * *Files identical despite different names*

