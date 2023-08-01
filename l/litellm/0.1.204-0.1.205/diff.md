# Comparing `tmp/litellm-0.1.204.tar.gz` & `tmp/litellm-0.1.205.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.204.tar", last modified: Tue Aug  1 00:48:52 2023, max compression
+gzip compressed data, was "litellm-0.1.205.tar", last modified: Tue Aug  1 01:52:10 2023, max compression
```

## Comparing `litellm-0.1.204.tar` & `litellm-0.1.205.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:48:52.024226 litellm-0.1.204/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 00:48:29.000000 litellm-0.1.204/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 00:48:52.024226 litellm-0.1.204/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-08-01 00:48:29.000000 litellm-0.1.204/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:48:52.024226 litellm-0.1.204/litellm/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 00:48:29.000000 litellm-0.1.204/litellm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19254 2023-08-01 00:48:29.000000 litellm-0.1.204/litellm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:48:52.024226 litellm-0.1.204/litellm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 00:48:51.000000 litellm-0.1.204/litellm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:48:52.024226 litellm-0.1.204/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 00:48:29.000000 litellm-0.1.204/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:52:10.700031 litellm-0.1.205/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 01:51:52.000000 litellm-0.1.205/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 01:52:10.700031 litellm-0.1.205/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-08-01 01:51:52.000000 litellm-0.1.205/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:52:10.700031 litellm-0.1.205/litellm/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-01 01:51:52.000000 litellm-0.1.205/litellm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-08-01 01:51:52.000000 litellm-0.1.205/litellm/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-08-01 01:51:52.000000 litellm-0.1.205/litellm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:52:10.700031 litellm-0.1.205/litellm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 01:52:10.000000 litellm-0.1.205/litellm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:52:10.700031 litellm-0.1.205/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 01:51:52.000000 litellm-0.1.205/setup.py
```

### Comparing `litellm-0.1.204/LICENSE` & `litellm-0.1.205/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.204/README.md` & `litellm-0.1.205/README.md`

 * *Files identical despite different names*

