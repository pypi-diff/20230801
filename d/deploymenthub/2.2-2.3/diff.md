# Comparing `tmp/deploymenthub-2.2.tar.gz` & `tmp/deploymenthub-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymenthub-2.2.tar", last modified: Fri Jul 28 18:38:39 2023, max compression
+gzip compressed data, was "deploymenthub-2.3.tar", last modified: Mon Jul 31 22:00:00 2023, max compression
```

## Comparing `deploymenthub-2.2.tar` & `deploymenthub-2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:38:39.422835 deploymenthub-2.2/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.2/LICENSE.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:38:39.422712 deploymenthub-2.2/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.2/README.md
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:38:39.421990 deploymenthub-2.2/bin/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1313 2023-07-28 18:35:59.000000 deploymenthub-2.2/bin/deploymenthub
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:38:39.422552 deploymenthub-2.2/deploymenthub.egg-info/
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:38:39.000000 deploymenthub-2.2/deploymenthub.egg-info/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-28 18:38:39.000000 deploymenthub-2.2/deploymenthub.egg-info/SOURCES.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:38:39.000000 deploymenthub-2.2/deploymenthub.egg-info/dependency_links.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:38:39.000000 deploymenthub-2.2/deploymenthub.egg-info/top_level.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-28 18:38:39.422874 deploymenthub-2.2/setup.cfg
--rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-28 18:38:27.000000 deploymenthub-2.2/setup.py
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:00:00.261521 deploymenthub-2.3/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.3/LICENSE.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:00:00.261404 deploymenthub-2.3/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.3/README.md
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:00:00.260594 deploymenthub-2.3/bin/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1533 2023-07-31 21:59:39.000000 deploymenthub-2.3/bin/deploymenthub
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:00:00.261231 deploymenthub-2.3/deploymenthub.egg-info/
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:00:00.000000 deploymenthub-2.3/deploymenthub.egg-info/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-31 22:00:00.000000 deploymenthub-2.3/deploymenthub.egg-info/SOURCES.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:00:00.000000 deploymenthub-2.3/deploymenthub.egg-info/dependency_links.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:00:00.000000 deploymenthub-2.3/deploymenthub.egg-info/top_level.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-31 22:00:00.261558 deploymenthub-2.3/setup.cfg
+-rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-31 21:59:39.000000 deploymenthub-2.3/setup.py
```

### Comparing `deploymenthub-2.2/LICENSE.txt` & `deploymenthub-2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deploymenthub-2.2/bin/deploymenthub` & `deploymenthub-2.3/bin/deploymenthub`

 * *Files 18% similar despite different names*

```diff
@@ -9,34 +9,40 @@
     parser = argparse.ArgumentParser(description='CLI client for Deployment Hub.')
     parser.add_argument('--project', '-p', required=True,
                         help='Name of the project you want to deploy or manage.')
     parser.add_argument('--action', '-a', required=True,
                         help='The action that is requested for the project.')
     parser.add_argument('--branch', '-b',
                         help='Branch you want to deploy.')
+    parser.add_argument('--verbose', '-v', action='store_true',
+                        help='Run in verbose mode.')
     parser.parse_args()
     args = parser.parse_args()
 
     project = args.project
     action = args.action
     branch = args.branch
-    url = "http://192.168.0.216:5000"
+    verbose = args.verbose
+    url = "http://192.168.0.216:5555"
 
     list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops', 'homebridge','deployment-hub-ui']
 
     if project in list_of_projects:
         if branch is None:
             command = ('curl ' + url + '/' + project + '/' + action + '/')
         else:
             command = ('curl ' + url + '/' + project + '/' + action + '/' + branch + '/')
 
-        command_list = json.loads(os.popen(command).read())
+        if verbose:
+            command_list = json.loads(os.popen(command).read())
+            for command in command_list:
+                print(command)
 
-        for command in command_list:
-            print(command)
+        else:
+            os.popen(command)
 
     else:
         print("Project does not exist!")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `deploymenthub-2.2/setup.py` & `deploymenthub-2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="deploymenthub",
-    version="2.2",
+    version="2.3",
     description='A CLI client for deployment-hub server.',
     license='MIT',
     author='Jared Wines',
     author_email='contact@jaredwines.com',
     url='https://github.com/jaredwines/deployment-hub-cli-client',
     packages=find_packages(exclude=['tests']),
     scripts=['bin/deploymenthub'],
```

