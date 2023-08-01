# Comparing `tmp/malala-0.3.tar.gz` & `tmp/malala-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malala-0.3.tar", last modified: Tue Aug  1 03:32:35 2023, max compression
+gzip compressed data, was "malala-0.4.tar", last modified: Tue Aug  1 04:00:44 2023, max compression
```

## Comparing `malala-0.3.tar` & `malala-0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 03:32:35.062692 malala-0.3/
--rw-r--r--   0 jmf        (501) staff       (20)      206 2023-08-01 03:32:35.062470 malala-0.3/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-0.3/README.md
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 03:32:35.060001 malala-0.3/constants/
--rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-01 02:23:15.000000 malala-0.3/constants/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)       75 2023-08-01 01:09:45.000000 malala-0.3/constants/sockets.py
--rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-01 00:55:04.000000 malala-0.3/constants/time.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 03:32:35.060312 malala-0.3/logger/
--rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:55:01.000000 malala-0.3/logger/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:43:31.000000 malala-0.3/logger/logging.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 03:32:35.060732 malala-0.3/malala.egg-info/
--rw-r--r--   0 jmf        (501) staff       (20)      206 2023-08-01 03:32:35.000000 malala-0.3/malala.egg-info/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      376 2023-08-01 03:32:35.000000 malala-0.3/malala.egg-info/SOURCES.txt
--rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 03:32:35.000000 malala-0.3/malala.egg-info/dependency_links.txt
--rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 03:32:35.000000 malala-0.3/malala.egg-info/top_level.txt
--rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 03:32:35.062738 malala-0.3/setup.cfg
--rw-r--r--   0 jmf        (501) staff       (20)      444 2023-08-01 03:30:38.000000 malala-0.3/setup.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 03:32:35.061715 malala-0.3/sockets/
--rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-01 01:16:34.000000 malala-0.3/sockets/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-01 01:15:29.000000 malala-0.3/sockets/tcp_socket.py
--rw-r--r--   0 jmf        (501) staff       (20)     1187 2023-08-01 01:14:23.000000 malala-0.3/sockets/transport.py
--rw-r--r--   0 jmf        (501) staff       (20)      733 2023-08-01 01:13:00.000000 malala-0.3/sockets/unix_socket.py
--rw-r--r--   0 jmf        (501) staff       (20)     1833 2023-08-01 01:11:57.000000 malala-0.3/sockets/websocket.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 03:32:35.062144 malala-0.3/tasks/
--rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 01:18:20.000000 malala-0.3/tasks/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-01 01:17:48.000000 malala-0.3/tasks/tasks.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 04:00:44.997428 malala-0.4/
+-rw-r--r--   0 jmf        (501) staff       (20)      206 2023-08-01 04:00:44.997263 malala-0.4/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-0.4/README.md
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 04:00:44.994971 malala-0.4/constants/
+-rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-01 02:23:15.000000 malala-0.4/constants/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)       75 2023-08-01 01:09:45.000000 malala-0.4/constants/sockets.py
+-rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-01 00:55:04.000000 malala-0.4/constants/time.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 04:00:44.995279 malala-0.4/logger/
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:55:01.000000 malala-0.4/logger/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:43:31.000000 malala-0.4/logger/logging.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 04:00:44.995922 malala-0.4/malala.egg-info/
+-rw-r--r--   0 jmf        (501) staff       (20)      206 2023-08-01 04:00:44.000000 malala-0.4/malala.egg-info/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      376 2023-08-01 04:00:44.000000 malala-0.4/malala.egg-info/SOURCES.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 04:00:44.000000 malala-0.4/malala.egg-info/dependency_links.txt
+-rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 04:00:44.000000 malala-0.4/malala.egg-info/top_level.txt
+-rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 04:00:44.997478 malala-0.4/setup.cfg
+-rw-r--r--   0 jmf        (501) staff       (20)      444 2023-08-01 03:53:16.000000 malala-0.4/setup.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 04:00:44.996730 malala-0.4/sockets/
+-rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-01 01:16:34.000000 malala-0.4/sockets/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-01 01:15:29.000000 malala-0.4/sockets/tcp_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1187 2023-08-01 01:14:23.000000 malala-0.4/sockets/transport.py
+-rw-r--r--   0 jmf        (501) staff       (20)      733 2023-08-01 01:13:00.000000 malala-0.4/sockets/unix_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1833 2023-08-01 01:11:57.000000 malala-0.4/sockets/websocket.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 04:00:44.997026 malala-0.4/tasks/
+-rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 01:18:20.000000 malala-0.4/tasks/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-01 01:17:48.000000 malala-0.4/tasks/tasks.py
```

### Comparing `malala-0.3/sockets/tcp_socket.py` & `malala-0.4/sockets/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `malala-0.3/sockets/transport.py` & `malala-0.4/sockets/transport.py`

 * *Files identical despite different names*

### Comparing `malala-0.3/sockets/unix_socket.py` & `malala-0.4/sockets/unix_socket.py`

 * *Files identical despite different names*

### Comparing `malala-0.3/sockets/websocket.py` & `malala-0.4/sockets/websocket.py`

 * *Files identical despite different names*

### Comparing `malala-0.3/tasks/tasks.py` & `malala-0.4/tasks/tasks.py`

 * *Files identical despite different names*

