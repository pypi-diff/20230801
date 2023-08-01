# Comparing `tmp/censoredzz-1.0.1.tar.gz` & `tmp/censoredzz-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredzz-1.0.1.tar", last modified: Tue Aug  1 04:54:48 2023, max compression
+gzip compressed data, was "censoredzz-1.0.2.tar", last modified: Tue Aug  1 05:05:59 2023, max compression
```

## Comparing `censoredzz-1.0.1.tar` & `censoredzz-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 04:54:48.173433 censoredzz-1.0.1/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      248 2023-08-01 04:54:48.173433 censoredzz-1.0.1/PKG-INFO
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 04:54:48.133433 censoredzz-1.0.1/censoredzz/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        0 2023-07-07 02:42:13.000000 censoredzz-1.0.1/censoredzz/__init__.py
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1422 2023-08-01 04:49:17.000000 censoredzz-1.0.1/censoredzz/censor.py
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 04:54:48.173433 censoredzz-1.0.1/censoredzz/models/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000) 21320521 2023-07-14 16:02:01.000000 censoredzz-1.0.1/censoredzz/models/rf_model.pkl
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)   116314 2023-07-14 15:43:19.000000 censoredzz-1.0.1/censoredzz/models/vocabulary.pkl
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1186 2023-08-01 04:48:21.000000 censoredzz-1.0.1/censoredzz/profanity.py
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      299 2023-08-01 04:44:16.000000 censoredzz-1.0.1/censoredzz/util.py
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 04:54:48.133433 censoredzz-1.0.1/censoredzz.egg-info/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      248 2023-08-01 04:54:48.000000 censoredzz-1.0.1/censoredzz.egg-info/PKG-INFO
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      328 2023-08-01 04:54:48.000000 censoredzz-1.0.1/censoredzz.egg-info/SOURCES.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        1 2023-08-01 04:54:48.000000 censoredzz-1.0.1/censoredzz.egg-info/dependency_links.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       14 2023-08-01 04:54:48.000000 censoredzz-1.0.1/censoredzz.egg-info/requires.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       11 2023-08-01 04:54:48.000000 censoredzz-1.0.1/censoredzz.egg-info/top_level.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       38 2023-08-01 04:54:48.173433 censoredzz-1.0.1/setup.cfg
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      492 2023-08-01 04:54:42.000000 censoredzz-1.0.1/setup.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:05:59.081629 censoredzz-1.0.2/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      248 2023-08-01 05:05:59.081629 censoredzz-1.0.2/PKG-INFO
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:05:59.053629 censoredzz-1.0.2/censoredzz/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        0 2023-07-07 02:42:13.000000 censoredzz-1.0.2/censoredzz/__init__.py
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1423 2023-08-01 05:05:29.000000 censoredzz-1.0.2/censoredzz/censor.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:05:59.081629 censoredzz-1.0.2/censoredzz/models/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000) 21320521 2023-07-14 16:02:01.000000 censoredzz-1.0.2/censoredzz/models/rf_model.pkl
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)   116314 2023-07-14 15:43:19.000000 censoredzz-1.0.2/censoredzz/models/vocabulary.pkl
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1187 2023-08-01 05:05:35.000000 censoredzz-1.0.2/censoredzz/profanity.py
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      299 2023-08-01 04:44:16.000000 censoredzz-1.0.2/censoredzz/util.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:05:59.053629 censoredzz-1.0.2/censoredzz.egg-info/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      248 2023-08-01 05:05:58.000000 censoredzz-1.0.2/censoredzz.egg-info/PKG-INFO
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      328 2023-08-01 05:05:59.000000 censoredzz-1.0.2/censoredzz.egg-info/SOURCES.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        1 2023-08-01 05:05:58.000000 censoredzz-1.0.2/censoredzz.egg-info/dependency_links.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       19 2023-08-01 05:05:58.000000 censoredzz-1.0.2/censoredzz.egg-info/requires.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       11 2023-08-01 05:05:58.000000 censoredzz-1.0.2/censoredzz.egg-info/top_level.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       38 2023-08-01 05:05:59.081629 censoredzz-1.0.2/setup.cfg
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      507 2023-08-01 05:05:46.000000 censoredzz-1.0.2/setup.py
```

### Comparing `censoredzz-1.0.1/censoredzz/censor.py` & `censoredzz-1.0.2/censoredzz/censor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import os
 import pickle
 from sklearn.feature_extraction.text import CountVectorizer
-from util import remove_recurring_letters
+from .util import remove_recurring_letters
 
 def censor_text(sentence):
     # Load the machine learning model
     model_path = os.path.join(os.path.dirname(__file__), 'models', 'rf_model.pkl')
     with open(model_path, 'rb') as f:
         model = pickle.load(f)
     # Load the vocabulary used for training
```

### Comparing `censoredzz-1.0.1/censoredzz/models/rf_model.pkl` & `censoredzz-1.0.2/censoredzz/models/rf_model.pkl`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.1/censoredzz/models/vocabulary.pkl` & `censoredzz-1.0.2/censoredzz/models/vocabulary.pkl`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.1/censoredzz/profanity.py` & `censoredzz-1.0.2/censoredzz/profanity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import os
 import pickle
 from sklearn.feature_extraction.text import CountVectorizer
-from util import remove_recurring_letters
+from .util import remove_recurring_letters
 
 def has_profanity(sentence):
     # Load the machine learning model
     model_path = os.path.join(os.path.dirname(__file__), 'models', 'rf_model.pkl')
     with open(model_path, 'rb') as f:
         model = pickle.load(f)
     # Load the vocabulary used for training
```

