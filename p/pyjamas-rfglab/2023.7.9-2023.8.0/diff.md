# Comparing `tmp/pyjamas-rfglab-2023.7.9.tar.gz` & `tmp/pyjamas-rfglab-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjamas-rfglab-2023.7.9.tar", last modified: Wed Jul 19 16:58:16 2023, max compression
+gzip compressed data, was "pyjamas-rfglab-2023.8.0.tar", last modified: Tue Aug  1 21:48:34 2023, max compression
```

## Comparing `pyjamas-rfglab-2023.7.9.tar` & `pyjamas-rfglab-2023.8.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.940948 pyjamas-rfglab-2023.7.9/
--rw-r--r--   0 rodrigo    (501) staff       (20)      265 2023-01-17 21:44:31.000000 pyjamas-rfglab-2023.7.9/MANIFEST.in
--rw-r--r--   0 rodrigo    (501) staff       (20)     1686 2023-07-19 16:58:16.939581 pyjamas-rfglab-2023.7.9/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     1202 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.7.9/README.md
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.833583 pyjamas-rfglab-2023.7.9/pyjamas/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33144 2020-02-04 05:51:32.000000 pyjamas-rfglab-2023.7.9/pyjamas/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     1088 2020-01-17 04:15:16.000000 pyjamas-rfglab-2023.7.9/pyjamas/__init__.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.903732 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1645 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    17513 2020-07-11 20:07:12.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/adjustcontrast.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    28797 2022-10-11 19:50:28.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/batchanalysis.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5453 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/batchprojectconcat.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6858 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/batchresize.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2980 2021-10-30 00:59:57.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/classifierdialogABC.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3143 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/classifiertype.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6381 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/expandnpropagateseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5171 2021-10-31 01:33:53.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/expandseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12944 2022-04-23 19:28:25.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/findseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11319 2021-10-30 00:56:56.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/logregression.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3432 2021-10-30 00:59:57.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/matplotlibdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     8762 2021-10-31 01:33:53.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/measurepoly.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13235 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/neuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     8642 2023-02-19 02:47:22.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/nonmax_suppr.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     5477 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/propagateseeds.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    14546 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/rescuneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12468 2021-10-30 01:12:49.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/svm.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2233 2020-05-13 06:00:08.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/textdialog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     4026 2021-10-30 01:12:49.000000 pyjamas-rfglab-2023.7.9/pyjamas/dialogs/timepoints.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1793 2021-08-22 22:40:45.000000 pyjamas-rfglab-2023.7.9/pyjamas/dragdropmainwindow.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.905242 pyjamas-rfglab-2023.7.9/pyjamas/external/
--rw-r--r--   0 rodrigo    (501) staff       (20)      899 2021-05-09 22:07:44.000000 pyjamas-rfglab-2023.7.9/pyjamas/external/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6852 2020-07-11 20:09:58.000000 pyjamas-rfglab-2023.7.9/pyjamas/external/pascal_voc_io.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     4901 2023-01-22 21:23:16.000000 pyjamas-rfglab-2023.7.9/pyjamas/orthogonalviewswindow.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    52550 2023-07-19 16:54:55.000000 pyjamas-rfglab-2023.7.9/pyjamas/pjscore.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    32616 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/pjseventfilter.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2123 2020-02-19 06:14:09.000000 pyjamas-rfglab-2023.7.9/pyjamas/pjsthreads.py
--rw-r--r--   0 rodrigo    (501) staff       (20)  2950837 2023-06-21 15:47:44.000000 pyjamas-rfglab-2023.7.9/pyjamas/pyjamas.tif
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.909136 pyjamas-rfglab-2023.7.9/pyjamas/rannotations/
--rw-r--r--   0 rodrigo    (501) staff       (20)      924 2022-06-20 21:44:00.000000 pyjamas-rfglab-2023.7.9/pyjamas/rannotations/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      856 2020-01-17 04:15:16.000000 pyjamas-rfglab-2023.7.9/pyjamas/rannotations/rannotation.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    16818 2023-01-29 04:49:19.000000 pyjamas-rfglab-2023.7.9/pyjamas/rannotations/rpolyline.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2288 2022-08-14 20:59:38.000000 pyjamas-rfglab-2023.7.9/pyjamas/rannotations/rvector2d.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.917108 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1257 2020-01-17 04:15:16.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7690 2023-06-21 15:47:44.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcallback.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1658 2023-02-07 15:13:59.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbabout.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    13560 2023-03-16 20:28:45.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbannotations.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    70337 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbbatchprocess.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    66441 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbclassifiers.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    77409 2023-02-22 03:17:35.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbimage.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    52722 2023-04-24 20:27:21.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbio.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11288 2022-12-29 14:40:38.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbmeasure.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12556 2023-03-16 20:12:57.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcboptions.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3617 2022-08-11 04:10:01.000000 pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbplugins.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.919657 pyjamas-rfglab-2023.7.9/pyjamas/rimage/
--rw-r--r--   0 rodrigo    (501) staff       (20)      913 2020-05-28 03:02:49.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3091 2021-08-22 22:13:16.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/csgraph.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3799 2023-03-14 22:07:07.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimcore.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.933400 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/
--rw-r--r--   0 rodrigo    (501) staff       (20)     1484 2021-02-14 22:27:21.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3557 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/batchclassifier.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1585 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/batchml.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2740 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/batchneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     7409 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/batchrecurrentneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      275 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/classifier_types.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1173 2020-08-28 21:52:01.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/featurecalculator.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1387 2020-12-27 23:49:18.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/featurecalculator_rawimage.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1289 2020-12-27 23:49:18.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     3196 2021-10-27 19:58:57.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/featurecalculator_sog.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    17339 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimclassifier.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1824 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimlr.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1382 2021-10-27 20:01:04.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimml.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1857 2021-10-27 20:01:04.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1960 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimrecurrentneuralnet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    20979 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimrescunet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     2084 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimsvm.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    15508 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimunet.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    67108 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimutils.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.935259 pyjamas-rfglab-2023.7.9/pyjamas/rplugins/
--rw-r--r--   0 rodrigo    (501) staff       (20)      847 2020-01-17 04:15:16.000000 pyjamas-rfglab-2023.7.9/pyjamas/rplugins/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     1249 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.7.9/pyjamas/rplugins/base.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    26659 2022-11-12 20:45:29.000000 pyjamas-rfglab-2023.7.9/pyjamas/rutils.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.936332 pyjamas-rfglab-2023.7.9/pyjamas/tests/
--rw-r--r--   0 rodrigo    (501) staff       (20)      796 2023-01-02 00:28:47.000000 pyjamas-rfglab-2023.7.9/pyjamas/tests/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)      857 2023-01-19 20:27:03.000000 pyjamas-rfglab-2023.7.9/pyjamas/tests/conftest.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.938266 pyjamas-rfglab-2023.7.9/pyjamas/tests/unit/
--rw-r--r--   0 rodrigo    (501) staff       (20)        0 2022-12-25 02:03:19.000000 pyjamas-rfglab-2023.7.9/pyjamas/tests/unit/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)     6326 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.7.9/pyjamas/tests/unit/pjsfixtures.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    12486 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.7.9/pyjamas/tests/unit/test_image.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    16795 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.7.9/pyjamas/tests/unit/test_io.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-19 16:58:16.938867 pyjamas-rfglab-2023.7.9/pyjamas_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     2494 2023-07-19 16:58:14.000000 pyjamas-rfglab-2023.7.9/pyjamas_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-07-19 16:58:16.941167 pyjamas-rfglab-2023.7.9/setup.cfg
--rw-r--r--   0 rodrigo    (501) staff       (20)     2924 2023-07-17 01:06:25.000000 pyjamas-rfglab-2023.7.9/setup.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.234128 pyjamas-rfglab-2023.8.0/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      265 2023-01-17 21:44:31.000000 pyjamas-rfglab-2023.8.0/MANIFEST.in
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1686 2023-08-01 21:48:34.232807 pyjamas-rfglab-2023.8.0/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1202 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.8.0/README.md
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.166028 pyjamas-rfglab-2023.8.0/pyjamas/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33144 2020-02-04 05:51:32.000000 pyjamas-rfglab-2023.8.0/pyjamas/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1088 2020-01-17 04:15:16.000000 pyjamas-rfglab-2023.8.0/pyjamas/__init__.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.187516 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1645 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    17513 2020-07-11 20:07:12.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/adjustcontrast.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    28797 2022-10-11 19:50:28.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/batchanalysis.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5453 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/batchprojectconcat.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6858 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/batchresize.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2980 2021-10-30 00:59:57.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/classifierdialogABC.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3143 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/classifiertype.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6381 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/expandnpropagateseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5171 2021-10-31 01:33:53.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/expandseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12944 2022-04-23 19:28:25.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/findseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11319 2021-10-30 00:56:56.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/logregression.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3432 2021-10-30 00:59:57.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/matplotlibdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     8762 2021-10-31 01:33:53.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/measurepoly.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13235 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/neuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     8642 2023-02-19 02:47:22.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/nonmax_suppr.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     5477 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/propagateseeds.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    14546 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/rescuneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12468 2021-10-30 01:12:49.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/svm.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2233 2020-05-13 06:00:08.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/textdialog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4026 2021-10-30 01:12:49.000000 pyjamas-rfglab-2023.8.0/pyjamas/dialogs/timepoints.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1793 2021-08-22 22:40:45.000000 pyjamas-rfglab-2023.8.0/pyjamas/dragdropmainwindow.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.188490 pyjamas-rfglab-2023.8.0/pyjamas/external/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      899 2021-05-09 22:07:44.000000 pyjamas-rfglab-2023.8.0/pyjamas/external/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6852 2020-07-11 20:09:58.000000 pyjamas-rfglab-2023.8.0/pyjamas/external/pascal_voc_io.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     4901 2023-01-22 21:23:16.000000 pyjamas-rfglab-2023.8.0/pyjamas/orthogonalviewswindow.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    52524 2023-08-01 21:47:42.000000 pyjamas-rfglab-2023.8.0/pyjamas/pjscore.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    32610 2023-07-31 21:14:06.000000 pyjamas-rfglab-2023.8.0/pyjamas/pjseventfilter.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2123 2020-02-19 06:14:09.000000 pyjamas-rfglab-2023.8.0/pyjamas/pjsthreads.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)  2950837 2023-06-21 15:47:44.000000 pyjamas-rfglab-2023.8.0/pyjamas/pyjamas.tif
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.192385 pyjamas-rfglab-2023.8.0/pyjamas/rannotations/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      924 2022-06-20 21:44:00.000000 pyjamas-rfglab-2023.8.0/pyjamas/rannotations/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      856 2020-01-17 04:15:16.000000 pyjamas-rfglab-2023.8.0/pyjamas/rannotations/rannotation.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    16818 2023-01-29 04:49:19.000000 pyjamas-rfglab-2023.8.0/pyjamas/rannotations/rpolyline.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2288 2022-08-14 20:59:38.000000 pyjamas-rfglab-2023.8.0/pyjamas/rannotations/rvector2d.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.203848 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1257 2020-01-17 04:15:16.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7690 2023-06-21 15:47:44.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcallback.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1658 2023-02-07 15:13:59.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbabout.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    13558 2023-07-31 21:14:06.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbannotations.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    70337 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbbatchprocess.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    66441 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbclassifiers.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    77409 2023-02-22 03:17:35.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbimage.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    52722 2023-04-24 20:27:21.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbio.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11288 2022-12-29 14:40:38.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbmeasure.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12553 2023-07-31 21:14:06.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcboptions.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3617 2022-08-11 04:10:01.000000 pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbplugins.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.206304 pyjamas-rfglab-2023.8.0/pyjamas/rimage/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      913 2020-05-28 03:02:49.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3091 2021-08-22 22:13:16.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/csgraph.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3862 2023-07-31 21:14:06.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimcore.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.222618 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1484 2021-02-14 22:27:21.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3557 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/batchclassifier.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1585 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/batchml.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2740 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/batchneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     7409 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/batchrecurrentneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      275 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/classifier_types.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1173 2020-08-28 21:52:01.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/featurecalculator.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1387 2020-12-27 23:49:18.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/featurecalculator_rawimage.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1289 2020-12-27 23:49:18.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3196 2021-10-27 19:58:57.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/featurecalculator_sog.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    17339 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimclassifier.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1824 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimlr.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1382 2021-10-27 20:01:04.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimml.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1857 2021-10-27 20:01:04.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1960 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimrecurrentneuralnet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    20979 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimrescunet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2084 2023-04-12 16:40:46.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimsvm.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    15508 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimunet.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    67059 2023-08-01 21:47:42.000000 pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimutils.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.224022 pyjamas-rfglab-2023.8.0/pyjamas/rplugins/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      847 2020-01-17 04:15:16.000000 pyjamas-rfglab-2023.8.0/pyjamas/rplugins/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     1249 2023-02-19 02:47:05.000000 pyjamas-rfglab-2023.8.0/pyjamas/rplugins/base.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    26659 2022-11-12 20:45:29.000000 pyjamas-rfglab-2023.8.0/pyjamas/rutils.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.227894 pyjamas-rfglab-2023.8.0/pyjamas/tests/
+-rw-r--r--   0 rodrigo    (501) staff       (20)      796 2023-01-02 00:28:47.000000 pyjamas-rfglab-2023.8.0/pyjamas/tests/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)      857 2023-01-19 20:27:03.000000 pyjamas-rfglab-2023.8.0/pyjamas/tests/conftest.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.230718 pyjamas-rfglab-2023.8.0/pyjamas/tests/unit/
+-rw-r--r--   0 rodrigo    (501) staff       (20)        0 2022-12-25 02:03:19.000000 pyjamas-rfglab-2023.8.0/pyjamas/tests/unit/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)     6326 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.8.0/pyjamas/tests/unit/pjsfixtures.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12486 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.8.0/pyjamas/tests/unit/test_image.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    16795 2023-07-11 19:12:22.000000 pyjamas-rfglab-2023.8.0/pyjamas/tests/unit/test_io.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-08-01 21:48:34.232039 pyjamas-rfglab-2023.8.0/pyjamas_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2494 2023-08-01 21:48:33.000000 pyjamas-rfglab-2023.8.0/pyjamas_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-08-01 21:48:34.234326 pyjamas-rfglab-2023.8.0/setup.cfg
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2924 2023-07-17 01:06:25.000000 pyjamas-rfglab-2023.8.0/setup.py
```

### Comparing `pyjamas-rfglab-2023.7.9/PKG-INFO` & `pyjamas-rfglab-2023.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjamas-rfglab
-Version: 2023.7.9
+Version: 2023.8.0
 Summary: PyJAMAS is Just A More Awesome SIESTA
 Home-page: https://bitbucket.org/rfg_lab/pyjamas
 Author: Rodrigo Fernandez-Gonzalez
 Author-email: rodrigo.fernandez.gonzalez@utoronto.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjamas-rfglab-2023.7.9/README.md` & `pyjamas-rfglab-2023.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/LICENSE` & `pyjamas-rfglab-2023.8.0/pyjamas/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/adjustcontrast.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/adjustcontrast.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/batchanalysis.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/batchanalysis.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/batchprojectconcat.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/batchprojectconcat.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/batchresize.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/batchresize.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/classifierdialogABC.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/classifierdialogABC.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/classifiertype.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/classifiertype.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/expandnpropagateseeds.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/expandnpropagateseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/expandseeds.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/expandseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/findseeds.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/findseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/logregression.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/logregression.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/matplotlibdialog.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/matplotlibdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/measurepoly.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/measurepoly.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/neuralnet.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/neuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/nonmax_suppr.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/nonmax_suppr.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/propagateseeds.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/propagateseeds.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/rescuneuralnet.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/rescuneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/svm.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/svm.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/textdialog.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/textdialog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dialogs/timepoints.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dialogs/timepoints.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/dragdropmainwindow.py` & `pyjamas-rfglab-2023.8.0/pyjamas/dragdropmainwindow.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/external/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/external/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/external/pascal_voc_io.py` & `pyjamas-rfglab-2023.8.0/pyjamas/external/pascal_voc_io.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/orthogonalviewswindow.py` & `pyjamas-rfglab-2023.8.0/pyjamas/orthogonalviewswindow.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/pjscore.py` & `pyjamas-rfglab-2023.8.0/pyjamas/pjscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,21 +119,21 @@
     fiducial_brush_style: QtGui.QBrush = QtGui.QBrush()  # No fill for fiducials (open circles).
     polyline_brush_style: QtGui.QBrush = QtGui.QBrush()
     fiducial_font: QtGui.QFont = QtGui.QFont('Arial', 8)
 
     zoom_factors: tuple = (1., 2., 4., 8., .125, .25, .5)
 
     livewire_margin: int = 5
-    livewire_heuristic_weight: float = 0.  # defaults to Dijkstra.
+    livewire_gaussian_sigma: float = 0.
     balloon_crop_size: int = 50  # crop size used to inflate balloons
 
     undo_stack_size: int = 500
 
     # Read version.
-    __version__: str = '2023.7.9'
+    __version__: str = '2023.8.0'
 
     def __init__(self):
         self.initData()  # Initialize object variables.
         self.setupUI()  # Build the GUI.
 
     def setupUI(self):
         self.app = QtWidgets.QApplication(sys.argv)
@@ -309,16 +309,16 @@
         self.addMenuItem(self.menuOptions, 'Set working folder ...', None, self.options.cbSetCWD)
 
         self.addMenuItem(self.menuOptions, 'Set crop margins ...', None, self.options.cbSetMarginSize)
 
         self.addMenuItem(self.menuOptions, 'Set balloon crop size ...', None,
                          self.options.cbSetImageProcessingCropSize)
 
-        self.addMenuItem(self.menuOptions, 'LiveWire heuristic weight ...', None,
-                         self.options.cbSetLiveWireHeuristicWeight)
+        self.addMenuItem(self.menuOptions, 'LiveWire Gaussian smoothing ...', None,
+                         self.options.cbSetLiveWireSmoothGaussian)
 
         self.addMenuItem(self.menuOptions, 'Toggle crop tracked polyline', None, self.options.cbCropTracked)
 
         self.addMenuItem(self.menuOptions, 'Dark/light display theme', None,
                          self.options.cbChangeDisplayTheme)
 
         self.menubar.addMenu(self.menuOptions)
```

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/pjseventfilter.py` & `pyjamas-rfglab-2023.8.0/pyjamas/pjseventfilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,15 +263,15 @@
                         if event.buttons() == QtCore.Qt.LeftButton:
                             if self.pjs._poly_ != []:
                                 thesource = self.pjs._poly_[-1][::-1]
                                 thedest = [self.y, self.x]
                                 thepoints = rimage(self.pjs.imagedata).livewire(thesource, thedest,
                                                                                 PyJAMAS.livewire_margin,
                                                                                 True,
-                                                                                self.pjs.livewire_heuristic_weight)  # Make livewire a static method?
+                                                                                self.pjs.livewire_gaussian_sigma)  # Make livewire a static method?
                                 self.pjs._poly_.extend(
                                     thepoints)  ### CHANGE: STORE ALL COORDINATES GENERATED BY LIVEWIRE FROM LAST CLICKED POINT
 
                                 if self.pjs._agraphicsitem_ and self.pjs._agraphicsitem_.scene():
                                     self.pjs.gScene.removeItem(self.pjs._agraphicsitem_)
 
                                 self.pjs._agraphicsitem_, _ = self.pjs.drawPath(self.pjs._poly_)
@@ -303,15 +303,15 @@
 
                             apoly = self.pjs._poly_.copy()
                             thesource = apoly.copy()[-1][::-1]
                             thedest = [self.y, self.x]
                             thepoints = rimage(self.pjs.imagedata).livewire(thesource, thedest,
                                                                             PyJAMAS.livewire_margin,
                                                                             True,
-                                                                            self.pjs.livewire_heuristic_weight)  # Make livewire a static method? Or make self.imagedata an RImage?
+                                                                            self.pjs.livewire_gaussian_sigma)  # Make livewire a static method? Or make self.imagedata an RImage?
                             apoly.extend(
                                 thepoints)  ### CHANGE: STORE ALL COORDINATES GENERATED BY LIVEWIRE FROM LAST CLICKED POINT
 
                             self.pjs._agraphicsitem_, _ = self.pjs.drawPath(apoly)
                             # self.statusbar.showMessage(str(self.curslice + 1) + '/' + str(self.n_frames) + '\t(' + str(self._poly_[0]) + ', ' + str(
                             # self._poly_[1]) + ') -> w: ' + str(abs(self._poly_[0] - self.x)) + ', h: ' + str(abs(self._poly_[1] - self.y)))
 
@@ -328,15 +328,15 @@
                         modifierPressed = QtWidgets.QApplication.keyboardModifiers()
                         if (modifierPressed & QtCore.Qt.ShiftModifier) != QtCore.Qt.ShiftModifier:
                             thesource = self.pjs._poly_[-1][::-1]
                             thedest = self.pjs._poly_[0][::-1]
                             thepoints = rimage(self.pjs.imagedata).livewire(thesource, thedest,
                                                                             PyJAMAS.livewire_margin,
                                                                             True,
-                                                                            self.pjs.livewire_heuristic_weight)  # Make livewire a static method? Or make self.imagedata an RImage?
+                                                                            self.pjs.livewire_gaussian_sigma)  # Make livewire a static method? Or make self.imagedata an RImage?
                             self.pjs._poly_.extend(thepoints)
 
                         self.pjs.addPolyline(self.pjs._poly_, self.pjs.curslice, pushundo=True)
                         self.pjs._poly_ = []
 
                 else:
                     self.pjs._poly_ = []
```

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/pjsthreads.py` & `pyjamas-rfglab-2023.8.0/pyjamas/pjsthreads.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/pyjamas.tif` & `pyjamas-rfglab-2023.8.0/pyjamas/pyjamas.tif`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rannotations/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rannotations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rannotations/rannotation.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rannotations/rannotation.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rannotations/rpolyline.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rannotations/rpolyline.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rannotations/rvector2d.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rannotations/rvector2d.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcallback.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcallback.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbabout.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbabout.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbannotations.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbannotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         return True
 
     def cbLiveWire(self) -> bool:
         """
         Set annotation mode to add/remove polylines using the LiveWire algorithm for semi-automated object delineation.
         The LiveWire is implemented using an A* algorithm, with a Euclidean distance heuristic that is weighted by
-        self.pjs.livewire_heuristic_weight (a weight of 0.0 is the equivalent of Dijkstra's minimal cost path search).
+        self.pjs.livewire_gaussian_sigma (a weight of 0.0 is the equivalent of Dijkstra's minimal cost path search).
 
         :return: True.
         """
 
         self.pjs.annotation_mode = PyJAMAS.livewire_annotations
         QtWidgets.QApplication.setOverrideCursor(QtCore.Qt.CrossCursor)
```

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbbatchprocess.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbbatchprocess.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbclassifiers.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbclassifiers.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbimage.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbimage.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbio.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbio.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbmeasure.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbmeasure.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcboptions.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcboptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -313,32 +313,32 @@
         if self.pjs.close_all_polylines:
             self.pjs.statusbar.showMessage('Close all polylines turned ON.')
         else:
             self.pjs.statusbar.showMessage('Close all polylines turned OFF.')
 
         return True
 
-    def cbSetLiveWireHeuristicWeight(self, weight: Optional[float] = None) -> bool:
+    def cbSetLiveWireSmoothGaussian(self, sigma: Optional[float] = None) -> bool:
         """
-        Set the weight of the distance heuristic used in the A* algorithm for LiveWire segmentation.
-        A weight of 0.0 is equivalent to Dijkstra's algorithm.
+        Set the standard deviation of the Gaussian used to smoothen images for LiveWire segmentation.
+        A weight of 0.0 is no smoothing.
 
-        :param weight: weight assigned to distance heuristic.
-        :return: True if heuristic weight was changed, False otherwise.
+        :param sigma: standard deviation of the Gaussian used for image smoothing.
+        :return: True if sigma was changed, False otherwise.
         """
-        theweight: float = 0.
+        thesigma: float = 0.
         ok_flag: bool = True
 
-        if weight is None or not weight:
+        if sigma is None or not sigma:
             # Read user input for margin size.
-            theweight, ok_flag = QtWidgets.QInputDialog.getDouble(None, 'Set heuristic weight: ',
-                                                                  'Enter new weight: ',
-                                                                  self.pjs.livewire_heuristic_weight, 0)
+            thesigma, ok_flag = QtWidgets.QInputDialog.getDouble(None, 'Set Gaussian sigma for LiveWire segmentation: ',
+                                                                  'Enter new sigma: ',
+                                                                 self.pjs.livewire_gaussian_sigma, 0)
         else:
-            theweight = weight
+            thesigma = sigma
             ok_flag = True
 
-        if ok_flag and (theweight >= 0.):
-            self.pjs.livewire_heuristic_weight = theweight
+        if ok_flag and (thesigma >= 0.):
+            self.pjs.livewire_gaussian_sigma = thesigma
             return True
         else:
             return False
```

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rcallbacks/rcbplugins.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rcallbacks/rcbplugins.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/csgraph.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/csgraph.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimcore.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimcore.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     image_extensions: Tuple[str] = ('.tif', '.tiff', '.jpg', '.jpeg', '.gif', '.png', '.bmp')
 
     def __init__(self, image_in):
         self.image_array: numpy.array = image_in
 
     # Return a tuple with all the points between thesrc and thedst. thesrc and thedst are in (r, c) format
-    def livewire(self, thesrc, thedst, margin, xy=False, heuristic_weight=0.0):
+    def livewire(self, thesrc, thedst, margin, xy=False, smooth_factor=0.0):
         # Copy parameters. This is critical. I had a headache, because the function was modifying the parameter values.
         src = thesrc.copy()
         dst = thedst.copy()
 
         # Crop image. Note that image_array.shape returns size in (rows, columns) format. But src and dst are in (col=x, row=y) format.
         minr = max(0, min(src[0], dst[0]) - margin)
         maxr = min(self.image_array.shape[0] - 1, max(src[0], dst[0]) + margin) + 1
@@ -74,16 +74,18 @@
         # Make sure the cropped image is a matrix and invert it so that high intensities become low ones, and we can
         # search for the minimal cost path.
         im[:] = numpy.max(im) - im[:]  # This modifies the array in place, which avoids having to reallocate the memory
         # (which is slow).
         # Doing im = numpy.max(im) - im produces the same result, but reallocates the memory.
 
         # Create graph.
-        G = rimutils.rimutils.makeGraphX(im)
-        path = rimutils.rimutils.path_astar(G, tuple(src), tuple(dst), heuristic_weight)
+        G = rimutils.rimutils.makeGraphX(rimutils.rimutils.gaussian_smoothing(im, smooth_factor))
+
+        # Find shortest path.
+        path = rimutils.rimutils.path_astar(G, tuple(src), tuple(dst))
 
         # Generate coordinates.
         if xy:
             return [[c + minc, r + minr] for (r, c) in path]
         else:
             return [[r + minr, c + minc] for (r, c) in path]
```

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/batchclassifier.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/batchclassifier.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/batchml.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/batchml.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/batchneuralnet.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/batchneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/batchrecurrentneuralnet.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/batchrecurrentneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/featurecalculator.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/featurecalculator.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/featurecalculator_rawimage.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/featurecalculator_rawimage.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/featurecalculator_rowofpixels.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/featurecalculator_sog.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/featurecalculator_sog.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimclassifier.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimclassifier.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimlr.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimlr.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimml.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimml.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimneuralnet.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimrecurrentneuralnet.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimrecurrentneuralnet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimrescunet.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimrescunet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimsvm.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimsvm.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimml/rimunet.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimml/rimunet.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rimage/rimutils.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rimage/rimutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,19 +417,18 @@
 
         return G
 
     @classmethod
     def astar_heuristic_euclidean(cls, a, b):
         (x1, y1) = a
         (x2, y2) = b
-        return cls.HEURISTIC_WEIGHT * ((x1 - x2) ** 2 + (y1 - y2) ** 2) ** 0.5
+        return ((x1 - x2) ** 2 + (y1 - y2) ** 2) ** 0.5
 
     @classmethod
-    def path_astar(cls, agraph, src, dst, heuristic_weight=0.0):
-        cls.HEURISTIC_WEIGHT = heuristic_weight
+    def path_astar(cls, agraph, src, dst):
         return astar_path(agraph, tuple(src), tuple(dst), heuristic=cls.astar_heuristic_euclidean)
 
     # 4 neighbours (removing pixels outside the image).
     @classmethod
     def _N4_(cls, row, col, imsize=(numpy.inf, numpy.inf)):
         # asarray vs array: The main difference is that array (by default) will make a copy of the object, while asarray will not unless necessary.
         initial = numpy.array([[row - 1, col], [row + 1, col], [row, col - 1], [row, col + 1]], dtype=numpy.int16)
@@ -1095,15 +1094,15 @@
         seed_image = dilation(seed_image, disk(3))
 
         # Run watershed.
         # image_color = cv2.cvtColor(rimutils.stretch(image).astype(numpy.uint8), cv2.COLOR_GRAY2BGR)
         # seed_image = seed_image.astype(numpy.int32)
         # labels = cv2.watershed(image_color, seed_image)
 
-        labels = watershed(image, seed_image, connectivity=2)  # , mask=image)
+        labels = watershed(image, seed_image.astype(int), connectivity=2)  # , mask=image)  # seed image must be int type.
 
         # Extract contours.
         return cls.extract_contours(labels, border_objects)
 
     @classmethod
     def extract_contours(cls, labeled_image: Optional[numpy.ndarray] = None, border_objects: bool = False) -> list:
         """
```

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rplugins/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rplugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rplugins/base.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rplugins/base.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/rutils.py` & `pyjamas-rfglab-2023.8.0/pyjamas/rutils.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/tests/__init__.py` & `pyjamas-rfglab-2023.8.0/pyjamas/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/tests/conftest.py` & `pyjamas-rfglab-2023.8.0/pyjamas/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/tests/unit/pjsfixtures.py` & `pyjamas-rfglab-2023.8.0/pyjamas/tests/unit/pjsfixtures.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/tests/unit/test_image.py` & `pyjamas-rfglab-2023.8.0/pyjamas/tests/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas/tests/unit/test_io.py` & `pyjamas-rfglab-2023.8.0/pyjamas/tests/unit/test_io.py`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/pyjamas_rfglab.egg-info/SOURCES.txt` & `pyjamas-rfglab-2023.8.0/pyjamas_rfglab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjamas-rfglab-2023.7.9/setup.py` & `pyjamas-rfglab-2023.8.0/setup.py`

 * *Files identical despite different names*

