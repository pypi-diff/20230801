# Comparing `tmp/snowcross-0.0.8.tar.gz` & `tmp/snowcross-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowcross-0.0.8.tar", last modified: Mon Jul 31 08:41:47 2023, max compression
+gzip compressed data, was "snowcross-0.1.0.tar", last modified: Tue Aug  1 01:22:20 2023, max compression
```

## Comparing `snowcross-0.0.8.tar` & `snowcross-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 08:41:24.000000 snowcross-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 08:41:24.000000 snowcross-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 08:41:47.821094 snowcross-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 08:41:24.000000 snowcross-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 08:41:24.000000 snowcross-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 08:41:24.000000 snowcross-0.0.8/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 08:41:24.000000 snowcross-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:41:47.821094 snowcross-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-31 08:41:24.000000 snowcross-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/snowcross/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:24.000000 snowcross-0.0.8/snowcross/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-31 08:41:24.000000 snowcross-0.0.8/snowcross/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 08:41:24.000000 snowcross-0.0.8/snowcross/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-31 08:41:24.000000 snowcross-0.0.8/snowcross/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/snowcross.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/fixtures/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/fixtures/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/helpers/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:22:20.750056 snowcross-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 01:21:55.000000 snowcross-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 01:21:55.000000 snowcross-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 01:22:20.750056 snowcross-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-01 01:21:55.000000 snowcross-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 01:21:55.000000 snowcross-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 01:21:55.000000 snowcross-0.1.0/requirements-locator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 01:21:55.000000 snowcross-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 01:21:55.000000 snowcross-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:22:20.750056 snowcross-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 01:21:55.000000 snowcross-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:22:20.750056 snowcross-0.1.0/snowcross/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:55.000000 snowcross-0.1.0/snowcross/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-08-01 01:21:55.000000 snowcross-0.1.0/snowcross/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 01:21:55.000000 snowcross-0.1.0/snowcross/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-01 01:21:55.000000 snowcross-0.1.0/snowcross/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-08-01 01:21:55.000000 snowcross-0.1.0/snowcross/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:22:20.750056 snowcross-0.1.0/snowcross.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 01:22:20.000000 snowcross-0.1.0/snowcross.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 01:22:20.000000 snowcross-0.1.0/snowcross.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:22:20.000000 snowcross-0.1.0/snowcross.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 01:22:20.000000 snowcross-0.1.0/snowcross.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 01:22:20.000000 snowcross-0.1.0/snowcross.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:22:20.746056 snowcross-0.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:22:20.750056 snowcross-0.1.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:55.000000 snowcross-0.1.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-01 01:21:55.000000 snowcross-0.1.0/tests/fixtures/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-01 01:21:55.000000 snowcross-0.1.0/tests/fixtures/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:22:20.750056 snowcross-0.1.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:55.000000 snowcross-0.1.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-01 01:21:55.000000 snowcross-0.1.0/tests/helpers/docker.py
```

### Comparing `snowcross-0.0.8/LICENSE` & `snowcross-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snowcross-0.0.8/PKG-INFO` & `snowcross-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: snowcross
-Version: 0.0.8
+Version: 0.1.0
 Summary: Adaptors for tools and services in a Snowflake-centric data platform
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: locator
 Provides-Extra: test
 License-File: LICENSE
 
 Adaptors for tools and services in a Snowflake-centric data platform.
 
 ## Requirements
```

### Comparing `snowcross-0.0.8/README.md` & `snowcross-0.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 ## Usage
 
 You can install from [PyPI](https://pypi.org/project/snowcross/):
 
 ```shell
 pip install snowcross
 ```
+
+When using `locator` functionality, install extra dependencies `snowcross[locator]`.
```

### Comparing `snowcross-0.0.8/setup.py` & `snowcross-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     long_description=description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     packages=find_packages(exclude=["tests"]),
     test_suite="tests",
     install_requires=requires_from_file("requirements.txt"),
     extras_require={
+        "locator": requires_from_file("requirements-locator.txt"),
         "test": requires_from_file("requirements-test.txt"),
     },
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `snowcross-0.0.8/snowcross/aws.py` & `snowcross-0.1.0/snowcross/aws.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import logging
+import time
 import re
 import urllib
+from random import randint
 from typing import Any, Dict, Generator, Literal, Optional, Union
 import boto3
 import botocore
-from botocore.response import StreamingBody
+from .errors import WorkflowRunException
 
 logger = logging.getLogger(__name__)
 
 
 def _client(
     service: Union[
         Literal["s3"],
         Literal["ssm"],
         Literal["ecr"],
+        Literal["sts"],
+        Literal["glue"],
     ],
 ) -> Any:
     """Creates a boto3 client for a service with default config.
 
     Args:
         service (str): The service to create a boto3 client for.
 
@@ -45,27 +49,16 @@
         service,
         config=botocore.config.Config(
             retries={"mode": "adaptive"},
         ),
     )
 
 
-def environment_storage_bucket(environment: str, name: str) -> str:
-    """Constructs environment-specific S3 bucket following convention.
-
-    Args:
-        environment (str): Environment name.
-        name (str): Partial bucket name.
-
-    Returns:
-        str: Full bucket name.
-    """
-    account = boto3.client("sts").get_caller_identity().get("Account")
-    region = boto3.session.Session().region_name
-    return f"{environment}-{name}-{account}-{region}"
+def _poll_wait():
+    time.sleep(randint(15, 30))
 
 
 def resolve_parameters(parameters: Dict[str, Optional[str]]) -> Dict[str, Optional[str]]:
     """Retrieves parameters from SSM.
 
     Args:
         parameters (Dict[Union[str, Optional[str]): Parameters by key (only those with ssm prefix are retrieved.)
@@ -82,40 +75,54 @@
             continue
 
         match = re.match(pattern=r"^(boto\+)?ssm:", string=v)
         if match:
             ssm_parameters[v[match.end() :]] = k
 
     if ssm_parameters:
-        client = _client("ssm")
-        resp = client.get_parameters(
+        resp = _client("ssm").get_parameters(
             Names=list(ssm_parameters.keys()),
             WithDecryption=True,
         )
         for p in resp.get("InvalidParameters", []):
             logger.critical("Parameter not found: %s", p)
 
         for p in resp.get("Parameters", []):
             parameters[ssm_parameters[p["Name"]]] = p["Value"]
 
     return parameters
 
 
-def get_storage_object(bucket: str, key: str) -> Optional[StreamingBody]:
+def environment_storage_bucket(environment: str, name: str) -> str:
+    """Constructs environment-specific S3 bucket following convention.
+
+    Args:
+        environment (str): Environment name.
+        name (str): Partial bucket name.
+
+    Returns:
+        str: Full bucket name.
+    """
+    account = _client("sts").get_caller_identity().get("Account")
+    region = boto3.session.Session().region_name
+    return f"{environment}-{name}-{account}-{region}"
+
+
+def get_storage_object(bucket: str, key: str) -> Optional[botocore.response.StreamingBody]:
     """Retrieves body of an object stream from S3.
 
     Args:
         bucket (str): Bucket name.
         key (str): Object key.
 
     Returns:
-        Optional[StreamingBody]: An S3 object body stream or None.
+        Optional[botocore.response.StreamingBody]: An S3 object body stream or None.
     """
     try:
-        s3_object = boto3.client("s3").get_object(Bucket=bucket, Key=key)
+        s3_object = _client("s3").get_object(Bucket=bucket, Key=key)
         return s3_object["Body"]
     except botocore.client.ClientError as ex:
         if ex.response["Error"]["Code"] == "NoSuchKey":
             logger.info("Object %s not found - returning None", key)
             return None
         raise
 
@@ -194,14 +201,38 @@
     parsed = urllib.parse.urlparse(url)
     if parsed.scheme in ("s3", "s3a"):
         obj["bucket"] = parsed.netloc
         obj["key"] = parsed.path.lstrip("/")
     return obj
 
 
+def run_workflow(name: str):
+    """Executes Glue workflow and waits for completion.
+
+    Args:
+        name (str): Workflow name.
+    """
+    glue = _client("glue")
+    start_workflow = glue.start_workflow_run(Name=name)
+    while True:
+        _poll_wait()
+        try:
+            workflow_run_resp = glue.get_workflow_run(
+                Name=name,
+                RunId=start_workflow.get("RunId"),
+            )
+            state = workflow_run_resp.get("Run").get("Status")
+        except glue.exceptions.ThrottlingException:
+            continue
+        if state == "COMPLETED":
+            break
+        if state not in ("RUNNING", "STOPPING"):
+            raise WorkflowRunException(f"get_workflow_run returned: {state}")
+
+
 def latest_image_version(registry_id: str, repository_name: str) -> str:
     """Gets the latest image version from ECR.
 
     Args:
         registry_id (str): The ECR registry id.
         repository_name (str): The ECR repository name.
```

### Comparing `snowcross-0.0.8/snowcross.egg-info/PKG-INFO` & `snowcross-0.1.0/snowcross.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: snowcross
-Version: 0.0.8
+Version: 0.1.0
 Summary: Adaptors for tools and services in a Snowflake-centric data platform
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: locator
 Provides-Extra: test
 License-File: LICENSE
 
 Adaptors for tools and services in a Snowflake-centric data platform.
 
 ## Requirements
```

### Comparing `snowcross-0.0.8/tests/fixtures/aws.py` & `snowcross-0.1.0/tests/fixtures/aws.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.0.8/tests/fixtures/snowflake.py` & `snowcross-0.1.0/tests/fixtures/snowflake.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.0.8/tests/helpers/docker.py` & `snowcross-0.1.0/tests/helpers/docker.py`

 * *Files identical despite different names*

