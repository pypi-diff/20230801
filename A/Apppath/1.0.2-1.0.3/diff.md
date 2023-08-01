# Comparing `tmp/Apppath-1.0.2.tar.gz` & `tmp/Apppath-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Apppath-1.0.2.tar", last modified: Tue Jun 13 10:24:32 2023, max compression
+gzip compressed data, was "Apppath-1.0.3.tar", last modified: Tue Aug  1 06:12:18 2023, max compression
```

## Comparing `Apppath-1.0.2.tar` & `Apppath-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.457472 Apppath-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:24.000000 Apppath-1.0.2/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/Apppath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 10:24:24.000000 Apppath-1.0.2/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-13 10:24:24.000000 Apppath-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-13 10:24:24.000000 Apppath-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-13 10:24:32.457472 Apppath-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-13 10:24:24.000000 Apppath-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 10:24:24.000000 Apppath-1.0.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/apppath/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34504 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/app_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/apppath/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/entry_points/clean_apppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/entry_points/open_apppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/system_open_path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/windows_path_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 10:24:24.000000 Apppath-1.0.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-13 10:24:24.000000 Apppath-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 10:24:24.000000 Apppath-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 10:24:32.457472 Apppath-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-13 10:24:24.000000 Apppath-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.457472 Apppath-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-13 10:24:24.000000 Apppath-1.0.2/tests/test_app_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-13 10:24:24.000000 Apppath-1.0.2/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 10:24:24.000000 Apppath-1.0.2/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:18.273335 Apppath-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:18.273335 Apppath-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:07.000000 Apppath-1.0.3/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:18.273335 Apppath-1.0.3/Apppath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-08-01 06:12:18.000000 Apppath-1.0.3/Apppath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-01 06:12:18.000000 Apppath-1.0.3/Apppath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:12:18.000000 Apppath-1.0.3/Apppath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 06:12:18.000000 Apppath-1.0.3/Apppath.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 06:12:18.000000 Apppath-1.0.3/Apppath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 06:12:18.000000 Apppath-1.0.3/Apppath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 06:12:07.000000 Apppath-1.0.3/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-01 06:12:07.000000 Apppath-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 06:12:07.000000 Apppath-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-08-01 06:12:18.273335 Apppath-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-08-01 06:12:07.000000 Apppath-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-01 06:12:07.000000 Apppath-1.0.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:18.273335 Apppath-1.0.3/apppath/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-01 06:12:07.000000 Apppath-1.0.3/apppath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-08-01 06:12:07.000000 Apppath-1.0.3/apppath/app_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:18.273335 Apppath-1.0.3/apppath/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:12:07.000000 Apppath-1.0.3/apppath/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-01 06:12:07.000000 Apppath-1.0.3/apppath/entry_points/clean_apppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 06:12:07.000000 Apppath-1.0.3/apppath/entry_points/open_apppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-01 06:12:07.000000 Apppath-1.0.3/apppath/system_open_path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-01 06:12:07.000000 Apppath-1.0.3/apppath/windows_path_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:18.273335 Apppath-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:12:07.000000 Apppath-1.0.3/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-01 06:12:08.000000 Apppath-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 06:12:08.000000 Apppath-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 06:12:18.277335 Apppath-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-08-01 06:12:08.000000 Apppath-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:18.273335 Apppath-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-01 06:12:08.000000 Apppath-1.0.3/tests/test_app_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-01 06:12:08.000000 Apppath-1.0.3/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-01 06:12:08.000000 Apppath-1.0.3/tests/test_sanity.py
```

### Comparing `Apppath-1.0.2/Apppath.egg-info/PKG-INFO` & `Apppath-1.0.3/Apppath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apppath
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/apppath
 Download-URL: https://github.com/pything/apppath/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,18 +19,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: setup
 Provides-Extra: dev
 Provides-Extra: tests
+Provides-Extra: docs
+Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![apppath](.github/images/apppath.svg)-->
 
 <p align="center">
   <img src=".github/images/apppath.svg" alt='AppPath' />
```

### Comparing `Apppath-1.0.2/Apppath.egg-info/SOURCES.txt` & `Apppath-1.0.3/Apppath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.2/LICENSE.md` & `Apppath-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.2/PKG-INFO` & `Apppath-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apppath
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/apppath
 Download-URL: https://github.com/pything/apppath/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,18 +19,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: setup
 Provides-Extra: dev
 Provides-Extra: tests
+Provides-Extra: docs
+Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![apppath](.github/images/apppath.svg)-->
 
 <p align="center">
   <img src=".github/images/apppath.svg" alt='AppPath' />
```

### Comparing `Apppath-1.0.2/README.md` & `Apppath-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.2/SECURITY.md` & `Apppath-1.0.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.2/apppath/__init__.py` & `Apppath-1.0.3/apppath/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import datetime
 import os
+from importlib.metadata import PackageNotFoundError
 from warnings import warn
+from typing import Any
+
+from importlib import resources
+from warg import package_is_editable
 
-import pkg_resources
 
 __project__ = "Apppath"
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __doc__ = r"""
 Created on 27/04/2019
 
 A class and a set of functions for providing for system-consensual path for apps to store data, logs, cache...
 
 @author: cnheider
 """
@@ -28,43 +32,28 @@
     "AppPath",
     "AppPathSubDirEnum",
     "open_app_path"
     # "INCLUDE_PROJECT_READMES",
     # "PACKAGE_DATA_PATH"
 ]
 
-from typing import Any
 from .app_path import *
 from .system_open_path_utilities import *
 
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
 PROJECT_ORGANISATION = "Pything"
 
-distributions = {v.key: v for v in pkg_resources.working_set}
-if PROJECT_NAME in distributions:
-    distribution = distributions[PROJECT_NAME]
-    DEVELOP = dist_is_editable(distribution)
-else:
+PACKAGE_DATA_PATH = resources.files(PROJECT_NAME) / "data"
+
+try:
+    DEVELOP = package_is_editable(PROJECT_NAME)
+except PackageNotFoundError as e:
     DEVELOP = True
 
 
 def get_version(append_time: Any = DEVELOP) -> str:
     """description"""
     version = __version__
     if not version:
```

### Comparing `Apppath-1.0.2/apppath/app_path.py` & `Apppath-1.0.3/apppath/app_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from warg import ensure_existence, sanitise_path
 from warg.os_utilities.platform_selection import SystemEnum, get_system
 
 
 class AppPath(object):
     r"""
     AppPath class for easing cross-platform access to proper app data directories
-    This class is an abstraction for getting system conventional application paths for data, logs, etc."""
+    This class is an abstraction for getting system conventional application paths for data, logs, etc.
+    """
 
     def __init__(
         self,
         app_name: str,
         app_author: str = None,
         app_version: str = None,
         roaming: bool = False,
```

### Comparing `Apppath-1.0.2/apppath/entry_points/clean_apppath.py` & `Apppath-1.0.3/apppath/entry_points/clean_apppath.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.2/apppath/entry_points/open_apppath.py` & `Apppath-1.0.3/apppath/entry_points/open_apppath.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.2/apppath/system_open_path_utilities.py` & `Apppath-1.0.3/apppath/system_open_path_utilities.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.2/pyproject.toml` & `Apppath-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.2/setup.py` & `Apppath-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from typing import List, Sequence, Union, TextIO
 
 
-def python_version_check(major: int = 3, minor: int = 7):
+def python_version_check(major: int = 3, minor: int = 8):
     """description"""
     import sys
 
     assert sys.version_info.major == major and sys.version_info.minor >= minor, (
         f"This project is utilises language features only present Python {major}.{minor} and greater. "
         f"You are running {sys.version_info}."
     )
```

### Comparing `Apppath-1.0.2/tests/test_app_path.py` & `Apppath-1.0.3/tests/test_app_path.py`

 * *Files identical despite different names*

