# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.946.tar", last modified: Mon Jul 31 00:37:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.947.tar", last modified: Tue Aug  1 00:57:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.946.tar` & `tencentcloud-sdk-python-tdmq-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94553 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10019 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   591304 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-31 00:37:11.000000 tencentcloud-sdk-python-tdmq-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95480 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10019 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   596365 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-01 00:57:22.000000 tencentcloud-sdk-python-tdmq-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.946/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,14 +390,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateRocketMQVipInstance(self, request):
+        """创建RocketMQ专享实例
+
+        :param request: Request instance for CreateRocketMQVipInstance.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRocketMQVipInstanceRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.CreateRocketMQVipInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateRocketMQVipInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateRocketMQVipInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreateRole(self, request):
         """创建角色
 
         :param request: Request instance for CreateRole.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.CreateRoleRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.CreateRoleResponse`
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/tdmq/v20200217/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3993,14 +3993,162 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class CreateRocketMQVipInstanceRequest(AbstractModel):
+    """CreateRocketMQVipInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: 实例名称
+        :type Name: str
+        :param _Spec: 实例规格：
+基础型，rocket-vip-basic-1
+标准型，rocket-vip-basic-2
+高阶Ⅰ型，rocket-vip-basic-3
+高阶Ⅱ型，rocket-vip-basic-4
+        :type Spec: str
+        :param _NodeCount: 节点数量，最小2，最大20
+        :type NodeCount: int
+        :param _StorageSize: 单节点存储空间，GB为单位，最低200GB
+        :type StorageSize: int
+        :param _ZoneIds: 节点部署的区域ID列表，如广州一区，则是100001，具体可查询腾讯云官网
+        :type ZoneIds: list of str
+        :param _VpcInfo: VPC信息
+        :type VpcInfo: :class:`tencentcloud.tdmq.v20200217.models.VpcInfo`
+        :param _TimeSpan: 购买时长，月为单位
+        :type TimeSpan: int
+        """
+        self._Name = None
+        self._Spec = None
+        self._NodeCount = None
+        self._StorageSize = None
+        self._ZoneIds = None
+        self._VpcInfo = None
+        self._TimeSpan = None
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Spec(self):
+        return self._Spec
+
+    @Spec.setter
+    def Spec(self, Spec):
+        self._Spec = Spec
+
+    @property
+    def NodeCount(self):
+        return self._NodeCount
+
+    @NodeCount.setter
+    def NodeCount(self, NodeCount):
+        self._NodeCount = NodeCount
+
+    @property
+    def StorageSize(self):
+        return self._StorageSize
+
+    @StorageSize.setter
+    def StorageSize(self, StorageSize):
+        self._StorageSize = StorageSize
+
+    @property
+    def ZoneIds(self):
+        return self._ZoneIds
+
+    @ZoneIds.setter
+    def ZoneIds(self, ZoneIds):
+        self._ZoneIds = ZoneIds
+
+    @property
+    def VpcInfo(self):
+        return self._VpcInfo
+
+    @VpcInfo.setter
+    def VpcInfo(self, VpcInfo):
+        self._VpcInfo = VpcInfo
+
+    @property
+    def TimeSpan(self):
+        return self._TimeSpan
+
+    @TimeSpan.setter
+    def TimeSpan(self, TimeSpan):
+        self._TimeSpan = TimeSpan
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        self._Spec = params.get("Spec")
+        self._NodeCount = params.get("NodeCount")
+        self._StorageSize = params.get("StorageSize")
+        self._ZoneIds = params.get("ZoneIds")
+        if params.get("VpcInfo") is not None:
+            self._VpcInfo = VpcInfo()
+            self._VpcInfo._deserialize(params.get("VpcInfo"))
+        self._TimeSpan = params.get("TimeSpan")
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
+class CreateRocketMQVipInstanceResponse(AbstractModel):
+    """CreateRocketMQVipInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ClusterId: 集群ID
+        :type ClusterId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._ClusterId = None
+        self._RequestId = None
+
+    @property
+    def ClusterId(self):
+        return self._ClusterId
+
+    @ClusterId.setter
+    def ClusterId(self, ClusterId):
+        self._ClusterId = ClusterId
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
+        self._ClusterId = params.get("ClusterId")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateRoleRequest(AbstractModel):
     """CreateRole请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -19930,8 +20078,53 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class VpcInfo(AbstractModel):
+    """vpc信息（由UniqVpcId和UniqSubnetId组成）
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _VpcId: vpc信息
+        :type VpcId: str
+        :param _SubnetId: 子网信息
+        :type SubnetId: str
+        """
+        self._VpcId = None
+        self._SubnetId = None
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
+    @property
+    def SubnetId(self):
+        return self._SubnetId
+
+    @SubnetId.setter
+    def SubnetId(self, SubnetId):
+        self._SubnetId = SubnetId
+
+
+    def _deserialize(self, params):
+        self._VpcId = params.get("VpcId")
+        self._SubnetId = params.get("SubnetId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.947/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.946/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.947/README.rst`

 * *Files identical despite different names*

