# Comparing `tmp/malala-0.5.tar.gz` & `tmp/malala-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malala-0.5.tar", last modified: Tue Aug  1 04:18:20 2023, max compression
+gzip compressed data, was "malala-0.7.tar", last modified: Tue Aug  1 05:00:49 2023, max compression
```

## Comparing `malala-0.5.tar` & `malala-0.7.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 04:18:20.274579 malala-0.5/
--rw-r--r--   0 jmf        (501) staff       (20)      206 2023-08-01 04:18:20.274459 malala-0.5/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-0.5/README.md
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 04:18:20.274311 malala-0.5/malala.egg-info/
--rw-r--r--   0 jmf        (501) staff       (20)      206 2023-08-01 04:18:20.000000 malala-0.5/malala.egg-info/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      138 2023-08-01 04:18:20.000000 malala-0.5/malala.egg-info/SOURCES.txt
--rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 04:18:20.000000 malala-0.5/malala.egg-info/dependency_links.txt
--rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 04:18:20.000000 malala-0.5/malala.egg-info/top_level.txt
--rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 04:18:20.274620 malala-0.5/setup.cfg
--rw-r--r--   0 jmf        (501) staff       (20)      474 2023-08-01 04:17:57.000000 malala-0.5/setup.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 05:00:49.578992 malala-0.7/
+-rw-r--r--   0 jmf        (501) staff       (20)      206 2023-08-01 05:00:49.578727 malala-0.7/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-0.7/README.md
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 05:00:49.578358 malala-0.7/malala.egg-info/
+-rw-r--r--   0 jmf        (501) staff       (20)      206 2023-08-01 05:00:49.000000 malala-0.7/malala.egg-info/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      129 2023-08-01 05:00:49.000000 malala-0.7/malala.egg-info/SOURCES.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 05:00:49.000000 malala-0.7/malala.egg-info/dependency_links.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 05:00:49.000000 malala-0.7/malala.egg-info/top_level.txt
+-rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 05:00:49.579075 malala-0.7/setup.cfg
```

