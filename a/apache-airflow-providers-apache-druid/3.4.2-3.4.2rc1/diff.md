# Comparing `tmp/apache-airflow-providers-apache-druid-3.4.2.tar.gz` & `tmp/apache-airflow-providers-apache-druid-3.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-druid-3.4.2.tar", last modified: Sat Jul 29 12:02:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-druid-3.4.2rc1.tar", last modified: Sat Jul 29 12:07:55 2023, max compression
```

## Comparing `apache-airflow-providers-apache-druid-3.4.2.tar` & `apache-airflow-providers-apache-druid-3.4.2rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.128781 apache-airflow-providers-apache-druid-3.4.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5878 2023-07-29 12:02:35.129384 apache-airflow-providers-apache-druid-3.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4164 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.041479 apache-airflow-providers-apache-druid-3.4.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.042602 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.043729 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.076792 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3266 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.082403 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6903 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/hooks/druid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.090679 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/operators/druid.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/operators/druid_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.096762 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10081 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/transfers/hive_to_druid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:02:35.125225 apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5878 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      959 2023-07-29 12:02:35.000000 apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-druid-3.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2019 2023-07-29 12:02:35.131545 apache-airflow-providers-apache-druid-3.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1819 2023-07-29 12:02:34.000000 apache-airflow-providers-apache-druid-3.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.275123 apache-airflow-providers-apache-druid-3.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:07:54.000000 apache-airflow-providers-apache-druid-3.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5884 2023-07-29 12:07:55.275744 apache-airflow-providers-apache-druid-3.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-07-29 12:07:54.000000 apache-airflow-providers-apache-druid-3.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.183444 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.184447 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.185553 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.218867 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-07-29 12:07:54.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.225870 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6903 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/hooks/druid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.238347 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/operators/druid.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/operators/druid_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.244923 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10081 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/transfers/hive_to_druid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:55.272062 apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5884 2023-07-29 12:07:55.000000 apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      959 2023-07-29 12:07:55.000000 apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:55.000000 apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:07:55.000000 apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:55.000000 apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-29 12:07:55.000000 apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:07:55.000000 apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-druid-3.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-29 12:07:55.277654 apache-airflow-providers-apache-druid-3.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-07-29 12:07:54.000000 apache-airflow-providers-apache-druid-3.4.2rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-druid-3.4.2/LICENSE` & `apache-airflow-providers-apache-druid-3.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/MANIFEST.in` & `apache-airflow-providers-apache-druid-3.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/PKG-INFO` & `apache-airflow-providers-apache-druid-3.4.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-druid
-Version: 3.4.2
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-druid package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-druid-3.4.2/README.rst` & `apache-airflow-providers-apache-druid-3.4.2rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/__init__.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/get_provider_info.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/hooks/__init__.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/hooks/druid.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/hooks/druid.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/operators/__init__.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/operators/druid.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/operators/druid.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/operators/druid_check.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/operators/druid_check.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/transfers/__init__.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/airflow/providers/apache/druid/transfers/hive_to_druid.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/airflow/providers/apache/druid/transfers/hive_to_druid.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/PKG-INFO` & `apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-druid
-Version: 3.4.2
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-druid package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-druid-3.4.2/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-druid-3.4.2rc1/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/pyproject.toml` & `apache-airflow-providers-apache-druid-3.4.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.2/setup.cfg` & `apache-airflow-providers-apache-druid-3.4.2rc1/setup.cfg`

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
 	pydruid>=0.4.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.druid.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.druid
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-druid-3.4.2/setup.py` & `apache-airflow-providers-apache-druid-3.4.2rc1/setup.py`

 * *Files identical despite different names*

