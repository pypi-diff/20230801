# Comparing `tmp/deploymenthub-2.6.tar.gz` & `tmp/deploymenthub-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymenthub-2.6.tar", last modified: Mon Jul 31 22:35:53 2023, max compression
+gzip compressed data, was "deploymenthub-2.7.tar", last modified: Mon Jul 31 22:43:50 2023, max compression
```

## Comparing `deploymenthub-2.6.tar` & `deploymenthub-2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:35:53.754077 deploymenthub-2.6/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.6/LICENSE.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:35:53.753957 deploymenthub-2.6/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.6/README.md
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:35:53.753228 deploymenthub-2.6/bin/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1556 2023-07-31 22:34:54.000000 deploymenthub-2.6/bin/deploymenthub
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:35:53.753798 deploymenthub-2.6/deploymenthub.egg-info/
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:35:53.000000 deploymenthub-2.6/deploymenthub.egg-info/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-31 22:35:53.000000 deploymenthub-2.6/deploymenthub.egg-info/SOURCES.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:35:53.000000 deploymenthub-2.6/deploymenthub.egg-info/dependency_links.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:35:53.000000 deploymenthub-2.6/deploymenthub.egg-info/top_level.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-31 22:35:53.754113 deploymenthub-2.6/setup.cfg
--rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-31 22:35:23.000000 deploymenthub-2.6/setup.py
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:43:50.241651 deploymenthub-2.7/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.7/LICENSE.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:43:50.241526 deploymenthub-2.7/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.7/README.md
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:43:50.240678 deploymenthub-2.7/bin/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1611 2023-07-31 22:42:50.000000 deploymenthub-2.7/bin/deploymenthub
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-31 22:43:50.241355 deploymenthub-2.7/deploymenthub.egg-info/
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-31 22:43:50.000000 deploymenthub-2.7/deploymenthub.egg-info/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-31 22:43:50.000000 deploymenthub-2.7/deploymenthub.egg-info/SOURCES.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:43:50.000000 deploymenthub-2.7/deploymenthub.egg-info/dependency_links.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-31 22:43:50.000000 deploymenthub-2.7/deploymenthub.egg-info/top_level.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-31 22:43:50.241689 deploymenthub-2.7/setup.cfg
+-rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-31 22:43:48.000000 deploymenthub-2.7/setup.py
```

### Comparing `deploymenthub-2.6/LICENSE.txt` & `deploymenthub-2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deploymenthub-2.6/bin/deploymenthub` & `deploymenthub-2.7/bin/deploymenthub`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,30 @@
     branch = args.branch
     verbose = args.verbose
     url = "http://192.168.0.216:5555"
 
     list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops', 'homebridge','deployment-hub-ui']
 
     if project in list_of_projects:
-        if branch is None:
+        command = None
+        if verbose:
             command = ('curl ' + url + '/' + project + '/' + action + '/')
         else:
-            command = ('curl ' + url + '/' + project + '/' + action + '/' + branch + '/')
+            command = ('curl -s ' + url + '/' + project + '/' + action + '/')
+
+        if branch is not None:
+            command += branch + '/'
 
         if verbose:
             command_list = json.loads(os.popen(command).read())
             for commandRow in command_list:
                 print(commandRow)
+
         else:
-            os.system(command + " > /dev/null")
+            os.popen(command)
 
     else:
         print("Project does not exist!")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `deploymenthub-2.6/setup.py` & `deploymenthub-2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="deploymenthub",
-    version="2.6",
+    version="2.7",
     description='A CLI client for deployment-hub server.',
     license='MIT',
     author='Jared Wines',
     author_email='contact@jaredwines.com',
     url='https://github.com/jaredwines/deployment-hub-cli-client',
     packages=find_packages(exclude=['tests']),
     scripts=['bin/deploymenthub'],
```

