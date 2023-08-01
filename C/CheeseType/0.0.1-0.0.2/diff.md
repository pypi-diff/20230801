# Comparing `tmp/CheeseType-0.0.1.tar.gz` & `tmp/CheeseType-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseType-0.0.1.tar", last modified: Wed Jul 26 06:29:36 2023, max compression
+gzip compressed data, was "CheeseType-0.0.2.tar", last modified: Tue Aug  1 07:19:25 2023, max compression
```

## Comparing `CheeseType-0.0.1.tar` & `CheeseType-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-26 06:29:36.927402 CheeseType-0.0.1/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-26 06:29:36.926508 CheeseType-0.0.1/CheeseType/
--rw-r--r--   0 cheese     (501) staff       (20)     4143 2023-07-26 06:03:26.000000 CheeseType-0.0.1/CheeseType/__init__.py
--rw-r--r--   0 cheese     (501) staff       (20)     1923 2023-07-26 06:29:34.000000 CheeseType-0.0.1/CheeseType/network.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-07-26 06:29:36.927087 CheeseType-0.0.1/CheeseType.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     2410 2023-07-26 06:29:36.000000 CheeseType-0.0.1/CheeseType.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      207 2023-07-26 06:29:36.000000 CheeseType-0.0.1/CheeseType.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-07-26 06:29:36.000000 CheeseType-0.0.1/CheeseType.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       11 2023-07-26 06:29:36.000000 CheeseType-0.0.1/CheeseType.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 03:42:05.000000 CheeseType-0.0.1/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     2410 2023-07-26 06:29:36.927286 CheeseType-0.0.1/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     1961 2023-07-26 06:23:07.000000 CheeseType-0.0.1/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-07-26 06:29:36.927449 CheeseType-0.0.1/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      747 2023-07-26 03:56:53.000000 CheeseType-0.0.1/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:19:25.922930 CheeseType-0.0.2/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:19:25.922140 CheeseType-0.0.2/CheeseType/
+-rw-r--r--   0 cheese     (501) staff       (20)     4126 2023-07-31 15:41:12.000000 CheeseType-0.0.2/CheeseType/__init__.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1914 2023-07-31 08:37:23.000000 CheeseType-0.0.2/CheeseType/network.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-01 07:19:25.922633 CheeseType-0.0.2/CheeseType.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     2397 2023-08-01 07:19:25.000000 CheeseType-0.0.2/CheeseType.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      207 2023-08-01 07:19:25.000000 CheeseType-0.0.2/CheeseType.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-01 07:19:25.000000 CheeseType-0.0.2/CheeseType.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       11 2023-08-01 07:19:25.000000 CheeseType-0.0.2/CheeseType.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 03:42:05.000000 CheeseType-0.0.2/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     2397 2023-08-01 07:19:25.922824 CheeseType-0.0.2/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     1961 2023-07-26 06:23:07.000000 CheeseType-0.0.2/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-01 07:19:25.922973 CheeseType-0.0.2/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      734 2023-08-01 07:18:57.000000 CheeseType-0.0.2/setup.py
```

### Comparing `CheeseType-0.0.1/CheeseType/__init__.py` & `CheeseType-0.0.2/CheeseType/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os, sys
 from enum import Enum
 
-sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
+sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 
 class Bool:
     def __new__(cls, value):
         if value in [ True, 'true', 'True', 'TRUE' ]:
             return True
         if value in [ False, 'false', 'False', 'FALSE' ]:
             return False
```

### Comparing `CheeseType-0.0.1/CheeseType/network.py` & `CheeseType-0.0.2/CheeseType/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from CheeseType import NonNegativeInt
+from . import NonNegativeInt
 
 class Port(NonNegativeInt):
     def __new__(cls, value):
         error = ValueError(f'could not convert {value.__class__.__name__} to Port: \'{value}\'' if isinstance(value, str) else f'could not convert {value.__class__.__name__} to Port: {value}')
 
         if isinstance(value, Port):
             return value
```

### Comparing `CheeseType-0.0.1/CheeseType.egg-info/PKG-INFO` & `CheeseType-0.0.2/CheeseType.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: CheeseType
-Version: 0.0.1
+Version: 0.0.2
 Summary: 存放了一些常用自定义类型的库。
 Home-page: https://github.com/CheeseUnknown/CheeseType
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
-Keywords: web framework api
+Keywords: type
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **CheeseType**
```

### Comparing `CheeseType-0.0.1/LICENSE` & `CheeseType-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseType-0.0.1/PKG-INFO` & `CheeseType-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: CheeseType
-Version: 0.0.1
+Version: 0.0.2
 Summary: 存放了一些常用自定义类型的库。
 Home-page: https://github.com/CheeseUnknown/CheeseType
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
-Keywords: web framework api
+Keywords: type
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **CheeseType**
```

### Comparing `CheeseType-0.0.1/README.md` & `CheeseType-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `CheeseType-0.0.1/setup.py` & `CheeseType-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseType',
-    version = '0.0.1',
+    version = '0.0.2',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '存放了一些常用自定义类型的库。',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseType',
     license = 'MIT',
     classifiers = [
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.11'
     ],
-    keywords = 'web framework api',
+    keywords = 'type',
     python_requires = '>=3.11',
     install_requires = [],
     packages = setuptools.find_packages()
 )
```

