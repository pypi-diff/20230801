# Comparing `tmp/napari-nanopyx-0.0.3.tar.gz` & `tmp/napari-nanopyx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-nanopyx-0.0.3.tar", last modified: Wed Jun 14 10:46:40 2023, max compression
+gzip compressed data, was "napari-nanopyx-0.0.4.tar", last modified: Tue Aug  1 11:30:13 2023, max compression
```

## Comparing `napari-nanopyx-0.0.3.tar` & `napari-nanopyx-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.381846 napari-nanopyx-0.0.3/
--rw-r--r--   0 abrito   (1547774166) 931978602     7653 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/LICENSE
--rw-r--r--   0 abrito   (1547774166) 931978602       96 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/MANIFEST.in
--rw-r--r--   0 abrito   (1547774166) 931978602     3418 2023-06-14 10:46:40.381922 napari-nanopyx-0.0.3/PKG-INFO
--rw-r--r--   0 abrito   (1547774166) 931978602     2573 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/README.md
--rw-r--r--   0 abrito   (1547774166) 931978602      179 2023-06-14 10:46:27.000000 napari-nanopyx-0.0.3/pyproject.toml
--rw-r--r--   0 abrito   (1547774166) 931978602     1222 2023-06-14 10:46:40.382296 napari-nanopyx-0.0.3/setup.cfg
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.378217 napari-nanopyx-0.0.3/src/
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.380376 napari-nanopyx-0.0.3/src/napari_nanopyx/
--rw-r--r--   0 abrito   (1547774166) 931978602       41 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/__init__.py
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.381705 napari-nanopyx-0.0.3/src/napari_nanopyx/_tests/
--rw-r--r--   0 abrito   (1547774166) 931978602        0 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/_tests/__init__.py
--rw-r--r--   0 abrito   (1547774166) 931978602     3980 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/channel_registration.py
--rw-r--r--   0 abrito   (1547774166) 931978602     4408 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/drift_alignment.py
--rw-r--r--   0 abrito   (1547774166) 931978602     2308 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/napari.yaml
--rw-r--r--   0 abrito   (1547774166) 931978602     3750 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/squirrel.py
--rw-r--r--   0 abrito   (1547774166) 931978602     2421 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/srrf.py
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.381440 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/
--rw-r--r--   0 abrito   (1547774166) 931978602     3418 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/PKG-INFO
--rw-r--r--   0 abrito   (1547774166) 931978602      547 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/SOURCES.txt
--rw-r--r--   0 abrito   (1547774166) 931978602        1 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/dependency_links.txt
--rw-r--r--   0 abrito   (1547774166) 931978602       62 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/entry_points.txt
--rw-r--r--   0 abrito   (1547774166) 931978602       29 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/requires.txt
--rw-r--r--   0 abrito   (1547774166) 931978602       15 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/top_level.txt
+drwxr-xr-x   0 bsaraiva (1075917574) 931978602        0 2023-08-01 11:30:13.854142 napari-nanopyx-0.0.4/
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     7653 2022-11-29 15:01:13.000000 napari-nanopyx-0.0.4/LICENSE
+-rw-r--r--   0 bsaraiva (1075917574) 931978602       96 2022-11-29 15:01:13.000000 napari-nanopyx-0.0.4/MANIFEST.in
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     3418 2023-08-01 11:30:13.854222 napari-nanopyx-0.0.4/PKG-INFO
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     2573 2023-02-07 12:06:32.000000 napari-nanopyx-0.0.4/README.md
+-rw-r--r--   0 bsaraiva (1075917574) 931978602      180 2023-08-01 11:20:32.000000 napari-nanopyx-0.0.4/pyproject.toml
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     1251 2023-08-01 11:30:13.854582 napari-nanopyx-0.0.4/setup.cfg
+drwxr-xr-x   0 bsaraiva (1075917574) 931978602        0 2023-08-01 11:30:13.849803 napari-nanopyx-0.0.4/src/
+drwxr-xr-x   0 bsaraiva (1075917574) 931978602        0 2023-08-01 11:30:13.852794 napari-nanopyx-0.0.4/src/napari_nanopyx/
+-rw-r--r--   0 bsaraiva (1075917574) 931978602       41 2022-11-29 15:01:13.000000 napari-nanopyx-0.0.4/src/napari_nanopyx/__init__.py
+drwxr-xr-x   0 bsaraiva (1075917574) 931978602        0 2023-08-01 11:30:13.854050 napari-nanopyx-0.0.4/src/napari_nanopyx/_tests/
+-rw-r--r--   0 bsaraiva (1075917574) 931978602        0 2022-11-29 15:01:13.000000 napari-nanopyx-0.0.4/src/napari_nanopyx/_tests/__init__.py
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     3980 2023-02-02 14:26:42.000000 napari-nanopyx-0.0.4/src/napari_nanopyx/channel_registration.py
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     4408 2023-02-22 14:09:57.000000 napari-nanopyx-0.0.4/src/napari_nanopyx/drift_alignment.py
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     2308 2023-02-24 09:57:03.000000 napari-nanopyx-0.0.4/src/napari_nanopyx/napari.yaml
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     3750 2023-04-10 16:15:42.000000 napari-nanopyx-0.0.4/src/napari_nanopyx/squirrel.py
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     2421 2023-02-22 14:39:32.000000 napari-nanopyx-0.0.4/src/napari_nanopyx/srrf.py
+drwxr-xr-x   0 bsaraiva (1075917574) 931978602        0 2023-08-01 11:30:13.853925 napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/
+-rw-r--r--   0 bsaraiva (1075917574) 931978602     3418 2023-08-01 11:30:13.000000 napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/PKG-INFO
+-rw-r--r--   0 bsaraiva (1075917574) 931978602      547 2023-08-01 11:30:13.000000 napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/SOURCES.txt
+-rw-r--r--   0 bsaraiva (1075917574) 931978602        1 2023-08-01 11:30:13.000000 napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/dependency_links.txt
+-rw-r--r--   0 bsaraiva (1075917574) 931978602       62 2023-08-01 11:30:13.000000 napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/entry_points.txt
+-rw-r--r--   0 bsaraiva (1075917574) 931978602       37 2023-08-01 11:30:13.000000 napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/requires.txt
+-rw-r--r--   0 bsaraiva (1075917574) 931978602       15 2023-08-01 11:30:13.000000 napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/top_level.txt
```

### Comparing `napari-nanopyx-0.0.3/LICENSE` & `napari-nanopyx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.3/PKG-INFO` & `napari-nanopyx-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-nanopyx
-Version: 0.0.3
+Version: 0.0.4
 Summary: napari plugin of Nanoscopy Python library (NanoPyx, the successor to NanoJ) - focused on light microscopy and super-resolution imaging
 Author: Ricardo Henriques, Bruno Saraiva, Inês Cunha, António Brito
 Author-email: bruno.msaraiva2@gmail.com
 License: LGPL-3.0-only
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-nanopyx-0.0.3/README.md` & `napari-nanopyx-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.3/setup.cfg` & `napari-nanopyx-0.0.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-nanopyx
-version = 0.0.3
+version = 0.0.4
 description = napari plugin of Nanoscopy Python library (NanoPyx, the successor to NanoJ) - focused on light microscopy and super-resolution imaging
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Ricardo Henriques, Bruno Saraiva, Inês Cunha, António Brito
 author_email = bruno.msaraiva2@gmail.com
 license = LGPL-3.0-only
 license_files = LICENSE
@@ -20,14 +20,16 @@
 
 [options]
 packages = find:
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
+install_requires = 
+	nanopyx
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 napari.manifest = 
 	napari-nanopyx = napari_nanopyx:napari.yaml
```

### Comparing `napari-nanopyx-0.0.3/src/napari_nanopyx/channel_registration.py` & `napari-nanopyx-0.0.4/src/napari_nanopyx/channel_registration.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.3/src/napari_nanopyx/drift_alignment.py` & `napari-nanopyx-0.0.4/src/napari_nanopyx/drift_alignment.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.3/src/napari_nanopyx/napari.yaml` & `napari-nanopyx-0.0.4/src/napari_nanopyx/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.3/src/napari_nanopyx/squirrel.py` & `napari-nanopyx-0.0.4/src/napari_nanopyx/squirrel.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.3/src/napari_nanopyx/srrf.py` & `napari-nanopyx-0.0.4/src/napari_nanopyx/srrf.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/PKG-INFO` & `napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-nanopyx
-Version: 0.0.3
+Version: 0.0.4
 Summary: napari plugin of Nanoscopy Python library (NanoPyx, the successor to NanoJ) - focused on light microscopy and super-resolution imaging
 Author: Ricardo Henriques, Bruno Saraiva, Inês Cunha, António Brito
 Author-email: bruno.msaraiva2@gmail.com
 License: LGPL-3.0-only
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/SOURCES.txt` & `napari-nanopyx-0.0.4/src/napari_nanopyx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

