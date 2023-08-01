# Comparing `tmp/decOM-0.0.8.tar.gz` & `tmp/decOM-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decOM-0.0.8.tar", last modified: Tue Mar 22 14:11:57 2022, max compression
+gzip compressed data, was "decOM-0.0.9.tar", last modified: Tue Mar 22 15:19:22 2022, max compression
```

## Comparing `decOM-0.0.8.tar` & `decOM-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 14:11:57.821756 decOM-0.0.8/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2022-03-03 17:15:32.000000 decOM-0.0.8/LICENSE
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      702 2022-03-22 14:11:57.821105 decOM-0.0.8/PKG-INFO
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       88 2022-03-15 10:52:41.000000 decOM-0.0.8/README.md
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      104 2022-03-03 17:22:44.000000 decOM-0.0.8/pyproject.toml
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       38 2022-03-22 14:11:57.822106 decOM-0.0.8/setup.cfg
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1198 2022-03-22 14:11:38.000000 decOM-0.0.8/setup.py
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 14:11:57.790460 decOM-0.0.8/src/
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 14:11:57.802281 decOM-0.0.8/src/decOM/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2022-03-03 17:12:08.000000 decOM-0.0.8/src/decOM/__init__.py
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     5180 2022-03-21 14:18:42.000000 decOM-0.0.8/src/decOM/__main__.py
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 14:11:57.818704 decOM-0.0.8/src/decOM/data/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2022-03-15 16:33:12.000000 decOM-0.0.8/src/decOM/data/__init__.py
--rw-r--r--   0 cduitama (36963) seqbio   (97979)    63288 2022-03-15 14:12:45.000000 decOM-0.0.8/src/decOM/data/kmtricks.fof
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   122885 2022-03-15 14:11:55.000000 decOM-0.0.8/src/decOM/data/metadata.csv
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 14:11:57.814381 decOM-0.0.8/src/decOM.egg-info/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      702 2022-03-22 14:11:57.000000 decOM-0.0.8/src/decOM.egg-info/PKG-INFO
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      368 2022-03-22 14:11:57.000000 decOM-0.0.8/src/decOM.egg-info/SOURCES.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        1 2022-03-22 14:11:57.000000 decOM-0.0.8/src/decOM.egg-info/dependency_links.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       46 2022-03-22 14:11:57.000000 decOM-0.0.8/src/decOM.egg-info/entry_points.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       72 2022-03-22 14:11:57.000000 decOM-0.0.8/src/decOM.egg-info/requires.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        6 2022-03-22 14:11:57.000000 decOM-0.0.8/src/decOM.egg-info/top_level.txt
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 15:19:22.099751 decOM-0.0.9/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2022-03-03 17:15:32.000000 decOM-0.0.9/LICENSE
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      702 2022-03-22 15:19:22.097850 decOM-0.0.9/PKG-INFO
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       88 2022-03-15 10:52:41.000000 decOM-0.0.9/README.md
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      104 2022-03-03 17:22:44.000000 decOM-0.0.9/pyproject.toml
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       38 2022-03-22 15:19:22.098678 decOM-0.0.9/setup.cfg
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1198 2022-03-22 15:09:15.000000 decOM-0.0.9/setup.py
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 15:19:22.064895 decOM-0.0.9/src/
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 15:19:22.077977 decOM-0.0.9/src/decOM/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2022-03-03 17:12:08.000000 decOM-0.0.9/src/decOM/__init__.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     5205 2022-03-22 15:14:39.000000 decOM-0.0.9/src/decOM/__main__.py
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 15:19:22.097638 decOM-0.0.9/src/decOM/data/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2022-03-15 16:33:12.000000 decOM-0.0.9/src/decOM/data/__init__.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)    63288 2022-03-15 14:12:45.000000 decOM-0.0.9/src/decOM/data/kmtricks.fof
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   122885 2022-03-15 14:11:55.000000 decOM-0.0.9/src/decOM/data/metadata.csv
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2022-03-22 15:19:22.090214 decOM-0.0.9/src/decOM.egg-info/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      702 2022-03-22 15:19:21.000000 decOM-0.0.9/src/decOM.egg-info/PKG-INFO
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      368 2022-03-22 15:19:22.000000 decOM-0.0.9/src/decOM.egg-info/SOURCES.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        1 2022-03-22 15:19:21.000000 decOM-0.0.9/src/decOM.egg-info/dependency_links.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       46 2022-03-22 15:19:21.000000 decOM-0.0.9/src/decOM.egg-info/entry_points.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       72 2022-03-22 15:19:21.000000 decOM-0.0.9/src/decOM.egg-info/requires.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        6 2022-03-22 15:19:22.000000 decOM-0.0.9/src/decOM.egg-info/top_level.txt
```

### Comparing `decOM-0.0.8/PKG-INFO` & `decOM-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decOM
-Version: 0.0.8
+Version: 0.0.9
 Summary: decOM: K-mer method for aOral metagenome decontamination
 Home-page: https://github.com/CamilaDuitama/decOM
 Author: Camila Duitama González
 Author-email: cduitama@pasteur.fr
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/CamilaDuitama/decOM/issues
 Platform: UNKNOWN
```

### Comparing `decOM-0.0.8/setup.py` & `decOM-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="decOM",
-    version="0.0.8",
+    version="0.0.9",
     author="Camila Duitama González",
     author_email="cduitama@pasteur.fr",
     description="decOM: K-mer method for aOral metagenome decontamination",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CamilaDuitama/decOM",
     project_urls={
```

### Comparing `decOM-0.0.8/src/decOM/__main__.py` & `decOM-0.0.9/src/decOM/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,22 @@
     parser.add_argument("-p_sink","--path_sink",help="Path to sink vector, the output of kmtricks filter Ex: ./kmtricks_output/matrices/100.vec",required=True)
     parser.add_argument("-p_missing", "--path_missing_kmers",help="Path to missing kmers, the output of kmtricks filter after using kmtricks aggregate Ex: ./kmtricks_output/count/{sink}_missing.txt",required=True)
     parser.add_argument("-mem","--memory",help="Write down how much memory you want to use. Ex: 500GiB",required=True)
     parser.add_argument("-t","--threads",help="Number of threads to use. Ex: 10",required=True)
     parser.add_argument("-plt","--plot",help="True if you want a plot with the source proportions of the sink, else False",required=False,default=True)
     args = parser.parse_args()
     
-    start=time.time()
-    
-    sink=args.s
-    p_sources=args.p_sources
-    path_sink=args.p_sink
-    path_missing_kmers=args.p_missing
-    mem=args.mem
-    t=args.t
-    plot=args.plt
+    start=time.time() 
+    sink=args.sink
+    p_sources=args.path_sources
+    path_sink=args.path_sink
+    path_missing_kmers=args.path_missing_kmers
+    mem=args.memory
+    t=args.threads
+    plot=args.plot
     
     cluster = LocalCluster(memory_limit=mem,n_workers=int(t))
     client = Client(cluster)
     client = Client()
     print("Client was set:")
     print(client)
 
@@ -129,8 +128,8 @@
         fig = px.bar(result, y=["p_aOral", "p_mOral","p_Sediment/Soil","p_Skin","p_Unknown"], color_discrete_sequence=px.colors.qualitative.G10, opacity=0.8, title="Proportions sink "+ sink)
         fig.update_layout(width=400,height=800)
         fig.write_image("result_plot.png",width=400,height=800,scale=5)
     
     client.close()
 
 if __name__ == "__main__":
-    sys.exit(main())
+    sys.exit(main())
```

### Comparing `decOM-0.0.8/src/decOM/data/kmtricks.fof` & `decOM-0.0.9/src/decOM/data/kmtricks.fof`

 * *Files identical despite different names*

### Comparing `decOM-0.0.8/src/decOM/data/metadata.csv` & `decOM-0.0.9/src/decOM/data/metadata.csv`

 * *Files identical despite different names*

### Comparing `decOM-0.0.8/src/decOM.egg-info/PKG-INFO` & `decOM-0.0.9/src/decOM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decOM
-Version: 0.0.8
+Version: 0.0.9
 Summary: decOM: K-mer method for aOral metagenome decontamination
 Home-page: https://github.com/CamilaDuitama/decOM
 Author: Camila Duitama González
 Author-email: cduitama@pasteur.fr
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/CamilaDuitama/decOM/issues
 Platform: UNKNOWN
```

