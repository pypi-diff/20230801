# Comparing `tmp/mtsql-1.4.202307251849-py3-none-any.whl.zip` & `tmp/mtsql-1.4.202308011012-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19220 bytes, number of entries: 11
--rw-r--r--  2.0 unx       44 b- defN 23-Jan-22 22:24 mt/sql/__init__.py
--rw-r--r--  2.0 unx     9994 b- defN 23-May-11 07:16 mt/sql/base.py
--rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 11:50 mt/sql/mysql.py
--rw-r--r--  2.0 unx    65224 b- defN 23-Jul-25 18:48 mt/sql/psql.py
--rw-r--r--  2.0 unx     8678 b- defN 23-Feb-23 10:22 mt/sql/sqlite.py
--rw-r--r--  2.0 unx      396 b- defN 23-Jul-25 18:49 mt/sql/version.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/LICENSE
--rw-r--r--  2.0 unx      597 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 23-Jul-25 18:49 mtsql-1.4.202307251849.dist-info/RECORD
-11 files, 91855 bytes uncompressed, 17766 bytes compressed:  80.7%
+Zip file size: 19218 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx       44 b- defN 23-Mar-28 14:19 mt/sql/__init__.py
+-rw-rw-r--  2.0 unx     9994 b- defN 23-May-07 05:12 mt/sql/base.py
+-rw-rw-r--  2.0 unx     4894 b- defN 23-Mar-28 14:19 mt/sql/mysql.py
+-rw-rw-r--  2.0 unx    65229 b- defN 23-Aug-01 10:12 mt/sql/psql.py
+-rw-rw-r--  2.0 unx     8678 b- defN 23-Mar-28 14:19 mt/sql/sqlite.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Aug-01 10:12 mt/sql/version.py
+-rw-rw-r--  2.0 unx     1070 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      597 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 23-Aug-01 10:13 mtsql-1.4.202308011012.dist-info/RECORD
+11 files, 91860 bytes uncompressed, 17764 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mt/sql/sqlite.py
 Comment: 
 
 Filename: mt/sql/version.py
 Comment: 
 
-Filename: mtsql-1.4.202307251849.dist-info/LICENSE
+Filename: mtsql-1.4.202308011012.dist-info/LICENSE
 Comment: 
 
-Filename: mtsql-1.4.202307251849.dist-info/METADATA
+Filename: mtsql-1.4.202308011012.dist-info/METADATA
 Comment: 
 
-Filename: mtsql-1.4.202307251849.dist-info/WHEEL
+Filename: mtsql-1.4.202308011012.dist-info/WHEEL
 Comment: 
 
-Filename: mtsql-1.4.202307251849.dist-info/top_level.txt
+Filename: mtsql-1.4.202308011012.dist-info/top_level.txt
 Comment: 
 
-Filename: mtsql-1.4.202307251849.dist-info/RECORD
+Filename: mtsql-1.4.202308011012.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/sql/psql.py

```diff
@@ -1,14 +1,14 @@
 """Useful modules for accessing PostgreSQL"""
 
 import sqlalchemy as sa
 import re
 import psycopg2 as ps
 import sqlalchemy.exc as se
-from tqdm import tqdm  # nice progress bar
+from tqdm.auto import tqdm  # nice progress bar
 
 from mt import tp, logg, pd, np, path, ctx
 from mt.base.bg_invoke import BgInvoke
 
 from .base import *
```

## mt/sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('07')
-VERSION_DAY = int('25')
-VERSION_HOUR = int('18')
-VERSION_MINUTE = int('49')
+VERSION_MONTH = int('08')
+VERSION_DAY = int('01')
+VERSION_HOUR = int('10')
+VERSION_MINUTE = int('12')
 MAJOR_VERSION = 1
 MINOR_VERSION = 4
-PATCH_VERSION = 202307251849
-version_date = '2023/07/25 18:49'
+PATCH_VERSION = 202308011012
+version_date = '2023/08/01 10:12'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtsql-1.4.202307251849.dist-info/LICENSE` & `mtsql-1.4.202308011012.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtsql-1.4.202307251849.dist-info/METADATA` & `mtsql-1.4.202308011012.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsql
-Version: 1.4.202307251849
+Version: 1.4.202308011012
 Summary: Extra Python modules to deal with the interaction between pandas dataframes and remote SQL servers, for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtsql
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.sql/mt.sql.html
 Project-URL: Source Code, https://github.com/inteplus/mtsql
 License-File: LICENSE
 Requires-Dist: sqlalchemy (>=2.0)
```

