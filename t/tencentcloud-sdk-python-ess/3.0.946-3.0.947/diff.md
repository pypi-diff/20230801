# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.946.tar", last modified: Mon Jul 31 00:26:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.947.tar", last modified: Tue Aug  1 00:37:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.946.tar` & `tencentcloud-sdk-python-ess-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    65988 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   454866 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    66079 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   471423 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:37:18.000000 tencentcloud-sdk-python-ess-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.946/setup.py` & `tencentcloud-sdk-python-ess-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -602,16 +602,16 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreatePrepareFlow(self, request):
         """创建快速发起流程
-        适用场景：用户通过API 合同文件及签署信息，并可通过我们返回的URL在页面完成签署控件等信息的编辑与确认，快速发起合同.
-        注：该接口文件的resourceId 是通过上传文件之后获取的。
+        <br/>适用场景：用户通过API 合同文件及签署信息，并可通过我们返回的URL在页面完成签署控件等信息的编辑与确认，快速发起合同.
+        <br/>注：该接口文件的resourceId 是通过上传文件之后获取的。
 
         :param request: Request instance for CreatePrepareFlow.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreatePrepareFlowRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreatePrepareFlowResponse`
 
         """
         try:
@@ -1396,15 +1396,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateIntegrationEmployees(self, request):
-        """更新员工信息(姓名，手机号，邮件、部门)，用户实名后无法更改姓名与手机号
+        """更新员工信息(姓名，手机号，邮件、部门)，用户实名后无法更改姓名与手机号。
+        可进行批量操作，Employees中的userID与openID二选一必填
 
         :param request: Request instance for UpdateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.UpdateIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.UpdateIntegrationEmployeesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.947/tencentcloud/ess/v20201111/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1279,15 +1279,15 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Component(AbstractModel):
-    """模板控件信息
+    """模板/流程中控件信息，可以是填充控件或签署控件
 
     """
 
     def __init__(self):
         r"""
         :param _ComponentType: 如果是Component填写控件类型，则可选的字段为：
 TEXT - 普通文本控件，输入文本字符串；
@@ -1307,33 +1307,36 @@
 SIGN_PERSONAL_SEAL - 个人签署印章控件（使用文件发起暂不支持此类型）；
 SIGN_PAGING_SEAL - 骑缝章；若文件发起，需要对应填充ComponentPosY、ComponentWidth、ComponentHeight
 SIGN_OPINION - 签署意见控件，用户需要根据配置的签署意见内容，完成对意见内容的确认；
 SIGN_LEGAL_PERSON_SEAL - 企业法定代表人控件。
 
 表单域的控件不能作为印章和签名控件
         :type ComponentType: str
-        :param _FileIndex: 控件所属文件的序号（取值为：0-N）。目前单文件的情况下，值是0
+        :param _FileIndex: 控件所属文件的序号（取值为：0-N）。
+目前单文件的情况下，值是0
         :type FileIndex: int
         :param _ComponentHeight: 参数控件高度，单位pt
         :type ComponentHeight: float
         :param _ComponentWidth: 参数控件宽度，单位pt
         :type ComponentWidth: float
         :param _ComponentPage: 参数控件所在页码，取值为：1-N
         :type ComponentPage: int
         :param _ComponentPosX: 参数控件X位置，单位pt
         :type ComponentPosX: float
         :param _ComponentPosY: 参数控件Y位置，单位pt
         :type ComponentPosY: float
-        :param _ComponentId: 查询时返回控件唯一Id。使用文件发起合同时用于GenerateMode==KEYWORD 指定关键字
+        :param _ComponentId: 控件唯一ID。
+或使用文件发起合同时用于GenerateMode==KEYWORD 指定关键字
         :type ComponentId: str
-        :param _ComponentName: 查询时返回控件名。使用文件发起合同时用于GenerateMode==FIELD 指定表单域名称
+        :param _ComponentName: 控件名。
+或使用文件发起合同时用于GenerateMode==FIELD 指定表单域名称
         :type ComponentName: str
-        :param _ComponentRequired: 是否必选，默认为false
+        :param _ComponentRequired: 是否必选，默认为false-非必选
         :type ComponentRequired: bool
-        :param _ComponentRecipientId: 控件关联的签署人ID
+        :param _ComponentRecipientId: 控件关联的参与方ID，对应Recipient结构体中的RecipientId
         :type ComponentRecipientId: str
         :param _ComponentExtra: 扩展参数：
 为JSON格式。
 
 ComponentType为FILL_IMAGE时，支持以下参数：
 NotMakeImageCenter：bool。是否设置图片居中。false：居中（默认）。 true: 不居中
 FillMethod: int. 填充方式。0-铺满（默认）；1-等比例缩放
@@ -1357,15 +1360,15 @@
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
 参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
 
 ComponentType为SIGN_SEAL类型时，支持以下参数：
 1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
 参数样例："ComponentExtra":"{\"PageRanges\":[{\"BeginPage\":1,\"EndPage\":-1}]}"
         :type ComponentExtra: str
-        :param _IsFormType: 是否是表单域类型，默认不false-不是
+        :param _IsFormType: 是否是表单域类型，默认false-不是
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsFormType: bool
         :param _ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
 CHECK_BOX - true/false
 FILL_IMAGE、ATTACHMENT - 附件的FileId，需要通过UploadFiles接口上传获取
@@ -1443,33 +1446,53 @@
         :type ComponentValue: str
         :param _GenerateMode: NORMAL 正常模式，使用坐标制定签署控件位置
 FIELD 表单域，需使用ComponentName指定表单域名称
 KEYWORD 关键字，使用ComponentId指定关键字
         :type GenerateMode: str
         :param _ComponentDateFontSize: 日期签署控件的字号，默认为 12
         :type ComponentDateFontSize: int
-        :param _ChannelComponentId: 第三方应用集成平台模板控件 id 标识
+        :param _ChannelComponentId: 第三方应用集成平台模板控件 ID 标识
         :type ChannelComponentId: str
         :param _OffsetX: 指定关键字时横坐标偏移量，单位pt
 注意：此字段可能返回 null，表示取不到有效值。
         :type OffsetX: float
         :param _OffsetY: 指定关键字时纵坐标偏移量，单位pt
 注意：此字段可能返回 null，表示取不到有效值。
         :type OffsetY: float
-        :param _ChannelComponentSource: 第三方应用集成中子客企业控件来源。0-平台指定；1-用户自定义
+        :param _ChannelComponentSource: 第三方应用集成中子客企业控件来源。
+0-平台指定；
+1-用户自定义
         :type ChannelComponentSource: int
-        :param _KeywordOrder: 指定关键字排序规则，Positive-正序，Reverse-倒序。传入Positive时会根据关键字在PDF文件内的顺序进行排列。在指定KeywordIndexes时，0代表在PDF内查找内容时，查找到的第一个关键字。
+        :param _KeywordOrder: 指定关键字排序规则，Positive-正序，Reverse-倒序。
+传入Positive时会根据关键字在PDF文件内的顺序进行排列。在指定KeywordIndexes时，0代表在PDF内查找内容时，查找到的第一个关键字。
 传入Reverse时会根据关键字在PDF文件内的反序进行排列。在指定KeywordIndexes时，0代表在PDF内查找内容时，查找到的最后一个关键字。
         :type KeywordOrder: str
-        :param _KeywordPage: 指定关键字页码，可选参数，指定页码后，将只在指定的页码内查找关键字，非该页码的关键字将不会查询出来
+        :param _KeywordPage: 指定关键字页码。
+指定页码后，将只在指定的页码内查找关键字，非该页码的关键字将不会查询出来
         :type KeywordPage: int
-        :param _RelativeLocation: 关键字位置模式，Middle-居中，Below-正下方，Right-正右方，LowerRight-右上角，UpperRight-右下角。示例：如果设置Middle的关键字盖章，则印章的中心会和关键字的中心重合，如果设置Below，则印章在关键字的正下方
+        :param _RelativeLocation: 关键字位置模式，
+Middle-居中，
+Below-正下方，
+Right-正右方，
+LowerRight-右上角，
+UpperRight-右下角。
+示例：如果设置Middle的关键字盖章，则印章的中心会和关键字的中心重合，如果设置Below，则印章在关键字的正下方
         :type RelativeLocation: str
-        :param _KeywordIndexes: 关键字索引，可选参数，如果一个关键字在PDF文件中存在多个，可以通过关键字索引指定使用第几个关键字作为最后的结果，可指定多个索引。示例：[0,2]，说明使用PDF文件内第1个和第3个关键字位置。
+        :param _KeywordIndexes: 关键字索引。
+如果一个关键字在PDF文件中存在多个，可以通过关键字索引指定使用第几个关键字作为最后的结果，可指定多个索引。
+示例：[0,2]，说明使用PDF文件内第1个和第3个关键字位置。
         :type KeywordIndexes: list of int
+        :param _LockComponentValue: 是否锁定控件值不允许编辑（嵌入式发起使用）
+<br/>默认false：不锁定控件值，允许在页面编辑控件值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LockComponentValue: bool
+        :param _ForbidMoveAndDelete: 是否禁止移动和删除控件
+<br/>默认false，不禁止移动和删除控件
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ForbidMoveAndDelete: bool
         """
         self._ComponentType = None
         self._FileIndex = None
         self._ComponentHeight = None
         self._ComponentWidth = None
         self._ComponentPage = None
         self._ComponentPosX = None
@@ -1487,14 +1510,16 @@
         self._OffsetX = None
         self._OffsetY = None
         self._ChannelComponentSource = None
         self._KeywordOrder = None
         self._KeywordPage = None
         self._RelativeLocation = None
         self._KeywordIndexes = None
+        self._LockComponentValue = None
+        self._ForbidMoveAndDelete = None
 
     @property
     def ComponentType(self):
         return self._ComponentType
 
     @ComponentType.setter
     def ComponentType(self, ComponentType):
@@ -1680,14 +1705,30 @@
     def KeywordIndexes(self):
         return self._KeywordIndexes
 
     @KeywordIndexes.setter
     def KeywordIndexes(self, KeywordIndexes):
         self._KeywordIndexes = KeywordIndexes
 
+    @property
+    def LockComponentValue(self):
+        return self._LockComponentValue
+
+    @LockComponentValue.setter
+    def LockComponentValue(self, LockComponentValue):
+        self._LockComponentValue = LockComponentValue
+
+    @property
+    def ForbidMoveAndDelete(self):
+        return self._ForbidMoveAndDelete
+
+    @ForbidMoveAndDelete.setter
+    def ForbidMoveAndDelete(self, ForbidMoveAndDelete):
+        self._ForbidMoveAndDelete = ForbidMoveAndDelete
+
 
     def _deserialize(self, params):
         self._ComponentType = params.get("ComponentType")
         self._FileIndex = params.get("FileIndex")
         self._ComponentHeight = params.get("ComponentHeight")
         self._ComponentWidth = params.get("ComponentWidth")
         self._ComponentPage = params.get("ComponentPage")
@@ -1706,14 +1747,16 @@
         self._OffsetX = params.get("OffsetX")
         self._OffsetY = params.get("OffsetY")
         self._ChannelComponentSource = params.get("ChannelComponentSource")
         self._KeywordOrder = params.get("KeywordOrder")
         self._KeywordPage = params.get("KeywordPage")
         self._RelativeLocation = params.get("RelativeLocation")
         self._KeywordIndexes = params.get("KeywordIndexes")
+        self._LockComponentValue = params.get("LockComponentValue")
+        self._ForbidMoveAndDelete = params.get("ForbidMoveAndDelete")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2286,29 +2329,33 @@
         :param _Operator: 操作者信息
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _EmbedType: WEB嵌入资源类型。
 <br/>CREATE_SEAL: 创建印章
 <br/>PREVIEW_SEAL_LIST：预览印章列表
 <br/>PREVIEW_SEAL_DETAIL：预览印章详情
 <br/>EXTEND_SERVICE：拓展服务
-
+<br/>PREVIEW_FLOW：预览合同
+<br/>PREVIEW_FLOW_DETAIL：查看合同详情
         :type EmbedType: str
         :param _BusinessId: WEB嵌入的业务资源ID
 <br/>PREVIEW_SEAL_DETAIL，必填，取值为印章id
         :type BusinessId: str
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Reviewer: 抄送方信息
         :type Reviewer: :class:`tencentcloud.ess.v20201111.models.ReviewerInfo`
+        :param _Option: 个性化参数
+        :type Option: :class:`tencentcloud.ess.v20201111.models.EmbedUrlOption`
         """
         self._Operator = None
         self._EmbedType = None
         self._BusinessId = None
         self._Agent = None
         self._Reviewer = None
+        self._Option = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -2342,27 +2389,38 @@
     def Reviewer(self):
         return self._Reviewer
 
     @Reviewer.setter
     def Reviewer(self, Reviewer):
         self._Reviewer = Reviewer
 
+    @property
+    def Option(self):
+        return self._Option
+
+    @Option.setter
+    def Option(self, Option):
+        self._Option = Option
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._EmbedType = params.get("EmbedType")
         self._BusinessId = params.get("BusinessId")
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         if params.get("Reviewer") is not None:
             self._Reviewer = ReviewerInfo()
             self._Reviewer._deserialize(params.get("Reviewer"))
+        if params.get("Option") is not None:
+            self._Option = EmbedUrlOption()
+            self._Option._deserialize(params.get("Option"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3293,14 +3351,168 @@
 
     def _deserialize(self, params):
         self._FlowGroupId = params.get("FlowGroupId")
         self._FlowIds = params.get("FlowIds")
         self._RequestId = params.get("RequestId")
 
 
+class CreateFlowOption(AbstractModel):
+    """创建合同个性化参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _CanEditFlow: 是否允许修改发起合同时确认弹窗的合同信息（合同名称、合同类型、签署截止时间），若不允许编辑，则表单字段将被禁止输入。
+<br/>true：允许编辑（默认），<br/>false：不允许编辑<br/>默认：false：不允许编辑
+        :type CanEditFlow: bool
+        :param _CanEditFormField: 是否允许编辑模版控件
+<br/>true:允许编辑模版控件信息
+<br/>false:不允许编辑模版控件信息
+<br/>默认false:不允许编辑模版控件信息
+        :type CanEditFormField: bool
+        :param _HideShowFlowName: 发起页面隐藏合同名称展示
+<br/>true:发起页面隐藏合同名称展示
+<br/>false:发起页面不隐藏合同名称展示
+<br/>默认false:发起页面不隐藏合同名称展示
+        :type HideShowFlowName: bool
+        :param _HideShowFlowType: 发起页面隐藏合同类型展示
+<br/>true:发起页面隐藏合同类型展示
+<br/>false:发起页面不隐藏合同类型展示
+<br/>默认false:发起页面不隐藏合同类型展示
+
+        :type HideShowFlowType: bool
+        :param _HideShowDeadline: 发起页面隐藏合同截止日期展示
+<br/>true:发起页面隐藏合同截止日期展示
+<br/>false:发起页面不隐藏合同截止日期展示
+<br/>默认false:发起页面不隐藏合同截止日期展示
+        :type HideShowDeadline: bool
+        :param _CanSkipAddApprover: 发起页面允许跳过添加签署人环节
+<br/>true:发起页面允许跳过添加签署人环节
+<br/>false:发起页面不允许跳过添加签署人环节
+<br/>默认false:发起页面不允许跳过添加签署人环节
+
+        :type CanSkipAddApprover: bool
+        :param _SkipUploadFile: 文件发起页面跳过文件上传步骤
+<br/>true:文件发起页面跳过文件上传步骤
+<br/>false:文件发起页面不跳过文件上传步骤
+<br/>默认false:文件发起页面不跳过文件上传步骤
+        :type SkipUploadFile: bool
+        :param _ForbidEditFillComponent: 禁止编辑填写控件
+<br/>true:禁止编辑填写控件
+<br/>false:允许编辑填写控件
+<br/>默认false:允许编辑填写控件
+        :type ForbidEditFillComponent: bool
+        :param _CustomCreateFlowDescription: 定制化发起合同弹窗的描述信息，描述信息最长500
+
+        :type CustomCreateFlowDescription: str
+        """
+        self._CanEditFlow = None
+        self._CanEditFormField = None
+        self._HideShowFlowName = None
+        self._HideShowFlowType = None
+        self._HideShowDeadline = None
+        self._CanSkipAddApprover = None
+        self._SkipUploadFile = None
+        self._ForbidEditFillComponent = None
+        self._CustomCreateFlowDescription = None
+
+    @property
+    def CanEditFlow(self):
+        return self._CanEditFlow
+
+    @CanEditFlow.setter
+    def CanEditFlow(self, CanEditFlow):
+        self._CanEditFlow = CanEditFlow
+
+    @property
+    def CanEditFormField(self):
+        return self._CanEditFormField
+
+    @CanEditFormField.setter
+    def CanEditFormField(self, CanEditFormField):
+        self._CanEditFormField = CanEditFormField
+
+    @property
+    def HideShowFlowName(self):
+        return self._HideShowFlowName
+
+    @HideShowFlowName.setter
+    def HideShowFlowName(self, HideShowFlowName):
+        self._HideShowFlowName = HideShowFlowName
+
+    @property
+    def HideShowFlowType(self):
+        return self._HideShowFlowType
+
+    @HideShowFlowType.setter
+    def HideShowFlowType(self, HideShowFlowType):
+        self._HideShowFlowType = HideShowFlowType
+
+    @property
+    def HideShowDeadline(self):
+        return self._HideShowDeadline
+
+    @HideShowDeadline.setter
+    def HideShowDeadline(self, HideShowDeadline):
+        self._HideShowDeadline = HideShowDeadline
+
+    @property
+    def CanSkipAddApprover(self):
+        return self._CanSkipAddApprover
+
+    @CanSkipAddApprover.setter
+    def CanSkipAddApprover(self, CanSkipAddApprover):
+        self._CanSkipAddApprover = CanSkipAddApprover
+
+    @property
+    def SkipUploadFile(self):
+        return self._SkipUploadFile
+
+    @SkipUploadFile.setter
+    def SkipUploadFile(self, SkipUploadFile):
+        self._SkipUploadFile = SkipUploadFile
+
+    @property
+    def ForbidEditFillComponent(self):
+        return self._ForbidEditFillComponent
+
+    @ForbidEditFillComponent.setter
+    def ForbidEditFillComponent(self, ForbidEditFillComponent):
+        self._ForbidEditFillComponent = ForbidEditFillComponent
+
+    @property
+    def CustomCreateFlowDescription(self):
+        return self._CustomCreateFlowDescription
+
+    @CustomCreateFlowDescription.setter
+    def CustomCreateFlowDescription(self, CustomCreateFlowDescription):
+        self._CustomCreateFlowDescription = CustomCreateFlowDescription
+
+
+    def _deserialize(self, params):
+        self._CanEditFlow = params.get("CanEditFlow")
+        self._CanEditFormField = params.get("CanEditFormField")
+        self._HideShowFlowName = params.get("HideShowFlowName")
+        self._HideShowFlowType = params.get("HideShowFlowType")
+        self._HideShowDeadline = params.get("HideShowDeadline")
+        self._CanSkipAddApprover = params.get("CanSkipAddApprover")
+        self._SkipUploadFile = params.get("SkipUploadFile")
+        self._ForbidEditFillComponent = params.get("ForbidEditFillComponent")
+        self._CustomCreateFlowDescription = params.get("CustomCreateFlowDescription")
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
 class CreateFlowRemindsRequest(AbstractModel):
     """CreateFlowReminds请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4726,36 +4938,81 @@
         r"""
         :param _Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _ResourceId: 资源Id，通过多文件上传（UploadFiles）接口获得
         :type ResourceId: str
         :param _FlowName: 合同名称
         :type FlowName: str
-        :param _Unordered: 是否顺序签署(true:无序签,false:顺序签)
+        :param _Unordered: 是否顺序签署
+true:无序签
+false:顺序签
         :type Unordered: bool
         :param _Deadline: 签署流程的签署截止时间。
-值为unix时间戳,精确到秒,不传默认为当前时间一年后
+值为unix时间戳,精确到秒
+不传默认为当前时间一年后
         :type Deadline: int
-        :param _UserFlowTypeId: 用户自定义合同类型
+        :param _UserFlowTypeId: 用户自定义合同类型Id
+该id为电子签企业内的合同类型id
         :type UserFlowTypeId: str
         :param _Approvers: 签署流程参与者信息，最大限制50方
         :type Approvers: list of FlowCreateApprover
-        :param _IntelligentStatus: 打开智能添加填写区(默认开启，打开:"OPEN" 关闭："CLOSE")
+        :param _IntelligentStatus: 打开智能添加填写区
+(默认开启，打开:"OPEN"
+ 关闭："CLOSE"
         :type IntelligentStatus: str
+        :param _ResourceType: 资源类型，
+1：文件，
+2：模板
+不传默认为1：文件
+目前仅支持文件
+        :type ResourceType: int
+        :param _Components: 发起方填写控件
+该类型控件由发起方完成填写
+        :type Components: :class:`tencentcloud.ess.v20201111.models.Component`
+        :param _FlowOption: 发起合同个性化参数
+用于满足创建及页面操作过程中的个性化要求
+具体定制化内容详见数据接口说明
+        :type FlowOption: :class:`tencentcloud.ess.v20201111.models.CreateFlowOption`
+        :param _NeedSignReview: 是否开启发起方签署审核
+true:开启发起方签署审核
+false:不开启发起方签署审核
+默认false:不开启发起方签署审核
+        :type NeedSignReview: bool
+        :param _NeedCreateReview: 开启发起方发起合同审核
+true:开启发起方发起合同审核
+false:不开启发起方发起合同审核
+默认false:不开启发起方发起合同审核
+        :type NeedCreateReview: bool
+        :param _UserData: 用户自定义参数
+        :type UserData: str
+        :param _FlowId: 合同id,用于通过已web页面发起的合同id快速生成一个web发起合同链接
+        :type FlowId: str
+        :param _FlowType: 合同类型名称
+该字段用于客户自定义合同类型
+建议使用时指定合同类型，便于之后合同分类以及查看
+        :type FlowType: str
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填	
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._ResourceId = None
         self._FlowName = None
         self._Unordered = None
         self._Deadline = None
         self._UserFlowTypeId = None
         self._Approvers = None
         self._IntelligentStatus = None
+        self._ResourceType = None
+        self._Components = None
+        self._FlowOption = None
+        self._NeedSignReview = None
+        self._NeedCreateReview = None
+        self._UserData = None
+        self._FlowId = None
+        self._FlowType = None
         self._Agent = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
@@ -4815,14 +5072,78 @@
         return self._IntelligentStatus
 
     @IntelligentStatus.setter
     def IntelligentStatus(self, IntelligentStatus):
         self._IntelligentStatus = IntelligentStatus
 
     @property
+    def ResourceType(self):
+        return self._ResourceType
+
+    @ResourceType.setter
+    def ResourceType(self, ResourceType):
+        self._ResourceType = ResourceType
+
+    @property
+    def Components(self):
+        return self._Components
+
+    @Components.setter
+    def Components(self, Components):
+        self._Components = Components
+
+    @property
+    def FlowOption(self):
+        return self._FlowOption
+
+    @FlowOption.setter
+    def FlowOption(self, FlowOption):
+        self._FlowOption = FlowOption
+
+    @property
+    def NeedSignReview(self):
+        return self._NeedSignReview
+
+    @NeedSignReview.setter
+    def NeedSignReview(self, NeedSignReview):
+        self._NeedSignReview = NeedSignReview
+
+    @property
+    def NeedCreateReview(self):
+        return self._NeedCreateReview
+
+    @NeedCreateReview.setter
+    def NeedCreateReview(self, NeedCreateReview):
+        self._NeedCreateReview = NeedCreateReview
+
+    @property
+    def UserData(self):
+        return self._UserData
+
+    @UserData.setter
+    def UserData(self, UserData):
+        self._UserData = UserData
+
+    @property
+    def FlowId(self):
+        return self._FlowId
+
+    @FlowId.setter
+    def FlowId(self, FlowId):
+        self._FlowId = FlowId
+
+    @property
+    def FlowType(self):
+        return self._FlowType
+
+    @FlowType.setter
+    def FlowType(self, FlowType):
+        self._FlowType = FlowType
+
+    @property
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
         self._Agent = Agent
 
@@ -4839,14 +5160,26 @@
         if params.get("Approvers") is not None:
             self._Approvers = []
             for item in params.get("Approvers"):
                 obj = FlowCreateApprover()
                 obj._deserialize(item)
                 self._Approvers.append(obj)
         self._IntelligentStatus = params.get("IntelligentStatus")
+        self._ResourceType = params.get("ResourceType")
+        if params.get("Components") is not None:
+            self._Components = Component()
+            self._Components._deserialize(params.get("Components"))
+        if params.get("FlowOption") is not None:
+            self._FlowOption = CreateFlowOption()
+            self._FlowOption._deserialize(params.get("FlowOption"))
+        self._NeedSignReview = params.get("NeedSignReview")
+        self._NeedCreateReview = params.get("NeedCreateReview")
+        self._UserData = params.get("UserData")
+        self._FlowId = params.get("FlowId")
+        self._FlowType = params.get("FlowType")
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
@@ -7549,15 +7882,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 调用方员工/经办人信息
 UserId 必填，在企业控制台组织架构中可以查到员工的UserId
-注：请保证对应
+注：请保证员工有相关的角色权限
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _Agent: 代理相关应用信息
 如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _ContentType: 查询内容类型
 0-模板列表及详情（默认）
 1-仅模板列表
@@ -9008,14 +9341,65 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class EmbedUrlOption(AbstractModel):
+    """个性化参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ShowFlowDetailComponent: 合同详情预览，允许展示控件信息
+<br/>true：允许在合同详情页展示控件
+<br/>false：不允许在合同详情页展示控件
+<br/>默认false，合同详情页不展示控件
+        :type ShowFlowDetailComponent: bool
+        :param _ShowTemplateComponent: 模版预览，允许展示模版控件信息
+<br/>true：允许在模版预览页展示控件
+<br/>false：不允许在模版预览页展示控件
+<br/>默认false，模版预览页不展示控件
+        :type ShowTemplateComponent: bool
+        """
+        self._ShowFlowDetailComponent = None
+        self._ShowTemplateComponent = None
+
+    @property
+    def ShowFlowDetailComponent(self):
+        return self._ShowFlowDetailComponent
+
+    @ShowFlowDetailComponent.setter
+    def ShowFlowDetailComponent(self, ShowFlowDetailComponent):
+        self._ShowFlowDetailComponent = ShowFlowDetailComponent
+
+    @property
+    def ShowTemplateComponent(self):
+        return self._ShowTemplateComponent
+
+    @ShowTemplateComponent.setter
+    def ShowTemplateComponent(self, ShowTemplateComponent):
+        self._ShowTemplateComponent = ShowTemplateComponent
+
+
+    def _deserialize(self, params):
+        self._ShowFlowDetailComponent = params.get("ShowFlowDetailComponent")
+        self._ShowTemplateComponent = params.get("ShowTemplateComponent")
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
 class ExtendAuthInfo(AbstractModel):
     """授权服务信息
 
     """
 
     def __init__(self):
         r"""
@@ -9378,21 +9762,21 @@
 class FileInfo(AbstractModel):
     """模板中文件的信息结构
 
     """
 
     def __init__(self):
         r"""
-        :param _FileId: 文件Id
+        :param _FileId: 文件ID
         :type FileId: str
         :param _FileName: 文件名
         :type FileName: str
         :param _FileSize: 文件大小，单位为Byte
         :type FileSize: int
-        :param _CreatedOn: 文件上传时间，10位时间戳（精确到秒）
+        :param _CreatedOn: 文件上传时间，格式为Unix标准时间戳（秒）
         :type CreatedOn: int
         """
         self._FileId = None
         self._FileName = None
         self._FileSize = None
         self._CreatedOn = None
 
@@ -9489,28 +9873,29 @@
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class FillApproverInfo(AbstractModel):
     """补充签署人信息
     - RecipientId 必须指定
-    -  通过企业自定义账号ID补充签署人时，ApproverSource 和 CustomUserId 必填
-    - 通过二要素（姓名/手机号）补充签署人时，ApproverName 和 ApproverMobile 必填
+    -  通过企业自定义账号ID补充签署人时，ApproverSource 和 CustomUserId 必填，ApproverSource取值：WEWORKAPP
+    - 通过二要素（姓名/手机号）补充签署人时，ApproverName 和 ApproverMobile 必填，ApproverSource设置为空
 
     """
 
     def __init__(self):
         r"""
         :param _RecipientId: 对应模板中的参与方ID
         :type RecipientId: str
         :param _ApproverSource: 签署人来源
 WEWORKAPP: 企业微信
+<br/>仅【企微或签】时指定WEWORKAPP
         :type ApproverSource: str
         :param _CustomUserId: 企业自定义账号ID
-WEWORKAPP场景下指企业自有应用获取企微明文的userid
+<br/>当ApproverSource为WEWORKAPP的企微或签场景下，必须指企业自有应用获取企微明文的userid
         :type CustomUserId: str
         :param _ApproverName: 补充签署人姓名
         :type ApproverName: str
         :param _ApproverMobile: 补充签署人手机号
         :type ApproverMobile: str
         """
         self._RecipientId = None
@@ -10161,59 +10546,83 @@
         r"""
         :param _ApproverType: 参与者类型：
 0：企业
 1：个人
 3：企业静默签署
 注：类型为3（企业静默签署）时，会默认完成该签署方的签署。静默签署仅进行盖章操作，不能是手写签名。
         :type ApproverType: int
-        :param _OrganizationName: 如果签署方为企业，需要填入企业全称
+        :param _OrganizationName: 签署人企业名称
+<br/>当approverType=1 或 approverType=3时，必须指定
+
+
         :type OrganizationName: str
         :param _ApproverName: 签署方经办人姓名
+<br/>在未指定签署人电子签UserId情况下，为必填参数
         :type ApproverName: str
         :param _ApproverMobile: 签署方经办人手机号码
+<br/>在未指定签署人电子签UserId情况下，为必填参数
+
         :type ApproverMobile: str
         :param _ApproverIdCardType: 签署方经办人证件类型ID_CARD 身份证
 HONGKONG_AND_MACAO 港澳居民来往内地通行证
 HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证(格式同居民身份证)
         :type ApproverIdCardType: str
         :param _ApproverIdCardNumber: 签署方经办人证件号码
         :type ApproverIdCardNumber: str
         :param _RecipientId: 签署方经办人在模板中的参与方ID
+<br/>模版发起合同时，该参数为必填项
+<br/>文件发起合同是，该参数无序传值
+
         :type RecipientId: str
         :param _VerifyChannel: 签署意愿确认渠道,WEIXINAPP:人脸识别
         :type VerifyChannel: list of str
-        :param _NotifyType: 是否发送短信，sms--短信通知，none--不通知，默认为sms；发起方=签署方时不发送短信
+        :param _NotifyType: 是否发送短信
+<br/>sms--短信通知
+<br/>none--不通知
+<br/>默认为sms
+<br/>发起方=签署方时不发送短信
         :type NotifyType: str
         :param _IsFullText: 合同强制需要阅读全文，无需传此参数
         :type IsFullText: bool
         :param _PreReadTime: 合同的强制预览时间：3~300s，未指定则按合同页数计算
         :type PreReadTime: int
-        :param _UserId: 签署方经办人的用户ID,和签署方经办人姓名+手机号+证件必须有一个。
+        :param _UserId: 签署方经办人的电子签用户ID
+<br/>当未指定签署人姓名+手机号的情况下，该字段毕传
+
         :type UserId: str
         :param _Required: 当前只支持true，默认为true
         :type Required: bool
-        :param _ApproverSource: 签署人用户来源,企微侧用户请传入：WEWORKAPP
+        :param _ApproverSource: 签署人用户来源
+<br/>企微侧用户请传入：WEWORKAPP
         :type ApproverSource: str
-        :param _CustomApproverTag: 企业签署方或签标识，客户自定义，64位长度。用于发起含有或签签署人的合同。或签参与人必须有此字段。合同内不同或签参与人CustomApproverTag需要保证唯一。如果或签签署人为本方企微参与人，ApproverSource参数需要指定WEWORKAPP
+        :param _CustomApproverTag: 企业签署方或签标识，客户自定义，64位长度
+<br>用于发起含有或签签署人的合同。或签参与人必须有此字段。
+<br/>合同内不同或签参与人CustomApproverTag需要保证唯一。
+<br/>如果或签签署人为本方企微参与人，ApproverSource参数需要指定WEWORKAPP
         :type CustomApproverTag: str
         :param _RegisterInfo: 快速注册相关信息，目前暂未开放！
         :type RegisterInfo: :class:`tencentcloud.ess.v20201111.models.RegisterInfo`
         :param _ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.ess.v20201111.models.ApproverOption`
         :param _JumpUrl: 签署完前端跳转的url，暂未使用
         :type JumpUrl: str
         :param _SignId: 签署ID
 - 发起流程时系统自动补充
 - 创建签署链接时，可以通过查询详情接口获得签署人的SignId，然后可传入此值为该签署人创建签署链接，无需再传姓名、手机号、证件号等其他信息
         :type SignId: str
-        :param _ApproverNeedSignReview: 当前签署方进行签署操作是否需要企业内部审批，true 则为需要。为个人签署方时则由发起方企业审核。
+        :param _ApproverNeedSignReview: 当前签署方进行签署操作是否需要企业内部审批
+<br>true 则为需要
+<br/>false,无序企业内部审批（默认）
+<br/>为个人签署方时则由发起方企业审核。
         :type ApproverNeedSignReview: bool
         :param _SignComponents: 签署人签署控件
+<br/>文件发起时，可通过该参数为签署人指定签署控件类型以及位置
         :type SignComponents: list of Component
         :param _Components: 签署人填写控件
+<br/>文件发起时，可通过该参数为签署人指定填写控件类型以及位置
         :type Components: list of Component
         :param _ComponentLimitType: 签署方控件类型为 SIGN_SIGNATURE时，可以指定签署方签名方式
 	HANDWRITE – 手写签名
 	OCR_ESIGN -- AI智能识别手写签名
 	ESIGN -- 个人印章类型
 	SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
         :type ComponentLimitType: list of str
@@ -12216,17 +12625,17 @@
         :type SignerName: str
         :param _SignTime: 签署时间戳，单位秒
         :type SignTime: int
         :param _SignAlgorithm: 签名算法
         :type SignAlgorithm: str
         :param _CertSn: 签名证书序列号
         :type CertSn: str
-        :param _CertNotBefore: 证书起始时间戳，单位秒
+        :param _CertNotBefore: 证书起始时间戳，单位毫秒
         :type CertNotBefore: int
-        :param _CertNotAfter: 证书过期时间戳，单位秒
+        :param _CertNotAfter: 证书过期时间戳，单位毫秒
         :type CertNotAfter: int
         :param _ComponentPosX: 签名域横坐标，单位pt
         :type ComponentPosX: float
         :param _ComponentPosY: 签名域纵坐标，单位pt
         :type ComponentPosY: float
         :param _ComponentWidth: 签名域宽度，单位pt
         :type ComponentWidth: float
@@ -12375,45 +12784,55 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Recipient(AbstractModel):
-    """签署参与者信息
+    """流程中参与方的信息结构
 
     """
 
     def __init__(self):
         r"""
-        :param _RecipientId: 签署参与者ID
+        :param _RecipientId: 签署参与者ID，唯一标识
         :type RecipientId: str
-        :param _RecipientType: 参与者类型。默认为空。ENTERPRISE-企业；INDIVIDUAL-个人；PROMOTER-发起方
+        :param _RecipientType: 参与者类型。
+默认为空。
+ENTERPRISE-企业；
+INDIVIDUAL-个人；
+PROMOTER-发起方
         :type RecipientType: str
         :param _Description: 描述信息
         :type Description: str
         :param _RoleName: 角色名称
         :type RoleName: str
-        :param _RequireValidation: 是否需要验证，默认为false
+        :param _RequireValidation: 是否需要验证，
+默认为false-不需要验证
         :type RequireValidation: bool
-        :param _RequireSign: 是否需要签署，默认为true
+        :param _RequireSign: 是否需要签署，
+默认为true-需要签署
         :type RequireSign: bool
-        :param _RoutingOrder: 添加序列，0～N
+        :param _RoutingOrder: 此参与方添加的顺序，从0～N
         :type RoutingOrder: int
-        :param _RequireDelivery: 是否需要发送，默认为true
+        :param _RequireDelivery: 是否需要发送，
+默认为true-需要发送
         :type RequireDelivery: bool
         :param _Email: 邮箱地址
         :type Email: str
         :param _Mobile: 电话号码
         :type Mobile: str
-        :param _UserId: 关联的用户ID
+        :param _UserId: 关联的用户ID，电子签系统的用户ID
         :type UserId: str
-        :param _DeliveryMethod: 发送方式。默认为EMAIL。EMAIL-邮件；MOBILE-手机短信；WECHAT-微信通知
+        :param _DeliveryMethod: 发送方式，默认为EMAIL。
+EMAIL-邮件；
+MOBILE-手机短信；
+WECHAT-微信通知
         :type DeliveryMethod: str
-        :param _RecipientExtra: 附属信息
+        :param _RecipientExtra: 参与方的一些附属信息，json格式
         :type RecipientExtra: str
         """
         self._RecipientId = None
         self._RecipientType = None
         self._Description = None
         self._RoleName = None
         self._RequireValidation = None
@@ -12979,18 +13398,75 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class SealInfo(AbstractModel):
-    """模板结构体中的印章信息
+    """模板中指定的印章信息
 
     """
 
+    def __init__(self):
+        r"""
+        :param _SealId: 印章ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SealId: str
+        :param _SealType: 印章类型。LEGAL_PERSON_SEAL: 法定代表人章；
+ORGANIZATIONSEAL：企业印章；
+OFFICIAL：企业公章；
+CONTRACT：合同专用章
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SealType: str
+        :param _SealName: 印章名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SealName: str
+        """
+        self._SealId = None
+        self._SealType = None
+        self._SealName = None
+
+    @property
+    def SealId(self):
+        return self._SealId
+
+    @SealId.setter
+    def SealId(self, SealId):
+        self._SealId = SealId
+
+    @property
+    def SealType(self):
+        return self._SealType
+
+    @SealType.setter
+    def SealType(self, SealType):
+        self._SealType = SealType
+
+    @property
+    def SealName(self):
+        return self._SealName
+
+    @SealName.setter
+    def SealName(self, SealName):
+        self._SealName = SealName
+
+
+    def _deserialize(self, params):
+        self._SealId = params.get("SealId")
+        self._SealType = params.get("SealType")
+        self._SealName = params.get("SealName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
 
 class SignQrCode(AbstractModel):
     """一码多扫签署二维码对象
 
     """
 
     def __init__(self):
@@ -13676,64 +14152,81 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class TemplateInfo(AbstractModel):
-    """企业模板的信息结构
+    """此结构体 (TemplateInfo) 用于描述模板的信息。
+
+    > **模板组成**
+    >
+    >  一个模板通常会包含以下结构信息
+    >- 模板基本信息
+    >- 发起方参与信息Promoter、签署参与方 Recipients，后者会在模板发起合同时用于指定参与方
+    >- 填写控件 Components
+    >- 签署控件 SignComponents
+    >- 生成模板的文件基础信息 FileInfos
 
     """
 
     def __init__(self):
         r"""
-        :param _TemplateId: 模板ID
+        :param _TemplateId: 模板ID，模板的唯一标识
         :type TemplateId: str
-        :param _TemplateName: 模板名字
+        :param _TemplateName: 模板名
         :type TemplateName: str
         :param _Description: 模板描述信息
         :type Description: str
         :param _DocumentResourceIds: 模板关联的资源ID列表
         :type DocumentResourceIds: list of str
-        :param _FileInfos: 返回的文件信息结构
+        :param _FileInfos: 生成模板的文件基础信息
         :type FileInfos: list of FileInfo
         :param _AttachmentResourceIds: 附件关联的资源ID
         :type AttachmentResourceIds: list of str
         :param _SignOrder: 签署顺序
+无序 -1
+有序为序列数字 0,1,2
         :type SignOrder: list of int
-        :param _Recipients: 签署参与者的信息
+        :param _Recipients: 模板中的签署参与方列表
         :type Recipients: list of Recipient
-        :param _Components: 模板信息结构
+        :param _Components: 模板的填充控件列表
         :type Components: list of Component
-        :param _SignComponents: 签署区模板信息结构
+        :param _SignComponents: 模板中的签署控件列表
         :type SignComponents: list of Component
-        :param _Status: 模板状态(-1:不可用；0:草稿态；1:正式态)
+        :param _Status: 模板状态
+-1:不可用
+0:草稿态
+1:正式态，可以正常使用
         :type Status: int
-        :param _Creator: 模板的创建人UserId
+        :param _Creator: 模板的创建者信息，电子签系统用户ID
         :type Creator: str
-        :param _CreatedOn: 模板创建的时间戳，单位秒
+        :param _CreatedOn: 模板创建的时间戳，格式为Unix标准时间戳（秒）
         :type CreatedOn: int
-        :param _Promoter: 发起人角色信息
+        :param _Promoter: 发起方参与信息Promoter
         :type Promoter: :class:`tencentcloud.ess.v20201111.models.Recipient`
-        :param _TemplateType: 模板类型
-取值：
+        :param _TemplateType: 模板类型：
 1  静默签,
 3  普通模板
         :type TemplateType: int
-        :param _Available: 模板可用状态，取值：1启用（默认），2停用
+        :param _Available: 模板可用状态：
+1 启用（默认）
+2 停用
         :type Available: int
-        :param _OrganizationId: 创建模板的机构id
+        :param _OrganizationId: 创建模板的企业ID，电子签的机构ID
         :type OrganizationId: str
         :param _PreviewUrl: 模板预览链接，有效时间5分钟
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreviewUrl: str
         :param _TemplateVersion: 模板版本。默认为空时，全数字字符，初始版本为yyyyMMdd001。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateVersion: str
-        :param _Published: 模板是否已发布。true-已发布；false-未发布
+        :param _Published: 模板是否已发布：
+true-已发布
+false-未发布
 注意：此字段可能返回 null，表示取不到有效值。
         :type Published: bool
         :param _TemplateSeals: 模板内部指定的印章列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateSeals: list of SealInfo
         :param _Seals: 模板内部指定的印章列表
 注意：此字段可能返回 null，表示取不到有效值。
@@ -14121,15 +14614,15 @@
 class UpdateIntegrationEmployeesRequest(AbstractModel):
     """UpdateIntegrationEmployees请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Operator: 操作人信息，userId必填
+        :param _Operator: 当前用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为YUFU；
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _Employees: 员工信息，不超过100个。
 根据UserId或OpenId更新员工，必填一个，优先UserId。
 可更新Mobile、DisplayName、Email和Department.DepartmentId字段，其他字段暂不支持
         :type Employees: list of Staff
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId需填充子企业Id
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.947/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.947/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.946/README.rst` & `tencentcloud-sdk-python-ess-3.0.947/README.rst`

 * *Files identical despite different names*

