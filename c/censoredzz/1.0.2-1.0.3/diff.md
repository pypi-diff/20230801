# Comparing `tmp/censoredzz-1.0.2.tar.gz` & `tmp/censoredzz-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredzz-1.0.2.tar", last modified: Tue Aug  1 05:05:59 2023, max compression
+gzip compressed data, was "censoredzz-1.0.3.tar", last modified: Tue Aug  1 05:11:08 2023, max compression
```

## Comparing `censoredzz-1.0.2.tar` & `censoredzz-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:05:59.081629 censoredzz-1.0.2/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      248 2023-08-01 05:05:59.081629 censoredzz-1.0.2/PKG-INFO
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:05:59.053629 censoredzz-1.0.2/censoredzz/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        0 2023-07-07 02:42:13.000000 censoredzz-1.0.2/censoredzz/__init__.py
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1423 2023-08-01 05:05:29.000000 censoredzz-1.0.2/censoredzz/censor.py
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:05:59.081629 censoredzz-1.0.2/censoredzz/models/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000) 21320521 2023-07-14 16:02:01.000000 censoredzz-1.0.2/censoredzz/models/rf_model.pkl
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)   116314 2023-07-14 15:43:19.000000 censoredzz-1.0.2/censoredzz/models/vocabulary.pkl
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1187 2023-08-01 05:05:35.000000 censoredzz-1.0.2/censoredzz/profanity.py
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      299 2023-08-01 04:44:16.000000 censoredzz-1.0.2/censoredzz/util.py
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:05:59.053629 censoredzz-1.0.2/censoredzz.egg-info/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      248 2023-08-01 05:05:58.000000 censoredzz-1.0.2/censoredzz.egg-info/PKG-INFO
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      328 2023-08-01 05:05:59.000000 censoredzz-1.0.2/censoredzz.egg-info/SOURCES.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        1 2023-08-01 05:05:58.000000 censoredzz-1.0.2/censoredzz.egg-info/dependency_links.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       19 2023-08-01 05:05:58.000000 censoredzz-1.0.2/censoredzz.egg-info/requires.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       11 2023-08-01 05:05:58.000000 censoredzz-1.0.2/censoredzz.egg-info/top_level.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       38 2023-08-01 05:05:59.081629 censoredzz-1.0.2/setup.cfg
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      507 2023-08-01 05:05:46.000000 censoredzz-1.0.2/setup.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:11:08.872063 censoredzz-1.0.3/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      248 2023-08-01 05:11:08.872063 censoredzz-1.0.3/PKG-INFO
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:11:08.844064 censoredzz-1.0.3/censoredzz/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        0 2023-07-07 02:42:13.000000 censoredzz-1.0.3/censoredzz/__init__.py
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1423 2023-08-01 05:05:29.000000 censoredzz-1.0.3/censoredzz/censor.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:11:08.872063 censoredzz-1.0.3/censoredzz/models/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000) 21320521 2023-07-14 16:02:01.000000 censoredzz-1.0.3/censoredzz/models/rf_model.pkl
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)   116314 2023-07-14 15:43:19.000000 censoredzz-1.0.3/censoredzz/models/vocabulary.pkl
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1187 2023-08-01 05:05:35.000000 censoredzz-1.0.3/censoredzz/profanity.py
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      299 2023-08-01 04:44:16.000000 censoredzz-1.0.3/censoredzz/util.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:11:08.844064 censoredzz-1.0.3/censoredzz.egg-info/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      248 2023-08-01 05:11:08.000000 censoredzz-1.0.3/censoredzz.egg-info/PKG-INFO
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      328 2023-08-01 05:11:08.000000 censoredzz-1.0.3/censoredzz.egg-info/SOURCES.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        1 2023-08-01 05:11:08.000000 censoredzz-1.0.3/censoredzz.egg-info/dependency_links.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       14 2023-08-01 05:11:08.000000 censoredzz-1.0.3/censoredzz.egg-info/requires.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       11 2023-08-01 05:11:08.000000 censoredzz-1.0.3/censoredzz.egg-info/top_level.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       38 2023-08-01 05:11:08.872063 censoredzz-1.0.3/setup.cfg
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      492 2023-08-01 05:10:39.000000 censoredzz-1.0.3/setup.py
```

### Comparing `censoredzz-1.0.2/censoredzz/censor.py` & `censoredzz-1.0.3/censoredzz/censor.py`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.2/censoredzz/models/rf_model.pkl` & `censoredzz-1.0.3/censoredzz/models/rf_model.pkl`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.2/censoredzz/models/vocabulary.pkl` & `censoredzz-1.0.3/censoredzz/models/vocabulary.pkl`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.2/censoredzz/profanity.py` & `censoredzz-1.0.3/censoredzz/profanity.py`

 * *Files identical despite different names*

