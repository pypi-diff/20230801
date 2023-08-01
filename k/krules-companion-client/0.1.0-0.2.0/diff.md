# Comparing `tmp/krules_companion_client-0.1.0.tar.gz` & `tmp/krules_companion_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krules_companion_client-0.1.0.tar", max compression
+gzip compressed data, was "krules_companion_client-0.2.0.tar", max compression
```

## Comparing `krules_companion_client-0.1.0.tar` & `krules_companion_client-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-18 15:35:18.271901 krules_companion_client-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-18 15:35:18.271855 krules_companion_client-0.1.0/krules_companion_client/__init__.py
--rw-r--r--   0        0        0    13206 2023-07-27 15:57:07.552180 krules_companion_client-0.1.0/krules_companion_client/commands.py
--rw-r--r--   0        0        0      506 2023-07-26 09:11:17.090145 krules_companion_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 krules_companion_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 15:35:18.271901 krules_companion_client-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 15:35:18.271855 krules_companion_client-0.2.0/krules_companion_client/__init__.py
+-rw-r--r--   0        0        0    13220 2023-08-01 09:35:33.690139 krules_companion_client-0.2.0/krules_companion_client/commands.py
+-rw-r--r--   0        0        0      523 2023-08-01 09:36:34.593570 krules_companion_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 krules_companion_client-0.2.0/PKG-INFO
```

### Comparing `krules_companion_client-0.1.0/krules_companion_client/commands.py` & `krules_companion_client-0.2.0/krules_companion_client/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import typer
 from requests import HTTPError
 from rich.console import Console
 from rich import print
 from pathlib import Path
 from typing import Optional, List, Tuple, Any
 from typing_extensions import Annotated
-import tomllib
+#import tomllib
+import tomli
 import validators
 
 app = typer.Typer()
 
 err_console = Console(stderr=True)
 
 RE_TOPIC = re.compile("^projects/.*/topics/.*$")
@@ -255,15 +256,15 @@
     _check_defaults()
 
     tt_sum = sum(p is not None for p in [when, seconds, now])
     if tt_sum > 1:
         err_console.print("You can specify only one from --when, --seconds, --now")
         raise typer.Abort()
     if tt_sum == 0:
-        now=True
+        now = True
 
     if url is not None and not validators.url(url):
         err_console.print(f"'{url}' is not a valid URL")
         raise typer.Abort()
 
     if topic is not None and not RE_TOPIC.match(topic):
         err_console.print(f"'{topic}' is not a valid pubsub topic name")
@@ -332,15 +333,15 @@
                                                        help="Authentication key (override defaults)")] = None,
 ):
     global defaults
     if config != DEFAULT_CONFIG_FILE and not config.exists():
         err_console.print(f"config file '{config}' does not exists")
         raise typer.Abort()
     elif config.exists() and config.is_file():
-        defaults = tomllib.load(config.open("rb"))
+        defaults = tomli.load(config.open("rb"))
 
     if address is not None:
         defaults["addresss"] = address
     if subscription is not None:
         defaults["subscription"] = subscription
     if api_key is not None:
         defaults["api_key"] = api_key
```

### Comparing `krules_companion_client-0.1.0/PKG-INFO` & `krules_companion_client-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: krules-companion-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: KRules Companion Client
 Author: AdE
 Author-email: alberto@airspot.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
```

