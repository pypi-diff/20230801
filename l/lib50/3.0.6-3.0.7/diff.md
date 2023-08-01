# Comparing `tmp/lib50-3.0.6.tar.gz` & `tmp/lib50-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib50-3.0.6.tar", last modified: Fri Mar 24 21:29:06 2023, max compression
+gzip compressed data, was "lib50-3.0.7.tar", last modified: Tue Aug  1 12:27:13 2023, max compression
```

## Comparing `lib50-3.0.6.tar` & `lib50-3.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:29:06.961031 lib50-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-24 21:28:27.000000 lib50-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-24 21:28:27.000000 lib50-3.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-24 21:29:06.961031 lib50-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 21:28:27.000000 lib50-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:29:06.961031 lib50-3.0.6/lib50/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-24 21:28:27.000000 lib50-3.0.6/lib50/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-03-24 21:28:27.000000 lib50-3.0.6/lib50/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-24 21:28:27.000000 lib50-3.0.6/lib50/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-03-24 21:28:27.000000 lib50-3.0.6/lib50/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-03-24 21:28:27.000000 lib50-3.0.6/lib50/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-03-24 21:28:27.000000 lib50-3.0.6/lib50/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:29:06.957031 lib50-3.0.6/lib50/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:29:06.957031 lib50-3.0.6/lib50/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:29:06.961031 lib50-3.0.6/lib50/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-03-24 21:28:48.000000 lib50-3.0.6/lib50/locale/es/LC_MESSAGES/lib50.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-03-24 21:28:27.000000 lib50-3.0.6/lib50/locale/es/LC_MESSAGES/lib50.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:29:06.961031 lib50-3.0.6/lib50.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-24 21:29:06.000000 lib50-3.0.6/lib50.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-24 21:29:06.000000 lib50-3.0.6/lib50.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 21:29:06.000000 lib50-3.0.6/lib50.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-24 21:29:06.000000 lib50-3.0.6/lib50.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-24 21:29:06.000000 lib50-3.0.6/lib50.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-24 21:29:06.961031 lib50-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-24 21:28:27.000000 lib50-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:27:13.900869 lib50-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 12:26:34.000000 lib50-3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 12:26:34.000000 lib50-3.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-01 12:27:13.900869 lib50-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 12:26:34.000000 lib50-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:27:13.900869 lib50-3.0.7/lib50/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-01 12:26:34.000000 lib50-3.0.7/lib50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-08-01 12:26:34.000000 lib50-3.0.7/lib50/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-08-01 12:26:34.000000 lib50-3.0.7/lib50/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-08-01 12:26:34.000000 lib50-3.0.7/lib50/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-08-01 12:26:34.000000 lib50-3.0.7/lib50/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-01 12:26:34.000000 lib50-3.0.7/lib50/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:27:13.900869 lib50-3.0.7/lib50/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:27:13.900869 lib50-3.0.7/lib50/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:27:13.900869 lib50-3.0.7/lib50/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-01 12:26:47.000000 lib50-3.0.7/lib50/locale/es/LC_MESSAGES/lib50.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-08-01 12:26:34.000000 lib50-3.0.7/lib50/locale/es/LC_MESSAGES/lib50.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:27:13.900869 lib50-3.0.7/lib50.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-01 12:27:13.000000 lib50-3.0.7/lib50.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-01 12:27:13.000000 lib50-3.0.7/lib50.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:27:13.000000 lib50-3.0.7/lib50.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-01 12:27:13.000000 lib50-3.0.7/lib50.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 12:27:13.000000 lib50-3.0.7/lib50.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-01 12:27:13.900869 lib50-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-01 12:26:34.000000 lib50-3.0.7/setup.py
```

### Comparing `lib50-3.0.6/LICENSE` & `lib50-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/PKG-INFO` & `lib50-3.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib50
-Version: 3.0.6
+Version: 3.0.7
 Summary: This is lib50, CS50's own internal library used in many of its tools.
 Home-page: https://github.com/cs50/lib50
 Author: CS50
 Author-email: sysadmins@cs50.harvard.edu
 License: GPLv3
 Keywords: lib50
 Classifier: Intended Audience :: Education
```

### Comparing `lib50-3.0.6/lib50/__init__.py` & `lib50-3.0.7/lib50/__init__.py`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/lib50/_api.py` & `lib50-3.0.7/lib50/_api.py`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/lib50/_errors.py` & `lib50-3.0.7/lib50/_errors.py`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/lib50/authentication.py` & `lib50-3.0.7/lib50/authentication.py`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/lib50/config.py` & `lib50-3.0.7/lib50/config.py`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/lib50/crypto.py` & `lib50-3.0.7/lib50/crypto.py`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/lib50/locale/es/LC_MESSAGES/lib50.mo` & `lib50-3.0.7/lib50/locale/es/LC_MESSAGES/lib50.mo`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/lib50/locale/es/LC_MESSAGES/lib50.po` & `lib50-3.0.7/lib50/locale/es/LC_MESSAGES/lib50.po`

 * *Files identical despite different names*

### Comparing `lib50-3.0.6/lib50.egg-info/PKG-INFO` & `lib50-3.0.7/lib50.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib50
-Version: 3.0.6
+Version: 3.0.7
 Summary: This is lib50, CS50's own internal library used in many of its tools.
 Home-page: https://github.com/cs50/lib50
 Author: CS50
 Author-email: sysadmins@cs50.harvard.edu
 License: GPLv3
 Keywords: lib50
 Classifier: Intended Audience :: Education
```

### Comparing `lib50-3.0.6/setup.py` & `lib50-3.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     ],
     message_extractors = {
         'lib50': [('**.py', 'python', None),],
     },
     license="GPLv3",
     description="This is lib50, CS50's own internal library used in many of its tools.",
     long_description="This is lib50, CS50's own internal library used in many of its tools.",
-    install_requires=["attrs>=18.1,<21", "pexpect>=4.6,<5", "pyyaml>=3.10,<6", "requests>=2.13,<3", "termcolor>=1.1,<2", "jellyfish>=0.7,<1", "cryptography>=2.7"],
+    install_requires=["attrs>=18.1,<21", "pexpect>=4.6,<5", "pyyaml<7", "requests>=2.13,<3", "termcolor>=1.1,<2", "jellyfish>=0.7,<1", "cryptography>=2.7"],
     extras_require = {
         "develop": ["sphinx", "sphinx-autobuild", "sphinx_rtd_theme"]
     },
     keywords=["lib50"],
     name="lib50",
     python_requires=">= 3.6",
     packages=["lib50"],
     url="https://github.com/cs50/lib50",
-    version="3.0.6",
+    version="3.0.7",
     include_package_data=True
 )
```

