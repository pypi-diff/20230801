# Comparing `tmp/TinetApiRequest-1.0.4.tar.gz` & `tmp/TinetApiRequest-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.0.4.tar", last modified: Tue Aug  1 06:40:29 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.0.5.tar", last modified: Tue Aug  1 07:29:28 2023, max compression
```

## Comparing `TinetApiRequest-1.0.4.tar` & `TinetApiRequest-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/
--rw-rw-rw-   0        0        0      272 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 06:40:28.000000 TinetApiRequest-1.0.4/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-08-01 06:33:02.000000 TinetApiRequest-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 06:40:29.000000 TinetApiRequest-1.0.4/tinet/
--rw-rw-rw-   0        0        0    22415 2023-08-01 06:40:22.000000 TinetApiRequest-1.0.4/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     7184 2023-08-01 06:36:16.000000 TinetApiRequest-1.0.4/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.4/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     3501 2023-08-01 03:14:37.000000 TinetApiRequest-1.0.4/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.4/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.4/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.4/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/
+-rw-rw-rw-   0        0        0      272 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3922 2023-08-01 07:06:19.000000 TinetApiRequest-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-08-01 07:07:09.000000 TinetApiRequest-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:29:28.000000 TinetApiRequest-1.0.5/tinet/
+-rw-rw-rw-   0        0        0    23048 2023-08-01 07:09:46.000000 TinetApiRequest-1.0.5/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     7188 2023-08-01 06:49:58.000000 TinetApiRequest-1.0.5/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.5/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3501 2023-08-01 03:14:37.000000 TinetApiRequest-1.0.5/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.5/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.5/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.5/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.0.4/README.md` & `TinetApiRequest-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,21 +85,23 @@
     parameter: # 请求参数 '#{}'取FAKER模拟数据方法   '${}' 取缓存变量  # todo '$${}' 取global变量  todo 方法传参数
       offset: 0
       limit: '#{get_sk_password}'  # 获取环境变量里 SK 加密密码
       cno: '#{random_number(args)}' # 生成随机数
       name: '[${queues}]'
       names: '$${names}'
     assertFail: stop、continue  # 断言失败处理模式 stop程序直接终止 continue断言失败仍运行。默认为stop
-    assert: # 断言 eq sge # todo 支持多个断言 eq  ne gt lt  ge le seq sne sgt slt sge sle
+    assert: # 断言 eq sge # todo 支持多个断言 eq  ne gt lt  ge le seq sne sgt slt sge sle in
       - status_code: 201
       - eq: [ '$.pageSize', '${size}' ]
       - eq: [ '$.pageSize', '$${size}' ]
       - sge: [ '$.queues[:2].id', 2 ]
-      - none : ['$.error']
-      - nn: ['$.error']
+      - none : ['$.error']   # 判断 返回值 是否为空
+      - nn: ['$.error']      # 判断 返回值 是否不为空
+      - in: ['$.pageSize', '$${size}'] # 判断 返回值 是否包含 预期
+      - in: [ '$.pageSize', '${size}' ]
     saveData: # 缓存变量  global变量 #todo cookie变量 header变量  request变量
       - json: [ 'queues','$.queues[:2].id' ]
       - json: [ 'names','$.name' ,'global']
 
 
   - name: 创建座席
     id: create_client
```

### Comparing `TinetApiRequest-1.0.4/setup.py` & `TinetApiRequest-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.0.4",
+    version="1.0.5",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.0.4/tinet/APIRequest.py` & `TinetApiRequest-1.0.5/tinet/APIRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,21 @@
                                   f"not none断言失败: {ass.get('nn')[0]}  ,jsonpath结果: {jsonpathResults}", failType)
             elif 'none' in ass:
                 # 判断json path 是否 返回FALSE
                 log.info(f"断言none结束: {jsonpathResults}")
                 allure.attach(f" {jsonpathResults} ", name=f"断言none结束", attachment_type=allure.attachment_type.TEXT)
                 self.assertChoose(jsonpathResults is True,
                                   f"none断言失败: {ass.get('none')[0]}  ,jsonpath结果: {jsonpathResults}", failType)
+            elif 'in' in ass:
+                # 判断预期值是否被返回值包含
+                expectedResults = PlaceholderYaml(attrObj=bean, reString=ass.get('in')[1]).replace().replaced_str
+                log.info(f"断言in结束: {expectedResults} 在 {jsonpathResults} 内")
+                allure.attach(f" {expectedResults} 在 {jsonpathResults} 内", name=f"断言in结束",
+                              attachment_type=allure.attachment_type.TEXT)
+                self.assertChoose(str(expectedResults) in str(jsonpathResults), f"断言in失败: {expectedResults} 不在 {jsonpathResults} 内", failType)
 
     # 根据data从response中根据json还是其他方法来获取response中的值
     def addAttrSaveBean(self, bean, globalBean, data: list, response):
         # 先解析data 如果data为空则直接返回
         if data is None:
             return
         for d in data:
```

### Comparing `TinetApiRequest-1.0.4/tinet/ApiConfig.py` & `TinetApiRequest-1.0.5/tinet/ApiConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         """
         num = str(random.randint(1000, 9999))
         src_uppercase = string.ascii_uppercase  # string_大写字母
         src_lowercase = string.ascii_lowercase  # string_小写字母
         chrs = random.sample(src_lowercase + src_uppercase, 3)
         for i in chrs:
             num += i
-        return
+        return num
 
     def encryptPassword(self, plain_text='Aa112233'):
         """
         # 加密
         """
         password = config.accessKeySecret
         # 设置随机数生成器的种子
```

### Comparing `TinetApiRequest-1.0.4/tinet/LogUtil.py` & `TinetApiRequest-1.0.5/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.4/tinet/RequestUtil.py` & `TinetApiRequest-1.0.5/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.4/tinet/SignUtil.py` & `TinetApiRequest-1.0.5/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.4/tinet/YamlUtil.py` & `TinetApiRequest-1.0.5/tinet/YamlUtil.py`

 * *Files identical despite different names*

