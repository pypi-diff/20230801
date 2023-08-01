# Comparing `tmp/ontouml_json2graph-1.0.0b3.tar.gz` & `tmp/ontouml_json2graph-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontouml_json2graph-1.0.0b3.tar", max compression
+gzip compressed data, was "ontouml_json2graph-1.0.0b4.tar", max compression
```

## Comparing `ontouml_json2graph-1.0.0b3.tar` & `ontouml_json2graph-1.0.0b4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b3/LICENSE
--rw-r--r--   0        0        0      736 2023-08-01 18:42:41.712671 ontouml_json2graph-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     7227 2023-08-01 15:24:11.505323 ontouml_json2graph-1.0.0b3/README.md
--rw-r--r--   0        0        0        0 2023-08-01 18:18:42.034762 ontouml_json2graph-1.0.0b3/src/__init__.py
--rw-r--r--   0        0        0     4536 2023-08-01 18:04:39.977624 ontouml_json2graph-1.0.0b3/src/main.py
--rw-r--r--   0        0        0        0 2023-08-01 15:24:11.472722 ontouml_json2graph-1.0.0b3/src/modules/__init__.py
--rw-r--r--   0        0        0     4134 2023-08-01 15:24:11.474722 ontouml_json2graph-1.0.0b3/src/modules/arguments.py
--rw-r--r--   0        0        0        0 2023-08-01 15:24:11.473968 ontouml_json2graph-1.0.0b3/src/modules/decoder/__init__.py
--rw-r--r--   0        0        0     9184 2023-08-01 15:24:11.477723 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_general.py
--rw-r--r--   0        0        0     9616 2023-08-01 15:24:11.478723 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_main.py
--rw-r--r--   0        0        0    20148 2023-08-01 15:24:11.480722 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_class.py
--rw-r--r--   0        0        0     3844 2023-08-01 15:24:11.482721 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_diagram.py
--rw-r--r--   0        0        0     4473 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_elementview.py
--rw-r--r--   0        0        0     2750 2023-08-01 15:24:11.483723 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_generalization.py
--rw-r--r--   0        0        0     4661 2023-08-01 15:24:11.486723 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_generalizationset.py
--rw-r--r--   0        0        0     4502 2023-08-01 15:24:11.482721 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_package.py
--rw-r--r--   0        0        0     2593 2023-08-01 15:24:11.484721 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_path.py
--rw-r--r--   0        0        0     5467 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_project.py
--rw-r--r--   0        0        0    14058 2023-08-01 15:24:11.485722 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_property.py
--rw-r--r--   0        0        0     3223 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_rectangularshape.py
--rw-r--r--   0        0        0     6594 2023-08-01 15:24:11.488721 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_relation.py
--rw-r--r--   0        0        0     2955 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b3/src/modules/errors.py
--rw-r--r--   0        0        0      701 2023-08-01 15:24:11.485722 ontouml_json2graph-1.0.0b3/src/modules/globals.py
--rw-r--r--   0        0        0     3476 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b3/src/modules/input_output.py
--rw-r--r--   0        0        0     2642 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b3/src/modules/logger.py
--rw-r--r--   0        0        0     7258 2023-08-01 15:24:11.495722 ontouml_json2graph-1.0.0b3/src/modules/messages.py
--rw-r--r--   0        0        0      878 2023-08-01 15:24:11.492800 ontouml_json2graph-1.0.0b3/src/modules/sparql_queries.py
--rw-r--r--   0        0        0     1486 2023-08-01 15:24:11.494722 ontouml_json2graph-1.0.0b3/src/modules/utils_general.py
--rw-r--r--   0        0        0     3688 2023-08-01 15:24:11.495722 ontouml_json2graph-1.0.0b3/src/modules/utils_graph.py
--rw-r--r--   0        0        0    84660 2023-08-01 15:24:11.505721 ontouml_json2graph-1.0.0b3/src/resources/logo-json2graph.png
--rw-r--r--   0        0        0    18036 2023-08-01 15:24:11.506917 ontouml_json2graph-1.0.0b3/src/resources/ontouml_v100.ttl
--rw-r--r--   0        0        0    78196 2023-08-01 15:24:11.507721 ontouml_json2graph-1.0.0b3/src/resources/ontouml_v110.ttl
--rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b4/LICENSE
+-rw-r--r--   0        0        0      788 2023-08-01 18:58:30.114670 ontouml_json2graph-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     7227 2023-08-01 15:24:11.505323 ontouml_json2graph-1.0.0b4/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 18:18:42.034762 ontouml_json2graph-1.0.0b4/src/__init__.py
+-rw-r--r--   0        0        0     4536 2023-08-01 18:04:39.977624 ontouml_json2graph-1.0.0b4/src/main.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:24:11.472722 ontouml_json2graph-1.0.0b4/src/modules/__init__.py
+-rw-r--r--   0        0        0     4134 2023-08-01 15:24:11.474722 ontouml_json2graph-1.0.0b4/src/modules/arguments.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:24:11.473968 ontouml_json2graph-1.0.0b4/src/modules/decoder/__init__.py
+-rw-r--r--   0        0        0     9184 2023-08-01 15:24:11.477723 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_general.py
+-rw-r--r--   0        0        0     9616 2023-08-01 15:24:11.478723 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_main.py
+-rw-r--r--   0        0        0    20148 2023-08-01 15:24:11.480722 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_class.py
+-rw-r--r--   0        0        0     3844 2023-08-01 15:24:11.482721 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_diagram.py
+-rw-r--r--   0        0        0     4473 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_elementview.py
+-rw-r--r--   0        0        0     2750 2023-08-01 15:24:11.483723 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_generalization.py
+-rw-r--r--   0        0        0     4661 2023-08-01 15:24:11.486723 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_generalizationset.py
+-rw-r--r--   0        0        0     4502 2023-08-01 15:24:11.482721 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_package.py
+-rw-r--r--   0        0        0     2593 2023-08-01 15:24:11.484721 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_path.py
+-rw-r--r--   0        0        0     5467 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_project.py
+-rw-r--r--   0        0        0    14058 2023-08-01 15:24:11.485722 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_property.py
+-rw-r--r--   0        0        0     3223 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_rectangularshape.py
+-rw-r--r--   0        0        0     6594 2023-08-01 15:24:11.488721 ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_relation.py
+-rw-r--r--   0        0        0     2955 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b4/src/modules/errors.py
+-rw-r--r--   0        0        0      701 2023-08-01 15:24:11.485722 ontouml_json2graph-1.0.0b4/src/modules/globals.py
+-rw-r--r--   0        0        0     3476 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b4/src/modules/input_output.py
+-rw-r--r--   0        0        0     2642 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b4/src/modules/logger.py
+-rw-r--r--   0        0        0     7258 2023-08-01 15:24:11.495722 ontouml_json2graph-1.0.0b4/src/modules/messages.py
+-rw-r--r--   0        0        0      878 2023-08-01 15:24:11.492800 ontouml_json2graph-1.0.0b4/src/modules/sparql_queries.py
+-rw-r--r--   0        0        0     1486 2023-08-01 15:24:11.494722 ontouml_json2graph-1.0.0b4/src/modules/utils_general.py
+-rw-r--r--   0        0        0     3688 2023-08-01 15:24:11.495722 ontouml_json2graph-1.0.0b4/src/modules/utils_graph.py
+-rw-r--r--   0        0        0    84660 2023-08-01 15:24:11.505721 ontouml_json2graph-1.0.0b4/src/resources/logo-json2graph.png
+-rw-r--r--   0        0        0    18036 2023-08-01 15:24:11.506917 ontouml_json2graph-1.0.0b4/src/resources/ontouml_v100.ttl
+-rw-r--r--   0        0        0    78196 2023-08-01 15:24:11.507721 ontouml_json2graph-1.0.0b4/src/resources/ontouml_v110.ttl
+-rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b4/PKG-INFO
```

### Comparing `ontouml_json2graph-1.0.0b3/LICENSE` & `ontouml_json2graph-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/pyproject.toml` & `ontouml_json2graph-1.0.0b4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "ontouml-json2graph"
 description = "OntoUML JSON2Graph Decoder"
-version = "v1.0.0b3"
+version = "v1.0.0b4"
 authors = ["Pedro Paulo F. Barcelos <pedropaulofb@gmail.com>"]
 license = "Apache-2.0"
 keywords = ["semantic-web", "knowledge-graph", "ontouml", "ontology-driven-development", "ontouml-schema",
     "ontouml-vocabulary", "ontouml-metamodel"]
 
 homepage = "https://w3id.org/ontouml/json2graph"
 repository = "https://w3id.org/ontouml/json2graph"
 documentation = "https://w3id.org/ontouml/json2graph/docs"
 readme = "README.md"
 
 #conformsTo = "https://w3id.org/ontouml"
 #conformsToVersion = "v1.1.0"
 
-packages = [{include = "src"}]
+packages =  [   { include = "src" },
+                { include = "src/main.py"} ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ontouml_json2graph-1.0.0b3/README.md` & `ontouml_json2graph-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/main.py` & `ontouml_json2graph-1.0.0b4/src/main.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/arguments.py` & `ontouml_json2graph-1.0.0b4/src/modules/arguments.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_general.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_general.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_main.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_main.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_class.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_class.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_diagram.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_diagram.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_elementview.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_elementview.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_generalization.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_generalization.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_generalizationset.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_generalizationset.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_package.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_package.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_path.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_path.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_project.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_project.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_property.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_property.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_rectangularshape.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_rectangularshape.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_relation.py` & `ontouml_json2graph-1.0.0b4/src/modules/decoder/decode_obj_relation.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/errors.py` & `ontouml_json2graph-1.0.0b4/src/modules/errors.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/globals.py` & `ontouml_json2graph-1.0.0b4/src/modules/globals.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/input_output.py` & `ontouml_json2graph-1.0.0b4/src/modules/input_output.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/logger.py` & `ontouml_json2graph-1.0.0b4/src/modules/logger.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/messages.py` & `ontouml_json2graph-1.0.0b4/src/modules/messages.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/sparql_queries.py` & `ontouml_json2graph-1.0.0b4/src/modules/sparql_queries.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/utils_general.py` & `ontouml_json2graph-1.0.0b4/src/modules/utils_general.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/modules/utils_graph.py` & `ontouml_json2graph-1.0.0b4/src/modules/utils_graph.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/resources/logo-json2graph.png` & `ontouml_json2graph-1.0.0b4/src/resources/logo-json2graph.png`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/resources/ontouml_v100.ttl` & `ontouml_json2graph-1.0.0b4/src/resources/ontouml_v100.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/src/resources/ontouml_v110.ttl` & `ontouml_json2graph-1.0.0b4/src/resources/ontouml_v110.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b3/PKG-INFO` & `ontouml_json2graph-1.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontouml-json2graph
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: OntoUML JSON2Graph Decoder
 Home-page: https://w3id.org/ontouml/json2graph
 License: Apache-2.0
 Keywords: semantic-web,knowledge-graph,ontouml,ontology-driven-development,ontouml-schema,ontouml-vocabulary,ontouml-metamodel
 Author: Pedro Paulo F. Barcelos
 Author-email: pedropaulofb@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
```

