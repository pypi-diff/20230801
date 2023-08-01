# Comparing `tmp/malala-0.8.1.tar.gz` & `tmp/malala-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malala-0.8.1.tar", last modified: Tue Aug  1 18:49:34 2023, max compression
+gzip compressed data, was "malala-0.8.2.tar", last modified: Tue Aug  1 19:14:09 2023, max compression
```

## Comparing `malala-0.8.1.tar` & `malala-0.8.2.tar`

### file list

```diff
@@ -1,10 +1,29 @@
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 18:49:34.431739 malala-0.8.1/
--rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 18:49:34.431561 malala-0.8.1/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-0.8.1/README.md
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 18:49:34.431411 malala-0.8.1/malala.egg-info/
--rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 18:49:34.000000 malala-0.8.1/malala.egg-info/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      138 2023-08-01 18:49:34.000000 malala-0.8.1/malala.egg-info/SOURCES.txt
--rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 18:49:34.000000 malala-0.8.1/malala.egg-info/dependency_links.txt
--rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 18:49:34.000000 malala-0.8.1/malala.egg-info/top_level.txt
--rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 18:49:34.431775 malala-0.8.1/setup.cfg
--rw-r--r--   0 jmf        (501) staff       (20)      426 2023-08-01 18:48:25.000000 malala-0.8.1/setup.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:14:09.070095 malala-0.8.2/
+-rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 19:14:09.069976 malala-0.8.2/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-0.8.2/README.md
+-rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 19:14:09.070131 malala-0.8.2/setup.cfg
+-rw-r--r--   0 jmf        (501) staff       (20)      466 2023-08-01 19:13:32.000000 malala-0.8.2/setup.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:14:09.065793 malala-0.8.2/src/
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:14:09.066426 malala-0.8.2/src/malala/
+-rw-r--r--   0 jmf        (501) staff       (20)       69 2023-08-01 03:29:26.000000 malala-0.8.2/src/malala/__init__.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:14:09.067798 malala-0.8.2/src/malala/constants/
+-rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-01 02:23:15.000000 malala-0.8.2/src/malala/constants/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)       75 2023-08-01 01:09:45.000000 malala-0.8.2/src/malala/constants/sockets.py
+-rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-01 00:55:04.000000 malala-0.8.2/src/malala/constants/time.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:14:09.068137 malala-0.8.2/src/malala/logger/
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:55:01.000000 malala-0.8.2/src/malala/logger/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:43:31.000000 malala-0.8.2/src/malala/logger/logging.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:14:09.069232 malala-0.8.2/src/malala/sockets/
+-rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-01 01:16:34.000000 malala-0.8.2/src/malala/sockets/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-01 01:15:29.000000 malala-0.8.2/src/malala/sockets/tcp_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1187 2023-08-01 01:14:23.000000 malala-0.8.2/src/malala/sockets/transport.py
+-rw-r--r--   0 jmf        (501) staff       (20)      733 2023-08-01 01:13:00.000000 malala-0.8.2/src/malala/sockets/unix_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1833 2023-08-01 01:11:57.000000 malala-0.8.2/src/malala/sockets/websocket.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:14:09.069701 malala-0.8.2/src/malala/tasks/
+-rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 01:18:20.000000 malala-0.8.2/src/malala/tasks/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-01 01:17:48.000000 malala-0.8.2/src/malala/tasks/tasks.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:14:09.067003 malala-0.8.2/src/malala.egg-info/
+-rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 19:14:09.000000 malala-0.8.2/src/malala.egg-info/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      547 2023-08-01 19:14:09.000000 malala-0.8.2/src/malala.egg-info/SOURCES.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 19:14:09.000000 malala-0.8.2/src/malala.egg-info/dependency_links.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        7 2023-08-01 19:14:09.000000 malala-0.8.2/src/malala.egg-info/top_level.txt
```

