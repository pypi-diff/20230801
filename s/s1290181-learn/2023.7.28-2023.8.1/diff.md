# Comparing `tmp/s1290181_learn-2023.7.28.tar.gz` & `tmp/s1290181_learn-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s1290181_learn-2023.7.28.tar", last modified: Fri Jul 28 05:08:34 2023, max compression
+gzip compressed data, was "s1290181_learn-2023.8.1.tar", last modified: Tue Aug  1 07:22:33 2023, max compression
```

## Comparing `s1290181_learn-2023.7.28.tar` & `s1290181_learn-2023.8.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 takanoriku   (501) staff       (20)        0 2023-07-28 05:08:34.334809 s1290181_learn-2023.7.28/
--rw-r--r--   0 takanoriku   (501) staff       (20)      143 2023-07-28 05:08:34.334413 s1290181_learn-2023.7.28/PKG-INFO
--rw-r--r--   0 takanoriku   (501) staff       (20)       17 2023-07-27 06:38:43.000000 s1290181_learn-2023.7.28/README.md
-drwxr-xr-x   0 takanoriku   (501) staff       (20)        0 2023-07-28 05:08:34.333749 s1290181_learn-2023.7.28/s1290181_learn.egg-info/
--rw-r--r--   0 takanoriku   (501) staff       (20)      143 2023-07-28 05:08:34.000000 s1290181_learn-2023.7.28/s1290181_learn.egg-info/PKG-INFO
--rw-r--r--   0 takanoriku   (501) staff       (20)      207 2023-07-28 05:08:34.000000 s1290181_learn-2023.7.28/s1290181_learn.egg-info/SOURCES.txt
--rw-r--r--   0 takanoriku   (501) staff       (20)        1 2023-07-28 05:08:34.000000 s1290181_learn-2023.7.28/s1290181_learn.egg-info/dependency_links.txt
--rw-r--r--   0 takanoriku   (501) staff       (20)       27 2023-07-28 05:08:34.000000 s1290181_learn-2023.7.28/s1290181_learn.egg-info/requires.txt
--rw-r--r--   0 takanoriku   (501) staff       (20)        1 2023-07-28 05:08:34.000000 s1290181_learn-2023.7.28/s1290181_learn.egg-info/top_level.txt
--rw-r--r--   0 takanoriku   (501) staff       (20)       38 2023-07-28 05:08:34.335148 s1290181_learn-2023.7.28/setup.cfg
--rw-r--r--   0 takanoriku   (501) staff       (20)      155 2023-07-28 05:00:41.000000 s1290181_learn-2023.7.28/setup.py
+drwxr-xr-x   0 takanoriku   (501) staff       (20)        0 2023-08-01 07:22:33.499583 s1290181_learn-2023.8.1/
+-rw-r--r--   0 takanoriku   (501) staff       (20)     1065 2023-08-01 06:51:52.000000 s1290181_learn-2023.8.1/LICENSE
+-rw-r--r--   0 takanoriku   (501) staff       (20)      164 2023-08-01 07:22:33.499192 s1290181_learn-2023.8.1/PKG-INFO
+-rw-r--r--   0 takanoriku   (501) staff       (20)       17 2023-07-27 06:38:43.000000 s1290181_learn-2023.8.1/README.md
+drwxr-xr-x   0 takanoriku   (501) staff       (20)        0 2023-08-01 07:22:33.498596 s1290181_learn-2023.8.1/s1290181_learn.egg-info/
+-rw-r--r--   0 takanoriku   (501) staff       (20)      164 2023-08-01 07:22:33.000000 s1290181_learn-2023.8.1/s1290181_learn.egg-info/PKG-INFO
+-rw-r--r--   0 takanoriku   (501) staff       (20)      215 2023-08-01 07:22:33.000000 s1290181_learn-2023.8.1/s1290181_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 takanoriku   (501) staff       (20)        1 2023-08-01 07:22:33.000000 s1290181_learn-2023.8.1/s1290181_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 takanoriku   (501) staff       (20)       19 2023-08-01 07:22:33.000000 s1290181_learn-2023.8.1/s1290181_learn.egg-info/requires.txt
+-rw-r--r--   0 takanoriku   (501) staff       (20)        1 2023-08-01 07:22:33.000000 s1290181_learn-2023.8.1/s1290181_learn.egg-info/top_level.txt
+-rw-r--r--   0 takanoriku   (501) staff       (20)       38 2023-08-01 07:22:33.499715 s1290181_learn-2023.8.1/setup.cfg
+-rw-r--r--   0 takanoriku   (501) staff       (20)      141 2023-08-01 07:22:29.000000 s1290181_learn-2023.8.1/setup.py
```

