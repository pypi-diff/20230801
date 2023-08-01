# Comparing `tmp/gougleai-1.0.5.tar.gz` & `tmp/gougleai-1.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gougleai-1.0.5.tar", last modified: Tue Aug  1 02:38:42 2023, max compression
+gzip compressed data, was "dist\gougleai-1.0.5.1.tar", last modified: Tue Aug  1 10:57:32 2023, max compression
```

## Comparing `gougleai-1.0.5.tar` & `gougleai-1.0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:38:42.000000 gougleai-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-08-01 02:38:42.000000 gougleai-1.0.5/gougleai.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-01 02:38:42.000000 gougleai-1.0.5/gougleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1073 2023-08-01 02:38:42.000000 gougleai-1.0.5/gougleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-08-01 02:38:42.000000 gougleai-1.0.5/gougleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0      187 2023-08-01 02:38:42.000000 gougleai-1.0.5/gougleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:38:42.000000 gougleai-1.0.5/gougleai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2023-08-01 02:38:42.000000 gougleai-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      624 2023-08-01 02:35:51.000000 gougleai-1.0.5/README.md
--rw-rw-rw-   0        0        0      471 2023-08-01 02:38:42.000000 gougleai-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-08-01 02:34:31.000000 gougleai-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/
+drwxrwxrwx   0        0        0        0 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/gougleai.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/gougleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1632 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/gougleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/gougleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      177 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/gougleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/gougleai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1632 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-08-01 10:55:46.000000 gougleai-1.0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 10:57:32.000000 gougleai-1.0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-08-01 10:55:46.000000 gougleai-1.0.5.1/setup.py
```

### Comparing `gougleai-1.0.5/gougleai.egg-info/PKG-INFO` & `gougleai-1.0.5.1/gougleai.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: gougleai
-Version: 1.0.5
+Version: 1.0.5.1
 Summary: The Python package for Gougle AI API.
 Home-page: https://www.github.com/gougle-official/gougleai-python
 Author: Gougle AI LLC
 Author-email: gouglellc@gmail.com
 License: UNKNOWN
 Description: # Gougle AI API `python`
+        [![Upload Python Package](https://github.com/gougle-official/gougleai-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gougle-official/gougleai-python/actions/workflows/python-publish.yml)  
         The Gougle AI API include Gougle AI models.
         
         # Models
-        | Model Name | Model ID                   |
-        | ---------- | -------------------------- |
-        | GLT-1      | gougleai.models.glt.glt1   |
-        | GLT-1.0.5  | gougleai.models.glt.glt105 |
+        | Model Name     | Model ID                   | Model Type                          |
+        | -------------- | -------------------------- | ----------------------------------- |
+        | GLT-1          | gougleai.models.glt.glt1   | Chat Completion and Text Completion |
+        | GLT-1.0.5 Beta | gougleai.models.glt.glt105 | Chat Completion and Text Completion |
+        | GIC-1          | gougleai.models.gic.gic1   | Image Generation                    |
+        | GIC-1.0.5 Beta | gougleai.models.gic.gic105 | Image Generation                    |
         
         # Docs
-        [https://www.github.com/gougle-official/gougleai-python/DOCS.md](https://github.com/gougle-official/gougleai-python/blob/main/DOCS.md)
+        See [DOCS.md](https://github.com/gougle-official/gougleai-python/blob/main/DOCS.md) for the docs.
         
         # More spécifications
         To see more than about Gougle AI API, you can read https://www.github.com/gougle-official/gougleai for `all` or https://www.github.com/gougle-official/gougleai-javascript for `javascript`. 
+        
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gougleai-1.0.5/PKG-INFO` & `gougleai-1.0.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: gougleai
-Version: 1.0.5
+Version: 1.0.5.1
 Summary: The Python package for Gougle AI API.
 Home-page: https://www.github.com/gougle-official/gougleai-python
 Author: Gougle AI LLC
 Author-email: gouglellc@gmail.com
 License: UNKNOWN
 Description: # Gougle AI API `python`
+        [![Upload Python Package](https://github.com/gougle-official/gougleai-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/gougle-official/gougleai-python/actions/workflows/python-publish.yml)  
         The Gougle AI API include Gougle AI models.
         
         # Models
-        | Model Name | Model ID                   |
-        | ---------- | -------------------------- |
-        | GLT-1      | gougleai.models.glt.glt1   |
-        | GLT-1.0.5  | gougleai.models.glt.glt105 |
+        | Model Name     | Model ID                   | Model Type                          |
+        | -------------- | -------------------------- | ----------------------------------- |
+        | GLT-1          | gougleai.models.glt.glt1   | Chat Completion and Text Completion |
+        | GLT-1.0.5 Beta | gougleai.models.glt.glt105 | Chat Completion and Text Completion |
+        | GIC-1          | gougleai.models.gic.gic1   | Image Generation                    |
+        | GIC-1.0.5 Beta | gougleai.models.gic.gic105 | Image Generation                    |
         
         # Docs
-        [https://www.github.com/gougle-official/gougleai-python/DOCS.md](https://github.com/gougle-official/gougleai-python/blob/main/DOCS.md)
+        See [DOCS.md](https://github.com/gougle-official/gougleai-python/blob/main/DOCS.md) for the docs.
         
         # More spécifications
         To see more than about Gougle AI API, you can read https://www.github.com/gougle-official/gougleai for `all` or https://www.github.com/gougle-official/gougleai-javascript for `javascript`. 
+        
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

