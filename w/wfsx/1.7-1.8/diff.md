# Comparing `tmp/wfsx-1.7-py3-none-any.whl.zip` & `tmp/wfsx-1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 32679 bytes, number of entries: 20
+Zip file size: 32794 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      413 b- defN 23-Jun-06 11:13 wfsx/CONST_j.py
 -rw-rw-rw-  2.0 fat     5163 b- defN 23-Jul-28 14:45 wfsx/Excel_x.py
 -rw-rw-rw-  2.0 fat     5280 b- defN 23-Jul-28 14:45 wfsx/Report.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 11:13 wfsx/__init__.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-Jul-28 14:31 wfsx/api.py
 -rw-rw-rw-  2.0 fat     6019 b- defN 23-Jun-15 14:25 wfsx/apivalid.py
 -rw-rw-rw-  2.0 fat    16574 b- defN 23-Jul-28 14:41 wfsx/apivalidation.py
 -rw-rw-rw-  2.0 fat    20715 b- defN 23-Aug-01 15:36 wfsx/common.py
--rw-rw-rw-  2.0 fat    12481 b- defN 23-Aug-01 15:32 wfsx/dataextract.py
+-rw-rw-rw-  2.0 fat    11542 b- defN 23-Aug-01 16:30 wfsx/dataextract.py
 -rw-rw-rw-  2.0 fat     2808 b- defN 23-Jun-06 11:13 wfsx/excel_json_reader.py
--rw-rw-rw-  2.0 fat     4189 b- defN 23-Jun-16 15:41 wfsx/ghelper.py
+-rw-rw-rw-  2.0 fat     6093 b- defN 23-Aug-01 16:30 wfsx/ghelper.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 23-Jun-06 11:13 wfsx/parseexcel.py
 -rw-rw-rw-  2.0 fat     7022 b- defN 23-Jun-13 11:44 wfsx/plite.py
 -rw-rw-rw-  2.0 fat    23242 b- defN 23-Jul-28 14:45 wfsx/results_validate.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 23-Jul-27 11:01 wfsx/inix/endpointapi.ini
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1260 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1477 b- defN 23-Aug-01 15:36 wfsx-1.7.dist-info/RECORD
-20 files, 134144 bytes uncompressed, 30347 bytes compressed:  77.4%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1477 b- defN 23-Aug-01 16:31 wfsx-1.8.dist-info/RECORD
+20 files, 135109 bytes uncompressed, 30462 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: wfsx/results_validate.py
 Comment: 
 
 Filename: wfsx/inix/endpointapi.ini
 Comment: 
 
-Filename: wfsx-1.7.dist-info/LICENSE
+Filename: wfsx-1.8.dist-info/LICENSE
 Comment: 
 
-Filename: wfsx-1.7.dist-info/METADATA
+Filename: wfsx-1.8.dist-info/METADATA
 Comment: 
 
-Filename: wfsx-1.7.dist-info/WHEEL
+Filename: wfsx-1.8.dist-info/WHEEL
 Comment: 
 
-Filename: wfsx-1.7.dist-info/top_level.txt
+Filename: wfsx-1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: wfsx-1.7.dist-info/RECORD
+Filename: wfsx-1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wfsx/dataextract.py

```diff
@@ -1,13 +1,14 @@
 import time
 import configparser
 from datetime import timedelta, date, datetime
 from wfsx.apivalidation import *
 from wfsx.plite import *
 from wfsx.common import *
+from wfsx.ghelper import get_nested_multiple_values
 import random, json
 import re
 
 mypath = Path.cwd()  # .parent
 config = configparser.ConfigParser()
 config.read(mypath / "config.ini")
 config.read(mypath / 'utils' / 'endpointapi.ini')
@@ -78,42 +79,14 @@
             # Create Splited Tables with Index
             # dbname = str(vroles).split('.')[0]
             # getCreateTables(jsonDatax=gettet, dbname=dbname, reqres='request')
             # time.sleep(1)
             # Create Splited Tables without Index
             # requdata(jsdata=gettet, dbname=dbname)
 
-
-def get_nested_multiple_values(data, keys="attributeRequests.attributeId"):
-    if isinstance(keys, str):
-        keys = keys.split(",")
-    if len(keys) == 0:
-        return None
-    values = [[] for _ in range(len(keys))]  # Create a list to store values for each key
-    for i, key in enumerate(keys):
-        nested_keys = key.split(".")
-        temp_data = data
-        for nested_key in nested_keys:
-            if isinstance(temp_data, list):
-                temp_values = []
-                for item in temp_data:
-                    if nested_key in item:
-                        temp_values.append(item[nested_key])
-                    else:
-                        temp_values.append(None)
-                temp_data = temp_values
-            elif nested_key in temp_data:
-                temp_data = temp_data[nested_key]
-            else:
-                temp_data = None
-                break
-        values[i] = temp_data
-    return tuple(values)
-
-
 def extractedValue(tdata, apipoint, ePoint=None, eValue=None, dictdata=None, gnx=0):
     global random_value, value
     getx, gnx, gxa = None, 0, None
     if ePoint is None and dictdata is None:
         if tdata != 'None' and tdata != '':
             eHome, ePoint, apxpoint, eValue = str(tdata).split('|')
             # print(eHome, ePoint, apxpoint, eValue)
```

## wfsx/ghelper.py

```diff
@@ -111,7 +111,63 @@
             if value is not None:
                 if isinstance(value, list):
                     values.extend(value)
                 else:
                     values.append(value)
         return values
     return None
+
+# value = get_nested_multiple_values(dictionary, keys)
+# Response : Add data infront / Request no need
+def get_nested_multiple_values(data, keys="data.Profiles.codex"):
+    if isinstance(keys, str):
+        keys = keys.split(",")
+    if len(keys) == 0:
+        return None
+
+    def recursive_extract(d, nested_keys):
+        if len(nested_keys) == 0:
+            return [d]
+
+        key = nested_keys[0]
+        rest_keys = nested_keys[1:]
+
+        if isinstance(d, list):
+            results = []
+            for item in d:
+                if key in item:
+                    results.extend(recursive_extract(item[key], rest_keys))
+            return results
+        elif isinstance(d, dict) and key in d:
+            return recursive_extract(d[key], rest_keys)
+        else:
+            return []
+
+    values = [recursive_extract(data, key.split(".")) for key in keys]
+    return tuple(values)
+
+
+def get_values_level(data, keys="attributeRequests.attributeId"):
+    if isinstance(keys, str):
+        keys = keys.split(",")
+    if len(keys) == 0:
+        return None
+    values = [[] for _ in range(len(keys))]  # Create a list to store values for each key
+    for i, key in enumerate(keys):
+        nested_keys = key.split(".")
+        temp_data = data
+        for nested_key in nested_keys:
+            if isinstance(temp_data, list):
+                temp_values = []
+                for item in temp_data:
+                    if nested_key in item:
+                        temp_values.append(item[nested_key])
+                    else:
+                        temp_values.append(None)
+                temp_data = temp_values
+            elif nested_key in temp_data:
+                temp_data = temp_data[nested_key]
+            else:
+                temp_data = None
+                break
+        values[i] = temp_data
+    return tuple(values)
```

## Comparing `wfsx-1.7.dist-info/LICENSE` & `wfsx-1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfsx-1.7.dist-info/METADATA` & `wfsx-1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfsx
-Version: 1.7
+Version: 1.8
 Summary: api automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfsx/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `wfsx-1.7.dist-info/RECORD` & `wfsx-1.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 wfsx/Excel_x.py,sha256=-RhqrKWTi2ias2f8sMpembEYSectGn6zvhlDEaGIkIc,5163
 wfsx/Report.py,sha256=kbydYbBv0YmoOdgCQ2y92nuBNUZmYcwq4gbajGUbKMc,5280
 wfsx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfsx/api.py,sha256=4RvVwxzel6i3jpIWOw8pzM_LOCc9P9lqk8QKrvOJGXM,6310
 wfsx/apivalid.py,sha256=OZz8aFjH9BSmrvJNY7XwV1yjUYHpd7Fa6pyO-X0z0G8,6019
 wfsx/apivalidation.py,sha256=Hl6G6bv66BVnlN6iZjxATfe19LyB7yfvSHQQZ_Ue0Sg,16574
 wfsx/common.py,sha256=g4wdM0P_O3Uw4WV5jLzD4-koqIgIrWPD4CsHzXNwLoY,20715
-wfsx/dataextract.py,sha256=L_F7JAB5Z-TzpFWLlPHx8VJF_4Jr6FPbKBPTxBCy_3Y,12481
+wfsx/dataextract.py,sha256=4Sn0xmVS8nHyqbSz0X-JJeFSgR4tJb1sLRAnLw9WH5A,11542
 wfsx/excel_json_reader.py,sha256=z4vQkNRLKCO7x3UAeI8EVd9vjY5GDTEYDOVTj2jqICA,2808
-wfsx/ghelper.py,sha256=oYgGDv8YZOKAX6vg4gel0kjpaAwZ40137AQhAFDFnW8,4189
+wfsx/ghelper.py,sha256=TCUuHHBjKbuXZFOWy73Ue11JU2k8WnebFRM_E4bD2r8,6093
 wfsx/parseexcel.py,sha256=uXXUcI9AiDHqdaKd8oGAxu_3OXFmuw66CLRXvJRXHtc,5407
 wfsx/plite.py,sha256=d2yNK_XkO17OFQbr4Ecf_OSkDgys9vzdefnm03Lm3Ck,7022
 wfsx/results_validate.py,sha256=Jzx6xUHcbrTQuKhc9q48vKR7BXmSrEbD8T7SB45c_NM,23242
 wfsx/inix/endpointapi.ini,sha256=0NfMZyTdLlBseaPlWWtzLFShX2qGODskfJ7PVUVnK34,4322
-wfsx-1.7.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfsx-1.7.dist-info/METADATA,sha256=c4F0LkrtEUnrDvF8r40Ehk2LI0IxM60DuMgtUOzIPGk,1260
-wfsx-1.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfsx-1.7.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
-wfsx-1.7.dist-info/RECORD,,
+wfsx-1.8.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfsx-1.8.dist-info/METADATA,sha256=kRllBKLo55sglIyLaArN5BFExhLwLsinmCTUmPo06Kw,1260
+wfsx-1.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfsx-1.8.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
+wfsx-1.8.dist-info/RECORD,,
```

