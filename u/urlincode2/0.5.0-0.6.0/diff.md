# Comparing `tmp/urlincode2-0.5.0.tar.gz` & `tmp/urlincode2-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlincode2-0.5.0.tar", last modified: Tue Aug  1 13:35:03 2023, max compression
+gzip compressed data, was "urlincode2-0.6.0.tar", last modified: Tue Aug  1 13:58:24 2023, max compression
```

## Comparing `urlincode2-0.5.0.tar` & `urlincode2-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 13:35:03.753496 urlincode2-0.5.0/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      239 2023-08-01 13:35:03.753496 urlincode2-0.5.0/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 13:35:03.753496 urlincode2-0.5.0/setup.cfg
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      338 2023-08-01 13:33:57.000000 urlincode2-0.5.0/setup.py
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 13:35:03.753496 urlincode2-0.5.0/urlincode2.egg-info/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      239 2023-08-01 13:35:03.000000 urlincode2-0.5.0/urlincode2.egg-info/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-01 13:35:03.000000 urlincode2-0.5.0/urlincode2.egg-info/SOURCES.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 13:35:03.000000 urlincode2-0.5.0/urlincode2.egg-info/dependency_links.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 13:35:03.000000 urlincode2-0.5.0/urlincode2.egg-info/top_level.txt
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 13:58:24.135453 urlincode2-0.6.0/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      709 2023-08-01 13:58:24.135453 urlincode2-0.6.0/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 13:58:24.135453 urlincode2-0.6.0/setup.cfg
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      808 2023-08-01 13:58:05.000000 urlincode2-0.6.0/setup.py
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 13:58:24.135453 urlincode2-0.6.0/urlincode2.egg-info/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      709 2023-08-01 13:58:24.000000 urlincode2-0.6.0/urlincode2.egg-info/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-01 13:58:24.000000 urlincode2-0.6.0/urlincode2.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 13:58:24.000000 urlincode2-0.6.0/urlincode2.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 13:58:24.000000 urlincode2-0.6.0/urlincode2.egg-info/top_level.txt
```

