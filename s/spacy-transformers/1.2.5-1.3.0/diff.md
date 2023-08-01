# Comparing `tmp/spacy-transformers-1.2.5.tar.gz` & `tmp/spacy-transformers-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-transformers-1.2.5.tar", last modified: Fri Jun  9 17:31:50 2023, max compression
+gzip compressed data, was "spacy-transformers-1.3.0.tar", last modified: Mon Jul 31 12:39:49 2023, max compression
```

## Comparing `spacy-transformers-1.2.5.tar` & `spacy-transformers-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4671 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      129 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3067 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.688743 spacy-transformers-1.2.5/spacy_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/align.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)     9887 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/align.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/annotation_setters.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14828 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/data_classes.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.688743 spacy-transformers-1.2.5/spacy_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/hf_shim.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2563 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/hf_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/listener.py
--rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/split_trf.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11549 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6448 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/trfs2arrays.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17118 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/pipeline_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/py.typed
--rw-r--r--   0 vsts      (1001) docker     (122)     2449 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/span_getters.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/spacy_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/spacy_transformers/tests/regression/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/regression/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/regression/test_spacy_issue6401.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/regression/test_spacy_issue7029.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_alignment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_configs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_data_classes.py
--rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_deprecations.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_model_sequence_classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3359 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_model_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16846 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_pipeline_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9837 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_spanners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1588 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_textcatcnn.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3132 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_tok2vectransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_truncation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4636 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/truncate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5440 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.688743 spacy-transformers-1.2.5/spacy_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1876 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:49.583187 spacy-transformers-1.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-07-31 12:39:49.583187 spacy-transformers-1.3.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4671 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      199 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3131 2023-07-31 12:39:49.583187 spacy-transformers-1.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2215 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:49.571186 spacy-transformers-1.3.0/spacy_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/align.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)     9887 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/align.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/annotation_setters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14828 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/data_classes.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:49.575186 spacy-transformers-1.3.0/spacy_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/layers/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5648 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/layers/hf_shim.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2563 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/layers/hf_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/layers/listener.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/layers/split_trf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11549 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/layers/transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6448 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/layers/trfs2arrays.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17118 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/pipeline_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (122)     2449 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/span_getters.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:49.579187 spacy-transformers-1.3.0/spacy_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:49.583187 spacy-transformers-1.3.0/spacy_transformers/tests/regression/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/regression/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/regression/test_spacy_issue6401.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/regression/test_spacy_issue7029.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_alignment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_configs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_data_classes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_deprecations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_model_sequence_classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3359 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_model_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21054 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_pipeline_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9837 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_spanners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1588 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_textcatcnn.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3132 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_tok2vectransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/test_truncation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4636 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/truncate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5440 2023-07-31 12:39:33.000000 spacy-transformers-1.3.0/spacy_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-31 12:39:49.575186 spacy-transformers-1.3.0/spacy_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-07-31 12:39:49.000000 spacy-transformers-1.3.0/spacy_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1876 2023-07-31 12:39:49.000000 spacy-transformers-1.3.0/spacy_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-31 12:39:49.000000 spacy-transformers-1.3.0/spacy_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-07-31 12:39:49.000000 spacy-transformers-1.3.0/spacy_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-31 12:39:48.000000 spacy-transformers-1.3.0/spacy_transformers.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      588 2023-07-31 12:39:49.000000 spacy-transformers-1.3.0/spacy_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-31 12:39:49.000000 spacy-transformers-1.3.0/spacy_transformers.egg-info/top_level.txt
```

### Comparing `spacy-transformers-1.2.5/LICENSE` & `spacy-transformers-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/PKG-INFO` & `spacy-transformers-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-transformers
-Version: 1.2.5
+Version: 1.3.0
 Summary: spaCy pipelines for pre-trained BERT and other transformers
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.5 Summary: spaCy
+Metadata-Version: 2.1 Name: spacy-transformers Version: 1.3.0 Summary: spaCy
 pipelines for pre-trained BERT and other transformers Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `spacy-transformers-1.2.5/README.md` & `spacy-transformers-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/setup.cfg` & `spacy-transformers-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.5
+version = 1.3.0
 description = spaCy pipelines for pre-trained BERT and other transformers
 url = https://spacy.io
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -28,16 +28,17 @@
 
 [options]
 zip_safe = false
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	spacy>=3.5.0,<4.0.0
-	numpy>=1.15.0
-	transformers>=3.4.0,<4.31.0
+	numpy>=1.15.0; python_version < "3.9"
+	numpy>=1.19.0; python_version >= "3.9"
+	transformers>=3.4.0,<4.32.0
 	torch>=1.8.0
 	srsly>=2.4.0,<3.0.0
 	dataclasses>=0.6,<1.0; python_version < "3.7"
 	spacy-alignments>=0.7.2,<1.0.0
 
 [options.extras_require]
 cuda =
```

### Comparing `spacy-transformers-1.2.5/setup.py` & `spacy-transformers-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, Extension, find_packages
-from distutils.command.build_ext import build_ext
+from setuptools.command.build_ext import build_ext
 from Cython.Build import cythonize
 from Cython.Compiler import Options
 import numpy
 
 
 # Preserve `__doc__` on functions and classes
 # http://docs.cython.org/en/latest/src/userguide/source_files_and_compilation.html#compiler-options
```

### Comparing `spacy-transformers-1.2.5/spacy_transformers/align.pyi` & `spacy-transformers-1.3.0/spacy_transformers/align.pyi`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/align.pyx` & `spacy-transformers-1.3.0/spacy_transformers/align.pyx`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/annotation_setters.py` & `spacy-transformers-1.3.0/spacy_transformers/annotation_setters.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/architectures.py` & `spacy-transformers-1.3.0/spacy_transformers/architectures.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/data_classes.py` & `spacy-transformers-1.3.0/spacy_transformers/data_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/layers/_util.py` & `spacy-transformers-1.3.0/spacy_transformers/layers/_util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/layers/hf_shim.py` & `spacy-transformers-1.3.0/spacy_transformers/layers/hf_shim.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict
 from io import BytesIO
 from pathlib import Path
 import srsly
 import torch
+import warnings
 from thinc.api import get_torch_default_device
 from spacy.util import SimpleFrozenDict
 
 from ..data_classes import HFObjects
 from ..util import make_tempdir
 
 from thinc.api import PyTorchGradScaler, PyTorchShim
@@ -20,17 +21,17 @@
     def __init__(
         self,
         model: HFObjects,
         config=None,
         optimizer: Any = None,
         mixed_precision: bool = False,
         grad_scaler_config: dict = {},
-        config_cls = AutoConfig,
-        model_cls = AutoModel,
-        tokenizer_cls = AutoTokenizer,
+        config_cls=AutoConfig,
+        model_cls=AutoModel,
+        tokenizer_cls=AutoTokenizer,
     ):
         self._hfmodel = model
         self.config_cls = config_cls
         self.model_cls = model_cls
         self.tokenizer_cls = tokenizer_cls
 
         # Enable gradient scaling when mixed precision is enabled and gradient
@@ -93,15 +94,17 @@
             with make_tempdir() as temp_dir:
                 config_file = temp_dir / "config.json"
                 srsly.write_json(config_file, config_dict)
                 config = self.config_cls.from_pretrained(config_file)
                 tok_kwargs = tok_dict.pop("kwargs", {})
                 for x, x_bytes in tok_dict.items():
                     Path(temp_dir / x).write_bytes(x_bytes)
-                tokenizer = self.tokenizer_cls.from_pretrained(str(temp_dir.absolute()), **tok_kwargs)
+                tokenizer = self.tokenizer_cls.from_pretrained(
+                    str(temp_dir.absolute()), **tok_kwargs
+                )
                 vocab_file_contents = None
                 if hasattr(tokenizer, "vocab_file"):
                     vocab_file_name = tokenizer.vocab_files_names["vocab_file"]
                     vocab_file_path = str((temp_dir / vocab_file_name).absolute())
                     with open(vocab_file_path, "rb") as fileh:
                         vocab_file_contents = fileh.read()
 
@@ -113,15 +116,29 @@
                 SimpleFrozenDict(),
                 SimpleFrozenDict(),
             )
             self._model = transformer
             filelike = BytesIO(msg["state"])
             filelike.seek(0)
             device = get_torch_default_device()
-            self._model.load_state_dict(torch.load(filelike, map_location=device))
+            try:
+                self._model.load_state_dict(torch.load(filelike, map_location=device))
+            except RuntimeError as ex:
+                warn_msg = (
+                    "Error loading saved torch model. If the error is related "
+                    "to unexpected key(s) in state_dict, a possible workaround "
+                    "is to load this model with 'transformers<4.31'. "
+                    "Alternatively, download a newer compatible model or "
+                    "retrain your custom model with the current "
+                    "transformers and spacy-transformers versions. For more "
+                    "details and available updates, run: python -m spacy "
+                    "validate"
+                )
+                warnings.warn(warn_msg)
+                raise ex
             self._model.to(device)
         else:
             self._hfmodel = HFObjects(
                 None,
                 None,
                 None,
                 msg["_init_tokenizer_config"],
```

### Comparing `spacy-transformers-1.2.5/spacy_transformers/layers/hf_wrapper.py` & `spacy-transformers-1.3.0/spacy_transformers/layers/hf_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/layers/listener.py` & `spacy-transformers-1.3.0/spacy_transformers/layers/listener.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/layers/transformer_model.py` & `spacy-transformers-1.3.0/spacy_transformers/layers/transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/layers/trfs2arrays.py` & `spacy-transformers-1.3.0/spacy_transformers/layers/trfs2arrays.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/pipeline_component.py` & `spacy-transformers-1.3.0/spacy_transformers/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/span_getters.py` & `spacy-transformers-1.3.0/spacy_transformers/span_getters.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/regression/test_spacy_issue6401.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/regression/test_spacy_issue6401.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/regression/test_spacy_issue7029.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/regression/test_spacy_issue7029.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_alignment.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_configs.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_data_classes.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_model_sequence_classification.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_model_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_model_wrapper.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_pipeline_component.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_pipeline_component.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import pytest
+from packaging.version import Version
 import torch
+import spacy
 from spacy.language import Language
 from spacy.training.example import Example
 from spacy.util import make_tempdir
 from spacy.vocab import Vocab
 from spacy.tokens import Doc
 from spacy import util
 from thinc.api import Model, Config, get_current_ops, NumpyOps
@@ -191,15 +193,14 @@
     train_examples = []
     for t in TRAIN_DATA:
         train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
         for tag in t[1]["tags"]:
             tagger.add_label(tag)
 
     # Check that the Transformer component finds it listeners
-    assert transformer.listeners == []
     optimizer = nlp.initialize(lambda: train_examples)
     assert tagger_trf in transformer.listeners
 
     for i in range(2):
         losses = {}
         nlp.update(train_examples, sgd=optimizer, losses=losses)
 
@@ -488,7 +489,128 @@
     nlp.initialize(lambda: examples)
 
     transformer.update(examples)
     assert listener._backprop is not None
 
     transformer.predict(docs)
     assert listener._backprop is not None
+
+
+@pytest.mark.skipif(
+    Version(spacy.__version__) < Version("3.5.4"), reason="Bug fixed in spaCy v3.5.4"
+)
+def test_source_replace_listeners():
+    """Test that a pipeline with a transformer+tagger+senter and some replaced
+    listeners runs and trains properly"""
+    orig_config = """
+    [nlp]
+    lang = "en"
+    pipeline = ["transformer","tagger","senter"]
+
+    [components]
+
+    [components.senter]
+    factory = "senter"
+
+    [components.senter.model]
+    @architectures = "spacy.Tagger.v1"
+    nO = null
+
+    [components.senter.model.tok2vec]
+    @architectures = "spacy-transformers.TransformerListener.v1"
+    grad_factor = 1.0
+    upstream = "transformer"
+
+    [components.senter.model.tok2vec.pooling]
+    @layers = "reduce_mean.v1"
+
+    [components.tagger]
+    factory = "tagger"
+
+    [components.tagger.model]
+    @architectures = "spacy.Tagger.v1"
+    nO = null
+
+    [components.tagger.model.tok2vec]
+    @architectures = "spacy-transformers.TransformerListener.v1"
+    grad_factor = 1.0
+    upstream = "transformer"
+
+    [components.tagger.model.tok2vec.pooling]
+    @layers = "reduce_mean.v1"
+
+    [components.transformer]
+    factory = "transformer"
+
+    [components.transformer.model]
+    @architectures = "spacy-transformers.TransformerModel.v3"
+    name = "distilbert-base-uncased"
+    """
+    orig_config = Config().from_str(cfg_string)
+    nlp = util.load_model_from_config(orig_config, auto_fill=True, validate=True)
+    assert nlp.pipe_names == ["transformer", "tagger", "senter"]
+    tagger = nlp.get_pipe("tagger")
+    train_examples = []
+    for t in TRAIN_DATA:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+        for tag in t[1]["tags"]:
+            tagger.add_label(tag)
+    optimizer = nlp.initialize(lambda: train_examples)
+    assert nlp.get_pipe("transformer").listening_components == ["tagger", "senter"]
+    for i in range(2):
+        losses = {}
+        nlp.update(train_examples, sgd=optimizer, losses=losses)
+
+    with make_tempdir() as dir_path:
+        nlp.to_disk(dir_path)
+        base_model = str(dir_path)
+        new_config = {
+            "nlp": {
+                "lang": "en",
+                "pipeline": ["transformer", "tagger", "senter", "ner"],
+            },
+            "components": {
+                "transformer": {"source": base_model},
+                "tagger": {
+                    "source": base_model,
+                    "replace_listeners": ["model.tok2vec"],
+                },
+                "senter": {
+                    "source": base_model,
+                    "replace_listeners": ["model.tok2vec"],
+                },
+                "ner": {
+                    "factory": "ner",
+                    "model": {
+                        "@architectures": "spacy.TransitionBasedParser.v2",
+                        "state_type": "ner",
+                        "tok2vec": {
+                            "@architectures": "spacy-transformers.TransformerListener.v1",
+                            "grad_factor": 1.0,
+                            "upstream": "transformer",
+                            "pooling": {"@layers": "reduce_mean.v1"},
+                        },
+                    },
+                },
+            },
+        }
+        new_nlp = util.load_model_from_config(new_config, auto_fill=True)
+        for component in ("tagger", "senter"):
+            assert (
+                new_nlp.config["components"][component]["model"]["tok2vec"][
+                    "@architectures"
+                ]
+                == "spacy-transformers.Tok2VecTransformer.v3"
+            )
+        assert new_nlp.get_pipe("transformer").listening_components == ["ner"]
+
+        with make_tempdir() as new_dir_path:
+            new_nlp.to_disk(new_dir_path)
+            new_nlp_re = spacy.load(new_dir_path)
+            for component in ("tagger", "senter"):
+                assert (
+                    new_nlp.config["components"][component]["model"]["tok2vec"][
+                        "@architectures"
+                    ]
+                    == "spacy-transformers.Tok2VecTransformer.v3"
+                )
+            assert new_nlp_re.get_pipe("transformer").listening_components == ["ner"]
```

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_serialize.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_spanners.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_spanners.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_textcatcnn.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_textcatcnn.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_tok2vectransformer.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_tok2vectransformer.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/test_truncation.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/test_truncation.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/tests/util.py` & `spacy-transformers-1.3.0/spacy_transformers/tests/util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/truncate.py` & `spacy-transformers-1.3.0/spacy_transformers/truncate.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers/util.py` & `spacy-transformers-1.3.0/spacy_transformers/util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers.egg-info/PKG-INFO` & `spacy-transformers-1.3.0/spacy_transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-transformers
-Version: 1.2.5
+Version: 1.3.0
 Summary: spaCy pipelines for pre-trained BERT and other transformers
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.5 Summary: spaCy
+Metadata-Version: 2.1 Name: spacy-transformers Version: 1.3.0 Summary: spaCy
 pipelines for pre-trained BERT and other transformers Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `spacy-transformers-1.2.5/spacy_transformers.egg-info/SOURCES.txt` & `spacy-transformers-1.3.0/spacy_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers.egg-info/entry_points.txt` & `spacy-transformers-1.3.0/spacy_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.5/spacy_transformers.egg-info/requires.txt` & `spacy-transformers-1.3.0/spacy_transformers.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 spacy<4.0.0,>=3.5.0
-numpy>=1.15.0
-transformers<4.31.0,>=3.4.0
+transformers<4.32.0,>=3.4.0
 torch>=1.8.0
 srsly<3.0.0,>=2.4.0
 spacy-alignments<1.0.0,>=0.7.2
 
 [:python_version < "3.7"]
 dataclasses<1.0,>=0.6
 
+[:python_version < "3.9"]
+numpy>=1.15.0
+
+[:python_version >= "3.9"]
+numpy>=1.19.0
+
 [cuda]
 cupy>=5.0.0b4
 
 [cuda100]
 cupy-cuda100>=5.0.0b4
 
 [cuda101]
```

