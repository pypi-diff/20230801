# Comparing `tmp/openai_parallel_toolkit-1.1.0-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,17 @@
-Zip file size: 6584 bytes, number of entries: 7
+Zip file size: 12918 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       77 b- defN 23-Jul-28 11:58 openai_parallel_toolkit/__init__.py
 -rw-r--r--  2.0 unx     3100 b- defN 23-Jul-31 02:05 openai_parallel_toolkit/main.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     8218 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      644 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/RECORD
-7 files, 13218 bytes uncompressed, 5420 bytes compressed:  59.0%
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 07:30 openai_parallel_toolkit/api/__init__.py
+-rw-r--r--  2.0 unx     3809 b- defN 23-Jul-29 05:11 openai_parallel_toolkit/api/keys.py
+-rw-r--r--  2.0 unx     1348 b- defN 23-Jul-27 06:52 openai_parallel_toolkit/api/model.py
+-rw-r--r--  2.0 unx     4504 b- defN 23-Jul-29 02:34 openai_parallel_toolkit/api/request.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 07:33 openai_parallel_toolkit/utils/__init__.py
+-rw-r--r--  2.0 unx     1488 b- defN 23-Jul-28 13:01 openai_parallel_toolkit/utils/logger.py
+-rw-r--r--  2.0 unx      424 b- defN 23-Jul-28 13:01 openai_parallel_toolkit/utils/process_bar.py
+-rw-r--r--  2.0 unx     3036 b- defN 23-Aug-01 07:32 openai_parallel_toolkit/utils/reader.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8218 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1404 b- defN 23-Aug-01 07:33 openai_parallel_toolkit-1.1.1.dist-info/RECORD
+15 files, 28587 bytes uncompressed, 10524 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,22 +1,46 @@
 Filename: openai_parallel_toolkit/__init__.py
 Comment: 
 
 Filename: openai_parallel_toolkit/main.py
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.0.dist-info/LICENSE
+Filename: openai_parallel_toolkit/api/__init__.py
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.0.dist-info/METADATA
+Filename: openai_parallel_toolkit/api/keys.py
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.0.dist-info/WHEEL
+Filename: openai_parallel_toolkit/api/model.py
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.0.dist-info/top_level.txt
+Filename: openai_parallel_toolkit/api/request.py
 Comment: 
 
-Filename: openai_parallel_toolkit-1.1.0.dist-info/RECORD
+Filename: openai_parallel_toolkit/utils/__init__.py
+Comment: 
+
+Filename: openai_parallel_toolkit/utils/logger.py
+Comment: 
+
+Filename: openai_parallel_toolkit/utils/process_bar.py
+Comment: 
+
+Filename: openai_parallel_toolkit/utils/reader.py
+Comment: 
+
+Filename: openai_parallel_toolkit-1.1.1.dist-info/LICENSE
+Comment: 
+
+Filename: openai_parallel_toolkit-1.1.1.dist-info/METADATA
+Comment: 
+
+Filename: openai_parallel_toolkit-1.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: openai_parallel_toolkit-1.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: openai_parallel_toolkit-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `openai_parallel_toolkit-1.1.0.dist-info/LICENSE` & `openai_parallel_toolkit-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-1.1.0.dist-info/METADATA` & `openai_parallel_toolkit-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 1.1.0
+Version: 1.1.1
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

