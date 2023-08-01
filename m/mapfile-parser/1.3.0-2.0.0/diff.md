# Comparing `tmp/mapfile_parser-1.3.0.tar.gz` & `tmp/mapfile_parser-2.0.0.tar.gz`

## Comparing `mapfile_parser-1.3.0.tar` & `mapfile_parser-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/.gitattributes
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/mypy.ini
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/requirements.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/.github/workflows/mypy.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/.github/workflows/upload_pypi.yml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/__main__.py
--rw-r--r--   0        0        0    17547 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/mapfile.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/progress_stats.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/utils.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/__init__.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/first_diff.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/jsonify.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/pj64_syms.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/progress.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/sym_info.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/symbol_sizes_csv.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/src/mapfile_parser/frontends/upload_frogress.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/LICENSE
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 mapfile_parser-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/.gitattributes
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/mypy.ini
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/requirements.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/.github/workflows/upload_pypi.yml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/__main__.py
+-rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/mapfile.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/progress_stats.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/utils.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/__init__.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/first_diff.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/jsonify.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/pj64_syms.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/progress.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/sym_info.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/symbol_sizes_csv.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/src/mapfile_parser/frontends/upload_frogress.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/README.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 mapfile_parser-2.0.0/PKG-INFO
```

### Comparing `mapfile_parser-1.3.0/.github/workflows/mypy.yml` & `mapfile_parser-2.0.0/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/.github/workflows/upload_pypi.yml` & `mapfile_parser-2.0.0/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/__init__.py` & `mapfile_parser-2.0.0/src/mapfile_parser/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python3
 
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-__version_info__ = (1, 3, 0)
+__version_info__ = (2, 0, 0)
 __version__ = ".".join(map(str, __version_info__))
 __author__ = "Decompollaborate"
 
 from . import utils as utils
 
 from .mapfile import MapFile as MapFile
 from .mapfile import Symbol as Symbol
 from .mapfile import File as File
+from .mapfile import Segment as Segment
 from .mapfile import FoundSymbolInfo as FoundSymbolInfo
 
 from .progress_stats import ProgressStats as ProgressStats
 
 from . import frontends as frontends
```

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/__main__.py` & `mapfile_parser-2.0.0/src/mapfile_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/progress_stats.py` & `mapfile_parser-2.0.0/src/mapfile_parser/progress_stats.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/utils.py` & `mapfile_parser-2.0.0/src/mapfile_parser/utils.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/frontends/first_diff.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/first_diff.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/frontends/jsonify.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/jsonify.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/frontends/pj64_syms.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/pj64_syms.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from typing import TextIO
 import sys
 
 from .. import mapfile
 
 
 def writePj64SymsToFile(mapFile: mapfile.MapFile, outFile: TextIO):
-    for file in mapFile:
-        for sym in file:
-            symType = "code" if file.segmentType == ".text" else "data"
-            outFile.write(f"{sym.vram:08X},{symType},{sym.name}\n")
+    for segment in mapFile:
+        for file in segment:
+            for sym in file:
+                symType = "code" if file.sectionType == ".text" else "data"
+                outFile.write(f"{sym.vram:08X},{symType},{sym.name}\n")
 
 def doPj64Syms(mapPath: Path, outputPath: Path|None) -> int:
     mapFile = mapfile.MapFile()
     mapFile.readMapFile(mapPath)
 
     if outputPath is None:
         writePj64SymsToFile(mapFile, sys.stdout)
```

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/frontends/progress.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def getProgress(mapPath: Path, asmPath: Path, nonmatchingsPath: Path, pathIndex: int=2, debugging: bool=False) -> tuple[progress_stats.ProgressStats, dict[str, progress_stats.ProgressStats]]:
     mapFile = mapfile.MapFile()
 
     mapFile.debugging = debugging
     mapFile.readMapFile(mapPath)
 
-    return mapFile.filterBySegmentType(".text").getProgress(asmPath, nonmatchingsPath, pathIndex=pathIndex)
+    return mapFile.filterBySectionType(".text").getProgress(asmPath, nonmatchingsPath, pathIndex=pathIndex)
 
 def doProgress(mapPath: Path, asmPath: Path, nonmatchingsPath: Path, pathIndex: int=2, debugging: bool=False) -> int:
     totalStats, progressPerFolder = getProgress(mapPath, asmPath, nonmatchingsPath, pathIndex=pathIndex, debugging=debugging)
 
     progress_stats.printStats(totalStats, progressPerFolder)
     return 0
```

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/frontends/sym_info.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/sym_info.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/frontends/symbol_sizes_csv.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/symbol_sizes_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .. import mapfile
 
 
 def processArguments(args: argparse.Namespace):
     mapFile = mapfile.MapFile()
     mapFile.readMapFile(args.mapfile)
     if args.filter_section is not None:
-        mapFile = mapFile.filterBySegmentType(args.filter_section)
+        mapFile = mapFile.filterBySectionType(args.filter_section)
 
     if args.same_folder:
         mapFile = mapFile.mixFolders()
 
     if args.symbols:
         mapFile.printSymbolsCsv()
     else:
```

### Comparing `mapfile_parser-1.3.0/src/mapfile_parser/frontends/upload_frogress.py` & `mapfile_parser-2.0.0/src/mapfile_parser/frontends/upload_frogress.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/.gitignore` & `mapfile_parser-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/LICENSE` & `mapfile_parser-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.3.0/README.md` & `mapfile_parser-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 pip install mapfile-parser
 ```
 
 In case you want to mess with the latest development version without wanting to clone the repository, then you could use the following command:
 
 ```bash
 pip uninstall mapfile-parser
-pip install git+https://github.com/Decompollaborate/mapfile_parser.git@1.x
+pip install git+https://github.com/Decompollaborate/mapfile_parser.git@develop
 ```
 
 NOTE: Installing the development version is not recommended. Proceed at your own risk.
 
 ## Examples
 
 Various cli examples are provided in the [frontends folder](src/mapfile_parser/frontends). Most of them are re-implementations of already existing tools using this library to show how to use this library and inspire new ideas.
```

### Comparing `mapfile_parser-1.3.0/pyproject.toml` & `mapfile_parser-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "mapfile_parser"
-version = "1.3.0"
+version = "2.0.0"
 description = "Map file parser library focusing decompilation projects"
 readme = "README.md"
 requires-python = ">=3.7"
 dynamic = ["dependencies"]
 
 [project.urls]
 "Homepage" = "https://github.com/Decompollaborate/mapfile_parser"
```

### Comparing `mapfile_parser-1.3.0/PKG-INFO` & `mapfile_parser-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapfile_parser
-Version: 1.3.0
+Version: 2.0.0
 Summary: Map file parser library focusing decompilation projects
 Project-URL: Homepage, https://github.com/Decompollaborate/mapfile_parser
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/mapfile_parser/issues
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: requests
 Description-Content-Type: text/markdown
@@ -27,15 +27,15 @@
 pip install mapfile-parser
 ```
 
 In case you want to mess with the latest development version without wanting to clone the repository, then you could use the following command:
 
 ```bash
 pip uninstall mapfile-parser
-pip install git+https://github.com/Decompollaborate/mapfile_parser.git@1.x
+pip install git+https://github.com/Decompollaborate/mapfile_parser.git@develop
 ```
 
 NOTE: Installing the development version is not recommended. Proceed at your own risk.
 
 ## Examples
 
 Various cli examples are provided in the [frontends folder](src/mapfile_parser/frontends). Most of them are re-implementations of already existing tools using this library to show how to use this library and inspire new ideas.
```

