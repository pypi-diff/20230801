# Comparing `tmp/b_cfn_lambda_integration-0.0.8.tar.gz` & `tmp/b_cfn_lambda_integration-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/b_cfn_lambda_integration-0.0.8.tar", last modified: Thu Dec 17 14:53:32 2020, max compression
+gzip compressed data, was "b_cfn_lambda_integration-1.0.0.tar", last modified: Tue Aug  1 11:26:05 2023, max compression
```

## Comparing `b_cfn_lambda_integration-0.0.8.tar` & `b_cfn_lambda_integration-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-17 14:53:32.412356 b_cfn_lambda_integration-0.0.8/
--rw-rw-r--   0 root         (0) root         (0)      477 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/HISTORY.md
--rw-rw-r--   0 root         (0) root         (0)    11357 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      118 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1265 2020-12-17 14:53:32.412356 b_cfn_lambda_integration-0.0.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        6 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/README.md
--rw-rw-r--   0 root         (0) root         (0)        5 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-17 14:53:32.412356 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration/
--rw-rw-r--   0 root         (0) root         (0)        0 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2352 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration/lambda_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-17 14:53:32.412356 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1265 2020-12-17 14:53:32.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      543 2020-12-17 14:53:32.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-12-17 14:53:32.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2020-12-17 14:53:32.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       55 2020-12-17 14:53:32.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-17 14:53:32.408356 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration_test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-17 14:53:32.412356 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration_test/integration/
--rw-rw-r--   0 root         (0) root         (0)        0 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration_test/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-17 14:53:32.412356 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration_test/unit/
--rw-rw-r--   0 root         (0) root         (0)        0 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration_test/unit/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      912 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration_test/unit/test_lambda_integration.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-12-17 14:53:32.412356 b_cfn_lambda_integration-0.0.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1265 2020-12-17 14:52:21.000000 b_cfn_lambda_integration-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:26:05.226242 b_cfn_lambda_integration-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      118 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-08-01 11:26:05.226242 b_cfn_lambda_integration-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:26:05.222242 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration/lambda_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:26:05.226242 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-08-01 11:26:05.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      543 2023-08-01 11:26:05.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 11:26:05.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-08-01 11:26:05.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-08-01 11:26:05.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:26:05.222242 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration_test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:26:05.226242 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration_test/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration_test/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:26:05.226242 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration_test/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration_test/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration_test/unit/test_lambda_integration.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 11:26:05.226242 b_cfn_lambda_integration-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-08-01 11:25:30.000000 b_cfn_lambda_integration-1.0.0/setup.py
```

### Comparing `b_cfn_lambda_integration-0.0.8/LICENSE` & `b_cfn_lambda_integration-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_integration-0.0.8/PKG-INFO` & `b_cfn_lambda_integration-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: b_cfn_lambda_integration
-Version: 0.0.8
+Version: 1.0.0
 Summary: AWS CDK based api gateway integration resource that creates a lambda integration as cfn resource.
 Home-page: https://github.com/biomapas/B.CfnLambdaIntegration.git
 Author: Laimonas Sutkus
 Author-email: laimonas.sutkus@biomapas.com
 License: Apache License 2.0
 Description: # TODO
         
         # Release history
         
+        ### 1.0.0
+        * Upgrade CDK support from v1 to v2.
+        * Upgrade GitHub pipelines checkout version.
+        * Upgrade biomapas/cicd-full image version to 5.0.0.
+        
         ### 0.0.8
         * Expose lambda function.
         
         ### 0.0.7
         * Add tests to the pipeline.
         
         ### 0.0.6
```

### Comparing `b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration/lambda_integration.py` & `b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration/lambda_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import hashlib
 from typing import Any, Union
+
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnIntegration
 from aws_cdk.aws_lambda import IFunction, CfnFunction
-from aws_cdk.core import Stack
 
 
 class LambdaIntegration(CfnIntegration):
     def __init__(
             self,
             scope: Stack,
             integration_name: str,
@@ -58,14 +59,14 @@
     @property
     def function(self) -> Union[IFunction, CfnFunction]:
         return self.__lambda_function
 
     @property
     def hash(self):
         hashable = (
-            self.__integration_name +
-            self.__integration_method +
-            self.__integration_type +
-            self.__connection_type
+                self.__integration_name +
+                self.__integration_method +
+                self.__integration_type +
+                self.__connection_type
         ).encode('utf-8')
 
         return hashlib.sha256(hashable).hexdigest()
```

### Comparing `b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration.egg-info/PKG-INFO` & `b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: b-cfn-lambda-integration
-Version: 0.0.8
+Version: 1.0.0
 Summary: AWS CDK based api gateway integration resource that creates a lambda integration as cfn resource.
 Home-page: https://github.com/biomapas/B.CfnLambdaIntegration.git
 Author: Laimonas Sutkus
 Author-email: laimonas.sutkus@biomapas.com
 License: Apache License 2.0
 Description: # TODO
         
         # Release history
         
+        ### 1.0.0
+        * Upgrade CDK support from v1 to v2.
+        * Upgrade GitHub pipelines checkout version.
+        * Upgrade biomapas/cicd-full image version to 5.0.0.
+        
         ### 0.0.8
         * Expose lambda function.
         
         ### 0.0.7
         * Add tests to the pipeline.
         
         ### 0.0.6
```

### Comparing `b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration.egg-info/SOURCES.txt` & `b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_integration-0.0.8/b_cfn_lambda_integration_test/unit/test_lambda_integration.py` & `b_cfn_lambda_integration-1.0.0/b_cfn_lambda_integration_test/unit/test_lambda_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from aws_cdk import Stack, App
 from aws_cdk.aws_apigatewayv2 import CfnApi
 from aws_cdk.aws_lambda import Function, Code, Runtime
-from aws_cdk.core import Stack, App
 
 from b_cfn_lambda_integration.lambda_integration import LambdaIntegration
 
 
 def test_FUNC_hash_WITH_valid_parameters_EXPECT_hash_created():
     """
     Test that hashing is consistent and works as expected.
@@ -18,12 +18,12 @@
         integration_name='TestIntegration',
         api=CfnApi(stack, 'TestApi'),
         lambda_function=Function(
             stack,
             'TestLambdaFunction',
             code=Code.from_inline('def handler(*args, **kwargs): return 123'),
             handler='index.handler',
-            runtime=Runtime.PYTHON_3_6
+            runtime=Runtime.PYTHON_3_10
         )
     )
 
     assert integration.hash == 'ab93cecc508e529c3791ba48a1275deec88cdd6b43a7e1d443906df48fa300e4'
```

### Comparing `b_cfn_lambda_integration-0.0.8/setup.py` & `b_cfn_lambda_integration-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     description=(
         'AWS CDK based api gateway integration resource that creates a lambda integration as cfn resource.'
     ),
     long_description=README + '\n\n' + HISTORY,
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=[
-        "aws-cdk.aws-apigatewayv2>=1.54.0,<2.0.0",
-        'pytest>=6.0.0,<7.0.0',
+        'aws-cdk-lib>=2.0.0,<3.0.0',
+        'aws-cdk-constructs>=2.0.0,<3.0.0'
     ],
     author='Laimonas Sutkus',
     author_email='laimonas.sutkus@biomapas.com',
     keywords='AWS CDK Lambda API Gateway Integration CFN',
     url='https://github.com/biomapas/B.CfnLambdaIntegration.git',
     classifiers=[
         'Programming Language :: Python :: 3',
```

