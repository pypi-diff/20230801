# Comparing `tmp/liangutil-0.0.9.tar.gz` & `tmp/liangutil-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.0.9.tar", last modified: Tue Aug  1 03:16:02 2023, max compression
+gzip compressed data, was "liangutil-0.1.0.tar", last modified: Tue Aug  1 03:31:58 2023, max compression
```

## Comparing `liangutil-0.0.9.tar` & `liangutil-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:16:02.435392 liangutil-0.0.9/
--rw-rw-rw-   0        0        0     4755 2023-08-01 03:16:02.435392 liangutil-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2949 2023-08-01 03:13:38.000000 liangutil-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 03:16:02.432336 liangutil-0.0.9/liangutil/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.0.9/liangutil/__init__.py
--rw-rw-rw-   0        0        0     2927 2023-07-31 10:15:04.000000 liangutil-0.0.9/liangutil/lianglog.py
--rw-rw-rw-   0        0        0     3493 2023-07-31 07:12:21.000000 liangutil-0.0.9/liangutil/liangutils.py
--rw-rw-rw-   0        0        0     2256 2023-07-31 10:15:21.000000 liangutil-0.0.9/liangutil/minioutils.py
--rw-rw-rw-   0        0        0     4893 2023-08-01 03:14:57.000000 liangutil-0.0.9/liangutil/mysqlutils.py
--rw-rw-rw-   0        0        0      447 2023-07-31 03:09:26.000000 liangutil-0.0.9/liangutil/redisutils.py
--rw-rw-rw-   0        0        0     9965 2023-07-31 10:13:08.000000 liangutil-0.0.9/liangutil/requestutils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:16:02.434394 liangutil-0.0.9/liangutil.egg-info/
--rw-rw-rw-   0        0        0     4755 2023-08-01 03:16:02.000000 liangutil-0.0.9/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-08-01 03:16:02.000000 liangutil-0.0.9/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:16:02.000000 liangutil-0.0.9/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 03:16:02.000000 liangutil-0.0.9/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 03:16:02.435392 liangutil-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-08-01 03:15:40.000000 liangutil-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:31:58.415410 liangutil-0.1.0/
+-rw-rw-rw-   0        0        0     4775 2023-08-01 03:31:58.415410 liangutil-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2953 2023-08-01 03:31:28.000000 liangutil-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 03:31:58.412384 liangutil-0.1.0/liangutil/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.0/liangutil/__init__.py
+-rw-rw-rw-   0        0        0     2927 2023-07-31 10:15:04.000000 liangutil-0.1.0/liangutil/lianglog.py
+-rw-rw-rw-   0        0        0     3595 2023-08-01 03:30:49.000000 liangutil-0.1.0/liangutil/liangutils.py
+-rw-rw-rw-   0        0        0     2256 2023-07-31 10:15:21.000000 liangutil-0.1.0/liangutil/minioutils.py
+-rw-rw-rw-   0        0        0     4893 2023-08-01 03:26:27.000000 liangutil-0.1.0/liangutil/mysqlutils.py
+-rw-rw-rw-   0        0        0      447 2023-07-31 03:09:26.000000 liangutil-0.1.0/liangutil/redisutils.py
+-rw-rw-rw-   0        0        0     9965 2023-07-31 10:13:08.000000 liangutil-0.1.0/liangutil/requestutils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:31:58.414413 liangutil-0.1.0/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     4775 2023-08-01 03:31:58.000000 liangutil-0.1.0/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-08-01 03:31:58.000000 liangutil-0.1.0/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:31:58.000000 liangutil-0.1.0/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 03:31:58.000000 liangutil-0.1.0/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:31:58.415410 liangutil-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-08-01 03:31:54.000000 liangutil-0.1.0/setup.py
```

### Comparing `liangutil-0.0.9/PKG-INFO` & `liangutil-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.9
+Version: 0.1.0
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -116,15 +116,17 @@
         
         # 更新日志
         
         ## 2023年
         
         ### 8月
         
-        **2023-08-01** `0.0.9`
+        
+        
+        **2023-08-01** `0.1.0`
         
         - mysqlutils 中增加了查询等方法
         - 修复了一些 Bug
         
         ### 7月
         
         **2023-07-31** `0.0.8`
```

### Comparing `liangutil-0.0.9/README.md` & `liangutil-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,17 @@
 
 # 更新日志
 
 ## 2023年
 
 ### 8月
 
-**2023-08-01** `0.0.9`
+
+
+**2023-08-01** `0.1.0`
 
 - mysqlutils 中增加了查询等方法
 - 修复了一些 Bug
 
 ### 7月
 
 **2023-07-31** `0.0.8`
```

### Comparing `liangutil-0.0.9/liangutil/lianglog.py` & `liangutil-0.1.0/liangutil/lianglog.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.9/liangutil/liangutils.py` & `liangutil-0.1.0/liangutil/liangutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,20 @@
     return bool(re.search(pattern, path))
 
 # 如果是文件路径，提取父级目录路径
 # 相对路径不要使用 ./ 开头
 def get_dirpath(path):
     # 是文件路径，需要提取父级目录路径
     if is_filepath(path):
+        # 获取当前操作系统的文件目录分隔符
+        separator = os.sep
+
         # 有父级目录
-        if str(path).rfind(".") != -1 and str(path).rfind("/") != -1:
-            return str(path).rsplit("/", 1)[0]
+        if str(path).rfind(".") != -1 and str(path).rfind(separator) != -1:
+            return str(path).rsplit(separator, 1)[0]
         elif str(path).rfind(".") != -1:
             # 类似 a.txt
             return ""
         else:
             return ""
     else:
         return path
```

### Comparing `liangutil-0.0.9/liangutil/minioutils.py` & `liangutil-0.1.0/liangutil/minioutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.9/liangutil/mysqlutils.py` & `liangutil-0.1.0/liangutil/mysqlutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.9/liangutil/requestutils.py` & `liangutil-0.1.0/liangutil/requestutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.9/liangutil.egg-info/PKG-INFO` & `liangutil-0.1.0/liangutil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.9
+Version: 0.1.0
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -116,15 +116,17 @@
         
         # 更新日志
         
         ## 2023年
         
         ### 8月
         
-        **2023-08-01** `0.0.9`
+        
+        
+        **2023-08-01** `0.1.0`
         
         - mysqlutils 中增加了查询等方法
         - 修复了一些 Bug
         
         ### 7月
         
         **2023-07-31** `0.0.8`
```

### Comparing `liangutil-0.0.9/setup.py` & `liangutil-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
 
-    version='0.0.9',
+    version='0.1.0',
     description='Encapsulate some common tool methods',
     author='LiAng',
     author_email='l2545721422@163.com',
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

