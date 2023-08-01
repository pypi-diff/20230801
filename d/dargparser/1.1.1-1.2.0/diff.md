# Comparing `tmp/dargparser-1.1.1.tar.gz` & `tmp/dargparser-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dargparser-1.1.1.tar", last modified: Thu Mar 30 12:11:12 2023, max compression
+gzip compressed data, was "dargparser-1.2.0.tar", last modified: Tue Aug  1 15:01:06 2023, max compression
```

## Comparing `dargparser-1.1.1.tar` & `dargparser-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:11:12.185512 dargparser-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:11:12.181512 dargparser-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:11:12.185512 dargparser-1.1.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2546 2023-03-30 12:10:58.000000 dargparser-1.1.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:11:12.185512 dargparser-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-30 12:10:58.000000 dargparser-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-30 12:10:58.000000 dargparser-1.1.1/.github/workflows/release_major.yml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-30 12:10:58.000000 dargparser-1.1.1/.github/workflows/release_minor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-30 12:10:58.000000 dargparser-1.1.1/.github/workflows/release_patch.yml
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-30 12:10:58.000000 dargparser-1.1.1/.github/workflows/test_all.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-30 12:10:58.000000 dargparser-1.1.1/.github/workflows/test_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-30 12:10:58.000000 dargparser-1.1.1/.github/workflows/test_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-30 12:10:58.000000 dargparser-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-30 12:10:58.000000 dargparser-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-03-30 12:11:12.185512 dargparser-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-03-30 12:10:58.000000 dargparser-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-30 12:10:58.000000 dargparser-1.1.1/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-30 12:10:58.000000 dargparser-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-30 12:11:12.185512 dargparser-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:11:12.181512 dargparser-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:11:12.185512 dargparser-1.1.1/src/dargparser/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-30 12:10:58.000000 dargparser-1.1.1/src/dargparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-03-30 12:10:58.000000 dargparser-1.1.1/src/dargparser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18572 2023-03-30 12:10:58.000000 dargparser-1.1.1/src/dargparser/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-30 12:10:58.000000 dargparser-1.1.1/src/dargparser/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:11:12.185512 dargparser-1.1.1/src/dargparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-03-30 12:11:12.000000 dargparser-1.1.1/src/dargparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-30 12:11:12.000000 dargparser-1.1.1/src/dargparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 12:11:12.000000 dargparser-1.1.1/src/dargparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-30 12:11:12.000000 dargparser-1.1.1/src/dargparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-30 12:11:12.000000 dargparser-1.1.1/src/dargparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-30 12:11:12.000000 dargparser-1.1.1/src/dargparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 12:11:11.000000 dargparser-1.1.1/src/dargparser.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 12:11:12.185512 dargparser-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-03-30 12:10:58.000000 dargparser-1.1.1/tests/test_dargparser_huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:06.546554 dargparser-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:06.542554 dargparser-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:06.546554 dargparser-1.2.0/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2546 2023-08-01 15:00:57.000000 dargparser-1.2.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:06.546554 dargparser-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 15:00:57.000000 dargparser-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 15:00:57.000000 dargparser-1.2.0/.github/workflows/release_major.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 15:00:57.000000 dargparser-1.2.0/.github/workflows/release_minor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 15:00:57.000000 dargparser-1.2.0/.github/workflows/release_patch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 15:00:57.000000 dargparser-1.2.0/.github/workflows/test_all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-01 15:00:57.000000 dargparser-1.2.0/.github/workflows/test_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 15:00:57.000000 dargparser-1.2.0/.github/workflows/test_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-01 15:00:57.000000 dargparser-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 15:00:57.000000 dargparser-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-01 15:01:06.546554 dargparser-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-01 15:00:57.000000 dargparser-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-01 15:00:57.000000 dargparser-1.2.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 15:00:57.000000 dargparser-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 15:01:06.550554 dargparser-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:06.546554 dargparser-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:06.546554 dargparser-1.2.0/src/dargparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 15:00:57.000000 dargparser-1.2.0/src/dargparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-01 15:00:57.000000 dargparser-1.2.0/src/dargparser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19036 2023-08-01 15:00:57.000000 dargparser-1.2.0/src/dargparser/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-01 15:00:57.000000 dargparser-1.2.0/src/dargparser/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:06.546554 dargparser-1.2.0/src/dargparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-01 15:01:06.000000 dargparser-1.2.0/src/dargparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 15:01:06.000000 dargparser-1.2.0/src/dargparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:01:06.000000 dargparser-1.2.0/src/dargparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 15:01:06.000000 dargparser-1.2.0/src/dargparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 15:01:06.000000 dargparser-1.2.0/src/dargparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 15:01:06.000000 dargparser-1.2.0/src/dargparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:01:06.000000 dargparser-1.2.0/src/dargparser.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:01:06.546554 dargparser-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-08-01 15:00:57.000000 dargparser-1.2.0/tests/test_dargparser_huggingface.py
```

### Comparing `dargparser-1.1.1/.github/scripts/release.py` & `dargparser-1.2.0/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/.github/workflows/test_all.yml` & `dargparser-1.2.0/.github/workflows/test_all.yml`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/.github/workflows/test_publish.yml` & `dargparser-1.2.0/.github/workflows/test_publish.yml`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/.github/workflows/test_ubuntu.yml` & `dargparser-1.2.0/.github/workflows/test_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/.gitignore` & `dargparser-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/LICENSE` & `dargparser-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/PKG-INFO` & `dargparser-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargparser
-Version: 1.1.1
+Version: 1.2.0
 Summary: A lean and hackable typed argument parser for Python.
 Home-page: https://github.com/konstantinjdobler/dargparser
 Project-URL: Bug Tracker, https://github.com/konstantinjdobler/dargparser/issues
 Project-URL: Changelog, https://github.com/konstantinjdobler/dargparser/releases
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dargparser-1.1.1/README.md` & `dargparser-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/example.py` & `dargparser-1.2.0/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Literal
 
-from dargparser import Choice, dArg, dargparse
+from src.dargparser import Choice, dArg, dargparse
 
 # flake8 doesn't like Choice with strings, you can use Literal instead.
 # flake8: noqa
 
 
 @dataclass
 class Args:
     epochs: int
     learning_rate: float = dArg(aliases="--lr", help="Required argument (no default).")
-    data_path: str = dArg(default="./data/", aliases=["--data", "-d"])
+    data_path: Path = dArg(default="./data/", aliases=["--data", "-d"], parsing_function=lambda x: Path(x).resolve())
     # str | None syntax is only available in Python >=3.10. Use Optional[str] for older versions.
     extra_data: str | None = dArg(default=None)
     cuda: bool = dArg(default=True, help="We automatically create a `--no_<arg>` flag for bools.")
     precision: Choice[32, 16, 8, "bf16", "tf32"] = dArg(default=32, help="Choices with mixed types are supported.")
     some_list_arg: list[int] = dArg(default=[1, 2, 3])
     evaluation_datasets: list[Choice["xnli", "tydiqa", "wikiann", "squad"]] = dArg(
         default=["xnli", "wikiann"], help="Select arbitrary number of datasets to evaluate on."
     )
+    complex_arg: tuple[int, list[str]] = dArg(
+        default=(1, ["a", "b"]), parsing_function=lambda x: (int(x.split(",")[0]), x.split(",")[1:])
+    )
 
 
 @dataclass
 class LoggingArgs:
     log_dir: str | None = dArg(default=None)
     log_backends: list[Choice["wandb", "tensorboard", "neptune"]] = dArg(default=["wandb"])
     # Choice is just an alias for Literal to be more descriptive.
```

### Comparing `dargparser-1.1.1/setup.cfg` & `dargparser-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/src/dargparser/helpers.py` & `dargparser-1.2.0/src/dargparser/helpers.py`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/src/dargparser/parsing.py` & `dargparser-1.2.0/src/dargparser/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 def dArg(
     *,
     default: Any = dataclasses.MISSING,
     aliases: Union[str, List[str]] = None,
     help: str = None,
     default_factory: Callable[[], Any] = dataclasses.MISSING,
     metadata: dict = None,
+    parsing_function: Callable[[str], Any] = None,
     **kwargs,
 ) -> dataclasses.Field:
     """
     Example using the `dArgParser` and `dArg`:
     ```
     from dargparse import dargparse, dArg
 
@@ -127,14 +128,16 @@
     if metadata is None:
         # Important, don't use as default param in function signature because dict is mutable and shared across function calls
         metadata = {}
     if aliases is not None:
         metadata["aliases"] = aliases
     if help is not None:
         metadata["help"] = help
+    if parsing_function is not None:
+        metadata["parsing_function"] = parsing_function
 
     # Catch list default values here and redirect to default_factory
     if isinstance(default, list):
         default_copy = copy(default)
         default_factory = lambda: default_copy  # noqa: E731
         default = dataclasses.MISSING
     return dataclasses.field(metadata=metadata, default=default, default_factory=default_factory, **kwargs)
@@ -177,14 +180,19 @@
         # it is provided as a third-party extension mechanism.
         if isinstance(field.type, str):
             raise RuntimeError(
                 "Unresolved type detected, which should have been done with the help of "
                 "`typing.get_type_hints` method by default"
             )
 
+        parsing_function = kwargs.pop("parsing_function", None)
+        if parsing_function is not None:
+            parsing_function_return_type = field.type
+            field.type = parsing_function
+
         aliases = kwargs.pop("aliases", [])
         if isinstance(aliases, str):
             aliases = [aliases]
 
         origin_type = getattr(field.type, "__origin__", field.type)
         if origin_type is Union:
             if str not in field.type.__args__ and (len(field.type.__args__) != 2 or type(None) not in field.type.__args__):
@@ -273,14 +281,16 @@
             if field.default is not dataclasses.MISSING:
                 kwargs["default"] = field.default
             elif field.default_factory is not dataclasses.MISSING:
                 kwargs["default"] = field.default_factory()
             else:
                 kwargs["required"] = True
             type_str = field.type.__name__.upper()
+            if parsing_function is not None:
+                type_str = parsing_function_return_type.__name__.upper()
 
         parser.add_argument(field_name, *aliases, **kwargs, metavar=type_str)
 
         # Add a complement `no_*` argument for a boolean field AFTER the initial field has already been added.
         # Order is important for arguments with the same destination!
         # We use a copy of earlier kwargs because the original kwargs have changed a lot before reaching down
         # here and we do not need those changes/additional keys.
```

### Comparing `dargparser-1.1.1/src/dargparser.egg-info/PKG-INFO` & `dargparser-1.2.0/src/dargparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargparser
-Version: 1.1.1
+Version: 1.2.0
 Summary: A lean and hackable typed argument parser for Python.
 Home-page: https://github.com/konstantinjdobler/dargparser
 Project-URL: Bug Tracker, https://github.com/konstantinjdobler/dargparser/issues
 Project-URL: Changelog, https://github.com/konstantinjdobler/dargparser/releases
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dargparser-1.1.1/src/dargparser.egg-info/SOURCES.txt` & `dargparser-1.2.0/src/dargparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dargparser-1.1.1/tests/test_dargparser_huggingface.py` & `dargparser-1.2.0/tests/test_dargparser_huggingface.py`

 * *Files identical despite different names*

