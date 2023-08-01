# Comparing `tmp/malala_labs-0.1.tar.gz` & `tmp/malala_labs-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malala_labs-0.1.tar", last modified: Tue Aug  1 02:18:15 2023, max compression
+gzip compressed data, was "malala_labs-0.2.tar", last modified: Tue Aug  1 02:23:46 2023, max compression
```

## Comparing `malala_labs-0.1.tar` & `malala_labs-0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:18:15.847362 malala_labs-0.1/
--rw-r--r--   0 jmf        (501) staff       (20)      211 2023-08-01 02:18:15.847251 malala_labs-0.1/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala_labs-0.1/README.md
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:18:15.844798 malala_labs-0.1/constants/
--rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-01 00:53:01.000000 malala_labs-0.1/constants/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)       75 2023-08-01 01:09:45.000000 malala_labs-0.1/constants/sockets.py
--rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-01 00:55:04.000000 malala_labs-0.1/constants/time.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:18:15.845086 malala_labs-0.1/logger/
--rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:55:01.000000 malala_labs-0.1/logger/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:43:31.000000 malala_labs-0.1/logger/logging.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:18:15.845630 malala_labs-0.1/malala_labs.egg-info/
--rw-r--r--   0 jmf        (501) staff       (20)      211 2023-08-01 02:18:15.000000 malala_labs-0.1/malala_labs.egg-info/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      430 2023-08-01 02:18:15.000000 malala_labs-0.1/malala_labs.egg-info/SOURCES.txt
--rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 02:18:15.000000 malala_labs-0.1/malala_labs.egg-info/dependency_links.txt
--rw-r--r--   0 jmf        (501) staff       (20)       59 2023-08-01 02:18:15.000000 malala_labs-0.1/malala_labs.egg-info/requires.txt
--rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 02:18:15.000000 malala_labs-0.1/malala_labs.egg-info/top_level.txt
--rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 02:18:15.847397 malala_labs-0.1/setup.cfg
--rw-r--r--   0 jmf        (501) staff       (20)      508 2023-08-01 02:17:37.000000 malala_labs-0.1/setup.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:18:15.846601 malala_labs-0.1/sockets/
--rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-01 01:16:34.000000 malala_labs-0.1/sockets/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-01 01:15:29.000000 malala_labs-0.1/sockets/tcp_socket.py
--rw-r--r--   0 jmf        (501) staff       (20)     1187 2023-08-01 01:14:23.000000 malala_labs-0.1/sockets/transport.py
--rw-r--r--   0 jmf        (501) staff       (20)      733 2023-08-01 01:13:00.000000 malala_labs-0.1/sockets/unix_socket.py
--rw-r--r--   0 jmf        (501) staff       (20)     1833 2023-08-01 01:11:57.000000 malala_labs-0.1/sockets/websocket.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:18:15.846996 malala_labs-0.1/tasks/
--rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 01:18:20.000000 malala_labs-0.1/tasks/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-01 01:17:48.000000 malala_labs-0.1/tasks/tasks.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:23:46.413166 malala_labs-0.2/
+-rw-r--r--   0 jmf        (501) staff       (20)      211 2023-08-01 02:23:46.413044 malala_labs-0.2/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala_labs-0.2/README.md
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:23:46.411142 malala_labs-0.2/constants/
+-rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-01 02:23:15.000000 malala_labs-0.2/constants/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)       75 2023-08-01 01:09:45.000000 malala_labs-0.2/constants/sockets.py
+-rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-01 00:55:04.000000 malala_labs-0.2/constants/time.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:23:46.411336 malala_labs-0.2/logger/
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:55:01.000000 malala_labs-0.2/logger/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:43:31.000000 malala_labs-0.2/logger/logging.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:23:46.411880 malala_labs-0.2/malala_labs.egg-info/
+-rw-r--r--   0 jmf        (501) staff       (20)      211 2023-08-01 02:23:46.000000 malala_labs-0.2/malala_labs.egg-info/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      430 2023-08-01 02:23:46.000000 malala_labs-0.2/malala_labs.egg-info/SOURCES.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 02:23:46.000000 malala_labs-0.2/malala_labs.egg-info/dependency_links.txt
+-rw-r--r--   0 jmf        (501) staff       (20)       13 2023-08-01 02:23:46.000000 malala_labs-0.2/malala_labs.egg-info/requires.txt
+-rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 02:23:46.000000 malala_labs-0.2/malala_labs.egg-info/top_level.txt
+-rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 02:23:46.413202 malala_labs-0.2/setup.cfg
+-rw-r--r--   0 jmf        (501) staff       (20)      508 2023-08-01 02:22:16.000000 malala_labs-0.2/setup.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:23:46.412486 malala_labs-0.2/sockets/
+-rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-01 01:16:34.000000 malala_labs-0.2/sockets/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-01 01:15:29.000000 malala_labs-0.2/sockets/tcp_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1187 2023-08-01 01:14:23.000000 malala_labs-0.2/sockets/transport.py
+-rw-r--r--   0 jmf        (501) staff       (20)      733 2023-08-01 01:13:00.000000 malala_labs-0.2/sockets/unix_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1833 2023-08-01 01:11:57.000000 malala_labs-0.2/sockets/websocket.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 02:23:46.412742 malala_labs-0.2/tasks/
+-rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 01:18:20.000000 malala_labs-0.2/tasks/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-01 01:17:48.000000 malala_labs-0.2/tasks/tasks.py
```

### Comparing `malala_labs-0.1/sockets/tcp_socket.py` & `malala_labs-0.2/sockets/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `malala_labs-0.1/sockets/transport.py` & `malala_labs-0.2/sockets/transport.py`

 * *Files identical despite different names*

### Comparing `malala_labs-0.1/sockets/unix_socket.py` & `malala_labs-0.2/sockets/unix_socket.py`

 * *Files identical despite different names*

### Comparing `malala_labs-0.1/sockets/websocket.py` & `malala_labs-0.2/sockets/websocket.py`

 * *Files identical despite different names*

### Comparing `malala_labs-0.1/tasks/tasks.py` & `malala_labs-0.2/tasks/tasks.py`

 * *Files identical despite different names*

