# Comparing `tmp/cybrex-1.1.6.tar.gz` & `tmp/cybrex-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.1.6.tar", last modified: Tue Aug  1 20:22:47 2023, max compression
+gzip compressed data, was "cybrex-1.1.7.tar", last modified: Tue Aug  1 20:46:17 2023, max compression
```

## Comparing `cybrex-1.1.6.tar` & `cybrex-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:22:47.797803 cybrex-1.1.6/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.6/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:22:47.797490 cybrex-1.1.6/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.6/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:22:47.794920 cybrex-1.1.6/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.6/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 19:57:30.000000 cybrex-1.1.6/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11529 2023-08-01 20:11:23.000000 cybrex-1.1.6/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.6/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:22:47.796954 cybrex-1.1.6/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:22:47.000000 cybrex-1.1.6/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-01 20:22:47.000000 cybrex-1.1.6/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 20:22:47.000000 cybrex-1.1.6/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 20:22:47.000000 cybrex-1.1.6/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:22:47.000000 cybrex-1.1.6/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 20:22:47.000000 cybrex-1.1.6/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 20:22:37.000000 cybrex-1.1.6/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:22:19.000000 cybrex-1.1.6/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 20:22:47.797905 cybrex-1.1.6/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:46:17.889213 cybrex-1.1.7/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.7/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:46:17.888766 cybrex-1.1.7/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.7/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:46:17.884742 cybrex-1.1.7/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.7/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5636 2023-08-01 20:40:01.000000 cybrex-1.1.7/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    11974 2023-08-01 20:45:51.000000 cybrex-1.1.7/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.7/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 20:46:17.887691 cybrex-1.1.7/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 20:46:17.000000 cybrex-1.1.7/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 20:45:51.000000 cybrex-1.1.7/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:22:19.000000 cybrex-1.1.7/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 20:46:17.889380 cybrex-1.1.7/setup.cfg
```

### Comparing `cybrex-1.1.6/PKG-INFO` & `cybrex-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.6
+Version: 1.1.7
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.6/README.md` & `cybrex-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.6/cybrex/cli.py` & `cybrex-1.1.7/cybrex/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import sys
 import textwrap
 
 import fire
 from termcolor import colored
 
-from .cybrex_ai import CybrexAI
+from cybrex_ai import CybrexAI
 
 
 def create_snippet(document):
     return document['metadata']['doi'] + ': ' + document['text']
 
 
 class CybrexCli:
```

### Comparing `cybrex-1.1.6/cybrex/cybrex_ai.py` & `cybrex-1.1.7/cybrex/cybrex_ai.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from izihawa_utils.exceptions import BaseError
 from izihawa_utils.file import mkdir_p
 from langchain.chains.summarize import load_summarize_chain
 from langchain.schema import Document
 from stc_geck.advices import get_documents_on_topic
 from stc_geck.client import StcGeck
 
-from .models import CybrexModel
+from models import CybrexModel
 
 
 class DocumentNotFoundError(BaseError):
     pass
 
 
 def print_color(text, color):
@@ -220,43 +220,55 @@
                 metadatas.append(processed_document['metadata'])
                 texts.append(processed_document['text'])
                 embedding = base64.b64decode(processed_document['embedding'])
                 embedding = [n.item() for n in np.frombuffer(embedding, dtype=np.float64)]
                 embeddings.append(embedding)
 
         if texts:
-            self.collection.upsert(
-                documents=texts,
-                metadatas=metadatas,
-                embeddings=embeddings,
-                ids=[str(uuid.uuid1()) for _ in range(len(texts))]
+            await asyncio.get_running_loop().run_in_executor(
+                None,
+                lambda: self.collection.upsert(
+                    documents=texts,
+                    metadatas=metadatas,
+                    embeddings=embeddings,
+                    ids=[str(uuid.uuid1()) for _ in range(len(texts))]
+                )
             )
 
     async def chat_document(self, field, value, query, n_results: int):
         await self.add_full_document_by_field_value(field, value)
 
         documents = await self._query(query, n_results, where={field: value})
-        result = self.model.llm.query_documents(query, documents)
+        result = await asyncio.get_running_loop().run_in_executor(
+            None,
+            lambda: self.model.llm.query_documents(query, documents),
+        )
 
         return result
 
     async def chat_science(self, query: str, n_results: int, n_summa_documents: int):
         full_documents = await self.keywords_search(query, n_summa_documents)
         await self.add_full_documents(full_documents)
 
         documents = await self._query(query, n_results)
-        result = self.model.llm.query_documents(query, documents)
+        result = await asyncio.get_running_loop().run_in_executor(
+            None,
+            lambda: self.model.llm.query_documents(query, documents),
+        )
         return result, await self.get_summa_documents_from_documents(documents)
 
     async def _query(self, query: str, n_results: int = 3, where: Optional[dict] = None):
-        response = self.collection.query(
-            query_embeddings=[self.model.embedder.embed_query(query)],
-            n_results=n_results,
-            include=['documents', 'metadatas', 'distances'],
-            where=where,
+        response = await asyncio.get_running_loop().run_in_executor(
+            None,
+            lambda: self.collection.query(
+                query_embeddings=[self.model.embedder.embed_query(query)],
+                n_results=n_results,
+                include=['documents', 'metadatas', 'distances'],
+                where=where,
+            )
         )
         documents = []
         for (text, metadata, distance) in zip(response['documents'][0], response['metadatas'][0], response['distances'][0]):
             documents.append({'text': text, 'metadata': metadata, 'distance': distance})
         return documents
 
     async def keywords_search(self, query: str, n_summa_documents: int):
```

### Comparing `cybrex-1.1.6/cybrex/models.py` & `cybrex-1.1.7/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.6/cybrex.egg-info/PKG-INFO` & `cybrex-1.1.7/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.6
+Version: 1.1.7
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.6/pyproject.toml` & `cybrex-1.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.1.6"
+version = "1.1.7"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

