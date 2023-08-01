# Comparing `tmp/TinetApiRequest-1.0.7.tar.gz` & `tmp/TinetApiRequest-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.0.7.tar", last modified: Tue Aug  1 07:53:54 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.0.8.tar", last modified: Tue Aug  1 08:01:13 2023, max compression
```

## Comparing `TinetApiRequest-1.0.7.tar` & `TinetApiRequest-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/
--rw-rw-rw-   0        0        0      272 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-08-01 07:53:47.000000 TinetApiRequest-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/tinet/
--rw-rw-rw-   0        0        0    23057 2023-08-01 07:53:30.000000 TinetApiRequest-1.0.7/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     7188 2023-08-01 06:49:58.000000 TinetApiRequest-1.0.7/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.7/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.0.7/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.7/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.7/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.7/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-08-01 08:01:09.000000 TinetApiRequest-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:01:13.000000 TinetApiRequest-1.0.8/tinet/
+-rw-rw-rw-   0        0        0    23081 2023-08-01 08:01:09.000000 TinetApiRequest-1.0.8/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     7188 2023-08-01 06:49:58.000000 TinetApiRequest-1.0.8/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.8/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.0.8/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.8/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.8/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.8/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.0.7/README.md` & `TinetApiRequest-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.7/setup.py` & `TinetApiRequest-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.0.7",
+    version="1.0.8",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.0.7/tinet/APIRequest.py` & `TinetApiRequest-1.0.8/tinet/APIRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
         yamlName = yaml.get('name')
         yamlKind = yaml.get('kind')
         yamlTestcase = yaml.get('testcases')
         # 先拿到所有testcase
         log.info(f"开始执行测试用例name: {yamlName}, id: {yamlId} , 测试用例: {yamlTestcase}")
         allure.attach(f"{yamlTestcase}", name=f"开始执行测试用例name: {yamlName}, id: {yamlId} ", attachment_type=allure.attachment_type.TEXT)
         # 添加公共session  判断是否有公共session
-        request = HttpClient()
+        clientSession = HttpClient()
         if config.session is not None:
-            request = config.session
+            clientSession = config.session
         # 开始遍历testcase
         # allure.dynamic.title(yamlName)
         for testcase in yamlTestcase:
             with allure.step(testcase.get('name')):
                 # 拿到用例如果是common的去common文件路径中拿测试用例
                 if testcase.get('skip'):  # 判断是否跳过
                     log.info(f"用例: {json.dumps(testcase.get('name'), indent=4, ensure_ascii=False)}跳过")
@@ -99,15 +99,15 @@
                     allure.attach(f"{jsonRequestParameter}", name=f"开始请求参数jsonRequestParameter", attachment_type=allure.attachment_type.TEXT)
                 if paramsData is not None:
                     log.info(f"开始请求参数paramsData: {paramsData}")
                     allure.attach(f"{paramsData}", name=f"开始请求参数paramsDatar", attachment_type=allure.attachment_type.TEXT)
                 # form-data请求 需要处理一下header
                 if dataRequestParameter is not None and requestType.lower() == 'form-data':
                     headers['Content-Type'] = dataRequestParameter.content_type
-                response = request.request(method=testcase.get('method'), url=requestUrl, data=dataRequestParameter, json=jsonRequestParameter, params=paramsData, headers=headers)
+                response = clientSession.request(method=testcase.get('method'), url=requestUrl, data=dataRequestParameter, json=jsonRequestParameter, params=paramsData, headers=headers)
                 try:  # 当返回不是 json 返回text
                     log.info(f"当前用例response: {json.dumps(response.json(), indent=4, ensure_ascii=False)}")
                     allure.attach(f"{json.dumps(response.json(), indent=4, ensure_ascii=False)}", name=f"当前用例response",
                                   attachment_type=allure.attachment_type.TEXT)
                 except:
                     log.info(f"当前用例response: {json.dumps(response.text, indent=4, ensure_ascii=False)}")
                     allure.attach(f"{json.dumps(response.text, indent=4, ensure_ascii=False)}", name=f"当前用例response",
@@ -120,15 +120,15 @@
                 self.assertType(testcase.get('assert'), response, dataSaveBean, failtype)
                 # 6. 处理response,根据data 来进行变量存取
                 # try 里面的代码是为了处理response不是json格式的情况
                 try:
                     self.addAttrSaveBean(dataSaveBean, self.globalBean, testcase.get('saveData'), response.json())
                 except:
                     self.addAttrSaveBean(dataSaveBean, self.globalBean, testcase.get('saveData'), response.text)
-        return request
+        return clientSession
 
     # 处理断言方法  - eq: [ 'body.userId', 1 ]  通过testcase中的assert来判断断言方式  先取断言的方式 再取断言的内容跟值
     def assertType(self, assertType, response, bean, failType):
         log.info(f"开始处理断言: {assertType}")
         allure.attach(f"{assertType}", name=f"开始处理断言", attachment_type=allure.attachment_type.TEXT)
         # 判断assertType是否为空
         if assertType is None:
```

### Comparing `TinetApiRequest-1.0.7/tinet/ApiConfig.py` & `TinetApiRequest-1.0.8/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.7/tinet/LogUtil.py` & `TinetApiRequest-1.0.8/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.7/tinet/RequestUtil.py` & `TinetApiRequest-1.0.8/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.7/tinet/SignUtil.py` & `TinetApiRequest-1.0.8/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.7/tinet/YamlUtil.py` & `TinetApiRequest-1.0.8/tinet/YamlUtil.py`

 * *Files identical despite different names*

