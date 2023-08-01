# Comparing `tmp/gitlab_sdk-0.2.1.tar.gz` & `tmp/gitlab_sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_sdk-0.2.1.tar", last modified: Tue Aug  1 16:13:00 2023, max compression
+gzip compressed data, was "gitlab_sdk-0.2.3.tar", last modified: Tue Aug  1 16:52:44 2023, max compression
```

## Comparing `gitlab_sdk-0.2.1.tar` & `gitlab_sdk-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:13:00.632813 gitlab_sdk-0.2.1/
--rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 16:13:00.631812 gitlab_sdk-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:13:00.630813 gitlab_sdk-0.2.1/gitlab_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/gitlab_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/gitlab_sdk/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2445 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/gitlab_sdk/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:13:00.631812 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      293 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-08-01 16:13:00.000000 gitlab_sdk-0.2.1/gitlab_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 16:13:00.632813 gitlab_sdk-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:13:00.631812 gitlab_sdk-0.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-08-01 16:12:47.000000 gitlab_sdk-0.2.1/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:52:44.098429 gitlab_sdk-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 16:52:44.098429 gitlab_sdk-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:52:44.096429 gitlab_sdk-0.2.3/gitlab_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/gitlab_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/gitlab_sdk/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2445 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/gitlab_sdk/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:52:44.098429 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-01 16:52:44.000000 gitlab_sdk-0.2.3/gitlab_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 16:52:44.099429 gitlab_sdk-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      471 2023-08-01 16:52:29.000000 gitlab_sdk-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 16:52:44.098429 gitlab_sdk-0.2.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-08-01 16:52:28.000000 gitlab_sdk-0.2.3/tests/test_client.py
```

### Comparing `gitlab_sdk-0.2.1/README.md` & `gitlab_sdk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gitlab_sdk-0.2.1/gitlab_sdk/client.py` & `gitlab_sdk-0.2.3/gitlab_sdk/client.py`

 * *Files identical despite different names*

### Comparing `gitlab_sdk-0.2.1/tests/test_client.py` & `gitlab_sdk-0.2.3/tests/test_client.py`

 * *Files identical despite different names*

