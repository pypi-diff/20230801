# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.946.tar", last modified: Mon Jul 31 00:26:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.947.tar", last modified: Tue Aug  1 00:48:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.946.tar` & `tencentcloud-sdk-python-faceid-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    34162 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)   212626 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-31 00:26:25.000000 tencentcloud-sdk-python-faceid-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    34162 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)   212767 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-08-01 00:48:41.000000 tencentcloud-sdk-python-faceid-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.946/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.947/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.946/setup.py` & `tencentcloud-sdk-python-faceid-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.946'
+__version__ = '3.0.947'
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.946/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.947/tencentcloud/faceid/v20180301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,16 @@
   '-13': '受限制的卡'
   '-14': '密码错误次数超限'
   '-15': '发卡行不支持此交易'
 不计费结果码：
   '-2': '姓名校验不通过'
   '-3': '银行卡号码有误'
   '-16': '验证中心服务繁忙'
+  '-17': '验证次数超限，请次日重试'
+
         :type Result: str
         :param _Description: 业务结果描述。
         :type Description: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Result = None
@@ -266,14 +268,15 @@
 '-17': '发卡行不支持此交易'
 不收费结果码：
 '-2': '姓名校验不通过'
 '-3': '身份证号码有误'
 '-4': '银行卡号码有误'
 '-5': '手机号码不合法'
 '-18': '验证中心服务繁忙'
+'-19': '验证次数超限，请次日重试'
         :type Result: str
         :param _Description: 业务结果描述。
         :type Description: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Result = None
@@ -419,14 +422,15 @@
 '-15': '密码错误次数超限'
 '-16': '发卡行不支持此交易'
 不收费结果码：
 '-2': '姓名校验不通过'
 '-3': '身份证号码有误'
 '-4': '银行卡号码有误'
 '-17': '验证中心服务繁忙'
+'-18': '验证次数超限，请次日重试'
         :type Result: str
         :param _Description: 业务结果描述。
         :type Description: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Result = None
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.947/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.946/README.rst` & `tencentcloud-sdk-python-faceid-3.0.947/README.rst`

 * *Files identical despite different names*

