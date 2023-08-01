# Comparing `tmp/kaparoo_python-0.1.1.tar.gz` & `tmp/kaparoo_python-0.1.2.tar.gz`

## Comparing `kaparoo_python-0.1.1.tar` & `kaparoo_python-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/beartype/__init__.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/beartype/numerics.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/filesystem/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/filesystem/exceptions.py
--rw-r--r--   0        0        0    24132 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/filesystem/path.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/filesystem/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/utils/__init__.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/utils/optional.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/kaparoo/utils/types.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/LICENSE
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/README.md
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 kaparoo_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/beartype/__init__.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/beartype/numerics.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/__init__.py
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/directory.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/exceptions.py
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/existence.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/types.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/filesystem/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/utils/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/utils/optional.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/kaparoo/utils/types.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/README.md
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 kaparoo_python-0.1.2/PKG-INFO
```

### Comparing `kaparoo_python-0.1.1/kaparoo/beartype/numerics.py` & `kaparoo_python-0.1.2/kaparoo/beartype/numerics.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.1/kaparoo/filesystem/__init__.py` & `kaparoo_python-0.1.2/kaparoo/filesystem/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 # -*- coding: utf-8 -*-
 
 __all__ = (
     # exceptions
+    "AbsolutePathError",
     "DirectoryNotFoundError",
     "NotAFileError",
     # types
     "StrPath",
     "StrPaths",
-    # path
-    # - stringify
+    # utils
+    "join_prefix",
     "stringify_path",
     "stringify_paths",
-    # - single existence
-    "check_if_path_exists",
-    "check_if_file_exists",
+    # existence
     "check_if_dir_exists",
-    # - multiple existences
-    "check_if_paths_exist",
-    "check_if_files_exist",
     "check_if_dirs_exist",
-    # - child path(s) search
-    "get_paths",
-    "get_files",
+    "check_if_file_exists",
+    "check_if_files_exist",
+    "check_if_path_exists",
+    "check_if_paths_exist",
+    "dir_exists",
+    "dirs_exist",
+    "file_exists",
+    "files_exist",
+    "path_exists",
+    "paths_exist",
+    # directory
+    "empty_dir",
+    "empty_dirs",
     "get_dirs",
-    # - empty directory check
-    "is_empty_dir",
-    "is_empty_dir_unsafe",
-    "are_empty_dirs",
-    "are_empty_dirs_unsafe",
+    "get_files",
+    "get_paths",
+    "make_dirs",
 )
 
-from kaparoo.filesystem.exceptions import DirectoryNotFoundError, NotAFileError
-from kaparoo.filesystem.path import (
-    are_empty_dirs,
-    are_empty_dirs_unsafe,
+from kaparoo.filesystem.directory import (
+    empty_dir,
+    empty_dirs,
+    get_dirs,
+    get_files,
+    get_paths,
+    make_dirs,
+)
+from kaparoo.filesystem.exceptions import (
+    AbsolutePathError,
+    DirectoryNotFoundError,
+    NotAFileError,
+)
+from kaparoo.filesystem.existence import (
     check_if_dir_exists,
     check_if_dirs_exist,
     check_if_file_exists,
     check_if_files_exist,
     check_if_path_exists,
     check_if_paths_exist,
-    get_dirs,
-    get_files,
-    get_paths,
-    is_empty_dir,
-    is_empty_dir_unsafe,
+    dir_exists,
+    dirs_exist,
+    file_exists,
+    files_exist,
+    path_exists,
+    paths_exist,
+)
+from kaparoo.filesystem.types import StrPath, StrPaths
+from kaparoo.filesystem.utils import (
+    join_prefix,
     stringify_path,
     stringify_paths,
 )
-from kaparoo.filesystem.types import StrPath, StrPaths
```

### Comparing `kaparoo_python-0.1.1/kaparoo/utils/optional.py` & `kaparoo_python-0.1.2/kaparoo/utils/optional.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,89 +24,80 @@
 
 @overload
 def replace_if_none(optional: T, surrogate: U) -> T:
     ...
 
 
 def replace_if_none(optional: T | None, surrogate: U) -> T | U:
-    """Replace the value with a surrogate if it is None.
+    """Replace the value if it is None.
 
     Args:
         optional: The optional value to be checked.
-        surrogate: The surrogate value to use if `optional` is None.
+        surrogate: The value to be returned if `optional` is None.
 
     Returns:
         The `optional` value if it is not None, otherwise the `surrogate` value.
     """
     return surrogate if optional is None else optional
 
 
 @overload
-def factory_if_none(
-    optional: None,
-    factory: Callable[[], U],
-) -> U:
+def factory_if_none(optional: None, factory: Callable[[], U]) -> U:
     ...
 
 
 @overload
-def factory_if_none(
-    optional: T,
-    factory: Callable[[], U],
-) -> T:
+def factory_if_none(optional: T, factory: Callable[[], U]) -> T:
     ...
 
 
-def factory_if_none(
-    optional: T | None,
-    factory: Callable[[], U],
-) -> T | U:
-    """Create a value using a factory if the optional value is None.
+def factory_if_none(optional: T | None, factory: Callable[[], U]) -> T | U:
+    """Replace the value using the factory if it is None.
 
     Args:
         optional: The optional value to be checked.
-        factory: A callable that returns the value to be used if `optional` is None.
+        factory: A callable that creates a value if `optional` is None.
 
     Returns:
-        The `optional` value if it is not None, otherwise the value returned by `factory`.
+        The `optional` value if it is not None, otherwise the value created by `factory`.
     """  # noqa: E501
     return factory() if optional is None else optional
 
 
 def unwrap_or_default(
     optional: T | None,
     default: T,
     callback: Callable[[T], T] | None = None,
 ) -> T:
-    """Unwrap the value or return a default value if it is None.
+    """Unwrap the optional value or replace it with a default if it is None.
 
     Args:
         optional: The optional value to be checked.
-        default: The default value to be returned if `optional` is None.
+        default: The value to be returned if `optional` is None.
         callback: An optional callable to be applied to the result. Defaults to None.
 
     Returns:
         The `optional` value if it is not None, otherwise the `default` value.
-        If a `callback` is provided, it is applied to the result before returning.
+            If a `callback` is provided, it is applied to the result before returning.
     """
     result = replace_if_none(optional, default)
     return callback(result) if callable(callback) else result
 
 
 def unwrap_or_factory(
     optional: T | None,
     factory: Callable[[], T],
     callback: Callable[[T], T] | None = None,
 ) -> T:
-    """Unwrap the value or create a value using a factory if it is None.
+    """Unwrap the optional value or replace it using the factory if it is None.
 
     Args:
         optional: The optional value to be checked.
-        factory: A callable that returns the value to be used if `optional` is None.
+        factory: A callable that creates a value if `optional` is None.
         callback: An optional callable to be applied to the result. Defaults to None.
 
     Returns:
-        The `optional` value if it is not None, otherwise the value returned by `factory`.
-        If a `callback` is provided, it is applied to the result before returning.
+        The `optional` value if it is not None, otherwise the value created by `factory`.
+            If `callback` is provided, it is applied to the result before returning.
     """  # noqa: E501
     result = factory_if_none(optional, factory)
     return callback(result) if callable(callback) else result
```

### Comparing `kaparoo_python-0.1.1/.gitignore` & `kaparoo_python-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.1/LICENSE` & `kaparoo_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.1/README.md` & `kaparoo_python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_python-0.1.1/pyproject.toml` & `kaparoo_python-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,27 @@
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
 ]
 dependencies = [
     "beartype>=0.14.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch>=1.7.0",
-    "ruff>=0.0.277",
+    "ruff>=0.0.280",
     "mypy>=1.4.1",
     "black>=23.7.0",
     "pytest>=7.4.0",
     "pytest-order>=1.1.0",
 ]
 
 [project.urls]
```

### Comparing `kaparoo_python-0.1.1/PKG-INFO` & `kaparoo_python-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for (personally) common and useful features.
 Project-URL: GitHub, https://www.github.com/kaparoo/python-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
         
@@ -30,25 +30,26 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: beartype>=0.14.1
 Provides-Extra: dev
 Requires-Dist: black>=23.7.0; extra == 'dev'
 Requires-Dist: hatch>=1.7.0; extra == 'dev'
 Requires-Dist: mypy>=1.4.1; extra == 'dev'
 Requires-Dist: pytest-order>=1.1.0; extra == 'dev'
 Requires-Dist: pytest>=7.4.0; extra == 'dev'
-Requires-Dist: ruff>=0.0.277; extra == 'dev'
+Requires-Dist: ruff>=0.0.280; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # ***kaparoo-python-package***
 
 
 
 <!-- [              MARKDOWN BADGES              ] -->
```

