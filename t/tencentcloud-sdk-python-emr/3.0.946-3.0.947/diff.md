# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.946.tar", last modified: Mon Jul 31 00:25:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.947.tar", last modified: Tue Aug  1 00:37:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.946.tar` & `tencentcloud-sdk-python-emr-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:25:57.000000 tencentcloud-sdk-python-emr-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:25:57.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30148 2023-07-31 00:25:57.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    14440 2023-07-31 00:25:57.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   455449 2023-07-31 00:25:57.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:25:57.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:25:57.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:25:58.000000 tencentcloud-sdk-python-emr-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:25:57.000000 tencentcloud-sdk-python-emr-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30148 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    14440 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   455975 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:37:08.000000 tencentcloud-sdk-python-emr-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-emr-3.0.946/setup.py` & `tencentcloud-sdk-python-emr-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.946/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.947/tencentcloud/emr/v20190103/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8753,14 +8753,17 @@
         :type ServiceClient: str
         :param _DisableApiTermination: 该实例是否开启实例保护，true为开启 false为关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type DisableApiTermination: bool
         :param _TradeVersion: 0表示老计费，1表示新计费
 注意：此字段可能返回 null，表示取不到有效值。
         :type TradeVersion: int
+        :param _ServicesStatus: 各组件状态，Zookeeper:STARTED,ResourceManager:STARTED，STARTED已启动，STOPED已停止
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ServicesStatus: str
         """
         self._AppId = None
         self._SerialNo = None
         self._OrderNo = None
         self._WanIp = None
         self._Flag = None
         self._Spec = None
@@ -8804,14 +8807,15 @@
         self._Clients = None
         self._CurrentTime = None
         self._IsFederation = None
         self._DeviceName = None
         self._ServiceClient = None
         self._DisableApiTermination = None
         self._TradeVersion = None
+        self._ServicesStatus = None
 
     @property
     def AppId(self):
         return self._AppId
 
     @AppId.setter
     def AppId(self, AppId):
@@ -9205,14 +9209,22 @@
     def TradeVersion(self):
         return self._TradeVersion
 
     @TradeVersion.setter
     def TradeVersion(self, TradeVersion):
         self._TradeVersion = TradeVersion
 
+    @property
+    def ServicesStatus(self):
+        return self._ServicesStatus
+
+    @ServicesStatus.setter
+    def ServicesStatus(self, ServicesStatus):
+        self._ServicesStatus = ServicesStatus
+
 
     def _deserialize(self, params):
         self._AppId = params.get("AppId")
         self._SerialNo = params.get("SerialNo")
         self._OrderNo = params.get("OrderNo")
         self._WanIp = params.get("WanIp")
         self._Flag = params.get("Flag")
@@ -9271,14 +9283,15 @@
         self._Clients = params.get("Clients")
         self._CurrentTime = params.get("CurrentTime")
         self._IsFederation = params.get("IsFederation")
         self._DeviceName = params.get("DeviceName")
         self._ServiceClient = params.get("ServiceClient")
         self._DisableApiTermination = params.get("DisableApiTermination")
         self._TradeVersion = params.get("TradeVersion")
+        self._ServicesStatus = params.get("ServicesStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-emr-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.946/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.947/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.947/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.946/README.rst` & `tencentcloud-sdk-python-emr-3.0.947/README.rst`

 * *Files identical despite different names*

