# Comparing `tmp/redis-metric-helper-0.2.5.tar.gz` & `tmp/redis-metric-helper-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.2.5.tar", last modified: Tue May 30 13:40:18 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.2.6.tar", last modified: Tue Aug  1 14:45:24 2023, max compression
```

## Comparing `redis-metric-helper-0.2.5.tar` & `redis-metric-helper-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-05-30 13:40:18.682794 redis-metric-helper-0.2.5/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2.5/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-05-30 13:40:18.682794 redis-metric-helper-0.2.5/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2.5/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-05-30 13:40:18.678794 redis-metric-helper-0.2.5/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-05-30 13:38:17.000000 redis-metric-helper-0.2.5/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7028 2023-05-30 13:39:30.000000 redis-metric-helper-0.2.5/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-14 11:03:12.000000 redis-metric-helper-0.2.5/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1202 2023-05-30 13:37:38.000000 redis-metric-helper-0.2.5/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2.5/metric_helper/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-05-30 12:53:52.000000 redis-metric-helper-0.2.5/metric_helper/registry.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-05-30 13:40:18.682794 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-05-30 13:40:18.682794 redis-metric-helper-0.2.5/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2.5/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-01 14:45:24.545147 redis-metric-helper-0.2.6/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2.6/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-08-01 14:45:24.545147 redis-metric-helper-0.2.6/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2.6/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-01 14:45:24.545147 redis-metric-helper-0.2.6/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-08-01 14:41:18.000000 redis-metric-helper-0.2.6/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7032 2023-08-01 14:40:40.000000 redis-metric-helper-0.2.6/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-08-01 14:44:17.000000 redis-metric-helper-0.2.6/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1202 2023-08-01 14:44:17.000000 redis-metric-helper-0.2.6/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2.6/metric_helper/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-07-17 15:53:17.000000 redis-metric-helper-0.2.6/metric_helper/registry.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-01 14:45:24.545147 redis-metric-helper-0.2.6/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-08-01 14:45:24.000000 redis-metric-helper-0.2.6/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-08-01 14:45:24.000000 redis-metric-helper-0.2.6/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-08-01 14:45:24.000000 redis-metric-helper-0.2.6/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-08-01 14:45:24.000000 redis-metric-helper-0.2.6/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-08-01 14:45:24.000000 redis-metric-helper-0.2.6/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-08-01 14:45:24.545147 redis-metric-helper-0.2.6/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2.6/setup.py
```

### Comparing `redis-metric-helper-0.2.5/LICENSE` & `redis-metric-helper-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2.5/PKG-INFO` & `redis-metric-helper-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.2.5
+Version: 0.2.6
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.2.5/metric_helper/base.py` & `redis-metric-helper-0.2.6/metric_helper/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.ts = self.redis.ts()
         self.retention_msecs = int(settings.TIMESERIES_RETENTION_MSECS)
         self.retention_seconds = int(self.retention_msecs / 1000)
 
 
     def handle_write_kwargs(self, **kwargs):
         value = kwargs.get('value', None)
-        if not value:
+        if value is None:
             raise ValueError('You must provide a value for the metric write method.')
         labels = kwargs.get('labels', {})
         timestamp = kwargs.get('timestamp', '*')
         duplicate_policy = kwargs.get('duplicate_policy', 'SUM')
         pipeline = kwargs.get('pipeline', None)
         round_timestamp_to = kwargs.get('round_timestamp_to', None)
         return {
```

### Comparing `redis-metric-helper-0.2.5/metric_helper/connections.py` & `redis-metric-helper-0.2.6/metric_helper/connections.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2.5/metric_helper/registry.py` & `redis-metric-helper-0.2.6/metric_helper/registry.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2.5/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.2.6/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.2.5
+Version: 0.2.6
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.2.5/setup.py` & `redis-metric-helper-0.2.6/setup.py`

 * *Files identical despite different names*

