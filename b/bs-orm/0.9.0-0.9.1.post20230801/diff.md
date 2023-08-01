# Comparing `tmp/bs_orm-0.9.0.tar.gz` & `tmp/bs_orm-0.9.1.post20230801.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.9.0.tar", last modified: Thu Jun 15 01:35:15 2023, max compression
+gzip compressed data, was "bs_orm-0.9.1.post20230801.tar", last modified: Tue Aug  1 19:25:05 2023, max compression
```

## Comparing `bs_orm-0.9.0.tar` & `bs_orm-0.9.1.post20230801.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:35:15.301392 bs_orm-0.9.0/
--rw-rw-rw-   0        0        0      108 2023-06-15 01:35:15.302604 bs_orm-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 01:35:15.292079 bs_orm-0.9.0/bs_orm/
--rw-rw-rw-   0        0        0     4887 2023-06-15 01:26:56.000000 bs_orm-0.9.0/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0    10036 2023-06-15 01:26:11.000000 bs_orm-0.9.0/bs_orm/Requests.py
--rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.9.0/bs_orm/__init__.py
--rw-rw-rw-   0        0        0       32 2023-06-15 00:01:44.000000 bs_orm-0.9.0/bs_orm/db_settings.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:35:15.300381 bs_orm-0.9.0/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      108 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 01:35:15.303616 bs_orm-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      292 2023-06-15 01:35:05.000000 bs_orm-0.9.0/setup.py
+drwxr-xr-x   0 jost221   (1000) jost221   (1000)        0 2023-08-01 19:25:05.338770 bs_orm-0.9.1.post20230801/
+-rw-r--r--   0 jost221   (1000) jost221   (1000)      131 2023-08-01 19:25:05.339770 bs_orm-0.9.1.post20230801/PKG-INFO
+-rw-r--r--   0 jost221   (1000) jost221   (1000)     2451 2023-07-27 10:23:46.000000 bs_orm-0.9.1.post20230801/README.md
+drwxr-xr-x   0 jost221   (1000) jost221   (1000)        0 2023-08-01 19:25:05.317770 bs_orm-0.9.1.post20230801/bs_orm/
+-rw-r--r--   0 jost221   (1000) jost221   (1000)     2875 2023-07-31 20:33:23.000000 bs_orm-0.9.1.post20230801/bs_orm/DataTypes.py
+-rw-r--r--   0 jost221   (1000) jost221   (1000)     6208 2023-07-27 18:51:12.000000 bs_orm-0.9.1.post20230801/bs_orm/Requests.py
+-rw-r--r--   0 jost221   (1000) jost221   (1000)        0 2023-07-27 10:23:46.000000 bs_orm-0.9.1.post20230801/bs_orm/__init__.py
+-rw-r--r--   0 jost221   (1000) jost221   (1000)       31 2023-07-27 10:23:46.000000 bs_orm-0.9.1.post20230801/bs_orm/db_settings.py
+drwxr-xr-x   0 jost221   (1000) jost221   (1000)        0 2023-08-01 19:25:05.336770 bs_orm-0.9.1.post20230801/bs_orm.egg-info/
+-rw-r--r--   0 jost221   (1000) jost221   (1000)      131 2023-08-01 19:25:05.000000 bs_orm-0.9.1.post20230801/bs_orm.egg-info/PKG-INFO
+-rw-r--r--   0 jost221   (1000) jost221   (1000)      257 2023-08-01 19:25:05.000000 bs_orm-0.9.1.post20230801/bs_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 jost221   (1000) jost221   (1000)        1 2023-08-01 19:25:05.000000 bs_orm-0.9.1.post20230801/bs_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 jost221   (1000) jost221   (1000)        1 2023-08-01 19:25:05.000000 bs_orm-0.9.1.post20230801/bs_orm.egg-info/not-zip-safe
+-rw-r--r--   0 jost221   (1000) jost221   (1000)        7 2023-08-01 19:25:05.000000 bs_orm-0.9.1.post20230801/bs_orm.egg-info/top_level.txt
+-rw-r--r--   0 jost221   (1000) jost221   (1000)       47 2023-08-01 19:25:05.346770 bs_orm-0.9.1.post20230801/setup.cfg
+-rw-r--r--   0 jost221   (1000) jost221   (1000)      294 2023-08-01 19:21:58.000000 bs_orm-0.9.1.post20230801/setup.py
```

### Comparing `bs_orm-0.9.0/README.md` & `bs_orm-0.9.1.post20230801/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# better-orm Python 
-
-История такова:
-
-> Писал я значит проект и меня так сильно затрахала привязанность 
-либо к одному фреймворку либо отсутствие миграций как например в 
-SQLAlhimy (либо я просто не разобрался как они работают) что решил 
-ебануть свою orm минут за 30 я понял что это относительно не сложно 
-и начал хуярить
-
-## How to use?
-
-Consider how to use
-
----
-
-### Create DB
-
-you need create file
-> models.py
-
-in this file you need keep only your model and variables your model
-
-example of a filling file
-
-```Python
-from better_orm import DataTypes
-
-class a(DataTypes.Table_Engine):
-    var1 = DataTypes.String(default='default', size=10)
-    var2 = DataTypes.Integer(primary_key=True, auto_increment=True) 
-
-class abob(DataTypes.Table_Engine):
-    name = DataTypes.String(primary_key=True)
-```
-
-then you need run function `create_db()`
-
----
-
-if you need custom name db you need `import DataType` and in replace `db_settings.path`
-
-you can add in your code this line
-
-```python
-from better_orm import DataTypes
-
-DataTypes.db_settings.path = 'database.db'
-```
----
-
-`create_db_from_models.py` creates your database. With this data you get next data base:
-
-| a | aboba |
-|-----:|-----------|
-|var1|name|
-|var2| |
-
----
-
-## Write data
-
-For write data with this library you need using function `write_row(table_name, **data)`
-
-Example:
-```python
-write_row(models.a, var1='value1')
-```
-
-with this function your database get next value
-Table a:
-
-| var1 | var2 |
-|-----:|-----------|
-|"value1"|1|
-
-or using models
-
-```Python
-mod = a.add(var1="oaoaoaoa")
-mod.save()
-```
-
-if you use this code you get the same result as with funcrions write_db
-
----
-
-after write data you need and read it. for read using your class with model
-
-Exemple:
-```python
-from models import *
-
-response = a.read()
-```
-in result you get list object 'a' with variables var1 and var2
-
-<picture>
-  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://im.wampi.ru/2023/03/10/image1cf39d530b24f1ae.png">
-</picture>
-
-further more.
-stages of development:
-1. adding complex values such as datetime
-2. Validations for programmer errors when creating a database
-3. Adding migration capability
+# better-orm Python 
+
+История такова:
+
+> Писал я значит проект и меня так сильно затрахала привязанность 
+либо к одному фреймворку либо отсутствие миграций как например в 
+SQLAlhimy (либо я просто не разобрался как они работают) что решил 
+ебануть свою orm минут за 30 я понял что это относительно не сложно 
+и начал хуярить
+
+## How to use?
+
+Consider how to use
+
+---
+
+### Create DB
+
+you need create file
+> models.py
+
+in this file you need keep only your model and variables your model
+
+example of a filling file
+
+```Python
+from better_orm import DataTypes
+
+class a(DataTypes.Table_Engine):
+    var1 = DataTypes.String(default='default', size=10)
+    var2 = DataTypes.Integer(primary_key=True, auto_increment=True) 
+
+class abob(DataTypes.Table_Engine):
+    name = DataTypes.String(primary_key=True)
+```
+
+then you need run function `create_db()`
+
+---
+
+if you need custom name db you need `import DataType` and in replace `db_settings.path`
+
+you can add in your code this line
+
+```python
+from better_orm import DataTypes
+
+DataTypes.db_settings.path = 'database.db'
+```
+---
+
+`create_db_from_models.py` creates your database. With this data you get next data base:
+
+| a | aboba |
+|-----:|-----------|
+|var1|name|
+|var2| |
+
+---
+
+## Write data
+
+For write data with this library you need using function `write_row(table_name, **data)`
+
+Example:
+```python
+write_row(models.a, var1='value1')
+```
+
+with this function your database get next value
+Table a:
+
+| var1 | var2 |
+|-----:|-----------|
+|"value1"|1|
+
+or using models
+
+```Python
+mod = a.add(var1="oaoaoaoa")
+mod.save()
+```
+
+if you use this code you get the same result as with funcrions write_db
+
+---
+
+after write data you need and read it. for read using your class with model
+
+Exemple:
+```python
+from models import *
+
+response = a.read()
+```
+in result you get list object 'a' with variables var1 and var2
+
+<picture>
+  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://im.wampi.ru/2023/03/10/image1cf39d530b24f1ae.png">
+</picture>
+
+further more.
+stages of development:
+1. adding complex values such as datetime
+2. Validations for programmer errors when creating a database
+3. Adding migration capability
 4. Injection protection
```

