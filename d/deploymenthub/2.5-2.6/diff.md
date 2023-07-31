# Comparing `tmp/deploymenthub-2.5.tar.gz` & `tmp/deploymenthub-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymenthub-2.5.tar", last modified: Mon Jul 31 22:29:16 2023, max compression
+gzip compressed data, was "deploymenthub-2.6.tar", last modified: Mon Jul 31 22:35:53 2023, max compression
```

## Comparing `deploymenthub-2.5.tar` & `deploymenthub-2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:29:16.745836 deploymenthub-2.5/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.5/LICENSE.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:29:16.745715 deploymenthub-2.5/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.5/README.md
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:29:16.744970 deploymenthub-2.5/bin/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1516 2023-07-31 22:28:46.000000 deploymenthub-2.5/bin/deploymenthub
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:29:16.745532 deploymenthub-2.5/deploymenthub.egg-info/
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:29:16.000000 deploymenthub-2.5/deploymenthub.egg-info/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-31 22:29:16.000000 deploymenthub-2.5/deploymenthub.egg-info/SOURCES.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:29:16.000000 deploymenthub-2.5/deploymenthub.egg-info/dependency_links.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:29:16.000000 deploymenthub-2.5/deploymenthub.egg-info/top_level.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-31 22:29:16.745871 deploymenthub-2.5/setup.cfg
--rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-31 22:28:46.000000 deploymenthub-2.5/setup.py
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:35:53.754077 deploymenthub-2.6/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.6/LICENSE.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:35:53.753957 deploymenthub-2.6/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.6/README.md
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:35:53.753228 deploymenthub-2.6/bin/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1556 2023-07-31 22:34:54.000000 deploymenthub-2.6/bin/deploymenthub
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:35:53.753798 deploymenthub-2.6/deploymenthub.egg-info/
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:35:53.000000 deploymenthub-2.6/deploymenthub.egg-info/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-31 22:35:53.000000 deploymenthub-2.6/deploymenthub.egg-info/SOURCES.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:35:53.000000 deploymenthub-2.6/deploymenthub.egg-info/dependency_links.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:35:53.000000 deploymenthub-2.6/deploymenthub.egg-info/top_level.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-31 22:35:53.754113 deploymenthub-2.6/setup.cfg
+-rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-31 22:35:23.000000 deploymenthub-2.6/setup.py
```

### Comparing `deploymenthub-2.5/LICENSE.txt` & `deploymenthub-2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deploymenthub-2.5/bin/deploymenthub` & `deploymenthub-2.6/bin/deploymenthub`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import argparse
-import json
 import os
+import json
 
 
 def main():
     parser = argparse.ArgumentParser(description='CLI client for Deployment Hub.')
     parser.add_argument('--project', '-p', required=True,
                         help='Name of the project you want to deploy or manage.')
     parser.add_argument('--action', '-a', required=True,
@@ -20,28 +20,28 @@
 
     project = args.project
     action = args.action
     branch = args.branch
     verbose = args.verbose
     url = "http://192.168.0.216:5555"
 
-    list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops',
-                        'homebridge', 'deployment-hub-ui']
+    list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops', 'homebridge','deployment-hub-ui']
 
     if project in list_of_projects:
         if branch is None:
             command = ('curl ' + url + '/' + project + '/' + action + '/')
         else:
             command = ('curl ' + url + '/' + project + '/' + action + '/' + branch + '/')
 
-        command_list = json.loads(os.popen(command).read())
-
         if verbose:
+            command_list = json.loads(os.popen(command).read())
             for commandRow in command_list:
                 print(commandRow)
+        else:
+            os.system(command + " > /dev/null")
 
     else:
         print("Project does not exist!")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `deploymenthub-2.5/setup.py` & `deploymenthub-2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="deploymenthub",
-    version="2.5",
+    version="2.6",
     description='A CLI client for deployment-hub server.',
     license='MIT',
     author='Jared Wines',
     author_email='contact@jaredwines.com',
     url='https://github.com/jaredwines/deployment-hub-cli-client',
     packages=find_packages(exclude=['tests']),
     scripts=['bin/deploymenthub'],
```

