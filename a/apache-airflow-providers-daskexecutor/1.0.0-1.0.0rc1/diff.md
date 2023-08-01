# Comparing `tmp/apache-airflow-providers-daskexecutor-1.0.0.tar.gz` & `tmp/apache-airflow-providers-daskexecutor-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-daskexecutor-1.0.0.tar", last modified: Sat Jul 29 12:02:56 2023, max compression
+gzip compressed data, was "apache-airflow-providers-daskexecutor-1.0.0rc1.tar", last modified: Sat Jul 29 12:08:17 2023, max compression
```

## Comparing `apache-airflow-providers-daskexecutor-1.0.0.tar` & `apache-airflow-providers-daskexecutor-1.0.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:56.578236 apache-airflow-providers-daskexecutor-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-daskexecutor-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:02:55.000000 apache-airflow-providers-daskexecutor-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-daskexecutor-1.0.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4598 2023-07-29 12:02:56.578853 apache-airflow-providers-daskexecutor-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2939 2023-07-29 12:02:55.000000 apache-airflow-providers-daskexecutor-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:56.509364 apache-airflow-providers-daskexecutor-1.0.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:56.510630 apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:56.542544 apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:56.550198 apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/executors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/executors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5049 2023-07-26 06:59:50.000000 apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/executors/dask_executor.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-07-29 12:02:55.000000 apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:56.575204 apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4598 2023-07-29 12:02:56.000000 apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      705 2023-07-29 12:02:56.000000 apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:56.000000 apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:02:56.000000 apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:56.000000 apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-29 12:02:56.000000 apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:02:56.000000 apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-daskexecutor-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2047 2023-07-29 12:02:56.580993 apache-airflow-providers-daskexecutor-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-29 12:02:55.000000 apache-airflow-providers-daskexecutor-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:17.212592 apache-airflow-providers-daskexecutor-1.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:16.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4604 2023-07-29 12:08:17.213299 apache-airflow-providers-daskexecutor-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-07-29 12:08:16.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:17.143617 apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:17.144932 apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:17.176102 apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:17.181666 apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/executors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/executors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-07-26 06:59:50.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/executors/dask_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-29 12:08:16.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:17.210036 apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4604 2023-07-29 12:08:17.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-29 12:08:17.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:17.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:08:17.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:17.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-29 12:08:17.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:17.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-07-29 12:08:17.215785 apache-airflow-providers-daskexecutor-1.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-29 12:08:16.000000 apache-airflow-providers-daskexecutor-1.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/LICENSE` & `apache-airflow-providers-daskexecutor-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/MANIFEST.in` & `apache-airflow-providers-daskexecutor-1.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/PKG-INFO` & `apache-airflow-providers-daskexecutor-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-daskexecutor
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-daskexecutor package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-daskexecutor/1.0.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-daskexecutor``
 
-Release: ``1.0.0``
+Release: ``1.0.0rc1``
 
 
 `Dask <https://www.dask.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/README.rst` & `apache-airflow-providers-daskexecutor-1.0.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-daskexecutor``
 
-Release: ``1.0.0``
+Release: ``1.0.0rc1``
 
 
 `Dask <https://www.dask.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/__init__.py` & `apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/executors/__init__.py` & `apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/executors/dask_executor.py` & `apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/executors/dask_executor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/airflow/providers/daskexecutor/get_provider_info.py` & `apache-airflow-providers-daskexecutor-1.0.0rc1/airflow/providers/daskexecutor/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/PKG-INFO` & `apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-daskexecutor
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-daskexecutor package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-daskexecutor/1.0.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-daskexecutor``
 
-Release: ``1.0.0``
+Release: ``1.0.0rc1``
 
 
 `Dask <https://www.dask.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/apache_airflow_providers_daskexecutor.egg-info/SOURCES.txt` & `apache-airflow-providers-daskexecutor-1.0.0rc1/apache_airflow_providers_daskexecutor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/pyproject.toml` & `apache-airflow-providers-daskexecutor-1.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/setup.cfg` & `apache-airflow-providers-daskexecutor-1.0.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	cloudpickle>=1.4.1
 	dask>=2.9.0,!=2022.10.1,!=2023.5.0
 	distributed>=2.11.1,!=2023.5.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.daskexecutor.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.daskexecutor
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-daskexecutor-1.0.0/setup.py` & `apache-airflow-providers-daskexecutor-1.0.0rc1/setup.py`

 * *Files identical despite different names*

