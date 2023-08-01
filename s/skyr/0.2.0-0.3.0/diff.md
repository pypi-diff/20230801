# Comparing `tmp/skyr-0.2.0.tar.gz` & `tmp/skyr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyr-0.2.0.tar", last modified: Wed Mar 29 01:00:55 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `skyr-0.2.0.tar` & `skyr-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.236625 skyr-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-29 01:00:38.000000 skyr-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-29 01:00:38.000000 skyr-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-29 01:00:38.000000 skyr-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-29 01:00:38.000000 skyr-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-29 01:00:38.000000 skyr-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-29 01:00:55.236625 skyr-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-29 01:00:38.000000 skyr-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.232625 skyr-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-03-29 01:00:38.000000 skyr-0.2.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    20569 2023-03-29 01:00:38.000000 skyr-0.2.0/docs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-03-29 01:00:38.000000 skyr-0.2.0/docs/tacit-lite.css
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-29 01:00:38.000000 skyr-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-29 01:00:38.000000 skyr-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 01:00:55.236625 skyr-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.232625 skyr-0.2.0/skyr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-29 01:00:55.000000 skyr-0.2.0/skyr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-29 01:00:55.000000 skyr-0.2.0/skyr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 01:00:55.000000 skyr-0.2.0/skyr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-29 01:00:55.000000 skyr-0.2.0/skyr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-29 01:00:55.000000 skyr-0.2.0/skyr.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-03-29 01:00:38.000000 skyr-0.2.0/skyr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.232625 skyr-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.232625 skyr-0.2.0/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/assets/a_file
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.232625 skyr-0.2.0/tests/assets/bad_cwd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/assets/bad_cwd/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.236625 skyr-0.2.0/tests/assets/other_dir/
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/assets/other_dir/build
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.236625 skyr-0.2.0/tests/assets/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:55.236625 skyr-0.2.0/tests/assets/script/a_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/assets/script/a_dir/.gitkeep
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/assets/script/build
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/assets/script/hello
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/assets/script/no-shebang
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/assets/script/not-executable
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-03-29 01:00:38.000000 skyr-0.2.0/tests/skyr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-29 01:00:38.000000 skyr-0.2.0/tox.ini
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 skyr-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 skyr-0.3.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 skyr-0.3.0/skyr.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 skyr-0.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 skyr-0.3.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skyr-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 skyr-0.3.0/docs/index.html
+-rw-r--r--   0        0        0    20569 2020-02-02 00:00:00.000000 skyr-0.3.0/docs/logo.svg
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 skyr-0.3.0/docs/tacit-lite.css
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 skyr-0.3.0/script/build
+-rwxr-xr-x   0        0        0      211 2020-02-02 00:00:00.000000 skyr-0.3.0/script/clean
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 skyr-0.3.0/script/fmt
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 skyr-0.3.0/script/lint
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 skyr-0.3.0/script/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/ruff.toml
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/skyr_test.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/assets/a_file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/assets/bad_cwd/.gitkeep
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/assets/other_dir/build
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/assets/script/build
+-rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/assets/script/hello
+-rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/assets/script/no-shebang
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/assets/script/not-executable
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skyr-0.3.0/tests/assets/script/a_dir/.gitkeep
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 skyr-0.3.0/.gitignore
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 skyr-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 skyr-0.3.0/README.md
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 skyr-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 skyr-0.3.0/PKG-INFO
```

### Comparing `skyr-0.2.0/.gitignore` & `skyr-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `skyr-0.2.0/CHANGELOG.md` & `skyr-0.3.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 # Skyr / Change Log
 
+## 0.3.0 - 2023-08-01
+
+## BREAKING
+
+- [#43](https://github.com/kytta/skyr/pull/43):
+  Drop support for Python 3.8
+
+### Behind-the-scenes
+
+- Migrated to Hatch as task runner and build system
+
 ## 0.2.0 - 2023-03-29
 
 ### Added
 
-* [#9](https://github.com/kytta/skyr/issues/9):
+- [#9](https://github.com/kytta/skyr/issues/9):
   Allow execution of scripts from `./.skyr/`.
 
 ### Changed
 
-* due to [#9](https://github.com/kytta/skyr/issues/9):
+- due to [#9](https://github.com/kytta/skyr/issues/9):
   script directory resolution logic was changed: if provided script dir doesn't
   exist, Skyr will fall back to `./.skyr/`, then `./script/`
 
 ## 0.1.1 - 2023-03-29
 
 ## Fixed
 
-* [`80afa7e3`](https://github.com/kytta/skyr/commit/80afa7e3ca3e3de47a1d1129efe866c743049954):
+- [`80afa7e3`](https://github.com/kytta/skyr/commit/80afa7e3ca3e3de47a1d1129efe866c743049954):
   Fixed setuptools module discovery
 
 ## Behind-the-scenes
 
-* [#7](https://github.com/kytta/skyr/pull/7):
+- [#7](https://github.com/kytta/skyr/pull/7):
   Eat our own dog food
-  * this means, Skyr uses Skyr scripts ✨
-* [#12](https://github.com/kytta/skyr/pull/12):
+  - this means, Skyr uses Skyr scripts ✨
+- [#12](https://github.com/kytta/skyr/pull/12):
   Add GitHub Pages site
 
 ## 0.1.0 - 2023-02-07
 
 ## Added
 
 - [#4](https://github.com/kytta/skyr/pull/4):
```

### Comparing `skyr-0.2.0/LICENSE` & `skyr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skyr-0.2.0/PKG-INFO` & `skyr-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: skyr
-Version: 0.2.0
+Version: 0.3.0
 Summary: A low-fat task runner.
+Project-URL: Issues, https://github.com/kytta/skyr/issues
+Project-URL: Source, https://github.com/kytta/skyr
 Author-email: Nikita Karamov <me@kytta.dev>
 Maintainer-email: Nikita Karamov <me@kytta.dev>
-License: ISC License
-Project-URL: Source, https://github.com/kytta/skyr
-Project-URL: Issues, https://github.com/kytta/skyr/issues
+License-Expression: ISC
+License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Skyr
 
 > Low-fat task runner.
 
 Skyr is a task runner, similar to Make. Just like Make, it can have tasks that
 depend on each other and are executed only if a file changes. But, unlike Make,
@@ -75,30 +78,30 @@
 ```sh
 skyr --script-dir ./dev/ test
 ```
 
 ## Roadmap
 
 - [x] Basic script running: Run .sh, .bash, .zsh, and other files from the
-      `script/` directory.
+  `script/` directory.
 - [ ] Target dependencies: Run scripts if other depend on them.
 - [ ] Dependency age: Run scripts only if the files it depends on changed.
 - [ ] Script validation: Check that Skyr understands the scripts it was given.
 - [ ] Make mode: Support running very basic Makefiles.
 - [ ] Make migration mode: Support migrating from a Makefile to a `script/`
-      directory.
+  directory.
 - [ ] Just mode: Support running very basic Justfiles.
 - [ ] Just migration mode: Support migrating from `just` to a `script/`
-      directory.
+  directory.
 
 ## Licence
 
 © 2023 [Nikita Karamov]\
 Code licensed under the [ISC License].
 
----
+______________________________________________________________________
 
 This project is hosted on GitHub:
 <https://github.com/kytta/skyr.git>
 
 [isc license]: https://spdx.org/licenses/ISC.html
 [nikita karamov]: https://www.kytta.dev/
```

### Comparing `skyr-0.2.0/README.md` & `skyr-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -49,30 +49,30 @@
 ```sh
 skyr --script-dir ./dev/ test
 ```
 
 ## Roadmap
 
 - [x] Basic script running: Run .sh, .bash, .zsh, and other files from the
-      `script/` directory.
+  `script/` directory.
 - [ ] Target dependencies: Run scripts if other depend on them.
 - [ ] Dependency age: Run scripts only if the files it depends on changed.
 - [ ] Script validation: Check that Skyr understands the scripts it was given.
 - [ ] Make mode: Support running very basic Makefiles.
 - [ ] Make migration mode: Support migrating from a Makefile to a `script/`
-      directory.
+  directory.
 - [ ] Just mode: Support running very basic Justfiles.
 - [ ] Just migration mode: Support migrating from `just` to a `script/`
-      directory.
+  directory.
 
 ## Licence
 
 © 2023 [Nikita Karamov]\
 Code licensed under the [ISC License].
 
----
+______________________________________________________________________
 
 This project is hosted on GitHub:
 <https://github.com/kytta/skyr.git>
 
 [isc license]: https://spdx.org/licenses/ISC.html
 [nikita karamov]: https://www.kytta.dev/
```

### Comparing `skyr-0.2.0/docs/index.html` & `skyr-0.3.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `skyr-0.2.0/docs/logo.svg` & `skyr-0.3.0/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `skyr-0.2.0/docs/tacit-lite.css` & `skyr-0.3.0/docs/tacit-lite.css`

 * *Files identical despite different names*

### Comparing `skyr-0.2.0/pyproject.toml` & `skyr-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 [build-system]
-requires = ["setuptools>=61", "setuptools_scm[toml]>=6.2"]
-build-backend = "setuptools.build_meta"
+build-backend = "hatchling.build"
+requires = [
+  "hatchling",
+]
 
 [project]
 name = "skyr"
 description = "A low-fat task runner."
 readme = "README.md"
-requires-python = ">=3.8"
-license = {text = "ISC License"}
-authors = [
+license = "ISC"
+maintainers = [
     { name = "Nikita Karamov", email = "me@kytta.dev" },
 ]
-maintainers = [
+authors = [
     { name = "Nikita Karamov", email = "me@kytta.dev" },
 ]
+requires-python = ">=3.9"
 classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Environment :: Console",
-    "Intended Audience :: Developers",
-    "Intended Audience :: System Administrators",
-    "License :: OSI Approved :: ISC License (ISCL)",
-    "Operating System :: MacOS",
-    "Operating System :: POSIX",
-    "Operating System :: Unix",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Topic :: Software Development :: Build Tools",
-    "Topic :: Utilities",
-    "Typing :: Typed",
+  "Development Status :: 3 - Alpha",
+  "Environment :: Console",
+  "Intended Audience :: Developers",
+  "Intended Audience :: System Administrators",
+  "License :: OSI Approved :: ISC License (ISCL)",
+  "Operating System :: MacOS",
+  "Operating System :: POSIX",
+  "Operating System :: Unix",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Software Development :: Build Tools",
+  "Topic :: Utilities",
+  "Typing :: Typed",
+]
+dynamic = [
+  "version",
+]
+dependencies = [
 ]
-dependencies = []
-dynamic = ["version"]
-
 [project.urls]
-Source = "https://github.com/kytta/skyr"
 Issues = "https://github.com/kytta/skyr/issues"
-
+Source = "https://github.com/kytta/skyr"
 [project.scripts]
 skyr = "skyr:main"
 
-[tool.setuptools]
-py-modules = ["skyr"]
+[tool.setuptools_scm]
 
-[tool.autopep8]
-ignore = ["W503"]
+[tool.hatch.version]
+path = "skyr.py"
 
-[tool.coverage.run]
-plugins = ["covdefaults"]
+[tool.hatch.envs.default]
+dependencies = [
+  "pytest",
+  "coverage[toml]",
+  "covdefaults",
+]
 
-[tool.mypy]
-python_version = 3.8
-check_untyped_defs = true
-disallow_any_generics = true
-disallow_incomplete_defs = true
-disallow_untyped_defs = true
-warn_redundant_casts = true
-warn_unused_ignores = true
+[tool.hatch.envs.default.scripts]
+test = [
+    "pytest {args:tests}",
+]
+cov = [
+    "coverage erase",
+    "coverage run -m pytest {args:tests}",
+    "coverage report",
+    "coverage xml"
+]
 
-[[tool.mypy.overrides]]
-module = ["tests.*"]
-ignore_missing_imports = true
-check_untyped_defs = false
-disallow_incomplete_defs = false
-disallow_untyped_defs = false
+[[tool.hatch.envs.test.matrix]]
+python = ["39", "310", "311"]
 
-[tool.pytest.ini_options]
-addopts = "--tb=short --showlocals"
+[tool.autopep8]
+ignore = ["W503"]
 
 [tool.ruff]
 line-length = 79
-target-version = "py38"
+target-version = "py39"
 
 select = [
     "F",       # pyflakes
     "E", "W",  # pycodestyle
     "C90",     # mccabe
     "N",       # pep8-naming
     "S",       # bandit
@@ -101,8 +108,28 @@
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "double"
 
-[tool.setuptools_scm]
+[tool.pytest.ini_options]
+addopts = "--tb=short --showlocals"
+
+[tool.coverage.run]
+plugins = ["covdefaults"]
+
+[tool.mypy]
+python_version = 3.9
+check_untyped_defs = true
+disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_untyped_defs = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+
+[[tool.mypy.overrides]]
+module = ["tests.*"]
+ignore_missing_imports = true
+check_untyped_defs = false
+disallow_incomplete_defs = false
+disallow_untyped_defs = false
```

### Comparing `skyr-0.2.0/skyr.py` & `skyr-0.3.0/skyr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 #!/usr/bin/env python3
 import argparse
 import errno
 import os
 import sys
-from importlib import metadata
+from collections.abc import Iterable
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Iterable
-from typing import List
 from typing import NoReturn
 from typing import Optional
-from typing import Sequence
 from typing import Union
 
-__version__ = metadata.version("skyr")
+__version__ = "0.3.0"
 
 
 def _warn(msg: str) -> None:
     sys.stderr.write(f"[WARNING] {msg}\n")
     sys.stderr.flush()
 
 
@@ -44,46 +42,47 @@
 
     :param name: Name of the script
     :param script_dir: Directory to search for the scripts
     """
     script_file = (script_dir / name).resolve()
 
     if not script_file.exists():
-        _err(f"Script doesn't exist: {str(script_file)}")
+        _err(f"Script doesn't exist: {script_file!s}")
         return None
 
     if not script_file.is_file():
-        _err(f"Script is not a file: {str(script_file)}")
+        _err(f"Script is not a file: {script_file!s}")
         return None
 
     return script_file
 
 
 def try_execute(
     name: str,
     script_file: Path,
-    argv: Optional[List[str]] = None,
+    argv: Optional[list[str]] = None,
 ) -> NoReturn:
     if argv is None:
         argv = []
 
     try:
-        os.execl(script_file, name, *argv)
+        # TODO: replace with a subprocess call
+        os.execl(script_file, name, *argv)  # noqa: S606
     except OSError as exc:
         if exc.errno is errno.EACCES:
             _err(
-                f"You are not allowed to execute {str(script_file)}. Please "
+                f"You are not allowed to execute {script_file!s}. Please "
                 "make sure that you've set the correct rights via chmod.", )
         elif exc.errno is errno.ENOEXEC:
             _err(
-                f"{str(script_file)} has a wrong executable format. Did you "
+                f"{script_file!s} has a wrong executable format. Did you "
                 "forget to add a shebang?",
             )
         else:
-            _err(f"Could not execute {str(script_file)}: {exc.strerror}")
+            _err(f"Could not execute {script_file!s}: {exc.strerror}")
         raise SystemExit(1) from exc
 
 
 def _get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         description="A low-fat task runner, Skyr runs scripts from the "
                     "'./script/' directory in a make(1) fashion.",
@@ -120,15 +119,15 @@
     args, rest = _get_parser().parse_known_args(argv)
 
     script_dir = None
     if hasattr(args, "script_dir"):
         if args.script_dir.exists():
             script_dir = args.script_dir
         else:
-            _warn(f"Script directory not found: {str(args.script_dir)}")
+            _warn(f"Script directory not found: {args.script_dir!s}")
 
     if script_dir is None:
         script_dir = find_dir([Path(".skyr"), Path("script")])
 
     if script_dir is None:
         _err("No script directory found.")
         raise SystemExit(1)
```

### Comparing `skyr-0.2.0/tests/skyr_test.py` & `skyr-0.3.0/tests/skyr_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import subprocess
+import sys
+from collections.abc import Iterable
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Iterable
-from typing import List
 from typing import Optional
-from typing import Sequence
 
 import pytest
 
 import skyr
 
 ASSETS_DIR = Path(__file__).parent / "assets"
 
 
 @pytest.mark.parametrize(
     ("argv", "return_code"), [
         (["--help"], 0),
         (["--version"], 0),
     ],
 )
-def test_argpase_exits_zero(argv: List[str], return_code: int):
+def test_argpase_exits_zero(argv: list[str], return_code: int):
     with pytest.raises(SystemExit):
         assert skyr.main(argv) == return_code
 
 
 @pytest.mark.parametrize(
     ("candidates", "return_value"), [
         ([], None),
@@ -142,19 +142,19 @@
         (
             ["--script-dir", "other_dir"],
             b"I'm a build script in a different directory",
         ),
     ],
 )
 def test_successful_execution(
-    argv: List[str],
+    argv: list[str],
     expected_out: bytes,
     monkeypatch,
 ):
     with monkeypatch.context() as m:
         m.chdir(Path(__file__).parent / "assets")
 
-        cmd = ["python3", "-m", "skyr", *argv]
-        result = subprocess.run(cmd, capture_output=True)
+        stdout = subprocess.check_output(
+            [sys.executable, "-m", "skyr", *argv],  # noqa: S603
+        )
 
-        assert result.returncode == 0
-        assert expected_out in result.stdout
+        assert expected_out in stdout
```

