# Comparing `tmp/TinetApiRequest-1.0.6.tar.gz` & `tmp/TinetApiRequest-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.0.6.tar", last modified: Tue Aug  1 07:50:23 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.0.7.tar", last modified: Tue Aug  1 07:53:54 2023, max compression
```

## Comparing `TinetApiRequest-1.0.6.tar` & `TinetApiRequest-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/
--rw-rw-rw-   0        0        0      272 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-08-01 07:36:37.000000 TinetApiRequest-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 07:50:23.000000 TinetApiRequest-1.0.6/tinet/
--rw-rw-rw-   0        0        0    23072 2023-08-01 07:46:44.000000 TinetApiRequest-1.0.6/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     7188 2023-08-01 06:49:58.000000 TinetApiRequest-1.0.6/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.6/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.0.6/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.6/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.6/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.6/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/
+-rw-rw-rw-   0        0        0      272 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4032 2023-08-01 07:46:44.000000 TinetApiRequest-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-08-01 07:53:47.000000 TinetApiRequest-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:53:54.000000 TinetApiRequest-1.0.7/tinet/
+-rw-rw-rw-   0        0        0    23057 2023-08-01 07:53:30.000000 TinetApiRequest-1.0.7/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     7188 2023-08-01 06:49:58.000000 TinetApiRequest-1.0.7/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.7/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3501 2023-08-01 07:45:55.000000 TinetApiRequest-1.0.7/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.7/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.7/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.7/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.0.6/README.md` & `TinetApiRequest-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.6/setup.py` & `TinetApiRequest-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.0.6",
+    version="1.0.7",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.0.6/tinet/APIRequest.py` & `TinetApiRequest-1.0.7/tinet/APIRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,16 @@
         yamlName = yaml.get('name')
         yamlKind = yaml.get('kind')
         yamlTestcase = yaml.get('testcases')
         # 先拿到所有testcase
         log.info(f"开始执行测试用例name: {yamlName}, id: {yamlId} , 测试用例: {yamlTestcase}")
         allure.attach(f"{yamlTestcase}", name=f"开始执行测试用例name: {yamlName}, id: {yamlId} ", attachment_type=allure.attachment_type.TEXT)
         # 添加公共session  判断是否有公共session
-        if config.session is None:
-            request = HttpClient()
-        else:
+        request = HttpClient()
+        if config.session is not None:
             request = config.session
         # 开始遍历testcase
         # allure.dynamic.title(yamlName)
         for testcase in yamlTestcase:
             with allure.step(testcase.get('name')):
                 # 拿到用例如果是common的去common文件路径中拿测试用例
                 if testcase.get('skip'):  # 判断是否跳过
```

### Comparing `TinetApiRequest-1.0.6/tinet/ApiConfig.py` & `TinetApiRequest-1.0.7/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.6/tinet/LogUtil.py` & `TinetApiRequest-1.0.7/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.6/tinet/RequestUtil.py` & `TinetApiRequest-1.0.7/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.6/tinet/SignUtil.py` & `TinetApiRequest-1.0.7/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.6/tinet/YamlUtil.py` & `TinetApiRequest-1.0.7/tinet/YamlUtil.py`

 * *Files identical despite different names*

