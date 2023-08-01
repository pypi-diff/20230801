# Comparing `tmp/cdk-opinionated-constructs-2.1.4.tar.gz` & `tmp/cdk-opinionated-constructs-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-opinionated-constructs-2.1.4.tar", last modified: Mon Jun  5 22:23:51 2023, max compression
+gzip compressed data, was "cdk-opinionated-constructs-2.1.5.tar", last modified: Tue Aug  1 20:29:35 2023, max compression
```

## Comparing `cdk-opinionated-constructs-2.1.4.tar` & `cdk-opinionated-constructs-2.1.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.846311 cdk-opinionated-constructs-2.1.4/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.1.4/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-06-05 22:23:51.846384 cdk-opinionated-constructs-2.1.4/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    27651 2023-05-22 07:55:27.000000 cdk-opinionated-constructs-2.1.4/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.796326 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4879 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2235 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     8661 2023-04-20 10:19:32.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5811 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/nlb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/rds_instance.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3325 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/s3.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1464 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/sns.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    12369 2023-05-22 07:49:31.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.846041 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       88 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-06-05 22:23:51.000000 cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-06-05 22:23:51.846978 cdk-opinionated-constructs-2.1.4/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      760 2023-06-05 22:23:38.000000 cdk-opinionated-constructs-2.1.4/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.803569 cdk-opinionated-constructs-2.1.4/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.4/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1781 2023-04-20 10:28:48.000000 cdk-opinionated-constructs-2.1.4/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.819347 cdk-opinionated-constructs-2.1.4/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.4/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1012 2022-11-20 14:04:19.000000 cdk-opinionated-constructs-2.1.4/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3241 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.4/test/stacks/lmb_docker_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3590 2022-11-25 10:57:28.000000 cdk-opinionated-constructs-2.1.4/test/stacks/lmb_monitoring_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-04-20 10:37:59.000000 cdk-opinionated-constructs-2.1.4/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/test/stacks/nlb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3290 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.4/test/stacks/rds_mysql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3304 2022-12-24 14:23:29.000000 cdk-opinionated-constructs-2.1.4/test/stacks/rds_postgresql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1630 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.4/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2593 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.4/test/stacks/wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-06-05 22:23:51.840314 cdk-opinionated-constructs-2.1.4/test/unit/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      852 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      685 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1921 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.4/test/unit/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-08-01 20:29:35.993781 cdk-opinionated-constructs-2.1.5/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk-opinionated-constructs-2.1.5/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-08-01 20:29:35.993867 cdk-opinionated-constructs-2.1.5/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27651 2023-05-22 07:55:27.000000 cdk-opinionated-constructs-2.1.5/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-08-01 20:29:35.936531 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       50 2022-11-05 21:10:53.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4883 2023-08-01 20:26:55.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2234 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     8739 2023-08-01 20:22:58.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5806 2023-08-01 20:26:55.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4643 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3325 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/s3.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1487 2023-08-01 20:26:55.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/sns.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    12369 2023-05-22 07:49:31.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-08-01 20:29:35.993467 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      340 2023-08-01 20:29:35.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1221 2023-08-01 20:29:35.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2023-08-01 20:29:35.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       88 2023-08-01 20:29:35.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2023-08-01 20:29:35.000000 cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2023-08-01 20:29:35.994578 cdk-opinionated-constructs-2.1.5/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      760 2023-08-01 20:29:13.000000 cdk-opinionated-constructs-2.1.5/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-08-01 20:29:35.937457 cdk-opinionated-constructs-2.1.5/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.5/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1782 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-08-01 20:29:35.948905 cdk-opinionated-constructs-2.1.5/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.5/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2322 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.5/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1011 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3256 2023-08-01 20:26:54.000000 cdk-opinionated-constructs-2.1.5/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3593 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2810 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2225 2023-01-13 23:20:26.000000 cdk-opinionated-constructs-2.1.5/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3306 2023-08-01 20:26:54.000000 cdk-opinionated-constructs-2.1.5/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3321 2023-08-01 20:26:54.000000 cdk-opinionated-constructs-2.1.5/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1629 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1108 2022-11-22 22:16:47.000000 cdk-opinionated-constructs-2.1.5/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2592 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2023-08-01 20:29:35.987487 cdk-opinionated-constructs-2.1.5/test/unit/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk-opinionated-constructs-2.1.5/test/unit/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1102 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.5/test/unit/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      701 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.5/test/unit/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1100 2022-11-20 20:49:21.000000 cdk-opinionated-constructs-2.1.5/test/unit/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      852 2023-05-19 08:53:43.000000 cdk-opinionated-constructs-2.1.5/test/unit/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      688 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/test/unit/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1923 2023-08-01 20:26:51.000000 cdk-opinionated-constructs-2.1.5/test/unit/test_wafv2_stack.py
```

### Comparing `cdk-opinionated-constructs-2.1.4/LICENSE` & `cdk-opinionated-constructs-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/README.md` & `cdk-opinionated-constructs-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/alb.py` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/alb.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,19 +26,18 @@
         """
         super().__init__(scope, construct_id)
 
     def create_access_logs_bucket(self, bucket_name: str, expiration_days: int) -> s3.Bucket:
         """Create dedicated access logs bucket using opinionated cdk construct
         from cdk-opinionated-constructs.
 
-        :param expiration_days: The number of days after which logs will be deleted
+        :param expiration_days: The number of days after which logs will be deleted is
         :param bucket_name: The name of S3 bucket
         :return: CDK S3 IBucket object
         """
-
         alb_access_logs_bucket_construct = S3Bucket(self, id=f"alb_access_logs_{bucket_name}_construct")
         alb_access_logs_bucket = alb_access_logs_bucket_construct.create_bucket(
             bucket_name=bucket_name, encryption=s3.BucketEncryption.S3_MANAGED
         )
 
         alb_access_logs_bucket.add_to_resource_policy(
             permission=iam.PolicyStatement(
@@ -56,15 +55,15 @@
                 actions=["s3:GetBucketAcl"],
                 principals=[iam.ServicePrincipal(service="delivery.logs.amazonaws.com")],
                 resources=[alb_access_logs_bucket.bucket_arn],
             )
         )
         alb_access_logs_bucket.add_lifecycle_rule(expiration=cdk.Duration.days(expiration_days))
 
-        # Supress few false positive alerts from the cfn-nag
+        # Supress a few false positive alerts from the cfn-nag
         NagSuppressions.add_resource_suppressions(
             alb_access_logs_bucket,
             [
                 {
                     "id": "AwsSolutions-S1",
                     "reason": "ALB access logs location, doesn't contain sensitive data"
                     "it doesn't require another resource for storing access logs from it",
```

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/ecr.py` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/ecr.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     ) -> ecr.Repository:
         """
         Create ecr repository with default lifecycle rule - max image count 10, tag immutability and image scan on push
         :param removal_policy: The type of removal policy to be applied when cloudformation stack will be deleted.
         If "retain" then ECR repository will not be deleted.
         :param repository_name: The name of the repository
         :param kwargs:
-            * max_image_age: int - the amount of days  an image can be stored in the repository before it expires.
-            * max_image_count: int - the amount of images to be stored, older images will be deleted.
-            max_image_age and max_image_count are mutually exclusive
+            * Max_image_age: int - the amount of days an image can be stored in the repository before it expires.
+            * Max_image_count: int - the number of images to be stored, older images will be deleted.
+            Max_image_age and max_image_count are mutually exclusive
         """
 
         removal_policy_map = {"retain": cdk.RemovalPolicy.RETAIN, "destroy": cdk.RemovalPolicy.DESTROY}
 
         max_image_age = None
         max_image_count = None
```

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/lmb.py` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/lmb.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         )
 
         return lmb.CodeSigningConfig(self, "conde-signing-config", signing_profiles=[profile])
 
     def create_lambda_layer(self, code_path: str, construct_id: str = "supporting_libraries") -> lmb.LayerVersion:
         """Create lambda layer.
 
-        :param code_path: path which contain lambda layer directory
+        :param code_path: path which contains lambda layer directory
         :param construct_id: construct id
         :return: Lambda layer
         """
         return lmb.LayerVersion(
             self,
             id=construct_id,
             code=lmb.Code.from_asset(code_path),
@@ -72,46 +72,50 @@
         handler: str = "handler.handler",
         signing_config: Union[lmb.ICodeSigningConfig, None] = None,
         **kwargs,
     ) -> lmb.Function:
         """Create lambda function.
 
         :param architecture: Lambda CPU architecture, default ARM_64
-        :param code_path: path which contain lambda function directory
+        :param code_path: path which contains lambda function directory
         :param env: The CDK Environment object which consist region and aws account id
         :param env_variables: Dictionary which contain additional lambda env variables
         :param function_name: The name of lambda function
         :param handler: Lambda handler, default handler.handler
         :param layers: Contains list of lambda layer objects
         :param memory_size: Lambda memory size, default 256MB
         :param reserved_concurrent_executions: The number of max concurrent lambda executions
         :param signing_config: Contains signing config for lambda, default None
         :param timeout: Lambda timeout in seconds,
         :param kwargs:
-            * security_groups - list of ec2.SecurityGroup, the vpc security groups to be assigned to lambda function
+            * Security_groups - list of ec2.SecurityGroup, the vpc security groups to be assigned to lambda function
             * vpc - the ec2.IVpc object, lambda will be assigned to this VPC
-            * vpc_subnets - ec2.SubnetSelection, in which subnets lambda will operate
+            * vpc_subnets - ec2.SubnetSelection, in which subnet lambda will operate
         :return: Lambda function
         """
         lambda_environment_default_variables = {
             "CLOUDWATCH_SAMPLING_RATE": "1",
             "REGION_NAME": env.region,
         }
         return lmb.Function(
             self,
             architecture=architecture,
             code=lmb.Code.from_asset(code_path),
             code_signing_config=signing_config,
-            environment={**lambda_environment_default_variables, **env_variables},
+            environment=lambda_environment_default_variables | env_variables,
             function_name=function_name,
             filesystem=kwargs.get("filesystem"),
             handler=handler,
             id=function_name,
             initial_policy=[
-                iam.PolicyStatement(effect=iam.Effect.ALLOW, actions=["logs:CreateLogGroup"], resources=["*"]),
+                iam.PolicyStatement(
+                    effect=iam.Effect.ALLOW,
+                    actions=["logs:CreateLogGroup"],
+                    resources=["*"],
+                ),
                 iam.PolicyStatement(
                     effect=iam.Effect.ALLOW,
                     actions=["logs:CreateLogStream", "logs:PutLogEvents"],
                     resources=["arn:aws:logs:*:*:log-group:/aws/lambda-insights:*"],
                 ),
             ],
             layers=layers,
@@ -157,24 +161,24 @@
         memory_size: int = 256,
         **kwargs,
     ) -> lmb.Function:
         """Create lambda function.
 
         :param architecture: Lambda CPU architecture, default ARM_64
         :param code: The AWS CDK lmb.Code object
-        :param env: The CDK Environment object which consist region and aws account id
+        :param env: The CDK Environment object which consists of region and aws account id
         :param env_variables: Dictionary which contain additional lambda env variables
         :param function_name: The name of lambda function
         :param memory_size: Lambda memory size, default 256MB
         :param reserved_concurrent_executions: The number of max concurrent lambda executions
         :param timeout: Lambda timeout in seconds
         :param kwargs:
-            * security_groups - list of ec2.SecurityGroup, the vpc security groups to be assigned to lambda function
+            * Security_groups - list of ec2.SecurityGroup, the vpc security groups to be assigned to lambda function
             * vpc - the ec2.IVpc object, lambda will be assigned to this VPC
-            * vpc_subnets - ec2.SubnetSelection, in which subnets lambda will operate
+            * vpc_subnets - ec2.SubnetSelection, in which subnet lambda will operate
             * ephemeral_storage_size - The size of the function’s /tmp directory in MiB. Default: 512 MiB
         :return: Lambda function
         """
         lambda_environment_default_variables = {
             "CLOUDWATCH_SAMPLING_RATE": "1",
             "REGION_NAME": env.region,
         }
```

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/nlb.py` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/nlb.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,18 @@
         """
         super().__init__(scope, construct_id)
 
     def create_access_logs_bucket(self, bucket_name: str, expiration_days: int) -> s3.Bucket:
         """Create dedicated access logs bucket using opinionated cdk construct
         from cdk-opinionated-constructs.
 
-        :param expiration_days: The number of days after which logs will be deleted
+        :param expiration_days: The number of days after which logs will be deleted is
         :param bucket_name: The name of S3 bucket
         :return: CDK S3 IBucket object
         """
-
         alb_access_logs_bucket_construct = S3Bucket(self, id=f"alb_access_logs_{bucket_name}_construct")
         alb_access_logs_bucket = alb_access_logs_bucket_construct.create_bucket(
             bucket_name=bucket_name, encryption=s3.BucketEncryption.S3_MANAGED
         )
 
         alb_access_logs_bucket.add_to_resource_policy(
             permission=iam.PolicyStatement(
@@ -57,15 +56,15 @@
                 actions=["s3:GetBucketAcl"],
                 principals=[iam.ServicePrincipal(service="delivery.logs.amazonaws.com")],
                 resources=[alb_access_logs_bucket.bucket_arn],
             )
         )
         alb_access_logs_bucket.add_lifecycle_rule(expiration=cdk.Duration.days(expiration_days))
 
-        # Supress few false positive alerts from the cfn-nag
+        # Supress a few false positive alerts from the cfn-nag
         NagSuppressions.add_resource_suppressions(
             alb_access_logs_bucket,
             [
                 {
                     "id": "AwsSolutions-S1",
                     "reason": "ALB access logs location, doesn't contain sensitive data"
                     "it doesn't require another resource for storing access logs from it",
@@ -93,16 +92,15 @@
                 {
                     "front_end_port": 6001,
                     "front_end_protocol": albv2.Protocol.UDP,
                     "targets": [service],
                     "back_end_port": 6001,
                     "back_end_protocol": albv2.Protocol.UDP,
                 },
-            ]
-        )
+            ])
         """
         for port_definition in ports:
             front_end_protocol: albv2.Protocol = port_definition["front_end_protocol"]
             front_end_port: int = port_definition["front_end_port"]
 
             if certificates:
                 listener = nlb.add_listener(
```

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/rds_instance.py` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/rds_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
-"""Opinionated CDK construct to create RDS PostgreSQL Instance with dedicated
+"""Opinionated CDK construct to create RDS PostgresSQL Instance with dedicated
 S3 bucket for storing access logs.
 
 Security parameters are set by default
 """
 from typing import Union
 from constructs import Construct
 import aws_cdk as cdk
 import aws_cdk.aws_secretsmanager as secretsmanager
 import aws_cdk.aws_ec2 as ec2
 import aws_cdk.aws_rds as rds
 
 
 class RDSInstance(Construct):
-    """Create AWS RDS  DB Instance."""
+    """Create AWS RDS DB Instance."""
 
     # pylint: disable=W0235
     # pylint: disable=W0622
     def __init__(self, scope: Construct, construct_id: str):
         """
 
         :param scope:
```

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/s3.py` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/s3.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/sns.py` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/sns.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""Opinionated CDK construct to create SNS topic.
+"""Opinionated CDK construct to create an SNS topic.
 
 Security parameters are set by default
 """
 from constructs import Construct
 import aws_cdk.aws_sns as sns
 from aws_cdk import aws_kms as kms
 from aws_cdk import aws_iam as iam
@@ -21,19 +21,20 @@
 
         :param scope:
         :param id:
         """
         super().__init__(scope, id)
 
     def create_sns_topic(self, topic_name: str, master_key: Union[kms.IKey, None]) -> sns.Topic:
-        """Create SNS topic with resource policy that enforce encrypted access.
+        """Create an SNS topic with resource policy that enforces encrypted
+        access.
 
-        :param topic_name: The name of SNS topic
-        :param master_key: The KMS key to encrypt messages going through sns topic
-        :return: The CDK object for SNS topic
+        :param topic_name: The name of SNS is topic
+        :param master_key: The KMS key to encrypted messages going through sns topic
+        :return: The CDK object for an SNS topic
         """
         topic = sns.Topic(self, id=topic_name, topic_name=topic_name, master_key=master_key)
         topic.add_to_resource_policy(
             iam.PolicyStatement(
                 sid="AllowPublishThroughSSLOnly",
                 actions=["sns:Publish"],
                 effect=iam.Effect.DENY,
```

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs/wafv2.py` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs/wafv2.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk-opinionated-constructs-2.1.5/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/setup.cfg` & `cdk-opinionated-constructs-2.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/setup.py` & `cdk-opinionated-constructs-2.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cdk-opinionated-constructs",
-    version="2.1.4",
+    version="2.1.5",
     description="AWS CDK constructs come without added security configurations.",
     long_description="The idea behind this project is to create secured constructs from the start. \n"
     "Supported constructs: ALB, ECR, LMB, NLB, S3, SNS, WAF, RDS",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
-        "aws-cdk-lib>=2.82.0",
+        "aws-cdk-lib>=2.89.0",
         "constructs>=10.2.43,<11.0.0",
         "cdk-monitoring-constructs>=4.0.0,<6.0.0",
     ],
     python_requires=">=3.10",
 )
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/app.py` & `cdk-opinionated-constructs-2.1.5/test/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,11 +40,11 @@
     env=CDK_ENV,
     props={"project": "test_project", "service_name": "example_lambda_function"},
 )
 TestWAFv2Stack(app, "TestWAFv2Stack", env=CDK_ENV)
 TestALBStack(app, "TestALBStack", env=CDK_ENV)
 TestECRStack(app, "TestECRStack", env=CDK_ENV)
 TestNLBStack(app, "TestNLBStack", env=CDK_ENV)
-TestRDSPostgreSQLStack(app, "TestRDSPostgreSQLStack", env=CDK_ENV)
+TestRDSPostgreSQLStack(app, "TestRDSPostgresSQLStack", env=CDK_ENV)
 TestRDSMySQLStack(app, "TestRDSMySQLStack", env=CDK_ENV)
 
 app.synth()
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/alb_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/ecr_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/ecr_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from constructs import Construct
 from cdk_opinionated_constructs.ecr import ECR
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NIST80053R5Checks, PCIDSS321Checks, HIPAASecurityChecks
 
 
 class TestECRStack(Stack):
-    """Test generated sns topic against AWS solutions  checks."""
+    """Test generated sns topic against AWS solutions checks."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         ecr_construct = ECR(self, id="ecr_construct")
         ecr_construct.repository(repository_name="repository_name", removal_policy="destroy", max_image_age=90)
 
         # Validate stack against AWS Solutions checklist
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/lmb_docker_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/lmb_docker_stack.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import aws_cdk as cdk
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NagSuppressions
 
 
 class TestAWSLambdaDockerFunctionStack(Stack):
-    """Test generated sns topic against AWS solutions  checks."""
+    """Test generated sns topic against AWS solutions checks."""
 
     def __init__(self, scope: Construct, construct_id: str, env, props, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
 
         vpc = ec2.Vpc(self, id="vpc")
         NagSuppressions.add_resource_suppressions(
             vpc,
@@ -29,15 +29,15 @@
             ],
         )
 
         ecr_repository = ecr.Repository(
             self,
             id="ecr_repository",
             auto_delete_images=True,
-            encryption=ecr.RepositoryEncryption.AES_256,
+            encryption=ecr.RepositoryEncryption.AES_256,  # type: ignore
             image_scan_on_push=True,
             image_tag_mutability=ecr.TagMutability.IMMUTABLE,
             repository_name="test_ecr_repository",
             removal_policy=cdk.RemovalPolicy.DESTROY,
         )
 
         lmb_construct = AWSDockerLambdaFunction(self, id="lmb_construct")
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/lmb_monitoring_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/lmb_monitoring_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class TestAWSPythonLambdaFunctionStackMonitoring(Stack):
     """Create monitoring resources for PRS.
 
     This includes:
     * AWS CW Dashboard
     * Metrics
     * Alarms
-    * Subscription to SNS topic
+    * Subscription to an SNS topic
     * similar
     """
 
     # pylint: disable=W0613
     def __init__(self, scope, name, env, props):
         super().__init__(scope, name)
         lmb_function: lmb.Function = props["lmb_function"]
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/lmb_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/lmb_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import aws_cdk.aws_lambda as lmb
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NagSuppressions
 
 
 class TestAWSPythonLambdaFunctionStack(Stack):
-    """Test generated sns topic against AWS solutions  checks."""
+    """Test generated sns topic against AWS solutions checks."""
 
     def __init__(self, scope: Construct, construct_id: str, env, props, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
 
         lmb_construct = AWSPythonLambdaFunction(self, id="lmb_construct")
         lmb_signing = lmb_construct.signing_config(signing_profile_name="signing_profile_name")
         lmb_function = lmb_construct.create_lambda_function(
@@ -50,15 +50,15 @@
         """Create CFN-NAG suppression.
 
         :return:
         """
         return [
             {
                 "id": "AwsSolutions-L1",
-                "reason": "Supressing false positive, lambda is using latest runtime available at the moment which"
+                "reason": "Suppressing false positive, lambda is using latest runtime available at the moment which"
                 "is python3.10",
             },
             {
                 "id": "AwsSolutions-IAM4",
                 "reason": "Using managed policies is allowed",
             },
             {
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/nlb_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/nlb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/rds_mysql_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/rds_mysql_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         rds_construct = RDSInstance(self, construct_id="rds_construct")
 
         database_name = "database-name"
 
         rds_instance = rds_construct.create_db_instance(
             database_name=database_name,
-            engine=rds.DatabaseInstanceEngine.mysql(version=rds.MysqlEngineVersion.VER_8_0_31),
+            engine=rds.DatabaseInstanceEngine.mysql(version=rds.MysqlEngineVersion.VER_8_0_31),  # type: ignore
             publicly_accessible=False,
             secret=secretsmanager.Secret.from_secret_name_v2(self, id="imported_secret", secret_name="secret-name"),
             security_group=security_group,
             snapshot_identifier="snapshot_identifier",
             stage="prod",
             storage_encryption_key=shared_kms_key,
             subnet_group=rds_subnet_group,
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/rds_postgresql_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/rds_postgresql_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks
 import aws_cdk.aws_secretsmanager as secretsmanager
 from cdk_opinionated_constructs.rds_instance import RDSInstance
 
 
 class TestRDSPostgreSQLStack(Stack):
-    """Test generated RDS PostgreSQL stack."""
+    """Test generated RDS PostgresSQL stack."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         shared_kms_key = kms.Key(self, "shared_kms_key", enable_key_rotation=True)
 
         private_subnet = ec2.SubnetConfiguration(
             name="Private", subnet_type=ec2.SubnetType.PRIVATE_WITH_EGRESS, cidr_mask=25
@@ -51,15 +51,15 @@
 
         rds_construct = RDSInstance(self, construct_id="rds_construct")
 
         database_name = "database-name"
 
         rds_instance = rds_construct.create_db_instance(
             database_name=database_name,
-            engine=rds.DatabaseInstanceEngine.postgres(version=rds.PostgresEngineVersion.VER_13_8),
+            engine=rds.DatabaseInstanceEngine.postgres(version=rds.PostgresEngineVersion.VER_13_8),  # type: ignore
             publicly_accessible=False,
             secret=secretsmanager.Secret.from_secret_name_v2(self, id="imported_secret", secret_name="secret-name"),
             security_group=security_group,
             snapshot_identifier="snapshot_identifier",
             stage="prod",
             storage_encryption_key=shared_kms_key,
             subnet_group=rds_subnet_group,
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/s3_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/s3_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import aws_cdk.aws_s3 as s3
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NagSuppressions
 
 
 class TestS3Stack(Stack):
-    """Test generated s3 bucket against AWS solutions  checks."""
+    """Test generated s3 bucket against AWS solutions checks."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         shared_kms_key = kms.Key(self, "SharedKmsKey", enable_key_rotation=True)
 
         s3_bucket_construct = S3Bucket(self, id="bucket")
         access_logs_bucket = s3_bucket_construct.create_bucket(
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/sns_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/test/stacks/wafv2_stack.py` & `cdk-opinionated-constructs-2.1.5/test/stacks/wafv2_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cdk_opinionated_constructs.wafv2 import WAFv2
 
 from aws_cdk import Aspects
 from cdk_nag import AwsSolutionsChecks, NagSuppressions
 
 
 class TestWAFv2Stack(Stack):
-    """Test generated sns topic against AWS solutions  checks."""
+    """Test generated sns topic against AWS solutions checks."""
 
     def __init__(self, scope: Construct, construct_id: str, **kwargs) -> None:
         super().__init__(scope, construct_id, **kwargs)
         vpc = ec2.Vpc(self, id="vpc")
 
         NagSuppressions.add_resource_suppressions(
             vpc,
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/unit/test_alb_stack.py` & `cdk-opinionated-constructs-2.1.5/test/unit/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/test/unit/test_ecr_stack.py` & `cdk-opinionated-constructs-2.1.5/test/unit/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/test/unit/test_lmb_stack.py` & `cdk-opinionated-constructs-2.1.5/test/unit/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/test/unit/test_s3_stack.py` & `cdk-opinionated-constructs-2.1.5/test/unit/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk-opinionated-constructs-2.1.4/test/unit/test_sns_stack.py` & `cdk-opinionated-constructs-2.1.5/test/unit/test_sns_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     app = cdk.App()
     stack = TestSNSStack(app, "TestSNSStack", env=CDK_ENV)
     return Template.from_stack(stack)
 
 
 # pylint: disable=redefined-outer-name
 def test_sns_topic(stack_template):
-    """Test if SNS topic is created."""
+    """Test if an SNS topic is created."""
     stack_template.resource_count_is("AWS::SNS::Topic", 1)
```

### Comparing `cdk-opinionated-constructs-2.1.4/test/unit/test_wafv2_stack.py` & `cdk-opinionated-constructs-2.1.5/test/unit/test_wafv2_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def test_application_load_balancer(stack_template):
     """Test if EC2 Application Load Balancer is created."""
     stack_template.resource_count_is("AWS::ElasticLoadBalancingV2::LoadBalancer", 1)
 
 
 # pylint: disable=redefined-outer-name
 def test_kms_key(stack_template):
-    """Test if KMS key is created."""
+    """Test if a KMS key is created."""
     stack_template.resource_count_is("AWS::KMS::Key", 1)
 
 
 # pylint: disable=redefined-outer-name
 def test_access_logs_bucket(stack_template):
     """Test if S3 bucket is created."""
     stack_template.resource_count_is("AWS::S3::Bucket", 1)
```

