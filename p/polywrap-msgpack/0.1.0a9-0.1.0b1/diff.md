# Comparing `tmp/polywrap_msgpack-0.1.0a9.tar.gz` & `tmp/polywrap_msgpack-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_msgpack-0.1.0a9.tar", max compression
+gzip compressed data, was "polywrap_msgpack-0.1.0b1.tar", max compression
```

## Comparing `polywrap_msgpack-0.1.0a9.tar` & `polywrap_msgpack-0.1.0b1.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0        0 2022-10-16 06:28:28.670104 polywrap_msgpack-0.1.0a9/README.md
--rw-r--r--   0        0        0     3467 2023-03-02 19:36:47.836502 polywrap_msgpack-0.1.0a9/polywrap_msgpack/__init__.py
--rw-r--r--   0        0        0      643 2023-03-02 19:01:29.239002 polywrap_msgpack-0.1.0a9/polywrap_msgpack/generic_map.py
--rw-r--r--   0        0        0     1004 2023-03-02 20:08:58.642060 polywrap_msgpack-0.1.0a9/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0a9/setup.py
--rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0a9/PKG-INFO
+-rw-r--r--   0        0        0      704 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/README.md
+-rw-r--r--   0        0        0      431 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/polywrap_msgpack/__init__.py
+-rw-r--r--   0        0        0     2100 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/polywrap_msgpack/decoder.py
+-rw-r--r--   0        0        0     2432 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/polywrap_msgpack/encoder.py
+-rw-r--r--   0        0        0      781 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/polywrap_msgpack/errors.py
+-rw-r--r--   0        0        0      316 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/polywrap_msgpack/extensions/__init__.py
+-rw-r--r--   0        0        0     3126 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/polywrap_msgpack/extensions/generic_map.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/polywrap_msgpack/py.typed
+-rw-r--r--   0        0        0     2893 2023-08-01 17:46:03.391535 polywrap_msgpack-0.1.0b1/polywrap_msgpack/sanitize.py
+-rw-r--r--   0        0        0     1205 2023-08-01 17:46:36.161272 polywrap_msgpack-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0b1/PKG-INFO
```

### Comparing `polywrap_msgpack-0.1.0a9/polywrap_msgpack/__init__.py` & `polywrap_msgpack-0.1.0b1/polywrap_msgpack/sanitize.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,124 +1,89 @@
-"""
-polywrap-msgpack adds ability to encode/decode to/from msgpack format.
+"""This module contains the sanitize function that converts\
+    python values into msgpack compatible values."""
+from __future__ import annotations
 
-It provides msgpack_encode and msgpack_decode functions
-which allows user to encode and decode to/from msgpack bytes
-
-It also defines the default Extension types and extension hook for
-custom extension types defined by wrap standard
-"""
-from enum import Enum
 from typing import Any, Dict, List, Set, Tuple, cast
 
-import msgpack
-from msgpack.ext import ExtType
-from msgpack.exceptions import UnpackValueError
-
-from .generic_map import GenericMap
-
-
-class ExtensionTypes(Enum):
-    """Wrap msgpack extension types."""
-
-    GENERIC_MAP = 1
-
-
-def encode_ext_hook(obj: Any) -> ExtType:
-    """Extension hook for extending the msgpack supported types.
-
-    Args:
-        obj (Any): object to be encoded
-
-    Raises:
-        TypeError: when given object is not supported
-
-    Returns:
-        Tuple[int, bytes]: extension type code and payload
-    """
-    if isinstance(obj, GenericMap):
-        return ExtType(ExtensionTypes.GENERIC_MAP.value, msgpack_encode(obj._map)) # type: ignore
-    raise TypeError(f"Object of type {type(obj)} is not supported")
-
-
-def decode_ext_hook(code: int, data: bytes) -> Any:
-    """Extension hook for extending the msgpack supported types.
-
-    Args:
-        code (int): extension type code (>0 & <256)
-        data (bytes): msgpack deserializable data as payload
-
-    Raises:
-        UnpackValueError: when given invalid extension type code
-
-    Returns:
-        Any: decoded object
-    """
-    if code == ExtensionTypes.GENERIC_MAP.value:
-        return GenericMap(msgpack_decode(data))
-    raise UnpackValueError("Invalid Extention type")
+from .extensions.generic_map import GenericMap
 
 
 def sanitize(value: Any) -> Any:
-    """Sanitizes the value into msgpack encoder compatible format.
+    """Sanitize the value into msgpack encoder compatible format.
 
     Args:
-        value: any valid python value
+        value (Any): any valid python value
 
     Raises:
         ValueError: when dict key isn't string
 
     Returns:
         Any: msgpack compatible sanitized value
+
+    Examples:
+        >>> sanitize({"a": 1})
+        {'a': 1}
+        >>> sanitize({1, 2, 3})
+        [1, 2, 3]
+        >>> sanitize((1, 2, 3))
+        [1, 2, 3]
+        >>> sanitize([{1}, (2, 3), [4]])
+        [[1], [2, 3], [4]]
+        >>> class Foo: pass
+        >>> foo = Foo()
+        >>> foo.bar = 1
+        >>> sanitize(foo)
+        {'bar': 1}
+        >>> sanitize({1: 1})
+        Traceback (most recent call last):
+        ...
+        ValueError: Dict key must be string, got 1 of type <class 'int'>
+        >>> sanitize(GenericMap({1: 2}))
+        Traceback (most recent call last):
+        ...
+        ValueError: GenericMap key must be string, got 1 of type <class 'int'>
     """
     if isinstance(value, GenericMap):
-        return cast(Any, value)
+        dictionary: Dict[Any, Any] = cast(
+            GenericMap[Any, Any], value
+        )._map  # pyright: ignore[reportPrivateUsage]
+        new_map: GenericMap[str, Any] = GenericMap({})
+        for key, val in dictionary.items():
+            if not isinstance(key, str):
+                raise ValueError(
+                    f"GenericMap key must be string, got {key} of type {type(key)}"
+                )
+            new_map[key] = sanitize(val)
+        return new_map
     if isinstance(value, dict):
         dictionary: Dict[Any, Any] = value
+        new_dict: Dict[str, Any] = {}
         for key, val in dictionary.items():
-            dictionary[str(key)] = sanitize(val)
-        return dictionary
+            if not isinstance(key, str):
+                raise ValueError(
+                    f"Dict key must be string, got {key} of type {type(key)}"
+                )
+            new_dict[key] = sanitize(val)
+        return new_dict
     if isinstance(value, list):
         array: List[Any] = value
         return [sanitize(a) for a in array]
     if isinstance(value, tuple):
-        array: List[Any] = list(cast(Tuple[Any], value))  
+        array: List[Any] = list(cast(Tuple[Any], value))
         return sanitize(array)
     if isinstance(value, set):
-        set_val: Set[Any] = value
-        return list(set_val)
+        set_val: List[Any] = list(cast(Set[Any], value))
+        return sanitize(set_val)
     if isinstance(value, complex):
         return str(value)
     if hasattr(value, "__slots__"):
         return {
             s: sanitize(getattr(value, s))
             for s in getattr(value, "__slots__")
             if hasattr(value, s)
         }
     if hasattr(value, "__dict__"):
         return {k: sanitize(v) for k, v in cast(Dict[Any, Any], vars(value)).items()}
     return value
 
 
-def msgpack_encode(value: Any) -> bytes:
-    """Encode any python object into msgpack bytes.
-
-    Args:
-        value: any valid python object
-
-    Returns:
-        bytes: encoded msgpack value
-    """
-    sanitized = sanitize(value)
-    return msgpack.packb(sanitized, default=encode_ext_hook, use_bin_type=True)
-
-
-def msgpack_decode(val: bytes) -> Any:
-    """Decode msgpack bytes into a valid python object.
-
-    Args:
-        val: msgpack encoded bytes
-
-    Returns:
-        Any: python object
-    """
-    return msgpack.unpackb(val, ext_hook=decode_ext_hook)
+__all__ = ["sanitize"]
```

### Comparing `polywrap_msgpack-0.1.0a9/pyproject.toml` & `polywrap_msgpack-0.1.0b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-msgpack"
-version = "0.1.0a9"
+version = "0.1.0b1"
 description = "WRAP msgpack encoding"
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 msgpack = "^1.0.4"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+msgpack-types = "^0.2.0"
 pytest = "^7.1.2"
-pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
 pydocstyle = "^6.1.1"
+pycln = "^2.1.3"
+hypothesis = "^6.70.0"
+pytest-cov = "^4.0.0"
+pytest-xdist = "^3.2.1"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportShadowedImports = false
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
 
 [tool.pylint]
 disable = [
-    "too-many-return-statements",
+    "too-many-return-statements",  # too picky about return statements
+    "protected-access",  # Needed for internal use
+    "invalid-name",  # too picky about names
 ]
 ignore = [
     "tests/"
 ]
 
 [tool.isort]
 profile = "black"
```

