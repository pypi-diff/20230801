# Comparing `tmp/adams_shell_wear-1.0.0.tar.gz` & `tmp/adams_shell_wear-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adams_shell_wear-1.0.0.tar", last modified: Tue Aug  1 17:37:32 2023, max compression
+gzip compressed data, was "adams_shell_wear-1.0.1.tar", last modified: Tue Aug  1 17:39:20 2023, max compression
```

## Comparing `adams_shell_wear-1.0.0.tar` & `adams_shell_wear-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 17:37:32.197769 adams_shell_wear-1.0.0/
--rw-rw-rw-   0        0        0     1091 2022-12-20 23:52:04.000000 adams_shell_wear-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       34 2022-12-20 23:52:04.000000 adams_shell_wear-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      802 2023-08-01 17:37:32.196771 adams_shell_wear-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-08-01 17:01:03.000000 adams_shell_wear-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 17:37:32.115770 adams_shell_wear-1.0.0/adams_shell_wear/
--rw-rw-rw-   0        0        0        0 2022-12-14 19:07:29.000000 adams_shell_wear-1.0.0/adams_shell_wear/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-06 13:31:09.000000 adams_shell_wear-1.0.0/adams_shell_wear/apply.py
--rw-rw-rw-   0        0        0     2198 2023-01-04 21:28:58.000000 adams_shell_wear-1.0.0/adams_shell_wear/archard.py
--rw-rw-rw-   0        0        0     3822 2023-01-09 18:51:31.000000 adams_shell_wear-1.0.0/adams_shell_wear/facets.py
--rw-rw-rw-   0        0        0     3675 2022-12-15 20:00:25.000000 adams_shell_wear-1.0.0/adams_shell_wear/parallel_face_finder.py
--rw-rw-rw-   0        0        0     1168 2022-12-08 21:02:56.000000 adams_shell_wear-1.0.0/adams_shell_wear/tmp.py
-drwxrwxrwx   0        0        0        0 2023-08-01 17:37:32.194772 adams_shell_wear-1.0.0/adams_shell_wear/utils/
--rw-rw-rw-   0        0        0       86 2022-12-15 19:28:36.000000 adams_shell_wear-1.0.0/adams_shell_wear/utils/__init__.py
--rw-rw-rw-   0        0        0     3432 2022-12-06 13:50:12.000000 adams_shell_wear-1.0.0/adams_shell_wear/utils/cs.py
--rw-rw-rw-   0        0        0     5698 2022-12-28 13:22:19.000000 adams_shell_wear-1.0.0/adams_shell_wear/utils/dereferencer.py
--rw-rw-rw-   0        0        0     2627 2023-01-09 21:46:59.000000 adams_shell_wear-1.0.0/adams_shell_wear/utils/plane.py
--rw-rw-rw-   0        0        0     1048 2022-12-21 00:33:37.000000 adams_shell_wear-1.0.0/adams_shell_wear/utils/shell_file.py
--rw-rw-rw-   0        0        0     1975 2023-01-19 14:19:56.000000 adams_shell_wear-1.0.0/adams_shell_wear/utils/utils.py
--rw-rw-rw-   0        0        0     7835 2022-12-21 14:12:09.000000 adams_shell_wear-1.0.0/adams_shell_wear/visualize.py
--rw-rw-rw-   0        0        0    21732 2023-01-26 20:32:20.000000 adams_shell_wear-1.0.0/adams_shell_wear/wearable_shell.py
-drwxrwxrwx   0        0        0        0 2023-08-01 17:37:32.136771 adams_shell_wear-1.0.0/adams_shell_wear.egg-info/
--rw-rw-rw-   0        0        0      802 2023-08-01 17:37:31.000000 adams_shell_wear-1.0.0/adams_shell_wear.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      709 2023-08-01 17:37:31.000000 adams_shell_wear-1.0.0/adams_shell_wear.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 17:37:31.000000 adams_shell_wear-1.0.0/adams_shell_wear.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-08-01 17:37:31.000000 adams_shell_wear-1.0.0/adams_shell_wear.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 17:37:31.000000 adams_shell_wear-1.0.0/adams_shell_wear.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 17:37:32.197769 adams_shell_wear-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1071 2022-12-21 14:20:27.000000 adams_shell_wear-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 17:37:32.195771 adams_shell_wear-1.0.0/test/
--rw-rw-rw-   0        0        0    20463 2023-02-28 20:09:39.000000 adams_shell_wear-1.0.0/test/test_wearable_shell.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:39:20.558718 adams_shell_wear-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2022-12-20 23:52:04.000000 adams_shell_wear-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-12-20 23:52:04.000000 adams_shell_wear-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      803 2023-08-01 17:39:20.558718 adams_shell_wear-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-08-01 17:38:48.000000 adams_shell_wear-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 17:39:20.528719 adams_shell_wear-1.0.1/adams_shell_wear/
+-rw-rw-rw-   0        0        0        0 2022-12-14 19:07:29.000000 adams_shell_wear-1.0.1/adams_shell_wear/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-12-06 13:31:09.000000 adams_shell_wear-1.0.1/adams_shell_wear/apply.py
+-rw-rw-rw-   0        0        0     2198 2023-01-04 21:28:58.000000 adams_shell_wear-1.0.1/adams_shell_wear/archard.py
+-rw-rw-rw-   0        0        0     3822 2023-01-09 18:51:31.000000 adams_shell_wear-1.0.1/adams_shell_wear/facets.py
+-rw-rw-rw-   0        0        0     3675 2022-12-15 20:00:25.000000 adams_shell_wear-1.0.1/adams_shell_wear/parallel_face_finder.py
+-rw-rw-rw-   0        0        0     1168 2022-12-08 21:02:56.000000 adams_shell_wear-1.0.1/adams_shell_wear/tmp.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:39:20.555718 adams_shell_wear-1.0.1/adams_shell_wear/utils/
+-rw-rw-rw-   0        0        0       86 2022-12-15 19:28:36.000000 adams_shell_wear-1.0.1/adams_shell_wear/utils/__init__.py
+-rw-rw-rw-   0        0        0     3432 2022-12-06 13:50:12.000000 adams_shell_wear-1.0.1/adams_shell_wear/utils/cs.py
+-rw-rw-rw-   0        0        0     5698 2022-12-28 13:22:19.000000 adams_shell_wear-1.0.1/adams_shell_wear/utils/dereferencer.py
+-rw-rw-rw-   0        0        0     2627 2023-01-09 21:46:59.000000 adams_shell_wear-1.0.1/adams_shell_wear/utils/plane.py
+-rw-rw-rw-   0        0        0     1048 2022-12-21 00:33:37.000000 adams_shell_wear-1.0.1/adams_shell_wear/utils/shell_file.py
+-rw-rw-rw-   0        0        0     1975 2023-01-19 14:19:56.000000 adams_shell_wear-1.0.1/adams_shell_wear/utils/utils.py
+-rw-rw-rw-   0        0        0     7835 2022-12-21 14:12:09.000000 adams_shell_wear-1.0.1/adams_shell_wear/visualize.py
+-rw-rw-rw-   0        0        0    21732 2023-01-26 20:32:20.000000 adams_shell_wear-1.0.1/adams_shell_wear/wearable_shell.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:39:20.547719 adams_shell_wear-1.0.1/adams_shell_wear.egg-info/
+-rw-rw-rw-   0        0        0      803 2023-08-01 17:39:20.000000 adams_shell_wear-1.0.1/adams_shell_wear.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      709 2023-08-01 17:39:20.000000 adams_shell_wear-1.0.1/adams_shell_wear.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 17:39:20.000000 adams_shell_wear-1.0.1/adams_shell_wear.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-01 17:39:20.000000 adams_shell_wear-1.0.1/adams_shell_wear.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 17:39:20.000000 adams_shell_wear-1.0.1/adams_shell_wear.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 17:39:20.559719 adams_shell_wear-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2022-12-21 14:20:27.000000 adams_shell_wear-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:39:20.556719 adams_shell_wear-1.0.1/test/
+-rw-rw-rw-   0        0        0    20463 2023-02-28 20:09:39.000000 adams_shell_wear-1.0.1/test/test_wearable_shell.py
```

### Comparing `adams_shell_wear-1.0.0/LICENSE` & `adams_shell_wear-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/PKG-INFO` & `adams_shell_wear-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adams_shell_wear
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python tools for calculating and applying wear to shell geometry in Adams
 Home-page: https://github.com/bthornton191/adams_shell_wear
 Author: Ben Thornton
 Author-email: ben.thornton@hexagon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,12 +15,12 @@
 
 Python tools for calculating and applying wear to shell geometry in [Adams](https://hexagon.com/products/product-groups/computer-aided-engineering-software/adams).
 
 ## Installation
 
 Install straight from the repo using pip.
 ```
-> pip installadams_shell_wear
+> pip install adams_shell_wear
 ```
 
 ## Usage
 > TBD
```

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/archard.py` & `adams_shell_wear-1.0.1/adams_shell_wear/archard.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/facets.py` & `adams_shell_wear-1.0.1/adams_shell_wear/facets.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/parallel_face_finder.py` & `adams_shell_wear-1.0.1/adams_shell_wear/parallel_face_finder.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/tmp.py` & `adams_shell_wear-1.0.1/adams_shell_wear/tmp.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/utils/cs.py` & `adams_shell_wear-1.0.1/adams_shell_wear/utils/cs.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/utils/dereferencer.py` & `adams_shell_wear-1.0.1/adams_shell_wear/utils/dereferencer.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/utils/plane.py` & `adams_shell_wear-1.0.1/adams_shell_wear/utils/plane.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/utils/shell_file.py` & `adams_shell_wear-1.0.1/adams_shell_wear/utils/shell_file.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/utils/utils.py` & `adams_shell_wear-1.0.1/adams_shell_wear/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/visualize.py` & `adams_shell_wear-1.0.1/adams_shell_wear/visualize.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear/wearable_shell.py` & `adams_shell_wear-1.0.1/adams_shell_wear/wearable_shell.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear.egg-info/PKG-INFO` & `adams_shell_wear-1.0.1/adams_shell_wear.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adams-shell-wear
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python tools for calculating and applying wear to shell geometry in Adams
 Home-page: https://github.com/bthornton191/adams_shell_wear
 Author: Ben Thornton
 Author-email: ben.thornton@hexagon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,12 +15,12 @@
 
 Python tools for calculating and applying wear to shell geometry in [Adams](https://hexagon.com/products/product-groups/computer-aided-engineering-software/adams).
 
 ## Installation
 
 Install straight from the repo using pip.
 ```
-> pip installadams_shell_wear
+> pip install adams_shell_wear
 ```
 
 ## Usage
 > TBD
```

### Comparing `adams_shell_wear-1.0.0/adams_shell_wear.egg-info/SOURCES.txt` & `adams_shell_wear-1.0.1/adams_shell_wear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/setup.py` & `adams_shell_wear-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `adams_shell_wear-1.0.0/test/test_wearable_shell.py` & `adams_shell_wear-1.0.1/test/test_wearable_shell.py`

 * *Files identical despite different names*

