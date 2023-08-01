# Comparing `tmp/efrem_utils-0.1.1.tar.gz` & `tmp/efrem_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.1.1.tar", max compression
+gzip compressed data, was "efrem_utils-0.1.3.tar", max compression
```

## Comparing `efrem_utils-0.1.1.tar` & `efrem_utils-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2676 2023-07-17 12:25:28.408764 efrem_utils-0.1.1/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.1.1/LICENSE
--rw-r--r--   0        0        0      361 2023-07-17 12:23:38.859527 efrem_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3008 2023-07-17 12:30:21.529798 efrem_utils-0.1.1/README.md
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4210 2023-08-01 19:52:25.082605 efrem_utils-0.1.3/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.1.3/LICENSE
+-rw-r--r--   0        0        0      361 2023-08-01 19:52:23.175320 efrem_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.1.3/README.md
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.1.3/PKG-INFO
```

### Comparing `efrem_utils-0.1.1/LICENSE` & `efrem_utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.1.1/README.md` & `efrem_utils-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # `efrem-utils`
 
-A package with utility functions to abstract some logic. 
+A package with utility functions to abstract some logic.
 
 ## `explanation`
 
-### `validated_input` usage:
+### `validated_input` usage
 
 The `validated_input` exists to simplify getting a valid input from a user that passes some criterias.
 
 Its signature/definition might be a bit hard to read, so a bit of an explanation:
+
 ```py
 ---
 msg: A string / None (by default), will be used as the prompt for the input() calls.
 If its None - it defaults to f"Enter a {constructor}: "
 ---
 precomp(utational function): A function which has to take a string and return.. anything, pretty much.
 Honourable mentions: str.strip, str.lower, str.split. Defaults to None so it doesnt mutate the input.
@@ -49,8 +50,8 @@
     validators=[
         (lambda buffer: buffer in choices, "{buffer} is not a valid choice") # the {buffer} in the template string is important
     ],
     precomp=lambda buffer: buffer.lower().strip() # using lambda to combine multiple precomputation functions
 )
 ```
 
-**For more information check:** [`examples directory`](https://github.com/NikitaNightBot/efrem-utils/tree/main/examples)
+**For more information check:** [`examples directory`](https://github.com/NikitaNightBot/efrem-utils/tree/main/examples)
```

### Comparing `efrem_utils-0.1.1/PKG-INFO` & `efrem_utils-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: efrem-utils
-Version: 0.1.1
+Version: 0.1.3
 Summary: Efrem's utilities
 Home-page: https://github.com/NikitaNightBot/efrem-utils
 Author: lone_druid
 Author-email: enikita332@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/NikitaNightBot/efrem-utils
 Description-Content-Type: text/markdown
 
 # `efrem-utils`
 
-A package with utility functions to abstract some logic. 
+A package with utility functions to abstract some logic.
 
 ## `explanation`
 
-### `validated_input` usage:
+### `validated_input` usage
 
 The `validated_input` exists to simplify getting a valid input from a user that passes some criterias.
 
 Its signature/definition might be a bit hard to read, so a bit of an explanation:
+
 ```py
 ---
 msg: A string / None (by default), will be used as the prompt for the input() calls.
 If its None - it defaults to f"Enter a {constructor}: "
 ---
 precomp(utational function): A function which has to take a string and return.. anything, pretty much.
 Honourable mentions: str.strip, str.lower, str.split. Defaults to None so it doesnt mutate the input.
@@ -63,7 +64,8 @@
         (lambda buffer: buffer in choices, "{buffer} is not a valid choice") # the {buffer} in the template string is important
     ],
     precomp=lambda buffer: buffer.lower().strip() # using lambda to combine multiple precomputation functions
 )
 ```
 
 **For more information check:** [`examples directory`](https://github.com/NikitaNightBot/efrem-utils/tree/main/examples)
+
```

