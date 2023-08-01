# Comparing `tmp/fastmysql-0.2.3.tar.gz` & `tmp/fastmysql-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmysql-0.2.3.tar", last modified: Tue Aug  1 03:24:24 2023, max compression
+gzip compressed data, was "fastmysql-0.2.4.tar", last modified: Tue Aug  1 03:39:37 2023, max compression
```

## Comparing `fastmysql-0.2.3.tar` & `fastmysql-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:24:24.439852 fastmysql-0.2.3/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-08-01 03:24:24.439725 fastmysql-0.2.3/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.3/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:24:24.438539 fastmysql-0.2.3/fastmysql/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.3/fastmysql/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.3/fastmysql/fastmysql.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    25861 2023-08-01 03:23:55.000000 fastmysql-0.2.3/fastmysql/fastmysql_test.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:24:24.439549 fastmysql-0.2.3/fastmysql.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-08-01 03:24:24.439894 fastmysql-0.2.3/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-08-01 03:23:55.000000 fastmysql-0.2.3/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:39:37.045730 fastmysql-0.2.4/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-08-01 03:39:37.045618 fastmysql-0.2.4/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.4/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:39:37.044738 fastmysql-0.2.4/fastmysql/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.4/fastmysql/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.4/fastmysql/fastmysql.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    26460 2023-08-01 03:39:08.000000 fastmysql-0.2.4/fastmysql/fastmysql_test.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:39:37.045467 fastmysql-0.2.4/fastmysql.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-08-01 03:39:37.000000 fastmysql-0.2.4/fastmysql.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-08-01 03:39:37.000000 fastmysql-0.2.4/fastmysql.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-08-01 03:39:37.000000 fastmysql-0.2.4/fastmysql.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-08-01 03:39:37.000000 fastmysql-0.2.4/fastmysql.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-08-01 03:39:37.000000 fastmysql-0.2.4/fastmysql.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-08-01 03:39:37.045769 fastmysql-0.2.4/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-08-01 03:39:08.000000 fastmysql-0.2.4/setup.py
```

### Comparing `fastmysql-0.2.3/PKG-INFO` & `fastmysql-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.2.3
+Version: 0.2.4
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.2.3/README.md` & `fastmysql-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fastmysql-0.2.3/fastmysql/fastmysql.py` & `fastmysql-0.2.4/fastmysql/fastmysql.py`

 * *Files identical despite different names*

### Comparing `fastmysql-0.2.3/fastmysql/fastmysql_test.py` & `fastmysql-0.2.4/fastmysql/fastmysql_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,17 @@
             self,
             env_file_name: str = env_file_name_default,
             silence: bool = silence_default,
             ssc: bool = False,
             auto_reconnect: bool = True,
             reconnect_wait: int = 5,
             max_connections: int = 10,
-            timeout: int = 120
+            max_shared: int = 10,
+            max_cached: int = 5,
+            min_cached: int = 2
     ):
         self.env_file_name = env_file_name
         self.silence = silence
         self.con_info = self.make_con_info()
         if self.con_info:
             pass
         else:
@@ -71,28 +73,28 @@
         self.charset = self.con_info.get("charset", "utf8mb4")
         self.ssc = ssc
         self.auto_reconnect = auto_reconnect
         self.reconnect_wait = reconnect_wait
         self.POOL = PooledDB(
             creator=pymysql,  # 使用pymysql作为连接器
             maxconnections=max_connections,  # 连接池允许的最大连接数
-            # maxcached=10,
-            # maxshared=10,
+            maxcached=max_cached,  # 参数用于指定连接池中允许缓存的最大空闲连接数。当连接池中存在多余的连接，并且超过了maxcached限制时，多余的空闲连接将会被关闭和释放，以避免连接池中连接数过多。
+            mincached=min_cached,
+            maxshared=max_shared,  # 参数用于指定在连接池中可以共享的最大连接数。当多个线程或进程同时请求数据库连接时，如果连接池中存在空闲的连接且未达到maxshared限制，那么这些请求将共享同一个连接，从而减少了连接的创建和销毁开销，提高了性能
             blocking=True,  # 如果连接池为空，getconn方法将会阻塞等待
             setsession=[],
             host=self.host,
             port=self.port,
             user=self.username,
             password=self.password,
             charset=self.charset,  # 设置字符集
             autocommit=True,  # 自动提交事务
             cursorclass=pymysql.cursors.DictCursor,  # 返回字典形式的查询结果
             maxusage=100,  # 每个连接的最大使用次数，表示每个连接最多被使用100次。当一个连接被使用次数达到100时，连接会自动关闭，并在以后的请求中重新创建一个新的连接。这样，当连接由于长时间使用而失效时，会自动重连，保证连接的可靠性。
-            connect_timeout=10,  # 连接数据库的最大超时时间，单位为秒;这表示连接数据库的最大超时时间为10秒。如果在连接数据库时，超过10秒仍然未成功建立连接，连接池会自动重试连接。
-            timeout=timeout  # sql执行超时时间
+            connect_timeout=10  # 连接数据库的最大超时时间，单位为秒;这表示连接数据库的最大超时时间为10秒。如果在连接数据库时，超过10秒仍然未成功建立连接，连接池会自动重试连接。
         )
 
     def make_con_info(
             self
     ):
         """
         读取当前环境的环境文件信息并生成连接信息
```

### Comparing `fastmysql-0.2.3/fastmysql.egg-info/PKG-INFO` & `fastmysql-0.2.4/fastmysql.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.2.3
+Version: 0.2.4
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.2.3/setup.py` & `fastmysql-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastmysql",
-    version="0.2.3",
+    version="0.2.4",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use pymysql",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/fastmysql",
     packages=setuptools.find_packages(),
```

