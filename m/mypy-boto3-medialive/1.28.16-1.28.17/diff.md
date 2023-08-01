# Comparing `tmp/mypy-boto3-medialive-1.28.16.tar.gz` & `tmp/mypy-boto3-medialive-1.28.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.28.16.tar", last modified: Tue Aug  1 11:37:19 2023, max compression
+gzip compressed data, was "mypy-boto3-medialive-1.28.17.tar", last modified: Tue Aug  1 19:33:25 2023, max compression
```

## Comparing `mypy-boto3-medialive-1.28.16.tar` & `mypy-boto3-medialive-1.28.17.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    38965 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37473 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52988 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-08-01 11:24:00.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   173232 2023-08-01 11:24:07.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   173055 2023-08-01 11:24:02.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-08-01 11:23:59.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38965 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:37:19.000000 mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:19.408824 mypy-boto3-medialive-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:23:58.000000 mypy-boto3-medialive-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.447423 mypy-boto3-medialive-1.28.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 19:32:27.000000 mypy-boto3-medialive-1.28.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    38965 2023-08-01 19:33:25.447423 mypy-boto3-medialive-1.28.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37473 2023-08-01 19:32:27.000000 mypy-boto3-medialive-1.28.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.435422 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-01 19:32:27.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-01 19:32:27.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 19:32:27.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53025 2023-08-01 19:32:28.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52935 2023-08-01 19:32:28.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39584 2023-08-01 19:32:29.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-08-01 19:32:29.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-08-01 19:32:28.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-08-01 19:32:28.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:32:27.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   173364 2023-08-01 19:32:34.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173187 2023-08-01 19:32:31.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 19:32:27.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-08-01 19:32:28.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-08-01 19:32:28.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:33:25.443422 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38965 2023-08-01 19:33:25.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 19:33:25.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:33:25.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:33:25.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 19:33:25.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 19:33:25.000000 mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:33:25.447423 mypy-boto3-medialive-1.28.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 19:32:27.000000 mypy-boto3-medialive-1.28.17/setup.py
```

### Comparing `mypy-boto3-medialive-1.28.16/LICENSE` & `mypy-boto3-medialive-1.28.17/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/PKG-INFO` & `mypy-boto3-medialive-1.28.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.28.16
-Summary: Type annotations for boto3.MediaLive 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.17
+Summary: Type annotations for boto3.MediaLive 1.28.17 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-medialive-1.28.16/README.md` & `mypy-boto3-medialive-1.28.17/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__init__.py` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__init__.pyi` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/__main__.py` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        "Type annotations for boto3.MediaLive 1.28.17\nVersion:         1.28.17\nBuilder version:"
         " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
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

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/client.py` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,15 +860,16 @@
 
     def update_input_device(
         self,
         *,
         InputDeviceId: str,
         HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
         Name: str = ...,
-        UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...
+        UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
+        AvailabilityZone: str = ...
     ) -> UpdateInputDeviceResponseTypeDef:
         """
         Updates the parameters for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_input_device)
         """
```

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/client.pyi` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -795,15 +795,16 @@
         """
     def update_input_device(
         self,
         *,
         InputDeviceId: str,
         HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
         Name: str = ...,
-        UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...
+        UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
+        AvailabilityZone: str = ...
     ) -> UpdateInputDeviceResponseTypeDef:
         """
         Updates the parameters for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_input_device)
         """
```

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/literals.py` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/literals.pyi` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/paginator.py` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/paginator.pyi` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/type_defs.py` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3452,14 +3452,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
@@ -3472,14 +3473,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
     },
     total=False,
 )
 
 UpdateInputDeviceResponseTypeDef = TypedDict(
     "UpdateInputDeviceResponseTypeDef",
     {
@@ -3492,14 +3494,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
@@ -3887,14 +3890,15 @@
 )
 _OptionalUpdateInputDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateInputDeviceRequestRequestTypeDef",
     {
         "HdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
         "Name": str,
         "UhdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
+        "AvailabilityZone": str,
     },
     total=False,
 )
 
 
 class UpdateInputDeviceRequestRequestTypeDef(
     _RequiredUpdateInputDeviceRequestRequestTypeDef, _OptionalUpdateInputDeviceRequestRequestTypeDef
```

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/type_defs.pyi` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -3367,14 +3367,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
@@ -3387,14 +3388,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
     },
     total=False,
 )
 
 UpdateInputDeviceResponseTypeDef = TypedDict(
     "UpdateInputDeviceResponseTypeDef",
     {
@@ -3407,14 +3409,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
@@ -3794,14 +3797,15 @@
 )
 _OptionalUpdateInputDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateInputDeviceRequestRequestTypeDef",
     {
         "HdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
         "Name": str,
         "UhdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
+        "AvailabilityZone": str,
     },
     total=False,
 )
 
 class UpdateInputDeviceRequestRequestTypeDef(
     _RequiredUpdateInputDeviceRequestRequestTypeDef, _OptionalUpdateInputDeviceRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/waiter.py` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive/waiter.pyi` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.28.16
-Summary: Type annotations for boto3.MediaLive 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.17
+Summary: Type annotations for boto3.MediaLive 1.28.17 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.28.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-medialive-1.28.16/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy-boto3-medialive-1.28.17/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.28.16/setup.py` & `mypy-boto3-medialive-1.28.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.28.16",
+    version="1.28.17",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaLive 1.28.16 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.MediaLive 1.28.17 service generated with mypy-boto3-builder"
         " 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

