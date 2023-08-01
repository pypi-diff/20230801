# Comparing `tmp/pulumi_slack-0.4.3a1690264522.tar.gz` & `tmp/pulumi_slack-0.4.3a1690907235.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_slack-0.4.3a1690264522.tar", last modified: Tue Jul 25 06:03:41 2023, max compression
+gzip compressed data, was "pulumi_slack-0.4.3a1690907235.tar", last modified: Tue Aug  1 16:30:58 2023, max compression
```

## Comparing `pulumi_slack-0.4.3a1690264522.tar` & `pulumi_slack-0.4.3a1690907235.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:41.505857 pulumi_slack-0.4.3a1690264522/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-25 06:03:41.505857 pulumi_slack-0.4.3a1690264522/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:41.505857 pulumi_slack-0.4.3a1690264522/pulumi_slack/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:41.505857 pulumi_slack-0.4.3a1690264522/pulumi_slack/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/get_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/get_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack/usergroup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:41.505857 pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:03:41.505857 pulumi_slack-0.4.3a1690264522/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-25 06:03:41.000000 pulumi_slack-0.4.3a1690264522/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:58.454037 pulumi_slack-0.4.3a1690907235/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-01 16:30:58.454037 pulumi_slack-0.4.3a1690907235/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:58.450036 pulumi_slack-0.4.3a1690907235/pulumi_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:58.454037 pulumi_slack-0.4.3a1690907235/pulumi_slack/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/get_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/get_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack/usergroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:58.454037 pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:30:58.454037 pulumi_slack-0.4.3a1690907235/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-08-01 16:30:58.000000 pulumi_slack-0.4.3a1690907235/setup.py
```

### Comparing `pulumi_slack-0.4.3a1690264522/PKG-INFO` & `pulumi_slack-0.4.3a1690907235/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.3a1690264522
+Version: 0.4.3a1690907235
 Summary: A Pulumi package for managing Slack workspaces.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi slack category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_slack-0.4.3a1690264522/README.md` & `pulumi_slack-0.4.3a1690907235/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/__init__.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/_utilities.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/config/vars.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/conversation.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/get_conversation.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/get_conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/get_user.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/get_usergroup.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/get_usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/provider.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack/usergroup.py` & `pulumi_slack-0.4.3a1690907235/pulumi_slack/usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/PKG-INFO` & `pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-slack
-Version: 0.4.3a1690264522
+Version: 0.4.3a1690907235
 Summary: A Pulumi package for managing Slack workspaces.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi slack category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_slack-0.4.3a1690264522/pulumi_slack.egg-info/SOURCES.txt` & `pulumi_slack-0.4.3a1690907235/pulumi_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.3a1690264522/setup.py` & `pulumi_slack-0.4.3a1690907235/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.3a1690264522"
-PLUGIN_VERSION = "0.4.3-alpha.1690264522+39f74a1e"
+VERSION = "0.4.3a1690907235"
+PLUGIN_VERSION = "0.4.3-alpha.1690907235+edda2419"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'slack', PLUGIN_VERSION])
         except OSError as error:
```

