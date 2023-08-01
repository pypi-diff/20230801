# Comparing `tmp/modelcraft-3.2.0.tar.gz` & `tmp/modelcraft-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelcraft-3.2.0.tar", last modified: Mon Jul 10 17:38:20 2023, max compression
+gzip compressed data, was "modelcraft-3.3.0.tar", last modified: Tue Aug  1 12:47:55 2023, max compression
```

## Comparing `modelcraft-3.2.0.tar` & `modelcraft-3.3.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.402209 modelcraft-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-10 17:38:10.000000 modelcraft-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 17:38:10.000000 modelcraft-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-10 17:38:20.402209 modelcraft-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 17:38:10.000000 modelcraft-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.394209 modelcraft-3.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.398209 modelcraft-3.2.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 17:38:10.000000 modelcraft-3.2.0/docs/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-10 17:38:10.000000 modelcraft-3.2.0/docs/css/milligram.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-10 17:38:10.000000 modelcraft-3.2.0/docs/css/normalize.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.398209 modelcraft-3.2.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    39305 2023-07-10 17:38:10.000000 modelcraft-3.2.0/docs/img/modelcraft.png
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-07-10 17:38:10.000000 modelcraft-3.2.0/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.398209 modelcraft-3.2.0/modelcraft/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/contents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.398209 modelcraft-3.2.0/modelcraft/coot/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/coot/morph.py
--rw-r--r--   0 runner    (1001) docker     (123)    35851 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/coot/prune.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/coot/sidechains.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.398209 modelcraft-3.2.0/modelcraft/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/acedrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/acorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/buccaneer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/comit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/coot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/ctruncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/emda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/findwaters.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/freerflag.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/libg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/molrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/nautilus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/parrot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/phasematch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/refmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/servalcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/jobs/sheetbend.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/modelcraftem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12350 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/modelcraftxray.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/monlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/reflections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.402209 modelcraft-3.2.0/modelcraft/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/scripts/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/scripts/copies.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/scripts/modelcraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/solvent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.402209 modelcraft-3.2.0/modelcraft/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.402209 modelcraft-3.2.0/modelcraft/tests/ccp4/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_acedrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_buccaneer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_comit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_coot.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_copies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_ctruncate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_findwaters.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_freerflag.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_libg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_molrep.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_monlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_nautilus.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_parrot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_phasematch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_reflections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_refmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_sheetbend.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_solvent.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccp4/test_xray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.402209 modelcraft-3.2.0/modelcraft/tests/ccpem/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccpem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccpem/test_em.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccpem/test_emda.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccpem/test_refmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/ccpem/test_servalcat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.402209 modelcraft-3.2.0/modelcraft/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/unittests/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/tests/unittests/test_reflections.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-10 17:38:10.000000 modelcraft-3.2.0/modelcraft/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:38:20.398209 modelcraft-3.2.0/modelcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-10 17:38:20.000000 modelcraft-3.2.0/modelcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-10 17:38:20.000000 modelcraft-3.2.0/modelcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:38:20.000000 modelcraft-3.2.0/modelcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 17:38:20.000000 modelcraft-3.2.0/modelcraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 17:38:20.000000 modelcraft-3.2.0/modelcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 17:38:20.000000 modelcraft-3.2.0/modelcraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 17:38:20.402209 modelcraft-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-10 17:38:10.000000 modelcraft-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.552776 modelcraft-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-08-01 12:47:46.000000 modelcraft-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 12:47:46.000000 modelcraft-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-08-01 12:47:55.552776 modelcraft-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-01 12:47:46.000000 modelcraft-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.524776 modelcraft-3.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.524776 modelcraft-3.3.0/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 12:47:46.000000 modelcraft-3.3.0/docs/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-08-01 12:47:46.000000 modelcraft-3.3.0/docs/css/milligram.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-08-01 12:47:46.000000 modelcraft-3.3.0/docs/css/normalize.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.524776 modelcraft-3.3.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    39305 2023-08-01 12:47:46.000000 modelcraft-3.3.0/docs/img/modelcraft.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-08-01 12:47:46.000000 modelcraft-3.3.0/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.528776 modelcraft-3.3.0/modelcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/contents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.532776 modelcraft-3.3.0/modelcraft/coot/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/coot/morph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35851 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/coot/prune.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/coot/sidechains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.536776 modelcraft-3.3.0/modelcraft/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/acedrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/acorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/buccaneer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/comit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/coot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/ctruncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/emda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/findwaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/freerflag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/libg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/molrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/nautilus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/parrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/phasematch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/refmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/servalcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/jobs/sheetbend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/modelcraftem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12350 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/modelcraftxray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/monlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/reflections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.540776 modelcraft-3.3.0/modelcraft/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/scripts/contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/scripts/copies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/scripts/modelcraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/solvent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.540776 modelcraft-3.3.0/modelcraft/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.548776 modelcraft-3.3.0/modelcraft/tests/ccp4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_acedrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_buccaneer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_comit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_coot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_copies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_ctruncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_findwaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_freerflag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_libg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_molrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_monlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_nautilus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_parrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_phasematch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_refmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_sheetbend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_solvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccp4/test_xray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.548776 modelcraft-3.3.0/modelcraft/tests/ccpem/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccpem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccpem/test_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccpem/test_emda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccpem/test_refmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/ccpem/test_servalcat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.552776 modelcraft-3.3.0/modelcraft/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/unittests/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/tests/unittests/test_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 12:47:46.000000 modelcraft-3.3.0/modelcraft/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:55.532776 modelcraft-3.3.0/modelcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-08-01 12:47:55.000000 modelcraft-3.3.0/modelcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-01 12:47:55.000000 modelcraft-3.3.0/modelcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:47:55.000000 modelcraft-3.3.0/modelcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 12:47:55.000000 modelcraft-3.3.0/modelcraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 12:47:55.000000 modelcraft-3.3.0/modelcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 12:47:55.000000 modelcraft-3.3.0/modelcraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-01 12:47:55.552776 modelcraft-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-01 12:47:46.000000 modelcraft-3.3.0/setup.py
```

### Comparing `modelcraft-3.2.0/LICENSE` & `modelcraft-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/PKG-INFO` & `modelcraft-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelcraft
-Version: 3.2.0
+Version: 3.3.0
 Summary: Automated model building pipeline for X-ray crystallography
 Home-page: https://github.com/paulsbond/modelcraft
 Author: Paul Bond
 Author-email: paul.bond@york.ac.uk
 License: LGPL-2.1
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `modelcraft-3.2.0/README.md` & `modelcraft-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/docs/css/milligram.min.css` & `modelcraft-3.3.0/docs/css/milligram.min.css`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/docs/css/normalize.min.css` & `modelcraft-3.3.0/docs/css/normalize.min.css`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/docs/img/modelcraft.png` & `modelcraft-3.3.0/docs/img/modelcraft.png`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/docs/index.html` & `modelcraft-3.3.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/__init__.py` & `modelcraft-3.3.0/modelcraft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 
 from .cell import max_distortion as max_cell_distortion
 from .cell import remove_scale
 from .cell import update_cell
 from .contents import AsuContents
 from .contents import PolymerType
 from .geometry import rmsz
```

### Comparing `modelcraft-3.2.0/modelcraft/arguments.py` & `modelcraft-3.3.0/modelcraft/arguments.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/cell.py` & `modelcraft-3.3.0/modelcraft/cell.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/contents.py` & `modelcraft-3.3.0/modelcraft/contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/coot/morph.py` & `modelcraft-3.3.0/modelcraft/coot/morph.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/coot/prune.py` & `modelcraft-3.3.0/modelcraft/coot/prune.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/coot/sidechains.py` & `modelcraft-3.3.0/modelcraft/coot/sidechains.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/environ.py` & `modelcraft-3.3.0/modelcraft/environ.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/geometry.py` & `modelcraft-3.3.0/modelcraft/geometry.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/job.py` & `modelcraft-3.3.0/modelcraft/job.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/acedrg.py` & `modelcraft-3.3.0/modelcraft/jobs/acedrg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/acorn.py` & `modelcraft-3.3.0/modelcraft/jobs/acorn.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/buccaneer.py` & `modelcraft-3.3.0/modelcraft/jobs/buccaneer.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/comit.py` & `modelcraft-3.3.0/modelcraft/jobs/comit.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/coot.py` & `modelcraft-3.3.0/modelcraft/jobs/coot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/ctruncate.py` & `modelcraft-3.3.0/modelcraft/jobs/ctruncate.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/emda.py` & `modelcraft-3.3.0/modelcraft/jobs/emda.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/findwaters.py` & `modelcraft-3.3.0/modelcraft/jobs/findwaters.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/freerflag.py` & `modelcraft-3.3.0/modelcraft/jobs/freerflag.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/libg.py` & `modelcraft-3.3.0/modelcraft/jobs/libg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/molrep.py` & `modelcraft-3.3.0/modelcraft/jobs/molrep.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/nautilus.py` & `modelcraft-3.3.0/modelcraft/jobs/nautilus.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/parrot.py` & `modelcraft-3.3.0/modelcraft/jobs/parrot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/phasematch.py` & `modelcraft-3.3.0/modelcraft/jobs/phasematch.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/refmac.py` & `modelcraft-3.3.0/modelcraft/jobs/refmac.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         freer: DataItem,
         phases: DataItem = None,
         cycles: int = 5,
         twinned: bool = False,
         jelly_body: bool = False,
         libin: str = None,
     ):
-        super().__init__("refmac5")
+        super().__init__("refmacat")
         self.structure = structure
         self.fsigf = fsigf
         self.freer = freer
         self.phases = phases
         self.cycles = cycles
         self.twinned = twinned
         self.jelly_body = jelly_body
@@ -113,15 +113,15 @@
 class RefmacMapToMtzResult:
     fphi: DataItem
     seconds: float
 
 
 class RefmacMapToMtz(Job):
     def __init__(self, density: gemmi.Ccp4Map, resolution: float, blur: float = 0):
-        super().__init__("refmac5")
+        super().__init__("refmacat")
         self.density = density
         self.resolution = resolution
         self.blur = blur
 
     def _setup(self) -> None:
         self.density.write_ccp4_map(self._path("mapin.ccp4"))
         self._args += ["MAPIN", "mapin.ccp4"]
```

### Comparing `modelcraft-3.2.0/modelcraft/jobs/servalcat.py` & `modelcraft-3.3.0/modelcraft/jobs/servalcat.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/jobs/sheetbend.py` & `modelcraft-3.3.0/modelcraft/jobs/sheetbend.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/modelcraftem.py` & `modelcraft-3.3.0/modelcraft/modelcraftem.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/modelcraftxray.py` & `modelcraft-3.3.0/modelcraft/modelcraftxray.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/monlib.py` & `modelcraft-3.3.0/modelcraft/monlib.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/pipeline.py` & `modelcraft-3.3.0/modelcraft/pipeline.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/reflections.py` & `modelcraft-3.3.0/modelcraft/reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/scripts/contents.py` & `modelcraft-3.3.0/modelcraft/scripts/contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/scripts/copies.py` & `modelcraft-3.3.0/modelcraft/scripts/copies.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/solvent.py` & `modelcraft-3.3.0/modelcraft/solvent.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/structure.py` & `modelcraft-3.3.0/modelcraft/structure.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/__init__.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/__init__.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_acedrg.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_acedrg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_arguments.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_arguments.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_buccaneer.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_buccaneer.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_cell.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_cell.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_comit.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_comit.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_contents.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_coot.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_coot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_ctruncate.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_ctruncate.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_findwaters.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_findwaters.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_geometry.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_geometry.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_molrep.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_molrep.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_monlib.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_monlib.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_nautilus.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_nautilus.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_parrot.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_parrot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_phasematch.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_phasematch.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_reflections.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_refmac.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_refmac.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_sheetbend.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_sheetbend.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_solvent.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_solvent.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccp4/test_xray.py` & `modelcraft-3.3.0/modelcraft/tests/ccp4/test_xray.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccpem/__init__.py` & `modelcraft-3.3.0/modelcraft/tests/ccpem/__init__.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccpem/test_em.py` & `modelcraft-3.3.0/modelcraft/tests/ccpem/test_em.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/ccpem/test_servalcat.py` & `modelcraft-3.3.0/modelcraft/tests/ccpem/test_servalcat.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/unittests/test_contents.py` & `modelcraft-3.3.0/modelcraft/tests/unittests/test_contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft/tests/unittests/test_reflections.py` & `modelcraft-3.3.0/modelcraft/tests/unittests/test_reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/modelcraft.egg-info/PKG-INFO` & `modelcraft-3.3.0/modelcraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelcraft
-Version: 3.2.0
+Version: 3.3.0
 Summary: Automated model building pipeline for X-ray crystallography
 Home-page: https://github.com/paulsbond/modelcraft
 Author: Paul Bond
 Author-email: paul.bond@york.ac.uk
 License: LGPL-2.1
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `modelcraft-3.2.0/modelcraft.egg-info/SOURCES.txt` & `modelcraft-3.3.0/modelcraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelcraft-3.2.0/setup.py` & `modelcraft-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 setuptools.setup(
     name="modelcraft",
-    version="3.2.0",
+    version="3.3.0",
     author="Paul Bond",
     author_email="paul.bond@york.ac.uk",
     description="Automated model building pipeline for X-ray crystallography",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/paulsbond/modelcraft",
     packages=setuptools.find_packages(),
```

