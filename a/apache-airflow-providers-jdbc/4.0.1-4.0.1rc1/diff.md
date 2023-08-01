# Comparing `tmp/apache-airflow-providers-jdbc-4.0.1.tar.gz` & `tmp/apache-airflow-providers-jdbc-4.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-jdbc-4.0.1.tar", last modified: Sat Jul 29 12:03:15 2023, max compression
+gzip compressed data, was "apache-airflow-providers-jdbc-4.0.1rc1.tar", last modified: Sat Jul 29 12:08:36 2023, max compression
```

## Comparing `apache-airflow-providers-jdbc-4.0.1.tar` & `apache-airflow-providers-jdbc-4.0.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:15.359027 apache-airflow-providers-jdbc-4.0.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:14.000000 apache-airflow-providers-jdbc-4.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5675 2023-07-29 12:03:15.359602 apache-airflow-providers-jdbc-4.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4021 2023-07-29 12:03:14.000000 apache-airflow-providers-jdbc-4.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:15.287729 apache-airflow-providers-jdbc-4.0.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:15.288705 apache-airflow-providers-jdbc-4.0.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:15.321060 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/
--rw-r--r--   0 root         (0) root         (0)     1573 2023-07-29 12:01:19.000000 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2853 2023-07-29 12:03:14.000000 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:15.326790 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7023 2023-06-17 16:45:00.000000 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/hooks/jdbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:15.332800 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-07-16 17:25:26.000000 apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/operators/jdbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:15.356356 apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5675 2023-07-29 12:03:15.000000 apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-07-29 12:03:15.000000 apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:15.000000 apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-29 12:03:15.000000 apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:15.000000 apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-29 12:03:15.000000 apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:15.000000 apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-jdbc-4.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1966 2023-07-29 12:03:15.361451 apache-airflow-providers-jdbc-4.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-29 12:03:14.000000 apache-airflow-providers-jdbc-4.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:36.928585 apache-airflow-providers-jdbc-4.0.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:35.000000 apache-airflow-providers-jdbc-4.0.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-07-29 12:08:36.929135 apache-airflow-providers-jdbc-4.0.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4024 2023-07-29 12:08:35.000000 apache-airflow-providers-jdbc-4.0.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:36.855003 apache-airflow-providers-jdbc-4.0.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:36.856561 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:36.890037 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-07-29 12:01:19.000000 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-07-29 12:08:35.000000 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:36.895612 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7023 2023-06-17 16:45:00.000000 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/hooks/jdbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:36.901348 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-07-16 17:25:26.000000 apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/operators/jdbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:36.925950 apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-07-29 12:08:36.000000 apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-29 12:08:36.000000 apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:36.000000 apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-29 12:08:36.000000 apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:36.000000 apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-29 12:08:36.000000 apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:36.000000 apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-jdbc-4.0.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-07-29 12:08:36.931084 apache-airflow-providers-jdbc-4.0.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-29 12:08:35.000000 apache-airflow-providers-jdbc-4.0.1rc1/setup.py
```

### Comparing `apache-airflow-providers-jdbc-4.0.1/LICENSE` & `apache-airflow-providers-jdbc-4.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/MANIFEST.in` & `apache-airflow-providers-jdbc-4.0.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/PKG-INFO` & `apache-airflow-providers-jdbc-4.0.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jdbc
-Version: 4.0.1
+Version: 4.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jdbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.1/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``4.0.1``
+Release: ``4.0.1rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jdbc-4.0.1/README.rst` & `apache-airflow-providers-jdbc-4.0.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``4.0.1``
+Release: ``4.0.1rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/__init__.py` & `apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/get_provider_info.py` & `apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/hooks/__init__.py` & `apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/hooks/jdbc.py` & `apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/hooks/jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/operators/__init__.py` & `apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/airflow/providers/jdbc/operators/jdbc.py` & `apache-airflow-providers-jdbc-4.0.1rc1/airflow/providers/jdbc/operators/jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/PKG-INFO` & `apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jdbc
-Version: 4.0.1
+Version: 4.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jdbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.1/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``4.0.1``
+Release: ``4.0.1rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jdbc-4.0.1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt` & `apache-airflow-providers-jdbc-4.0.1rc1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/pyproject.toml` & `apache-airflow-providers-jdbc-4.0.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.1/setup.cfg` & `apache-airflow-providers-jdbc-4.0.1rc1/setup.cfg`

 * *Files 3% similar despite different names*

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
 	jaydebeapi>=1.1.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.jdbc.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.jdbc
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-jdbc-4.0.1/setup.py` & `apache-airflow-providers-jdbc-4.0.1rc1/setup.py`

 * *Files identical despite different names*

