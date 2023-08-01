# Comparing `tmp/passwordless-client-0.1.5.tar.gz` & `tmp/passwordless-client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-client-0.1.5.tar", last modified: Tue Aug  1 13:09:53 2023, max compression
+gzip compressed data, was "passwordless-client-0.1.6.tar", last modified: Tue Aug  1 13:30:14 2023, max compression
```

## Comparing `passwordless-client-0.1.5.tar` & `passwordless-client-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 13:09:53.875827 passwordless-client-0.1.5/
--rw-rw-rw-   0        0        0     4410 2023-08-01 13:09:53.875322 passwordless-client-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3623 2023-08-01 13:09:17.000000 passwordless-client-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 13:09:53.874307 passwordless-client-0.1.5/passwordless_client.egg-info/
--rw-rw-rw-   0        0        0     4410 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 13:09:53.000000 passwordless-client-0.1.5/passwordless_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 13:09:53.875827 passwordless-client-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-08-01 13:09:34.000000 passwordless-client-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:30:14.903492 passwordless-client-0.1.6/
+-rw-rw-rw-   0        0        0     4421 2023-08-01 13:30:14.902982 passwordless-client-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3623 2023-08-01 13:09:17.000000 passwordless-client-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 13:30:14.899934 passwordless-client-0.1.6/passwordless/
+-rw-rw-rw-   0        0        0       38 2023-08-01 13:27:57.000000 passwordless-client-0.1.6/passwordless/__init__.py
+-rw-rw-rw-   0        0        0     2171 2023-08-01 16:57:10.000000 passwordless-client-0.1.6/passwordless/client.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:30:14.902475 passwordless-client-0.1.6/passwordless_client.egg-info/
+-rw-rw-rw-   0        0        0     4421 2023-08-01 13:30:14.000000 passwordless-client-0.1.6/passwordless_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-08-01 13:30:14.000000 passwordless-client-0.1.6/passwordless_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:30:14.000000 passwordless-client-0.1.6/passwordless_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 13:30:14.000000 passwordless-client-0.1.6/passwordless_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 13:30:14.000000 passwordless-client-0.1.6/passwordless_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 13:30:14.903492 passwordless-client-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-08-01 13:29:28.000000 passwordless-client-0.1.6/setup.py
```

### Comparing `passwordless-client-0.1.5/PKG-INFO` & `passwordless-client-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: passwordless-client
-Version: 0.1.5
-Summary: A client library for Passwordless.dev API
+Version: 0.1.6
+Summary: A client library for Bitwardens Passwordless.dev API
 Home-page: https://github.com/yourusername/passwordless-client
 Author: Matthew Fiallos
 Author-email: matthew.fiallos@randstadusa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `passwordless-client-0.1.5/README.md` & `passwordless-client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `passwordless-client-0.1.5/passwordless_client.egg-info/PKG-INFO` & `passwordless-client-0.1.6/passwordless_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: passwordless-client
-Version: 0.1.5
-Summary: A client library for Passwordless.dev API
+Version: 0.1.6
+Summary: A client library for Bitwardens Passwordless.dev API
 Home-page: https://github.com/yourusername/passwordless-client
 Author: Matthew Fiallos
 Author-email: matthew.fiallos@randstadusa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `passwordless-client-0.1.5/setup.py` & `passwordless-client-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='passwordless-client',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Matthew Fiallos',
     author_email='matthew.fiallos@randstadusa.com',
-    description='A client library for Passwordless.dev API',
+    description='A client library for Bitwarden''s Passwordless.dev API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/passwordless-client',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

