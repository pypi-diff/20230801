# Comparing `tmp/AshCrypt-3.0.8.tar.gz` & `tmp/AshCrypt-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.0.8.tar", last modified: Tue Aug  1 14:01:18 2023, max compression
+gzip compressed data, was "dist/AshCrypt-3.0.9.tar", last modified: Tue Aug  1 18:36:44 2023, max compression
```

## Comparing `AshCrypt-3.0.8.tar` & `AshCrypt-3.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39544 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 14:01:17.000000 AshCrypt-3.0.8/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:01:18.000000 AshCrypt-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-01 14:01:00.000000 AshCrypt-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39544 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:36:44.000000 AshCrypt-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-01 18:36:32.000000 AshCrypt-3.0.9/setup.py
```

### Comparing `AshCrypt-3.0.8/AshCrypt/clicrypt.py` & `AshCrypt-3.0.9/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.8/AshCrypt/crypt.py` & `AshCrypt-3.0.9/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.8/AshCrypt/database.py` & `AshCrypt-3.0.9/AshCrypt/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 @dataclass
 class Database:
     """
     Represents a simple SQLite database class with various methods to interact with a given database.
     """
     dbname: str = field()
-    tablename: str = field(default='Classified')
+    tablename: Optional[str] = field(default='Classified')
     conn: sqlite3.Connection = field(init=False, repr=False)
     c: sqlite3.Cursor = field(init=False, repr=False)
 
     def __post_init__(self):
         self.conn = sqlite3.connect(self.dbname)
         self.c = self.conn.cursor()
 
@@ -67,46 +67,46 @@
                         result.append(
                             {f'query {i}': ['SUCCESS', self.c.fetchall()]})
 
             except sqlite3.Error as e:
                 result.append({f'query {i}': ('FAILURE', e.__str__())})
         return result
 
-    def addtable(self, optional_tablename: Optional[str] = None) -> Union[int, tuple]:
+    def addtable(self, tablename: Optional[str] = None) -> Union[int, tuple]:
         """Creates a new table in the database with the given table name.
         If the table name is not provided, it uses the default table name  : 'Classified'."""
-        if optional_tablename is None:
+        if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f"CREATE TABLE IF NOT EXISTS {self.tablename} "
                         "(ID INTEGER PRIMARY KEY, Name Text , Content BLOB ,Key TEXT )")
                 return 11
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f"CREATE TABLE IF NOT EXISTS {optional_tablename} "
+                        f"CREATE TABLE IF NOT EXISTS {tablename} "
                         "(ID INTEGER PRIMARY KEY,"
                         "Name TEXT ,"
                         "Content BLOB ,"
                         "Key TEXT )")
-                    self.tablename = optional_tablename
+                    self.tablename = tablename
                 return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
     def insert(self, name: str, content: Union[bytes, str], key: str,
-               optional_table_name: Optional[str] = None) -> Union[int, tuple]:
+               tablename: Optional[str] = None) -> Union[int, tuple]:
         """Inserts a new row into the specified table or the default table."""
-        if optional_table_name is None:
+        if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) ",
                         (name,
                          content,
                          key))
@@ -115,108 +115,108 @@
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f"INSERT INTO {optional_table_name} (Name, Content ,Key) VALUES (? , ? , ?) ",
+                        f"INSERT INTO {tablename} (Name, Content ,Key) VALUES (? , ? , ?) ",
                         (name,
                          content,
                          key))
                 return 1
             except sqlite3.Error as e:
                 return 0, e
 
     def update(
             self,
             column_name: str,
             new_column_val: str,
-            idd: int,
-            optional_table_name: Optional[str] = None) -> Union[int, tuple]:
+            id: int,
+            tablename: Optional[str] = None) -> Union[int, tuple]:
         """Updates a specific column of a row based on the given ID in the specified table or the default table."""
-        if optional_table_name is None:
+        if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? ',
                         (new_column_val,
-                         idd))
+                         id))
                     return 11
 
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'UPDATE {optional_table_name} SET {column_name} = ? WHERE ID = ? ',
+                        f'UPDATE {tablename} SET {column_name} = ? WHERE ID = ? ',
                         (new_column_val,
-                         idd))
+                         id))
                     return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def content(self, optional_tablename: Optional[str] = None) -> Union[Generator, tuple]:
+    def content(self, tablename: Optional[str] = None) -> Union[Generator, tuple]:
         """Yields all rows from the specified table or the default table
-         ( as a Generator object ) ."""
-        if optional_tablename is None:
+        if no arguments are passed ( as a Generator object ) ."""
+        if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(f'SELECT * FROM {self.tablename} ')
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
-                    self.c.execute(f'SELECT * FROM {optional_tablename} ')
+                    self.c.execute(f'SELECT * FROM {tablename} ')
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return 0, e
 
     def content_by_id(
-            self, idd: int, optional_tablename: Optional[str] = None) -> Union[Generator, tuple]:
+            self, id: int, tablename: Optional[str] = None) -> Union[Generator, tuple]:
         """Yields a specific row from the specified table or the default table based on a given ID.
         ( Generator object )"""
-        if optional_tablename is None:
+        if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (idd,))
+                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (id,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'SELECT * FROM {optional_tablename} WHERE ID = ? ', (idd,))
+                        f'SELECT * FROM {tablename} WHERE ID = ? ', (id,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def show_contents(self, *optional_tablenames: str) -> Union[Generator, tuple]:
+    def show_contents(self, *tablenames: str) -> Union[Generator, tuple]:
         """Yields all rows from specified tables or the default table.
         ( Generator object )"""
-        if optional_tablenames:
+        if tablenames:
             try:
-                for arg in optional_tablenames:
+                for arg in tablenames:
                     with self.conn:
                         self.c.execute(f'SELECT * FROM {arg} ')
                         for row in self.c.fetchall():
                             yield {arg: row}
 
             except sqlite3.Error as e:
                 return -1, e
@@ -252,19 +252,19 @@
                 for table in self.c.fetchall():
                     self.c.execute(f'DROP TABLE {table[0]}')
                 return 1
 
         except sqlite3.Error as e:
             return 0, e
 
-    def drop_table(self, *table_names: str) -> Union[int, tuple]:
+    def drop_table(self, *tablenames: str) -> Union[int, tuple]:
         """Drops a/many specific table(s) in the Database."""
-        if table_names:
+        if tablenames:
             try:
-                for arg in table_names:
+                for arg in tablenames:
                     with self.conn:
                         self.c.execute(f"DROP TABLE {arg}")
                 return 1
             except sqlite3.Error as e:
                 return -1, e
 
         else:
@@ -272,28 +272,28 @@
                 with self.conn:
                     self.c.execute(f'DROP TABLE {self.tablename}')
                     return 1
 
             except sqlite3.Error as e:
                 return 0, e
 
-    def drop_content(self, idd: int, optional_table_name: Optional[str] = None) -> Union[int, tuple]:
+    def drop_content(self, id: int, tablename: Optional[str] = None) -> Union[int, tuple]:
         """Deletes a row from the specified table or the default table based on the given ID."""
-        if optional_table_name is None:
+        if tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'DELETE FROM {self.tablename} WHERE ID = {idd}')
+                        f'DELETE FROM {self.tablename} WHERE ID = {id}')
                 return 11
 
             except sqlite3.Error as e:
                 return -1, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'DELETE FROM {optional_table_name} WHERE ID = {idd}')
+                        f'DELETE FROM {tablename} WHERE ID = {id}')
                 return 1
 
             except sqlite3.Error as e:
                 return 0, e
```

### Comparing `AshCrypt-3.0.8/AshCrypt/filecrypt.py` & `AshCrypt-3.0.9/AshCrypt/filecrypt.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 class KeyLengthError(Exception):
     def __init__(self):
         self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
 
 
 class CryptFile:
+    '''Class to encrypt/decrypt a given file. Pass in the filename
+                as well as a 256-bit key '''
     def __init__(self, filename : str, key : str):
         self.filename = filename
         self.not_256_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
             self.not_256_bit_key = 1  # Raise KeyError() / you can switch error handling
```

### Comparing `AshCrypt-3.0.8/AshCrypt/gui.py` & `AshCrypt-3.0.9/AshCrypt/gui.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.8/AshCrypt/textcrypt.py` & `AshCrypt-3.0.9/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.8/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-3.0.9/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.8/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.0.9/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.8
+Version: 3.0.9
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.8/PKG-INFO` & `AshCrypt-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.8
+Version: 3.0.9
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.8/README.md` & `AshCrypt-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.8/setup.py` & `AshCrypt-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('AshCrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='3.0.8',
+    version='3.0.9',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

