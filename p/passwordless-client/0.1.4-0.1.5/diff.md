# Comparing `tmp/passwordless-client-0.1.4.tar.gz` & `tmp/passwordless-client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-client-0.1.4.tar", last modified: Tue Aug  1 13:04:39 2023, max compression
+gzip compressed data, was "passwordless-client-0.1.5.tar", last modified: Tue Aug  1 13:09:53 2023, max compression
```

## Comparing `passwordless-client-0.1.4.tar` & `passwordless-client-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 13:04:39.574367 passwordless-client-0.1.4/
--rw-rw-rw-   0        0        0     4395 2023-08-01 13:04:39.573862 passwordless-client-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3608 2023-08-01 16:57:10.000000 passwordless-client-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 13:04:39.572848 passwordless-client-0.1.4/passwordless_client.egg-info/
--rw-rw-rw-   0        0        0     4395 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 13:04:39.000000 passwordless-client-0.1.4/passwordless_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 13:04:39.574367 passwordless-client-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-08-01 13:04:10.000000 passwordless-client-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:09:53.875827 passwordless-client-0.1.5/
+-rw-rw-rw-   0        0        0     4410 2023-08-01 13:09:53.875322 passwordless-client-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3623 2023-08-01 13:09:17.000000 passwordless-client-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 13:09:53.874307 passwordless-client-0.1.5/passwordless_client.egg-info/
+-rw-rw-rw-   0        0        0     4410 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 13:09:53.875827 passwordless-client-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-08-01 13:09:34.000000 passwordless-client-0.1.5/setup.py
```

### Comparing `passwordless-client-0.1.4/PKG-INFO` & `passwordless-client-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: passwordless-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A client library for Passwordless.dev API
 Home-page: https://github.com/yourusername/passwordless-client
 Author: Matthew Fiallos
 Author-email: matthew.fiallos@randstadusa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 
-# Passwordless.dev Python SDK Client
+# Bitwarden Passwordless.dev Python 3.8+ SDK Client
 
 A Python client library for interacting with the Passwordless.dev API.
 
 ## Installation
 
 1. Install the package using pip:
```

### Comparing `passwordless-client-0.1.4/README.md` & `passwordless-client-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Passwordless.dev Python SDK Client
+# Bitwarden Passwordless.dev Python 3.8+ SDK Client
 
 A Python client library for interacting with the Passwordless.dev API.
 
 ## Installation
 
 1. Install the package using pip:
```

### Comparing `passwordless-client-0.1.4/passwordless_client.egg-info/PKG-INFO` & `passwordless-client-0.1.5/passwordless_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: passwordless-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A client library for Passwordless.dev API
 Home-page: https://github.com/yourusername/passwordless-client
 Author: Matthew Fiallos
 Author-email: matthew.fiallos@randstadusa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 
-# Passwordless.dev Python SDK Client
+# Bitwarden Passwordless.dev Python 3.8+ SDK Client
 
 A Python client library for interacting with the Passwordless.dev API.
 
 ## Installation
 
 1. Install the package using pip:
```

### Comparing `passwordless-client-0.1.4/setup.py` & `passwordless-client-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='passwordless-client',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Matthew Fiallos',
     author_email='matthew.fiallos@randstadusa.com',
     description='A client library for Passwordless.dev API',
```

