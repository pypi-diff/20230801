# Comparing `tmp/tencentcloud-sdk-python-oceanus-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-oceanus-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.946.tar", last modified: Mon Jul 31 00:33:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.947.tar", last modified: Tue Aug  1 00:53:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-oceanus-3.0.946.tar` & `tencentcloud-sdk-python-oceanus-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9664 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/v20190422/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25417 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)   217602 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud_sdk_python_oceanus.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-31 00:33:03.000000 tencentcloud-sdk-python-oceanus-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9664 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/v20190422/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25417 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)   236219 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud_sdk_python_oceanus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-08-01 00:53:04.000000 tencentcloud-sdk-python-oceanus-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.946/setup.py` & `tencentcloud-sdk-python-oceanus-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud/oceanus/v20190422/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,64 @@
 
     def _deserialize(self, params):
         self._SerialId = params.get("SerialId")
         self._SavepointStatus = params.get("SavepointStatus")
         self._RequestId = params.get("RequestId")
 
 
+class ClazzLevel(AbstractModel):
+    """{
+    "Clazz": "c1", // java类全路径
+    "Level": "WARN" // 日志级别  TRACE，DEBUG、INFO、WARN、ERROR
+    }
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Clazz: java类全路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Clazz: str
+        :param _Level: 日志级别  TRACE，DEBUG、INFO、WARN、ERROR
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Level: str
+        """
+        self._Clazz = None
+        self._Level = None
+
+    @property
+    def Clazz(self):
+        return self._Clazz
+
+    @Clazz.setter
+    def Clazz(self, Clazz):
+        self._Clazz = Clazz
+
+    @property
+    def Level(self):
+        return self._Level
+
+    @Level.setter
+    def Level(self, Level):
+        self._Level = Level
+
+
+    def _deserialize(self, params):
+        self._Clazz = params.get("Clazz")
+        self._Level = params.get("Level")
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
 class Cluster(AbstractModel):
     """描述用户创建的集群信息
 
     """
 
     def __init__(self):
         r"""
@@ -1498,14 +1548,20 @@
         :type PythonVersion: str
         :param _WorkSpaceId: 工作空间 SerialId
         :type WorkSpaceId: str
         :param _LogLevel: 日志级别
         :type LogLevel: str
         :param _AutoRecover: Oceanus 平台恢复作业开关 1:开启 -1: 关闭
         :type AutoRecover: int
+        :param _ClazzLevels: 类日志级别
+        :type ClazzLevels: list of ClazzLevel
+        :param _ExpertModeOn: 是否打开专家模式
+        :type ExpertModeOn: bool
+        :param _ExpertModeConfiguration: 专家模式的配置
+        :type ExpertModeConfiguration: :class:`tencentcloud.oceanus.v20190422.models.ExpertModeConfiguration`
         """
         self._JobId = None
         self._EntrypointClass = None
         self._ProgramArgs = None
         self._Remark = None
         self._ResourceRefs = None
         self._DefaultParallelism = None
@@ -1518,14 +1574,17 @@
         self._ClsLogsetId = None
         self._ClsTopicId = None
         self._LogCollectType = None
         self._PythonVersion = None
         self._WorkSpaceId = None
         self._LogLevel = None
         self._AutoRecover = None
+        self._ClazzLevels = None
+        self._ExpertModeOn = None
+        self._ExpertModeConfiguration = None
 
     @property
     def JobId(self):
         return self._JobId
 
     @JobId.setter
     def JobId(self, JobId):
@@ -1671,14 +1730,38 @@
     def AutoRecover(self):
         return self._AutoRecover
 
     @AutoRecover.setter
     def AutoRecover(self, AutoRecover):
         self._AutoRecover = AutoRecover
 
+    @property
+    def ClazzLevels(self):
+        return self._ClazzLevels
+
+    @ClazzLevels.setter
+    def ClazzLevels(self, ClazzLevels):
+        self._ClazzLevels = ClazzLevels
+
+    @property
+    def ExpertModeOn(self):
+        return self._ExpertModeOn
+
+    @ExpertModeOn.setter
+    def ExpertModeOn(self, ExpertModeOn):
+        self._ExpertModeOn = ExpertModeOn
+
+    @property
+    def ExpertModeConfiguration(self):
+        return self._ExpertModeConfiguration
+
+    @ExpertModeConfiguration.setter
+    def ExpertModeConfiguration(self, ExpertModeConfiguration):
+        self._ExpertModeConfiguration = ExpertModeConfiguration
+
 
     def _deserialize(self, params):
         self._JobId = params.get("JobId")
         self._EntrypointClass = params.get("EntrypointClass")
         self._ProgramArgs = params.get("ProgramArgs")
         self._Remark = params.get("Remark")
         if params.get("ResourceRefs") is not None:
@@ -1702,14 +1785,24 @@
         self._ClsLogsetId = params.get("ClsLogsetId")
         self._ClsTopicId = params.get("ClsTopicId")
         self._LogCollectType = params.get("LogCollectType")
         self._PythonVersion = params.get("PythonVersion")
         self._WorkSpaceId = params.get("WorkSpaceId")
         self._LogLevel = params.get("LogLevel")
         self._AutoRecover = params.get("AutoRecover")
+        if params.get("ClazzLevels") is not None:
+            self._ClazzLevels = []
+            for item in params.get("ClazzLevels"):
+                obj = ClazzLevel()
+                obj._deserialize(item)
+                self._ClazzLevels.append(obj)
+        self._ExpertModeOn = params.get("ExpertModeOn")
+        if params.get("ExpertModeConfiguration") is not None:
+            self._ExpertModeConfiguration = ExpertModeConfiguration()
+            self._ExpertModeConfiguration._deserialize(params.get("ExpertModeConfiguration"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -4402,14 +4495,86 @@
                 obj = WorkSpaceSetItem()
                 obj._deserialize(item)
                 self._WorkSpaceSetItem.append(obj)
         self._TotalCount = params.get("TotalCount")
         self._RequestId = params.get("RequestId")
 
 
+class ExpertModeConfiguration(AbstractModel):
+    """作业配置 -- 专家模式的详细配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _JobGraph: Job graph
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobGraph: :class:`tencentcloud.oceanus.v20190422.models.JobGraph`
+        :param _NodeConfig: Node configuration
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NodeConfig: list of NodeConfig
+        :param _SlotSharingGroups: Slot sharing groups
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SlotSharingGroups: list of SlotSharingGroup
+        """
+        self._JobGraph = None
+        self._NodeConfig = None
+        self._SlotSharingGroups = None
+
+    @property
+    def JobGraph(self):
+        return self._JobGraph
+
+    @JobGraph.setter
+    def JobGraph(self, JobGraph):
+        self._JobGraph = JobGraph
+
+    @property
+    def NodeConfig(self):
+        return self._NodeConfig
+
+    @NodeConfig.setter
+    def NodeConfig(self, NodeConfig):
+        self._NodeConfig = NodeConfig
+
+    @property
+    def SlotSharingGroups(self):
+        return self._SlotSharingGroups
+
+    @SlotSharingGroups.setter
+    def SlotSharingGroups(self, SlotSharingGroups):
+        self._SlotSharingGroups = SlotSharingGroups
+
+
+    def _deserialize(self, params):
+        if params.get("JobGraph") is not None:
+            self._JobGraph = JobGraph()
+            self._JobGraph._deserialize(params.get("JobGraph"))
+        if params.get("NodeConfig") is not None:
+            self._NodeConfig = []
+            for item in params.get("NodeConfig"):
+                obj = NodeConfig()
+                obj._deserialize(item)
+                self._NodeConfig.append(obj)
+        if params.get("SlotSharingGroups") is not None:
+            self._SlotSharingGroups = []
+            for item in params.get("SlotSharingGroups"):
+                obj = SlotSharingGroup()
+                obj._deserialize(item)
+                self._SlotSharingGroups.append(obj)
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
 class Filter(AbstractModel):
     """查询作业列表时的过滤器
 
     """
 
     def __init__(self):
         r"""
@@ -4514,14 +4679,23 @@
         :type PythonVersion: str
         :param _AutoRecover: Oceanus 平台恢复作业开关 1:开启 -1: 关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type AutoRecover: int
         :param _LogLevel: 日志级别
 注意：此字段可能返回 null，表示取不到有效值。
         :type LogLevel: str
+        :param _ClazzLevels: 类日志级别
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClazzLevels: list of ClazzLevel
+        :param _ExpertModeOn: 是否开启专家模式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExpertModeOn: bool
+        :param _ExpertModeConfiguration: 专家模式的配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExpertModeConfiguration: :class:`tencentcloud.oceanus.v20190422.models.ExpertModeConfiguration`
         """
         self._JobId = None
         self._EntrypointClass = None
         self._ProgramArgs = None
         self._Remark = None
         self._CreateTime = None
         self._Version = None
@@ -4536,14 +4710,17 @@
         self._JobManagerSpec = None
         self._TaskManagerSpec = None
         self._ClsLogsetId = None
         self._ClsTopicId = None
         self._PythonVersion = None
         self._AutoRecover = None
         self._LogLevel = None
+        self._ClazzLevels = None
+        self._ExpertModeOn = None
+        self._ExpertModeConfiguration = None
 
     @property
     def JobId(self):
         return self._JobId
 
     @JobId.setter
     def JobId(self, JobId):
@@ -4705,14 +4882,38 @@
     def LogLevel(self):
         return self._LogLevel
 
     @LogLevel.setter
     def LogLevel(self, LogLevel):
         self._LogLevel = LogLevel
 
+    @property
+    def ClazzLevels(self):
+        return self._ClazzLevels
+
+    @ClazzLevels.setter
+    def ClazzLevels(self, ClazzLevels):
+        self._ClazzLevels = ClazzLevels
+
+    @property
+    def ExpertModeOn(self):
+        return self._ExpertModeOn
+
+    @ExpertModeOn.setter
+    def ExpertModeOn(self, ExpertModeOn):
+        self._ExpertModeOn = ExpertModeOn
+
+    @property
+    def ExpertModeConfiguration(self):
+        return self._ExpertModeConfiguration
+
+    @ExpertModeConfiguration.setter
+    def ExpertModeConfiguration(self, ExpertModeConfiguration):
+        self._ExpertModeConfiguration = ExpertModeConfiguration
+
 
     def _deserialize(self, params):
         self._JobId = params.get("JobId")
         self._EntrypointClass = params.get("EntrypointClass")
         self._ProgramArgs = params.get("ProgramArgs")
         self._Remark = params.get("Remark")
         self._CreateTime = params.get("CreateTime")
@@ -4738,14 +4939,201 @@
         self._JobManagerSpec = params.get("JobManagerSpec")
         self._TaskManagerSpec = params.get("TaskManagerSpec")
         self._ClsLogsetId = params.get("ClsLogsetId")
         self._ClsTopicId = params.get("ClsTopicId")
         self._PythonVersion = params.get("PythonVersion")
         self._AutoRecover = params.get("AutoRecover")
         self._LogLevel = params.get("LogLevel")
+        if params.get("ClazzLevels") is not None:
+            self._ClazzLevels = []
+            for item in params.get("ClazzLevels"):
+                obj = ClazzLevel()
+                obj._deserialize(item)
+                self._ClazzLevels.append(obj)
+        self._ExpertModeOn = params.get("ExpertModeOn")
+        if params.get("ExpertModeConfiguration") is not None:
+            self._ExpertModeConfiguration = ExpertModeConfiguration()
+            self._ExpertModeConfiguration._deserialize(params.get("ExpertModeConfiguration"))
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
+class JobGraph(AbstractModel):
+    """作业运行图
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Nodes: 运行图的点集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Nodes: list of JobGraphNode
+        :param _Edges: 运行图的边集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Edges: list of JobGraphEdge
+        """
+        self._Nodes = None
+        self._Edges = None
+
+    @property
+    def Nodes(self):
+        return self._Nodes
+
+    @Nodes.setter
+    def Nodes(self, Nodes):
+        self._Nodes = Nodes
+
+    @property
+    def Edges(self):
+        return self._Edges
+
+    @Edges.setter
+    def Edges(self, Edges):
+        self._Edges = Edges
+
+
+    def _deserialize(self, params):
+        if params.get("Nodes") is not None:
+            self._Nodes = []
+            for item in params.get("Nodes"):
+                obj = JobGraphNode()
+                obj._deserialize(item)
+                self._Nodes.append(obj)
+        if params.get("Edges") is not None:
+            self._Edges = []
+            for item in params.get("Edges"):
+                obj = JobGraphEdge()
+                obj._deserialize(item)
+                self._Edges.append(obj)
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
+class JobGraphEdge(AbstractModel):
+    """Flink Job 运行图的边信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Source: 边的起始节点ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Source: int
+        :param _Target: 边的目标节点ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Target: int
+        """
+        self._Source = None
+        self._Target = None
+
+    @property
+    def Source(self):
+        return self._Source
+
+    @Source.setter
+    def Source(self, Source):
+        self._Source = Source
+
+    @property
+    def Target(self):
+        return self._Target
+
+    @Target.setter
+    def Target(self, Target):
+        self._Target = Target
+
+
+    def _deserialize(self, params):
+        self._Source = params.get("Source")
+        self._Target = params.get("Target")
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
+class JobGraphNode(AbstractModel):
+    """Flink Job 运行图的点信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: 节点ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: int
+        :param _Description: 节点描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param _Name: 节点名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param _Parallelism: 节点并行度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Parallelism: int
+        """
+        self._Id = None
+        self._Description = None
+        self._Name = None
+        self._Parallelism = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
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
+    def Parallelism(self):
+        return self._Parallelism
+
+    @Parallelism.setter
+    def Parallelism(self, Parallelism):
+        self._Parallelism = Parallelism
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._Description = params.get("Description")
+        self._Name = params.get("Name")
+        self._Parallelism = params.get("Parallelism")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5438,14 +5826,105 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class NodeConfig(AbstractModel):
+    """专家模式  计算节点的配置信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: Node ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: int
+        :param _Parallelism: Node parallelism
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Parallelism: int
+        :param _SlotSharingGroup: Slot sharing group
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SlotSharingGroup: str
+        :param _Configuration: Configuration properties
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Configuration: list of Property
+        :param _StateTTL: 节点的状态ttl配置, 多个用 ; 分割
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StateTTL: str
+        """
+        self._Id = None
+        self._Parallelism = None
+        self._SlotSharingGroup = None
+        self._Configuration = None
+        self._StateTTL = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Parallelism(self):
+        return self._Parallelism
+
+    @Parallelism.setter
+    def Parallelism(self, Parallelism):
+        self._Parallelism = Parallelism
+
+    @property
+    def SlotSharingGroup(self):
+        return self._SlotSharingGroup
+
+    @SlotSharingGroup.setter
+    def SlotSharingGroup(self, SlotSharingGroup):
+        self._SlotSharingGroup = SlotSharingGroup
+
+    @property
+    def Configuration(self):
+        return self._Configuration
+
+    @Configuration.setter
+    def Configuration(self, Configuration):
+        self._Configuration = Configuration
+
+    @property
+    def StateTTL(self):
+        return self._StateTTL
+
+    @StateTTL.setter
+    def StateTTL(self, StateTTL):
+        self._StateTTL = StateTTL
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._Parallelism = params.get("Parallelism")
+        self._SlotSharingGroup = params.get("SlotSharingGroup")
+        if params.get("Configuration") is not None:
+            self._Configuration = []
+            for item in params.get("Configuration"):
+                obj = Property()
+                obj._deserialize(item)
+                self._Configuration.append(obj)
+        self._StateTTL = params.get("StateTTL")
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
 class Property(AbstractModel):
     """系统配置属性
 
     """
 
     def __init__(self):
         r"""
@@ -6816,14 +7295,149 @@
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
+class SlotSharingGroup(AbstractModel):
+    """SlotSharingGroup 描述
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: SlotSharingGroup的名字
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param _Spec: SlotSharingGroup的规格
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Spec: :class:`tencentcloud.oceanus.v20190422.models.SlotSharingGroupSpec`
+        :param _Description: SlotSharingGroup的描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        """
+        self._Name = None
+        self._Spec = None
+        self._Description = None
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
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        if params.get("Spec") is not None:
+            self._Spec = SlotSharingGroupSpec()
+            self._Spec._deserialize(params.get("Spec"))
+        self._Description = params.get("Description")
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
+class SlotSharingGroupSpec(AbstractModel):
+    """SlotSharingGroup的规格描述
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _CPU: 适用的cpu
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CPU: float
+        :param _HeapMemory: 默认为b, 支持单位有 b, kb, mb, gb
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HeapMemory: str
+        :param _OffHeapMemory: 默认为b, 支持单位有 b, kb, mb, gb
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OffHeapMemory: str
+        :param _ManagedMemory: 默认为b, 支持单位有 b, kb, mb, gb
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ManagedMemory: str
+        """
+        self._CPU = None
+        self._HeapMemory = None
+        self._OffHeapMemory = None
+        self._ManagedMemory = None
+
+    @property
+    def CPU(self):
+        return self._CPU
+
+    @CPU.setter
+    def CPU(self, CPU):
+        self._CPU = CPU
+
+    @property
+    def HeapMemory(self):
+        return self._HeapMemory
+
+    @HeapMemory.setter
+    def HeapMemory(self, HeapMemory):
+        self._HeapMemory = HeapMemory
+
+    @property
+    def OffHeapMemory(self):
+        return self._OffHeapMemory
+
+    @OffHeapMemory.setter
+    def OffHeapMemory(self, OffHeapMemory):
+        self._OffHeapMemory = OffHeapMemory
+
+    @property
+    def ManagedMemory(self):
+        return self._ManagedMemory
+
+    @ManagedMemory.setter
+    def ManagedMemory(self, ManagedMemory):
+        self._ManagedMemory = ManagedMemory
+
+
+    def _deserialize(self, params):
+        self._CPU = params.get("CPU")
+        self._HeapMemory = params.get("HeapMemory")
+        self._OffHeapMemory = params.get("OffHeapMemory")
+        self._ManagedMemory = params.get("ManagedMemory")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class StopJobDescription(AbstractModel):
     """停止作业的描述信息
 
     """
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.946/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.947/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.947/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.946/README.rst` & `tencentcloud-sdk-python-oceanus-3.0.947/README.rst`

 * *Files identical despite different names*

