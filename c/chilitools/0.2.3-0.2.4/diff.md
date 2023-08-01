# Comparing `tmp/chilitools-0.2.3.tar.gz` & `tmp/chilitools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chilitools-0.2.3.tar", max compression
+gzip compressed data, was "chilitools-0.2.4.tar", max compression
```

## Comparing `chilitools-0.2.3.tar` & `chilitools-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     3655 2023-06-22 22:39:37.123359 chilitools-0.2.3/chilitools/__init__.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257043 chilitools-0.2.3/chilitools/api/__init__.py
--rw-r--r--   0        0        0     7160 2023-03-20 16:14:22.242821 chilitools-0.2.3/chilitools/api/connector.py
--rw-r--r--   0        0        0    20998 2023-06-22 22:35:35.839958 chilitools-0.2.3/chilitools/api/endpoints.py
--rw-r--r--   0        0        0     3728 2023-03-21 14:29:37.670561 chilitools-0.2.3/chilitools/api/mycp.py
--rw-r--r--   0        0        0     3114 2022-09-20 16:25:32.069762 chilitools-0.2.3/chilitools/api/response.py
--rw-r--r--   0        0        0        0 2023-06-20 02:25:18.519289 chilitools-0.2.3/chilitools/grafx/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 19:59:39.899564 chilitools-0.2.3/chilitools/grafx/api/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-22 21:44:25.944416 chilitools-0.2.3/chilitools/grafx/api/environment.py
--rw-r--r--   0        0        0      513 2023-06-22 22:42:14.136612 chilitools-0.2.3/chilitools/grafx/api/platform.py
--rw-r--r--   0        0        0     2232 2023-06-20 04:20:59.710105 chilitools-0.2.3/chilitools/grafx/auth.py
--rw-r--r--   0        0        0     1999 2023-06-22 22:41:24.669863 chilitools-0.2.3/chilitools/grafx/connector.py
--rw-r--r--   0        0        0     2099 2023-06-22 21:08:30.949881 chilitools-0.2.3/chilitools/grafx/document.py
--rw-r--r--   0        0        0      662 2023-06-22 22:26:48.267393 chilitools-0.2.3/chilitools/grafx/environment.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257581 chilitools-0.2.3/chilitools/settings/__init__.py
--rw-r--r--   0        0        0      199 2022-04-15 23:48:49.570757 chilitools-0.2.3/chilitools/settings/config.py
--rw-r--r--   0        0        0    12468 2022-09-27 16:58:06.159255 chilitools-0.2.3/chilitools/utilities/ServerMigration.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257751 chilitools-0.2.3/chilitools/utilities/__init__.py
--rw-r--r--   0        0        0     2104 2022-10-28 20:09:34.951802 chilitools-0.2.3/chilitools/utilities/backoffice.py
--rw-r--r--   0        0        0      602 2022-04-15 23:48:53.626324 chilitools-0.2.3/chilitools/utilities/defaults.py
--rw-r--r--   0        0        0     2069 2023-06-13 15:46:56.759605 chilitools-0.2.3/chilitools/utilities/document.py
--rw-r--r--   0        0        0      897 2022-07-21 19:16:13.652722 chilitools-0.2.3/chilitools/utilities/errors.py
--rw-r--r--   0        0        0     6022 2022-10-28 20:05:22.841538 chilitools-0.2.3/chilitools/utilities/file.py
--rw-r--r--   0        0        0      807 2023-06-20 15:02:52.753030 chilitools-0.2.3/chilitools/utilities/logger.py
--rw-r--r--   0        0        0      509 2022-06-29 19:01:07.878458 chilitools-0.2.3/chilitools/utilities/strings.py
--rw-r--r--   0        0        0     3831 2023-03-21 15:07:48.139637 chilitools-0.2.3/chilitools/utilities/xmltools.py
--rw-r--r--   0        0        0      505 2023-06-22 22:39:25.392049 chilitools-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 chilitools-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3655 2023-08-01 18:55:06.483874 chilitools-0.2.4/chilitools/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257043 chilitools-0.2.4/chilitools/api/__init__.py
+-rw-r--r--   0        0        0     7202 2023-07-26 02:58:58.897478 chilitools-0.2.4/chilitools/api/connector.py
+-rw-r--r--   0        0        0    21203 2023-07-31 18:36:41.911804 chilitools-0.2.4/chilitools/api/endpoints.py
+-rw-r--r--   0        0        0     3728 2023-03-21 14:29:37.670561 chilitools-0.2.4/chilitools/api/mycp.py
+-rw-r--r--   0        0        0     3114 2022-09-20 16:25:32.069762 chilitools-0.2.4/chilitools/api/response.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:25:18.519289 chilitools-0.2.4/chilitools/grafx/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 19:59:39.899564 chilitools-0.2.4/chilitools/grafx/api/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-22 21:44:25.944416 chilitools-0.2.4/chilitools/grafx/api/environment.py
+-rw-r--r--   0        0        0      513 2023-06-22 22:42:14.136612 chilitools-0.2.4/chilitools/grafx/api/platform.py
+-rw-r--r--   0        0        0     2584 2023-07-27 16:52:54.465186 chilitools-0.2.4/chilitools/grafx/auth.py
+-rw-r--r--   0        0        0     1941 2023-07-27 16:52:30.339296 chilitools-0.2.4/chilitools/grafx/connector.py
+-rw-r--r--   0        0        0     2370 2023-07-27 17:26:37.658495 chilitools-0.2.4/chilitools/grafx/document.py
+-rw-r--r--   0        0        0      662 2023-06-22 22:26:48.267393 chilitools-0.2.4/chilitools/grafx/environment.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:57:26.204562 chilitools-0.2.4/chilitools/publisher/__init__.py
+-rw-r--r--   0        0        0     2263 2023-07-12 15:49:38.021139 chilitools-0.2.4/chilitools/publisher/document.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257581 chilitools-0.2.4/chilitools/settings/__init__.py
+-rw-r--r--   0        0        0      199 2022-04-15 23:48:49.570757 chilitools-0.2.4/chilitools/settings/config.py
+-rw-r--r--   0        0        0    17933 2023-07-31 19:18:35.661107 chilitools-0.2.4/chilitools/utilities/ServerMigration.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257751 chilitools-0.2.4/chilitools/utilities/__init__.py
+-rw-r--r--   0        0        0     2104 2022-10-28 20:09:34.951802 chilitools-0.2.4/chilitools/utilities/backoffice.py
+-rw-r--r--   0        0        0      602 2022-04-15 23:48:53.626324 chilitools-0.2.4/chilitools/utilities/defaults.py
+-rw-r--r--   0        0        0     2903 2023-07-31 18:31:52.474774 chilitools-0.2.4/chilitools/utilities/document.py
+-rw-r--r--   0        0        0      897 2022-07-21 19:16:13.652722 chilitools-0.2.4/chilitools/utilities/errors.py
+-rw-r--r--   0        0        0     6022 2022-10-28 20:05:22.841538 chilitools-0.2.4/chilitools/utilities/file.py
+-rw-r--r--   0        0        0      807 2023-06-20 15:02:52.753030 chilitools-0.2.4/chilitools/utilities/logger.py
+-rw-r--r--   0        0        0      509 2022-06-29 19:01:07.878458 chilitools-0.2.4/chilitools/utilities/strings.py
+-rw-r--r--   0        0        0     3831 2023-03-21 15:07:48.139637 chilitools-0.2.4/chilitools/utilities/xmltools.py
+-rw-r--r--   0        0        0      505 2023-08-01 18:55:21.533000 chilitools-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 chilitools-0.2.4/PKG-INFO
```

### Comparing `chilitools-0.2.3/chilitools/__init__.py` & `chilitools-0.2.4/chilitools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 import pyperclip as pc
 from chilitools.utilities.backoffice import backofficeURLInput
 from chilitools.api.connector import ChiliConnector
 from chilitools.api.mycp import generateLoginTokenForURL, generateOAuthTokenFromCredentials, setUserType, deleteLoginFile
 from chilitools.utilities.defaults import STAFF_TYPE
```

### Comparing `chilitools-0.2.3/chilitools/api/connector.py` & `chilitools-0.2.4/chilitools/api/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,17 @@
 
         return response
 
 
     def getAPIKey(self) -> str:
         genKey = True
 
-        if self.username and self.password:
-            self._displayMsg("ChiliConnector: Using supplied credentials instead of stored credentials to authenticate")
+        if self.debugLevel == 2:
+            if self.username and self.password:
+                self._displayMsg("ChiliConnector: Using supplied credentials instead of stored credentials to authenticate")
 
         if self.forceKeyRegen:
             self._displayMsg("ChiliConnector: Forcing a new API key to be generated")
         else:
             if checkForFile(APIKEY_FILE):
                 try:
                     apiKeys = readFile(fileName=APIKEY_FILE, isJSON=True)
```

### Comparing `chilitools-0.2.3/chilitools/api/endpoints.py` & `chilitools-0.2.4/chilitools/api/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     from chilitools.api.response import ChiliResponse
 
 from time import sleep
 from chilitools.api.mycp import generateLoginTokenForURL, getCredentials
 from chilitools.utilities.errors import ErrorHandler
 from chilitools.utilities.file import getBase64String
 from chilitools.utilities.defaults import DEFAULT_TASKPRIORITY, DEFAULT_TASKUPDATETIME, STAFF_TYPE, USER_TYPE
+from chilitools.utilities.document import ChiliDocument
 
 class Resources:
   def __init__(self, connector: ChiliConnector):
     self.connector = connector
   def DownloadTempFile(self, assetType: str, path: str = '', data: str = '', dynamicAssetProviderID: str = '', noContentHeader: bool = None) -> ChiliResponse:
     return self.connector.makeRequest(
       method='get',
@@ -185,15 +186,15 @@
     return self.ResourceFolderAdd(
       resourceType=resourceType,
       newName=folderName,
       parentPath=folderPath,
       )
 
   def doesItemExist(self, resourceType: str, itemID: str) -> bool:
-    res = self.ResourceItemGetDefinitionXML(resourceType, itemID)
+    res = self.ResourceItemGetXML(resourceType, itemID)
     if res.statusCode == 404:
       return False
     return True
 
   def get_name_if_exists(self, resourceType: str, itemID: str):
     res = self.ResourceItemGetDefinitionXML(resourceType, itemID)
     if res.statusCode == 404:
@@ -389,14 +390,19 @@
     )
   def processServerSide(self, documentID: str) -> ChiliResponse:
     return self.connector.makeRequest(
     method='put',
     endpoint=f"/resources/documents/documentprocessor",
     json={'itemID':documentID, 'resourceXML':''}
   )
+  def is_blank(self, doc) -> bool:
+    if isinstance(doc, str):
+      doc = ChiliDocument(doc)
+    if len(doc.frames) > 0: return False
+    return True
 
 class System:
   def __init__(self, connector: ChiliConnector):
     self.connector = connector
 
   def getTaskStatus(self, taskID: str) -> ChiliResponse:
     return self.connector.makeRequest(
@@ -434,11 +440,11 @@
       json=requestJSON,
       authRequired=False
     )
 
   def SetAutomaticPreviewGeneration(self, createPreviews: bool) -> ChiliResponse:
     return self.connector.makeRequest(
       method='put',
-      endpoint='system/apikey/autopreviewgeneration',
+      endpoint='/system/apikey/autopreviewgeneration',
       queryParams={'createPreviews':createPreviews}
     )
```

### Comparing `chilitools-0.2.3/chilitools/api/mycp.py` & `chilitools-0.2.4/chilitools/api/mycp.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/api/response.py` & `chilitools-0.2.4/chilitools/api/response.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/grafx/api/environment.py` & `chilitools-0.2.4/chilitools/grafx/api/environment.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/grafx/api/platform.py` & `chilitools-0.2.4/chilitools/grafx/api/platform.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/grafx/auth.py` & `chilitools-0.2.4/chilitools/grafx/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import requests
 import datetime
 
 from os import getenv
 
 
 class GraFxAuth:
-    def __init__(self, email: str = None, password: str = None, client_id: str = None, client_secret: str = None):
+    def __init__(self, client_id: str = None, client_secret: str = None):
         # Check if credentials were supplied
-        if all([email, password, client_id, client_secret]):
-            self.email = email
-            self.password = password
-            self.client_id = client_id,
+        if all([client_id, client_secret]):
+            self.client_id = client_id
             self.client_secret = client_secret
         elif getenv("GRAFX_EMAIL") and getenv("GRAFX_PASSWORD") and getenv("GRAFX_CLIENT_ID") and getenv("GRAFX_CLIENT_SECRET"):
             self.email = getenv("GRAFX_EMAIL")
             self.password = getenv("GRAFX_PASSWORD")
             self.client_id = getenv("GRAFX_CLIENT_ID")
             self.client_secret = getenv("GRAFX_CLIENT_SECRET")
         else:
@@ -26,26 +24,39 @@
         if hasattr(self, "_token") and not self._is_token_expired(self._token):
           return self._token["access_token"]
 
         headers = {
             "content-type": "application/json",
         }
 
-        body = {
-            "grant_type": "password",
-            "audience": "https://chiligrafx.com",
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
-            "username": self.email,
-            "password": self.password,
-        }
-
-        resp = requests.post(url="https://login.chiligrafx.com/oauth/token",
-                     headers=headers,
-                     json=body)
+        # User credentials password flow
+        if hasattr(self, "email"):
+            url = "https://login.chili-grafx.com/oauth/token"
+            body = {
+                "grant_type": "password",
+                "audience": "https://chiligrafx.com",
+                "client_id": self.client_id,
+                "client_secret": self.client_secret,
+                "username": self.email,
+                "password": self.password,
+            }
+        # Integration flow
+        else:
+            url = "https://integration-login.chiligrafx.com/oauth/token"
+            body = {
+                "grant_type": "client_credentials",
+                "audience": "https://chiligrafx.com",
+                "client_id": self.client_id,
+                "client_secret": self.client_secret,
+            }
+
+        resp = requests.post(
+            url=url,
+            headers=headers,
+            json=body)
 
         if (resp.status_code != 200):
             raise Exception(f"There was an error generating the auth token\n{resp.text}")
 
         resp = resp.json()
         expiration_offset = int(resp['expires_in'] * .9)
         self._token = {
```

### Comparing `chilitools-0.2.3/chilitools/grafx/connector.py` & `chilitools-0.2.4/chilitools/grafx/connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from chilitools.grafx.api.platform import Platform
 
 
 #Todo(austin): Make some like exception handling thing where you just check_response(resp) and it throws for the usual 401 stuff, etc.
 
 # Gonna embrace the class madness I guess.
 class GraFxConnector:
-    def __init__(self, environment: str, environment_type: str = "production", email: str = None, password: str = None, client_id: str = None, client_secret: str = None, logger = None, api_version: str = "1"):
+    def __init__(self, environment: str, environment_type: str = "production", client_id: str = None, client_secret: str = None, logger = None, api_version: str = "1"):
         self.environment = environment
-        self.auth = GraFxAuth(email, password, client_id, client_secret)
+        self.auth = GraFxAuth(client_id, client_secret)
         self.environment = GraFxEnvironment(
             environment_name=environment,
             environment_type=environment_type,
             api_version=api_version
         )
         self.logger = logger
         self.templates = Templates(self)
```

### Comparing `chilitools-0.2.3/chilitools/grafx/document.py` & `chilitools-0.2.4/chilitools/grafx/document.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 class DocumentFont:
     def __init__(self, id: str, name: str, family: str, style: str):
         self.id = id
         self.name = name
         self.family = family
         self.style = style
 
+class DocumentImage:
+    def __init__(self, id: str):
+        self.id = id;
+
 class GraFxDocument:
     def __init__(self, doc: str, id: str = None, name: str = None):
         try:
             # We were passed a parsed JSON document
             if isinstance(doc, dict):
                 self.doc = doc
             # We were passed the raw JSON string of the document
@@ -27,32 +31,35 @@
     def json(self): return str(self)
 
     @property
     def images(self):
       image_frames = []
       for page in self.doc["pages"]:
           for frame in page["frames"]:
-              # Todo(austin): Figure out how the hell you want to handle this
-              if frame["frameType"] == "image":
+                print(frame)
+                if frame.get("frameType") == "image" or frame.get("type") == "image":
                     # Image is coming from a connector
-                    if frame["src"].get("connectorId") == "grafx-media":
-                        image_frames.append(frame)
+                    if frame["src"].get("connectorId") or frame["src"].get("id") == "grafx-media":
+                        image_id = frame["src"]["assetId"]
                     # Image is is a variable
-                    if frame["src"].get("variableId"):
+                    if frame["src"].get("variableId") or frame["src"].get("type") == "variable":
+                        var_id = frame["src"].get("variableId") or frame["src"].get("id")
                         # Find and get the asset Id from the variable
                         for var in self.doc["variables"]:
-                            if var.get("id") == frame["src"].get("variableId"):
-                                frame["src"]["assetId"] = var["src"]["assetId"]
-                                image_frames.append(frame)
+                            if var.get("id") == var_id:
+                                image_id = var["src"]["assetId"]
+                                break
+                    image = DocumentImage(image_id)
+                    image_frames.append(image)
       return image_frames
 
     @property
     def fonts(self):
         fonts = []
-        for font in self.doc["styleKit"]["fonts"]:
+        for font in self.doc["stylekit"]["fonts"]:
             #TODO(austin) Fix this when they break me
             fonts.append(DocumentFont(font["fontId"], font["name"], font["fontFamily"], font["fontStyle"]))
         return fonts
 
 
     def __str__(self): return json.dumps(self.doc)
     def __repr__(self): return self.doc
```

### Comparing `chilitools-0.2.3/chilitools/grafx/environment.py` & `chilitools-0.2.4/chilitools/grafx/environment.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/utilities/ServerMigration.py` & `chilitools-0.2.4/chilitools/utilities/ServerMigration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,44 @@
-import os
 import base64
 from time import sleep
 from chilitools.api.connector import ChiliConnector
 from chilitools.utilities.file import writeFile, readFile, checkForFile
-from chilitools.utilities.backoffice import backofficeURLInput
 from chilitools.utilities.logger import getLogger
+from chilitools.utilities.document import ChiliDocument
 
 
 class ServerMigrator:
-  def __init__(self, directory: str, verbose: bool = False, update: bool = False, sourceChili: str = None, destChili: str = None):
+  def __init__(self, srcChili: ChiliConnector, destChili: ChiliConnector, directory: str, verbose: bool = False, update: bool = False):
     # Try to load the progress JSON file
     self.progressFile = directory+'/progress.json'
     if checkForFile(fileName=self.progressFile):
       print("Found progress file for server migration, loading it.")
       self.progress = readFile(fileName=self.progressFile, isJSON=True)
-      self.source = ChiliConnector(backofficeURL=self.progress['sourceURL'])
-      self.dest = ChiliConnector(backofficeURL=self.progress['destURL'])
+      if self.progress.get('sourceUsername'):
+        print("Loading user information for source environment")
+        self.source = ChiliConnector(backofficeURL=self.progress['sourceURL'], username=self.progress['sourceUsername'], password=self.progress['sourcePassword'])
+      else:
+        self.source = ChiliConnector(backofficeURL=self.progress['sourceURL'])
+
+      if self.progress.get('destUsername'):
+        print("Loading user information for destination environment")
+        self.dest = ChiliConnector(backofficeURL=self.progress['destURL'], username=self.progress['destUsername'], password=self.progress['destPassword'])
+      else:
+        self.dest = ChiliConnector(backofficeURL=self.progress['destURL'])
     else:
       # progress JSON not found
-      if sourceChili is None:
-        print("-------------SOURCE CHILI BACKOFFICE URL---------------")
-        sourceChili = backofficeURLInput()
-      if destChili is None:
-        print("-------------DESTINATION CHILI BACKOFFICE URL---------------")
-        destChili = backofficeURLInput()
-      self.source = ChiliConnector(backofficeURL=sourceChili)
-      self.dest = ChiliConnector(backofficeURL=destChili)
-      self.progress = {'sourceURL': sourceChili, 'destURL': destChili, 'resources':{}}
+      self.source = srcChili
+      self.dest = destChili
+      self.progress = {'sourceURL': srcChili.backofficeURL, 'destURL': destChili.backofficeURL, 'resources':{}}
+      if self.source.username:
+        self.progress['sourceUsername'] = self.source.username
+        self.progress['sourcePassword'] = self.source.password
+      if self.dest.username:
+        self.progress['destUsername'] = self.dest.username
+        self.progress['destPassword'] = self.dest.password
       self._saveProgressFile()
 
     self.directory = directory
     self.logger = getLogger(directory+'/ServerMigrator.log')
     self.verbose = verbose
     self.interval = 1
     self.update = update
@@ -39,15 +47,15 @@
     self.logger.info("Getting list of resource items")
     resources = set()
     r = self.source.resources.getResourceList().content
     for item in r['resources']['item']: resources.add(item['@name'].lower())
     for resource in resources:
       if not resource in self.progress['resources'].keys() or self.update:
         self.getResourceTree(resource)
-      elif self.verbose: print(f"Already found resource tree for {resource}. Pass the update=True arg to force update")
+      elif self.verbose: print(f"Already found resource tree for {resource}. Pass the update=True arg to force update the tree")
 
   def getResourceTree(self, resource: str, parentFolder: str = ''):
     resource = resource.lower()
     self.logger.info(f"Getting resource tree for {resource}.. This may take some time depending on size")
     resp = self.source.resources.ResourceGetTreeLevel(resourceType=resource, parentFolder=parentFolder, numLevels=-1, includeSubDirectories=True)
     if resp.success:
       path = f"{self.directory}/{resource}/{resource}.json"
@@ -76,21 +84,25 @@
         if self.verbose:
           self.logger.info(f"Getting item definition XML for ID: {item}")
         resp = self.source.resources.ResourceItemGetDefinitionXML(
           resourceType=resource,
           itemID=item
         )
         if not resp.success:
-          self.logger.error(f"There was an issue getting item definition xml for the item id: {item}")
+          if resource == "fonts":
+            self.logger.warn(f"There was an issue getting item definition for {resource} with id: {item}")
+          else:
+            self.logger.error(f"There was an issue getting item definition for {resource} with id: {item}")
           if self.verbose:
             print(resp.asDict())
-        itemXML = resp.contentAsDict()['item']
-        itemXML['@path'] = itemXML['@relativePath']
-        self.progress['resources'][resource]['toTransfer'].append(itemXML)
-        #self._saveProgressFile()
+        else:
+          itemXML = resp.contentAsDict()['item']
+          itemXML['@path'] = itemXML['@relativePath']
+          self.progress['resources'][resource]['toTransfer'].append(itemXML)
+          #self._saveProgressFile()
       self.__transferItems(resource=resource, disablePreviews=False)
 
   def transferResource(self, resource: str, parentFolder: str = '', customPath: str = None):
     resource = resource.lower()
     if not resource in self.progress['resources'].keys() or self.update or 'treeFile' not in self.progress['resources'][resource].keys():
       self.logger.info(f'Updating {resource} directory tree structure')
       self.getResourceTree(resource, parentFolder)
@@ -132,37 +144,44 @@
       itemList = items.copy()
       itemAmount = len(itemList)
       self.logger.info(f'Amount of {resource} to transfer: {itemAmount}')
       for r in itemList:
         if self.verbose:
           print(f"Name: {r['@name']}\nID: {r['@id']}\nPath: {r['@path']}\nDownload URL: {self.getDownloadURL(resource, r['@id'])}\n")
 
+        self.logger.info(f"Checking if {resource}: {r.get('@id')} exists on destination environment")
+        if self.dest.resources.doesItemExist(resource, r.get('@id')):
+          self.logger.info(f"{resource}: {r.get('@id')} exists on destination environment. Skipping...")
+          continue
+
         # Set ID for the next item
         self.logger.info(f"Setting the ID for the next uploaded item to: {r['@id']}")
         resp = self.dest.resources.setNextResourceItemID(resourceType=resource, itemID=r['@id'])
         if not resp.didSucceed():
           self.logger.error(f"There was an issue setting the next item ID for {r['@name']}: {r['@id']}\n{resp.text}")
           continue
         elif self.verbose:
           print(f"\n{resp.text}\n")
 
-        # Extract path from resource tree item (orginal path is full path ending with <document name>.xml)
+        # Extract path from resource tree item (original path is full path ending with <document name>.xml)
         if len(r['@path']) != 0:
           splitPath = r['@path'].split("\\")
           fileName = splitPath.pop()
           resourceItemPath = "\\".join(splitPath)+"\\"
         else:
+          fileName = r['@name']
           resourceItemPath = ''
+        print(f"Path: {resourceItemPath}")
 
-        # IF ASSET = NEED TO USE MACHINE AS MIDDLEMAN
-        if resource.lower() == 'assets':
-          # Download Asset
+        # If the resource is an asset or font.
+        if resource == 'assets' or resource == 'fonts':
+          # Download the resource file data
           self.logger.info(f"Downloading asset file data temporarily for: {r['@name']}")
           fileData = self.source.resources.DownloadAsset(
-            resourceType='assets',
+            resourceType=resource,
             id=r['@id'],
             itemPath=r['@path'],
             assetType='original',
             page=1
           )
           if not resp.didSucceed():
             self.logger.error(f"There was an issue downloading the asset - Name: {r['@name']} -- Item ID: {r['@id']}\n{resp.text}")
@@ -170,33 +189,137 @@
 
           # Base64 Encode the byte data
           fileData = base64.b64encode(fileData.response.content)
           fileData = fileData.decode('utf-8')
 
           self.logger.info(f"Uploading asset data to destination CHILI server: {r['@name']}")
           resp = self.dest.resources.ResourceItemAdd(
-            resourceType='assets',
+            resourceType=resource,
             newName=fileName,
             fileData=fileData,
-            xml='',
+            xml=None,
             folderPath=resourceItemPath
           )
           if not resp.didSucceed():
             self.logger.error(f"There was an issue uploading the asset to the destination server- Name: {r['@name']} -- Item ID: {r['@id']}\n{resp.text}")
             continue
 
+          self.logger.info(f"Comparing file sizes for - Name: {r['@name']} -- Item ID: {r['@id']}\n") 
+          itemSizeDest = self.dest.resources.ResourceItemGetDefinitionXML(resourceType=resource, itemID=r['@id'])
+          itemSizeSrc = self.source.resources.ResourceItemGetDefinitionXML(resourceType=resource, itemID=r['@id'])
+
+          # Check file size
+          if itemSizeSrc.data['item']['fileInfo']['@fileSize'] != itemSizeDest.data['item']['fileInfo']['@fileSize']:
+            self.logger.error(f"{resource} wrong size from dest to src - Name: {r['@name']} -- Item ID: {r['@id']}\n")
+
+        elif resource == "documents":
+          # Download document
+          self.logger.info(f"Downloading document XML temporarily for: {r['@name']}")
+          resp = self.source.resources.ResourceItemGetXML(
+            resourceType='documents',
+            itemID=r['@id'],
+          )
+          if not resp.didSucceed():
+            self.logger.error(f"There was an issue downloading the document - Name: {r['@name']} -- Item ID: {r['@id']}\n{resp.text}")
+            continue
+
+          docXml = resp.text
+
+          cd = ChiliDocument(docXml)
+
+          # Get the DataSource ID attached to the document if there is one
+          datasource_id = cd.datasource_id
+
+          fonts = []
+          for font in cd.get_fonts():
+            fonts.append(font["id"])
+
+          assets = cd.get_images()
+          images = [image.get("id") for image in assets if image.get("resource_type") == "Assets"]
+          daps = [image.get("id") for image in assets if image.get("resource_type" == "DynamicAssetProviders")]
+          barcodes = cd.get_barcode_ids()
+
+
+          if fonts:
+            self.logger.info(f"Found fonts in document, transferring... (Arial Regular will probably fail)")
+            self.transferList(itemList=fonts, resource="Fonts")
+          if images:
+            self.logger.info(f"Found images in document, transferring...")
+            self.transferList(itemList=images, resource="Assets")
+          if daps:
+            self.logger.info(f"Found Dynamic Asset Providers in document, transferring settings for DAP...")
+            self.transferList(itemList=daps, resource="DynamicAssetProviders")
+          if barcodes:
+            self.logger.info(f"Found Barcode frames in document, transferring Barcode settings...")
+            self.transferList(itemList=barcodes, resource="BarcodeTypes")
+          if datasource_id:
+            self.logger.info(f"Found DataSource attached to document, transferring DataSource settings")
+            self.transferList(itemList=[datasource_id], resource="DataSources")
+
+          # Create a placeholder document because if you ResourceItemAdd a document, CHILI will process the XML and will remove spaces
+          self.logger.info(f"Creating placeholder document to destination CHILI server: {r['@name']}")
+          resp = self.dest.resources.ResourceItemAdd(
+            resourceType='documents',
+            newName=fileName,
+            folderPath=resourceItemPath,
+            xml='<document />'
+          )
+          if not resp.didSucceed():
+            self.logger.error(f"There was an issue creating a placeholder document to the destination server- Name: {r['@name']} -- Item ID: {r['@id']}\n{resp.text}")
+            continue
+
+          # CHILI loves blank documents so retry until it's not blank
+          blank_doc = True
+
+          while blank_doc:
+            self.logger.info(f"Uploading document data to destination CHILI server: {r['@name']}")
+            resp = self.dest.resources.ResourceItemSave(
+              resourceType="documents",
+              itemID=r['@id'],
+              xml=docXml,
+            )
+            if not resp.didSucceed():
+              self.logger.error(f"There was an issue uploading the document to the destination server- Name: {r['@name']} -- Item ID: {r['@id']}\n{resp.text}")
+              break
+
+            self.logger.info(f"Processing document server side: {r['@name']}")
+            resp = self.dest.documents.processServerSide(
+              documentID=r['@id']
+            )
+            sleep(1)
+
+            self.logger.info(f"Checking if uploading doc is blank: {r['@name']}")
+            resp = self.dest.resources.ResourceItemGetXML(
+              resourceType="documents",
+              itemID=r['@id'])
+            if not resp.didSucceed():
+              self.logger.error(f"There was an issue getting the document XML for the blank document check- Name: {r['@name']} -- Item ID: {r['@id']}\n{resp.text}")
+              break
+
+            blank_doc = self.dest.documents.is_blank(resp.text)
+            if blank_doc: self.logger.info(f"Uploaded document was blank. Going to retry the ResourceItemSave{r['@name']}")
+            else: self.logger.info(f"Uploaded document is not blank")
+
+        # Item is not a document, asset, or font
         else:
-          # Items other than assets
-          # Transfer the item
-          resp = self.dest.resources.ResourceItemAddFromURL(
+          # Get the item XML (I think only assets and fonts are using fileData)
+          resp = self.source.resources.ResourceItemGetXML(resourceType=resource, itemID=r['@id'])
+          if not resp.didSucceed():
+            self.logger.error(f"There was an issue getting the item XML - Name: {r['@name']} -- Item ID: {r['@id']}\n{resp.text}")
+            continue
+          elif self.verbose:
+            print(f"\n{resp.text}\n")
+
+          item_xml = resp.text
+
+          resp = self.dest.resources.ResourceItemAdd(
             resourceType=resource,
             newName=r['@name'],
             folderPath=resourceItemPath,
-            url=self.getDownloadURL(resource, r['@id']),
-            reuseExisting=True
+            xml=item_xml
           )
           if not resp.didSucceed():
             self.logger.error(f"There was an issue adding the item - Name: {r['@name']} -- Item ID: {r['@id']}\n{resp.text}")
             continue
           elif self.verbose:
             print(f"\n{resp.text}\n")
 
@@ -240,23 +363,12 @@
             if self.verbose:
               self.logger.info(f"Adding {v} to the transfer queue")
       elif isinstance(v, str):
         if isinstance(d[v], list):
           self.__iterresource(resource, d[v])
 
   def getDownloadURL(self, resource: str, itemID: str):
-    #http://cp-cqd-514/download.aspx?type=original&resourceName=Assets&id=2288c92c-7154-48f1-a8b3-599c0df6e368&apiKey=xyl678LaRqKrOK0VNtB9HvlnElxhdDsq6Wig8zGKjYoDGyPsKhf79UtPzIr8Q1agid2MgNLNJAxPXjY6bB8dzg==&pageNum=1
     downloadURL =  self.source.baseURL + self.source.enviroment + '/download.aspx?type=original&resourceName=' + resource + '&id=' + itemID + '&apiKey=' + self.source.getAPIKey() + '&pageNum=1'
     return downloadURL
 
   def _saveProgressFile(self):
-    writeFile(fileName=self.progressFile, data=self.progress, isJSON=True)
-
-if __name__ == '__main__':
-  path = os.path.dirname(os.path.realpath(__file__))+'/'
-  # print('Please enter a name for the migration project')
-  # print('A progress folder can also be found using this name, if it does not exist, one will be created')
-  # migrationName = input().strip().lower()
-  # ServerMigrator(directory=path+'/'+migrationName)
-  m = ServerMigrator(directory=path+'coke', verbose=True, sourceChili='https://chili1-cdn.dmex.coke.com/CHILI/Admin/interface.aspx', destChili='https://ft-nostress.chili-publish-sandbox.online/ft-nostress/interface.aspx')
-
-  m.transferResource(resource='Workspaces', parentFolder='\\')
+    writeFile(fileName=self.progressFile, data=self.progress, isJSON=True)
```

### Comparing `chilitools-0.2.3/chilitools/utilities/backoffice.py` & `chilitools-0.2.4/chilitools/utilities/backoffice.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/utilities/defaults.py` & `chilitools-0.2.4/chilitools/utilities/defaults.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/utilities/document.py` & `chilitools-0.2.4/chilitools/utilities/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 from lxml import etree
 
 class ChiliDocument:
   def __init__(self, doc_xml: str):
     try:
       self.doc: etree._Element = etree.fromstring(doc_xml)
-      self.name = self._extract_name()
-      self.id = self._extract_id()
     except Exception as e:
+      self.doc = None
       print(f"There was an error creating a Document from the XML\n {e}")
 
-  def _extract_name(self):
+  @property
+  def name(self):
     if self.doc is None: return
     return self.doc.attrib.get('name')
 
-  def _extract_id(self):
+  @property
+  def id(self):
     if self.doc is None: return
     return self.doc.attrib.get('id')
 
   def __str__(self) -> str:
     return self.to_xml()
 
   def to_xml(self) -> str:
     return etree.tostring(self.doc, method="xml", encoding="unicode")
 
+  @property
+  def datasource_id(self):
+    if self.doc is None: return
+    ds = self.get_datasource()
+    if ds is not None: return ds.get('dataSourceID')
+    return None
+
   def get_datasource(self):
     return self.doc.find("dataSource")
 
   def get_datasource_string(self) -> str:
     return etree.tostring(self.get_datasource(), encoding="unicode")
 
   def set_datasource(self, new_datasource):
@@ -43,19 +51,37 @@
         "name": font.get("name"),
         "family": font.get("family"),
         "style": font.get("style")
       })
 
     return fonts
 
+  def _get_frames(self, frame_type: str = "any"):
+    if self.doc is None: return
+    frames = []
+
+    for frame in self.doc.findall("pages//frames/item"):
+      inline_frames = frame.findall("inlineFrames//item//frame")
+      if inline_frames:
+        for e in inline_frames:
+          if frame_type == "any" or e.get("type") == frame_type:
+            frames.append(e)
+      if frame_type == "any" or frame.get("type") == frame_type:
+        frames.append(frame)
+    return frames
+
+  @property
+  def frames(self):
+    return self._get_frames(frame_type="any")
+
   def get_images(self):
     if self.doc is None: return
     images = []
 
-    for image_frame in self.doc.findall("pages//item[@type='image']"):
+    for image_frame in self._get_frames("image"):
       if image_frame.get("hasContent", "false") == "true":
         if len(image_frame.get("dynamicAssetProviderID", "")) > 1:
           images.append({
             "resource_type": "DynamicAssetProviders",
             "id": image_frame.get("dynamicAssetProviderID")
           })
         else:
@@ -64,9 +90,15 @@
             "id": image_frame.get("externalID"),
             "name": image_frame.get("externalName", ""),
             "path": image_frame.get("path", "")
           })
 
     return images
 
+  def get_barcode_ids(self):
+    return [b.get("barcodeTypeID") for b in self.barcode_frames()]
+
+  def barcode_frames(self):
+    return self._get_frames(frame_type="barcode")
+
   def text_frames(self):
-    return self.doc.findall("pages//item[@type='text']")
+    return self._get_frames(frame_type="text")
```

### Comparing `chilitools-0.2.3/chilitools/utilities/errors.py` & `chilitools-0.2.4/chilitools/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/utilities/file.py` & `chilitools-0.2.4/chilitools/utilities/file.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/utilities/logger.py` & `chilitools-0.2.4/chilitools/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/chilitools/utilities/xmltools.py` & `chilitools-0.2.4/chilitools/utilities/xmltools.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.3/PKG-INFO` & `chilitools-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chilitools
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of tools for working with CHILI products
 Author: Austin
 Author-email: austin.meier@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

