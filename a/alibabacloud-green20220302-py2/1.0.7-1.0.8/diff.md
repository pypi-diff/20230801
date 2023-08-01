# Comparing `tmp/alibabacloud_green20220302_py2-1.0.7.tar.gz` & `tmp/alibabacloud_green20220302_py2-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302_py2-1.0.7.tar", last modified: Mon Jul 17 05:43:45 2023, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302_py2-1.0.8.tar", last modified: Tue Aug  1 12:11:43 2023, max compression
```

## Comparing `alibabacloud_green20220302_py2-1.0.7.tar` & `alibabacloud_green20220302_py2-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9927 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)    41590 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2023-07-17 05:43:45.000000 alibabacloud_green20220302_py2-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:11:43.000000 alibabacloud_green20220302_py2-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-08-01 12:11:43.000000 alibabacloud_green20220302_py2-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:11:43.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12160 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)    60692 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:11:43.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-08-01 12:11:43.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-01 12:11:43.000000 alibabacloud_green20220302_py2-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-08-01 12:11:42.000000 alibabacloud_green20220302_py2-1.0.8/setup.py
```

### Comparing `alibabacloud_green20220302_py2-1.0.7/LICENSE` & `alibabacloud_green20220302_py2-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.7/PKG-INFO` & `alibabacloud_green20220302_py2-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302_py2
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302_py2-1.0.7/README-CN.md` & `alibabacloud_green20220302_py2-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.7/README.md` & `alibabacloud_green20220302_py2-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -158,14 +158,74 @@
             self.call_api(params, req, runtime)
         )
 
     def text_moderation(self, request):
         runtime = util_models.RuntimeOptions()
         return self.text_moderation_with_options(request, runtime)
 
+    def video_moderation_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.service):
+            body['Service'] = request.service
+        if not UtilClient.is_unset(request.service_parameters):
+            body['ServiceParameters'] = request.service_parameters
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='VideoModeration',
+            version='2022-03-02',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            green_20220302_models.VideoModerationResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def video_moderation(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.video_moderation_with_options(request, runtime)
+
+    def video_moderation_result_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.service):
+            body['Service'] = request.service
+        if not UtilClient.is_unset(request.service_parameters):
+            body['ServiceParameters'] = request.service_parameters
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='VideoModerationResult',
+            version='2022-03-02',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            green_20220302_models.VideoModerationResultResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def video_moderation_result(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.video_moderation_result_with_options(request, runtime)
+
     def voice_moderation_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service):
             body['Service'] = request.service
         if not UtilClient.is_unset(request.service_parameters):
             body['ServiceParameters'] = request.service_parameters
```

### Comparing `alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -716,14 +716,554 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = TextModerationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class VideoModerationRequest(TeaModel):
+    def __init__(self, service=None, service_parameters=None):
+        self.service = service  # type: str
+        self.service_parameters = service_parameters  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VideoModerationRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.service is not None:
+            result['Service'] = self.service
+        if self.service_parameters is not None:
+            result['ServiceParameters'] = self.service_parameters
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Service') is not None:
+            self.service = m.get('Service')
+        if m.get('ServiceParameters') is not None:
+            self.service_parameters = m.get('ServiceParameters')
+        return self
+
+
+class VideoModerationResponseBodyData(TeaModel):
+    def __init__(self, task_id=None):
+        self.task_id = task_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VideoModerationResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class VideoModerationResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
+        self.code = code  # type: int
+        self.data = data  # type: VideoModerationResponseBodyData
+        self.message = message  # type: str
+        # Id of the request
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = VideoModerationResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class VideoModerationResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: VideoModerationResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = VideoModerationResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class VideoModerationResultRequest(TeaModel):
+    def __init__(self, service=None, service_parameters=None):
+        self.service = service  # type: str
+        self.service_parameters = service_parameters  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VideoModerationResultRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.service is not None:
+            result['Service'] = self.service
+        if self.service_parameters is not None:
+            result['ServiceParameters'] = self.service_parameters
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Service') is not None:
+            self.service = m.get('Service')
+        if m.get('ServiceParameters') is not None:
+            self.service_parameters = m.get('ServiceParameters')
+        return self
+
+
+class VideoModerationResultResponseBodyDataAudioResultSliceDetails(TeaModel):
+    def __init__(self, end_time=None, end_timestamp=None, extend=None, labels=None, risk_tips=None, risk_words=None,
+                 score=None, start_time=None, start_timestamp=None, text=None, url=None):
+        self.end_time = end_time  # type: long
+        self.end_timestamp = end_timestamp  # type: long
+        self.extend = extend  # type: str
+        self.labels = labels  # type: str
+        self.risk_tips = risk_tips  # type: str
+        self.risk_words = risk_words  # type: str
+        self.score = score  # type: float
+        self.start_time = start_time  # type: long
+        self.start_timestamp = start_timestamp  # type: long
+        self.text = text  # type: str
+        self.url = url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponseBodyDataAudioResultSliceDetails, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.end_timestamp is not None:
+            result['EndTimestamp'] = self.end_timestamp
+        if self.extend is not None:
+            result['Extend'] = self.extend
+        if self.labels is not None:
+            result['Labels'] = self.labels
+        if self.risk_tips is not None:
+            result['RiskTips'] = self.risk_tips
+        if self.risk_words is not None:
+            result['RiskWords'] = self.risk_words
+        if self.score is not None:
+            result['Score'] = self.score
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.start_timestamp is not None:
+            result['StartTimestamp'] = self.start_timestamp
+        if self.text is not None:
+            result['Text'] = self.text
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('EndTimestamp') is not None:
+            self.end_timestamp = m.get('EndTimestamp')
+        if m.get('Extend') is not None:
+            self.extend = m.get('Extend')
+        if m.get('Labels') is not None:
+            self.labels = m.get('Labels')
+        if m.get('RiskTips') is not None:
+            self.risk_tips = m.get('RiskTips')
+        if m.get('RiskWords') is not None:
+            self.risk_words = m.get('RiskWords')
+        if m.get('Score') is not None:
+            self.score = m.get('Score')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('StartTimestamp') is not None:
+            self.start_timestamp = m.get('StartTimestamp')
+        if m.get('Text') is not None:
+            self.text = m.get('Text')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class VideoModerationResultResponseBodyDataAudioResult(TeaModel):
+    def __init__(self, slice_details=None):
+        self.slice_details = slice_details  # type: list[VideoModerationResultResponseBodyDataAudioResultSliceDetails]
+
+    def validate(self):
+        if self.slice_details:
+            for k in self.slice_details:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponseBodyDataAudioResult, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['SliceDetails'] = []
+        if self.slice_details is not None:
+            for k in self.slice_details:
+                result['SliceDetails'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.slice_details = []
+        if m.get('SliceDetails') is not None:
+            for k in m.get('SliceDetails'):
+                temp_model = VideoModerationResultResponseBodyDataAudioResultSliceDetails()
+                self.slice_details.append(temp_model.from_map(k))
+        return self
+
+
+class VideoModerationResultResponseBodyDataFrameResultFramesResultsResult(TeaModel):
+    def __init__(self, confidence=None, label=None):
+        self.confidence = confidence  # type: float
+        self.label = label  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponseBodyDataFrameResultFramesResultsResult, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.confidence is not None:
+            result['Confidence'] = self.confidence
+        if self.label is not None:
+            result['Label'] = self.label
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Confidence') is not None:
+            self.confidence = m.get('Confidence')
+        if m.get('Label') is not None:
+            self.label = m.get('Label')
+        return self
+
+
+class VideoModerationResultResponseBodyDataFrameResultFramesResults(TeaModel):
+    def __init__(self, result=None, service=None):
+        self.result = result  # type: list[VideoModerationResultResponseBodyDataFrameResultFramesResultsResult]
+        self.service = service  # type: str
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponseBodyDataFrameResultFramesResults, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['Result'].append(k.to_map() if k else None)
+        if self.service is not None:
+            result['Service'] = self.service
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.result = []
+        if m.get('Result') is not None:
+            for k in m.get('Result'):
+                temp_model = VideoModerationResultResponseBodyDataFrameResultFramesResultsResult()
+                self.result.append(temp_model.from_map(k))
+        if m.get('Service') is not None:
+            self.service = m.get('Service')
+        return self
+
+
+class VideoModerationResultResponseBodyDataFrameResultFrames(TeaModel):
+    def __init__(self, offset=None, results=None, temp_url=None):
+        self.offset = offset  # type: float
+        self.results = results  # type: list[VideoModerationResultResponseBodyDataFrameResultFramesResults]
+        self.temp_url = temp_url  # type: str
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponseBodyDataFrameResultFrames, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.offset is not None:
+            result['Offset'] = self.offset
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        if self.temp_url is not None:
+            result['TempUrl'] = self.temp_url
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Offset') is not None:
+            self.offset = m.get('Offset')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = VideoModerationResultResponseBodyDataFrameResultFramesResults()
+                self.results.append(temp_model.from_map(k))
+        if m.get('TempUrl') is not None:
+            self.temp_url = m.get('TempUrl')
+        return self
+
+
+class VideoModerationResultResponseBodyDataFrameResult(TeaModel):
+    def __init__(self, frame_num=None, frames=None):
+        self.frame_num = frame_num  # type: int
+        self.frames = frames  # type: list[VideoModerationResultResponseBodyDataFrameResultFrames]
+
+    def validate(self):
+        if self.frames:
+            for k in self.frames:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponseBodyDataFrameResult, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.frame_num is not None:
+            result['FrameNum'] = self.frame_num
+        result['Frames'] = []
+        if self.frames is not None:
+            for k in self.frames:
+                result['Frames'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('FrameNum') is not None:
+            self.frame_num = m.get('FrameNum')
+        self.frames = []
+        if m.get('Frames') is not None:
+            for k in m.get('Frames'):
+                temp_model = VideoModerationResultResponseBodyDataFrameResultFrames()
+                self.frames.append(temp_model.from_map(k))
+        return self
+
+
+class VideoModerationResultResponseBodyData(TeaModel):
+    def __init__(self, audio_result=None, data_id=None, frame_result=None, live_id=None):
+        self.audio_result = audio_result  # type: VideoModerationResultResponseBodyDataAudioResult
+        self.data_id = data_id  # type: str
+        self.frame_result = frame_result  # type: VideoModerationResultResponseBodyDataFrameResult
+        self.live_id = live_id  # type: str
+
+    def validate(self):
+        if self.audio_result:
+            self.audio_result.validate()
+        if self.frame_result:
+            self.frame_result.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.audio_result is not None:
+            result['AudioResult'] = self.audio_result.to_map()
+        if self.data_id is not None:
+            result['DataId'] = self.data_id
+        if self.frame_result is not None:
+            result['FrameResult'] = self.frame_result.to_map()
+        if self.live_id is not None:
+            result['LiveId'] = self.live_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AudioResult') is not None:
+            temp_model = VideoModerationResultResponseBodyDataAudioResult()
+            self.audio_result = temp_model.from_map(m['AudioResult'])
+        if m.get('DataId') is not None:
+            self.data_id = m.get('DataId')
+        if m.get('FrameResult') is not None:
+            temp_model = VideoModerationResultResponseBodyDataFrameResult()
+            self.frame_result = temp_model.from_map(m['FrameResult'])
+        if m.get('LiveId') is not None:
+            self.live_id = m.get('LiveId')
+        return self
+
+
+class VideoModerationResultResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
+        self.code = code  # type: int
+        self.data = data  # type: VideoModerationResultResponseBodyData
+        self.message = message  # type: str
+        # Id of the request
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = VideoModerationResultResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class VideoModerationResultResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: VideoModerationResultResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(VideoModerationResultResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = VideoModerationResultResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class VoiceModerationRequest(TeaModel):
     def __init__(self, service=None, service_parameters=None):
         self.service = service  # type: str
         self.service_parameters = service_parameters  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_green20220302_py2-1.0.7/alibabacloud_green20220302_py2.egg-info/PKG-INFO` & `alibabacloud_green20220302_py2-1.0.8/alibabacloud_green20220302_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302-py2
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302_py2-1.0.7/setup.py` & `alibabacloud_green20220302_py2-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302_py2.
 
-Created on 17/07/2023
+Created on 01/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

