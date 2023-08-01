# Comparing `tmp/apache-airflow-providers-celery-3.3.0.tar.gz` & `tmp/apache-airflow-providers-celery-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-celery-3.3.0.tar", last modified: Sat Jul 29 12:02:49 2023, max compression
+gzip compressed data, was "apache-airflow-providers-celery-3.3.0rc1.tar", last modified: Sat Jul 29 12:08:10 2023, max compression
```

## Comparing `apache-airflow-providers-celery-3.3.0.tar` & `apache-airflow-providers-celery-3.3.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:49.844326 apache-airflow-providers-celery-3.3.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:02:48.000000 apache-airflow-providers-celery-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5575 2023-07-29 12:02:49.844920 apache-airflow-providers-celery-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3908 2023-07-29 12:02:48.000000 apache-airflow-providers-celery-3.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:49.759319 apache-airflow-providers-celery-3.3.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:49.760379 apache-airflow-providers-celery-3.3.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:49.793842 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:49.812352 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/
--rw-r--r--   0 root         (0) root         (0)     1584 2023-07-12 12:42:21.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18336 2023-07-29 09:53:35.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/celery_executor.py
--rw-r--r--   0 root         (0) root         (0)    13011 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/celery_executor_utils.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-29 06:50:08.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/celery_kubernetes_executor.py
--rw-r--r--   0 root         (0) root         (0)     5800 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/default_celery.py
--rw-r--r--   0 root         (0) root         (0)    16209 2023-07-29 12:02:48.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:49.817948 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2780 2023-06-29 05:49:30.000000 apache-airflow-providers-celery-3.3.0/airflow/providers/celery/sensors/celery_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:49.841994 apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5575 2023-07-29 12:02:49.000000 apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-29 12:02:49.000000 apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:49.000000 apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:02:49.000000 apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:49.000000 apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-29 12:02:49.000000 apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:02:49.000000 apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-celery-3.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-29 12:02:49.846767 apache-airflow-providers-celery-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1708 2023-07-29 12:02:48.000000 apache-airflow-providers-celery-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.464499 apache-airflow-providers-celery-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-07-29 12:08:10.465122 apache-airflow-providers-celery-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.376279 apache-airflow-providers-celery-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.377486 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.414891 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.430149 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-12 12:42:21.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18336 2023-07-29 09:53:35.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor.py
+-rw-r--r--   0 root         (0) root         (0)    13011 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-29 06:50:08.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/default_celery.py
+-rw-r--r--   0 root         (0) root         (0)    16209 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.437531 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-06-29 05:49:30.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/celery_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.461789 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-celery-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-29 12:08:10.466958 apache-airflow-providers-celery-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-celery-3.3.0/LICENSE` & `apache-airflow-providers-celery-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/MANIFEST.in` & `apache-airflow-providers-celery-3.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/PKG-INFO` & `apache-airflow-providers-celery-3.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-celery
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-celery package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-celery-3.3.0/README.rst` & `apache-airflow-providers-celery-3.3.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/__init__.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/__init__.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/celery_executor.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/celery_executor_utils.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor_utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/celery_kubernetes_executor.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/executors/default_celery.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/default_celery.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/get_provider_info.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/sensors/__init__.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/airflow/providers/celery/sensors/celery_queue.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/celery_queue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/PKG-INFO` & `apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-celery
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-celery package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-celery-3.3.0/apache_airflow_providers_celery.egg-info/SOURCES.txt` & `apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/pyproject.toml` & `apache-airflow-providers-celery-3.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0/setup.cfg` & `apache-airflow-providers-celery-3.3.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	celery>=5.2.3,<6
 	flower>=1.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.celery.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.celery
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-celery-3.3.0/setup.py` & `apache-airflow-providers-celery-3.3.0rc1/setup.py`

 * *Files identical despite different names*

