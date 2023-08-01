# Comparing `tmp/apache-airflow-providers-microsoft-mssql-3.4.2.tar.gz` & `tmp/apache-airflow-providers-microsoft-mssql-3.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-microsoft-mssql-3.4.2.tar", last modified: Sat Jul 29 12:03:20 2023, max compression
+gzip compressed data, was "apache-airflow-providers-microsoft-mssql-3.4.2rc1.tar", last modified: Sat Jul 29 12:08:41 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-mssql-3.4.2.tar` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:20.282063 apache-airflow-providers-microsoft-mssql-3.4.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:19.000000 apache-airflow-providers-microsoft-mssql-3.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5794 2023-07-29 12:03:20.282728 apache-airflow-providers-microsoft-mssql-3.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4096 2023-07-29 12:03:19.000000 apache-airflow-providers-microsoft-mssql-3.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:20.207848 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:20.208968 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:20.210072 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:20.242129 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/
--rw-r--r--   0 root         (0) root         (0)     1584 2023-07-29 12:01:19.000000 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3018 2023-07-29 12:03:19.000000 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:20.250285 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4199 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/hooks/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:20.256233 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-07-16 17:25:26.000000 apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/operators/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:20.279454 apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5794 2023-07-29 12:03:20.000000 apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-07-29 12:03:20.000000 apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:20.000000 apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-29 12:03:20.000000 apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:20.000000 apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-29 12:03:20.000000 apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:20.000000 apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-microsoft-mssql-3.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2040 2023-07-29 12:03:20.284734 apache-airflow-providers-microsoft-mssql-3.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-29 12:03:19.000000 apache-airflow-providers-microsoft-mssql-3.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.821562 apache-airflow-providers-microsoft-mssql-3.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:40.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-29 12:08:41.822228 apache-airflow-providers-microsoft-mssql-3.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-07-29 12:08:40.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.743542 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.744691 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.745962 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.780244 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-29 12:01:19.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2023-07-29 12:08:40.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.786324 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4199 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.792105 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-07-16 17:25:26.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.818364 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-07-29 12:08:41.824371 apache-airflow-providers-microsoft-mssql-3.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-29 12:08:40.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/LICENSE` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/MANIFEST.in` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/PKG-INFO` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.4.2
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-mssql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/README.rst` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/get_provider_info.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/hooks/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/hooks/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/mssql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/operators/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/airflow/providers/microsoft/mssql/operators/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/mssql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.4.2
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-mssql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/pyproject.toml` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/setup.cfg` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/setup.cfg`

 * *Files 5% similar despite different names*

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
 	pymssql>=2.1.5
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.mssql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.mssql
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.2/setup.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/setup.py`

 * *Files identical despite different names*

