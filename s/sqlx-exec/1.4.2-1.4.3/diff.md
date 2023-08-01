# Comparing `tmp/sqlx-exec-1.4.2.tar.gz` & `tmp/sqlx-exec-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.4.2.tar", last modified: Mon Jul 31 11:35:00 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.4.3.tar", last modified: Tue Aug  1 10:46:56 2023, max compression
```

## Comparing `sqlx-exec-1.4.2.tar` & `sqlx-exec-1.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     3728 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.4.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-07-31 11:21:49.000000 sqlx-exec-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlexec/
--rw-rw-rw-   0        0        0      962 2023-07-30 16:50:50.000000 sqlx-exec-1.4.2/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.2/sqlexec/engine.py
--rw-rw-rw-   0        0        0    13957 2023-07-31 11:32:07.000000 sqlx-exec-1.4.2/sqlexec/exec.py
--rw-rw-rw-   0        0        0     2060 2023-07-31 10:39:13.000000 sqlx-exec-1.4.2/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      989 2023-07-30 14:49:13.000000 sqlx-exec-1.4.2/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.2/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1772 2023-07-30 15:17:09.000000 sqlx-exec-1.4.2/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.2/sqlexec/support.py
--rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.2/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3728 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     3750 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3163 2023-08-01 10:41:13.000000 sqlx-exec-1.4.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-08-01 10:35:42.000000 sqlx-exec-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlexec/
+-rw-rw-rw-   0        0        0      962 2023-07-30 16:50:50.000000 sqlx-exec-1.4.3/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.3/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    13903 2023-08-01 03:53:45.000000 sqlx-exec-1.4.3/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     2025 2023-08-01 10:12:06.000000 sqlx-exec-1.4.3/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      989 2023-07-30 14:49:13.000000 sqlx-exec-1.4.3/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.3/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1772 2023-07-30 15:17:09.000000 sqlx-exec-1.4.3/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.3/sqlexec/support.py
+-rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.3/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3750 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.4.2/LICENSE` & `sqlx-exec-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.2/PKG-INFO` & `sqlx-exec-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.2
+Version: 1.4.3
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
@@ -16,16 +16,18 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
-       # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+       sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       # or
+       sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+       # or
        sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
        effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
```

### Comparing `sqlx-exec-1.4.2/README.rst` & `sqlx-exec-1.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
-       # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+       sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       # or
+       sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+       # or
        sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
        effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
```

### Comparing `sqlx-exec-1.4.2/setup.py` & `sqlx-exec-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.4.2',
+    version='1.4.3',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.4.2/sqlexec/constant.py` & `sqlx-exec-1.4.3/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.2/sqlexec/engine.py` & `sqlx-exec-1.4.3/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.2/sqlexec/exec.py` & `sqlx-exec-1.4.3/sqlexec/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,16 @@
     engine, driver, creator = import_driver(driver, curr_engine)
     prepared = MYSQL_CONNECTOR_DRIVER == driver
     if PARAM_DEBUG in kwargs and kwargs.pop(PARAM_DEBUG):
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
     if PARAM_POOL_SIZE in kwargs:
-        if prepared:
-            # mysql.connector 用自带连接池
-            pool_size = kwargs[PARAM_POOL_SIZE]
-        else:
-            pool_size = kwargs.pop(PARAM_POOL_SIZE)
+        # mysql.connector 用自带连接池
+        pool_size = kwargs[PARAM_POOL_SIZE] if prepared else kwargs.pop(PARAM_POOL_SIZE)
 
     pool_args = ['mincached', 'maxcached', 'maxshared', 'maxconnections', 'blocking', 'maxusage', 'setsession', 'reset', 'failures', 'ping']
     pool_kwargs = {key: kwargs.pop(key) for key in pool_args if key in kwargs}
     connect = lambda: creator.connect(*args, **kwargs)
     if pool_size >= 1 and not prepared:
         from .pooling import pooled_connect
         connect = pooled_connect(connect, pool_size, **pool_kwargs)
@@ -69,15 +66,15 @@
         logger.info("Inited db engine <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engine, driver, pool_size))
     else:
         logger.info("Inited db engine <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engine, driver))
 
 
 def connection():
     """
-    Return _ConnectionCtx object that can be used by 'with' statement:
+    Return ConnectionCtx object that can be used by 'with' statement:
     with connection():
         pass
     """
     global _DB_CTX
     return ConnectionCtx(_DB_CTX)
```

### Comparing `sqlx-exec-1.4.2/sqlexec/init_import.py` & `sqlx-exec-1.4.3/sqlexec/init_import.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 
 
 def get_engine(driver: str, *args, **kwargs):
     curr_engine = Engine.current_engine()
     if driver is None and (curr_engine is None or curr_engine == UNKNOW):
         if args and isinstance(args[0], str):
             if 'mysql://' in args[0]:
-                curr_engine = MYSQL
+                return MYSQL
             elif 'postgres://' in args[0]:
-                curr_engine = POSTGRESQL
+                return POSTGRESQL
             elif '://' not in args[0]:
-                curr_engine = SQLITE
+                return SQLITE
         elif  PARAM_PORT in kwargs:
             port = kwargs[PARAM_PORT]
             if port == MYSQL_PORT:
-                curr_engine = MYSQL
+                return MYSQL
             elif port == POSTGRESQL_PORT:
-                curr_engine = POSTGRESQL
+                return POSTGRESQL
     return curr_engine
```

### Comparing `sqlx-exec-1.4.2/sqlexec/log_support.py` & `sqlx-exec-1.4.3/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.2/sqlexec/pooling.py` & `sqlx-exec-1.4.3/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.2/sqlexec/sql_support.py` & `sqlx-exec-1.4.3/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.2/sqlexec/support.py` & `sqlx-exec-1.4.3/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.2/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.4.3/sqlx_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.2
+Version: 1.4.3
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
@@ -16,16 +16,18 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       # sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
-       # sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+       sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       # or
+       sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+       # or
        sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
        effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
```

