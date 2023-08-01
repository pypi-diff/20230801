# Comparing `tmp/devcloud-2023.3.1-py2.py3-none-any.whl.zip` & `tmp/devcloud-2023.4.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 20042 bytes, number of entries: 14
--rw-rw-r--  2.0 unx     1833 b- defN 23-Mar-16 03:16 devcloud/Devcloud.py
--rw-rw-r--  2.0 unx       32 b- defN 23-Mar-16 03:16 devcloud/__init__.py
--rw-rw-r--  2.0 unx     7531 b- defN 23-Mar-16 03:16 devcloud/common.py
--rw-rw-r--  2.0 unx    15842 b- defN 23-Mar-16 03:16 devcloud/container.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Mar-16 03:16 devcloud/edgenode.py
--rw-rw-r--  2.0 unx     2553 b- defN 23-Mar-16 03:16 devcloud/environment.json
--rw-rw-r--  2.0 unx     5860 b- defN 23-Mar-16 03:16 devcloud/project.py
--rw-rw-r--  2.0 unx     1908 b- defN 23-Mar-16 03:16 devcloud/result.py
--rw-rw-r--  2.0 unx     2553 b- defN 23-Mar-16 03:16 devcloud-2023.3.1.data/data/devcloud/environment.json
--rw-rw-r--  2.0 unx    11357 b- defN 23-Mar-16 03:16 devcloud-2023.3.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7464 b- defN 23-Mar-16 03:16 devcloud-2023.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Mar-16 03:16 devcloud-2023.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Mar-16 03:16 devcloud-2023.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1133 b- defN 23-Mar-16 03:16 devcloud-2023.3.1.dist-info/RECORD
-14 files, 66381 bytes uncompressed, 18170 bytes compressed:  72.6%
+Zip file size: 20181 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx     1847 b- defN 23-Aug-01 04:02 devcloud/Devcloud.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Aug-01 04:02 devcloud/__init__.py
+-rw-rw-r--  2.0 unx     7531 b- defN 23-Aug-01 04:02 devcloud/common.py
+-rw-rw-r--  2.0 unx    15842 b- defN 23-Aug-01 04:02 devcloud/container.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Aug-01 04:02 devcloud/edgenode.py
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Aug-01 04:02 devcloud/environment.json
+-rw-rw-r--  2.0 unx     5860 b- defN 23-Aug-01 04:02 devcloud/project.py
+-rw-rw-r--  2.0 unx     1908 b- defN 23-Aug-01 04:02 devcloud/result.py
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Aug-01 04:02 devcloud-2023.4.2.data/data/devcloud/environment.json
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Aug-01 04:02 devcloud-2023.4.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7606 b- defN 23-Aug-01 04:02 devcloud-2023.4.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Aug-01 04:02 devcloud-2023.4.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Aug-01 04:02 devcloud-2023.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Aug-01 04:02 devcloud-2023.4.2.dist-info/RECORD
+14 files, 67513 bytes uncompressed, 18309 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: devcloud/project.py
 Comment: 
 
 Filename: devcloud/result.py
 Comment: 
 
-Filename: devcloud-2023.3.1.data/data/devcloud/environment.json
+Filename: devcloud-2023.4.2.data/data/devcloud/environment.json
 Comment: 
 
-Filename: devcloud-2023.3.1.dist-info/LICENSE
+Filename: devcloud-2023.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: devcloud-2023.3.1.dist-info/METADATA
+Filename: devcloud-2023.4.2.dist-info/METADATA
 Comment: 
 
-Filename: devcloud-2023.3.1.dist-info/WHEEL
+Filename: devcloud-2023.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: devcloud-2023.3.1.dist-info/top_level.txt
+Filename: devcloud-2023.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: devcloud-2023.3.1.dist-info/RECORD
+Filename: devcloud-2023.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## devcloud/Devcloud.py

```diff
@@ -2,20 +2,20 @@
 from devcloud.project import *
 from devcloud.container import *
 from devcloud.edgenode import *
 import getpass
 from devcloud.result import *
 
 
-def connect(token: str = ""):
+def connect(token: str = "", env: str = "CP"):
     if len(token) == 0:
         token=os.getenv('DEVCLOUD_TOKEN')
         if token == None:
             token = getpass.getpass("Token:")
-    login(token, "PROD")
+    login(token, env)
     print("LoggedIn")
     updateEdgeId()
     print("Overview - Project")
     getProject()
     print("Overview - Dashboard")
     getStatus(output="wide")
```

## devcloud/environment.json

### Pretty-printed

 * *Similarity: 0.4%*

 * *Differences: {"'CP'": "OrderedDict([('BYOC_ENV', 'https://frontend.apps.cfa.devcloud.intel.com/byoc/'), "*

 * *         "('BYOS_ENV', 'https://frontend.apps.cfa.devcloud.intel.com/byos/'), ('EDGENODE_ENV', "*

 * *         "'https://frontend.apps.cfa.devcloud.intel.com/edgenode/'), ('EXECUTION_ENV', "*

 * *         "'https://frontend.apps.cfa.devcloud.intel.com/execution/'), ('CONFIG_ENV', "*

 * *         "'https://frontend.apps.cfa.devcloud.intel.com/config/')])",*

 * * "'PRC'": "OrderedDict([('BYOC_ENV', "*

 * *          "'https://frontend-devcloud […]*

```diff
@@ -1,15 +1,22 @@
 {
-    "PROD": {
+    "CP": {
         "BYOC_ENV": "https://frontend.apps.cfa.devcloud.intel.com/byoc/",
         "BYOS_ENV": "https://frontend.apps.cfa.devcloud.intel.com/byos/",
         "CONFIG_ENV": "https://frontend.apps.cfa.devcloud.intel.com/config/",
         "EDGENODE_ENV": "https://frontend.apps.cfa.devcloud.intel.com/edgenode/",
         "EXECUTION_ENV": "https://frontend.apps.cfa.devcloud.intel.com/execution/"
     },
+    "PRC": {
+        "BYOC_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/byoc/",
+        "BYOS_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/byos/",
+        "CONFIG_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/config/",
+        "EDGENODE_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/edgenode/",
+        "EXECUTION_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/execution/"
+    },
     "endPoints": {
         "configuration": "api/v1/container/createConfiguration",
         "containers": "api/v1/containers",
         "deleteBuild": "api/v1/s2i/user/deleteBuild/{}",
         "deployMultipleHardware": "api/v1/containers/deploy-multi-hardware",
         "edgenode": "api/v1/edge-node/edges",
         "log": "api/v1/logs/pod?podName={}",
```

## Comparing `devcloud-2023.3.1.data/data/devcloud/environment.json` & `devcloud-2023.4.2.data/data/devcloud/environment.json`

 * *Files 18% similar despite different names*

### Pretty-printed

 * *Similarity: 0.4%*

 * *Differences: {"'CP'": "OrderedDict([('BYOC_ENV', 'https://frontend.apps.cfa.devcloud.intel.com/byoc/'), "*

 * *         "('BYOS_ENV', 'https://frontend.apps.cfa.devcloud.intel.com/byos/'), ('EDGENODE_ENV', "*

 * *         "'https://frontend.apps.cfa.devcloud.intel.com/edgenode/'), ('EXECUTION_ENV', "*

 * *         "'https://frontend.apps.cfa.devcloud.intel.com/execution/'), ('CONFIG_ENV', "*

 * *         "'https://frontend.apps.cfa.devcloud.intel.com/config/')])",*

 * * "'PRC'": "OrderedDict([('BYOC_ENV', "*

 * *          "'https://frontend-devcloud […]*

```diff
@@ -1,15 +1,22 @@
 {
-    "PROD": {
+    "CP": {
         "BYOC_ENV": "https://frontend.apps.cfa.devcloud.intel.com/byoc/",
         "BYOS_ENV": "https://frontend.apps.cfa.devcloud.intel.com/byos/",
         "CONFIG_ENV": "https://frontend.apps.cfa.devcloud.intel.com/config/",
         "EDGENODE_ENV": "https://frontend.apps.cfa.devcloud.intel.com/edgenode/",
         "EXECUTION_ENV": "https://frontend.apps.cfa.devcloud.intel.com/execution/"
     },
+    "PRC": {
+        "BYOC_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/byoc/",
+        "BYOS_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/byos/",
+        "CONFIG_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/config/",
+        "EDGENODE_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/edgenode/",
+        "EXECUTION_ENV": "https://frontend-devcloud-prc.apps.prc.cfa.devcloud.intel.cn/execution/"
+    },
     "endPoints": {
         "configuration": "api/v1/container/createConfiguration",
         "containers": "api/v1/containers",
         "deleteBuild": "api/v1/s2i/user/deleteBuild/{}",
         "deployMultipleHardware": "api/v1/containers/deploy-multi-hardware",
         "edgenode": "api/v1/edge-node/edges",
         "log": "api/v1/logs/pod?podName={}",
```

## Comparing `devcloud-2023.3.1.dist-info/LICENSE` & `devcloud-2023.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `devcloud-2023.3.1.dist-info/METADATA` & `devcloud-2023.4.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcloud
-Version: 2023.3.1
+Version: 2023.4.2
 Summary: Intel® Devcloud - Developer Cloud for the Edge Python library
 Home-page: https://github.com/intel/DevCloudContent-git
 License: OSI Approved :: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -116,15 +116,15 @@
 ```
 pip install devcloud -i https://mirrors.aliyun.com/pypi/simple/
 ```
 Use the ```--trusted-host``` parameter if the URL above is http instead of https.
 ## List of API
 | Method |  Description | Parameters |  Return
 |---|---|---|---|
-| Devcloud.connect | Validates the token and gives the snapshot of Dashboard and Project deployed by the user | token: str(Optional) API Token of the user, if not provided then will be prompted  | None |
+| Devcloud.connect | Validates the token and gives the snapshot of Dashboard and Project deployed by the user | token: str(Optional) API Token of the user, if not provided then will be prompted <br> env: str - Name of the environment, default is "CP" which connects to container playground and for user's of PRC region please use "PRC"  | None |
 | Devcloud.transfer | Transfers file from Cloud storage like AWS S3 to Devcloud  |region: str - AWS bucket region<br>bucketName: str - Name of the bucket<br>path: str - file/folder path present relative to the bucket to be copied to devcloud<br>accessKey: str (Optional) - Access key of AWS S3 bucket<br>secretKey: str (Optional) - Secret key of AWS S3 bucket | None |
 | Devcloud.availableHardware | Prints available hardware and their respective ID, Processor Name, Integrated GPU Name and Memory detail | None | None |
 | Devcloud.createContainer | Creates container image and stores in the devcloud |projectName: str - Unique name of the project<br>containerName: str - Unique name of the container<br>url: str - Container image URL | None |
 | Devcloud.configureContainer | Configures the container with various option as mentioned in parameters | projectName: str - Name of the project under which container present<br>containerName: str - Name of the container which needs to configured (This should be assigned to the project name mentioned above)<br>port: list[int] - Port number which must be exposed to external consumption. Port range must be above 1024<br>label: list[str] - Label to be associated to the container<br>entryScript: str - Initial file which must be executed when container boots up<br>output: str - Output mount folder, which can be later accessed using Devcloud file system<br>mountPoint: list[(str, str)] - To mount Devcloud file system to user's container. This is a tuple, were first one is for Devcloud file system path and second is mount point in container. Multiple such mount path can be assigned<br>environment: str - environment variable to be passed to container. eg., -e token=XYZ  | None |
 | Devcloud.launch | Launches the Project against the selected hardward | projectName: str - Name of the project which should be lauched<br>edgeNode: int - Intel's latest and greatest hardware to be used. Get the list by calling Devcloud.availableHardware() | None |
 | Devcloud.getStatus  | Displays launched project status | projectName: str (Optional) If provided will show dashboard detail of the project<br> output: str (Optional) if value is wide then provided additional detail such as Performance and create time  | None |
 | Devcloud.getFilesPreview  | Gets the response object of the requested file path in the Devcloud's filesystem | projectName: str - Name of the project<br>path: str - Relative path from the project's output folder<br> edgeNode: str (Optional) - Intel processor used, if not provided then latest completed container's in the specified project will be used<br> createTime: str (Optional) - If present then this timestamp is used to retrieve the files present under the given runtime of the container<br> | _io.BytesIO |
```

