# Comparing `tmp/apache-airflow-providers-sftp-4.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-sftp-4.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sftp-4.4.0rc1.tar", last modified: Wed Jul 12 19:13:33 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sftp-4.5.0rc1.tar", last modified: Sat Jul 29 12:09:03 2023, max compression
```

## Comparing `apache-airflow-providers-sftp-4.4.0rc1.tar` & `apache-airflow-providers-sftp-4.5.0rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.597969 apache-airflow-providers-sftp-4.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5472 2023-07-12 19:13:33.598522 apache-airflow-providers-sftp-4.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3822 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.504568 apache-airflow-providers-sftp-4.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.505728 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.546449 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-12 19:08:31.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.549508 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.555289 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2862 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.560953 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14745 2023-06-05 12:50:36.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.566531 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8458 2023-07-06 04:42:33.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.572295 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.595702 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5472 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      918 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-sftp-4.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1953 2023-07-12 19:13:33.600765 apache-airflow-providers-sftp-4.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.958669 apache-airflow-providers-sftp-4.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:02.000000 apache-airflow-providers-sftp-4.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-07-29 12:09:03.959274 apache-airflow-providers-sftp-4.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4062 2023-07-29 12:09:02.000000 apache-airflow-providers-sftp-4.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.858890 apache-airflow-providers-sftp-4.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.860043 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.905151 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-07-29 12:01:19.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.908048 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/decorators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.913768 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/decorators/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     3410 2023-07-29 12:09:02.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.919543 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14745 2023-06-05 12:50:36.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/hooks/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.925383 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11475 2023-07-26 06:59:50.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/operators/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.931254 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/sensors/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:03.956411 apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-07-29 12:09:03.000000 apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      918 2023-07-29 12:09:03.000000 apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:03.000000 apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-29 12:09:03.000000 apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:03.000000 apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-29 12:09:03.000000 apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:03.000000 apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-sftp-4.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-07-29 12:09:03.961142 apache-airflow-providers-sftp-4.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-07-29 12:09:02.000000 apache-airflow-providers-sftp-4.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/LICENSE` & `apache-airflow-providers-sftp-4.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/MANIFEST.in` & `apache-airflow-providers-sftp-4.5.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/PKG-INFO` & `apache-airflow-providers-sftp-4.5.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sftp
-Version: 4.4.0rc1
+Version: 4.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: openlineage
 Provides-Extra: ssh
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -67,28 +68,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.4.0rc1``
+Release: ``4.5.0rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sftp`` provider. All classes for this provider package
 are in ``airflow.providers.sftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -112,18 +113,19 @@
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
 
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
-    pip install apache-airflow-providers-sftp[ssh]
+    pip install apache-airflow-providers-sftp[openlineage]
 
 
-==============================================================================================  =======
-Dependent package                                                                               Extra
-==============================================================================================  =======
-`apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_  ``ssh``
-==============================================================================================  =======
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+`apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                  ``ssh``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/README.rst` & `apache-airflow-providers-sftp-4.5.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.4.0rc1``
+Release: ``4.5.0rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sftp`` provider. All classes for this provider package
 are in ``airflow.providers.sftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -77,18 +77,19 @@
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
 
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
-    pip install apache-airflow-providers-sftp[ssh]
+    pip install apache-airflow-providers-sftp[openlineage]
 
 
-==============================================================================================  =======
-Dependent package                                                                               Extra
-==============================================================================================  =======
-`apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_  ``ssh``
-==============================================================================================  =======
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+`apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                  ``ssh``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/__init__.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.4.0"
+__version__ = "4.5.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-sftp:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/__init__.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/get_provider_info.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-sftp",
         "name": "SFTP",
         "description": "`SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__\n",
         "suspended": False,
         "versions": [
+            "4.5.0",
             "4.4.0",
             "4.3.1",
             "4.3.0",
             "4.2.4",
             "4.2.3",
             "4.2.2",
             "4.2.1",
```

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/__init__.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/sftp.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/hooks/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/__init__.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/__init__.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/sftp.py` & `apache-airflow-providers-sftp-4.5.0rc1/airflow/providers/sftp/sensors/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO` & `apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sftp
-Version: 4.4.0rc1
+Version: 4.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: openlineage
 Provides-Extra: ssh
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -67,28 +68,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.4.0rc1``
+Release: ``4.5.0rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sftp`` provider. All classes for this provider package
 are in ``airflow.providers.sftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -112,18 +113,19 @@
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
 
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
-    pip install apache-airflow-providers-sftp[ssh]
+    pip install apache-airflow-providers-sftp[openlineage]
 
 
-==============================================================================================  =======
-Dependent package                                                                               Extra
-==============================================================================================  =======
-`apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_  ``ssh``
-==============================================================================================  =======
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+`apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                  ``ssh``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt` & `apache-airflow-providers-sftp-4.5.0rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/pyproject.toml` & `apache-airflow-providers-sftp-4.5.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
     "airflow/providers/common/sql/*/*.pyi",
-    "airflow/migrations/versions/*.py"
+    "airflow/migrations/versions/*.py",
+    "tests/dags/test_imports.py",
 ]
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
@@ -69,14 +70,16 @@
     "D212",
     "D213",
     "D214",
     "D215",
     "E731",
 ]
 
+namespace-packages = ["airflow/providers"]
+
 [tool.pytest.ini_options]
 # * Disable `flaky` plugin for pytest. This plugin conflicts with `rerunfailures` because provide same marker.
 # * Disable `nose` builtin plugin for pytest. This feature deprecated in 7.2 and will be removed in pytest>=8
 # * And we focus on use native pytest capabilities rather than adopt another frameworks.
 addopts = "-rasl --verbosity=2 -p no:flaky -p no:nose --asyncio-mode=strict"
 norecursedirs = [
     ".eggs",
@@ -95,54 +98,28 @@
     "ignore::DeprecationWarning:flask_appbuilder.widgets",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
-    "*.py",
+    "test_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
 required-imports = ["from __future__ import annotations"]
 combine-as-imports = true
 
-# TODO: for now, https://github.com/charliermarsh/ruff/issues/1817
-known-third-party = [
-    "asana",
-    "atlassian",
-    "celery",
-    "cloudant",
-    "databricks",
-    "datadog",
-    "docker",
-    "elasticsearch",
-    "github",
-    "google",
-    "grpc",
-    "jenkins",
-    "mysql",
-    "neo4j",
-    "papermill",
-    "redis",
-    "sendgrid",
-    "snowflake",
-    "telegram",
-    "trino",
-]
-
 [tool.ruff.per-file-ignores]
 "airflow/models/__init__.py" = ["F401"]
 "airflow/models/sqla_models.py" = ["F401"]
 
-
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
 "airflow/serialization/pydantic/*.py" = ["I002"]
```

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/setup.cfg` & `apache-airflow-providers-sftp-4.5.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.5.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-sftp-4.4.0rc1/setup.py` & `apache-airflow-providers-sftp-4.5.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-sftp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.4.0"
+version = "4.5.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-sftp setup."""
     setup(
         version=version,
-        extras_require={"ssh": ["apache-airflow-providers-ssh"]},
+        extras_require={
+            "openlineage": ["apache-airflow-providers-openlineage"],
+            "ssh": ["apache-airflow-providers-ssh"],
+        },
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.sftp",
                 "airflow.providers.sftp.*",
                 "airflow.providers.sftp_vendor",
                 "airflow.providers.sftp_vendor.*",
             ],
```

