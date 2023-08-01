# Comparing `tmp/d20-communications-0.0.5a5.tar.gz` & `tmp/d20-communications-0.0.5a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-oxg8_ycj\d20-communications-0.0.5a5.tar", last modified: Tue Aug  1 01:01:55 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-84_6tasi\d20-communications-0.0.5a6.tar", last modified: Tue Aug  1 02:23:34 2023, max compression
```

## Comparing `d20-communications-0.0.5a5.tar` & `d20-communications-0.0.5a6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 01:01:55.873962 d20-communications-0.0.5a5/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a5/LICENSE
--rw-rw-rw-   0        0        0      657 2023-08-01 01:01:55.871012 d20-communications-0.0.5a5/PKG-INFO
--rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a5/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 01:01:55.874992 d20-communications-0.0.5a5/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-08-01 01:00:44.000000 d20-communications-0.0.5a5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:01:55.486599 d20-communications-0.0.5a5/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 01:01:55.752884 d20-communications-0.0.5a5/src/d20_communications.egg-info/
--rw-rw-rw-   0        0        0      657 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-08-01 01:01:55.000000 d20-communications-0.0.5a5/src/d20_communications.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 01:01:55.864963 d20-communications-0.0.5a5/src/dtwentyCommunications/
--rw-rw-rw-   0        0        0    14817 2023-08-01 00:59:54.000000 d20-communications-0.0.5a5/src/dtwentyCommunications/Communications.py
--rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a5/src/dtwentyCommunications/Exceptions.py
--rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a5/src/dtwentyCommunications/__init__.py
--rw-rw-rw-   0        0        0      157 2023-08-01 01:00:47.000000 d20-communications-0.0.5a5/src/dtwentyCommunications/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:23:34.977215 d20-communications-0.0.5a6/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a6/LICENSE
+-rw-rw-rw-   0        0        0      657 2023-08-01 02:23:34.974224 d20-communications-0.0.5a6/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a6/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 02:23:34.978226 d20-communications-0.0.5a6/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-08-01 02:22:21.000000 d20-communications-0.0.5a6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:23:34.618230 d20-communications-0.0.5a6/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 02:23:34.857221 d20-communications-0.0.5a6/src/d20_communications.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 02:23:34.968237 d20-communications-0.0.5a6/src/dtwentyCommunications/
+-rw-rw-rw-   0        0        0    14801 2023-08-01 02:22:04.000000 d20-communications-0.0.5a6/src/dtwentyCommunications/Communications.py
+-rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a6/src/dtwentyCommunications/Exceptions.py
+-rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a6/src/dtwentyCommunications/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-08-01 02:22:16.000000 d20-communications-0.0.5a6/src/dtwentyCommunications/__version__.py
```

### Comparing `d20-communications-0.0.5a5/LICENSE` & `d20-communications-0.0.5a6/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-communications-0.0.5a5/PKG-INFO` & `d20-communications-0.0.5a6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a5
+Version: 0.0.5a6
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a5/setup.py` & `d20-communications-0.0.5a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-communications",
-    version="0.0.5a5",
+    version="0.0.5a6",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/python_arango_communications_module",
     project_urls={
```

### Comparing `d20-communications-0.0.5a5/src/d20_communications.egg-info/PKG-INFO` & `d20-communications-0.0.5a6/src/d20_communications.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a5
+Version: 0.0.5a6
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a5/src/dtwentyCommunications/Communications.py` & `d20-communications-0.0.5a6/src/dtwentyCommunications/Communications.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 if False in [a in contact_data for a in requirement]:
                     if ignore_errors:
                         return
                     else:
                         raise MissingRequiredParametersException
             url = "https://api.sendgrid.com/v3/marketing/contacts"
 
-            lists_ids = [Metadata.Parameter().find(list_id).get('value') for list_id in lists  if Metadata.Parameter('find', {'_key' : list_id}).get('value') != None and Metadata.Parameter('find', {'_key' : list_id}).get('value') != '']
+            lists_ids = [Metadata.Parameter().load(list_id).get('value') for list_id in lists  if Metadata.Parameter().load(list_id).get('value') not in [None, '']]
 
             contacts = []
             
             for contact_data in contacts_data:
                 if '_key' in contact_data:
                     contact_data['uid'] = contact_data['_key']
                 if "gender" in contact_data and contact_data["gender"] == 'Femenino':
@@ -89,15 +89,16 @@
 
             payload = {
                 "list_ids": lists_ids,
                 "contacts": contacts
             }
 
 
-            p = Metadata.Parameter().find('sg_conf')
+            p = Metadata.Parameter()
+            p.load('sg_conf')
 
             sg = p.get('value')['api_key']     
 
             headers = {
                 'authorization': f"Bearer {sg}",
                 'content-type': "application/json"
                 }
@@ -135,25 +136,27 @@
                     }
                 ]
             }
             return data
 
 
         def send(self):
-            p = Metadata.Parameter().find(self.get('type'))
+            p = Metadata.Parameter()
+            p.load(self.get('type'))
             template_id = p.get('value')
             return self.sg_send(template_id)
 
         def send_by_id(self, template_id):
             return self.sg_send(template_id)
 
         def sg_send(self, template_id):
             if self.get('receiver', None) == None or self.get('receiver', None) == '':
                 raise MissingRequiredParametersException 
-            p = Metadata.Parameter().find('sg_conf')
+            p = Metadata.Parameter()
+            p.load('sg_conf')
 
             sg = sendgrid.SendGridAPIClient(api_key=p.get('value')['api_key'])            
             email_from_name = p.get('value')['email_from_name']
             email_from_inbox = p.get('value')['email_from_inbox']
 
             data = self.personalize()
             data['template_id'] = template_id
@@ -287,15 +290,16 @@
                     pass
                 except PushTicketError as exc:
                     raise self.retry(exc=exc)
             return sent
 
         def send_desktop(self):
 
-            p = Metadata.Parameter().find('os_conf')
+            p = Metadata.Parameter()
+            p.load('os_conf')
             api_key=p.get('value')['api_key']
             app_id=p.get('value')['app_id']
 
 
 
             header = {"Content-Type": "application/json; charset=utf-8",
                     "Authorization": f"Basic {api_key}"}
```

### Comparing `d20-communications-0.0.5a5/src/dtwentyCommunications/Exceptions.py` & `d20-communications-0.0.5a6/src/dtwentyCommunications/Exceptions.py`

 * *Files identical despite different names*

