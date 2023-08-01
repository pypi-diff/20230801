# Comparing `tmp/apache-airflow-providers-apprise-1.0.1.tar.gz` & `tmp/apache-airflow-providers-apprise-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apprise-1.0.1.tar", last modified: Sat Jul 29 12:02:46 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apprise-1.0.1rc1.tar", last modified: Sat Jul 29 12:08:06 2023, max compression
```

## Comparing `apache-airflow-providers-apprise-1.0.1.tar` & `apache-airflow-providers-apprise-1.0.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:46.447678 apache-airflow-providers-apprise-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:02:45.000000 apache-airflow-providers-apprise-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4396 2023-07-29 12:02:46.448254 apache-airflow-providers-apprise-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2757 2023-07-29 12:02:45.000000 apache-airflow-providers-apprise-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:46.375449 apache-airflow-providers-apprise-1.0.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:46.376445 apache-airflow-providers-apprise-1.0.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:46.410702 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/
--rw-r--r--   0 root         (0) root         (0)     1576 2023-07-29 12:01:19.000000 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2019 2023-07-29 12:02:45.000000 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:46.416357 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/hooks/
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5225 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/hooks/apprise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:46.421983 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/notifications/
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/notifications/apprise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:46.445073 apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4396 2023-07-29 12:02:46.000000 apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-07-29 12:02:46.000000 apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:46.000000 apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-29 12:02:46.000000 apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:46.000000 apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-29 12:02:46.000000 apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:02:46.000000 apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1933 2023-07-29 12:02:46.450224 apache-airflow-providers-apprise-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-07-29 12:02:45.000000 apache-airflow-providers-apprise-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.978369 apache-airflow-providers-apprise-1.0.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:05.000000 apache-airflow-providers-apprise-1.0.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-29 12:08:06.978922 apache-airflow-providers-apprise-1.0.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-07-29 12:08:05.000000 apache-airflow-providers-apprise-1.0.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.901871 apache-airflow-providers-apprise-1.0.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.903227 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.939635 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-07-29 12:01:19.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-07-29 12:08:05.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.945822 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/apprise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.951850 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/apprise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.976101 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-29 12:08:06.981045 apache-airflow-providers-apprise-1.0.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-29 12:08:05.000000 apache-airflow-providers-apprise-1.0.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apprise-1.0.1/LICENSE` & `apache-airflow-providers-apprise-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/MANIFEST.in` & `apache-airflow-providers-apprise-1.0.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/PKG-INFO` & `apache-airflow-providers-apprise-1.0.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apprise
-Version: 1.0.1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apprise package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apprise-1.0.1/README.rst` & `apache-airflow-providers-apprise-1.0.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/__init__.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/get_provider_info.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/hooks/__init__.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/hooks/apprise.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/apprise.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/notifications/__init__.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/airflow/providers/apprise/notifications/apprise.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/apprise.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/PKG-INFO` & `apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apprise
-Version: 1.0.1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apprise package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apprise-1.0.1/apache_airflow_providers_apprise.egg-info/SOURCES.txt` & `apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/pyproject.toml` & `apache-airflow-providers-apprise-1.0.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.1/setup.cfg` & `apache-airflow-providers-apprise-1.0.1rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	apprise
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apprise.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apprise
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apprise-1.0.1/setup.py` & `apache-airflow-providers-apprise-1.0.1rc1/setup.py`

 * *Files identical despite different names*

