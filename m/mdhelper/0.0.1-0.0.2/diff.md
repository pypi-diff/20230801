# Comparing `tmp/mdhelper-0.0.1.tar.gz` & `tmp/mdhelper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdhelper-0.0.1.tar", last modified: Mon Jul 31 23:18:18 2023, max compression
+gzip compressed data, was "mdhelper-0.0.2.tar", last modified: Tue Aug  1 03:01:16 2023, max compression
```

## Comparing `mdhelper-0.0.1.tar` & `mdhelper-0.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:20.673817 mdhelper-0.0.1/
--rwxrwxrwx   0 bye       (1000) bye       (1000)    35148 2023-07-31 20:46:01.000000 mdhelper-0.0.1/LICENSE
--rwxrwxrwx   0 bye       (1000) bye       (1000)    45682 2023-07-31 23:18:20.671817 mdhelper-0.0.1/PKG-INFO
--rwxrwxrwx   0 bye       (1000) bye       (1000)     4440 2023-07-31 23:16:36.000000 mdhelper-0.0.1/README.md
--rwxrwxrwx   0 bye       (1000) bye       (1000)      936 2023-07-31 21:42:52.000000 mdhelper-0.0.1/pyproject.toml
--rwxrwxrwx   0 bye       (1000) bye       (1000)       38 2023-07-31 23:18:20.674817 mdhelper-0.0.1/setup.cfg
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:19.898759 mdhelper-0.0.1/src/
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:19.967759 mdhelper-0.0.1/src/mdhelper/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      335 2023-07-31 23:17:57.000000 mdhelper-0.0.1/src/mdhelper/__init__.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:20.133454 mdhelper-0.0.1/src/mdhelper/algorithm/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      297 2023-07-31 22:39:08.000000 mdhelper-0.0.1/src/mdhelper/algorithm/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    31675 2023-07-30 08:08:03.000000 mdhelper-0.0.1/src/mdhelper/algorithm/correlation.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    22733 2023-07-31 06:41:37.000000 mdhelper-0.0.1/src/mdhelper/algorithm/molecule.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     9495 2023-07-31 05:39:23.000000 mdhelper-0.0.1/src/mdhelper/algorithm/topology.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     4078 2023-07-31 06:14:54.000000 mdhelper-0.0.1/src/mdhelper/algorithm/utility.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:20.232520 mdhelper-0.0.1/src/mdhelper/analysis/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      311 2023-07-31 22:39:17.000000 mdhelper-0.0.1/src/mdhelper/analysis/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    12707 2023-07-31 06:19:00.000000 mdhelper-0.0.1/src/mdhelper/analysis/base.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    34576 2023-07-31 07:07:54.000000 mdhelper-0.0.1/src/mdhelper/analysis/polymer.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    26052 2023-07-31 07:08:01.000000 mdhelper-0.0.1/src/mdhelper/analysis/profile.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    40749 2023-07-31 07:12:20.000000 mdhelper-0.0.1/src/mdhelper/analysis/structure.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    44585 2023-07-31 07:08:26.000000 mdhelper-0.0.1/src/mdhelper/analysis/transport.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:20.350562 mdhelper-0.0.1/src/mdhelper/fit/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      442 2023-07-31 22:39:24.000000 mdhelper-0.0.1/src/mdhelper/fit/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     2043 2023-07-06 00:11:20.000000 mdhelper-0.0.1/src/mdhelper/fit/distribution.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     5175 2023-07-06 00:11:17.000000 mdhelper-0.0.1/src/mdhelper/fit/exponential.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    15872 2023-07-06 00:11:06.000000 mdhelper-0.0.1/src/mdhelper/fit/fourier.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    16781 2023-07-06 00:11:01.000000 mdhelper-0.0.1/src/mdhelper/fit/gaussian.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    10617 2023-07-06 00:10:56.000000 mdhelper-0.0.1/src/mdhelper/fit/polynomial.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     2023 2023-07-06 00:10:53.000000 mdhelper-0.0.1/src/mdhelper/fit/power.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:20.507381 mdhelper-0.0.1/src/mdhelper/openmm/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      339 2023-07-31 22:39:52.000000 mdhelper-0.0.1/src/mdhelper/openmm/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     3125 2023-07-04 06:36:31.000000 mdhelper-0.0.1/src/mdhelper/openmm/bond.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    12753 2023-07-06 02:59:50.000000 mdhelper-0.0.1/src/mdhelper/openmm/file.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    32978 2023-07-04 06:33:05.000000 mdhelper-0.0.1/src/mdhelper/openmm/pair.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     6742 2023-07-31 07:09:18.000000 mdhelper-0.0.1/src/mdhelper/openmm/reporter.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    27274 2023-07-31 07:00:53.000000 mdhelper-0.0.1/src/mdhelper/openmm/system.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     8495 2023-07-05 23:47:00.000000 mdhelper-0.0.1/src/mdhelper/openmm/topology.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     3146 2023-07-04 04:37:02.000000 mdhelper-0.0.1/src/mdhelper/openmm/unit.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)    11770 2023-07-05 23:55:48.000000 mdhelper-0.0.1/src/mdhelper/openmm/utility.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:20.561816 mdhelper-0.0.1/src/mdhelper/plot/
--rwxrwxrwx   0 bye       (1000) bye       (1000)      284 2023-07-31 22:46:37.000000 mdhelper-0.0.1/src/mdhelper/plot/__init__.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     4318 2023-07-31 06:59:18.000000 mdhelper-0.0.1/src/mdhelper/plot/axis.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     2613 2023-07-31 06:58:40.000000 mdhelper-0.0.1/src/mdhelper/plot/rcparam.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)      521 2023-07-27 08:49:14.000000 mdhelper-0.0.1/src/mdhelper/utility.py
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:20.041943 mdhelper-0.0.1/src/mdhelper.egg-info/
--rwxrwxrwx   0 bye       (1000) bye       (1000)    45682 2023-07-31 23:18:19.000000 mdhelper-0.0.1/src/mdhelper.egg-info/PKG-INFO
--rwxrwxrwx   0 bye       (1000) bye       (1000)     1461 2023-07-31 23:18:19.000000 mdhelper-0.0.1/src/mdhelper.egg-info/SOURCES.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)        1 2023-07-31 23:18:19.000000 mdhelper-0.0.1/src/mdhelper.egg-info/dependency_links.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)       62 2023-07-31 23:18:19.000000 mdhelper-0.0.1/src/mdhelper.egg-info/requires.txt
--rwxrwxrwx   0 bye       (1000) bye       (1000)        9 2023-07-31 23:18:19.000000 mdhelper-0.0.1/src/mdhelper.egg-info/top_level.txt
-drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-07-31 23:18:20.656817 mdhelper-0.0.1/tests/
--rwxrwxrwx   0 bye       (1000) bye       (1000)    20973 2023-07-29 23:12:15.000000 mdhelper-0.0.1/tests/test_algorithm_correlation.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     6697 2023-07-31 06:30:50.000000 mdhelper-0.0.1/tests/test_algorithm_molecule.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     3583 2023-07-31 03:39:46.000000 mdhelper-0.0.1/tests/test_algorithm_topology.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     1394 2023-07-31 06:27:12.000000 mdhelper-0.0.1/tests/test_algorithm_utility.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     1676 2023-07-31 06:46:07.000000 mdhelper-0.0.1/tests/test_analysis_polymer.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     1817 2023-07-31 06:56:38.000000 mdhelper-0.0.1/tests/test_analysis_profile.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     4704 2023-07-31 06:56:49.000000 mdhelper-0.0.1/tests/test_analysis_structure.py
--rwxrwxrwx   0 bye       (1000) bye       (1000)     7204 2023-07-31 06:57:57.000000 mdhelper-0.0.1/tests/test_analysis_transport.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.679887 mdhelper-0.0.2/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    35148 2023-07-31 23:42:30.000000 mdhelper-0.0.2/LICENSE
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    45730 2023-08-01 03:01:18.677888 mdhelper-0.0.2/PKG-INFO
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     4519 2023-08-01 01:10:54.000000 mdhelper-0.0.2/README.md
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      889 2023-08-01 00:55:39.000000 mdhelper-0.0.2/pyproject.toml
+-rwxrwxrwx   0 bye       (1000) bye       (1000)       38 2023-08-01 03:01:18.679887 mdhelper-0.0.2/setup.cfg
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:17.802352 mdhelper-0.0.2/src/
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:17.879350 mdhelper-0.0.2/src/mdhelper/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      335 2023-08-01 00:06:54.000000 mdhelper-0.0.2/src/mdhelper/__init__.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.064379 mdhelper-0.0.2/src/mdhelper/algorithm/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      297 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/algorithm/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    31675 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/algorithm/correlation.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    22733 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/algorithm/molecule.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     9398 2023-08-01 00:56:40.000000 mdhelper-0.0.2/src/mdhelper/algorithm/topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     4078 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/algorithm/utility.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.191950 mdhelper-0.0.2/src/mdhelper/analysis/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      311 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/analysis/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    12707 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/analysis/base.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    34372 2023-08-01 00:58:08.000000 mdhelper-0.0.2/src/mdhelper/analysis/polymer.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    25470 2023-08-01 01:00:38.000000 mdhelper-0.0.2/src/mdhelper/analysis/profile.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    40452 2023-08-01 01:02:44.000000 mdhelper-0.0.2/src/mdhelper/analysis/structure.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    44274 2023-08-01 01:04:20.000000 mdhelper-0.0.2/src/mdhelper/analysis/transport.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.329887 mdhelper-0.0.2/src/mdhelper/fit/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      442 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     2043 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/distribution.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     5175 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/exponential.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    15872 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/fourier.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    16781 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/gaussian.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    10617 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/polynomial.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     2023 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/fit/power.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.500888 mdhelper-0.0.2/src/mdhelper/openmm/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      339 2023-08-01 00:55:13.000000 mdhelper-0.0.2/src/mdhelper/openmm/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3125 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/bond.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    12753 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/file.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    32978 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/pair.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     6742 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/reporter.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    27274 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/system.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     8495 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3146 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/unit.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    11770 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/openmm/utility.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.558888 mdhelper-0.0.2/src/mdhelper/plot/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      284 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/plot/__init__.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     4318 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/plot/axis.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     2613 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/plot/rcparam.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)      521 2023-07-31 23:42:59.000000 mdhelper-0.0.2/src/mdhelper/utility.py
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:17.961380 mdhelper-0.0.2/src/mdhelper.egg-info/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    45730 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/PKG-INFO
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1461 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)        1 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)       48 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/requires.txt
+-rwxrwxrwx   0 bye       (1000) bye       (1000)        9 2023-08-01 03:01:17.000000 mdhelper-0.0.2/src/mdhelper.egg-info/top_level.txt
+drwxrwxrwx   0 bye       (1000) bye       (1000)        0 2023-08-01 03:01:18.659886 mdhelper-0.0.2/tests/
+-rwxrwxrwx   0 bye       (1000) bye       (1000)    20973 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_algorithm_correlation.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     6697 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_algorithm_molecule.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     3583 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_algorithm_topology.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1394 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_algorithm_utility.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1676 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_analysis_polymer.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     1817 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_analysis_profile.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     4704 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_analysis_structure.py
+-rwxrwxrwx   0 bye       (1000) bye       (1000)     7204 2023-07-31 23:42:59.000000 mdhelper-0.0.2/tests/test_analysis_transport.py
```

### Comparing `mdhelper-0.0.1/LICENSE` & `mdhelper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/PKG-INFO` & `mdhelper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdhelper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A batteries-included toolkit of analysis modules and helper functions 
 Author-email: "Benjamin B. Ye" <bye@caltech.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,29 +675,31 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/bbye98/mdhelper
 Project-URL: Bug Tracker, https://github.com/bbye98/mdhelper/issues
-Keywords: feed,reader,tutorial
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MDHelper
 
 MDHelper is a batteries-included toolkit of analysis modules and helper
 functions for molecular dynamics (MD) simulations.
 
+* **Documentation**: https://bbye98.github.io/mdhelper/
+* **Python Package Index (PyPI)**: https://pypi.org/project/mdhelper/
+
 Note that MDHelper is currently an *experimental* library that has 
 only been tested on Linux and may contain bugs and issues. If you come 
 across one, please 
 [submit a new issue](https://github.com/bbye98/mdhelper/issues/new). If 
 you would like to contribute to MDHelper, please 
 [submit a pull request](https://github.com/bbye98/mdhelper/compare).
 
@@ -715,31 +717,29 @@
 Extensions to the high-performance OpenMM toolkit, such as custom 
 bond/pair potentials, support for NetCDF trajectories, and much more.
 * [`plot`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/plot): 
 Settings and additional functionality for Matplotlib figures.
 * [`utility`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/utility): 
 General utility functions.
 
-**Documentation**: https://bbye98.github.io/mdhelper/
-
 ## Installation and usage
 
 ### Prerequisites
 
 If you use pip to manage your Python packages or plan on using OpenMM
 with third-party extensions, such as 
 [`constvplugin`](https://github.com/scychon/openmm_constV) for the
 method of image charges, you must compile and install OpenMM prior to
 installing MDHelper. See the 
 ["Compiling OpenMM from Source Code"](http://docs.openmm.org/latest/userguide/library/02_compiling.html) 
 for more section of the OpenMM User Guide for more information. This 
 additional step is necessary since precompiled versions of OpenMM do not
 expose their header files, which are needed to link against custom 
 plugins. Otherwise, the lastest precompiled version of OpenMM on 
-conda-forge will be installed automatically alongside MDHelper.
+conda-forge will be installed during the installation of MDHelper.
 
 ### Virtual environment
 
 It is recommended, but not necessary, that you create a virtual 
 environment to prevent dependency conflicts.
 
 If you are using pip to manage Python packages, use
@@ -752,15 +752,15 @@
 If you are using Anaconda or Miniconda, use
 
     conda create --name venv
     conda activate venv
 
 ### Install using pip
 
-Install MDHelper and its dependencies using 
+ 1. Install MDHelper and its dependencies using 
 
     pip install mdhelper
 
 ### Install using Anaconda or Miniconda
 
  1. Add the conda-forge channel using
```

### Comparing `mdhelper-0.0.1/README.md` & `mdhelper-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # MDHelper
 
 MDHelper is a batteries-included toolkit of analysis modules and helper
 functions for molecular dynamics (MD) simulations.
 
+* **Documentation**: https://bbye98.github.io/mdhelper/
+* **Python Package Index (PyPI)**: https://pypi.org/project/mdhelper/
+
 Note that MDHelper is currently an *experimental* library that has 
 only been tested on Linux and may contain bugs and issues. If you come 
 across one, please 
 [submit a new issue](https://github.com/bbye98/mdhelper/issues/new). If 
 you would like to contribute to MDHelper, please 
 [submit a pull request](https://github.com/bbye98/mdhelper/compare).
 
@@ -24,31 +27,29 @@
 Extensions to the high-performance OpenMM toolkit, such as custom 
 bond/pair potentials, support for NetCDF trajectories, and much more.
 * [`plot`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/plot): 
 Settings and additional functionality for Matplotlib figures.
 * [`utility`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/utility): 
 General utility functions.
 
-**Documentation**: https://bbye98.github.io/mdhelper/
-
 ## Installation and usage
 
 ### Prerequisites
 
 If you use pip to manage your Python packages or plan on using OpenMM
 with third-party extensions, such as 
 [`constvplugin`](https://github.com/scychon/openmm_constV) for the
 method of image charges, you must compile and install OpenMM prior to
 installing MDHelper. See the 
 ["Compiling OpenMM from Source Code"](http://docs.openmm.org/latest/userguide/library/02_compiling.html) 
 for more section of the OpenMM User Guide for more information. This 
 additional step is necessary since precompiled versions of OpenMM do not
 expose their header files, which are needed to link against custom 
 plugins. Otherwise, the lastest precompiled version of OpenMM on 
-conda-forge will be installed automatically alongside MDHelper.
+conda-forge will be installed during the installation of MDHelper.
 
 ### Virtual environment
 
 It is recommended, but not necessary, that you create a virtual 
 environment to prevent dependency conflicts.
 
 If you are using pip to manage Python packages, use
@@ -61,15 +62,15 @@
 If you are using Anaconda or Miniconda, use
 
     conda create --name venv
     conda activate venv
 
 ### Install using pip
 
-Install MDHelper and its dependencies using 
+ 1. Install MDHelper and its dependencies using 
 
     pip install mdhelper
 
 ### Install using Anaconda or Miniconda
 
  1. Add the conda-forge channel using
```

### Comparing `mdhelper-0.0.1/pyproject.toml` & `mdhelper-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "mdhelper"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name = "Benjamin B. Ye", email = "bye@caltech.edu" }
 ]
 classifiers = [
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3"
 ]
+dependencies = [
+  "matplotlib",
+  "mdanalysis",
+  "netCDF4",
+  "numpy",
+  "scipy",
+  "sympy"
+]
 description = """
 A batteries-included toolkit of analysis modules and helper functions 
 for molecular dynamics (MD) simulations.
 """
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.6"
-keywords = ["feed", "reader", "tutorial"]
-dependencies = [
-    "feedparser >= 5.2.0",
-    "html2text",
-    'tomli; python_version < "3.11"',
-]
 
 [project.urls]
 "Homepage" = "https://github.com/bbye98/mdhelper"
 "Bug Tracker" = "https://github.com/bbye98/mdhelper/issues"
```

### Comparing `mdhelper-0.0.1/src/mdhelper/algorithm/correlation.py` & `mdhelper-0.0.2/src/mdhelper/algorithm/correlation.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/algorithm/molecule.py` & `mdhelper-0.0.2/src/mdhelper/algorithm/molecule.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/algorithm/topology.py` & `mdhelper-0.0.2/src/mdhelper/algorithm/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,22 @@
 This module contains implementations of common topology 
 transformations, like the generation of initial particle positions.
 """
 
 from typing import Any, Union
 
 import numpy as np
-
-try:
-    from openmm import app, unit
-    FOUND_OPENMM = True
-except: # pragma: no cover
-    FOUND_OPENMM = False
+from openmm import app, unit
 
 from . import utility
 
 def create_atoms(
-        dims: Union[np.ndarray, "unit.Quantity", "app.Topology"], N: int = None,
+        dims: Union[np.ndarray, unit.Quantity, app.Topology], N: int = None,
         N_p: int = 1, *, lattice: str = None, 
-        length: Union[float, "unit.Quantity"] = 0.34,
+        length: Union[float, unit.Quantity] = 0.34,
         flexible: bool = False, connectivity: bool = False, 
         randomize: bool = False, length_unit: unit.Unit = None, 
         wrap: bool = False) -> Any:
 
     r"""
     Generates initial particle positions for coarse-grained simulations.
 
@@ -130,20 +125,20 @@
         **Shape**: :math:`(3,)`.
 
         **Reference unit**: :math:`\mathrm{nm}`.
     """
 
     # Remove units, if necessary
     if not isinstance(dims, np.ndarray):
-        if type(dims).__name__ == "Topology":
+        if isinstance(dims, app.Topology):
             dims = dims.getUnitCellDimensions()
         if length_unit is None:
             length_unit = dims.unit
         dims /= length_unit
-    if type(length).__name__ == "Quantity":
+    if isinstance(length, unit.Quantity):
         if length_unit is None:
             length_unit = length.unit
         length /= length_unit
 
     if lattice is None:
 
         # Ensure the user-specified values are valid
```

### Comparing `mdhelper-0.0.1/src/mdhelper/algorithm/utility.py` & `mdhelper-0.0.2/src/mdhelper/algorithm/utility.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/analysis/base.py` & `mdhelper-0.0.2/src/mdhelper/analysis/base.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/analysis/polymer.py` & `mdhelper-0.0.2/src/mdhelper/analysis/polymer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,17 @@
 
 from typing import Union
 import warnings
 
 import MDAnalysis as mda
 from MDAnalysis.lib.log import ProgressBar
 import numpy as np
+from openmm import unit
 from scipy import optimize
 
-try:
-    from openmm import unit
-    FOUND_OPENMM = True
-except: # pragma: no cover
-    FOUND_OPENMM = False
-
 from .base import SerialAnalysisBase, ParallelAnalysisBase
 from .. import ArrayLike
 from ..algorithm import correlation, molecule
 from ..fit.exponential import stretched_exp
 
 def correlation_fft(*args, **kwargs):
 
@@ -226,16 +221,15 @@
                 emsg = ("The number of chain lengths is not equal to the "
                         "number of groups.")
                 raise ValueError(emsg)
 
         self._unwrap = unwrap
         self._verbose = verbose
 
-        if FOUND_OPENMM:
-            self.results.units = {"_dims": unit.angstrom}
+        self.results.units = {"_dims": unit.angstrom}
 
 class Gyradius(_PolymerAnalysisBase):
 
     r"""
     A serial implementation to calculate the radius of gyration 
     :math:`R_\mathrm{g}` of a polymer.
 
@@ -361,16 +355,15 @@
 
         # Preallocate arrays to store results
         shape = (self._n_groups, self.n_frames, 3) if self._components \
                 else (self._n_groups, self.n_frames)
         self.results.gyradius = np.empty(shape, dtype=float)
         
         # Store reference units
-        if FOUND_OPENMM:
-            self.results.units = {"results.gyradius": unit.angstrom}
+        self.results.units = {"results.gyradius": unit.angstrom}
 
     def _single_frame(self) -> None:
 
         for i, (g, gr, M, N_p) in enumerate(
                 zip(self._groups, self._groupings, self._n_chains, 
                     self._n_monomers)):
 
@@ -528,15 +521,15 @@
     """
 
     def __init__(
             self, groups: Union[mda.AtomGroup, ArrayLike],
             groupings: Union[str, ArrayLike] = "atoms", 
             n_chains: Union[int, ArrayLike] = None, 
             n_monomers: Union[int, ArrayLike] = None, *, n_blocks: int = 1,
-            fft: bool = True, dt: Union[float, "unit.Quantity"] = None, 
+            fft: bool = True, dt: Union[float, unit.Quantity] = None, 
             unwrap: bool = False, verbose: bool = True, **kwargs) -> None:
 
         super().__init__(groups, groupings, n_chains, n_monomers, 
                          unwrap=unwrap, verbose=verbose, **kwargs)
                         
         self._n_blocks = n_blocks
         self._fft = fft
@@ -723,16 +716,15 @@
             ), -1
         ).reshape(-1, 3)
         self._wavenumbers = np.linalg.norm(self._wavevectors, axis=1)
 
         self._unwrap = unwrap
         self._verbose = verbose
 
-        if FOUND_OPENMM:
-            self.results.units = {"_dims": unit.angstrom}
+        self.results.units = {"_dims": unit.angstrom}
 
     def _prepare(self) -> None:
 
         # Unwrap particle positions if necessary
         if self._unwrap:
             self.universe.trajectory[
                 self._sliced_trajectory.frames[0] 
@@ -744,16 +736,15 @@
                                   else molecule.center_of_mass(self._group, 
                                                                self._grouping)
             self._images = np.zeros(self._positions_old.shape, dtype=int)
             self._threshold = self._dims / 2
 
         # Determine the unique wavenumbers
         self.results.wavenumbers = np.unique(self._wavenumbers.round(11))
-        if FOUND_OPENMM:
-            self.results.units["results.wavenumbers"] = unit.angstrom ** -1
+        self.results.units["results.wavenumbers"] = unit.angstrom ** -1
 
         # Preallocate arrays to store results
         self.results.scsf = np.zeros(len(self._wavevectors), dtype=float)
 
     def _single_frame(self) -> None:
 
         # Get atom or center-of-mass positions in the current frame
```

### Comparing `mdhelper-0.0.1/src/mdhelper/analysis/profile.py` & `mdhelper-0.0.2/src/mdhelper/analysis/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,29 @@
 """
 
 from typing import Any, Union
 import warnings
 
 import MDAnalysis as mda
 import numpy as np
+from openmm import unit
 from scipy import integrate
 
-try:
-    from openmm import unit
-    FOUND_OPENMM = True
-except:
-    FOUND_OPENMM = False
-
 from .base import SerialAnalysisBase
 from .. import ArrayLike
 from ..algorithm import molecule
 from ..openmm import unit as u
 
 def potential_profile(
-        bins: Union[np.ndarray, "unit.Quantity"], 
-        charge_density: Union[np.ndarray, "unit.Quantity"], 
-        L: Union[float, "unit.Quantity"], dielectric: float = 1, *,
-        sigma_e: Union[float, "unit.Quantity"] = None,
-        dV: Union[float, "unit.Quantity"] = None,
-        threshold: float = 1e-5, V0: Union[float, "unit.Quantity"] = 0,
+        bins: Union[np.ndarray, unit.Quantity], 
+        charge_density: Union[np.ndarray, unit.Quantity], 
+        L: Union[float, unit.Quantity], dielectric: float = 1, *,
+        sigma_e: Union[float, unit.Quantity] = None,
+        dV: Union[float, unit.Quantity] = None,
+        threshold: float = 1e-5, V0: Union[float, unit.Quantity] = 0,
         reduced: bool = False) -> None:
     
     r"""
     Calculates the potential profile :math:`\varphi(z)` using the charge
     density profile by numerically solving Poisson's equation for 
     electrostatics.
 
@@ -107,44 +102,38 @@
     V0 : `float` or `openmm.unit.Quantity`, keyword-only, default: :code:`0`
         Potential :math:`\varphi_0` at the left boundary. 
         
         **Reference unit**: :math:`\mathrm{V}`.
     """
         
     # Check V0 for unit consistency
-    if type(V0).__name__ == "Quantity":
+    if isinstance(V0, unit.Quantity):
         if reduced:
             emsg = ("'V0' has units, while the rest of the data is "
                     "reduced.")
             raise ValueError(emsg)
-        
-        # If V0 is an openmm.unit.Quantity object, it is assumed
-        # that an OpenMM installation can be found
         V0 /= unit.volt
         if isinstance(V0, unit.Quantity):
             raise ValueError("'V0' has invalid units.")
     
     # Calculate the first integral of the charge density profile
     potential = integrate.cumulative_trapezoid(charge_density, bins, initial=0)
 
     if sigma_e is None:
         
         # Calculate surface charge density for system with perfectly
         # conducting boundaries
         if dV is not None:
 
             # Check dV for unit consistency
-            if type(dV).__name__ == "Quantity":
+            if isinstance(dV, unit.Quantity):
                 if reduced:
                     emsg = ("'dV' has units, while the rest of the data is "
                             "reduced.")
                     raise ValueError(emsg)
-                
-                # If dV is an openmm.unit.Quantity object, it is 
-                # assumed that an OpenMM installation can be found
                 dV /= unit.volt
                 if isinstance(V0, unit.Quantity):
                     raise ValueError("'dV' has invalid units.")
         
             sigma_e = dielectric * dV / L
             if reduced:
                 sigma_e /= 4 * np.pi
@@ -168,22 +157,19 @@
             target_index = len(potential) // 2
             sigma_e = potential[
                 cut_indices[cut_indices <= target_index][-1]:
                 cut_indices[cut_indices >= target_index][0]
             ].mean()
     
     # Check sigma_e for unit consistency
-    elif type(sigma_e).__name__ == "Quantity":
+    elif isinstance(sigma_e, unit.Quantity):
         if reduced:
             emsg = ("'sigma_e' has units, while the rest of the data "
                     "is reduced.")
             raise ValueError(emsg)
-        
-        # If sigma_e is an openmm.unit.Quantity object, it is 
-        # assumed that an OpenMM installation can be found
         sigma_e /= unit.elementary_charge / unit.angstrom ** 2
         if isinstance(sigma_e, unit.Quantity):
             raise ValueError("'sigma_e' has invalid units.")
 
     # Calculate the second integral of the charge density profile
     potential = -integrate.cumulative_trapezoid(potential - sigma_e, bins, 
                                                 initial=V0) / dielectric
@@ -430,30 +416,30 @@
                 raise ValueError(emsg)
         else:
             emsg = ("The specified bin counts must be an integer or an "
                     "iterable object.")
             raise ValueError(emsg)
 
         self._reduced = reduced
-        if not self._reduced and FOUND_OPENMM:
+        if not self._reduced:
             self.results.units = {"_dims": unit.angstrom}
 
         if charges is None:
             self._charges = np.fromiter(
                 (getattr(g, gr).charges[0] 
                  for g, gr in zip(self._groups, self._groupings)),
                 dtype=float
             ) if hasattr(self.universe.atoms, "charges") else None
         elif len(charges) == self._n_groups:
             self._charges = np.asarray(charges, dtype=float)
         else:
             emsg = ("The dimension of the array of group charges is "
                     f"incompatible with the number of {self._groupings}.")
             raise ValueError(emsg)
-        if self._charges is not None and not self._reduced and FOUND_OPENMM:
+        if self._charges is not None and not self._reduced:
             self.results.units["_charges"] = unit.elementary_charge
 
         if recenter is None:
             self._recenter = recenter
         elif isinstance(recenter, mda.AtomGroup):
             self._recenter = (recenter, self._dims / 2)
         elif isinstance(recenter, tuple) \
@@ -488,25 +474,25 @@
 
         # Preallocate arrays to hold number density data
         self.results.number_density = [
             np.zeros((self._n_groups, n), dtype=float) for n in self._n_bins
         ]
 
         # Store reference units
-        if not self._reduced and FOUND_OPENMM:
+        if not self._reduced:
             self.results.units["results.bins"] = unit.angstrom
             self.results.units["results.number_density"] = unit.angstrom ** -3
 
         # Preallocate arrays to hold charge density data, if charge
         # information is available
         if self._charges is not None:
             self.results.charge_density = [
                 np.zeros((self._n_groups, n), dtype=float) for n in self._n_bins
             ]
-            if not self._reduced and FOUND_OPENMM:
+            if not self._reduced:
                 self.results.units["_charge"] = unit.elementary_charge
                 self.results.units["results.charge_density"] = \
                     self.results.units["_charge"] / unit.angstrom ** 3
     
     def _single_frame(self):
 
         positions = self.universe.atoms.positions.copy()
@@ -574,17 +560,17 @@
             if self._charges is not None:
                 self.results.charge_density[a] = np.dot(
                     self._charges, self.results.number_density[a]
                 )
 
     def calculate_potential_profile(
             self, dielectric: float, axis: Union[int, str], *,
-            sigma_e: Union[float, "unit.Quantity"] = None,
-            dV: Union[float, "unit.Quantity"] = None,
-            threshold: float = 1e-5, V0: Union[float, "unit.Quantity"] = 0
+            sigma_e: Union[float, unit.Quantity] = None,
+            dV: Union[float, unit.Quantity] = None,
+            threshold: float = 1e-5, V0: Union[float, unit.Quantity] = 0
         ) -> None:
         
         r"""
         Calculates the potential profile in the given dimension using
         the charge density profile by numerically solving Poisson's 
         equation for electrostatics.
 
@@ -645,15 +631,15 @@
                     "DensityProfile object.")
             raise RuntimeError(emsg)
         
         if not hasattr(self.results, "potential"):
             self.results.potential = {}
 
             # Store reference units
-            if not self._reduced and FOUND_OPENMM:
+            if not self._reduced:
                 self.results.units["results.potential"] = unit.volt
 
         if isinstance(axis, str):
             axis = ord(axis.lower()) - 120
         index = np.where(self._axes == axis)[0][0]
 
         self.results.potential[axis] = potential_profile(
```

### Comparing `mdhelper-0.0.1/src/mdhelper/analysis/structure.py` & `mdhelper-0.0.2/src/mdhelper/analysis/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,18 @@
 
 from typing import Union
 import warnings
 
 import MDAnalysis as mda
 from MDAnalysis.lib import distances
 import numpy as np
+from openmm import unit
 from scipy.integrate import simpson
 from scipy.signal import argrelextrema
 
-try:
-    from openmm import unit
-    FOUND_OPENMM = True
-except:
-    FOUND_OPENMM = False
-
 from .base import SerialAnalysisBase, ParallelAnalysisBase
 from .. import ArrayLike
 from ..algorithm import molecule
 
 def radial_histogram(
         pos1: np.ndarray, pos2: np.ndarray, n_bins: int, range: ArrayLike,
         dims: ArrayLike, *, exclusion: ArrayLike = None) -> np.ndarray:
@@ -587,15 +582,15 @@
     def _prepare(self) -> None:
 
         # Preallocate arrays to store neighbor counts
         self.results.edges = np.linspace(*self._range, self._n_bins + 1)
         self.results.bins = (self.results.edges[:-1] 
                              + self.results.edges[1:]) / 2
         self.results.counts = np.zeros(self._n_bins, dtype=int)
-        if not self._reduced and FOUND_OPENMM:
+        if not self._reduced:
             self.results.units = {"results.bins": unit.angstrom,
                                   "results.edges": unit.angstrom}
 
         # Preallocate floating-point number for total volume analyzed
         # (for when system dimensions can change, such as during NpT
         # equilibration)
         if self._norm == "rdf":
@@ -689,15 +684,15 @@
             considered the boundary of a radial shell.
         """
 
         self.results.coordination_numbers = coordination_number(
             self.results.bins, self._get_rdf(), rho, n=n, threshold=threshold
         )
 
-    def calculate_pmf(self, temp: Union[float, "unit.Quantity"]) -> None:
+    def calculate_pmf(self, temp: Union[float, unit.Quantity]) -> None:
 
         r"""
         Calculates the potential of mean force :math:`w_{ij}(r)`.
 
         Parameters
         ----------
         temp : `float` or `openmm.unit.Quantity`
@@ -713,25 +708,21 @@
             **Reference unit**: :math:`\mathrm{K}`.
         """
 
         if self._reduced:
             kBT = temp
         else:
             if isinstance(temp, (int, float)):
-                if FOUND_OPENMM:
-                    kBT = (unit.AVOGADRO_CONSTANT_NA 
-                           * unit.BOLTZMANN_CONSTANT_kB * temp * unit.kelvin
-                           / unit.kilojoule_per_mole)
-                else:
-                    kBT = 0.00831446261815324 * temp
+                kBT = (unit.AVOGADRO_CONSTANT_NA 
+                       * unit.BOLTZMANN_CONSTANT_kB * temp * unit.kelvin
+                       / unit.kilojoule_per_mole)
             else:
                 kBT = (unit.AVOGADRO_CONSTANT_NA * unit.BOLTZMANN_CONSTANT_kB
                        * temp / unit.kilojoule_per_mole)
-            if FOUND_OPENMM:
-                self.results.units = {"results.pmf": unit.kilojoule_per_mole}
+            self.results.units = {"results.pmf": unit.kilojoule_per_mole}
 
         self.results.pmf = -kBT * np.log(self._get_rdf())
 
     def calculate_structure_factor(
             self, rho: float, x_i: float = None, x_j: float = None, 
             q: np.ndarray = None, *, q_lower: float = None, 
             q_upper: float = None, n_q: int = 1000, formalism: str = "FZ"
@@ -996,16 +987,15 @@
             ), -1
         ).reshape(-1, 3)
         self._wavenumbers = np.linalg.norm(self._wavevectors, axis=1)
 
         self._unwrap = unwrap
         self._verbose = verbose
 
-        if FOUND_OPENMM:
-            self.results.units = {"_dims": unit.angstrom}
+        self.results.units = {"_dims": unit.angstrom}
 
     def _prepare(self) -> None:
 
         # Unwrap particle positions if necessary
         self._positions = np.empty((self._N, 3), dtype=float)
         if self._unwrap:
             self.universe.trajectory[
@@ -1019,16 +1009,15 @@
                     g.positions if gr == "atoms" \
                     else molecule.center_of_mass(g, gr)
             self._images = np.zeros(self._positions_old.shape, dtype=int)
             self._threshold = self._dims / 2
 
         # Determine the unique wavenumbers
         self.results.wavenumbers = np.unique(self._wavenumbers.round(11))
-        if FOUND_OPENMM:
-            self.results.units["results.wavenumbers"] = unit.angstrom ** -1
+        self.results.units["results.wavenumbers"] = unit.angstrom ** -1
 
         # Preallocate arrays to store results
         self.results.ssf = np.zeros(len(self._wavenumbers), dtype=float)
         
     def _single_frame(self) -> None:
 
         for g, gr, s in zip(self._groups, self._groupings, self._slices):
```

### Comparing `mdhelper-0.0.1/src/mdhelper/analysis/transport.py` & `mdhelper-0.0.2/src/mdhelper/analysis/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,16 @@
 import itertools
 from typing import Union
 import warnings
 
 import MDAnalysis as mda
 from MDAnalysis.lib.log import ProgressBar
 import numpy as np
+from openmm import unit
 from scipy import optimize
- 
-try:
-    from openmm import unit
-    FOUND_OPENMM = True
-except:
-    FOUND_OPENMM = False
 
 from .base import SerialAnalysisBase
 from .. import ArrayLike
 from ..algorithm import correlation, molecule
 from ..fit.polynomial import poly1
 
 def msd_fft(*args, **kwargs) -> np.ndarray:
@@ -751,17 +746,17 @@
     """
 
     _GROUPINGS = {"atoms", "residues", "segments"}
 
     def __init__(
             self, groups: Union[mda.AtomGroup, ArrayLike],
             groupings: Union[str, ArrayLike] = "atoms",
-            temp: Union[float, "unit.Quantity"] = 300, *, n_blocks: int = 1,
+            temp: Union[float, unit.Quantity] = 300, *, n_blocks: int = 1,
             center: bool = False, com_wrap: bool = False, 
-            dt: Union[float, "unit.Quantity"] = None, fft: bool = True, 
+            dt: Union[float, unit.Quantity] = None, fft: bool = True, 
             reduced: bool = False, unwrap: bool = False, verbose: bool = True,
             **kwargs) -> None:
         
         self._groups = [groups] if isinstance(groups, mda.AtomGroup) else groups
         self.universe = self._groups[0].universe
         super().__init__(self.universe.trajectory, verbose=verbose, **kwargs)
         if self.universe.dimensions is None:
@@ -789,34 +784,30 @@
             self._groupings = groupings
 
         self._reduced = reduced
         if self._reduced:
             self._kBT = temp
         else:
             if isinstance(temp, (int, float)):
-                if FOUND_OPENMM:
-                    self._kBT = (unit.AVOGADRO_CONSTANT_NA 
-                                 * unit.BOLTZMANN_CONSTANT_kB
-                                 * temp * unit.kelvin 
-                                 / unit.kilojoule_per_mole)
-                else:
-                    self._kBT = 0.00831446261815324 * temp
+                self._kBT = (unit.AVOGADRO_CONSTANT_NA 
+                             * unit.BOLTZMANN_CONSTANT_kB
+                             * temp * unit.kelvin 
+                             / unit.kilojoule_per_mole)
             else:
                 self._kBT = (unit.AVOGADRO_CONSTANT_NA * unit.BOLTZMANN_CONSTANT_kB
                              * temp / unit.kilojoule_per_mole)
-            if FOUND_OPENMM:
-                self.results.units = {"_dims": unit.angstrom,
-                                      "_kBT": unit.kilojoule_per_mole}
+            self.results.units = {"_dims": unit.angstrom,
+                                  "_kBT": unit.kilojoule_per_mole}
         
         self._n_blocks = n_blocks
         self._center = center
         self._com_wrap = com_wrap
         if dt:
             self._dt = dt
-            if type(dt).__name__ == "Quantity":
+            if isinstance(dt, unit.Quantity):
                 self._dt /= unit.picosecond
         else:
             self._dt = self._trajectory.dt
         self._fft = fft
         self._unwrap = unwrap
         self._verbose = verbose
 
@@ -872,15 +863,15 @@
         )
         self.results.msd_self = np.empty(
             (self._n_groups, self._n_blocks, self._n_frames_block), 
             dtype=float
         )
 
         # Store reference units
-        if not self._reduced and FOUND_OPENMM:
+        if not self._reduced:
             self.results.units["results.time"] = unit.picosecond
             self.results.units["results.msd_cross"] = unit.angstrom ** 2
             self.results.units["results.msd_self"] = unit.angstrom ** 2
     
     def _single_frame(self) -> None:
 
         # Unwrap all particle positions, if necessary
@@ -1052,15 +1043,15 @@
                 stop_self=stop_self, 
                 scale_self=scale_self,
                 enforce_linear=enforce_linear, 
                 verbose=self._verbose
             )
 
         # Store reference units
-        if not self._reduced and FOUND_OPENMM:
+        if not self._reduced:
             self.results.units["results.D_i"] = (unit.angstrom ** 2 
                                                  / unit.picosecond)
             self.results.units["results.L_ii_self"] = \
             self.results.units["results.L_ij"] = \
                 1 / (unit.kilojoule_per_mole * unit.angstrom * unit.picosecond)
 
     def calculate_conductivity(self, *, charges: ArrayLike = None) -> None:
@@ -1094,15 +1085,15 @@
             raise ValueError("No charge number information available.")
         
         self.results.conductivity = conductivity(
             self.results.L_ij.mean(axis=0), self._charges, 
             reduced=self._reduced
         )
 
-        if not self._reduced and FOUND_OPENMM:
+        if not self._reduced:
             self.results.units["results.conductivity"] = \
                 unit.coulomb ** 2 / (unit.kilojoule * unit.angstrom
                                      * unit.picosecond)
 
     def calculate_electrophoretic_mobility(
             self, *, charges: ArrayLike = None, rhos: ArrayLike = None
         ) -> None:
@@ -1142,28 +1133,28 @@
         if charges is not None:
             self._charges = charges if isinstance(charges, np.ndarray) \
                             else np.array(charges)
         if self._charges is None:
             raise ValueError("No charge number information available.")
 
         if rhos is not None:
-            if type(rhos).__name__ == "Quantity":
+            if isinstance(rhos, unit.Quantity):
                 self.results.units["_rho"] = rhos.units
                 rhos = rhos.value_in_unit(self.results.units)
             self._rhos = rhos if isinstance(rhos, np.ndarray) \
                          else np.array(rhos)
         if self._rhos is None:
             raise ValueError("No number density information available.")
 
         self.results.mobility = electrophoretic_mobility(
             self.results.L_ij.mean(axis=0), charges, rhos,
             reduced=self._reduced
         )
         
-        if not self._reduced and FOUND_OPENMM:
+        if not self._reduced:
             self.results.units["results.mobility"] = \
                 unit.angstrom ** 2 * unit.coulomb / (unit.kilojoule
                                                      * unit.picosecond)
 
     def calculate_transference_number(
             self, *, charges: ArrayLike = None) -> None:
```

### Comparing `mdhelper-0.0.1/src/mdhelper/fit/distribution.py` & `mdhelper-0.0.2/src/mdhelper/fit/distribution.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/fit/exponential.py` & `mdhelper-0.0.2/src/mdhelper/fit/exponential.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/fit/fourier.py` & `mdhelper-0.0.2/src/mdhelper/fit/fourier.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/fit/gaussian.py` & `mdhelper-0.0.2/src/mdhelper/fit/gaussian.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/fit/polynomial.py` & `mdhelper-0.0.2/src/mdhelper/fit/polynomial.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/fit/power.py` & `mdhelper-0.0.2/src/mdhelper/fit/power.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/openmm/bond.py` & `mdhelper-0.0.2/src/mdhelper/openmm/bond.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/openmm/file.py` & `mdhelper-0.0.2/src/mdhelper/openmm/file.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/openmm/pair.py` & `mdhelper-0.0.2/src/mdhelper/openmm/pair.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/openmm/reporter.py` & `mdhelper-0.0.2/src/mdhelper/openmm/reporter.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/openmm/system.py` & `mdhelper-0.0.2/src/mdhelper/openmm/system.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/openmm/topology.py` & `mdhelper-0.0.2/src/mdhelper/openmm/topology.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/openmm/unit.py` & `mdhelper-0.0.2/src/mdhelper/openmm/unit.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/openmm/utility.py` & `mdhelper-0.0.2/src/mdhelper/openmm/utility.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/plot/axis.py` & `mdhelper-0.0.2/src/mdhelper/plot/axis.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/plot/rcparam.py` & `mdhelper-0.0.2/src/mdhelper/plot/rcparam.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper/utility.py` & `mdhelper-0.0.2/src/mdhelper/utility.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/src/mdhelper.egg-info/PKG-INFO` & `mdhelper-0.0.2/src/mdhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdhelper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A batteries-included toolkit of analysis modules and helper functions 
 Author-email: "Benjamin B. Ye" <bye@caltech.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,29 +675,31 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/bbye98/mdhelper
 Project-URL: Bug Tracker, https://github.com/bbye98/mdhelper/issues
-Keywords: feed,reader,tutorial
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MDHelper
 
 MDHelper is a batteries-included toolkit of analysis modules and helper
 functions for molecular dynamics (MD) simulations.
 
+* **Documentation**: https://bbye98.github.io/mdhelper/
+* **Python Package Index (PyPI)**: https://pypi.org/project/mdhelper/
+
 Note that MDHelper is currently an *experimental* library that has 
 only been tested on Linux and may contain bugs and issues. If you come 
 across one, please 
 [submit a new issue](https://github.com/bbye98/mdhelper/issues/new). If 
 you would like to contribute to MDHelper, please 
 [submit a pull request](https://github.com/bbye98/mdhelper/compare).
 
@@ -715,31 +717,29 @@
 Extensions to the high-performance OpenMM toolkit, such as custom 
 bond/pair potentials, support for NetCDF trajectories, and much more.
 * [`plot`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/plot): 
 Settings and additional functionality for Matplotlib figures.
 * [`utility`](https://github.com/bbye98/mdhelper/tree/main/src/mdhelper/utility): 
 General utility functions.
 
-**Documentation**: https://bbye98.github.io/mdhelper/
-
 ## Installation and usage
 
 ### Prerequisites
 
 If you use pip to manage your Python packages or plan on using OpenMM
 with third-party extensions, such as 
 [`constvplugin`](https://github.com/scychon/openmm_constV) for the
 method of image charges, you must compile and install OpenMM prior to
 installing MDHelper. See the 
 ["Compiling OpenMM from Source Code"](http://docs.openmm.org/latest/userguide/library/02_compiling.html) 
 for more section of the OpenMM User Guide for more information. This 
 additional step is necessary since precompiled versions of OpenMM do not
 expose their header files, which are needed to link against custom 
 plugins. Otherwise, the lastest precompiled version of OpenMM on 
-conda-forge will be installed automatically alongside MDHelper.
+conda-forge will be installed during the installation of MDHelper.
 
 ### Virtual environment
 
 It is recommended, but not necessary, that you create a virtual 
 environment to prevent dependency conflicts.
 
 If you are using pip to manage Python packages, use
@@ -752,15 +752,15 @@
 If you are using Anaconda or Miniconda, use
 
     conda create --name venv
     conda activate venv
 
 ### Install using pip
 
-Install MDHelper and its dependencies using 
+ 1. Install MDHelper and its dependencies using 
 
     pip install mdhelper
 
 ### Install using Anaconda or Miniconda
 
  1. Add the conda-forge channel using
```

### Comparing `mdhelper-0.0.1/src/mdhelper.egg-info/SOURCES.txt` & `mdhelper-0.0.2/src/mdhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/tests/test_algorithm_correlation.py` & `mdhelper-0.0.2/tests/test_algorithm_correlation.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/tests/test_algorithm_molecule.py` & `mdhelper-0.0.2/tests/test_algorithm_molecule.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/tests/test_algorithm_topology.py` & `mdhelper-0.0.2/tests/test_algorithm_topology.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/tests/test_algorithm_utility.py` & `mdhelper-0.0.2/tests/test_algorithm_utility.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/tests/test_analysis_polymer.py` & `mdhelper-0.0.2/tests/test_analysis_polymer.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/tests/test_analysis_profile.py` & `mdhelper-0.0.2/tests/test_analysis_profile.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/tests/test_analysis_structure.py` & `mdhelper-0.0.2/tests/test_analysis_structure.py`

 * *Files identical despite different names*

### Comparing `mdhelper-0.0.1/tests/test_analysis_transport.py` & `mdhelper-0.0.2/tests/test_analysis_transport.py`

 * *Files identical despite different names*

