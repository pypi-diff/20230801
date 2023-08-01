# Comparing `tmp/doctorr-0.0.1.tar.gz` & `tmp/doctorr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctorr-0.0.1.tar", last modified: Fri Jul 28 13:53:59 2023, max compression
+gzip compressed data, was "doctorr-0.1.0.tar", last modified: Tue Aug  1 14:06:24 2023, max compression
```

## Comparing `doctorr-0.0.1.tar` & `doctorr-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:53:59.369997 doctorr-0.0.1/
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-28 13:53:59.369997 doctorr-0.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      243 2023-07-28 13:53:14.000000 doctorr-0.0.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      242 2023-07-28 13:53:14.000000 doctorr-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 13:53:59.369997 doctorr-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:53:59.365997 doctorr-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:53:59.365997 doctorr-0.0.1/src/doctorr/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       68 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:53:59.369997 doctorr-0.0.1/src/doctorr/autocli/
--rw-rw-r--   0 root         (0) root         (0)       59 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autocli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      214 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autocli/__main__.py
--rw-rw-r--   0 root         (0) root         (0)      283 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autocli/inspection.py
--rw-rw-r--   0 root         (0) root         (0)     2451 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autocli/parse_argparse.py
--rw-rw-r--   0 root         (0) root         (0)      644 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autocli/parse_config.py
--rw-rw-r--   0 root         (0) root         (0)     1364 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autocli/run.py
--rw-rw-r--   0 root         (0) root         (0)       91 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autocli/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:53:59.369997 doctorr-0.0.1/src/doctorr/autodoc/
--rw-rw-r--   0 root         (0) root         (0)       59 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autodoc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7527 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autodoc/docstring.py
--rw-rw-r--   0 root         (0) root         (0)     3473 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autodoc/inspection.py
--rw-rw-r--   0 root         (0) root         (0)     1719 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autodoc/parse_config.py
--rw-rw-r--   0 root         (0) root         (0)     1493 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autodoc/run.py
--rw-rw-r--   0 root         (0) root         (0)     2201 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/autodoc/templates.py
--rw-rw-r--   0 root         (0) root         (0)     2575 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/cli.py
--rw-rw-r--   0 root         (0) root         (0)      186 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/parse_config.py
--rw-rw-r--   0 root         (0) root         (0)      736 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/templates.py
--rw-rw-r--   0 root         (0) root         (0)     2031 2023-07-28 13:53:14.000000 doctorr-0.0.1/src/doctorr/watchmode.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:53:59.365997 doctorr-0.0.1/src/doctorr.egg-info/
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-28 13:53:59.000000 doctorr-0.0.1/src/doctorr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-28 13:53:59.000000 doctorr-0.0.1/src/doctorr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 13:53:59.000000 doctorr-0.0.1/src/doctorr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 13:53:59.000000 doctorr-0.0.1/src/doctorr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 13:53:59.000000 doctorr-0.0.1/src/doctorr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.533500 doctorr-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 14:06:24.533500 doctorr-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-01 14:06:15.000000 doctorr-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 14:06:15.000000 doctorr-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:06:24.533500 doctorr-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.529499 doctorr-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.529499 doctorr-0.1.0/src/doctorr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.533500 doctorr-0.1.0/src/doctorr/autocli/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/parse_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autocli/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.533500 doctorr-0.1.0/src/doctorr/autodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/autodoc/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/parse_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-01 14:06:15.000000 doctorr-0.1.0/src/doctorr/watchmode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:06:24.533500 doctorr-0.1.0/src/doctorr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 14:06:24.000000 doctorr-0.1.0/src/doctorr.egg-info/top_level.txt
```

### Comparing `doctorr-0.0.1/src/doctorr/autocli/parse_argparse.py` & `doctorr-0.1.0/src/doctorr/autocli/parse_argparse.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.0.1/src/doctorr/autocli/parse_config.py` & `doctorr-0.1.0/src/doctorr/autocli/parse_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import List, Optional
 
+from doctorr.include import IncludeConfig
 from doctorr.parse_config import _parse_yaml, _read_file
 
 
 @dataclass
 class CLIConfig:
     module_source: str
     getter: str
     prog: str
     output_name: str
     output_dir: Optional[Path] = None
     watch: List[str] = field(default_factory=list)
+    include: List[IncludeConfig] = field(default_factory=list)
 
     def __post_init__(self):
         self.output_dir = self.output_dir and Path(self.output_dir)
 
 
 def main(config_path):
     file_content = _read_file(config_path)
```

### Comparing `doctorr-0.0.1/src/doctorr/autocli/run.py` & `doctorr-0.1.0/src/doctorr/autocli/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from enum import Enum
 from shutil import rmtree
 
 from doctorr.autocli.inspection import get_parser
 from doctorr.autocli.parse_argparse import parse_parser
 from doctorr.autocli.parse_config import main as read_config
 from doctorr.autocli.templates import render_cli
+from doctorr.include import run_include
+from doctorr.parse_config import parse_include_config
 from doctorr.templates import TemplateRenderer
 from doctorr.watchmode import main as watchmode
 
 
 class AutoCliDefault(Enum):
     CONFIG_PATH = "./doctorr.yml"
     THEME = "md_basic"
@@ -30,12 +32,15 @@
     output_dir = output_dir or config.output_dir
     assert output_dir, "Please provide through cli or through the yaml"
 
     rmtree(output_dir, ignore_errors=True)
     output_dir.mkdir(parents=True, exist_ok=True)
     (output_dir / config.output_name).write_text(text)
 
+    include_configs = parse_include_config(config)
+    run_include(include_configs)
+
 
 def generate_cli_documentation(parser, renderer):
     parsed_data = parse_parser(parser)
     markdown_doc = render_cli(parsed_data, renderer)
     return markdown_doc
```

### Comparing `doctorr-0.0.1/src/doctorr/autodoc/docstring.py` & `doctorr-0.1.0/src/doctorr/autodoc/docstring.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.0.1/src/doctorr/autodoc/inspection.py` & `doctorr-0.1.0/src/doctorr/autodoc/inspection.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.0.1/src/doctorr/autodoc/parse_config.py` & `doctorr-0.1.0/src/doctorr/autodoc/parse_config.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.0.1/src/doctorr/autodoc/run.py` & `doctorr-0.1.0/src/doctorr/autodoc/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from shutil import rmtree
 
 from doctorr.autodoc.docstring import process_page
 from doctorr.autodoc.inspection import import_and_inspect
 from doctorr.autodoc.parse_config import main as parse_config
 from doctorr.autodoc.parse_config import parse_output_dir, parse_page_configs
 from doctorr.autodoc.templates import render_page
+from doctorr.include import run_include
+from doctorr.parse_config import parse_include_config
 from doctorr.templates import TemplateRenderer
 from doctorr.watchmode import main as watchmode
 
 
 class AutoDocDefault(Enum):
     CONFIG_PATH = "./doctorr.yml"
     THEME = "md_basic"
@@ -32,7 +34,10 @@
 
     output_dir = output_dir or parse_output_dir(config)
 
     rmtree(output_dir, ignore_errors=True)
     output_dir.mkdir(parents=True, exist_ok=True)
     for page, text in zip(processed_pages, rendered_pages):
         (output_dir / page.output_name).write_text(text)
+
+    include_configs = parse_include_config(config)
+    run_include(include_configs)
```

### Comparing `doctorr-0.0.1/src/doctorr/autodoc/templates.py` & `doctorr-0.1.0/src/doctorr/autodoc/templates.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.0.1/src/doctorr/cli.py` & `doctorr-0.1.0/src/doctorr/cli.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.0.1/src/doctorr/templates.py` & `doctorr-0.1.0/src/doctorr/templates.py`

 * *Files identical despite different names*

### Comparing `doctorr-0.0.1/src/doctorr/watchmode.py` & `doctorr-0.1.0/src/doctorr/watchmode.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import time
 from threading import Timer
 
 from watchdog.events import FileModifiedEvent, FileSystemEventHandler
 from watchdog.observers import Observer
 
+from doctorr.utils import _get
+
 
 def debounce(wait):
     """Decorator that will postpone a functions
     execution until after wait seconds
     have elapsed since the last time it was invoked."""
 
     def decorator(fn):
@@ -23,24 +25,14 @@
             debounced.t.start()
 
         return debounced
 
     return decorator
 
 
-def _get(key, obj):
-    # bad design:
-    # config["watch"] in autodoc
-    # config.watch in autocli
-    # this works around this bad design
-    if isinstance(obj, dict):
-        return obj[key]
-    return getattr(obj, key)
-
-
 def main(func, config):
     @debounce(0.1)
     def build_doc():
         # watchdog sees more events than actually happen,
         # this makes sure it runs once
         print("rebuilding...")
         func()
```

### Comparing `doctorr-0.0.1/src/doctorr.egg-info/SOURCES.txt` & `doctorr-0.1.0/src/doctorr.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 README.md
 pyproject.toml
 src/doctorr/__init__.py
 src/doctorr/__main__.py
 src/doctorr/cli.py
+src/doctorr/include.py
 src/doctorr/parse_config.py
 src/doctorr/templates.py
+src/doctorr/utils.py
 src/doctorr/watchmode.py
 src/doctorr.egg-info/PKG-INFO
 src/doctorr.egg-info/SOURCES.txt
 src/doctorr.egg-info/dependency_links.txt
 src/doctorr.egg-info/requires.txt
 src/doctorr.egg-info/top_level.txt
 src/doctorr/autocli/__init__.py
```

