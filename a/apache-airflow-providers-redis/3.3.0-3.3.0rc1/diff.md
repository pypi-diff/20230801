# Comparing `tmp/apache-airflow-providers-redis-3.3.0.tar.gz` & `tmp/apache-airflow-providers-redis-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-redis-3.3.0.tar", last modified: Sat Jul 29 12:03:38 2023, max compression
+gzip compressed data, was "apache-airflow-providers-redis-3.3.0rc1.tar", last modified: Sat Jul 29 12:09:00 2023, max compression
```

## Comparing `apache-airflow-providers-redis-3.3.0.tar` & `apache-airflow-providers-redis-3.3.0rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:38.040624 apache-airflow-providers-redis-3.3.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:36.000000 apache-airflow-providers-redis-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4378 2023-07-29 12:03:38.041167 apache-airflow-providers-redis-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-29 12:03:36.000000 apache-airflow-providers-redis-3.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:37.947805 apache-airflow-providers-redis-3.3.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:37.948877 apache-airflow-providers-redis-3.3.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:37.986841 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-07-29 12:03:36.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:37.993013 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/hooks/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:37.999482 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/log/
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/log/redis_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:38.005495 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/operators/redis_publish.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:38.013997 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/sensors/redis_key.py
--rw-r--r--   0 root         (0) root         (0)     2586 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0/airflow/providers/redis/sensors/redis_pub_sub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:38.037775 apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4378 2023-07-29 12:03:37.000000 apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      937 2023-07-29 12:03:37.000000 apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:37.000000 apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:03:37.000000 apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:37.000000 apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-29 12:03:37.000000 apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:37.000000 apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-redis-3.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-29 12:03:38.043065 apache-airflow-providers-redis-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-07-29 12:03:36.000000 apache-airflow-providers-redis-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:00.031960 apache-airflow-providers-redis-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:58.000000 apache-airflow-providers-redis-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-07-29 12:09:00.032626 apache-airflow-providers-redis-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-29 12:08:58.000000 apache-airflow-providers-redis-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.929772 apache-airflow-providers-redis-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.931310 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.971091 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-07-29 12:08:58.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.977186 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.984895 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/redis_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.991024 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/redis_publish.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:00.001303 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/redis_key.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/redis_pub_sub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:00.028927 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      937 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-redis-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-07-29 12:09:00.034847 apache-airflow-providers-redis-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-07-29 12:08:58.000000 apache-airflow-providers-redis-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-redis-3.3.0/LICENSE` & `apache-airflow-providers-redis-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/MANIFEST.in` & `apache-airflow-providers-redis-3.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/PKG-INFO` & `apache-airflow-providers-redis-3.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-redis package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.3.0/README.rst` & `apache-airflow-providers-redis-3.3.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/__init__.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/get_provider_info.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/hooks/__init__.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/hooks/redis.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/redis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/log/__init__.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/log/redis_task_handler.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/redis_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/operators/__init__.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/operators/redis_publish.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/redis_publish.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/sensors/__init__.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/sensors/redis_key.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/redis_key.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/airflow/providers/redis/sensors/redis_pub_sub.py` & `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/redis_pub_sub.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/PKG-INFO` & `apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-redis package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.3.0/apache_airflow_providers_redis.egg-info/SOURCES.txt` & `apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/pyproject.toml` & `apache-airflow-providers-redis-3.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0/setup.cfg` & `apache-airflow-providers-redis-3.3.0rc1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	redis>=3.2.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.redis.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.redis
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-redis-3.3.0/setup.py` & `apache-airflow-providers-redis-3.3.0rc1/setup.py`

 * *Files identical despite different names*

