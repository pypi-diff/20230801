# Comparing `tmp/pypomes_crypto-0.1.2.tar.gz` & `tmp/pypomes_crypto-0.1.3.tar.gz`

## Comparing `pypomes_crypto-0.1.2.tar` & `pypomes_crypto-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.2/src/pypomes_crypto/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.2/src/pypomes_crypto/crypto_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.2/README.md
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/src/pypomes_crypto/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/src/pypomes_crypto/crypto_pkcs7.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/src/pypomes_crypto/crypto_pomes.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/README.md
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 pypomes_crypto-0.1.3/PKG-INFO
```

### Comparing `pypomes_crypto-0.1.2/src/pypomes_crypto/crypto_pomes.py` & `pypomes_crypto-0.1.3/src/pypomes_crypto/crypto_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import hashlib
 import os
 from typing import Final
-from pypomes_core.env_pomes import APP_PREFIX, env_get_str
+from pypomes_core import APP_PREFIX, env_get_str
 
 CRYPTO_HASH_ALGORITHM: Final[str] = env_get_str(f"{APP_PREFIX}_DEFAULT_HASH_ALGORITHM", "sha256")
 
 
 def crypto_hash(msg: str | bytes, alg: str = CRYPTO_HASH_ALGORITHM) -> bytes:
     """
     Compute the hash of *msg*, using the algorithm specified in *alg*.
-    Return *None* if computing the hash not possible.
 
+    Return *None* if computing the hash not possible.
     Supported algorithms: md5, blake2b, blake2s, sha1, sha224, sha256, sha384 sha512,
     sha3_224, sha3_256, sha3_384, sha3_512, shake_128, shake_256.
 
     :param msg: The message to calculate the hash for, or a path to a file.
     :param alg: The algorithm to use, or a default value (either 'sha256', or an environment-defined value).
     :return: The hash value obtained, or None if the hash could not be computed.
     """
-
     hasher = hashlib.new(alg.lower())
 
     # what is the type of the argument ?
     if isinstance(msg, bytes):
         # argument is type 'bytes'
         hasher.update(msg)
```

### Comparing `pypomes_crypto-0.1.2/LICENSE` & `pypomes_crypto-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_crypto-0.1.2/pyproject.toml` & `pypomes_crypto-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_crypto"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (cryptography modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "asn1crypto>=1.5.1",
-    "cryptography>=41.0.1",
-    "pip>=23.1.2",
-    "pypomes_core>=0.1.2",
+    "cryptography>=41.0.2",
+    "pip>=23.3.1",
+    "pypomes_core>=0.2.1",
     "setuptools>=68.0.0",
-    "wheel>=0.40.0"
+    "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Crypto"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-Crypto/issues"
```

### Comparing `pypomes_crypto-0.1.2/PKG-INFO` & `pypomes_crypto-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pypomes_crypto
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of Python pomes, pennyeach (cryptography modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Crypto
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Crypto/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: asn1crypto>=1.5.1
-Requires-Dist: cryptography>=41.0.1
-Requires-Dist: pip>=23.1.2
-Requires-Dist: pypomes-core>=0.1.2
+Requires-Dist: cryptography>=41.0.2
+Requires-Dist: pip>=23.3.1
+Requires-Dist: pypomes-core>=0.2.1
 Requires-Dist: setuptools>=68.0.0
-Requires-Dist: wheel>=0.40.0
+Requires-Dist: wheel>=0.41.0
```

