# Comparing `tmp/tencentcloud-sdk-python-mna-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-mna-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mna-3.0.946.tar", last modified: Mon Jul 31 00:32:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mna-3.0.947.tar", last modified: Tue Aug  1 00:52:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mna-3.0.946.tar` & `tencentcloud-sdk-python-mna-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/v20210119/
--rw-r--r--   0 root         (0) root         (0)    12133 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/v20210119/mna_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/v20210119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/v20210119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    66678 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/v20210119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud_sdk_python_mna.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud_sdk_python_mna.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud_sdk_python_mna.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud_sdk_python_mna.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/tencentcloud_sdk_python_mna.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:32:10.000000 tencentcloud-sdk-python-mna-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/v20210119/
+-rw-r--r--   0 root         (0) root         (0)    12133 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/v20210119/mna_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/v20210119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/v20210119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    67068 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/v20210119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud_sdk_python_mna.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud_sdk_python_mna.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud_sdk_python_mna.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud_sdk_python_mna.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/tencentcloud_sdk_python_mna.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:52:14.000000 tencentcloud-sdk-python-mna-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-mna-3.0.946/setup.py` & `tencentcloud-sdk-python-mna-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mna-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/v20210119/mna_client.py` & `tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/v20210119/mna_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/v20210119/errorcodes.py` & `tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/v20210119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.946/tencentcloud/mna/v20210119/models.py` & `tencentcloud-sdk-python-mna-3.0.947/tencentcloud/mna/v20210119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1522,18 +1522,24 @@
         r"""
         :param _PageSize: 每页显示记录数，PageSize、PageNumber值均为-1 时，按照1页无限制条数匹配所有设备
         :type PageSize: int
         :param _PageNumber: 当前查看页码，PageSize、PageNumber值均为-1 时，按照1页无限制条数匹配所有设备
         :type PageNumber: int
         :param _Keyword: 搜索设备的关键字（ID或者设备名），为空时匹配所有设备
         :type Keyword: str
+        :param _DeviceType: DeviceType
+不传：返回所有设备；
+1:自有设备；
+2:三方设备
+        :type DeviceType: int
         """
         self._PageSize = None
         self._PageNumber = None
         self._Keyword = None
+        self._DeviceType = None
 
     @property
     def PageSize(self):
         return self._PageSize
 
     @PageSize.setter
     def PageSize(self, PageSize):
@@ -1551,19 +1557,28 @@
     def Keyword(self):
         return self._Keyword
 
     @Keyword.setter
     def Keyword(self, Keyword):
         self._Keyword = Keyword
 
+    @property
+    def DeviceType(self):
+        return self._DeviceType
+
+    @DeviceType.setter
+    def DeviceType(self, DeviceType):
+        self._DeviceType = DeviceType
+
 
     def _deserialize(self, params):
         self._PageSize = params.get("PageSize")
         self._PageNumber = params.get("PageNumber")
         self._Keyword = params.get("Keyword")
+        self._DeviceType = params.get("DeviceType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-mna-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-mna-3.0.947/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mna
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Mna SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mna-3.0.946/tencentcloud_sdk_python_mna.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mna-3.0.947/tencentcloud_sdk_python_mna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mna
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Mna SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mna-3.0.946/README.rst` & `tencentcloud-sdk-python-mna-3.0.947/README.rst`

 * *Files identical despite different names*

