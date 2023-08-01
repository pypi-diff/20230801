# Comparing `tmp/fastmysql-0.2.2.tar.gz` & `tmp/fastmysql-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmysql-0.2.2.tar", last modified: Wed Jul 26 07:51:57 2023, max compression
+gzip compressed data, was "fastmysql-0.2.3.tar", last modified: Tue Aug  1 03:24:24 2023, max compression
```

## Comparing `fastmysql-0.2.2.tar` & `fastmysql-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:51:57.138688 fastmysql-0.2.2/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 07:51:57.138575 fastmysql-0.2.2/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.2/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:51:57.137582 fastmysql-0.2.2/fastmysql/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.2/fastmysql/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.2/fastmysql/fastmysql.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    25775 2023-07-26 07:40:51.000000 fastmysql-0.2.2/fastmysql/fastmysql_test.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:51:57.138421 fastmysql-0.2.2/fastmysql.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-26 07:51:57.138728 fastmysql-0.2.2/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-07-26 07:51:25.000000 fastmysql-0.2.2/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:24:24.439852 fastmysql-0.2.3/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-08-01 03:24:24.439725 fastmysql-0.2.3/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.3/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:24:24.438539 fastmysql-0.2.3/fastmysql/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.3/fastmysql/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.3/fastmysql/fastmysql.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    25861 2023-08-01 03:23:55.000000 fastmysql-0.2.3/fastmysql/fastmysql_test.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-01 03:24:24.439549 fastmysql-0.2.3/fastmysql.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-08-01 03:24:24.000000 fastmysql-0.2.3/fastmysql.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-08-01 03:24:24.439894 fastmysql-0.2.3/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-08-01 03:23:55.000000 fastmysql-0.2.3/setup.py
```

### Comparing `fastmysql-0.2.2/PKG-INFO` & `fastmysql-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.2.2
+Version: 0.2.3
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.2.2/README.md` & `fastmysql-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fastmysql-0.2.2/fastmysql/fastmysql.py` & `fastmysql-0.2.3/fastmysql/fastmysql.py`

 * *Files identical despite different names*

### Comparing `fastmysql-0.2.2/fastmysql/fastmysql_test.py` & `fastmysql-0.2.3/fastmysql/fastmysql_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     def __init__(
             self,
             env_file_name: str = env_file_name_default,
             silence: bool = silence_default,
             ssc: bool = False,
             auto_reconnect: bool = True,
             reconnect_wait: int = 5,
-            max_connections: int = 10
+            max_connections: int = 10,
+            timeout: int = 120
     ):
         self.env_file_name = env_file_name
         self.silence = silence
         self.con_info = self.make_con_info()
         if self.con_info:
             pass
         else:
@@ -82,15 +83,16 @@
             port=self.port,
             user=self.username,
             password=self.password,
             charset=self.charset,  # 设置字符集
             autocommit=True,  # 自动提交事务
             cursorclass=pymysql.cursors.DictCursor,  # 返回字典形式的查询结果
             maxusage=100,  # 每个连接的最大使用次数，表示每个连接最多被使用100次。当一个连接被使用次数达到100时，连接会自动关闭，并在以后的请求中重新创建一个新的连接。这样，当连接由于长时间使用而失效时，会自动重连，保证连接的可靠性。
-            connect_timeout=10  # 连接数据库的最大超时时间，单位为秒;这表示连接数据库的最大超时时间为10秒。如果在连接数据库时，超过10秒仍然未成功建立连接，连接池会自动重试连接。
+            connect_timeout=10,  # 连接数据库的最大超时时间，单位为秒;这表示连接数据库的最大超时时间为10秒。如果在连接数据库时，超过10秒仍然未成功建立连接，连接池会自动重试连接。
+            timeout=timeout  # sql执行超时时间
         )
 
     def make_con_info(
             self
     ):
         """
         读取当前环境的环境文件信息并生成连接信息
```

### Comparing `fastmysql-0.2.2/fastmysql.egg-info/PKG-INFO` & `fastmysql-0.2.3/fastmysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.2.2
+Version: 0.2.3
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.2.2/setup.py` & `fastmysql-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastmysql",
-    version="0.2.2",
+    version="0.2.3",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use pymysql",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/fastmysql",
     packages=setuptools.find_packages(),
```

