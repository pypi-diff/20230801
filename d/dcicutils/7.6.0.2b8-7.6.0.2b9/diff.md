# Comparing `tmp/dcicutils-7.6.0.2b8.tar.gz` & `tmp/dcicutils-7.6.0.2b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.6.0.2b8.tar", max compression
+gzip compressed data, was "dcicutils-7.6.0.2b9.tar", max compression
```

## Comparing `dcicutils-7.6.0.2b8.tar` & `dcicutils-7.6.0.2b9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1103 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/README.rst
--rw-r--r--   0        0        0        0 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3763 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68885 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27797 2023-07-30 13:17:35.699077 dcicutils-7.6.0.2b8/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    38497 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20511 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    13576 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     4387 2023-07-30 13:17:35.703076 dcicutils-7.6.0.2b8/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b8/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b8/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/README.rst
+-rw-r--r--   0        0        0        0 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3763 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68885 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-08-01 18:39:50.141009 dcicutils-7.6.0.2b9/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27797 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    38905 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20511 2023-08-01 18:39:50.145009 dcicutils-7.6.0.2b9/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     4387 2023-08-01 18:39:50.149009 dcicutils-7.6.0.2b9/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b9/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b9/PKG-INFO
```

### Comparing `dcicutils-7.6.0.2b8/LICENSE.txt` & `dcicutils-7.6.0.2b9/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright 2017-2023 President and Fellows of Harvard College.
+Copyright 2017-2023 President and Fellows of Harvard College
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dcicutils-7.6.0.2b8/README.rst` & `dcicutils-7.6.0.2b9/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/base.py` & `dcicutils-7.6.0.2b9/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/beanstalk_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/cloudformation_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/codebuild_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/command_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/common.py` & `dcicutils-7.6.0.2b9/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/contribution_scripts.py` & `dcicutils-7.6.0.2b9/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/contribution_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/creds_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/data_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/deployment_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/diff_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/docker_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/ecr_scripts.py` & `dcicutils-7.6.0.2b9/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/ecr_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/ecs_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/env_base.py` & `dcicutils-7.6.0.2b9/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/env_manager.py` & `dcicutils-7.6.0.2b9/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/env_scripts.py` & `dcicutils-7.6.0.2b9/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/env_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/env_utils_legacy.py` & `dcicutils-7.6.0.2b9/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/es_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/exceptions.py` & `dcicutils-7.6.0.2b9/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/ff_mocks.py` & `dcicutils-7.6.0.2b9/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/ff_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/function_cache_decorator.py` & `dcicutils-7.6.0.2b9/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/glacier_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/jh_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/kibana/dashboards.json` & `dcicutils-7.6.0.2b9/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/kibana/readme.md` & `dcicutils-7.6.0.2b9/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/lang_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/license_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/license_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -663,34 +663,46 @@
         # Ref: https://github.com/tlsfuzzer/python-ecdsa/blob/master/LICENSE
         'ecdsa',
 
         # This has an MIT license in its source repository
         # Ref: https://github.com/xlwings/jsondiff/blob/master/LICENSE
         'jsondiff',
 
+        # This has an MIT license in its source repository
+        # Ref: https://github.com/pkerpedjiev/negspy/blob/master/LICENSE
+        'negspy',
+
         # This license statement is complicated, but seems adequately permissive.
         # Ref: https://foss.heptapod.net/python-libs/passlib/-/blob/branch/stable/LICENSE
         'passlib',
 
         # This seems to be a BSD-3-Clause license.
         # Ref: https://github.com/protocolbuffers/protobuf/blob/main/LICENSE
         # pypi agrees in the Meta section of protobuf's page, where it says "3-Clause BSD License"
         # Ref: https://pypi.org/project/protobuf/
         'protobuf',
 
         # The WTFPL license is permissive.
         # Ref: https://github.com/mk-fg/pretty-yaml/blob/master/COPYING
         'pyaml',
 
+        # This uses a BSD license
+        # Ref: https://github.com/eliben/pycparser/blob/master/LICENSE
+        'pycparser',
+
         # The source repo for pyDes says this is under an MIT license
         # Ref: https://github.com/twhiteman/pyDes/blob/master/LICENSE.txt
         # pypi, probably wrongly, thinks this is in the public domain (as of 2023-07-21)
         # Ref: https://pypi.org/project/pyDes/
         'pyDes',
 
+        # This uses an MIT license
+        # Ref: https://github.com/pysam-developers/pysam/blob/master/COPYING
+        'pysam',
+
         # The version of python-lambda that we forked calls itself this (and publishes at pypi under this name)
         "python-lambda-4dn",
 
         # This is MIT-licensed:
         # Ref: https://github.com/themiurgo/ratelim/blob/master/LICENSE
         # pypi agrees
         # Ref: https://pypi.org/project/ratelim/
```

### Comparing `dcicutils-7.6.0.2b8/dcicutils/log_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/misc_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/obfuscation_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/opensearch_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/project_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/qa_checkers.py` & `dcicutils-7.6.0.2b9/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/qa_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/redis_tools.py` & `dcicutils-7.6.0.2b9/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/redis_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/s3_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.6.0.2b9/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/secrets_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/snapshot_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/task_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/dcicutils/trace_utils.py` & `dcicutils-7.6.0.2b9/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b8/pyproject.toml` & `dcicutils-7.6.0.2b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.6.0.2b8"
+version = "7.6.0.2b9"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.6.0.2b8/setup.py` & `dcicutils-7.6.0.2b9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 entry_points = \
 {'console_scripts': ['publish-to-pypi = dcicutils.scripts.publish_to_pypi:main',
                      'show-contributors = '
                      'dcicutils.contribution_scripts:show_contributors_main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.6.0.2b8',
+    'version': '7.6.0.2b9',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.6.0.2b8/PKG-INFO` & `dcicutils-7.6.0.2b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.6.0.2b8
+Version: 7.6.0.2b9
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

