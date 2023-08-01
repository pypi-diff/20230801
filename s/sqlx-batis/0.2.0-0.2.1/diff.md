# Comparing `tmp/sqlx-batis-0.2.0.tar.gz` & `tmp/sqlx-batis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.2.0.tar", last modified: Mon Jul 31 11:36:14 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.2.1.tar", last modified: Tue Aug  1 10:36:41 2023, max compression
```

## Comparing `sqlx-batis-0.2.0.tar` & `sqlx-batis-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/
--rw-rw-rw-   0        0        0     5701 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-0.2.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1352 2023-07-31 11:35:19.000000 sqlx-batis-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlbatis/
--rw-rw-rw-   0        0        0      902 2023-07-30 16:13:17.000000 sqlx-batis-0.2.0/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8588 2023-07-31 11:27:17.000000 sqlx-batis-0.2.0/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-0.2.0/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     6724 2023-07-30 16:13:17.000000 sqlx-batis-0.2.0/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     3883 2023-07-31 11:35:56.000000 sqlx-batis-0.2.0/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.2.0/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.2.0/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.2.0/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-0.2.0/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1637 2023-07-31 11:12:07.000000 sqlx-batis-0.2.0/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.2.0/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.2.0/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5701 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/
+-rw-rw-rw-   0        0        0     5701 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-0.2.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-08-01 10:36:35.000000 sqlx-batis-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlbatis/
+-rw-rw-rw-   0        0        0      933 2023-08-01 10:18:34.000000 sqlx-batis-0.2.1/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8726 2023-08-01 10:31:42.000000 sqlx-batis-0.2.1/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-0.2.1/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6724 2023-07-30 16:13:17.000000 sqlx-batis-0.2.1/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     3883 2023-07-31 11:35:56.000000 sqlx-batis-0.2.1/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.2.1/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.2.1/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.2.1/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-0.2.1/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1659 2023-08-01 10:31:42.000000 sqlx-batis-0.2.1/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.2.1/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1662 2023-08-01 10:18:34.000000 sqlx-batis-0.2.1/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5701 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.2.0/PKG-INFO` & `sqlx-batis-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.2.0/README.rst` & `sqlx-batis-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.0/setup.py` & `sqlx-batis-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'sqlx-exec>=1.4.2',
     ],
-    version='0.2.0',
+    version='0.2.1',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.2.0/sqlbatis/constant.py` & `sqlx-batis-0.2.1/sqlbatis/constant.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 LIMIT_1 = 1
 
 NO_LIMIT = 0
 
 CACHE_SIZE = 256
 
+MAPPER_PATH = 'mapper_path'
+
 MYSQL_SELECT_KEY = "SELECT LAST_INSERT_ID()"
 
 SQLITE_SELECT_KEY = 'SELECT last_insert_rowid()'
 
 MYSQL_COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
                         FROM information_schema.columns WHERE table_schema = (SELECT DATABASE()) AND table_name = ? LIMIT ?'''
```

### Comparing `sqlx-batis-0.2.0/sqlbatis/db.py` & `sqlx-batis-0.2.1/sqlbatis/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,26 +145,26 @@
 def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     page_log('query_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    sql, args = _try_mapping(sql, *args, **kwargs)
     return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     page_log('select_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    sql, args = _try_mapping(sql, *args, **kwargs)
     return do_select_page(sql, page_num, page_size, *args)
 
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
@@ -185,10 +185,14 @@
 
 
 def _try_dynamic_sql(function, sql, *args, **kwargs):
     sql = sql_support.dynamic_sql(sql, **kwargs)
     return try_mapping(function, sql, *args, **kwargs)
 
 
+def _try_mapping(sql, *args, **kwargs):
+    sql = sql_support.dynamic_sql(sql, **kwargs)
+    return sql_support.get_mapping_sql_args(sql, *args, **kwargs)
+
 def _do_limit_sql_args(function, sql, *args):
     do_sql_log(function, sql, *args)
     return sql_support.limit_one_sql_args(sql, *args)
```

### Comparing `sqlx-batis-0.2.0/sqlbatis/dbx.py` & `sqlx-batis-0.2.1/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.0/sqlbatis/engine.py` & `sqlx-batis-0.2.1/sqlbatis/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.0/sqlbatis/log_support.py` & `sqlx-batis-0.2.1/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.0/sqlbatis/orm.py` & `sqlx-batis-0.2.1/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.0/sqlbatis/snowflake.py` & `sqlx-batis-0.2.1/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.0/sqlbatis/sql_holder.py` & `sqlx-batis-0.2.1/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.0/sqlbatis/sql_mapper.py` & `sqlx-batis-0.2.1/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.0/sqlbatis/sql_support.py` & `sqlx-batis-0.2.1/sqlbatis/sql_support.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from jinja2 import Template
 from functools import lru_cache
 from .support import MapperError
 from .constant import LIMIT_1, DYNAMIC_REGEX, CACHE_SIZE
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec.sql_support import get_named_args, get_named_sql, get_batch_args, get_named_sql_args, is_mapping
+from sqlexec.sql_support import get_named_args, get_named_sql, get_batch_args, get_named_sql_args, is_mapping, get_mapping_sql_args
 
 
 def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
 
 
 def dynamic_sql(sql: str, **kwargs):
```

### Comparing `sqlx-batis-0.2.0/sqlbatis/__init__.py` & `sqlx-batis-0.2.1/sqlbatis/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     :param show_sql=False: bool,  if True, print sql
     :param debug=False: bool, if True, print debug context
     :param trans_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
 
+    from .constant import MAPPER_PATH
     from .sql_holder import load_mapper
     from sqlexec import init_db as supper_init_db
 
-    mapper_path = kwargs.pop('mapper_path') if 'mapper_path' in kwargs else None
+    mapper_path = kwargs.pop(MAPPER_PATH) if MAPPER_PATH in kwargs else None
     Engine.init()
     supper_init_db(*args, **kwargs)
     if mapper_path:
         load_mapper(mapper_path)
```

### Comparing `sqlx-batis-0.2.0/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.2.1/sqlx_batis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

