# Comparing `tmp/list_packages-1.0.6.tar.gz` & `tmp/list_packages-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_packages-1.0.6.tar", last modified: Tue Aug  1 12:14:28 2023, max compression
+gzip compressed data, was "list_packages-1.0.7.tar", last modified: Tue Aug  1 13:54:54 2023, max compression
```

## Comparing `list_packages-1.0.6.tar` & `list_packages-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:14:28.005318 list_packages-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 12:14:17.000000 list_packages-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 12:14:17.000000 list_packages-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-01 12:14:28.005318 list_packages-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-01 12:14:17.000000 list_packages-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:14:28.005318 list_packages-1.0.6/list_packages/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 12:14:17.000000 list_packages-1.0.6/list_packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 12:14:17.000000 list_packages-1.0.6/list_packages/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:14:28.005318 list_packages-1.0.6/list_packages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-01 12:14:27.000000 list_packages-1.0.6/list_packages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 12:14:28.000000 list_packages-1.0.6/list_packages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:14:27.000000 list_packages-1.0.6/list_packages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 12:14:27.000000 list_packages-1.0.6/list_packages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 12:14:27.000000 list_packages-1.0.6/list_packages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:14:28.005318 list_packages-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 12:14:17.000000 list_packages-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:14:28.005318 list_packages-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 12:14:17.000000 list_packages-1.0.6/tests/test_list_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:54:54.194581 list_packages-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 13:54:45.000000 list_packages-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 13:54:45.000000 list_packages-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 13:54:54.194581 list_packages-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-01 13:54:45.000000 list_packages-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:54:54.194581 list_packages-1.0.7/list_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 13:54:45.000000 list_packages-1.0.7/list_packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 13:54:45.000000 list_packages-1.0.7/list_packages/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:54:54.194581 list_packages-1.0.7/list_packages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 13:54:54.000000 list_packages-1.0.7/list_packages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:54:54.194581 list_packages-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 13:54:45.000000 list_packages-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:54:54.194581 list_packages-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 13:54:45.000000 list_packages-1.0.7/tests/test_list_packages.py
```

### Comparing `list_packages-1.0.6/LICENSE` & `list_packages-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `list_packages-1.0.6/PKG-INFO` & `list_packages-1.0.7/list_packages.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: list_packages
-Version: 1.0.6
+Name: list-packages
+Version: 1.0.7
 Summary: A package to list all the installed Python packages and their dependencies
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
@@ -72,14 +72,20 @@
 ``` bash
 Package                 Dependency
 setuptools==59.6.0      None
 Jinja2==3.1.2           markupsafe>=2.0
 requests==2.31.0        charset-normalizer<4,>=2,certifi>=2017.4.17,urllib3<3,>=1.21.1,idna<4,>=2.5
 ```
 
+The output can also be obtained in `json` format by using the following command in the terminal
+
+``` bash
+list_packages json
+```
+
 ### Python script/Notebook
 
 By default, the function returns a list of dictionaries containing package information. Each dictionary has the following keys:
 
 - package: Package name (str)
 - version: Package version (str)
 - depends: List of dictionaries containing package information (list)
```

### Comparing `list_packages-1.0.6/README.md` & `list_packages-1.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,20 @@
 ``` bash
 Package                 Dependency
 setuptools==59.6.0      None
 Jinja2==3.1.2           markupsafe>=2.0
 requests==2.31.0        charset-normalizer<4,>=2,certifi>=2017.4.17,urllib3<3,>=1.21.1,idna<4,>=2.5
 ```
 
+The output can also be obtained in `json` format by using the following command in the terminal
+
+``` bash
+list_packages json
+```
+
 ### Python script/Notebook
 
 By default, the function returns a list of dictionaries containing package information. Each dictionary has the following keys:
 
 - package: Package name (str)
 - version: Package version (str)
 - depends: List of dictionaries containing package information (list)
```

### Comparing `list_packages-1.0.6/list_packages/main.py` & `list_packages-1.0.7/list_packages/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,31 +46,14 @@
 
 
 def command_line():
     """
     :meta private:
     """
     installed_packages = list_installed_packages()
-    print("Package\tDependency")
-    for package in installed_packages:
-        dep_list = []
-        dep_string = None
-        if package['depends']:
-            for dep in package['depends']:
-                if dep['version']:
-                    dep_list.append(dep['package']+dep['version'])
-                else:
-                    dep_list.append(dep['package']+'')
-        if dep_list:
-            dep_string = ','.join(dep_list)
-        print(f"{package['package']}=={package['version']}\t{dep_string}")
-
-
-if __name__ == '__main__':
-    installed_packages = list_installed_packages()
     if len(sys.argv) > 1 and sys.argv[1] == 'json':
         json_string = json.dumps(installed_packages, indent=2)
         print(json_string)
     else:
         print("Package\tDependency")
         for package in installed_packages:
             dep_list = []
@@ -80,7 +63,11 @@
                     if dep['version']:
                         dep_list.append(dep['package']+dep['version'])
                     else:
                         dep_list.append(dep['package']+'')
             if dep_list:
                 dep_string = ','.join(dep_list)
             print(f"{package['package']}=={package['version']}\t{dep_string}")
+
+
+if __name__ == '__main__':
+    command_line()
```

### Comparing `list_packages-1.0.6/list_packages.egg-info/PKG-INFO` & `list_packages-1.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: list-packages
-Version: 1.0.6
+Name: list_packages
+Version: 1.0.7
 Summary: A package to list all the installed Python packages and their dependencies
 Home-page: https://github.com/maurya-anand/py-list-packages
 Author: Anand Maurya
 Author-email: anandmaurya@hotmail.com
 License: MIT
 Platform: Any
 Classifier: License :: OSI Approved :: MIT License
@@ -72,14 +72,20 @@
 ``` bash
 Package                 Dependency
 setuptools==59.6.0      None
 Jinja2==3.1.2           markupsafe>=2.0
 requests==2.31.0        charset-normalizer<4,>=2,certifi>=2017.4.17,urllib3<3,>=1.21.1,idna<4,>=2.5
 ```
 
+The output can also be obtained in `json` format by using the following command in the terminal
+
+``` bash
+list_packages json
+```
+
 ### Python script/Notebook
 
 By default, the function returns a list of dictionaries containing package information. Each dictionary has the following keys:
 
 - package: Package name (str)
 - version: Package version (str)
 - depends: List of dictionaries containing package information (list)
```

### Comparing `list_packages-1.0.6/setup.py` & `list_packages-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='list_packages',
-    version='1.0.6',
+    version='1.0.7',
     description='A package to list all the installed Python packages and their dependencies',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Anand Maurya',
     author_email='anandmaurya@hotmail.com',
     platforms=['Any'],
     packages=find_packages(),
```

### Comparing `list_packages-1.0.6/tests/test_list_packages.py` & `list_packages-1.0.7/tests/test_list_packages.py`

 * *Files identical despite different names*

