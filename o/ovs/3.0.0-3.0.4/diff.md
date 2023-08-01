# Comparing `tmp/ovs-3.0.0.tar.gz` & `tmp/ovs-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovs-3.0.0.tar", last modified: Tue Aug  1 18:47:51 2023, max compression
+gzip compressed data, was "ovs-3.0.4.tar", last modified: Tue Aug  1 19:22:37 2023, max compression
```

## Comparing `ovs-3.0.0.tar` & `ovs-3.0.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.685744 ovs-3.0.0/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 18:47:51.685744 ovs-3.0.0/PKG-INFO
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       45 2021-09-20 16:15:26.000000 ovs-3.0.0/README.rst
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.680744 ovs-3.0.0/ovs/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     7038 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/_json.c
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.681744 ovs-3.0.0/ovs/compat/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)        0 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/compat/__init__.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.682744 ovs-3.0.0/ovs/compat/sortedcontainers/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     2131 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/compat/sortedcontainers/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    22712 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/compat/sortedcontainers/sorteddict.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    76293 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/compat/sortedcontainers/sortedlist.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    19825 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/compat/sortedcontainers/sortedset.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    20710 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/daemon.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.683744 ovs-3.0.0/ovs/db/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/db/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     4856 2021-11-05 13:35:58.000000 ovs-3.0.0/ovs/db/custom_index.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    21659 2023-06-14 20:52:13.000000 ovs-3.0.0/ovs/db/data.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1156 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/db/error.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    96770 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/db/idl.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3647 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/db/parser.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    11947 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/db/schema.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    23240 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/db/types.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1329 2023-08-01 18:44:12.000000 ovs-3.0.0/ovs/dirs.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     4765 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/fatal_signal.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1330 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/fcntl_win.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.684744 ovs-3.0.0/ovs/flow/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)      476 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/flow/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    14382 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/flow/decoders.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     7502 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/flow/filter.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3772 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/flow/flow.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    10505 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/kv.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3819 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/list.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    26900 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/odp.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    13396 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/ofp.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     8786 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/ofp_act.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     7348 2023-08-01 18:44:27.000000 ovs-3.0.0/ovs/flow/ofp_fields.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    16843 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/json.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    21087 2023-04-18 01:01:46.000000 ovs-3.0.0/ovs/jsonrpc.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1869 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/ovsuuid.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    10282 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/poller.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1467 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/process.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    26007 2023-05-17 03:37:46.000000 ovs-3.0.0/ovs/reconnect.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    11976 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/socket_util.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    32107 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/stream.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     2432 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/timeval.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.684744 ovs-3.0.0/ovs/unixctl/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3032 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/unixctl/__init__.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1999 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/unixctl/client.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     8121 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/unixctl/server.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     3120 2022-09-19 19:15:14.000000 ovs-3.0.0/ovs/util.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       93 2023-08-01 18:44:27.000000 ovs-3.0.0/ovs/version.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)    16694 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/vlog.py
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     9226 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/winutils.py
-drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.681744 ovs-3.0.0/ovs.egg-info/
--rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/PKG-INFO
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     1028 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/SOURCES.txt
--rw-rw-r--   0 twilson   (1000) twilson   (1000)        1 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/dependency_links.txt
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       84 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/requires.txt
--rw-rw-r--   0 twilson   (1000) twilson   (1000)        4 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/top_level.txt
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       85 2022-04-28 18:38:11.000000 ovs-3.0.0/pyproject.toml
--rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2023-08-01 18:47:51.685744 ovs-3.0.0/setup.cfg
--rw-rw-r--   0 twilson   (1000) twilson   (1000)     4350 2023-08-01 15:27:48.000000 ovs-3.0.0/setup.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.230654 ovs-3.0.4/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 19:22:37.229654 ovs-3.0.4/PKG-INFO
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       45 2021-09-20 16:15:26.000000 ovs-3.0.4/README.rst
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.226654 ovs-3.0.4/ovs/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     7038 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/_json.c
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.226654 ovs-3.0.4/ovs/compat/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        0 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/compat/__init__.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.227654 ovs-3.0.4/ovs/compat/sortedcontainers/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     2131 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/compat/sortedcontainers/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    22712 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/compat/sortedcontainers/sorteddict.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    76293 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/compat/sortedcontainers/sortedlist.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    19825 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/compat/sortedcontainers/sortedset.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    20710 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/daemon.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.228654 ovs-3.0.4/ovs/db/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/db/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4856 2021-11-05 13:35:58.000000 ovs-3.0.4/ovs/db/custom_index.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    21659 2023-06-14 20:52:13.000000 ovs-3.0.4/ovs/db/data.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1156 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/db/error.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    96817 2023-08-01 18:54:03.000000 ovs-3.0.4/ovs/db/idl.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3647 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/db/parser.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    11947 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/db/schema.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    23240 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/db/types.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1329 2023-08-01 18:44:12.000000 ovs-3.0.4/ovs/dirs.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4765 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/fatal_signal.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1330 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/fcntl_win.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.229654 ovs-3.0.4/ovs/flow/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      476 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/flow/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    14382 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/flow/decoders.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     7502 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/flow/filter.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3772 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/flow/flow.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    10505 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/flow/kv.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3819 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/flow/list.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    27561 2023-08-01 18:54:03.000000 ovs-3.0.4/ovs/flow/odp.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    13396 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/flow/ofp.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     8786 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/flow/ofp_act.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     7348 2023-08-01 18:55:30.000000 ovs-3.0.4/ovs/flow/ofp_fields.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    16843 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/json.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    21087 2023-04-18 01:01:46.000000 ovs-3.0.4/ovs/jsonrpc.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1869 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/ovsuuid.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    10282 2023-01-27 14:27:10.000000 ovs-3.0.4/ovs/poller.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1467 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/process.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    26007 2023-05-17 03:37:46.000000 ovs-3.0.4/ovs/reconnect.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    11976 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/socket_util.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    32107 2023-08-01 15:27:48.000000 ovs-3.0.4/ovs/stream.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     2432 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/timeval.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.229654 ovs-3.0.4/ovs/unixctl/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3032 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/unixctl/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1999 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/unixctl/client.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     8121 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/unixctl/server.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3120 2022-09-19 19:15:14.000000 ovs-3.0.4/ovs/util.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       93 2023-08-01 18:55:30.000000 ovs-3.0.4/ovs/version.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    16694 2021-10-20 17:21:43.000000 ovs-3.0.4/ovs/vlog.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     9226 2021-09-20 16:15:26.000000 ovs-3.0.4/ovs/winutils.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 19:22:37.226654 ovs-3.0.4/ovs.egg-info/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/PKG-INFO
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1028 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/SOURCES.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        1 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/dependency_links.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       84 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/requires.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        4 2023-08-01 19:22:37.000000 ovs-3.0.4/ovs.egg-info/top_level.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       85 2022-04-28 18:38:11.000000 ovs-3.0.4/pyproject.toml
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2023-08-01 19:22:37.230654 ovs-3.0.4/setup.cfg
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4350 2023-08-01 15:27:48.000000 ovs-3.0.4/setup.py
```

### Comparing `ovs-3.0.0/PKG-INFO` & `ovs-3.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovs
-Version: 3.0.0
+Version: 3.0.4
 Summary: Open vSwitch library
 Home-page: http://www.openvswitch.org/
 Author: Open vSwitch
 Author-email: dev@openvswitch.org
 License: Apache 2.0
 Keywords: openvswitch,ovs,OVSDB
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ovs-3.0.0/ovs/_json.c` & `ovs-3.0.4/ovs/_json.c`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/compat/sortedcontainers/__init__.py` & `ovs-3.0.4/ovs/compat/sortedcontainers/__init__.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/compat/sortedcontainers/sorteddict.py` & `ovs-3.0.4/ovs/compat/sortedcontainers/sorteddict.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/compat/sortedcontainers/sortedlist.py` & `ovs-3.0.4/ovs/compat/sortedcontainers/sortedlist.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/compat/sortedcontainers/sortedset.py` & `ovs-3.0.4/ovs/compat/sortedcontainers/sortedset.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/daemon.py` & `ovs-3.0.4/ovs/daemon.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/db/custom_index.py` & `ovs-3.0.4/ovs/db/custom_index.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/db/data.py` & `ovs-3.0.4/ovs/db/data.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/db/error.py` & `ovs-3.0.4/ovs/db/error.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/db/idl.py` & `ovs-3.0.4/ovs/db/idl.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,17 +81,17 @@
     monitor = OVSDB_UPDATE
     monitor_cond = OVSDB_UPDATE2
     monitor_cond_since = OVSDB_UPDATE3
 
 
 class ConditionState(object):
     def __init__(self):
-        self._ack_cond = None
+        self._ack_cond = [True]
         self._req_cond = None
-        self._new_cond = [True]
+        self._new_cond = None
 
     def __iter__(self):
         return iter([self._new_cond, self._req_cond, self._ack_cond])
 
     @property
     def new(self):
         """The latest freshly initialized condition change"""
@@ -1291,15 +1291,16 @@
     def __hash__(self):
         return int(self.__dict__['uuid'])
 
     def __str__(self):
         return "{table}({data})".format(
             table=self._table.name,
             data=", ".join("{col}={val}".format(col=c, val=getattr(self, c))
-                           for c in sorted(self._table.columns)))
+                           for c in sorted(self._table.columns)
+                           if hasattr(self, c)))
 
     def _uuid_to_row(self, atom, base):
         if base.ref_table:
             try:
                 table = self._idl.tables[base.ref_table.name]
             except KeyError as e:
                 msg = "Table {} is not registered".format(base.ref_table.name)
```

### Comparing `ovs-3.0.0/ovs/db/parser.py` & `ovs-3.0.4/ovs/db/parser.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/db/schema.py` & `ovs-3.0.4/ovs/db/schema.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/db/types.py` & `ovs-3.0.4/ovs/db/types.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/dirs.py` & `ovs-3.0.4/ovs/dirs.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/fatal_signal.py` & `ovs-3.0.4/ovs/fatal_signal.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/fcntl_win.py` & `ovs-3.0.4/ovs/fcntl_win.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/flow/decoders.py` & `ovs-3.0.4/ovs/flow/decoders.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/flow/filter.py` & `ovs-3.0.4/ovs/flow/filter.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/flow/flow.py` & `ovs-3.0.4/ovs/flow/flow.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/flow/kv.py` & `ovs-3.0.4/ovs/flow/kv.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/flow/list.py` & `ovs-3.0.4/ovs/flow/list.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/flow/odp.py` & `ovs-3.0.4/ovs/flow/odp.py`

 * *Files 5% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                             )
                         ),
                         "slow_path": decode_default,
                         "flow_sample": nested_kv_decoder(
                             KVDecoders(
                                 {
                                     "probability": decode_int,
-                                    "collector_sed_id": decode_int,
+                                    "collector_set_id": decode_int,
                                     "obs_domain_id": decode_int,
                                     "obs_point_id": decode_int,
                                     "output_port": decode_default,
                                     "ingress": decode_flag,
                                     "egress": decode_flag,
                                 }
                             )
@@ -299,14 +299,29 @@
                         "c4": decode_int,
                         "md2": decode_int,
                     }
                 )
             ),
             "pop_nsh": decode_flag,
             "tnl_pop": decode_int,
+            "pop_mpls": KVDecoders({"eth_type": decode_int}),
+            **dict.fromkeys(
+                ["push_mpls", "add_mpls"],
+                nested_kv_decoder(
+                    KVDecoders(
+                        {
+                            "label": decode_int,
+                            "tc": decode_int,
+                            "ttl": decode_int,
+                            "bos": decode_int,
+                            "eth_type": decode_int,
+                        }
+                    )
+                ),
+            ),
             "ct_clear": decode_flag,
             "ct": nested_kv_decoder(
                 KVDecoders(
                     {
                         "commit": decode_flag,
                         "force_commit": decode_flag,
                         "zone": decode_int,
@@ -408,15 +423,15 @@
                                         )
                                     ),
                                     "udp": nested_kv_decoder(
                                         KVDecoders(
                                             {
                                                 "src": decode_int,
                                                 "dst": decode_int,
-                                                "dsum": Mask16,
+                                                "csum": Mask16,
                                             }
                                         )
                                     ),
                                     "vxlan": nested_kv_decoder(
                                         KVDecoders(
                                             {
                                                 "flags": decode_int,
@@ -495,16 +510,16 @@
             "ct_label": Mask128,
             "ct_tuple4": nested_kv_decoder(
                 KVDecoders(
                     {
                         "src": IPMask,
                         "dst": IPMask,
                         "proto": Mask8,
-                        "tcp_src": Mask16,
-                        "tcp_dst": Mask16,
+                        "tp_src": Mask16,
+                        "tp_dst": Mask16,
                     }
                 )
             ),
             "ct_tuple6": nested_kv_decoder(
                 KVDecoders(
                     {
                         "src": IPMask,
@@ -537,22 +552,24 @@
                                     "hwid": Mask8,
                                 }
                             )
                         ),
                         "vxlan": nested_kv_decoder(
                             KVDecoders(
                                 {
+                                    "flags": decode_int,
+                                    "vni": decode_int,
                                     "gbp": nested_kv_decoder(
                                         KVDecoders(
                                             {
                                                 "id": Mask16,
                                                 "flags": Mask8,
                                             }
                                         )
-                                    )
+                                    ),
                                 }
                             )
                         ),
                         "geneve": partial(decode_geneve, True),
                         "gtpu": nested_kv_decoder(
                             KVDecoders(
                                 {
```

### Comparing `ovs-3.0.0/ovs/flow/ofp.py` & `ovs-3.0.4/ovs/flow/ofp.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/flow/ofp_act.py` & `ovs-3.0.4/ovs/flow/ofp_act.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/flow/ofp_fields.py` & `ovs-3.0.4/ovs/flow/ofp_fields.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/json.py` & `ovs-3.0.4/ovs/json.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/jsonrpc.py` & `ovs-3.0.4/ovs/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/ovsuuid.py` & `ovs-3.0.4/ovs/ovsuuid.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/poller.py` & `ovs-3.0.4/ovs/poller.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/process.py` & `ovs-3.0.4/ovs/process.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/reconnect.py` & `ovs-3.0.4/ovs/reconnect.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/socket_util.py` & `ovs-3.0.4/ovs/socket_util.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/stream.py` & `ovs-3.0.4/ovs/stream.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/timeval.py` & `ovs-3.0.4/ovs/timeval.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/unixctl/__init__.py` & `ovs-3.0.4/ovs/unixctl/__init__.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/unixctl/client.py` & `ovs-3.0.4/ovs/unixctl/client.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/unixctl/server.py` & `ovs-3.0.4/ovs/unixctl/server.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/util.py` & `ovs-3.0.4/ovs/util.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/vlog.py` & `ovs-3.0.4/ovs/vlog.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs/winutils.py` & `ovs-3.0.4/ovs/winutils.py`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/ovs.egg-info/PKG-INFO` & `ovs-3.0.4/ovs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovs
-Version: 3.0.0
+Version: 3.0.4
 Summary: Open vSwitch library
 Home-page: http://www.openvswitch.org/
 Author: Open vSwitch
 Author-email: dev@openvswitch.org
 License: Apache 2.0
 Keywords: openvswitch,ovs,OVSDB
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ovs-3.0.0/ovs.egg-info/SOURCES.txt` & `ovs-3.0.4/ovs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovs-3.0.0/setup.py` & `ovs-3.0.4/setup.py`

 * *Files identical despite different names*

