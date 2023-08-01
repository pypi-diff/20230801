# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.946.tar", last modified: Mon Jul 31 00:26:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.947.tar", last modified: Tue Aug  1 00:37:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.946.tar` & `tencentcloud-sdk-python-essbasic-3.0.947.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    56205 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   392627 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   393237 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:37:23.000000 tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -669,15 +669,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelGetTaskResultApi(self, request):
-        """通过发起转换任务接口（ChannelCreateConvertTaskApi）返回的任务Id查询转换任务状态，通过本接口确认转换任务是否完成。大文件转换所需的时间可能会比较长。
+        """查询转换任务的状态。转换任务Id通过发起转换任务接口（ChannelCreateConvertTaskApi）获取。
+        注意：大文件转换所需的时间可能会比较长。
 
         :param request: Request instance for ChannelGetTaskResultApi.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelGetTaskResultApiRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelGetTaskResultApiResponse`
 
         """
         try:
@@ -974,15 +975,25 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTemplates(self, request):
-        """通过此接口（DescribeTemplates）查询该第三方平台子客企业在电子签拥有的有效模板，不包括第三方平台模板
+        """通过此接口（DescribeTemplates）查询该第三方平台子客企业在电子签拥有的有效模板，不包括第三方平台模板。
+
+        > **适用场景**
+        >
+        >  该接口常用来配合“使用模板创建签署流程”接口作为前置的接口使用。
+        >  一个模板通常会包含以下结构信息
+        >- 模板基本信息
+        >- 发起方参与信息Promoter、签署参与方 Recipients，后者会在模板发起合同时用于指定参与方
+        >- 填写控件 Components
+        >- 签署控件 SignComponents
+        >- 生成模板的文件基础信息 FileInfos
 
         :param request: Request instance for DescribeTemplates.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.DescribeTemplatesRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.DescribeTemplatesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4942,16 +4942,15 @@
         r"""
         :param _ComponentId: 控件编号
 
 CreateFlowByTemplates发起合同时优先以ComponentId（不为空）填充；否则以ComponentName填充
 
 注：
 当GenerateMode=KEYWORD时，通过"^"来决定是否使用关键字整词匹配能力。
-例：
-当GenerateMode=KEYWORD时，如果传入关键字"^甲方签署^"，则会在PDF文件中有且仅有"甲方签署"关键字的地方进行对应操作。
+例：当GenerateMode=KEYWORD时，如果传入关键字"^甲方签署^"，则会在PDF文件中有且仅有"甲方签署"关键字的地方进行对应操作。
 如传入的关键字为"甲方签署"，则PDF文件中每个出现关键字的位置都会执行相应操作。
 
 创建控件时，此值为空
 查询时返回完整结构
         :type ComponentId: str
         :param _ComponentType: 如果是Component控件类型，则可选的字段为：
 TEXT - 普通文本控件，输入文本字符串；
@@ -4971,19 +4970,20 @@
 SIGN_PERSONAL_SEAL - 个人签署印章控件（使用文件发起暂不支持此类型）；
 SIGN_PAGING_SEAL - 骑缝章；若文件发起，需要对应填充ComponentPosY、ComponentWidth、ComponentHeight
 SIGN_OPINION - 签署意见控件，用户需要根据配置的签署意见内容，完成对意见内容的确认;
 SIGN_LEGAL_PERSON_SEAL - 企业法定代表人控件。
 
 表单域的控件不能作为印章和签名控件
         :type ComponentType: str
-        :param _ComponentName: 控件简称，不能超过30个字符
+        :param _ComponentName: 控件简称，不超过30个字符
         :type ComponentName: str
-        :param _ComponentRequired: 定义控件是否为必填项，默认为false
+        :param _ComponentRequired: 控件是否为必填项，
+默认为false-非必填
         :type ComponentRequired: bool
-        :param _ComponentRecipientId: 控件关联的签署方id
+        :param _ComponentRecipientId: 控件关联的参与方ID，对应Recipient结构体中的RecipientId	
         :type ComponentRecipientId: str
         :param _FileIndex: 控件所属文件的序号 (文档中文件的排列序号，从0开始)
         :type FileIndex: int
         :param _GenerateMode: 控件生成的方式：
 NORMAL - 普通控件
 FIELD - 表单域
 KEYWORD - 关键字
@@ -5114,33 +5114,44 @@
 学历控件：
   同单行文本控件约束，填写选择值中的字符串
         :type ComponentValue: str
         :param _ComponentDateFontSize: 日期签署控件的字号，默认为 12
 
 签署区日期控件会转换成图片格式并带存证，需要通过字体决定图片大小
         :type ComponentDateFontSize: int
-        :param _DocumentId: 控件所属文档的Id, 模块相关接口为空值
+        :param _DocumentId: 控件所属文档的Id, 模板相关接口为空值
         :type DocumentId: str
-        :param _ComponentDescription: 控件描述，不能超过30个字符
+        :param _ComponentDescription: 控件描述，不超过30个字符
         :type ComponentDescription: str
         :param _OffsetX: 指定关键字时横坐标偏移量，单位pt
         :type OffsetX: float
         :param _OffsetY: 指定关键字时纵坐标偏移量，单位pt
         :type OffsetY: float
         :param _ChannelComponentId: 平台企业控件ID。
 如果不为空，属于平台企业预设控件；
         :type ChannelComponentId: str
-        :param _KeywordOrder: 指定关键字排序规则，Positive-正序，Reverse-倒序。传入Positive时会根据关键字在PDF文件内的顺序进行排列。在指定KeywordIndexes时，0代表在PDF内查找内容时，查找到的第一个关键字。
+        :param _KeywordOrder: 指定关键字排序规则，
+Positive-正序，
+Reverse-倒序。
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
-        :param _KeywordIndexes: 关键字索引，可选参数，如果一个关键字在PDF文件中存在多个，可以通过关键字索引指定使用第几个关键字作为最后的结果，可指定多个索引。示例[0,2]，说明使用PDF文件内第1个和第3个关键字位置。
+        :param _KeywordIndexes: 关键字索引，如果一个关键字在PDF文件中存在多个，可以通过关键字索引指定使用第几个关键字作为最后的结果，可指定多个索引。
+示例[0,2]，说明使用PDF文件内第1个和第3个关键字位置。
         :type KeywordIndexes: list of int
         :param _Placeholder: 填写提示的内容
 注意：此字段可能返回 null，表示取不到有效值。
         :type Placeholder: str
         """
         self._ComponentId = None
         self._ComponentType = None
@@ -6965,31 +6976,41 @@
 class DescribeTemplatesRequest(AbstractModel):
     """DescribeTemplates请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId必填。
+        :param _Agent: 应用相关信息。 
+此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _TemplateId: 模板唯一标识，查询单个模板时使用
         :type TemplateId: str
-        :param _ContentType: 查询内容：0-模板列表及详情（默认），1-仅模板列表
+        :param _ContentType: 查询内容：
+0-模板列表及详情（默认），
+1-仅模板列表
         :type ContentType: int
-        :param _Limit: 查询个数，默认20，最大100；在查询列表的时候有效
+        :param _Limit: 指定每页多少条数据，如果不传默认为20，单页最大100。
         :type Limit: int
-        :param _Offset: 查询偏移位置，默认0；在查询列表的时候有效
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默从第一页返回。页码从0开始，即首页为0。
         :type Offset: int
-        :param _QueryAllComponents: 是否返回所有组件信息。默认false，只返回发起方控件；true，返回所有签署方控件
+        :param _QueryAllComponents: 是否返回所有组件信息。
+默认false，只返回发起方控件；
+true，返回所有签署方控件
         :type QueryAllComponents: bool
         :param _TemplateName: 模糊搜索模板名称，最大长度200
         :type TemplateName: str
-        :param _WithPreviewUrl: 是否获取模板预览链接
+        :param _WithPreviewUrl: 是否获取模板预览链接，
+默认false-不获取
+true-获取
         :type WithPreviewUrl: bool
-        :param _WithPdfUrl: 是否获取模板的PDF文件链接- 第三方应用集成需要开启白名单时才能使用。
+        :param _WithPdfUrl: 是否获取模板的PDF文件链接。
+默认false-不获取
+true-获取
+请联系客户经理开白后使用。
         :type WithPdfUrl: bool
         :param _ChannelTemplateId: 对应第三方应用平台企业的模板ID
         :type ChannelTemplateId: str
         :param _Operator: 操作者的信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
@@ -7126,21 +7147,21 @@
 class DescribeTemplatesResponse(AbstractModel):
     """DescribeTemplates返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Templates: 模板详情
+        :param _Templates: 模板列表
         :type Templates: list of TemplateInfo
-        :param _TotalCount: 查询总数
+        :param _TotalCount: 查询到的总数
         :type TotalCount: int
-        :param _Limit: 查询数量
+        :param _Limit: 每页多少条数据
         :type Limit: int
-        :param _Offset: 查询起始偏移
+        :param _Offset: 查询结果分页返回，此处指定第几页。页码从0开始，即首页为0。
         :type Offset: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Templates = None
         self._TotalCount = None
         self._Limit = None
@@ -9439,37 +9460,47 @@
 class OperateChannelTemplateRequest(AbstractModel):
     """OperateChannelTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.AppId必填。
+        :param _Agent: 应用相关信息。 
+此接口Agent.AppId必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
-        :param _OperateType: 操作类型，查询:"SELECT"，删除:"DELETE"，更新:"UPDATE"
+        :param _OperateType: 操作类型，
+查询:"SELECT"，
+删除:"DELETE"，
+更新:"UPDATE"
         :type OperateType: str
         :param _TemplateId: 第三方应用平台模板库模板唯一标识
         :type TemplateId: str
-        :param _ProxyOrganizationOpenIds: 合作企业方第三方机构唯一标识数据，支持多个， 用","进行分隔
+        :param _ProxyOrganizationOpenIds: 合作企业方第三方机构唯一标识数据.
+支持多个， 用","进行分隔
         :type ProxyOrganizationOpenIds: str
-        :param _AuthTag: 模板可见性, 全部可见-"all", 部分可见-"part"
+        :param _AuthTag: 模板可见性, 
+全部可见-"all",
+ 部分可见-"part"
         :type AuthTag: str
-        :param _Operator: 暂未开放
-        :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
-        :param _Available: 当OperateType=UPADATE时，可以通过设置此字段对模板启停用状态进行操作。若此字段值为0，则不会修改模板Available，1为启用模板，2为停用模板。
+        :param _Available: 当OperateType=UPADATE时，可以通过设置此字段对模板启停用状态进行操作。
+若此字段值为0，则不会修改模板Available，
+1为启用模板，
+2为停用模板。
 启用后模板可以正常领取。停用后，推送方式为【自动推送】的模板则无法被子客使用，推送方式为【手动领取】的模板则无法出现被模板库被子客领用。如果Available更新失败，会直接返回错误。
         :type Available: int
+        :param _Operator: 暂未开放
+        :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
         self._OperateType = None
         self._TemplateId = None
         self._ProxyOrganizationOpenIds = None
         self._AuthTag = None
-        self._Operator = None
         self._Available = None
+        self._Operator = None
 
     @property
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
@@ -9504,46 +9535,46 @@
         return self._AuthTag
 
     @AuthTag.setter
     def AuthTag(self, AuthTag):
         self._AuthTag = AuthTag
 
     @property
+    def Available(self):
+        return self._Available
+
+    @Available.setter
+    def Available(self, Available):
+        self._Available = Available
+
+    @property
     def Operator(self):
         warnings.warn("parameter `Operator` is deprecated", DeprecationWarning) 
 
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
         warnings.warn("parameter `Operator` is deprecated", DeprecationWarning) 
 
         self._Operator = Operator
 
-    @property
-    def Available(self):
-        return self._Available
-
-    @Available.setter
-    def Available(self, Available):
-        self._Available = Available
-
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         self._OperateType = params.get("OperateType")
         self._TemplateId = params.get("TemplateId")
         self._ProxyOrganizationOpenIds = params.get("ProxyOrganizationOpenIds")
         self._AuthTag = params.get("AuthTag")
+        self._Available = params.get("Available")
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
-        self._Available = params.get("Available")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -9559,18 +9590,23 @@
         r"""
         :param _AppId: 腾讯电子签颁发给第三方应用平台的应用ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type AppId: str
         :param _TemplateId: 第三方应用平台模板库模板唯一标识
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateId: str
-        :param _OperateResult: 描述模板可见性更改的结果，和参数中Available无关，全部成功-"all-success",部分成功-"part-success", 全部失败-"fail"失败的会在FailMessageList中展示。
+        :param _OperateResult: 描述模板可见性更改的结果，和参数中Available无关。
+全部成功-"all-success",
+部分成功-"part-success", 
+全部失败-"fail"，失败的会在FailMessageList中展示。
 注意：此字段可能返回 null，表示取不到有效值。
         :type OperateResult: str
-        :param _AuthTag: 模板可见性, 全部可见-"all", 部分可见-"part"
+        :param _AuthTag: 模板可见性, 
+全部可见-"all", 
+部分可见-"part"
 注意：此字段可能返回 null，表示取不到有效值。
         :type AuthTag: str
         :param _ProxyOrganizationOpenIds: 合作企业方第三方机构唯一标识数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProxyOrganizationOpenIds: list of str
         :param _FailMessageList: 操作失败信息数组
 注意：此字段可能返回 null，表示取不到有效值。
@@ -10151,37 +10187,46 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Recipient(AbstractModel):
-    """签署参与者信息
+    """流程中参与方的信息结构
 
     """
 
     def __init__(self):
         r"""
-        :param _RecipientId: 签署人唯一标识，在通过模板发起合同的时候对应签署方Id
+        :param _RecipientId: 签署人唯一标识，在通过模板发起合同的时候对应签署方ID
         :type RecipientId: str
-        :param _RecipientType: 参与者类型。默认为空。ENTERPRISE-企业；INDIVIDUAL-个人；PROMOTER-发起方
+        :param _RecipientType: 参与者类型，默认为空。
+ENTERPRISE-企业；
+INDIVIDUAL-个人；
+PROMOTER-发起方
         :type RecipientType: str
-        :param _Description: 描述
+        :param _Description: 描述信息	
         :type Description: str
-        :param _RoleName: 签署方备注角色名
+        :param _RoleName: 角色名称	
         :type RoleName: str
-        :param _RequireValidation: 是否需要校验，true-是，false-否
+        :param _RequireValidation: 是否需要校验，
+true-是，
+false-否
         :type RequireValidation: bool
-        :param _RequireSign: 是否必须填写，true-是，false-否
+        :param _RequireSign: 是否必须填写，
+true-是，
+false-否
         :type RequireSign: bool
-        :param _SignType: 签署类型
+        :param _SignType: 内部字段，签署类型
         :type SignType: int
         :param _RoutingOrder: 签署顺序：数字越小优先级越高
         :type RoutingOrder: int
-        :param _IsPromoter: 是否是发起方
+        :param _IsPromoter: 是否是发起方，
+true-是 
+false-否
         :type IsPromoter: bool
         """
         self._RecipientId = None
         self._RecipientType = None
         self._Description = None
         self._RoleName = None
         self._RequireValidation = None
@@ -11610,56 +11655,72 @@
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class TemplateInfo(AbstractModel):
     """此结构体 (TemplateInfo) 用于描述模板的信息。
 
+    > **模板组成**
+    >
+    >  一个模板通常会包含以下结构信息
+    >- 模板基本信息
+    >- 签署参与方 Recipients，在模板发起合同时用于指定参与方
+    >- 填写控件 Components
+    >- 签署控件 SignComponents
+
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
-        :param _Components: 模板的填充控件信息结构
+        :param _Components: 模板的填充控件列表
         :type Components: list of Component
-        :param _Recipients: 模板中的流程参与人信息
+        :param _Recipients: 模板中的签署参与方列表
         :type Recipients: list of Recipient
-        :param _SignComponents: 模板中的签署控件信息结构
+        :param _SignComponents: 模板中的签署控件列表
         :type SignComponents: list of Component
         :param _TemplateType: 模板类型：1-静默签；3-普通模板
         :type TemplateType: int
         :param _IsPromoter: 是否是发起人 ,已弃用
         :type IsPromoter: bool
         :param _Creator: 模板的创建者信息，电子签系统用户ID
         :type Creator: str
-        :param _CreatedOn: 模板创建的时间戳，单位秒
+        :param _CreatedOn: 模板创建的时间戳，格式为Unix标准时间戳（秒）
         :type CreatedOn: int
-        :param _PreviewUrl: 模板的H5预览链接,可以通过浏览器打开此链接预览模板，或者嵌入到iframe中预览模板。请求参数WithPreviewUrl=true时返回，有效期5分钟。
+        :param _PreviewUrl: 模板的H5预览链接,有效期5分钟。
+可以通过浏览器打开此链接预览模板，或者嵌入到iframe中预览模板。
+（此功能开放需要联系客户经理）
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreviewUrl: str
-        :param _PdfUrl: 第三方应用集成-模板PDF文件链接。请求参数WithPdfUrl=true时返回（此功能开放需要联系客户经理），有效期5分钟。
+        :param _PdfUrl: 第三方应用集成-模板PDF文件链接，有效期5分钟。
+请求参数WithPdfUrl=true时返回
+（此功能开放需要联系客户经理）。
 注意：此字段可能返回 null，表示取不到有效值。
         :type PdfUrl: str
-        :param _ChannelTemplateId: 关联的第三方应用平台企业模板ID
+        :param _ChannelTemplateId: 本模板关联的第三方应用平台企业模板ID
         :type ChannelTemplateId: str
-        :param _ChannelTemplateName: 关联的三方应用平台平台企业模板名称
+        :param _ChannelTemplateName: 本模板关联的三方应用平台平台企业模板名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChannelTemplateName: str
-        :param _ChannelAutoSave: 0-需要子客企业手动领取平台企业的模板(默认); 1-平台自动设置子客模板
+        :param _ChannelAutoSave: 0-需要子客企业手动领取平台企业的模板(默认); 
+1-平台自动设置子客模板
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChannelAutoSave: int
-        :param _TemplateVersion: 模板版本，全数字字符。默认为空，初始版本为yyyyMMdd001。
+        :param _TemplateVersion: 模板版本，全数字字符。
+默认为空，初始版本为yyyyMMdd001。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateVersion: str
-        :param _Available: 模板可用状态，取值：1启用（默认），2停用
+        :param _Available: 模板可用状态：
+1启用（默认）
+2停用
 注意：此字段可能返回 null，表示取不到有效值。
         :type Available: int
         """
         self._TemplateId = None
         self._TemplateName = None
         self._Description = None
         self._Components = None
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.947/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.947/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.947/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

