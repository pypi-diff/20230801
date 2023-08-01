# Comparing `tmp/mongodriver-1.2.4.tar.gz` & `tmp/mongodriver-1.2.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.2.4.tar", last modified: Tue Aug  1 11:17:09 2023, max compression
+gzip compressed data, was "mongodriver-1.2.41.tar", last modified: Tue Aug  1 11:22:23 2023, max compression
```

## Comparing `mongodriver-1.2.4.tar` & `mongodriver-1.2.41.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:17:09.747630 mongodriver-1.2.4/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.4/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)      363 2023-08-01 11:17:09.747770 mongodriver-1.2.4/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.4/README.md
--rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.4/pyproject.toml
--rw-r--r--   0 jstrouse   (501) staff       (20)      491 2023-08-01 11:17:09.748170 mongodriver-1.2.4/setup.cfg
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:17:09.743393 mongodriver-1.2.4/src/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:17:09.746220 mongodriver-1.2.4/src/mongodriver/
--rw-r--r--   0 jstrouse   (501) staff       (20)       26 2023-08-01 11:16:52.000000 mongodriver-1.2.4/src/mongodriver/__init__.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     7965 2023-08-01 11:16:52.000000 mongodriver-1.2.4/src/mongodriver/mongodriver.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:17:09.747433 mongodriver-1.2.4/src/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)      363 2023-08-01 11:17:09.000000 mongodriver-1.2.4/src/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      295 2023-08-01 11:17:09.000000 mongodriver-1.2.4/src/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-08-01 11:17:09.000000 mongodriver-1.2.4/src/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-08-01 11:17:09.000000 mongodriver-1.2.4/src/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-08-01 11:17:09.000000 mongodriver-1.2.4/src/mongodriver.egg-info/top_level.txt
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:22:23.010102 mongodriver-1.2.41/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.41/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)      364 2023-08-01 11:22:23.010228 mongodriver-1.2.41/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.41/README.md
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.41/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)      492 2023-08-01 11:22:23.010620 mongodriver-1.2.41/setup.cfg
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:22:23.007710 mongodriver-1.2.41/src/
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2023-08-01 11:22:23.009900 mongodriver-1.2.41/src/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)      364 2023-08-01 11:22:23.000000 mongodriver-1.2.41/src/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      236 2023-08-01 11:22:23.000000 mongodriver-1.2.41/src/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-08-01 11:22:23.000000 mongodriver-1.2.41/src/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       29 2023-08-01 11:22:23.000000 mongodriver-1.2.41/src/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2023-08-01 11:22:23.000000 mongodriver-1.2.41/src/mongodriver.egg-info/top_level.txt
```

### Comparing `mongodriver-1.2.4/LICENSE` & `mongodriver-1.2.41/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.4/README.md` & `mongodriver-1.2.41/README.md`

 * *Files identical despite different names*

