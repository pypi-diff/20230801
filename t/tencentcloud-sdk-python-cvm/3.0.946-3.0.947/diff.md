# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.946.tar", last modified: Mon Jul 31 00:23:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.947.tar", last modified: Tue Aug  1 00:35:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.946.tar` & `tencentcloud-sdk-python-cvm-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44311 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   119676 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)   624916 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:23:49.000000 tencentcloud-sdk-python-cvm-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44911 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   119676 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)   624916 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:35:00.000000 tencentcloud-sdk-python-cvm-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.946/setup.py` & `tencentcloud-sdk-python-cvm-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.946/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.947/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,17 @@
 
 # 镜像被其他操作占用，请检查，并稍后重试。
 INVALIDPARAMETERVALUE_INVALIDIMAGESTATE = 'InvalidParameterValue.InvalidImageState'
 
 # 该实例配置来自免费升配活动，暂不支持3个月内进行降配。
 INVALIDPARAMETERVALUE_INVALIDINSTANCESOURCE = 'InvalidParameterValue.InvalidInstanceSource'
 
+# 指定机型不支持包销付费模式。
+INVALIDPARAMETERVALUE_INVALIDINSTANCETYPEUNDERWRITE = 'InvalidParameterValue.InvalidInstanceTypeUnderwrite'
+
 # IP地址不符合规范
 INVALIDPARAMETERVALUE_INVALIDIPFORMAT = 'InvalidParameterValue.InvalidIpFormat'
 
 # 实例启动模板描述格式错误。
 INVALIDPARAMETERVALUE_INVALIDLAUNCHTEMPLATEDESCRIPTION = 'InvalidParameterValue.InvalidLaunchTemplateDescription'
 
 # 实例启动模板名称格式错误。
@@ -811,14 +814,17 @@
 
 # 中心可用区和边缘可用区实例不能混用批量操作。
 UNSUPPORTEDOPERATION_INSTANCEMIXEDZONETYPE = 'UnsupportedOperation.InstanceMixedZoneType'
 
 # 请求不支持操作系统为`Xserver windows2012cndatacenterx86_64`的实例`ins-xxxxxx` 。
 UNSUPPORTEDOPERATION_INSTANCEOSWINDOWS = 'UnsupportedOperation.InstanceOsWindows'
 
+# 当前实例为重装系统失败状态，不支持此操作；推荐您再次重装系统，也可以销毁/退还实例或提交工单
+UNSUPPORTEDOPERATION_INSTANCEREINSTALLFAILED = 'UnsupportedOperation.InstanceReinstallFailed'
+
 # 该子机处于封禁状态，请联系相关人员处理。
 UNSUPPORTEDOPERATION_INSTANCESTATEBANNING = 'UnsupportedOperation.InstanceStateBanning'
 
 # 请求不支持永久故障的实例。
 UNSUPPORTEDOPERATION_INSTANCESTATECORRUPTED = 'UnsupportedOperation.InstanceStateCorrupted'
 
 # 请求不支持进入救援模式的实例
@@ -994,14 +1000,17 @@
 
 # 不支持关机不收费机器做同类型变配操作。
 UNSUPPORTEDOPERATION_STOPPEDMODESTOPCHARGINGSAMEFAMILY = 'UnsupportedOperation.StoppedModeStopChargingSameFamily'
 
 # 请求不支持该类型系统盘。
 UNSUPPORTEDOPERATION_SYSTEMDISKTYPE = 'UnsupportedOperation.SystemDiskType'
 
+# 包月转包销，不支持包销折扣高于现有包年包月折扣。
+UNSUPPORTEDOPERATION_UNDERWRITEDISCOUNTGREATERTHANPREPAIDDISCOUNT = 'UnsupportedOperation.UnderwriteDiscountGreaterThanPrepaidDiscount'
+
 # 该机型为包销机型，RenewFlag的值只允许设置为NOTIFY_AND_AUTO_RENEW。
 UNSUPPORTEDOPERATION_UNDERWRITINGINSTANCETYPEONLYSUPPORTAUTORENEW = 'UnsupportedOperation.UnderwritingInstanceTypeOnlySupportAutoRenew'
 
 # 当前实例不允许变配到非ARM机型。
 UNSUPPORTEDOPERATION_UNSUPPORTEDARMCHANGEINSTANCEFAMILY = 'UnsupportedOperation.UnsupportedARMChangeInstanceFamily'
 
 # 指定机型不支持跨机型调整配置。
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.946/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.947/tencentcloud/cvm/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.947/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.946/README.rst` & `tencentcloud-sdk-python-cvm-3.0.947/README.rst`

 * *Files identical despite different names*

