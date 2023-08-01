# Comparing `tmp/mechanics-0.1.2.tar.gz` & `tmp/mechanics-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanics-0.1.2.tar", last modified: Tue Aug  1 17:56:01 2023, max compression
+gzip compressed data, was "mechanics-0.2.tar", last modified: Tue Aug  1 17:41:13 2023, max compression
```

## Comparing `mechanics-0.1.2.tar` & `mechanics-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-01 17:56:01.425500 mechanics-0.1.2/
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1762 2023-08-01 17:56:01.417334 mechanics-0.1.2/PKG-INFO
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1502 2023-08-01 17:21:26.000000 mechanics-0.1.2/README.md
-drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-01 17:56:01.348306 mechanics-0.1.2/mechanics.egg-info/
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1762 2023-08-01 17:56:00.000000 mechanics-0.1.2/mechanics.egg-info/PKG-INFO
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)      163 2023-08-01 17:56:00.000000 mechanics-0.1.2/mechanics.egg-info/SOURCES.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)        1 2023-08-01 17:56:00.000000 mechanics-0.1.2/mechanics.egg-info/dependency_links.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)       10 2023-08-01 17:56:00.000000 mechanics-0.1.2/mechanics.egg-info/top_level.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1079 2023-08-01 17:15:31.000000 mechanics-0.1.2/mechanics.py
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)       38 2023-08-01 17:56:01.428195 mechanics-0.1.2/setup.cfg
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)      446 2023-08-01 17:55:53.000000 mechanics-0.1.2/setup.py
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

### Comparing `mechanics-0.1.2/PKG-INFO` & `mechanics-0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: mechanics
-Version: 0.1.2
-Summary: A library for solving simple mechanics problems
-Home-page: UNKNOWN
-Author: alextras
-Author-email: alextrasias@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # My Library
 
 This is a Python library for solving simple mechanics problems. Currently, it includes functions for the following calculations:
 
 1. `final_velocity(initial_velocity, acceleration, time)`: This function calculates the final velocity of an object given the initial velocity, acceleration, and time. The inputs and output are in meters per second (m/s).
 
 2. `displacement(initial_velocity, time, acceleration)`: This function calculates the displacement of an object given the initial velocity, time, and acceleration. The inputs and output are in meters (m).
@@ -29,9 +18,7 @@
 
 ```python
 import mechanics
 
 v = mechanics.final_velocity(0, 9.8, 10)
 print(v)  # Prints: 98.0
 
-
-
```

### Comparing `mechanics-0.1.2/mechanics.py` & `mechanics-0.2/mechanics.py`

 * *Files identical despite different names*

