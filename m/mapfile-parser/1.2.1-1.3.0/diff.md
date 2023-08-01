# Comparing `tmp/mapfile_parser-1.2.1.tar.gz` & `tmp/mapfile_parser-1.3.0.tar.gz`

## Comparing `mapfile_parser-1.2.1.tar` & `mapfile_parser-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/.gitattributes
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/mypy.ini
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/requirements.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/.github/workflows/mypy.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/.github/workflows/upload_pypi.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/__main__.py
--rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/mapfile.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/progress_stats.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/utils.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/__init__.py
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/first_diff.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/pj64_syms.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/progress.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/sym_info.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/symbol_sizes_csv.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/upload_frogress.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/LICENSE
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/.gitattributes
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/mypy.ini
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/requirements.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/.github/workflows/upload_pypi.yml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/__main__.py
+-rw-r--r--   0        0        0    17547 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/mapfile.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/progress_stats.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/utils.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/__init__.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/first_diff.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/jsonify.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/pj64_syms.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/progress.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/sym_info.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/symbol_sizes_csv.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/upload_frogress.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/README.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/PKG-INFO
```

### Comparing `mapfile_parser-1.2.1/.github/workflows/mypy.yml` & `mapfile_parser-1.3.0/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.1/.github/workflows/upload_pypi.yml` & `mapfile_parser-1.3.0/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/__main__.py` & `mapfile_parser-1.3.0/src/mapfile_parser/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 
 import mapfile_parser
@@ -12,14 +12,15 @@
 
 def mapfileParserMain():
     parser = argparse.ArgumentParser()
 
     subparsers = parser.add_subparsers(description="action", help="the action to perform", required=True)
 
     mapfile_parser.frontends.first_diff.addSubparser(subparsers)
+    mapfile_parser.frontends.jsonify.addSubparser(subparsers)
     mapfile_parser.frontends.pj64_syms.addSubparser(subparsers)
     mapfile_parser.frontends.progress.addSubparser(subparsers)
     mapfile_parser.frontends.sym_info.addSubparser(subparsers)
     mapfile_parser.frontends.symbol_sizes_csv.addSubparser(subparsers)
     mapfile_parser.frontends.upload_frogress.addSubparser(subparsers)
 
     args = parser.parse_args()
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/mapfile.py` & `mapfile_parser-1.3.0/src/mapfile_parser/mapfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import dataclasses
 import re
 from typing import Generator
@@ -32,46 +32,75 @@
     vram: int
     size: int = -1 # in bytes
     vrom: int|None = None
 
     def getVramStr(self) -> str:
         return f"0x{self.vram:08X}"
 
+    def getSizeStr(self) -> str:
+        if self.size < 0:
+            return "None"
+        return f"0x{self.size:X}"
+
     def getVromStr(self) -> str:
         if self.vrom is None:
             return "None"
         return f"0x{self.vrom:06X}"
 
-    def getSizeStr(self) -> str:
+    def serializeSize(self) -> str|None:
         if self.size < 0:
-            return "None"
+            return None
         return f"0x{self.size:X}"
 
 
     @staticmethod
     def printCsvHeader():
         print("Symbol name,VRAM,Size in bytes")
 
     def printAsCsv(self):
         print(f"{self.name},{self.vram:08X},{self.size}")
 
+
+    def toJson(self) -> dict:
+        result = {
+            "name": self.name,
+            "vram": self.getVramStr(),
+            "size": self.serializeSize(),
+            "vrom": self.getVromStr(),
+        }
+
+        return result
+
+
 @dataclasses.dataclass
 class File:
     filepath: Path
     vram: int
     size: int # in bytes
     segmentType: str
     symbols: list[Symbol] = dataclasses.field(default_factory=list)
     vrom: int|None = None
 
     @property
     def isNoloadSegment(self) -> bool:
         return self.segmentType == ".bss"
 
 
+    def serializeVram(self) -> str|None:
+        return f"0x{self.vram:08X}"
+
+    def serializeSize(self) -> str|None:
+        return f"0x{self.size:X}"
+
+    def serializeVrom(self) -> str|None:
+        if self.vrom is None:
+            return None
+        return f"0x{self.vrom:06X}"
+
+
     def getName(self) -> Path:
         return Path(*self.filepath.with_suffix("").parts[2:])
 
     def findSymbolByName(self, symName: str) -> Symbol|None:
         for sym in self.symbols:
             if sym.name == symName:
                 return sym
@@ -135,14 +164,31 @@
                 maxSize = symSize
 
         if printVram:
             print(f"{self.vram:08X},", end="")
         print(f"{self.filepath},{self.segmentType},{symCount},{maxSize},{self.size},{averageSize:0.2f}")
 
 
+    def toJson(self) -> dict:
+        fileDict = {
+            "filepath": str(self.filepath),
+            "segmentType": self.segmentType,
+            "vram": self.serializeVram(),
+            "size": self.serializeSize(),
+            "vrom": self.serializeVrom(),
+        }
+
+        symbolsList = []
+        for symbol in self.symbols:
+            symbolsList.append(symbol.toJson())
+
+        fileDict["symbols"] = symbolsList
+        return fileDict
+
+
     def __iter__(self) -> Generator[Symbol, None, None]:
         for sym in self.symbols:
             yield sym
 
     def __getitem__(self, index) -> Symbol:
         return self.symbols[index]
 
@@ -227,15 +273,15 @@
                     size = int(entryMatch["size"], 16)
                     vram = int(entryMatch["vram"], 16)
                     segmentType = entryMatch["section"]
 
                     if size > 0:
                         inFile = True
                         tempFile = File(filepath, vram, size, segmentType)
-                        if loadAddressData is not None and loadAddressData.vram == vram:
+                        if loadAddressData is not None and loadAddressData.vram == vram and not tempFile.isNoloadSegment:
                             tempFile.vrom = loadAddressData.vrom
                         tempFilesList.append(tempFile)
 
                 elif loadAddressMatch is not None:
                     vram = int(loadAddressMatch["vram"], 0)
                     size = int(loadAddressMatch["size"], 0)
                     vrom = int(loadAddressMatch["vrom"], 0)
@@ -454,13 +500,25 @@
 
             for sym in file.symbols:
                 print(f"{file.filepath},", end="")
                 sym.printAsCsv()
         return
 
 
+    def toJson(self) -> dict:
+        filesList = []
+
+        for file in self.filesList:
+            filesList.append(file.toJson())
+
+        result = {
+            "files": filesList
+        }
+        return result
+
+
     def __iter__(self) -> Generator[File, None, None]:
         for file in self.filesList:
             yield file
 
     def __getitem__(self, index) -> File:
         return self.filesList[index]
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/progress_stats.py` & `mapfile_parser-1.3.0/src/mapfile_parser/progress_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import dataclasses
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/utils.py` & `mapfile_parser-1.3.0/src/mapfile_parser/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from pathlib import Path
 import subprocess
 import sys
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/frontends/first_diff.py` & `mapfile_parser-1.3.0/src/mapfile_parser/frontends/first_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
 from typing import Callable
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/frontends/pj64_syms.py` & `mapfile_parser-1.3.0/src/mapfile_parser/frontends/pj64_syms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
 from typing import TextIO
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/frontends/progress.py` & `mapfile_parser-1.3.0/src/mapfile_parser/frontends/progress.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/frontends/sym_info.py` & `mapfile_parser-1.3.0/src/mapfile_parser/frontends/sym_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/frontends/symbol_sizes_csv.py` & `mapfile_parser-1.3.0/src/mapfile_parser/frontends/symbol_sizes_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
```

### Comparing `mapfile_parser-1.2.1/src/mapfile_parser/frontends/upload_frogress.py` & `mapfile_parser-1.3.0/src/mapfile_parser/frontends/upload_frogress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
 import requests # type: ignore
```

### Comparing `mapfile_parser-1.2.1/.gitignore` & `mapfile_parser-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.1/LICENSE` & `mapfile_parser-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.1/README.md` & `mapfile_parser-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 pip install mapfile-parser
 ```
 
 In case you want to mess with the latest development version without wanting to clone the repository, then you could use the following command:
 
 ```bash
 pip uninstall mapfile-parser
-pip install git+https://github.com/Decompollaborate/mapfile_parser.git@develop
+pip install git+https://github.com/Decompollaborate/mapfile_parser.git@1.x
 ```
 
 NOTE: Installing the development version is not recommended. Proceed at your own risk.
 
 ## Examples
 
 Various cli examples are provided in the [frontends folder](src/mapfile_parser/frontends). Most of them are re-implementations of already existing tools using this library to show how to use this library and inspire new ideas.
 
 The list can be checked in runtime with `python3 -m mapfile_parser --help`.
 
 Each one of them can be executed with `python3 -m mapfile_parser utilityname`, for example `python3 -m mapfile_parser pj64_syms`.
 
 - `first_diff`: Find the first difference(s) between the built ROM and the base ROM.
+- `jsonify`: Converts a mapfile into a json format.
 - `pj64_syms`: Produce a PJ64 compatible symbol map.
 - `progress`: Computes current progress of the matched functions. Relies on a [splat](https://github.com/ethteck/splat) folder structure and matched functions not longer having a file.
 - `sym_info`: Display various information about a symbol or address.
 - `symbol_sizes_csv`: Produces a csv summarizing the files sizes by parsing a map file.
 - `upload_frogress`: Uploads current progress (calculated by the `progress` utility) of the matched functions to [frogress](https://github.com/decompals/frogress).
 
 None of the provided cli utilities are meant to be used directly on a command line, because they need a large number of long parameters to them and every repo has their own quirks which would need them to be adapted. Those have been written mostly to facilitate people to write those utilities in a way which accomodates their own repo.
```

### Comparing `mapfile_parser-1.2.1/PKG-INFO` & `mapfile_parser-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapfile_parser
-Version: 1.2.1
+Version: 1.3.0
 Summary: Map file parser library focusing decompilation projects
 Project-URL: Homepage, https://github.com/Decompollaborate/mapfile_parser
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/mapfile_parser/issues
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: requests
 Description-Content-Type: text/markdown
@@ -27,28 +27,29 @@
 pip install mapfile-parser
 ```
 
 In case you want to mess with the latest development version without wanting to clone the repository, then you could use the following command:
 
 ```bash
 pip uninstall mapfile-parser
-pip install git+https://github.com/Decompollaborate/mapfile_parser.git@develop
+pip install git+https://github.com/Decompollaborate/mapfile_parser.git@1.x
 ```
 
 NOTE: Installing the development version is not recommended. Proceed at your own risk.
 
 ## Examples
 
 Various cli examples are provided in the [frontends folder](src/mapfile_parser/frontends). Most of them are re-implementations of already existing tools using this library to show how to use this library and inspire new ideas.
 
 The list can be checked in runtime with `python3 -m mapfile_parser --help`.
 
 Each one of them can be executed with `python3 -m mapfile_parser utilityname`, for example `python3 -m mapfile_parser pj64_syms`.
 
 - `first_diff`: Find the first difference(s) between the built ROM and the base ROM.
+- `jsonify`: Converts a mapfile into a json format.
 - `pj64_syms`: Produce a PJ64 compatible symbol map.
 - `progress`: Computes current progress of the matched functions. Relies on a [splat](https://github.com/ethteck/splat) folder structure and matched functions not longer having a file.
 - `sym_info`: Display various information about a symbol or address.
 - `symbol_sizes_csv`: Produces a csv summarizing the files sizes by parsing a map file.
 - `upload_frogress`: Uploads current progress (calculated by the `progress` utility) of the matched functions to [frogress](https://github.com/decompals/frogress).
 
 None of the provided cli utilities are meant to be used directly on a command line, because they need a large number of long parameters to them and every repo has their own quirks which would need them to be adapted. Those have been written mostly to facilitate people to write those utilities in a way which accomodates their own repo.
```

