# Comparing `tmp/pgvector-0.2.0-py2.py3-none-any.whl.zip` & `tmp/pgvector-0.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 7669 bytes, number of entries: 11
+Zip file size: 8400 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      272 b- defN 21-Jun-23 06:42 pgvector/asyncpg/__init__.py
--rw-r--r--  2.0 unx     2624 b- defN 23-Jul-23 16:11 pgvector/django/__init__.py
+-rw-r--r--  2.0 unx     2766 b- defN 23-Aug-01 04:00 pgvector/django/__init__.py
+-rw-r--r--  2.0 unx      356 b- defN 23-Aug-01 04:00 pgvector/django/forms.py
+-rw-r--r--  2.0 unx      272 b- defN 23-Aug-01 04:00 pgvector/django/widgets.py
 -rw-r--r--  2.0 unx     1743 b- defN 23-May-10 04:14 pgvector/psycopg/__init__.py
 -rw-r--r--  2.0 unx      881 b- defN 21-Jun-13 19:29 pgvector/psycopg2/__init__.py
 -rw-r--r--  2.0 unx     1033 b- defN 22-May-23 01:12 pgvector/sqlalchemy/__init__.py
 -rw-r--r--  2.0 unx     1305 b- defN 21-Jun-23 02:28 pgvector/utils/__init__.py
--rw-r--r--  2.0 unx     1083 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6666 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      904 b- defN 23-Jul-24 03:06 pgvector-0.2.0.dist-info/RECORD
-11 files, 16630 bytes uncompressed, 6137 bytes compressed:  63.1%
+-rw-r--r--  2.0 unx     1083 b- defN 23-Aug-01 04:20 pgvector-0.2.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6666 b- defN 23-Aug-01 04:20 pgvector-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Aug-01 04:20 pgvector-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-01 04:20 pgvector-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Aug-01 04:20 pgvector-0.2.1.dist-info/RECORD
+13 files, 17562 bytes uncompressed, 6616 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -1,34 +1,40 @@
 Filename: pgvector/asyncpg/__init__.py
 Comment: 
 
 Filename: pgvector/django/__init__.py
 Comment: 
 
+Filename: pgvector/django/forms.py
+Comment: 
+
+Filename: pgvector/django/widgets.py
+Comment: 
+
 Filename: pgvector/psycopg/__init__.py
 Comment: 
 
 Filename: pgvector/psycopg2/__init__.py
 Comment: 
 
 Filename: pgvector/sqlalchemy/__init__.py
 Comment: 
 
 Filename: pgvector/utils/__init__.py
 Comment: 
 
-Filename: pgvector-0.2.0.dist-info/LICENSE.txt
+Filename: pgvector-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pgvector-0.2.0.dist-info/METADATA
+Filename: pgvector-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: pgvector-0.2.0.dist-info/WHEEL
+Filename: pgvector-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: pgvector-0.2.0.dist-info/top_level.txt
+Filename: pgvector-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pgvector-0.2.0.dist-info/RECORD
+Filename: pgvector-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pgvector/django/__init__.py

```diff
@@ -1,10 +1,11 @@
 from django.contrib.postgres.operations import CreateExtension
 from django.contrib.postgres.indexes import PostgresIndex
 from django.db.models import Field, FloatField, Func, Value
+from .forms import VectorFormField
 from ..utils import from_db, to_db
 
 __all__ = ['VectorExtension', 'VectorField', 'IvfflatIndex', 'L2Distance', 'MaxInnerProduct', 'CosineDistance']
 
 
 class VectorExtension(CreateExtension):
     def __init__(self):
@@ -44,14 +45,17 @@
 
     def validate(self, value, model_instance):
         super().validate(value.tolist(), model_instance)
 
     def run_validators(self, value):
         super().run_validators(value.tolist())
 
+    def formfield(self, **kwargs):
+        return super().formfield(form_class=VectorFormField, **kwargs)
+
 
 class IvfflatIndex(PostgresIndex):
     suffix = 'ivfflat'
 
     def __init__(self, *expressions, lists=None, **kwargs):
         self.lists = lists
         super().__init__(*expressions, **kwargs)
```

## Comparing `pgvector-0.2.0.dist-info/LICENSE.txt` & `pgvector-0.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pgvector-0.2.0.dist-info/METADATA` & `pgvector-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgvector
-Version: 0.2.0
+Version: 0.2.1
 Summary: pgvector support for Python
 Home-page: https://github.com/pgvector/pgvector-python
 Author: Andrew Kane
 Author-email: andrew@ankane.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

## Comparing `pgvector-0.2.0.dist-info/RECORD` & `pgvector-0.2.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 pgvector/asyncpg/__init__.py,sha256=VffBZUNIwvinQdh0lIYoSWgSQq57nFkpj9VhPjp11QQ,272
-pgvector/django/__init__.py,sha256=Gm_rZr0WVv6HfZUzar9QndJqElKhQjzGycffRrRWvlo,2624
+pgvector/django/__init__.py,sha256=lt7aJ2RZsXKJCuOFE7Ztvx-NK5jxiwSstEkdagunNO4,2766
+pgvector/django/forms.py,sha256=rUz-4vNr_uFscClbZF0HMHcYKOubvyiJBgVY4zYawZ8,356
+pgvector/django/widgets.py,sha256=kVn9jPyIZotJGHgqn1POwHJWJ-48wdvDu0hPV4jATro,272
 pgvector/psycopg/__init__.py,sha256=BjyTM_VGtl3RB-Fh4gPBppr8LutuH7hR3l0C7MJYMyw,1743
 pgvector/psycopg2/__init__.py,sha256=w_uHyKJzHMI79IyKYwFv6CK_k1RI1X6sWiML55Wo4b4,881
 pgvector/sqlalchemy/__init__.py,sha256=LUEkR6UIxW_o6fmjRKQmasMm6ZkyylnkW7VDMWyi-EI,1033
 pgvector/utils/__init__.py,sha256=udvrI2Gl5cjO-eXYkb5opTDUFs0indJIPQJ9qgpH-j4,1305
-pgvector-0.2.0.dist-info/LICENSE.txt,sha256=3Nr5vwERQHKYiiQHzy_AO2HurO6I3TonpJlYOmwbmcI,1083
-pgvector-0.2.0.dist-info/METADATA,sha256=HGNl3-iv2BPJkqniB0tQCY2V9H0-7uDSZ9oMhFruiNQ,6666
-pgvector-0.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-pgvector-0.2.0.dist-info/top_level.txt,sha256=xGGaXFRcSRHEhn0HS1FN_UjCWr1G-WSPgxx4a0NJc0M,9
-pgvector-0.2.0.dist-info/RECORD,,
+pgvector-0.2.1.dist-info/LICENSE.txt,sha256=3Nr5vwERQHKYiiQHzy_AO2HurO6I3TonpJlYOmwbmcI,1083
+pgvector-0.2.1.dist-info/METADATA,sha256=nguJAuM9uino7gchAjjiQL9RCIlFh-B32gMwRvrxGxY,6666
+pgvector-0.2.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pgvector-0.2.1.dist-info/top_level.txt,sha256=xGGaXFRcSRHEhn0HS1FN_UjCWr1G-WSPgxx4a0NJc0M,9
+pgvector-0.2.1.dist-info/RECORD,,
```

