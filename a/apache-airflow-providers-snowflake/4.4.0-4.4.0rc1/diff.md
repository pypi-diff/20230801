# Comparing `tmp/apache-airflow-providers-snowflake-4.4.0.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-snowflake-4.4.0.tar", last modified: Sat Jul 29 12:03:46 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.4.0rc1.tar", last modified: Sat Jul 29 12:09:08 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.4.0.tar` & `apache-airflow-providers-snowflake-4.4.0rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.546275 apache-airflow-providers-snowflake-4.4.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:45.000000 apache-airflow-providers-snowflake-4.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6038 2023-07-29 12:03:46.547277 apache-airflow-providers-snowflake-4.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4314 2023-07-29 12:03:45.000000 apache-airflow-providers-snowflake-4.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.346442 apache-airflow-providers-snowflake-4.4.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.347618 apache-airflow-providers-snowflake-4.4.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.397008 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 12:01:19.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4991 2023-07-29 12:03:45.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.414560 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/hooks/snowflake_sql_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.423531 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24878 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.457196 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5098 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.472751 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/triggers/snowflake_trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.496701 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:46.542662 apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6038 2023-07-29 12:03:46.000000 apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-29 12:03:46.000000 apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:46.000000 apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-29 12:03:46.000000 apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:46.000000 apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-29 12:03:46.000000 apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:46.000000 apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-snowflake-4.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2046 2023-07-29 12:03:46.556873 apache-airflow-providers-snowflake-4.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1858 2023-07-29 12:03:45.000000 apache-airflow-providers-snowflake-4.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.761202 apache-airflow-providers-snowflake-4.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-29 12:09:08.761764 apache-airflow-providers-snowflake-4.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4317 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.655883 apache-airflow-providers-snowflake-4.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.657068 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.694162 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 12:01:19.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4991 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.703082 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.708868 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24878 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.720597 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.726145 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.734576 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.758540 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      279 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-snowflake-4.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-29 12:09:08.763589 apache-airflow-providers-snowflake-4.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.4.0/LICENSE` & `apache-airflow-providers-snowflake-4.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/MANIFEST.in` & `apache-airflow-providers-snowflake-4.4.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/PKG-INFO` & `apache-airflow-providers-snowflake-4.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.4.0
+Version: 4.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/
@@ -69,15 +69,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.0``
+Release: ``4.4.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.4.0/README.rst` & `apache-airflow-providers-snowflake-4.4.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.0``
+Release: ``4.4.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/triggers/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/triggers/snowflake_trigger.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.4.0
+Version: 4.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/
@@ -69,15 +69,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.0``
+Release: ``4.4.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.4.0/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/pyproject.toml` & `apache-airflow-providers-snowflake-4.4.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0/setup.cfg` & `apache-airflow-providers-snowflake-4.4.0rc1/setup.cfg`

 * *Files 9% similar despite different names*

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
 	snowflake-connector-python>=2.4.1
 	snowflake-sqlalchemy>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.4.0/setup.py` & `apache-airflow-providers-snowflake-4.4.0rc1/setup.py`

 * *Files identical despite different names*

