# Comparing `tmp/pyrotash-0.1.tar.gz` & `tmp/pyrotash-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrotash-0.1.tar", last modified: Sat Jul 29 13:15:38 2023, max compression
+gzip compressed data, was "pyrotash-0.2.tar", last modified: Tue Aug  1 09:23:20 2023, max compression
```

## Comparing `pyrotash-0.1.tar` & `pyrotash-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 13:15:38.013162 pyrotash-0.1/
--rw-rw-rw-   0        0        0      325 2023-07-29 13:15:38.011170 pyrotash-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 13:15:37.955505 pyrotash-0.1/pyrotash.egg-info/
--rw-rw-rw-   0        0        0      325 2023-07-29 13:15:37.000000 pyrotash-0.1/pyrotash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-29 13:15:37.000000 pyrotash-0.1/pyrotash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 13:15:37.000000 pyrotash-0.1/pyrotash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 13:15:37.000000 pyrotash-0.1/pyrotash.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 13:15:38.013162 pyrotash-0.1/setup.cfg
--rw-rw-rw-   0        0        0      482 2023-07-29 13:14:48.000000 pyrotash-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 13:15:38.009214 pyrotash-0.1/tpyconfig/
--rw-rw-rw-   0        0        0       89 2023-07-29 13:14:07.000000 pyrotash-0.1/tpyconfig/__init__.py
--rw-rw-rw-   0        0        0      114 2023-07-29 13:13:56.000000 pyrotash-0.1/tpyconfig/tpyconfig.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:23:20.177477 pyrotash-0.2/
+-rw-rw-rw-   0        0        0      325 2023-08-01 09:23:20.073756 pyrotash-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 09:23:20.065781 pyrotash-0.2/pyrotash.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-08-01 09:23:18.000000 pyrotash-0.2/pyrotash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-08-01 09:23:18.000000 pyrotash-0.2/pyrotash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:23:18.000000 pyrotash-0.2/pyrotash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 09:23:18.000000 pyrotash-0.2/pyrotash.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:23:20.178473 pyrotash-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      482 2023-08-01 09:11:15.000000 pyrotash-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:23:20.071761 pyrotash-0.2/tpyconfig/
+-rw-rw-rw-   0        0        0       89 2023-07-29 13:14:07.000000 pyrotash-0.2/tpyconfig/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-08-01 09:09:44.000000 pyrotash-0.2/tpyconfig/tpyconfig.py
```

