# Comparing `tmp/apache-airflow-providers-mysql-5.2.0.tar.gz` & `tmp/apache-airflow-providers-mysql-5.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-mysql-5.2.0.tar", last modified: Sat Jul 29 12:03:23 2023, max compression
+gzip compressed data, was "apache-airflow-providers-mysql-5.2.0rc1.tar", last modified: Sat Jul 29 12:08:45 2023, max compression
```

## Comparing `apache-airflow-providers-mysql-5.2.0.tar` & `apache-airflow-providers-mysql-5.2.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:23.528537 apache-airflow-providers-mysql-5.2.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:22.000000 apache-airflow-providers-mysql-5.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.2.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6417 2023-07-29 12:03:23.529085 apache-airflow-providers-mysql-5.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4600 2023-07-29 12:03:22.000000 apache-airflow-providers-mysql-5.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:23.439860 apache-airflow-providers-mysql-5.2.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:23.441007 apache-airflow-providers-mysql-5.2.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:23.473785 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-07-29 12:03:22.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:23.479626 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12988 2023-07-26 06:59:50.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/hooks/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:23.485695 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-07-16 17:25:26.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/operators/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:23.502613 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-05 07:19:39.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/presto_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/s3_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3251 2023-07-05 07:19:39.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/trino_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/vertica_to_mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:23.526280 apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6417 2023-07-29 12:03:23.000000 apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      955 2023-07-29 12:03:23.000000 apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:23.000000 apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:03:23.000000 apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:23.000000 apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-29 12:03:23.000000 apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:23.000000 apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-mysql-5.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1974 2023-07-29 12:03:23.530983 apache-airflow-providers-mysql-5.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2087 2023-07-29 12:03:22.000000 apache-airflow-providers-mysql-5.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.227311 apache-airflow-providers-mysql-5.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:44.000000 apache-airflow-providers-mysql-5.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6423 2023-07-29 12:08:45.228022 apache-airflow-providers-mysql-5.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4603 2023-07-29 12:08:44.000000 apache-airflow-providers-mysql-5.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.133757 apache-airflow-providers-mysql-5.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.134899 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.169049 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-07-29 12:08:44.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.174888 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12988 2023-07-26 06:59:50.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.181079 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-07-16 17:25:26.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.195588 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-05 07:19:39.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3251 2023-07-05 07:19:39.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.224156 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6423 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      955 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-mysql-5.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-07-29 12:08:45.230492 apache-airflow-providers-mysql-5.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-07-29 12:08:44.000000 apache-airflow-providers-mysql-5.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-mysql-5.2.0/LICENSE` & `apache-airflow-providers-mysql-5.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/MANIFEST.in` & `apache-airflow-providers-mysql-5.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/PKG-INFO` & `apache-airflow-providers-mysql-5.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.2.0
+Version: 5.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/
@@ -73,15 +73,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.2.0``
+Release: ``5.2.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mysql-5.2.0/README.rst` & `apache-airflow-providers-mysql-5.2.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.2.0``
+Release: ``5.2.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/__init__.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/get_provider_info.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/hooks/__init__.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/hooks/mysql.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/operators/__init__.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/operators/mysql.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/__init__.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/presto_to_mysql.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/s3_to_mysql.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/trino_to_mysql.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/airflow/providers/mysql/transfers/vertica_to_mysql.py` & `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/PKG-INFO` & `apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.2.0
+Version: 5.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/
@@ -73,15 +73,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.2.0``
+Release: ``5.2.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mysql-5.2.0/apache_airflow_providers_mysql.egg-info/SOURCES.txt` & `apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/pyproject.toml` & `apache-airflow-providers-mysql-5.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0/setup.cfg` & `apache-airflow-providers-mysql-5.2.0rc1/setup.cfg`

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
 	mysqlclient>=1.3.6
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.mysql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.mysql
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-mysql-5.2.0/setup.py` & `apache-airflow-providers-mysql-5.2.0rc1/setup.py`

 * *Files identical despite different names*

