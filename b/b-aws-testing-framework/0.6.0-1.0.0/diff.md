# Comparing `tmp/b_aws_testing_framework-0.6.0.tar.gz` & `tmp/b_aws_testing_framework-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/b_aws_testing_framework-0.6.0.tar", last modified: Sun May  2 09:40:40 2021, max compression
+gzip compressed data, was "b_aws_testing_framework-1.0.0.tar", last modified: Tue Aug  1 09:52:03 2023, max compression
```

## Comparing `b_aws_testing_framework-0.6.0.tar` & `b_aws_testing_framework-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.893028 b_aws_testing_framework-0.6.0/
--rw-rw-r--   0 root         (0) root         (0)     2680 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/HISTORY.md
--rw-rw-r--   0 root         (0) root         (0)    11357 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      164 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9864 2021-05-02 09:40:40.893028 b_aws_testing_framework-0.6.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4389 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/README.md
--rw-rw-r--   0 root         (0) root         (0)        5 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.889028 b_aws_testing_framework-0.6.0/b_aws_testing_framework/
--rw-rw-r--   0 root         (0) root         (0)      538 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3945 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/base_testing_manager.py
--rw-rw-r--   0 root         (0) root         (0)     1891 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.889028 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.889028 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cdk_testing/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cdk_testing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1807 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cdk_testing/cdk_tool_config.py
--rw-rw-r--   0 root         (0) root         (0)     4242 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cdk_testing/testing_manager.py
--rw-rw-r--   0 root         (0) root         (0)     3389 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cdk_testing/testing_stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.889028 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cf_testing/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cf_testing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      271 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cf_testing/cf_tool_config.py
--rw-rw-r--   0 root         (0) root         (0)     2075 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cf_testing/stack_waiter.py
--rw-rw-r--   0 root         (0) root         (0)     2899 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cf_testing/testing_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.889028 b_aws_testing_framework-0.6.0/b_aws_testing_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9864 2021-05-02 09:40:40.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1720 2021-05-02 09:40:40.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-02 09:40:40.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2021-05-02 09:40:40.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2021-05-02 09:40:40.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.885028 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.889028 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.889028 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      169 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/app.py
--rw-rw-r--   0 root         (0) root         (0)      784 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/conftest.py
--rw-rw-r--   0 root         (0) root         (0)      516 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/infrastructure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.893028 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      432 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_outputs.py
--rw-rw-r--   0 root         (0) root         (0)      565 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_stack_exists.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.893028 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cf/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cf/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1104 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cf/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-02 09:40:40.893028 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      686 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/test_stack_exists.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-05-02 09:40:40.893028 b_aws_testing_framework-0.6.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1353 2021-05-02 09:38:07.000000 b_aws_testing_framework-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      164 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10064 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.506086 b_aws_testing_framework-1.0.0/b_aws_testing_framework/
+-rw-r--r--   0 root         (0) root         (0)      538 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/base_testing_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/cdk_tool_config.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/testing_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3406 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/testing_stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/cf_tool_config.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/stack_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/testing_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10064 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.502086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/app.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      514 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/infrastructure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_outputs.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_stack_exists.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/test_stack_exists.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/setup.py
```

### Comparing `b_aws_testing_framework-0.6.0/HISTORY.md` & `b_aws_testing_framework-1.0.0/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Release history
 
+### 1.0.0
+* Upgrade CDK support from v1 to v2.
+* Upgrade GitHub pipelines checkout version from v2 to v3.
+* Upgrade biomapas/cicd-full image version to 5.0.0.
+
 ### 0.6.0
 * Too many bugs. Revert.
 
 ### 0.5.5
 * Warn if not cdk tool was found.
 
 ### 0.5.4
```

### Comparing `b_aws_testing_framework-0.6.0/LICENSE` & `b_aws_testing_framework-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/PKG-INFO` & `b_aws_testing_framework-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b_aws_testing_framework
-Version: 0.6.0
+Version: 1.0.0
 Summary: AWS infrastructure testing framework that supports multiple IAC tools.
 Home-page: https://github.com/biomapas/B.AwsTestingFramework.git
 Author: Laimonas Sutkus
 Author-email: laimonas.sutkus@biomapas.com
 License: Apache License 2.0
 Description: # B.AwsTestingFramework
         
@@ -158,14 +158,19 @@
         Contributions of any kind are gladly welcome. You may contact us 
         directly, create a pull-request or an issue in github platform.
         Lets modernize the world together.
         
         
         # Release history
         
+        ### 1.0.0
+        * Upgrade CDK support from v1 to v2.
+        * Upgrade GitHub pipelines checkout version from v2 to v3.
+        * Upgrade biomapas/cicd-full image version to 5.0.0.
+        
         ### 0.6.0
         * Too many bugs. Revert.
         
         ### 0.5.5
         * Warn if not cdk tool was found.
         
         ### 0.5.4
```

### Comparing `b_aws_testing_framework-0.6.0/README.md` & `b_aws_testing_framework-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework/__init__.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework/base_testing_manager.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework/base_testing_manager.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework/credentials.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework/credentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             region_name: Optional[str] = os.environ.get('AWS_DEFAULT_REGION'),
     ) -> None:
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.aws_session_token = aws_session_token
         self.profile_name = profile_name
         self.region_name = region_name
+        self.aws_account_id = self.boto_session.client("sts").get_caller_identity()["Account"]
 
     @property
     def boto_session(self) -> Session:
         """
         Property for boto session.
 
         :return: Boto session instance.
@@ -47,9 +48,10 @@
         :return: Credentials in a form of a dict.
         """
         return {key: value for key, value in {
             'AWS_ACCESS_KEY_ID': self.aws_access_key_id,
             'AWS_SECRET_ACCESS_KEY': self.aws_secret_access_key,
             'AWS_SESSION_TOKEN': self.aws_session_token,
             'AWS_PROFILE': self.profile_name,
-            'AWS_DEFAULT_REGION': self.region_name
+            'AWS_DEFAULT_REGION': self.region_name,
+            'AWS_ACCOUNT_ID': self.aws_account_id
         }.items() if value} or None
```

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cdk_testing/cdk_tool_config.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/cdk_tool_config.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cdk_testing/testing_manager.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/testing_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,35 +81,34 @@
         self.delete_global_prefix()
 
     """
     Infrastructure functions.
     """
 
     def __bootstrap_infrastructure(self) -> None:
-        sub = ContinuousSubprocess(TestingManager.__aws_cdk_bootstrap_command())
+        sub = ContinuousSubprocess(self.__aws_cdk_bootstrap_command())
         output = sub.execute(path=self.__config.cdk_app_path, env=self.__config.deployment_process_environment)
         for line in output: logger.info(line.strip())
 
     def __create_infrastructure(self) -> None:
-        sub = ContinuousSubprocess(TestingManager.__aws_cdk_deploy_command())
+        sub = ContinuousSubprocess(self.__aws_cdk_deploy_command())
         output = sub.execute(path=self.__config.cdk_app_path, env=self.__config.deployment_process_environment)
         for line in output: logger.info(line.strip())
 
     def __destroy_infrastructure(self) -> None:
-        sub = ContinuousSubprocess(TestingManager.__aws_cdk_destroy_command())
+        sub = ContinuousSubprocess(self.__aws_cdk_destroy_command())
         output = sub.execute(path=self.__config.cdk_app_path, env=self.__config.deployment_process_environment)
         for line in output: logger.info(line.strip())
 
     """
     CDK Commands.
     """
 
-    @classmethod
-    def __aws_cdk_bootstrap_command(cls) -> str:
-        return f'cdk bootstrap'
+    def __aws_cdk_bootstrap_command(self) -> str:
+        return f'cdk bootstrap aws://{self.credentials.aws_account_id}/{self.credentials.region_name}'
 
     @classmethod
     def __aws_cdk_deploy_command(cls) -> str:
         return f'cdk deploy --all --require-approval never'
 
     @classmethod
     def __aws_cdk_destroy_command(cls) -> str:
```

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cdk_testing/testing_stack.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/testing_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import lru_cache
 from typing import Dict, Optional
 
+from aws_cdk import Stack, CfnOutput
 from aws_cdk.aws_ssm import StringParameter
-from aws_cdk.core import Stack, Construct, CfnOutput
 from b_cf_outputs.cf_outputs import CfOutputs
+from constructs import Construct
 
 from b_aws_testing_framework import b_aws_testing_framework_version
 from b_aws_testing_framework.credentials import Credentials
 from b_aws_testing_framework.tools.cdk_testing.testing_manager import TestingManager
 
 
 class TestingStack(Stack):
```

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cf_testing/stack_waiter.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/stack_waiter.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework/tools/cf_testing/testing_manager.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/testing_manager.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework.egg-info/PKG-INFO` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b-aws-testing-framework
-Version: 0.6.0
+Version: 1.0.0
 Summary: AWS infrastructure testing framework that supports multiple IAC tools.
 Home-page: https://github.com/biomapas/B.AwsTestingFramework.git
 Author: Laimonas Sutkus
 Author-email: laimonas.sutkus@biomapas.com
 License: Apache License 2.0
 Description: # B.AwsTestingFramework
         
@@ -158,14 +158,19 @@
         Contributions of any kind are gladly welcome. You may contact us 
         directly, create a pull-request or an issue in github platform.
         Lets modernize the world together.
         
         
         # Release history
         
+        ### 1.0.0
+        * Upgrade CDK support from v1 to v2.
+        * Upgrade GitHub pipelines checkout version from v2 to v3.
+        * Upgrade biomapas/cicd-full image version to 5.0.0.
+        
         ### 0.6.0
         * Too many bugs. Revert.
         
         ### 0.5.5
         * Warn if not cdk tool was found.
         
         ### 0.5.4
```

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework.egg-info/SOURCES.txt` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/conftest.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/conftest.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/infrastructure.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/infrastructure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from aws_cdk.core import Construct
+from constructs import Construct
 
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 
 
 class Infrastructure(TestingStack):
     """
     This is an entry point for your infrastructure.
```

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_stack_exists.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_stack_exists.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import itertools
 import logging
+from typing import Iterable, Dict, Any
 
 from b_aws_testing_framework.credentials import Credentials
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 
 logger = logging.getLogger(__name__)
 
 
@@ -10,11 +12,15 @@
     """
     Tests that stack actually was created.
 
     :return: No return.
     """
     client = Credentials().boto_session.client('cloudformation')
 
-    stacks = client.list_stacks(StackStatusFilter=['CREATE_COMPLETE'])['StackSummaries']
-    stacks = [stack['StackName'] for stack in stacks]
+    response_iterator = client.get_paginator('list_stacks').paginate(StackStatusFilter=['CREATE_COMPLETE'])
+    stack_summaries: Iterable[Dict[str, Any]] = itertools.chain.from_iterable(
+        page['StackSummaries'] for page in response_iterator
+    )
 
-    assert TestingStack.name() in stacks
+    stack_names = [stack['StackName'] for stack in stack_summaries]
+
+    assert TestingStack.name() in stack_names
```

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cf/conftest.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/conftest.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-0.6.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/test_stack_exists.py` & `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/test_stack_exists.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import itertools
 import logging
+from typing import Any, Dict, Iterable
 
 from b_aws_testing_framework.credentials import Credentials
 from b_aws_testing_framework.tools.cf_testing.testing_manager import TestingManager
 
 logger = logging.getLogger(__name__)
 
 
@@ -13,11 +15,15 @@
     :return: No return.
     """
     # The stack name is provided by the cf testing manager.
     stack_name = f'{TestingManager.get_global_prefix()}TestStack'
 
     client = Credentials().boto_session.client('cloudformation')
 
-    stacks = client.list_stacks(StackStatusFilter=['CREATE_COMPLETE'])['StackSummaries']
-    stacks = [stack['StackName'] for stack in stacks]
+    response_iterator = client.get_paginator('list_stacks').paginate(StackStatusFilter=['CREATE_COMPLETE'])
+    stack_summaries: Iterable[Dict[str, Any]] = itertools.chain.from_iterable(
+        page['StackSummaries'] for page in response_iterator
+    )
 
-    assert stack_name in stacks
+    stack_names = [stack['StackName'] for stack in stack_summaries]
+
+    assert stack_name in stack_names
```

### Comparing `b_aws_testing_framework-0.6.0/setup.py` & `b_aws_testing_framework-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     description=(
         'AWS infrastructure testing framework that supports multiple IAC tools.'
     ),
     long_description=README + '\n\n' + HISTORY,
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=[
-        'aws-cdk.core>=1.50.0,<2.0.0',
-        'aws-cdk.aws-ssm>=1.50.0,<2.0.0',
+        'aws-cdk-lib>=2.0.0,<3.0.0',
+        'aws-cdk-constructs>=2.0.0,<3.0.0',
         'boto3>=1.16.0,<2.0.0',
         'pytest>=6.0.2,<7.0.0',
         'b-continuous-subprocess>=0.3.2,<1.0.0',
         'b-cf-outputs>=0.0.3,<1.0.0'
     ],
     author='Laimonas Sutkus',
     author_email='laimonas.sutkus@biomapas.com',
```

