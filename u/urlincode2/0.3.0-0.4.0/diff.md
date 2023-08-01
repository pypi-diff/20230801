# Comparing `tmp/urlincode2-0.3.0.tar.gz` & `tmp/urlincode2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlincode2-0.3.0.tar", last modified: Tue Aug  1 18:26:24 2023, max compression
+gzip compressed data, was "urlincode2-0.4.0.tar", last modified: Tue Aug  1 18:30:34 2023, max compression
```

## Comparing `urlincode2-0.3.0.tar` & `urlincode2-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 18:26:24.436859 urlincode2-0.3.0/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      257 2023-08-01 18:26:24.436859 urlincode2-0.3.0/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 18:26:24.436859 urlincode2-0.3.0/setup.cfg
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      404 2023-08-01 18:26:17.000000 urlincode2-0.3.0/setup.py
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 18:26:24.436859 urlincode2-0.3.0/urlincode2.egg-info/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      257 2023-08-01 18:26:24.000000 urlincode2-0.3.0/urlincode2.egg-info/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-01 18:26:24.000000 urlincode2-0.3.0/urlincode2.egg-info/SOURCES.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 18:26:24.000000 urlincode2-0.3.0/urlincode2.egg-info/dependency_links.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 18:26:24.000000 urlincode2-0.3.0/urlincode2.egg-info/top_level.txt
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 18:30:34.843509 urlincode2-0.4.0/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      140 2023-08-01 18:30:34.843509 urlincode2-0.4.0/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 18:30:34.843509 urlincode2-0.4.0/setup.cfg
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      305 2023-08-01 18:30:28.000000 urlincode2-0.4.0/setup.py
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 18:30:34.843509 urlincode2-0.4.0/urlincode2.egg-info/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      140 2023-08-01 18:30:34.000000 urlincode2-0.4.0/urlincode2.egg-info/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-01 18:30:34.000000 urlincode2-0.4.0/urlincode2.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 18:30:34.000000 urlincode2-0.4.0/urlincode2.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 18:30:34.000000 urlincode2-0.4.0/urlincode2.egg-info/top_level.txt
```

