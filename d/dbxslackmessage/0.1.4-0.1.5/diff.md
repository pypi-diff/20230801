# Comparing `tmp/dbxslackmessage-0.1.4.tar.gz` & `tmp/dbxslackmessage-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxslackmessage-0.1.4.tar", last modified: Tue Aug  1 18:26:50 2023, max compression
+gzip compressed data, was "dbxslackmessage-0.1.5.tar", last modified: Tue Aug  1 18:33:15 2023, max compression
```

## Comparing `dbxslackmessage-0.1.4.tar` & `dbxslackmessage-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:26:50.715925 dbxslackmessage-0.1.4/
--rw-r--r--   0 vkhairnar   (502) staff       (20)      402 2023-08-01 18:26:50.715704 dbxslackmessage-0.1.4/PKG-INFO
-drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:26:50.712888 dbxslackmessage-0.1.4/dbxslackmessage/
--rw-r--r--   0 vkhairnar   (502) staff       (20)       96 2023-08-01 16:55:56.000000 dbxslackmessage-0.1.4/dbxslackmessage/__init__.py
--rw-r--r--   0 vkhairnar   (502) staff       (20)     1129 2023-07-26 16:28:31.000000 dbxslackmessage-0.1.4/dbxslackmessage/slackmessage.py
-drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:26:50.715327 dbxslackmessage-0.1.4/dbxslackmessage.egg-info/
--rw-r--r--   0 vkhairnar   (502) staff       (20)      402 2023-08-01 18:26:50.000000 dbxslackmessage-0.1.4/dbxslackmessage.egg-info/PKG-INFO
--rw-r--r--   0 vkhairnar   (502) staff       (20)      224 2023-08-01 18:26:50.000000 dbxslackmessage-0.1.4/dbxslackmessage.egg-info/SOURCES.txt
--rw-r--r--   0 vkhairnar   (502) staff       (20)        1 2023-08-01 18:26:50.000000 dbxslackmessage-0.1.4/dbxslackmessage.egg-info/dependency_links.txt
--rw-r--r--   0 vkhairnar   (502) staff       (20)       16 2023-08-01 18:26:50.000000 dbxslackmessage-0.1.4/dbxslackmessage.egg-info/top_level.txt
--rw-r--r--   0 vkhairnar   (502) staff       (20)       38 2023-08-01 18:26:50.715996 dbxslackmessage-0.1.4/setup.cfg
--rw-r--r--   0 vkhairnar   (502) staff       (20)      551 2023-08-01 18:26:31.000000 dbxslackmessage-0.1.4/setup.py
+drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:33:15.718440 dbxslackmessage-0.1.5/
+-rw-r--r--   0 vkhairnar   (502) staff       (20)      918 2023-08-01 18:33:15.718245 dbxslackmessage-0.1.5/PKG-INFO
+drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:33:15.716239 dbxslackmessage-0.1.5/dbxslackmessage/
+-rw-r--r--   0 vkhairnar   (502) staff       (20)       96 2023-08-01 16:55:56.000000 dbxslackmessage-0.1.5/dbxslackmessage/__init__.py
+-rw-r--r--   0 vkhairnar   (502) staff       (20)     1129 2023-07-26 16:28:31.000000 dbxslackmessage-0.1.5/dbxslackmessage/slackmessage.py
+drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:33:15.717829 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/
+-rw-r--r--   0 vkhairnar   (502) staff       (20)      918 2023-08-01 18:33:15.000000 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/PKG-INFO
+-rw-r--r--   0 vkhairnar   (502) staff       (20)      224 2023-08-01 18:33:15.000000 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 vkhairnar   (502) staff       (20)        1 2023-08-01 18:33:15.000000 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 vkhairnar   (502) staff       (20)       16 2023-08-01 18:33:15.000000 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/top_level.txt
+-rw-r--r--   0 vkhairnar   (502) staff       (20)       38 2023-08-01 18:33:15.718497 dbxslackmessage-0.1.5/setup.cfg
+-rw-r--r--   0 vkhairnar   (502) staff       (20)     1225 2023-08-01 18:33:05.000000 dbxslackmessage-0.1.5/setup.py
```

### Comparing `dbxslackmessage-0.1.4/dbxslackmessage/slackmessage.py` & `dbxslackmessage-0.1.5/dbxslackmessage/slackmessage.py`

 * *Files identical despite different names*

