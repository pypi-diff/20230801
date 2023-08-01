# Comparing `tmp/get-some-ncbi-genomes-0.1.tar.gz` & `tmp/get-some-ncbi-genomes-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-some-ncbi-genomes-0.1.tar", last modified: Sun Jul 30 10:10:42 2023, max compression
+gzip compressed data, was "get-some-ncbi-genomes-0.2.tar", last modified: Tue Aug  1 14:32:46 2023, max compression
```

## Comparing `get-some-ncbi-genomes-0.1.tar` & `get-some-ncbi-genomes-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:10:42.297807 get-some-ncbi-genomes-0.1/
--rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-29 20:20:27.000000 get-some-ncbi-genomes-0.1/LICENSE
--rw-r--r--   0 t          (502) staff       (20)      635 2023-07-30 10:10:42.297652 get-some-ncbi-genomes-0.1/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      430 2023-07-30 00:41:09.000000 get-some-ncbi-genomes-0.1/README.md
--rw-r--r--   0 t          (502) staff       (20)      456 2023-07-29 20:28:32.000000 get-some-ncbi-genomes-0.1/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-07-30 10:10:42.297852 get-some-ncbi-genomes-0.1/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:10:42.289869 get-some-ncbi-genomes-0.1/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:10:42.297215 get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.egg-info/
--rw-r--r--   0 t          (502) staff       (20)      635 2023-07-30 10:10:42.000000 get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      387 2023-07-30 10:10:42.000000 get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-07-30 10:10:42.000000 get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)      149 2023-07-30 10:10:42.000000 get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       31 2023-07-30 10:10:42.000000 get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       22 2023-07-30 10:10:42.000000 get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     9296 2023-07-29 21:09:53.000000 get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:10:42.297347 get-some-ncbi-genomes-0.1/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2023-07-29 20:20:27.000000 get-some-ncbi-genomes-0.1/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:32:46.554401 get-some-ncbi-genomes-0.2/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-29 20:20:27.000000 get-some-ncbi-genomes-0.2/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     1185 2023-08-01 14:32:46.554268 get-some-ncbi-genomes-0.2/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      980 2023-08-01 14:31:06.000000 get-some-ncbi-genomes-0.2/README.md
+-rw-r--r--   0 t          (502) staff       (20)      458 2023-08-01 14:31:26.000000 get-some-ncbi-genomes-0.2/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-08-01 14:32:46.554518 get-some-ncbi-genomes-0.2/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:32:46.552063 get-some-ncbi-genomes-0.2/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:32:46.553462 get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     1185 2023-08-01 14:32:46.000000 get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      393 2023-08-01 14:32:46.000000 get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-01 14:32:46.000000 get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      151 2023-08-01 14:32:46.000000 get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       31 2023-08-01 14:32:46.000000 get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       22 2023-08-01 14:32:46.000000 get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)     9620 2023-08-01 14:31:06.000000 get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:32:46.553659 get-some-ncbi-genomes-0.2/tests/
+-rw-r--r--   0 t          (502) staff       (20)      864 2023-08-01 14:31:06.000000 get-some-ncbi-genomes-0.2/tests/test_get_some_ncbi_genomes.py
```

### Comparing `get-some-ncbi-genomes-0.1/LICENSE` & `get-some-ncbi-genomes-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `get-some-ncbi-genomes-0.1/src/get_some_ncbi_genomes.py` & `get-some-ncbi-genomes-0.2/src/get_some_ncbi_genomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-# @CTB document me!
+"""\
+download one or more NCBI genomes + associated taxonomic info
+"""
+
+usage="""
+sourmash scripts get-genomes <accession>
+"""
+
+epilog="""
+See https://github.com/ctb/get-some-ncbi-genomes for more examples.
+
+Need help? Have questions? Ask at http://github.com/sourmash/issues!
+"""
+
 import sys
 import os
 import argparse
 import urllib.request
 from urllib.parse import urlparse
 import csv
 
@@ -239,15 +252,18 @@
 
 #
 # CLI plugin for sourmash - supports 'sourmash scripts get-genomes'
 #
 
 class Command_DownloadNCBI(CommandLinePlugin):
     command = 'get-genomes'
-    description = "retrieve one or more NCBI genomes"
+    description = __doc__
+    usage = usage
+    epilog = epilog
+    formatter_class = argparse.RawTextHelpFormatter
 
     def __init__(self, subparser):
         super().__init__(subparser)
         # add argparse arguments here.
         subparser.add_argument('accessions', nargs='+')
         subparser.add_argument('--output-directory', default=None,
                                help="directory to save genomes")
```

