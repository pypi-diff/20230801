# Comparing `tmp/TinetApiRequest-1.1.0.tar.gz` & `tmp/TinetApiRequest-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.1.0.tar", last modified: Tue Aug  1 08:16:25 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.1.1.tar", last modified: Tue Aug  1 08:23:41 2023, max compression
```

## Comparing `TinetApiRequest-1.1.0.tar` & `TinetApiRequest-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/
--rw-rw-rw-   0        0        0      272 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-08-01 08:16:17.000000 TinetApiRequest-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:16:25.000000 TinetApiRequest-1.1.0/tinet/
--rw-rw-rw-   0        0        0    23085 2023-08-01 08:16:17.000000 TinetApiRequest-1.1.0/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     7147 2023-08-01 08:09:23.000000 TinetApiRequest-1.1.0/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.1.0/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.1.0/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.1.0/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.1.0/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.1.0/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-08-01 08:23:28.000000 TinetApiRequest-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:23:41.000000 TinetApiRequest-1.1.1/tinet/
+-rw-rw-rw-   0        0        0    23109 2023-08-01 08:22:27.000000 TinetApiRequest-1.1.1/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     7147 2023-08-01 08:09:23.000000 TinetApiRequest-1.1.1/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.1.1/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.1.1/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.1.1/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.1.1/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.1.1/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.1.0/README.md` & `TinetApiRequest-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.0/setup.py` & `TinetApiRequest-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.1.0",
+    version="1.1.1",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.1.0/tinet/APIRequest.py` & `TinetApiRequest-1.1.1/tinet/APIRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,17 @@
         yamlKind = yaml.get('kind')
         yamlTestcase = yaml.get('testcases')
         # 先拿到所有testcase
         log.info(f"开始执行测试用例name: {yamlName}, id: {yamlId} , 测试用例: {yamlTestcase}")
         allure.attach(f"{yamlTestcase}", name=f"开始执行测试用例name: {yamlName}, id: {yamlId} ", attachment_type=allure.attachment_type.TEXT)
         # 添加公共session  判断是否有公共session
         clientSession = HttpClient()
-        # if config.session is not None:
-        #     clientSession = config.session
+        # 判断是否有公共session
+        if config.session:
+            clientSession = config.session
         # 开始遍历testcase
         # allure.dynamic.title(yamlName)
         for testcase in yamlTestcase:
             with allure.step(testcase.get('name')):
                 # 拿到用例如果是common的去common文件路径中拿测试用例
                 if testcase.get('skip'):  # 判断是否跳过
                     log.info(f"用例: {json.dumps(testcase.get('name'), indent=4, ensure_ascii=False)}跳过")
```

### Comparing `TinetApiRequest-1.1.0/tinet/ApiConfig.py` & `TinetApiRequest-1.1.1/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.0/tinet/LogUtil.py` & `TinetApiRequest-1.1.1/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.0/tinet/RequestUtil.py` & `TinetApiRequest-1.1.1/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.0/tinet/SignUtil.py` & `TinetApiRequest-1.1.1/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.0/tinet/YamlUtil.py` & `TinetApiRequest-1.1.1/tinet/YamlUtil.py`

 * *Files identical despite different names*

