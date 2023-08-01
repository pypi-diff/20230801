# Comparing `tmp/conda_package_streaming-0.8.0.tar.gz` & `tmp/conda_package_streaming-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda_package_streaming-0.8.0.tar", last modified: Mon May  8 18:40:36 2023, max compression
+gzip compressed data, was "conda_package_streaming-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `conda_package_streaming-0.8.0.tar` & `conda_package_streaming-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2670 2023-05-08 18:38:19.008597 conda_package_streaming-0.8.0/LICENSE
--rw-r--r--   0        0        0     3165 2023-05-08 18:38:19.008779 conda_package_streaming-0.8.0/README.md
--rw-r--r--   0        0        0       22 2023-05-08 18:38:19.009078 conda_package_streaming-0.8.0/conda_package_streaming/__init__.py
--rw-r--r--   0        0        0      677 2023-05-08 18:38:19.009179 conda_package_streaming-0.8.0/conda_package_streaming/exceptions.py
--rw-r--r--   0        0        0     2538 2023-05-08 18:38:19.009288 conda_package_streaming-0.8.0/conda_package_streaming/extract.py
--rw-r--r--   0        0        0     9449 2023-05-08 18:38:19.009415 conda_package_streaming-0.8.0/conda_package_streaming/lazy_wheel.py
--rw-r--r--   0        0        0     3733 2023-05-08 18:38:19.009640 conda_package_streaming-0.8.0/conda_package_streaming/package_streaming.py
--rw-r--r--   0        0        0     2286 2023-05-08 18:38:19.009804 conda_package_streaming-0.8.0/conda_package_streaming/s3.py
--rw-r--r--   0        0        0     5663 2023-05-08 18:38:19.009938 conda_package_streaming-0.8.0/conda_package_streaming/transmute.py
--rw-r--r--   0        0        0     2707 2023-05-08 18:38:19.010056 conda_package_streaming-0.8.0/conda_package_streaming/url.py
--rw-r--r--   0        0        0     1314 2023-05-08 18:38:19.011624 conda_package_streaming-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4491 1970-01-01 00:00:00.000000 conda_package_streaming-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2670 2023-08-01 15:03:31.553652 conda_package_streaming-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3165 2023-08-01 15:03:31.553869 conda_package_streaming-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-01 15:03:31.554222 conda_package_streaming-0.9.0/conda_package_streaming/__init__.py
+-rw-r--r--   0        0        0      677 2023-08-01 15:03:31.554349 conda_package_streaming-0.9.0/conda_package_streaming/exceptions.py
+-rw-r--r--   0        0        0     2538 2023-08-01 15:03:31.554471 conda_package_streaming-0.9.0/conda_package_streaming/extract.py
+-rw-r--r--   0        0        0     9449 2023-08-01 15:03:31.554611 conda_package_streaming-0.9.0/conda_package_streaming/lazy_wheel.py
+-rw-r--r--   0        0        0     4819 2023-08-01 15:03:31.554806 conda_package_streaming-0.9.0/conda_package_streaming/package_streaming.py
+-rw-r--r--   0        0        0     2286 2023-08-01 15:03:31.555056 conda_package_streaming-0.9.0/conda_package_streaming/s3.py
+-rw-r--r--   0        0        0     5718 2023-08-01 15:03:31.555276 conda_package_streaming-0.9.0/conda_package_streaming/transmute.py
+-rw-r--r--   0        0        0     2707 2023-08-01 15:03:31.555425 conda_package_streaming-0.9.0/conda_package_streaming/url.py
+-rw-r--r--   0        0        0     1314 2023-08-01 15:03:31.557076 conda_package_streaming-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4491 1970-01-01 00:00:00.000000 conda_package_streaming-0.9.0/PKG-INFO
```

### Comparing `conda_package_streaming-0.8.0/LICENSE` & `conda_package_streaming-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.8.0/README.md` & `conda_package_streaming-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.8.0/conda_package_streaming/exceptions.py` & `conda_package_streaming-0.9.0/conda_package_streaming/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.8.0/conda_package_streaming/extract.py` & `conda_package_streaming-0.9.0/conda_package_streaming/extract.py`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.8.0/conda_package_streaming/lazy_wheel.py` & `conda_package_streaming-0.9.0/conda_package_streaming/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.8.0/conda_package_streaming/package_streaming.py` & `conda_package_streaming-0.9.0/conda_package_streaming/package_streaming.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
 Unpack conda packages without using a temporary file.
 """
 
 from __future__ import annotations
 
 import bz2
+import os
 import os.path
 import tarfile
 import zipfile
 from enum import Enum
 from typing import Generator
 
+# acquire umask taking advantage of import system lock, instead of possibly in
+# multiple threads at once.
+UMASK = os.umask(0)
+os.umask(UMASK)
+
 try:
     import zstandard
 except ImportError:
     import warnings
 
     warnings.warn("zstandard could not be imported. Running without .conda support.")
 
@@ -26,21 +32,43 @@
     info = "info"
 
     def __str__(self):
         return self.value
 
 
 class TarfileNoSameOwner(tarfile.TarFile):
+    def __init__(self, *args, umask=UMASK, **kwargs):
+        """Open an (uncompressed) tar archive `name'. `mode' is either 'r' to
+        read from an existing archive, 'a' to append data to an existing
+        file or 'w' to create a new file overwriting an existing one. `mode'
+        defaults to 'r'.
+        If `fileobj' is given, it is used for reading or writing data. If it
+        can be determined, `mode' is overridden by `fileobj's mode.
+        `fileobj' is not closed, when TarFile is closed.
+        """
+        super().__init__(*args, **kwargs)
+        self.umask = umask
+
     def chown(self, tarinfo, targetpath, numeric_owner):
         """
         Override chown to be a no-op, since we don't want to preserve ownership
         here. (tarfile.TarFile only lets us toggle all of (chown, chmod, mtime))
         """
         return
 
+    def chmod(self, tarinfo, targetpath):
+        """
+        Set file permissions of targetpath according to tarinfo, respecting
+        umask.
+        """
+        try:
+            os.chmod(targetpath, tarinfo.mode & (0o777 - self.umask))
+        except OSError as e:
+            raise tarfile.ExtractError("could not change mode") from e
+
 
 def tar_generator(
     fileobj, tarfile_open=TarfileNoSameOwner.open, closefd=False
 ) -> Generator[tuple[tarfile.TarFile, tarfile.TarInfo], None, None]:
     """
     Yield (tar, member) from fileobj.
     """
```

### Comparing `conda_package_streaming-0.8.0/conda_package_streaming/s3.py` & `conda_package_streaming-0.9.0/conda_package_streaming/s3.py`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.8.0/conda_package_streaming/transmute.py` & `conda_package_streaming-0.9.0/conda_package_streaming/transmute.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-Convert .tar.bz2 to .conda without temporary files.
+Convert .tar.bz2 to .conda
 
-Streams main `pkg-*` `.tar.zst` into open `ZipFile`, while buffering `info-*`
-`.tar.zst` in memory, writing it out at the end.
+Uses `tempfile.SpooledTemporaryFile` to buffer `pkg-*` `.tar` and `info-*`
+`.tar`, then compress directly into an open `ZipFile` at the end.
+`SpooledTemporaryFile` buffers the first 10MB of the package and its metadata in
+memory, but writes out to disk for larger packages.
 
-Works well for a typical ~10k `info-*`, but the conda format does not guarantee
-a small `info-*`.
-
-Conda packages created this way will also have `info-*` as the last element in
-the `ZipFile`, instead of the first for normal conda packages.
+Conda packages created this way have `info-*` as the last element in the
+`ZipFile`, instead of the first for `.conda` packages created with pre-2.0
+`conda-package-handling`.
 """
 
 from __future__ import annotations
 
 import json
 import os
 import shutil
```

### Comparing `conda_package_streaming-0.8.0/conda_package_streaming/url.py` & `conda_package_streaming-0.9.0/conda_package_streaming/url.py`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.8.0/pyproject.toml` & `conda_package_streaming-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.8.0/PKG-INFO` & `conda_package_streaming-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda_package_streaming
-Version: 0.8.0
+Version: 0.9.0
 Summary: An efficient library to read from new and old format .conda and .tar.bz2 conda packages.
 Author-email: "Anaconda, Inc. & Contributors" <conda@continuum.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

