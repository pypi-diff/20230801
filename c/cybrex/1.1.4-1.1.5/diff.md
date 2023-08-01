# Comparing `tmp/cybrex-1.1.4.tar.gz` & `tmp/cybrex-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.1.4.tar", last modified: Tue Aug  1 20:04:35 2023, max compression
+gzip compressed data, was "cybrex-1.1.5.tar", last modified: Tue Aug  1 20:13:20 2023, max compression
```

## Comparing `cybrex-1.1.4.tar` & `cybrex-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:04:35.153126 cybrex-1.1.4/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.4/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:04:35.152810 cybrex-1.1.4/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.4/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:04:35.150243 cybrex-1.1.4/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.4/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 19:57:30.000000 cybrex-1.1.4/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11678 2023-08-01 19:57:40.000000 cybrex-1.1.4/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.4/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:04:35.152232 cybrex-1.1.4/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      219 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 20:04:35.000000 cybrex-1.1.4/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 20:04:17.000000 cybrex-1.1.4/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      219 2023-08-01 20:03:15.000000 cybrex-1.1.4/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 20:04:35.153227 cybrex-1.1.4/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:13:20.164502 cybrex-1.1.5/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.5/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:13:20.164131 cybrex-1.1.5/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.5/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:13:20.161773 cybrex-1.1.5/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.5/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 19:57:30.000000 cybrex-1.1.5/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    11529 2023-08-01 20:11:23.000000 cybrex-1.1.5/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.5/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:13:20.163608 cybrex-1.1.5/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:13:20.000000 cybrex-1.1.5/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-01 20:13:20.000000 cybrex-1.1.5/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 20:13:20.000000 cybrex-1.1.5/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 20:13:20.000000 cybrex-1.1.5/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      218 2023-08-01 20:13:20.000000 cybrex-1.1.5/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 20:13:20.000000 cybrex-1.1.5/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 20:13:05.000000 cybrex-1.1.5/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      218 2023-08-01 20:13:01.000000 cybrex-1.1.5/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 20:13:20.164620 cybrex-1.1.5/setup.cfg
```

### Comparing `cybrex-1.1.4/PKG-INFO` & `cybrex-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.4
+Version: 1.1.5
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.4/README.md` & `cybrex-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.4/cybrex/cli.py` & `cybrex-1.1.5/cybrex/cli.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.4/cybrex/cybrex_ai.py` & `cybrex-1.1.5/cybrex/cybrex_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,15 @@
 
         config = Configurator(configs=[
             config_path,
         ])
 
         self.model = CybrexModel(config['model'])
 
-        self.client_settings = chromadb.config.Settings(
-            chroma_db_impl="duckdb+parquet",
-            persist_directory=os.path.join(self.home_path, 'chroma'),
-        )
-        self.db = chromadb.Client(self.client_settings)
+        self.db = chromadb.PersistentClient(path=os.path.join(self.home_path, 'chroma'))
         self.collection_name = self.model.get_embeddings_id()
 
         self.collection = self.db.get_or_create_collection(
             name=self.collection_name,
             embedding_function=self.model.embedder.embed_documents,
         )
         self.geck = geck
```

### Comparing `cybrex-1.1.4/cybrex/models.py` & `cybrex-1.1.5/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.4/cybrex.egg-info/PKG-INFO` & `cybrex-1.1.5/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.4
+Version: 1.1.5
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.4/pyproject.toml` & `cybrex-1.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.1.4"
+version = "1.1.5"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

