# Comparing `tmp/AugmentedSocialScientist-2.0.2.tar.gz` & `tmp/AugmentedSocialScientist-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AugmentedSocialScientist-2.0.2.tar", last modified: Tue Aug  1 13:24:34 2023, max compression
+gzip compressed data, was "AugmentedSocialScientist-2.1.0.tar", last modified: Tue Aug  1 13:35:45 2023, max compression
```

## Comparing `AugmentedSocialScientist-2.0.2.tar` & `AugmentedSocialScientist-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:24:34.652019 AugmentedSocialScientist-2.0.2/
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:24:34.647616 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/
--rw-r--r--   0 rubing     (501) staff       (20)      434 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/__init__.py
--rw-r--r--   0 rubing     (501) staff       (20)     1591 2023-08-01 13:14:40.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/bert_abc.py
--rw-r--r--   0 rubing     (501) staff       (20)    20288 2023-08-01 13:15:21.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/bert_base.py
--rw-r--r--   0 rubing     (501) staff       (20)     4605 2023-08-01 13:15:51.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/models.py
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:24:34.651616 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/
--rw-r--r--   0 rubing     (501) staff       (20)     5715 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)      469 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/SOURCES.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/dependency_links.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/not-zip-safe
--rw-r--r--   0 rubing     (501) staff       (20)       63 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/requires.txt
--rw-r--r--   0 rubing     (501) staff       (20)       25 2023-08-01 13:24:34.000000 AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/top_level.txt
--rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-2.0.2/LICENSE
--rw-r--r--   0 rubing     (501) staff       (20)     5715 2023-08-01 13:24:34.652210 AugmentedSocialScientist-2.0.2/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)     5269 2023-07-28 16:21:34.000000 AugmentedSocialScientist-2.0.2/README.md
--rw-r--r--   0 rubing     (501) staff       (20)       79 2023-08-01 13:24:34.652886 AugmentedSocialScientist-2.0.2/setup.cfg
--rw-r--r--   0 rubing     (501) staff       (20)      853 2023-08-01 13:17:32.000000 AugmentedSocialScientist-2.0.2/setup.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:35:45.532927 AugmentedSocialScientist-2.1.0/
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:35:45.528414 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist/
+-rw-r--r--   0 rubing     (501) staff       (20)      434 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist/__init__.py
+-rw-r--r--   0 rubing     (501) staff       (20)     1591 2023-08-01 13:14:40.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist/bert_abc.py
+-rw-r--r--   0 rubing     (501) staff       (20)    20288 2023-08-01 13:15:21.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist/bert_base.py
+-rw-r--r--   0 rubing     (501) staff       (20)     4605 2023-08-01 13:15:51.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist/models.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-08-01 13:35:45.532532 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist.egg-info/
+-rw-r--r--   0 rubing     (501) staff       (20)     5735 2023-08-01 13:35:44.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist.egg-info/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)      469 2023-08-01 13:35:45.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist.egg-info/SOURCES.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-08-01 13:35:44.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist.egg-info/dependency_links.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist.egg-info/not-zip-safe
+-rw-r--r--   0 rubing     (501) staff       (20)       63 2023-08-01 13:35:45.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist.egg-info/requires.txt
+-rw-r--r--   0 rubing     (501) staff       (20)       25 2023-08-01 13:35:45.000000 AugmentedSocialScientist-2.1.0/AugmentedSocialScientist.egg-info/top_level.txt
+-rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-2.1.0/LICENSE
+-rw-r--r--   0 rubing     (501) staff       (20)     5735 2023-08-01 13:35:45.533135 AugmentedSocialScientist-2.1.0/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)     5269 2023-07-28 16:21:34.000000 AugmentedSocialScientist-2.1.0/README.md
+-rw-r--r--   0 rubing     (501) staff       (20)       79 2023-08-01 13:35:45.533853 AugmentedSocialScientist-2.1.0/setup.cfg
+-rw-r--r--   0 rubing     (501) staff       (20)      853 2023-08-01 13:33:07.000000 AugmentedSocialScientist-2.1.0/setup.py
```

### Comparing `AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/bert_abc.py` & `AugmentedSocialScientist-2.1.0/AugmentedSocialScientist/bert_abc.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/bert_base.py` & `AugmentedSocialScientist-2.1.0/AugmentedSocialScientist/bert_base.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.2/AugmentedSocialScientist/models.py` & `AugmentedSocialScientist-2.1.0/AugmentedSocialScientist/models.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.2/AugmentedSocialScientist.egg-info/PKG-INFO` & `AugmentedSocialScientist-2.1.0/AugmentedSocialScientist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: AugmentedSocialScientist
-Version: 2.0.2
+Version: 2.1.0
 Summary: A Package to Easily Train Bert-Like Models for Text Classification
 Home-page: https://github.com/rubingshen/AugmentedSocialScientist
-Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.2.tar.gz
+Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.1.0.tar.gz
 Author: Rubing Shen
 Author-email: shenrubing1996@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Augmented Social Scientist
 
 **New release v2**
 
@@ -157,7 +158,9 @@
 By default, the package automatically detects the presence of a GPU and uses it to accelerate computation. You can also set your own device, by providing a `torch.Device` object to the parameter `device` when instanciating `Bert`.
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(device=...)  #set your own device
 ```
+
+
```

### Comparing `AugmentedSocialScientist-2.0.2/LICENSE` & `AugmentedSocialScientist-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.2/PKG-INFO` & `AugmentedSocialScientist-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: AugmentedSocialScientist
-Version: 2.0.2
+Version: 2.1.0
 Summary: A Package to Easily Train Bert-Like Models for Text Classification
 Home-page: https://github.com/rubingshen/AugmentedSocialScientist
-Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.2.tar.gz
+Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.1.0.tar.gz
 Author: Rubing Shen
 Author-email: shenrubing1996@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Augmented Social Scientist
 
 **New release v2**
 
@@ -157,7 +158,9 @@
 By default, the package automatically detects the presence of a GPU and uses it to accelerate computation. You can also set your own device, by providing a `torch.Device` object to the parameter `device` when instanciating `Bert`.
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(device=...)  #set your own device
 ```
+
+
```

### Comparing `AugmentedSocialScientist-2.0.2/README.md` & `AugmentedSocialScientist-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.2/setup.py` & `AugmentedSocialScientist-2.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description = fh.read()
     
 setup(name='AugmentedSocialScientist',
       author='Rubing Shen',
       license='MIT',
       author_email='shenrubing1996@gmail.com',
       url='https://github.com/rubingshen/AugmentedSocialScientist',
-      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.2.tar.gz',
-      version='2.0.2',
+      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.1.0.tar.gz',
+      version='2.1.0',
       description='A Package to Easily Train Bert-Like Models for Text Classification',
       long_description=long_description,
       long_description_content_type="text/markdown",
       packages=['AugmentedSocialScientist'],
       zip_safe=False,
       install_requires=environment)
```

