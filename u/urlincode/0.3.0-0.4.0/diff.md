# Comparing `tmp/urlincode-0.3.0.tar.gz` & `tmp/urlincode-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlincode-0.3.0.tar", last modified: Mon Jul 24 10:44:04 2023, max compression
+gzip compressed data, was "urlincode-0.4.0.tar", last modified: Tue Aug  1 13:25:55 2023, max compression
```

## Comparing `urlincode-0.3.0.tar` & `urlincode-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-07-24 10:44:04.260579 urlincode-0.3.0/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      238 2023-07-24 10:44:04.260579 urlincode-0.3.0/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-07-24 10:44:04.260579 urlincode-0.3.0/setup.cfg
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      358 2023-07-24 10:43:48.000000 urlincode-0.3.0/setup.py
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-07-24 10:44:04.260579 urlincode-0.3.0/urlincode.egg-info/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      238 2023-07-24 10:44:04.000000 urlincode-0.3.0/urlincode.egg-info/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      140 2023-07-24 10:44:04.000000 urlincode-0.3.0/urlincode.egg-info/SOURCES.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-07-24 10:44:04.000000 urlincode-0.3.0/urlincode.egg-info/dependency_links.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-07-24 10:44:04.000000 urlincode-0.3.0/urlincode.egg-info/top_level.txt
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 13:25:55.666000 urlincode-0.4.0/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      238 2023-08-01 13:25:55.666000 urlincode-0.4.0/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 13:25:55.666000 urlincode-0.4.0/setup.cfg
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      337 2023-08-01 13:25:16.000000 urlincode-0.4.0/setup.py
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 13:25:55.666000 urlincode-0.4.0/urlincode.egg-info/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      238 2023-08-01 13:25:55.000000 urlincode-0.4.0/urlincode.egg-info/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      140 2023-08-01 13:25:55.000000 urlincode-0.4.0/urlincode.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 13:25:55.000000 urlincode-0.4.0/urlincode.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 13:25:55.000000 urlincode-0.4.0/urlincode.egg-info/top_level.txt
```

