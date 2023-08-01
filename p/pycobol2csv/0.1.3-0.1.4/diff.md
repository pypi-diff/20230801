# Comparing `tmp/pycobol2csv-0.1.3-py3-none-any.whl.zip` & `tmp/pycobol2csv-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7986 bytes, number of entries: 7
+Zip file size: 8017 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       52 b- defN 21-Sep-15 00:40 pycobol2csv/__init__.py
--rw-rw-rw-  2.0 fat    18899 b- defN 23-Jul-14 07:06 pycobol2csv/convert.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2167 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      564 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/RECORD
-7 files, 22872 bytes uncompressed, 6984 bytes compressed:  69.5%
+-rw-rw-rw-  2.0 fat    18955 b- defN 23-Aug-01 04:43 pycobol2csv/convert.py
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2190 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      564 b- defN 23-Aug-01 04:54 pycobol2csv-0.1.4.dist-info/RECORD
+7 files, 22951 bytes uncompressed, 7015 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pycobol2csv/__init__.py
 Comment: 
 
 Filename: pycobol2csv/convert.py
 Comment: 
 
-Filename: pycobol2csv-0.1.3.dist-info/LICENSE
+Filename: pycobol2csv-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: pycobol2csv-0.1.3.dist-info/METADATA
+Filename: pycobol2csv-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: pycobol2csv-0.1.3.dist-info/WHEEL
+Filename: pycobol2csv-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: pycobol2csv-0.1.3.dist-info/top_level.txt
+Filename: pycobol2csv-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pycobol2csv-0.1.3.dist-info/RECORD
+Filename: pycobol2csv-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycobol2csv/convert.py

```diff
@@ -12,15 +12,16 @@
 
 class CobolPatterns:
     opt_pattern_format = "({})?"
     row_pattern_base = r"^(?P<level>\d{2})\s+(?P<name>\S+)"
     row_pattern_occurs = r"\s+OCCURS (?P<occurs>\d+) TIMES"
     row_pattern_indexed_by = r"\s+INDEXED BY\s(?P<indexed_by>\S+)"
     row_pattern_redefines = r"\s+REDEFINES\s(?P<redefines>\S+)"
-    row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)"
+    # row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)"
+    row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)\s*\S+"
     row_pattern_end = r"\.$"
     row_pattern = re.compile(
         row_pattern_base
         + opt_pattern_format.format(row_pattern_redefines)
         + opt_pattern_format.format(row_pattern_occurs)
         + opt_pattern_format.format(row_pattern_indexed_by)
         + opt_pattern_format.format(row_pattern_pic)
```

## Comparing `pycobol2csv-0.1.3.dist-info/LICENSE` & `pycobol2csv-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycobol2csv-0.1.3.dist-info/METADATA` & `pycobol2csv-0.1.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pycobol2csv
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library to convert COBOL ebcdic file to CSV format
 Home-page: https://github.com/jasonli-lijie/pycobol2csv
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Jason Li
 Author-email: niomobileapp@gmail.com
 License: MIT
+Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Project-URL: Bug Tracker, https://github.com/jasonli-lijie/pycobol2csv/issues
 Keywords: COBOL,EBCDIC,CSV
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -55,7 +56,9 @@
 
 ```
 python convert_cobol_test_main.py --copybook [COPYBOOK_FILE] --data [DATA_FILE] --output [CSV_FILE]
 
 ```
 
 Repo: https://github.com/jasonli-lijie/pycobol2csv
+
+
```

## Comparing `pycobol2csv-0.1.3.dist-info/RECORD` & `pycobol2csv-0.1.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pycobol2csv/__init__.py,sha256=q_ngSSKPu6OI2yQM0kHOOIU1tJkrSHwilFYszju4ZAc,52
-pycobol2csv/convert.py,sha256=ngm3mU_6V4ZxglusjZvIKIbeRqncZMs07vseZXi0kvg,18899
-pycobol2csv-0.1.3.dist-info/LICENSE,sha256=gpfrbvkPCMPpkAd1Hj5QOiDUlc3YiekPESzqUOnrAXc,1086
-pycobol2csv-0.1.3.dist-info/METADATA,sha256=KsBZEV-CvNfsIJzemt6SsYlMjRysV1rILmI-2ulBemQ,2167
-pycobol2csv-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pycobol2csv-0.1.3.dist-info/top_level.txt,sha256=7vXJihqVTBYjcbl6skF7mXGZeB8VZfPBuFavaMCxtGk,12
-pycobol2csv-0.1.3.dist-info/RECORD,,
+pycobol2csv/convert.py,sha256=VBwY0hd7Gyyqf8mcDADEHTHK5dT5jqgb7EdFg1lgjSo,18955
+pycobol2csv-0.1.4.dist-info/LICENSE,sha256=gpfrbvkPCMPpkAd1Hj5QOiDUlc3YiekPESzqUOnrAXc,1086
+pycobol2csv-0.1.4.dist-info/METADATA,sha256=Oh3MokjWPaky-vT30amUuVWzMRj0-p0Ov2EiUMGz7_E,2190
+pycobol2csv-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pycobol2csv-0.1.4.dist-info/top_level.txt,sha256=7vXJihqVTBYjcbl6skF7mXGZeB8VZfPBuFavaMCxtGk,12
+pycobol2csv-0.1.4.dist-info/RECORD,,
```

