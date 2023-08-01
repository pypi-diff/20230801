# Comparing `tmp/lynkpy-0.0.4.tar.gz` & `tmp/lynkpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lynkpy-0.0.4.tar", last modified: Tue Aug  1 07:27:30 2023, max compression
+gzip compressed data, was "lynkpy-0.0.5.tar", last modified: Tue Aug  1 08:10:25 2023, max compression
```

## Comparing `lynkpy-0.0.4.tar` & `lynkpy-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 07:27:30.541009 lynkpy-0.0.4/
--rw-rw-rw-   0        0        0      234 2023-08-01 07:27:30.536022 lynkpy-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 07:27:30.454132 lynkpy-0.0.4/lynkpy/
--rw-rw-rw-   0        0        0       32 2023-08-01 07:26:39.000000 lynkpy-0.0.4/lynkpy/__init__.py
--rw-rw-rw-   0        0        0      918 2023-07-31 08:46:21.000000 lynkpy-0.0.4/lynkpy/logger.py
-drwxrwxrwx   0        0        0        0 2023-08-01 07:27:30.527185 lynkpy-0.0.4/lynkpy.egg-info/
--rw-rw-rw-   0        0        0      234 2023-08-01 07:27:29.000000 lynkpy-0.0.4/lynkpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-08-01 07:27:30.000000 lynkpy-0.0.4/lynkpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:27:29.000000 lynkpy-0.0.4/lynkpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-01 07:27:29.000000 lynkpy-0.0.4/lynkpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-01 07:27:29.000000 lynkpy-0.0.4/lynkpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 07:27:30.543005 lynkpy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      494 2023-08-01 07:27:22.000000 lynkpy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:10:25.857752 lynkpy-0.0.5/
+-rw-rw-rw-   0        0        0      234 2023-08-01 08:10:25.855429 lynkpy-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 08:10:25.778843 lynkpy-0.0.5/lynkpy/
+-rw-rw-rw-   0        0        0       32 2023-08-01 07:26:39.000000 lynkpy-0.0.5/lynkpy/__init__.py
+-rw-rw-rw-   0        0        0     1740 2023-08-01 08:08:09.000000 lynkpy-0.0.5/lynkpy/image.py
+-rw-rw-rw-   0        0        0      918 2023-07-31 08:46:21.000000 lynkpy-0.0.5/lynkpy/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:10:25.848217 lynkpy-0.0.5/lynkpy.egg-info/
+-rw-rw-rw-   0        0        0      234 2023-08-01 08:10:25.000000 lynkpy-0.0.5/lynkpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-08-01 08:10:25.000000 lynkpy-0.0.5/lynkpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:10:25.000000 lynkpy-0.0.5/lynkpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-08-01 08:10:25.000000 lynkpy-0.0.5/lynkpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 08:10:25.000000 lynkpy-0.0.5/lynkpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:10:25.858723 lynkpy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      504 2023-08-01 08:09:36.000000 lynkpy-0.0.5/setup.py
```

### Comparing `lynkpy-0.0.4/lynkpy/logger.py` & `lynkpy-0.0.5/lynkpy/logger.py`

 * *Files identical despite different names*

