# Comparing `tmp/BIDSit-0.0.6.tar.gz` & `tmp/BIDSit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BIDSit-0.0.6.tar", last modified: Mon Jul 31 22:21:16 2023, max compression
+gzip compressed data, was "BIDSit-0.0.7.tar", last modified: Mon Jul 31 22:48:47 2023, max compression
```

## Comparing `BIDSit-0.0.6.tar` & `BIDSit-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:21:16.411529 BIDSit-0.0.6/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:21:16.411140 BIDSit-0.0.6/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.6/README.rst
--rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-07-31 22:21:16.411671 BIDSit-0.0.6/setup.cfg
--rw-r--r--   0 labmanager   (501) staff       (20)     2068 2023-07-31 20:54:57.000000 BIDSit-0.0.6/setup.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:21:16.405954 BIDSit-0.0.6/src/
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:21:16.409013 BIDSit-0.0.6/src/BIDSit/
--rw-r--r--   0 labmanager   (501) staff       (20)     5330 2023-06-28 22:32:23.000000 BIDSit-0.0.6/src/BIDSit/Test_script.py
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.6/src/BIDSit/__init__.py
--rw-r--r--   0 labmanager   (501) staff       (20)    24979 2023-04-26 21:48:18.000000 BIDSit-0.0.6/src/BIDSit/dicom_to_bids2.py
--rw-r--r--   0 labmanager   (501) staff       (20)    68398 2023-07-31 21:09:49.000000 BIDSit-0.0.6/src/BIDSit/go.py
--rw-r--r--   0 labmanager   (501) staff       (20)       83 2023-07-31 20:13:14.000000 BIDSit-0.0.6/src/BIDSit/main.py
--rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-07-31 20:27:12.000000 BIDSit-0.0.6/src/BIDSit/version.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:21:16.410724 BIDSit-0.0.6/src/BIDSit.egg-info/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      324 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/SOURCES.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/dependency_links.txt
--rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/requires.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/top_level.txt
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:48:47.981430 BIDSit-0.0.7/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:48:47.981066 BIDSit-0.0.7/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.7/README.rst
+-rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-07-31 22:48:47.981568 BIDSit-0.0.7/setup.cfg
+-rw-r--r--   0 labmanager   (501) staff       (20)     2068 2023-07-31 20:54:57.000000 BIDSit-0.0.7/setup.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:48:47.973009 BIDSit-0.0.7/src/
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:48:47.978850 BIDSit-0.0.7/src/BIDSit/
+-rw-r--r--   0 labmanager   (501) staff       (20)     5330 2023-06-28 22:32:23.000000 BIDSit-0.0.7/src/BIDSit/Test_script.py
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.7/src/BIDSit/__init__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)       83 2023-07-31 20:13:14.000000 BIDSit-0.0.7/src/BIDSit/__main__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    24979 2023-04-26 21:48:18.000000 BIDSit-0.0.7/src/BIDSit/dicom_to_bids2.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    68398 2023-07-31 21:09:49.000000 BIDSit-0.0.7/src/BIDSit/go.py
+-rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-07-31 22:47:16.000000 BIDSit-0.0.7/src/BIDSit/version.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:48:47.980654 BIDSit-0.0.7/src/BIDSit.egg-info/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:48:47.000000 BIDSit-0.0.7/src/BIDSit.egg-info/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      328 2023-07-31 22:48:47.000000 BIDSit-0.0.7/src/BIDSit.egg-info/SOURCES.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-07-31 22:48:47.000000 BIDSit-0.0.7/src/BIDSit.egg-info/dependency_links.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-07-31 22:48:47.000000 BIDSit-0.0.7/src/BIDSit.egg-info/requires.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-07-31 22:48:47.000000 BIDSit-0.0.7/src/BIDSit.egg-info/top_level.txt
```

### Comparing `BIDSit-0.0.6/PKG-INFO` & `BIDSit-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.6
+Version: 0.0.7
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `BIDSit-0.0.6/README.rst` & `BIDSit-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.6/setup.py` & `BIDSit-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.6/src/BIDSit/Test_script.py` & `BIDSit-0.0.7/src/BIDSit/Test_script.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.6/src/BIDSit/dicom_to_bids2.py` & `BIDSit-0.0.7/src/BIDSit/dicom_to_bids2.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.6/src/BIDSit/go.py` & `BIDSit-0.0.7/src/BIDSit/go.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.6/src/BIDSit/version.py` & `BIDSit-0.0.7/src/BIDSit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Script Name: version.py                                                    #
 #                                                                            #
 # Description: specifies version for BIDSit                                  #
 #                                                                            #
 # Author:      Jen Burrell (April 17th, 2023)                                #
 #============================================================================#
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
```

### Comparing `BIDSit-0.0.6/src/BIDSit.egg-info/PKG-INFO` & `BIDSit-0.0.7/src/BIDSit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.6
+Version: 0.0.7
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

