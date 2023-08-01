# Comparing `tmp/lynkpy-0.0.3.tar.gz` & `tmp/lynkpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lynkpy-0.0.3.tar", last modified: Tue Aug  1 07:21:30 2023, max compression
+gzip compressed data, was "lynkpy-0.0.4.tar", last modified: Tue Aug  1 07:27:30 2023, max compression
```

## Comparing `lynkpy-0.0.3.tar` & `lynkpy-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 07:21:30.798839 lynkpy-0.0.3/
--rw-rw-rw-   0        0        0      234 2023-08-01 07:21:30.778993 lynkpy-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 07:21:30.690307 lynkpy-0.0.3/lynkpy/
--rw-rw-rw-   0        0        0       25 2023-08-01 07:20:06.000000 lynkpy-0.0.3/lynkpy/__init__.py
--rw-rw-rw-   0        0        0      918 2023-07-31 08:46:21.000000 lynkpy-0.0.3/lynkpy/logger.py
-drwxrwxrwx   0        0        0        0 2023-08-01 07:21:30.771015 lynkpy-0.0.3/lynkpy.egg-info/
--rw-rw-rw-   0        0        0      234 2023-08-01 07:21:29.000000 lynkpy-0.0.3/lynkpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-08-01 07:21:30.000000 lynkpy-0.0.3/lynkpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:21:29.000000 lynkpy-0.0.3/lynkpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-01 07:21:29.000000 lynkpy-0.0.3/lynkpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-01 07:21:29.000000 lynkpy-0.0.3/lynkpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 07:21:30.799705 lynkpy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      494 2023-08-01 07:21:22.000000 lynkpy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:27:30.541009 lynkpy-0.0.4/
+-rw-rw-rw-   0        0        0      234 2023-08-01 07:27:30.536022 lynkpy-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 07:27:30.454132 lynkpy-0.0.4/lynkpy/
+-rw-rw-rw-   0        0        0       32 2023-08-01 07:26:39.000000 lynkpy-0.0.4/lynkpy/__init__.py
+-rw-rw-rw-   0        0        0      918 2023-07-31 08:46:21.000000 lynkpy-0.0.4/lynkpy/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:27:30.527185 lynkpy-0.0.4/lynkpy.egg-info/
+-rw-rw-rw-   0        0        0      234 2023-08-01 07:27:29.000000 lynkpy-0.0.4/lynkpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-08-01 07:27:30.000000 lynkpy-0.0.4/lynkpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:27:29.000000 lynkpy-0.0.4/lynkpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-01 07:27:29.000000 lynkpy-0.0.4/lynkpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 07:27:29.000000 lynkpy-0.0.4/lynkpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:27:30.543005 lynkpy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      494 2023-08-01 07:27:22.000000 lynkpy-0.0.4/setup.py
```

### Comparing `lynkpy-0.0.3/lynkpy/logger.py` & `lynkpy-0.0.4/lynkpy/logger.py`

 * *Files identical despite different names*

