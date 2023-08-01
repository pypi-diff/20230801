# Comparing `tmp/modelscan-0.1.0.tar.gz` & `tmp/modelscan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelscan-0.1.0.tar", max compression
+gzip compressed data, was "modelscan-0.1.1.tar", max compression
```

## Comparing `modelscan-0.1.0.tar` & `modelscan-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10754 2023-07-27 22:53:02.959662 modelscan-0.1.0/LICENSE
--rw-r--r--   0        0        0     4152 2023-07-27 22:53:02.959662 modelscan-0.1.0/README.md
--rw-r--r--   0        0        0      155 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/__init__.py
--rw-r--r--   0        0        0       22 2023-07-27 22:53:24.867857 modelscan-0.1.0/modelscan/_version.py
--rw-r--r--   0        0        0     2304 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/cli.py
--rw-r--r--   0        0        0      530 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/error.py
--rw-r--r--   0        0        0     2626 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/issues.py
--rw-r--r--   0        0        0      198 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/models/h5/__init__.py
--rw-r--r--   0        0        0     2308 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/models/h5/scan.py
--rw-r--r--   0        0        0        0 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/models/pickle/__init__.py
--rw-r--r--   0        0        0     1963 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/models/pickle/scan.py
--rw-r--r--   0        0        0        0 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/models/saved_model/__init__.py
--rw-r--r--   0        0        0     5049 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/models/saved_model/scan.py
--rw-r--r--   0        0        0      620 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/models/scan.py
--rw-r--r--   0        0        0     4154 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/modelscan.py
--rw-r--r--   0        0        0     2052 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/reports.py
--rw-r--r--   0        0        0     1072 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/tools/LICENSE
--rw-r--r--   0        0        0     9634 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/tools/picklescanner.py
--rw-r--r--   0        0        0     3688 2023-07-27 22:53:02.963662 modelscan-0.1.0/modelscan/tools/utils.py
--rw-r--r--   0        0        0     1276 2023-07-27 22:53:25.267862 modelscan-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 modelscan-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10754 2023-08-01 00:26:57.102215 modelscan-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4152 2023-08-01 00:26:57.102215 modelscan-0.1.1/README.md
+-rw-r--r--   0        0        0      155 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-01 00:27:27.294091 modelscan-0.1.1/modelscan/_version.py
+-rw-r--r--   0        0        0     2304 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/cli.py
+-rw-r--r--   0        0        0      530 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/error.py
+-rw-r--r--   0        0        0     2742 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/issues.py
+-rw-r--r--   0        0        0      198 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/h5/__init__.py
+-rw-r--r--   0        0        0     2308 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/h5/scan.py
+-rw-r--r--   0        0        0        0 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/pickle/__init__.py
+-rw-r--r--   0        0        0     1963 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/pickle/scan.py
+-rw-r--r--   0        0        0        0 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/saved_model/__init__.py
+-rw-r--r--   0        0        0     5049 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/saved_model/scan.py
+-rw-r--r--   0        0        0      620 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/scan.py
+-rw-r--r--   0        0        0     4483 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/modelscan.py
+-rw-r--r--   0        0        0     2052 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/reports.py
+-rw-r--r--   0        0        0     1072 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/tools/LICENSE
+-rw-r--r--   0        0        0     9387 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/tools/picklescanner.py
+-rw-r--r--   0        0        0     3800 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/tools/utils.py
+-rw-r--r--   0        0        0     1276 2023-08-01 00:27:27.762089 modelscan-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 modelscan-0.1.1/PKG-INFO
```

### Comparing `modelscan-0.1.0/LICENSE` & `modelscan-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/README.md` & `modelscan-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/cli.py` & `modelscan-0.1.1/modelscan/cli.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/error.py` & `modelscan-0.1.1/modelscan/error.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/issues.py` & `modelscan-0.1.1/modelscan/issues.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 import logging
 from enum import Enum
 from pathlib import Path
-from typing import List, Union, Dict
+from typing import List, Union, Dict, Optional
 
 from collections import defaultdict
 
 logger = logging.getLogger("modelscan")
 
 
 class IssueSeverity(Enum):
@@ -58,16 +58,21 @@
         print(f"\n{issue_description} found:")
         print(f"  - Severity: {self.severity.name}")
         for output_line in self.details.output_lines():
             print(f"  - {output_line}")
 
 
 class Issues:
-    def __init__(self, issues: List[Issue] = []) -> None:
-        self.all_issues: List[Issue] = issues
+    all_issues: List[Issue]
+
+    def __init__(self, issues: Optional[List[Issue]] = None) -> None:
+        if issues is None:
+            self.all_issues = []
+        else:
+            self.all_issues = issues
 
     def add_issue(self, issue: Issue) -> None:
         """
         Add a single issue
         """
         self.all_issues.append(issue)
```

### Comparing `modelscan-0.1.0/modelscan/models/h5/scan.py` & `modelscan-0.1.1/modelscan/models/h5/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/models/pickle/scan.py` & `modelscan-0.1.1/modelscan/models/pickle/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/models/saved_model/scan.py` & `modelscan-0.1.1/modelscan/models/saved_model/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/models/scan.py` & `modelscan-0.1.1/modelscan/models/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/modelscan.py` & `modelscan-0.1.1/modelscan/modelscan.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,19 +63,26 @@
             if file_name is not None
         ]
 
         # Scan model files
         for file_name in file_names:
             file_ext = os.path.splitext(file_name)[1]
             url = f"https://huggingface.co/{repo_id}/resolve/main/{file_name}"
-            self._scan_source(
-                source=url,
-                extension=file_ext,
-                data=io.BytesIO(_http_get(url)),
-            )
+            data = io.BytesIO(_http_get(url))
+            if (
+                _is_zipfile(source=url, data=data)
+                or file_ext in self._supported_zip_extensions()
+            ):
+                self._scan_zip(source=url, data=data)
+            else:
+                self._scan_source(
+                    source=url,
+                    extension=file_ext,
+                    data=data,
+                )
 
     def scan_url(self, url: str) -> None:
         # Todo: before it was just scanning scanning_pickle_bytes
         # We need to validate this url and determine what type of file it is
         # self._scan_bytes(
         #     data=io.BytesIO(_http_get(url)),
         #     source=url,
@@ -101,16 +108,18 @@
             if extension in scan.supported_extensions():
                 logger.info(f"Scanning {source} using {scan.name()} model scan")
                 issues, errors = scan.scan(source=source, data=data)
 
         self._issues.add_issues(issues)
         self._errors.extend(errors)
 
-    def _scan_zip(self, source: Union[str, Path]) -> None:
-        with zipfile.ZipFile(source, "r") as zip:
+    def _scan_zip(
+        self, source: Union[str, Path], data: Optional[IO[bytes]] = None
+    ) -> None:
+        with zipfile.ZipFile(data if data else source, "r") as zip:
             file_names = zip.namelist()
             for file_name in file_names:
                 file_ext = os.path.splitext(file_name)[1]
                 with zip.open(file_name, "r") as file_io:
                     self._scan_source(
                         source=f"{source}:{file_name}",
                         extension=file_ext,
```

### Comparing `modelscan-0.1.0/modelscan/reports.py` & `modelscan-0.1.1/modelscan/reports.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/tools/LICENSE` & `modelscan-0.1.1/modelscan/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.0/modelscan/tools/picklescanner.py` & `modelscan-0.1.1/modelscan/tools/picklescanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,14 @@
             ModelScanError(scan_name, f"Error parsing pickle file {source}: {e}")
         ]
 
     logger.debug("Global imports in %s: %s", source, raw_globals)
 
     for rg in raw_globals:
         global_module, global_name, severity = rg[0], rg[1], None
-        safe_filter = _safe_globals.get(global_module)
         unsafe_critical_filter = _unsafe_globals["CRITICAL"].get(global_module)
         unsafe_high_filter = _unsafe_globals["HIGH"].get(global_module)
         unsafe_medium_filter = _unsafe_globals["MEDIUM"].get(global_module)
         unsafe_low_filter = _unsafe_globals["LOW"].get(global_module)
         if unsafe_critical_filter is not None and (
             unsafe_critical_filter == "*" or global_name in unsafe_critical_filter
         ):
@@ -210,20 +209,14 @@
             severity = IssueSeverity.MEDIUM
         elif unsafe_low_filter is not None and (
             unsafe_low_filter == "*" or global_name in unsafe_low_filter
         ):
             severity = IssueSeverity.LOW
         elif "unknown" in global_module or "unknown" in global_name:
             severity = IssueSeverity.MEDIUM
-        elif (
-            unsafe_critical_filter is None
-            and unsafe_high_filter is None
-            and safe_filter is None
-        ):
-            severity = IssueSeverity.MEDIUM
         else:
             continue
         issues.append(
             Issue(
                 code=IssueCode.UNSAFE_OPERATOR,
                 severity=severity,
                 details=OperatorIssueDetails(
```

### Comparing `modelscan-0.1.0/modelscan/tools/utils.py` & `modelscan-0.1.1/modelscan/tools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,34 +48,40 @@
         return False
     except AttributeError:
         return False
 
 
 # copied from pytorch code
 # https://github.com/pytorch/pytorch/blob/0b3316ad2c6ff61416597ef29e8865876dcb12f5/torch/serialization.py#L66
-def _is_zipfile(source: Union[Path, str]) -> bool:
+def _is_zipfile(source: Union[Path, str], data: Optional[IO[bytes]] = None) -> bool:
     # This is a stricter implementation than zipfile.is_zipfile().
     # zipfile.is_zipfile() is True if the magic number appears anywhere in the
     # binary. Since we expect the files here to be generated by torch.save or
     # torch.jit.save, it's safe to only check the start bytes and avoid
     # collisions and assume the zip has only 1 file.
     # See bugs.python.org/issue28494.
+    if not data:
+        data = open(source, "rb")
+        file = True
+    else:
+        file = False
 
     # Read the first 4 bytes of the file
-    with open(source, "rb") as f:
-        read_bytes = []
-        start = f.tell()
-
-        byte = f.read(1)
-        while byte != b"":
-            read_bytes.append(byte)
-            if len(read_bytes) == 4:
-                break
-            byte = f.read(1)
-        f.seek(start)
+    read_bytes = []
+    start = data.tell()
+
+    byte = data.read(1)
+    while byte != b"":
+        read_bytes.append(byte)
+        if len(read_bytes) == 4:
+            break
+        byte = data.read(1)
+    data.seek(start)
+    if file:
+        data.close()
 
     local_header_magic_number = [b"P", b"K", b"\x03", b"\x04"]
     return read_bytes == local_header_magic_number
 
 
 def get_magic_number(data: IO[bytes]) -> Optional[int]:
     for opcode, args, _ in genops(data):
```

### Comparing `modelscan-0.1.0/pyproject.toml` & `modelscan-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelscan"
-version = "0.1.0"
+version = "0.1.1"
 description = "The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats."
 authors = ["ProtectAI <community@protectai.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{ include = "modelscan" }]
 exclude = ["tests/*", "Makefile"]
```

### Comparing `modelscan-0.1.0/PKG-INFO` & `modelscan-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelscan
-Version: 0.1.0
+Version: 0.1.1
 Summary: The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats.
 License: Apache-2.0
 Author: ProtectAI
 Author-email: community@protectai.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelscan Version: 0.1.0 Summary: The modelscan
+Metadata-Version: 2.1 Name: modelscan Version: 0.1.1 Summary: The modelscan
 package is a cli tool for detecting unsafe operations in model files across
 various model serialization formats. License: Apache-2.0 Author: ProtectAI
 Author-email: community@protectai.com Requires-Python: >=3.8,<3.11 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Provides-Extra: h5py Provides-Extra: tensorflow
```

