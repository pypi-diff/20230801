# Comparing `tmp/apache-airflow-providers-trino-5.2.1.tar.gz` & `tmp/apache-airflow-providers-trino-5.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-trino-5.2.1.tar", last modified: Sat Jul 29 12:03:52 2023, max compression
+gzip compressed data, was "apache-airflow-providers-trino-5.2.1rc1.tar", last modified: Sat Jul 29 12:09:14 2023, max compression
```

## Comparing `apache-airflow-providers-trino-5.2.1.tar` & `apache-airflow-providers-trino-5.2.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:52.391546 apache-airflow-providers-trino-5.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:51.000000 apache-airflow-providers-trino-5.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5815 2023-07-29 12:03:52.392320 apache-airflow-providers-trino-5.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4134 2023-07-29 12:03:51.000000 apache-airflow-providers-trino-5.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:52.286926 apache-airflow-providers-trino-5.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:52.288247 apache-airflow-providers-trino-5.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:52.325838 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-07-29 12:03:51.000000 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:52.331984 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9073 2023-07-26 06:59:50.000000 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/hooks/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:52.337982 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-16 17:25:26.000000 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/operators/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:52.345113 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/transfers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.2.1/airflow/providers/trino/transfers/gcs_to_trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:52.388712 apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5815 2023-07-29 12:03:52.000000 apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-07-29 12:03:52.000000 apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:52.000000 apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:03:52.000000 apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:52.000000 apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      187 2023-07-29 12:03:52.000000 apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:52.000000 apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-trino-5.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1986 2023-07-29 12:03:52.394387 apache-airflow-providers-trino-5.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1767 2023-07-29 12:03:51.000000 apache-airflow-providers-trino-5.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.456011 apache-airflow-providers-trino-5.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:13.000000 apache-airflow-providers-trino-5.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-29 12:09:14.456555 apache-airflow-providers-trino-5.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-07-29 12:09:13.000000 apache-airflow-providers-trino-5.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.378819 apache-airflow-providers-trino-5.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.380084 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.413526 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-07-29 12:09:13.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.419229 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9073 2023-07-26 06:59:50.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.424892 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-16 17:25:26.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.430414 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/gcs_to_trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.453338 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-trino-5.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-07-29 12:09:14.458548 apache-airflow-providers-trino-5.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-29 12:09:13.000000 apache-airflow-providers-trino-5.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-trino-5.2.1/LICENSE` & `apache-airflow-providers-trino-5.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/MANIFEST.in` & `apache-airflow-providers-trino-5.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/PKG-INFO` & `apache-airflow-providers-trino-5.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.2.1
+Version: 5.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.1``
+Release: ``5.2.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.2.1/README.rst` & `apache-airflow-providers-trino-5.2.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.1``
+Release: ``5.2.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.2.1/airflow/providers/trino/__init__.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/airflow/providers/trino/get_provider_info.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/airflow/providers/trino/hooks/__init__.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/airflow/providers/trino/hooks/trino.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/airflow/providers/trino/operators/__init__.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/airflow/providers/trino/operators/trino.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/airflow/providers/trino/transfers/__init__.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/airflow/providers/trino/transfers/gcs_to_trino.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/gcs_to_trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/PKG-INFO` & `apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.2.1
+Version: 5.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.1``
+Release: ``5.2.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.2.1/apache_airflow_providers_trino.egg-info/SOURCES.txt` & `apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/pyproject.toml` & `apache-airflow-providers-trino-5.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.1/setup.cfg` & `apache-airflow-providers-trino-5.2.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,23 @@
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
 	pandas>=0.17.1
 	trino>=0.318.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.trino.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.trino
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-trino-5.2.1/setup.py` & `apache-airflow-providers-trino-5.2.1rc1/setup.py`

 * *Files identical despite different names*

