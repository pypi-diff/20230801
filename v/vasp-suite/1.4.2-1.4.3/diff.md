# Comparing `tmp/vasp_suite-1.4.2.tar.gz` & `tmp/vasp_suite-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.4.2.tar", last modified: Tue Aug  1 13:58:55 2023, max compression
+gzip compressed data, was "vasp_suite-1.4.3.tar", last modified: Tue Aug  1 14:11:08 2023, max compression
```

## Comparing `vasp_suite-1.4.2.tar` & `vasp_suite-1.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:58:55.889824 vasp_suite-1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:58:55.889824 vasp_suite-1.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 13:58:55.889824 vasp_suite-1.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-08-01 13:58:53.000000 vasp_suite-1.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:58:55.887824 vasp_suite-1.4.2/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 13:58:53.000000 vasp_suite-1.4.2/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    18448 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5387 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/core.py
--rwxrwxrwx   0 root         (0) root         (0)    19106 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     3850 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/phonon.py
--rw-rw-rw-   0 root         (0) root         (0)    20919 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:58:55.888824 vasp_suite-1.4.2/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:11:08.071435 vasp_suite-1.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 14:11:08.071435 vasp_suite-1.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 14:11:08.071435 vasp_suite-1.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-08-01 14:11:05.000000 vasp_suite-1.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:11:08.069435 vasp_suite-1.4.3/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 14:11:05.000000 vasp_suite-1.4.3/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18446 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5387 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/vasp_suite/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    19106 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     3850 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/vasp_suite/phonon.py
+-rw-rw-rw-   0 root         (0) root         (0)    20919 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-08-01 14:10:33.000000 vasp_suite-1.4.3/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:11:08.071435 vasp_suite-1.4.3/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 14:11:08.000000 vasp_suite-1.4.3/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 14:11:08.000000 vasp_suite-1.4.3/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 14:11:08.000000 vasp_suite-1.4.3/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-08-01 14:11:08.000000 vasp_suite-1.4.3/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-08-01 14:11:08.000000 vasp_suite-1.4.3/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 14:11:08.000000 vasp_suite-1.4.3/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.4.2/LICENSE` & `vasp_suite-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.2/PKG-INFO` & `vasp_suite-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.4.2/README.md` & `vasp_suite-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.2/setup.py` & `vasp_suite-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.4.2"
+__version__ = "1.4.3"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.4.2/vasp_suite/cli.py` & `vasp_suite-1.4.3/vasp_suite/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
     bec = args.bec
 
 # Check if the config file exists
     if not phonon.check_config():
         raise ValueError('No config file found, please run the start_up command')
 
 # Generate the input files
-    # core.generate_input('POSCAR', 'phonon')
+    core.generate_input('POSCAR', 'phonon')
     core.generate_kpoints(mesh=mesh)
 
     with open('INCAR', 'a') as f:
         f.write('ENCUT = {}\n'.format(str(encut)))
         if bec:
             f.write('LEPSILON = .TRUE.')
```

### Comparing `vasp_suite-1.4.2/vasp_suite/core.py` & `vasp_suite-1.4.3/vasp_suite/core.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.2/vasp_suite/ewald.py` & `vasp_suite-1.4.3/vasp_suite/ewald.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.2/vasp_suite/input.py` & `vasp_suite-1.4.3/vasp_suite/input.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.2/vasp_suite/phonon.py` & `vasp_suite-1.4.3/vasp_suite/phonon.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.2/vasp_suite/structure.py` & `vasp_suite-1.4.3/vasp_suite/structure.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.2/vasp_suite/submission.py` & `vasp_suite-1.4.3/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.2/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.4.3/vasp_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

