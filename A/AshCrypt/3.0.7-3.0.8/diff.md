# Comparing `tmp/AshCrypt-3.0.7.tar.gz` & `tmp/AshCrypt-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.0.7.tar", last modified: Mon Jul 31 18:18:28 2023, max compression
+gzip compressed data, was "dist/AshCrypt-3.0.8.tar", last modified: Tue Aug  1 14:01:18 2023, max compression
```

## Comparing `AshCrypt-3.0.7.tar` & `AshCrypt-3.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39544 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/setup.py
```

### Comparing `AshCrypt-3.0.7/AshCrypt/clicrypt.py` & `AshCrypt-3.0.8/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.7/AshCrypt/crypt.py` & `AshCrypt-3.0.8/AshCrypt/crypt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module provides classes and functions for AES-256 encryption and decryption"""
 
 
-from typing import Union
+from typing import Union, Optional
 import hmac as hmc
 import base64
 import os
 import struct
 import bcrypt
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.backends import default_backend
@@ -14,32 +14,33 @@
 
 
 class IterationsOutofRangeError(Exception):
     """Exception raised when iterations come to be out of range usually due to message tampering
     where the bytes representing the KDF iterations get touched"""
 
     def __init__(self, num: any) -> None:
-        self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num} '
+        self.display = f'Iterations must be between 50 and 100000. RECEIVED : {num}'
         super().__init__(self.display)
 
 
 class Enc:
     """Class to encrypt data of either type bytes or strings"""
 
-    def __init__(self, message: Union[str, bytes], mainkey: str) -> None:
+    def __init__(self, message: Union[str, bytes], mainkey: str,
+                 iterations: Optional[int] = 50) -> None:
         if isinstance(message, str):
             self.message = message.encode()
         elif isinstance(message, bytes):
             self.message = message
 
         self.mainkey = mainkey
         self._iv = os.urandom(16)
         self.salt = os.urandom(16)
         self.pepper = os.urandom(16)
-        self.iterations = 50
+        self.iterations = iterations
         if self.iterations < 50 or self.iterations > 100000:
             raise IterationsOutofRangeError(self.iterations)
         self.enc_key = self.derkey(self.mainkey, self.salt, self.iterations)
         self.hmac_key = self.derkey(self.mainkey, self.pepper, self.iterations)
 
     @staticmethod
     def derkey(mainkey: str, salt_pepper: bytes, iterations: int) -> bytes:
@@ -47,17 +48,24 @@
         return bcrypt.kdf(
             password=mainkey.encode('UTF-8'),
             salt=salt_pepper,
             desired_key_bytes=32,
             rounds=iterations)
 
     @staticmethod
-    def genkey() -> str:
-        """Generates a random 256-bit key as a hex string."""
-        return os.urandom(32).hex()
+    def genkey(raw_bytes: Optional[bool] = False,
+               desired_bytes: Optional[int] = 32) -> Union[str, bytes]:
+        """Generates a random 256-bit ( by default )
+        key as either raw bytes or a hex string. Set raw_bytes to True to get
+        the key in bytes. Set the number of desired_bytes to a strictly positive integer
+        to override the default value"""
+        if desired_bytes <= 0:
+            raise ValueError("desired_bytes must be strictly greater than 0")
+        key = os.urandom(desired_bytes)
+        return key if raw_bytes else key.hex()
 
     def mode(self):
         """Returns AES Cipher Block Chaining (CBC) mode with the chosen initialization vector"""
         return modes.CBC(self._iv)
 
     def cipher(self):
         """Creates AES cipher object using the encryption key and CBC mode"""
@@ -79,18 +87,18 @@
     def ciphertext(self) -> bytes:
         """Encrypts the padded message using AES and returns the ciphertext"""
         return self.cipher_encryptor().update(self.padded_message()) + \
             self.cipher_encryptor().finalize()
 
     def hmac(self) -> bytes:
         """Computes the HMAC-SHA512 of the ciphertext"""
-        _hmac = self.hmac_key
-        _hmac = hmac.HMAC(_hmac, hashes.SHA512())
-        _hmac.update(self.ciphertext())
-        return _hmac.finalize()
+        hmac_ = self.hmac_key
+        hmac_ = hmac.HMAC(hmac_, hashes.SHA512())
+        hmac_.update(self.ciphertext())
+        return hmac_.finalize()
 
     def setup_iterations(self) -> bytes:
         """Packs the number of iterations into bytes using the 'big-endian' format"""
         iters_bytes = struct.pack('!I', self.iterations)
         return iters_bytes
 
     def enc_to_bytes(self) -> bytes:
@@ -137,18 +145,18 @@
             self.rec_pepper,
             self.rec_iterations)
         if self.verify_hmac() is False:
             raise MessageTamperingError()
 
     def calculated_hmac(self) -> bytes:
         """Computes the HMAC-SHA512 of the received ciphertext"""
-        _hmac = self.hmac_k
-        _hmac = hmac.HMAC(_hmac, hashes.SHA512())
-        _hmac.update(self.rec_ciphertext)
-        return _hmac.finalize()
+        hmac_ = self.hmac_k
+        hmac_ = hmac.HMAC(hmac_, hashes.SHA512())
+        hmac_.update(self.rec_ciphertext)
+        return hmac_.finalize()
 
     def verify_hmac(self) -> bool:
         """Verifies the received HMAC-SHA512 against the calculated HMAC"""
         return hmc.compare_digest(self.calculated_hmac(), self.rec_hmac)
 
     def mode(self):
         """Returns the AES Cipher Block Chaining (CBC) mode with the received  IV"""
```

### Comparing `AshCrypt-3.0.7/AshCrypt/database.py` & `AshCrypt-3.0.8/AshCrypt/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Module to interact with an SQLite database"""
 
 from dataclasses import dataclass, field
-from typing import Union, Generator
+from typing import Union, Generator, Optional
 from datetime import datetime
 import sqlite3
 import os
 
 
 @dataclass
 class Database:
     """
-    Represents a simple SQLite database wrapper with various methods to interact with the database.
+    Represents a simple SQLite database class with various methods to interact with a given database.
     """
     dbname: str = field()
     tablename: str = field(default='Classified')
     conn: sqlite3.Connection = field(init=False, repr=False)
     c: sqlite3.Cursor = field(init=False, repr=False)
 
     def __post_init__(self):
@@ -67,15 +67,15 @@
                         result.append(
                             {f'query {i}': ['SUCCESS', self.c.fetchall()]})
 
             except sqlite3.Error as e:
                 result.append({f'query {i}': ('FAILURE', e.__str__())})
         return result
 
-    def addtable(self, optional_tablename=None) -> Union[int, tuple]:
+    def addtable(self, optional_tablename: Optional[str] = None) -> Union[int, tuple]:
         """Creates a new table in the database with the given table name.
         If the table name is not provided, it uses the default table name  : 'Classified'."""
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f"CREATE TABLE IF NOT EXISTS {self.tablename} "
@@ -95,16 +95,16 @@
                         "Key TEXT )")
                     self.tablename = optional_tablename
                 return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def insert(self, name, content, key,
-               optional_table_name=None) -> Union[int, tuple]:
+    def insert(self, name: str, content: Union[bytes, str], key: str,
+               optional_table_name: Optional[str] = None) -> Union[int, tuple]:
         """Inserts a new row into the specified table or the default table."""
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) ",
                         (name,
@@ -128,15 +128,15 @@
                 return 0, e
 
     def update(
             self,
             column_name: str,
             new_column_val: str,
             idd: int,
-            optional_table_name=None) -> Union[int, tuple]:
+            optional_table_name: Optional[str] = None) -> Union[int, tuple]:
         """Updates a specific column of a row based on the given ID in the specified table or the default table."""
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? ',
                         (new_column_val,
@@ -154,15 +154,15 @@
                         (new_column_val,
                          idd))
                     return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def content(self, optional_tablename=None) -> Union[Generator, tuple]:
+    def content(self, optional_tablename: Optional[str] = None) -> Union[Generator, tuple]:
         """Yields all rows from the specified table or the default table
          ( as a Generator object ) ."""
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(f'SELECT * FROM {self.tablename} ')
                     for row in self.c.fetchall():
@@ -178,15 +178,15 @@
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return 0, e
 
     def content_by_id(
-            self, idd: int, optional_tablename=None) -> Union[Generator, tuple]:
+            self, idd: int, optional_tablename: Optional[str] = None) -> Union[Generator, tuple]:
         """Yields a specific row from the specified table or the default table based on a given ID.
         ( Generator object )"""
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f'SELECT * FROM {self.tablename} WHERE ID = ? ', (idd,))
@@ -203,15 +203,15 @@
                         f'SELECT * FROM {optional_tablename} WHERE ID = ? ', (idd,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def show_contents(self, *optional_tablenames) -> Union[Generator, tuple]:
+    def show_contents(self, *optional_tablenames: str) -> Union[Generator, tuple]:
         """Yields all rows from specified tables or the default table.
         ( Generator object )"""
         if optional_tablenames:
             try:
                 for arg in optional_tablenames:
                     with self.conn:
                         self.c.execute(f'SELECT * FROM {arg} ')
@@ -252,15 +252,15 @@
                 for table in self.c.fetchall():
                     self.c.execute(f'DROP TABLE {table[0]}')
                 return 1
 
         except sqlite3.Error as e:
             return 0, e
 
-    def drop_table(self, *table_names) -> Union[int, tuple]:
+    def drop_table(self, *table_names: str) -> Union[int, tuple]:
         """Drops a/many specific table(s) in the Database."""
         if table_names:
             try:
                 for arg in table_names:
                     with self.conn:
                         self.c.execute(f"DROP TABLE {arg}")
                 return 1
@@ -272,15 +272,15 @@
                 with self.conn:
                     self.c.execute(f'DROP TABLE {self.tablename}')
                     return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def drop_content(self, idd, optional_table_name=None) -> Union[int, tuple]:
+    def drop_content(self, idd: int, optional_table_name: Optional[str] = None) -> Union[int, tuple]:
         """Deletes a row from the specified table or the default table based on the given ID."""
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f'DELETE FROM {self.tablename} WHERE ID = {idd}')
                 return 11
```

### Comparing `AshCrypt-3.0.7/AshCrypt/filecrypt.py` & `AshCrypt-3.0.8/AshCrypt/filecrypt.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class KeyLengthError(Exception):
     def __init__(self):
         self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
 
 
 class CryptFile:
-    def __init__(self, filename, key):
+    def __init__(self, filename : str, key : str):
         self.filename = filename
         self.not_256_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
             self.not_256_bit_key = 1  # Raise KeyError() / you can switch error handling
```

### Comparing `AshCrypt-3.0.7/AshCrypt/gui.py` & `AshCrypt-3.0.8/AshCrypt/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -803,16 +803,20 @@
             filename = filenameStringVar.get().strip()
             key = mainkey
             target = Af.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
                 filename = filename + '.crypt'
                 filenameStringVar.set(filename)
-                resultvarfile.set(
-                    '      Encrypted Successfully / added .crypt')
+                if platform.system() == 'Windows':
+                    resultvarfile.set(
+                        '    Encrypted Successfully / added .crypt')
+                else:
+                    resultvarfile.set(
+                        '      Encrypted Successfully / added .crypt')
                 if encfiletoolbuttvar.get() == 1:
                     with open(filename, 'rb') as f:
                         file_content = f.read()
                     try:
                         main_db_conn.insert(
                             filename, file_content, outputKeyref.get().strip())
                     except BaseException:
@@ -862,16 +866,20 @@
             filename = filenameStringVar.get().strip()
             key = mainkey
             target = Af.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
                 filename = os.path.splitext(filename)[0]
                 filenameStringVar.set(filename)
-                resultvarfile.set(
-                    '     Decrypted Successfully + removed .crypt')
+                if platform.system() == 'Windows':
+                    resultvarfile.set(
+                        '    Decrypted Successfully + removed .crypt')
+                else:
+                    resultvarfile.set(
+                        '     Decrypted Successfully + removed .crypt')
                 if decfiletoolbuttvar.get() == 1:
                     with open(filename, 'rb') as f:
                         file_content = f.read()
                     try:
                         main_db_conn.insert(
                             filename, file_content, outputKeyref.get().strip())
                     except BaseException:
```

### Comparing `AshCrypt-3.0.7/AshCrypt/textcrypt.py` & `AshCrypt-3.0.8/AshCrypt/textcrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,27 +42,27 @@
                 ins = cp.Enc(self.text, self.key)
                 new_content = ins.enc_to_str()
                 return 1, new_content
             except BaseException:
                 output = 'E'
                 return 0, output
         else:
-            return 0.0, 0.0
+            return 0.0, 'Empty'
 
     def decrypt(self) -> tuple:
         if self.text:
             try:
                 dec_instance = cp.Dec(message=self.text, mainkey=self.key)
                 a = dec_instance.dec_to_str()
                 output = a
                 return 1, output
             except Exception:
                 output = self.text
                 return 0, output
         else:
-            return 0.0, 0.0
+            return 0.0, 'Empty'
 
     def __str__(self):
         return f'Encrypting/Decrypting Text {self.text[:8]}.. With {self.key} Key '
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self.text[:8]},{self.key})'
```

### Comparing `AshCrypt-3.0.7/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-3.0.8/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.7/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.0.8/AshCrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.7
+Version: 3.0.8
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.7/PKG-INFO` & `AshCrypt-3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.7
+Version: 3.0.8
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.7/README.md` & `AshCrypt-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.7/setup.py` & `AshCrypt-3.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('AshCrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='3.0.7',
+    version='3.0.8',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

