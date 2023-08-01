# Comparing `tmp/python_config_server_client-1.0.3.tar.gz` & `tmp/python_config_server_client-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python_config_server_client-1.0.3.tar", last modified: Tue Aug  1 07:23:51 2023, max compression
+gzip compressed data, was "dist/python_config_server_client-2.0.0.tar", last modified: Tue Aug  1 07:29:36 2023, max compression
```

## Comparing `python_config_server_client-1.0.3.tar` & `python_config_server_client-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/
--rw-r--r--   0 jayant     (501) staff       (20)      256 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/PKG-INFO
--rw-r--r--   0 jayant     (501) staff       (20)      317 2023-08-01 07:23:42.000000 python_config_server_client-1.0.3/setup.py
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/python_config_server_client.egg-info/
--rw-r--r--   0 jayant     (501) staff       (20)      256 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/python_config_server_client.egg-info/PKG-INFO
--rw-r--r--   0 jayant     (501) staff       (20)      262 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/python_config_server_client.egg-info/SOURCES.txt
--rw-r--r--   0 jayant     (501) staff       (20)        9 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/python_config_server_client.egg-info/requires.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/python_config_server_client.egg-info/top_level.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/python_config_server_client.egg-info/dependency_links.txt
--rw-r--r--   0 jayant     (501) staff       (20)       38 2023-08-01 07:23:51.000000 python_config_server_client-1.0.3/setup.cfg
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/
+-rw-r--r--   0 jayant     (501) staff       (20)      264 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)       32 2023-08-01 07:26:37.000000 python_config_server_client-2.0.0/README.md
+-rw-r--r--   0 jayant     (501) staff       (20)      325 2023-08-01 07:29:09.000000 python_config_server_client-2.0.0/setup.py
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/python_config_server_client.egg-info/
+-rw-r--r--   0 jayant     (501) staff       (20)      264 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/python_config_server_client.egg-info/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)      272 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/python_config_server_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        9 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/python_config_server_client.egg-info/requires.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/python_config_server_client.egg-info/top_level.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/python_config_server_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jayant     (501) staff       (20)       38 2023-08-01 07:29:36.000000 python_config_server_client-2.0.0/setup.cfg
```

