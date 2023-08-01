# Comparing `tmp/tencentcloud-sdk-python-msp-3.0.946.tar.gz` & `tmp/tencentcloud-sdk-python-msp-3.0.947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-msp-3.0.946.tar", last modified: Mon Jul 31 00:32:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-msp-3.0.947.tar", last modified: Tue Aug  1 00:52:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-msp-3.0.946.tar` & `tencentcloud-sdk-python-msp-3.0.947.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud_sdk_python_msp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud_sdk_python_msp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud_sdk_python_msp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud_sdk_python_msp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud_sdk_python_msp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/v20180319/
--rw-r--r--   0 root         (0) root         (0)     7386 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/v20180319/msp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/v20180319/__init__.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/v20180319/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    30960 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/v20180319/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:32:43.000000 tencentcloud-sdk-python-msp-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud_sdk_python_msp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud_sdk_python_msp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud_sdk_python_msp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud_sdk_python_msp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud_sdk_python_msp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/v20180319/
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/v20180319/msp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/v20180319/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      791 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/v20180319/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    30960 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/v20180319/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-01 00:52:47.000000 tencentcloud-sdk-python-msp-3.0.947/README.rst
```

### Comparing `tencentcloud-sdk-python-msp-3.0.946/setup.py` & `tencentcloud-sdk-python-msp-3.0.947/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-msp-3.0.946/tencentcloud_sdk_python_msp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-msp-3.0.947/tencentcloud_sdk_python_msp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-msp
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Msp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-msp-3.0.946/tencentcloud/__init__.py` & `tencentcloud-sdk-python-msp-3.0.947/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/v20180319/msp_client.py` & `tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/v20180319/msp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/v20180319/errorcodes.py` & `tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/v20180319/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-msp-3.0.946/tencentcloud/msp/v20180319/models.py` & `tencentcloud-sdk-python-msp-3.0.947/tencentcloud/msp/v20180319/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-msp-3.0.946/PKG-INFO` & `tencentcloud-sdk-python-msp-3.0.947/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-msp
-Version: 3.0.946
+Version: 3.0.947
 Summary: Tencent Cloud Msp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-msp-3.0.946/README.rst` & `tencentcloud-sdk-python-msp-3.0.947/README.rst`

 * *Files identical despite different names*

