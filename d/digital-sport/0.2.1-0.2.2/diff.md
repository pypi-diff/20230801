# Comparing `tmp/digital_sport-0.2.1-py3-none-any.whl.zip` & `tmp/digital_sport-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10055 bytes, number of entries: 11
--rw-rw-r--  2.0 unx      112 b- defN 23-Aug-01 11:59 sport/__init__.py
--rw-rw-r--  2.0 unx      678 b- defN 22-Apr-30 18:33 sport/abstract.py
--rw-rw-r--  2.0 unx     9345 b- defN 23-Aug-01 10:41 sport/api.py
--rw-rw-r--  2.0 unx     7298 b- defN 23-Aug-01 11:59 sport/interface.py
--rw-rw-r--  2.0 unx      982 b- defN 23-Aug-01 10:41 sport/report_service.py
--rw-rw-r--  2.0 unx     4267 b- defN 23-Aug-01 10:41 sport/search_center.py
--rw-rw-r--  2.0 unx     1172 b- defN 22-Apr-30 18:33 sport/tool.py
--rw-rw-r--  2.0 unx     2163 b- defN 23-Aug-01 11:59 digital_sport-0.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 11:59 digital_sport-0.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Aug-01 11:59 digital_sport-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      839 b- defN 23-Aug-01 11:59 digital_sport-0.2.1.dist-info/RECORD
-11 files, 26954 bytes uncompressed, 8649 bytes compressed:  67.9%
+Zip file size: 10054 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx      100 b- defN 23-Aug-01 12:04 sport/__init__.py
+-rw-rw-r--  2.0 unx      678 b- defN 23-Aug-01 12:00 sport/abstract.py
+-rw-rw-r--  2.0 unx     9345 b- defN 23-Aug-01 12:00 sport/api.py
+-rw-rw-r--  2.0 unx     7298 b- defN 23-Aug-01 12:00 sport/interface.py
+-rw-rw-r--  2.0 unx      982 b- defN 23-Aug-01 12:00 sport/report_service.py
+-rw-rw-r--  2.0 unx     4267 b- defN 23-Aug-01 12:00 sport/search_center.py
+-rw-rw-r--  2.0 unx     1172 b- defN 23-Aug-01 12:00 sport/tool.py
+-rw-rw-r--  2.0 unx     2163 b- defN 23-Aug-01 12:06 digital_sport-0.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 12:06 digital_sport-0.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Aug-01 12:06 digital_sport-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      839 b- defN 23-Aug-01 12:06 digital_sport-0.2.2.dist-info/RECORD
+11 files, 26942 bytes uncompressed, 8648 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: sport/search_center.py
 Comment: 
 
 Filename: sport/tool.py
 Comment: 
 
-Filename: digital_sport-0.2.1.dist-info/METADATA
+Filename: digital_sport-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: digital_sport-0.2.1.dist-info/WHEEL
+Filename: digital_sport-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: digital_sport-0.2.1.dist-info/top_level.txt
+Filename: digital_sport-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: digital_sport-0.2.1.dist-info/RECORD
+Filename: digital_sport-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sport/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .api import FootballSport as Football
+from .api import FootballSport
 from .interface import IFootballMatch, IStatistics, Ih2h, IMarketData
```

## Comparing `digital_sport-0.2.1.dist-info/METADATA` & `digital_sport-0.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-sport
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sport Api - structured data.
 Home-page: https://github.com/repen/digital-sport
 Author: Andrey Plugin
 Author-email: 9keepa@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

## Comparing `digital_sport-0.2.1.dist-info/RECORD` & `digital_sport-0.2.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-sport/__init__.py,sha256=6M5-m21g225jWrt423ekYL2TGRug8HB5Jjjv3D2Pr2g,112
+sport/__init__.py,sha256=mc2cGQaj2e9YszLQjusEgTTr0uRGfZ4lujzps2dAdO4,100
 sport/abstract.py,sha256=ftcV_6vemANYLbyhXuDyD4rW8Yr5ijbLA2g9W1M1BD0,678
 sport/api.py,sha256=uGh1TOo9_PWtoauIyjZbhF5Dmv60fbb5Xj_8MU8un3s,9345
 sport/interface.py,sha256=jUW5DFEN4NkZ4DaS94vK-_4gVienFpjzz9nQLBqnbdw,7298
 sport/report_service.py,sha256=rnMarqmPBVnipHMGzfxlraZyBOen3n5hS-TkiiCy2r0,982
 sport/search_center.py,sha256=aRrOct_6YXjF7AGBBTJ0qcvm-DZkH-NOW8NaPXkkkdE,4267
 sport/tool.py,sha256=7GlmTYUQo-oBVJsApGjiyIUmHlKHE_g3L92gUP-X8JM,1172
-digital_sport-0.2.1.dist-info/METADATA,sha256=vV8uCB1FWGWndePLze0pB4xrUpKj6dAkKvZw-MSrE04,2163
-digital_sport-0.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-digital_sport-0.2.1.dist-info/top_level.txt,sha256=0xTzN6mhGlQHtRaLSIr3s9xbt3IsYcpGkhw6I2he6_s,6
-digital_sport-0.2.1.dist-info/RECORD,,
+digital_sport-0.2.2.dist-info/METADATA,sha256=apeURji-lTheJuGUf1LHKIAsOwaslbXLxf9Ln7adXZg,2163
+digital_sport-0.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+digital_sport-0.2.2.dist-info/top_level.txt,sha256=0xTzN6mhGlQHtRaLSIr3s9xbt3IsYcpGkhw6I2he6_s,6
+digital_sport-0.2.2.dist-info/RECORD,,
```

