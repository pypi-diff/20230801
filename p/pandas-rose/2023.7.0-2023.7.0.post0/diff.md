# Comparing `tmp/pandas-rose-2023.7.0.tar.gz` & `tmp/pandas-rose-2023.7.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-rose-2023.7.0.tar", last modified: Tue Aug  1 05:35:41 2023, max compression
+gzip compressed data, was "pandas-rose-2023.7.0.post0.tar", last modified: Tue Aug  1 05:20:17 2023, max compression
```

## Comparing `pandas-rose-2023.7.0.tar` & `pandas-rose-2023.7.0.post0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.460889 pandas-rose-2023.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.456889 pandas-rose-2023.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.456889 pandas-rose-2023.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/.github/workflows/release-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.456889 pandas-rose-2023.7.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/HOW_TO_RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-01 05:35:41.460889 pandas-rose-2023.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   338948 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.456889 pandas-rose-2023.7.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   532263 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/images/pandas-rose.png
--rw-r--r--   0 runner    (1001) docker     (123)    45880 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/images/sample_bar.png
--rw-r--r--   0 runner    (1001) docker     (123)    90999 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/images/sample_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    41538 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/images/sample_table.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.456889 pandas-rose-2023.7.0/pandas_rose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-01 05:35:41.000000 pandas-rose-2023.7.0/pandas_rose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 05:35:41.000000 pandas-rose-2023.7.0/pandas_rose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:35:41.000000 pandas-rose-2023.7.0/pandas_rose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 05:35:41.000000 pandas-rose-2023.7.0/pandas_rose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 05:35:41.000000 pandas-rose-2023.7.0/pandas_rose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.456889 pandas-rose-2023.7.0/rose/
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/rose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.456889 pandas-rose-2023.7.0/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)   117589 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/sample_data/WBB.csv
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 05:35:41.460889 pandas-rose-2023.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:41.460889 pandas-rose-2023.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 05:35:25.000000 pandas-rose-2023.7.0/tests/test_rose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.859776 pandas-rose-2023.7.0.post0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.851776 pandas-rose-2023.7.0.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/.github/workflows/release-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/HOW_TO_RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   338948 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   532263 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/images/pandas-rose.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45880 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/images/sample_bar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90999 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/images/sample_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41538 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/images/sample_table.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/rose/
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/rose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/rose/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   117589 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/sample_data/WBB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 05:20:17.859776 pandas-rose-2023.7.0.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/tests/test_rose.py
```

### Comparing `pandas-rose-2023.7.0/.github/workflows/release-and-publish.yml` & `pandas-rose-2023.7.0.post0/.github/workflows/release-and-publish.yml`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/LICENSE` & `pandas-rose-2023.7.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/PKG-INFO` & `pandas-rose-2023.7.0.post0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-rose
-Version: 2023.7.0
+Version: 2023.7.0.post0
 Summary: A simple Pandas accessor to make windrose plots.
 Author-email: Brian Blaylock <blaylockbk@gmail.com>
 Maintainer-email: Brian Blaylock <blaylockbk@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Brian K. Blaylock
         
@@ -36,15 +36,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 <div align=center>
 
-<img src="https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
+<img src="images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
 
 </div>
 
 # Pandas Rose
 
 This python package adds a custom Pandas accessor to generate polar wind rose plots from a Pandas dataframe.
 
@@ -75,15 +75,15 @@
     "wind_direction":[20, 10, 190,300]
 })
 
 # Display a polar wind plot of the data
 df.rose.plot()
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_plot.png)
+![Alt text](images/sample_plot.png)
 
 You can specify the pandas column to use for wind direction and wind speed. You may also change the number of sectors to bin the wind direction .
 
 ```python
 df.rose.plot(
     var_column="A",    # name of variable column
     dir_column="B",    # name of direction column
@@ -97,15 +97,15 @@
 There are two other accessors that give some information.
 
 ```python
 # Display a dataframe of the binned values
 df.rose.table(sectors=8)
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_table.png)
+![Alt text](images/sample_table.png)
 
 ```python
 # Display the binned data as bar graph on regular axes.
 df.rose.bar()
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_bar.png)
+![Alt text](images/sample_bar.png)
```

### Comparing `pandas-rose-2023.7.0/README.md` & `pandas-rose-2023.7.0.post0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align=center>
 
-<img src="https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
+<img src="images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
 
 </div>
 
 # Pandas Rose
 
 This python package adds a custom Pandas accessor to generate polar wind rose plots from a Pandas dataframe.
 
@@ -35,15 +35,15 @@
     "wind_direction":[20, 10, 190,300]
 })
 
 # Display a polar wind plot of the data
 df.rose.plot()
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_plot.png)
+![Alt text](images/sample_plot.png)
 
 You can specify the pandas column to use for wind direction and wind speed. You may also change the number of sectors to bin the wind direction .
 
 ```python
 df.rose.plot(
     var_column="A",    # name of variable column
     dir_column="B",    # name of direction column
@@ -57,15 +57,15 @@
 There are two other accessors that give some information.
 
 ```python
 # Display a dataframe of the binned values
 df.rose.table(sectors=8)
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_table.png)
+![Alt text](images/sample_table.png)
 
 ```python
 # Display the binned data as bar graph on regular axes.
 df.rose.bar()
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_bar.png)
+![Alt text](images/sample_bar.png)
```

### Comparing `pandas-rose-2023.7.0/demo.ipynb` & `pandas-rose-2023.7.0.post0/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/images/pandas-rose.png` & `pandas-rose-2023.7.0.post0/images/pandas-rose.png`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/images/sample_bar.png` & `pandas-rose-2023.7.0.post0/images/sample_bar.png`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/images/sample_plot.png` & `pandas-rose-2023.7.0.post0/images/sample_plot.png`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/images/sample_table.png` & `pandas-rose-2023.7.0.post0/images/sample_table.png`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/pandas_rose.egg-info/PKG-INFO` & `pandas-rose-2023.7.0.post0/pandas_rose.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-rose
-Version: 2023.7.0
+Version: 2023.7.0.post0
 Summary: A simple Pandas accessor to make windrose plots.
 Author-email: Brian Blaylock <blaylockbk@gmail.com>
 Maintainer-email: Brian Blaylock <blaylockbk@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Brian K. Blaylock
         
@@ -36,15 +36,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 <div align=center>
 
-<img src="https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
+<img src="images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
 
 </div>
 
 # Pandas Rose
 
 This python package adds a custom Pandas accessor to generate polar wind rose plots from a Pandas dataframe.
 
@@ -75,15 +75,15 @@
     "wind_direction":[20, 10, 190,300]
 })
 
 # Display a polar wind plot of the data
 df.rose.plot()
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_plot.png)
+![Alt text](images/sample_plot.png)
 
 You can specify the pandas column to use for wind direction and wind speed. You may also change the number of sectors to bin the wind direction .
 
 ```python
 df.rose.plot(
     var_column="A",    # name of variable column
     dir_column="B",    # name of direction column
@@ -97,15 +97,15 @@
 There are two other accessors that give some information.
 
 ```python
 # Display a dataframe of the binned values
 df.rose.table(sectors=8)
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_table.png)
+![Alt text](images/sample_table.png)
 
 ```python
 # Display the binned data as bar graph on regular axes.
 df.rose.bar()
 ```
 
-![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_bar.png)
+![Alt text](images/sample_bar.png)
```

### Comparing `pandas-rose-2023.7.0/pyproject.toml` & `pandas-rose-2023.7.0.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/rose/__init__.py` & `pandas-rose-2023.7.0.post0/rose/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0/sample_data/WBB.csv` & `pandas-rose-2023.7.0.post0/sample_data/WBB.csv`

 * *Files identical despite different names*

