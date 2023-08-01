# Comparing `tmp/imaginaryNLP-0.0.1.tar.gz` & `tmp/imaginaryNLP-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaginaryNLP-0.0.1.tar", last modified: Mon May 22 16:19:35 2023, max compression
+gzip compressed data, was "imaginaryNLP-0.0.2.tar", last modified: Tue Aug  1 10:05:00 2023, max compression
```

## Comparing `imaginaryNLP-0.0.1.tar` & `imaginaryNLP-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxr-x   0 justus-jonas  (1000) justus-jonas  (1000)        0 2023-05-22 16:19:35.054319 imaginaryNLP-0.0.1/
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)    11343 2023-05-22 15:53:46.000000 imaginaryNLP-0.0.1/LICENSE
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)     1083 2023-05-22 16:19:35.054319 imaginaryNLP-0.0.1/PKG-INFO
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)      387 2023-05-20 10:42:28.000000 imaginaryNLP-0.0.1/README.md
-drwxrwxr-x   0 justus-jonas  (1000) justus-jonas  (1000)        0 2023-05-22 16:19:35.050319 imaginaryNLP-0.0.1/imaginaryNLP/
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)      575 2023-05-22 16:19:23.000000 imaginaryNLP-0.0.1/imaginaryNLP/ImaginaryEmbeddings.py
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)        0 2023-05-20 10:44:17.000000 imaginaryNLP-0.0.1/imaginaryNLP/__init__.py
-drwxrwxr-x   0 justus-jonas  (1000) justus-jonas  (1000)        0 2023-05-22 16:19:35.054319 imaginaryNLP-0.0.1/imaginaryNLP.egg-info/
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)     1083 2023-05-22 16:19:34.000000 imaginaryNLP-0.0.1/imaginaryNLP.egg-info/PKG-INFO
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)      266 2023-05-22 16:19:34.000000 imaginaryNLP-0.0.1/imaginaryNLP.egg-info/SOURCES.txt
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)        1 2023-05-22 16:19:34.000000 imaginaryNLP-0.0.1/imaginaryNLP.egg-info/dependency_links.txt
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)       56 2023-05-22 16:19:34.000000 imaginaryNLP-0.0.1/imaginaryNLP.egg-info/requires.txt
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)       13 2023-05-22 16:19:34.000000 imaginaryNLP-0.0.1/imaginaryNLP.egg-info/top_level.txt
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)       38 2023-05-22 16:19:35.054319 imaginaryNLP-0.0.1/setup.cfg
--rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)     1062 2023-05-22 16:19:23.000000 imaginaryNLP-0.0.1/setup.py
+drwxrwxr-x   0 justus-jonas  (1000) justus-jonas  (1000)        0 2023-08-01 10:05:00.474548 imaginaryNLP-0.0.2/
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)    11343 2023-05-22 15:53:46.000000 imaginaryNLP-0.0.2/LICENSE
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)    10095 2023-08-01 10:05:00.474548 imaginaryNLP-0.0.2/PKG-INFO
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)     9399 2023-08-01 08:53:42.000000 imaginaryNLP-0.0.2/README.md
+drwxrwxr-x   0 justus-jonas  (1000) justus-jonas  (1000)        0 2023-08-01 10:05:00.474548 imaginaryNLP-0.0.2/imaginaryNLP/
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)      734 2023-07-09 03:13:34.000000 imaginaryNLP-0.0.2/imaginaryNLP/ImaginaryEmbeddings.py
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)    25558 2023-07-09 12:03:56.000000 imaginaryNLP-0.0.2/imaginaryNLP/ImaginaryEmbeddingsForLTP.py
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)     9951 2023-07-09 15:53:01.000000 imaginaryNLP-0.0.2/imaginaryNLP/ImaginaryEmbeddingsForSTP.py
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)    21179 2023-07-09 12:58:45.000000 imaginaryNLP-0.0.2/imaginaryNLP/ImaginaryEmbeddingsForSequenceModeling.py
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)        0 2023-05-20 10:44:17.000000 imaginaryNLP-0.0.2/imaginaryNLP/__init__.py
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)    14396 2023-08-01 08:59:09.000000 imaginaryNLP-0.0.2/imaginaryNLP/trainer.py
+drwxrwxr-x   0 justus-jonas  (1000) justus-jonas  (1000)        0 2023-08-01 10:05:00.474548 imaginaryNLP-0.0.2/imaginaryNLP.egg-info/
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)    10095 2023-08-01 10:05:00.000000 imaginaryNLP-0.0.2/imaginaryNLP.egg-info/PKG-INFO
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)      429 2023-08-01 10:05:00.000000 imaginaryNLP-0.0.2/imaginaryNLP.egg-info/SOURCES.txt
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)        1 2023-08-01 10:05:00.000000 imaginaryNLP-0.0.2/imaginaryNLP.egg-info/dependency_links.txt
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)       91 2023-08-01 10:05:00.000000 imaginaryNLP-0.0.2/imaginaryNLP.egg-info/requires.txt
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)       13 2023-08-01 10:05:00.000000 imaginaryNLP-0.0.2/imaginaryNLP.egg-info/top_level.txt
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)       38 2023-08-01 10:05:00.474548 imaginaryNLP-0.0.2/setup.cfg
+-rw-rw-r--   0 justus-jonas  (1000) justus-jonas  (1000)     1140 2023-08-01 10:04:53.000000 imaginaryNLP-0.0.2/setup.py
```

### Comparing `imaginaryNLP-0.0.1/LICENSE` & `imaginaryNLP-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imaginaryNLP-0.0.1/setup.py` & `imaginaryNLP-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 with open("README.md", mode="r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 
 
 setup(
     name="imaginaryNLP",
-    version="0.0.1",
+    version="0.0.2",
     author="Justus-Jonas Erker",
     author_email="j.erker@student.maastrichtuniversity.nl",
     description="Imaginary Embeddings for NLP",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     download_url="https://github.com/Justus-Jonas/nlp-i",
     packages=find_packages(),
     python_requires=">=3.6.0",
     install_requires=[
-        'transformers>=4.6.0,<5.0.0',
-        'sentence-transformers>=2.0.0',
+        'datasets==2.13.1',
+        'transformers>=2.0.0',
+        'torch==2.0.1',
+        'numpy==1.21.5',
+        'pandas==1.4.4',
+        'tqdm==4.64.1'
     ],
     classifiers=[
         "Development Status :: 1 - Planning",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.6",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Intended Audience :: Science/Research",
```

