# Comparing `tmp/taxonerd-1.5.1.tar.gz` & `tmp/taxonerd-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxonerd-1.5.1.tar", last modified: Tue Feb 21 15:57:19 2023, max compression
+gzip compressed data, was "taxonerd-1.5.2.tar", last modified: Tue Aug  1 09:36:35 2023, max compression
```

## Comparing `taxonerd-1.5.1.tar` & `taxonerd-1.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-02-21 15:57:19.684868 taxonerd-1.5.1/
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     1078 2019-12-04 15:52:33.000000 taxonerd-1.5.1/LICENSE
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)    15679 2023-02-21 15:57:19.684868 taxonerd-1.5.1/PKG-INFO
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)    14616 2023-02-21 15:56:33.000000 taxonerd-1.5.1/README.md
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)       90 2022-09-30 09:20:00.000000 taxonerd-1.5.1/pyproject.toml
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     1669 2023-02-21 15:57:19.684868 taxonerd-1.5.1/setup.cfg
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)       36 2022-10-17 14:24:16.000000 taxonerd-1.5.1/setup.py
-drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-02-21 15:57:19.684868 taxonerd-1.5.1/taxonerd/
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)       73 2023-02-21 15:56:11.000000 taxonerd-1.5.1/taxonerd/__init__.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     4924 2022-10-03 15:27:00.000000 taxonerd-1.5.1/taxonerd/abbreviation.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     2867 2023-02-17 16:26:18.000000 taxonerd-1.5.1/taxonerd/cli.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     2974 2022-10-03 15:18:08.000000 taxonerd-1.5.1/taxonerd/extractor.py
-drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-02-21 15:57:19.684868 taxonerd-1.5.1/taxonerd/linking/
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)        0 2020-12-14 18:34:32.000000 taxonerd-1.5.1/taxonerd/linking/__init__.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)    21402 2023-02-21 15:46:26.000000 taxonerd-1.5.1/taxonerd/linking/candidate_generation.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     5314 2021-08-06 14:34:08.000000 taxonerd-1.5.1/taxonerd/linking/file_cache.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     7582 2023-02-21 15:47:47.000000 taxonerd-1.5.1/taxonerd/linking/linking.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     6725 2021-08-10 15:47:16.000000 taxonerd-1.5.1/taxonerd/linking/linking_utils.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     5710 2023-02-21 14:22:45.000000 taxonerd-1.5.1/taxonerd/taxonerd.py
-drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-02-21 15:57:19.684868 taxonerd-1.5.1/taxonerd.egg-info/
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)    15679 2023-02-21 15:57:19.000000 taxonerd-1.5.1/taxonerd.egg-info/PKG-INFO
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)      599 2023-02-21 15:57:19.000000 taxonerd-1.5.1/taxonerd.egg-info/SOURCES.txt
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)        1 2023-02-21 15:57:19.000000 taxonerd-1.5.1/taxonerd.egg-info/dependency_links.txt
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)       47 2023-02-21 15:57:19.000000 taxonerd-1.5.1/taxonerd.egg-info/entry_points.txt
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)        1 2020-12-07 13:57:26.000000 taxonerd-1.5.1/taxonerd.egg-info/not-zip-safe
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)      399 2023-02-21 15:57:19.000000 taxonerd-1.5.1/taxonerd.egg-info/requires.txt
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)        9 2023-02-21 15:57:19.000000 taxonerd-1.5.1/taxonerd.egg-info/top_level.txt
-drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-02-21 15:57:19.684868 taxonerd-1.5.1/tests/
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)      602 2022-10-03 14:50:52.000000 taxonerd-1.5.1/tests/test_cli.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     1407 2022-10-03 14:33:22.000000 taxonerd-1.5.1/tests/test_init.py
--rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     1609 2022-10-03 15:33:49.000000 taxonerd-1.5.1/tests/test_ner.py
+drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-08-01 09:36:35.928161 taxonerd-1.5.2/
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     1078 2019-12-04 15:52:33.000000 taxonerd-1.5.2/LICENSE
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)    15679 2023-08-01 09:36:35.928161 taxonerd-1.5.2/PKG-INFO
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)    14616 2023-02-21 15:56:33.000000 taxonerd-1.5.2/README.md
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)       90 2022-09-30 09:20:00.000000 taxonerd-1.5.2/pyproject.toml
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     1669 2023-08-01 09:36:35.928161 taxonerd-1.5.2/setup.cfg
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)       36 2022-10-17 14:24:16.000000 taxonerd-1.5.2/setup.py
+drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-08-01 09:36:35.900161 taxonerd-1.5.2/taxonerd/
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)       73 2023-07-31 08:38:28.000000 taxonerd-1.5.2/taxonerd/__init__.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     4924 2022-10-03 15:27:00.000000 taxonerd-1.5.2/taxonerd/abbreviation.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     2867 2023-02-17 16:26:18.000000 taxonerd-1.5.2/taxonerd/cli.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     2974 2022-10-03 15:18:08.000000 taxonerd-1.5.2/taxonerd/extractor.py
+drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-08-01 09:36:35.912161 taxonerd-1.5.2/taxonerd/linking/
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)        0 2020-12-14 18:34:32.000000 taxonerd-1.5.2/taxonerd/linking/__init__.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)    22464 2023-08-01 09:05:27.000000 taxonerd-1.5.2/taxonerd/linking/candidate_generation.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     5314 2021-08-06 14:34:08.000000 taxonerd-1.5.2/taxonerd/linking/file_cache.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     7660 2023-08-01 08:56:41.000000 taxonerd-1.5.2/taxonerd/linking/linking.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     6371 2023-07-31 12:45:31.000000 taxonerd-1.5.2/taxonerd/linking/linking_utils.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     5748 2023-08-01 09:03:16.000000 taxonerd-1.5.2/taxonerd/taxonerd.py
+drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-08-01 09:36:35.904161 taxonerd-1.5.2/taxonerd.egg-info/
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)    15679 2023-08-01 09:36:35.000000 taxonerd-1.5.2/taxonerd.egg-info/PKG-INFO
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)      599 2023-08-01 09:36:35.000000 taxonerd-1.5.2/taxonerd.egg-info/SOURCES.txt
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)        1 2023-08-01 09:36:35.000000 taxonerd-1.5.2/taxonerd.egg-info/dependency_links.txt
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)       47 2023-08-01 09:36:35.000000 taxonerd-1.5.2/taxonerd.egg-info/entry_points.txt
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)        1 2020-12-07 13:57:26.000000 taxonerd-1.5.2/taxonerd.egg-info/not-zip-safe
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)      399 2023-08-01 09:36:35.000000 taxonerd-1.5.2/taxonerd.egg-info/requires.txt
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)        9 2023-08-01 09:36:35.000000 taxonerd-1.5.2/taxonerd.egg-info/top_level.txt
+drwxrwxr-x   0 leguilln  (1001) leguilln  (1001)        0 2023-08-01 09:36:35.920161 taxonerd-1.5.2/tests/
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)      602 2022-10-03 14:50:52.000000 taxonerd-1.5.2/tests/test_cli.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     1407 2022-10-03 14:33:22.000000 taxonerd-1.5.2/tests/test_init.py
+-rw-rw-r--   0 leguilln  (1001) leguilln  (1001)     1609 2022-10-03 15:33:49.000000 taxonerd-1.5.2/tests/test_ner.py
```

### Comparing `taxonerd-1.5.1/LICENSE` & `taxonerd-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/PKG-INFO` & `taxonerd-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxonerd
-Version: 1.5.1
+Version: 1.5.2
 Summary: A Python package and CLI tool based on spaCy for detecting mentions of taxonomic entities in text
 Home-page: https://github.com/nleguillarme/taxonerd
 Author-email: nicolas.leguillarme@univ-grenoble-alpes.fr
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/nleguillarme/taxonerd/issues
 Keywords: spacy,ner,transformers,deep neural networks,ecology,evolution
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `taxonerd-1.5.1/README.md` & `taxonerd-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/setup.cfg` & `taxonerd-1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/taxonerd/abbreviation.py` & `taxonerd-1.5.2/taxonerd/abbreviation.py`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/taxonerd/cli.py` & `taxonerd-1.5.2/taxonerd/cli.py`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/taxonerd/extractor.py` & `taxonerd-1.5.2/taxonerd/extractor.py`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/taxonerd/linking/candidate_generation.py` & `taxonerd-1.5.2/taxonerd/linking/candidate_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Dict, Tuple, NamedTuple, Type
-from pathlib import Path
+from os import path
 import json
 import datetime
 from collections import defaultdict
 
 import scipy
 import numpy
 import joblib
@@ -27,18 +27,20 @@
         Path to the joblib serialized sklearn TfidfVectorizer.
     tfidf_vectors: str
         Path to the float-16 encoded tf-idf vectors for the entities in the KB.
     concept_aliases_list: str
         Path to the indices mapping concepts to aliases in the index.
     """
 
-    ann_index: str
-    tfidf_vectorizer: str
-    tfidf_vectors: str
-    concept_aliases_list: str
+    ann_index: str | Tuple[str, str]
+    tfidf_vectorizer: str | Tuple[str, str]
+    tfidf_vectors: str | Tuple[str, str]
+    concept_aliases_list: str | Tuple[str, str]
+    # kb: str | Path = None
+    # prefix: str = None
 
 
 GbifLinkerPaths = LinkerPaths(
     ann_index=(
         "https://cloud.univ-grenoble-alpes.fr/index.php/s/TrgYQDqPsasW6o9/download",
         "gbif_backbone_2019_09_06/nmslib_index.bin",
     ),  # nmslib_index.bin
@@ -214,58 +216,68 @@
     verbose: bool
         Setting to true will print extra information about the generated candidates.
     ef_search: int
         The efs search parameter used in the index. This substantially effects runtime speed
         (higher is slower but slightly more accurate). Note that this parameter is ignored
         if a preconstructed ann_index is passed.
     name: str, optional (default = None)
-        The name of the pretrained entity linker to load. Must be one of 'umls' or 'mesh'.
+        The name of the prPathetrained entity linker to load. Must be one of 'umls' or 'mesh'.
     """
 
     def __init__(
         self,
         ann_index: FloatIndex = None,
         tfidf_vectorizer: TfidfVectorizer = None,
         ann_concept_aliases_list: List[str] = None,
         kb: KnowledgeBase = None,
         verbose: bool = False,
         ef_search: int = 200,
-        name: str = None,
+        name_or_path: str = None,
+        # path: Path = None,
     ) -> None:
-
-        if name is not None and any(
+        if name_or_path is not None and any(
             [ann_index, tfidf_vectorizer, ann_concept_aliases_list]  # , kb]
         ):
             raise ValueError(
                 "You cannot pass both a name argument and other constuctor arguments."
             )
 
-        # Set the name to the default, after we have checked
-        # the compatability with the args above.
-        if name is None:
+        if name_or_path:
+            self.kb = kb or KnowledgeBaseFactory().get_kb(name_or_path)
+            if not self.kb:
+                if path.exists(name_or_path):
+                    with open(name_or_path) as f:
+                        linker_cfg = json.load(f)
+                    name = linker_cfg["name"]
+                    self.kb = KnowledgeBase(**linker_cfg["kb"])
+                    linker_paths = LinkerPaths(**linker_cfg["linker_paths"])
+                else:
+                    raise ValueError(
+                        f"{name_or_path} is not a valid linker name nor a valid path to a linker config."
+                    )
+            else:
+                name = name_or_path
+                linker_paths = DEFAULT_PATHS.get(name_or_path)
+        else:
             name = "gbif_backbone"
-
-        linker_paths = DEFAULT_PATHS.get(name, GbifLinkerPaths)
+            self.kb = KnowledgeBaseFactory().get_kb(name)
+            linker_paths = DEFAULT_PATHS.get(name, GbifLinkerPaths)
 
         self.ann_index = ann_index or load_approximate_nearest_neighbours_index(
             linker_paths=linker_paths, ef_search=ef_search
         )
         self.vectorizer = tfidf_vectorizer or joblib.load(
             cached_path(linker_paths.tfidf_vectorizer)
         )
         self.ann_concept_aliases_list = ann_concept_aliases_list or json.load(
             open(cached_path(linker_paths.concept_aliases_list))
         )
 
-        self.kb = kb or KnowledgeBaseFactory().get_kb(name)
         self.verbose = verbose
 
-        # TODO(Mark): Remove in scispacy v1.0.
-        # self.umls = self.kb
-
     def nmslib_knn_with_zero_vectors(
         self, vectors: numpy.ndarray, k: int
     ) -> Tuple[numpy.ndarray, numpy.ndarray]:
         """
         ann_index.knnQueryBatch crashes if any of the vectors is all zeros.
         This function is a wrapper around `ann_index.knnQueryBatch` that solves this problem. It works as follows:
         - remove empty vectors from `vectors`.
@@ -301,16 +313,16 @@
         )
         neighbors = list(neighbors)
         distances = list(distances)
 
         # neighbors need to be converted to an np.array of objects instead of ndarray of dimensions len(vectors)xk
         # Solution: add a row to `neighbors` with any length other than k. This way, calling np.array(neighbors)
         # returns an np.array of objects
-        neighbors.append([None]*(k+1)) # Just using [] create a ValueError in R
-        distances.append([None]*(k+1))
+        neighbors.append([None] * (k + 1))  # Just using [] create a ValueError in R
+        distances.append([None] * (k + 1))
 
         # interleave `neighbors` and Nones in `extended_neighbors`
         extended_neighbors[empty_vectors_boolean_flags] = numpy.array(
             neighbors, dtype=object
         )[:-1]
         extended_distances[empty_vectors_boolean_flags] = numpy.array(
             distances, dtype=object
@@ -434,15 +446,19 @@
     kb = kb or UmlsKnowledgeBase()
 
     # nmslib hyperparameters (very important)
     # guide: https://github.com/nmslib/nmslib/blob/master/python_bindings/parameters.md
     # Default values resulted in very low recall.
 
     # set to the maximum recommended value. Improves recall at the expense of longer indexing time.
-    # TODO: This variable name is so hot because I don't actually know what this parameter does.
+    # We use the HNSW (Hierarchical Navigable Small World Graph) representation which is constructed
+    # by consecutive insertion of elements in a random order by connecting them to M closest neighbours
+    # from the previously inserted elements. These later become bridges between the network hubs that
+    # improve overall graph connectivity. (bigger M -> higher recall, slower creation)
+    # For more details see:  https://arxiv.org/pdf/1603.09320.pdf?
     m_parameter = 100
     # `C` for Construction. Set to the maximum recommended value
     # Improves recall at the expense of longer indexing time
     construction = 2000
     num_threads = 60  # set based on the machine
     index_params = {
         "M": m_parameter,
@@ -458,19 +474,15 @@
 
     # NOTE: here we are creating the tf-idf vectorizer with float32 type, but we can serialize the
     # resulting vectors using float16, meaning they take up half the memory on disk. Unfortunately
     # we can't use the float16 format to actually run the vectorizer, because of this bug in sparse
     # matrix representations in scipy: https://github.com/scipy/scipy/issues/7408
     print(f"Fitting tfidf vectorizer on {len(concept_aliases)} aliases")
     tfidf_vectorizer = TfidfVectorizer(
-        analyzer="char_wb",
-        ngram_range=(3, 3),
-        min_df=10,
-        dtype=numpy.float32,
-        lowercase=True,
+        analyzer="char_wb", ngram_range=(3, 3), min_df=10, dtype=numpy.float32
     )
     start_time = datetime.datetime.now()
     concept_alias_tfidfs = tfidf_vectorizer.fit_transform(concept_aliases)
     print(f"Saving tfidf vectorizer to {tfidf_vectorizer_path}")
     joblib.dump(tfidf_vectorizer, tfidf_vectorizer_path)
     end_time = datetime.datetime.now()
     total_time = end_time - start_time
@@ -495,16 +507,17 @@
     concept_alias_tfidfs = concept_alias_tfidfs[empty_tfidfs_boolean_flags]
     assert len(concept_aliases) == numpy.size(concept_alias_tfidfs, 0)
 
     print(
         f"Saving list of concept ids and tfidfs vectors to {uml_concept_aliases_path} and {tfidf_vectors_path}"
     )
     json.dump(concept_aliases, open(uml_concept_aliases_path, "w"))
+
     scipy.sparse.save_npz(
-        tfidf_vectors_path, concept_alias_tfidfs.astype(numpy.float16)
+        tfidf_vectors_path, concept_alias_tfidfs  # .astype(numpy.float16)
     )
 
     print(f"Fitting ann index on {len(concept_aliases)} aliases (takes 2 hours)")
     start_time = datetime.datetime.now()
     ann_index = nmslib.init(
         method="hnsw",
         space="cosinesimil_sparse",
```

### Comparing `taxonerd-1.5.1/taxonerd/linking/file_cache.py` & `taxonerd-1.5.2/taxonerd/linking/file_cache.py`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/taxonerd/linking/linking.py` & `taxonerd-1.5.2/taxonerd/linking/linking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from spacy.tokens import Doc
 from spacy.tokens import Span
 from spacy.language import Language
-from taxonerd.linking.candidate_generation import CandidateGenerator
+from taxonerd.linking.candidate_generation import CandidateGenerator, LinkerPaths
+from typing import Optional
 
 
 @Language.factory("taxo_linker")
 class EntityLinker:
     """
     A spacy pipeline component which identifies entities in text which appear
     in a knowledge base.
@@ -61,31 +62,31 @@
         how many are nearest neighbours are found.
     linker_name: str, optional (default = None)
         The name of the pretrained entity linker to load.
     """
 
     def __init__(
         self,
-        nlp: Language = None,
+        nlp: Optional[Language] = None,
         name: str = "taxonerd_linker",
-        candidate_generator: CandidateGenerator = None,
+        candidate_generator: Optional[CandidateGenerator] = None,
         resolve_abbreviations: bool = True,
         k: int = 30,
         threshold: float = 0.7,
         no_definition_threshold: float = 0.95,
         filter_for_definitions: bool = True,
         max_entities_per_mention: int = 5,
-        linker_name: str = None,
+        linker_name: Optional[str] = None,
     ):
         # TODO(Mark): Remove in scispacy v1.0.
         # Span.set_extension("umls_ents", default=[], force=True)
         Span.set_extension("kb_ents", default=[], force=True)
 
         self.candidate_generator = candidate_generator or CandidateGenerator(
-            name=linker_name
+            name_or_path=linker_name
         )
         self.resolve_abbreviations = resolve_abbreviations
         self.k = k
         self.threshold = threshold
         self.no_definition_threshold = no_definition_threshold
         self.kb = self.candidate_generator.kb
         self.filter_for_definitions = filter_for_definitions
@@ -112,15 +113,14 @@
             # mention_strings = [
             #     " ".join([tok.lemma_ for tok in ent]) for ent in doc.ents
             # ]
         # print(doc.ents, mention_strings)
         unique_mention_strings = set(mention_strings)
 
         if len(unique_mention_strings) > 0:
-
             batch_candidates = self.candidate_generator(unique_mention_strings, self.k)
             # batch_candidates = self.candidate_generator(mention_strings, self.k)
 
             kb_ents_per_mention_string = {}
 
             for mention_string, candidates in zip(
                 unique_mention_strings, batch_candidates
```

### Comparing `taxonerd-1.5.1/taxonerd/linking/linking_utils.py` & `taxonerd-1.5.2/taxonerd/linking/linking_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 from typing import List, Dict, NamedTuple, Optional, Set, Tuple, Union
 import json
 from pathlib import Path
 from collections import defaultdict
 import sqlite3
-
 from .file_cache import cached_path
-from scispacy.umls_semantic_type_tree import (
-    UmlsSemanticTypeTree,
-    construct_umls_tree_from_tsv,
-)
-
 from urllib.request import pathname2url
 import os
-
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def escape_quotes(alias):
     alias = alias.replace("'", "''")
     alias = alias.replace('"', '""')
     return alias
 
 
 class Entity(NamedTuple):
-
     concept_id: str
     canonical_name: str
     aliases: List[str]
     types: List[str] = []
     definition: Optional[str] = None
 
     def __repr__(self):
-
         rep = ""
         num_aliases = len(self.aliases)
         rep = rep + f"CUI: {self.concept_id}, Name: {self.canonical_name}\n"
         rep = rep + f"Definition: {self.definition}\n"
         rep = rep + f"TUI(s): {', '.join(self.types)}\n"
         if num_aliases > 10:
             rep = (
@@ -68,54 +59,48 @@
         if file_path is None:
             raise ValueError(
                 "Do not use the default arguments to KnowledgeBase. "
                 "Instead, use a subclass (e.g GbifKnowledgeBase) or pass a path to a kb."
             )
 
         file_path = cached_path(file_path)
-        if type(file_path) is tuple:
-            user_friendly_name = file_path[1]
-            file_path = file_path[0]
         db_path = os.path.splitext(file_path)[0] + ".db"
 
-        if not os.path.exists(db_path):
-            logger.info(
-                "File {} not found, create SQLite database from {}".format(
-                    db_path, file_path
-                )
-            )
-            self.conn = self.json_to_sqlite(file_path, db_path)
-
-        self.conn = self.get_conn_to_db(db_path)
-
-    def json_to_sqlite(self, file_path: str = None, db_path: str = None):
         if file_path.endswith("jsonl"):
             raw = (json.loads(line) for line in open(cached_path(file_path)))
         else:
             raw = json.load(open(cached_path(file_path)))
 
-        alias_to_cuis = defaultdict(set)
-        cui_to_entity = {}
+        alias_to_cuis: Dict[str, Set[str]] = defaultdict(set)
+        self.cui_to_entity: Dict[str, Entity] = {}
 
         for concept in raw:
             unique_aliases = set(concept["aliases"])
             unique_aliases.add(concept["canonical_name"])
             for alias in unique_aliases:
-                # alias_to_cuis[alias] = (
-                #     set() if alias not in alias_to_cuis else alias_to_cuis[alias]
-                # )
                 alias_to_cuis[alias].add(concept["concept_id"])
-            cui_to_entity[concept["concept_id"]] = Entity(**concept)
+            self.cui_to_entity[concept["concept_id"]] = Entity(**concept)
+
+        self.alias_to_cuis: Dict[str, Set[str]] = {**alias_to_cuis}
 
-        alias_to_cuis: Dict[str, Set[str]] = {**alias_to_cuis}
+        if not os.path.exists(db_path):
+            logger.info(
+                "File {} not found, create SQLite database from {}".format(
+                    db_path, file_path
+                )
+            )
+            self.conn = self.json_to_sqlite(db_path)
+
+        self.conn = self.get_conn_to_db(db_path)
 
+    def json_to_sqlite(self, db_path: str = None):
         conn = sqlite3.connect(db_path)
         c = conn.cursor()
         c.execute("""CREATE TABLE alias_to_cuis (alias, cuis)""")
-        entries = [(k, str(v)) for k, v in alias_to_cuis.items()]
+        entries = [(k, str(v)) for k, v in self.alias_to_cuis.items()]
         c.executemany("INSERT INTO alias_to_cuis VALUES (?,?)", entries)
         conn.commit()
         return conn
 
     def get_conn_to_db(self, file_path: str = None):
         dburi = "file:{}?mode=rw".format(pathname2url(file_path))
         conn = sqlite3.connect(dburi, uri=True)
@@ -142,32 +127,31 @@
             "SELECT alias, cuis FROM alias_to_cuis WHERE alias IN ({});".format(
                 ",".join(aliases_str)
             )
         )
         mentions_to_concepts: Dict[str, List[str]] = defaultdict(list)
         for x in c.fetchall():
             concept_ids = [self.prefix + t.strip() for t in x[1].strip("{}").split(",")]
-            mentions_to_concepts[x[0]].extend(
-                concept_ids
-            )  # self.prefix + x[1].strip("{}"))
+            mentions_to_concepts[x[0]].extend(concept_ids)
         return mentions_to_concepts
 
 
 class KnowledgeBaseFactory:
     def get_kb(self, name=None):
         if name == "gbif_backbone":
             return GbifKnowledgeBase()
         elif name == "taxref":
             return TaxRefKnowledgeBase()
         elif name == "ncbi_taxonomy":
             return NCBIKnowledgeBase()
         elif name == "ncbi_lite":
             return NCBILiteKnowledgeBase()
         else:
-            raise ValueError(name)
+            logger.info(f"Cannot initialize KnowledgeBase with name {name}")
+            return None
 
 
 class GbifKnowledgeBase(KnowledgeBase):
     def __init__(
         self,
         file_path=(
             "https://cloud.univ-grenoble-alpes.fr/index.php/s/dm8attDW7EsdBpp/download",
```

### Comparing `taxonerd-1.5.1/taxonerd/taxonerd.py` & `taxonerd-1.5.2/taxonerd/taxonerd.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         if "taxo_abbrev_detector" not in exclude:
             from taxonerd.abbreviation import TaxonomicAbbreviationDetector
 
             self.nlp.add_pipe("taxo_abbrev_detector")
             self.abbrev = "taxo_abbrev_detector"
         if linker:
             if "lemmatizer" in exclude:
-                raise Exception("Lemmatizer is needed for entity linking. Make sure lemmatizer is not excluded from the pipeline")
+                raise Exception(
+                    "Lemmatizer is needed for entity linking. Make sure lemmatizer is not excluded from the pipeline"
+                )
 
             from taxonerd.linking.linking_utils import KnowledgeBaseFactory
             from taxonerd.linking.candidate_generation import CandidateGenerator
             from taxonerd.linking.linking import EntityLinker
 
             self.nlp.add_pipe(
                 "taxo_linker",
```

### Comparing `taxonerd-1.5.1/taxonerd.egg-info/PKG-INFO` & `taxonerd-1.5.2/taxonerd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxonerd
-Version: 1.5.1
+Version: 1.5.2
 Summary: A Python package and CLI tool based on spaCy for detecting mentions of taxonomic entities in text
 Home-page: https://github.com/nleguillarme/taxonerd
 Author-email: nicolas.leguillarme@univ-grenoble-alpes.fr
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/nleguillarme/taxonerd/issues
 Keywords: spacy,ner,transformers,deep neural networks,ecology,evolution
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `taxonerd-1.5.1/taxonerd.egg-info/SOURCES.txt` & `taxonerd-1.5.2/taxonerd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/tests/test_cli.py` & `taxonerd-1.5.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/tests/test_init.py` & `taxonerd-1.5.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `taxonerd-1.5.1/tests/test_ner.py` & `taxonerd-1.5.2/tests/test_ner.py`

 * *Files identical despite different names*

