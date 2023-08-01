# Comparing `tmp/ediri_azapi-1.7.0.tar.gz` & `tmp/ediri_azapi-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_azapi-1.7.0.tar", last modified: Sun Jul  2 07:59:39 2023, max compression
+gzip compressed data, was "ediri_azapi-1.8.0.tar", last modified: Tue Aug  1 07:28:36 2023, max compression
```

## Comparing `ediri_azapi-1.7.0.tar` & `ediri_azapi-1.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/ediri_azapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/ediri_azapi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    51844 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/data_plane_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/get_resource_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48794 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/resource_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/update_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/ediri_azapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:28:36.988615 ediri_azapi-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-08-01 07:28:36.984615 ediri_azapi-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:28:36.984615 ediri_azapi-1.8.0/ediri_azapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:28:36.984615 ediri_azapi-1.8.0/ediri_azapi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51844 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/data_plane_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/get_resource_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48794 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26763 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/resource_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi/update_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:28:36.984615 ediri_azapi-1.8.0/ediri_azapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/ediri_azapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 07:28:36.988615 ediri_azapi-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-01 07:28:36.000000 ediri_azapi-1.8.0/setup.py
```

### Comparing `ediri_azapi-1.7.0/PKG-INFO` & `ediri_azapi-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri_azapi
-Version: 1.7.0
+Version: 1.8.0
 Summary: A Pulumi package for creating and managing Azapi resources
 Home-page: https://github.com/dirien/pulumi-azapi
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-azapi
 Keywords: pulumi azapi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_azapi-1.7.0/README.md` & `ediri_azapi-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/__init__.py` & `ediri_azapi-1.8.0/ediri_azapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/_inputs.py` & `ediri_azapi-1.8.0/ediri_azapi/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/_utilities.py` & `ediri_azapi-1.8.0/ediri_azapi/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/config/vars.py` & `ediri_azapi-1.8.0/ediri_azapi/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/data_plane_resource.py` & `ediri_azapi-1.8.0/ediri_azapi/data_plane_resource.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/get_resource.py` & `ediri_azapi-1.8.0/ediri_azapi/get_resource.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/get_resource_action.py` & `ediri_azapi-1.8.0/ediri_azapi/get_resource_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,18 @@
     """
     This resource can perform resource action which gets information from an existing resource.
     It's recommended to use `ResourceAction` data source to perform readonly action, please use `ResourceAction` resource,
     if user wants to perform actions which change a resource's state.
 
     ## Example Usage
 
+    Here's an example to use the `ResourceAction` data source to get a provider's permissions.
+
+    Here's an example to use the `ResourceAction` data source to perform a provider action.
+
 
     :param str action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
     :param str body: A JSON object that contains the request body.
     :param str method: Specifies the Http method of the azure resource action. Allowed values are `POST` and `GET`. Defaults to `POST`.
     :param str resource_id: The ID of an existing azure source.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
@@ -188,14 +192,18 @@
     """
     This resource can perform resource action which gets information from an existing resource.
     It's recommended to use `ResourceAction` data source to perform readonly action, please use `ResourceAction` resource,
     if user wants to perform actions which change a resource's state.
 
     ## Example Usage
 
+    Here's an example to use the `ResourceAction` data source to get a provider's permissions.
+
+    Here's an example to use the `ResourceAction` data source to perform a provider action.
+
 
     :param str action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
     :param str body: A JSON object that contains the request body.
     :param str method: Specifies the Http method of the azure resource action. Allowed values are `POST` and `GET`. Defaults to `POST`.
     :param str resource_id: The ID of an existing azure source.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
```

### Comparing `ediri_azapi-1.7.0/ediri_azapi/outputs.py` & `ediri_azapi-1.8.0/ediri_azapi/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/provider.py` & `ediri_azapi-1.8.0/ediri_azapi/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/resource.py` & `ediri_azapi-1.8.0/ediri_azapi/resource.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi/resource_action.py` & `ediri_azapi-1.8.0/ediri_azapi/resource_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,14 +359,18 @@
         It's recommended to use `ResourceAction` resource to perform actions which change a resource's state, please use `ResourceAction` data source,
         if user wants to perform readonly action.
 
         > **Note** When delete `ResourceAction`, no operation will be performed.
 
         ## Example Usage
 
+        Here's an example to use the `ResourceAction` resource to register a provider.
+
+        Here's an example to use the `ResourceAction` resource to perform a provider action.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
         :param pulumi.Input[str] body: A JSON object that contains the request body.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid modify azapi resources at the same time.
         :param pulumi.Input[str] method: Specifies the Http method of the azure resource action. Allowed values are `POST`, `PATCH`, `PUT` and `DELETE`. Defaults to `POST`.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source.
@@ -403,14 +407,18 @@
         It's recommended to use `ResourceAction` resource to perform actions which change a resource's state, please use `ResourceAction` data source,
         if user wants to perform readonly action.
 
         > **Note** When delete `ResourceAction`, no operation will be performed.
 
         ## Example Usage
 
+        Here's an example to use the `ResourceAction` resource to register a provider.
+
+        Here's an example to use the `ResourceAction` resource to perform a provider action.
+
         :param str resource_name: The name of the resource.
         :param ResourceActionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ResourceActionArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `ediri_azapi-1.7.0/ediri_azapi/update_resource.py` & `ediri_azapi-1.8.0/ediri_azapi/update_resource.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/ediri_azapi.egg-info/PKG-INFO` & `ediri_azapi-1.8.0/ediri_azapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri-azapi
-Version: 1.7.0
+Version: 1.8.0
 Summary: A Pulumi package for creating and managing Azapi resources
 Home-page: https://github.com/dirien/pulumi-azapi
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-azapi
 Keywords: pulumi azapi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_azapi-1.7.0/ediri_azapi.egg-info/SOURCES.txt` & `ediri_azapi-1.8.0/ediri_azapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.7.0/setup.py` & `ediri_azapi-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.7.0"
-PLUGIN_VERSION = "1.7.0"
+VERSION = "1.8.0"
+PLUGIN_VERSION = "1.8.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'azapi', PLUGIN_VERSION, '--server', 'github://api.github.com/dirien/pulumi-azapi'])
         except OSError as error:
```

