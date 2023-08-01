# Comparing `tmp/vasp_suite-1.4.1.tar.gz` & `tmp/vasp_suite-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.4.1.tar", last modified: Tue Aug  1 13:25:01 2023, max compression
+gzip compressed data, was "vasp_suite-1.4.2.tar", last modified: Tue Aug  1 13:58:55 2023, max compression
```

## Comparing `vasp_suite-1.4.1.tar` & `vasp_suite-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:25:01.621911 vasp_suite-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:25:01.620911 vasp_suite-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 13:25:01.621911 vasp_suite-1.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-08-01 13:24:59.000000 vasp_suite-1.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:25:01.619911 vasp_suite-1.4.1/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 13:24:59.000000 vasp_suite-1.4.1/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    18206 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/core.py
--rwxrwxrwx   0 root         (0) root         (0)    19106 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     3850 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/phonon.py
--rw-rw-rw-   0 root         (0) root         (0)    20919 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:25:01.620911 vasp_suite-1.4.1/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:58:55.889824 vasp_suite-1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:58:55.889824 vasp_suite-1.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 13:58:55.889824 vasp_suite-1.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-08-01 13:58:53.000000 vasp_suite-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:58:55.887824 vasp_suite-1.4.2/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 13:58:53.000000 vasp_suite-1.4.2/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18448 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5387 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    19106 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     3850 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/phonon.py
+-rw-rw-rw-   0 root         (0) root         (0)    20919 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-08-01 13:58:22.000000 vasp_suite-1.4.2/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:58:55.888824 vasp_suite-1.4.2/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 13:58:55.000000 vasp_suite-1.4.2/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.4.1/LICENSE` & `vasp_suite-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.1/PKG-INFO` & `vasp_suite-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.4.1
+Version: 1.4.2
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.4.1/README.md` & `vasp_suite-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.1/setup.py` & `vasp_suite-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.4.1/vasp_suite/cli.py` & `vasp_suite-1.4.2/vasp_suite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,34 +266,38 @@
 
     parameters
     ----------
     supercell : list
     mesh : list
     encut : int
     cores : int
+    bec : bool
 
     Returns
     -------
     None
     '''
     supercell = args.supercell
     mesh = args.mesh
     encut = args.encut
     cores = args.cores
+    bec = args.bec
 
 # Check if the config file exists
     if not phonon.check_config():
         raise ValueError('No config file found, please run the start_up command')
 
 # Generate the input files
     # core.generate_input('POSCAR', 'phonon')
     core.generate_kpoints(mesh=mesh)
 
     with open('INCAR', 'a') as f:
         f.write('ENCUT = {}\n'.format(str(encut)))
+        if bec:
+            f.write('LEPSILON = .TRUE.')
 
 # Create displacements
     phonon.create_displacements(supercell)
 
 # get the number of displacements
     disp = phonon.disp_files()
 
@@ -717,14 +721,20 @@
             '--supercell', '-s',
             help='The supercell to use for the phonon calculation',
             nargs=3,
             type=int,
             default=[1, 1, 1],
             )
 
+    phonon.add_argument(
+            '--bec',
+            help='Calculate the Born effective charges',
+            action='store_true',
+            )
+
     # Parse the ArgumentParser
     parser.set_defaults(func=lambda args: parser.print_help())
     args = parser.parse_known_args(arg_list)
 
     # Select programme 
     if args in ['generate_input, generate_job, calculate_kpoints, generate_kpoints, generate_supercell, start_up, dope_structure, generate_defect, asymmetric_unit, ewald, plot_potential, convert_cif']:
         args.func(args)
```

### Comparing `vasp_suite-1.4.1/vasp_suite/core.py` & `vasp_suite-1.4.2/vasp_suite/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,14 @@
 ALGO = Normal
 EDIFF = 1E-8
 GGA = PE
 ISIF = 2
 ISMEAR = 0
 LASPH = .TRUE.
 LCHARG = .FALSE.
-LEPSILON = .TRUE.
 LREAL = .FLASE.
 LWAVE = .FALSE.
 NSW = 0
 PREC = Accurate
 SIGMA = 0.01
 ''')
     os.chdir(cwd)
```

### Comparing `vasp_suite-1.4.1/vasp_suite/ewald.py` & `vasp_suite-1.4.2/vasp_suite/ewald.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.1/vasp_suite/input.py` & `vasp_suite-1.4.2/vasp_suite/input.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.1/vasp_suite/phonon.py` & `vasp_suite-1.4.2/vasp_suite/phonon.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.1/vasp_suite/structure.py` & `vasp_suite-1.4.2/vasp_suite/structure.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.1/vasp_suite/submission.py` & `vasp_suite-1.4.2/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.1/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.4.2/vasp_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.4.1
+Version: 1.4.2
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

