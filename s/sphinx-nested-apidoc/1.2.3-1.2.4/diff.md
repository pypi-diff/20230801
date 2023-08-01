# Comparing `tmp/sphinx_nested_apidoc-1.2.3.tar.gz` & `tmp/sphinx_nested_apidoc-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_nested_apidoc-1.2.3.tar", max compression
+gzip compressed data, was "sphinx_nested_apidoc-1.2.4.tar", max compression
```

## Comparing `sphinx_nested_apidoc-1.2.3.tar` & `sphinx_nested_apidoc-1.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/LICENSE
--rw-r--r--   0        0        0    10887 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/README.rst
--rw-r--r--   0        0        0     2321 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/pyproject.toml
--rw-r--r--   0        0        0      730 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/__init__.py
--rw-r--r--   0        0        0     4088 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/__main__.py
--rw-r--r--   0        0        0     3145 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/_ext.py
--rw-r--r--   0        0        0    10848 2023-05-27 14:48:23.868826 sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/core.py
--rw-r--r--   0        0        0    11949 1970-01-01 00:00:00.000000 sphinx_nested_apidoc-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-01 12:57:11.824303 sphinx_nested_apidoc-1.2.4/LICENSE
+-rw-r--r--   0        0        0    10887 2023-08-01 12:57:11.824303 sphinx_nested_apidoc-1.2.4/README.rst
+-rw-r--r--   0        0        0     2425 2023-08-01 12:57:11.828303 sphinx_nested_apidoc-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-08-01 12:57:11.828303 sphinx_nested_apidoc-1.2.4/src/sphinx_nested_apidoc/__init__.py
+-rw-r--r--   0        0        0     4076 2023-08-01 12:57:11.828303 sphinx_nested_apidoc-1.2.4/src/sphinx_nested_apidoc/__main__.py
+-rw-r--r--   0        0        0     3145 2023-08-01 12:57:11.828303 sphinx_nested_apidoc-1.2.4/src/sphinx_nested_apidoc/_ext.py
+-rw-r--r--   0        0        0    10848 2023-08-01 12:57:11.828303 sphinx_nested_apidoc-1.2.4/src/sphinx_nested_apidoc/core.py
+-rw-r--r--   0        0        0    11949 1970-01-01 00:00:00.000000 sphinx_nested_apidoc-1.2.4/PKG-INFO
```

### Comparing `sphinx_nested_apidoc-1.2.3/LICENSE` & `sphinx_nested_apidoc-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_nested_apidoc-1.2.3/README.rst` & `sphinx_nested_apidoc-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_nested_apidoc-1.2.3/pyproject.toml` & `sphinx_nested_apidoc-1.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "sphinx-nested-apidoc"
-version = "1.2.3"
+version = "1.2.4"
 description = "sphinx-nested-apidoc: When flattened is not enough"
 authors = ["Arunanshu Biswas <mydellpc07@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 scripts = {sphinx-nested-apidoc = "sphinx_nested_apidoc.__main__:main"}
 repository = "https://github.com/arunanshub/sphinx-nested-apidoc"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-    "Topic :: Documentation :: Sphinx",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Intended Audience :: Developers",
+  "Topic :: Documentation :: Sphinx",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/arunanshub/sphinx-nested-apidoc/issues"
 "Changelog" = "https://github.com/arunanshub/sphinx-nested-apidoc/blob/master/CHANGELOG.md"
 
 [tool.poetry.dependencies]
@@ -45,15 +46,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.3"
+version = "1.2.4"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 annotated_tag = true
 changelog_start_rev = "v0.3.1"
 version_files = [
     "pyproject.toml",
@@ -62,45 +63,47 @@
 
 [tool.black]
 line-length = 79
 target-verson = "py38"
 
 [tool.coverage.report]
 exclude_lines = [
-    "pragma: no cover",
-    "if TYPE_CHECKING",
-    "if typing.TYPE_CHECKING",
+  "pragma: no cover",
+  "if TYPE_CHECKING",
+  "if typing.TYPE_CHECKING",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--strict-config --strict-markers"
 
 [tool.ruff]
 line-length = 79
 target-version = "py38"
 exclude = [
-    "docs",
-    "tests",
-]
-ignore = [
-    "ANN101",
-    "ANN102",
-    "ANN401",
-    "B024",
+  "docs",
+  "tests",
 ]
+ignore = ["ANN101", "ANN102", "ANN401", "B024", "PLR0913"]
 select = [
   "ANN",
   "B",
   "E",
   "F",
   "W",
   "I",
   "RET",
   "EM",
   "UP",
   "C90",
   "PTH",
   "SIM",
+  "TCH",
+  "PIE",
+  "TID",
+  "G",
+  "PL",
 ]
 
 [tool.ruff.isort]
 required-imports = ["from __future__ import annotations"]
+combine-as-imports = true
+force-wrap-aliases = true
```

### Comparing `sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/__init__.py` & `sphinx_nested_apidoc-1.2.4/src/sphinx_nested_apidoc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 LOGGER_FORMAT = "[{levelname}: {filename}:{lineno}]: {message}"
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 
 
 def start_logging(
     level: int | str = logging.DEBUG,
     fmt: str = LOGGER_FORMAT,
 ) -> logging.Handler:
     """
@@ -24,10 +24,10 @@
     logger.addHandler(handler)
     logger.setLevel(level)
     logger.debug("Logging enabled for %s", __name__)
 
     return handler
 
 
-from ._ext import setup  # noqa: E402
+from ._ext import setup  # noqa: E402,TCH001
 
 __all__ = ["setup"]
```

### Comparing `sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/__main__.py` & `sphinx_nested_apidoc-1.2.4/src/sphinx_nested_apidoc/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import argparse
+import enum
 import logging
 from pathlib import Path
 
 from . import __version__, start_logging
 from .core import feed_sphinx_apidoc, rename_files, sanitize_path
 
 logger = logging.getLogger(__name__)
@@ -20,21 +21,21 @@
 CLI_APP_EPILOG = f"""\
 {APP_NAME} is licensed under MIT license.
 
 Visit <https://github.com/arunanshub/sphinx-nested-apidoc> for more info.
 """
 
 
-def main(argv: list[str] | None = None) -> int:
-    logging_levels = {
-        3: logging.WARNING,
-        4: logging.INFO,
-        5: logging.DEBUG,
-    }
+class LoggingLevel(enum.IntEnum):
+    WARNING = 3
+    INFO = 4
+    DEBUG = 5
+
 
+def main(argv: list[str] | None = None) -> int:
     ps = argparse.ArgumentParser(
         description=APP_DESC,
         epilog=CLI_APP_EPILOG,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     group = ps.add_mutually_exclusive_group()
     group.add_argument(
@@ -111,17 +112,17 @@
         " arguments like `--dry-run` are ignored.",
         metavar="...",
     )
 
     args = ps.parse_args(argv)
     if not args.quiet:
         verbose = args.verbose
-        if args.verbose > 5:
+        if args.verbose > LoggingLevel.WARNING:
             verbose = 5
-        start_logging(logging_levels[verbose])
+        start_logging(LoggingLevel(verbose))
 
     is_help = feed_sphinx_apidoc(
         args.destdir,
         args.module_path,
         *args.sphinx_commands,
         implicit_namespaces=args.implicit_namespaces,
         force=args.force,
@@ -142,15 +143,15 @@
             ),
             extension=args.suffix,
             implicit_namespaces=args.implicit_namespaces,
             dry_run=args.dry_run,
             force=args.force,
         )
     except ValueError as e:
-        logger.error("%s", e, exc_info=True)
+        logger.exception("%s", e)
         return 1
 
     return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/_ext.py` & `sphinx_nested_apidoc-1.2.4/src/sphinx_nested_apidoc/_ext.py`

 * *Files identical despite different names*

### Comparing `sphinx_nested_apidoc-1.2.3/src/sphinx_nested_apidoc/core.py` & `sphinx_nested_apidoc-1.2.4/src/sphinx_nested_apidoc/core.py`

 * *Files identical despite different names*

### Comparing `sphinx_nested_apidoc-1.2.3/PKG-INFO` & `sphinx_nested_apidoc-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-nested-apidoc
-Version: 1.2.3
+Version: 1.2.4
 Summary: sphinx-nested-apidoc: When flattened is not enough
 Home-page: https://github.com/arunanshub/sphinx-nested-apidoc
 License: MIT
 Author: Arunanshu Biswas
 Author-email: mydellpc07@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

