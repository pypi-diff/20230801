# Comparing `tmp/cybrex-1.1.1.tar.gz` & `tmp/cybrex-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.1.1.tar", last modified: Mon Jul 31 15:35:14 2023, max compression
+gzip compressed data, was "cybrex-1.1.2.tar", last modified: Tue Aug  1 19:52:16 2023, max compression
```

## Comparing `cybrex-1.1.1.tar` & `cybrex-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-31 15:35:14.015954 cybrex-1.1.1/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.1/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24132 2023-07-31 15:35:14.015514 cybrex-1.1.1/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23856 2023-07-23 19:18:23.000000 cybrex-1.1.1/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-31 15:35:14.012817 cybrex-1.1.1/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.1/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5659 2023-07-31 15:18:57.000000 cybrex-1.1.1/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11486 2023-07-31 15:34:26.000000 cybrex-1.1.1/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)     3213 2023-07-31 15:18:57.000000 cybrex-1.1.1/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-31 15:35:14.014842 cybrex-1.1.1/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24132 2023-07-31 15:35:13.000000 cybrex-1.1.1/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-07-31 15:35:14.000000 cybrex-1.1.1/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-31 15:35:14.000000 cybrex-1.1.1/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-31 15:35:14.000000 cybrex-1.1.1/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      182 2023-07-31 15:35:14.000000 cybrex-1.1.1/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-31 15:35:14.000000 cybrex-1.1.1/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-31 15:34:57.000000 cybrex-1.1.1/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      182 2023-07-30 14:20:06.000000 cybrex-1.1.1/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-31 15:35:14.016074 cybrex-1.1.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:52:16.888172 cybrex-1.1.2/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.2/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 19:52:16.887852 cybrex-1.1.2/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.2/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:52:16.885432 cybrex-1.1.2/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.2/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5636 2023-08-01 19:14:39.000000 cybrex-1.1.2/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    11690 2023-08-01 19:12:09.000000 cybrex-1.1.2/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13594 2023-08-01 18:15:58.000000 cybrex-1.1.2/cybrex/models.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13911 2023-08-01 13:45:04.000000 cybrex-1.1.2/cybrex/test.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 19:52:16.887380 cybrex-1.1.2/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      320 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      204 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 19:52:16.000000 cybrex-1.1.2/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 19:51:49.000000 cybrex-1.1.2/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      204 2023-08-01 19:51:35.000000 cybrex-1.1.2/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 19:52:16.888273 cybrex-1.1.2/setup.cfg
```

### Comparing `cybrex-1.1.1/PKG-INFO` & `cybrex-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.1
+Version: 1.1.2
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -69,15 +69,15 @@
 Zika virus (ZIKV). Resveratrol appears to block the activities of the TIR-domain-containing
 adapter-inducing interferon-β (TRIF) complex, suggesting that resveratrol would also inhibit NF-κB
 transcription induced by TRIF. Additionally, it has been reported to reduce the activity of respiratory
 syncytial virus (RSV) and to stimulate the secretion of higher levels of TNF-α, promoting cell death
 and RSV clearance.
 
 # Question enitre science
-cybrex - chat-sci --question "What is the antivirus effect of resveratrol?" --top-n 15 --summa-documents 40
+cybrex - chat-sci --question "What is the antivirus effect of resveratrol?" --n-results 15 --n-summa-documents 40
 
 Q: What is the antivirus effect of resveratrol?
 A: Resveratrol has been found to possess antiviral activity against a variety of viruses, including herpes simplex virus, human immunodeficiency virus, and hepatitis C virus. It has been shown to inhibit the replication of several viruses, including HIV, herpes simplex virus, and influenza virus, and to regulate TLR3 expression, thus affecting the recruitment of downstream related factors and finally affecting the regulation process of related signal pathways. It has also been studied for its antiviral activity against Reoviridae, and for its potential to inhibit Zika virus cytopathy effect. It has been active against Epstein virus, rotavirus, and vesicular stomatitis virus, and has been reported to alleviate virus-induced reproductive failure and to promote RSV clearance in the body more quickly.
 Sources:
  - 10.1155/2022/7138756: The Antiviral Activity of Resveratrol
  - 10.1155/2022/7138756: Antiviral Mechanisms of Resveratrol
  - 10.1155/2022/7138756: The antiviral effects of resveratrol are well demonstrated. Currently, studies on the antiviral mechanism of resveratrol mainly focus on two points.On the one hand, resveratrol possesses the ability to activate the host's immune defenses, turning on a complex network of bodies to fight or eliminate incoming viruses. NF-κB belongs to a family of inducible nuclear transcription factors, which regulates a wide array of genes involved in various processes of antiviral activity, inflammatory, and immune response . Meanwhile, it is noteworthy that Toll-like receptors (TLRs) are located upstream of the NF-κB signaling pathway and are responsible for induction of antiviral innate immune responses by recognizing virus infection, which leads to the production of proinflammatory cytokines, chemokines, and interferons . Thus, the TLRs/NF-κB pathway has been extensively studied during viral infection. Likewise, most research on antiviral drugs has focused on this pathway. Resveratrol regulated TLR3 expression, thus affecting the recruitment of downstream related factors and finally affecting the regulation process of related signal pathways. Moreover, resveratrol inhibits PRV by inhibiting the IκBα degradation induced by PRV infection, thereby inhibiting the activation of the NF-κB cell signaling pathway, and subsequently inhibiting the transcription of viral genes, protein and DNA synthesis, and virion production . Thus, the TLRs/NF-κB signaling pathway plays a crucial role in the antiviral process of resveratrol. On the other hand, resveratrol also has the ability to inhibit the production of virions by directly inhibiting the expression of key viral genes or by binding to key enzymes and proteins that disrupt the viral replication cycle. In this case, resveratrol could possess antiviral activities against ZIKV NS2B 18 NS3 and helicase 3 . Overall, the antiviral mechanisms of resveratrol are diverse. We have summarized many studies and found that most of them focus on the effects of resveratrol on host signal pathways and
```

### Comparing `cybrex-1.1.1/README.md` & `cybrex-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 Zika virus (ZIKV). Resveratrol appears to block the activities of the TIR-domain-containing
 adapter-inducing interferon-β (TRIF) complex, suggesting that resveratrol would also inhibit NF-κB
 transcription induced by TRIF. Additionally, it has been reported to reduce the activity of respiratory
 syncytial virus (RSV) and to stimulate the secretion of higher levels of TNF-α, promoting cell death
 and RSV clearance.
 
 # Question enitre science
-cybrex - chat-sci --question "What is the antivirus effect of resveratrol?" --top-n 15 --summa-documents 40
+cybrex - chat-sci --question "What is the antivirus effect of resveratrol?" --n-results 15 --n-summa-documents 40
 
 Q: What is the antivirus effect of resveratrol?
 A: Resveratrol has been found to possess antiviral activity against a variety of viruses, including herpes simplex virus, human immunodeficiency virus, and hepatitis C virus. It has been shown to inhibit the replication of several viruses, including HIV, herpes simplex virus, and influenza virus, and to regulate TLR3 expression, thus affecting the recruitment of downstream related factors and finally affecting the regulation process of related signal pathways. It has also been studied for its antiviral activity against Reoviridae, and for its potential to inhibit Zika virus cytopathy effect. It has been active against Epstein virus, rotavirus, and vesicular stomatitis virus, and has been reported to alleviate virus-induced reproductive failure and to promote RSV clearance in the body more quickly.
 Sources:
  - 10.1155/2022/7138756: The Antiviral Activity of Resveratrol
  - 10.1155/2022/7138756: Antiviral Mechanisms of Resveratrol
  - 10.1155/2022/7138756: The antiviral effects of resveratrol are well demonstrated. Currently, studies on the antiviral mechanism of resveratrol mainly focus on two points.On the one hand, resveratrol possesses the ability to activate the host's immune defenses, turning on a complex network of bodies to fight or eliminate incoming viruses. NF-κB belongs to a family of inducible nuclear transcription factors, which regulates a wide array of genes involved in various processes of antiviral activity, inflammatory, and immune response . Meanwhile, it is noteworthy that Toll-like receptors (TLRs) are located upstream of the NF-κB signaling pathway and are responsible for induction of antiviral innate immune responses by recognizing virus infection, which leads to the production of proinflammatory cytokines, chemokines, and interferons . Thus, the TLRs/NF-κB pathway has been extensively studied during viral infection. Likewise, most research on antiviral drugs has focused on this pathway. Resveratrol regulated TLR3 expression, thus affecting the recruitment of downstream related factors and finally affecting the regulation process of related signal pathways. Moreover, resveratrol inhibits PRV by inhibiting the IκBα degradation induced by PRV infection, thereby inhibiting the activation of the NF-κB cell signaling pathway, and subsequently inhibiting the transcription of viral genes, protein and DNA synthesis, and virion production . Thus, the TLRs/NF-κB signaling pathway plays a crucial role in the antiviral process of resveratrol. On the other hand, resveratrol also has the ability to inhibit the production of virions by directly inhibiting the expression of key viral genes or by binding to key enzymes and proteins that disrupt the viral replication cycle. In this case, resveratrol could possess antiviral activities against ZIKV NS2B 18 NS3 and helicase 3 . Overall, the antiviral mechanisms of resveratrol are diverse. We have summarized many studies and found that most of them focus on the effects of resveratrol on host signal pathways and
```

### Comparing `cybrex-1.1.1/cybrex/cli.py` & `cybrex-1.1.2/cybrex/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import json
 import logging
+import re
 import sys
 import textwrap
 
 import fire
 from termcolor import colored
 
-from .cybrex_ai import CybrexAI
+from cybrex_ai import CybrexAI
 
 
-def create_snippet(document, metadata):
-    return metadata['doi'] + ': ' + document
+def create_snippet(document):
+    return document['metadata']['doi'] + ': ' + document['text']
 
 
 class CybrexCli:
     def __init__(self):
         self.cybrex = CybrexAI()
 
     async def add_all_documents(self):
         async with self.cybrex as cybrex:
             async for document in cybrex.geck.get_summa_client().documents('nexus_science'):
                 document = json.loads(document)
-                await self.cybrex.add_documents([document])
+                await self.cybrex.add_full_documents([document])
 
     async def dump_texts(self, query: str, output_path: str, n_summa_documents: int = 100):
         """
         Store STC text chunks in ZIP archive
 
         :param query: query to STC
         :param output_path: where to store result
@@ -46,15 +47,15 @@
         :param input_path:
         """
         async with self.cybrex as cybrex:
             await cybrex.import_texts(
                 input_path=input_path,
             )
 
-    async def chat_doc(self, field: str, value: str, question: str, n_results: int = 7):
+    async def chat_doc(self, field: str, value: str, question: str, n_results: int = 4):
         """
         Ask a question about content of document identified by DOI.
 
         :param field: name of the field in document used for selection
         :param value: value of the field in document used for selection
         :param question: Text question to the document
         :param n_results: the number of documents to extract from Chroma
@@ -62,67 +63,68 @@
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Document', 'green')}: {field}:{value}")
             print(f"{colored('Q', 'green')}: {question}")
             response = await cybrex.chat_document(field, value, question, n_results)
             print(f"{colored('A', 'green')}: {response}")
 
-    async def chat_sci(self, question: str, n_results: int = 7, n_summa_documents: int = 9):
+    async def chat_sci(self, query: str, n_results: int = 4, n_summa_documents: int = 10):
         """
         Ask a question about content of document identified by DOI.
 
-        :param question: Text question to the document
+        :param query: Text question to the document
         :param n_results: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
         :param n_summa_documents: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
-            print(f"{colored('Q', 'green')}: {question}")
-            response = await cybrex.chat_science(
-                question=question,
+            print(f"{colored('Q', 'green')}: {query}")
+            response, documents = await cybrex.chat_science(
+                query=query,
                 n_results=n_results,
                 n_summa_documents=n_summa_documents,
             )
-            print(f"{colored('A', 'green')}: {response['result'].strip()}")
-            snippets = [create_snippet(source_document.page_content, source_document.metadata) for source_document in response['source_documents']]
-            sources = textwrap.indent('\n'.join(snippets), ' - ')
-            print(f"{colored('Sources', 'green')}:\n{sources}")
+            response = re.sub(r'\(DOI: ([^)]+)\)', r'(https://doi.org/\g<1>)', response)
+            documents = [f'{document["doi"]}: {document["title"]}' for document in documents]
+            sources = '\n'.join(documents)
+            print(f"{colored('A', 'green')}: {response}")
+            print(f"{colored('References', 'green')}:\n{textwrap.indent(sources, ' - ')}")
 
     async def sum_doc(self, field: str, value: str):
         """
         Summarization of the document
 
         :param field: name of the field in document used for selection
         :param value: value of the field in document used for selection
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Document', 'green')}: {field}:{value}")
             response = await cybrex.summarize_document(field, value)
             print(f"{colored('Summarization', 'green')}: {response}")
 
-    async def semantic_search(self, query: str, n_results: int = 7, n_summa_documents: int = 9):
+    async def semantic_search(self, query: str, n_results: int = 10, n_summa_documents: int = 30):
         """
         Ask a question about content of document identified by DOI.
 
         :param query: query to STC
         :param n_results: number of pieces to return
         :param n_summa_documents: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Q', 'green')}: {query}")
-            response = await cybrex.semantic_search(
+            documents = await cybrex.semantic_search(
                 query=query,
                 n_results=n_results,
                 n_summa_documents=n_summa_documents
             )
             snippets = [
-                ' - ' + create_snippet(document, metadata)
-                for (document, metadata) in zip(response['documents'][0], response['metadatas'][0])
+                ' - ' + create_snippet(document)
+                for document in documents
             ]
             sources = '\n'.join(snippets)
             print(f"{colored('Sources', 'green')}:\n{sources}")
 
 
 async def cybrex_cli(debug: bool = False):
     """
```

### Comparing `cybrex-1.1.1/cybrex/cybrex_ai.py` & `cybrex-1.1.2/cybrex/cybrex_ai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import base64
 import io
 import json
 import logging
 import os.path
 import uuid
 from gzip import GzipFile
@@ -15,25 +16,20 @@
 import pypdf
 import yaml
 from aiokit import AioThing
 from bs4 import BeautifulSoup
 from izihawa_configurator import Configurator
 from izihawa_utils.exceptions import BaseError
 from izihawa_utils.file import mkdir_p
-from langchain.chains import RetrievalQA
 from langchain.chains.summarize import load_summarize_chain
 from langchain.schema import Document
-from langchain.vectorstores import Chroma
 from stc_geck.advices import get_documents_on_topic
 from stc_geck.client import StcGeck
 
-from .models import (
-    DefaultModel,
-    models_dict,
-)
+from models import CybrexModel
 
 
 class DocumentNotFoundError(BaseError):
     pass
 
 
 def print_color(text, color):
@@ -43,15 +39,15 @@
 def default_config():
     return {
         'ipfs': {
             'http': {
                 'base_url': 'http://127.0.0.1:8080'
             }
         },
-        'model': DefaultModel.name,
+        'model': CybrexModel.default_config(),
         'summa': {
             'endpoint': '127.0.0.1:10082'
         },
     }
 
 
 class CybrexAI(AioThing):
@@ -74,27 +70,26 @@
             with open(config_path, 'w') as f:
                 f.write(yaml.dump(default_config(), default_flow_style=False))
 
         config = Configurator(configs=[
             config_path,
         ])
 
+        self.model = CybrexModel(config['model'])
+
         self.client_settings = chromadb.config.Settings(
             chroma_db_impl="duckdb+parquet",
             persist_directory=os.path.join(self.home_path, 'chroma'),
         )
         self.db = chromadb.Client(self.client_settings)
-        self.collection_name = config['model']
-
-        self.model = models_dict[config['model']]()
+        self.collection_name = self.model.get_embeddings_id()
 
-        real_embedding_function = self.model.embedding_function.embed_documents
         self.collection = self.db.get_or_create_collection(
             name=self.collection_name,
-            embedding_function=real_embedding_function,
+            embedding_function=self.model.embedder.embed_documents,
         )
         self.geck = geck
         if not self.geck:
             self.geck = StcGeck(
                 ipfs_http_base_url=config['ipfs']['http']['base_url'],
                 grpc_api_endpoint=config['summa']['endpoint']
             )
@@ -176,46 +171,37 @@
                 'doi': doi,
             })
             document_metadatas, document_texts = await self.generate_chunks_from_document(document)
             metadatas.extend(document_metadatas)
             texts.extend(document_texts)
         return metadatas, texts
 
-    async def add_documents(self, documents: List[dict], skip_downloading_pdf: bool = True):
+    async def add_full_documents(self, documents: List[dict], skip_downloading_pdf: bool = True):
         if not documents:
             return
         metadatas, texts = await self._get_missing_documents_chunks(documents, skip_downloading_pdf=skip_downloading_pdf)
         if texts:
             self.collection.upsert(
                 documents=texts,
                 metadatas=metadatas,
                 ids=[str(uuid.uuid1()) for _ in range(len(texts))]
             )
 
-    async def add_document_by_field_value(self, field, value) -> List[Document]:
+    async def add_full_document_by_field_value(self, field, value) -> List[Document]:
         documents = await self.geck.get_summa_client().search_documents([{
             'index_alias': 'nexus_science',
             'collectors': [{'top_docs': {'limit': 1}}],
             'query': {'term': {'field': field, 'value': value}}
         }])
         if not documents:
             raise DocumentNotFoundError(**{field: value})
-        await self.add_documents(documents)
+        await self.add_full_documents(documents)
         documents = [Document(page_content=text) for text in self.collection.get(where={field: value})['documents']]
         return documents
 
-    def as_retriever(self, embedding_function=None, **kwargs):
-        chroma = Chroma(
-            client=self.db,
-            collection_name=self.collection_name,
-            persist_directory=self.home_path,
-            embedding_function=embedding_function or self.model.embedding_function,
-        )
-        return chroma.as_retriever(**kwargs)
-
     async def dump_texts(self, query: str, output_path: str, n_summa_documents: int, skip_downloading_pdf: bool = True):
         documents = await self.keywords_search(query, n_summa_documents=n_summa_documents)
         metadatas, texts = await self._get_missing_documents_chunks(
             documents,
             skip_downloading_pdf=skip_downloading_pdf,
         )
         with GzipFile(output_path, mode='wb') as zipper:
@@ -248,74 +234,76 @@
             self.collection.upsert(
                 documents=texts,
                 metadatas=metadatas,
                 embeddings=embeddings,
                 ids=[str(uuid.uuid1()) for _ in range(len(texts))]
             )
 
-    async def chat_document(self, field, value, question, n_results: int):
-        await self.add_document_by_field_value(field, value)
-        if n_results > 3:
-            chain_type = 'map_reduce'
-        else:
-            chain_type = 'stuff'
-        qa = RetrievalQA.from_chain_type(
-            llm=self.model.llm,
-            chain_type=chain_type,
-            retriever=self.as_retriever(
-                search_type='similarity',
-                search_kwargs={
-                    'k': n_results,
-                    'filter': {
-                        field: value,
-                    }
-                },
-            ),
-        )
-        result = qa({"query": question})
-        return result["result"].strip()
+    async def chat_document(self, field, value, query, n_results: int):
+        await self.add_full_document_by_field_value(field, value)
 
-    async def chat_science(self, query: str, n_results: int, n_summa_documents: int):
-        documents = await self.keywords_search(query, n_summa_documents)
-        await self.add_documents(documents)
+        documents = await self._query(query, n_results, where={field: value})
+        result = self.model.llm.query_documents(query, documents)
 
-        qa = self.model.get_retrieval_qa(retriever=self.as_retriever(
-            search_type='similarity',
-            search_kwargs={
-                'k': n_results,
-            },
-        ))
-        result = qa({"query": query})
         return result
 
+    async def chat_science(self, query: str, n_results: int, n_summa_documents: int):
+        full_documents = await self.keywords_search(query, n_summa_documents)
+        await self.add_full_documents(full_documents)
+
+        documents = await self._query(query, n_results)
+        result = self.model.llm.query_documents(query, documents)
+        return result, await self.get_summa_documents_from_documents(documents)
+
+    async def _query(self, query: str, n_results: int = 3, where: Optional[dict] = None):
+        response = self.collection.query(
+            query_embeddings=[self.model.embedder.embed_query(query)],
+            n_results=n_results,
+            include=['documents', 'metadatas', 'distances'],
+            where=where,
+        )
+        documents = []
+        for (text, metadata, distance) in zip(response['documents'][0], response['metadatas'][0], response['distances'][0]):
+            documents.append({'text': text, 'metadata': metadata, 'distance': distance})
+        return documents
+
     async def keywords_search(self, query: str, n_summa_documents: int):
         if not n_summa_documents:
             return []
         keywords = self.model.keyword_extractor.extract_keywords(
             query,
-            top_n=3,
             keyphrase_ngram_range=(1, 1),
         )
-        topic = ' '.join(map(lambda x: x[0], keywords))
+        topic = ' '.join(map(lambda x: x[0], filter(lambda x: x[1] > 0.5, keywords)))
         documents = await get_documents_on_topic(
             summa_client=self.geck.get_summa_client(),
             topic=topic,
             documents=n_summa_documents,
         )
         return documents
 
-    async def semantic_search(self, query: str, n_results: int = 10, n_summa_documents: int = 10):
-        documents = await self.keywords_search(query, n_summa_documents)
-        await self.add_documents(documents)
-
-        query_embedding = self.model.embedding_function.embed_query(query)
-        return self.collection.query(
-            query_embeddings=[query_embedding],
-            n_results=n_results,
-            include=['documents', 'metadatas', 'distances'],
-        )
+    async def get_summa_documents_from_documents(self, documents):
+        dois = set([document['metadata']['doi'] for document in documents])
+        _summa_documents = await asyncio.gather(*[
+            self.geck.get_summa_client().search_documents([{
+                'index_alias': 'nexus_science',
+                'query': {'term': {'field': 'doi', 'value': doi}},
+                'collectors': [{'top_docs': {'limit': 100}}],
+            }])
+            for doi in dois
+        ])
+        summa_documents = []
+        for summa_document in _summa_documents:
+            summa_documents.append(summa_document[0])
+        return summa_documents
+
+    async def semantic_search(self, query: str, n_results: int = 10, n_summa_documents: int = 30):
+        full_documents = await self.keywords_search(query, n_summa_documents)
+        await self.add_full_documents(full_documents)
+        documents = await self._query(query, n_results)
+        return await self.get_summa_documents_from_documents(documents)
 
     async def summarize_document(self, field, value):
-        documents = await self.add_document_by_field_value(field, value)
+        documents = await self.add_full_document_by_field_value(field, value)
         chain = load_summarize_chain(llm=self.model.llm, chain_type="map_reduce")
         result = chain.run(documents)
         return result.strip()
```

### Comparing `cybrex-1.1.1/cybrex.egg-info/PKG-INFO` & `cybrex-1.1.2/cybrex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.1
+Version: 1.1.2
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -69,15 +69,15 @@
 Zika virus (ZIKV). Resveratrol appears to block the activities of the TIR-domain-containing
 adapter-inducing interferon-β (TRIF) complex, suggesting that resveratrol would also inhibit NF-κB
 transcription induced by TRIF. Additionally, it has been reported to reduce the activity of respiratory
 syncytial virus (RSV) and to stimulate the secretion of higher levels of TNF-α, promoting cell death
 and RSV clearance.
 
 # Question enitre science
-cybrex - chat-sci --question "What is the antivirus effect of resveratrol?" --top-n 15 --summa-documents 40
+cybrex - chat-sci --question "What is the antivirus effect of resveratrol?" --n-results 15 --n-summa-documents 40
 
 Q: What is the antivirus effect of resveratrol?
 A: Resveratrol has been found to possess antiviral activity against a variety of viruses, including herpes simplex virus, human immunodeficiency virus, and hepatitis C virus. It has been shown to inhibit the replication of several viruses, including HIV, herpes simplex virus, and influenza virus, and to regulate TLR3 expression, thus affecting the recruitment of downstream related factors and finally affecting the regulation process of related signal pathways. It has also been studied for its antiviral activity against Reoviridae, and for its potential to inhibit Zika virus cytopathy effect. It has been active against Epstein virus, rotavirus, and vesicular stomatitis virus, and has been reported to alleviate virus-induced reproductive failure and to promote RSV clearance in the body more quickly.
 Sources:
  - 10.1155/2022/7138756: The Antiviral Activity of Resveratrol
  - 10.1155/2022/7138756: Antiviral Mechanisms of Resveratrol
  - 10.1155/2022/7138756: The antiviral effects of resveratrol are well demonstrated. Currently, studies on the antiviral mechanism of resveratrol mainly focus on two points.On the one hand, resveratrol possesses the ability to activate the host's immune defenses, turning on a complex network of bodies to fight or eliminate incoming viruses. NF-κB belongs to a family of inducible nuclear transcription factors, which regulates a wide array of genes involved in various processes of antiviral activity, inflammatory, and immune response . Meanwhile, it is noteworthy that Toll-like receptors (TLRs) are located upstream of the NF-κB signaling pathway and are responsible for induction of antiviral innate immune responses by recognizing virus infection, which leads to the production of proinflammatory cytokines, chemokines, and interferons . Thus, the TLRs/NF-κB pathway has been extensively studied during viral infection. Likewise, most research on antiviral drugs has focused on this pathway. Resveratrol regulated TLR3 expression, thus affecting the recruitment of downstream related factors and finally affecting the regulation process of related signal pathways. Moreover, resveratrol inhibits PRV by inhibiting the IκBα degradation induced by PRV infection, thereby inhibiting the activation of the NF-κB cell signaling pathway, and subsequently inhibiting the transcription of viral genes, protein and DNA synthesis, and virion production . Thus, the TLRs/NF-κB signaling pathway plays a crucial role in the antiviral process of resveratrol. On the other hand, resveratrol also has the ability to inhibit the production of virions by directly inhibiting the expression of key viral genes or by binding to key enzymes and proteins that disrupt the viral replication cycle. In this case, resveratrol could possess antiviral activities against ZIKV NS2B 18 NS3 and helicase 3 . Overall, the antiviral mechanisms of resveratrol are diverse. We have summarized many studies and found that most of them focus on the effects of resveratrol on host signal pathways and
```

### Comparing `cybrex-1.1.1/pyproject.toml` & `cybrex-1.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.1.1"
+version = "1.1.2"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

