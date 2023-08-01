# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.946.tar", last modified: Mon Jul 31 00:23:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.947.tar", last modified: Tue Aug  1 00:34:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.946.tar` & `tencentcloud-sdk-python-cls-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)    81890 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9048 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   499514 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)    83686 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9048 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   508181 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:34:14.000000 tencentcloud-sdk-python-cls-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-cls-3.0.946/setup.py` & `tencentcloud-sdk-python-cls-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/v20201016/cls_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1103,14 +1103,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeKafkaConsumer(self, request):
+        """获取Kafka协议消费信息
+
+        :param request: Request instance for DescribeKafkaConsumer.
+        :type request: :class:`tencentcloud.cls.v20201016.models.DescribeKafkaConsumerRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeKafkaConsumerResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeKafkaConsumer", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeKafkaConsumerResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeKafkaRecharges(self, request):
         """本接口用于获取Kafka数据订阅任务
 
         :param request: Request instance for DescribeKafkaRecharges.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeKafkaRechargesRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeKafkaRechargesResponse`
 
@@ -1607,14 +1630,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def ModifyKafkaConsumer(self, request):
+        """修改Kafka协议消费信息
+
+        :param request: Request instance for ModifyKafkaConsumer.
+        :type request: :class:`tencentcloud.cls.v20201016.models.ModifyKafkaConsumerRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.ModifyKafkaConsumerResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyKafkaConsumer", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyKafkaConsumerResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ModifyKafkaRecharge(self, request):
         """本接口用于修改Kafka数据订阅任务
 
         :param request: Request instance for ModifyKafkaRecharge.
         :type request: :class:`tencentcloud.cls.v20201016.models.ModifyKafkaRechargeRequest`
```

### Comparing `tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.947/tencentcloud/cls/v20201016/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1372,15 +1372,15 @@
 class CloseKafkaConsumerRequest(AbstractModel):
     """CloseKafkaConsumer请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _FromTopicId: CLS对应的topic标识
+        :param _FromTopicId: 日志主题ID
         :type FromTopicId: str
         """
         self._FromTopicId = None
 
     @property
     def FromTopicId(self):
         return self._FromTopicId
@@ -1558,14 +1558,21 @@
         :type LogsetId: str
         :param _LogsetName: 日志集name
 注意：此字段可能返回 null，表示取不到有效值。
         :type LogsetName: str
         :param _TopicName: 日志主题name
 注意：此字段可能返回 null，表示取不到有效值。
         :type TopicName: str
+        :param _AdvancedConfig: 高级采集配置。 Json字符串， Key/Value定义为如下：
+- ClsAgentFileTimeout(超时属性), 取值范围: 大于等于0的整数， 0为不超时
+- ClsAgentMaxDepth(最大目录深度)，取值范围: 大于等于0的整数
+- ClsAgentParseFailMerge(合并解析失败日志)，取值范围: true或false
+样例：{"ClsAgentFileTimeout":0,"ClsAgentMaxDepth":10,"ClsAgentParseFailMerge":true}
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AdvancedConfig: str
         """
         self._ConfigExtraId = None
         self._Name = None
         self._TopicId = None
         self._Type = None
         self._HostFile = None
         self._ContainerFile = None
@@ -1578,14 +1585,15 @@
         self._CreateTime = None
         self._UserDefineRule = None
         self._GroupId = None
         self._ConfigFlag = None
         self._LogsetId = None
         self._LogsetName = None
         self._TopicName = None
+        self._AdvancedConfig = None
 
     @property
     def ConfigExtraId(self):
         return self._ConfigExtraId
 
     @ConfigExtraId.setter
     def ConfigExtraId(self, ConfigExtraId):
@@ -1731,14 +1739,22 @@
     def TopicName(self):
         return self._TopicName
 
     @TopicName.setter
     def TopicName(self, TopicName):
         self._TopicName = TopicName
 
+    @property
+    def AdvancedConfig(self):
+        return self._AdvancedConfig
+
+    @AdvancedConfig.setter
+    def AdvancedConfig(self, AdvancedConfig):
+        self._AdvancedConfig = AdvancedConfig
+
 
     def _deserialize(self, params):
         self._ConfigExtraId = params.get("ConfigExtraId")
         self._Name = params.get("Name")
         self._TopicId = params.get("TopicId")
         self._Type = params.get("Type")
         if params.get("HostFile") is not None:
@@ -1765,14 +1781,15 @@
         self._CreateTime = params.get("CreateTime")
         self._UserDefineRule = params.get("UserDefineRule")
         self._GroupId = params.get("GroupId")
         self._ConfigFlag = params.get("ConfigFlag")
         self._LogsetId = params.get("LogsetId")
         self._LogsetName = params.get("LogsetName")
         self._TopicName = params.get("TopicName")
+        self._AdvancedConfig = params.get("AdvancedConfig")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1812,26 +1829,34 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: str
         :param _CreateTime: 创建时间
         :type CreateTime: str
         :param _UserDefineRule: 用户自定义解析字符串
 注意：此字段可能返回 null，表示取不到有效值。
         :type UserDefineRule: str
+        :param _AdvancedConfig: 高级采集配置。 Json字符串， Key/Value定义为如下：
+- ClsAgentFileTimeout(超时属性), 取值范围: 大于等于0的整数， 0为不超时
+- ClsAgentMaxDepth(最大目录深度)，取值范围: 大于等于0的整数
+- ClsAgentParseFailMerge(合并解析失败日志)，取值范围: true或false
+样例：{"ClsAgentFileTimeout":0,"ClsAgentMaxDepth":10,"ClsAgentParseFailMerge":true}
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AdvancedConfig: str
         """
         self._ConfigId = None
         self._Name = None
         self._LogFormat = None
         self._Path = None
         self._LogType = None
         self._ExtractRule = None
         self._ExcludePaths = None
         self._Output = None
         self._UpdateTime = None
         self._CreateTime = None
         self._UserDefineRule = None
+        self._AdvancedConfig = None
 
     @property
     def ConfigId(self):
         return self._ConfigId
 
     @ConfigId.setter
     def ConfigId(self, ConfigId):
@@ -1913,14 +1938,22 @@
     def UserDefineRule(self):
         return self._UserDefineRule
 
     @UserDefineRule.setter
     def UserDefineRule(self, UserDefineRule):
         self._UserDefineRule = UserDefineRule
 
+    @property
+    def AdvancedConfig(self):
+        return self._AdvancedConfig
+
+    @AdvancedConfig.setter
+    def AdvancedConfig(self, AdvancedConfig):
+        self._AdvancedConfig = AdvancedConfig
+
 
     def _deserialize(self, params):
         self._ConfigId = params.get("ConfigId")
         self._Name = params.get("Name")
         self._LogFormat = params.get("LogFormat")
         self._Path = params.get("Path")
         self._LogType = params.get("LogType")
@@ -1933,14 +1966,15 @@
                 obj = ExcludePathInfo()
                 obj._deserialize(item)
                 self._ExcludePaths.append(obj)
         self._Output = params.get("Output")
         self._UpdateTime = params.get("UpdateTime")
         self._CreateTime = params.get("CreateTime")
         self._UserDefineRule = params.get("UserDefineRule")
+        self._AdvancedConfig = params.get("AdvancedConfig")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2987,14 +3021,20 @@
         :type ExcludePaths: list of ExcludePathInfo
         :param _UserDefineRule: 用户自定义采集规则，Json格式序列化的字符串
         :type UserDefineRule: str
         :param _GroupId: 绑定的机器组id
         :type GroupId: str
         :param _GroupIds: 绑定的机器组id列表
         :type GroupIds: list of str
+        :param _AdvancedConfig: 高级采集配置。 Json字符串， Key/Value定义为如下：
+- ClsAgentFileTimeout(超时属性), 取值范围: 大于等于0的整数， 0为不超时
+- ClsAgentMaxDepth(最大目录深度)，取值范围: 大于等于0的整数
+- ClsAgentParseFailMerge(合并解析失败日志)，取值范围: true或false
+样例：{"ClsAgentFileTimeout":0,"ClsAgentMaxDepth":10,"ClsAgentParseFailMerge":true}
+        :type AdvancedConfig: str
         """
         self._Name = None
         self._TopicId = None
         self._Type = None
         self._LogType = None
         self._ConfigFlag = None
         self._LogsetId = None
@@ -3005,14 +3045,15 @@
         self._ContainerStdout = None
         self._LogFormat = None
         self._ExtractRule = None
         self._ExcludePaths = None
         self._UserDefineRule = None
         self._GroupId = None
         self._GroupIds = None
+        self._AdvancedConfig = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
     def Name(self, Name):
@@ -3142,14 +3183,22 @@
     def GroupIds(self):
         return self._GroupIds
 
     @GroupIds.setter
     def GroupIds(self, GroupIds):
         self._GroupIds = GroupIds
 
+    @property
+    def AdvancedConfig(self):
+        return self._AdvancedConfig
+
+    @AdvancedConfig.setter
+    def AdvancedConfig(self, AdvancedConfig):
+        self._AdvancedConfig = AdvancedConfig
+
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._TopicId = params.get("TopicId")
         self._Type = params.get("Type")
         self._LogType = params.get("LogType")
         self._ConfigFlag = params.get("ConfigFlag")
@@ -3174,14 +3223,15 @@
             for item in params.get("ExcludePaths"):
                 obj = ExcludePathInfo()
                 obj._deserialize(item)
                 self._ExcludePaths.append(obj)
         self._UserDefineRule = params.get("UserDefineRule")
         self._GroupId = params.get("GroupId")
         self._GroupIds = params.get("GroupIds")
+        self._AdvancedConfig = params.get("AdvancedConfig")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3242,15 +3292,19 @@
         :type LogType: str
         :param _ExtractRule: 提取规则，如果设置了ExtractRule，则必须设置LogType
         :type ExtractRule: :class:`tencentcloud.cls.v20201016.models.ExtractRuleInfo`
         :param _ExcludePaths: 采集黑名单路径列表
         :type ExcludePaths: list of ExcludePathInfo
         :param _UserDefineRule: 用户自定义采集规则，Json格式序列化的字符串
         :type UserDefineRule: str
-        :param _AdvancedConfig: 高级采集配置
+        :param _AdvancedConfig: 高级采集配置。 Json字符串， Key/Value定义为如下：
+- ClsAgentFileTimeout(超时属性), 取值范围: 大于等于0的整数， 0为不超时
+- ClsAgentMaxDepth(最大目录深度)，取值范围: 大于等于0的整数
+- ClsAgentParseFailMerge(合并解析失败日志)，取值范围: true或false
+样例：{"ClsAgentFileTimeout":0,"ClsAgentMaxDepth":10,"ClsAgentParseFailMerge":true}
         :type AdvancedConfig: str
         """
         self._Name = None
         self._Output = None
         self._Path = None
         self._LogType = None
         self._ExtractRule = None
@@ -8214,14 +8268,108 @@
             self._Rule._deserialize(params.get("Rule"))
         self._ModifyTime = params.get("ModifyTime")
         self._IncludeInternalFields = params.get("IncludeInternalFields")
         self._MetadataFlag = params.get("MetadataFlag")
         self._RequestId = params.get("RequestId")
 
 
+class DescribeKafkaConsumerRequest(AbstractModel):
+    """DescribeKafkaConsumer请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FromTopicId: 日志主题ID
+        :type FromTopicId: str
+        """
+        self._FromTopicId = None
+
+    @property
+    def FromTopicId(self):
+        return self._FromTopicId
+
+    @FromTopicId.setter
+    def FromTopicId(self, FromTopicId):
+        self._FromTopicId = FromTopicId
+
+
+    def _deserialize(self, params):
+        self._FromTopicId = params.get("FromTopicId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeKafkaConsumerResponse(AbstractModel):
+    """DescribeKafkaConsumer返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Status: Kafka协议消费是否打开
+        :type Status: bool
+        :param _TopicID: KafkaConsumer 消费时使用的Topic参数
+        :type TopicID: str
+        :param _Compression: 压缩方式[0:NONE；2:SNAPPY；3:LZ4]
+        :type Compression: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Status = None
+        self._TopicID = None
+        self._Compression = None
+        self._RequestId = None
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def TopicID(self):
+        return self._TopicID
+
+    @TopicID.setter
+    def TopicID(self, TopicID):
+        self._TopicID = TopicID
+
+    @property
+    def Compression(self):
+        return self._Compression
+
+    @Compression.setter
+    def Compression(self, Compression):
+        self._Compression = Compression
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Status = params.get("Status")
+        self._TopicID = params.get("TopicID")
+        self._Compression = params.get("Compression")
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeKafkaRechargesRequest(AbstractModel):
     """DescribeKafkaRecharges请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12814,14 +12962,20 @@
         :type ConfigFlag: str
         :param _LogsetId: 日志集ID
         :type LogsetId: str
         :param _LogsetName: 日志集name
         :type LogsetName: str
         :param _TopicName: 日志主题name
         :type TopicName: str
+        :param _AdvancedConfig: 高级采集配置。 Json字符串， Key/Value定义为如下：
+- ClsAgentFileTimeout(超时属性), 取值范围: 大于等于0的整数， 0为不超时
+- ClsAgentMaxDepth(最大目录深度)，取值范围: 大于等于0的整数
+- ClsAgentParseFailMerge(合并解析失败日志)，取值范围: true或false
+样例：{"ClsAgentFileTimeout":0,"ClsAgentMaxDepth":10,"ClsAgentParseFailMerge":true}
+        :type AdvancedConfig: str
         """
         self._ConfigExtraId = None
         self._Name = None
         self._TopicId = None
         self._HostFile = None
         self._ContainerFile = None
         self._ContainerStdout = None
@@ -12832,14 +12986,15 @@
         self._UserDefineRule = None
         self._Type = None
         self._GroupId = None
         self._ConfigFlag = None
         self._LogsetId = None
         self._LogsetName = None
         self._TopicName = None
+        self._AdvancedConfig = None
 
     @property
     def ConfigExtraId(self):
         return self._ConfigExtraId
 
     @ConfigExtraId.setter
     def ConfigExtraId(self, ConfigExtraId):
@@ -12969,14 +13124,22 @@
     def TopicName(self):
         return self._TopicName
 
     @TopicName.setter
     def TopicName(self, TopicName):
         self._TopicName = TopicName
 
+    @property
+    def AdvancedConfig(self):
+        return self._AdvancedConfig
+
+    @AdvancedConfig.setter
+    def AdvancedConfig(self, AdvancedConfig):
+        self._AdvancedConfig = AdvancedConfig
+
 
     def _deserialize(self, params):
         self._ConfigExtraId = params.get("ConfigExtraId")
         self._Name = params.get("Name")
         self._TopicId = params.get("TopicId")
         if params.get("HostFile") is not None:
             self._HostFile = HostFileInfo()
@@ -13001,14 +13164,15 @@
         self._UserDefineRule = params.get("UserDefineRule")
         self._Type = params.get("Type")
         self._GroupId = params.get("GroupId")
         self._ConfigFlag = params.get("ConfigFlag")
         self._LogsetId = params.get("LogsetId")
         self._LogsetName = params.get("LogsetName")
         self._TopicName = params.get("TopicName")
+        self._AdvancedConfig = params.get("AdvancedConfig")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -13059,23 +13223,30 @@
         :type ExtractRule: :class:`tencentcloud.cls.v20201016.models.ExtractRuleInfo`
         :param _ExcludePaths: 采集黑名单路径列表
         :type ExcludePaths: list of ExcludePathInfo
         :param _Output: 采集配置关联的日志主题（TopicId）
         :type Output: str
         :param _UserDefineRule: 用户自定义解析字符串，Json格式序列化的字符串
         :type UserDefineRule: str
+        :param _AdvancedConfig: 高级采集配置。 Json字符串， Key/Value定义为如下：
+- ClsAgentFileTimeout(超时属性), 取值范围: 大于等于0的整数， 0为不超时
+- ClsAgentMaxDepth(最大目录深度)，取值范围: 大于等于0的整数
+- ClsAgentParseFailMerge(合并解析失败日志)，取值范围: true或false
+样例：{"ClsAgentFileTimeout":0,"ClsAgentMaxDepth":10,"ClsAgentParseFailMerge":true}
+        :type AdvancedConfig: str
         """
         self._ConfigId = None
         self._Name = None
         self._Path = None
         self._LogType = None
         self._ExtractRule = None
         self._ExcludePaths = None
         self._Output = None
         self._UserDefineRule = None
+        self._AdvancedConfig = None
 
     @property
     def ConfigId(self):
         return self._ConfigId
 
     @ConfigId.setter
     def ConfigId(self, ConfigId):
@@ -13133,14 +13304,22 @@
     def UserDefineRule(self):
         return self._UserDefineRule
 
     @UserDefineRule.setter
     def UserDefineRule(self, UserDefineRule):
         self._UserDefineRule = UserDefineRule
 
+    @property
+    def AdvancedConfig(self):
+        return self._AdvancedConfig
+
+    @AdvancedConfig.setter
+    def AdvancedConfig(self, AdvancedConfig):
+        self._AdvancedConfig = AdvancedConfig
+
 
     def _deserialize(self, params):
         self._ConfigId = params.get("ConfigId")
         self._Name = params.get("Name")
         self._Path = params.get("Path")
         self._LogType = params.get("LogType")
         if params.get("ExtractRule") is not None:
@@ -13150,14 +13329,15 @@
             self._ExcludePaths = []
             for item in params.get("ExcludePaths"):
                 obj = ExcludePathInfo()
                 obj._deserialize(item)
                 self._ExcludePaths.append(obj)
         self._Output = params.get("Output")
         self._UserDefineRule = params.get("UserDefineRule")
+        self._AdvancedConfig = params.get("AdvancedConfig")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -13625,14 +13805,84 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class ModifyKafkaConsumerRequest(AbstractModel):
+    """ModifyKafkaConsumer请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FromTopicId: 日志主题ID
+        :type FromTopicId: str
+        :param _Compression: 压缩方式[0:NONE；2:SNAPPY；3:LZ4]
+        :type Compression: int
+        """
+        self._FromTopicId = None
+        self._Compression = None
+
+    @property
+    def FromTopicId(self):
+        return self._FromTopicId
+
+    @FromTopicId.setter
+    def FromTopicId(self, FromTopicId):
+        self._FromTopicId = FromTopicId
+
+    @property
+    def Compression(self):
+        return self._Compression
+
+    @Compression.setter
+    def Compression(self, Compression):
+        self._Compression = Compression
+
+
+    def _deserialize(self, params):
+        self._FromTopicId = params.get("FromTopicId")
+        self._Compression = params.get("Compression")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyKafkaConsumerResponse(AbstractModel):
+    """ModifyKafkaConsumer返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class ModifyKafkaRechargeRequest(AbstractModel):
     """ModifyKafkaRecharge请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -14822,15 +15072,15 @@
 class OpenKafkaConsumerRequest(AbstractModel):
     """OpenKafkaConsumer请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _FromTopicId: CLS控制台创建的TopicId
+        :param _FromTopicId: 日志主题ID
         :type FromTopicId: str
         :param _Compression: 压缩方式[0:NONE；2:SNAPPY；3:LZ4]
         :type Compression: int
         :param _ConsumerContent: kafka协议消费数据格式
         :type ConsumerContent: :class:`tencentcloud.cls.v20201016.models.KafkaConsumerContent`
         """
         self._FromTopicId = None
@@ -14881,15 +15131,15 @@
 class OpenKafkaConsumerResponse(AbstractModel):
     """OpenKafkaConsumer返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TopicID: 待消费TopicId
+        :param _TopicID: KafkaConsumer 消费时使用的Topic参数
         :type TopicID: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TopicID = None
         self._RequestId = None
```

### Comparing `tencentcloud-sdk-python-cls-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.947/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.947/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.946/README.rst` & `tencentcloud-sdk-python-cls-3.0.947/README.rst`

 * *Files identical despite different names*

