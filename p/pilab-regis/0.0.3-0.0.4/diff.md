# Comparing `tmp/pilab-regis-0.0.3.tar.gz` & `tmp/pilab-regis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilab-regis-0.0.3.tar", last modified: Tue Jul 11 08:34:29 2023, max compression
+gzip compressed data, was "pilab-regis-0.0.4.tar", last modified: Tue Aug  1 13:23:06 2023, max compression
```

## Comparing `pilab-regis-0.0.3.tar` & `pilab-regis-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 08:34:29.330000 pilab-regis-0.0.3/
--rw-rw-rw-   0        0        0     2350 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2039 2023-03-09 14:32:46.000000 pilab-regis-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 08:34:29.340000 pilab-regis-0.0.3/pilab_regis.egg-info/
--rw-rw-rw-   0        0        0     2350 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 08:34:29.350000 pilab-regis-0.0.3/regis/
--rw-rw-rw-   0        0        0       70 2023-07-11 08:33:34.000000 pilab-regis-0.0.3/regis/__init__.py
--rw-rw-rw-   0        0        0     8611 2023-04-06 12:42:04.000000 pilab-regis-0.0.3/regis/core.py
--rw-rw-rw-   0        0        0       42 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-03-02 09:42:46.000000 pilab-regis-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:23:06.110000 pilab-regis-0.0.4/
+-rw-rw-rw-   0        0        0     2350 2023-08-01 13:23:08.000000 pilab-regis-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2039 2023-03-09 14:32:46.000000 pilab-regis-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 13:23:06.120000 pilab-regis-0.0.4/pilab_regis.egg-info/
+-rw-rw-rw-   0        0        0     2350 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 13:23:06.000000 pilab-regis-0.0.4/pilab_regis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 13:23:06.130000 pilab-regis-0.0.4/regis/
+-rw-rw-rw-   0        0        0       70 2023-08-01 13:22:32.000000 pilab-regis-0.0.4/regis/__init__.py
+-rw-rw-rw-   0        0        0     8866 2023-08-01 13:21:24.000000 pilab-regis-0.0.4/regis/core.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 13:23:08.000000 pilab-regis-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-03-02 09:42:46.000000 pilab-regis-0.0.4/setup.py
```

### Comparing `pilab-regis-0.0.3/PKG-INFO` & `pilab-regis-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilab-regis
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/PiLAB-Medical-Imaging/registration
 Author: PiLAB
 Author-email: nicolas.delinte@uclouvain.be
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `pilab-regis-0.0.3/README.md` & `pilab-regis-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pilab-regis-0.0.3/pilab_regis.egg-info/PKG-INFO` & `pilab-regis-0.0.4/pilab_regis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilab-regis
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/PiLAB-Medical-Imaging/registration
 Author: PiLAB
 Author-email: nicolas.delinte@uclouvain.be
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `pilab-regis-0.0.3/regis/core.py` & `pilab-regis-0.0.4/regis/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 from dipy.align.imwarp import SymmetricDiffeomorphicRegistration
 
 
 def find_transform(moving_file: str, static_file: str,
                    only_affine: bool = False, diffeomorph: bool = True,
                    level_iters_diff=[10000, 1000, 100],
                    sanity_check: bool = False, normalize: bool = False,
-                   static_mask=None, moving_mask=None):
+                   static_mask=None, moving_mask=None,
+                   hard_static_mask=None):
     '''
     If volume are 4D+, only the first 3D volume is taken into account.
 
     Parameters
     ----------
     moving_file : str
         3D array of moving volume.
@@ -46,14 +47,17 @@
         improves robustness of registration. The default is False.
     static_mask : array, optional
         Static image mask that defines which pixels in the static image
         are used to calculate the mutual information.
     moving_mask : array, optional
         Moving image mask that defines which pixels in the moving image
         are used to calculate the mutual information.
+    hard_static_mask : array, optional
+        Static image mask that defines which pixels in the static image
+        are not set to 0 (black).
 
     Returns
     -------
     mapping : TYPE
         transform operation to send moving_volume to static_volume space.
 
     '''
@@ -68,14 +72,17 @@
     if len(moving.shape) > 3:
         moving = moving[:, :, :, 0]
 
     if normalize:
         static = static/np.max(static)
         moving = moving/np.max(moving)
 
+    if hard_static_mask:
+        static *= hard_static_mask
+
     # Affine registration ------------------------------------------------------
 
     if sanity_check or only_affine:
 
         identity = np.eye(4)
         affine_map = AffineMap(identity,
                                static.shape, static_grid2world,
```

### Comparing `pilab-regis-0.0.3/setup.py` & `pilab-regis-0.0.4/setup.py`

 * *Files identical despite different names*

