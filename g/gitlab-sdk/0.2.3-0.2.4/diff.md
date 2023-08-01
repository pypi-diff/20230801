# Comparing `tmp/gitlab_sdk-0.2.3.tar.gz` & `tmp/gitlab_sdk-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_sdk-0.2.3.tar", last modified: Tue Aug  1 16:52:44 2023, max compression
+gzip compressed data, was "gitlab_sdk-0.2.4.tar", last modified: Tue Aug  1 17:06:26 2023, max compression
```

## Comparing `gitlab_sdk-0.2.3.tar` & `gitlab_sdk-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:52:44.098429 gitlab_sdk-0.2.3/
--rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 16:52:44.098429 gitlab_sdk-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:52:44.096429 gitlab_sdk-0.2.3/gitlab_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/gitlab_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/gitlab_sdk/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2445 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/gitlab_sdk/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:52:44.098429 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      293 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 16:52:44.099429 gitlab_sdk-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      471 2023-08-01 16:52:29.000000 gitlab_sdk-0.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:52:44.098429 gitlab_sdk-0.2.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 17:06:26.757894 gitlab_sdk-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 17:06:26.757894 gitlab_sdk-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2023-08-01 17:06:12.000000 gitlab_sdk-0.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 17:06:26.755894 gitlab_sdk-0.2.4/gitlab_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-08-01 17:06:12.000000 gitlab_sdk-0.2.4/gitlab_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-01 17:06:12.000000 gitlab_sdk-0.2.4/gitlab_sdk/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2445 2023-08-01 17:06:12.000000 gitlab_sdk-0.2.4/gitlab_sdk/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 17:06:26.756894 gitlab_sdk-0.2.4/gitlab_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 17:06:26.000000 gitlab_sdk-0.2.4/gitlab_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2023-08-01 17:06:26.000000 gitlab_sdk-0.2.4/gitlab_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 17:06:26.000000 gitlab_sdk-0.2.4/gitlab_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-08-01 17:06:26.000000 gitlab_sdk-0.2.4/gitlab_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-01 17:06:26.000000 gitlab_sdk-0.2.4/gitlab_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 17:06:26.757894 gitlab_sdk-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      471 2023-08-01 17:06:13.000000 gitlab_sdk-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 17:06:26.757894 gitlab_sdk-0.2.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 17:06:12.000000 gitlab_sdk-0.2.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-08-01 17:06:12.000000 gitlab_sdk-0.2.4/tests/test_client.py
```

### Comparing `gitlab_sdk-0.2.3/README.md` & `gitlab_sdk-0.2.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # GitLab Application SDK - Python
 
 This SDK is for using GitLab Application Services with Python.
 
 ## How to use the SDK
 
-### Installing the package
+### Installing the package using pip
 
-To install the package, enter the direction of this repository and run:
+To install the package run:
 
 ```bash
-python setup.py install
+pip install gitlab_sdk
 ```
 
 ### Using the client
 
 Initialize the client:
 
 ```python
```

### Comparing `gitlab_sdk-0.2.3/gitlab_sdk/client.py` & `gitlab_sdk-0.2.4/gitlab_sdk/client.py`

 * *Files identical despite different names*

### Comparing `gitlab_sdk-0.2.3/tests/test_client.py` & `gitlab_sdk-0.2.4/tests/test_client.py`

 * *Files identical despite different names*

