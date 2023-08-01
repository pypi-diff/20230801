# Comparing `tmp/dalpha-0.1.4.tar.gz` & `tmp/dalpha-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.1.4.tar", max compression
+gzip compressed data, was "dalpha-0.1.6.tar", max compression
```

## Comparing `dalpha-0.1.4.tar` & `dalpha-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      459 2023-05-27 07:33:56.211092 dalpha-0.1.4/README.md
--rw-r--r--   0        0        0     6468 2023-07-07 12:13:08.221508 dalpha-0.1.4/dalpha/__init__.py
--rw-r--r--   0        0        0      800 2023-07-07 12:13:34.068442 dalpha-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 dalpha-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      459 2023-05-28 23:48:43.785059 dalpha-0.1.6/README.md
+-rw-r--r--   0        0        0     7360 2023-08-01 04:31:57.475292 dalpha-0.1.6/dalpha/__init__.py
+-rw-r--r--   0        0        0      800 2023-08-01 04:34:33.970466 dalpha-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 dalpha-0.1.6/PKG-INFO
```

### Comparing `dalpha-0.1.4/dalpha/__init__.py` & `dalpha-0.1.6/dalpha/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,26 @@
-import requests, json, boto3, io, logging, sys, os
+import requests, json, boto3, io, logging, sys, os, pkg_resources
 import time
 
+logging.basicConfig(level=logging.INFO)
+def check_package_version(package_name):
+    installed_version = pkg_resources.get_distribution(package_name).version
+    try:
+        url = f"https://pypi.org/pypi/{package_name}/json"
+        response = requests.get(url)
+        data = response.json()
+        latest_version = data["info"]["version"]
+        if latest_version != installed_version:
+            logging.warning(" dalpha sdk 버전 -> " + installed_version + " / 최신 버전 -> " + latest_version)
+        else:
+            logging.info(" dalpha sdk 버전 -> " + installed_version + " (latest)")
+    except Exception as e:
+        logging.warning("dalpha sdk 버전 확인 중 오류가 발생했습니다:", e)
+check_package_version("dalpha")
+
 class Agent:
     def __init__(self, api_id, use_sqs = False, dev_server=False):
         self.cfg_path = os.path.join(sys.path[0],'.dalphacfg')
         self.__load_config(self.cfg_path)
         self.token = os.environ['TOKEN']
         if dev_server:
             self.base_url = os.environ['DEV_BASE_URL']
@@ -14,15 +30,17 @@
         self.evaluate_url = os.path.join(self.base_url, f"inferences/{api_id}/evaluate")
         self.api_id = api_id
         self.mock = {}
         self.s3 = boto3.client('s3')
         self.sqs = boto3.client('sqs', region_name='ap-northeast-2')
         self.evaluates = {}
         self.use_sqs = use_sqs
-        
+        if self.use_sqs and dev_server:
+            raise Exception(f'개발 서버에서는 sqs를 사용할 수 없습니다.')
+
     def __load_config(self,file_path):
         if not os.path.isfile(file_path):
             logging.warning(f"{file_path} 파일을 찾을 수 없습니다.")
             return
         
         with open(file_path, 'r') as file:
             lines = file.readlines()
```

### Comparing `dalpha-0.1.4/pyproject.toml` & `dalpha-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.1.4"
+version = "0.1.6"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -13,15 +13,15 @@
 build = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.1.2"
+version = "0.1.6"
 authors = [
   { name="Beomseok", email="beomseok.lee@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dalpha-0.1.4/PKG-INFO` & `dalpha-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.1.4
+Version: 0.1.6
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

