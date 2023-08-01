# Comparing `tmp/saa-0.0.5.tar.gz` & `tmp/saa-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saa-0.0.5.tar", max compression
+gzip compressed data, was "saa-0.0.6.tar", max compression
```

## Comparing `saa-0.0.5.tar` & `saa-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1079 2023-06-24 14:38:26.102207 saa-0.0.5/LICENSE
--rw-r--r--   0        0        0     7699 2023-06-24 14:38:26.102207 saa-0.0.5/README.md
--rw-r--r--   0        0        0      561 2023-06-24 14:38:26.102207 saa-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      125 2023-06-24 14:38:26.102207 saa-0.0.5/saa/__init__.py
--rw-r--r--   0        0        0     1519 2023-06-24 14:38:26.102207 saa-0.0.5/saa/clock.py
--rw-r--r--   0        0        0        0 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/__init__.py
--rw-r--r--   0        0        0      662 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/language.py
--rw-r--r--   0        0        0      837 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/numbers.py
--rw-r--r--   0        0        0      308 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/plugins.py
--rw-r--r--   0        0        0      644 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/template.py
--rw-r--r--   0        0        0      827 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/watch.py
--rw-r--r--   0        0        0     1599 2023-06-24 14:38:26.102207 saa-0.0.5/saa/luga/da/__init__.py
--rw-r--r--   0        0        0     1434 2023-06-24 14:38:26.102207 saa-0.0.5/saa/luga/en/__init__.py
--rw-r--r--   0        0        0     2187 2023-06-24 14:38:26.102207 saa-0.0.5/saa/luga/sw/__init__.py
--rw-r--r--   0        0        0     8191 1970-01-01 00:00:00.000000 saa-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-08-01 14:52:22.135514 saa-0.0.6/LICENSE
+-rw-r--r--   0        0        0     8080 2023-08-01 14:52:22.135514 saa-0.0.6/README.md
+-rw-r--r--   0        0        0      561 2023-08-01 14:52:22.135514 saa-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-08-01 14:52:22.135514 saa-0.0.6/saa/__init__.py
+-rw-r--r--   0        0        0     1519 2023-08-01 14:52:22.135514 saa-0.0.6/saa/clock.py
+-rw-r--r--   0        0        0        0 2023-08-01 14:52:22.135514 saa-0.0.6/saa/core/__init__.py
+-rw-r--r--   0        0        0      662 2023-08-01 14:52:22.135514 saa-0.0.6/saa/core/language.py
+-rw-r--r--   0        0        0      837 2023-08-01 14:52:22.135514 saa-0.0.6/saa/core/numbers.py
+-rw-r--r--   0        0        0      308 2023-08-01 14:52:22.135514 saa-0.0.6/saa/core/plugins.py
+-rw-r--r--   0        0        0      644 2023-08-01 14:52:22.139514 saa-0.0.6/saa/core/template.py
+-rw-r--r--   0        0        0      827 2023-08-01 14:52:22.139514 saa-0.0.6/saa/core/watch.py
+-rw-r--r--   0        0        0     1599 2023-08-01 14:52:22.139514 saa-0.0.6/saa/luga/da/__init__.py
+-rw-r--r--   0        0        0     1684 2023-08-01 14:52:22.139514 saa-0.0.6/saa/luga/de/__init__.py
+-rw-r--r--   0        0        0     1434 2023-08-01 14:52:22.139514 saa-0.0.6/saa/luga/en/__init__.py
+-rw-r--r--   0        0        0     2187 2023-08-01 14:52:22.139514 saa-0.0.6/saa/luga/sw/__init__.py
+-rw-r--r--   0        0        0     8572 1970-01-01 00:00:00.000000 saa-0.0.6/PKG-INFO
```

### Comparing `saa-0.0.5/LICENSE` & `saa-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/README.md` & `saa-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 
 clock = Clock("en")
 clock("11:15") # 'quarter past eleven'
 
 ur = Clock("da")
 t = time(hour=7, minute=30)
 ur(t) # 'halvotte'
+
+muda = Clock("sw")
+muda("7:29") # 'saa moja na dakika ishirini na tisa asubuhi'
 ```
 
 ## Features
 
 - Convert time into spoken expressions in various languages.
 - Easy-to-use API with a simple and intuitive design.
 - Pure Python implementation with no external dependencies.
 - Extensible architecture for adding support for additional languages using the plugin design pattern.
-- Compatible with Python 3.8 and higher.
+- Compatible with Python 3.6 and higher.
 
 ## Installation
 
 You can install **Saa** using pip:
 
 ```shell
 pip install -U saa
@@ -97,18 +100,18 @@
 Prompt: `How many minutes are left before it is a quarter past twelve? Think step by step` 
 
 ![image](https://github.com/Proteusiq/saa/assets/14926709/5244c159-5fc3-4ac6-a9fa-829f9cf6ece6)
 
 </details>
 
 <details>
-  <summary>Adding New Language</summary>
+  <summary>Adding New Language 💾</summary>
 
-Using `Kiswahili` as an example as ABC of how to add a new language
- 1. Create a folder with  under the `saa/luga` directory, using the ISO 639-1 language code
+Using `Kiswahili` as an example of how to add a new language
+ 1. Create a folder under `saa/luga` directory, using the ISO 639-1 language code, with dunder init python file.
  ```bash
  mkdir saa/luga/sw && touch saa/luga/sw/__init__.py
  ```
 
  2. Contents of  `__init__.py` must have the following pattern
  ```python
 from dataclasses import dataclass
@@ -133,22 +136,22 @@
     ...
 
 class Language(Swahili):
     pass
 ...
 ```
 
-Since we are implementing `Luga`, our tasks now is to implement both the properties (`time`, `number_connector`, `connect_format`) and static methods (`time_logic`, `post_logic`).
+Since we are implementing `Luga`, our tasks now are to implement both the properties (`time`, `number_connector`, `connect_format`) and static methods (`time_logic`, `post_logic`).
 
-In Swahili `class`, time is expressed in terms of hour and then minutes. time_indicator
+In Swahili `class`, time is expressed in terms of hour first and then minutes. time_indicator is a placeholder for whatever changing logic, e.g. minute or minutes. For Swahili the logic is what part of the day it is, morning, noon, evenning or night.
 
 ```python
 time = {
-    "to": "saa {hour} na dakika {minute} time_indicator",
-    "past": "saa {hour} kasoro dakika {minute}time_indicator",
+    "past": "saa {hour} na dakika {minute} time_indicator",
+    "to": "saa {hour} kasoro dakika {minute} time_indicator",
     0: "saa {hour} time_indicator",
     15: "saa {hour} na robo time_indicator",
     45: "saa {hour} kasorobo time_indicator",
     30: "saa {hour} na nusu time_indicator",
 }
 ```
 
@@ -185,15 +188,15 @@
     20: "ishirini",
     30: "thelathini",
     40: "arobaini",
     50: "hamsini",
 }
 ```
 
-The major task is on time logic. In Swahili, 7 AM is the first hour in the morning, while 7 PM is the first hour in the evenning (jioni). 6 AM is the 12th hour in the morning ( asubuhi), while 6 PM is the 12th hour in the evenning.
+The major task is on time logic. In Swahili, 7 AM is the first hour in the morning (asubuhi), while 7 PM is the first hour in the evenning (jioni). 6 AM is the 12th hour in the morning ( asubuhi), while 6 PM is the 12th hour in the evenning(jioni).
 
 ```
 """
  0 - 11 asubuhi 
  12 - 15 mchana 
  16 - 19 jioni
  20 - 23 usiku 
@@ -233,14 +236,15 @@
 
 Time to write tests ...
 
 </details>
 
 
 ## Supported Languages
+![IMG_1009](https://github.com/Proteusiq/saa/assets/14926709/8562ac6e-eef6-4912-bfe8-b74141010f23)
 
 **Saa** currently supports the following languages:
 
 - English (`en`)
 - Danish (`da`)
 - Swahile(`sw`)
```

### Comparing `saa-0.0.5/pyproject.toml` & `saa-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saa"
-version = "0.0.5"
+version = "0.0.6"
 description = "Converting time into natural language phrases"
 authors = ["Prayson W. Daniel <praysonpi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.8.5"
```

### Comparing `saa-0.0.5/saa/clock.py` & `saa-0.0.6/saa/clock.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/saa/core/language.py` & `saa-0.0.6/saa/core/language.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/saa/core/numbers.py` & `saa-0.0.6/saa/core/numbers.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/saa/core/template.py` & `saa-0.0.6/saa/core/template.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/saa/core/watch.py` & `saa-0.0.6/saa/core/watch.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/saa/luga/da/__init__.py` & `saa-0.0.6/saa/luga/da/__init__.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/saa/luga/en/__init__.py` & `saa-0.0.6/saa/luga/en/__init__.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/saa/luga/sw/__init__.py` & `saa-0.0.6/saa/luga/sw/__init__.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.5/PKG-INFO` & `saa-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saa
-Version: 0.0.5
+Version: 0.0.6
 Summary: Converting time into natural language phrases
 License: MIT
 Author: Prayson W. Daniel
 Author-email: praysonpi@gmail.com
 Requires-Python: >3.8.5
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,23 +27,26 @@
 
 clock = Clock("en")
 clock("11:15") # 'quarter past eleven'
 
 ur = Clock("da")
 t = time(hour=7, minute=30)
 ur(t) # 'halvotte'
+
+muda = Clock("sw")
+muda("7:29") # 'saa moja na dakika ishirini na tisa asubuhi'
 ```
 
 ## Features
 
 - Convert time into spoken expressions in various languages.
 - Easy-to-use API with a simple and intuitive design.
 - Pure Python implementation with no external dependencies.
 - Extensible architecture for adding support for additional languages using the plugin design pattern.
-- Compatible with Python 3.8 and higher.
+- Compatible with Python 3.6 and higher.
 
 ## Installation
 
 You can install **Saa** using pip:
 
 ```shell
 pip install -U saa
@@ -112,18 +115,18 @@
 Prompt: `How many minutes are left before it is a quarter past twelve? Think step by step` 
 
 ![image](https://github.com/Proteusiq/saa/assets/14926709/5244c159-5fc3-4ac6-a9fa-829f9cf6ece6)
 
 </details>
 
 <details>
-  <summary>Adding New Language</summary>
+  <summary>Adding New Language 💾</summary>
 
-Using `Kiswahili` as an example as ABC of how to add a new language
- 1. Create a folder with  under the `saa/luga` directory, using the ISO 639-1 language code
+Using `Kiswahili` as an example of how to add a new language
+ 1. Create a folder under `saa/luga` directory, using the ISO 639-1 language code, with dunder init python file.
  ```bash
  mkdir saa/luga/sw && touch saa/luga/sw/__init__.py
  ```
 
  2. Contents of  `__init__.py` must have the following pattern
  ```python
 from dataclasses import dataclass
@@ -148,22 +151,22 @@
     ...
 
 class Language(Swahili):
     pass
 ...
 ```
 
-Since we are implementing `Luga`, our tasks now is to implement both the properties (`time`, `number_connector`, `connect_format`) and static methods (`time_logic`, `post_logic`).
+Since we are implementing `Luga`, our tasks now are to implement both the properties (`time`, `number_connector`, `connect_format`) and static methods (`time_logic`, `post_logic`).
 
-In Swahili `class`, time is expressed in terms of hour and then minutes. time_indicator
+In Swahili `class`, time is expressed in terms of hour first and then minutes. time_indicator is a placeholder for whatever changing logic, e.g. minute or minutes. For Swahili the logic is what part of the day it is, morning, noon, evenning or night.
 
 ```python
 time = {
-    "to": "saa {hour} na dakika {minute} time_indicator",
-    "past": "saa {hour} kasoro dakika {minute}time_indicator",
+    "past": "saa {hour} na dakika {minute} time_indicator",
+    "to": "saa {hour} kasoro dakika {minute} time_indicator",
     0: "saa {hour} time_indicator",
     15: "saa {hour} na robo time_indicator",
     45: "saa {hour} kasorobo time_indicator",
     30: "saa {hour} na nusu time_indicator",
 }
 ```
 
@@ -200,15 +203,15 @@
     20: "ishirini",
     30: "thelathini",
     40: "arobaini",
     50: "hamsini",
 }
 ```
 
-The major task is on time logic. In Swahili, 7 AM is the first hour in the morning, while 7 PM is the first hour in the evenning (jioni). 6 AM is the 12th hour in the morning ( asubuhi), while 6 PM is the 12th hour in the evenning.
+The major task is on time logic. In Swahili, 7 AM is the first hour in the morning (asubuhi), while 7 PM is the first hour in the evenning (jioni). 6 AM is the 12th hour in the morning ( asubuhi), while 6 PM is the 12th hour in the evenning(jioni).
 
 ```
 """
  0 - 11 asubuhi 
  12 - 15 mchana 
  16 - 19 jioni
  20 - 23 usiku 
@@ -248,14 +251,15 @@
 
 Time to write tests ...
 
 </details>
 
 
 ## Supported Languages
+![IMG_1009](https://github.com/Proteusiq/saa/assets/14926709/8562ac6e-eef6-4912-bfe8-b74141010f23)
 
 **Saa** currently supports the following languages:
 
 - English (`en`)
 - Danish (`da`)
 - Swahile(`sw`)
```

