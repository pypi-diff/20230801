# Comparing `tmp/Geode_Background-7.3.2rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Background-7.3.2rc2-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 4722697 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      216 b- defN 23-Jul-31 08:11 geode_background/__init__.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-Jul-31 08:11 geode_background/brep.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-Jul-31 08:11 geode_background/solid.py
--rw-rw-rw-  2.0 fat      203 b- defN 23-Jul-31 08:11 geode_background/surface.py
--rw-rw-rw-  2.0 fat  3750912 b- defN 23-Jul-31 08:12 geode_background/bin/Geode-Background_brep.dll
--rw-rw-rw-  2.0 fat    54272 b- defN 23-Jul-31 08:12 geode_background/bin/Geode-Background_common.dll
--rw-rw-rw-  2.0 fat  3992576 b- defN 23-Jul-31 08:12 geode_background/bin/Geode-Background_solid.dll
--rw-rw-rw-  2.0 fat  3776000 b- defN 23-Jul-31 08:12 geode_background/bin/Geode-Background_surface.dll
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Jul-31 08:12 geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Jul-31 08:12 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Jul-31 08:12 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Jul-31 08:12 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1105 b- defN 23-Jul-31 08:12 Geode_Background-7.3.2rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-31 08:12 Geode_Background-7.3.2rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-31 08:12 Geode_Background-7.3.2rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1601 b- defN 23-Jul-31 08:12 Geode_Background-7.3.2rc1.dist-info/RECORD
-16 files, 12079160 bytes uncompressed, 4719995 bytes compressed:  60.9%
+Zip file size: 3251648 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      110 b- defN 23-Aug-01 12:57 geode_background/__init__.py
+-rw-r--r--  2.0 unx      191 b- defN 23-Aug-01 12:57 geode_background/brep.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Aug-01 12:57 geode_background/solid.py
+-rw-r--r--  2.0 unx      196 b- defN 23-Aug-01 12:57 geode_background/surface.py
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-Aug-01 12:58 geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-Aug-01 12:58 geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-Aug-01 12:58 geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-Aug-01 12:58 geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   155296 b- defN 23-Aug-01 12:58 geode_background/lib64/libGeode-Background_brep.so
+-rwxr-xr-x  2.0 unx   125528 b- defN 23-Aug-01 12:58 geode_background/lib64/libGeode-Background_common.so
+-rwxr-xr-x  2.0 unx  3515728 b- defN 23-Aug-01 12:58 geode_background/lib64/libGeode-Background_solid.so
+-rwxr-xr-x  2.0 unx  3218960 b- defN 23-Aug-01 12:58 geode_background/lib64/libGeode-Background_surface.so
+-rw-r--r--  2.0 unx     1061 b- defN 23-Aug-01 12:58 Geode_Background-7.3.2rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Aug-01 12:58 Geode_Background-7.3.2rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-01 12:58 Geode_Background-7.3.2rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1673 b- defN 23-Aug-01 12:58 Geode_Background-7.3.2rc2.dist-info/RECORD
+16 files, 7507983 bytes uncompressed, 3248802 bytes compressed:  56.7%
```

## zipnote {}

```diff
@@ -6,44 +6,44 @@
 
 Filename: geode_background/solid.py
 Comment: 
 
 Filename: geode_background/surface.py
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_brep.dll
+Filename: geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_common.dll
+Filename: geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_solid.dll
+Filename: geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/Geode-Background_surface.dll
+Filename: geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_brep.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_common.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_solid.so
 Comment: 
 
-Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+Filename: geode_background/lib64/libGeode-Background_surface.so
 Comment: 
 
-Filename: Geode_Background-7.3.2rc1.dist-info/METADATA
+Filename: Geode_Background-7.3.2rc2.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Background-7.3.2rc1.dist-info/WHEEL
+Filename: Geode_Background-7.3.2rc2.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Background-7.3.2rc1.dist-info/top_level.txt
+Filename: Geode_Background-7.3.2rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Background-7.3.2rc1.dist-info/RECORD
+Filename: Geode_Background-7.3.2rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_background/__init__.py

```diff
@@ -1,8 +1,5 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .surface import *
-from .solid import *
-from .brep import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .surface import *
+from .solid import *
+from .brep import *
```

## geode_background/brep.py

```diff
@@ -1,10 +1,10 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_brep import *
-
-BackgroundBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_brep import *
+
+BackgroundBRepLibrary.initialize()
```

## geode_background/solid.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_solid import *
-BackgroundSolidLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_solid import *
+BackgroundSolidLibrary.initialize()
```

## geode_background/surface.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_background_py_surface import *
-BackgroundSurfaceLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_background_py_surface import *
+BackgroundSurfaceLibrary.initialize()
```

