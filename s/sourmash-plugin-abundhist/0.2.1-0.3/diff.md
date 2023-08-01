# Comparing `tmp/sourmash_plugin_abundhist-0.2.1.tar.gz` & `tmp/sourmash_plugin_abundhist-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_abundhist-0.2.1.tar", last modified: Mon Jul 31 13:39:22 2023, max compression
+gzip compressed data, was "sourmash_plugin_abundhist-0.3.tar", last modified: Tue Aug  1 14:29:15 2023, max compression
```

## Comparing `sourmash_plugin_abundhist-0.2.1.tar` & `sourmash_plugin_abundhist-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:39:22.017693 sourmash_plugin_abundhist-0.2.1/
--rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-30 11:13:48.000000 sourmash_plugin_abundhist-0.2.1/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     1665 2023-07-31 13:39:22.017538 sourmash_plugin_abundhist-0.2.1/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     1452 2023-07-31 13:38:21.000000 sourmash_plugin_abundhist-0.2.1/README.md
--rw-r--r--   0 t          (502) staff       (20)      417 2023-07-31 13:38:21.000000 sourmash_plugin_abundhist-0.2.1/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-07-31 13:39:22.017736 sourmash_plugin_abundhist-0.2.1/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:39:22.016118 sourmash_plugin_abundhist-0.2.1/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:39:22.017067 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     1665 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      415 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)       86 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       45 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       26 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     5405 2023-07-31 13:38:21.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:39:22.017200 sourmash_plugin_abundhist-0.2.1/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2023-07-30 11:13:48.000000 sourmash_plugin_abundhist-0.2.1/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:29:15.082900 sourmash_plugin_abundhist-0.3/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-30 11:13:48.000000 sourmash_plugin_abundhist-0.3/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     1709 2023-08-01 14:29:15.082757 sourmash_plugin_abundhist-0.3/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     1498 2023-08-01 14:27:48.000000 sourmash_plugin_abundhist-0.3/README.md
+-rw-r--r--   0 t          (502) staff       (20)      415 2023-08-01 14:27:59.000000 sourmash_plugin_abundhist-0.3/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-08-01 14:29:15.082936 sourmash_plugin_abundhist-0.3/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:29:15.081373 sourmash_plugin_abundhist-0.3/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:29:15.082255 sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     1709 2023-08-01 14:29:15.000000 sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      418 2023-08-01 14:29:15.000000 sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-08-01 14:29:15.000000 sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)       86 2023-08-01 14:29:15.000000 sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       45 2023-08-01 14:29:15.000000 sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       26 2023-08-01 14:29:15.000000 sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)     5401 2023-08-01 14:27:48.000000 sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-08-01 14:29:15.082381 sourmash_plugin_abundhist-0.3/tests/
+-rw-r--r--   0 t          (502) staff       (20)     1821 2023-08-01 14:27:48.000000 sourmash_plugin_abundhist-0.3/tests/test_sourmash_abundhist.py
```

### Comparing `sourmash_plugin_abundhist-0.2.1/LICENSE` & `sourmash_plugin_abundhist-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_abundhist-0.2.1/PKG-INFO` & `sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sourmash_plugin_abundhist
-Version: 0.2.1
+Name: sourmash-plugin-abundhist
+Version: 0.3
 Summary: sourmash plugin to calculate abundance profiles.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_abundhist
 
@@ -17,15 +17,15 @@
 ## Usage
 
 ### Example
 
 
 #### Basic command-line usage:
 ```
-% sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip
+% sourmash scripts abundhist examples/SRR606249-abund-100k.sig.zip
 
 == This is sourmash version 4.8.3.dev0. ==
 == Please cite Brown and Irber (2016), doi:10.21105/joss.00027. ==
 
 loaded 1 total that matched ksize & molecule type
 
 36   [3487]  ****************************************
@@ -39,38 +39,45 @@
 320  [   2]
 356  [   2]
 ```
 
 #### Create a nice histogram figure for an isolate reads data set
 
 ```
-sourmash scripts abundhist --max 100 --min 1 --bins 100 example/reads.sig.gz --figure example/ecoli-reads.png --ymax=200
+sourmash scripts abundhist --max 100 --min 1 --bins 100 examples/reads.sig.gz --figure examples/ecoli-reads.png --ymax=200
 ```
 
 will create:
 
-![histogram](example/ecoli-reads.png)
+![histogram](examples/ecoli-reads.png)
 
 #### Create a nice histogram figure for a metagenome:
 
 ```
-% sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip --figure hist.png
+% sourmash scripts abundhist examples/SRR606249-abund-100k.sig.zip --figure hist.png
 ```
 will create this figure:
 
-![histogram](example/hist.png)
+![histogram](examples/hist.png)
 
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
 
 `abundhist` is developed at https://github.com/ctb/sourmash_plugin_abundhist.
 
+### Testing
+
+Run:
+```
+pytest tests
+```
+
 ### Generating a release
 
 Bump version number in `pyproject.toml` and push.
 
 Make a new release on github.
 
 Then pull, and:
```

### Comparing `sourmash_plugin_abundhist-0.2.1/README.md` & `sourmash_plugin_abundhist-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ## Usage
 
 ### Example
 
 
 #### Basic command-line usage:
 ```
-% sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip
+% sourmash scripts abundhist examples/SRR606249-abund-100k.sig.zip
 
 == This is sourmash version 4.8.3.dev0. ==
 == Please cite Brown and Irber (2016), doi:10.21105/joss.00027. ==
 
 loaded 1 total that matched ksize & molecule type
 
 36   [3487]  ****************************************
@@ -31,38 +31,45 @@
 320  [   2]
 356  [   2]
 ```
 
 #### Create a nice histogram figure for an isolate reads data set
 
 ```
-sourmash scripts abundhist --max 100 --min 1 --bins 100 example/reads.sig.gz --figure example/ecoli-reads.png --ymax=200
+sourmash scripts abundhist --max 100 --min 1 --bins 100 examples/reads.sig.gz --figure examples/ecoli-reads.png --ymax=200
 ```
 
 will create:
 
-![histogram](example/ecoli-reads.png)
+![histogram](examples/ecoli-reads.png)
 
 #### Create a nice histogram figure for a metagenome:
 
 ```
-% sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip --figure hist.png
+% sourmash scripts abundhist examples/SRR606249-abund-100k.sig.zip --figure hist.png
 ```
 will create this figure:
 
-![histogram](example/hist.png)
+![histogram](examples/hist.png)
 
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
 
 `abundhist` is developed at https://github.com/ctb/sourmash_plugin_abundhist.
 
+### Testing
+
+Run:
+```
+pytest tests
+```
+
 ### Generating a release
 
 Bump version number in `pyproject.toml` and push.
 
 Make a new release on github.
 
 Then pull, and:
```

### Comparing `sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/PKG-INFO` & `sourmash_plugin_abundhist-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sourmash-plugin-abundhist
-Version: 0.2.1
+Name: sourmash_plugin_abundhist
+Version: 0.3
 Summary: sourmash plugin to calculate abundance profiles.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_abundhist
 
@@ -17,15 +17,15 @@
 ## Usage
 
 ### Example
 
 
 #### Basic command-line usage:
 ```
-% sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip
+% sourmash scripts abundhist examples/SRR606249-abund-100k.sig.zip
 
 == This is sourmash version 4.8.3.dev0. ==
 == Please cite Brown and Irber (2016), doi:10.21105/joss.00027. ==
 
 loaded 1 total that matched ksize & molecule type
 
 36   [3487]  ****************************************
@@ -39,38 +39,45 @@
 320  [   2]
 356  [   2]
 ```
 
 #### Create a nice histogram figure for an isolate reads data set
 
 ```
-sourmash scripts abundhist --max 100 --min 1 --bins 100 example/reads.sig.gz --figure example/ecoli-reads.png --ymax=200
+sourmash scripts abundhist --max 100 --min 1 --bins 100 examples/reads.sig.gz --figure examples/ecoli-reads.png --ymax=200
 ```
 
 will create:
 
-![histogram](example/ecoli-reads.png)
+![histogram](examples/ecoli-reads.png)
 
 #### Create a nice histogram figure for a metagenome:
 
 ```
-% sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip --figure hist.png
+% sourmash scripts abundhist examples/SRR606249-abund-100k.sig.zip --figure hist.png
 ```
 will create this figure:
 
-![histogram](example/hist.png)
+![histogram](examples/hist.png)
 
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
 
 `abundhist` is developed at https://github.com/ctb/sourmash_plugin_abundhist.
 
+### Testing
+
+Run:
+```
+pytest tests
+```
+
 ### Generating a release
 
 Bump version number in `pyproject.toml` and push.
 
 Make a new release on github.
 
 Then pull, and:
```

### Comparing `sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.py` & `sourmash_plugin_abundhist-0.3/src/sourmash_plugin_abundhist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""calculate abundance profiles from one or more abund sketches
+"""\
+calculate abundance profiles from one or more abund sketches
 
 Display histograms of k-mer/hash multiplicity in sourmash sketches created
 with `-p abund`.
 
 'abundhist' provides text output, as well as CSV output.
 """
 
@@ -45,15 +46,15 @@
 
     def __init__(self, subparser):
         super().__init__(subparser)
         # add argparse arguments here.
         subparser.add_argument('signature_file', nargs='+')
 
         subparser.add_argument(
-            '-o', '--csv', metavar='FILE',
+            '--csv', metavar='FILE',
             help='output histogram to this file (in CSV format)'
         )
         subparser.add_argument('--figure', help='save figure to this file')
         subparser.add_argument(
             '--abundances-csv', metavar='FILE',
             help='output hashes and abundances to this file (in CSV format)')
         subparser.add_argument(
```

