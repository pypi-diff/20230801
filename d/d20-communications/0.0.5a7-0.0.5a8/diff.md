# Comparing `tmp/d20-communications-0.0.5a7.tar.gz` & `tmp/d20-communications-0.0.5a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-4zocxlwj\d20-communications-0.0.5a7.tar", last modified: Tue Aug  1 02:37:10 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-f744ffy_\d20-communications-0.0.5a8.tar", last modified: Tue Aug  1 05:09:32 2023, max compression
```

## Comparing `d20-communications-0.0.5a7.tar` & `d20-communications-0.0.5a8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:37:10.472169 d20-communications-0.0.5a7/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a7/LICENSE
--rw-rw-rw-   0        0        0      657 2023-08-01 02:37:10.469169 d20-communications-0.0.5a7/PKG-INFO
--rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a7/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 02:37:10.473166 d20-communications-0.0.5a7/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-08-01 02:36:10.000000 d20-communications-0.0.5a7/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:37:10.296054 d20-communications-0.0.5a7/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 02:37:10.395169 d20-communications-0.0.5a7/src/d20_communications.egg-info/
--rw-rw-rw-   0        0        0      657 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 02:37:10.465169 d20-communications-0.0.5a7/src/dtwentyCommunications/
--rw-rw-rw-   0        0        0    14745 2023-08-01 02:35:48.000000 d20-communications-0.0.5a7/src/dtwentyCommunications/Communications.py
--rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a7/src/dtwentyCommunications/Exceptions.py
--rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a7/src/dtwentyCommunications/__init__.py
--rw-rw-rw-   0        0        0      157 2023-08-01 02:36:08.000000 d20-communications-0.0.5a7/src/dtwentyCommunications/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:09:32.466252 d20-communications-0.0.5a8/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a8/LICENSE
+-rw-rw-rw-   0        0        0      657 2023-08-01 05:09:32.462971 d20-communications-0.0.5a8/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a8/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 05:09:32.466252 d20-communications-0.0.5a8/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-08-01 05:08:53.000000 d20-communications-0.0.5a8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:09:32.330328 d20-communications-0.0.5a8/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 05:09:32.403452 d20-communications-0.0.5a8/src/d20_communications.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-08-01 05:09:32.000000 d20-communications-0.0.5a8/src/d20_communications.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-08-01 05:09:32.000000 d20-communications-0.0.5a8/src/d20_communications.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:09:32.000000 d20-communications-0.0.5a8/src/d20_communications.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-01 05:09:32.000000 d20-communications-0.0.5a8/src/d20_communications.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-01 05:09:32.000000 d20-communications-0.0.5a8/src/d20_communications.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 05:09:32.459968 d20-communications-0.0.5a8/src/dtwentyCommunications/
+-rw-rw-rw-   0        0        0    14745 2023-08-01 05:08:45.000000 d20-communications-0.0.5a8/src/dtwentyCommunications/Communications.py
+-rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a8/src/dtwentyCommunications/Exceptions.py
+-rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a8/src/dtwentyCommunications/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-08-01 05:08:50.000000 d20-communications-0.0.5a8/src/dtwentyCommunications/__version__.py
```

### Comparing `d20-communications-0.0.5a7/LICENSE` & `d20-communications-0.0.5a8/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-communications-0.0.5a7/PKG-INFO` & `d20-communications-0.0.5a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a7
+Version: 0.0.5a8
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a7/setup.py` & `d20-communications-0.0.5a8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-communications",
-    version="0.0.5a7",
+    version="0.0.5a8",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/python_arango_communications_module",
     project_urls={
```

### Comparing `d20-communications-0.0.5a7/src/d20_communications.egg-info/PKG-INFO` & `d20-communications-0.0.5a8/src/d20_communications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a7
+Version: 0.0.5a8
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a7/src/dtwentyCommunications/Communications.py` & `d20-communications-0.0.5a8/src/dtwentyCommunications/Communications.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,17 @@
             # print(sg)
             # print(template_id)
                 response = sg.client.mail.send.post(request_body=data)
                 self.sender = email_from_inbox
                 self.status_code = response.status_code
                 # print(response.status_code)
                 # print(response.headers)
-                self.create()
+                self.insert()
             except Exception:
-                self.create()
+                self.insert()
                 return {'res': False, 'err_code': self.status_code, 'err_desc': 'Cannot send email', 'err_params': '?error=invalid_request'}
             if self.status_code in [200,202,'200','202']:
                 return {'res': True}
             return {'res': False, 'err_code': self.status_code, 'err_desc': 'Cannot send email', 'err_params': '?error=invalid_request'}
 
 
 
@@ -280,15 +280,15 @@
             for i, response in enumerate(responses):
                 try:
                     # We got a response back, but we don't know whether it's an error yet.
                     # This call raises errors so we can handle them with normal exception
                     # flows.
                     response.validate_response()
                     sent += 1
-                    self.create()
+                    self.insert()
                 except DeviceNotRegisteredError:
                     pass
                 except PushTicketError as exc:
                     raise self.retry(exc=exc)
             return sent
 
         def send_desktop(self):
@@ -343,15 +343,15 @@
 
             payload['data'].update(self.get('additional_data', {}))
 
             try:
 
                 req = requests.post("https://onesignal.com/api/v1/notifications", headers=header, data=json.dumps(payload))
                 self.status = req.status_code
-                self.create()
+                self.insert()
             except Exception:
                 return {'res': False, 'err_code': 500, 'err_desc': 'Cannot send', 'err_params': '?error=invalid_request'}
             if req.status_code == "200" or req.status_code == 200:
                 return {'res': True}
             return {'res': False, 'err_code': 500, 'err_desc': 'Cannot send', 'err_params': '?error=invalid_request'}
 
     # class Whatsapp(BasicElement):
```

### Comparing `d20-communications-0.0.5a7/src/dtwentyCommunications/Exceptions.py` & `d20-communications-0.0.5a8/src/dtwentyCommunications/Exceptions.py`

 * *Files identical despite different names*

