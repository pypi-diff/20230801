# Comparing `tmp/TinetApiRequest-1.0.8.tar.gz` & `tmp/TinetApiRequest-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.0.8.tar", last modified: Tue Aug  1 08:01:13 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.0.9.tar", last modified: Tue Aug  1 08:09:28 2023, max compression
```

## Comparing `TinetApiRequest-1.0.8.tar` & `TinetApiRequest-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/
--rw-rw-rw-   0        0        0      272 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-08-01 08:01:09.000000 TinetApiRequest-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/tinet/
--rw-rw-rw-   0        0        0    23081 2023-08-01 08:01:09.000000 TinetApiRequest-1.0.8/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     7188 2023-08-01 06:49:58.000000 TinetApiRequest-1.0.8/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.8/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.0.8/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.8/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.8/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.8/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-08-01 08:09:23.000000 TinetApiRequest-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:09:28.000000 TinetApiRequest-1.0.9/tinet/
+-rw-rw-rw-   0        0        0    23081 2023-08-01 08:01:09.000000 TinetApiRequest-1.0.9/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     7147 2023-08-01 08:09:23.000000 TinetApiRequest-1.0.9/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.9/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.0.9/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.9/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.9/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.9/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.0.8/README.md` & `TinetApiRequest-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.8/setup.py` & `TinetApiRequest-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.0.8",
+    version="1.0.9",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.0.8/tinet/APIRequest.py` & `TinetApiRequest-1.0.9/tinet/APIRequest.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.8/tinet/ApiConfig.py` & `TinetApiRequest-1.0.9/tinet/ApiConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import random
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
 import datetime
 import pytz
 import hashlib
 import base64
-from requests import Session
 
 
 class times:
     def __init__(self, dt=None, tz=pytz.timezone('Asia/Shanghai')):
         """
         初始化时间工具类
 
@@ -161,15 +160,15 @@
 
 
 class config:
     """
     配置文件
     """
 
-    def __init__(self, baseUrl=None, AccessKeyId=None, AccessKeySecret=None, SKPassword=None, commonTestCasePath=None, methObj=None, assertFail='stop', session: Session = None):
+    def __init__(self, baseUrl=None, AccessKeyId=None, AccessKeySecret=None, SKPassword=None, commonTestCasePath=None, methObj=None, assertFail='stop', session=None):
         """
         初始化配置文件
         """
         self._baseUrl = baseUrl
         self._accessKeyId = AccessKeyId
         self._accessKeySecret = AccessKeySecret
         # SK加密 登录密码 后的 密码加密文本
```

### Comparing `TinetApiRequest-1.0.8/tinet/LogUtil.py` & `TinetApiRequest-1.0.9/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.8/tinet/RequestUtil.py` & `TinetApiRequest-1.0.9/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.8/tinet/SignUtil.py` & `TinetApiRequest-1.0.9/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.8/tinet/YamlUtil.py` & `TinetApiRequest-1.0.9/tinet/YamlUtil.py`

 * *Files identical despite different names*

