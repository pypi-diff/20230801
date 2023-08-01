# Comparing `tmp/mypy-boto3-batch-1.28.16.tar.gz` & `tmp/mypy-boto3-batch-1.28.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-batch-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
+gzip compressed data, was "mypy-boto3-batch-1.28.17.tar", last modified: Tue Aug  1 19:33:25 2023, max compression
```

## Comparing `mypy-boto3-batch-1.28.16.tar` & `mypy-boto3-batch-1.28.17.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18553 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/mypy_boto3_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-08-01 11:11:36.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-08-01 11:11:37.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52029 2023-08-01 11:11:36.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18553 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.427422 mypy-boto3-batch-1.28.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18553 2023-08-01 19:33:25.423421 mypy-boto3-batch-1.28.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.423421 mypy-boto3-batch-1.28.17/mypy_boto3_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-08-01 19:32:16.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52029 2023-08-01 19:32:16.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.423421 mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18553 2023-08-01 19:33:25.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 19:33:25.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:33:25.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:33:25.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 19:33:25.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 19:33:25.000000 mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:33:25.427422 mypy-boto3-batch-1.28.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 19:32:14.000000 mypy-boto3-batch-1.28.17/setup.py
```

### Comparing `mypy-boto3-batch-1.28.16/LICENSE` & `mypy-boto3-batch-1.28.17/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/PKG-INFO` & `mypy-boto3-batch-1.28.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.16
-Summary: Type annotations for boto3.Batch 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.17
+Summary: Type annotations for boto3.Batch 1.28.17 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-batch-1.28.16/README.md` & `mypy-boto3-batch-1.28.17/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/__init__.py` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/__init__.pyi` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/__main__.py` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Batch 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        "Type annotations for boto3.Batch 1.28.17\nVersion:         1.28.17\nBuilder version:"
         " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.17")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/client.py` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/client.pyi` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/literals.py` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,21 @@
 
 
 ArrayJobDependencyType = Literal["N_TO_N", "SEQUENTIAL"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CEStateType = Literal["DISABLED", "ENABLED"]
 CEStatusType = Literal["CREATING", "DELETED", "DELETING", "INVALID", "UPDATING", "VALID"]
 CETypeType = Literal["MANAGED", "UNMANAGED"]
-CRAllocationStrategyType = Literal["BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
+CRAllocationStrategyType = Literal[
+    "BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
+]
 CRTypeType = Literal["EC2", "FARGATE", "FARGATE_SPOT", "SPOT"]
-CRUpdateAllocationStrategyType = Literal["BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
+CRUpdateAllocationStrategyType = Literal[
+    "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
+]
 DescribeComputeEnvironmentsPaginatorName = Literal["describe_compute_environments"]
 DescribeJobDefinitionsPaginatorName = Literal["describe_job_definitions"]
 DescribeJobQueuesPaginatorName = Literal["describe_job_queues"]
 DeviceCgroupPermissionType = Literal["MKNOD", "READ", "WRITE"]
 EFSAuthorizationConfigIAMType = Literal["DISABLED", "ENABLED"]
 EFSTransitEncryptionType = Literal["DISABLED", "ENABLED"]
 JQStateType = Literal["DISABLED", "ENABLED"]
```

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/literals.pyi` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,21 @@
 )
 
 ArrayJobDependencyType = Literal["N_TO_N", "SEQUENTIAL"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CEStateType = Literal["DISABLED", "ENABLED"]
 CEStatusType = Literal["CREATING", "DELETED", "DELETING", "INVALID", "UPDATING", "VALID"]
 CETypeType = Literal["MANAGED", "UNMANAGED"]
-CRAllocationStrategyType = Literal["BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
+CRAllocationStrategyType = Literal[
+    "BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
+]
 CRTypeType = Literal["EC2", "FARGATE", "FARGATE_SPOT", "SPOT"]
-CRUpdateAllocationStrategyType = Literal["BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
+CRUpdateAllocationStrategyType = Literal[
+    "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
+]
 DescribeComputeEnvironmentsPaginatorName = Literal["describe_compute_environments"]
 DescribeJobDefinitionsPaginatorName = Literal["describe_job_definitions"]
 DescribeJobQueuesPaginatorName = Literal["describe_job_queues"]
 DeviceCgroupPermissionType = Literal["MKNOD", "READ", "WRITE"]
 EFSAuthorizationConfigIAMType = Literal["DISABLED", "ENABLED"]
 EFSTransitEncryptionType = Literal["DISABLED", "ENABLED"]
 JQStateType = Literal["DISABLED", "ENABLED"]
```

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/paginator.py` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/paginator.pyi` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/type_defs.py` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch/type_defs.pyi` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/PKG-INFO` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.16
-Summary: Type annotations for boto3.Batch 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.17
+Summary: Type annotations for boto3.Batch 1.28.17 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/SOURCES.txt` & `mypy-boto3-batch-1.28.17/mypy_boto3_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.16/setup.py` & `mypy-boto3-batch-1.28.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-batch",
-    version="1.28.16",
+    version="1.28.17",
     packages=["mypy_boto3_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Batch 1.28.16 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.Batch 1.28.17 service generated with mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

