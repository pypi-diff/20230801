# Comparing `tmp/syslog_ng_cfg_helper-1.0.7.tar.gz` & `tmp/syslog_ng_cfg_helper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syslog_ng_cfg_helper-1.0.7.tar", max compression
+gzip compressed data, was "syslog_ng_cfg_helper-1.1.0.tar", max compression
```

## Comparing `syslog_ng_cfg_helper-1.0.7.tar` & `syslog_ng_cfg_helper-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    35148 2023-07-21 11:44:07.511030 syslog_ng_cfg_helper-1.0.7/LICENSE
--rw-r--r--   0        0        0     2869 2023-07-21 11:44:07.511030 syslog_ng_cfg_helper-1.0.7/README.md
--rw-r--r--   0        0        0     1147 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/__init__.py
--rw-r--r--   0        0        0      941 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/build_db.py
--rw-r--r--   0        0        0     2486 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/console.py
--rw-r--r--   0        0        0      244 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/__init__.py
--rw-r--r--   0        0        0     3783 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/block.py
--rw-r--r--   0        0        0     1769 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/driver.py
--rw-r--r--   0        0        0     2263 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/driver_db.py
--rw-r--r--   0        0        0       42 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/exceptions.py
--rw-r--r--   0        0        0     2249 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/option.py
--rw-r--r--   0        0        0      479 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/utils.py
--rw-r--r--   0        0        0      893 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/globals.py
--rw-r--r--   0        0        0       75 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/__init__.py
--rw-r--r--   0        0        0     6094 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/load_modules.py
--rw-r--r--   0        0        0     4225 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/parse_sentence.py
--rw-r--r--   0        0        0   235140 2023-07-21 11:45:17.349223 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/syslog-ng-cfg-helper.db
--rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 syslog_ng_cfg_helper-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2288 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/README.md
+-rw-r--r--   0        0        0     1147 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/__init__.py
+-rw-r--r--   0        0        0      941 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/build_db.py
+-rw-r--r--   0        0        0     3299 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/console.py
+-rw-r--r--   0        0        0      244 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/driver_db/__init__.py
+-rw-r--r--   0        0        0     7846 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/driver_db/block.py
+-rw-r--r--   0        0        0     2964 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/driver_db/driver.py
+-rw-r--r--   0        0        0     6547 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/driver_db/driver_db.py
+-rw-r--r--   0        0        0       85 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/driver_db/exceptions.py
+-rw-r--r--   0        0        0     4747 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/driver_db/option.py
+-rw-r--r--   0        0        0     1387 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/driver_db/utils.py
+-rw-r--r--   0        0        0     1022 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/generate_diff.py
+-rw-r--r--   0        0        0      893 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/globals.py
+-rw-r--r--   0        0        0       75 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/module_loader/__init__.py
+-rw-r--r--   0        0        0     6094 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/module_loader/load_modules.py
+-rw-r--r--   0        0        0     4225 2023-08-01 16:59:16.032853 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/module_loader/parse_sentence.py
+-rw-r--r--   0        0        0   235140 2023-08-01 17:00:26.005705 syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/syslog-ng-cfg-helper.db
+-rw-r--r--   0        0        0     3230 1970-01-01 00:00:00.000000 syslog_ng_cfg_helper-1.1.0/PKG-INFO
```

### Comparing `syslog_ng_cfg_helper-1.0.7/LICENSE` & `syslog_ng_cfg_helper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.7/README.md` & `syslog_ng_cfg_helper-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,67 +11,28 @@
 pipx install syslog-ng-cfg-helper
 ```
 
 ### List the contexts
 ```
 syslog-ng-cfg-helper
 ```
-```
-Valid contexts:
-  destination
-  filter
-  options
-  parser
-  rewrite
-  source
-Print the drivers of CONTEXT with `--context CONTEXT`.
-```
 
 ### List the drivers in a context
 ```
-syslog-ng-cfg-helper -c destination
-```
-```
-Drivers of context 'destination':
-  amqp
-  example-destination
-  fifo
-  file
-  http
-  java
-...
-Print the options of DRIVER with `--context destination --driver DRIVER`.
+syslog-ng-cfg-helper --context parser
 ```
 
 ### List the options of a driver
 ```
-syslog-ng-cfg-helper -c destination -d http
-```
-```
-http(
-    accept-redirects(<yesno>)
-    azure-auth-header(
-        <path>(<string>)
-        content-type(<string>)
-        method(<string>)
-        secret(<string>)
-        workspace-id(<string>)
-    )
-    batch-bytes(<nonnegative-integer>)
-    batch-lines(<nonnegative-integer>)
-    batch-timeout(<positive-integer>)
-    body(<template-content>)
-    body-prefix(<string>)
-    body-suffix(<string>)
-    ca-dir(<string>)
-    ca-file(<path>)
-    cert-file(<path>)
-...
+syslog-ng-cfg-helper --context parser --driver csv-parser
 ```
 
+### Example
+[![Example](https://raw.githubusercontent.com/alltilla/syslog-ng-cfg-helper/assets/example.gif)](https://raw.githubusercontent.com/alltilla/syslog-ng-cfg-helper/assets/example.gif)
+
 ## Development
 The tool is still in development, but most of the drivers are supported.
 
 Missing features are:
   * Proper `rewrite` support.
   * Proper `filter` support.
   * Drivers defined in `SCL`s.
```

### Comparing `syslog_ng_cfg_helper-1.0.7/pyproject.toml` & `syslog_ng_cfg_helper-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "syslog-ng-cfg-helper"
-version = "1.0.7"
+version = "1.1.0"
 description = "Configuration helper for syslog-ng."
 authors = ["Attila Szakacs <szakacs.attila96@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://github.com/alltilla/syslog-ng-cfg-helper"
 repository = "https://github.com/alltilla/syslog-ng-cfg-helper"
 keywords = ["syslog-ng", "configuration", "cfg"]
```

### Comparing `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/build_db.py` & `syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/build_db.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/globals.py` & `syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/globals.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/load_modules.py` & `syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/module_loader/load_modules.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/parse_sentence.py` & `syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/module_loader/parse_sentence.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/syslog-ng-cfg-helper.db` & `syslog_ng_cfg_helper-1.1.0/syslog_ng_cfg_helper/syslog-ng-cfg-helper.db`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999668334597085%*

 * *Differences: {"'contexts'": "{'source': {'opentelemetry': {'blocks': {'auth': {'blocks': {'tls': {'options': "*

 * *               "{'peer-verify': {'params': {insert: [(2, ['required-untrusted']), (3, "*

 * *               "['optional-trusted'])], delete: [1, 0]}}}}}}}, 'options': {'flags': {'params': "*

 * *               "{insert: [(1, ['<empty>'])], delete: [0]}}}}, 'program': {'options': {'flags': "*

 * *               "{'params': {insert: [(2, ['<empty>'])], delete: [0]}}}}, 'mqtt': {'blocks': "*

 * *               "{'tls': {'blocks': {'c […]*

```diff
@@ -400,31 +400,31 @@
                                 ]
                             },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<empty>"
                                     ]
                                 ]
                             }
                         }
                     }
                 },
                 "context": "destination",
@@ -1068,51 +1068,51 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -1136,18 +1136,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -1187,18 +1187,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -1206,18 +1206,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pad-size": {
                         "name": "pad-size",
                         "params": [
                             [
@@ -1225,18 +1225,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -1515,29 +1515,29 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
@@ -1548,18 +1548,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -1591,18 +1591,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -1642,18 +1642,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -1677,18 +1677,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pad-size": {
                         "name": "pad-size",
                         "params": [
                             [
@@ -1696,18 +1696,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -1881,18 +1881,18 @@
                         "blocks": {},
                         "name": "cipher-suite",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "tls12-and-older": {
                                 "name": "tls12-and-older",
                                 "params": [
                                     [
@@ -2081,45 +2081,45 @@
                                 "blocks": {},
                                 "name": "options",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
                                                 "<string>",
                                                 "=>",
-                                                "<float>"
+                                                "<python-yesno>"
                                             ],
                                             [
                                                 "<string>",
                                                 "=>",
                                                 "[",
                                                 "<string-list>",
                                                 "]"
                                             ],
                                             [
-                                                "<string>"
-                                            ],
-                                            [
                                                 "<string>",
                                                 "=>",
-                                                "<python-yesno>"
+                                                "<number>"
                                             ],
                                             [
                                                 "<string>",
                                                 "=>",
-                                                "<number>"
+                                                "<string>"
                                             ],
                                             [
                                                 "<string>",
                                                 "=>",
-                                                "<string>"
+                                                "<float>"
+                                            ],
+                                            [
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "LogTemplate": {
                                         "name": "LogTemplate",
                                         "params": [
                                             [
@@ -2164,18 +2164,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -2490,35 +2490,35 @@
                             ]
                         ]
                     },
                     "response-action": {
                         "name": "response-action",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<positive-integer>",
                                 "=>",
-                                "success"
+                                "disconnect"
                             ],
                             [
                                 "<positive-integer>",
                                 "=>",
-                                "disconnect"
+                                "retry"
                             ],
                             [
                                 "<positive-integer>",
                                 "=>",
-                                "retry"
+                                "drop"
                             ],
                             [
                                 "<positive-integer>",
                                 "=>",
-                                "drop"
+                                "success"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "retries": {
                         "name": "retries",
                         "params": [
                             [
@@ -2853,41 +2853,41 @@
                             ]
                         ]
                     },
                     "option": {
                         "name": "option",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>",
                                 "<string-or-number>"
                             ],
                             [
                                 "<string>",
                                 "=>",
                                 "<string-or-number>"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "options": {
                         "name": "options",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>",
+                                "<string-or-number>"
                             ],
                             [
                                 "<string>",
                                 "=>",
                                 "<string-or-number>"
                             ],
                             [
-                                "<string>",
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -2959,24 +2959,24 @@
                         "blocks": {},
                         "name": "config",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>",
+                                        "<string-or-number>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<string-or-number>"
                                     ],
                                     [
-                                        "<string>",
-                                        "<string-or-number>"
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "<string>": {
                                 "name": "<string>",
                                 "params": [
                                     [
@@ -3688,31 +3688,31 @@
                                 ]
                             },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<empty>"
                                     ]
                                 ]
                             }
                         }
                     }
                 },
                 "context": "destination",
@@ -3878,24 +3878,24 @@
                             ]
                         ]
                     },
                     "write-concern": {
                         "name": "write-concern",
                         "params": [
                             [
-                                "<positive-integer>"
+                                "acked"
                             ],
                             [
-                                "acked"
+                                "unacked"
                             ],
                             [
                                 "majority"
                             ],
                             [
-                                "unacked"
+                                "<positive-integer>"
                             ]
                         ]
                     }
                 }
             },
             "mqtt": {
                 "blocks": {
@@ -4056,18 +4056,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -4532,18 +4532,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -4668,31 +4668,31 @@
                                     ]
                                 ]
                             },
                             "openssl-conf-cmds": {
                                 "name": "openssl-conf-cmds",
                                 "params": [
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
                                         "<string>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -4792,18 +4792,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -4931,18 +4931,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -5193,18 +5193,18 @@
                                             ]
                                         ]
                                     },
                                     "target-service-accounts": {
                                         "name": "target-service-accounts",
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     }
                                 }
                             },
                             "tls": {
                                 "blocks": {},
@@ -5675,51 +5675,51 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -5743,18 +5743,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -5794,18 +5794,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -5813,18 +5813,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pad-size": {
                         "name": "pad-size",
                         "params": [
                             [
@@ -5832,18 +5832,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -6114,18 +6114,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -6205,18 +6205,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -6750,45 +6750,45 @@
                         "blocks": {},
                         "name": "options",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<float>"
+                                        "<python-yesno>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "[",
                                         "<string-list>",
                                         "]"
                                     ],
                                     [
-                                        "<string>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
-                                        "<python-yesno>"
+                                        "<number>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<number>"
+                                        "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<string>"
+                                        "<float>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "LogTemplate": {
                                 "name": "LogTemplate",
                                 "params": [
                                     [
@@ -6998,31 +6998,31 @@
                                 ]
                             },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<empty>"
                                     ]
                                 ]
                             }
                         }
                     }
                 },
                 "context": "destination",
@@ -7699,31 +7699,31 @@
                                 ]
                             },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<empty>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "disk-buffer": {
                         "blocks": {},
@@ -9095,19 +9095,19 @@
                         ]
                     },
                     "dbd-option": {
                         "name": "dbd-option",
                         "params": [
                             [
                                 "<string>",
-                                "<number>"
+                                "<string>"
                             ],
                             [
                                 "<string>",
-                                "<string>"
+                                "<number>"
                             ]
                         ]
                     },
                     "dbi-driver-dir": {
                         "name": "dbi-driver-dir",
                         "params": [
                             [
@@ -9115,18 +9115,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -9703,31 +9703,31 @@
                                 ]
                             },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<empty>"
                                     ]
                                 ]
                             }
                         }
                     }
                 },
                 "context": "destination",
@@ -10099,18 +10099,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -10235,31 +10235,31 @@
                                     ]
                                 ]
                             },
                             "openssl-conf-cmds": {
                                 "name": "openssl-conf-cmds",
                                 "params": [
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
                                         "<string>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -10359,18 +10359,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -10498,18 +10498,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -10712,21 +10712,21 @@
                     "transport": {
                         "name": "transport",
                         "params": [
                             [
                                 "<string>"
                             ],
                             [
-                                "tcp"
+                                "udp"
                             ],
                             [
-                                "tls"
+                                "tcp"
                             ],
                             [
-                                "udp"
+                                "tls"
                             ]
                         ]
                     },
                     "truncate-size": {
                         "name": "truncate-size",
                         "params": [
                             [
@@ -10948,18 +10948,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -11084,31 +11084,31 @@
                                     ]
                                 ]
                             },
                             "openssl-conf-cmds": {
                                 "name": "openssl-conf-cmds",
                                 "params": [
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
                                         "<string>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -11208,18 +11208,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -11339,18 +11339,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -11756,18 +11756,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -11892,31 +11892,31 @@
                                     ]
                                 ]
                             },
                             "openssl-conf-cmds": {
                                 "name": "openssl-conf-cmds",
                                 "params": [
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
                                         "<string>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -12016,18 +12016,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -12147,18 +12147,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -12594,18 +12594,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -12725,18 +12725,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -13188,18 +13188,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -13319,18 +13319,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -13721,18 +13721,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -13804,18 +13804,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -14158,18 +14158,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "flush-lines": {
                         "name": "flush-lines",
                         "params": [
                             [
@@ -14241,18 +14241,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -14653,18 +14653,18 @@
                         "blocks": {},
                         "name": "delimiters",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "chars": {
                                 "name": "chars",
                                 "params": [
                                     [
@@ -14710,21 +14710,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
                                 "drop-invalid"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -14779,18 +14779,18 @@
                 "context": "parser",
                 "name": "date-parser",
                 "options": {
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -14861,18 +14861,18 @@
                             ]
                         ]
                     },
                     "inject-mode": {
                         "name": "inject-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -15117,18 +15117,18 @@
                             ]
                         ]
                     },
                     "inject-mode": {
                         "name": "inject-mode",
                         "params": [
                             [
-                                "<string>"
+                                "internal"
                             ],
                             [
-                                "internal"
+                                "<string>"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -15584,31 +15584,31 @@
                         ]
                     },
                     "pair": {
                         "name": "pair",
                         "params": [
                             [
                                 "<string>",
-                                ":",
                                 "<template-content>"
                             ],
                             [
                                 "<string>",
+                                ":",
                                 "<template-content>"
                             ]
                         ]
                     },
                     "scope": {
                         "name": "scope",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     }
                 }
             },
             "metrics-probe": {
                 "blocks": {},
@@ -15647,20 +15647,20 @@
                             ]
                         ]
                     },
                     "labels": {
                         "name": "labels",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>",
                                 "=>",
                                 "<template-content>"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "level": {
                         "name": "level",
                         "params": [
                             [
@@ -15747,45 +15747,45 @@
                         "blocks": {},
                         "name": "options",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<float>"
+                                        "<python-yesno>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "[",
                                         "<string-list>",
                                         "]"
                                     ],
                                     [
-                                        "<string>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
-                                        "<python-yesno>"
+                                        "<number>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<number>"
+                                        "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<string>"
+                                        "<float>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "LogTemplate": {
                                 "name": "LogTemplate",
                                 "params": [
                                     [
@@ -15846,18 +15846,18 @@
                 "context": "parser",
                 "name": "regexp-parser",
                 "options": {
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -16017,21 +16017,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "check-hostname"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -16382,18 +16382,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -16788,20 +16788,20 @@
                             ]
                         ]
                     },
                     "values": {
                         "name": "values",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>",
                                 "=>",
                                 "<template-content>"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     }
                 }
             },
             "example-random-generator": {
                 "blocks": {
@@ -16934,18 +16934,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -16953,18 +16953,18 @@
                             ]
                         ]
                     },
                     "freq": {
                         "name": "freq",
                         "params": [
                             [
-                                "<positive-integer>"
+                                "<float>"
                             ],
                             [
-                                "<float>"
+                                "<positive-integer>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -17252,29 +17252,29 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
@@ -17301,18 +17301,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
                                 "<empty>"
                             ]
                         ]
                     },
                     "format": {
@@ -17323,18 +17323,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -17454,18 +17454,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pad-size": {
                         "name": "pad-size",
                         "params": [
                             [
@@ -17700,40 +17700,40 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dns-cache": {
                         "name": "dns-cache",
                         "params": [
                             [
@@ -17749,21 +17749,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "check-hostname"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "follow-freq": {
                         "name": "follow-freq",
                         "params": [
                             [
@@ -17790,18 +17790,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -17921,18 +17921,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pad-size": {
                         "name": "pad-size",
                         "params": [
                             [
@@ -18118,18 +18118,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -18287,18 +18287,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -18569,18 +18569,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -18697,31 +18697,31 @@
                                     ]
                                 ]
                             },
                             "openssl-conf-cmds": {
                                 "name": "openssl-conf-cmds",
                                 "params": [
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
                                         "<string>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -18861,18 +18861,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
                                 "<empty>"
                             ]
                         ]
                     },
                     "format": {
@@ -19371,24 +19371,24 @@
                                             ]
                                         ]
                                     },
                                     "peer-verify": {
                                         "name": "peer-verify",
                                         "params": [
                                             [
-                                                "optional-trusted"
+                                                "optional-untrusted"
                                             ],
                                             [
-                                                "required-untrusted"
+                                                "required-trusted"
                                             ],
                                             [
-                                                "optional-untrusted"
+                                                "required-untrusted"
                                             ],
                                             [
-                                                "required-trusted"
+                                                "optional-trusted"
                                             ]
                                         ]
                                     }
                                 }
                             }
                         },
                         "name": "auth",
@@ -19532,18 +19532,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -19839,29 +19839,29 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
@@ -19888,18 +19888,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
                                 "<empty>"
                             ]
                         ]
                     },
                     "format": {
@@ -19910,18 +19910,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -20041,18 +20041,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pad-size": {
                         "name": "pad-size",
                         "params": [
                             [
@@ -20060,18 +20060,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -20303,21 +20303,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "check-hostname"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -20570,45 +20570,45 @@
                         "blocks": {},
                         "name": "options",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<float>"
+                                        "<python-yesno>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "[",
                                         "<string-list>",
                                         "]"
                                     ],
                                     [
-                                        "<string>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
-                                        "<python-yesno>"
+                                        "<number>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<number>"
+                                        "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<string>"
+                                        "<float>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "LogTemplate": {
                                 "name": "LogTemplate",
                                 "params": [
                                     [
@@ -20681,18 +20681,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -20921,45 +20921,45 @@
                         "blocks": {},
                         "name": "options",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<string>"
+                                        "<python-yesno>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "[",
                                         "<string-list>",
                                         "]"
                                     ],
                                     [
-                                        "<string>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
-                                        "<python-yesno>"
+                                        "<number>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<number>"
+                                        "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<float>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "LogTemplate": {
                                 "name": "LogTemplate",
                                 "params": [
                                     [
@@ -21043,18 +21043,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -21350,18 +21350,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -21644,40 +21644,40 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dns-cache": {
                         "name": "dns-cache",
                         "params": [
                             [
@@ -21693,18 +21693,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
                                 "<empty>"
                             ]
                         ]
                     },
                     "follow-freq": {
@@ -21734,18 +21734,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -21865,18 +21865,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pad-size": {
                         "name": "pad-size",
                         "params": [
                             [
@@ -21884,18 +21884,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -22274,18 +22274,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -22402,31 +22402,31 @@
                                     ]
                                 ]
                             },
                             "openssl-conf-cmds": {
                                 "name": "openssl-conf-cmds",
                                 "params": [
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
                                         "<string>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -22566,21 +22566,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "check-hostname"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -23141,20 +23141,20 @@
                             ]
                         ]
                     },
                     "matches": {
                         "name": "matches",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>",
                                 "=>",
                                 "<string>"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "max-field-size": {
                         "name": "max-field-size",
                         "params": [
                             [
@@ -23394,18 +23394,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
                                 "<empty>"
                             ]
                         ]
                     },
                     "format": {
@@ -23711,18 +23711,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -23839,31 +23839,31 @@
                                     ]
                                 ]
                             },
                             "openssl-conf-cmds": {
                                 "name": "openssl-conf-cmds",
                                 "params": [
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
                                         "<string>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -24003,21 +24003,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "check-hostname"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -24432,18 +24432,18 @@
                                 "blocks": {},
                                 "name": "cipher-suite",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<empty>"
                                             ]
                                         ]
                                     },
                                     "tls12-and-older": {
                                         "name": "tls12-and-older",
                                         "params": [
                                             [
@@ -24560,31 +24560,31 @@
                                     ]
                                 ]
                             },
                             "openssl-conf-cmds": {
                                 "name": "openssl-conf-cmds",
                                 "params": [
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>",
                                         "=>",
                                         "<string>"
+                                    ],
+                                    [
+                                        "<empty>"
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -24724,21 +24724,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "check-hostname"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -25218,21 +25218,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "check-hostname"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -25688,18 +25688,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
                                 "<empty>"
                             ]
                         ]
                     },
                     "format": {
@@ -26158,29 +26158,29 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
@@ -26234,18 +26234,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
                                 "<empty>"
                             ]
                         ]
                     },
                     "format": {
@@ -26256,18 +26256,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -26387,18 +26387,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pass-unix-credentials": {
                         "name": "pass-unix-credentials",
                         "params": [
                             [
@@ -26705,29 +26705,29 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
@@ -26781,21 +26781,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "check-hostname"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -26803,18 +26803,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -26934,18 +26934,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pass-unix-credentials": {
                         "name": "pass-unix-credentials",
                         "params": [
                             [
@@ -26953,18 +26953,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<empty>"
+                                "<number>"
                             ],
                             [
-                                "<number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -27244,29 +27244,29 @@
                             ]
                         ]
                     },
                     "dir-group": {
                         "name": "dir-group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-owner": {
                         "name": "dir-owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
@@ -27301,18 +27301,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
                                 "<empty>"
                             ]
                         ]
                     },
                     "follow-freq": {
@@ -27334,18 +27334,18 @@
                             ]
                         ]
                     },
                     "group": {
                         "name": "group",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -27481,18 +27481,18 @@
                             ]
                         ]
                     },
                     "owner": {
                         "name": "owner",
                         "params": [
                             [
-                                "<empty>"
+                                "<string-or-number>"
                             ],
                             [
-                                "<string-or-number>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "pad-size": {
                         "name": "pad-size",
                         "params": [
                             [
```

### Comparing `syslog_ng_cfg_helper-1.0.7/PKG-INFO` & `syslog_ng_cfg_helper-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syslog-ng-cfg-helper
-Version: 1.0.7
+Version: 1.1.0
 Summary: Configuration helper for syslog-ng.
 Home-page: https://github.com/alltilla/syslog-ng-cfg-helper
 License: GPL-3.0-only
 Keywords: syslog-ng,configuration,cfg
 Author: Attila Szakacs
 Author-email: szakacs.attila96@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -34,67 +34,28 @@
 pipx install syslog-ng-cfg-helper
 ```
 
 ### List the contexts
 ```
 syslog-ng-cfg-helper
 ```
-```
-Valid contexts:
-  destination
-  filter
-  options
-  parser
-  rewrite
-  source
-Print the drivers of CONTEXT with `--context CONTEXT`.
-```
 
 ### List the drivers in a context
 ```
-syslog-ng-cfg-helper -c destination
-```
-```
-Drivers of context 'destination':
-  amqp
-  example-destination
-  fifo
-  file
-  http
-  java
-...
-Print the options of DRIVER with `--context destination --driver DRIVER`.
+syslog-ng-cfg-helper --context parser
 ```
 
 ### List the options of a driver
 ```
-syslog-ng-cfg-helper -c destination -d http
-```
-```
-http(
-    accept-redirects(<yesno>)
-    azure-auth-header(
-        <path>(<string>)
-        content-type(<string>)
-        method(<string>)
-        secret(<string>)
-        workspace-id(<string>)
-    )
-    batch-bytes(<nonnegative-integer>)
-    batch-lines(<nonnegative-integer>)
-    batch-timeout(<positive-integer>)
-    body(<template-content>)
-    body-prefix(<string>)
-    body-suffix(<string>)
-    ca-dir(<string>)
-    ca-file(<path>)
-    cert-file(<path>)
-...
+syslog-ng-cfg-helper --context parser --driver csv-parser
 ```
 
+### Example
+[![Example](https://raw.githubusercontent.com/alltilla/syslog-ng-cfg-helper/assets/example.gif)](https://raw.githubusercontent.com/alltilla/syslog-ng-cfg-helper/assets/example.gif)
+
 ## Development
 The tool is still in development, but most of the drivers are supported.
 
 Missing features are:
   * Proper `rewrite` support.
   * Proper `filter` support.
   * Drivers defined in `SCL`s.
```

