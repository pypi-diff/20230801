# Comparing `tmp/runpandarun-0.2.5.tar.gz` & `tmp/runpandarun-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpandarun-0.2.5.tar", max compression
+gzip compressed data, was "runpandarun-0.3.0.tar", max compression
```

## Comparing `runpandarun-0.2.5.tar` & `runpandarun-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-15 09:47:01.438078 runpandarun-0.2.5/LICENSE
--rw-r--r--   0        0        0     9535 2023-07-24 12:17:57.602391 runpandarun-0.2.5/README.md
--rw-r--r--   0        0        0     1445 2023-07-24 12:02:46.793891 runpandarun-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      145 2023-07-24 12:02:46.793891 runpandarun-0.2.5/runpandarun/__init__.py
--rw-r--r--   0        0        0     1111 2023-07-19 09:57:41.380531 runpandarun-0.2.5/runpandarun/cli.py
--rw-r--r--   0        0        0       37 2023-07-15 09:47:01.438078 runpandarun-0.2.5/runpandarun/exceptions.py
--rw-r--r--   0        0        0     3812 2023-07-21 09:39:05.058473 runpandarun-0.2.5/runpandarun/io.py
--rw-r--r--   0        0        0     2864 2023-07-21 08:03:58.316549 runpandarun-0.2.5/runpandarun/playbook.py
--rw-r--r--   0        0        0     2146 2023-07-19 09:57:41.380531 runpandarun-0.2.5/runpandarun/util.py
--rw-r--r--   0        0        0    10949 1970-01-01 00:00:00.000000 runpandarun-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-15 09:47:01.438078 runpandarun-0.3.0/LICENSE
+-rw-r--r--   0        0        0    10474 2023-08-01 10:06:21.601275 runpandarun-0.3.0/README.md
+-rw-r--r--   0        0        0     1466 2023-08-01 10:05:22.129295 runpandarun-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-08-01 10:05:22.129295 runpandarun-0.3.0/runpandarun/__init__.py
+-rw-r--r--   0        0        0     1111 2023-07-19 09:57:41.380531 runpandarun-0.3.0/runpandarun/cli.py
+-rw-r--r--   0        0        0     1112 2023-08-01 10:04:38.949314 runpandarun-0.3.0/runpandarun/datapatch.py
+-rw-r--r--   0        0        0       37 2023-07-15 09:47:01.438078 runpandarun-0.3.0/runpandarun/exceptions.py
+-rw-r--r--   0        0        0     3746 2023-07-28 18:28:39.258003 runpandarun-0.3.0/runpandarun/io.py
+-rw-r--r--   0        0        0     3181 2023-08-01 10:04:38.949314 runpandarun-0.3.0/runpandarun/playbook.py
+-rw-r--r--   0        0        0      269 2023-08-01 10:04:38.949314 runpandarun-0.3.0/runpandarun/types.py
+-rw-r--r--   0        0        0     2111 2023-07-28 18:27:34.273930 runpandarun-0.3.0/runpandarun/util.py
+-rw-r--r--   0        0        0    11930 1970-01-01 00:00:00.000000 runpandarun-0.3.0/PKG-INFO
```

### Comparing `runpandarun-0.2.5/LICENSE` & `runpandarun-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runpandarun-0.2.5/README.md` & `runpandarun-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 # Run Panda Run
 
 :panda_face: :panda_face: :panda_face: :panda_face: :panda_face: :panda_face: :panda_face:
 
 A simple interface written in python for reproducible i/o workflows around tabular data via [pandas](https://pandas.pydata.org/) `DataFrame` specified via `yaml` "playbooks".
 
+Apart from any `pandas` function possible that can alter data, also [datapatch](https://github.com/pudo/datapatch) is included for an additional and easier way to patch data.
+
 **NOTICE**
 
 As of july 2023, this package only handles pandas transform logic, no data warehousing anymore.  See [archived version](https://github.com/simonwoerpel/runpandarun/tree/master)
 
 ## Quickstart
 
 [Install via pip](#installation)
@@ -201,14 +203,20 @@
 
   - handler: DataFrame.sort_values
     options:
       by:
         - state
         - city
 
+patch:
+  city:
+    options:
+      - match: Zarizri
+        value: Zar1zr1
+
 write:
   uri: ftp://user:${FTP_PASSWORD}@host/data.csv
   options:
     index: false
 ```
 
 ## How to...
@@ -296,17 +304,45 @@
 ```yaml
 read:
   uri: postgresql://user:password@host/database
   options:
     sql: "SELECT * FROM my_table WHERE category = 'A'"
 ```
 
+### Patch data
+
+Apart from any `pandas` function possible that can alter data, also [datapatch](https://github.com/pudo/datapatch) is included for an additional and easier way to patch data.
+
+Simply add a `patch` config to the yaml. Refer to the datapatch readme for details.
+
+The patching is applied *after* all the `operations` are applied.
+
+```yaml
+patch:
+  countries:
+    normalize: true
+    lowercase: true
+    options:
+      - match: Frankreich
+        value: France
+      - match:
+          - Northkorea
+          - Nordkorea
+          - Northern Korea
+          - NKorea
+          - DPRK
+        value: North Korea
+      - contains: Britain
+        value: Great Britain
+```
+
+
 ## save eval
 
-Ok wait, you are executing arbitrary python code in the yaml specs?
+**Ok wait, you are executing arbitrary python code in the yaml specs?**
 
 Not really, there is a strict allow list of possible modules that can be used. See [runpandarun.util.safe_eval](https://github.com/investigativedata/runpandarun/blob/develop/runpandarun/util.py)
 
 This includes:
 - any pandas or numpy modules
 - [normality](https://github.com/pudo/normality/)
 - [fingerprints](https://github.com/alephdata/fingerprints)
```

### Comparing `runpandarun-0.2.5/pyproject.toml` & `runpandarun-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runpandarun"
-version = "0.2.5"
+version = "0.3.0"
 description = "Tell pandas what to do – easy tabular data I/O playbooks"
 authors = ["Simon Wörpel <simon@investigativedata.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://investigraph.dev"
 repository = "https://github.com/investigativedata/investigraph-etl"
 documentation = "https://docs.investigraph.dev/runpandarun"
@@ -35,14 +35,15 @@
 fsspec = "^2023.6.0"
 s3fs = "^2023.6.0"
 orjson = "^3.9.2"
 pantomime = "^0.6.1"
 openpyxl = "^3.1.2"
 sqlalchemy = "^2.0.19"
 aiohttp = ">=3.8.5"
+datapatch = "^1.0.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
```

### Comparing `runpandarun-0.2.5/runpandarun/cli.py` & `runpandarun-0.3.0/runpandarun/cli.py`

 * *Files identical despite different names*

### Comparing `runpandarun-0.2.5/runpandarun/io.py` & `runpandarun-0.3.0/runpandarun/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import sys
-from io import BytesIO, StringIO
-from typing import Any, TypeVar
+from typing import Any
 from urllib.parse import urlparse
 
 import fsspec
 import orjson
 import pandas as pd
 from pantomime import types
 from pydantic import BaseModel
 from pydantic import validator as field_validator
 
 from .exceptions import SpecError
-from .util import PathLike, guess_mimetype
-
-IO = TypeVar("IO", bound=StringIO | BytesIO)
+from .types import IO, PathLike
+from .util import guess_mimetype
 
 
 class Handler(BaseModel):
     options: dict[str, Any] | None = {}
     uri: str | None = "-"
     handler: str | None = None
```

### Comparing `runpandarun-0.2.5/runpandarun/playbook.py` & `runpandarun-0.3.0/runpandarun/playbook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from pathlib import Path
 from typing import Any, TypeVar
 
 import yaml
 from pandas import DataFrame, Series
 from pydantic import BaseModel, root_validator
 
+from .datapatch import Patches, apply_patches
 from .exceptions import SpecError
 from .io import ReadHandler, WriteHandler
-from .util import PathLike, absolute_path_uri, expandvars, getattr_by_path, safe_eval
+from .types import PathLike
+from .util import absolute_path_uri, expandvars, getattr_by_path, safe_eval
 
 P = TypeVar("P", bound="Playbook")
 
 
 class ExpandMixin:
     def __init__(self, **data):
         super().__init__(**expandvars(data))
@@ -47,41 +49,49 @@
         try:
             getattr_by_path(MODULES[module], func)
         except Exception as e:
             raise SpecError(f"Could not load function `{handler}`: {e}")
         return values
 
     def apply(self, df: DataFrame) -> DataFrame:
-        if "func" in self.options:
-            self.options["func"] = safe_eval(self.options["func"])
+        options = {}
+        for key, value in self.options.items():
+            if key == "func" or (isinstance(value, str) and value.startswith("lambda")):
+                options[key] = safe_eval(value)
+            else:
+                options[key] = value
         _, func = self.handler.split(".", 1)
         if self.column:
             func = getattr_by_path(df[self.column], func)
-            df[self.column] = func(**self.options)
+            df[self.column] = func(**options)
         else:
             func = getattr_by_path(df, func)
-            df = func(**self.options)
+            df = func(**options)
         return df
 
 
 class Playbook(ExpandMixin, BaseModel):
     read: ReadHandler | None = ReadHandler()
     operations: list[Operation] | None = []
+    patch: Patches | None = None
     write: WriteHandler | None = WriteHandler()
 
     class Config:
         extra = "forbid"
 
     def run(self, df: DataFrame | None = None, write: bool | None = False) -> DataFrame:
         if df is None:
             df = self.read.handle()
 
         for op in self.operations:
             df = op.apply(df)
 
+        if self.patch:
+            df = apply_patches(self.patch, df)
+
         if write:
             self.write.handle(df)
         return df
 
     @classmethod
     def from_yaml(cls, path: PathLike) -> P:
         path = Path(path)
```

### Comparing `runpandarun-0.2.5/runpandarun/util.py` & `runpandarun-0.3.0/runpandarun/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import mimetypes
 import os
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import Any, TypeAlias
+from typing import Any
 from urllib.parse import urlparse
 
 import banal
 import fingerprints
 import normality
 import numpy as np
 import pandas as pd
 from pantomime import normalize_mimetype
 
-PathLike: TypeAlias = str | os.PathLike[str] | Path
+from .types import PathLike
 
 
 def safe_eval(value):
     return eval(
         str(value),
         {
             "__builtins__": {
```

### Comparing `runpandarun-0.2.5/PKG-INFO` & `runpandarun-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpandarun
-Version: 0.2.5
+Version: 0.3.0
 Summary: Tell pandas what to do – easy tabular data I/O playbooks
 Home-page: https://investigraph.dev
 License: MIT
 Author: Simon Wörpel
 Author-email: simon@investigativedata.org
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5)
 Requires-Dist: banal (>=1.0.6,<2.0.0)
+Requires-Dist: datapatch (>=1.0.2,<2.0.0)
 Requires-Dist: fingerprints (>=1.1.0,<2.0.0)
 Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
 Requires-Dist: normality (>=2.4.0,<3.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: orjson (>=3.9.2,<4.0.0)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: pantomime (>=0.6.1,<0.7.0)
@@ -41,14 +42,16 @@
 
 # Run Panda Run
 
 :panda_face: :panda_face: :panda_face: :panda_face: :panda_face: :panda_face: :panda_face:
 
 A simple interface written in python for reproducible i/o workflows around tabular data via [pandas](https://pandas.pydata.org/) `DataFrame` specified via `yaml` "playbooks".
 
+Apart from any `pandas` function possible that can alter data, also [datapatch](https://github.com/pudo/datapatch) is included for an additional and easier way to patch data.
+
 **NOTICE**
 
 As of july 2023, this package only handles pandas transform logic, no data warehousing anymore.  See [archived version](https://github.com/simonwoerpel/runpandarun/tree/master)
 
 ## Quickstart
 
 [Install via pip](#installation)
@@ -236,14 +239,20 @@
 
   - handler: DataFrame.sort_values
     options:
       by:
         - state
         - city
 
+patch:
+  city:
+    options:
+      - match: Zarizri
+        value: Zar1zr1
+
 write:
   uri: ftp://user:${FTP_PASSWORD}@host/data.csv
   options:
     index: false
 ```
 
 ## How to...
@@ -331,17 +340,45 @@
 ```yaml
 read:
   uri: postgresql://user:password@host/database
   options:
     sql: "SELECT * FROM my_table WHERE category = 'A'"
 ```
 
+### Patch data
+
+Apart from any `pandas` function possible that can alter data, also [datapatch](https://github.com/pudo/datapatch) is included for an additional and easier way to patch data.
+
+Simply add a `patch` config to the yaml. Refer to the datapatch readme for details.
+
+The patching is applied *after* all the `operations` are applied.
+
+```yaml
+patch:
+  countries:
+    normalize: true
+    lowercase: true
+    options:
+      - match: Frankreich
+        value: France
+      - match:
+          - Northkorea
+          - Nordkorea
+          - Northern Korea
+          - NKorea
+          - DPRK
+        value: North Korea
+      - contains: Britain
+        value: Great Britain
+```
+
+
 ## save eval
 
-Ok wait, you are executing arbitrary python code in the yaml specs?
+**Ok wait, you are executing arbitrary python code in the yaml specs?**
 
 Not really, there is a strict allow list of possible modules that can be used. See [runpandarun.util.safe_eval](https://github.com/investigativedata/runpandarun/blob/develop/runpandarun/util.py)
 
 This includes:
 - any pandas or numpy modules
 - [normality](https://github.com/pudo/normality/)
 - [fingerprints](https://github.com/alephdata/fingerprints)
```

