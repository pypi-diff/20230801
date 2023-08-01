# Comparing `tmp/mdast_cli_core-2023.5.1.tar.gz` & `tmp/mdast_cli_core-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdast_cli_core-2023.5.1.tar", last modified: Wed May 31 09:56:36 2023, max compression
+gzip compressed data, was "mdast_cli_core-2023.8.1.tar", last modified: Tue Aug  1 11:23:01 2023, max compression
```

## Comparing `mdast_cli_core-2023.5.1.tar` & `mdast_cli_core-2023.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:36.207982 mdast_cli_core-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 09:56:36.207982 mdast_cli_core-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:36.203982 mdast_cli_core-2023.5.1/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/mdast_cli_core/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:36.207982 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:56:36.207982 mdast_cli_core-2023.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27547 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/mdast_cli_core/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/setup.py
```

### Comparing `mdast_cli_core-2023.5.1/PKG-INFO` & `mdast_cli_core-2023.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast_cli_core
-Version: 2023.5.1
+Version: 2023.8.1
 Summary: mDast core package
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli-core
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli_core-2023.5.1/mdast_cli_core/api.py` & `mdast_cli_core-2023.8.1/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli_core-2023.5.1/mdast_cli_core/base.py` & `mdast_cli_core-2023.8.1/mdast_cli_core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,44 +313,72 @@
         }
         return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/applications/',
                              headers=headers_multipart,
                              files=multipart_form_data,
                              data={'architecture_type': architecture_type},
                              verify=False)
 
-    def create_manual_scan(self, profile_id, app_id, arch_id):
+    def create_manual_scan(self, project_id, profile_id, app_id, arch_id):
         data = {
-            'profile_id': profile_id,
             'application_id': app_id,
             'architecture_id': arch_id,
             'type': 0
         }
+        if project_id:
+            data['project_id'] = project_id
+        if profile_id:
+            data['profile_id'] = profile_id
         return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/dasts/',
                              headers=self.headers,
                              data=json.dumps(data),
                              verify=False)
 
-    def create_manual_scan_autocreate_profile(self, app_id, arch_id):
+    def create_auto_scan(self, project_id, profile_id, app_id, arch_id, test_case_id):
         data = {
             'application_id': app_id,
             'architecture_id': arch_id,
-            'type': 0
+            'test_case_id': test_case_id,
+            'type': 1
         }
+        if project_id:
+            data['project_id'] = project_id
+        if profile_id:
+            data['profile_id'] = profile_id
         return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/dasts/',
                              headers=self.headers,
                              data=json.dumps(data),
                              verify=False)
 
-    def create_auto_scan(self, profile_id, app_id, arch_id, test_case_id):
+    def create_appium_scan(self, project_id, profile_id, app_id, arch_id, appium_script_path):
         data = {
-            'profile_id': profile_id,
             'application_id': app_id,
             'architecture_id': arch_id,
-            'test_case_id': test_case_id,
-            'type': 1
+            'type': 2
+        }
+        headers = {
+            'Authorization': self.headers['Authorization']
+        }
+
+        if project_id:
+            data['project_id'] = project_id
+        if profile_id:
+            data['profile_id'] = profile_id
+        with open(appium_script_path, 'rb') as f:
+            files = {'script': f}
+            return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/dasts/',
+                                 headers=headers,
+                                 data=data,
+                                 files=files,
+                                 verify=False)
+
+    def create_manual_scan_autocreate_profile(self, app_id, arch_id):
+        data = {
+            'application_id': app_id,
+            'architecture_id': arch_id,
+            'type': 0
         }
         return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/dasts/',
                              headers=self.headers,
                              data=json.dumps(data),
                              verify=False)
 
     def start_scan(self, dast_id):
```

### Comparing `mdast_cli_core-2023.5.1/mdast_cli_core/token.py` & `mdast_cli_core-2023.8.1/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/PKG-INFO` & `mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast-cli-core
-Version: 2023.5.1
+Version: 2023.8.1
 Summary: mDast core package
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli-core
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli_core-2023.5.1/setup.py` & `mdast_cli_core-2023.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli_core",
-    version='2023.05.01',
+    version='2023.08.01',
     author="Dynamic-Mobile-Security",
     description="mDast core package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dynamic-Mobile-Security/mdast-cli-core",
     packages=find_packages(),
     include_package_data=True,
```

