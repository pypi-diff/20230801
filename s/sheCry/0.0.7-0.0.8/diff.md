# Comparing `tmp/sheCry-0.0.7.tar.gz` & `tmp/sheCry-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheCry-0.0.7.tar", last modified: Tue Aug  1 08:41:59 2023, max compression
+gzip compressed data, was "sheCry-0.0.8.tar", last modified: Tue Aug  1 08:43:02 2023, max compression
```

## Comparing `sheCry-0.0.7.tar` & `sheCry-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:41:59.642058 sheCry-0.0.7/
--rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.7/LICENSE.md
--rw-rw-rw-   0        0        0    10135 2023-08-01 08:41:59.635057 sheCry-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9488 2023-08-01 08:41:46.000000 sheCry-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 08:41:59.642058 sheCry-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-08-01 08:36:44.000000 sheCry-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:41:59.634058 sheCry-0.0.7/sheCry.egg-info/
--rw-rw-rw-   0        0        0    10135 2023-08-01 08:41:59.000000 sheCry-0.0.7/sheCry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-08-01 08:41:59.000000 sheCry-0.0.7/sheCry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:41:59.000000 sheCry-0.0.7/sheCry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:41:59.000000 sheCry-0.0.7/sheCry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:43:02.083583 sheCry-0.0.8/
+-rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0    10131 2023-08-01 08:43:02.077584 sheCry-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9484 2023-08-01 08:42:37.000000 sheCry-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:43:02.083583 sheCry-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-08-01 08:42:56.000000 sheCry-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:43:02.075585 sheCry-0.0.8/sheCry.egg-info/
+-rw-rw-rw-   0        0        0    10131 2023-08-01 08:43:01.000000 sheCry-0.0.8/sheCry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-08-01 08:43:01.000000 sheCry-0.0.8/sheCry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:43:01.000000 sheCry-0.0.8/sheCry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:43:01.000000 sheCry-0.0.8/sheCry.egg-info/top_level.txt
```

### Comparing `sheCry-0.0.7/LICENSE.md` & `sheCry-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sheCry-0.0.7/PKG-INFO` & `sheCry-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheCry
-Version: 0.0.7
+Version: 0.0.8
 Summary: SHE Cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,SHE,SHE cryptography,Symmetric Hybrid Encryption,Symmetric Hybrid Encryption cryptography,sheCry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -52,17 +52,15 @@
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-``
-pip install sheCry
-``
+    pip install sheCry
 
 ----------------------------
 **Usage / Example**
 ----------------------------
 This is an example how you can write your code so that it runs successfully.
 
     from sheCry import crypto
```

### Comparing `sheCry-0.0.7/README.md` & `sheCry-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,15 @@
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-``
-pip install sheCry
-``
+    pip install sheCry
 
 ----------------------------
 **Usage / Example**
 ----------------------------
 This is an example how you can write your code so that it runs successfully.
 
     from sheCry import crypto
```

### Comparing `sheCry-0.0.7/setup.py` & `sheCry-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "sheCry",
 
-    version = "0.0.7",
+    version = "0.0.8",
     
     author = "Tahsin Ahmed",
 
     description = "SHE Cryptography is architectured by Tahsin Ahmed.",
 
     long_description = open("README.md", encoding="utf-8").read(),
```

### Comparing `sheCry-0.0.7/sheCry.egg-info/PKG-INFO` & `sheCry-0.0.8/sheCry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheCry
-Version: 0.0.7
+Version: 0.0.8
 Summary: SHE Cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,SHE,SHE cryptography,Symmetric Hybrid Encryption,Symmetric Hybrid Encryption cryptography,sheCry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -52,17 +52,15 @@
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-``
-pip install sheCry
-``
+    pip install sheCry
 
 ----------------------------
 **Usage / Example**
 ----------------------------
 This is an example how you can write your code so that it runs successfully.
 
     from sheCry import crypto
```

