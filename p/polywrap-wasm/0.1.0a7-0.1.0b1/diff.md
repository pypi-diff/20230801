# Comparing `tmp/polywrap_wasm-0.1.0a7.tar.gz` & `tmp/polywrap_wasm-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_wasm-0.1.0a7.tar", max compression
+gzip compressed data, was "polywrap_wasm-0.1.0b1.tar", max compression
```

## Comparing `polywrap_wasm-0.1.0a7.tar` & `polywrap_wasm-0.1.0b1.tar`

### file list

```diff
@@ -1,16 +1,39 @@
--rw-r--r--   0        0        0        4 2022-10-16 06:28:28.645779 polywrap_wasm-0.1.0a7/README.md
--rw-r--r--   0        0        0      228 2022-10-17 13:37:13.496919 polywrap_wasm-0.1.0a7/polywrap_wasm/__init__.py
--rw-r--r--   0        0        0     1880 2023-02-24 14:26:10.918069 polywrap_wasm-0.1.0a7/polywrap_wasm/buffer.py
--rw-r--r--   0        0        0       64 2023-02-22 15:57:14.720682 polywrap_wasm-0.1.0a7/polywrap_wasm/constants.py
--rw-r--r--   0        0        0      381 2022-10-16 06:28:28.649783 polywrap_wasm-0.1.0a7/polywrap_wasm/errors.py
--rw-r--r--   0        0        0    31434 2022-10-16 06:28:28.650532 polywrap_wasm-0.1.0a7/polywrap_wasm/example-wasm-files/wrap.wasm
--rw-r--r--   0        0        0      859 2022-10-27 11:21:02.039549 polywrap_wasm-0.1.0a7/polywrap_wasm/exports.py
--rw-r--r--   0        0        0    16304 2023-03-02 18:40:25.696994 polywrap_wasm-0.1.0a7/polywrap_wasm/imports.py
--rw-r--r--   0        0        0      994 2023-02-22 15:57:14.720770 polywrap_wasm-0.1.0a7/polywrap_wasm/inmemory_file_reader.py
--rw-r--r--   0        0        0       21 2022-10-16 06:28:28.652225 polywrap_wasm-0.1.0a7/polywrap_wasm/types/__init__.py
--rw-r--r--   0        0        0     1009 2023-02-22 15:57:14.720871 polywrap_wasm-0.1.0a7/polywrap_wasm/types/state.py
--rw-r--r--   0        0        0     2648 2023-02-22 15:57:14.721422 polywrap_wasm-0.1.0a7/polywrap_wasm/wasm_package.py
--rw-r--r--   0        0        0     3276 2023-02-22 15:57:14.721526 polywrap_wasm-0.1.0a7/polywrap_wasm/wasm_wrapper.py
--rw-r--r--   0        0        0     1133 2023-03-02 20:02:08.941294 polywrap_wasm-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0a7/setup.py
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0      872 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/README.md
+-rw-r--r--   0        0        0      182 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/__init__.py
+-rw-r--r--   0        0        0     3699 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/buffer.py
+-rw-r--r--   0        0        0      282 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/constants.py
+-rw-r--r--   0        0        0      491 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/errors.py
+-rw-r--r--   0        0        0     1693 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/exports.py
+-rw-r--r--   0        0        0       85 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/__init__.py
+-rw-r--r--   0        0        0     1854 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/abort.py
+-rw-r--r--   0        0        0      604 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/debug.py
+-rw-r--r--   0        0        0      940 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/env.py
+-rw-r--r--   0        0        0     3046 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/get_implementations.py
+-rw-r--r--   0        0        0     2372 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/invoke.py
+-rw-r--r--   0        0        0     5182 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/subinvoke.py
+-rw-r--r--   0        0        0      111 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/types/__init__.py
+-rw-r--r--   0        0        0     1657 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/types/base_wrap_imports.py
+-rw-r--r--   0        0        0     1626 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/imports/wrap_imports.py
+-rw-r--r--   0        0        0     1637 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/inmemory_file_reader.py
+-rw-r--r--   0        0        0     1162 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/instance.py
+-rw-r--r--   0        0        0      100 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/__init__.py
+-rw-r--r--   0        0        0     1143 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/abort.py
+-rw-r--r--   0        0        0      865 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/debug.py
+-rw-r--r--   0        0        0      813 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/env.py
+-rw-r--r--   0        0        0     2646 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/get_implementations.py
+-rw-r--r--   0        0        0     1864 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/invoke.py
+-rw-r--r--   0        0        0     3466 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/subinvoke.py
+-rw-r--r--   0        0        0     4502 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/subinvoke_implementation.py
+-rw-r--r--   0        0        0      104 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/types/__init__.py
+-rw-r--r--   0        0        0      309 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/types/base_wrap_linker.py
+-rw-r--r--   0        0        0     1580 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/linker/wrap_linker.py
+-rw-r--r--   0        0        0     1848 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/memory.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/py.typed
+-rw-r--r--   0        0        0      180 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/types/__init__.py
+-rw-r--r--   0        0        0      766 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/types/invoke_result.py
+-rw-r--r--   0        0        0      996 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/types/state.py
+-rw-r--r--   0        0        0      902 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/types/wasm_invoke_options.py
+-rw-r--r--   0        0        0     3529 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/wasm_package.py
+-rw-r--r--   0        0        0     5642 2023-08-01 17:46:03.403536 polywrap_wasm-0.1.0b1/polywrap_wasm/wasm_wrapper.py
+-rw-r--r--   0        0        0     1138 2023-08-01 17:51:18.926937 polywrap_wasm-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0b1/PKG-INFO
```

### Comparing `polywrap_wasm-0.1.0a7/polywrap_wasm/inmemory_file_reader.py` & `polywrap_wasm-0.1.0b1/polywrap_wasm/inmemory_file_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,51 @@
+"""This module contains the InMemoryFileReader type for reading files from memory."""
 from typing import Optional
 
-from polywrap_core import IFileReader
-from polywrap_result import Ok, Result
+from polywrap_core import FileReader
 
 from .constants import WRAP_MANIFEST_PATH, WRAP_MODULE_PATH
 
 
-class InMemoryFileReader(IFileReader):
+class InMemoryFileReader(FileReader):
+    """InMemoryFileReader is an implementation of the FileReader protocol\
+        that reads files from memory.
+
+    Args:
+        base_file_reader (FileReader): The base file reader\
+            used to read any files.
+        wasm_module (Optional[bytes]): The Wasm module file of the wrapper.
+        wasm_manifest (Optional[bytes]): The manifest of the wrapper.
+    """
+
     _wasm_manifest: Optional[bytes]
     _wasm_module: Optional[bytes]
-    _base_file_reader: IFileReader
+    _base_file_reader: FileReader
 
     def __init__(
         self,
-        base_file_reader: IFileReader,
+        base_file_reader: FileReader,
         wasm_module: Optional[bytes] = None,
         wasm_manifest: Optional[bytes] = None,
     ):
+        """Initialize a new InMemoryFileReader instance."""
         self._wasm_module = wasm_module
         self._wasm_manifest = wasm_manifest
         self._base_file_reader = base_file_reader
 
-    async def read_file(self, file_path: str) -> Result[bytes]:
+    def read_file(self, file_path: str) -> bytes:
+        """Read a file from memory.
+
+        Args:
+            file_path: The path of the file to read.
+
+        Returns:
+            The file contents or an error.
+        """
         if file_path == WRAP_MODULE_PATH and self._wasm_module:
-            return Ok(self._wasm_module)
-        elif file_path == WRAP_MANIFEST_PATH and self._wasm_manifest:
-            return Ok(self._wasm_manifest)
-        else:
-            return await self._base_file_reader.read_file(file_path=file_path)
+            return self._wasm_module
+        if file_path == WRAP_MANIFEST_PATH and self._wasm_manifest:
+            return self._wasm_manifest
+        return self._base_file_reader.read_file(file_path=file_path)
+
+
+__all__ = ["InMemoryFileReader"]
```

### Comparing `polywrap_wasm-0.1.0a7/pyproject.toml` & `polywrap_wasm-0.1.0b1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-wasm"
-version = "0.1.0a7"
+version = "0.1.0b1"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-wasmtime = "^1.0.1"
-polywrap-core = "0.1.0a7"
-polywrap-manifest = "0.1.0a7"
-polywrap-msgpack = "0.1.0a7"
-polywrap-result = "0.1.0a7"
-unsync = "^1.4.0"
+wasmtime = "^9.0.0"
+polywrap-msgpack = "^0.1.0b1"
+polywrap-manifest = "^0.1.0b1"
+polywrap-core = "^0.1.0b1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pycln = "^2.1.3"
 pytest = "^7.1.2"
-pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
@@ -38,22 +36,24 @@
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
+    "too-few-public-methods",
+    "broad-exception-caught",
+    "too-many-arguments",
+    "duplicate-code",
 ]
 ignore = [
     "tests/"
 ]
 
 [tool.isort]
 profile = "black"
```

