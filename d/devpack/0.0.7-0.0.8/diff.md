# Comparing `tmp/devpack-0.0.7.tar.gz` & `tmp/devpack-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpack-0.0.7.tar", last modified: Tue Dec  6 12:44:14 2022, max compression
+gzip compressed data, was "devpack-0.0.8.tar", last modified: Tue Aug  1 06:11:54 2023, max compression
```

## Comparing `devpack-0.0.7.tar` & `devpack-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:14.634638 devpack-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:14.634638 devpack-0.0.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:07.000000 devpack-0.0.7/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:14.634638 devpack-0.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2022-12-06 12:44:07.000000 devpack-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2022-12-06 12:44:07.000000 devpack-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-06 12:44:07.000000 devpack-0.0.7/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2022-12-06 12:44:07.000000 devpack-0.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2022-12-06 12:44:07.000000 devpack-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2022-12-06 12:44:14.634638 devpack-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-06 12:44:07.000000 devpack-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:14.634638 devpack-0.0.7/devpack/
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:14.634638 devpack-0.0.7/devpack/batch_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/alls.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/authors.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/inits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/privates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/readmes.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/batch_tools/shebangs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/development.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:14.634638 devpack-0.0.7/devpack/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/entry_points/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2022-12-06 12:44:07.000000 devpack-0.0.7/devpack/entry_points/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:14.634638 devpack-0.0.7/devpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2022-12-06 12:44:14.000000 devpack-0.0.7/devpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2022-12-06 12:44:14.000000 devpack-0.0.7/devpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 12:44:14.000000 devpack-0.0.7/devpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-06 12:44:14.000000 devpack-0.0.7/devpack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-06 12:44:14.000000 devpack-0.0.7/devpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-06 12:44:14.000000 devpack-0.0.7/devpack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 12:44:14.634638 devpack-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-06 12:44:07.000000 devpack-0.0.7/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-06 12:44:07.000000 devpack-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-06 12:44:07.000000 devpack-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-06 12:44:14.634638 devpack-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2022-12-06 12:44:07.000000 devpack-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.874159 devpack-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.870159 devpack-0.0.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:45.000000 devpack-0.0.8/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.870159 devpack-0.0.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-01 06:11:45.000000 devpack-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-01 06:11:45.000000 devpack-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:11:45.000000 devpack-0.0.8/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-01 06:11:45.000000 devpack-0.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-01 06:11:45.000000 devpack-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-01 06:11:54.874159 devpack-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 06:11:45.000000 devpack-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.870159 devpack-0.0.8/devpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.874159 devpack-0.0.8/devpack/batch_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/alls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/inits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/privates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/readmes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/shebangs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/batch_tools/typing_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/development.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.874159 devpack-0.0.8/devpack/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/entry_points/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/entry_points/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/entry_points/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.874159 devpack-0.0.8/devpack/versioning_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/versioning_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-01 06:11:45.000000 devpack-0.0.8/devpack/versioning_tools/bump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.870159 devpack-0.0.8/devpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-01 06:11:54.000000 devpack-0.0.8/devpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-01 06:11:54.000000 devpack-0.0.8/devpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:11:54.000000 devpack-0.0.8/devpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-01 06:11:54.000000 devpack-0.0.8/devpack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-01 06:11:54.000000 devpack-0.0.8/devpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 06:11:54.000000 devpack-0.0.8/devpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.874159 devpack-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:11:45.000000 devpack-0.0.8/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 06:11:45.000000 devpack-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 06:11:45.000000 devpack-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 06:11:54.874159 devpack-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-08-01 06:11:45.000000 devpack-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:54.874159 devpack-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-01 06:11:45.000000 devpack-0.0.8/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 06:11:45.000000 devpack-0.0.8/tests/test_sanity.py
```

### Comparing `devpack-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md` & `devpack-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md` & `devpack-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/LICENSE.md` & `devpack-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/PKG-INFO` & `devpack-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpack
-Version: 0.0.7
+Version: 0.0.8
 Summary: DevPack is a package for managing your dev environment
 Home-page: https://github.com/pything/devpack
 Download-URL: https://github.com/pything/devpack/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -20,16 +20,16 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: setup
 Provides-Extra: tests
+Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 # DevPack
 
 ```bash
 pip install devpack -U
```

### Comparing `devpack-0.0.7/devpack/__init__.py` & `devpack-0.0.8/devpack/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import datetime
 import os
 from warnings import warn
-
-import pkg_resources
-
+from importlib.metadata import PackageNotFoundError
+from importlib import resources
 from apppath import AppPath
 
 __project__ = "devpack"
 __author__ = "Christian Heider Nielsen"
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 __doc__ = """
 Created on 15/04/2020
 
 @author: cnheider
 """
 
 from typing import Any
@@ -27,40 +26,28 @@
     "PROJECT_ORGANISATION",
     "PROJECT_AUTHOR",
     "PROJECT_YEAR",
     # "INCLUDE_PROJECT_READMES",
     # "PACKAGE_DATA_PATH"
 ]
 
-
-def dist_is_editable(dist: Any) -> bool:
-    """
-    Return True if given Distribution is an editable installation."""
-    import sys
-    from pathlib import Path
-
-    for path_item in sys.path:
-        egg_link = Path(path_item) / f"{dist.project_name}.egg-link"
-        if egg_link.is_file():
-            return True
-    return False
-
-
 PROJECT_NAME = __project__.lower().strip().replace(" ", "_")
 PROJECT_VERSION = __version__
 PROJECT_YEAR = 2018
 PROJECT_AUTHOR = __author__.lower().strip().replace(" ", "_")
 PROJECT_APP_PATH = AppPath(app_name=PROJECT_NAME, app_author=PROJECT_AUTHOR)
 PROJECT_ORGANISATION = "pything"
 
-distributions = {v.key: v for v in pkg_resources.working_set}
-if PROJECT_NAME in distributions:
-    distribution = distributions[PROJECT_NAME]
-    DEVELOP = dist_is_editable(distribution)
-else:
+from warg import package_is_editable
+
+PACKAGE_DATA_PATH = resources.files(PROJECT_NAME) / "data"
+
+try:
+    DEVELOP = package_is_editable(PROJECT_NAME)
+except PackageNotFoundError as e:
     DEVELOP = True
 
 
 def get_version(append_time: Any = DEVELOP) -> str:
     """
 
     :param append_time:
```

### Comparing `devpack-0.0.7/devpack/batch_tools/aliases.py` & `devpack-0.0.8/devpack/batch_tools/aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
            """
 
 __all__ = ["recursive_detect_import_aliasing"]
 
 from pathlib import Path
 from typing import Iterable, Callable, Optional, Sequence, Mapping, List
 
-from warg.os_utilities.filtering import negate, is_python_module, is_python_package
+from warg.os_utilities.filtering import negate, is_python_package
 
 
 def has_import_aliases(path: Path, *, verbose: bool = False) -> bool:
     """
 
     :param verbose:
     :type verbose:
```

### Comparing `devpack-0.0.7/devpack/batch_tools/alls.py` & `devpack-0.0.8/devpack/batch_tools/alls.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,14 +241,18 @@
     if is_library_file(path, verbose=verbose):
         if has_all_declaration(path, verbose=verbose):
             if not has_non_empty_all(path, verbose=verbose):
                 if verbose:
                     print("WARNING library file with empty __all__ declaration")
 
 
+def has_multiple_alls() -> bool:
+    ...
+
+
 def recursive_check_alls(
     path: Path,
     exclusion_filter: Optional[Iterable[Callable]] = (negate(is_python_package),),
     *,
     alls_mode: AutoAllsModeEnum = AutoAllsModeEnum.empty,
     verbose: bool = True,
 ) -> None:
@@ -266,15 +270,14 @@
     path = Path(path)
 
     for child in path.iterdir():
         if child.is_dir():
             if exclusion_filter is None or not any(
                 flt(child) for flt in exclusion_filter
             ):
-
                 recursive_check_alls(
                     child,
                     exclusion_filter,
                     verbose=verbose,
                 )
             else:
                 if verbose:
```

### Comparing `devpack-0.0.7/devpack/batch_tools/authors.py` & `devpack-0.0.8/devpack/batch_tools/authors.py`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/devpack/batch_tools/docs.py` & `devpack-0.0.8/devpack/batch_tools/docs.py`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/devpack/batch_tools/entry_points.py` & `devpack-0.0.8/devpack/batch_tools/entry_points.py`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/devpack/batch_tools/inits.py` & `devpack-0.0.8/devpack/batch_tools/inits.py`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/devpack/batch_tools/privates.py` & `devpack-0.0.8/devpack/batch_tools/privates.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 __all__ = ["recursive_check_for_privates"]
 
 from pathlib import Path
 from typing import Optional, Callable, Iterable
 
 from draugr.os_utilities.linux_utilities.user_utilities import get_username
+
 from warg.os_utilities.filtering import is_python_module, negate
 
 
 def contains_specific_home_reference(path: Path, *, verbose: bool = True) -> bool:
     """
 
     :param verbose:
```

### Comparing `devpack-0.0.7/devpack/batch_tools/readmes.py` & `devpack-0.0.8/devpack/batch_tools/readmes.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 __all__ = ["auto_add_readme", "recursive_add_readmes", "TouchModeEnum"]
 
 from enum import Enum
 from pathlib import Path
 from typing import Callable, Iterable, Optional
 
 from sorcery import assigned_names
+
 from warg.os_utilities.filtering import negate, is_python_package
 
 
 class TouchModeEnum(Enum):
     """
     The touch mode enum
```

### Comparing `devpack-0.0.7/devpack/batch_tools/shebangs.py` & `devpack-0.0.8/devpack/batch_tools/shebangs.py`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/devpack/development.py` & `devpack-0.0.8/devpack/development.py`

 * *Files identical despite different names*

### Comparing `devpack-0.0.7/devpack/entry_points/batch.py` & `devpack-0.0.8/devpack/entry_points/batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
            """
 
 __all__ = []
 
 import argparse
 from pathlib import Path
 
-from devpack.batch_tools.readmes import TouchModeEnum, recursive_add_readmes
 from devpack.batch_tools.inits import recursive_remove_inits
+from devpack.batch_tools.readmes import TouchModeEnum, recursive_add_readmes
 
 
 def recursively_add_readmes_from_here():
     """
     Add readmes to all python modules in the current directory
     """
     parser = argparse.ArgumentParser(description="DevPack add readmes from here")
@@ -67,10 +67,31 @@
     recursive_remove_inits(
         args.path,
         init_name=args.init_name,
         verbose=args.verbose,
     )
 
 
+def recursively_check_typing():
+    """
+    Add readmes to all python modules in the current directory
+    """
+    parser = argparse.ArgumentParser(description="DevPack remove inits from here")
+    parser.add_argument(
+        "--path", "-p", type=Path, default=Path.cwd(), help="Path to remove inits from"
+    )
+    parser.add_argument(
+        "--verbose", action="store_true", help="Verbose output of removed files"
+    )
+    args = parser.parse_args()
+
+    recursive_remove_inits(
+        args.path,
+        init_name=args.init_name,
+        verbose=args.verbose,
+    )
+
+
 if __name__ == "__main__":
-    recursively_add_readmes_from_here()
-    recursively_remove_inits_from_here()
+    # recursively_add_readmes_from_here()
+    # recursively_remove_inits_from_here()
+    recursively_check_typing()
```

### Comparing `devpack-0.0.7/devpack/entry_points/cli.py` & `devpack-0.0.8/devpack/entry_points/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
            Entry points for package development.
 """
 
 import argparse
 
-from devpack.development import pip_uninstall_package
 from devpack.development import pip_install_development_package
+from devpack.development import pip_uninstall_package
 
 
 def install_develop():
-    """description"""
+    """For programmatically installing a package as a development install"""
     parser = argparse.ArgumentParser(description="DevPack Develop Installation")
     parser.add_argument(
         "PACKAGE_NAME", metavar="Name", type=str, help="Package name to install"
     )
     """
 parser.add_argument(
 "--SITE",
@@ -29,15 +29,15 @@
 """
     args = parser.parse_args()
 
     pip_install_development_package(args.PACKAGE_NAME)
 
 
 def uninstall():
-    """description"""
+    """For programmatically uninstalling a package"""
     parser = argparse.ArgumentParser(description="DevPack Uninstall")
     parser.add_argument(
         "PACKAGE_NAME", metavar="Name", type=str, help="Package name to uninstall"
     )
     args = parser.parse_args()
 
     pip_uninstall_package(args.PACKAGE_NAME)
```

### Comparing `devpack-0.0.7/devpack.egg-info/PKG-INFO` & `devpack-0.0.8/devpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpack
-Version: 0.0.7
+Version: 0.0.8
 Summary: DevPack is a package for managing your dev environment
 Home-page: https://github.com/pything/devpack
 Download-URL: https://github.com/pything/devpack/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -20,16 +20,16 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: setup
 Provides-Extra: tests
+Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 # DevPack
 
 ```bash
 pip install devpack -U
```

### Comparing `devpack-0.0.7/devpack.egg-info/SOURCES.txt` & `devpack-0.0.8/devpack.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,11 +23,17 @@
 devpack/batch_tools/authors.py
 devpack/batch_tools/docs.py
 devpack/batch_tools/entry_points.py
 devpack/batch_tools/inits.py
 devpack/batch_tools/privates.py
 devpack/batch_tools/readmes.py
 devpack/batch_tools/shebangs.py
+devpack/batch_tools/typing_hints.py
 devpack/entry_points/__init__.py
 devpack/entry_points/batch.py
 devpack/entry_points/cli.py
-docs/README.md
+devpack/entry_points/versioning.py
+devpack/versioning_tools/__init__.py
+devpack/versioning_tools/bump.py
+docs/README.md
+tests/test_imports.py
+tests/test_sanity.py
```

### Comparing `devpack-0.0.7/setup.py` & `devpack-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,15 @@
         return {
             "console_scripts": [
                 # "name_of_executable = module.with:function_to_execute"
                 "devpack_install = devpack.entry_points.cli:install_develop",
                 "devpack_uninstall = devpack.entry_points.cli:uninstall",
                 "devpack_add_readmes = devpack.entry_points.batch:recursively_add_readmes_from_here",
                 "devpack_remove_inits = devpack.entry_points.batch:recursively_remove_inits_from_here",
+                "devpack_bump = devpack.entry_points.versioning:bump",
             ]
         }
 
     @property
     def extras(self) -> dict:
         """description"""
         these_extras = {
```

