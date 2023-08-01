# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.946.tar", last modified: Mon Jul 31 00:32:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.947.tar", last modified: Tue Aug  1 00:52:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.946.tar` & `tencentcloud-sdk-python-mps-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99431 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13604 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1229873 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:32:27.000000 tencentcloud-sdk-python-mps-3.0.946/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99431 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1232124 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:52:30.000000 tencentcloud-sdk-python-mps-3.0.947/tencentcloud_sdk_python_mps.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-mps-3.0.946/setup.py` & `tencentcloud-sdk-python-mps-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/v20190612/mps_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.946/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.947/tencentcloud/mps/v20190612/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7651,30 +7651,35 @@
 当外层参数 Container 为 mp4 或 flv 时，可选值为：
 <li>libfdk_aac：更适合 mp4；</li>
 <li>libmp3lame：更适合 flv；</li>
 <li>mp2。</li>
 当外层参数 Container 为 hls 时，可选值为：
 <li>libfdk_aac；</li>
 <li>libmp3lame。</li>
+注意：此字段可能返回 null，表示取不到有效值。
         :type Codec: str
         :param _Bitrate: 音频流的码率，取值范围：0 和 [26, 256]，单位：kbps。 当取值为 0，表示音频码率和原始音频保持一致。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Bitrate: int
         :param _SampleRate: 音频流的采样率，可选值：
 <li>32000</li>
 <li>44100</li>
 <li>48000</li>
 单位：Hz。
+注意：此字段可能返回 null，表示取不到有效值。
         :type SampleRate: int
         :param _AudioChannel: 音频通道方式，可选值：
 <li>1：单通道</li>
 <li>2：双通道</li>
 <li>6：立体声</li>
 当媒体的封装格式是音频格式时（flac，ogg，mp3，m4a）时，声道数不允许设为立体声。
+注意：此字段可能返回 null，表示取不到有效值。
         :type AudioChannel: int
         :param _StreamSelects: 指定输出要保留的音频轨道。默认是全部保留源的。
+注意：此字段可能返回 null，表示取不到有效值。
         :type StreamSelects: list of int
         """
         self._Codec = None
         self._Bitrate = None
         self._SampleRate = None
         self._AudioChannel = None
         self._StreamSelects = None
@@ -29956,23 +29961,27 @@
         :type TEHDConfig: :class:`tencentcloud.mps.v20190612.models.TEHDConfigForUpdate`
         :param _SubtitleTemplate: 字幕流配置参数。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SubtitleTemplate: :class:`tencentcloud.mps.v20190612.models.SubtitleTemplate`
         :param _AddonAudioStream: 外挂音轨参数。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AddonAudioStream: list of MediaInputInfo
+        :param _StdExtInfo: 转码扩展字段。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StdExtInfo: str
         """
         self._Container = None
         self._RemoveVideo = None
         self._RemoveAudio = None
         self._VideoTemplate = None
         self._AudioTemplate = None
         self._TEHDConfig = None
         self._SubtitleTemplate = None
         self._AddonAudioStream = None
+        self._StdExtInfo = None
 
     @property
     def Container(self):
         return self._Container
 
     @Container.setter
     def Container(self, Container):
@@ -30030,14 +30039,22 @@
     def AddonAudioStream(self):
         return self._AddonAudioStream
 
     @AddonAudioStream.setter
     def AddonAudioStream(self, AddonAudioStream):
         self._AddonAudioStream = AddonAudioStream
 
+    @property
+    def StdExtInfo(self):
+        return self._StdExtInfo
+
+    @StdExtInfo.setter
+    def StdExtInfo(self, StdExtInfo):
+        self._StdExtInfo = StdExtInfo
+
 
     def _deserialize(self, params):
         self._Container = params.get("Container")
         self._RemoveVideo = params.get("RemoveVideo")
         self._RemoveAudio = params.get("RemoveAudio")
         if params.get("VideoTemplate") is not None:
             self._VideoTemplate = VideoTemplateInfoForUpdate()
@@ -30053,14 +30070,15 @@
             self._SubtitleTemplate._deserialize(params.get("SubtitleTemplate"))
         if params.get("AddonAudioStream") is not None:
             self._AddonAudioStream = []
             for item in params.get("AddonAudioStream"):
                 obj = MediaInputInfo()
                 obj._deserialize(item)
                 self._AddonAudioStream.append(obj)
+        self._StdExtInfo = params.get("StdExtInfo")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -33238,25 +33256,30 @@
     """AWS S3存储输入
 
     """
 
     def __init__(self):
         r"""
         :param _S3Bucket: S3 bucket。
+注意：此字段可能返回 null，表示取不到有效值。
         :type S3Bucket: str
         :param _S3Region: S3 bucket 对应的区域，目前支持：  
 us-east-1  
 eu-west-3
 
+注意：此字段可能返回 null，表示取不到有效值。
         :type S3Region: str
         :param _S3Object: S3 bucket 中的媒体资源路径。
+注意：此字段可能返回 null，表示取不到有效值。
         :type S3Object: str
         :param _S3SecretId: AWS 内网访问 媒体资源的秘钥id。
+注意：此字段可能返回 null，表示取不到有效值。
         :type S3SecretId: str
         :param _S3SecretKey: AWS 内网访问 媒体资源的秘钥key。
+注意：此字段可能返回 null，表示取不到有效值。
         :type S3SecretKey: str
         """
         self._S3Bucket = None
         self._S3Region = None
         self._S3Object = None
         self._S3SecretId = None
         self._S3SecretKey = None
@@ -35191,32 +35214,38 @@
     """字幕流配置参数。
 
     """
 
     def __init__(self):
         r"""
         :param _Path: 要压制到视频中的字幕文件地址。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Path: str
         :param _StreamIndex: 指定要压制到视频中的字幕轨道，如果有指定Path，则Path 优先级更高。Path 和 StreamIndex 至少指定一个。
+注意：此字段可能返回 null，表示取不到有效值。
         :type StreamIndex: int
         :param _FontType: 字体类型，
 <li>hei.ttf：黑体</li>
 <li>song.ttf：宋体</li>
 <li>simkai.ttf：楷体</li>
 <li>arial.ttf：仅支持英文</li>
 默认hei.ttf
+注意：此字段可能返回 null，表示取不到有效值。
         :type FontType: str
         :param _FontSize: 字体大小，格式：Npx，N 为数值，不指定则以字幕文件中为准。
+注意：此字段可能返回 null，表示取不到有效值。
         :type FontSize: str
         :param _FontColor: 字体颜色，格式：0xRRGGBB，默认值：0xFFFFFF（白色）
+注意：此字段可能返回 null，表示取不到有效值。
         :type FontColor: str
         :param _FontAlpha: 文字透明度，取值范围：(0, 1]
 <li>0：完全透明</li>
 <li>1：完全不透明</li>
 默认值：1。
+注意：此字段可能返回 null，表示取不到有效值。
         :type FontAlpha: float
         """
         self._Path = None
         self._StreamIndex = None
         self._FontType = None
         self._FontSize = None
         self._FontColor = None
@@ -35533,16 +35562,18 @@
 
     def __init__(self):
         r"""
         :param _Type: 极速高清类型，可选值：
 <li>TEHD-100：极速高清-100（视频极速高清）。</li>
 <li>TEHD-200：极速高清-200（音频极速高清）。</li>
 不填代表不修改。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Type: str
         :param _MaxVideoBitrate: 视频码率上限，不填代表不修改。
+注意：此字段可能返回 null，表示取不到有效值。
         :type MaxVideoBitrate: int
         """
         self._Type = None
         self._MaxVideoBitrate = None
 
     @property
     def Type(self):
@@ -37978,49 +38009,59 @@
         r"""
         :param _Codec: 视频流的编码格式，可选值：
 <li>libx264：H.264 编码</li>
 <li>libx265：H.265 编码</li>
 <li>av1：AOMedia Video 1 编码</li>
 注意：目前 H.265 编码必须指定分辨率，并且需要在 640*480 以内。
 注意：av1 编码容器目前只支持 mp4 。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Codec: str
         :param _Fps: 视频帧率，取值范围：[0, 120]，单位：Hz。
 当取值为 0，表示帧率和原始视频保持一致。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Fps: int
         :param _Bitrate: 视频流的码率，取值范围：0 和 [128, 35000]，单位：kbps。
 当取值为 0，表示视频码率和原始视频保持一致。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Bitrate: int
         :param _ResolutionAdaptive: 分辨率自适应，可选值：
 <li>open：开启，此时，Width 代表视频的长边，Height 表示视频的短边；</li>
 <li>close：关闭，此时，Width 代表视频的宽度，Height 表示视频的高度。</li>
 注意：自适应模式时，Width不能小于Height。
+注意：此字段可能返回 null，表示取不到有效值。
         :type ResolutionAdaptive: str
         :param _Width: 视频流宽度（或长边）的最大值，取值范围：0 和 [128, 4096]，单位：px。
 <li>当 Width、Height 均为 0，则分辨率同源；</li>
 <li>当 Width 为 0，Height 非 0，则 Width 按比例缩放；</li>
 <li>当 Width 非 0，Height 为 0，则 Height 按比例缩放；</li>
 <li>当 Width、Height 均非 0，则分辨率按用户指定。</li>
+注意：此字段可能返回 null，表示取不到有效值。
         :type Width: int
         :param _Height: 视频流高度（或短边）的最大值，取值范围：0 和 [128, 4096]，单位：px。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Height: int
         :param _Gop: 关键帧 I 帧之间的间隔，取值范围：0 和 [1, 100000]，单位：帧数。当填 0 时，系统将自动设置 gop 长度。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Gop: int
         :param _FillType: 填充方式，当视频流配置宽高参数与原始视频的宽高比不一致时，对转码的处理方式，即为“填充”。可选填充方式：
 <li> stretch：拉伸，对每一帧进行拉伸，填满整个画面，可能导致转码后的视频被“压扁“或者“拉长“；</li>
 <li>black：留黑，保持视频宽高比不变，边缘剩余部分使用黑色填充。</li>
 <li>white：留白，保持视频宽高比不变，边缘剩余部分使用白色填充。</li>
 <li>gauss：高斯模糊，保持视频宽高比不变，边缘剩余部分使用高斯模糊填充。</li>
+注意：此字段可能返回 null，表示取不到有效值。
         :type FillType: str
         :param _Vcrf: 视频恒定码率控制因子。取值范围为[0, 51]，填0表示禁用该参数。
 如果没有特殊需求，不建议指定该参数。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Vcrf: int
         :param _ContentAdaptStream: 内容自适应编码。可选值：
 <li>0：不开启</li>
 <li>1：开启</li>
 默认值: 0.   当开启该参数时，将会自适应生成多个不同分辨率，不同码率的码流， 其中VideoTemplate的宽和高为多个码流中的最大分辨率，VideoTemplate中的码率为多个码流中的最高码率， VideoTemplate中的vcrf为多个码流中的最高质量。 当不设置分辨率、码率和vcrf时， ContentAdaptStream 参数生成的最高分辨率为视频源的分辨率，视频质量为接近vmaf95分。 若要开启该参数或了解计费细节, 请联系您的腾讯云商务。
+注意：此字段可能返回 null，表示取不到有效值。
         :type ContentAdaptStream: int
         """
         self._Codec = None
         self._Fps = None
         self._Bitrate = None
         self._ResolutionAdaptive = None
         self._Width = None
```

### Comparing `tencentcloud-sdk-python-mps-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.947/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.946/README.rst` & `tencentcloud-sdk-python-mps-3.0.947/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.946/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.947/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

