# Comparing `tmp/h5_to_edf-1.0.1.tar.gz` & `tmp/h5_to_edf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5_to_edf-1.0.1.tar", last modified: Tue Jul 11 11:51:25 2023, max compression
+gzip compressed data, was "h5_to_edf-1.0.2.tar", last modified: Tue Aug  1 12:35:42 2023, max compression
```

## Comparing `h5_to_edf-1.0.1.tar` & `h5_to_edf-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mammeri  (201685) soft      (3401)        0 2023-07-11 11:51:25.908046 h5_to_edf-1.0.1/
--rw-r--r--   0 mammeri  (201685) soft      (3401)      968 2023-07-11 11:51:25.908046 h5_to_edf-1.0.1/PKG-INFO
--rw-r--r--   0 mammeri  (201685) soft      (3401)      467 2023-07-11 11:45:56.000000 h5_to_edf-1.0.1/README.rst
--rw-r--r--   0 mammeri  (201685) soft      (3401)      920 2023-07-11 11:45:56.000000 h5_to_edf-1.0.1/pyproject.toml
--rw-r--r--   0 mammeri  (201685) soft      (3401)       38 2023-07-11 11:51:25.908046 h5_to_edf-1.0.1/setup.cfg
-drwxr-xr-x   0 mammeri  (201685) soft      (3401)        0 2023-07-11 11:51:25.908046 h5_to_edf-1.0.1/src/
-drwxr-xr-x   0 mammeri  (201685) soft      (3401)        0 2023-07-11 11:51:25.908046 h5_to_edf-1.0.1/src/h5_to_edf/
--rw-r--r--   0 mammeri  (201685) soft      (3401)       47 2023-07-11 11:45:56.000000 h5_to_edf-1.0.1/src/h5_to_edf/__init__.py
--rw-r--r--   0 mammeri  (201685) soft      (3401)    35601 2023-07-11 11:45:56.000000 h5_to_edf-1.0.1/src/h5_to_edf/converter.py
--rw-r--r--   0 mammeri  (201685) soft      (3401)    34920 2023-07-11 11:45:56.000000 h5_to_edf-1.0.1/src/h5_to_edf/converter_oven.py
-drwxr-xr-x   0 mammeri  (201685) soft      (3401)        0 2023-07-11 11:51:25.908046 h5_to_edf-1.0.1/src/h5_to_edf.egg-info/
--rw-r--r--   0 mammeri  (201685) soft      (3401)      968 2023-07-11 11:51:25.000000 h5_to_edf-1.0.1/src/h5_to_edf.egg-info/PKG-INFO
--rw-r--r--   0 mammeri  (201685) soft      (3401)      334 2023-07-11 11:51:25.000000 h5_to_edf-1.0.1/src/h5_to_edf.egg-info/SOURCES.txt
--rw-r--r--   0 mammeri  (201685) soft      (3401)        1 2023-07-11 11:51:25.000000 h5_to_edf-1.0.1/src/h5_to_edf.egg-info/dependency_links.txt
--rw-r--r--   0 mammeri  (201685) soft      (3401)       62 2023-07-11 11:51:25.000000 h5_to_edf-1.0.1/src/h5_to_edf.egg-info/entry_points.txt
--rw-r--r--   0 mammeri  (201685) soft      (3401)       22 2023-07-11 11:51:25.000000 h5_to_edf-1.0.1/src/h5_to_edf.egg-info/requires.txt
--rw-r--r--   0 mammeri  (201685) soft      (3401)       10 2023-07-11 11:51:25.000000 h5_to_edf-1.0.1/src/h5_to_edf.egg-info/top_level.txt
+drwxr-xr-x   0 mammeri  (201685) soft      (3401)        0 2023-08-01 12:35:42.617624 h5_to_edf-1.0.2/
+-rw-r--r--   0 mammeri  (201685) soft      (3401)      974 2023-08-01 12:35:42.617624 h5_to_edf-1.0.2/PKG-INFO
+-rw-r--r--   0 mammeri  (201685) soft      (3401)      474 2023-08-01 12:32:28.000000 h5_to_edf-1.0.2/README.rst
+-rw-r--r--   0 mammeri  (201685) soft      (3401)      920 2023-08-01 12:32:05.000000 h5_to_edf-1.0.2/pyproject.toml
+-rw-r--r--   0 mammeri  (201685) soft      (3401)       38 2023-08-01 12:35:42.617624 h5_to_edf-1.0.2/setup.cfg
+drwxr-xr-x   0 mammeri  (201685) soft      (3401)        0 2023-08-01 12:35:42.613624 h5_to_edf-1.0.2/src/
+drwxr-xr-x   0 mammeri  (201685) soft      (3401)        0 2023-08-01 12:35:42.613624 h5_to_edf-1.0.2/src/h5_to_edf/
+-rw-r--r--   0 mammeri  (201685) soft      (3401)       47 2023-08-01 12:35:01.000000 h5_to_edf-1.0.2/src/h5_to_edf/__init__.py
+-rw-r--r--   0 mammeri  (201685) soft      (3401)    35960 2023-08-01 12:32:09.000000 h5_to_edf-1.0.2/src/h5_to_edf/converter.py
+-rw-r--r--   0 mammeri  (201685) soft      (3401)    34920 2023-08-01 12:32:05.000000 h5_to_edf-1.0.2/src/h5_to_edf/converter_oven.py
+drwxr-xr-x   0 mammeri  (201685) soft      (3401)        0 2023-08-01 12:35:42.617624 h5_to_edf-1.0.2/src/h5_to_edf.egg-info/
+-rw-r--r--   0 mammeri  (201685) soft      (3401)      974 2023-08-01 12:35:42.000000 h5_to_edf-1.0.2/src/h5_to_edf.egg-info/PKG-INFO
+-rw-r--r--   0 mammeri  (201685) soft      (3401)      334 2023-08-01 12:35:42.000000 h5_to_edf-1.0.2/src/h5_to_edf.egg-info/SOURCES.txt
+-rw-r--r--   0 mammeri  (201685) soft      (3401)        1 2023-08-01 12:35:42.000000 h5_to_edf-1.0.2/src/h5_to_edf.egg-info/dependency_links.txt
+-rw-r--r--   0 mammeri  (201685) soft      (3401)       62 2023-08-01 12:35:42.000000 h5_to_edf-1.0.2/src/h5_to_edf.egg-info/entry_points.txt
+-rw-r--r--   0 mammeri  (201685) soft      (3401)       22 2023-08-01 12:35:42.000000 h5_to_edf-1.0.2/src/h5_to_edf.egg-info/requires.txt
+-rw-r--r--   0 mammeri  (201685) soft      (3401)       10 2023-08-01 12:35:42.000000 h5_to_edf-1.0.2/src/h5_to_edf.egg-info/top_level.txt
```

### Comparing `h5_to_edf-1.0.1/PKG-INFO` & `h5_to_edf-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5_to_edf
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert a HDF5 file to EDF files
 Author-email: Jibril MAMMERI <mammeri@esrf.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.esrf.fr/mammeri/h5_to_edf
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/mammeri/h5_to_edf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,12 +22,12 @@
 
 How to use
 ~~~~~~~~~~
 
 The converter needs the name of the hdf5 file to be converted, and the output directory where the EDF files will
 be created.
 
-``convert_to_edf "path/file_001.h5" output_directory``
+``convert_to_edf "path/file_001.h5" -o output_directory``
 
 You can also convert multiple hdf5 files at once with the following command:
 
-``convert_to_edf "path/file_0*.h5" output_directory``
+``convert_to_edf "path/file_0*.h5" -o output_directory``
```

### Comparing `h5_to_edf-1.0.1/pyproject.toml` & `h5_to_edf-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `h5_to_edf-1.0.1/src/h5_to_edf/converter.py` & `h5_to_edf-1.0.2/src/h5_to_edf/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,22 +660,26 @@
         self.dmt = f"%s_%0{digits}d%s"
 
         setattr(self, "acq_frame", kwds["acq_frame"])
         if self.stem == "dark":
             self.filename_list = [self.name(0)]
             self.filename_lut = {self.name(0): 0}
             if self.acq_frame > 1 and self.data.dtype == np.int32:
-                self.data = np.array([np.mean(self.data, axis=0)] / self.acq_frame, dtype='intc')
+                self.data = np.array([np.mean(self.data, axis=0)] / self.acq_frame, dtype='float32')
+            else:
+                self.data = np.array([np.mean(self.data, axis=0)], dtype='float32')
             
 
         elif self.stem == "ref":
             self.filename_list = [self.name(0)]
             self.filename_lut = {self.name(0): 0}
             if self.acq_frame > 1 and self.data.dtype == np.int32:
-                self.data = np.array([np.median(self.data, axis=0)] / self.acq_frame, dtype='intc')
+                self.data = np.array([np.median(self.data, axis=0)] / self.acq_frame, dtype='float32')
+            else:
+                self.data = np.array([np.median(self.data, axis=0)], dtype='float32')
             
             
         elif "static" in self.stem:
             self.stem = self.stem.replace("static", "")
             self.filename_list = [self.rename_static(i) for i in range(len(self))]
             self.filename_lut = {fname: i for i, fname in enumerate(self.filename_list)}
             self.filename_lut = {fname: i for i, fname in
@@ -796,15 +800,15 @@
 
     
 
 
 def makeargs():
     parser = argparse.ArgumentParser()
     parser.add_argument('h5_names')
-    parser.add_argument('edf_directory')
+    parser.add_argument('-o', dest="edf_directory", default=None)
     # parser.add_argument('--start_nb', dest="start_nb", default=1)
     parser.add_argument('--report', dest="report", default="False")
     parser.add_argument(
         '--no-dark',
         dest="no_dark",
         default='False',
         help="If the h5 does not contains darks, will skip dark creation",
@@ -837,18 +841,21 @@
         for i in glob(args.h5_names):
             for j in glob(i + "/*.h5"):
                 if "tomwer" not in j and "nabu" not in j:
                     h5_names.append(j)
         h5_names.sort()
 
     edf_directory = args.edf_directory
+    if edf_directory is None:
+        edf_directory = os.path.join(h5_names[0].split("RAW_DATA")[0], "NOBACKUP")
+
     # start_nb = args.start_nb
     if not os.path.exists(edf_directory):
         os.system(f"mkdir {edf_directory}")
-
+        
     for h5_name in h5_names:
         # try:
         print(h5_name)
         directory = os.path.dirname(h5_name)
         dataset = directory.split("/")[-1]
         dataset_output = os.path.join(edf_directory, dataset + "_")
         rights = os.popen(f"ls -l {dataset_output}").read()
```

### Comparing `h5_to_edf-1.0.1/src/h5_to_edf/converter_oven.py` & `h5_to_edf-1.0.2/src/h5_to_edf/converter_oven.py`

 * *Files identical despite different names*

### Comparing `h5_to_edf-1.0.1/src/h5_to_edf.egg-info/PKG-INFO` & `h5_to_edf-1.0.2/src/h5_to_edf.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5-to-edf
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert a HDF5 file to EDF files
 Author-email: Jibril MAMMERI <mammeri@esrf.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.esrf.fr/mammeri/h5_to_edf
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/mammeri/h5_to_edf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,12 +22,12 @@
 
 How to use
 ~~~~~~~~~~
 
 The converter needs the name of the hdf5 file to be converted, and the output directory where the EDF files will
 be created.
 
-``convert_to_edf "path/file_001.h5" output_directory``
+``convert_to_edf "path/file_001.h5" -o output_directory``
 
 You can also convert multiple hdf5 files at once with the following command:
 
-``convert_to_edf "path/file_0*.h5" output_directory``
+``convert_to_edf "path/file_0*.h5" -o output_directory``
```

