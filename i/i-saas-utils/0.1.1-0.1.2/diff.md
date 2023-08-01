# Comparing `tmp/i_saas_utils-0.1.1.tar.gz` & `tmp/i_saas_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i_saas_utils-0.1.1.tar", max compression
+gzip compressed data, was "i_saas_utils-0.1.2.tar", max compression
```

## Comparing `i_saas_utils-0.1.1.tar` & `i_saas_utils-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6254 2023-07-28 20:15:16.157658 i_saas_utils-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-28 15:49:56.000000 i_saas_utils-0.1.1/i_saas_utils/__init__.py
--rw-r--r--   0        0        0       28 2023-07-29 11:00:00.646286 i_saas_utils-0.1.1/i_saas_utils/ansible/__init__.py
--rw-r--r--   0        0        0      517 2023-07-29 11:08:59.134950 i_saas_utils-0.1.1/i_saas_utils/ansible/ansibl.py
--rw-r--r--   0        0        0       30 2023-07-29 14:27:09.403296 i_saas_utils-0.1.1/i_saas_utils/git/__init__.py
--rw-r--r--   0        0        0      680 2023-07-29 19:49:55.616690 i_saas_utils-0.1.1/i_saas_utils/git/git.py
--rw-r--r--   0        0        0     1297 2023-07-29 19:49:55.604690 i_saas_utils-0.1.1/i_saas_utils/git/project.py
--rw-r--r--   0        0        0       23 2023-07-29 11:01:01.438716 i_saas_utils-0.1.1/i_saas_utils/k8s/__init__.py
--rw-r--r--   0        0        0      916 2023-07-28 21:36:56.880915 i_saas_utils-0.1.1/i_saas_utils/k8s/kube.py
--rw-r--r--   0        0        0      134 2023-07-29 16:20:21.734883 i_saas_utils-0.1.1/i_saas_utils/saas/__init__.py
--rw-r--r--   0        0        0     3002 2023-08-01 16:38:00.722425 i_saas_utils-0.1.1/i_saas_utils/saas/saas.py
--rw-r--r--   0        0        0       57 2023-07-29 11:01:01.418716 i_saas_utils-0.1.1/i_saas_utils/templates/__init__.py
--rw-r--r--   0        0        0      646 2023-07-29 19:49:55.600690 i_saas_utils-0.1.1/i_saas_utils/templates/render.py
--rw-r--r--   0        0        0       71 2023-07-29 11:01:59.506737 i_saas_utils-0.1.1/i_saas_utils/types/__init__.py
--rw-r--r--   0        0        0      386 2023-08-01 17:18:14.449299 i_saas_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 i_saas_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6254 2023-07-28 20:15:16.157658 i_saas_utils-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 15:49:56.000000 i_saas_utils-0.1.2/i_saas_utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-29 11:00:00.646286 i_saas_utils-0.1.2/i_saas_utils/ansible/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-29 11:08:59.134950 i_saas_utils-0.1.2/i_saas_utils/ansible/ansibl.py
+-rw-r--r--   0        0        0       30 2023-07-29 14:27:09.403296 i_saas_utils-0.1.2/i_saas_utils/git/__init__.py
+-rw-r--r--   0        0        0      680 2023-07-29 19:49:55.616690 i_saas_utils-0.1.2/i_saas_utils/git/git.py
+-rw-r--r--   0        0        0     1297 2023-07-29 19:49:55.604690 i_saas_utils-0.1.2/i_saas_utils/git/project.py
+-rw-r--r--   0        0        0       23 2023-07-29 11:01:01.438716 i_saas_utils-0.1.2/i_saas_utils/k8s/__init__.py
+-rw-r--r--   0        0        0      916 2023-07-28 21:36:56.880915 i_saas_utils-0.1.2/i_saas_utils/k8s/kube.py
+-rw-r--r--   0        0        0      134 2023-07-29 16:20:21.734883 i_saas_utils-0.1.2/i_saas_utils/saas/__init__.py
+-rw-r--r--   0        0        0     3013 2023-08-01 18:30:59.609803 i_saas_utils-0.1.2/i_saas_utils/saas/saas.py
+-rw-r--r--   0        0        0       57 2023-07-29 11:01:01.418716 i_saas_utils-0.1.2/i_saas_utils/templates/__init__.py
+-rw-r--r--   0        0        0      646 2023-07-29 19:49:55.600690 i_saas_utils-0.1.2/i_saas_utils/templates/render.py
+-rw-r--r--   0        0        0       71 2023-07-29 11:01:59.506737 i_saas_utils-0.1.2/i_saas_utils/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-08-01 18:31:21.538258 i_saas_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 i_saas_utils-0.1.2/PKG-INFO
```

### Comparing `i_saas_utils-0.1.1/README.md` & `i_saas_utils-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.1/i_saas_utils/ansible/ansibl.py` & `i_saas_utils-0.1.2/i_saas_utils/ansible/ansibl.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.1/i_saas_utils/git/git.py` & `i_saas_utils-0.1.2/i_saas_utils/git/git.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.1/i_saas_utils/git/project.py` & `i_saas_utils-0.1.2/i_saas_utils/git/project.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.1/i_saas_utils/k8s/kube.py` & `i_saas_utils-0.1.2/i_saas_utils/k8s/kube.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.1/i_saas_utils/saas/saas.py` & `i_saas_utils-0.1.2/i_saas_utils/saas/saas.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from random import shuffle
 
 import dns.resolver
 import requests
 
 
 def get_list_dirs(path: str):
-    return list(filter(os.path.isdir, os.listdir(path)))
+    return [d for d in os.listdir(path) if os.path.isdir(os.path.join(path, d))]
 
 
-def get_list_files(source: str, short_name: bool = False) -> list[str]:
+def get_list_files(source: str, short_name: bool = False):
     list_files = []
     for path, dirs, files in os.walk(source):
         if short_name:
             short_path = os.path.relpath(path, source)
         else:
             short_path = path
```

### Comparing `i_saas_utils-0.1.1/i_saas_utils/templates/render.py` & `i_saas_utils-0.1.2/i_saas_utils/templates/render.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.1/PKG-INFO` & `i_saas_utils-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-saas-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Fedorov Stepan
 Author-email: fedorov.stepan2@wb.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dnspython (>=2.4.1,<3.0.0)
```

