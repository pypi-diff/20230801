# Comparing `tmp/pyfiscal-2.0.tar.gz` & `tmp/pyfiscal-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfiscal-2.0.tar", last modified: Sat Mar 26 23:14:23 2022, max compression
+gzip compressed data, was "pyfiscal-2.1.tar", last modified: Tue Aug  1 07:01:23 2023, max compression
```

## Comparing `pyfiscal-2.0.tar` & `pyfiscal-2.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 iamroot   (1000) iamroot   (1000)        0 2022-03-26 23:14:23.382648 pyfiscal-2.0/
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)       82 2022-02-22 23:40:51.000000 pyfiscal-2.0/MANIFEST.in
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)      590 2022-03-26 23:14:23.382648 pyfiscal-2.0/PKG-INFO
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     1911 2022-02-22 23:40:51.000000 pyfiscal-2.0/README.md
-drwxrwxr-x   0 iamroot   (1000) iamroot   (1000)        0 2022-03-26 23:14:23.382648 pyfiscal-2.0/pyfiscal/
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)        0 2022-02-22 23:40:51.000000 pyfiscal-2.0/pyfiscal/__init__.py
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)    10906 2022-03-26 22:11:07.000000 pyfiscal-2.0/pyfiscal/base.py
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     9293 2022-03-26 22:10:44.000000 pyfiscal-2.0/pyfiscal/generate.py
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     1044 2022-03-26 07:06:19.000000 pyfiscal-2.0/pyfiscal/utils.py
-drwxrwxr-x   0 iamroot   (1000) iamroot   (1000)        0 2022-03-26 23:14:23.382648 pyfiscal-2.0/pyfiscal.egg-info/
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)      590 2022-03-26 23:14:23.000000 pyfiscal-2.0/pyfiscal.egg-info/PKG-INFO
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)      245 2022-03-26 23:14:23.000000 pyfiscal-2.0/pyfiscal.egg-info/SOURCES.txt
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)        1 2022-03-26 23:14:23.000000 pyfiscal-2.0/pyfiscal.egg-info/dependency_links.txt
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)        9 2022-03-26 23:14:23.000000 pyfiscal-2.0/pyfiscal.egg-info/top_level.txt
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)       79 2022-03-26 23:14:23.382648 pyfiscal-2.0/setup.cfg
--rw-rw-r--   0 iamroot   (1000) iamroot   (1000)      739 2022-03-26 23:09:55.000000 pyfiscal-2.0/setup.py
+drwxrwxr-x   0 iamroot   (1000) iamroot   (1000)        0 2023-08-01 07:01:23.241272 pyfiscal-2.1/
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     1063 2023-08-01 06:31:13.000000 pyfiscal-2.1/LICENSE
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)       82 2023-08-01 06:31:13.000000 pyfiscal-2.1/MANIFEST.in
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)      658 2023-08-01 07:01:23.241272 pyfiscal-2.1/PKG-INFO
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     1417 2023-08-01 07:00:59.000000 pyfiscal-2.1/README.md
+drwxrwxr-x   0 iamroot   (1000) iamroot   (1000)        0 2023-08-01 07:01:23.241272 pyfiscal-2.1/pyfiscal/
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)        0 2023-08-01 06:31:13.000000 pyfiscal-2.1/pyfiscal/__init__.py
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)    11367 2023-08-01 06:31:13.000000 pyfiscal-2.1/pyfiscal/base.py
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     3841 2023-08-01 06:31:13.000000 pyfiscal-2.1/pyfiscal/constants.py
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     7172 2023-08-01 06:31:13.000000 pyfiscal-2.1/pyfiscal/generate.py
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     3412 2023-08-01 06:31:13.000000 pyfiscal-2.1/pyfiscal/helpers.py
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     1481 2023-08-01 06:31:13.000000 pyfiscal-2.1/pyfiscal/utils.py
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)     1637 2023-08-01 06:31:13.000000 pyfiscal-2.1/pyfiscal/validators.py
+drwxrwxr-x   0 iamroot   (1000) iamroot   (1000)        0 2023-08-01 07:01:23.241272 pyfiscal-2.1/pyfiscal.egg-info/
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)      658 2023-08-01 07:01:23.000000 pyfiscal-2.1/pyfiscal.egg-info/PKG-INFO
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)      318 2023-08-01 07:01:23.000000 pyfiscal-2.1/pyfiscal.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)        1 2023-08-01 07:01:23.000000 pyfiscal-2.1/pyfiscal.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)        9 2023-08-01 07:01:23.000000 pyfiscal-2.1/pyfiscal.egg-info/top_level.txt
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)       79 2023-08-01 07:01:23.241272 pyfiscal-2.1/setup.cfg
+-rw-rw-r--   0 iamroot   (1000) iamroot   (1000)      674 2023-08-01 06:31:13.000000 pyfiscal-2.1/setup.py
```

