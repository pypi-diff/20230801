# Comparing `tmp/d20-communications-0.0.5a4.tar.gz` & `tmp/d20-communications-0.0.5a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-vxy8rl2h\d20-communications-0.0.5a4.tar", last modified: Sat May 27 00:05:34 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-oxg8_ycj\d20-communications-0.0.5a5.tar", last modified: Tue Aug  1 01:01:55 2023, max compression
```

## Comparing `d20-communications-0.0.5a4.tar` & `d20-communications-0.0.5a5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 00:05:34.808166 d20-communications-0.0.5a4/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a4/LICENSE
--rw-rw-rw-   0        0        0      657 2023-05-27 00:05:34.805810 d20-communications-0.0.5a4/PKG-INFO
--rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a4/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 00:05:34.809320 d20-communications-0.0.5a4/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-05-27 00:05:00.000000 d20-communications-0.0.5a4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:05:34.719226 d20-communications-0.0.5a4/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 00:05:34.776330 d20-communications-0.0.5a4/src/d20_communications.egg-info/
--rw-rw-rw-   0        0        0      657 2023-05-27 00:05:34.000000 d20-communications-0.0.5a4/src/d20_communications.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-05-27 00:05:34.000000 d20-communications-0.0.5a4/src/d20_communications.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 00:05:34.000000 d20-communications-0.0.5a4/src/d20_communications.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-05-27 00:05:34.000000 d20-communications-0.0.5a4/src/d20_communications.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-27 00:05:34.000000 d20-communications-0.0.5a4/src/d20_communications.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 00:05:34.802792 d20-communications-0.0.5a4/src/dtwentyCommunications/
--rw-rw-rw-   0        0        0    14817 2023-05-27 00:04:19.000000 d20-communications-0.0.5a4/src/dtwentyCommunications/Communications.py
--rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a4/src/dtwentyCommunications/Exceptions.py
--rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a4/src/dtwentyCommunications/__init__.py
--rw-rw-rw-   0        0        0      159 2023-02-28 23:58:15.000000 d20-communications-0.0.5a4/src/dtwentyCommunications/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:01:55.873962 d20-communications-0.0.5a5/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a5/LICENSE
+-rw-rw-rw-   0        0        0      657 2023-08-01 01:01:55.871012 d20-communications-0.0.5a5/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a5/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 01:01:55.874992 d20-communications-0.0.5a5/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-08-01 01:00:44.000000 d20-communications-0.0.5a5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:01:55.486599 d20-communications-0.0.5a5/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 01:01:55.752884 d20-communications-0.0.5a5/src/d20_communications.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 01:01:55.864963 d20-communications-0.0.5a5/src/dtwentyCommunications/
+-rw-rw-rw-   0        0        0    14817 2023-08-01 00:59:54.000000 d20-communications-0.0.5a5/src/dtwentyCommunications/Communications.py
+-rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a5/src/dtwentyCommunications/Exceptions.py
+-rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a5/src/dtwentyCommunications/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-08-01 01:00:47.000000 d20-communications-0.0.5a5/src/dtwentyCommunications/__version__.py
```

### Comparing `d20-communications-0.0.5a4/LICENSE` & `d20-communications-0.0.5a5/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-communications-0.0.5a4/PKG-INFO` & `d20-communications-0.0.5a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a4
+Version: 0.0.5a5
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a4/setup.py` & `d20-communications-0.0.5a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-communications",
-    version="0.0.5a4",
+    version="0.0.5a5",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/python_arango_communications_module",
     project_urls={
```

### Comparing `d20-communications-0.0.5a4/src/d20_communications.egg-info/PKG-INFO` & `d20-communications-0.0.5a5/src/d20_communications.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a4
+Version: 0.0.5a5
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a4/src/dtwentyCommunications/Communications.py` & `d20-communications-0.0.5a5/src/dtwentyCommunications/Communications.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         factory = GraphClassFactory.ClassFactory(graphname, db_name, collections = collections, edgeDefinitions=edgeDefinitions, conf=conf)
 
         print(factory, " - OK")
 
  
     class Email(BasicElement):
         def __init__(self, data=None):
-            self.collection = 'Messages'
             super().__init__(db_name = comm_dbname(), data=data)
+            self.collection = 'Messages'
 
         def make(self):
             self.attributes = ['sender', 'receiver', 'type', 'params', 'channel', 'status_code']
             for key in self.attributes:
                 setattr(self, key, None)
             self.channel = 'email'
 
@@ -180,16 +180,16 @@
                 return {'res': True}
             return {'res': False, 'err_code': self.status_code, 'err_desc': 'Cannot send email', 'err_params': '?error=invalid_request'}
 
 
 
     class PushNotification(BasicElement):
         def __init__(self, data=None):
-            self.collection = 'Messages'
             super().__init__(db_name = comm_dbname(), data=data)
+            self.collection = 'Messages'
 
         type_buttons = {
             "intake" : [
                     {
                         "id": "intake-confirm-button",
                         "text": "Registrar toma",
                         "icon": "https://icons.getbootstrap.com/icons/check2-circle.svg",
```

### Comparing `d20-communications-0.0.5a4/src/dtwentyCommunications/Exceptions.py` & `d20-communications-0.0.5a5/src/dtwentyCommunications/Exceptions.py`

 * *Files identical despite different names*

