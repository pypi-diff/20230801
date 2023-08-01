# Comparing `tmp/sheCry-0.0.5.tar.gz` & `tmp/sheCry-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheCry-0.0.5.tar", last modified: Tue Aug  1 08:28:45 2023, max compression
+gzip compressed data, was "sheCry-0.0.6.tar", last modified: Tue Aug  1 08:34:30 2023, max compression
```

## Comparing `sheCry-0.0.5.tar` & `sheCry-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:28:45.382835 sheCry-0.0.5/
--rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.5/LICENSE.md
--rw-rw-rw-   0        0        0     9505 2023-08-01 08:28:45.375834 sheCry-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     8858 2023-08-01 08:28:27.000000 sheCry-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 08:28:45.382835 sheCry-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-08-01 08:28:40.000000 sheCry-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:28:45.373833 sheCry-0.0.5/sheCry.egg-info/
--rw-rw-rw-   0        0        0     9505 2023-08-01 08:28:45.000000 sheCry-0.0.5/sheCry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-08-01 08:28:45.000000 sheCry-0.0.5/sheCry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:28:45.000000 sheCry-0.0.5/sheCry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:28:45.000000 sheCry-0.0.5/sheCry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:34:30.098606 sheCry-0.0.6/
+-rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0    10131 2023-08-01 08:34:30.092576 sheCry-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9484 2023-08-01 08:34:13.000000 sheCry-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:34:30.099574 sheCry-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-08-01 08:32:30.000000 sheCry-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:34:30.090577 sheCry-0.0.6/sheCry.egg-info/
+-rw-rw-rw-   0        0        0    10131 2023-08-01 08:34:29.000000 sheCry-0.0.6/sheCry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-08-01 08:34:29.000000 sheCry-0.0.6/sheCry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:34:29.000000 sheCry-0.0.6/sheCry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:34:29.000000 sheCry-0.0.6/sheCry.egg-info/top_level.txt
```

### Comparing `sheCry-0.0.5/LICENSE.md` & `sheCry-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sheCry-0.0.5/PKG-INFO` & `sheCry-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheCry
-Version: 0.0.5
+Version: 0.0.6
 Summary: SHE Cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,SHE,SHE cryptography,Symmetric Hybrid Encryption,Symmetric Hybrid Encryption cryptography,sheCry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -52,17 +52,41 @@
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-```bash
-pip install sheCry
-```
+    pip install sheCry
+
+----------------------------
+**Usage / Example**
+----------------------------
+This is an example how you can write your code so that it runs successfully.
+
+    from sheCry import crypto
+    
+    sharedKey = int(input("Key length for shared key value: "))
+    privatedKey = int(input("Key length for private key: "))
+        
+    message = input("Enter message: ")
+    
+    she = crypto()
+    
+    she.key(sharedKey, privatedKey)
+    
+    ciphertext = she.encrypt(message)
+    
+    print("Ciphertext:", ciphertext)
+    
+    plaintext = she.decrypt()
+    
+    print("Plaintext:", plaintext)
+    
+    she.show()
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputs the length of private keys and generated shared keys.
 * A user inputs message.
 * Generates prime number according to Fermat Prime Number Theorem.
```

### Comparing `sheCry-0.0.5/README.md` & `sheCry-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,41 @@
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-```bash
-pip install sheCry
-```
+    pip install sheCry
+
+----------------------------
+**Usage / Example**
+----------------------------
+This is an example how you can write your code so that it runs successfully.
+
+    from sheCry import crypto
+    
+    sharedKey = int(input("Key length for shared key value: "))
+    privatedKey = int(input("Key length for private key: "))
+        
+    message = input("Enter message: ")
+    
+    she = crypto()
+    
+    she.key(sharedKey, privatedKey)
+    
+    ciphertext = she.encrypt(message)
+    
+    print("Ciphertext:", ciphertext)
+    
+    plaintext = she.decrypt()
+    
+    print("Plaintext:", plaintext)
+    
+    she.show()
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputs the length of private keys and generated shared keys.
 * A user inputs message.
 * Generates prime number according to Fermat Prime Number Theorem.
```

### Comparing `sheCry-0.0.5/setup.py` & `sheCry-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "sheCry",
 
-    version = "0.0.5",
+    version = "0.0.6",
     
     author = "Tahsin Ahmed",
 
     description = "SHE Cryptography is architectured by Tahsin Ahmed.",
 
     long_description = open("README.md", encoding="utf-8").read(),
```

### Comparing `sheCry-0.0.5/sheCry.egg-info/PKG-INFO` & `sheCry-0.0.6/sheCry.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheCry
-Version: 0.0.5
+Version: 0.0.6
 Summary: SHE Cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,SHE,SHE cryptography,Symmetric Hybrid Encryption,Symmetric Hybrid Encryption cryptography,sheCry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -52,17 +52,41 @@
 * **Banking**: Many online banking and payment applications require the verification of personally identifiable information before proceeding with their transactions. It helps in predicting the correct information to prevent fraudulent activities and cybercrime. This is where SHE can easily authenticate users in the money transaction system, such as credit or debit card transactions or online banking sessions.
 
 ----------------------------
 **Installation**
 ----------------------------
 To install this project in your local server -
 
-```bash
-pip install sheCry
-```
+    pip install sheCry
+
+----------------------------
+**Usage / Example**
+----------------------------
+This is an example how you can write your code so that it runs successfully.
+
+    from sheCry import crypto
+    
+    sharedKey = int(input("Key length for shared key value: "))
+    privatedKey = int(input("Key length for private key: "))
+        
+    message = input("Enter message: ")
+    
+    she = crypto()
+    
+    she.key(sharedKey, privatedKey)
+    
+    ciphertext = she.encrypt(message)
+    
+    print("Ciphertext:", ciphertext)
+    
+    plaintext = she.decrypt()
+    
+    print("Plaintext:", plaintext)
+    
+    she.show()
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputs the length of private keys and generated shared keys.
 * A user inputs message.
 * Generates prime number according to Fermat Prime Number Theorem.
```

