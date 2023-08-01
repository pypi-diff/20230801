# Comparing `tmp/shshsh-1.0.1.tar.gz` & `tmp/shshsh-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shshsh-1.0.1.tar", max compression
+gzip compressed data, was "shshsh-1.0.2.tar", max compression
```

## Comparing `shshsh-1.0.1.tar` & `shshsh-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1657 2023-08-01 18:09:47.654031 shshsh-1.0.1/README.md
--rw-r--r--   0        0        0      345 2023-08-01 18:05:36.107353 shshsh-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      176 2023-08-01 18:14:56.490713 shshsh-1.0.1/shshsh/__init__.py
--rw-r--r--   0        0        0       52 2023-08-01 19:00:12.394172 shshsh-1.0.1/shshsh/global_vars.py
--rw-r--r--   0        0        0      449 2023-07-29 15:04:40.678142 shshsh-1.0.1/shshsh/pipe.py
--rw-r--r--   0        0        0     2656 2023-08-01 19:05:37.427520 shshsh-1.0.1/shshsh/quick.py
--rw-r--r--   0        0        0    14782 2023-08-01 19:26:56.044246 shshsh-1.0.1/shshsh/shell.py
--rw-r--r--   0        0        0     5748 2023-08-01 19:06:50.924190 shshsh-1.0.1/shshsh/streamer.py
--rw-r--r--   0        0        0      934 2023-08-01 19:23:06.874235 shshsh-1.0.1/shshsh/utils.py
--rw-r--r--   0        0        0     2115 1970-01-01 00:00:00.000000 shshsh-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2420 2023-08-01 19:44:09.097627 shshsh-1.0.2/README.md
+-rw-r--r--   0        0        0      345 2023-08-01 19:47:35.550970 shshsh-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-08-01 18:14:56.490713 shshsh-1.0.2/shshsh/__init__.py
+-rw-r--r--   0        0        0       52 2023-08-01 19:00:12.394172 shshsh-1.0.2/shshsh/global_vars.py
+-rw-r--r--   0        0        0      449 2023-07-29 15:04:40.678142 shshsh-1.0.2/shshsh/pipe.py
+-rw-r--r--   0        0        0     2656 2023-08-01 19:05:37.427520 shshsh-1.0.2/shshsh/quick.py
+-rw-r--r--   0        0        0    14782 2023-08-01 19:26:56.044246 shshsh-1.0.2/shshsh/shell.py
+-rw-r--r--   0        0        0     5748 2023-08-01 19:06:50.924190 shshsh-1.0.2/shshsh/streamer.py
+-rw-r--r--   0        0        0      934 2023-08-01 19:23:06.874235 shshsh-1.0.2/shshsh/utils.py
+-rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 shshsh-1.0.2/PKG-INFO
```

### Comparing `shshsh-1.0.1/shshsh/quick.py` & `shshsh-1.0.2/shshsh/quick.py`

 * *Files identical despite different names*

### Comparing `shshsh-1.0.1/shshsh/shell.py` & `shshsh-1.0.2/shshsh/shell.py`

 * *Files identical despite different names*

### Comparing `shshsh-1.0.1/shshsh/streamer.py` & `shshsh-1.0.2/shshsh/streamer.py`

 * *Files identical despite different names*

### Comparing `shshsh-1.0.1/shshsh/utils.py` & `shshsh-1.0.2/shshsh/utils.py`

 * *Files identical despite different names*

