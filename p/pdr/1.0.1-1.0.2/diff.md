# Comparing `tmp/pdr-1.0.1.tar.gz` & `tmp/pdr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdr-1.0.1.tar", last modified: Tue Jun 20 17:24:19 2023, max compression
+gzip compressed data, was "pdr-1.0.2.tar", last modified: Tue Aug  1 21:10:53 2023, max compression
```

## Comparing `pdr-1.0.1.tar` & `pdr-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,66 @@
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.648991 pdr-1.0.1/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-02 18:30:59.000000 pdr-1.0.1/LICENSE
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    10893 2023-06-20 17:24:19.648991 pdr-1.0.1/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    10315 2023-06-20 17:15:41.000000 pdr-1.0.1/README.md
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.644991 pdr-1.0.1/pdr/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      595 2023-06-20 17:15:58.000000 pdr-1.0.1/pdr/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3956 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/_scaling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5212 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/bit_handling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    11544 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/browsify.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7128 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/datatypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       97 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/errors.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.648991 pdr-1.0.1/pdr/formats/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      602 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3846 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/cassini.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    12685 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/formats/checkers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      940 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/clementine.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      650 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/diviner.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      993 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/formats/galileo.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      884 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/juno.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1940 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/lro.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      125 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/lroc.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      335 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/mex_marsis.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/formats/mgn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      420 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/mgs.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      214 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/msl_apxs.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      210 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/msl_ccam.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      518 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/msl_cmn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      530 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/pvo.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      221 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/rosetta.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1053 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/themis.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5457 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/func.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.648991 pdr-1.0.1/pdr/loaders/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/_helpers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4623 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/datawrap.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4398 2023-06-13 19:04:43.000000 pdr-1.0.1/pdr/loaders/dispatch.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2767 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/handlers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5219 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/image.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    17607 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/loaders/queries.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     6429 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/loaders/table.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2473 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/text.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1516 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/utility.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3493 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/np_utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.648991 pdr-1.0.1/pdr/parselabel/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.0.1/pdr/parselabel/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    11104 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/parselabel/pds3.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1397 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/parselabel/pds4.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      731 2023-05-02 18:30:59.000000 pdr-1.0.1/pdr/parselabel/utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7294 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/pd_utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    26437 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/pdr.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      208 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/pdrtypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      490 2023-05-02 18:30:59.000000 pdr-1.0.1/pdr/pvl_utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     6652 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.644991 pdr-1.0.1/pdr.egg-info/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    10893 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1086 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/SOURCES.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/dependency_links.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      177 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/requires.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/top_level.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-06-20 17:24:19.648991 pdr-1.0.1/setup.cfg
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1076 2023-06-20 17:15:58.000000 pdr-1.0.1/setup.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-01 21:10:53.626910 pdr-1.0.2/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2248 2023-08-01 21:02:15.000000 pdr-1.0.2/LICENSE.md
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    12466 2023-08-01 21:10:53.626910 pdr-1.0.2/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11885 2023-08-01 21:02:15.000000 pdr-1.0.2/README.md
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-01 21:10:53.622910 pdr-1.0.2/pdr/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      595 2023-08-01 21:07:17.000000 pdr-1.0.2/pdr/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3956 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/_scaling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5212 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/bit_handling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11564 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/browsify.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7777 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/datatypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       97 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/errors.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-01 21:10:53.622910 pdr-1.0.2/pdr/formats/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      732 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3846 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/cassini.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    15187 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/checkers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      940 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/clementine.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      650 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/diviner.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2724 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/galileo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      884 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/juno.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2149 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/lro.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      125 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/lroc.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      335 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/mex_marsis.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2045 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/mgn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      420 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/mgs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      214 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/msl_apxs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      210 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/msl_ccam.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      518 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/msl_cmn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      280 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/near.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1315 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/nh.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      472 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/odyssey.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      530 2023-08-01 18:51:13.000000 pdr-1.0.2/pdr/formats/pvo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      221 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/rosetta.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1053 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/formats/themis.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      391 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/formats/vega.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5457 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/func.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-01 21:10:53.626910 pdr-1.0.2/pdr/loaders/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/loaders/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/loaders/_helpers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5043 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/loaders/datawrap.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4174 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/loaders/dispatch.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5014 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/loaders/handlers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5606 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/loaders/image.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    19225 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/loaders/queries.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7283 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/loaders/table.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2473 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/loaders/text.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1516 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/loaders/utility.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4206 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/np_utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-01 21:10:53.626910 pdr-1.0.2/pdr/parselabel/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.0.2/pdr/parselabel/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11392 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/parselabel/pds3.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1397 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/parselabel/pds4.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      731 2023-05-02 18:30:59.000000 pdr-1.0.2/pdr/parselabel/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     9525 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/pd_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    26472 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/pdr.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      208 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/pdrtypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      490 2023-05-02 18:30:59.000000 pdr-1.0.2/pdr/pvl_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     6652 2023-06-05 15:54:44.000000 pdr-1.0.2/pdr/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    14542 2023-08-01 21:02:15.000000 pdr-1.0.2/pdr/vax.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-08-01 21:10:53.622910 pdr-1.0.2/pdr.egg-info/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    12466 2023-08-01 21:10:53.000000 pdr-1.0.2/pdr.egg-info/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1181 2023-08-01 21:10:53.000000 pdr-1.0.2/pdr.egg-info/SOURCES.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-08-01 21:10:53.000000 pdr-1.0.2/pdr.egg-info/dependency_links.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      177 2023-08-01 21:10:53.000000 pdr-1.0.2/pdr.egg-info/requires.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2023-08-01 21:10:53.000000 pdr-1.0.2/pdr.egg-info/top_level.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-08-01 21:10:53.626910 pdr-1.0.2/setup.cfg
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1076 2023-08-01 21:07:17.000000 pdr-1.0.2/setup.py
```

### Comparing `pdr-1.0.1/LICENSE` & `pdr-1.0.2/LICENSE.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-BSD 3-Clause License
+###  BSD 3-Clause License
 
 Copyright (c) 2021, Million Concepts
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
@@ -23,7 +23,25 @@
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+### pdr/vax.py is derived from code in the SETI [pds-tools module](https://github.com/SETI/pds-tools/) and carries this additional license:
+
+Apache License, Version 2.0
+
+Copyright (c) 2023, SETI
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+  http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `pdr-1.0.1/PKG-INFO` & `pdr-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: pdr
-Version: 1.0.1
-Summary: Planetary Data Reader
-Home-page: https://github.com/MillionConcepts/pdr
-Author: Chase Million
-Author-email: chase@millionconcepts.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: notebooks
-Provides-Extra: browsify
-Provides-Extra: fits
-Provides-Extra: tiff
-Provides-Extra: pvl
-License-File: LICENSE
-
 README.md
 ## The Planetary Data Reader (pdr)
 
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
 (under PDS3 or PDS4) should be covered eventually. [Currently-supported datasets are listed here.](supported_datasets.md) 
@@ -166,30 +146,54 @@
 it causes us to break strict PEP-8 standards for attribute capitalization.
 There are three exceptions at present:
 1. Some table formats include repeated column names. For usability and
 compatibility, we force these to be unique by suffixing 0-indexed increasing
 integers. So a table definition with two separate columns named "COLUMN" will 
 return a pandas DataFrame with columns named "COLUMN_0" and "COLUMN_1."
 2. PDS3 data object names sometimes contain spaces. _pdr_ replaces the spaces
-with underscores in order to make them usable as attributes.
+with underscores in order to make them easily usable as Python attributes.
 
 #### PDS4 products
 `pdr.Data` wraps [`pds4_tools`](https://github.com/Small-Bodies-Node/pds4_tools/) 
 to read PDS4 products. All valid PDS4 products should be fully supported. `pdr`
 modifies some `pds4_tools` outputs in order to provide interface and behavior
 consistency. In general, you should be able to use `pdr` with PDS4 products 
 the same way you do with PDS3 products.
 
 Some PDS data products have both PDS3 and PDS4 labels. Data object names, 
 metadata, and even data field names and format specifications often differ 
-slightly between these labels, so `pdr` may produce slightly different outputs
+slightly between these labels, so `pdr.Data` may produce different outputs
 depending on which label you use to initialize it. This is not a bug. 
 However, in general, if a PDS3 label is available, we recommend initializing 
 the object from the PDS3 label rather than the PDS4 label.
 
+#### FITS files
+`pdr.Data` wraps [ `astropy.io.fits` ](https://github.com/astropy/astropy/tree/main/astropy/io/fits)
+to read data from FITS files associated with PDS3 products, and prefers the 
+data specification given in FITS headers to the data specification in the PDS3 
+label. In our experience, because FITS is more rigorously standardized than 
+PDS3, using the FITS header is more reliable; also, the FITS header often 
+contains useful metadata that the PDS3 label does not. `pdr` converts objects 
+produced by`astropy` to `np.ndarrays` (FITS arrays and compressed arrays), 
+`pd.DataFrames` (FITS ASCII and binary tables), or `MultiDicts` (FITS 
+headers), so you do not need to change your code simply because a file is in
+FITS format. 
+
+Whenever you load a data object from a FITS file, `pdr` also 
+places the associated FITS header in a key of your `Data` object named 
+"$objectname_HEADER" -- for instance, if you load an object named "HK_TABLE", 
+its FITS header will appear in `Data.HK_TABLE_HEADER`. You can also use the same 
+name to directly load the header *without* loading the entire data object.
+
+Note that in some cases, the specification in the FITS header may differ 
+from the specification in the PDS3 label, even when the specification in the 
+PDS3 label is technically valid. For instance, column names might be given 
+differently in the FITS header, or a PDS3 TABLE might be stored as a FITS 
+array HDU. 
+
 #### Lazy loading
 Because many planetary data objects are very large, `pdr` helps conserve 
 your time and memory by loading them lazily. It loads data objects into memory
 when they are explicitly referenced, not when `pdr.Data` is initialized. 
 For example, referencing`data.IMAGE` will immediately load the IMAGE object if 
 it has not already been loaded. Alternatively, you can load objects by using 
 the `load` method, like `data.load("IMAGE")`. You can also pass the 'all' 
@@ -203,14 +207,18 @@
 objects loaded from files that are actually present in your filesystem.
 
 #### Big files (like HiRISE)
 `pdr` currently performs no special memory management, so use caution 
 when attempting to read very large files. We intend to implement memory
 management in the future.
 
+#### WSL
+`.jp2` support is not guaranteed for WSL (Windows Subsystem for Linux). It is supported 
+on Windows itself and Linux. 
+
 ### tests
 
 Our testing methodology for *pdr* currently focuses on end-to-end integration
 testing to ensure consistency, coverage of supported datasets, and 
 (to the extent we can verify it) correctness of output.
 
 the test suite for *pdr* lives in a different repository:
```

### Comparing `pdr-1.0.1/README.md` & `pdr-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: pdr
+Version: 1.0.2
+Summary: Planetary Data Reader
+Home-page: https://github.com/MillionConcepts/pdr
+Author: Chase Million
+Author-email: chase@millionconcepts.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: notebooks
+Provides-Extra: browsify
+Provides-Extra: fits
+Provides-Extra: tiff
+Provides-Extra: pvl
+License-File: LICENSE.md
+
 README.md
 ## The Planetary Data Reader (pdr)
 
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
 (under PDS3 or PDS4) should be covered eventually. [Currently-supported datasets are listed here.](supported_datasets.md) 
@@ -146,30 +166,54 @@
 it causes us to break strict PEP-8 standards for attribute capitalization.
 There are three exceptions at present:
 1. Some table formats include repeated column names. For usability and
 compatibility, we force these to be unique by suffixing 0-indexed increasing
 integers. So a table definition with two separate columns named "COLUMN" will 
 return a pandas DataFrame with columns named "COLUMN_0" and "COLUMN_1."
 2. PDS3 data object names sometimes contain spaces. _pdr_ replaces the spaces
-with underscores in order to make them usable as attributes.
+with underscores in order to make them easily usable as Python attributes.
 
 #### PDS4 products
 `pdr.Data` wraps [`pds4_tools`](https://github.com/Small-Bodies-Node/pds4_tools/) 
 to read PDS4 products. All valid PDS4 products should be fully supported. `pdr`
 modifies some `pds4_tools` outputs in order to provide interface and behavior
 consistency. In general, you should be able to use `pdr` with PDS4 products 
 the same way you do with PDS3 products.
 
 Some PDS data products have both PDS3 and PDS4 labels. Data object names, 
 metadata, and even data field names and format specifications often differ 
-slightly between these labels, so `pdr` may produce slightly different outputs
+slightly between these labels, so `pdr.Data` may produce different outputs
 depending on which label you use to initialize it. This is not a bug. 
 However, in general, if a PDS3 label is available, we recommend initializing 
 the object from the PDS3 label rather than the PDS4 label.
 
+#### FITS files
+`pdr.Data` wraps [ `astropy.io.fits` ](https://github.com/astropy/astropy/tree/main/astropy/io/fits)
+to read data from FITS files associated with PDS3 products, and prefers the 
+data specification given in FITS headers to the data specification in the PDS3 
+label. In our experience, because FITS is more rigorously standardized than 
+PDS3, using the FITS header is more reliable; also, the FITS header often 
+contains useful metadata that the PDS3 label does not. `pdr` converts objects 
+produced by`astropy` to `np.ndarrays` (FITS arrays and compressed arrays), 
+`pd.DataFrames` (FITS ASCII and binary tables), or `MultiDicts` (FITS 
+headers), so you do not need to change your code simply because a file is in
+FITS format. 
+
+Whenever you load a data object from a FITS file, `pdr` also 
+places the associated FITS header in a key of your `Data` object named 
+"$objectname_HEADER" -- for instance, if you load an object named "HK_TABLE", 
+its FITS header will appear in `Data.HK_TABLE_HEADER`. You can also use the same 
+name to directly load the header *without* loading the entire data object.
+
+Note that in some cases, the specification in the FITS header may differ 
+from the specification in the PDS3 label, even when the specification in the 
+PDS3 label is technically valid. For instance, column names might be given 
+differently in the FITS header, or a PDS3 TABLE might be stored as a FITS 
+array HDU. 
+
 #### Lazy loading
 Because many planetary data objects are very large, `pdr` helps conserve 
 your time and memory by loading them lazily. It loads data objects into memory
 when they are explicitly referenced, not when `pdr.Data` is initialized. 
 For example, referencing`data.IMAGE` will immediately load the IMAGE object if 
 it has not already been loaded. Alternatively, you can load objects by using 
 the `load` method, like `data.load("IMAGE")`. You can also pass the 'all' 
@@ -183,14 +227,18 @@
 objects loaded from files that are actually present in your filesystem.
 
 #### Big files (like HiRISE)
 `pdr` currently performs no special memory management, so use caution 
 when attempting to read very large files. We intend to implement memory
 management in the future.
 
+#### WSL
+`.jp2` support is not guaranteed for WSL (Windows Subsystem for Linux). It is supported 
+on Windows itself and Linux. 
+
 ### tests
 
 Our testing methodology for *pdr* currently focuses on end-to-end integration
 testing to ensure consistency, coverage of supported datasets, and 
 (to the extent we can verify it) correctness of output.
 
 the test suite for *pdr* lives in a different repository:
```

### Comparing `pdr-1.0.1/pdr/__init__.py` & `pdr-1.0.2/pdr/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os.path as _osp
 from pdr.pdr import Data, Metadata
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 pkg_dir = _osp.abspath(_osp.dirname(__file__))
 
 
 def read(fp, **kwargs):
     from pdr.pdr import Data, Metadata
     from pdr.utils import check_cases
```

### Comparing `pdr-1.0.1/pdr/_scaling.py` & `pdr-1.0.2/pdr/_scaling.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/bit_handling.py` & `pdr-1.0.2/pdr/bit_handling.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/browsify.py` & `pdr-1.0.2/pdr/browsify.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,19 @@
             # automatically typecasting it.
             # TODO: detect rollover cases, etc.
             image //= maximum - minimum
         else:
             image /= maximum - minimum
         image += range_min
         return image
-    return (image - minimum) * (range_max - range_min) / (
-        maximum - minimum
-    ) + range_min
+    return (
+        (image - minimum) *
+        ((range_max - range_min) / (maximum - minimum))
+        + range_min
+    )
 
 
 def eightbit(
     array: np.array,
     clip: Union[float, tuple[float, float]] = 0,
     inplace: bool = False,
 ) -> np.ndarray:
```

### Comparing `pdr-1.0.1/pdr/datatypes.py` & `pdr-1.0.2/pdr/datatypes.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,18 @@
         "ASCII" not in sample_type
     ):
         endian = determine_byte_order(sample_type)
         signed = "UNSIGNED" not in sample_type
         return integer_bytes(endian, signed, sample_bytes, for_numpy)
     void = "V" if for_numpy is True else "s"
     _float = "d" if sample_bytes == 8 else "f"
+    if sample_type == "VAX_REAL" and sample_bytes != 4:
+        raise NotImplementedError(
+            "VAX reals that are not 4 bytes wide are not supported."
+        )
     return {
         "IEEE_REAL": f">{_float}",
         "PC_REAL": f"<{_float}",
         "FLOAT": f">{_float}",
         "REAL": f">{_float}",
         "MAC_REAL": f">{_float}",
         "SUN_REAL": f">{_float}",
@@ -69,14 +73,22 @@
         # (e.g. 1990-08-01T23:59:59)
         "DATE": f"S{sample_bytes}",
         "CHARACTER": f"S{sample_bytes}",  # ASCII character string
         "TIME": f"S{sample_bytes}",
         "VOID": f"{void}{sample_bytes}",
         "BCD": f"{void}{sample_bytes}",
         "BINARY_CODED_DECIMAL": f"{void}{sample_bytes}",
+        # this one (VAX_REAL) unfortunately doesn't work perfectly cleanly -- numpy
+        # doesn't have built-in support for it, so we just get the byte width
+        # correct here and add an additional check to transform it after load.
+        # the data type used here is totally arbitrary apart from byte size.
+        "VAX_REAL": f"<{_float}",
+        "IBM_REAL": f">u{sample_bytes}",
+        "EBCDIC": f"V{sample_bytes}",
+        "EBCDIC_CHARACTER": f"V{sample_bytes}",
     }[sample_type]
 
 
 # "basic" PDS3 special constants
 PDS3_CONSTANT_NAMES = (
     "INVALID_CONSTANT",
     "MISSING_CONSTANT",
```

### Comparing `pdr-1.0.1/pdr/formats/__init__.py` & `pdr-1.0.2/pdr/formats/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,10 +8,14 @@
 import pdr.formats.lro as lro
 import pdr.formats.mex_marsis as mex_marsis
 import pdr.formats.mgn as mgn
 import pdr.formats.mgs as mgs
 import pdr.formats.msl_apxs as msl_apxs
 import pdr.formats.msl_cmn as msl_cmn
 import pdr.formats.msl_ccam as msl_ccam
+import pdr.formats.near as near
+import pdr.formats.nh as nh
+import pdr.formats.odyssey as odyssey
 import pdr.formats.pvo as pvo
 import pdr.formats.rosetta as rosetta
 import pdr.formats.themis as themis
+import pdr.formats.vega as vega
```

### Comparing `pdr-1.0.1/pdr/formats/cassini.py` & `pdr-1.0.2/pdr/formats/cassini.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/formats/checkers.py` & `pdr-1.0.2/pdr/formats/checkers.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,33 +37,35 @@
                 "TIME",
                 "SUN",
                 "SOLAR",
             ]
         )
     ):
         return formats.cassini.get_offset(fn, identifiers)
+    if (
+        identifiers["INSTRUMENT_ID"] == "CRAT"
+        and identifiers["PRODUCT_TYPE"] == "EDR"
+        and name == "TABLE_1"
+    ):
+        return formats.lro.get_crater_offset()
     return False, None
 
 
-def check_special_table_reader(
-    identifiers, name, fn, fmtdef_dt, block
-):
+def check_special_table_reader(identifiers, name, fn, fmtdef_dt, block):
     if identifiers["DATA_SET_ID"] in (
         "CO-S-MIMI-4-CHEMS-CALIB-V1.0",
         "CO-S-MIMI-4-LEMMS-CALIB-V1.0",
         "CO-S-MIMI-4-INCA-CALIB-V1.0",
         "CO-E/J/S/SW-MIMI-2-LEMMS-UNCALIB-V1.0",
         "CO-SSA-RADAR-3-ABDR-SUMMARY-V1.0",
     ):
         return True, formats.cassini.spreadsheet_loader(
             fn, fmtdef_dt, identifiers["DATA_SET_ID"]
         )
-    if identifiers["INSTRUMENT_ID"] == "CHEMIN" and (
-        "SPREADSHEET" in name
-    ):
+    if identifiers["INSTRUMENT_ID"] == "CHEMIN" and ("SPREADSHEET" in name):
         # mangled object names + positions
         return True, formats.msl_cmn.spreadsheet_loader(fn)
     if (
         identifiers["INSTRUMENT_NAME"]
         == "ROSETTA PLASMA CONSORTIUM - MUTUAL IMPEDANCE "
         "PROBE"
         and "SPECTRUM_TABLE" in name
@@ -91,17 +93,25 @@
             identifiers, fmtdef_dt, block, fn
         )
     if (
         identifiers["INSTRUMENT_ID"] == "DLRE"
         and identifiers["PRODUCT_TYPE"] in ("GCP", "PCP", "PRP")
         and name == "TABLE"
     ):
-        return True, formats.diviner.diviner_l4_table_loader(
-            fmtdef_dt, fn
-        )
+        return True, formats.diviner.diviner_l4_table_loader(fmtdef_dt, fn)
+    if (
+        identifiers["DATA_SET_ID"] == "GO-J-PWS-5-DDR-PLASMA-DENSITY-FULL-V1.0"
+        and name == "SPREADSHEET"
+    ):
+        return True, formats.galileo.pws_table_loader(fn, fmtdef_dt)
+    if (
+        identifiers["DATA_SET_ID"] == "ODY-M-GRS-5-ELEMENTS-V1.0"
+        and name == "TABLE"
+    ):
+        return True, formats.odyssey.map_table_loader(fn, fmtdef_dt)
     return False, None
 
 
 def check_special_structure(block, name, fn, identifiers, data):
     if (
         identifiers["DATA_SET_ID"] == "CLEM1-L-RSS-5-BSR-V1.0"
         and name == "DATA_TABLE"
@@ -132,20 +142,41 @@
                 and "PWA" not in identifiers["FILE_NAME"]
             )
         )
     ):
         return True, formats.cassini.get_structure(
             block, name, fn, data, identifiers
         )
+    if (
+        identifiers["DATA_SET_ID"] == "GP-J-NMS-3-ENTRY-V1.0"
+        or identifiers["DATA_SET_ID"] == "GP-J-ASI-3-ENTRY-V1.0"
+    ) and name == "TABLE":
+        return True, formats.galileo.probe_structure(
+            block, name, fn, data, identifiers
+        )
+    if (
+        identifiers["DATA_SET_ID"] == "GO-E-EPD-2-SAMP-PAD-V1.0"
+        and identifiers["PRODUCT_ID"] == "E1PAD_7.TAB"
+        and name == "TIME_SERIES"
+    ):
+        return True, formats.galileo.epd_structure(
+            block, name, fn, data, identifiers
+        )
+    if (
+        "VEGA" in identifiers["DATA_SET_ID"]
+        and "-C-DUCMA-3-RDR-HALLEY-V1.0" in identifiers["DATA_SET_ID"]
+        and name == "TABLE"
+    ):
+        return True, formats.vega.get_structure(
+            block, name, fn, data, identifiers
+        )
     return False, None
 
 
-def check_special_position(
-    identifiers, block, target, name, fn, start_byte
-):
+def check_special_position(identifiers, block, target, name, fn, start_byte):
     if (
         identifiers["INSTRUMENT_ID"] == "MARSIS"
         and " TEC " in identifiers["DATA_SET_NAME"]
     ):
         return True, formats.mex_marsis.get_position(
             identifiers, block, target, name, start_byte
         )
@@ -271,14 +302,26 @@
     ):
         return True, formats.pvo.orpa_low_res_loader(data, name)
     if (
         identifiers["DATA_SET_ID"] == "PVO-V-OIMS-4-IONDENSITY-12S-V1.0"
         and name == "TABLE"
     ):
         return True, formats.pvo.oims_12s_loader(data, name)
+    if (
+        "GO-E-EPD-4-SUMM-" in identifiers["DATA_SET_ID"]
+        and "E1_" in identifiers["PRODUCT_ID"]
+        and name == "TIME_SERIES"
+    ):
+        return True, formats.galileo.epd_special_block(data, name)
+    if (
+        identifiers["INSTRUMENT_NAME"] == "PLASMA WAVE RECEIVER"
+        and "SUMM" in identifiers["DATA_SET_ID"]
+        and (name == "TIME_SERIES" or name == "TABLE")
+    ):
+        return True, formats.galileo.pws_special_block(data, name)
     return False, None
 
 
 def check_trivial_case(pointer, identifiers, fn) -> bool:
     if is_trivial(pointer):
         return True
     if (
@@ -316,17 +359,15 @@
     if (
         "GO-A-SSI-3-" in identifiers["DATA_SET_ID"]
         and "-CALIMAGES-V1.0" in identifiers["DATA_SET_ID"]
         and "QUB" in identifiers["PRODUCT_ID"]
         and pointer == "HEADER"
     ):
         return formats.galileo.ssi_cubes_header_loader()
-    if identifiers["INSTRUMENT_ID"] == "CHEMIN" and (
-        pointer == "HEADER"
-    ):
+    if identifiers["INSTRUMENT_ID"] == "CHEMIN" and (pointer == "HEADER"):
         return formats.msl_cmn.trivial_header_loader()
     return False
 
 
 def special_image_constants(identifiers):
     consts = {}
     if identifiers["INSTRUMENT_ID"] == "CRISM":
@@ -367,7 +408,28 @@
         identifiers["INSTRUMENT_HOST_NAME"]
         == "CASSINI_ORBITER"
         # and object_name == "QUBE" #should be repetitive because it's only called
         # inside a QUBE reading function.
     ):
         return formats.cassini.get_special_qube_band_storage()
     return False, None
+
+
+def check_special_hdu_name(identifiers, name):
+    if (
+        identifiers["INSTRUMENT_ID"] == "LORRI"
+        and identifiers["PRODUCT_TYPE"] == "EDR"
+    ):
+        return formats.nh.lorri_edr_hdu_name(name)
+    if (
+        identifiers["INSTRUMENT_ID"] == "LEISA"
+        and "-3-" in identifiers["DATA_SET_ID"]
+    ):
+        return formats.nh.leisa_cal_hdu_name(name)
+    if (
+        identifiers["INSTRUMENT_ID"] == "LEISA"
+        and identifiers["PRODUCT_TYPE"] == "EDR"
+    ):
+        return formats.nh.leisa_raw_hdu_name(name)
+    if re.match(r"NEAR-.*-EDR-", identifiers["DATA_SET_ID"]):
+        return formats.near.near_edr_hdu_name(name, identifiers["DATA_SET_ID"])
+    return False, None
```

### Comparing `pdr-1.0.1/pdr/formats/clementine.py` & `pdr-1.0.2/pdr/formats/clementine.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/formats/diviner.py` & `pdr-1.0.2/pdr/formats/diviner.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/formats/juno.py` & `pdr-1.0.2/pdr/formats/juno.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/formats/lro.py` & `pdr-1.0.2/pdr/formats/lro.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,16 +14,22 @@
     # Products can have multiple unique pointers that are
     # defined by a single image object (CAL_HISTOGRAM_DATA_IMAGE).
     object_name = "CAL_HISTOGRAM_DATA_IMAGE"
     block = data.metablock_(object_name)
     return block
 
 
+def get_crater_offset():
+    # lro crater edr products have a header table with 64 bytes per row, the second
+    # table start byte is given in rows (also the wrong row) but had a different number
+    # of row bytes
+    return True, 64
+
+
 def crater_bit_col_sample_type(base_samp_info):
-    # not yet in test corpus
     from pdr.datatypes import sample_types
 
     sample_type = base_samp_info["SAMPLE_TYPE"]
     sample_bytes = base_samp_info["BYTES_PER_PIXEL"]
     if "BIT_STRING" == sample_type:
         sample_type = "MSB_BIT_STRING"
         return True, sample_types(
```

### Comparing `pdr-1.0.1/pdr/formats/mgn.py` & `pdr-1.0.2/pdr/formats/mgn.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     # adapted from _interpret_as_ascii()
     colspecs = []
     from pdr.pd_utils import compute_offsets
 
     position_records = compute_offsets(fmtdef).to_dict("records")
     for record in position_records:
         col_length = record["BYTES"]
-        colspecs.append((record["OFFSET"], record["OFFSET"] + col_length))
+        colspecs.append((record["SB_OFFSET"], record["SB_OFFSET"] + col_length))
     string_buffer.seek(0)
     table = pd.read_fwf(string_buffer, header=None, colspecs=colspecs)
     string_buffer.close()
 
     table.columns = fmtdef.NAME.tolist()
     return table
```

### Comparing `pdr-1.0.1/pdr/formats/msl_cmn.py` & `pdr-1.0.2/pdr/formats/msl_cmn.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/formats/pvo.py` & `pdr-1.0.2/pdr/formats/pvo.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/formats/themis.py` & `pdr-1.0.2/pdr/formats/themis.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/func.py` & `pdr-1.0.2/pdr/func.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/loaders/_helpers.py` & `pdr-1.0.2/pdr/loaders/_helpers.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/loaders/datawrap.py` & `pdr-1.0.2/pdr/loaders/datawrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 from pdr.formats import (
     check_special_sample_type,
     check_special_qube_band_storage,
     check_special_position,
     check_special_structure,
     check_special_table_reader,
+    check_special_hdu_name
 )
 from pdr.func import get_argnames, softquery, specialize, call_kwargfiltered
 from pdr.parselabel.pds3 import depointerize
 from pdr.pdrtypes import LoaderFunction, PDRLike
-from pdr.loaders.queries import DEFAULT_DATA_QUERIES
+from pdr.loaders.queries import DEFAULT_DATA_QUERIES, get_identifiers, \
+    get_fits_name, get_file_mapping
 
 
 class Loader:
     """
     compact wrapper for loader functions, intended principally but not solely
     for library-internal use. provides a common interface, adds compactness,
     delays imports, etc.
@@ -59,14 +61,15 @@
             "sample_type": specialize(
                 im_sample_type, check_special_sample_type
             ),
             "band_storage_type": specialize(
                 get_qube_band_storage_type, check_special_qube_band_storage
             ),
             "gen_props": specialize(generic_image_properties, check_if_qube),
+            # just modifies gen_props in place, triggers transform in load step
         }
 
 
 class ReadTable(Loader):
     """wrapper for read_table"""
 
     def __init__(self):
@@ -118,15 +121,22 @@
 
     def __init__(self):
         from pdr.loaders.handlers import handle_fits_file
 
         super().__init__(handle_fits_file)
 
     def __call__(self, pdrlike: PDRLike, name: str, **kwargs):
-        return super().__call__(pdrlike, name, **kwargs)[name]
+        # slightly hacky but works with how we've done dictionary construction
+        return tuple(super().__call__(pdrlike, name, **kwargs).values())[0]
+
+    queries = {
+        'identifiers': get_identifiers,
+        "fn": get_file_mapping,
+        'hdu_name': specialize(get_fits_name, check_special_hdu_name)
+    }
 
 
 class ReadCompressedImage(Loader):
     """wrapper for handle_compressed_image"""
 
     def __init__(self):
         from pdr.loaders.handlers import handle_compressed_image
```

### Comparing `pdr-1.0.1/pdr/loaders/dispatch.py` & `pdr-1.0.2/pdr/loaders/dispatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     """
     if check_trivial_case(
         pointer, data.identifiers, data.filename
     ):
         return Trivial()
     if pointer == "LABEL":
         return ReadLabel()
+    if image_lib_dispatch(pointer, data) is not None:
+        return image_lib_dispatch(pointer, data)
     if (
         "TEXT" in pointer
         or "PDF" in pointer
         or "MAP_PROJECTION_CATALOG" in pointer
     ):
         return ReadText()
     if "DESC" in pointer:  # probably points to a reference file
@@ -86,24 +88,18 @@
     # binary tables named things like "Image Time Table". If there are pictures
     # of tables, we will need to do something more sophisticated.
     if (
         ("IMAGE" in pointer)
         or ("QUB" in pointer)
         or ("XDR_DOCUMENT" in pointer)
     ):
-        # TODO: sloppy pt. 1. this may be problematic for
-        #  products with a 'secondary' fits file, etc.
-        if image_lib_dispatch(pointer, data) is not None:
-            return image_lib_dispatch(pointer, data)
         return ReadImage()
     if "FILE_NAME" in pointer:
         return file_extension_to_loader(pointer)
     # TODO: sloppy pt. 2
-    if image_lib_dispatch(pointer, data) is not None:
-        return image_lib_dispatch(pointer, data)
     return TBD()
 
 
 def file_extension_to_loader(fn: str) -> Callable:
     """
     attempt to select the correct method of pdr.Data for objects only
     specified by a PDS3 FILE_NAME pointer (or by filename otherwise).
```

### Comparing `pdr-1.0.1/pdr/loaders/image.py` & `pdr-1.0.2/pdr/loaders/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from itertools import product
 
 import numpy as np
 
 from pdr.loaders.queries import get_image_properties
 from pdr.np_utils import np_from_buffered_io
 from pdr.utils import decompress
+from pdr import vax
 
 
 def read_image(name, gen_props, fn, start_byte):
     """
     Read an image object from this product and return it as a numpy array.
     """
     # TODO: Check for and apply BIT_MASK.
@@ -51,21 +52,28 @@
         image = image[:, : -props["line_suffix_pix"]]
     if props.get("line_prefix_pix", 0) > 0:
         prefix = image[:, : props["line_prefix_pix"]]
         image = image[:, props["line_prefix_pix"] :]
     return image, prefix, suffix
 
 
+def convert_if_vax(image, props):
+    if props.get('is_vax_real') is True:
+        return vax.from_vax32(image)
+    return image
+
+
 def process_single_band_image(f, props):
     _, numpy_dtype = make_format_specifications(props)
     # TODO: added this 'count' parameter to handle a case in which the image
     #  was not the last object in the file. We might want to add it to
     #  the multiband loaders too.
     image = np_from_buffered_io(f, dtype=numpy_dtype, count=props["pixels"])
     image, prefix, suffix = extract_single_band_linefix(image, props)
+    image = convert_if_vax(image, props)
     image = image.reshape(
         (props["nrows"] + props["rowpad"], props["ncols"] + props["colpad"])
     )
     image, axplanes = extract_axplanes(image, props)
     return make_c_contiguous(image), axplanes, prefix, suffix
 
 
@@ -81,29 +89,33 @@
         prefix = image[:, : props["line_prefix_pix"]]
         image = image[:, props["line_prefix_pix"] :]
     return image, prefix, suffix
 
 
 def process_multiband_image(f, props):
     bst = props["band_storage_type"]
-    if bst not in ("BAND_SEQUENTIAL", "LINE_INTERLEAVED"):
+    if bst not in ("BAND_SEQUENTIAL", "LINE_INTERLEAVED", "SAMPLE_INTERLEAVED"):
         warnings.warn(
             f"Unsupported BAND_STORAGE_TYPE={bst}. Guessing BAND_SEQUENTIAL."
         )
         bst = "BAND_SEQUENTIAL"
     _, numpy_dtype = make_format_specifications(props)
     image = np_from_buffered_io(f, numpy_dtype, count=props["pixels"])
+    image = convert_if_vax(image, props)
     bands, lines, samples = (
         props["nbands"] + props["bandpad"],
         props["nrows"] + props["rowpad"],
         props["ncols"] + props["colpad"],
     )
     prefix, suffix = None, None
     if bst == "BAND_SEQUENTIAL":
         image = image.reshape(bands, lines, samples)
+    elif bst == "SAMPLE_INTERLEAVED":
+        image = image.reshape(lines, samples, bands)
+        image = np.moveaxis(image, 2, 0)
     elif bst == "LINE_INTERLEAVED":
         image, prefix, suffix = extract_bil_linefix(image, props)
         image = image.reshape(lines, bands, samples)
         image = np.moveaxis(image, 0, 1)
     image, axplanes = extract_axplanes(image, props)
     return make_c_contiguous(image), axplanes, prefix, suffix
```

### Comparing `pdr-1.0.1/pdr/loaders/queries.py` & `pdr-1.0.2/pdr/loaders/queries.py`

 * *Files 14% similar despite different names*

```diff
@@ -177,15 +177,18 @@
         "BYTES_PER_PIXEL": int(block.get("SAMPLE_BITS", 0) / 8),
         "SAMPLE_TYPE": block.get("SAMPLE_TYPE", ""),
     }
 
 
 def generic_image_properties(block, sample_type):
     props = {
+        # TODO: BYTES_PER_PIXEL check appears repeated with slight variation
+        #  from base_sample_info()
         "BYTES_PER_PIXEL": int(block["SAMPLE_BITS"] / 8),
+        "is_vax_real": block.get("SAMPLE_TYPE") == "VAX_REAL",
         "sample_type": sample_type,
         "nrows": block["LINES"],
         "ncols": block["LINE_SAMPLES"],
     }
     if "BANDS" in block:
         props["nbands"] = block["BANDS"]
         props["band_storage_type"] = block.get("BAND_STORAGE_TYPE", None)
@@ -340,27 +343,30 @@
 def parse_table_structure(name, block, fn, data, identifiers):
     """
     Read a table's format specification and generate a DataFrame
     and -- if it's binary -- a numpy dtype object. These are later passed
     to np.fromfile or one of several ASCII table readers.
     """
     fmtdef = read_table_structure(block, name, fn, data, identifiers)
+    if fmtdef['DATA_TYPE'].str.contains('VAX_REAL').any():
+        raise NotImplementedError(
+            "VAX reals are not currently supported in tables."
+        )
     if fmtdef["DATA_TYPE"].str.contains("ASCII").any() or looks_like_ascii(
         block, name
     ):
         # don't try to load it as a binary file
         return fmtdef, None
     if fmtdef is None:
         return fmtdef, np.dtype([])
     for end in ("_PREFIX", "_SUFFIX", ""):
         length = block.get(f"ROW{end}_BYTES")
         if length is not None:
             fmtdef[f"ROW{end}_BYTES"] = length
     from pdr.pd_utils import insert_sample_types_into_df
-
     return insert_sample_types_into_df(fmtdef, identifiers)
 
 
 def read_table_structure(block, name, fn, data, identifiers):
     """
     Try to turn the TABLE definition into a column name / data type
     array. Requires renaming some columns to maintain uniqueness. Also
@@ -374,58 +380,80 @@
     will attempt to locate it in the same directory as the data / label,
     and throw an error if it's not there.
     TODO, maybe: Grab external format files as needed.
     """
     if "HISTOGRAM" in name:
         fields = get_histogram_fields(block)
     else:
-        fields = read_format_block(block, name, fn, data, identifiers)
+        fields, _ = read_format_block(block, name, fn, data, identifiers)
     # give columns unique names so that none of our table handling explodes
     import pandas as pd
 
     fmtdef = pd.DataFrame.from_records(fields)
     if "NAME" not in fmtdef.columns:
         fmtdef["NAME"] = name
 
     from pdr.pd_utils import reindex_df_values
-
     return reindex_df_values(fmtdef)
 
 
-def read_format_block(block, object_name, fn, data, identifiers):
+def read_format_block(
+    block, object_name, fn, data, identifiers, within_container=False
+):
     # load external structure specifications
     format_block = list(block.items())
     block_name = block.get("NAME")
     while "^STRUCTURE" in [obj[0] for obj in format_block]:
         format_block = inject_format_files(format_block, object_name, fn, data)
-    fields = []
+    fields, needs_placeholder, add_placeholder = [], False, False
     for item_type, definition in format_block:
         if item_type in ("COLUMN", "FIELD"):
+            if "^STRUCTURE" in definition:
+                definition_l = list(definition.items())
+                definition_l = inject_format_files(definition_l, object_name, fn, data)
+                definition = MultiDict()
+                for key, val in definition_l:
+                    definition.add(key, val)
             obj = dict(definition) | {"BLOCK_NAME": block_name}
             repeat_count = definition.get("ITEMS")
             obj = add_bit_column_info(obj, definition, identifiers)
+            add_placeholder = False
         elif item_type == "CONTAINER":
-            obj = read_format_block(
-                definition, object_name, fn, data, identifiers
+            if within_container is True and len(fields) == 0:
+                needs_placeholder = True
+            obj, add_placeholder = read_format_block(
+                definition, object_name, fn, data, identifiers, True
             )
             repeat_count = definition.get("REPETITIONS")
         else:
             continue
+        if add_placeholder is True:
+            dummy_column = {
+                'NAME': f'PLACEHOLDER_{definition["NAME"]}',
+                'DATA_TYPE': 'VOID',
+                'START_BYTE': definition['START_BYTE'],
+                'BYTES': 0,
+                'BLOCK_NAME': block_name
+            }
+            # dblock_name = None if len(fields) == 0 else fields[-1]['BLOCK_NAME']
+            # dummy_column['BLOCK_NAME'] = dblock_name
+            fields.append(dummy_column)
         # containers can have REPETITIONS,
         # and some "columns" contain a lot of columns (ITEMS)
         # repeat the definition, renaming duplicates, for these cases
         if repeat_count is not None:
             fields = append_repeated_object(obj, fields, repeat_count)
         else:
             fields.append(obj)
     # semi-legal top-level containers not wrapped in other objects
     if object_name == "CONTAINER":
         if (repeat_count := block.get("REPETITIONS")) is not None:
             fields = list(chain(*[fields for _ in range(repeat_count)]))
-    return fields
+
+    return fields, needs_placeholder
 
 
 def get_histogram_fields(block):
     # This error could go somewhere else, but at least we catch it early here
     if block.get("INTERCHANGE_FORMAT") == "ASCII":
         raise NotImplementedError(
             "ASCII histograms are not currently supported."
@@ -477,14 +505,23 @@
         raise FileNotFoundError
 
 
 def get_identifiers(data):
     return data.identifiers
 
 
+def get_fits_name(name):
+    """
+    just a target for specialize(check_special_fits_name) to maintain
+    signatures
+    TODO: consider moving the HDU extension identifying stuff in here
+    """
+    return name
+
+
 DEFAULT_DATA_QUERIES = MappingProxyType(
         {
             "identifiers": get_identifiers,
             "block": specialize(get_block, check_special_block),
             "fn": get_file_mapping,
             "target": get_target,
             "start_byte": specialize(data_start_byte, check_special_offset),
```

### Comparing `pdr-1.0.1/pdr/loaders/table.py` & `pdr-1.0.2/pdr/loaders/table.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from pandas.errors import ParserError
 
 from pdr.loaders._helpers import check_explicit_delimiter
 from pdr.loaders.queries import get_array_num_items, check_array_for_subobject
 from pdr import bit_handling
 from pdr.datatypes import sample_types
 from pdr.np_utils import np_from_buffered_io, enforce_order_and_object
-from pdr.pd_utils import booleanize_booleans
+from pdr.pd_utils import booleanize_booleans, convert_ebcdic, convert_ibm_reals
 from pdr.utils import decompress, head_file
 
 
 def read_array(fn, block, start_byte):
     """
     Read an array object from this product and return it as a numpy array.
     """
     # TODO: Maybe add block[AXES] as names? Might have to switch to pandas
     #  or a flattened structured array or something weirder
+    # TODO: Include offset calculations once an example with them is found
     obj = check_array_for_subobject(block)
     if block.get("INTERCHANGE_FORMAT") == "BINARY":
         with decompress(fn) as f:
             binary = np_from_buffered_io(
                 f,
                 dtype=sample_types(obj["DATA_TYPE"], obj["BYTES"], True),
                 count=get_array_num_items(block),
@@ -64,30 +65,43 @@
         table.columns = fmtdef.NAME.tolist()
     else:
         table = _interpret_as_binary(fn, fmtdef, dt, block, start_byte)
     # If there were any cruft "placeholder" columns, discard them
     table = table.drop(
         [k for k in table.keys() if "PLACEHOLDER" in k], axis=1
     )
+    # If there is an offset and/or scaling factor, apply them:
+    if fmtdef.get("OFFSET") is not None or fmtdef.get("SCALING_FACTOR") is not None:
+        for col in table.columns:
+            record = fmtdef.loc[fmtdef['NAME'] == col].to_dict("records")[0]
+            if record.get("SCALING_FACTOR") and not pd.isnull(record.get("SCALING_FACTOR")):
+                table[col] = table[col].mul(record["SCALING_FACTOR"])
+            else:
+                scaling_factor = 1  # TODO: appears superfluous
+            if record.get("OFFSET") and not pd.isnull(record.get("OFFSET")):
+                offset = record["OFFSET"]
+                table[col] = table[col]+offset
     return table
 
 
 def _interpret_as_binary(fn, fmtdef, dt, block, start_byte):
     # TODO: this works poorly (from a usability and performance
     #  perspective; it's perfectly stable) for tables defined as
     #  a single row with tens or hundreds of thousands of columns
     count = block.get("ROWS")
     count = count if count is not None else 1
     with decompress(fn) as f:
-        array = np_from_buffered_io(
+        table = np_from_buffered_io(
             f, dtype=dt, offset=start_byte, count=count
         )
-    swapped = enforce_order_and_object(array, inplace=False)
-    table = pd.DataFrame(swapped)
+    table = enforce_order_and_object(table)
+    table = pd.DataFrame(table)
+    table = convert_ibm_reals(table, fmtdef)
     table.columns = fmtdef.NAME.tolist()
+    table = convert_ebcdic(table, fmtdef)
     table = booleanize_booleans(table, fmtdef)
     table = bit_handling.expand_bit_strings(table, fmtdef)
     return table
 
 
 # noinspection PyTypeChecker
 def _interpret_as_ascii(identifiers, fn, fmtdef, block, table_props):
@@ -156,15 +170,15 @@
             position_records = compute_offsets(fmtdef).to_dict("records")
             for record in position_records:
                 if np.isnan(record.get("ITEM_BYTES", np.nan)):
                     col_length = record["BYTES"]
                 else:
                     col_length = int(record["ITEM_BYTES"])
                 colspecs.append(
-                    (record["OFFSET"], record["OFFSET"] + col_length)
+                    (record["SB_OFFSET"], record["SB_OFFSET"] + col_length)
                 )
             table = pd.read_fwf(string_buffer, header=None, colspecs=colspecs)
             string_buffer.close()
             return table
         except (pd.errors.EmptyDataError, pd.errors.ParserError):
             string_buffer.seek(0)
     table = pd.read_fwf(string_buffer, header=None)
```

### Comparing `pdr-1.0.1/pdr/loaders/text.py` & `pdr-1.0.2/pdr/loaders/text.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/loaders/utility.py` & `pdr-1.0.2/pdr/loaders/utility.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/np_utils.py` & `pdr-1.0.2/pdr/np_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -89,7 +89,28 @@
     return np.fromfile(buffered_io, dtype=dtype, count=count)
 
 
 def make_c_contiguous(arr: np.ndarray) -> np.ndarray:
     if arr.flags["C_CONTIGUOUS"] is False:
         return np.ascontiguousarray(arr)
     return arr
+
+
+# TODO: really all arguments but ibm/sreg are redundant for basic S/360 formats
+def ibm_to_np(ibm, sreg, ereg, mmask):
+    # dtype conversion: this field must be signed
+    ibm_sign = (ibm >> sreg & 0x01).astype('int8')
+    # dtype_conversion: largest values possible will overfloat int64 or float32
+    ibm_exponent = (ibm >> ereg & 0x7f).astype('float64')
+    ibm_mantissa = ibm & mmask
+    mantissa = ibm_mantissa / (2 ** ereg)
+    exponent = 16 ** (ibm_exponent - 64)
+    sign = 1 - (2 * ibm_sign).astype('int8')
+    return sign * mantissa * exponent
+
+
+def ibm32_to_np_f32(ibm):
+    return ibm_to_np(ibm, 31, 24, 0x00ffffff)
+
+
+def ibm64_to_np_f64(ibm):
+    return ibm_to_np(ibm, 63, 56, 0x00ffffffffffffff)
```

### Comparing `pdr-1.0.1/pdr/parselabel/pds3.py` & `pdr-1.0.2/pdr/parselabel/pds3.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,44 +13,53 @@
 from multidict import MultiDict
 
 from pdr.parselabel.utils import trim_label, DEFAULT_PVL_LIMIT
 from pdr.utils import decompress
 
 
 PVL_BLOCK_INITIALS = ("OBJECT", "GROUP", "BEGIN_OBJECT", "BEGIN_GROUP")
-PVL_BLOCK_TERMINALS = ("END",)
+PVL_BLOCK_TERMINAL = re.compile(r"END(_OBJECT|$)")
+PVL_QUANTITY_VALUE = re.compile(r"((\d|\.|-)+|NULL|UNK|N/A)")
+PVL_QUANTITY_UNITS = re.compile(r"<(.*)>")
+
+
+def extract_pvl_block_terminal(line):
+    try:
+        return re.match(PVL_BLOCK_TERMINAL, line).group()
+    except AttributeError:
+        return None
 
 
 def is_an_assignment_line(line):
     """
     pick lines that begin assignment statements.
 
     in PDS labels, it never (?) seems to be the case that people use
     delimiters to put multiple assignment statements on a line
 
     there is an issue with people who put '=' in text blocks --
     looking for a block of capital letters is usually good enough
     """
     if "=" not in line:
-        if line.startswith("END_OBJECT"):
+        if extract_pvl_block_terminal(line) is not None:
             return True
         return False
     start = line[:8]
     if start != start.upper():
         return False
     return True
 
 
 def chunk_statements(trimmed_lines: Iterable[str]):
     """chunk trimmed lines from a pvl-text into assignment statements."""
     statements = []
     for statement in split_before(trimmed_lines, is_an_assignment_line):
         assignment = statement[0]
-        if assignment.startswith("END_OBJECT"):
-            statements.append(("END_OBJECT", ""))
+        if (terminal := extract_pvl_block_terminal(assignment)) is not None:
+            statements.append((terminal, ""))
             continue
         try:
             parameter, value_head = map(str.strip, assignment.split("="))
         except ValueError:
             # some people like to put extra '='s on assignment lines,, like:
             # MRO:SPECIMEN_DESC      = "MONTMORILLONITE + FEOX, 100 % FECL2 SOL_N, PH=7,
             # i strongly suspect we will never make semantic use of
@@ -78,16 +87,15 @@
 
     def parse_statements(self, statements):
         for parameter, value in statements:
             if parameter in PVL_BLOCK_INITIALS:
                 self._step_in(value)
             elif (
                 # ignore invalid end block statements at top level
-                parameter.startswith(PVL_BLOCK_TERMINALS)
-                and len(self.names) > 0
+                parameter.startswith("END") and len(self.names) > 0
             ):
                 # not bothering with aggregation name verification
                 self._step_out()
             else:
                 self.add_statement(parameter, value)
         if len(self.aggregations) > 1:
             warnings.warn(
@@ -120,17 +128,17 @@
         mapping, params = index_duplicate_pointers(pointers, mapping, params)
     return mapping, params
 
 
 def parse_pvl_quantity_object(obj):
     return {
         "value": literalize_pvl(
-            re.search(r"((\d|\.|-)+|NULL|UNK|N/A)", obj).group()
+            re.search(PVL_QUANTITY_VALUE, obj).group()
         ),
-        "units": literalize_pvl(re.search(r"<(.*)>", obj).group(1)),
+        "units": literalize_pvl(re.search(PVL_QUANTITY_UNITS, obj).group(1)),
     }
 
 
 def parse_pvl_quantity_statement(statement):
     """
     parse pvl statements including quantities. returns quantities as mappings.
     this will also handle statements that do not consist entirely of
```

### Comparing `pdr-1.0.1/pdr/parselabel/pds4.py` & `pdr-1.0.2/pdr/parselabel/pds4.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/parselabel/utils.py` & `pdr-1.0.2/pdr/parselabel/utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr/pd_utils.py` & `pdr-1.0.2/pdr/pd_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 methods for working with pandas objects, primarily intended as components of
 pdr.Data's processing pipelines. some may require a Data object as an
 argument.
 """
+import re
 import warnings
 from typing import Hashable
 
 import numpy as np
 import pandas.api.types
 import pandas as pd
 
 from pdr.datatypes import sample_types
 from pdr.formats import check_special_sample_type
-from pdr.np_utils import enforce_order_and_object
+from pdr.np_utils import enforce_order_and_object, ibm32_to_np_f32, \
+    ibm64_to_np_f64
 
 
 def numeric_columns(df: pd.DataFrame) -> list[Hashable]:
     return [
         col
         for col, dtype in df.dtypes.iteritems()
         if pandas.api.types.is_numeric_dtype(dtype)
@@ -54,51 +56,51 @@
     item_offsets.loc[offset.index] = offset["ITEM_OFFSET"]
     return item_offsets
 
 
 def compute_offsets(fmtdef):
     """
     given a DataFrame containing PDS3 binary table structure specifications,
-    including a START_BYTE column, add an OFFSET column, unpacking objects
+    including a START_BYTE column, add an SB_OFFSET column, unpacking objects
     if necessary
     """
     # START_BYTE is 1-indexed, but we're preparing these offsets for
     # numpy, which 0-indexes
-    fmtdef["OFFSET"] = fmtdef["START_BYTE"] - 1
+    fmtdef["SB_OFFSET"] = fmtdef["START_BYTE"] - 1
     if "ROW_PREFIX_BYTES" in fmtdef.columns:
-        fmtdef["OFFSET"] += fmtdef["ROW_PREFIX_BYTES"]
+        fmtdef["SB_OFFSET"] += fmtdef["ROW_PREFIX_BYTES"]
     block_names = fmtdef["BLOCK_NAME"].unique()
     # calculate offsets for formats loaded in by reference
     for block_name in block_names[1:]:
         fmt_block = fmtdef.loc[fmtdef["BLOCK_NAME"] == block_name]
         prior = fmtdef.loc[fmt_block.index[0] - 1]
-        fmtdef.loc[fmt_block.index, "OFFSET"] += (
-            prior["OFFSET"] + prior["BYTES"]
+        fmtdef.loc[fmt_block.index, "SB_OFFSET"] += (
+            prior["SB_OFFSET"] + prior["BYTES"]
         )
     # correctly compute offsets within columns w/multiple items
     if "ITEM_BYTES" in fmtdef:
         fmtdef["ITEM_SIZE"] = _apply_item_offsets(fmtdef)
         column_groups = fmtdef.loc[fmtdef["ITEM_SIZE"].notna()]
-        for _, group in column_groups.groupby("OFFSET"):
-            fmtdef.loc[group.index, "OFFSET"] = group["OFFSET"] + int(
+        for _, group in column_groups.groupby("SB_OFFSET"):
+            fmtdef.loc[group.index, "SB_OFFSET"] = group["SB_OFFSET"] + int(
                 group["ITEM_SIZE"].iloc[0]
             ) * np.arange(len(group))
     pad_length = 0
-    end_byte = fmtdef["OFFSET"].iloc[-1] + fmtdef["BYTES"].iloc[-1]
+    end_byte = fmtdef["SB_OFFSET"].iloc[-1] + fmtdef["BYTES"].iloc[-1]
     if "ROW_BYTES" in fmtdef.columns:
         pad_length += fmtdef["ROW_BYTES"].iloc[0] - end_byte
     if "ROW_SUFFIX_BYTES" in fmtdef.columns:
         pad_length += fmtdef["ROW_SUFFIX_BYTES"].iloc[0]
     if pad_length > 0:
         placeholder_rec = {
             "NAME": "PLACEHOLDER_0",
             "DATA_TYPE": "VOID",
             "BYTES": pad_length,
             "START_BYTE": end_byte,
-            "OFFSET": end_byte,
+            "SB_OFFSET": end_byte,
         }
         fmtdef = pd.concat(
             [fmtdef, pd.DataFrame([placeholder_rec])]
         ).reset_index(drop=True)
     return fmtdef
 
 
@@ -153,15 +155,15 @@
                     dt, int(sample_bytes), for_numpy=True
                 )
         except KeyError:
             raise KeyError(
                 f"{data_type} is not a currently-supported data type."
             )
     dtype_spec = fmtdef[
-        [c for c in ("NAME", "dt", "OFFSET") if c in fmtdef.columns]
+        [c for c in ("NAME", "dt", "SB_OFFSET") if c in fmtdef.columns]
     ].to_dict("list")
     spec_keys = ("names", "formats", "offsets")[: len(dtype_spec)]
     return (
         fmtdef,
         np.dtype({k: v for k, v in zip(spec_keys, dtype_spec.values())}),
     )
 
@@ -170,15 +172,37 @@
     table: pd.DataFrame, fmtdef: pd.DataFrame
 ) -> pd.DataFrame:
     boolean_columns = fmtdef.loc[fmtdef["DATA_TYPE"] == "BOOLEAN", "NAME"]
     table[boolean_columns] = table[boolean_columns].astype(bool)
     return table
 
 
+def convert_ebcdic(
+    table: pd.DataFrame, fmtdef: pd.DataFrame
+) -> pd.DataFrame:
+    ebcdic_columns = fmtdef.loc[fmtdef["DATA_TYPE"].str.contains("EBCDIC"), "NAME"]
+    for col in ebcdic_columns:
+        series = pd.Series(table[col])
+        table[col] = series.str.decode('cp500')
+    return table
+
+
 def rectified_rec_df(array: np.ndarray) -> pd.DataFrame:
+    if len(array.shape) == 3:
+        # it's possible to pack 2D arrays into individual records. this
+        # obviously does not work for pandas. if we encounter > 2D elements,
+        # we can generalize this.
+        array = array.reshape(array.shape[0], array.shape[1] * array.shape[2])
+    elif len(array.shape) > 3:
+        raise NotImplementedError("dtypes with >2D elements are not supported")
+    if len(array.dtype) == 0:
+        # if it doesn't have a structured dtype, don't call from_records --
+        # it's slow and acts weird
+        return pd.DataFrame(enforce_order_and_object(array))
+    # but if it does, do
     return pd.DataFrame.from_records(enforce_order_and_object(array))
 
 
 def structured_array_to_df(array: np.ndarray) -> pd.DataFrame:
     sub_dfs = []
     name_buffer = []
     for field in array.dtype.descr:
@@ -191,11 +215,42 @@
             sub_df = rectified_rec_df(array[field[0]])
             sub_df.columns = [
                 f"{field[0]}_{ix}" for ix in range(len(sub_df.columns))
             ]
             sub_dfs.append(sub_df)
     if len(name_buffer) > 0:
         sub_dfs.append(rectified_rec_df(array[name_buffer]))
-    if len(sub_dfs) == 0:
+    if len(sub_dfs) == 1:
         return sub_dfs[0]
-    df = pd.concat(sub_dfs, axis=1)
+    return pd.concat(sub_dfs, axis=1)
+
+
+def convert_ibm_reals(df: pd.DataFrame, fmtdef: pd.DataFrame) -> pd.DataFrame:
+    """
+    converts all IBM reals in a dataframe from packed 16- or 32-bit integer
+    form to floating-point
+    """
+    if not fmtdef['DATA_TYPE'].str.contains('IBM').any():
+        return df
+    reals = {}
+    for _, field in fmtdef.iterrows():
+        if not re.match(r'IBM.*REAL', field['DATA_TYPE']):
+            continue
+        func = ibm32_to_np_f32 if field['BYTES'] == 4 else ibm64_to_np_f64
+        converted = func(df[field['NAME']].values)
+        if field['BYTES'] == 4:
+            # IBM shorts are wider-range than IEEE shorts
+            absolute = abs(converted)
+            big = absolute.max() > np.finfo(np.float32).max
+            nonzero = absolute[absolute > 0]
+            if len(nonzero) > 0:
+                small = nonzero.min() < 1e-44
+            else:
+                small = False
+            if not (big or small):
+                converted = converted.astype(np.float32)
+        reals[field['NAME']] = converted
+        # IBM longs just get more precise, not wider-ranged, so we don't need
+        # to check for longlong or anything like that
+    for k, v in reals.items():
+        df[k] = v
     return df
```

### Comparing `pdr-1.0.1/pdr/pdr.py` & `pdr-1.0.2/pdr/pdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,17 @@
     def load_from_pointer(self, pointer, **load_kwargs):
         from pdr.loaders.dispatch import pointer_to_loader
 
         loader = pointer_to_loader(pointer, self)
         if self.debug is True:
             loader = Dynamic.from_function(loader, optional=True)
         self.loaders[pointer] = loader
-        self.tracker.set_metadata(filename=self.file_mapping[pointer])
+        self.tracker.set_metadata(
+            filename=self.file_mapping[pointer], obj=pointer
+        )
         return self.loaders[pointer](
             self, pointer, tracker=self.tracker, **load_kwargs
         )
 
     def get_scaled(
         self, object_name: str, inplace=False, float_dtype=None
     ) -> "np.ndarray":
```

### Comparing `pdr-1.0.1/pdr/utils.py` & `pdr-1.0.2/pdr/utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.1/pdr.egg-info/PKG-INFO` & `pdr-1.0.2/pdr.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 1.0.1
+Version: 1.0.2
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: notebooks
 Provides-Extra: browsify
 Provides-Extra: fits
 Provides-Extra: tiff
 Provides-Extra: pvl
-License-File: LICENSE
+License-File: LICENSE.md
 
 README.md
 ## The Planetary Data Reader (pdr)
 
 This tool provides a single command---`read(‘/path/to/file’)`---for ingesting
 _all_ common planetary data types. It is currently in development. Almost every kind
 of "primary observational data" product currently archived in the PDS
@@ -166,30 +166,54 @@
 it causes us to break strict PEP-8 standards for attribute capitalization.
 There are three exceptions at present:
 1. Some table formats include repeated column names. For usability and
 compatibility, we force these to be unique by suffixing 0-indexed increasing
 integers. So a table definition with two separate columns named "COLUMN" will 
 return a pandas DataFrame with columns named "COLUMN_0" and "COLUMN_1."
 2. PDS3 data object names sometimes contain spaces. _pdr_ replaces the spaces
-with underscores in order to make them usable as attributes.
+with underscores in order to make them easily usable as Python attributes.
 
 #### PDS4 products
 `pdr.Data` wraps [`pds4_tools`](https://github.com/Small-Bodies-Node/pds4_tools/) 
 to read PDS4 products. All valid PDS4 products should be fully supported. `pdr`
 modifies some `pds4_tools` outputs in order to provide interface and behavior
 consistency. In general, you should be able to use `pdr` with PDS4 products 
 the same way you do with PDS3 products.
 
 Some PDS data products have both PDS3 and PDS4 labels. Data object names, 
 metadata, and even data field names and format specifications often differ 
-slightly between these labels, so `pdr` may produce slightly different outputs
+slightly between these labels, so `pdr.Data` may produce different outputs
 depending on which label you use to initialize it. This is not a bug. 
 However, in general, if a PDS3 label is available, we recommend initializing 
 the object from the PDS3 label rather than the PDS4 label.
 
+#### FITS files
+`pdr.Data` wraps [ `astropy.io.fits` ](https://github.com/astropy/astropy/tree/main/astropy/io/fits)
+to read data from FITS files associated with PDS3 products, and prefers the 
+data specification given in FITS headers to the data specification in the PDS3 
+label. In our experience, because FITS is more rigorously standardized than 
+PDS3, using the FITS header is more reliable; also, the FITS header often 
+contains useful metadata that the PDS3 label does not. `pdr` converts objects 
+produced by`astropy` to `np.ndarrays` (FITS arrays and compressed arrays), 
+`pd.DataFrames` (FITS ASCII and binary tables), or `MultiDicts` (FITS 
+headers), so you do not need to change your code simply because a file is in
+FITS format. 
+
+Whenever you load a data object from a FITS file, `pdr` also 
+places the associated FITS header in a key of your `Data` object named 
+"$objectname_HEADER" -- for instance, if you load an object named "HK_TABLE", 
+its FITS header will appear in `Data.HK_TABLE_HEADER`. You can also use the same 
+name to directly load the header *without* loading the entire data object.
+
+Note that in some cases, the specification in the FITS header may differ 
+from the specification in the PDS3 label, even when the specification in the 
+PDS3 label is technically valid. For instance, column names might be given 
+differently in the FITS header, or a PDS3 TABLE might be stored as a FITS 
+array HDU. 
+
 #### Lazy loading
 Because many planetary data objects are very large, `pdr` helps conserve 
 your time and memory by loading them lazily. It loads data objects into memory
 when they are explicitly referenced, not when `pdr.Data` is initialized. 
 For example, referencing`data.IMAGE` will immediately load the IMAGE object if 
 it has not already been loaded. Alternatively, you can load objects by using 
 the `load` method, like `data.load("IMAGE")`. You can also pass the 'all' 
@@ -203,14 +227,18 @@
 objects loaded from files that are actually present in your filesystem.
 
 #### Big files (like HiRISE)
 `pdr` currently performs no special memory management, so use caution 
 when attempting to read very large files. We intend to implement memory
 management in the future.
 
+#### WSL
+`.jp2` support is not guaranteed for WSL (Windows Subsystem for Linux). It is supported 
+on Windows itself and Linux. 
+
 ### tests
 
 Our testing methodology for *pdr* currently focuses on end-to-end integration
 testing to ensure consistency, coverage of supported datasets, and 
 (to the extent we can verify it) correctness of output.
 
 the test suite for *pdr* lives in a different repository:
```

### Comparing `pdr-1.0.1/pdr.egg-info/SOURCES.txt` & `pdr-1.0.2/pdr.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE
+LICENSE.md
 README.md
 setup.py
 pdr/__init__.py
 pdr/_scaling.py
 pdr/bit_handling.py
 pdr/browsify.py
 pdr/datatypes.py
@@ -10,14 +10,15 @@
 pdr/func.py
 pdr/np_utils.py
 pdr/pd_utils.py
 pdr/pdr.py
 pdr/pdrtypes.py
 pdr/pvl_utils.py
 pdr/utils.py
+pdr/vax.py
 pdr.egg-info/PKG-INFO
 pdr.egg-info/SOURCES.txt
 pdr.egg-info/dependency_links.txt
 pdr.egg-info/requires.txt
 pdr.egg-info/top_level.txt
 pdr/formats/__init__.py
 pdr/formats/cassini.py
@@ -30,17 +31,21 @@
 pdr/formats/lroc.py
 pdr/formats/mex_marsis.py
 pdr/formats/mgn.py
 pdr/formats/mgs.py
 pdr/formats/msl_apxs.py
 pdr/formats/msl_ccam.py
 pdr/formats/msl_cmn.py
+pdr/formats/near.py
+pdr/formats/nh.py
+pdr/formats/odyssey.py
 pdr/formats/pvo.py
 pdr/formats/rosetta.py
 pdr/formats/themis.py
+pdr/formats/vega.py
 pdr/loaders/__init__.py
 pdr/loaders/_helpers.py
 pdr/loaders/datawrap.py
 pdr/loaders/dispatch.py
 pdr/loaders/handlers.py
 pdr/loaders/image.py
 pdr/loaders/queries.py
```

### Comparing `pdr-1.0.1/setup.py` & `pdr-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdr",
-    version="1.0.1",
+    version="1.0.2",
     author="Chase Million",
     author_email="chase@millionconcepts.com",
     description="Planetary Data Reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MillionConcepts/pdr",
     packages=setuptools.find_packages(),
```

