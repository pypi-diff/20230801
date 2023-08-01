# Comparing `tmp/d20-communications-0.0.5a6.tar.gz` & `tmp/d20-communications-0.0.5a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-84_6tasi\d20-communications-0.0.5a6.tar", last modified: Tue Aug  1 02:23:34 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\python_arango_communications_module\dist\.tmp-4zocxlwj\d20-communications-0.0.5a7.tar", last modified: Tue Aug  1 02:37:10 2023, max compression
```

## Comparing `d20-communications-0.0.5a6.tar` & `d20-communications-0.0.5a7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:23:34.977215 d20-communications-0.0.5a6/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a6/LICENSE
--rw-rw-rw-   0        0        0      657 2023-08-01 02:23:34.974224 d20-communications-0.0.5a6/PKG-INFO
--rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a6/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 02:23:34.978226 d20-communications-0.0.5a6/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-08-01 02:22:21.000000 d20-communications-0.0.5a6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:23:34.618230 d20-communications-0.0.5a6/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 02:23:34.857221 d20-communications-0.0.5a6/src/d20_communications.egg-info/
--rw-rw-rw-   0        0        0      657 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-08-01 02:23:34.000000 d20-communications-0.0.5a6/src/d20_communications.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 02:23:34.968237 d20-communications-0.0.5a6/src/dtwentyCommunications/
--rw-rw-rw-   0        0        0    14801 2023-08-01 02:22:04.000000 d20-communications-0.0.5a6/src/dtwentyCommunications/Communications.py
--rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a6/src/dtwentyCommunications/Exceptions.py
--rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a6/src/dtwentyCommunications/__init__.py
--rw-rw-rw-   0        0        0      157 2023-08-01 02:22:16.000000 d20-communications-0.0.5a6/src/dtwentyCommunications/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:37:10.472169 d20-communications-0.0.5a7/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-communications-0.0.5a7/LICENSE
+-rw-rw-rw-   0        0        0      657 2023-08-01 02:37:10.469169 d20-communications-0.0.5a7/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2021-09-24 00:12:42.000000 d20-communications-0.0.5a7/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-communications-0.0.5a7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 02:37:10.473166 d20-communications-0.0.5a7/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-08-01 02:36:10.000000 d20-communications-0.0.5a7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:37:10.296054 d20-communications-0.0.5a7/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 02:37:10.395169 d20-communications-0.0.5a7/src/d20_communications.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-01 02:37:10.000000 d20-communications-0.0.5a7/src/d20_communications.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 02:37:10.465169 d20-communications-0.0.5a7/src/dtwentyCommunications/
+-rw-rw-rw-   0        0        0    14745 2023-08-01 02:35:48.000000 d20-communications-0.0.5a7/src/dtwentyCommunications/Communications.py
+-rw-rw-rw-   0        0        0     1677 2021-09-24 00:11:26.000000 d20-communications-0.0.5a7/src/dtwentyCommunications/Exceptions.py
+-rw-rw-rw-   0        0        0       29 2021-09-24 00:32:35.000000 d20-communications-0.0.5a7/src/dtwentyCommunications/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-08-01 02:36:08.000000 d20-communications-0.0.5a7/src/dtwentyCommunications/__version__.py
```

### Comparing `d20-communications-0.0.5a6/LICENSE` & `d20-communications-0.0.5a7/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-communications-0.0.5a6/PKG-INFO` & `d20-communications-0.0.5a7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a6
+Version: 0.0.5a7
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a6/setup.py` & `d20-communications-0.0.5a7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-communications",
-    version="0.0.5a6",
+    version="0.0.5a7",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A small ORM for multimodel DBs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/python_arango_communications_module",
     project_urls={
```

### Comparing `d20-communications-0.0.5a6/src/d20_communications.egg-info/PKG-INFO` & `d20-communications-0.0.5a7/src/d20_communications.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-communications
-Version: 0.0.5a6
+Version: 0.0.5a7
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/python_arango_communications_module
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/python_arango_communications_module/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-communications-0.0.5a6/src/dtwentyCommunications/Communications.py` & `d20-communications-0.0.5a7/src/dtwentyCommunications/Communications.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,14 @@
                 response = sg.client.mail.send.post(request_body=data)
                 self.sender = email_from_inbox
                 self.status_code = response.status_code
                 # print(response.status_code)
                 # print(response.headers)
                 self.create()
             except Exception:
-                self.status_code = response.status_code
                 self.create()
                 return {'res': False, 'err_code': self.status_code, 'err_desc': 'Cannot send email', 'err_params': '?error=invalid_request'}
             if self.status_code in [200,202,'200','202']:
                 return {'res': True}
             return {'res': False, 'err_code': self.status_code, 'err_desc': 'Cannot send email', 'err_params': '?error=invalid_request'}
```

### Comparing `d20-communications-0.0.5a6/src/dtwentyCommunications/Exceptions.py` & `d20-communications-0.0.5a7/src/dtwentyCommunications/Exceptions.py`

 * *Files identical despite different names*

