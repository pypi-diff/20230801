# Comparing `tmp/htmx-components-python-0.0.1.tar.gz` & `tmp/htmx-components-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmx-components-python-0.0.1.tar", last modified: Wed Jul 26 00:06:43 2023, max compression
+gzip compressed data, was "htmx-components-python-0.0.2.tar", last modified: Tue Aug  1 21:39:38 2023, max compression
```

## Comparing `htmx-components-python-0.0.1.tar` & `htmx-components-python-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:06:43.062289 htmx-components-python-0.0.1/
--rw-rw-r--   0 neil      (1000) neil      (1000)       45 2023-07-26 00:02:13.000000 htmx-components-python-0.0.1/.gitignore
--rw-rw-r--   0 neil      (1000) neil      (1000)      176 2023-07-26 00:06:43.062289 htmx-components-python-0.0.1/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)      323 2023-07-25 23:21:10.000000 htmx-components-python-0.0.1/pyproject.toml
--rw-rw-r--   0 neil      (1000) neil      (1000)       38 2023-07-26 00:06:43.062289 htmx-components-python-0.0.1/setup.cfg
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:06:43.058289 htmx-components-python-0.0.1/src/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:06:43.058289 htmx-components-python-0.0.1/src/htmx_components_python/
--rw-rw-r--   0 neil      (1000) neil      (1000)      887 2023-07-25 23:27:25.000000 htmx-components-python-0.0.1/src/htmx_components_python/__init__.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-07-26 00:06:43.062289 htmx-components-python-0.0.1/src/htmx_components_python.egg-info/
--rw-rw-r--   0 neil      (1000) neil      (1000)      176 2023-07-26 00:06:43.000000 htmx-components-python-0.0.1/src/htmx_components_python.egg-info/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)      264 2023-07-26 00:06:43.000000 htmx-components-python-0.0.1/src/htmx_components_python.egg-info/SOURCES.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-07-26 00:06:43.000000 htmx-components-python-0.0.1/src/htmx_components_python.egg-info/dependency_links.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)       23 2023-07-26 00:06:43.000000 htmx-components-python-0.0.1/src/htmx_components_python.egg-info/top_level.txt
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:39:38.795361 htmx-components-python-0.0.2/
+-rw-rw-r--   0 neil      (1000) neil      (1000)       52 2023-07-26 00:06:53.000000 htmx-components-python-0.0.2/.gitignore
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1069 2023-08-01 21:36:18.000000 htmx-components-python-0.0.2/LICENSE
+-rw-rw-r--   0 neil      (1000) neil      (1000)      236 2023-08-01 21:39:38.795361 htmx-components-python-0.0.2/PKG-INFO
+-rw-rw-r--   0 neil      (1000) neil      (1000)      385 2023-08-01 21:39:09.000000 htmx-components-python-0.0.2/pyproject.toml
+-rw-rw-r--   0 neil      (1000) neil      (1000)       38 2023-08-01 21:39:38.795361 htmx-components-python-0.0.2/setup.cfg
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:39:38.783360 htmx-components-python-0.0.2/src/
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:39:38.787361 htmx-components-python-0.0.2/src/htmx_components_python/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1581 2023-08-01 20:15:37.000000 htmx-components-python-0.0.2/src/htmx_components_python/__init__.py
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-08-01 21:39:38.791360 htmx-components-python-0.0.2/src/htmx_components_python.egg-info/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      236 2023-08-01 21:39:38.000000 htmx-components-python-0.0.2/src/htmx_components_python.egg-info/PKG-INFO
+-rw-rw-r--   0 neil      (1000) neil      (1000)      272 2023-08-01 21:39:38.000000 htmx-components-python-0.0.2/src/htmx_components_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-08-01 21:39:38.000000 htmx-components-python-0.0.2/src/htmx_components_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)       23 2023-08-01 21:39:38.000000 htmx-components-python-0.0.2/src/htmx_components_python.egg-info/top_level.txt
```

### Comparing `htmx-components-python-0.0.1/src/htmx_components_python/__init__.py` & `htmx-components-python-0.0.2/src/htmx_components_python/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 from __future__ import annotations
 
 import typing as t
 from abc import abstractstaticmethod
 from dataclasses import dataclass, field
+from enum import Enum
+
+
+@dataclass
+class TreeConfig:
+    data: t.Callable | list
+    lazy: bool = False
+    prefix: str = ""
+    key_attr: str = "id"
+    text_attr: str = "name"
+    parent_id_attr: str = "parent_id"
+    render_node: t.Callable[[t.Mapping], str] = lambda item: item["name"]
+    htmx_endpoint: str = ""
+    search: bool = True
+    toggle_all: bool = True
+    expand_icon: str = "bi-caret-right-fill text-secondary"
+    collapse_icon: str = "bi-caret-down-fill text-secondary"
+
+    def __post_init__(self):
+        if self.prefix and not self.prefix.endswith("-"):
+            self.prefix = f"{self.prefix}-"
 
 
 @dataclass
 class Column:
     attr: str
     text: str = ""
     render: t.Callable = str
@@ -34,7 +55,13 @@
     def get_records(
         page: int = 1,
         page_size: int = 20,
         sorts=list[tuple[str, str]],
         q: str = "",
     ) -> tuple[t.Iterable[t.Any], int]:
         ...
+
+
+class SelectionMode(Enum):
+    NONE = 0
+    SINGLE = 1
+    MULTI = 2
```

