# Comparing `tmp/apache-airflow-providers-postgres-5.6.0.tar.gz` & `tmp/apache-airflow-providers-postgres-5.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-postgres-5.6.0.tar", last modified: Sat Jul 29 12:03:33 2023, max compression
+gzip compressed data, was "apache-airflow-providers-postgres-5.6.0rc1.tar", last modified: Sat Jul 29 12:08:55 2023, max compression
```

## Comparing `apache-airflow-providers-postgres-5.6.0.tar` & `apache-airflow-providers-postgres-5.6.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:33.828894 apache-airflow-providers-postgres-5.6.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:32.000000 apache-airflow-providers-postgres-5.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.6.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5974 2023-07-29 12:03:33.829666 apache-airflow-providers-postgres-5.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4253 2023-07-29 12:03:32.000000 apache-airflow-providers-postgres-5.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:33.716464 apache-airflow-providers-postgres-5.6.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:33.717809 apache-airflow-providers-postgres-5.6.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:33.774066 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/
--rw-r--r--   0 root         (0) root         (0)     1577 2023-07-29 12:01:19.000000 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-07-29 12:03:32.000000 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:33.780884 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15392 2023-07-27 05:54:58.000000 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/hooks/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:33.790098 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-07-16 17:25:26.000000 apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/operators/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:33.825025 apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5974 2023-07-29 12:03:33.000000 apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-29 12:03:33.000000 apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:33.000000 apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-29 12:03:33.000000 apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:33.000000 apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      239 2023-07-29 12:03:33.000000 apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:33.000000 apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-postgres-5.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1999 2023-07-29 12:03:33.831904 apache-airflow-providers-postgres-5.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1861 2023-07-29 12:03:32.000000 apache-airflow-providers-postgres-5.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.714646 apache-airflow-providers-postgres-5.6.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.6.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:54.000000 apache-airflow-providers-postgres-5.6.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.6.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-07-29 12:08:55.715213 apache-airflow-providers-postgres-5.6.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4256 2023-07-29 12:08:54.000000 apache-airflow-providers-postgres-5.6.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.643536 apache-airflow-providers-postgres-5.6.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.644825 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.676948 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-29 12:01:19.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-29 12:08:54.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.682658 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15392 2023-07-27 05:54:58.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.688432 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-07-16 17:25:26.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.712231 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      249 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-postgres-5.6.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-29 12:08:55.717130 apache-airflow-providers-postgres-5.6.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-07-29 12:08:54.000000 apache-airflow-providers-postgres-5.6.0rc1/setup.py
```

### Comparing `apache-airflow-providers-postgres-5.6.0/LICENSE` & `apache-airflow-providers-postgres-5.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/MANIFEST.in` & `apache-airflow-providers-postgres-5.6.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/PKG-INFO` & `apache-airflow-providers-postgres-5.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.6.0
+Version: 5.6.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/
@@ -69,15 +69,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.6.0``
+Release: ``5.6.0rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.6.0/README.rst` & `apache-airflow-providers-postgres-5.6.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.6.0``
+Release: ``5.6.0rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/__init__.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/get_provider_info.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/hooks/__init__.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/hooks/postgres.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/operators/__init__.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/airflow/providers/postgres/operators/postgres.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/PKG-INFO` & `apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.6.0
+Version: 5.6.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/
@@ -69,15 +69,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.6.0``
+Release: ``5.6.0rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.6.0/apache_airflow_providers_postgres.egg-info/SOURCES.txt` & `apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/pyproject.toml` & `apache-airflow-providers-postgres-5.6.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.6.0/setup.cfg` & `apache-airflow-providers-postgres-5.6.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

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
 	psycopg2-binary>=2.8.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.postgres.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.postgres
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-postgres-5.6.0/setup.py` & `apache-airflow-providers-postgres-5.6.0rc1/setup.py`

 * *Files identical despite different names*

