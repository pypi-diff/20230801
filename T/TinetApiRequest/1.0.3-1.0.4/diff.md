# Comparing `tmp/TinetApiRequest-1.0.3.tar.gz` & `tmp/TinetApiRequest-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.0.3.tar", last modified: Tue Jul 25 06:18:11 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.0.4.tar", last modified: Tue Aug  1 06:40:29 2023, max compression
```

## Comparing `TinetApiRequest-1.0.3.tar` & `TinetApiRequest-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/
--rw-rw-rw-   0        0        0      272 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-07-25 06:18:06.000000 TinetApiRequest-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/tinet/
--rw-rw-rw-   0        0        0    22254 2023-07-25 06:11:50.000000 TinetApiRequest-1.0.3/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-1.0.3/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.3/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     3479 2023-07-20 12:03:44.000000 TinetApiRequest-1.0.3/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.3/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.3/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.3/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/
+-rw-rw-rw-   0        0        0      272 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-08-01 06:33:02.000000 TinetApiRequest-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/tinet/
+-rw-rw-rw-   0        0        0    22415 2023-08-01 06:40:22.000000 TinetApiRequest-1.0.4/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     7184 2023-08-01 06:36:16.000000 TinetApiRequest-1.0.4/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.4/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3501 2023-08-01 03:14:37.000000 TinetApiRequest-1.0.4/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.4/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.4/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.4/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.0.3/README.md` & `TinetApiRequest-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.3/setup.py` & `TinetApiRequest-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.0.3",
+    version="1.0.4",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.0.3/tinet/APIRequest.py` & `TinetApiRequest-1.0.4/tinet/APIRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,19 @@
         yamlId = yaml.get('id')
         yamlName = yaml.get('name')
         yamlKind = yaml.get('kind')
         yamlTestcase = yaml.get('testcases')
         # 先拿到所有testcase
         log.info(f"开始执行测试用例name: {yamlName}, id: {yamlId} , 测试用例: {yamlTestcase}")
         allure.attach(f"{yamlTestcase}", name=f"开始执行测试用例name: {yamlName}, id: {yamlId} ", attachment_type=allure.attachment_type.TEXT)
-        request = HttpClient()  # todo 定制化接口HttpClient
+        # 添加公共session  判断是否有公共session
+        if config.session is None:
+            request = HttpClient()
+        else:
+            request = config.session
         # 开始遍历testcase
         # allure.dynamic.title(yamlName)
         for testcase in yamlTestcase:
             with allure.step(testcase.get('name')):
                 # 拿到用例如果是common的去common文件路径中拿测试用例
                 if testcase.get('skip'):  # 判断是否跳过
                     log.info(f"用例: {json.dumps(testcase.get('name'), indent=4, ensure_ascii=False)}跳过")
@@ -74,14 +78,15 @@
                 # 执行当前用例 格式化为json 间隔4个空格
                 log.info(f"执行当前用例name: {testcase.get('name')}, id: {testcase.get('id')}")
                 allure.attach(f"{json.dumps(testcase, indent=4, ensure_ascii=False)}", name=f"执行当前用例name: {testcase.get('name')}, id: {testcase.get('id')}",
                               attachment_type=allure.attachment_type.TEXT)
                 # 1. 先看看参数中是否有需要替换的参数
                 repParameter = self.replaceParameterAttr(dataSaveBean, testcase.get('parameter'))
                 repApi = self.replaceParameterAttr(dataSaveBean, testcase.get('api'))
+                headers = self.replaceParameterAttr(dataSaveBean, testcase.get('headers'))
                 # 2. 判断鉴权方式 authType 返回请求地址
                 requestParameter, requestUrl = self.authType(testcase.get('authType'), repApi, testcase.get('method'), repParameter)
                 # 3. 判断请求 requestType
                 dataRequestParameter, jsonRequestParameter, paramsData, requestType = self.requestType(testcase.get('requestType'), requestParameter)
                 # 4. 开始请求
                 log.info(f"开始请求地址: {requestUrl} ")
                 allure.attach(f"{requestUrl}", name=f"开始请求地址", attachment_type=allure.attachment_type.TEXT)
@@ -93,15 +98,14 @@
                 if jsonRequestParameter is not None:
                     log.info(f"开始请求参数jsonRequestParameter: {jsonRequestParameter}")
                     allure.attach(f"{jsonRequestParameter}", name=f"开始请求参数jsonRequestParameter", attachment_type=allure.attachment_type.TEXT)
                 if paramsData is not None:
                     log.info(f"开始请求参数paramsData: {paramsData}")
                     allure.attach(f"{paramsData}", name=f"开始请求参数paramsDatar", attachment_type=allure.attachment_type.TEXT)
                 # form-data请求 需要处理一下header
-                headers = testcase.get('headers')
                 if dataRequestParameter is not None and requestType.lower() == 'form-data':
                     headers['Content-Type'] = dataRequestParameter.content_type
                 response = request.request(method=testcase.get('method'), url=requestUrl, data=dataRequestParameter, json=jsonRequestParameter, params=paramsData, headers=headers)
                 try:  # 当返回不是 json 返回text
                     log.info(f"当前用例response: {json.dumps(response.json(), indent=4, ensure_ascii=False)}")
                     allure.attach(f"{json.dumps(response.json(), indent=4, ensure_ascii=False)}", name=f"当前用例response",
                                   attachment_type=allure.attachment_type.TEXT)
```

### Comparing `TinetApiRequest-1.0.3/tinet/ApiConfig.py` & `TinetApiRequest-1.0.4/tinet/ApiConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import random
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
 import datetime
 import pytz
 import hashlib
 import base64
-
+from requests import Session
 
 
 class times:
     def __init__(self, dt=None, tz=pytz.timezone('Asia/Shanghai')):
         """
         初始化时间工具类
 
@@ -161,26 +161,36 @@
 
 
 class config:
     """
     配置文件
     """
 
-    def __init__(self, baseUrl=None, AccessKeyId=None, AccessKeySecret=None, SKPassword=None, commonTestCasePath=None, methObj=None, assertFail='stop'):
+    def __init__(self, baseUrl=None, AccessKeyId=None, AccessKeySecret=None, SKPassword=None, commonTestCasePath=None, methObj=None, assertFail='stop', session: Session = None):
         """
         初始化配置文件
         """
         self._baseUrl = baseUrl
         self._accessKeyId = AccessKeyId
         self._accessKeySecret = AccessKeySecret
         # SK加密 登录密码 后的 密码加密文本
         self._SKPassword = SKPassword
         self._commonTestCasePath = commonTestCasePath
         self._methObj = methObj
         self._assertFail = assertFail
+        # 构建全局session
+        self._session = session
+
+    @property
+    def session(self):
+        return self._session
+
+    @session.setter
+    def session(self, value):
+        self._session = value
 
     @property
     def methObj(self):
         return self._methObj
 
     @methObj.setter
     def methObj(self, value):
```

### Comparing `TinetApiRequest-1.0.3/tinet/LogUtil.py` & `TinetApiRequest-1.0.4/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.3/tinet/RequestUtil.py` & `TinetApiRequest-1.0.4/tinet/RequestUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         :param url: str 请求 URL，会和 base_url 拼接成完整的 URL。
         :param kwargs: dict 其他 requests.request 方法支持的参数。
         :return: requests.Response 响应对象。
         """
 
         response = self.session.request(method, url, **kwargs)
         # 判断请求url 是否包含 openapi_login  用于处理 单点登录到系统后进行系统的接口请求鉴权处理
-        if 'openapi_login' in url:
-            # 需要请求接口 获取 Tsessionid
-            # 先从url 中解析出请求域名
-            parsed_url = urlparse(url)
-            domain = parsed_url.scheme + '://' + parsed_url.netloc
-            # 进行接口请求 拿到响应
-            personalResponse = self.session.request(method='GET', url=domain + '/api/personal/info/get')
-            # 拿响应的$.result.authToken
-            authToken = jsonpath.jsonpath(personalResponse.json(), '$.result.authToken')[0]
-            # 后续的请求头上都需要带上 Tsessionid
-            self.session.headers.update({'Tsessionid': authToken})
+        # if 'openapi_login' in url:
+        #     # 需要请求接口 获取 Tsessionid
+        #     # 先从url 中解析出请求域名
+        #     parsed_url = urlparse(url)
+        #     domain = parsed_url.scheme + '://' + parsed_url.netloc
+        #     # 进行接口请求 拿到响应
+        #     personalResponse = self.session.request(method='GET', url=domain + '/api/personal/info/get')
+        #     # 拿响应的$.result.authToken
+        #     authToken = jsonpath.jsonpath(personalResponse.json(), '$.result.authToken')[0]
+        #     # 后续的请求头上都需要带上 Tsessionid
+        #     self.session.headers.update({'Tsessionid': authToken})
 
 
         http_error_msg = None
         if 400 <= response.status_code < 500:
             http_error_msg = (
                 f"{response.status_code} 客户端错误 Error: {response.text} for url: {response.url}"
             )
```

### Comparing `TinetApiRequest-1.0.3/tinet/SignUtil.py` & `TinetApiRequest-1.0.4/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.3/tinet/YamlUtil.py` & `TinetApiRequest-1.0.4/tinet/YamlUtil.py`

 * *Files identical despite different names*

