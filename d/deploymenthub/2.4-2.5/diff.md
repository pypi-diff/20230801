# Comparing `tmp/deploymenthub-2.4.tar.gz` & `tmp/deploymenthub-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymenthub-2.4.tar", last modified: Mon Jul 31 22:26:54 2023, max compression
+gzip compressed data, was "deploymenthub-2.5.tar", last modified: Mon Jul 31 22:29:16 2023, max compression
```

## Comparing `deploymenthub-2.4.tar` & `deploymenthub-2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:26:54.223513 deploymenthub-2.4/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.4/LICENSE.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:26:54.223408 deploymenthub-2.4/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.4/README.md
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:26:54.222789 deploymenthub-2.4/bin/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1616 2023-07-31 22:26:29.000000 deploymenthub-2.4/bin/deploymenthub
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:26:54.223251 deploymenthub-2.4/deploymenthub.egg-info/
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:26:54.000000 deploymenthub-2.4/deploymenthub.egg-info/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-31 22:26:54.000000 deploymenthub-2.4/deploymenthub.egg-info/SOURCES.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:26:54.000000 deploymenthub-2.4/deploymenthub.egg-info/dependency_links.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:26:54.000000 deploymenthub-2.4/deploymenthub.egg-info/top_level.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-31 22:26:54.223553 deploymenthub-2.4/setup.cfg
--rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-31 22:26:29.000000 deploymenthub-2.4/setup.py
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:29:16.745836 deploymenthub-2.5/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.5/LICENSE.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:29:16.745715 deploymenthub-2.5/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.5/README.md
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:29:16.744970 deploymenthub-2.5/bin/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1516 2023-07-31 22:28:46.000000 deploymenthub-2.5/bin/deploymenthub
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:29:16.745532 deploymenthub-2.5/deploymenthub.egg-info/
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:29:16.000000 deploymenthub-2.5/deploymenthub.egg-info/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-31 22:29:16.000000 deploymenthub-2.5/deploymenthub.egg-info/SOURCES.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:29:16.000000 deploymenthub-2.5/deploymenthub.egg-info/dependency_links.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:29:16.000000 deploymenthub-2.5/deploymenthub.egg-info/top_level.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-31 22:29:16.745871 deploymenthub-2.5/setup.cfg
+-rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-31 22:28:46.000000 deploymenthub-2.5/setup.py
```

### Comparing `deploymenthub-2.4/LICENSE.txt` & `deploymenthub-2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deploymenthub-2.4/bin/deploymenthub` & `deploymenthub-2.5/bin/deploymenthub`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import argparse
-import os
 import json
+import os
 
 
 def main():
     parser = argparse.ArgumentParser(description='CLI client for Deployment Hub.')
     parser.add_argument('--project', '-p', required=True,
                         help='Name of the project you want to deploy or manage.')
     parser.add_argument('--action', '-a', required=True,
@@ -20,32 +20,28 @@
 
     project = args.project
     action = args.action
     branch = args.branch
     verbose = args.verbose
     url = "http://192.168.0.216:5555"
 
-    #http://192.168.0.216:5555/home-assistant/start/
-    list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops', 'homebridge','deployment-hub-ui']
+    list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops',
+                        'homebridge', 'deployment-hub-ui']
 
     if project in list_of_projects:
         if branch is None:
             command = ('curl ' + url + '/' + project + '/' + action + '/')
         else:
             command = ('curl ' + url + '/' + project + '/' + action + '/' + branch + '/')
 
-        print(command)
+        command_list = json.loads(os.popen(command).read())
 
         if verbose:
-            command_list = json.loads(os.popen(command).read())
             for commandRow in command_list:
                 print(commandRow)
 
-        else:
-            os.popen(command)
-
     else:
         print("Project does not exist!")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `deploymenthub-2.4/setup.py` & `deploymenthub-2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="deploymenthub",
-    version="2.4",
+    version="2.5",
     description='A CLI client for deployment-hub server.',
     license='MIT',
     author='Jared Wines',
     author_email='contact@jaredwines.com',
     url='https://github.com/jaredwines/deployment-hub-cli-client',
     packages=find_packages(exclude=['tests']),
     scripts=['bin/deploymenthub'],
```

