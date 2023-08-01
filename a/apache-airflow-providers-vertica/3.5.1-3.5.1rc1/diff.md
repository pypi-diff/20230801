# Comparing `tmp/apache-airflow-providers-vertica-3.5.1.tar.gz` & `tmp/apache-airflow-providers-vertica-3.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-vertica-3.5.1.tar", last modified: Sat Jul 29 12:03:54 2023, max compression
+gzip compressed data, was "apache-airflow-providers-vertica-3.5.1rc1.tar", last modified: Sat Jul 29 12:09:16 2023, max compression
```

## Comparing `apache-airflow-providers-vertica-3.5.1.tar` & `apache-airflow-providers-vertica-3.5.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:54.259554 apache-airflow-providers-vertica-3.5.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:53.000000 apache-airflow-providers-vertica-3.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5646 2023-07-29 12:03:54.260133 apache-airflow-providers-vertica-3.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3980 2023-07-29 12:03:53.000000 apache-airflow-providers-vertica-3.5.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:54.182528 apache-airflow-providers-vertica-3.5.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:54.183766 apache-airflow-providers-vertica-3.5.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:54.217443 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/
--rw-r--r--   0 root         (0) root         (0)     1576 2023-07-29 12:01:19.000000 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-07-29 12:03:53.000000 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:54.223576 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-06-30 08:49:17.000000 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/hooks/vertica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:54.229545 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2100 2023-07-16 17:25:26.000000 apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/operators/vertica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:54.256830 apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5646 2023-07-29 12:03:54.000000 apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      731 2023-07-29 12:03:54.000000 apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:54.000000 apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-29 12:03:54.000000 apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:54.000000 apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      137 2023-07-29 12:03:54.000000 apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:54.000000 apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-vertica-3.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1991 2023-07-29 12:03:54.262131 apache-airflow-providers-vertica-3.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-07-29 12:03:53.000000 apache-airflow-providers-vertica-3.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:16.283940 apache-airflow-providers-vertica-3.5.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:15.000000 apache-airflow-providers-vertica-3.5.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5652 2023-07-29 12:09:16.284517 apache-airflow-providers-vertica-3.5.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3983 2023-07-29 12:09:15.000000 apache-airflow-providers-vertica-3.5.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:16.213623 apache-airflow-providers-vertica-3.5.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:16.214655 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:16.246203 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-07-29 12:01:19.000000 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-07-29 12:09:15.000000 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:16.251890 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-30 08:49:17.000000 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/hooks/vertica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:16.257629 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-07-16 17:25:26.000000 apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/operators/vertica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:16.281364 apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5652 2023-07-29 12:09:16.000000 apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      731 2023-07-29 12:09:16.000000 apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:16.000000 apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-29 12:09:16.000000 apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:16.000000 apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-29 12:09:16.000000 apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:16.000000 apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-vertica-3.5.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-29 12:09:16.286387 apache-airflow-providers-vertica-3.5.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-07-29 12:09:15.000000 apache-airflow-providers-vertica-3.5.1rc1/setup.py
```

### Comparing `apache-airflow-providers-vertica-3.5.1/LICENSE` & `apache-airflow-providers-vertica-3.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/MANIFEST.in` & `apache-airflow-providers-vertica-3.5.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/PKG-INFO` & `apache-airflow-providers-vertica-3.5.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-vertica
-Version: 3.5.1
+Version: 3.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-vertica package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.5.1/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-vertica``
 
-Release: ``3.5.1``
+Release: ``3.5.1rc1``
 
 
 `Vertica <https://www.vertica.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-vertica-3.5.1/README.rst` & `apache-airflow-providers-vertica-3.5.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-vertica``
 
-Release: ``3.5.1``
+Release: ``3.5.1rc1``
 
 
 `Vertica <https://www.vertica.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/__init__.py` & `apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/get_provider_info.py` & `apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/hooks/__init__.py` & `apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/hooks/vertica.py` & `apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/hooks/vertica.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/operators/__init__.py` & `apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/airflow/providers/vertica/operators/vertica.py` & `apache-airflow-providers-vertica-3.5.1rc1/airflow/providers/vertica/operators/vertica.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/PKG-INFO` & `apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-vertica
-Version: 3.5.1
+Version: 3.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-vertica package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.5.1/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-vertica``
 
-Release: ``3.5.1``
+Release: ``3.5.1rc1``
 
 
 `Vertica <https://www.vertica.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-vertica-3.5.1/apache_airflow_providers_vertica.egg-info/SOURCES.txt` & `apache-airflow-providers-vertica-3.5.1rc1/apache_airflow_providers_vertica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/pyproject.toml` & `apache-airflow-providers-vertica-3.5.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-vertica-3.5.1/setup.cfg` & `apache-airflow-providers-vertica-3.5.1rc1/setup.cfg`

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
 	vertica-python>=0.5.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.vertica.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.vertica
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-vertica-3.5.1/setup.py` & `apache-airflow-providers-vertica-3.5.1rc1/setup.py`

 * *Files identical despite different names*

