# Comparing `tmp/liangutil-0.0.8.tar.gz` & `tmp/liangutil-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.0.8.tar", last modified: Mon Jul 31 09:44:04 2023, max compression
+gzip compressed data, was "liangutil-0.0.9.tar", last modified: Tue Aug  1 03:16:02 2023, max compression
```

## Comparing `liangutil-0.0.8.tar` & `liangutil-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:44:04.084361 liangutil-0.0.8/
--rw-rw-rw-   0        0        0     4615 2023-07-31 09:44:04.083365 liangutil-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2849 2023-07-31 09:37:16.000000 liangutil-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 09:44:04.081376 liangutil-0.0.8/liangutil/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.0.8/liangutil/__init__.py
--rw-rw-rw-   0        0        0     2934 2023-07-31 09:41:46.000000 liangutil-0.0.8/liangutil/lianglog.py
--rw-rw-rw-   0        0        0     3493 2023-07-31 07:12:21.000000 liangutil-0.0.8/liangutil/liangutils.py
--rw-rw-rw-   0        0        0     2262 2023-07-31 03:31:30.000000 liangutil-0.0.8/liangutil/minioutils.py
--rw-rw-rw-   0        0        0     2621 2023-07-31 02:14:57.000000 liangutil-0.0.8/liangutil/mysqlutils.py
--rw-rw-rw-   0        0        0      447 2023-07-31 03:09:26.000000 liangutil-0.0.8/liangutil/redisutils.py
--rw-rw-rw-   0        0        0     9850 2023-07-31 09:40:17.000000 liangutil-0.0.8/liangutil/requestutils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:44:04.083365 liangutil-0.0.8/liangutil.egg-info/
--rw-rw-rw-   0        0        0     4615 2023-07-31 09:44:04.000000 liangutil-0.0.8/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-07-31 09:44:04.000000 liangutil-0.0.8/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 09:44:04.000000 liangutil-0.0.8/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 09:44:04.000000 liangutil-0.0.8/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 09:44:04.084361 liangutil-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-07-31 09:44:02.000000 liangutil-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:16:02.435392 liangutil-0.0.9/
+-rw-rw-rw-   0        0        0     4755 2023-08-01 03:16:02.435392 liangutil-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2949 2023-08-01 03:13:38.000000 liangutil-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 03:16:02.432336 liangutil-0.0.9/liangutil/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.0.9/liangutil/__init__.py
+-rw-rw-rw-   0        0        0     2927 2023-07-31 10:15:04.000000 liangutil-0.0.9/liangutil/lianglog.py
+-rw-rw-rw-   0        0        0     3493 2023-07-31 07:12:21.000000 liangutil-0.0.9/liangutil/liangutils.py
+-rw-rw-rw-   0        0        0     2256 2023-07-31 10:15:21.000000 liangutil-0.0.9/liangutil/minioutils.py
+-rw-rw-rw-   0        0        0     4893 2023-08-01 03:14:57.000000 liangutil-0.0.9/liangutil/mysqlutils.py
+-rw-rw-rw-   0        0        0      447 2023-07-31 03:09:26.000000 liangutil-0.0.9/liangutil/redisutils.py
+-rw-rw-rw-   0        0        0     9965 2023-07-31 10:13:08.000000 liangutil-0.0.9/liangutil/requestutils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:16:02.434394 liangutil-0.0.9/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     4755 2023-08-01 03:16:02.000000 liangutil-0.0.9/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-08-01 03:16:02.000000 liangutil-0.0.9/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:16:02.000000 liangutil-0.0.9/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 03:16:02.000000 liangutil-0.0.9/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:16:02.435392 liangutil-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-08-01 03:15:40.000000 liangutil-0.0.9/setup.py
```

### Comparing `liangutil-0.0.8/PKG-INFO` & `liangutil-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.8
+Version: 0.0.9
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -110,25 +110,30 @@
         
         - **get_configfile(self)**：读取配置文件
         - **upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO
         - **upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO，并向Redis通知
         
         
         
-        
-        
         # 更新日志
         
         ## 2023年
         
-        ### 7月
+        ### 8月
         
-        **2023-7-31** `V0.0.6`   第一个发布版本
+        **2023-08-01** `0.0.9`
+        
+        - mysqlutils 中增加了查询等方法
+        - 修复了一些 Bug
+        
+        ### 7月
         
+        **2023-07-31** `0.0.8`
         
+        - 第一个发布版本
         
         
 Keywords: python,utils,windows,mac,linux
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
```

### Comparing `liangutil-0.0.8/README.md` & `liangutil-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -102,19 +102,24 @@
 
 - **get_configfile(self)**：读取配置文件
 - **upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO
 - **upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO，并向Redis通知
 
 
 
-
-
 # 更新日志
 
 ## 2023年
 
-### 7月
+### 8月
 
-**2023-7-31** `V0.0.6`   第一个发布版本
+**2023-08-01** `0.0.9`
+
+- mysqlutils 中增加了查询等方法
+- 修复了一些 Bug
+
+### 7月
 
+**2023-07-31** `0.0.8`
 
+- 第一个发布版本
```

### Comparing `liangutil-0.0.8/liangutil/lianglog.py` & `liangutil-0.0.9/liangutil/lianglog.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         # is_print_console 是否打印到控制台
         # is_record_file 是否记录到文件中
         # is_record_db 是否记录到mysql中
         self.is_print_console = is_print_console
         self.is_record_file = is_record_file
         self.is_record_db = is_record_db
 
-        # dir_path 如果记录到文件，文件放在哪个目录
+        # file_path 如果记录到文件，文件放在哪个目录
         self.dir_path = dir_path
 
         if is_record_file == True:
             check_path(dir_path)
 
         if is_record_db == True:
             # 检查数据库连接
@@ -55,20 +55,16 @@
 
 
     def record_log_to_db(self, level, content):
         now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
         formatted_log = "{} EXCEPTION: {}".format(code_location(depth=-4), content)
         self.mysql.insert_data("program_logs", {"datetime":get_nowdatetime(), "level":level, "name":self.name, "content":formatted_log})
 
+
     # 推荐调用这个方法
     def record_log(self, level, content):
         if self.is_print_console:
             self.print_log(level, content)
         if self.is_record_file:
             self.record_log_to_file(level, content)
         if self.is_record_db:
             self.record_log_to_db(level, content)
-
-
-
-
-
```

### Comparing `liangutil-0.0.8/liangutil/liangutils.py` & `liangutil-0.0.9/liangutil/liangutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.8/liangutil/minioutils.py` & `liangutil-0.0.9/liangutil/minioutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,10 +58,7 @@
             self.minioClient.fput_object(bucket_name, file_path, current_path)
             print(current_path, "上传成功, MinIO的路径：", bucket_name + "/" + file_path)
         except Exception as e:
             print("出错了", e)
 
 
 
-
-
-
```

### Comparing `liangutil-0.0.8/liangutil/requestutils.py` & `liangutil-0.0.9/liangutil/requestutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,14 +84,17 @@
                         "content": "",
                         "url": url}
 
         return {"error": status_code,
                 "content": "",
                 "url": url}
 
+
+# https://selenium-python.readthedocs.io/page-objects.html
+# https://www.selenium.dev/zh-cn/documentation/
 # 封装 selenium
 class ChromeUtils:
     def __init__(self, timeout: int, is_ssl_verify: bool=False, is_chrome_headless:bool = False, is_undetected_chromedriver:bool = False, proxy=None):
         self.timeout = timeout  # 请求超时时间
         self.is_ssl_verify = is_ssl_verify  # 是否验证SSL证书
         self.is_chrome_headless = is_chrome_headless # Linux下 is_chrome_headless为True
         self.is_undetected_chromedriver = is_undetected_chromedriver
@@ -207,7 +210,9 @@
                     "url": self.driver.current_url}
         else:
             return {"error": "没有获得 page_source",
                     "content": "",
                     "url": self.driver.current_url}
 
 
+
+
```

### Comparing `liangutil-0.0.8/liangutil.egg-info/PKG-INFO` & `liangutil-0.0.9/liangutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.8
+Version: 0.0.9
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -110,25 +110,30 @@
         
         - **get_configfile(self)**：读取配置文件
         - **upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO
         - **upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO，并向Redis通知
         
         
         
-        
-        
         # 更新日志
         
         ## 2023年
         
-        ### 7月
+        ### 8月
         
-        **2023-7-31** `V0.0.6`   第一个发布版本
+        **2023-08-01** `0.0.9`
+        
+        - mysqlutils 中增加了查询等方法
+        - 修复了一些 Bug
+        
+        ### 7月
         
+        **2023-07-31** `0.0.8`
         
+        - 第一个发布版本
         
         
 Keywords: python,utils,windows,mac,linux
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
```

### Comparing `liangutil-0.0.8/setup.py` & `liangutil-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
 
-    version='0.0.8',
+    version='0.0.9',
     description='Encapsulate some common tool methods',
     author='LiAng',
     author_email='l2545721422@163.com',
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

