# Comparing `tmp/canvas_langchain-0.1.tar.gz` & `tmp/canvas_langchain-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas_langchain-0.1.tar", last modified: Mon Jul 31 20:40:03 2023, max compression
+gzip compressed data, was "canvas_langchain-0.2.tar", last modified: Tue Aug  1 12:59:18 2023, max compression
```

## Comparing `canvas_langchain-0.1.tar` & `canvas_langchain-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2023-07-31 20:40:03.108381 canvas_langchain-0.1/
--rw-r--r--   0 jparisea   (501) staff       (20)    35148 2023-07-31 20:28:17.000000 canvas_langchain-0.1/LICENSE.txt
--rw-r--r--   0 jparisea   (501) staff       (20)     1805 2023-07-31 20:40:03.108221 canvas_langchain-0.1/PKG-INFO
--rw-r--r--   0 jparisea   (501) staff       (20)     1372 2023-07-31 19:15:41.000000 canvas_langchain-0.1/README.md
-drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2023-07-31 20:40:03.107113 canvas_langchain-0.1/canvas_langchain/
--rw-r--r--   0 jparisea   (501) staff       (20)        0 2023-07-31 15:52:56.000000 canvas_langchain-0.1/canvas_langchain/__init__.py
--rw-r--r--   0 jparisea   (501) staff       (20)    18459 2023-07-31 19:38:48.000000 canvas_langchain-0.1/canvas_langchain/canvas.py
-drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2023-07-31 20:40:03.108015 canvas_langchain-0.1/canvas_langchain.egg-info/
--rw-r--r--   0 jparisea   (501) staff       (20)     1805 2023-07-31 20:40:03.000000 canvas_langchain-0.1/canvas_langchain.egg-info/PKG-INFO
--rw-r--r--   0 jparisea   (501) staff       (20)      285 2023-07-31 20:40:03.000000 canvas_langchain-0.1/canvas_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 jparisea   (501) staff       (20)        1 2023-07-31 20:40:03.000000 canvas_langchain-0.1/canvas_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 jparisea   (501) staff       (20)       69 2023-07-31 20:40:03.000000 canvas_langchain-0.1/canvas_langchain.egg-info/requires.txt
--rw-r--r--   0 jparisea   (501) staff       (20)       17 2023-07-31 20:40:03.000000 canvas_langchain-0.1/canvas_langchain.egg-info/top_level.txt
--rw-r--r--   0 jparisea   (501) staff       (20)       38 2023-07-31 20:40:03.108429 canvas_langchain-0.1/setup.cfg
--rw-r--r--   0 jparisea   (501) staff       (20)      763 2023-07-31 20:39:07.000000 canvas_langchain-0.1/setup.py
+drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2023-08-01 12:59:18.000979 canvas_langchain-0.2/
+-rw-r--r--   0 jparisea   (501) staff       (20)    35148 2023-07-31 20:28:17.000000 canvas_langchain-0.2/LICENSE.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)     1805 2023-08-01 12:59:18.000854 canvas_langchain-0.2/PKG-INFO
+-rw-r--r--   0 jparisea   (501) staff       (20)     1372 2023-07-31 19:15:41.000000 canvas_langchain-0.2/README.md
+drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2023-08-01 12:59:18.000018 canvas_langchain-0.2/canvas_langchain/
+-rw-r--r--   0 jparisea   (501) staff       (20)        0 2023-07-31 15:52:56.000000 canvas_langchain-0.2/canvas_langchain/__init__.py
+-rw-r--r--   0 jparisea   (501) staff       (20)    18459 2023-07-31 19:38:48.000000 canvas_langchain-0.2/canvas_langchain/canvas.py
+drwxr-xr-x   0 jparisea   (501) staff       (20)        0 2023-08-01 12:59:18.000686 canvas_langchain-0.2/canvas_langchain.egg-info/
+-rw-r--r--   0 jparisea   (501) staff       (20)     1805 2023-08-01 12:59:17.000000 canvas_langchain-0.2/canvas_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 jparisea   (501) staff       (20)      285 2023-08-01 12:59:17.000000 canvas_langchain-0.2/canvas_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)        1 2023-08-01 12:59:17.000000 canvas_langchain-0.2/canvas_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)       78 2023-08-01 12:59:17.000000 canvas_langchain-0.2/canvas_langchain.egg-info/requires.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)       17 2023-08-01 12:59:17.000000 canvas_langchain-0.2/canvas_langchain.egg-info/top_level.txt
+-rw-r--r--   0 jparisea   (501) staff       (20)       38 2023-08-01 12:59:18.001023 canvas_langchain-0.2/setup.cfg
+-rw-r--r--   0 jparisea   (501) staff       (20)      783 2023-08-01 12:55:06.000000 canvas_langchain-0.2/setup.py
```

### Comparing `canvas_langchain-0.1/LICENSE.txt` & `canvas_langchain-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `canvas_langchain-0.1/PKG-INFO` & `canvas_langchain-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas_langchain
-Version: 0.1
+Version: 0.2
 Summary: A canvas langchain integration
 Home-page: https://github.com/umich-its-ai/langchain-doc-canvas
 Author: University of Michigan
 Author-email: noreply@umich.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.8.1
```

### Comparing `canvas_langchain-0.1/README.md` & `canvas_langchain-0.2/README.md`

 * *Files identical despite different names*

### Comparing `canvas_langchain-0.1/canvas_langchain/canvas.py` & `canvas_langchain-0.2/canvas_langchain/canvas.py`

 * *Files identical despite different names*

### Comparing `canvas_langchain-0.1/canvas_langchain.egg-info/PKG-INFO` & `canvas_langchain-0.2/canvas_langchain.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas-langchain
-Version: 0.1
+Version: 0.2
 Summary: A canvas langchain integration
 Home-page: https://github.com/umich-its-ai/langchain-doc-canvas
 Author: University of Michigan
 Author-email: noreply@umich.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.8.1
```

### Comparing `canvas_langchain-0.1/setup.py` & `canvas_langchain-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='canvas_langchain',
-    version='0.1',
+    version='0.2',
     description='A canvas langchain integration',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='University of Michigan',
     author_email='noreply@umich.edu',
     url='https://github.com/umich-its-ai/langchain-doc-canvas',
     packages=find_packages(),
@@ -17,11 +17,12 @@
     install_requires=[
         'langchain',
         'unstructured',
         'canvasapi',
         'beautifulsoup4',
         'lxml',
         'PyPDF2',
+        'docx2txt',
         'striprtf'
     ],
     python_requires='>=3.8.1',
 )
```

