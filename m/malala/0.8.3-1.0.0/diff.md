# Comparing `tmp/malala-0.8.3.tar.gz` & `tmp/malala-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malala-0.8.3.tar", last modified: Tue Aug  1 19:44:43 2023, max compression
+gzip compressed data, was "malala-1.0.0.tar", last modified: Tue Aug  1 19:48:40 2023, max compression
```

## Comparing `malala-0.8.3.tar` & `malala-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:44:43.001376 malala-0.8.3/
--rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 19:44:43.001189 malala-0.8.3/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-0.8.3/README.md
--rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 19:44:43.001436 malala-0.8.3/setup.cfg
--rw-r--r--   0 jmf        (501) staff       (20)      466 2023-08-01 19:44:31.000000 malala-0.8.3/setup.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:44:42.996302 malala-0.8.3/src/
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:44:42.997506 malala-0.8.3/src/malala/
--rw-r--r--   0 jmf        (501) staff       (20)       69 2023-08-01 19:41:47.000000 malala-0.8.3/src/malala/__init__.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:44:42.999015 malala-0.8.3/src/malala/constants/
--rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-01 02:23:15.000000 malala-0.8.3/src/malala/constants/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)       75 2023-08-01 01:09:45.000000 malala-0.8.3/src/malala/constants/sockets.py
--rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-01 00:55:04.000000 malala-0.8.3/src/malala/constants/time.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:44:42.999417 malala-0.8.3/src/malala/logger/
--rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:55:01.000000 malala-0.8.3/src/malala/logger/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:43:31.000000 malala-0.8.3/src/malala/logger/logging.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:44:43.000393 malala-0.8.3/src/malala/sockets/
--rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-01 01:16:34.000000 malala-0.8.3/src/malala/sockets/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-01 01:15:29.000000 malala-0.8.3/src/malala/sockets/tcp_socket.py
--rw-r--r--   0 jmf        (501) staff       (20)     1189 2023-08-01 19:41:49.000000 malala-0.8.3/src/malala/sockets/transport.py
--rw-r--r--   0 jmf        (501) staff       (20)      735 2023-08-01 19:26:05.000000 malala-0.8.3/src/malala/sockets/unix_socket.py
--rw-r--r--   0 jmf        (501) staff       (20)     1835 2023-08-01 19:26:27.000000 malala-0.8.3/src/malala/sockets/websocket.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:44:43.000913 malala-0.8.3/src/malala/tasks/
--rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 01:18:20.000000 malala-0.8.3/src/malala/tasks/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-01 01:17:48.000000 malala-0.8.3/src/malala/tasks/tasks.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:44:42.998417 malala-0.8.3/src/malala.egg-info/
--rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 19:44:42.000000 malala-0.8.3/src/malala.egg-info/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      547 2023-08-01 19:44:42.000000 malala-0.8.3/src/malala.egg-info/SOURCES.txt
--rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 19:44:42.000000 malala-0.8.3/src/malala.egg-info/dependency_links.txt
--rw-r--r--   0 jmf        (501) staff       (20)        7 2023-08-01 19:44:42.000000 malala-0.8.3/src/malala.egg-info/top_level.txt
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.428255 malala-1.0.0/
+-rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 19:48:40.428143 malala-1.0.0/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-1.0.0/README.md
+-rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 19:48:40.428290 malala-1.0.0/setup.cfg
+-rw-r--r--   0 jmf        (501) staff       (20)      466 2023-08-01 19:47:59.000000 malala-1.0.0/setup.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.425506 malala-1.0.0/src/
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.426154 malala-1.0.0/src/malala/
+-rw-r--r--   0 jmf        (501) staff       (20)       69 2023-08-01 19:41:47.000000 malala-1.0.0/src/malala/__init__.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.426931 malala-1.0.0/src/malala/constants/
+-rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-01 02:23:15.000000 malala-1.0.0/src/malala/constants/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)       75 2023-08-01 01:09:45.000000 malala-1.0.0/src/malala/constants/sockets.py
+-rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-01 00:55:04.000000 malala-1.0.0/src/malala/constants/time.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.427146 malala-1.0.0/src/malala/logger/
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:55:01.000000 malala-1.0.0/src/malala/logger/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:43:31.000000 malala-1.0.0/src/malala/logger/logging.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.427759 malala-1.0.0/src/malala/sockets/
+-rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-01 01:16:34.000000 malala-1.0.0/src/malala/sockets/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-01 01:15:29.000000 malala-1.0.0/src/malala/sockets/tcp_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1189 2023-08-01 19:41:49.000000 malala-1.0.0/src/malala/sockets/transport.py
+-rw-r--r--   0 jmf        (501) staff       (20)      735 2023-08-01 19:26:05.000000 malala-1.0.0/src/malala/sockets/unix_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1835 2023-08-01 19:26:27.000000 malala-1.0.0/src/malala/sockets/websocket.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.428003 malala-1.0.0/src/malala/tasks/
+-rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 01:18:20.000000 malala-1.0.0/src/malala/tasks/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-01 01:17:48.000000 malala-1.0.0/src/malala/tasks/tasks.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.426608 malala-1.0.0/src/malala.egg-info/
+-rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 19:48:40.000000 malala-1.0.0/src/malala.egg-info/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      547 2023-08-01 19:48:40.000000 malala-1.0.0/src/malala.egg-info/SOURCES.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 19:48:40.000000 malala-1.0.0/src/malala.egg-info/dependency_links.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        7 2023-08-01 19:48:40.000000 malala-1.0.0/src/malala.egg-info/top_level.txt
```

### Comparing `malala-0.8.3/src/malala/sockets/tcp_socket.py` & `malala-1.0.0/src/malala/sockets/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `malala-0.8.3/src/malala/sockets/transport.py` & `malala-1.0.0/src/malala/sockets/transport.py`

 * *Files identical despite different names*

### Comparing `malala-0.8.3/src/malala/sockets/unix_socket.py` & `malala-1.0.0/src/malala/sockets/unix_socket.py`

 * *Files identical despite different names*

### Comparing `malala-0.8.3/src/malala/sockets/websocket.py` & `malala-1.0.0/src/malala/sockets/websocket.py`

 * *Files identical despite different names*

### Comparing `malala-0.8.3/src/malala/tasks/tasks.py` & `malala-1.0.0/src/malala/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `malala-0.8.3/src/malala.egg-info/SOURCES.txt` & `malala-1.0.0/src/malala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

