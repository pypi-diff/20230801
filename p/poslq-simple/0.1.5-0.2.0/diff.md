# Comparing `tmp/poslq_simple-0.1.5.tar.gz` & `tmp/poslq_simple-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poslq_simple-0.1.5.tar", last modified: Sun Jul 16 23:39:29 2023, max compression
+gzip compressed data, was "poslq_simple-0.2.0.tar", last modified: Tue Aug  1 19:17:11 2023, max compression
```

## Comparing `poslq_simple-0.1.5.tar` & `poslq_simple-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/
--rw-rw-rw-   0        0        0     1091 2023-07-12 18:29:23.000000 poslq_simple-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     3394 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2870 2023-07-16 19:45:03.000000 poslq_simple-0.1.5/README.md
--rw-rw-rw-   0        0        0      611 2023-07-16 23:37:47.000000 poslq_simple-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 23:39:29.651425 poslq_simple-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/src/poslq_simple.egg-info/
--rw-rw-rw-   0        0        0     3394 2023-07-16 23:39:29.000000 poslq_simple-0.1.5/src/poslq_simple.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-16 23:39:29.000000 poslq_simple-0.1.5/src/poslq_simple.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 23:39:29.000000 poslq_simple-0.1.5/src/poslq_simple.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 23:39:29.000000 poslq_simple-0.1.5/src/poslq_simple.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 23:39:29.682673 poslq_simple-0.1.5/src/posql_simple/
--rw-rw-rw-   0        0        0        0 2023-07-12 18:18:07.000000 poslq_simple-0.1.5/src/posql_simple/__init__.py
--rw-rw-rw-   0        0        0     5371 2023-07-16 22:52:41.000000 poslq_simple-0.1.5/src/posql_simple/w_out_sql.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:11.090421 poslq_simple-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 16:11:42.000000 poslq_simple-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3436 2023-08-01 19:17:11.090421 poslq_simple-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2912 2023-08-01 19:12:02.000000 poslq_simple-0.2.0/README.md
+-rw-rw-rw-   0        0        0      611 2023-08-01 19:13:26.000000 poslq_simple-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 19:17:11.090421 poslq_simple-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:11.061864 poslq_simple-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:11.086370 poslq_simple-0.2.0/src/poslq_simple.egg-info/
+-rw-rw-rw-   0        0        0     3436 2023-08-01 19:17:11.000000 poslq_simple-0.2.0/src/poslq_simple.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-08-01 19:17:11.000000 poslq_simple-0.2.0/src/poslq_simple.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 19:17:11.000000 poslq_simple-0.2.0/src/poslq_simple.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 19:17:11.000000 poslq_simple-0.2.0/src/poslq_simple.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 19:17:11.090421 poslq_simple-0.2.0/src/posql_simple/
+-rw-rw-rw-   0        0        0        0 2023-08-01 16:11:42.000000 poslq_simple-0.2.0/src/posql_simple/__init__.py
+-rw-rw-rw-   0        0        0     5738 2023-08-01 19:10:49.000000 poslq_simple-0.2.0/src/posql_simple/w_out_sql.py
```

### Comparing `poslq_simple-0.1.5/LICENSE` & `poslq_simple-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poslq_simple-0.1.5/PKG-INFO` & `poslq_simple-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poslq_simple
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,15 @@
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
 if the transaction is OK, and false if it's not ok ).
 Each object is **padded** with the "_id" entry ( uuid generated string ).
-You can add your own custom "_id" entry.
+You can add your own custom "_id" entry ( or _id is a fully generated new uuid4 ).
 
 ``delete_by_id`` method takes one positional param which is the id ( making a linear search ). Like the ``add_record`` method, it returns a boolean.
 
 ``find_by_id`` same as ``delete_by_id`` ; returning **deep copy** of the dict ( avoid mutability ) or else None.
 
 ``update_obj`` : takes two positional args : new_obj ( the obj to persist, must contain an "_id" entry , or else throwing an error ),
 returning a bool.
```

### Comparing `poslq_simple-0.1.5/README.md` & `poslq_simple-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
 if the transaction is OK, and false if it's not ok ).
 Each object is **padded** with the "_id" entry ( uuid generated string ).
-You can add your own custom "_id" entry.
+You can add your own custom "_id" entry ( or _id is a fully generated new uuid4 ).
 
 ``delete_by_id`` method takes one positional param which is the id ( making a linear search ). Like the ``add_record`` method, it returns a boolean.
 
 ``find_by_id`` same as ``delete_by_id`` ; returning **deep copy** of the dict ( avoid mutability ) or else None.
 
 ``update_obj`` : takes two positional args : new_obj ( the obj to persist, must contain an "_id" entry , or else throwing an error ),
 returning a bool.
```

### Comparing `poslq_simple-0.1.5/pyproject.toml` & `poslq_simple-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "poslq_simple"
-version = "0.1.5"
+version = "0.2.0"
 authors = [
   { name="enyos", email="lebedevhh@outlook.fr" },
 ]
 description = "A simple nosql json storage for small projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `poslq_simple-0.1.5/src/poslq_simple.egg-info/PKG-INFO` & `poslq_simple-0.2.0/src/poslq_simple.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poslq-simple
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple nosql json storage for small projects.
 Author-email: enyos <lebedevhh@outlook.fr>
 Project-URL: Homepage, https://github.com/enyoos/nosql
 Project-URL: Bug Tracker, https://github.com/enyoos/nosql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,15 @@
 __init__ method requires a name ( collect_name ),
 and a list of the json records ( the data persisted ) which is optinal.
 
 
 ``add_record`` method takes one positional argument which is the json obj that you want to store. Returns a boolean ( True,
 if the transaction is OK, and false if it's not ok ).
 Each object is **padded** with the "_id" entry ( uuid generated string ).
-You can add your own custom "_id" entry.
+You can add your own custom "_id" entry ( or _id is a fully generated new uuid4 ).
 
 ``delete_by_id`` method takes one positional param which is the id ( making a linear search ). Like the ``add_record`` method, it returns a boolean.
 
 ``find_by_id`` same as ``delete_by_id`` ; returning **deep copy** of the dict ( avoid mutability ) or else None.
 
 ``update_obj`` : takes two positional args : new_obj ( the obj to persist, must contain an "_id" entry , or else throwing an error ),
 returning a bool.
```

### Comparing `poslq_simple-0.1.5/src/posql_simple/w_out_sql.py` & `poslq_simple-0.2.0/src/posql_simple/w_out_sql.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,63 +3,76 @@
 import time
 import uuid
 from os.path import exists, isfile, isfile
 import os
 from pathlib import Path
 
 LOCK = threading.Lock()
+# bool
 
 # custom error class
 class InvalidFileExtensionError( Exception ):
     "File extension must be .pst"
     pass
 
 class Database:
+    WC_MSG = True
+    DEBUG = True
     # for ezz mig \ you can pass directly the data
     # need to input the password ( for decrypting the file )
-    def __init__(self, __data : dict = {}, path : str = "./default.pst"):
-        self.__data=__data # this holds all the collections
+    def __init__(self, data: dict = {}, path : str = "./default.pst"):
+        self.__data= data # this holds all the collections
         self.path = path
-        print ( "thanks for using this library..." )
+        if ( Database.WC_MSG ):
+            print ( "thanks for using this library..." )
           
+    @staticmethod
+    def offW ( ):
+        Database.WC_MSG = not ( Database.WC_MSG )
+
+    @staticmethod
+    def offD ( ):
+        Database.DEBUG = not ( Database.DEBUG )
+
     # persisting the collect obj 
     # Want to debug ( the message on the console ) -> YES ( leave the debug param to true ) : NO  -> ( make false ) 
-    def save(self, debug : bool = True ):
+    def save(self):
         # try and catch ? 
         obj_serialized = json.dumps( self.__data )
         # issue : always on save we write the whole object ( maybe implement some cache ? )
         with open(self.path , "w") as y:
             y.write(obj_serialized)
             length_byte_written = len( obj_serialized ) * 8
             log_message = "data saved on file {fname} [written : {data_length} bytes ]".format(fname=self.path, data_length=length_byte_written)
-            if (debug):
+            if (Database.DEBUG):
                 print (log_message )
             y.close()
 
     # throws an exception
     @staticmethod
     def load(path : str) :
         # we need to check if the file is encrypted ( if yes, then decrypt )
         if (exists( path ) ):
             if path[-4:] == ".pst":
                 with open ( path, "r") as file : 
                     data = file.readlines()
-                    data = json.loads( data )
-                    return Database(__data = data, path = path )
+                    data = ''.join( data )
+                    data = json.loads( str ( data ) )
+                    return Database(data= data, path = path )
             else :
                 raise InvalidFileExtensionError
         else:
             raise FileNotFoundError("file {fname} doesn't exist".format( fname = path))
 
     def __repr__( self ):
         return "path : {path_name}, collections : {coll}".format( path_name = self.path, coll = self.__data )
 
     def bind_new_collection(self, collection ):
         self.__data[collection.collect_name] = collection.get_all_slot()
-        self.save(debug = False)
+        self.save()
 
     def get_collection(self, coll_name : str ):
         if ( col_name in list(self.__data.keys())):
             return Collection( coll_name, self.__data[coll_name])
         else :
             print ( "[INFO] this is collection doesn't exist")
             print ( "[INFO] created new collection into {db_name}, with name {coll_name}".format(db_name = self.path, coll_name = coll_name))
@@ -73,74 +86,78 @@
 class Collection:
     def __init__(self, collect_name : str , __container_documents : list = []): # by default is list ( not None )
         self.collect_name=collect_name
         self.__container_documents = __container_documents# empty list to stores one all the documents
     
     def add_record(self, record : dict ) -> bool :
         # we need to check / if it has the _id prop
-        lock.acquire()
+        LOCK.acquire()
         try : 
             add_thing = record.copy()
             if not ("_id" in list(add_thing.keys())):
-                add_thing['_id'] = Cypher.generate_random_id()            
+                add_thing['_id'] = self.generate_random_id()            
             self.__container_documents.append(add_thing)
-            lock.release() 
+            LOCK.release() 
             return True 
         except:
-            lock.release() 
+            LOCK.release() 
             return False 
             
     def __repr__(self):
         return str(self.__container_documents)
 
     def delete_by_id (self, id : int ) -> bool :
-        lock.acquire()
+        LOCK.acquire()
         for slot in self.__container_documents :
             if ( slot["_id"] == id ):
                 self.__container_documents.remove( slot )
-                lock.release() 
+                LOCK.release() 
                 return True 
 
-        lock.release() 
+        LOCK.release() 
         return False
 
     # returns a copy object
     # can return a null value
     def find_by_id (self, id : int ) -> dict:
         for  slot in self.__container_documents :
             if ( slot["_id"] == id ):
                 return slot.copy()
         return None  
 
     def update_obj(self, new_obj : dict) -> bool :
-        lock.acquire()
+        LOCK.acquire()
         counter = 0
         cpy_new_obj = new_obj.copy() # immutability
         target_id = cpy_new_obj["_id"]
         found = False
         for  slot in self.__container_documents :
             if ( slot["_id"] == target_id ):
                 found = True
                 break 
 
             counter += 1 
 
         if found : 
             self.__container_documents[counter] = cpy_new_obj
-            lock.release()
+            LOCK.release()
             return True 
 
-        lock.release()
+        LOCK.release()
         return False 
 
     # the user will provide the search function
     # this function can return a null value
     # returns a cpy of the func
     def search_by(self, slot_name : str , slot_value):
         for  slot in self.__container_documents :
             if ( slot[slot_name] == slot_value ):
                 return slot.copy() 
         return None
 
+    def generate_random_id( self, ) -> str:
+        return str ( uuid.uuid4() )
+
     # getter
     def get_all_slot(self):
-        return self.__container_documents
+        return self.__container_documents
+
```

