# Comparing `tmp/apache-airflow-providers-presto-5.1.2.tar.gz` & `tmp/apache-airflow-providers-presto-5.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-presto-5.1.2.tar", last modified: Sat Jul 29 12:03:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-presto-5.1.2rc1.tar", last modified: Sat Jul 29 12:08:57 2023, max compression
```

## Comparing `apache-airflow-providers-presto-5.1.2.tar` & `apache-airflow-providers-presto-5.1.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:35.671602 apache-airflow-providers-presto-5.1.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:34.000000 apache-airflow-providers-presto-5.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5835 2023-07-29 12:03:35.672264 apache-airflow-providers-presto-5.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4150 2023-07-29 12:03:34.000000 apache-airflow-providers-presto-5.1.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:35.587867 apache-airflow-providers-presto-5.1.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:35.588924 apache-airflow-providers-presto-5.1.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:35.627662 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2948 2023-07-29 12:03:34.000000 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:35.634832 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8316 2023-07-26 06:59:50.000000 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/hooks/presto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:35.641205 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4836 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.2/airflow/providers/presto/transfers/gcs_to_presto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:35.668859 apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5835 2023-07-29 12:03:35.000000 apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      723 2023-07-29 12:03:35.000000 apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:35.000000 apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:03:35.000000 apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:35.000000 apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-07-29 12:03:35.000000 apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:35.000000 apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-presto-5.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2006 2023-07-29 12:03:35.674526 apache-airflow-providers-presto-5.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2023-07-29 12:03:34.000000 apache-airflow-providers-presto-5.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.574103 apache-airflow-providers-presto-5.1.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:56.000000 apache-airflow-providers-presto-5.1.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-07-29 12:08:57.574694 apache-airflow-providers-presto-5.1.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-07-29 12:08:56.000000 apache-airflow-providers-presto-5.1.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.502162 apache-airflow-providers-presto-5.1.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.503250 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.534941 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-07-29 12:08:56.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.540718 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8316 2023-07-26 06:59:50.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/presto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.547217 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/gcs_to_presto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.571464 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      723 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      210 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-presto-5.1.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-07-29 12:08:57.576640 apache-airflow-providers-presto-5.1.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-07-29 12:08:56.000000 apache-airflow-providers-presto-5.1.2rc1/setup.py
```

### Comparing `apache-airflow-providers-presto-5.1.2/LICENSE` & `apache-airflow-providers-presto-5.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/MANIFEST.in` & `apache-airflow-providers-presto-5.1.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/PKG-INFO` & `apache-airflow-providers-presto-5.1.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-presto
-Version: 5.1.2
+Version: 5.1.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-presto package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.2``
+Release: ``5.1.2rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-presto-5.1.2/README.rst` & `apache-airflow-providers-presto-5.1.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.2``
+Release: ``5.1.2rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-presto-5.1.2/airflow/providers/presto/__init__.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/airflow/providers/presto/get_provider_info.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/airflow/providers/presto/hooks/__init__.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/airflow/providers/presto/hooks/presto.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/presto.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/airflow/providers/presto/transfers/__init__.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/airflow/providers/presto/transfers/gcs_to_presto.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/gcs_to_presto.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/PKG-INFO` & `apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-presto
-Version: 5.1.2
+Version: 5.1.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-presto package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.2``
+Release: ``5.1.2rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-presto-5.1.2/apache_airflow_providers_presto.egg-info/SOURCES.txt` & `apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/pyproject.toml` & `apache-airflow-providers-presto-5.1.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.2/setup.cfg` & `apache-airflow-providers-presto-5.1.2rc1/setup.cfg`

 * *Files 5% similar despite different names*

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
 	presto-python-client>=0.8.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.presto.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.presto
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-presto-5.1.2/setup.py` & `apache-airflow-providers-presto-5.1.2rc1/setup.py`

 * *Files identical despite different names*

