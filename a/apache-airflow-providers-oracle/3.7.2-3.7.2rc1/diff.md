# Comparing `tmp/apache-airflow-providers-oracle-3.7.2.tar.gz` & `tmp/apache-airflow-providers-oracle-3.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-oracle-3.7.2.tar", last modified: Sat Jul 29 12:03:30 2023, max compression
+gzip compressed data, was "apache-airflow-providers-oracle-3.7.2rc1.tar", last modified: Sat Jul 29 12:08:52 2023, max compression
```

## Comparing `apache-airflow-providers-oracle-3.7.2.tar` & `apache-airflow-providers-oracle-3.7.2rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.519830 apache-airflow-providers-oracle-3.7.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:29.000000 apache-airflow-providers-oracle-3.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5667 2023-07-29 12:03:30.520652 apache-airflow-providers-oracle-3.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3983 2023-07-29 12:03:29.000000 apache-airflow-providers-oracle-3.7.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.373634 apache-airflow-providers-oracle-3.7.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.375411 apache-airflow-providers-oracle-3.7.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.443082 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.455229 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/example_dags/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/example_dags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/example_dags/example_oracle.py
--rw-r--r--   0 root         (0) root         (0)     2992 2023-07-29 12:03:29.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.463114 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17488 2023-06-05 12:50:36.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/hooks/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.473137 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-07-16 17:25:26.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/operators/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.481223 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3646 2023-06-28 06:26:40.000000 apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/transfers/oracle_to_oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:30.513849 apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5667 2023-07-29 12:03:30.000000 apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2023-07-29 12:03:30.000000 apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:30.000000 apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:03:30.000000 apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:30.000000 apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-29 12:03:30.000000 apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:30.000000 apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-oracle-3.7.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1978 2023-07-29 12:03:30.523186 apache-airflow-providers-oracle-3.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1711 2023-07-29 12:03:29.000000 apache-airflow-providers-oracle-3.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.296187 apache-airflow-providers-oracle-3.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:51.000000 apache-airflow-providers-oracle-3.7.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-07-29 12:08:52.296949 apache-airflow-providers-oracle-3.7.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-07-29 12:08:51.000000 apache-airflow-providers-oracle-3.7.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.199591 apache-airflow-providers-oracle-3.7.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.200703 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.239182 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.245825 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/example_oracle.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-07-29 12:08:51.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.254024 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17488 2023-06-05 12:50:36.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.261930 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-07-16 17:25:26.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.268432 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-06-28 06:26:40.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.293630 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-oracle-3.7.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-07-29 12:08:52.299039 apache-airflow-providers-oracle-3.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-29 12:08:51.000000 apache-airflow-providers-oracle-3.7.2rc1/setup.py
```

### Comparing `apache-airflow-providers-oracle-3.7.2/LICENSE` & `apache-airflow-providers-oracle-3.7.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/MANIFEST.in` & `apache-airflow-providers-oracle-3.7.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/PKG-INFO` & `apache-airflow-providers-oracle-3.7.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.7.2
+Version: 3.7.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-oracle package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.2``
+Release: ``3.7.2rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-oracle-3.7.2/README.rst` & `apache-airflow-providers-oracle-3.7.2rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.2``
+Release: ``3.7.2rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/example_dags/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/example_dags/example_oracle.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/example_oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/get_provider_info.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/hooks/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/hooks/oracle.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/operators/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/operators/oracle.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/transfers/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/airflow/providers/oracle/transfers/oracle_to_oracle.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/PKG-INFO` & `apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.7.2
+Version: 3.7.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-oracle package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.2``
+Release: ``3.7.2rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-oracle-3.7.2/apache_airflow_providers_oracle.egg-info/SOURCES.txt` & `apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/pyproject.toml` & `apache-airflow-providers-oracle-3.7.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.2/setup.cfg` & `apache-airflow-providers-oracle-3.7.2rc1/setup.cfg`

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
 	oracledb>=1.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.oracle.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.oracle
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-oracle-3.7.2/setup.py` & `apache-airflow-providers-oracle-3.7.2rc1/setup.py`

 * *Files identical despite different names*

