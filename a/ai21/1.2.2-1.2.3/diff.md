# Comparing `tmp/ai21-1.2.2.tar.gz` & `tmp/ai21-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-1.2.2.tar", last modified: Mon Jul 24 10:32:09 2023, max compression
+gzip compressed data, was "ai21-1.2.3.tar", last modified: Tue Aug  1 11:02:07 2023, max compression
```

## Comparing `ai21-1.2.2.tar` & `ai21-1.2.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.142168 ai21-1.2.2/
--rw-r--r--   0 haimon     (501) staff       (20)     1065 2023-07-24 08:05:55.000000 ai21-1.2.2/LICENSE
--rw-r--r--   0 haimon     (501) staff       (20)     4577 2023-07-24 10:32:09.142324 ai21-1.2.2/PKG-INFO
--rw-r--r--   0 haimon     (501) staff       (20)     3595 2023-07-24 08:05:55.000000 ai21-1.2.2/README.md
-drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.127043 ai21-1.2.2/ai21/
--rw-r--r--   0 haimon     (501) staff       (20)     2317 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/AWS_utils.py
--rw-r--r--   0 haimon     (501) staff       (20)      919 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/__init__.py
--rw-r--r--   0 haimon     (501) staff       (20)      971 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/ai21_object.py
--rw-r--r--   0 haimon     (501) staff       (20)     2055 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/ai21_studio_client.py
--rw-r--r--   0 haimon     (501) staff       (20)      473 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/api_resources.py
--rw-r--r--   0 haimon     (501) staff       (20)     2195 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/bedrock_client.py
--rw-r--r--   0 haimon     (501) staff       (20)      250 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/constants.py
--rw-r--r--   0 haimon     (501) staff       (20)     3273 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/errors.py
--rw-r--r--   0 haimon     (501) staff       (20)     4034 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/http_client.py
-drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.133197 ai21-1.2.2/ai21/modules/
--rw-r--r--   0 haimon     (501) staff       (20)        0 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/__init__.py
--rw-r--r--   0 haimon     (501) staff       (20)     1993 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/completion.py
--rw-r--r--   0 haimon     (501) staff       (20)      856 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/custom_model.py
--rw-r--r--   0 haimon     (501) staff       (20)      658 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/dataset.py
--rw-r--r--   0 haimon     (501) staff       (20)      534 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/destination.py
--rw-r--r--   0 haimon     (501) staff       (20)     1740 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/experimental.py
--rw-r--r--   0 haimon     (501) staff       (20)      970 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/gec.py
--rw-r--r--   0 haimon     (501) staff       (20)      925 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/improvements.py
--rw-r--r--   0 haimon     (501) staff       (20)     1463 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/library.py
--rw-r--r--   0 haimon     (501) staff       (20)      984 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/paraphrase.py
--rw-r--r--   0 haimon     (501) staff       (20)     1088 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/question_answering.py
-drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.141720 ai21-1.2.2/ai21/modules/resources/
--rw-r--r--   0 haimon     (501) staff       (20)        0 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/__init__.py
--rw-r--r--   0 haimon     (501) staff       (20)      585 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 haimon     (501) staff       (20)      371 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 haimon     (501) staff       (20)      395 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/deletable_resource.py
--rw-r--r--   0 haimon     (501) staff       (20)     1793 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/execution_utils.py
--rw-r--r--   0 haimon     (501) staff       (20)      352 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 haimon     (501) staff       (20)     2059 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 haimon     (501) staff       (20)      391 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 haimon     (501) staff       (20)      404 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/updatable_resource.py
--rw-r--r--   0 haimon     (501) staff       (20)      480 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/resources/uploadable_resource.py
--rw-r--r--   0 haimon     (501) staff       (20)      915 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/segmentation.py
--rw-r--r--   0 haimon     (501) staff       (20)     1148 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/summarize.py
--rw-r--r--   0 haimon     (501) staff       (20)      693 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/modules/tokenization.py
--rw-r--r--   0 haimon     (501) staff       (20)     3038 2023-07-24 08:05:55.000000 ai21-1.2.2/ai21/utils.py
--rw-r--r--   0 haimon     (501) staff       (20)       22 2023-07-24 10:13:17.000000 ai21-1.2.2/ai21/version.py
-drwxr-xr-x   0 haimon     (501) staff       (20)        0 2023-07-24 10:32:09.129269 ai21-1.2.2/ai21.egg-info/
--rw-r--r--   0 haimon     (501) staff       (20)     4577 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/PKG-INFO
--rw-r--r--   0 haimon     (501) staff       (20)     1188 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 haimon     (501) staff       (20)        1 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/dependency_links.txt
--rw-r--r--   0 haimon     (501) staff       (20)       50 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/requires.txt
--rw-r--r--   0 haimon     (501) staff       (20)        5 2023-07-24 10:32:09.000000 ai21-1.2.2/ai21.egg-info/top_level.txt
--rwxr-xr-x   0 haimon     (501) staff       (20)      155 2023-07-24 10:32:09.142671 ai21-1.2.2/setup.cfg
--rwxr-xr-x   0 haimon     (501) staff       (20)      613 2023-07-24 08:05:55.000000 ai21-1.2.2/setup.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-08-01 11:02:07.044983 ai21-1.2.3/
+-rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.2.3/LICENSE
+-rw-r--r--   0 etang      (501) staff       (20)     4577 2023-08-01 11:02:07.045158 ai21-1.2.3/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     3595 2023-06-11 11:49:53.000000 ai21-1.2.3/README.md
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-08-01 11:02:07.035195 ai21-1.2.3/ai21/
+-rw-r--r--   0 etang      (501) staff       (20)     3068 2023-08-01 09:17:46.000000 ai21-1.2.3/ai21/AWS_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      964 2023-08-01 09:17:46.000000 ai21-1.2.3/ai21/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.2.3/ai21/ai21_object.py
+-rw-r--r--   0 etang      (501) staff       (20)     2055 2023-06-07 10:54:53.000000 ai21-1.2.3/ai21/ai21_studio_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      517 2023-08-01 09:17:46.000000 ai21-1.2.3/ai21/api_resources.py
+-rw-r--r--   0 etang      (501) staff       (20)     2195 2023-06-11 11:49:53.000000 ai21-1.2.3/ai21/bedrock_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      404 2023-08-01 09:17:46.000000 ai21-1.2.3/ai21/constants.py
+-rw-r--r--   0 etang      (501) staff       (20)     3535 2023-08-01 09:17:46.000000 ai21-1.2.3/ai21/errors.py
+-rw-r--r--   0 etang      (501) staff       (20)     4034 2023-06-09 06:49:33.000000 ai21-1.2.3/ai21/http_client.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-08-01 11:02:07.041605 ai21-1.2.3/ai21/modules/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.2.3/ai21/modules/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)     1993 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/completion.py
+-rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.2.3/ai21/modules/custom_model.py
+-rw-r--r--   0 etang      (501) staff       (20)      658 2023-07-31 10:21:52.000000 ai21-1.2.3/ai21/modules/dataset.py
+-rw-r--r--   0 etang      (501) staff       (20)      534 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/destination.py
+-rw-r--r--   0 etang      (501) staff       (20)     1740 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/experimental.py
+-rw-r--r--   0 etang      (501) staff       (20)      970 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/gec.py
+-rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-07 10:54:53.000000 ai21-1.2.3/ai21/modules/improvements.py
+-rw-r--r--   0 etang      (501) staff       (20)     1463 2023-07-31 10:21:52.000000 ai21-1.2.3/ai21/modules/library.py
+-rw-r--r--   0 etang      (501) staff       (20)      984 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/paraphrase.py
+-rw-r--r--   0 etang      (501) staff       (20)     1088 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/question_answering.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-08-01 11:02:07.044725 ai21-1.2.3/ai21/modules/resources/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.2.3/ai21/modules/resources/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.2.3/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.2.3/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      395 2023-07-31 10:21:52.000000 ai21-1.2.3/ai21/modules/resources/deletable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     1793 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/resources/execution_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.2.3/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-07 10:54:53.000000 ai21-1.2.3/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 etang      (501) staff       (20)      391 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      404 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/resources/updatable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      480 2023-07-31 10:21:52.000000 ai21-1.2.3/ai21/modules/resources/uploadable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      239 2023-08-01 09:17:46.000000 ai21-1.2.3/ai21/modules/sagemaker.py
+-rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-07 10:54:53.000000 ai21-1.2.3/ai21/modules/segmentation.py
+-rw-r--r--   0 etang      (501) staff       (20)     1148 2023-07-20 11:53:08.000000 ai21-1.2.3/ai21/modules/summarize.py
+-rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-07 10:54:53.000000 ai21-1.2.3/ai21/modules/tokenization.py
+-rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-09 06:54:03.000000 ai21-1.2.3/ai21/utils.py
+-rw-r--r--   0 etang      (501) staff       (20)       22 2023-08-01 09:17:46.000000 ai21-1.2.3/ai21/version.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-08-01 11:02:07.036523 ai21-1.2.3/ai21.egg-info/
+-rw-r--r--   0 etang      (501) staff       (20)     4577 2023-08-01 11:02:06.000000 ai21-1.2.3/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     1214 2023-08-01 11:02:07.000000 ai21-1.2.3/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 etang      (501) staff       (20)        1 2023-08-01 11:02:06.000000 ai21-1.2.3/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 etang      (501) staff       (20)       50 2023-08-01 11:02:06.000000 ai21-1.2.3/ai21.egg-info/requires.txt
+-rw-r--r--   0 etang      (501) staff       (20)        5 2023-08-01 11:02:06.000000 ai21-1.2.3/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-08-01 11:02:07.045567 ai21-1.2.3/setup.cfg
+-rwxr-xr-x   0 etang      (501) staff       (20)      613 2023-07-20 11:53:08.000000 ai21-1.2.3/setup.py
```

### Comparing `ai21-1.2.2/LICENSE` & `ai21-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/PKG-INFO` & `ai21-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.2.2
+Version: 1.2.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
```

### Comparing `ai21-1.2.2/README.md` & `ai21-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/AWS_utils.py` & `ai21-1.2.3/ai21/AWS_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
 import re
 from typing import Optional
 
 import boto3
+import requests
 import sagemaker
 from botocore.exceptions import ClientError
 
 import ai21
-from ai21.errors import ServerError, ServiceUnavailable, BadRequest, APIError
+from ai21.constants import SAGEMAKER_MODEL_PACKAGE_NAMES
+from ai21.errors import ServerError, ServiceUnavailable, BadRequest, APIError, ModelPackageDoesntExistException
 from ai21.http_client import handle_non_success_response
 from ai21.utils import convert_to_ai21_object, log_error
 
+MODEL_PACKAGE_URL_FORMAT = 'https://raw.githubusercontent.com/AI21Labs/SageMaker/master/versions/{model_name}/latest.json'
+
 sm_runtime = boto3.client("sagemaker-runtime", region_name=ai21.aws_region)
 
 
 def invoke_sm_endpoint(endpoint_name: str, input_json: str, sm_session: Optional[sagemaker.session.Session]):
     sm_session = sm_session if sm_session else sm_runtime
 
     try:
@@ -49,7 +53,22 @@
         model_error_message = error_message_template.search(error_message).group(2)
         handle_non_success_response(model_status_code, model_error_message)
     if status_code == 429 or status_code == 503:
         raise ServiceUnavailable(details=error_message)
     if status_code == 500:
         raise ServerError(details=error_message)
     raise APIError(status_code, details=error_message)
+
+
+def get_model_package_arn(model_name: str, region: str) -> str:
+    if model_name not in SAGEMAKER_MODEL_PACKAGE_NAMES:
+        raise ModelPackageDoesntExistException(model_name=model_name, region=region)
+
+    response = requests.get(MODEL_PACKAGE_URL_FORMAT.format(model_name=model_name))
+    response.raise_for_status()
+
+    model_package_id = response.json().get(region)
+
+    if not model_package_id:
+        raise ModelPackageDoesntExistException(model_name=model_name, region=region)
+
+    return model_package_id
```

### Comparing `ai21-1.2.2/ai21/__init__.py` & `ai21-1.2.3/ai21/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ai21.modules.custom_model import CustomModel
 from ai21.modules.experimental import Experimental
 from ai21.modules.paraphrase import Paraphrase
 from ai21.modules.summarize import Summarize
 from ai21.modules.segmentation import Segmentation
 from ai21.modules.improvements import Improvements
 from ai21.modules.question_answering import Answer
+from ai21.modules.sagemaker import SageMaker
 from ai21.modules.library import Library
 from ai21.modules.gec import GEC
 from ai21.modules.destination import BedrockDestination, AI21Destination, BedrockModelID, SageMakerDestination
 
 
 api_key = None
 organization = None
```

### Comparing `ai21-1.2.2/ai21/ai21_object.py` & `ai21-1.2.3/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/ai21_studio_client.py` & `ai21-1.2.3/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/bedrock_client.py` & `ai21-1.2.3/ai21/bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/errors.py` & `ai21-1.2.3/ai21/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,7 +94,14 @@
 
 
 class NoSpecifiedRegionException(AI21ClientException):
     def __init__(self):
         message = 'No AWS region provided'
         super().__init__(message)
         self.message = message
+
+
+class ModelPackageDoesntExistException(AI21ClientException):
+    def __init__(self, model_name: str, region: str):
+        message = f"model_name: {model_name} doesn't exist in region: {region}"
+        super().__init__(message)
+        self.message = message
```

### Comparing `ai21-1.2.2/ai21/http_client.py` & `ai21-1.2.3/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/completion.py` & `ai21-1.2.3/ai21/modules/completion.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/custom_model.py` & `ai21-1.2.3/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/dataset.py` & `ai21-1.2.3/ai21/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/destination.py` & `ai21-1.2.3/ai21/modules/destination.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/experimental.py` & `ai21-1.2.3/ai21/modules/experimental.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/gec.py` & `ai21-1.2.3/ai21/modules/gec.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/improvements.py` & `ai21-1.2.3/ai21/modules/improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/library.py` & `ai21-1.2.3/ai21/modules/library.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/paraphrase.py` & `ai21-1.2.3/ai21/modules/paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/question_answering.py` & `ai21-1.2.3/ai21/modules/question_answering.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/resources/ai21_module.py` & `ai21-1.2.3/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/resources/execution_utils.py` & `ai21-1.2.3/ai21/modules/resources/execution_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/resources/nlp_task.py` & `ai21-1.2.3/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/segmentation.py` & `ai21-1.2.3/ai21/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/summarize.py` & `ai21-1.2.3/ai21/modules/summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/modules/tokenization.py` & `ai21-1.2.3/ai21/modules/tokenization.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21/utils.py` & `ai21-1.2.3/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.2.2/ai21.egg-info/PKG-INFO` & `ai21-1.2.3/ai21.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.2.2
+Version: 1.2.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
```

### Comparing `ai21-1.2.2/ai21.egg-info/SOURCES.txt` & `ai21-1.2.3/ai21.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ai21/modules/destination.py
 ai21/modules/experimental.py
 ai21/modules/gec.py
 ai21/modules/improvements.py
 ai21/modules/library.py
 ai21/modules/paraphrase.py
 ai21/modules/question_answering.py
+ai21/modules/sagemaker.py
 ai21/modules/segmentation.py
 ai21/modules/summarize.py
 ai21/modules/tokenization.py
 ai21/modules/resources/__init__.py
 ai21/modules/resources/ai21_module.py
 ai21/modules/resources/creatable_resource.py
 ai21/modules/resources/deletable_resource.py
```

### Comparing `ai21-1.2.2/setup.py` & `ai21-1.2.3/setup.py`

 * *Files identical despite different names*

