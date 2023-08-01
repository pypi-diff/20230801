# Comparing `tmp/pycobol2csv-0.1.4-py3-none-any.whl.zip` & `tmp/pycobol2csv-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8017 bytes, number of entries: 7
+Zip file size: 8071 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       52 b- defN 21-Sep-15 00:40 pycobol2csv/__init__.py
--rw-rw-rw-  2.0 fat    18955 b- defN 23-Aug-01 04:43 pycobol2csv/convert.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2190 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      564 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/RECORD
-7 files, 22951 bytes uncompressed, 7015 bytes compressed:  69.4%
+-rw-rw-rw-  2.0 fat    19023 b- defN 23-Aug-01 05:33 pycobol2csv/convert.py
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      564 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/RECORD
+7 files, 23097 bytes uncompressed, 7069 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pycobol2csv/__init__.py
 Comment: 
 
 Filename: pycobol2csv/convert.py
 Comment: 
 
-Filename: pycobol2csv-0.1.4.dist-info/LICENSE
+Filename: pycobol2csv-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: pycobol2csv-0.1.4.dist-info/METADATA
+Filename: pycobol2csv-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pycobol2csv-0.1.4.dist-info/WHEEL
+Filename: pycobol2csv-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pycobol2csv-0.1.4.dist-info/top_level.txt
+Filename: pycobol2csv-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pycobol2csv-0.1.4.dist-info/RECORD
+Filename: pycobol2csv-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycobol2csv/convert.py

```diff
@@ -11,15 +11,16 @@
 
 
 class CobolPatterns:
     opt_pattern_format = "({})?"
     row_pattern_base = r"^(?P<level>\d{2})\s+(?P<name>\S+)"
     row_pattern_occurs = r"\s+OCCURS (?P<occurs>\d+) TIMES"
     row_pattern_indexed_by = r"\s+INDEXED BY\s(?P<indexed_by>\S+)"
-    row_pattern_redefines = r"\s+REDEFINES\s(?P<redefines>\S+)"
+    # row_pattern_redefines = r"\s+REDEFINES\s(?P<redefines>\S+)"
+    row_pattern_redefines = r"\s+REDEFINES\s+(?P<redefines>\S+)"
     # row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)"
     row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)\s*\S+"
     row_pattern_end = r"\.$"
     row_pattern = re.compile(
         row_pattern_base
         + opt_pattern_format.format(row_pattern_redefines)
         + opt_pattern_format.format(row_pattern_occurs)
```

## Comparing `pycobol2csv-0.1.4.dist-info/LICENSE` & `pycobol2csv-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycobol2csv-0.1.4.dist-info/METADATA` & `pycobol2csv-0.1.5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobol2csv
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library to convert COBOL ebcdic file to CSV format
 Home-page: https://github.com/jasonli-lijie/pycobol2csv
 Author: Jason Li
 Author-email: niomobileapp@gmail.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Project-URL: Bug Tracker, https://github.com/jasonli-lijie/pycobol2csv/issues
@@ -24,14 +24,16 @@
 
 # pycobol2csv
 pycobol2csv is a Python library to convert COBOL ebcdic file to CSV format. The package is built to cater for advanced features in COBOL copybooks such as *OCCURES x TIMES*. 
 
 The CSV file is RDBMS friendly and all headers are ready to be used as database column names.
 CSV conversion is controlled by config file in *csv_config.json*
 
+Added more fixes for the outdated REDEFINE and PIC syntax for a new client
+
 Install the python module:
 
 `pip install pycobol2csv`
 
 To use the module:
 
 ```
```

