# Comparing `tmp/TinetApiRequest-1.1.3.tar.gz` & `tmp/TinetApiRequest-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.1.3.tar", last modified: Tue Aug  1 08:43:11 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.1.4.tar", last modified: Tue Aug  1 08:57:06 2023, max compression
```

## Comparing `TinetApiRequest-1.1.3.tar` & `TinetApiRequest-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/
--rw-rw-rw-   0        0        0      272 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-08-01 08:43:10.000000 TinetApiRequest-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:43:11.000000 TinetApiRequest-1.1.3/tinet/
--rw-rw-rw-   0        0        0    23046 2023-08-01 08:43:10.000000 TinetApiRequest-1.1.3/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     7199 2023-08-01 08:43:10.000000 TinetApiRequest-1.1.3/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.1.3/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.1.3/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.1.3/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.1.3/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.1.3/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-08-01 08:57:05.000000 TinetApiRequest-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:57:06.000000 TinetApiRequest-1.1.4/tinet/
+-rw-rw-rw-   0        0        0    22997 2023-08-01 08:57:05.000000 TinetApiRequest-1.1.4/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     7199 2023-08-01 08:43:10.000000 TinetApiRequest-1.1.4/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.1.4/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.1.4/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.1.4/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.1.4/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      237 2023-08-01 08:57:05.000000 TinetApiRequest-1.1.4/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.1.3/README.md` & `TinetApiRequest-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.3/setup.py` & `TinetApiRequest-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.1.3",
+    version="1.1.4",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.1.3/tinet/APIRequest.py` & `TinetApiRequest-1.1.4/tinet/APIRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         """
         self.commonCase = commonCase
         self.baseUrl = config.baseUrl
         self.AccessKeyId = config.accessKeyId
         self.AccessKeySecret = config.accessKeySecret
         self.globalBean = config
         self.assertFail = config.assertFail
-        self.clientSession = config.Session
 
     # 请求核心方法, 拿到文件后开始解析
     def doRequest(self, file, bean):
         # 请求的时候最终参数  先替换parameter中的占位符  再判断鉴权方式,如果是SIGN的POST就完整parameter否则GET就为空
         requestParameter = None
         dataSaveBean = bean
         yaml = ReadYaml(file).load_yaml()
@@ -47,15 +46,15 @@
         yamlName = yaml.get('name')
         yamlKind = yaml.get('kind')
         yamlTestcase = yaml.get('testcases')
         # 先拿到所有testcase
         log.info(f"开始执行测试用例name: {yamlName}, id: {yamlId} , 测试用例: {yamlTestcase}")
         allure.attach(f"{yamlTestcase}", name=f"开始执行测试用例name: {yamlName}, id: {yamlId} ", attachment_type=allure.attachment_type.TEXT)
         # 添加公共session  判断是否有公共session
-        clientSession = self.clientSession
+        clientSession = config.Session
         # 开始遍历testcase
         # allure.dynamic.title(yamlName)
         for testcase in yamlTestcase:
             with allure.step(testcase.get('name')):
                 # 拿到用例如果是common的去common文件路径中拿测试用例
                 if testcase.get('skip'):  # 判断是否跳过
                     log.info(f"用例: {json.dumps(testcase.get('name'), indent=4, ensure_ascii=False)}跳过")
```

### Comparing `TinetApiRequest-1.1.3/tinet/ApiConfig.py` & `TinetApiRequest-1.1.4/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.3/tinet/LogUtil.py` & `TinetApiRequest-1.1.4/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.3/tinet/RequestUtil.py` & `TinetApiRequest-1.1.4/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.3/tinet/SignUtil.py` & `TinetApiRequest-1.1.4/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.1.3/tinet/YamlUtil.py` & `TinetApiRequest-1.1.4/tinet/YamlUtil.py`

 * *Files identical despite different names*

