# Comparing `tmp/tencentcloud-sdk-python-ms-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-ms-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.946.tar", last modified: Mon Jul 31 00:32:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.947.tar", last modified: Tue Aug  1 00:52:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ms-3.0.946.tar` & `tencentcloud-sdk-python-ms-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud_sdk_python_ms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud_sdk_python_ms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/v20180408/
--rw-r--r--   0 root         (0) root         (0)    21305 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/v20180408/ms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5901 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   169826 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-31 00:32:39.000000 tencentcloud-sdk-python-ms-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    21299 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/ms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5911 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   169759 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-08-01 00:52:42.000000 tencentcloud-sdk-python-ms-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-01 00:52:41.000000 tencentcloud-sdk-python-ms-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-ms-3.0.946/tencentcloud_sdk_python_ms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.947/tencentcloud_sdk_python_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.946/setup.py` & `tencentcloud-sdk-python-ms-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/v20180408/ms_client.py` & `tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/ms_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateOrderInstance(self, request):
         """该接口供渠道合作应用加固使用，接口调用有白名单用户限制。
         订单类型有：免费试用、按年收费、按次收费。
-        应用加固支持的平台类型有：android安卓加固 、ios源码混淆 、sdk加固、applet小程序加固。
+        应用加固支持的平台类型有：android加固 、ios源码混淆 、sdk加固、applet小程序加固。
 
         :param request: Request instance for CreateOrderInstance.
         :type request: :class:`tencentcloud.ms.v20180408.models.CreateOrderInstanceRequest`
         :rtype: :class:`tencentcloud.ms.v20180408.models.CreateOrderInstanceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/v20180408/errorcodes.py` & `tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/errorcodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,51 +43,51 @@
 
 # 不能找到指定的加固策略。
 INVALIDPARAMETER_PLANIDNOTFOUND = 'InvalidParameter.PlanIdNotFound'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
-# 安卓在线加固任务,入参字段AppMd5必输。
+# Android在线加固任务,入参字段AppMd5必输。
 INVALIDPARAMETERVALUE_ANDROIDAPPMD5ERROR = 'InvalidParameterValue.AndroidAppMd5Error'
 
-# 安卓应用包名必输,请求参数中的AppPkgName值要相等。
+# Android应用包名必输,请求参数中的AppPkgName值要相等。
 INVALIDPARAMETERVALUE_ANDROIDAPPPKGNAMEERROR = 'InvalidParameterValue.AndroidAppPkgNameError'
 
 # AppPkgNameList字段检查不通过，必输字段，值可为单个包年或多个包名时。值为多个包名时，包名需用逗号隔开，其数量不能超过10个。
 INVALIDPARAMETERVALUE_ANDROIDAPPPKGNAMELISTERROR = 'InvalidParameterValue.AndroidAppPkgNameListError'
 
-# 安卓应用类型必输,请求参数中的AppType值要相等，其值需等于“apk”或“aab”。
+# Android应用类型必输,请求参数中的AppType值要相等，其值需等于“apk”或“aab”。
 INVALIDPARAMETERVALUE_ANDROIDAPPTYPEERROR = 'InvalidParameterValue.AndroidAppTypeError'
 
-# 安卓在线加固任务,入参字段AppUrl必输。
+# Android在线加固任务,入参字段AppUrl必输。
 INVALIDPARAMETERVALUE_ANDROIDAPPURLERROR = 'InvalidParameterValue.AndroidAppUrlError'
 
-# 安卓加固配置错误,assets资源文件路径格式错误。
+# Android加固配置错误,assets资源文件路径格式错误。
 INVALIDPARAMETERVALUE_ANDROIDASSETSERROR = 'InvalidParameterValue.AndroidAssetsError'
 
-# 安卓加固配置参数不正确
+# Android加固配置参数不正确
 INVALIDPARAMETERVALUE_ANDROIDENCRYPTPARAMERROR = 'InvalidParameterValue.AndroidEncryptParamError'
 
-# 安卓加固配置错误,res资源文件路径格式错误。
+# Android加固配置错误,res资源文件路径格式错误。
 INVALIDPARAMETERVALUE_ANDROIDRESERROR = 'InvalidParameterValue.AndroidResError'
 
-# 安卓加固配置错误,so库文件路径格式错误。
+# Android加固配置错误,so库文件路径格式错误。
 INVALIDPARAMETERVALUE_ANDROIDSOERROR = 'InvalidParameterValue.AndroidSoError'
 
-# 安卓加固配置错误,vmp加固profile文件必输
+# Android加固配置错误,vmp加固profile文件必输
 INVALIDPARAMETERVALUE_ANDROIDVMPERROR = 'InvalidParameterValue.AndroidVMPError'
 
 # 小程序加固配置错误,请检查相关配置。
 INVALIDPARAMETERVALUE_APPLETENCRYPTPARAMERROR = 'InvalidParameterValue.AppletEncryptParamError'
 
 # 请求参数中值为Url下载链接的相关字段检查不通过。
 INVALIDPARAMETERVALUE_CHECKURLERROR = 'InvalidParameterValue.CheckUrlError'
 
-# 安卓加固配置错误,入参字段AppType必输。
+# Android加固配置错误,入参字段AppType必输。
 INVALIDPARAMETERVALUE_ENCRYPTPARAMAPPTYPEERROR = 'InvalidParameterValue.EncryptParamAppTypeError'
 
 # 不能同时指定ItemIds和Filters。
 INVALIDPARAMETERVALUE_INVALIDCOEXISTITEMIDSFILTERS = 'InvalidParameterValue.InvalidCoexistItemIdsFilters'
 
 # 无效的过滤器。
 INVALIDPARAMETERVALUE_INVALIDFILTER = 'InvalidParameterValue.InvalidFilter'
```

### Comparing `tencentcloud-sdk-python-ms-3.0.946/tencentcloud/ms/v20180408/models.py` & `tencentcloud-sdk-python-ms-3.0.947/tencentcloud/ms/v20180408/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
 class AndroidAppInfo(AbstractModel):
-    """渠道合作安卓加固App信息
+    """渠道合作Android加固App信息
 
     """
 
     def __init__(self):
         r"""
         :param _AppMd5: app文件的md5算法值，需要正确传递，在线加固必输。
 例如linux环境下执行算法命令md5sum ：
@@ -33,22 +33,22 @@
         :param _AppSize: app的大小，非必输。
         :type AppSize: int
         :param _AppUrl: app下载链接，在线加固必输。
         :type AppUrl: str
         :param _AppName: app名称，非必输
         :type AppName: str
         :param _AppPkgName: app的包名，本次操作的包名。
-当安卓是按年收费、免费试用加固时，在线加固和输出工具要求该字段必输，且与AndroidPlan.AppPkgName值相等。
+当Android是按年收费、免费试用加固时，在线加固和输出工具要求该字段必输，且与AndroidPlan.AppPkgName值相等。
         :type AppPkgName: str
         :param _AppFileName: app的文件名，非必输。
         :type AppFileName: str
         :param _AppVersion: app版本号，非必输。
         :type AppVersion: str
-        :param _AppType: 安卓app的文件类型，本次加固操作的应用类型 。
-安卓在线加固和输出工具加固必输，其值需等于“apk”或“aab”，且与AndroidAppInfo.AppType值相等。
+        :param _AppType: Android app的文件类型，本次加固操作的应用类型 。
+Android在线加固和输出工具加固必输，其值需等于“apk”或“aab”，且与AndroidAppInfo.AppType值相等。
         :type AppType: str
         """
         self._AppMd5 = None
         self._AppSize = None
         self._AppUrl = None
         self._AppName = None
         self._AppPkgName = None
@@ -1867,25 +1867,25 @@
 class CreateEncryptInstanceRequest(AbstractModel):
     """CreateEncryptInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _PlatformType: 平台类型  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :param _PlatformType: 平台类型  1.android加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
         :type PlatformType: int
         :param _OrderType: 订单采购类型 1-免费试用 2-按年收费 3-按次收费
         :type OrderType: int
         :param _EncryptOpType: 1-在线加固、  2-输出工具加固
         :type EncryptOpType: int
         :param _ResourceId: 本次加固使用的资源id
         :type ResourceId: str
-        :param _AndroidAppInfo: 渠道合作安卓加固App信息 
+        :param _AndroidAppInfo: 渠道合作android加固App信息 
         :type AndroidAppInfo: :class:`tencentcloud.ms.v20180408.models.AndroidAppInfo`
-        :param _AndroidPlan: 渠道合作安卓加固策略信息
+        :param _AndroidPlan: 渠道合作android加固策略信息
         :type AndroidPlan: :class:`tencentcloud.ms.v20180408.models.AndroidPlan`
         :param _AppletInfo: 小程序加固信息
         :type AppletInfo: :class:`tencentcloud.ms.v20180408.models.AppletInfo`
         """
         self._PlatformType = None
         self._OrderType = None
         self._EncryptOpType = None
@@ -2015,20 +2015,20 @@
 class CreateOrderInstanceRequest(AbstractModel):
     """CreateOrderInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _PlatformType: 平台类型枚举值：1-android安卓加固  ；2-ios源码混淆 ； 3-sdk加固 ； 4-applet小程序加固
+        :param _PlatformType: 平台类型枚举值：1-android加固  ；2-ios源码混淆 ； 3-sdk加固 ； 4-applet小程序加固
         :type PlatformType: int
         :param _OrderType: 订单采购类型 1-免费试用 ；2-按年收费 ；3-按次收费
         :type OrderType: int
         :param _AppPkgNameList: 代表应用包名列表，值为单个包名（例如：“a.b.xxx”）或多个包名用逗号隔开(例如：“a.b.xxx,b.c.xxx”)。
-当安卓按年收费加固或安卓免费试用加固时，该字段要求非空，即PlatformType=1 并且 OrderType=2时，AppPkgNameList必传值。
+当android按年收费加固或android免费试用加固时，该字段要求非空，即PlatformType=1 并且 OrderType=2时，AppPkgNameList必传值。
 
         :type AppPkgNameList: str
         """
         self._PlatformType = None
         self._OrderType = None
         self._AppPkgNameList = None
 
@@ -2624,29 +2624,29 @@
         :type PageNumber: int
         :param _PageSize: 多记录每页展示数量
         :type PageSize: int
         :param _OrderField: 多记录查询时排序使用  仅支持CreateTime 任务创建时间排序
         :type OrderField: str
         :param _OrderDirection: 升序（asc）还是降序（desc），默认：desc。
         :type OrderDirection: str
-        :param _PlatformType: (条件过滤字段) 平台类型  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :param _PlatformType: (条件过滤字段) 平台类型  1.android加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
         :type PlatformType: int
         :param _OrderType: (条件过滤字段) 订单采购类型 1-免费试用 2-按年收费 3-按次收费
         :type OrderType: int
         :param _EncryptOpType: (条件过滤字段) 1-在线加固 或 2-输出工具加固
         :type EncryptOpType: int
         :param _ResultId: (条件过滤字段) 单记录查询时使用，结果ID该字段非空时，结构会根据结果ID进行单记录查询，符合查询条件时，只返回一条记录。
         :type ResultId: str
         :param _OrderId: (条件过滤字段) 查询与订单Id关联的任务
         :type OrderId: str
         :param _ResourceId: (条件过滤字段) 查询与资源Id关联的任务
         :type ResourceId: str
-        :param _AppType: (条件过滤字段) 安卓应用类型：安卓-apk; 安卓-aab;
+        :param _AppType: (条件过滤字段) 应用类型：android-apk; android-aab;
         :type AppType: str
-        :param _AppPkgName: （条件过滤字段）安卓应用的包名
+        :param _AppPkgName: （条件过滤字段）应用的包名
         :type AppPkgName: str
         :param _EncryptState: 加固结果，
 0：正在排队；
 1：加固成功；
 2：加固中；
 3：加固失败；
 5：重试；
@@ -2853,25 +2853,25 @@
 class DescribeEncryptPlanRequest(AbstractModel):
     """DescribeEncryptPlan请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _PlatformType: 平台类型  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :param _PlatformType: 平台类型  1.android加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
         :type PlatformType: int
         :param _OrderType: 订单采购类型 1-免费试用 2-按年收费 3-按次收费
         :type OrderType: int
         :param _EncryptOpType: 1-在线加固；2-输出工具
         :type EncryptOpType: int
         :param _ResourceId: 本次加固使用的资源id
         :type ResourceId: str
-        :param _AppPkgName: （条件过滤字段）安卓加固查询时，根据包名查询
+        :param _AppPkgName: （条件过滤字段）加固查询时，根据包名查询
         :type AppPkgName: str
-        :param _AppType: （条件过滤字段）安卓加固查询时，根据应用格式查询，枚举值：“apk”、“aab”
+        :param _AppType: （条件过滤字段）加固查询时，根据应用格式查询，枚举值：“apk”、“aab”
         :type AppType: str
         """
         self._PlatformType = None
         self._OrderType = None
         self._EncryptOpType = None
         self._ResourceId = None
         self._AppPkgName = None
@@ -2948,27 +2948,27 @@
 
     """
 
     def __init__(self):
         r"""
         :param _PlatformType: 平台类型整型值  
         :type PlatformType: int
-        :param _PlatformTypeDesc: 平台类型描述 1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :param _PlatformTypeDesc: 平台类型描述 1.android加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
         :type PlatformTypeDesc: str
         :param _EncryptOpType: 1- 在线加固 2-输出工具加固
         :type EncryptOpType: int
         :param _EncryptOpTypeDesc: 1- 在线加固 2-输出工具加固
         :type EncryptOpTypeDesc: str
         :param _OrderType: 订单收费类型枚举值
         :type OrderType: int
         :param _OrderTypeDesc: 订单收费类型描述
         :type OrderTypeDesc: str
         :param _ResourceId: 资源id
         :type ResourceId: str
-        :param _AndroidPlan: 上次安卓加固策略
+        :param _AndroidPlan: 上次加固策略
 注意：此字段可能返回 null，表示取不到有效值。
         :type AndroidPlan: :class:`tencentcloud.ms.v20180408.models.AndroidPlan`
         :param _AppletPlan: 上次小程序加固策略
 注意：此字段可能返回 null，表示取不到有效值。
         :type AppletPlan: :class:`tencentcloud.ms.v20180408.models.AppletPlan`
         :param _IOSPlan: 上次ios源码混淆加固配置
 注意：此字段可能返回 null，表示取不到有效值。
@@ -3123,27 +3123,27 @@
         :type PageNumber: int
         :param _PageSize: 每页展示数量
         :type PageSize: int
         :param _OrderField: 按某个字段排序，目前仅支持CreateTime排序。
         :type OrderField: str
         :param _OrderDirection: 升序（asc）还是降序（desc），默认：desc。
         :type OrderDirection: str
-        :param _PlatformType: （条件过滤字段）平台类型  1.android安卓加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
+        :param _PlatformType: （条件过滤字段）平台类型  1.android加固   2.ios源码混淆  3.sdk加固  4.applet小程序加固
         :type PlatformType: int
         :param _OrderType: （条件过滤字段）订单采购类型 1-免费试用 2-按年收费 3-按次收费
         :type OrderType: int
         :param _ApprovalStatus: （条件过滤字段）订单审批状态：
         :type ApprovalStatus: int
         :param _ResourceStatus: （条件过滤字段）资源状态：
         :type ResourceStatus: int
         :param _OrderId: （条件过滤字段）订单ID
         :type OrderId: str
         :param _ResourceId: （条件过滤字段）资源ID
         :type ResourceId: str
-        :param _AppPkgName: （条件过滤字段）安卓包名，查询android安卓加固订单时使用
+        :param _AppPkgName: （条件过滤字段）包名，查询android加固订单时使用
         :type AppPkgName: str
         """
         self._PageNumber = None
         self._PageSize = None
         self._OrderField = None
         self._OrderDirection = None
         self._PlatformType = None
```

### Comparing `tencentcloud-sdk-python-ms-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ms-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ms-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.947/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.946/README.rst` & `tencentcloud-sdk-python-ms-3.0.947/README.rst`

 * *Files identical despite different names*

