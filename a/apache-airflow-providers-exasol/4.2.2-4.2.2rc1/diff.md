# Comparing `tmp/apache-airflow-providers-exasol-4.2.2.tar.gz` & `tmp/apache-airflow-providers-exasol-4.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-exasol-4.2.2.tar", last modified: Sat Jul 29 12:03:03 2023, max compression
+gzip compressed data, was "apache-airflow-providers-exasol-4.2.2rc1.tar", last modified: Sat Jul 29 12:08:24 2023, max compression
```

## Comparing `apache-airflow-providers-exasol-4.2.2.tar` & `apache-airflow-providers-exasol-4.2.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:03.004535 apache-airflow-providers-exasol-4.2.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:01.000000 apache-airflow-providers-exasol-4.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5696 2023-07-29 12:03:03.005139 apache-airflow-providers-exasol-4.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4034 2023-07-29 12:03:01.000000 apache-airflow-providers-exasol-4.2.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:02.929826 apache-airflow-providers-exasol-4.2.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:02.931299 apache-airflow-providers-exasol-4.2.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:02.966623 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-07-29 12:03:01.000000 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:02.973269 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11648 2023-07-26 06:59:50.000000 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/hooks/exasol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:02.979044 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-06-02 11:31:21.000000 apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/operators/exasol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:03.001950 apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5696 2023-07-29 12:03:02.000000 apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      716 2023-07-29 12:03:02.000000 apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:02.000000 apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:03:02.000000 apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:02.000000 apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-29 12:03:02.000000 apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:02.000000 apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-exasol-4.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1994 2023-07-29 12:03:03.007117 apache-airflow-providers-exasol-4.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-07-29 12:03:01.000000 apache-airflow-providers-exasol-4.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.194316 apache-airflow-providers-exasol-4.2.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:23.000000 apache-airflow-providers-exasol-4.2.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5702 2023-07-29 12:08:24.194905 apache-airflow-providers-exasol-4.2.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-07-29 12:08:23.000000 apache-airflow-providers-exasol-4.2.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.124786 apache-airflow-providers-exasol-4.2.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.125874 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.157247 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-29 12:08:23.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.162968 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11648 2023-07-26 06:59:50.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/exasol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.168963 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-06-02 11:31:21.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/exasol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.192073 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5702 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      716 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-exasol-4.2.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-07-29 12:08:24.196761 apache-airflow-providers-exasol-4.2.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-29 12:08:23.000000 apache-airflow-providers-exasol-4.2.2rc1/setup.py
```

### Comparing `apache-airflow-providers-exasol-4.2.2/LICENSE` & `apache-airflow-providers-exasol-4.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/MANIFEST.in` & `apache-airflow-providers-exasol-4.2.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/PKG-INFO` & `apache-airflow-providers-exasol-4.2.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-exasol
-Version: 4.2.2
+Version: 4.2.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-exasol package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.2``
+Release: ``4.2.2rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-exasol-4.2.2/README.rst` & `apache-airflow-providers-exasol-4.2.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.2``
+Release: ``4.2.2rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/__init__.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/get_provider_info.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/hooks/__init__.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/hooks/exasol.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/exasol.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/operators/__init__.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/airflow/providers/exasol/operators/exasol.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/exasol.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/PKG-INFO` & `apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-exasol
-Version: 4.2.2
+Version: 4.2.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-exasol package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.2``
+Release: ``4.2.2rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-exasol-4.2.2/apache_airflow_providers_exasol.egg-info/SOURCES.txt` & `apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/pyproject.toml` & `apache-airflow-providers-exasol-4.2.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.2/setup.cfg` & `apache-airflow-providers-exasol-4.2.2rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
 	pyexasol>=0.5.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.exasol.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.exasol
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-exasol-4.2.2/setup.py` & `apache-airflow-providers-exasol-4.2.2rc1/setup.py`

 * *Files identical despite different names*

