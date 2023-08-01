# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.946.tar", last modified: Mon Jul 31 00:39:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.947.tar", last modified: Tue Aug  1 00:59:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.946.tar` & `tencentcloud-sdk-python-tts-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5572 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23747 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5922 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:39:14.000000 tencentcloud-sdk-python-tts-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23733 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5922 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:59:33.000000 tencentcloud-sdk-python-tts-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-tts-3.0.946/setup.py` & `tencentcloud-sdk-python-tts-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/v20190823/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,15 +498,15 @@
     def __init__(self):
         r"""
         :param _Text: 合成语音的源文本，按UTF-8编码统一计算。
 中文最大支持150个汉字（全角标点符号算一个汉字）；英文最大支持500个字母（半角标点符号算一个字母）。
         :type Text: str
         :param _SessionId: 一次请求对应一个SessionId，会原样返回，建议传入类似于uuid的字符串防止重复。
         :type SessionId: str
-        :param _Volume: 音量大小，范围：[0，10]，分别对应11个等级的音量，默认为0，代表正常音量。没有静音选项。
+        :param _Volume: 音量大小，范围[0，10]，对应音量大小。默认为0，代表正常音量，值越大音量越高。
         :type Volume: float
         :param _Speed: 语速，范围：[-2，6]，分别对应不同语速：<li>-2代表0.6倍</li><li>-1代表0.8倍</li><li>0代表1.0倍（默认）</li><li>1代表1.2倍</li><li>2代表1.5倍</li><li>6代表2.5倍</li>如果需要更细化的语速，可以保留小数点后 2 位，例如0.5 1.1 1.8等。<br>参数值与实际语速转换，可参考[代码示例](https://sdk-1300466766.cos.ap-shanghai.myqcloud.com/sample/speed_sample.tar.gz)
         :type Speed: float
         :param _ProjectId: 项目id，用户自定义，默认为0。
         :type ProjectId: int
         :param _ModelType: 模型类型，1-默认模型。
         :type ModelType: int
```

### Comparing `tencentcloud-sdk-python-tts-3.0.946/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.947/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.946/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.947/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.947/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.946/README.rst` & `tencentcloud-sdk-python-tts-3.0.947/README.rst`

 * *Files identical despite different names*

