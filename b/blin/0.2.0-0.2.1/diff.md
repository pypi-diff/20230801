# Comparing `tmp/blin-0.2.0.tar.gz` & `tmp/blin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blin-0.2.0.tar", last modified: Wed Jul  5 22:48:57 2023, max compression
+gzip compressed data, was "blin-0.2.1.tar", last modified: Mon Jul 31 21:58:47 2023, max compression
```

## Comparing `blin-0.2.0.tar` & `blin-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 22:48:57.075543 blin-0.2.0/
--rw-rw-rw-   0        0        0     6955 2023-07-05 22:48:57.074542 blin-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6733 2023-07-05 21:14:07.000000 blin-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 22:48:57.049536 blin-0.2.0/blin/
--rw-rw-rw-   0        0        0     6252 2023-07-05 22:47:23.000000 blin-0.2.0/blin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 22:48:57.073542 blin-0.2.0/blin.egg-info/
--rw-rw-rw-   0        0        0     6955 2023-07-05 22:48:56.000000 blin-0.2.0/blin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-07-05 22:48:57.000000 blin-0.2.0/blin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 22:48:56.000000 blin-0.2.0/blin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-05 22:48:56.000000 blin-0.2.0/blin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-05 22:48:56.000000 blin-0.2.0/blin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1063 2023-05-27 00:54:38.000000 blin-0.2.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 22:48:57.075543 blin-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      475 2023-07-05 22:48:18.000000 blin-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:58:47.758286 blin-0.2.1/
+-rw-rw-rw-   0        0        0     6955 2023-07-31 21:58:47.757286 blin-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6733 2023-07-05 21:14:07.000000 blin-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 21:58:47.731280 blin-0.2.1/blin/
+-rw-rw-rw-   0        0        0     8255 2023-07-31 21:43:16.000000 blin-0.2.1/blin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 21:58:47.756285 blin-0.2.1/blin.egg-info/
+-rw-rw-rw-   0        0        0     6955 2023-07-31 21:58:47.000000 blin-0.2.1/blin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-31 21:58:47.000000 blin-0.2.1/blin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 21:58:47.000000 blin-0.2.1/blin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 21:58:47.000000 blin-0.2.1/blin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-31 21:58:47.000000 blin-0.2.1/blin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1063 2023-05-27 00:54:38.000000 blin-0.2.1/license.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 21:58:47.758286 blin-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      475 2023-07-31 21:44:49.000000 blin-0.2.1/setup.py
```

### Comparing `blin-0.2.0/PKG-INFO` & `blin-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client library for Blin API (natural language to API service)
 Author: lemeni.com
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # Blin
```

### Comparing `blin-0.2.0/README.md` & `blin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `blin-0.2.0/blin/__init__.py` & `blin-0.2.1/blin/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def version():
     """
     blin package version
 
     Returns:
     str: blin package version
     """
-    return "0.2.0"
+    return "0.2.1"
 
 
 class HTTPError(Exception):
     def __init__(self, response):
         super().__init__(f'HTTPError {response.status_code}: {response.reason}. Content: {response.text}' )
 
 class Error(Exception):
@@ -200,14 +200,72 @@
         Returns:
         str: result. Raises exception if the knowledge was not deleted. 
         """  
         response = requests.delete(f"{url}/project/{self.project_id}/knowledge/{name}", headers=self.headers)
         
         return result(response, expectedResult='Deleted', orError="Error during knowledge deletion")
 
+    def generate_testcases(self, command, data={}):
+        """
+        Generate test cases for command
+
+        Parameters:
+        command (str) : command name
+        data (dict)   : data dict with following optional fields:
+         {
+            "count"             : <number of testcases to be generated, 1 by default>,
+            "exclude_prompts"   : <prompts to be excluded from list of test cases>
+         }
+
+        Returns:
+        list: list of test cases with following fields:
+         {
+            "prompt"    : <test case prompt>,
+            "commands"  : <expected commands>, 
+            "text"      : <expected text>,
+            "notes"     : <test description> 
+         }
+        """  
+        if type(command) == str:
+            commands = [command]
+        elif type(command) == list:
+            commands = command
+        else:
+            raise Error("Command must be string or list")
+
+        call_data = data.copy()
+        call_data['commands'] = commands
+
+        response = requests.get(f"{url}/project/{self.project_id}/testcases",
+            headers=self.headers,
+            json   ={'data':call_data})
+
+        return result(response)
+
+    def update_settings(self, settings):
+        """
+        Update project settings. Note that old settings will be completely replaced by new settings
+
+        Parameters:
+        settings (dict)  : project settings dict with following required fields:
+         {
+            "openai_key"    : <openapi_key>,
+            "pinecone_key"  : <pinecone_key>,
+            "pinecone_index": <pinecone_index_name>,
+         }
+
+        Returns:
+        str: result. Raises exception in case of an update error
+        """
+        response = requests.put(f"{url}/project/{self.project_id}",
+            headers=self.headers,
+            json   ={"settings": settings})
+            
+        return result(response, expectedResult='Updated', orError="Update error")
+        
 
     def _call_learn(self, name, data, _type):
         response = requests.post(f"{url}/project/{self.project_id}/knowledge/{name}",
             headers=self.headers,
             json   ={'knowledge': {name:data},'type':_type})        
         
         return result(response)
```

### Comparing `blin-0.2.0/blin.egg-info/PKG-INFO` & `blin-0.2.1/blin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client library for Blin API (natural language to API service)
 Author: lemeni.com
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # Blin
```

### Comparing `blin-0.2.0/license.txt` & `blin-0.2.1/license.txt`

 * *Files identical despite different names*

