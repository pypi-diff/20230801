# Comparing `tmp/tencentcloud-sdk-python-tcex-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-tcex-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcex-3.0.946.tar", last modified: Mon Jul 31 00:36:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcex-3.0.947.tar", last modified: Tue Aug  1 00:56:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcex-3.0.946.tar` & `tencentcloud-sdk-python-tcex-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/v20200727/
--rw-r--r--   0 root         (0) root         (0)     3127 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/v20200727/tcex_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/v20200727/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/v20200727/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     8678 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/v20200727/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud_sdk_python_tcex.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud_sdk_python_tcex.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud_sdk_python_tcex.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud_sdk_python_tcex.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/tencentcloud_sdk_python_tcex.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-31 00:36:31.000000 tencentcloud-sdk-python-tcex-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/v20200727/
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/v20200727/tcex_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/v20200727/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/v20200727/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     8678 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/v20200727/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud_sdk_python_tcex.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud_sdk_python_tcex.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud_sdk_python_tcex.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud_sdk_python_tcex.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/tencentcloud_sdk_python_tcex.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-01 00:56:41.000000 tencentcloud-sdk-python-tcex-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-tcex-3.0.946/setup.py` & `tencentcloud-sdk-python-tcex-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/v20200727/tcex_client.py` & `tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/v20200727/tcex_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/v20200727/errorcodes.py` & `tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/v20200727/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcex-3.0.946/tencentcloud/tcex/v20200727/models.py` & `tencentcloud-sdk-python-tcex-3.0.947/tencentcloud/tcex/v20200727/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcex-3.0.946/tencentcloud_sdk_python_tcex.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcex-3.0.947/tencentcloud_sdk_python_tcex.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcex
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Tcex SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcex-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-tcex-3.0.947/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcex
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Tcex SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcex-3.0.946/README.rst` & `tencentcloud-sdk-python-tcex-3.0.947/README.rst`

 * *Files identical despite different names*

