# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.946.tar", last modified: Mon Jul 31 00:18:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.947.tar", last modified: Tue Aug  1 00:19:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.946.tar` & `tencentcloud-sdk-python-apigateway-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21197 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   644386 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)    95541 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-31 00:18:53.000000 tencentcloud-sdk-python-apigateway-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21714 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   644386 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)    95541 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-08-01 00:19:05.000000 tencentcloud-sdk-python-apigateway-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,20 @@
 
 # api类错误。
 FAILEDOPERATION_APIERROR = 'FailedOperation.ApiError'
 
 # 当前API正在操作中，请稍后再试。
 FAILEDOPERATION_APIINOPERATION = 'FailedOperation.ApiInOperation'
 
+# 返回域名错误
+FAILEDOPERATION_BACKENDDOMAINERROR = 'FailedOperation.BackendDomainError'
+
+# CAM异常
+FAILEDOPERATION_CAMEXCEPTION = 'FailedOperation.CamException'
+
 # 证书绑定错误。
 FAILEDOPERATION_CERTIFICATEIDBINDERROR = 'FailedOperation.CertificateIdBindError'
 
 # 该证书为企业证书，待提交。
 FAILEDOPERATION_CERTIFICATEIDENTERPRISEWAITSUBMIT = 'FailedOperation.CertificateIdEnterpriseWaitSubmit'
 
 # 证书不存在或者您没有权限查看，请在ssl证书管理平台上传有效证书。
@@ -172,14 +178,17 @@
 
 # CLB内部请求错误，请稍后重试。若无法解决，请联系智能客服或提交工单。
 INTERNALERROR_CLBEXCEPTION = 'InternalError.ClbException'
 
 # oss内部请求错误，请稍后重试。若无法解决，请联系智能客服或提交工单。
 INTERNALERROR_OSSEXCEPTION = 'InternalError.OssException'
 
+# 标签回调失败。
+INTERNALERROR_RETURNABLEEXCEPTION = 'InternalError.ReturnableException'
+
 # SCF内部请求错误，请稍后重试。若无法解决，请联系智能客服或提交工单。
 INTERNALERROR_SCFEXCEPTION = 'InternalError.ScfException'
 
 # TSF内部请求错误，请稍后重试。若无法解决，请联系智能客服或提交工单。
 INTERNALERROR_TSFEXCEPTION = 'InternalError.TsfException'
 
 # vpc内部请求错误，请稍后重试。若无法解决，请联系智能客服或提交工单。
@@ -451,14 +460,17 @@
 
 # 当前插件不支持绑定。
 UNSUPPORTEDOPERATION_ATTACHPLUGIN = 'UnsupportedOperation.AttachPlugin'
 
 # 基础版服务不能创建超过一个API。
 UNSUPPORTEDOPERATION_BASICSERVICENOMOREAPI = 'UnsupportedOperation.BasicServiceNoMoreApi'
 
+# 基础服务不允许连接插件
+UNSUPPORTEDOPERATION_BASICSERVICENOTALLOWATTACHPLUGIN = 'UnsupportedOperation.BasicServiceNotAllowAttachPlugin'
+
 # 日志检索起始时间间隔。
 UNSUPPORTEDOPERATION_CLSSEARCHTIME = 'UnsupportedOperation.ClsSearchTime'
 
 # 存在现网环境
 UNSUPPORTEDOPERATION_EXISTINGONLINEENVIRONMENT = 'UnsupportedOperation.ExistingOnlineEnvironment'
 
 # 协议为HTTP时，不支持强制Https。
@@ -490,14 +502,17 @@
 
 # 当前使用计划未绑定环境。
 UNSUPPORTEDOPERATION_NOUSAGEPLANENV = 'UnsupportedOperation.NoUsagePlanEnv'
 
 # 不支持减少网络类型的操作。
 UNSUPPORTEDOPERATION_REDUCENETTYPES = 'UnsupportedOperation.ReduceNetTypes'
 
+# 请求Post失败
+UNSUPPORTEDOPERATION_REQUESTPOSTERROR = 'UnsupportedOperation.RequestPostError'
+
 # 资源已关联，请先解除。
 UNSUPPORTEDOPERATION_RESOURCEASSOCIATED = 'UnsupportedOperation.ResourceAssociated'
 
 # 密钥已绑定使用计划，请先解绑再试。
 UNSUPPORTEDOPERATION_RESOURCEISINUSE = 'UnsupportedOperation.ResourceIsInUse'
 
 # 资源未关联。
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.947/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.947/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.946/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.947/README.rst`

 * *Files identical despite different names*

