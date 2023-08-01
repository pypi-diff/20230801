# Comparing `tmp/tm_config_server_client_python-0.4.tar.gz` & `tmp/tm_config_server_client_python-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tm_config_server_client_python-0.4.tar", last modified: Tue Aug  1 09:42:26 2023, max compression
+gzip compressed data, was "dist/tm_config_server_client_python-0.5.tar", last modified: Tue Aug  1 09:54:19 2023, max compression
```

## Comparing `tm_config_server_client_python-0.4.tar` & `tm_config_server_client_python-0.5.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/
--rw-r--r--   0 jayant     (501) staff       (20)      253 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/PKG-INFO
--rw-rw-r--   0 jayant     (501) staff       (20)       38 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/setup.cfg
--rw-rw-r--   0 jayant     (501) staff       (20)      279 2023-08-01 09:42:23.000000 tm_config_server_client_python-0.4/setup.py
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/tm_config_server_client_python/
--rw-rw-r--   0 jayant     (501) staff       (20)     4648 2018-06-19 18:46:08.000000 tm_config_server_client_python-0.4/tm_config_server_client_python/Binomialdistribution.py
--rw-rw-r--   0 jayant     (501) staff       (20)     3631 2018-06-19 18:46:08.000000 tm_config_server_client_python-0.4/tm_config_server_client_python/Gaussiandistribution.py
--rw-rw-r--   0 jayant     (501) staff       (20)      932 2018-06-19 18:46:08.000000 tm_config_server_client_python-0.4/tm_config_server_client_python/Generaldistribution.py
--rw-r--r--   0 jayant     (501) staff       (20)       87 2023-08-01 09:41:27.000000 tm_config_server_client_python-0.4/tm_config_server_client_python/Pythonclient.py
--rw-rw-r--   0 jayant     (501) staff       (20)      125 2023-08-01 09:41:59.000000 tm_config_server_client_python-0.4/tm_config_server_client_python/__init__.py
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/tm_config_server_client_python.egg-info/
--rw-r--r--   0 jayant     (501) staff       (20)      253 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/tm_config_server_client_python.egg-info/PKG-INFO
--rw-r--r--   0 jayant     (501) staff       (20)      541 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/tm_config_server_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/tm_config_server_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/tm_config_server_client_python.egg-info/not-zip-safe
--rw-r--r--   0 jayant     (501) staff       (20)       31 2023-08-01 09:42:26.000000 tm_config_server_client_python-0.4/tm_config_server_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/
+-rw-r--r--   0 jayant     (501) staff       (20)      253 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/PKG-INFO
+-rw-rw-r--   0 jayant     (501) staff       (20)       38 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/setup.cfg
+-rw-rw-r--   0 jayant     (501) staff       (20)      279 2023-08-01 09:54:17.000000 tm_config_server_client_python-0.5/setup.py
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/tm_config_server_client_python/
+-rw-r--r--   0 jayant     (501) staff       (20)       87 2023-08-01 09:41:27.000000 tm_config_server_client_python-0.5/tm_config_server_client_python/Pythonclient.py
+-rw-rw-r--   0 jayant     (501) staff       (20)       39 2023-08-01 09:53:59.000000 tm_config_server_client_python-0.5/tm_config_server_client_python/__init__.py
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/tm_config_server_client_python.egg-info/
+-rw-r--r--   0 jayant     (501) staff       (20)      253 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/tm_config_server_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)      377 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/tm_config_server_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/tm_config_server_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/tm_config_server_client_python.egg-info/not-zip-safe
+-rw-r--r--   0 jayant     (501) staff       (20)       31 2023-08-01 09:54:19.000000 tm_config_server_client_python-0.5/tm_config_server_client_python.egg-info/top_level.txt
```

