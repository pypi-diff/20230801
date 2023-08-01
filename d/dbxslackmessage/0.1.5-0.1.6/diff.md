# Comparing `tmp/dbxslackmessage-0.1.5.tar.gz` & `tmp/dbxslackmessage-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxslackmessage-0.1.5.tar", last modified: Tue Aug  1 18:33:15 2023, max compression
+gzip compressed data, was "dbxslackmessage-0.1.6.tar", last modified: Tue Aug  1 18:36:33 2023, max compression
```

## Comparing `dbxslackmessage-0.1.5.tar` & `dbxslackmessage-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:33:15.718440 dbxslackmessage-0.1.5/
--rw-r--r--   0 vkhairnar   (502) staff       (20)      918 2023-08-01 18:33:15.718245 dbxslackmessage-0.1.5/PKG-INFO
-drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:33:15.716239 dbxslackmessage-0.1.5/dbxslackmessage/
--rw-r--r--   0 vkhairnar   (502) staff       (20)       96 2023-08-01 16:55:56.000000 dbxslackmessage-0.1.5/dbxslackmessage/__init__.py
--rw-r--r--   0 vkhairnar   (502) staff       (20)     1129 2023-07-26 16:28:31.000000 dbxslackmessage-0.1.5/dbxslackmessage/slackmessage.py
-drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:33:15.717829 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/
--rw-r--r--   0 vkhairnar   (502) staff       (20)      918 2023-08-01 18:33:15.000000 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/PKG-INFO
--rw-r--r--   0 vkhairnar   (502) staff       (20)      224 2023-08-01 18:33:15.000000 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/SOURCES.txt
--rw-r--r--   0 vkhairnar   (502) staff       (20)        1 2023-08-01 18:33:15.000000 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/dependency_links.txt
--rw-r--r--   0 vkhairnar   (502) staff       (20)       16 2023-08-01 18:33:15.000000 dbxslackmessage-0.1.5/dbxslackmessage.egg-info/top_level.txt
--rw-r--r--   0 vkhairnar   (502) staff       (20)       38 2023-08-01 18:33:15.718497 dbxslackmessage-0.1.5/setup.cfg
--rw-r--r--   0 vkhairnar   (502) staff       (20)     1225 2023-08-01 18:33:05.000000 dbxslackmessage-0.1.5/setup.py
+drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:36:33.409255 dbxslackmessage-0.1.6/
+-rw-r--r--   0 vkhairnar   (502) staff       (20)      927 2023-08-01 18:36:33.409073 dbxslackmessage-0.1.6/PKG-INFO
+drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:36:33.407353 dbxslackmessage-0.1.6/dbxslackmessage/
+-rw-r--r--   0 vkhairnar   (502) staff       (20)       96 2023-08-01 16:55:56.000000 dbxslackmessage-0.1.6/dbxslackmessage/__init__.py
+-rw-r--r--   0 vkhairnar   (502) staff       (20)     1129 2023-07-26 16:28:31.000000 dbxslackmessage-0.1.6/dbxslackmessage/slackmessage.py
+drwxr-xr-x   0 vkhairnar   (502) staff       (20)        0 2023-08-01 18:36:33.408717 dbxslackmessage-0.1.6/dbxslackmessage.egg-info/
+-rw-r--r--   0 vkhairnar   (502) staff       (20)      927 2023-08-01 18:36:33.000000 dbxslackmessage-0.1.6/dbxslackmessage.egg-info/PKG-INFO
+-rw-r--r--   0 vkhairnar   (502) staff       (20)      224 2023-08-01 18:36:33.000000 dbxslackmessage-0.1.6/dbxslackmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 vkhairnar   (502) staff       (20)        1 2023-08-01 18:36:33.000000 dbxslackmessage-0.1.6/dbxslackmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 vkhairnar   (502) staff       (20)       16 2023-08-01 18:36:33.000000 dbxslackmessage-0.1.6/dbxslackmessage.egg-info/top_level.txt
+-rw-r--r--   0 vkhairnar   (502) staff       (20)       38 2023-08-01 18:36:33.409311 dbxslackmessage-0.1.6/setup.cfg
+-rw-r--r--   0 vkhairnar   (502) staff       (20)     1234 2023-08-01 18:35:54.000000 dbxslackmessage-0.1.6/setup.py
```

### Comparing `dbxslackmessage-0.1.5/PKG-INFO` & `dbxslackmessage-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dbxslackmessage
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package to send slack messages via databricks notebooks
-Author: Vaishali
+Author: Vaishali Khairnar
 Author-email: vkhairnar@ripple.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -18,16 +18,16 @@
 Here is a simple usage example:
 
 ```python
 from dbxslackmessage import SlackMessage
 
 webhook_url = 'https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX'
 channel = '#your-channel'
+messages = ['Hello, World!', 'This is a test message from dbxslackmessage package']
 
 slack_message = SlackMessage(webhook_url, channel)
-messages = ['Hello, World!', 'This is a test message from dbxslackmessage package']
 slack_message.send_messages(messages)
 ```
 ### Installing  dbxslackmessage
 
 ``` python -m pip install dbxslackmessage ```
```

### Comparing `dbxslackmessage-0.1.5/dbxslackmessage/slackmessage.py` & `dbxslackmessage-0.1.6/dbxslackmessage/slackmessage.py`

 * *Files identical despite different names*

### Comparing `dbxslackmessage-0.1.5/dbxslackmessage.egg-info/PKG-INFO` & `dbxslackmessage-0.1.6/dbxslackmessage.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dbxslackmessage
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package to send slack messages via databricks notebooks
-Author: Vaishali
+Author: Vaishali Khairnar
 Author-email: vkhairnar@ripple.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
@@ -18,16 +18,16 @@
 Here is a simple usage example:
 
 ```python
 from dbxslackmessage import SlackMessage
 
 webhook_url = 'https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX'
 channel = '#your-channel'
+messages = ['Hello, World!', 'This is a test message from dbxslackmessage package']
 
 slack_message = SlackMessage(webhook_url, channel)
-messages = ['Hello, World!', 'This is a test message from dbxslackmessage package']
 slack_message.send_messages(messages)
 ```
 ### Installing  dbxslackmessage
 
 ``` python -m pip install dbxslackmessage ```
```

### Comparing `dbxslackmessage-0.1.5/setup.py` & `dbxslackmessage-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     Here is a simple usage example:
 
     ```python
     from dbxslackmessage import SlackMessage
 
     webhook_url = 'https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX'
     channel = '#your-channel'
+    messages = ['Hello, World!', 'This is a test message from dbxslackmessage package']
 
     slack_message = SlackMessage(webhook_url, channel)
-    messages = ['Hello, World!', 'This is a test message from dbxslackmessage package']
     slack_message.send_messages(messages)
     ```
     ### Installing  dbxslackmessage
 
     ``` python -m pip install dbxslackmessage ```
 
 """)
 
 setup(
     name='dbxslackmessage',
-    version='0.1.5',
-    author='Vaishali',
+    version='0.1.6',
+    author='Vaishali Khairnar',
     author_email='vkhairnar@ripple.com',
     description='Package to send slack messages via databricks notebooks',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

