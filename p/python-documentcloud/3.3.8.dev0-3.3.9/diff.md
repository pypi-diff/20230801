# Comparing `tmp/python-documentcloud-3.3.8.dev0.tar.gz` & `tmp/python-documentcloud-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-documentcloud-3.3.8.dev0.tar", last modified: Tue Feb 28 21:26:37 2023, max compression
+gzip compressed data, was "python-documentcloud-3.3.9.tar", last modified: Tue Mar 14 16:20:49 2023, max compression
```

## Comparing `python-documentcloud-3.3.8.dev0.tar` & `python-documentcloud-3.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-02-28 21:26:37.068323 python-documentcloud-3.3.8.dev0/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1151 2020-06-11 15:56:14.000000 python-documentcloud-3.3.8.dev0/LICENSE
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2136 2023-02-28 21:26:37.068323 python-documentcloud-3.3.8.dev0/PKG-INFO
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1175 2022-03-23 18:09:12.000000 python-documentcloud-3.3.8.dev0/README.md
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-02-28 21:26:37.064323 python-documentcloud-3.3.8.dev0/documentcloud/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      220 2020-06-13 15:35:49.000000 python-documentcloud-3.3.8.dev0/documentcloud/__init__.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)    10750 2023-02-28 21:26:30.000000 python-documentcloud-3.3.8.dev0/documentcloud/addon.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2712 2020-06-16 14:28:21.000000 python-documentcloud-3.3.8.dev0/documentcloud/annotations.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     7193 2023-02-21 18:27:59.000000 python-documentcloud-3.3.8.dev0/documentcloud/base.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     5974 2022-03-14 16:33:38.000000 python-documentcloud-3.3.8.dev0/documentcloud/client.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      256 2021-03-11 15:48:51.000000 python-documentcloud-3.3.8.dev0/documentcloud/constants.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)    15989 2023-02-24 21:34:15.000000 python-documentcloud-3.3.8.dev0/documentcloud/documents.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1270 2020-06-15 18:35:58.000000 python-documentcloud-3.3.8.dev0/documentcloud/exceptions.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      565 2020-06-15 18:35:58.000000 python-documentcloud-3.3.8.dev0/documentcloud/organizations.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     5392 2022-03-14 16:33:38.000000 python-documentcloud-3.3.8.dev0/documentcloud/projects.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1123 2020-06-15 18:35:58.000000 python-documentcloud-3.3.8.dev0/documentcloud/sections.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2012 2020-06-15 18:35:58.000000 python-documentcloud-3.3.8.dev0/documentcloud/toolbox.py
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      527 2020-06-15 18:35:58.000000 python-documentcloud-3.3.8.dev0/documentcloud/users.py
-drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-02-28 21:26:37.068323 python-documentcloud-3.3.8.dev0/python_documentcloud.egg-info/
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     2136 2023-02-28 21:26:37.000000 python-documentcloud-3.3.8.dev0/python_documentcloud.egg-info/PKG-INFO
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      592 2023-02-28 21:26:37.000000 python-documentcloud-3.3.8.dev0/python_documentcloud.egg-info/SOURCES.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)        1 2023-02-28 21:26:37.000000 python-documentcloud-3.3.8.dev0/python_documentcloud.egg-info/dependency_links.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      188 2023-02-28 21:26:37.000000 python-documentcloud-3.3.8.dev0/python_documentcloud.egg-info/requires.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)       14 2023-02-28 21:26:37.000000 python-documentcloud-3.3.8.dev0/python_documentcloud.egg-info/top_level.txt
--rw-rw-r--   0 mitch     (1000) mitch     (1000)      102 2023-02-28 21:26:37.068323 python-documentcloud-3.3.8.dev0/setup.cfg
--rw-rw-r--   0 mitch     (1000) mitch     (1000)     1670 2023-02-28 21:26:28.000000 python-documentcloud-3.3.8.dev0/setup.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-03-14 16:20:49.603093 python-documentcloud-3.3.9/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1151 2020-06-11 15:56:14.000000 python-documentcloud-3.3.9/LICENSE
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2131 2023-03-14 16:20:49.603093 python-documentcloud-3.3.9/PKG-INFO
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1175 2022-03-23 18:09:12.000000 python-documentcloud-3.3.9/README.md
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-03-14 16:20:49.599092 python-documentcloud-3.3.9/documentcloud/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      220 2020-06-13 15:35:49.000000 python-documentcloud-3.3.9/documentcloud/__init__.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)    10750 2023-03-14 12:52:00.000000 python-documentcloud-3.3.9/documentcloud/addon.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2712 2020-06-16 14:28:21.000000 python-documentcloud-3.3.9/documentcloud/annotations.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     7143 2023-03-14 16:17:17.000000 python-documentcloud-3.3.9/documentcloud/base.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     5974 2022-03-14 16:33:38.000000 python-documentcloud-3.3.9/documentcloud/client.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      256 2021-03-11 15:48:51.000000 python-documentcloud-3.3.9/documentcloud/constants.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)    15989 2023-02-24 21:34:15.000000 python-documentcloud-3.3.9/documentcloud/documents.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1270 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/exceptions.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      565 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/organizations.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     5392 2022-03-14 16:33:38.000000 python-documentcloud-3.3.9/documentcloud/projects.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1123 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/sections.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2012 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/toolbox.py
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      527 2020-06-15 18:35:58.000000 python-documentcloud-3.3.9/documentcloud/users.py
+drwxrwxr-x   0 mitch     (1000) mitch     (1000)        0 2023-03-14 16:20:49.603093 python-documentcloud-3.3.9/python_documentcloud.egg-info/
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     2131 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/PKG-INFO
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      592 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)        1 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      188 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/requires.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)       14 2023-03-14 16:20:49.000000 python-documentcloud-3.3.9/python_documentcloud.egg-info/top_level.txt
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)      102 2023-03-14 16:20:49.603093 python-documentcloud-3.3.9/setup.cfg
+-rw-rw-r--   0 mitch     (1000) mitch     (1000)     1665 2023-03-14 16:20:35.000000 python-documentcloud-3.3.9/setup.py
```

### Comparing `python-documentcloud-3.3.8.dev0/LICENSE` & `python-documentcloud-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/PKG-INFO` & `python-documentcloud-3.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-documentcloud
-Version: 3.3.8.dev0
+Version: 3.3.9
 Summary: A simple Python wrapper for the DocumentCloud API
 Home-page: https://github.com/muckrock/python-documentcloud
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-documentcloud-3.3.8.dev0/README.md` & `python-documentcloud-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/addon.py` & `python-documentcloud-3.3.9/documentcloud/addon.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/annotations.py` & `python-documentcloud-3.3.9/documentcloud/annotations.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/base.py` & `python-documentcloud-3.3.9/documentcloud/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,22 +50,20 @@
         if key < length:
             return self.results[key]
         elif self.next_url:
             return self.next[key - length]
         raise IndexError
 
     def __iter__(self):
-        for result in self.results:
-            yield result
-        if self.next_url:
-            # pylint: disable=not-an-iterable
-            for result in self.next:
-                yield result
-        else:
-            return
+        yield from self.results
+
+        api_results = self
+        while api_results.next_url:
+            api_results = api_results.next
+            yield from api_results.results
 
     def _fetch(self, url, next_=None, previous=None):
         if url:
             response = self.client.get(url, full_url=True)
             return APIResults(
                 self.resource,
                 self.client,
```

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/client.py` & `python-documentcloud-3.3.9/documentcloud/client.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/documents.py` & `python-documentcloud-3.3.9/documentcloud/documents.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/exceptions.py` & `python-documentcloud-3.3.9/documentcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/organizations.py` & `python-documentcloud-3.3.9/documentcloud/organizations.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/projects.py` & `python-documentcloud-3.3.9/documentcloud/projects.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/sections.py` & `python-documentcloud-3.3.9/documentcloud/sections.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/toolbox.py` & `python-documentcloud-3.3.9/documentcloud/toolbox.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/documentcloud/users.py` & `python-documentcloud-3.3.9/documentcloud/users.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/python_documentcloud.egg-info/PKG-INFO` & `python-documentcloud-3.3.9/python_documentcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-documentcloud
-Version: 3.3.8.dev0
+Version: 3.3.9
 Summary: A simple Python wrapper for the DocumentCloud API
 Home-page: https://github.com/muckrock/python-documentcloud
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-documentcloud-3.3.8.dev0/python_documentcloud.egg-info/SOURCES.txt` & `python-documentcloud-3.3.9/python_documentcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-documentcloud-3.3.8.dev0/setup.py` & `python-documentcloud-3.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='python-documentcloud',
-    version='3.3.8.dev0',
+    version='3.3.9',
     description='A simple Python wrapper for the DocumentCloud API',
     author='Mitchell Kotler',
     author_email='mitch@muckrock.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/muckrock/python-documentcloud',
     license="MIT",
```

