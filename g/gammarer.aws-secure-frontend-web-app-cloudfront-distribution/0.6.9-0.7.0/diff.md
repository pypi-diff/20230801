# Comparing `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9.tar.gz` & `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9.tar", last modified: Thu Jul 27 18:27:38 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0.tar", last modified: Tue Aug  1 04:35:11 2023, max compression
```

## Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9.tar` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:27:38.240731 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-27 18:27:38.240731 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:27:38.240731 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:27:38.236731 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:27:38.236731 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:27:38.236731 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:27:38.240731 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.6.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:27:26.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:27:38.236731 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-27 18:27:38.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-27 18:27:38.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:27:38.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 18:27:38.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 18:27:38.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:35:11.119762 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-01 04:35:11.119762 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:35:11.119762 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:35:11.115762 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:35:11.115762 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:35:11.119762 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:35:11.119762 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:34:55.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:35:11.119762 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-01 04:35:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-01 04:35:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:35:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 04:35:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 04:35:11.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/LICENSE` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 0.6.9
+Version: 0.7.0
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -40,23 +40,20 @@
 
 ```shell
 pip install gammarer.aws-secure-frontend-web-app-cloudfront-distribution
 ```
 
 ## Example
 
-```shell
-npm install @gammarer/aws-secure-frontend-web-app-cloudfront-distribution
-```
-
 ```python
 import { SecureFrontendWebAppCloudFrontDistribution } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
 
 new SecureFrontendWebAppCloudFrontDistribution(stack, 'SecureFrontendWebAppCloudFrontDistribution', {
-  accessLogBucket: new s3.Bucket(stack, 'LogBucket'),
+  comment: 'frontend web app distribution.', // optional
+  accessLogBucket: new s3.Bucket(stack, 'LogBucket'), // optional
   certificate: new acm.Certificate(stack, 'Certificate', {
     domainName: 'example.com',
   }),
   distributionDomainName: 'example.com',
   originAccessIdentity: new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity'),
   originBucket: new s3.Bucket(stack, 'OriginBucket'),
 });
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/README.md` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,20 @@
 
 ```shell
 pip install gammarer.aws-secure-frontend-web-app-cloudfront-distribution
 ```
 
 ## Example
 
-```shell
-npm install @gammarer/aws-secure-frontend-web-app-cloudfront-distribution
-```
-
 ```python
 import { SecureFrontendWebAppCloudFrontDistribution } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
 
 new SecureFrontendWebAppCloudFrontDistribution(stack, 'SecureFrontendWebAppCloudFrontDistribution', {
-  accessLogBucket: new s3.Bucket(stack, 'LogBucket'),
+  comment: 'frontend web app distribution.', // optional
+  accessLogBucket: new s3.Bucket(stack, 'LogBucket'), // optional
   certificate: new acm.Certificate(stack, 'Certificate', {
     domainName: 'example.com',
   }),
   distributionDomainName: 'example.com',
   originAccessIdentity: new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity'),
   originBucket: new s3.Bucket(stack, 'OriginBucket'),
 });
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/setup.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-frontend-web-app-cloudfront-distribution",
-    "version": "0.6.9",
+    "version": "0.7.0",
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution",
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii": [
-            "aws-secure-frontend-web-app-cloudfront-distribution@0.6.9.jsii.tgz"
+            "aws-secure-frontend-web-app-cloudfront-distribution@0.7.0.jsii.tgz"
         ],
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,23 +17,20 @@
 
 ```shell
 pip install gammarer.aws-secure-frontend-web-app-cloudfront-distribution
 ```
 
 ## Example
 
-```shell
-npm install @gammarer/aws-secure-frontend-web-app-cloudfront-distribution
-```
-
 ```python
 import { SecureFrontendWebAppCloudFrontDistribution } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
 
 new SecureFrontendWebAppCloudFrontDistribution(stack, 'SecureFrontendWebAppCloudFrontDistribution', {
-  accessLogBucket: new s3.Bucket(stack, 'LogBucket'),
+  comment: 'frontend web app distribution.', // optional
+  accessLogBucket: new s3.Bucket(stack, 'LogBucket'), // optional
   certificate: new acm.Certificate(stack, 'Certificate', {
     domainName: 'example.com',
   }),
   distributionDomainName: 'example.com',
   originAccessIdentity: new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity'),
   originBucket: new s3.Bucket(stack, 'OriginBucket'),
 });
@@ -65,103 +62,98 @@
     jsii_type="@gammarer/aws-secure-frontend-web-app-cloudfront-distribution.SecureFrontendWebAppCloudFrontDistribution",
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        access_log_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
         certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
         domain_name: builtins.str,
         origin_access_identity: _aws_cdk_aws_cloudfront_ceddda9d.IOriginAccessIdentity,
         origin_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        access_log_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         comment: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
-        :param access_log_bucket: 
         :param certificate: 
         :param domain_name: 
         :param origin_access_identity: 
         :param origin_bucket: 
+        :param access_log_bucket: 
         :param comment: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ab68d83b630cc02546d77e48c8646f50b0e2f872bcc124abfd93eb26fa3bfc75)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = SecureFrontendWebAppCloudFrontDistributionProps(
-            access_log_bucket=access_log_bucket,
             certificate=certificate,
             domain_name=domain_name,
             origin_access_identity=origin_access_identity,
             origin_bucket=origin_bucket,
+            access_log_bucket=access_log_bucket,
             comment=comment,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
 @jsii.data_type(
     jsii_type="@gammarer/aws-secure-frontend-web-app-cloudfront-distribution.SecureFrontendWebAppCloudFrontDistributionProps",
     jsii_struct_bases=[],
     name_mapping={
-        "access_log_bucket": "accessLogBucket",
         "certificate": "certificate",
         "domain_name": "domainName",
         "origin_access_identity": "originAccessIdentity",
         "origin_bucket": "originBucket",
+        "access_log_bucket": "accessLogBucket",
         "comment": "comment",
     },
 )
 class SecureFrontendWebAppCloudFrontDistributionProps:
     def __init__(
         self,
         *,
-        access_log_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
         certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
         domain_name: builtins.str,
         origin_access_identity: _aws_cdk_aws_cloudfront_ceddda9d.IOriginAccessIdentity,
         origin_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        access_log_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         comment: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param access_log_bucket: 
         :param certificate: 
         :param domain_name: 
         :param origin_access_identity: 
         :param origin_bucket: 
+        :param access_log_bucket: 
         :param comment: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__46fcd4037c1afe9dd0632bd9133c92d55839ac1c45b0d25a564b359716dceb26)
-            check_type(argname="argument access_log_bucket", value=access_log_bucket, expected_type=type_hints["access_log_bucket"])
             check_type(argname="argument certificate", value=certificate, expected_type=type_hints["certificate"])
             check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
             check_type(argname="argument origin_access_identity", value=origin_access_identity, expected_type=type_hints["origin_access_identity"])
             check_type(argname="argument origin_bucket", value=origin_bucket, expected_type=type_hints["origin_bucket"])
+            check_type(argname="argument access_log_bucket", value=access_log_bucket, expected_type=type_hints["access_log_bucket"])
             check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "access_log_bucket": access_log_bucket,
             "certificate": certificate,
             "domain_name": domain_name,
             "origin_access_identity": origin_access_identity,
             "origin_bucket": origin_bucket,
         }
+        if access_log_bucket is not None:
+            self._values["access_log_bucket"] = access_log_bucket
         if comment is not None:
             self._values["comment"] = comment
 
     @builtins.property
-    def access_log_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
-        result = self._values.get("access_log_bucket")
-        assert result is not None, "Required property 'access_log_bucket' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
-
-    @builtins.property
     def certificate(self) -> _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate:
         result = self._values.get("certificate")
         assert result is not None, "Required property 'certificate' is missing"
         return typing.cast(_aws_cdk_aws_certificatemanager_ceddda9d.ICertificate, result)
 
     @builtins.property
     def domain_name(self) -> builtins.str:
@@ -180,14 +172,19 @@
     @builtins.property
     def origin_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
         result = self._values.get("origin_bucket")
         assert result is not None, "Required property 'origin_bucket' is missing"
         return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
 
     @builtins.property
+    def access_log_bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
+        result = self._values.get("access_log_bucket")
+        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
+
+    @builtins.property
     def comment(self) -> typing.Optional[builtins.str]:
         result = self._values.get("comment")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -207,28 +204,28 @@
 
 publication.publish()
 
 def _typecheckingstub__ab68d83b630cc02546d77e48c8646f50b0e2f872bcc124abfd93eb26fa3bfc75(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    access_log_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
     certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
     domain_name: builtins.str,
     origin_access_identity: _aws_cdk_aws_cloudfront_ceddda9d.IOriginAccessIdentity,
     origin_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    access_log_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
     comment: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__46fcd4037c1afe9dd0632bd9133c92d55839ac1c45b0d25a564b359716dceb26(
     *,
-    access_log_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
     certificate: _aws_cdk_aws_certificatemanager_ceddda9d.ICertificate,
     domain_name: builtins.str,
     origin_access_identity: _aws_cdk_aws_cloudfront_ceddda9d.IOriginAccessIdentity,
     origin_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    access_log_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
     comment: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 0.6.9
+Version: 0.7.0
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -40,23 +40,20 @@
 
 ```shell
 pip install gammarer.aws-secure-frontend-web-app-cloudfront-distribution
 ```
 
 ## Example
 
-```shell
-npm install @gammarer/aws-secure-frontend-web-app-cloudfront-distribution
-```
-
 ```python
 import { SecureFrontendWebAppCloudFrontDistribution } from '@gammarer/aws-secure-frontend-web-app-cloudfront-distribution';
 
 new SecureFrontendWebAppCloudFrontDistribution(stack, 'SecureFrontendWebAppCloudFrontDistribution', {
-  accessLogBucket: new s3.Bucket(stack, 'LogBucket'),
+  comment: 'frontend web app distribution.', // optional
+  accessLogBucket: new s3.Bucket(stack, 'LogBucket'), // optional
   certificate: new acm.Certificate(stack, 'Certificate', {
     domainName: 'example.com',
   }),
   distributionDomainName: 'example.com',
   originAccessIdentity: new cloudfront.OriginAccessIdentity(stack, 'OriginAccessIdentity'),
   originBucket: new s3.Bucket(stack, 'OriginBucket'),
 });
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.9/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.7.0/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
-src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.6.9.jsii.tgz
+src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.7.0.jsii.tgz
```

