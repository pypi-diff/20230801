# Comparing `tmp/apache-airflow-providers-slack-7.3.2.tar.gz` & `tmp/apache-airflow-providers-slack-7.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-slack-7.3.2.tar", last modified: Sat Jul 29 12:03:44 2023, max compression
+gzip compressed data, was "apache-airflow-providers-slack-7.3.2rc1.tar", last modified: Sat Jul 29 12:09:06 2023, max compression
```

## Comparing `apache-airflow-providers-slack-7.3.2.tar` & `apache-airflow-providers-slack-7.3.2rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:44.017766 apache-airflow-providers-slack-7.3.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:03:42.000000 apache-airflow-providers-slack-7.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5616 2023-07-29 12:03:44.018389 apache-airflow-providers-slack-7.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3958 2023-07-29 12:03:42.000000 apache-airflow-providers-slack-7.3.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:43.918124 apache-airflow-providers-slack-7.3.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:43.919120 apache-airflow-providers-slack-7.3.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:43.954934 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3634 2023-07-29 12:03:42.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:43.965438 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14482 2023-07-06 04:42:33.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/hooks/slack.py
--rw-r--r--   0 root         (0) root         (0)    21222 2023-07-06 04:42:33.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/hooks/slack_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:43.974758 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/notifications/slack.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/notifications/slack_notifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:43.983326 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-06-05 12:50:36.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/operators/slack.py
--rw-r--r--   0 root         (0) root         (0)     7402 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/operators/slack_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:43.989044 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12923 2023-07-26 06:59:50.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/transfers/sql_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:43.991957 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/utils/
--rw-r--r--   0 root         (0) root         (0)     5132 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2/airflow/providers/slack/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:03:44.015390 apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5616 2023-07-29 12:03:43.000000 apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-29 12:03:43.000000 apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:43.000000 apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:03:43.000000 apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:03:43.000000 apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-29 12:03:43.000000 apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:03:43.000000 apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-slack-7.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1972 2023-07-29 12:03:44.020184 apache-airflow-providers-slack-7.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2023-07-29 12:03:42.000000 apache-airflow-providers-slack-7.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.359030 apache-airflow-providers-slack-7.3.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:05.000000 apache-airflow-providers-slack-7.3.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-07-29 12:09:06.359646 apache-airflow-providers-slack-7.3.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-07-29 12:09:05.000000 apache-airflow-providers-slack-7.3.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.256000 apache-airflow-providers-slack-7.3.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.257146 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.294291 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-07-29 12:09:05.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.303304 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14482 2023-07-06 04:42:33.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/slack.py
+-rw-r--r--   0 root         (0) root         (0)    21222 2023-07-06 04:42:33.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/slack_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.312758 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/slack.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/slack_notifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.321545 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-06-05 12:50:36.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/slack.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/slack_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.327221 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12923 2023-07-26 06:59:50.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/sql_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.330505 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/utils/
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.356268 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-slack-7.3.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-07-29 12:09:06.361593 apache-airflow-providers-slack-7.3.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-29 12:09:05.000000 apache-airflow-providers-slack-7.3.2rc1/setup.py
```

### Comparing `apache-airflow-providers-slack-7.3.2/LICENSE` & `apache-airflow-providers-slack-7.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/MANIFEST.in` & `apache-airflow-providers-slack-7.3.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/PKG-INFO` & `apache-airflow-providers-slack-7.3.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-slack
-Version: 7.3.2
+Version: 7.3.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-slack package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.3.2``
+Release: ``7.3.2rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-slack-7.3.2/README.rst` & `apache-airflow-providers-slack-7.3.2rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.3.2``
+Release: ``7.3.2rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/get_provider_info.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/hooks/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/hooks/slack.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/hooks/slack_webhook.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/notifications/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/notifications/slack.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/notifications/slack_notifier.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/operators/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/operators/slack.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/operators/slack_webhook.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/transfers/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/transfers/sql_to_slack.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/sql_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/airflow/providers/slack/utils/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/PKG-INFO` & `apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-slack
-Version: 7.3.2
+Version: 7.3.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-slack package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.2/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.3.2``
+Release: ``7.3.2rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-slack-7.3.2/apache_airflow_providers_slack.egg-info/SOURCES.txt` & `apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/pyproject.toml` & `apache-airflow-providers-slack-7.3.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.2/setup.cfg` & `apache-airflow-providers-slack-7.3.2rc1/setup.cfg`

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
 	slack_sdk>=3.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.slack.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.slack
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-slack-7.3.2/setup.py` & `apache-airflow-providers-slack-7.3.2rc1/setup.py`

 * *Files identical despite different names*

