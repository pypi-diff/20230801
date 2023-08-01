# Comparing `tmp/tencentcloud-sdk-python-live-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.946.tar", last modified: Mon Jul 31 00:31:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.947.tar", last modified: Tue Aug  1 00:51:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.946.tar` & `tencentcloud-sdk-python-live-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20054 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   154723 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)   756776 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20054 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   154723 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)   758493 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-01 00:51:26.000000 tencentcloud-sdk-python-live-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-live-3.0.946/setup.py` & `tencentcloud-sdk-python-live-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.947/tencentcloud/live/v20180801/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1667,18 +1667,21 @@
 当LayoutParams.InputType=0(音视频)/4(纯音频)/5(纯视频)时，该值为需要混流的流名称。
 当LayoutParams.InputType=2(图片)/3(画布)时，该值仅用作标识输入，可用类似Canvas1、Pictrue1的名称。
         :type InputStreamName: str
         :param _LayoutParams: 输入流布局参数。
         :type LayoutParams: :class:`tencentcloud.live.v20180801.models.CommonMixLayoutParams`
         :param _CropParams: 输入流裁剪参数。
         :type CropParams: :class:`tencentcloud.live.v20180801.models.CommonMixCropParams`
+        :param _PortraitSegmentParams: 抠图参数。
+        :type PortraitSegmentParams: :class:`tencentcloud.live.v20180801.models.MixPortraitSegmentParams`
         """
         self._InputStreamName = None
         self._LayoutParams = None
         self._CropParams = None
+        self._PortraitSegmentParams = None
 
     @property
     def InputStreamName(self):
         return self._InputStreamName
 
     @InputStreamName.setter
     def InputStreamName(self, InputStreamName):
@@ -1696,23 +1699,34 @@
     def CropParams(self):
         return self._CropParams
 
     @CropParams.setter
     def CropParams(self, CropParams):
         self._CropParams = CropParams
 
+    @property
+    def PortraitSegmentParams(self):
+        return self._PortraitSegmentParams
+
+    @PortraitSegmentParams.setter
+    def PortraitSegmentParams(self, PortraitSegmentParams):
+        self._PortraitSegmentParams = PortraitSegmentParams
+
 
     def _deserialize(self, params):
         self._InputStreamName = params.get("InputStreamName")
         if params.get("LayoutParams") is not None:
             self._LayoutParams = CommonMixLayoutParams()
             self._LayoutParams._deserialize(params.get("LayoutParams"))
         if params.get("CropParams") is not None:
             self._CropParams = CommonMixCropParams()
             self._CropParams._deserialize(params.get("CropParams"))
+        if params.get("PortraitSegmentParams") is not None:
+            self._PortraitSegmentParams = MixPortraitSegmentParams()
+            self._PortraitSegmentParams._deserialize(params.get("PortraitSegmentParams"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3395,14 +3409,15 @@
 1：慢直播。
         :type IsDelayLive: int
         :param _HlsSpecialParam: HLS专属录制参数。
         :type HlsSpecialParam: :class:`tencentcloud.live.v20180801.models.HlsSpecialParam`
         :param _Mp3Param: Mp3录制参数，开启Mp3录制时设置。
         :type Mp3Param: :class:`tencentcloud.live.v20180801.models.RecordParam`
         :param _RemoveWatermark: 是否去除水印，类型为慢直播时此参数无效。
+如果为false，则录制水印流或转码流；如果为true，则录制原始流。
         :type RemoveWatermark: bool
         :param _FlvSpecialParam: FLV 录制特殊参数。
         :type FlvSpecialParam: :class:`tencentcloud.live.v20180801.models.FlvSpecialParam`
         """
         self._TemplateName = None
         self._Description = None
         self._FlvParam = None
@@ -17943,14 +17958,55 @@
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
+class MixPortraitSegmentParams(AbstractModel):
+    """混流抠图参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Color: 抠图背景颜色，
+常用的颜色有：
+红色：0xcc0033。
+黄色：0xcc9900。
+绿色：0xcccc33。
+蓝色：0x99CCFF。
+黑色：0x000000。
+白色：0xFFFFFF。
+灰色：0x999999。
+        :type Color: str
+        """
+        self._Color = None
+
+    @property
+    def Color(self):
+        return self._Color
+
+    @Color.setter
+    def Color(self, Color):
+        self._Color = Color
+
+
+    def _deserialize(self, params):
+        self._Color = params.get("Color")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ModifyLiveCallbackTemplateRequest(AbstractModel):
     """ModifyLiveCallbackTemplate请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-live-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.947/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.947/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.946/README.rst` & `tencentcloud-sdk-python-live-3.0.947/README.rst`

 * *Files identical despite different names*

