# Comparing `tmp/photcalib-0.1.tar.gz` & `tmp/photcalib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photcalib-0.1.tar", last modified: Tue May 30 12:54:04 2023, max compression
+gzip compressed data, was "photcalib-0.2.tar", last modified: Tue Aug  1 14:11:47 2023, max compression
```

## Comparing `photcalib-0.1.tar` & `photcalib-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-30 12:54:04.651829 photcalib-0.1/
--rw-r--r--   0 zyuan      (502) staff       (20)     1089 2023-05-19 07:26:16.000000 photcalib-0.1/LICENSE
--rw-r--r--   0 zyuan      (502) staff       (20)     2463 2023-05-30 12:54:04.651690 photcalib-0.1/PKG-INFO
--rw-r--r--   0 zyuan      (502) staff       (20)     1979 2023-05-19 14:44:00.000000 photcalib-0.1/README.rst
-drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-30 12:54:04.650646 photcalib-0.1/photcalib/
--rw-r--r--   0 zyuan      (502) staff       (20)      493 2023-05-30 12:45:58.000000 photcalib-0.1/photcalib/__init__.py
--rw-r--r--   0 zyuan      (502) staff       (20)     1878 2023-05-30 12:52:57.000000 photcalib-0.1/photcalib/apply_calib.py
--rw-r--r--   0 zyuan      (502) staff       (20)     1900 2023-05-30 12:52:21.000000 photcalib-0.1/photcalib/deform_norm.py
--rw-r--r--   0 zyuan      (502) staff       (20)    28842 2023-05-30 12:46:47.000000 photcalib-0.1/photcalib/make_plots.py
--rw-r--r--   0 zyuan      (502) staff       (20)     1277 2023-05-19 06:50:53.000000 photcalib-0.1/photcalib/model_old.py
--rw-r--r--   0 zyuan      (502) staff       (20)     3456 2023-05-19 07:01:27.000000 photcalib-0.1/photcalib/set_argparse.py
--rw-r--r--   0 zyuan      (502) staff       (20)     6281 2023-05-19 07:05:19.000000 photcalib-0.1/photcalib/training.py
-drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-05-30 12:54:04.651500 photcalib-0.1/photcalib.egg-info/
--rw-r--r--   0 zyuan      (502) staff       (20)     2463 2023-05-30 12:54:04.000000 photcalib-0.1/photcalib.egg-info/PKG-INFO
--rw-r--r--   0 zyuan      (502) staff       (20)      358 2023-05-30 12:54:04.000000 photcalib-0.1/photcalib.egg-info/SOURCES.txt
--rw-r--r--   0 zyuan      (502) staff       (20)        1 2023-05-30 12:54:04.000000 photcalib-0.1/photcalib.egg-info/dependency_links.txt
--rw-r--r--   0 zyuan      (502) staff       (20)        1 2023-05-18 09:18:41.000000 photcalib-0.1/photcalib.egg-info/not-zip-safe
--rw-r--r--   0 zyuan      (502) staff       (20)       10 2023-05-30 12:54:04.000000 photcalib-0.1/photcalib.egg-info/top_level.txt
--rw-r--r--   0 zyuan      (502) staff       (20)       38 2023-05-30 12:54:04.651873 photcalib-0.1/setup.cfg
--rw-r--r--   0 zyuan      (502) staff       (20)      766 2023-05-19 16:02:16.000000 photcalib-0.1/setup.py
+drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-08-01 14:11:47.571084 photcalib-0.2/
+-rw-r--r--   0 zyuan      (502) staff       (20)     1089 2023-05-19 07:26:16.000000 photcalib-0.2/LICENSE
+-rw-r--r--   0 zyuan      (502) staff       (20)     2421 2023-08-01 14:11:47.570952 photcalib-0.2/PKG-INFO
+-rw-r--r--   0 zyuan      (502) staff       (20)     1937 2023-05-30 13:11:04.000000 photcalib-0.2/README.rst
+drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-08-01 14:11:47.570067 photcalib-0.2/photcalib/
+-rw-r--r--   0 zyuan      (502) staff       (20)      493 2023-05-30 12:45:58.000000 photcalib-0.2/photcalib/__init__.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     1592 2023-08-01 14:11:17.000000 photcalib-0.2/photcalib/apply_calib.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     1900 2023-05-30 12:52:21.000000 photcalib-0.2/photcalib/deform_norm.py
+-rw-r--r--   0 zyuan      (502) staff       (20)    28842 2023-05-30 12:46:47.000000 photcalib-0.2/photcalib/make_plots.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     1277 2023-05-19 06:50:53.000000 photcalib-0.2/photcalib/model_old.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     3456 2023-08-01 14:05:50.000000 photcalib-0.2/photcalib/set_argparse.py
+-rw-r--r--   0 zyuan      (502) staff       (20)     6281 2023-05-19 07:05:19.000000 photcalib-0.2/photcalib/training.py
+drwxr-xr-x   0 zyuan      (502) staff       (20)        0 2023-08-01 14:11:47.570767 photcalib-0.2/photcalib.egg-info/
+-rw-r--r--   0 zyuan      (502) staff       (20)     2421 2023-08-01 14:11:47.000000 photcalib-0.2/photcalib.egg-info/PKG-INFO
+-rw-r--r--   0 zyuan      (502) staff       (20)      358 2023-08-01 14:11:47.000000 photcalib-0.2/photcalib.egg-info/SOURCES.txt
+-rw-r--r--   0 zyuan      (502) staff       (20)        1 2023-08-01 14:11:47.000000 photcalib-0.2/photcalib.egg-info/dependency_links.txt
+-rw-r--r--   0 zyuan      (502) staff       (20)        1 2023-05-18 09:18:41.000000 photcalib-0.2/photcalib.egg-info/not-zip-safe
+-rw-r--r--   0 zyuan      (502) staff       (20)       10 2023-08-01 14:11:47.000000 photcalib-0.2/photcalib.egg-info/top_level.txt
+-rw-r--r--   0 zyuan      (502) staff       (20)       38 2023-08-01 14:11:47.571122 photcalib-0.2/setup.cfg
+-rw-r--r--   0 zyuan      (502) staff       (20)      766 2023-08-01 14:06:46.000000 photcalib-0.2/setup.py
```

### Comparing `photcalib-0.1/LICENSE` & `photcalib-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `photcalib-0.1/PKG-INFO` & `photcalib-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photcalib
-Version: 0.1
+Version: 0.2
 Summary: calibration tool for photometric data
 Home-page: https://github.com/zyuan-astro/PhotCalib
 Author: Zhen Yuan
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
@@ -66,19 +66,19 @@
 
   cd examples
  
 
 To Calibrate CaHK data using the run model trained by the main survey:
 .. code::
 
-  python calib_raw.py 17Am05 combined_catalogue_17Am05_sel.fits -D device
+  python calib_raw.py 17Am05 combined_catalogue_17Am05_sel.fits -D cpu
  
 Substitute 17Am05 to the run you need and make sure the input data for calibration has the same format as that in the examples/data/.fits
 
-* D (str) is the device (default:cpu, mps, gpu) to run pytorch. mps is not faster than cpu on M1. If gpu is chosen, it will use the first graphic card cuda:0 by default.
+* D (str) is the device (default:cpu, gpu) to run pytorch. If gpu is chosen, it will use the first graphic card cuda:0 by default.
 
 
 To train calibration run model:
 .. code::
 
   python calib_mod.py 17Am05
```

### Comparing `photcalib-0.1/README.rst` & `photcalib-0.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -51,19 +51,19 @@
 
   cd examples
  
 
 To Calibrate CaHK data using the run model trained by the main survey:
 .. code::
 
-  python calib_raw.py 17Am05 combined_catalogue_17Am05_sel.fits -D device
+  python calib_raw.py 17Am05 combined_catalogue_17Am05_sel.fits -D cpu
  
 Substitute 17Am05 to the run you need and make sure the input data for calibration has the same format as that in the examples/data/.fits
 
-* D (str) is the device (default:cpu, mps, gpu) to run pytorch. mps is not faster than cpu on M1. If gpu is chosen, it will use the first graphic card cuda:0 by default.
+* D (str) is the device (default:cpu, gpu) to run pytorch. If gpu is chosen, it will use the first graphic card cuda:0 by default.
 
 
 To train calibration run model:
 .. code::
 
   python calib_mod.py 17Am05
```

### Comparing `photcalib-0.1/photcalib/apply_calib.py` & `photcalib-0.2/photcalib/apply_calib.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,38 +34,32 @@
 
     z_new = zn-dz
    
     return dz_fov, z_new
     
 def generate_newcat(DEVICE, mod, p):
      
-      
-    batch_size = 1000
-    num_batches = int(len(p) / batch_size)
+  
+    fn_nb = p['image_nb']
+    fn_nb_list = np.unique(fn_nb)
+
+    # p['run'] = run
     
+
     dz_fov = np.array([0])
     z_new = np.array([0])
-    
+        
     tic = time.perf_counter()
     
-    for batch in range(num_batches):
-        
-        batch_p = p[batch*batch_size:(batch+1)*batch_size]   
-        batch_dz_fov, batch_z_new = add_correction(DEVICE, batch_p, mod)
-        
-        
-        dz_fov = np.append(dz_fov, batch_dz_fov)
-        z_new = np.append(z_new, batch_z_new)
-        
-    if len(p) - (batch+1)*batch_size > 0:
-        
-        batch_p = p[(batch+1)*batch_size:] 
+    for i in range(len(fn_nb_list)):
+
+        ind = fn_nb == fn_nb_list[i]
+        batch_p = p[ind]   
         batch_dz_fov, batch_z_new = add_correction(DEVICE, batch_p, mod)
         
-        
         dz_fov = np.append(dz_fov, batch_dz_fov)
         z_new = np.append(z_new, batch_z_new)
         
         
     toc = time.perf_counter()
     
     print(f"Apply the model in {toc - tic:0.4f} seconds")
```

### Comparing `photcalib-0.1/photcalib/deform_norm.py` & `photcalib-0.2/photcalib/deform_norm.py`

 * *Files identical despite different names*

### Comparing `photcalib-0.1/photcalib/make_plots.py` & `photcalib-0.2/photcalib/make_plots.py`

 * *Files identical despite different names*

### Comparing `photcalib-0.1/photcalib/model_old.py` & `photcalib-0.2/photcalib/model_old.py`

 * *Files identical despite different names*

### Comparing `photcalib-0.1/photcalib/set_argparse.py` & `photcalib-0.2/photcalib/set_argparse.py`

 * *Files identical despite different names*

### Comparing `photcalib-0.1/photcalib/training.py` & `photcalib-0.2/photcalib/training.py`

 * *Files identical despite different names*

### Comparing `photcalib-0.1/photcalib.egg-info/PKG-INFO` & `photcalib-0.2/photcalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photcalib
-Version: 0.1
+Version: 0.2
 Summary: calibration tool for photometric data
 Home-page: https://github.com/zyuan-astro/PhotCalib
 Author: Zhen Yuan
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
@@ -66,19 +66,19 @@
 
   cd examples
  
 
 To Calibrate CaHK data using the run model trained by the main survey:
 .. code::
 
-  python calib_raw.py 17Am05 combined_catalogue_17Am05_sel.fits -D device
+  python calib_raw.py 17Am05 combined_catalogue_17Am05_sel.fits -D cpu
  
 Substitute 17Am05 to the run you need and make sure the input data for calibration has the same format as that in the examples/data/.fits
 
-* D (str) is the device (default:cpu, mps, gpu) to run pytorch. mps is not faster than cpu on M1. If gpu is chosen, it will use the first graphic card cuda:0 by default.
+* D (str) is the device (default:cpu, gpu) to run pytorch. If gpu is chosen, it will use the first graphic card cuda:0 by default.
 
 
 To train calibration run model:
 .. code::
 
   python calib_mod.py 17Am05
```

### Comparing `photcalib-0.1/setup.py` & `photcalib-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(name = "photcalib",
-    version = 0.1,
+    version = 0.2,
     description = "calibration tool for photometric data",
     long_description = readme(),
     long_description_content_type="text/x-rst",
     author = "Zhen Yuan",
     author_email = "",
     url = "https://github.com/zyuan-astro/PhotCalib",
     packages = find_packages(),
```

