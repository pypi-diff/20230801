# Comparing `tmp/python_config_server_client-1.0.1.tar.gz` & `tmp/python_config_server_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python_config_server_client-1.0.1.tar", last modified: Tue Aug  1 06:17:27 2023, max compression
+gzip compressed data, was "dist/python_config_server_client-1.0.2.tar", last modified: Tue Aug  1 07:15:56 2023, max compression
```

## Comparing `python_config_server_client-1.0.1.tar` & `python_config_server_client-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/
--rw-r--r--   0 jayant     (501) staff       (20)      256 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/PKG-INFO
--rw-r--r--   0 jayant     (501) staff       (20)      317 2023-08-01 06:17:14.000000 python_config_server_client-1.0.1/setup.py
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/python_config_server_client.egg-info/
--rw-r--r--   0 jayant     (501) staff       (20)      256 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/python_config_server_client.egg-info/PKG-INFO
--rw-r--r--   0 jayant     (501) staff       (20)      262 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/python_config_server_client.egg-info/SOURCES.txt
--rw-r--r--   0 jayant     (501) staff       (20)        9 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/python_config_server_client.egg-info/requires.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/python_config_server_client.egg-info/top_level.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/python_config_server_client.egg-info/dependency_links.txt
--rw-r--r--   0 jayant     (501) staff       (20)       38 2023-08-01 06:17:27.000000 python_config_server_client-1.0.1/setup.cfg
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/
+-rw-r--r--   0 jayant     (501) staff       (20)      256 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)      317 2023-08-01 07:15:31.000000 python_config_server_client-1.0.2/setup.py
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/python_config_server_client.egg-info/
+-rw-r--r--   0 jayant     (501) staff       (20)      256 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/python_config_server_client.egg-info/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)      262 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/python_config_server_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        9 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/python_config_server_client.egg-info/requires.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/python_config_server_client.egg-info/top_level.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/python_config_server_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jayant     (501) staff       (20)       38 2023-08-01 07:15:56.000000 python_config_server_client-1.0.2/setup.cfg
```

