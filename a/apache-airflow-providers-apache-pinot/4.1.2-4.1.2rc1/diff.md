# Comparing `tmp/apache-airflow-providers-apache-pinot-4.1.2.tar.gz` & `tmp/apache-airflow-providers-apache-pinot-4.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-pinot-4.1.2.tar", last modified: Sat Jul 29 12:02:42 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-pinot-4.1.2rc1.tar", last modified: Sat Jul 29 12:08:02 2023, max compression
```

## Comparing `apache-airflow-providers-apache-pinot-4.1.2.tar` & `apache-airflow-providers-apache-pinot-4.1.2rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:42.104767 apache-airflow-providers-apache-pinot-4.1.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-pinot-4.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-pinot-4.1.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5706 2023-07-29 12:02:42.105432 apache-airflow-providers-apache-pinot-4.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4020 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:42.036949 apache-airflow-providers-apache-pinot-4.1.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:42.037959 apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:42.039086 apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:42.069247 apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:42.075354 apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11872 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/hooks/pinot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:42.101681 apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5706 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-29 12:02:42.000000 apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      129 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-pinot-4.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2018 2023-07-29 12:02:42.107586 apache-airflow-providers-apache-pinot-4.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-29 12:02:41.000000 apache-airflow-providers-apache-pinot-4.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:02.908613 apache-airflow-providers-apache-pinot-4.1.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:01.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5712 2023-07-29 12:08:02.909165 apache-airflow-providers-apache-pinot-4.1.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4023 2023-07-29 12:08:01.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:02.838407 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:02.839650 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:02.840920 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:02.871550 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-07-29 12:08:01.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:02.877320 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11872 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/hooks/pinot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:02.906310 apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5712 2023-07-29 12:08:02.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-29 12:08:02.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:02.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:08:02.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:02.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-29 12:08:02.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:02.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-07-29 12:08:02.911004 apache-airflow-providers-apache-pinot-4.1.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-29 12:08:01.000000 apache-airflow-providers-apache-pinot-4.1.2rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/LICENSE` & `apache-airflow-providers-apache-pinot-4.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/MANIFEST.in` & `apache-airflow-providers-apache-pinot-4.1.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/PKG-INFO` & `apache-airflow-providers-apache-pinot-4.1.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-pinot
-Version: 4.1.2
+Version: 4.1.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-pinot package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pinot/4.1.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-pinot``
 
-Release: ``4.1.2``
+Release: ``4.1.2rc1``
 
 
 `Apache Pinot <https://pinot.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/README.rst` & `apache-airflow-providers-apache-pinot-4.1.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-pinot``
 
-Release: ``4.1.2``
+Release: ``4.1.2rc1``
 
 
 `Apache Pinot <https://pinot.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/__init__.py` & `apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/get_provider_info.py` & `apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/hooks/__init__.py` & `apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/airflow/providers/apache/pinot/hooks/pinot.py` & `apache-airflow-providers-apache-pinot-4.1.2rc1/airflow/providers/apache/pinot/hooks/pinot.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/PKG-INFO` & `apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-pinot
-Version: 4.1.2
+Version: 4.1.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-pinot package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pinot/4.1.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-pinot``
 
-Release: ``4.1.2``
+Release: ``4.1.2rc1``
 
 
 `Apache Pinot <https://pinot.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/apache_airflow_providers_apache_pinot.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-pinot-4.1.2rc1/apache_airflow_providers_apache_pinot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/pyproject.toml` & `apache-airflow-providers-apache-pinot-4.1.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/setup.cfg` & `apache-airflow-providers-apache-pinot-4.1.2rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.3.1
-	apache-airflow>=2.4.0
+	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow>=2.4.0.dev0
 	pinotdb>0.4.7
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.pinot.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.pinot
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-pinot-4.1.2/setup.py` & `apache-airflow-providers-apache-pinot-4.1.2rc1/setup.py`

 * *Files identical despite different names*

