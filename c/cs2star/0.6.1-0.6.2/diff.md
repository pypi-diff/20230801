# Comparing `tmp/cs2star-0.6.1.tar.gz` & `tmp/cs2star-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2star-0.6.1.tar", last modified: Mon Jul 31 13:52:17 2023, max compression
+gzip compressed data, was "cs2star-0.6.2.tar", last modified: Tue Aug  1 10:08:05 2023, max compression
```

## Comparing `cs2star-0.6.1.tar` & `cs2star-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 13:52:17.174568 cs2star-0.6.1/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-05-03 16:46:56.000000 cs2star-0.6.1/.gitignore
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-05-03 16:12:49.000000 cs2star-0.6.1/LICENSE
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-07-31 13:52:17.171235 cs2star-0.6.1/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2167 2023-03-16 10:09:28.000000 cs2star-0.6.1/README.md
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 13:52:17.171235 cs2star-0.6.1/cs2star/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2021-02-26 10:09:35.000000 cs2star-0.6.1/cs2star/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star/_version.py
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)    11537 2023-07-31 13:49:43.000000 cs2star-0.6.1/cs2star/cs2star.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3422 2023-03-29 12:13:31.000000 cs2star-0.6.1/cs2star/job_parser.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 13:52:17.171235 cs2star-0.6.1/cs2star.egg-info/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      312 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       49 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/entry_points.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       24 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/requires.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        8 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/top_level.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      841 2023-07-31 12:44:31.000000 cs2star-0.6.1/pyproject.toml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-07-31 13:52:17.174568 cs2star-0.6.1/setup.cfg
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-01 10:08:05.026715 cs2star-0.6.2/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-05-03 16:46:56.000000 cs2star-0.6.2/.gitignore
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-05-03 16:12:49.000000 cs2star-0.6.2/LICENSE
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-08-01 10:08:05.023382 cs2star-0.6.2/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2167 2023-03-16 10:09:28.000000 cs2star-0.6.2/README.md
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-01 10:08:05.023382 cs2star-0.6.2/cs2star/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2021-02-26 10:09:35.000000 cs2star-0.6.2/cs2star/__init__.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-08-01 10:08:04.000000 cs2star-0.6.2/cs2star/_version.py
+-rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)    11664 2023-08-01 10:06:51.000000 cs2star-0.6.2/cs2star/cs2star.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3422 2023-03-29 12:13:31.000000 cs2star-0.6.2/cs2star/job_parser.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-01 10:08:05.023382 cs2star-0.6.2/cs2star.egg-info/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-08-01 10:08:04.000000 cs2star-0.6.2/cs2star.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      312 2023-08-01 10:08:05.000000 cs2star-0.6.2/cs2star.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-08-01 10:08:04.000000 cs2star-0.6.2/cs2star.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       49 2023-08-01 10:08:04.000000 cs2star-0.6.2/cs2star.egg-info/entry_points.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       24 2023-08-01 10:08:04.000000 cs2star-0.6.2/cs2star.egg-info/requires.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        8 2023-08-01 10:08:04.000000 cs2star-0.6.2/cs2star.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      841 2023-07-31 12:44:31.000000 cs2star-0.6.2/pyproject.toml
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-08-01 10:08:05.026715 cs2star-0.6.2/setup.cfg
```

### Comparing `cs2star-0.6.1/LICENSE` & `cs2star-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2star-0.6.1/PKG-INFO` & `cs2star-0.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.6.1
+Version: 0.6.2
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.6.1/README.md` & `cs2star-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `cs2star-0.6.1/cs2star/cs2star.py` & `cs2star-0.6.2/cs2star/cs2star.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,27 +179,28 @@
         cleaning = progress.add_task('Cleaning up data...', total=2)
         df_part = pyem.star.check_defaults(df_part, inplace=True)
         progress.update(cleaning, advance=1)
         df_part = pyem.star.remove_deprecated_relion2(df_part, inplace=True)
         progress.update(cleaning, advance=1)
 
         # clean up
-        cleaning = progress.add_task('Cleaning up data...', total=2)
+        cleaning = progress.add_task('Cleaning up data...', total=3)
+        # also, optics are changed to 1-based indexing by pyem in parse_cryosparc_2_cs so we match it
+        # and we do it before the opticgroupname is generated from it
+        df_mic['rlnOpticsGroup'] += 1
         df_mic = pyem.star.check_defaults(df_mic, inplace=True)
         progress.update(cleaning, advance=1)
         df_mic = pyem.star.remove_deprecated_relion2(df_mic, inplace=True)
         progress.update(cleaning, advance=1)
-
         # need to fix the micrographs optics because pyem is missing some things that relion wants
-        # also, optics are changed to 1-based indexing by pyem in parse_cryosparc_2_cs!!
-        df_mic['rlnOpticsGroup'] += 1
         optics = ['rlnOpticsGroup'] + [head for head in ('rlnVoltage', 'rlnSphericalAberration') if head in df_part and head not in df_mic]
         opt = df_part.get(optics).drop_duplicates()
         df_mic = df_mic.loc[:, ~df_mic.columns.duplicated()]
         df_mic = df_mic.merge(opt, on='rlnOpticsGroup')
+        progress.update(cleaning, advance=1)
 
         # symlink/copy images
         def copy_images(paths, to_dir, label='micrographs', copy=False, add_s=False):
             exists = False
             for img in progress.track(paths, description=f'{"Copying" if copy else "Linking"} {label} to {to_dir}...'):
                 orig = job_dir.parent / img
                 # new path + add s to extension for relion
```

### Comparing `cs2star-0.6.1/cs2star/job_parser.py` & `cs2star-0.6.2/cs2star/job_parser.py`

 * *Files identical despite different names*

### Comparing `cs2star-0.6.1/cs2star.egg-info/PKG-INFO` & `cs2star-0.6.2/cs2star.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.6.1
+Version: 0.6.2
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.6.1/pyproject.toml` & `cs2star-0.6.2/pyproject.toml`

 * *Files identical despite different names*

