# Comparing `tmp/censoredzz-1.0.5.tar.gz` & `tmp/censoredzz-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredzz-1.0.5.tar", last modified: Tue Aug  1 05:32:50 2023, max compression
+gzip compressed data, was "censoredzz-1.0.6.tar", last modified: Tue Aug  1 05:37:09 2023, max compression
```

## Comparing `censoredzz-1.0.5.tar` & `censoredzz-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:32:50.222530 censoredzz-1.0.5/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      759 2023-08-01 05:32:50.222530 censoredzz-1.0.5/PKG-INFO
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      470 2023-08-01 05:31:58.000000 censoredzz-1.0.5/README.md
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:32:50.190529 censoredzz-1.0.5/censoredzz/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        0 2023-07-07 02:42:13.000000 censoredzz-1.0.5/censoredzz/__init__.py
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1423 2023-08-01 05:05:29.000000 censoredzz-1.0.5/censoredzz/censor.py
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:32:50.222530 censoredzz-1.0.5/censoredzz/models/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000) 21320521 2023-07-14 16:02:01.000000 censoredzz-1.0.5/censoredzz/models/rf_model.pkl
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)   116314 2023-07-14 15:43:19.000000 censoredzz-1.0.5/censoredzz/models/vocabulary.pkl
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1187 2023-08-01 05:05:35.000000 censoredzz-1.0.5/censoredzz/profanity.py
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      299 2023-08-01 04:44:16.000000 censoredzz-1.0.5/censoredzz/util.py
-drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:32:50.190529 censoredzz-1.0.5/censoredzz.egg-info/
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      759 2023-08-01 05:32:50.000000 censoredzz-1.0.5/censoredzz.egg-info/PKG-INFO
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      338 2023-08-01 05:32:50.000000 censoredzz-1.0.5/censoredzz.egg-info/SOURCES.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        1 2023-08-01 05:32:50.000000 censoredzz-1.0.5/censoredzz.egg-info/dependency_links.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       14 2023-08-01 05:32:50.000000 censoredzz-1.0.5/censoredzz.egg-info/requires.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       11 2023-08-01 05:32:50.000000 censoredzz-1.0.5/censoredzz.egg-info/top_level.txt
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       38 2023-08-01 05:32:50.222530 censoredzz-1.0.5/setup.cfg
--rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      668 2023-08-01 05:32:05.000000 censoredzz-1.0.5/setup.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:37:09.217531 censoredzz-1.0.6/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      759 2023-08-01 05:37:09.217531 censoredzz-1.0.6/PKG-INFO
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      470 2023-08-01 05:31:58.000000 censoredzz-1.0.6/README.md
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:37:09.181530 censoredzz-1.0.6/censoredzz/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        0 2023-07-07 02:42:13.000000 censoredzz-1.0.6/censoredzz/__init__.py
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1423 2023-08-01 05:05:29.000000 censoredzz-1.0.6/censoredzz/censor.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:37:09.217531 censoredzz-1.0.6/censoredzz/models/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000) 21320521 2023-07-14 16:02:01.000000 censoredzz-1.0.6/censoredzz/models/rf_model.pkl
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)   116314 2023-07-14 15:43:19.000000 censoredzz-1.0.6/censoredzz/models/vocabulary.pkl
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)     1187 2023-08-01 05:05:35.000000 censoredzz-1.0.6/censoredzz/profanity.py
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      299 2023-08-01 04:44:16.000000 censoredzz-1.0.6/censoredzz/util.py
+drwxrwxr-x   0 l3gion    (1000) l3gion    (1000)        0 2023-08-01 05:37:09.185530 censoredzz-1.0.6/censoredzz.egg-info/
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      759 2023-08-01 05:37:09.000000 censoredzz-1.0.6/censoredzz.egg-info/PKG-INFO
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      338 2023-08-01 05:37:09.000000 censoredzz-1.0.6/censoredzz.egg-info/SOURCES.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)        1 2023-08-01 05:37:09.000000 censoredzz-1.0.6/censoredzz.egg-info/dependency_links.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       19 2023-08-01 05:37:09.000000 censoredzz-1.0.6/censoredzz.egg-info/requires.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       11 2023-08-01 05:37:09.000000 censoredzz-1.0.6/censoredzz.egg-info/top_level.txt
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)       38 2023-08-01 05:37:09.217531 censoredzz-1.0.6/setup.cfg
+-rw-rw-r--   0 l3gion    (1000) l3gion    (1000)      673 2023-08-01 05:36:55.000000 censoredzz-1.0.6/setup.py
```

### Comparing `censoredzz-1.0.5/PKG-INFO` & `censoredzz-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredzz
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for censoring profane words in Nepali-(Roman) text
 Home-page: https://github.com/12-Twelvve/pypi_censored_text
 Author: Kuber Budhathoki
 Author-email: koobear99@gmail.com
 Description-Content-Type: text/markdown
 
 # Censoredzz
```

### Comparing `censoredzz-1.0.5/censoredzz/censor.py` & `censoredzz-1.0.6/censoredzz/censor.py`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.5/censoredzz/models/rf_model.pkl` & `censoredzz-1.0.6/censoredzz/models/rf_model.pkl`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.5/censoredzz/models/vocabulary.pkl` & `censoredzz-1.0.6/censoredzz/models/vocabulary.pkl`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.5/censoredzz/profanity.py` & `censoredzz-1.0.6/censoredzz/profanity.py`

 * *Files identical despite different names*

### Comparing `censoredzz-1.0.5/censoredzz.egg-info/PKG-INFO` & `censoredzz-1.0.6/censoredzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredzz
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for censoring profane words in Nepali-(Roman) text
 Home-page: https://github.com/12-Twelvve/pypi_censored_text
 Author: Kuber Budhathoki
 Author-email: koobear99@gmail.com
 Description-Content-Type: text/markdown
 
 # Censoredzz
```

### Comparing `censoredzz-1.0.5/setup.py` & `censoredzz-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='censoredzz',
-    version='1.0.5',
+    version='1.0.6',
     description='Python package for censoring profane words in Nepali-(Roman) text',
     author='Kuber Budhathoki',
     author_email='koobear99@gmail.com',
     url='https://github.com/12-Twelvve/pypi_censored_text',
     packages=['censoredzz'],
     package_data={
         'censoredzz': ['models/rf_model.pkl', 'models/vocabulary.pkl'],
     },
     install_requires=[
         'regex',
-        'sklearn',
+        'scikit-learn',
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

