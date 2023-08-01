# Comparing `tmp/drone_env-0.0.1.tar.gz` & `tmp/drone_env-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drone_env-0.0.1.tar", last modified: Tue Aug  1 15:55:31 2023, max compression
+gzip compressed data, was "drone_env-0.0.2.tar", last modified: Tue Aug  1 16:35:22 2023, max compression
```

## Comparing `drone_env-0.0.1.tar` & `drone_env-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 15:55:31.122676 drone_env-0.0.1/
--rw-rw-rw-   0        0        0      105 2023-08-01 15:55:31.121676 drone_env-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 15:55:31.085676 drone_env-0.0.1/drone_env/
--rw-rw-rw-   0        0        0      143 2023-07-10 04:20:44.000000 drone_env-0.0.1/drone_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:55:31.120675 drone_env-0.0.1/drone_env/envs/
--rw-rw-rw-   0        0        0      171 2023-07-17 06:28:27.000000 drone_env-0.0.1/drone_env/envs/__init__.py
--rw-rw-rw-   0        0        0     8394 2023-08-01 14:47:42.000000 drone_env-0.0.1/drone_env/envs/drone_env.py
--rw-rw-rw-   0        0        0     3167 2023-07-17 06:58:43.000000 drone_env-0.0.1/drone_env/envs/simulink_connect.py
--rw-rw-rw-   0        0        0     4349 2023-08-01 14:25:09.000000 drone_env-0.0.1/drone_env/envs/track_generation.py
--rw-rw-rw-   0        0        0     2155 2023-08-01 07:44:59.000000 drone_env-0.0.1/drone_env/envs/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:55:31.121676 drone_env-0.0.1/drone_env/wrappers/
--rw-rw-rw-   0        0        0        0 2023-07-10 04:08:02.000000 drone_env-0.0.1/drone_env/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:55:31.103675 drone_env-0.0.1/drone_env.egg-info/
--rw-rw-rw-   0        0        0      105 2023-08-01 15:55:31.000000 drone_env-0.0.1/drone_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-08-01 15:55:31.000000 drone_env-0.0.1/drone_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 15:55:31.000000 drone_env-0.0.1/drone_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-08-01 15:55:31.000000 drone_env-0.0.1/drone_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 15:55:31.000000 drone_env-0.0.1/drone_env.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 15:55:31.122676 drone_env-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-08-01 15:55:17.000000 drone_env-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.054769 drone_env-0.0.2/
+-rw-rw-rw-   0        0        0      105 2023-08-01 16:35:22.054769 drone_env-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.028976 drone_env-0.0.2/drone_env/
+-rw-rw-rw-   0        0        0      134 2023-08-01 16:30:50.000000 drone_env-0.0.2/drone_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.052769 drone_env-0.0.2/drone_env/envs/
+-rw-rw-rw-   0        0        0      171 2023-07-17 06:28:27.000000 drone_env-0.0.2/drone_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     8394 2023-08-01 14:47:42.000000 drone_env-0.0.2/drone_env/envs/drone_env.py
+-rw-rw-rw-   0        0        0     3167 2023-07-17 06:58:43.000000 drone_env-0.0.2/drone_env/envs/simulink_connect.py
+-rw-rw-rw-   0        0        0     4349 2023-08-01 14:25:09.000000 drone_env-0.0.2/drone_env/envs/track_generation.py
+-rw-rw-rw-   0        0        0     2155 2023-08-01 07:44:59.000000 drone_env-0.0.2/drone_env/envs/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.053769 drone_env-0.0.2/drone_env/wrappers/
+-rw-rw-rw-   0        0        0        0 2023-07-10 04:08:02.000000 drone_env-0.0.2/drone_env/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:35:22.048777 drone_env-0.0.2/drone_env.egg-info/
+-rw-rw-rw-   0        0        0      105 2023-08-01 16:35:21.000000 drone_env-0.0.2/drone_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-08-01 16:35:22.000000 drone_env-0.0.2/drone_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 16:35:21.000000 drone_env-0.0.2/drone_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-01 16:35:21.000000 drone_env-0.0.2/drone_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 16:35:21.000000 drone_env-0.0.2/drone_env.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 16:35:22.054769 drone_env-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-08-01 16:35:14.000000 drone_env-0.0.2/setup.py
```

### Comparing `drone_env-0.0.1/drone_env/envs/drone_env.py` & `drone_env-0.0.2/drone_env/envs/drone_env.py`

 * *Files identical despite different names*

### Comparing `drone_env-0.0.1/drone_env/envs/simulink_connect.py` & `drone_env-0.0.2/drone_env/envs/simulink_connect.py`

 * *Files identical despite different names*

### Comparing `drone_env-0.0.1/drone_env/envs/track_generation.py` & `drone_env-0.0.2/drone_env/envs/track_generation.py`

 * *Files identical despite different names*

### Comparing `drone_env-0.0.1/drone_env/envs/utils.py` & `drone_env-0.0.2/drone_env/envs/utils.py`

 * *Files identical despite different names*

