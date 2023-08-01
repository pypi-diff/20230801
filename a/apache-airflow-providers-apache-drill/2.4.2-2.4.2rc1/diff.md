# Comparing `tmp/apache-airflow-providers-apache-drill-2.4.2.tar.gz` & `tmp/apache-airflow-providers-apache-drill-2.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-drill-2.4.2.tar", last modified: Sat Jul 29 12:02:33 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-drill-2.4.2rc1.tar", last modified: Sat Jul 29 12:07:53 2023, max compression
```

## Comparing `apache-airflow-providers-apache-drill-2.4.2.tar` & `apache-airflow-providers-apache-drill-2.4.2rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:33.341198 apache-airflow-providers-apache-drill-2.4.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:02:32.000000 apache-airflow-providers-apache-drill-2.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5708 2023-07-29 12:02:33.341781 apache-airflow-providers-apache-drill-2.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4022 2023-07-29 12:02:32.000000 apache-airflow-providers-apache-drill-2.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:33.263759 apache-airflow-providers-apache-drill-2.4.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:33.264892 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:33.265969 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:33.300144 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2757 2023-07-29 12:02:32.000000 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:33.307307 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3660 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/hooks/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:33.313130 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2346 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/operators/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:33.338528 apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5708 2023-07-29 12:02:33.000000 apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-29 12:02:33.000000 apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:33.000000 apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:02:33.000000 apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:33.000000 apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-29 12:02:33.000000 apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:02:33.000000 apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-drill-2.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2028 2023-07-29 12:02:33.343717 apache-airflow-providers-apache-drill-2.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-29 12:02:32.000000 apache-airflow-providers-apache-drill-2.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.339467 apache-airflow-providers-apache-drill-2.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:07:52.000000 apache-airflow-providers-apache-drill-2.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-07-29 12:07:53.340090 apache-airflow-providers-apache-drill-2.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-07-29 12:07:52.000000 apache-airflow-providers-apache-drill-2.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.266945 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.267946 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.269070 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.301790 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2023-07-29 12:07:52.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.307588 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.313272 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.336782 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-drill-2.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-07-29 12:07:53.342061 apache-airflow-providers-apache-drill-2.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-29 12:07:52.000000 apache-airflow-providers-apache-drill-2.4.2rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2/LICENSE` & `apache-airflow-providers-apache-drill-2.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/MANIFEST.in` & `apache-airflow-providers-apache-drill-2.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.4.2
+Version: 2.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.2``
+Release: ``2.4.2rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2/README.rst` & `apache-airflow-providers-apache-drill-2.4.2rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.2``
+Release: ``2.4.2rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/__init__.py` & `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/get_provider_info.py` & `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/hooks/__init__.py` & `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/hooks/drill.py` & `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/drill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/operators/__init__.py` & `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/airflow/providers/apache/drill/operators/drill.py` & `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/drill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.4.2
+Version: 2.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.2``
+Release: ``2.4.2rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/pyproject.toml` & `apache-airflow-providers-apache-drill-2.4.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2/setup.cfg` & `apache-airflow-providers-apache-drill-2.4.2rc1/setup.cfg`

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
 	sqlalchemy-drill>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.drill.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.drill
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2/setup.py` & `apache-airflow-providers-apache-drill-2.4.2rc1/setup.py`

 * *Files identical despite different names*

