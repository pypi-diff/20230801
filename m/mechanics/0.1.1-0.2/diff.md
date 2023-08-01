# Comparing `tmp/mechanics-0.1.1.tar.gz` & `tmp/mechanics-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanics-0.1.1.tar", last modified: Tue Aug  1 17:50:13 2023, max compression
+gzip compressed data, was "mechanics-0.2.tar", last modified: Tue Aug  1 17:41:13 2023, max compression
```

## Comparing `mechanics-0.1.1.tar` & `mechanics-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-01 17:50:13.944923 mechanics-0.1.1/
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)      227 2023-08-01 17:50:13.936925 mechanics-0.1.1/PKG-INFO
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1502 2023-08-01 17:21:26.000000 mechanics-0.1.1/README.md
-drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-01 17:50:13.862001 mechanics-0.1.1/mechanics.egg-info/
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)      227 2023-08-01 17:50:13.000000 mechanics-0.1.1/mechanics.egg-info/PKG-INFO
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)      163 2023-08-01 17:50:13.000000 mechanics-0.1.1/mechanics.egg-info/SOURCES.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)        1 2023-08-01 17:50:13.000000 mechanics-0.1.1/mechanics.egg-info/dependency_links.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)       10 2023-08-01 17:50:13.000000 mechanics-0.1.1/mechanics.egg-info/top_level.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1079 2023-08-01 17:15:31.000000 mechanics-0.1.1/mechanics.py
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)       38 2023-08-01 17:50:13.948926 mechanics-0.1.1/setup.cfg
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)      356 2023-08-01 17:50:08.000000 mechanics-0.1.1/setup.py
+drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-01 17:41:13.509314 mechanics-0.2/
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)      225 2023-08-01 17:41:13.501321 mechanics-0.2/PKG-INFO
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1502 2023-08-01 17:21:26.000000 mechanics-0.2/README.md
+drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-01 17:41:13.432312 mechanics-0.2/mechanics.egg-info/
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)      225 2023-08-01 17:41:12.000000 mechanics-0.2/mechanics.egg-info/PKG-INFO
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)      163 2023-08-01 17:41:12.000000 mechanics-0.2/mechanics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)        1 2023-08-01 17:41:12.000000 mechanics-0.2/mechanics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)       10 2023-08-01 17:41:12.000000 mechanics-0.2/mechanics.egg-info/top_level.txt
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1079 2023-08-01 17:15:31.000000 mechanics-0.2/mechanics.py
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)       38 2023-08-01 17:41:13.515313 mechanics-0.2/setup.cfg
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)      266 2023-08-01 17:41:07.000000 mechanics-0.2/setup.py
```

### Comparing `mechanics-0.1.1/README.md` & `mechanics-0.2/README.md`

 * *Files identical despite different names*

### Comparing `mechanics-0.1.1/mechanics.py` & `mechanics-0.2/mechanics.py`

 * *Files identical despite different names*

