# Comparing `tmp/pilab-regis-0.0.4.tar.gz` & `tmp/pilab-regis-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilab-regis-0.0.4.tar", last modified: Tue Aug  1 13:23:06 2023, max compression
+gzip compressed data, was "pilab-regis-0.0.5.tar", last modified: Tue Aug  1 13:39:53 2023, max compression
```

## Comparing `pilab-regis-0.0.4.tar` & `pilab-regis-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 13:23:06.110000 pilab-regis-0.0.4/
--rw-rw-rw-   0        0        0     2350 2023-08-01 13:23:08.000000 pilab-regis-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2039 2023-03-09 14:32:46.000000 pilab-regis-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 13:23:06.120000 pilab-regis-0.0.4/pilab_regis.egg-info/
--rw-rw-rw-   0        0        0     2350 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 13:23:06.130000 pilab-regis-0.0.4/regis/
--rw-rw-rw-   0        0        0       70 2023-08-01 13:22:32.000000 pilab-regis-0.0.4/regis/__init__.py
--rw-rw-rw-   0        0        0     8866 2023-08-01 13:21:24.000000 pilab-regis-0.0.4/regis/core.py
--rw-rw-rw-   0        0        0       42 2023-08-01 13:23:08.000000 pilab-regis-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-03-02 09:42:46.000000 pilab-regis-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:39:53.890000 pilab-regis-0.0.5/
+-rw-rw-rw-   0        0        0     2350 2023-08-01 13:39:54.000000 pilab-regis-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2039 2023-03-09 14:32:46.000000 pilab-regis-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 13:39:53.900000 pilab-regis-0.0.5/pilab_regis.egg-info/
+-rw-rw-rw-   0        0        0     2350 2023-08-01 13:39:54.000000 pilab-regis-0.0.5/pilab_regis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-08-01 13:39:54.000000 pilab-regis-0.0.5/pilab_regis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:39:54.000000 pilab-regis-0.0.5/pilab_regis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-01 13:39:54.000000 pilab-regis-0.0.5/pilab_regis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 13:39:54.000000 pilab-regis-0.0.5/pilab_regis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 13:39:53.910000 pilab-regis-0.0.5/regis/
+-rw-rw-rw-   0        0        0       70 2023-08-01 13:39:30.000000 pilab-regis-0.0.5/regis/__init__.py
+-rw-rw-rw-   0        0        0     8886 2023-08-01 13:38:58.000000 pilab-regis-0.0.5/regis/core.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 13:39:54.000000 pilab-regis-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-03-02 09:42:46.000000 pilab-regis-0.0.5/setup.py
```

### Comparing `pilab-regis-0.0.4/PKG-INFO` & `pilab-regis-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilab-regis
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/PiLAB-Medical-Imaging/registration
 Author: PiLAB
 Author-email: nicolas.delinte@uclouvain.be
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `pilab-regis-0.0.4/README.md` & `pilab-regis-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pilab-regis-0.0.4/pilab_regis.egg-info/PKG-INFO` & `pilab-regis-0.0.5/pilab_regis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilab-regis
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/PiLAB-Medical-Imaging/registration
 Author: PiLAB
 Author-email: nicolas.delinte@uclouvain.be
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `pilab-regis-0.0.4/regis/core.py` & `pilab-regis-0.0.5/regis/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     if len(moving.shape) > 3:
         moving = moving[:, :, :, 0]
 
     if normalize:
         static = static/np.max(static)
         moving = moving/np.max(moving)
 
-    if hard_static_mask:
+    if type(hard_static_mask) is np.ndarray:
         static *= hard_static_mask
 
     # Affine registration ------------------------------------------------------
 
     if sanity_check or only_affine:
 
         identity = np.eye(4)
```

### Comparing `pilab-regis-0.0.4/setup.py` & `pilab-regis-0.0.5/setup.py`

 * *Files identical despite different names*

