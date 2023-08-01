# Comparing `tmp/vasp_suite-1.4.0.tar.gz` & `tmp/vasp_suite-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.4.0.tar", last modified: Tue Aug  1 13:12:33 2023, max compression
+gzip compressed data, was "vasp_suite-1.4.1.tar", last modified: Tue Aug  1 13:25:01 2023, max compression
```

## Comparing `vasp_suite-1.4.0.tar` & `vasp_suite-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:12:33.681620 vasp_suite-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:12:33.681620 vasp_suite-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 13:12:33.681620 vasp_suite-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-08-01 13:12:31.000000 vasp_suite-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:12:33.679620 vasp_suite-1.4.0/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 13:12:31.000000 vasp_suite-1.4.0/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    18206 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/core.py
--rwxrwxrwx   0 root         (0) root         (0)    19106 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     3850 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/phonon.py
--rw-rw-rw-   0 root         (0) root         (0)    20919 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:12:33.680620 vasp_suite-1.4.0/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:25:01.621911 vasp_suite-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:25:01.620911 vasp_suite-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 13:25:01.621911 vasp_suite-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-08-01 13:24:59.000000 vasp_suite-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:25:01.619911 vasp_suite-1.4.1/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 13:24:59.000000 vasp_suite-1.4.1/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18206 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    19106 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     3850 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/phonon.py
+-rw-rw-rw-   0 root         (0) root         (0)    20919 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-08-01 13:24:28.000000 vasp_suite-1.4.1/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:25:01.620911 vasp_suite-1.4.1/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 13:25:01.000000 vasp_suite-1.4.1/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.4.0/LICENSE` & `vasp_suite-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.0/PKG-INFO` & `vasp_suite-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.4.0/README.md` & `vasp_suite-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.0/setup.py` & `vasp_suite-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.4.0/vasp_suite/cli.py` & `vasp_suite-1.4.1/vasp_suite/cli.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.0/vasp_suite/core.py` & `vasp_suite-1.4.1/vasp_suite/core.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.0/vasp_suite/ewald.py` & `vasp_suite-1.4.1/vasp_suite/ewald.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.0/vasp_suite/input.py` & `vasp_suite-1.4.1/vasp_suite/input.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.0/vasp_suite/phonon.py` & `vasp_suite-1.4.1/vasp_suite/phonon.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,23 +60,23 @@
         else:
             self.hostname = None
             self.sub = 'mpirun ...'
 
     def write_submit(self, disp):
         with open('submit.sh', 'w') as f:
             if self.hostname == 'csf3':
-                f.write("#!/bin/bash --login")
-                f.write("#$ -cwd")
-                f.write("#$ -pe smp.pe {}".format(self.cores))
+                f.write("#!/bin/bash --login \n")
+                f.write("#$ -cwd \n")
+                f.write("#$ -pe smp.pe {} \n".format(self.cores))
                 f.write("#$ -N phonopy \n \n")
                 f.write("module load {} \n \n".format(self.module))
             if self.hostname == 'csf4':
-                f.write("#!/bin/bash --login")
-                f.write("#SBATCH -p multicore")
-                f.write("#SBATCH -n {}".format(self.cores))
+                f.write("#!/bin/bash --login \n")
+                f.write("#SBATCH -p multicore \n")
+                f.write("#SBATCH -n {} \n".format(self.cores))
                 f.write("#SBATCH --job-name=phonopy \n \n")
                 f.write("module load {} \n \n".format(self.module))
 
             f.write("echo 'Started running at `date`' \n \n")
             f.write("for f in $(ls POSCAR-{001..%03d}) \n" % disp)
             f.write("do \n")
             f.write('if [ -f "${f}" ] \n then \n')
```

### Comparing `vasp_suite-1.4.0/vasp_suite/structure.py` & `vasp_suite-1.4.1/vasp_suite/structure.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.0/vasp_suite/submission.py` & `vasp_suite-1.4.1/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.4.0/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.4.1/vasp_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

