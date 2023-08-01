# Comparing `tmp/jsno-1.0.4.tar.gz` & `tmp/jsno-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsno-1.0.4.tar", last modified: Sun Jul 30 15:35:23 2023, max compression
+gzip compressed data, was "jsno-1.0.5.tar", last modified: Tue Aug  1 12:18:00 2023, max compression
```

## Comparing `jsno-1.0.4.tar` & `jsno-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-30 15:35:23.490697 jsno-1.0.4/
--rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.4/LICENSE
--rw-r--r--   0 pekka      (501) staff       (20)    10330 2023-07-30 15:35:23.490381 jsno-1.0.4/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)     8604 2023-07-30 15:31:42.000000 jsno-1.0.4/README.md
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-30 15:35:23.482623 jsno-1.0.4/jsno/
--rw-r--r--   0 pekka      (501) staff       (20)     1748 2023-07-30 15:33:51.000000 jsno-1.0.4/jsno/__init__.py
--rw-r--r--   0 pekka      (501) staff       (20)     2316 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     4542 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      710 2023-07-30 15:32:48.000000 jsno-1.0.4/jsno/jsonize.py
--rw-r--r--   0 pekka      (501) staff       (20)      630 2023-07-29 19:08:24.000000 jsno-1.0.4/jsno/method.py
--rw-r--r--   0 pekka      (501) staff       (20)     5243 2023-07-29 19:40:07.000000 jsno-1.0.4/jsno/standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     3976 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      882 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/utils.py
--rw-r--r--   0 pekka      (501) staff       (20)     3437 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/variant.py
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-30 15:35:23.484047 jsno-1.0.4/jsno.egg-info/
--rw-r--r--   0 pekka      (501) staff       (20)    10330 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)      568 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/SOURCES.txt
--rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/dependency_links.txt
--rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/requires.txt
--rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/top_level.txt
--rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-30 15:33:55.000000 jsno-1.0.4/pyproject.toml
--rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-30 15:35:23.490768 jsno-1.0.4/setup.cfg
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-30 15:35:23.489733 jsno-1.0.4/tests/
--rw-r--r--   0 pekka      (501) staff       (20)     1223 2023-07-29 19:21:09.000000 jsno-1.0.4/tests/test_abc.py
--rw-r--r--   0 pekka      (501) staff       (20)      936 2023-07-30 15:34:37.000000 jsno-1.0.4/tests/test_ast_example.py
--rw-r--r--   0 pekka      (501) staff       (20)     4205 2023-07-29 18:53:29.000000 jsno-1.0.4/tests/test_dataclasses.py
--rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 18:50:18.000000 jsno-1.0.4/tests/test_dates.py
--rw-r--r--   0 pekka      (501) staff       (20)      165 2023-07-30 07:55:38.000000 jsno-1.0.4/tests/test_dumps_and_loads.py
--rw-r--r--   0 pekka      (501) staff       (20)     1794 2023-07-30 15:34:48.000000 jsno-1.0.4/tests/test_examples.py
--rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 18:53:15.000000 jsno-1.0.4/tests/test_jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2735 2023-07-29 18:46:29.000000 jsno-1.0.4/tests/test_methods.py
--rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 18:45:56.000000 jsno-1.0.4/tests/test_standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4437 2023-07-29 18:50:19.000000 jsno-1.0.4/tests/test_unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2886 2023-07-29 18:52:46.000000 jsno-1.0.4/tests/test_variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-01 12:18:00.653600 jsno-1.0.5/
+-rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.5/LICENSE
+-rw-r--r--   0 pekka      (501) staff       (20)    10756 2023-08-01 12:18:00.653119 jsno-1.0.5/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)     9082 2023-08-01 12:15:43.000000 jsno-1.0.5/README.md
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-01 12:18:00.647870 jsno-1.0.5/jsno/
+-rw-r--r--   0 pekka      (501) staff       (20)     1748 2023-08-01 12:17:09.000000 jsno-1.0.5/jsno/__init__.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2316 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4542 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      710 2023-07-30 15:32:48.000000 jsno-1.0.5/jsno/jsonize.py
+-rw-r--r--   0 pekka      (501) staff       (20)      630 2023-07-29 19:08:24.000000 jsno-1.0.5/jsno/method.py
+-rw-r--r--   0 pekka      (501) staff       (20)     5243 2023-07-29 19:40:07.000000 jsno-1.0.5/jsno/standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3976 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      882 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/utils.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3437 2023-07-29 19:39:45.000000 jsno-1.0.5/jsno/variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-01 12:18:00.649085 jsno-1.0.5/jsno.egg-info/
+-rw-r--r--   0 pekka      (501) staff       (20)    10756 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)      568 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/SOURCES.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        1 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/dependency_links.txt
+-rw-r--r--   0 pekka      (501) staff       (20)       23 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/requires.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        5 2023-08-01 12:18:00.000000 jsno-1.0.5/jsno.egg-info/top_level.txt
+-rw-r--r--   0 pekka      (501) staff       (20)      639 2023-08-01 12:17:32.000000 jsno-1.0.5/pyproject.toml
+-rw-r--r--   0 pekka      (501) staff       (20)       38 2023-08-01 12:18:00.653705 jsno-1.0.5/setup.cfg
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-01 12:18:00.652546 jsno-1.0.5/tests/
+-rw-r--r--   0 pekka      (501) staff       (20)     1223 2023-07-29 19:21:09.000000 jsno-1.0.5/tests/test_abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)      936 2023-07-30 15:34:37.000000 jsno-1.0.5/tests/test_ast_example.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4205 2023-07-29 18:53:29.000000 jsno-1.0.5/tests/test_dataclasses.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 18:50:18.000000 jsno-1.0.5/tests/test_dates.py
+-rw-r--r--   0 pekka      (501) staff       (20)      165 2023-07-30 07:55:38.000000 jsno-1.0.5/tests/test_dumps_and_loads.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1794 2023-07-30 15:34:48.000000 jsno-1.0.5/tests/test_examples.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 18:53:15.000000 jsno-1.0.5/tests/test_jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2735 2023-07-29 18:46:29.000000 jsno-1.0.5/tests/test_methods.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 18:45:56.000000 jsno-1.0.5/tests/test_standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4437 2023-07-29 18:50:19.000000 jsno-1.0.5/tests/test_unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2886 2023-07-29 18:52:46.000000 jsno-1.0.5/tests/test_variant.py
```

### Comparing `jsno-1.0.4/LICENSE` & `jsno-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/PKG-INFO` & `jsno-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.4
+Version: 1.0.5
 Summary: Convert Python data to and from json-compatible data structures
-Author-email: Pekka Uronen <pekka.uronen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -40,15 +39,15 @@
 
 Jsno provides functions that turn any Python values into JSON-compatible
 structures and back. The jsonified data can then be used wherever JSON
 data is required: it can be dumped into a file, sent over the network
 in an API call, or stored in a database that support JSON data.
 
 Note that jsno does not replace the standard _json_ module - it does not
-produce JSON encoded string, but turns arbitrary Python values into
+produce JSON encoded string, but instead turns arbitrary Python values into
 structures that _can_ be JSON encoded.
 
 Jsno provides jsonification for most of the standard Python datatypes.
 It is also easily _extensible_, so that custom jsonification can be
 defined for new datatypes.
 
 Jsno has special support for _dataclasses_, so no effort is needed to
@@ -130,15 +129,14 @@
         "enabled_at": "1992-01-01"
     },
     {
         "domain": "another.example.com",
         "ips": []
     }
 ]
---
 ```
 
 To read and use the domains later:
 
 ```py
 jsonified = json.loads(pathlib.Path('domains.json').read_text())
 domains = jsno.unjsonify[list[DomainRecord]](jsonified)
@@ -186,14 +184,15 @@
 
 ### Other standard Python types
 
 * tuples
 * ranges
 * enums
 * date and datetime objects (converted to ISO-formatted strings)
+* complex
 * decimal.Decimal (converted to JSON strings)
 * pathlib.Path
 * zoneinfo.ZoneInfo
 * Literal (only int and str literals)
 
 ## Dumps and loads
 
@@ -233,15 +232,14 @@
     # first unjsonify the state
     state = jsno.unjsonify[tuple[int, tuple[int, ...], float | None]](value)
 
     # create a new Random object and install the unjsonified state
     result = Random()
     result.setstate(state)
     return result
-
 ```
 
 Now it's possible to for example have a random number generator as a part of a data
 structure defined using dataclasses, and have it converted to and from JSON
 automatically:
 
 ```py
@@ -257,14 +255,28 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
+## Jsonification as string
+
+For types that can be converted to strings and back, jsno has a convenience
+function _jsonify_as_string_. For example, to provide jsonification for the _furl_
+class of the furl library:
+
+```py
+from furl import furl
+
+jsno.jsnonify_as_string(furl)
+```
+
+
+
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
 defined using a hierarchy of dataclasses:
 
@@ -326,33 +338,34 @@
 ```
 
 However, reading the AST back from JSON won't work. Trying to unjsonify it as an
 _Expression_ fails:
 
 ```py
 jsno.unjsonify[Expression](json)
-# TypeError: Unjsonify not defined for <class 'test_ast_example.Expression'>
+# TypeError: Unjsonify not defined for <class 'Expression'>
 ```
 
 Even if you defined the base Expression class as a dataclass, jsno wouldn't not which
 of the subclasses should it choose.
 
 The solution to the problem is to mark the root of the expression as the root of a
-_variant family_, using the
-`variantfamily` decorator:
+_variant family_, using the `variantfamily` decorator:
 
 ```py
 @jsno.variantfamily(label="type")
 class Expression:
     pass
 ```
 
-When a class is marked to form a variant family, jsno will add a label to the jsonfied
-data, to denote the class. Now, the JSON produced by `jsonify` contains labels to
-differntiate between the subclasses (variants):
+When a class is marked to form a variant family, jsno will add a label to the data
+jsonfied from it's, or it's subclasses' instances, to identify the class.
+
+Adter adding the decorator, the JSON produced by _jsonify_ contains labels to
+differentiate between the subclasses (variants):
 
 ```json
 {
     "type": "Add",
     "left": {
         "type": "LiteralInt",
         "value": 1
@@ -372,19 +385,30 @@
 ```
 
 The variant label's name (`type`) was given in the decorator.
 
 Now, jsno is able to unjsonify the AST:
 
 ```py
-assert jsno.unjsonify[Expression](json) == ast
+unjsonified_ast = jsno.unjsonify[Expression](json)
+assert unjsonified_ast == ast
 ```
 
 By default, the label for a class is taken from the class name. It's also possible
-to give it explicitly, if needed, using the `variantlabel` decorator:
+to give it explicitly using the `variantlabel` decorator:
 
-```
+```py
 @jsno.variantlabel('mult')
 class Multiply(Expression):
     # ...
 
 ```
+
+## Installation
+
+Install jsno with pip:
+
+```bash
+pip install jsno
+```
+
+Jsno has no 3rd party dependencies.
```

### Comparing `jsno-1.0.4/README.md` & `jsno-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Jsno provides functions that turn any Python values into JSON-compatible
 structures and back. The jsonified data can then be used wherever JSON
 data is required: it can be dumped into a file, sent over the network
 in an API call, or stored in a database that support JSON data.
 
 Note that jsno does not replace the standard _json_ module - it does not
-produce JSON encoded string, but turns arbitrary Python values into
+produce JSON encoded string, but instead turns arbitrary Python values into
 structures that _can_ be JSON encoded.
 
 Jsno provides jsonification for most of the standard Python datatypes.
 It is also easily _extensible_, so that custom jsonification can be
 defined for new datatypes.
 
 Jsno has special support for _dataclasses_, so no effort is needed to
@@ -93,15 +93,14 @@
         "enabled_at": "1992-01-01"
     },
     {
         "domain": "another.example.com",
         "ips": []
     }
 ]
---
 ```
 
 To read and use the domains later:
 
 ```py
 jsonified = json.loads(pathlib.Path('domains.json').read_text())
 domains = jsno.unjsonify[list[DomainRecord]](jsonified)
@@ -149,14 +148,15 @@
 
 ### Other standard Python types
 
 * tuples
 * ranges
 * enums
 * date and datetime objects (converted to ISO-formatted strings)
+* complex
 * decimal.Decimal (converted to JSON strings)
 * pathlib.Path
 * zoneinfo.ZoneInfo
 * Literal (only int and str literals)
 
 ## Dumps and loads
 
@@ -196,15 +196,14 @@
     # first unjsonify the state
     state = jsno.unjsonify[tuple[int, tuple[int, ...], float | None]](value)
 
     # create a new Random object and install the unjsonified state
     result = Random()
     result.setstate(state)
     return result
-
 ```
 
 Now it's possible to for example have a random number generator as a part of a data
 structure defined using dataclasses, and have it converted to and from JSON
 automatically:
 
 ```py
@@ -220,14 +219,28 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
+## Jsonification as string
+
+For types that can be converted to strings and back, jsno has a convenience
+function _jsonify_as_string_. For example, to provide jsonification for the _furl_
+class of the furl library:
+
+```py
+from furl import furl
+
+jsno.jsnonify_as_string(furl)
+```
+
+
+
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
 defined using a hierarchy of dataclasses:
 
@@ -289,33 +302,34 @@
 ```
 
 However, reading the AST back from JSON won't work. Trying to unjsonify it as an
 _Expression_ fails:
 
 ```py
 jsno.unjsonify[Expression](json)
-# TypeError: Unjsonify not defined for <class 'test_ast_example.Expression'>
+# TypeError: Unjsonify not defined for <class 'Expression'>
 ```
 
 Even if you defined the base Expression class as a dataclass, jsno wouldn't not which
 of the subclasses should it choose.
 
 The solution to the problem is to mark the root of the expression as the root of a
-_variant family_, using the
-`variantfamily` decorator:
+_variant family_, using the `variantfamily` decorator:
 
 ```py
 @jsno.variantfamily(label="type")
 class Expression:
     pass
 ```
 
-When a class is marked to form a variant family, jsno will add a label to the jsonfied
-data, to denote the class. Now, the JSON produced by `jsonify` contains labels to
-differntiate between the subclasses (variants):
+When a class is marked to form a variant family, jsno will add a label to the data
+jsonfied from it's, or it's subclasses' instances, to identify the class.
+
+Adter adding the decorator, the JSON produced by _jsonify_ contains labels to
+differentiate between the subclasses (variants):
 
 ```json
 {
     "type": "Add",
     "left": {
         "type": "LiteralInt",
         "value": 1
@@ -335,19 +349,30 @@
 ```
 
 The variant label's name (`type`) was given in the decorator.
 
 Now, jsno is able to unjsonify the AST:
 
 ```py
-assert jsno.unjsonify[Expression](json) == ast
+unjsonified_ast = jsno.unjsonify[Expression](json)
+assert unjsonified_ast == ast
 ```
 
 By default, the label for a class is taken from the class name. It's also possible
-to give it explicitly, if needed, using the `variantlabel` decorator:
+to give it explicitly using the `variantlabel` decorator:
 
-```
+```py
 @jsno.variantlabel('mult')
 class Multiply(Expression):
     # ...
 
 ```
+
+## Installation
+
+Install jsno with pip:
+
+```bash
+pip install jsno
+```
+
+Jsno has no 3rd party dependencies.
```

### Comparing `jsno-1.0.4/jsno/__init__.py` & `jsno-1.0.5/jsno/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from jsno.unjsonify import unjsonify, UnjsonifyError
 from jsno.variant import get_variantfamily, variantfamily, variantlabel, VariantFamily
 
 # import to register jsonifiers
 import jsno.abc  # noqa
 
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 __all__ = [
     "dumps",
     "jsonify",
     "jsonify_as_string",
     "jsonify_with_method",
     "get_variantfamily",
```

### Comparing `jsno-1.0.4/jsno/abc.py` & `jsno-1.0.5/jsno/abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/jsno/jsonify.py` & `jsno-1.0.5/jsno/jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/jsno/jsonize.py` & `jsno-1.0.5/jsno/jsonize.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/jsno/method.py` & `jsno-1.0.5/jsno/method.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/jsno/standard.py` & `jsno-1.0.5/jsno/standard.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/jsno/unjsonify.py` & `jsno-1.0.5/jsno/unjsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/jsno/utils.py` & `jsno-1.0.5/jsno/utils.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/jsno/variant.py` & `jsno-1.0.5/jsno/variant.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/jsno.egg-info/PKG-INFO` & `jsno-1.0.5/jsno.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.4
+Version: 1.0.5
 Summary: Convert Python data to and from json-compatible data structures
-Author-email: Pekka Uronen <pekka.uronen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -40,15 +39,15 @@
 
 Jsno provides functions that turn any Python values into JSON-compatible
 structures and back. The jsonified data can then be used wherever JSON
 data is required: it can be dumped into a file, sent over the network
 in an API call, or stored in a database that support JSON data.
 
 Note that jsno does not replace the standard _json_ module - it does not
-produce JSON encoded string, but turns arbitrary Python values into
+produce JSON encoded string, but instead turns arbitrary Python values into
 structures that _can_ be JSON encoded.
 
 Jsno provides jsonification for most of the standard Python datatypes.
 It is also easily _extensible_, so that custom jsonification can be
 defined for new datatypes.
 
 Jsno has special support for _dataclasses_, so no effort is needed to
@@ -130,15 +129,14 @@
         "enabled_at": "1992-01-01"
     },
     {
         "domain": "another.example.com",
         "ips": []
     }
 ]
---
 ```
 
 To read and use the domains later:
 
 ```py
 jsonified = json.loads(pathlib.Path('domains.json').read_text())
 domains = jsno.unjsonify[list[DomainRecord]](jsonified)
@@ -186,14 +184,15 @@
 
 ### Other standard Python types
 
 * tuples
 * ranges
 * enums
 * date and datetime objects (converted to ISO-formatted strings)
+* complex
 * decimal.Decimal (converted to JSON strings)
 * pathlib.Path
 * zoneinfo.ZoneInfo
 * Literal (only int and str literals)
 
 ## Dumps and loads
 
@@ -233,15 +232,14 @@
     # first unjsonify the state
     state = jsno.unjsonify[tuple[int, tuple[int, ...], float | None]](value)
 
     # create a new Random object and install the unjsonified state
     result = Random()
     result.setstate(state)
     return result
-
 ```
 
 Now it's possible to for example have a random number generator as a part of a data
 structure defined using dataclasses, and have it converted to and from JSON
 automatically:
 
 ```py
@@ -257,14 +255,28 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
+## Jsonification as string
+
+For types that can be converted to strings and back, jsno has a convenience
+function _jsonify_as_string_. For example, to provide jsonification for the _furl_
+class of the furl library:
+
+```py
+from furl import furl
+
+jsno.jsnonify_as_string(furl)
+```
+
+
+
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
 defined using a hierarchy of dataclasses:
 
@@ -326,33 +338,34 @@
 ```
 
 However, reading the AST back from JSON won't work. Trying to unjsonify it as an
 _Expression_ fails:
 
 ```py
 jsno.unjsonify[Expression](json)
-# TypeError: Unjsonify not defined for <class 'test_ast_example.Expression'>
+# TypeError: Unjsonify not defined for <class 'Expression'>
 ```
 
 Even if you defined the base Expression class as a dataclass, jsno wouldn't not which
 of the subclasses should it choose.
 
 The solution to the problem is to mark the root of the expression as the root of a
-_variant family_, using the
-`variantfamily` decorator:
+_variant family_, using the `variantfamily` decorator:
 
 ```py
 @jsno.variantfamily(label="type")
 class Expression:
     pass
 ```
 
-When a class is marked to form a variant family, jsno will add a label to the jsonfied
-data, to denote the class. Now, the JSON produced by `jsonify` contains labels to
-differntiate between the subclasses (variants):
+When a class is marked to form a variant family, jsno will add a label to the data
+jsonfied from it's, or it's subclasses' instances, to identify the class.
+
+Adter adding the decorator, the JSON produced by _jsonify_ contains labels to
+differentiate between the subclasses (variants):
 
 ```json
 {
     "type": "Add",
     "left": {
         "type": "LiteralInt",
         "value": 1
@@ -372,19 +385,30 @@
 ```
 
 The variant label's name (`type`) was given in the decorator.
 
 Now, jsno is able to unjsonify the AST:
 
 ```py
-assert jsno.unjsonify[Expression](json) == ast
+unjsonified_ast = jsno.unjsonify[Expression](json)
+assert unjsonified_ast == ast
 ```
 
 By default, the label for a class is taken from the class name. It's also possible
-to give it explicitly, if needed, using the `variantlabel` decorator:
+to give it explicitly using the `variantlabel` decorator:
 
-```
+```py
 @jsno.variantlabel('mult')
 class Multiply(Expression):
     # ...
 
 ```
+
+## Installation
+
+Install jsno with pip:
+
+```bash
+pip install jsno
+```
+
+Jsno has no 3rd party dependencies.
```

### Comparing `jsno-1.0.4/jsno.egg-info/SOURCES.txt` & `jsno-1.0.5/jsno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/pyproject.toml` & `jsno-1.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsno"
-version = "1.0.4"
+version = "1.0.5"
 description = "Convert Python data to and from json-compatible data structures"
 readme = "README.md"
-authors = [{ name = "Pekka Uronen", email = "pekka.uronen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["json"]
```

### Comparing `jsno-1.0.4/tests/test_abc.py` & `jsno-1.0.5/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_ast_example.py` & `jsno-1.0.5/tests/test_ast_example.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_dataclasses.py` & `jsno-1.0.5/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_dates.py` & `jsno-1.0.5/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_examples.py` & `jsno-1.0.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_jsonify.py` & `jsno-1.0.5/tests/test_jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_methods.py` & `jsno-1.0.5/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_standard.py` & `jsno-1.0.5/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_unjsonify.py` & `jsno-1.0.5/tests/test_unjsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.4/tests/test_variant.py` & `jsno-1.0.5/tests/test_variant.py`

 * *Files identical despite different names*

