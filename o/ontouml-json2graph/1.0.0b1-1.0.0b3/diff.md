# Comparing `tmp/ontouml_json2graph-1.0.0b1.tar.gz` & `tmp/ontouml_json2graph-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontouml_json2graph-1.0.0b1.tar", max compression
+gzip compressed data, was "ontouml_json2graph-1.0.0b3.tar", max compression
```

## Comparing `ontouml_json2graph-1.0.0b1.tar` & `ontouml_json2graph-1.0.0b3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11558 2023-07-24 20:35:51.747413 ontouml_json2graph-1.0.0b1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-25 15:33:07.727086 ontouml_json2graph-1.0.0b1/ontouml-json2graph/__init__.py
--rw-r--r--   0        0        0     4213 2023-07-25 15:03:27.095167 ontouml_json2graph-1.0.0b1/ontouml-json2graph/main.py
--rw-r--r--   0        0        0        0 2023-07-25 14:42:55.544538 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/__init__.py
--rw-r--r--   0        0        0     3929 2023-07-25 15:02:15.606088 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/arguments.py
--rw-r--r--   0        0        0        0 2023-07-25 14:54:26.672953 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/__init__.py
--rw-r--r--   0        0        0     9194 2023-07-25 14:46:51.913772 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_general.py
--rw-r--r--   0        0        0     9422 2023-07-25 14:55:19.363219 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_main.py
--rw-r--r--   0        0        0    20166 2023-07-25 15:06:36.529526 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_class.py
--rw-r--r--   0        0        0     3790 2023-07-25 15:06:03.590107 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_diagram.py
--rw-r--r--   0        0        0     4388 2023-07-25 14:46:51.883770 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_elementview.py
--rw-r--r--   0        0        0     2731 2023-07-25 14:46:51.842772 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_generalization.py
--rw-r--r--   0        0        0     4644 2023-07-25 14:46:52.165773 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_generalizationset.py
--rw-r--r--   0        0        0     4484 2023-07-25 14:46:51.701770 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_package.py
--rw-r--r--   0        0        0     2575 2023-07-25 14:46:51.812769 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_path.py
--rw-r--r--   0        0        0     5427 2023-07-25 14:46:52.111768 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_project.py
--rw-r--r--   0        0        0    14091 2023-07-25 14:46:51.734770 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_property.py
--rw-r--r--   0        0        0     3205 2023-07-25 14:46:52.050769 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_rectangularshape.py
--rw-r--r--   0        0        0     6584 2023-07-25 14:46:51.984772 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_relation.py
--rw-r--r--   0        0        0     2948 2023-07-25 14:44:14.511883 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/errors.py
--rw-r--r--   0        0        0     1614 2023-07-24 20:35:51.760754 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/globals.py
--rw-r--r--   0        0        0     3462 2023-07-25 14:44:06.644938 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/input_output.py
--rw-r--r--   0        0        0     2642 2023-07-24 20:35:51.756565 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/logger.py
--rw-r--r--   0        0        0     7235 2023-07-25 14:47:10.955099 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/messages.py
--rw-r--r--   0        0        0      878 2023-07-24 20:35:51.764412 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/sparql_queries.py
--rw-r--r--   0        0        0     1486 2023-07-24 20:35:51.771414 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/utils_general.py
--rw-r--r--   0        0        0     3211 2023-07-25 15:04:39.709944 ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/utils_graph.py
--rw-r--r--   0        0        0    23343 2023-07-25 17:50:05.145714 ontouml_json2graph-1.0.0b1/ontouml-json2graph/poetry.lock
--rw-r--r--   0        0        0   260791 2023-07-24 20:35:51.766413 ontouml_json2graph-1.0.0b1/ontouml-json2graph/resources/Logo JSON2Graph Decoder.png
--rw-r--r--   0        0        0    18036 2023-07-24 20:35:51.763411 ontouml_json2graph-1.0.0b1/ontouml-json2graph/resources/ontouml_v100.ttl
--rw-r--r--   0        0        0    81820 2023-07-24 20:35:51.767413 ontouml_json2graph-1.0.0b1/ontouml-json2graph/resources/ontouml_v110.ttl
--rw-r--r--   0        0        0      351 2023-07-25 17:55:55.214235 ontouml_json2graph-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 15:24:11.470721 ontouml_json2graph-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0      736 2023-08-01 18:42:41.712671 ontouml_json2graph-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     7227 2023-08-01 15:24:11.505323 ontouml_json2graph-1.0.0b3/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 18:18:42.034762 ontouml_json2graph-1.0.0b3/src/__init__.py
+-rw-r--r--   0        0        0     4536 2023-08-01 18:04:39.977624 ontouml_json2graph-1.0.0b3/src/main.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:24:11.472722 ontouml_json2graph-1.0.0b3/src/modules/__init__.py
+-rw-r--r--   0        0        0     4134 2023-08-01 15:24:11.474722 ontouml_json2graph-1.0.0b3/src/modules/arguments.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:24:11.473968 ontouml_json2graph-1.0.0b3/src/modules/decoder/__init__.py
+-rw-r--r--   0        0        0     9184 2023-08-01 15:24:11.477723 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_general.py
+-rw-r--r--   0        0        0     9616 2023-08-01 15:24:11.478723 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_main.py
+-rw-r--r--   0        0        0    20148 2023-08-01 15:24:11.480722 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_class.py
+-rw-r--r--   0        0        0     3844 2023-08-01 15:24:11.482721 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_diagram.py
+-rw-r--r--   0        0        0     4473 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_elementview.py
+-rw-r--r--   0        0        0     2750 2023-08-01 15:24:11.483723 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_generalization.py
+-rw-r--r--   0        0        0     4661 2023-08-01 15:24:11.486723 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_generalizationset.py
+-rw-r--r--   0        0        0     4502 2023-08-01 15:24:11.482721 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_package.py
+-rw-r--r--   0        0        0     2593 2023-08-01 15:24:11.484721 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_path.py
+-rw-r--r--   0        0        0     5467 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_project.py
+-rw-r--r--   0        0        0    14058 2023-08-01 15:24:11.485722 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_property.py
+-rw-r--r--   0        0        0     3223 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_rectangularshape.py
+-rw-r--r--   0        0        0     6594 2023-08-01 15:24:11.488721 ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_relation.py
+-rw-r--r--   0        0        0     2955 2023-08-01 15:24:11.484866 ontouml_json2graph-1.0.0b3/src/modules/errors.py
+-rw-r--r--   0        0        0      701 2023-08-01 15:24:11.485722 ontouml_json2graph-1.0.0b3/src/modules/globals.py
+-rw-r--r--   0        0        0     3476 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b3/src/modules/input_output.py
+-rw-r--r--   0        0        0     2642 2023-08-01 15:24:11.490848 ontouml_json2graph-1.0.0b3/src/modules/logger.py
+-rw-r--r--   0        0        0     7258 2023-08-01 15:24:11.495722 ontouml_json2graph-1.0.0b3/src/modules/messages.py
+-rw-r--r--   0        0        0      878 2023-08-01 15:24:11.492800 ontouml_json2graph-1.0.0b3/src/modules/sparql_queries.py
+-rw-r--r--   0        0        0     1486 2023-08-01 15:24:11.494722 ontouml_json2graph-1.0.0b3/src/modules/utils_general.py
+-rw-r--r--   0        0        0     3688 2023-08-01 15:24:11.495722 ontouml_json2graph-1.0.0b3/src/modules/utils_graph.py
+-rw-r--r--   0        0        0    84660 2023-08-01 15:24:11.505721 ontouml_json2graph-1.0.0b3/src/resources/logo-json2graph.png
+-rw-r--r--   0        0        0    18036 2023-08-01 15:24:11.506917 ontouml_json2graph-1.0.0b3/src/resources/ontouml_v100.ttl
+-rw-r--r--   0        0        0    78196 2023-08-01 15:24:11.507721 ontouml_json2graph-1.0.0b3/src/resources/ontouml_v110.ttl
+-rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 ontouml_json2graph-1.0.0b3/PKG-INFO
```

### Comparing `ontouml_json2graph-1.0.0b1/LICENSE` & `ontouml_json2graph-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/main.py` & `ontouml_json2graph-1.0.0b3/src/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-""" Main file for ontouml-json2graph. """
+""" Main file for ontouml-json2graph.
+
+It provides a convenient interface for converting OntoUML JSON files into knowledge graphs,
+with the flexibility to customize the output and control the execution mode for different use cases.
+"""
 
 import time
 
 from rdflib import RDF
 
-from modules.arguments import ARGUMENTS
+import modules.arguments as args
 from modules.decoder.decode_main import decode_json_to_graph
-from modules.globals import SOFTWARE_NAME, SOFTWARE_VERSION, MODEL_ELEMENTS
+from modules.globals import METADATA
 from modules.input_output import safe_load_json_file, write_graph_file
 from modules.logger import initialize_logger
 from modules.utils_general import get_date_time
 
 
 def decode_ontouml_json2graph(json_path: str, graph_format: str, language: str = "",
                               execution_mode: str = "production") -> str:
@@ -26,75 +30,75 @@
     :type execution_mode: str
     :return: Saved output file path. Used for testing.
     :rtype: str
     """
 
     logger = initialize_logger(execution_mode)
 
-    print(f"{ARGUMENTS = }")
+    model_elements = ["Class", "Property", "Generalization", "GeneralizationSet", "Relation", "Cardinality"]
 
-    # Setting tests' ARGUMENTS
+    # Setting tests' arguments
     if execution_mode == "test":
-        ARGUMENTS["correct"] = True
-        ARGUMENTS["silent"] = True
-        ARGUMENTS["base_uri"] = 'https://example.org#'
-        ARGUMENTS["model_only"] = False
+        args.ARGUMENTS["correct"] = True
+        args.ARGUMENTS["silent"] = True
+        args.ARGUMENTS["base_uri"] = 'https://example.org#'
+        args.ARGUMENTS["model_only"] = False
 
-    if execution_mode == "production" and not ARGUMENTS["silent"]:
+    if execution_mode == "production" and not args.ARGUMENTS["silent"]:
         # Initial time information
         time_screen_format = "%d-%m-%Y %H:%M:%S"
         start_date_time = get_date_time(time_screen_format)
         st = time.perf_counter()
 
-        logger.info(f"{SOFTWARE_NAME} v{SOFTWARE_VERSION} started on {start_date_time}!")
-        logger.debug(f"Selected ARGUMENTS are: {ARGUMENTS}")
-        logger.info(f"Decoding JSON file {json_path} to {(ARGUMENTS['format']).upper()} graph format.\n")
+        logger.info(f"{METADATA['name']} v{METADATA['version']} started on {start_date_time}!")
+        logger.debug(f"Selected arguments are: {args.ARGUMENTS}")
+        logger.info(f"Decoding JSON file {json_path} to {(args.ARGUMENTS['format']).upper()} graph format.\n")
 
-        if not ARGUMENTS['language']:
+        if not args.ARGUMENTS['language']:
             logger.warning("Ontology's language not informed by the user. "
                            "Transformation will not generate language tag.")
-        if not ARGUMENTS['correct']:
+        if not args.ARGUMENTS['correct']:
             logger.warning("Basic correction feature not enabled by the user. "
                            "The transformation may generate an invalid result.")
 
     # Load JSON
     json_data = safe_load_json_file(json_path)
 
     # Decode JSON into Graph
     ontouml_graph = decode_json_to_graph(json_data, language, execution_mode)
 
     # If set by user, remove all diagrammatic elements
-    if ARGUMENTS["model_only"]:
+    if args.ARGUMENTS["model_only"]:
         for s, p, o in ontouml_graph.triples((None, RDF.type, None)):
             s_type = s.toPython()
             o_type = o.fragment
             # Remove if not a model element and if it is defined by of the ontology being handled
-            if (ARGUMENTS["base_uri"] in s_type) and (o_type not in MODEL_ELEMENTS):
+            if (args.ARGUMENTS["base_uri"] in s_type) and (o_type not in model_elements):
                 ontouml_graph.remove((s, None, None))
                 ontouml_graph.remove((None, None, s))
-        if not ARGUMENTS["silent"]:
+        if not args.ARGUMENTS["silent"]:
             logger.info("All diagrammatic data removed from the output. The output contains only model elements.")
 
-    if execution_mode == "production" and not ARGUMENTS["silent"]:
+    if execution_mode == "production" and not args.ARGUMENTS["silent"]:
         # Get software's execution conclusion time
         end_date_time = get_date_time(time_screen_format)
         et = time.perf_counter()
         elapsed_time = round((et - st), 3)
         logger.info(f"Decoding concluded on {end_date_time}. Total execution time: {elapsed_time} seconds.")
 
     # Save graph as specified format
     output_file_path = write_graph_file(ontouml_graph, json_path, graph_format)
     logger.info(f"Output graph file successfully saved at {output_file_path}.")
 
     return output_file_path
 
 
 if __name__ == '__main__':
-    # Treat and publish user's ARGUMENTS
-    print(f"{ARGUMENTS = }")
+    # Treat and publish user's arguments
+    args.publish_user_arguments()
 
-    json_path = ARGUMENTS["json_path"]
-    graph_format = ARGUMENTS["format"]
-    language = ARGUMENTS["language"]
+    json_path = args.ARGUMENTS["json_path"]
+    graph_format = args.ARGUMENTS["format"]
+    language = args.ARGUMENTS["language"]
 
     # Execute the transformation
     decode_ontouml_json2graph(json_path, graph_format, language, "production")
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/arguments.py` & `ontouml_json2graph-1.0.0b3/src/modules/arguments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 """ Argument Treatments """
 
 import argparse
 
 import validators as validators
 
-from .globals import SOFTWARE_ACRONYM, SOFTWARE_VERSION, SOFTWARE_NAME, SOFTWARE_URL, ALLOWED_GRAPH_FORMATS
-from .logger import initialize_logger
+from modules.globals import METADATA
+from modules.logger import initialize_logger
 
 LOGGER = initialize_logger()
+ARGUMENTS = {}
 
 
 def treat_user_arguments() -> dict:
     """ Treat arguments provided by the user when starting software execution.
 
     :return: Dictionary with json path (key 'json_path') and final file format (key 'format').
     :rtype: dict
     :raises OSError: If provided input is not of JSON type.
     """
 
+    # Formats for saving graphs supported by RDFLib
+    # https://rdflib.readthedocs.io/en/stable/intro_to_parsing.html#saving-rdf
+    allowed_graph_formats = ["turtle", "ttl", "turtle2", "xml", "pretty-xml", "json-ld", "ntriples", "nt", "nt11", "n3",
+                             "trig", "trix", "nquads"]
+
     LOGGER.debug("Parsing user's arguments...")
 
-    about_message = SOFTWARE_ACRONYM + " - version " + SOFTWARE_VERSION
+    about_message = METADATA["name"] + " - version " + METADATA["version"]
 
     # PARSING ARGUMENTS
-    arguments_parser = argparse.ArgumentParser(prog=SOFTWARE_ACRONYM,
-                                               description=SOFTWARE_NAME + ". Version: " + SOFTWARE_VERSION,
-                                               allow_abbrev=False, epilog="More information at: " + SOFTWARE_URL)
+    args_parser = argparse.ArgumentParser(prog=METADATA["name"],
+                                          description=METADATA["description"] + ". Version: " + METADATA["version"],
+                                          allow_abbrev=False, epilog="More information at: " + METADATA["repository"])
 
-    arguments_parser.version = about_message
+    args_parser.version = about_message
 
     # POSITIONAL ARGUMENT
-    arguments_parser.add_argument("json_file", type=str, action="store",
-                                  help="The path of the JSON file to be encoded.")
+    args_parser.add_argument("json_file", type=str, action="store",
+                             help="The path of the JSON file to be encoded.")
 
     # OPTIONAL ARGUMENT
-    arguments_parser.add_argument("-f", "--format", action="store", choices=ALLOWED_GRAPH_FORMATS, default="ttl",
-                                  help="Format to save the decoded file. Default is 'ttl'.")
-    arguments_parser.add_argument("-l", "--language", action="store", type=str, default="",
-                                  help="Language tag for the ontology's concepts. Default is 'None'.")
-    arguments_parser.add_argument("-c", "--correct", action="store_true",
-                                  help="Enables syntactical and semantic validations and corrections.")
-    arguments_parser.add_argument("-s", "--silent", action="store_true",
-                                  help="Silent mode. Does not present validation warnings and errors.")
-    arguments_parser.add_argument("-u", "--base_uri", action="store", type=str, default="https://example.org#",
-                                  help="Base URI of the resulting graph. Default is 'https://example.org#'.")
-    arguments_parser.add_argument("-m", "--model_only", action="store_true",
-                                  help="Keep only model elements, eliminating all diagrammatic data from output.")
+    args_parser.add_argument("-f", "--format", action="store", choices=allowed_graph_formats, default="ttl",
+                             help="Format to save the decoded file. Default is 'ttl'.")
+    args_parser.add_argument("-l", "--language", action="store", type=str, default="",
+                             help="Language tag for the ontology's concepts. Default is 'None'.")
+    args_parser.add_argument("-c", "--correct", action="store_true",
+                             help="Enables syntactical and semantic validations and corrections.")
+    args_parser.add_argument("-s", "--silent", action="store_true",
+                             help="Silent mode. Does not present validation warnings and errors.")
+    args_parser.add_argument("-u", "--base_uri", action="store", type=str, default="https://example.org#",
+                             help="Base URI of the resulting graph. Default is 'https://example.org#'.")
+    args_parser.add_argument("-m", "--model_only", action="store_true",
+                             help="Keep only model elements, eliminating all diagrammatic data from output.")
 
     # AUTOMATIC ARGUMENTS
-    arguments_parser.add_argument("-v", "--version", action="version", help="Print the software version and exit.")
+    args_parser.add_argument("-v", "--version", action="version", help="Print the software version and exit.")
 
     # Execute arguments parser
-    arguments = arguments_parser.parse_args()
+    arguments = args_parser.parse_args()
 
     # Asserting dictionary keys
     arguments_dictionary = {"format": arguments.format,
                             "language": arguments.language,
                             "correct": arguments.correct,
                             "silent": arguments.silent,
                             "json_path": arguments.json_file,
@@ -73,11 +79,11 @@
         arguments_dictionary["base_uri"] += '#'
 
     LOGGER.debug(f"Arguments parsed. Obtained values are: {arguments_dictionary}.")
 
     return arguments_dictionary
 
 
-global ARGUMENTS
-arguments_dictionary = treat_user_arguments()
-ARGUMENTS = arguments_dictionary
-print(f"args {ARGUMENTS = }")
+def publish_user_arguments():
+    arguments_dictionary = treat_user_arguments()
+    global ARGUMENTS
+    ARGUMENTS = arguments_dictionary
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_general.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """ General decoding functions. """
 
 from rdflib import Graph, URIRef, Literal, RDF
 
-from ..arguments import ARGUMENTS as args
-from ..globals import URI_ONTOUML
-from ..logger import initialize_logger
-from ..sparql_queries import GET_ELEMENT_AND_TYPE
-from ..utils_graph import load_ontouml_vocabulary
+import modules.arguments as args
+from modules.logger import initialize_logger
+from modules.sparql_queries import GET_ELEMENT_AND_TYPE
+from modules.utils_graph import load_ontouml_vocabulary, ontouml_ref
 
 LOGGER = initialize_logger()
 
 
 def create_point(point_id: str, x_coord: int, y_coord: int, ontouml_graph: Graph) -> None:
     """ Creates a new instance of ontouml:Point with its ontouml:xCoordinate, and ontouml:yCoordinate properties.
 
@@ -20,24 +19,24 @@
     :type x_coord: int
     :param y_coord: Vertical coordinate of the new ontouml:Point.
     :type y_coord: int
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    ontouml_graph.add((URIRef(args["base_uri"] + point_id), RDF.type, URIRef(URI_ONTOUML + "Point")))
+    ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + point_id), RDF.type, ontouml_ref("Point")))
 
     # Setting x coordinate
-    ontouml_graph.add((URIRef(args["base_uri"] + point_id),
-                       URIRef(URI_ONTOUML + "xCoordinate"),
+    ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + point_id),
+                       ontouml_ref("xCoordinate"),
                        Literal(x_coord)))
 
     # Setting y coordinate
-    ontouml_graph.add((URIRef(args["base_uri"] + point_id),
-                       URIRef(URI_ONTOUML + "yCoordinate"),
+    ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + point_id),
+                       ontouml_ref("yCoordinate"),
                        Literal(y_coord)))
 
 
 def count_elements_graph(ontouml_graph: Graph) -> dict:
     """ Returns a dictionary with all element types on graphs and their respective quantity.
 
     :param ontouml_graph: Knowledge graph with loaded objects' ids and types
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_main.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """ JSON decode functions."""
 
 from rdflib import Graph, URIRef, Literal, RDF, XSD, OWL, RDFS
 
-from ..arguments import ARGUMENTS
-from .decode_general import clean_null_data, count_elements_graph
-from .decode_obj_class import create_class_properties
-from .decode_obj_diagram import create_diagram_properties
-from .decode_obj_elementview import create_elementview_properties
-from .decode_obj_generalization import create_generalization_properties
-from .decode_obj_generalizationset import create_generalizationset_properties
-from .decode_obj_package import create_package_properties
-from .decode_obj_path import create_path_properties
-from .decode_obj_project import create_project_properties
-from .decode_obj_property import create_property_properties
-from .decode_obj_rectangularshape import create_rectangularshape_properties
-from .decode_obj_relation import create_relation_properties
-from ..globals import URI_ONTOUML, ELEMENT_VIEW_TYPES, SOFTWARE_NAME, SOFTWARE_VERSION, SOFTWARE_URL, \
-    CONFORMS_TO_VOCAB_VERSION
-from ..logger import initialize_logger
-from ..utils_general import get_date_time
+import modules.arguments as args
+from modules.decoder.decode_general import clean_null_data, count_elements_graph
+from modules.decoder.decode_obj_class import create_class_properties
+from modules.decoder.decode_obj_diagram import create_diagram_properties
+from modules.decoder.decode_obj_elementview import create_elementview_properties
+from modules.decoder.decode_obj_generalization import create_generalization_properties
+from modules.decoder.decode_obj_generalizationset import create_generalizationset_properties
+from modules.decoder.decode_obj_package import create_package_properties
+from modules.decoder.decode_obj_path import create_path_properties
+from modules.decoder.decode_obj_project import create_project_properties
+from modules.decoder.decode_obj_property import create_property_properties
+from modules.decoder.decode_obj_rectangularshape import create_rectangularshape_properties
+from modules.decoder.decode_obj_relation import create_relation_properties
+from modules.globals import URI_ONTOUML, ELEMENT_VIEW_TYPES, METADATA
+from modules.logger import initialize_logger
+from modules.utils_general import get_date_time
+from modules.utils_graph import ontouml_ref
 
 LOGGER = initialize_logger()
 
 
 def add_metadata(ontouml_graph: Graph) -> None:
     """ Adds basic metadata to the generated graph when not in test mode. The metadata added are:
         - dct:conformsTo URI_ONTOUML
@@ -33,41 +33,41 @@
 
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     uri_dct = "http://purl.org/dc/terms/"
     ontouml_graph.bind("dct", uri_dct)
-    uriref_ontology = URIRef(ARGUMENTS["base_uri"][:-1])
+    uriref_ontology = URIRef(args.ARGUMENTS["base_uri"][:-1])
 
     # Adding conforms to
     dct_conforms_to = URIRef(uri_dct + "conformsTo")
-    vocab_uri = URIRef(URI_ONTOUML[:-1])
+    vocab_uri = URIRef(METADATA['conformsTo'])
     ontouml_graph.add((uriref_ontology, dct_conforms_to, vocab_uri))
-    ontouml_graph.add((uriref_ontology, dct_conforms_to, vocab_uri + "/vocabulary/v" + CONFORMS_TO_VOCAB_VERSION))
+    ontouml_graph.add((uriref_ontology, dct_conforms_to, vocab_uri + "/vocabulary/" + METADATA['conformsToVersion']))
 
     # Adding creation date
     date_format = "%Y-%m-%d"
     created_date = get_date_time(date_format)
     dct_created = URIRef(uri_dct + "created")
     ontouml_graph.add((uriref_ontology, dct_created, Literal(created_date, datatype=XSD.date)))
 
     # Adding language
-    if ARGUMENTS["language"]:
+    if args.ARGUMENTS["language"]:
         dct_language = URIRef(uri_dct + "language")
         language_uri = "http://dbpedia.org/resource/ISO_639:"
-        ontouml_graph.add((uriref_ontology, dct_language, URIRef(language_uri + ARGUMENTS["language"])))
+        ontouml_graph.add((uriref_ontology, dct_language, URIRef(language_uri + args.ARGUMENTS["language"])))
 
     # Adding type
     ontouml_graph.add((uriref_ontology, RDF.type, OWL.Ontology))
 
     # Adding generator information
-    comment_message = f"Generated by {SOFTWARE_NAME} v{SOFTWARE_VERSION}"
+    comment_message = f"Generated by {METADATA['name']} v{METADATA['version']}"
     ontouml_graph.add((uriref_ontology, RDFS.comment, Literal(comment_message)))
-    ontouml_graph.add((uriref_ontology, RDFS.seeAlso, Literal(SOFTWARE_URL, datatype=XSD.anyURI)))
+    ontouml_graph.add((uriref_ontology, RDFS.seeAlso, Literal(METADATA['repository'], datatype=XSD.anyURI)))
 
 
 def decode_dictionary(dictionary_data: dict, ontouml_graph: Graph, language: str) -> None:
     """ Receives the full dictionary with the loaded JSON data and decode known allowed values to the OntoUML Graph.
     Recursively evaluates the dictionary to create all possible instances, setting their types and attributes.
 
     OntoUML-Vocabulary properties that are directly decoded in the general decoder:
@@ -89,19 +89,19 @@
     mapped_fields = {"value": "text"}
 
     # Treating Path sub dictionaries
     if "id" not in dictionary_data:
         return
 
     # Creating instance
-    instance_uri = ARGUMENTS["base_uri"] + dictionary_data["id"]
+    instance_uri = args.ARGUMENTS["base_uri"] + dictionary_data["id"]
     new_instance = URIRef(instance_uri)
 
     # Setting instance type
-    instance_type = URIRef(URI_ONTOUML + dictionary_data["type"])
+    instance_type = ontouml_ref(dictionary_data["type"])
     ontouml_graph.add((new_instance, RDF.type, instance_type))
 
     # Adding other attributes
     for key in dictionary_data.keys():
 
         # if id or type was already treated, skip
         if key == "id" or key == "type":
@@ -122,17 +122,17 @@
         if type(dictionary_data[key]) is dict:
             decode_dictionary(dictionary_data[key], ontouml_graph, language)
             continue
 
         # Graph's PREDICATE definition
         # May be direct or mapped
         if key not in mapped_fields.keys():
-            new_predicate = URIRef(URI_ONTOUML + key)
+            new_predicate = ontouml_ref(key)
         else:
-            new_predicate = URIRef(URI_ONTOUML + mapped_fields[key])
+            new_predicate = ontouml_ref(mapped_fields[key])
 
         # Graph's OBJECT definition
         if (key == "name") and language != "":
             new_object = Literal(dictionary_data[key], lang=language)
         elif key in positive_integer_fields:
             # Checking if is not integer (as int or as string)
             if type(dictionary_data[key]) is not int:
@@ -161,15 +161,15 @@
     :return: Knowledge graph that complies with the OntoUML Vocabulary
     :rtype: Graph
     """
 
     # Creating OntoUML Graph
     ontouml_graph = Graph()
     ontouml_graph.bind("ontouml", URI_ONTOUML)
-    ontouml_graph.bind("", ARGUMENTS["base_uri"])
+    ontouml_graph.bind("", args.ARGUMENTS["base_uri"])
 
     # Get clean data
     # Dictionary data is all the JSON data loaded as a dictionary to be manipulated
     dictionary_data = clean_null_data(json_data)
 
     # GENERAL DECODING: creating all instances and setting their types.
     decode_dictionary(dictionary_data, ontouml_graph, language)
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_class.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     - Functions that set both object and data properties are named: set_<subject>_properties.
 """
 
 import inspect
 
 from rdflib import Graph, URIRef, XSD, Literal
 
-from ..arguments import ARGUMENTS
-from .decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
-from ..errors import report_error_end_of_switch
-from ..globals import URI_ONTOUML
-from ..messages import print_decode_log_message
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
+from modules.errors import report_error_end_of_switch
+from modules.messages import print_decode_log_message
+from modules.utils_graph import ontouml_ref
 
 
 def validate_class_attribute_constraints(class_dict: dict) -> None:
     """ Verifies all Class dictionaries and check if the constraints related to classes were correctly considered and
     fixes them when they are not.
 
     The pair of attribute/stereotype: isExtensional/collective and isPowertype/type checked constraints are:
@@ -30,15 +30,15 @@
     VCA3a) If class has stereotype different from 'collective' and isExtensional is not null, remove isExtensional.
     VCA3b) If class has stereotype different from 'type' and isPowertype is True, set isPowertype as False.
 
     :param class_dict: Class object loaded as a dictionary.
     :type class_dict: dict
     """
 
-    if not ARGUMENTS["correct"]:
+    if not args.ARGUMENTS["correct"]:
         return
 
     class_stereotype = get_stereotype(class_dict)
 
     # VCA1: Reports Class different from 'type' with isExtensional value not null and isPowertype value True.
     if (class_stereotype != 'type') and ("isExtensional" in class_dict) and ("isPowertype" in class_dict):
         if class_dict["isPowertype"]:
@@ -78,15 +78,15 @@
 
     The above codes are used to display warning/error messages when necessary.
 
     :param class_dict: Class object loaded as a dictionary.
     :type class_dict: dict
     """
 
-    if not ARGUMENTS["correct"]:
+    if not args.ARGUMENTS["correct"]:
         return
 
     class_stereotype = get_stereotype(class_dict)
 
     # Constraints VCO1 and VCO2 depend on the existence of the order attribute
     if "order" in class_dict:
 
@@ -117,36 +117,36 @@
     """
 
     class_stereotype = get_stereotype(class_dict)
 
     # DCA1: Setting ontouml:isExtensional default value to False when it's not set in a class with stereotype collective
     if "isExtensional" not in class_dict and class_stereotype == "collective":
         print_decode_log_message(class_dict, "DCA1", property_name='isExtensional', att_valid_stereotype='collective')
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isExtensional"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("isExtensional"), Literal(False, datatype=XSD.boolean)))
 
     # DCA2, DCA3, and DCA4 use the same message DGA1, as they are not associated to their holder's stereotype
 
     # DCA2: Setting ontouml:isPowertype attribute default value
     if "isPowertype" not in class_dict:
         print_decode_log_message(class_dict, "DGA1", property_name='isPowertype')
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isPowertype"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("isPowertype"), Literal(False, datatype=XSD.boolean)))
 
     # DCA3: Setting ontouml:isDerived attribute default value
     if "isDerived" not in class_dict:
         print_decode_log_message(class_dict, "DGA1", property_name='isDerived')
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isDerived"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("isDerived"), Literal(False, datatype=XSD.boolean)))
 
     # DCA4: Setting ontouml:isAbstract attribute default value
     if "isAbstract" not in class_dict:
         print_decode_log_message(class_dict, "DGA1", property_name='isAbstract')
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isAbstract"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("isAbstract"), Literal(False, datatype=XSD.boolean)))
 
 
 def set_defaults_class_order(class_dict: dict, ontouml_graph: Graph) -> None:
     """ Verifies a class dictionary and check if their non-nullable attribute order was set or not.
     If not, creates default values.
 
     Default values checked are:
@@ -166,22 +166,22 @@
 
     # Setting ORDER attribute default value. Do nothing if the stereotype is unknown.
     if ("order" not in class_dict) and (class_stereotype != 'null'):
 
         # DCO1: 'order' default value = 1 when stereotype is not 'type'
         if class_stereotype != 'type':
             print_decode_log_message(class_dict, "DCO1", property_name='order')
-            ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                               URIRef(URI_ONTOUML + "order"), Literal(1, datatype=XSD.nonNegativeInteger)))
+            ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                               ontouml_ref("order"), Literal(1, datatype=XSD.nonNegativeInteger)))
 
         # DCO2: 'order' default value = 2 when stereotype is 'type'
         elif class_stereotype == 'type':
             print_decode_log_message(class_dict, "DCO2", property_name='order')
-            ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                               URIRef(URI_ONTOUML + "order"), Literal(2, datatype=XSD.nonNegativeInteger)))
+            ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                               ontouml_ref("order"), Literal(2, datatype=XSD.nonNegativeInteger)))
 
         # Unexpected value received for class_stereotype
         else:
             current_function = inspect.stack()[0][3]
             report_error_end_of_switch("class_stereotype", current_function)
 
 
@@ -206,17 +206,17 @@
     class_stereotype = get_stereotype(class_dict)
     class_type = class_dict["type"]
 
     # If stereotype not declared, report warning.
     if class_stereotype == "null":
         print_decode_log_message(class_dict, "VCS1", "stereotype")
     else:
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "stereotype"),
-                           URIRef(URI_ONTOUML + class_dict['stereotype'])))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("stereotype"),
+                           ontouml_ref(class_dict['stereotype'])))
 
         # If declared but invalid, create and report error. Uses generic message with code 'VCSG'.
         if class_stereotype not in ENUM_CLASS_STEREOTYPE:
             print_decode_log_message(class_dict, "VCSG", property_name="stereotype")
 
 
 def set_class_order_nonnegativeinteger(class_dict: dict, ontouml_graph: Graph) -> None:
@@ -235,26 +235,26 @@
 
     # Case A: if 'order' field is null, it will receive the default value (see function set_class_defaults)
     if "order" not in class_dict:
         return
 
     # Case C: receives 0, representing an orderless class.
     elif class_dict["order"] == "*":
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "order"),
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("order"),
                            Literal(0, datatype=XSD.nonNegativeInteger)))
 
     # Case A: remove invalid information so the field can be treated as null and then receive the default value.
     elif (type(class_dict["order"]) is int) and (class_dict["order"] <= 0):
         class_dict.pop("order")
 
     # Case B
     elif type(class_dict["order"]):
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "order"),
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("order"),
                            Literal(class_dict['order'], datatype=XSD.nonNegativeInteger)))
 
     # Case A: remove invalid information so the field can be treated as null and then receive the default value.
     else:
         class_dict.pop("order")
 
 
@@ -280,17 +280,17 @@
         "situation": "situationNature",
         "type": "typeNature"
     }
 
     if "restrictedTo" in class_dict:
 
         for restriction in class_dict["restrictedTo"]:
-            ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                               URIRef(URI_ONTOUML + "restrictedTo"),
-                               URIRef(URI_ONTOUML + restriction_nature_mapping[restriction])))
+            ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                               ontouml_ref("restrictedTo"),
+                               ontouml_ref(restriction_nature_mapping[restriction])))
 
 
 def set_class_attributes(class_dict: dict, ontouml_graph: Graph) -> None:
     """ Defines the ontouml:isPowertype and ontouml:isExtensional data properties of an ontouml:Class in the graph.
 
     This function must be called after the function set_class_defaults, as the received value may change because of
     identified problems.
@@ -298,21 +298,21 @@
     :param class_dict: Class object loaded as a dictionary.
     :type class_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     if "isExtensional" in class_dict:
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isExtensional"),
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("isExtensional"),
                            Literal(class_dict["isExtensional"], datatype=XSD.boolean)))
 
     if "isPowertype" in class_dict:
-        ontouml_graph.add((URIRef(ARGUMENTS["base_uri"] + class_dict['id']),
-                           URIRef(URI_ONTOUML + "isPowertype"),
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_dict['id']),
+                           ontouml_ref("isPowertype"),
                            Literal(class_dict["isPowertype"], datatype=XSD.boolean)))
 
 
 def set_class_attribute_property(class_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets ontouml:attribute relation between an ontouml:Class and an ontouml:Property.
 
     :param class_dict: Class object loaded as a dictionary.
@@ -320,17 +320,17 @@
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     list_related_properties = get_list_subdictionaries_for_specific_type(class_dict, "Property")
 
     for related_property in list_related_properties:
-        statement_subject = URIRef(ARGUMENTS["base_uri"] + class_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "attribute")
-        statement_object = URIRef(ARGUMENTS["base_uri"] + related_property["id"])
+        statement_subject = URIRef(args.ARGUMENTS["base_uri"] + class_dict["id"])
+        statement_predicate = ontouml_ref("attribute")
+        statement_object = URIRef(args.ARGUMENTS["base_uri"] + related_property["id"])
 
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def set_class_literal_literal(class_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets ontouml:literal relation between an ontouml:Class and its related ontouml:Literal individuals.
 
@@ -339,17 +339,17 @@
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     list_related_literals = get_list_subdictionaries_for_specific_type(class_dict, "Literal")
 
     for related_literal in list_related_literals:
-        statement_subject = URIRef(ARGUMENTS["base_uri"] + class_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "literal")
-        statement_object = URIRef(ARGUMENTS["base_uri"] + related_literal["id"])
+        statement_subject = URIRef(args.ARGUMENTS["base_uri"] + class_dict["id"])
+        statement_predicate = ontouml_ref("literal")
+        statement_object = URIRef(args.ARGUMENTS["base_uri"] + related_literal["id"])
 
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def create_class_properties(json_data: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Main function for decoding an object of type 'Class'.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_diagram.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_diagram.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,31 +6,32 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-from ..arguments import ARGUMENTS
-from .decode_general import get_list_subdictionaries_for_specific_type
-from ..globals import URI_ONTOUML, ELEMENT_VIEW_TYPES
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
+from modules.globals import ELEMENT_VIEW_TYPES
+from modules.utils_graph import ontouml_ref
 
 
 def set_diagram_owner_modelelement(diagram_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:owner property between an ontouml:Diagram and its related ontouml:Package.
 
     :param diagram_dict: Diagram object loaded as a dictionary.
     :type diagram_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    statement_subject = URIRef(ARGUMENTS["base_uri"] + diagram_dict["id"])
-    statement_predicate = URIRef(URI_ONTOUML + "owner")
-    statement_object = URIRef(ARGUMENTS["base_uri"] + diagram_dict["owner"]["id"])
+    statement_subject = URIRef(args.ARGUMENTS["base_uri"] + diagram_dict["id"])
+    statement_predicate = ontouml_ref("owner")
+    statement_object = URIRef(args.ARGUMENTS["base_uri"] + diagram_dict["owner"]["id"])
     ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def set_diagram_containsview_elementview(diagram_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:containsView property between an ontouml:Diagram and its related ontouml:ElementView.
 
     :param diagram_dict: Diagram object loaded as a dictionary.
@@ -41,17 +42,17 @@
 
     list_related_elementviews = []
 
     for view_type in ELEMENT_VIEW_TYPES:
         list_related_elementviews += get_list_subdictionaries_for_specific_type(diagram_dict, view_type)
 
     for related_elementview in list_related_elementviews:
-        statement_subject = URIRef(ARGUMENTS["base_uri"] + diagram_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "containsView")
-        statement_object = URIRef(ARGUMENTS["base_uri"] + related_elementview["id"])
+        statement_subject = URIRef(args.ARGUMENTS["base_uri"] + diagram_dict["id"])
+        statement_predicate = ontouml_ref("containsView")
+        statement_object = URIRef(args.ARGUMENTS["base_uri"] + related_elementview["id"])
 
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def create_diagram_properties(json_data: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Main function for decoding objects of type 'Diagram'.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_elementview.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_elementview.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,19 @@
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 import inspect
 
 from rdflib import Graph, URIRef
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
-from ..errors import report_error_end_of_switch
-from ..globals import URI_ONTOUML, ELEMENT_VIEW_TYPES
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
+from modules.errors import report_error_end_of_switch
+from modules.globals import ELEMENT_VIEW_TYPES
+from modules.utils_graph import ontouml_ref
 
 
 def set_elementview_relations(elementview_dict: dict, ontouml_graph: Graph) -> None:
     """ Set an ontouml:ElementView's ontouml:shape and ontouml:isViewOf object properties in the resulting graph.
 
     :param elementview_dict: ElementView object loaded as a dictionary.
     :type elementview_dict: dict
@@ -35,34 +36,34 @@
     elif elementview_dict["shape"]["type"] == 'Path':
         shape_name += "_path"
     else:
         current_function = inspect.stack()[0][3]
         report_error_end_of_switch("classview_dict['shape']['type']", current_function)
 
     # Setting shape property
-    ontouml_graph.add((URIRef(args["base_uri"] + elementview_dict['id']),
-                       URIRef(URI_ONTOUML + "shape"),
-                       URIRef(args["base_uri"] + shape_name)))
+    ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['id']),
+                       ontouml_ref("shape"),
+                       URIRef(args.ARGUMENTS["base_uri"] + shape_name)))
 
     # Setting isViewOf property
     if "modelElement" in elementview_dict:
-        ontouml_graph.add((URIRef(args["base_uri"] + elementview_dict['id']),
-                           URIRef(URI_ONTOUML + "isViewOf"),
-                           URIRef(args["base_uri"] + elementview_dict['modelElement']['id'])))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['id']),
+                           ontouml_ref("isViewOf"),
+                           URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['modelElement']['id'])))
 
     # Setting sourceView and targetView properties
     if "source" in elementview_dict:
-        ontouml_graph.add((URIRef(args["base_uri"] + elementview_dict['id']),
-                           URIRef(URI_ONTOUML + "sourceView"),
-                           URIRef(args["base_uri"] + elementview_dict['source']['id'])))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['id']),
+                           ontouml_ref("sourceView"),
+                           URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['source']['id'])))
 
     if "target" in elementview_dict:
-        ontouml_graph.add((URIRef(args["base_uri"] + elementview_dict['id']),
-                           URIRef(URI_ONTOUML + "targetView"),
-                           URIRef(args["base_uri"] + elementview_dict['target']['id'])))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['id']),
+                           ontouml_ref("targetView"),
+                           URIRef(args.ARGUMENTS["base_uri"] + elementview_dict['target']['id'])))
 
 
 def create_elementview_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type ElementView.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
     object's type is domain of.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_generalization.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_generalization.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,34 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
-from ..globals import URI_ONTOUML
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
+from modules.utils_graph import ontouml_ref
 
 
 def set_generalization_relations(generalization_dict: dict, ontouml_graph: Graph) -> None:
     """ Set the ontouml:general and ontouml:specific properties in the resulting graph.
 
     :param generalization_dict: Generalization object loaded as a dictionary.
     :type generalization_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    generalization_individual = URIRef(args["base_uri"] + generalization_dict['id'])
-    general_individual = URIRef(args["base_uri"] + generalization_dict["general"]['id'])
-    specific_individual = URIRef(args["base_uri"] + generalization_dict["specific"]['id'])
+    generalization_individual = URIRef(args.ARGUMENTS["base_uri"] + generalization_dict['id'])
+    general_individual = URIRef(args.ARGUMENTS["base_uri"] + generalization_dict["general"]['id'])
+    specific_individual = URIRef(args.ARGUMENTS["base_uri"] + generalization_dict["specific"]['id'])
 
-    ontouml_graph.add((generalization_individual, URIRef(URI_ONTOUML + "general"), general_individual))
-    ontouml_graph.add((generalization_individual, URIRef(URI_ONTOUML + "specific"), specific_individual))
+    ontouml_graph.add((generalization_individual, ontouml_ref("general"), general_individual))
+    ontouml_graph.add((generalization_individual, ontouml_ref("specific"), specific_individual))
 
 
 def create_generalization_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type Generalization.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
     object's type is domain of.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_generalizationset.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_generalizationset.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,67 +6,67 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef, Literal, XSD
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
-from ..globals import URI_ONTOUML
-from ..messages import print_decode_log_message
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
+from modules.messages import print_decode_log_message
+from modules.utils_graph import ontouml_ref
 
 
 def set_generalizationset_defaults(generalizationset_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the default values to ontouml:generalizationSets to the resulting graph.
 
     - Default isDisjoint: If isDisjoint is null, set as False.
     - Default isComplete: If isComplete is null, set as False.
 
     :param generalizationset_dict: GeneralizationSet object loaded as a dictionary.
     :type generalizationset_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    generalizationset_individual = URIRef(args["base_uri"] + generalizationset_dict['id'])
+    generalizationset_individual = URIRef(args.ARGUMENTS["base_uri"] + generalizationset_dict['id'])
     set_false = Literal(False, datatype=XSD.boolean)
 
     if "isDisjoint" not in generalizationset_dict:
         print_decode_log_message(generalizationset_dict, "DGA1", property_name="isDisjoint")
-        is_disjoint_property = URIRef(URI_ONTOUML + "isDisjoint")
+        is_disjoint_property = ontouml_ref("isDisjoint")
         ontouml_graph.add((generalizationset_individual, is_disjoint_property, set_false))
 
     if "isComplete" not in generalizationset_dict:
         print_decode_log_message(generalizationset_dict, "DGA1", property_name="isComplete")
-        is_complete_property = URIRef(URI_ONTOUML + "isComplete")
+        is_complete_property = ontouml_ref("isComplete")
         ontouml_graph.add((generalizationset_individual, is_complete_property, set_false))
 
 
 def set_generalizationset_relations(generalizationset_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the ontouml:generalization and ontouml:categorizer property to the resulting graph.
 
     :param generalizationset_dict: GeneralizationSet object loaded as a dictionary.
     :type generalizationset_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    generalizationset_individual = URIRef(args["base_uri"] + generalizationset_dict['id'])
-    generalization_property = URIRef(URI_ONTOUML + "generalization")
-    categorizer_property = URIRef(URI_ONTOUML + "categorizer")
+    generalizationset_individual = URIRef(args.ARGUMENTS["base_uri"] + generalizationset_dict['id'])
+    generalization_property = ontouml_ref("generalization")
+    categorizer_property = ontouml_ref("categorizer")
 
     # Setting ontouml:generalization property
     for generalization_dict in generalizationset_dict["generalizations"]:
-        generalization_individual = URIRef(args["base_uri"] + generalization_dict["id"])
+        generalization_individual = URIRef(args.ARGUMENTS["base_uri"] + generalization_dict["id"])
         ontouml_graph.add((generalizationset_individual, generalization_property, generalization_individual))
 
     # Setting ontouml:categorizer property
     if "categorizer" in generalizationset_dict:
-        categorizer_individual = URIRef(args["base_uri"] + generalizationset_dict["categorizer"]["id"])
+        categorizer_individual = URIRef(args.ARGUMENTS["base_uri"] + generalizationset_dict["categorizer"]["id"])
         ontouml_graph.add((generalizationset_individual, categorizer_property, categorizer_individual))
 
 
 def create_generalizationset_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type GeneralizationSet.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_package.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_package.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
-from ..globals import URI_ONTOUML
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
+from modules.utils_graph import ontouml_ref
 
 
 def get_package_contents(package_dict: dict, package_id: str, list_contents: list = []) -> list[dict]:
     """ Receives the dictionary with all loaded JSON data and returns the value of the 'contents' field for a given
     object (defined by the received value of its ID).
 
     :param package_dict: Package's data to have its fields decoded.
@@ -79,17 +79,17 @@
         # Create a list of all ids inside the returned list
         list_related_ids = []
         for content in package_id_contents_list:
             list_related_ids.append(content["id"])
 
         # Include found related elements in graph using ontouml:containsModelElement
         for related_id in list_related_ids:
-            ontouml_graph.add((URIRef(args["base_uri"] + package_dict["id"]),
-                               URIRef(URI_ONTOUML + "containsModelElement"),
-                               URIRef(args["base_uri"] + related_id)))
+            ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + package_dict["id"]),
+                               ontouml_ref("containsModelElement"),
+                               URIRef(args.ARGUMENTS["base_uri"] + related_id)))
 
 
 def create_package_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type Package.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
     object's type is domain of.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_path.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_path.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
-from ..globals import URI_ONTOUML
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
+from modules.utils_graph import ontouml_ref
 
 
 def set_path_path_point(path_dict: dict, ontouml_graph: Graph) -> None:
     """ Creates an ontouml:Point, their properties and the ontouml:point of an ontouml:Path.
 
     :param path_dict: Path object loaded as a dictionary.
     :type path_dict: dict
@@ -29,17 +29,17 @@
 
     for point_dict in path_dict["points"]:
         # Creating new Point instance
         point_name = base_point_name + str(point_counter)
         create_point(point_name, point_dict["x"], point_dict["y"], ontouml_graph)
 
         # Associating new Point with the Path
-        ontouml_graph.add((URIRef(args["base_uri"] + path_dict["id"]),
-                           URIRef(URI_ONTOUML + "point"),
-                           URIRef(args["base_uri"] + point_name)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + path_dict["id"]),
+                           ontouml_ref("point"),
+                           URIRef(args.ARGUMENTS["base_uri"] + point_name)))
 
         point_counter += 1
 
 
 def create_path_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type Path.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_project.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_all_ids_of_specific_type, get_list_subdictionaries_for_specific_type
-from ..globals import URI_ONTOUML
+import modules.arguments as args
+from modules.decoder.decode_general import get_all_ids_of_specific_type, get_list_subdictionaries_for_specific_type
+from modules.utils_graph import ontouml_ref
 
 
 def set_ontoumlelement_project_project(project_dict: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Sets the ontouml:project object property between an ontouml:Project (obj) and all its related entities (subj).
 
     :param project_dict: Project's data to have its fields decoded.
     :type project_dict: dict
@@ -33,33 +33,33 @@
         if available_type == "Project":
             continue
 
         # Get every project's related objects' ids
         list_objects_ids = get_all_ids_of_specific_type(project_dict, available_type)
 
         for json_object_id in list_objects_ids:
-            statement_subject = URIRef(args["base_uri"] + json_object_id)
-            statement_predicate = URIRef(URI_ONTOUML + "project")
-            statement_object = URIRef(args["base_uri"] + project_dict["id"])
+            statement_subject = URIRef(args.ARGUMENTS["base_uri"] + json_object_id)
+            statement_predicate = ontouml_ref("project")
+            statement_object = URIRef(args.ARGUMENTS["base_uri"] + project_dict["id"])
             ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def set_project_model_package(project_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets ontouml:model relation between an ontouml:Project and its related model.
 
     :param project_dict: Project's data to have its fields decoded.
     :type project_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     if "model" in project_dict:
-        statement_subject = URIRef(args["base_uri"] + project_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "model")
-        statement_object = URIRef(args["base_uri"] + project_dict["model"]["id"])
+        statement_subject = URIRef(args.ARGUMENTS["base_uri"] + project_dict["id"])
+        statement_predicate = ontouml_ref("model")
+        statement_object = URIRef(args.ARGUMENTS["base_uri"] + project_dict["model"]["id"])
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def set_project_diagram_diagram(project_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the ontouml:diagram object property between an ontouml:Project and its related ontouml:Diagram entities.
 
     :param project_dict: Project's data to have its fields decoded.
@@ -68,17 +68,17 @@
     :type ontouml_graph: Graph
     """
 
     # Getting all Diagrams for a specific Project
     list_all_diagram_ids = get_all_ids_of_specific_type(project_dict, "Diagram")
 
     for diagram_id in list_all_diagram_ids:
-        statement_subject = URIRef(args["base_uri"] + project_dict["id"])
-        statement_predicate = URIRef(URI_ONTOUML + "diagram")
-        statement_object = URIRef(args["base_uri"] + diagram_id)
+        statement_subject = URIRef(args.ARGUMENTS["base_uri"] + project_dict["id"])
+        statement_predicate = ontouml_ref("diagram")
+        statement_object = URIRef(args.ARGUMENTS["base_uri"] + diagram_id)
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def create_project_properties(json_data: dict, ontouml_graph: Graph, element_counting: dict) -> None:
     """ Main function for decoding objects of type 'Project'.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_property.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_property.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,20 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef, RDF, Literal, XSD
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_list_subdictionaries_for_specific_type
-from ..globals import URI_ONTOUML
-from ..logger import initialize_logger
-from ..messages import print_decode_log_message
-from ..sparql_queries import GET_CLASS_STEREOTYPE_ATTRIBUTE_STEREOTYPE
-from ..utils_graph import load_ontouml_vocabulary
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type
+from modules.logger import initialize_logger
+from modules.messages import print_decode_log_message
+from modules.sparql_queries import GET_CLASS_STEREOTYPE_ATTRIBUTE_STEREOTYPE
+from modules.utils_graph import load_ontouml_vocabulary, ontouml_ref
 
 LOGGER = initialize_logger()
 
 
 def validate_property_stereotype(ontouml_graph: Graph) -> None:
     """ Performs syntactical and semantic validations on an ontouml:Property's stereotype.
 
@@ -33,15 +32,15 @@
     I.e., a class stereotype that is known and different from 'event'.
     VPS3) Sets class stereotype as 'event' when it is associated to a property that has an assigned valid stereotype.
 
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    if not args["correct"]:
+    if not args.ARGUMENTS["correct"]:
         return
 
     ontouml_meta_graph = load_ontouml_vocabulary()
     aggregated_graph = ontouml_meta_graph + ontouml_graph
     query_answer = aggregated_graph.query(GET_CLASS_STEREOTYPE_ATTRIBUTE_STEREOTYPE)
 
     for row in query_answer:
@@ -65,17 +64,17 @@
         # VPS3: If class has unknown stereotype and stereotyped property, set its stereotype as 'event'.
         elif class_stereotype == "null":
 
             dict_argument = {"type": "Class", "name": class_name, "id": class_id, "stereotype": class_stereotype,
                              "propID": property_id, "propST": property_stereotype}
             print_decode_log_message(dict_argument, "VPS3")
 
-            ontouml_graph.add((URIRef(args["base_uri"] + class_id),
-                               URIRef(URI_ONTOUML + "stereotype"),
-                               URIRef(URI_ONTOUML + "event")))
+            ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + class_id),
+                               ontouml_ref("stereotype"),
+                               ontouml_ref("event")))
 
 
 def set_property_defaults(property_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets default values for ontouml:Property elements that do not present them. The defaults are:
     
     DPA1) ontouml:isDerived default value = False
     DPA2) ontouml:isOrdered default value = False
@@ -88,77 +87,77 @@
     """
 
     # DPA1, DPA2, and DPA3 use the same message DGA1, as they are not associated to their holder's stereotype.
 
     # DPA1: Setting ontouml:isDerived attribute default value
     if "isDerived" not in property_dict:
         print_decode_log_message(property_dict, "DGA1", property_name='isDerived')
-        ontouml_graph.add((URIRef(args["base_uri"] + property_dict['id']),
-                           URIRef(URI_ONTOUML + "isDerived"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + property_dict['id']),
+                           ontouml_ref("isDerived"), Literal(False, datatype=XSD.boolean)))
 
     # DPA2: Setting ontouml:isOrdered attribute default value
     if "isOrdered" not in property_dict:
         print_decode_log_message(property_dict, "DGA1", property_name='isOrdered')
-        ontouml_graph.add((URIRef(args["base_uri"] + property_dict['id']),
-                           URIRef(URI_ONTOUML + "isOrdered"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + property_dict['id']),
+                           ontouml_ref("isOrdered"), Literal(False, datatype=XSD.boolean)))
 
     # DPA3: Setting ontouml:isReadOnly attribute default value
     if "isReadOnly" not in property_dict:
         print_decode_log_message(property_dict, "DGA1", property_name='isReadOnly')
-        ontouml_graph.add((URIRef(args["base_uri"] + property_dict['id']),
-                           URIRef(URI_ONTOUML + "isReadOnly"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + property_dict['id']),
+                           ontouml_ref("isReadOnly"), Literal(False, datatype=XSD.boolean)))
 
 
 def set_property_relations(property_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the ontouml:aggregationKind and ontouml:propertyType object properties between an ontouml:Property and
     its related elements.
 
     :param property_dict: Property object loaded as a dictionary.
     :type property_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    statement_subject = URIRef(args["base_uri"] + property_dict["id"])
+    statement_subject = URIRef(args.ARGUMENTS["base_uri"] + property_dict["id"])
 
     # Setting ontouml:aggregationKind
     if "aggregationKind" not in property_dict:
-        statement_object = URIRef(URI_ONTOUML + "none")
+        statement_object = ontouml_ref("none")
     else:
-        statement_object = URIRef(URI_ONTOUML + property_dict["aggregationKind"].lower())
+        statement_object = ontouml_ref(property_dict["aggregationKind"].lower())
 
-    statement_predicate = URIRef(URI_ONTOUML + "aggregationKind")
+    statement_predicate = ontouml_ref("aggregationKind")
     ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
     # Setting ontouml:propertyType
     if "propertyType" in property_dict:
-        statement_predicate = URIRef(URI_ONTOUML + "propertyType")
-        statement_object = URIRef(args["base_uri"] + property_dict["propertyType"]["id"])
+        statement_predicate = ontouml_ref("propertyType")
+        statement_object = URIRef(args.ARGUMENTS["base_uri"] + property_dict["propertyType"]["id"])
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
     # Setting ontouml:stereotype. Its validation is performed later in function validate_property_stereotype
     if "stereotype" in property_dict:
-        statement_predicate = URIRef(URI_ONTOUML + "stereotype")
-        statement_object = URIRef(URI_ONTOUML + property_dict["stereotype"])
+        statement_predicate = ontouml_ref("stereotype")
+        statement_object = ontouml_ref(property_dict["stereotype"])
         ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
     # Setting ontouml:subsetsProperty
     if "subsettedProperties" in property_dict:
-        statement_predicate = URIRef(URI_ONTOUML + "subsetsProperty")
+        statement_predicate = ontouml_ref("subsetsProperty")
 
         for subsetted_prop_dict in property_dict["subsettedProperties"]:
-            statement_object = URIRef(args["base_uri"] + subsetted_prop_dict["id"])
+            statement_object = URIRef(args.ARGUMENTS["base_uri"] + subsetted_prop_dict["id"])
             ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
     # Setting ontouml:redefinesProperty
     if "redefinedProperties" in property_dict:
-        statement_predicate = URIRef(URI_ONTOUML + "redefinesProperty")
+        statement_predicate = ontouml_ref("redefinesProperty")
 
         for redefined_prop_dict in property_dict["redefinedProperties"]:
-            statement_object = URIRef(args["base_uri"] + redefined_prop_dict["id"])
+            statement_object = URIRef(args.ARGUMENTS["base_uri"] + redefined_prop_dict["id"])
             ontouml_graph.add((statement_subject, statement_predicate, statement_object))
 
 
 def determine_cardinality_bounds(cardinalities: str, property_id: str) -> (str, str, str):
     """ Receives a string with an ontouml:Cardinality's ontouml:cardinalityValue, fix its format and decouple it into
     its ontouml:lowerBound and ontouml:upperBound. Checks and displays warning if the obtained values are not valid.
 
@@ -178,18 +177,18 @@
     # If lower bound is * it is converted to zero
     if lower_bound == "*":
         lower_bound = "0"
 
     full_cardinality = lower_bound + ".." + upper_bound
 
     # Validating discovered cardinality bounds
-    if not (upper_bound.isnumeric() or upper_bound == "*") and not args["silent"]:
+    if not (upper_bound.isnumeric() or upper_bound == "*") and not args.ARGUMENTS["silent"]:
         LOGGER.warning(f"Invalid cardinality's upper bound (value '{upper_bound}') for Property individual with "
                        f"ID '{property_id}'. Transformation proceeded as is.")
-    if not lower_bound.isnumeric() and not args["silent"]:
+    if not lower_bound.isnumeric() and not args.ARGUMENTS["silent"]:
         LOGGER.warning(f"Invalid cardinality's lower bound (value '{lower_bound}') for Property individual with "
                        f"ID '{property_id}'. Transformation proceeded as is.")
 
     return full_cardinality, lower_bound, upper_bound
 
 
 def set_cardinality_relations(property_dict: dict, ontouml_graph: Graph) -> None:
@@ -198,23 +197,23 @@
     :param property_dict: Property object loaded as a dictionary.
     :type property_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
     if "cardinality" in property_dict:
-        ontology_property_individual = URIRef(args["base_uri"] + property_dict["id"])
-        ontology_cardinality_individual = URIRef(args["base_uri"] + property_dict["id"] + '_cardinality')
+        ontology_property_individual = URIRef(args.ARGUMENTS["base_uri"] + property_dict["id"])
+        ontology_cardinality_individual = URIRef(args.ARGUMENTS["base_uri"] + property_dict["id"] + '_cardinality')
 
-        ontouml_cardinality_class = URIRef(URI_ONTOUML + "Cardinality")
-        ontouml_cardinality_property = URIRef(URI_ONTOUML + "cardinality")
+        ontouml_cardinality_class = ontouml_ref("Cardinality")
+        ontouml_cardinality_property = ontouml_ref("cardinality")
 
-        ontouml_cardinalityvalue_property = URIRef(URI_ONTOUML + "cardinalityValue")
-        ontouml_lowerbound_property = URIRef(URI_ONTOUML + "lowerBound")
-        ontouml_upperbound_property = URIRef(URI_ONTOUML + "upperBound")
+        ontouml_cardinalityvalue_property = ontouml_ref("cardinalityValue")
+        ontouml_lowerbound_property = ontouml_ref("lowerBound")
+        ontouml_upperbound_property = ontouml_ref("upperBound")
 
         # Creating ontouml:Cardinality individuals (named after its related Property's name + '_cardinality' string)
         ontouml_graph.add((ontology_cardinality_individual, RDF.type, ontouml_cardinality_class))
 
         # Setting the ontouml:cardinality between an ontouml:Property and its ontouml:Cardinality
         ontouml_graph.add((ontology_property_individual, ontouml_cardinality_property, ontology_cardinality_individual))
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_rectangularshape.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_rectangularshape.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
-from ..globals import URI_ONTOUML
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, create_point
+from modules.utils_graph import ontouml_ref
 
 
 def set_rectangularshape_coordinates(rectangularshape_dict: dict, ontouml_graph: Graph) -> None:
     """ Creates an ontouml:Point, their properties and the ontouml:topLeftPosition of an ontouml:RectangularShape.
 
     :param rectangularshape_dict: RectangularShape object loaded as a dictionary.
     :type rectangularshape_dict: dict
@@ -25,17 +25,17 @@
     """
 
     # Creating new Point instance
     point_name = rectangularshape_dict["id"] + "_point"
     create_point(point_name, rectangularshape_dict["x"], rectangularshape_dict["y"], ontouml_graph)
 
     # Associating new Point with Rectangle
-    ontouml_graph.add((URIRef(args["base_uri"] + rectangularshape_dict["id"]),
-                       URIRef(URI_ONTOUML + "topLeftPosition"),
-                       URIRef(args["base_uri"] + point_name)))
+    ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + rectangularshape_dict["id"]),
+                       ontouml_ref("topLeftPosition"),
+                       URIRef(args.ARGUMENTS["base_uri"] + point_name)))
 
 
 def create_rectangularshape_properties(json_data: dict, ontouml_graph: Graph) -> None:
     """ Main function for decoding an object of type RectangularShape.
 
     Receives the whole JSON loaded data as a dictionary and manipulates it to create all properties in which the
     object's type is domain of.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/decoder/decode_obj_relation.py` & `ontouml_json2graph-1.0.0b3/src/modules/decoder/decode_obj_relation.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     - Functions that set multiple data properties are named: set_<subject>_attributes.
     - Functions that set both object and data properties are named: set_<subject>_properties.
     - Functions that set default values: set_<subject>_defaults.
 """
 
 from rdflib import Graph, URIRef, Literal, XSD
 
-from ..arguments import ARGUMENTS as args
-from ..decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
-from ..globals import URI_ONTOUML
-from ..messages import print_decode_log_message
+import modules.arguments as args
+from modules.decoder.decode_general import get_list_subdictionaries_for_specific_type, get_stereotype
+from modules.messages import print_decode_log_message
+from modules.utils_graph import ontouml_ref
 
 
 def set_relation_defaults(relation_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets the following attribute's default values for ontouml:Relation:
 
     DRA1) ontouml:isDerived default value = False
     DRA2) ontouml:isAbstract default value = False
@@ -29,22 +29,22 @@
     """
 
     # DRA1, and DRA2 use the same message DGA1, as they are not associated to their holder's stereotype.
 
     # DCA3: Setting ontouml:isDerived attribute default value
     if "isDerived" not in relation_dict:
         print_decode_log_message(relation_dict, "DGA1", property_name='isDerived')
-        ontouml_graph.add((URIRef(args["base_uri"] + relation_dict['id']),
-                           URIRef(URI_ONTOUML + "isDerived"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + relation_dict['id']),
+                           ontouml_ref("isDerived"), Literal(False, datatype=XSD.boolean)))
 
     # DCA4: Setting ontouml:isAbstract attribute default value
     if "isAbstract" not in relation_dict:
         print_decode_log_message(relation_dict, "DGA1", property_name='isAbstract')
-        ontouml_graph.add((URIRef(args["base_uri"] + relation_dict['id']),
-                           URIRef(URI_ONTOUML + "isAbstract"), Literal(False, datatype=XSD.boolean)))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + relation_dict['id']),
+                           ontouml_ref("isAbstract"), Literal(False, datatype=XSD.boolean)))
 
 
 def set_relation_stereotype(relation_dict: dict, ontouml_graph: Graph) -> None:
     """ Sets ontouml:stereotype property between an instance of ontouml:Relation and an instance representing an
     ontouml:RelationStereotype.
 
     Warning messages:
@@ -60,17 +60,17 @@
                                 "derivation", "externalDependence", "historicalDependence", "instantiation",
                                 "manifestation", "material", "mediation", "memberOf", "participation",
                                 "participational", "subCollectionOf", "subQuantityOf", "termination", "triggers"]
 
     relation_stereotype = get_stereotype(relation_dict)
 
     if relation_stereotype != "null":
-        ontouml_graph.add((URIRef(args["base_uri"] + relation_dict['id']),
-                           URIRef(URI_ONTOUML + "stereotype"),
-                           URIRef(URI_ONTOUML + relation_dict['stereotype'])))
+        ontouml_graph.add((URIRef(args.ARGUMENTS["base_uri"] + relation_dict['id']),
+                           ontouml_ref("stereotype"),
+                           ontouml_ref(relation_dict['stereotype'])))
 
         # If declared but invalid, create and report error. Uses generic message with code 'VCSG'.
         if relation_stereotype not in ENUM_RELATION_STEREOTYPE:
             print_decode_log_message(relation_dict, "VCSG", property_name="stereotype")
 
 
 def set_relation_relations(relation_dict: dict, ontouml_graph: Graph) -> None:
@@ -81,25 +81,25 @@
 
     :param relation_dict: Relation object loaded as a dictionary.
     :type relation_dict: dict
     :param ontouml_graph: Knowledge graph that complies with the OntoUML Vocabulary.
     :type ontouml_graph: Graph
     """
 
-    relation_individual = URIRef(args["base_uri"] + relation_dict['id'])
-    uri_relation_end = URIRef(URI_ONTOUML + "relationEnd")
-    uri_relation_sourceend = URIRef(URI_ONTOUML + "sourceEnd")
-    uri_relation_targetend = URIRef(URI_ONTOUML + "targetEnd")
+    relation_individual = URIRef(args.ARGUMENTS["base_uri"] + relation_dict['id'])
+    uri_relation_end = ontouml_ref("relationEnd")
+    uri_relation_sourceend = ontouml_ref("sourceEnd")
+    uri_relation_targetend = ontouml_ref("targetEnd")
 
     ends_list = []
     for property_dict in relation_dict["properties"]:
         ends_list.append(property_dict["id"])
 
-    source_id = URIRef(args["base_uri"] + ends_list[0])
-    target_id = URIRef(args["base_uri"] + ends_list[1])
+    source_id = URIRef(args.ARGUMENTS["base_uri"] + ends_list[0])
+    target_id = URIRef(args.ARGUMENTS["base_uri"] + ends_list[1])
 
     # Setting ontouml:relationEnd
     ontouml_graph.add((relation_individual, uri_relation_end, source_id))
     ontouml_graph.add((relation_individual, uri_relation_end, target_id))
 
     # Setting ontouml:sourceEnd and ontouml:targetEnd
     ontouml_graph.add((relation_individual, uri_relation_sourceend, source_id))
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/errors.py` & `ontouml_json2graph-1.0.0b3/src/modules/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Functions related to the verification and treatment of identified ERROR cases. """
 
-from .logger import initialize_logger
+from modules.logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
 def report_error_requirement_not_met(error_message: str) -> None:
     """ Reports the error caused when a requirement is not met. As this is a generic function, the error message
     parameter must be used to identify the error to the user.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/input_output.py` & `ontouml_json2graph-1.0.0b3/src/modules/input_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import json
 import os
 from pathlib import Path
 
 from rdflib import Graph
 
-from .errors import report_error_io_read, report_error_io_write
-from .logger import initialize_logger
+from modules.errors import report_error_io_read, report_error_io_write
+from modules.logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
 def create_directory_if_not_exists(directory_path: str, file_description: str) -> None:
     """ Checks if the directory that has the path received as argument exists.
     If it does, do nothing. If it does not, create it.
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/logger.py` & `ontouml_json2graph-1.0.0b3/src/modules/logger.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/messages.py` & `ontouml_json2graph-1.0.0b3/src/modules/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Decoding messages to be displayed to users must be concentrated in this module whenever possibile. """
 import inspect
 
-from .arguments import ARGUMENTS as args
-from .decoder.decode_general import get_stereotype
-from .errors import report_error_end_of_switch
-from .logger import initialize_logger
+import modules.arguments as args
+from modules.decoder.decode_general import get_stereotype
+from modules.errors import report_error_end_of_switch
+from modules.logger import initialize_logger
 
 LOGGER = initialize_logger()
 
 
 def get_decode_log_message(object_dict: dict, warning_code: str, property_name: str,
                            att_valid_stereotype: str = "") -> str:
     """ Mounts and returns a warning message according to the information received as parameter.
@@ -130,12 +130,12 @@
     :param property_name: Information about a property or attribute type to be displayed in a warning message. Optional.
     :type property_name: str
     :param att_valid_stereotype: Optional attribute's stereotype to be displayed in a warning message.
     :type att_valid_stereotype: str
     """
 
     # If in silent mode, exit function and do not print anything
-    if args["silent"]:
+    if args.ARGUMENTS["silent"]:
         return
 
     log_message = get_decode_log_message(object_dict, warning_code, property_name, att_valid_stereotype)
     LOGGER.warning(log_message)
```

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/sparql_queries.py` & `ontouml_json2graph-1.0.0b3/src/modules/sparql_queries.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/modules/utils_general.py` & `ontouml_json2graph-1.0.0b3/src/modules/utils_general.py`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/resources/ontouml_v100.ttl` & `ontouml_json2graph-1.0.0b3/src/resources/ontouml_v100.ttl`

 * *Files identical despite different names*

### Comparing `ontouml_json2graph-1.0.0b1/ontouml-json2graph/resources/ontouml_v110.ttl` & `ontouml_json2graph-1.0.0b3/src/resources/ontouml_v110.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -1,94 +1,87 @@
-@prefix :        <https://w3id.org/ontouml#> .
 @prefix dcat:    <http://www.w3.org/ns/dcat#> .
 @prefix dct:     <http://purl.org/dc/terms/> .
 @prefix foaf:    <http://xmlns.com/foaf/0.1/> .
 @prefix ontouml: <https://w3id.org/ontouml#> .
 @prefix owl:     <http://www.w3.org/2002/07/owl#> .
 @prefix rdf:     <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rdfs:    <http://www.w3.org/2000/01/rdf-schema#> .
-@prefix sdo:     <https://schema.org/> .
 @prefix vann:    <http://purl.org/vocab/vann/> .
 @prefix xml:     <http://www.w3.org/XML/1998/namespace> .
 @prefix xsd:     <http://www.w3.org/2001/XMLSchema#> .
 @base <https://w3id.org/ontouml> .
 
+
 #################################################################
 #    Metadata
 #################################################################
 
 <https://w3id.org/ontouml>
-    rdf:type                                                                                    owl:Ontology,
-                                                                                                dct:Standard ;
+    rdf:type                      owl:Ontology, dct:Standard ;
 
 ################################################################# VERSIONING
 
-    owl:versionIRI                                                                              <https://w3id.org/ontouml/1.1.0> ;
-    owl:versionInfo                                                                             "General review for compliance with the OntoUML Metamodel 1.1.0."@en ;
-    owl:priorVersion                                                                            <https://w3id.org/ontouml/1.0.0> ;
-    dct:issued                                                                                  "2022-04-03"^^xsd:date ;
-    dct:modified                                                                                "2023-07-23"^^xsd:date ;
+    owl:versionIRI                <https://w3id.org/ontouml/vocabulary/v1.1.0> ;
+    owl:versionInfo               "General review for compliance with the OntoUML Metamodel 1.1.1."@en ;
+    owl:priorVersion              <https://w3id.org/ontouml/vocabulary/v1.0.0> ;
+    dct:issued                    "2022-04-03"^^xsd:date ;
+    dct:modified                  "2023-07-27"^^xsd:date ;
 
 ################################################################# IDENTIFICATION
 
-    dct:title                                                                                   "OntoUML Metamodel Vocabulary"@en ;
-    dct:description                                                                             "A reference implementation of the OntoUML Metamodel in OWL."@en ;
-    dct:identifier                                                                              "https://w3id.org/ontouml"^^xsd:anyURI ;
-    dct:license                                                                                 <https://creativecommons.org/licenses/by-sa/4.0> ;
-    dct:conformsTo                                                                              <https://w3id.org/ontouml/metamodel/v1.1.0> ;
-    dcat:landingPage                                                                            <https://w3id.org/ontouml/vocabulary> ;
-    vann:preferredNamespacePrefix                                                               "ontouml" ;
-    vann:preferredNamespaceUri                                                                  "https://w3id.org/ontouml#"^^xsd:anyURI ;
-    foaf:homepage                                                                               <https://purl.org/> ;
-    dct:language                                                                                <http://id.loc.gov/vocabulary/iso639-1/en> ;
-    dct:isReferencedBy                                                                          <https://dblp.org/rec/conf/jowo/FonsecaSVFGA21.html>,
-                                                                                                <https://doi.org/10.1007/978-3-031-17995-2_1> ;
-    dcat:keyword                                                                                "OntoUML"@en,
-                                                                                                "OntoUML-Metamodel"@en,
-                                                                                                "OntoUML-Vocabulary"@en,
-                                                                                                "Ontology-Driven Conceptual Modeling"@en ;
+    dct:title                     "OntoUML Vocabulary"@en ;
+    dct:description               "An OWL vocabulary to allow the serialization and exchanging of OntoUML models in conformance with the Ontouml Metamodel."@en ;
+    dct:identifier                "https://w3id.org/ontouml"^^xsd:anyURI ;
+    dct:license                   <https://creativecommons.org/licenses/by-sa/4.0> ;
+    dct:conformsTo                <https://w3id.org/ontouml/metamodel/v1.1.1> ;
+    dcat:landingPage              <https://w3id.org/ontouml/vocabulary> ;
+    foaf:homepage                 <https://w3id.org/ontouml/vocabulary/docs> ;
+    vann:preferredNamespacePrefix "ontouml" ;
+    vann:preferredNamespaceUri    "https://w3id.org/ontouml#"^^xsd:anyURI ;
+    dct:language                  <http://id.loc.gov/vocabulary/iso639-1/en> ;
+    dct:isReferencedBy            <https://dblp.org/rec/conf/jowo/FonsecaSVFGA21.html>,
+                                  <https://doi.org/10.1007/978-3-031-17995-2_1> ;
+    dcat:keyword                  "OntoUML"@en, "OntoUML-Metamodel"@en, "Ontology-Driven Conceptual Modeling"@en ;
 
 ################################################################# AUTHORSHIP
 
-    dct:publisher                                                                               <https://www.utwente.nl/en/eemcs/scs/> ;
-    dct:creator                                                                                 [ sdo:name
-                                                                                                          "Tiago Prince Sales"@en ;
-                                                                                                  sdo:identifier
-                                                                                                          <https://orcid.org/0000-0002-5385-5761> ;
-                                                                                                  sdo:affiliation
-                                                                                                          <https://www.utwente.nl/en/eemcs/scs/> ; ],
-                                                                                                [ sdo:name
-                                                                                                          "Claudenir M. Fonseca"@en ;
-                                                                                                  sdo:identifier
-                                                                                                          <https://orcid.org/0000-0003-2528-3118> ;
-                                                                                                  sdo:affiliation
-                                                                                                          <https://www.utwente.nl/en/eemcs/scs/> ; ],
-                                                                                                [ sdo:name
-                                                                                                          "Pedro Paulo Favato Barcelos"@en ;
-                                                                                                  sdo:identifier
-                                                                                                          <https://orcid.org/0000-0003-2736-7817> ;
-                                                                                                  sdo:affiliation
-                                                                                                          <https://www.utwente.nl/en/eemcs/scs/> ; ] ;
-    dct:contributor                                                                             [ sdo:name
-                                                                                                          "Mattia Fumagalli"@en ;
-                                                                                                  sdo:identifier
-                                                                                                          <https://orcid.org/0000-0003-3385-4769> ;
-                                                                                                  sdo:affiliation
-                                                                                                          <https://www.inf.unibz.it/krdb/> ; ] .
-
+    dct:publisher                 <https://www.utwente.nl/en/eemcs/scs/> ;
+    dct:creator                   <https://orcid.org/0000-0002-5385-5761>, <https://orcid.org/0000-0003-2528-3118>,
+                                  <https://orcid.org/0000-0003-2736-7817> ;
+    dct:contributor               <https://orcid.org/0000-0003-3385-4769> .
 
 <https://www.inf.unibz.it/krdb/>
-    rdf:type sdo:Organization ;
-    sdo:name "KRDB Research Centre for Knowledge and Data, Free University of Bozen-Bolzano, Italy" ;
-    sdo:url  "https://www.inf.unibz.it/krdb/"^^xsd:anyURI .
+    rdf:type      foaf:Organization ;
+    foaf:name     "KRDB Research Centre for Knowledge and Data, Free University of Bozen-Bolzano, Italy" ;
+    foaf:homepage "https://www.inf.unibz.it/krdb/"^^xsd:anyURI ;
+    foaf:member   <https://orcid.org/0000-0003-3385-4769> .
 
 <https://www.utwente.nl/en/eemcs/scs/>
-    rdf:type sdo:Organization ;
-    sdo:name "Semantics, Cybersecurity & Services (SCS), University of Twente, the Netherlands" ;
-    sdo:url  "https://www.utwente.nl/en/eemcs/scs/"^^xsd:anyURI .
+    rdf:type      foaf:Organization ;
+    foaf:name     "Semantics, Cybersecurity & Services (SCS), University of Twente, the Netherlands" ;
+    foaf:homepage "https://www.utwente.nl/en/eemcs/scs/"^^xsd:anyURI ;
+    foaf:member   <https://orcid.org/0000-0002-5385-5761>, <https://orcid.org/0000-0003-2528-3118>,
+                  <https://orcid.org/0000-0003-2736-7817> .
+
+<https://orcid.org/0000-0003-3385-4769>
+    foaf:name "Mattia Fumagalli" ;
+    foaf:mbox "mattia.fumagalli@unibz.it" .
+
+<https://orcid.org/0000-0002-5385-5761>
+    foaf:name "Tiago Prince Sales" ;
+    foaf:mbox "t.princesales@utwente.nl" .
+
+<https://orcid.org/0000-0003-2528-3118>
+    foaf:name "Claudenir M. Fonseca" ;
+    foaf:mbox "c.moraisfonseca@utwente.nl" .
+
+<https://orcid.org/0000-0003-2736-7817>
+    foaf:name "Pedro Paulo Favato Barcelos" ;
+    foaf:mbox "p.p.favatobarcelos@uwente.nl" .
+
 
 #################################################################
 #    Object Properties
 #################################################################
 
 ###  https://w3id.org/ontouml#aggregationKind
 ontouml:aggregationKind
@@ -124,16 +117,16 @@
 ###  https://w3id.org/ontouml#categorizer
 ontouml:categorizer
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:GeneralizationSet ;
     rdfs:range       ontouml:Class ;
     rdfs:label       "categorizer"@en ;
     rdfs:isDefinedBy <https://w3id.org/ontouml> ;
-    rdfs:comment     "Identifies individuals of an ontouml:GeneralizationSet that are instances of a higher order ontouml:Class."@en ;
-    rdfs:seeAlso     <https://doi.org/10.1007/978-3-319-39696-5_19> .
+    rdfs:comment     " Identifies the ontouml:Class that is instantiated by the specific classes of the ontouml:Generalization type composing the ontouml:GeneralizationSet"@en ;
+    rdfs:seeAlso     <https://doi.org/10.1016/j.datak.2022.102012>, <https://doi.org/10.1007/978-3-031-17995-2_2> .
 
 
 ###  https://w3id.org/ontouml#containsModelElement
 ontouml:containsModelElement
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:Package ;
     rdfs:range       ontouml:ModelElement ;
@@ -344,15 +337,15 @@
 ###  https://w3id.org/ontouml#stereotype
 ontouml:stereotype
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:DecoratableElement ;
     rdfs:range       ontouml:Stereotype ;
     rdfs:label       "stereotype"@en ;
     rdfs:isDefinedBy <https://w3id.org/ontouml> ;
-    rdfs:comment     "Identifies an ontouml:Stereotype applied to an ontouml:DecoratableElement."@en .
+    rdfs:comment     "Identifies the ontouml:Stereotype applied to the ontouml:DecoratableElement."@en .
 
 
 ###  https://w3id.org/ontouml#subsetsProperty
 ontouml:subsetsProperty
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:Property ;
     rdfs:range       ontouml:Property ;
@@ -375,15 +368,15 @@
 ###  https://w3id.org/ontouml#targetView
 ontouml:targetView
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:ConnectorView ;
     rdfs:range       ontouml:ElementView ;
     rdfs:label       "targetView"@en ;
     rdfs:isDefinedBy <https://w3id.org/ontouml> ;
-    rdfs:comment     "Identifies an ontouml:ElementView that participates as target of an ontouml:RelationView or ontouml:GeneralizationView."@en .
+    rdfs:comment     "Identifies an ontouml:ElementView that participates as target of an ontouml:ConnectorView."@en .
 
 
 ###  https://w3id.org/ontouml#topLeftPosition
 ontouml:topLeftPosition
     rdf:type         owl:ObjectProperty ;
     rdfs:domain      ontouml:RectangularShape ;
     rdfs:range       ontouml:Point ;
```

