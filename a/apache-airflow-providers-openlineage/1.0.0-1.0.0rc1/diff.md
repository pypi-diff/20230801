# Comparing `tmp/apache-airflow-providers-openlineage-1.0.0.tar.gz` & `tmp/apache-airflow-providers-openlineage-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-openlineage-1.0.0.tar", last modified: Sat Jul 29 12:03:28 2023, max compression
+gzip compressed data, was "apache-airflow-providers-openlineage-1.0.0rc1.tar", last modified: Sat Jul 29 12:08:49 2023, max compression
```

## Comparing `apache-airflow-providers-openlineage-1.0.0.tar` & `apache-airflow-providers-openlineage-1.0.0rc1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:28.054764 apache-airflow-providers-openlineage-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:26.000000 apache-airflow-providers-openlineage-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5800 2023-07-29 12:03:28.055333 apache-airflow-providers-openlineage-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4118 2023-07-29 12:03:26.000000 apache-airflow-providers-openlineage-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:27.951104 apache-airflow-providers-openlineage-1.0.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:27.952351 apache-airflow-providers-openlineage-1.0.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:27.989097 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/
--rw-r--r--   0 root         (0) root         (0)     1580 2023-07-29 12:01:19.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:28.003309 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/
--rw-r--r--   0 root         (0) root         (0)     1081 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/base.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/bash.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/manager.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/python.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-07-29 12:03:26.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:28.020321 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12484 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/adapter.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/facets.py
--rw-r--r--   0 root         (0) root         (0)     7256 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/listener.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/macros.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/openlineage.py
--rw-r--r--   0 root         (0) root         (0)    11218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/sqlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:28.028832 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7038 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/utils/sql.py
--rw-r--r--   0 root         (0) root         (0)    13269 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:28.052185 apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5800 2023-07-29 12:03:27.000000 apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1316 2023-07-29 12:03:27.000000 apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:27.000000 apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-29 12:03:27.000000 apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:27.000000 apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      193 2023-07-29 12:03:27.000000 apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:27.000000 apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2185 2023-07-29 12:03:28.057268 apache-airflow-providers-openlineage-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1721 2023-07-29 12:03:26.000000 apache-airflow-providers-openlineage-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.878147 apache-airflow-providers-openlineage-1.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:48.000000 apache-airflow-providers-openlineage-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-07-29 12:08:49.878673 apache-airflow-providers-openlineage-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-07-29 12:08:48.000000 apache-airflow-providers-openlineage-1.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.773138 apache-airflow-providers-openlineage-1.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.774433 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.811232 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-07-29 12:01:19.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.826250 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/base.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/bash.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/manager.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/python.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-07-29 12:08:48.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.843215 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12484 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/adapter.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/facets.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/listener.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/macros.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/openlineage.py
+-rw-r--r--   0 root         (0) root         (0)    11218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/sqlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.851742 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7038 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/sql.py
+-rw-r--r--   0 root         (0) root         (0)    13269 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.875542 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-07-29 12:08:49.880511 apache-airflow-providers-openlineage-1.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-07-29 12:08:48.000000 apache-airflow-providers-openlineage-1.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-openlineage-1.0.0/LICENSE` & `apache-airflow-providers-openlineage-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/MANIFEST.in` & `apache-airflow-providers-openlineage-1.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/PKG-INFO` & `apache-airflow-providers-openlineage-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openlineage package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.0``
+Release: ``1.0.0rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openlineage-1.0.0/README.rst` & `apache-airflow-providers-openlineage-1.0.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.0``
+Release: ``1.0.0rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/__init__.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/__init__.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/base.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/bash.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/bash.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/manager.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/extractors/python.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/python.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/get_provider_info.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/__init__.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/adapter.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/adapter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/facets.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/facets.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/listener.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/listener.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/macros.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/macros.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/plugins/openlineage.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/openlineage.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/sqlparser.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/sqlparser.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/utils/__init__.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/utils/sql.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/airflow/providers/openlineage/utils/utils.py` & `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/PKG-INFO` & `apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openlineage package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.0``
+Release: ``1.0.0rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openlineage-1.0.0/apache_airflow_providers_openlineage.egg-info/SOURCES.txt` & `apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/pyproject.toml` & `apache-airflow-providers-openlineage-1.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0/setup.cfg` & `apache-airflow-providers-openlineage-1.0.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -43,26 +43,26 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.6.0
-	apache-airflow>=2.7.0
+	apache-airflow-providers-common-sql>=1.6.0.dev0
+	apache-airflow>=2.7.0.dev0
 	attrs>=22.2
 	openlineage-integration-common>=0.28.0
 	openlineage-python>=0.28.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.openlineage.get_provider_info:get_provider_info
 airflow.plugins = 
 	openlineage=airflow.providers.openlineage.plugins.openlineage:OpenLineageProviderPlugin
 
 [files]
 packages = airflow.providers.openlineage
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-openlineage-1.0.0/setup.py` & `apache-airflow-providers-openlineage-1.0.0rc1/setup.py`

 * *Files identical despite different names*

