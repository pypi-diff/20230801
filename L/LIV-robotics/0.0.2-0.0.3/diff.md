# Comparing `tmp/LIV-robotics-0.0.2.tar.gz` & `tmp/LIV-robotics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LIV-robotics-0.0.2.tar", last modified: Mon Jul 31 22:58:55 2023, max compression
+gzip compressed data, was "LIV-robotics-0.0.3.tar", last modified: Mon Jul 31 23:26:23 2023, max compression
```

## Comparing `LIV-robotics-0.0.2.tar` & `LIV-robotics-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 22:58:55.711029 LIV-robotics-0.0.2/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)    19346 2023-07-28 00:25:56.000000 LIV-robotics-0.0.2/LICENSE
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 22:58:55.707029 LIV-robotics-0.0.2/LIV_robotics.egg-info/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6157 2023-07-31 22:58:55.000000 LIV-robotics-0.0.2/LIV_robotics.egg-info/PKG-INFO
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      423 2023-07-31 22:58:55.000000 LIV-robotics-0.0.2/LIV_robotics.egg-info/SOURCES.txt
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        1 2023-07-31 22:58:55.000000 LIV-robotics-0.0.2/LIV_robotics.egg-info/dependency_links.txt
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      229 2023-07-31 22:58:55.000000 LIV-robotics-0.0.2/LIV_robotics.egg-info/requires.txt
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        4 2023-07-31 22:58:55.000000 LIV-robotics-0.0.2/LIV_robotics.egg-info/top_level.txt
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6157 2023-07-31 22:58:55.711029 LIV-robotics-0.0.2/PKG-INFO
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5598 2023-07-28 00:25:56.000000 LIV-robotics-0.0.2/README.md
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 22:58:55.711029 LIV-robotics-0.0.2/liv/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     1854 2023-07-31 22:51:27.000000 LIV-robotics-0.0.2/liv/__init__.py
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 22:58:55.711029 LIV-robotics-0.0.2/liv/models/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       36 2023-07-28 00:25:57.000000 LIV-robotics-0.0.2/liv/models/__init__.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     3683 2023-07-31 22:57:04.000000 LIV-robotics-0.0.2/liv/models/model_liv.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6835 2023-07-28 00:25:57.000000 LIV-robotics-0.0.2/liv/train_liv.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4635 2023-07-28 00:25:57.000000 LIV-robotics-0.0.2/liv/trainer.py
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 22:58:55.711029 LIV-robotics-0.0.2/liv/utils/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      262 2023-07-28 00:25:57.000000 LIV-robotics-0.0.2/liv/utils/__init__.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5928 2023-07-28 00:25:57.000000 LIV-robotics-0.0.2/liv/utils/data_loaders.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5934 2023-07-28 00:25:57.000000 LIV-robotics-0.0.2/liv/utils/logger.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5591 2023-07-28 00:25:57.000000 LIV-robotics-0.0.2/liv/utils/plotter.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4777 2023-07-28 00:25:57.000000 LIV-robotics-0.0.2/liv/utils/utils.py
--rw-r--r--   0 haonanyu  (1000) haonanyu  (1000)      616 2023-07-31 22:58:41.000000 LIV-robotics-0.0.2/pyproject.toml
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       38 2023-07-31 22:58:55.711029 LIV-robotics-0.0.2/setup.cfg
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     1071 2023-07-31 22:58:39.000000 LIV-robotics-0.0.2/setup.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:26:23.692385 LIV-robotics-0.0.3/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)    19346 2023-07-28 00:25:56.000000 LIV-robotics-0.0.3/LICENSE
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:26:23.692385 LIV-robotics-0.0.3/LIV_robotics.egg-info/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6157 2023-07-31 23:26:23.000000 LIV-robotics-0.0.3/LIV_robotics.egg-info/PKG-INFO
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      666 2023-07-31 23:26:23.000000 LIV-robotics-0.0.3/LIV_robotics.egg-info/SOURCES.txt
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        1 2023-07-31 23:26:23.000000 LIV-robotics-0.0.3/LIV_robotics.egg-info/dependency_links.txt
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      229 2023-07-31 23:26:23.000000 LIV-robotics-0.0.3/LIV_robotics.egg-info/requires.txt
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        4 2023-07-31 23:26:23.000000 LIV-robotics-0.0.3/LIV_robotics.egg-info/top_level.txt
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6157 2023-07-31 23:26:23.692385 LIV-robotics-0.0.3/PKG-INFO
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5598 2023-07-28 00:25:56.000000 LIV-robotics-0.0.3/README.md
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:26:23.688385 LIV-robotics-0.0.3/liv/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     1854 2023-07-31 22:51:27.000000 LIV-robotics-0.0.3/liv/__init__.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:26:23.688385 LIV-robotics-0.0.3/liv/models/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       36 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/models/__init__.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:26:23.688385 LIV-robotics-0.0.3/liv/models/clip/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:23:28.000000 LIV-robotics-0.0.3/liv/models/clip/__init__.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:26:23.688385 LIV-robotics-0.0.3/liv/models/clip/clip/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       20 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/models/clip/clip/__init__.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)  1356917 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/models/clip/clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     9445 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/models/clip/clip/clip.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)    17411 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/models/clip/clip/model.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4632 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/models/clip/clip/simple_tokenizer.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     3683 2023-07-31 22:57:04.000000 LIV-robotics-0.0.3/liv/models/model_liv.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6835 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/train_liv.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4635 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/trainer.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:26:23.688385 LIV-robotics-0.0.3/liv/utils/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      262 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/utils/__init__.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5928 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/utils/data_loaders.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5934 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/utils/logger.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5591 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/utils/plotter.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4777 2023-07-28 00:25:57.000000 LIV-robotics-0.0.3/liv/utils/utils.py
+-rw-r--r--   0 haonanyu  (1000) haonanyu  (1000)      616 2023-07-31 23:26:10.000000 LIV-robotics-0.0.3/pyproject.toml
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       38 2023-07-31 23:26:23.692385 LIV-robotics-0.0.3/setup.cfg
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     1154 2023-07-31 23:26:08.000000 LIV-robotics-0.0.3/setup.py
```

### Comparing `LIV-robotics-0.0.2/LICENSE` & `LIV-robotics-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/LIV_robotics.egg-info/PKG-INFO` & `LIV-robotics-0.0.3/LIV_robotics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LIV-robotics
-Version: 0.0.2
+Version: 0.0.3
 Summary: LIV: Language-Image Representations and Rewards for Robotic Control
 Author: Jason Ma
 Author-email: Jason Ma <jasonyma@seas.upenn.edu>
 Project-URL: Homepage, https://github.com/penn-pal-lab/LIV
 Project-URL: Bug Tracker, https://github.com/penn-pal-lab/LIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LIV-robotics-0.0.2/PKG-INFO` & `LIV-robotics-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LIV-robotics
-Version: 0.0.2
+Version: 0.0.3
 Summary: LIV: Language-Image Representations and Rewards for Robotic Control
 Author: Jason Ma
 Author-email: Jason Ma <jasonyma@seas.upenn.edu>
 Project-URL: Homepage, https://github.com/penn-pal-lab/LIV
 Project-URL: Bug Tracker, https://github.com/penn-pal-lab/LIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LIV-robotics-0.0.2/README.md` & `LIV-robotics-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/liv/__init__.py` & `LIV-robotics-0.0.3/liv/__init__.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/liv/models/model_liv.py` & `LIV-robotics-0.0.3/liv/models/model_liv.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/liv/train_liv.py` & `LIV-robotics-0.0.3/liv/train_liv.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/liv/trainer.py` & `LIV-robotics-0.0.3/liv/trainer.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/liv/utils/data_loaders.py` & `LIV-robotics-0.0.3/liv/utils/data_loaders.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/liv/utils/logger.py` & `LIV-robotics-0.0.3/liv/utils/logger.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/liv/utils/plotter.py` & `LIV-robotics-0.0.3/liv/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/liv/utils/utils.py` & `LIV-robotics-0.0.3/liv/utils/utils.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.0.2/pyproject.toml` & `LIV-robotics-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LIV-robotics"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jason Ma", email="jasonyma@seas.upenn.edu" },
 ]
 description = "LIV: Language-Image Representations and Rewards for Robotic Control"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `LIV-robotics-0.0.2/setup.py` & `LIV-robotics-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 if sys.version_info.major != 3:
     print("This Python is only compatible with Python 3, but you are running "
           "Python {}. The installation will likely fail.".format(sys.version_info.major))
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
+
 setup(
     name='liv',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     description='LIV: Language-Image Representations and Rewards for Robotic Control',
     long_description=read('README.md'),
     author='Jason Ma',
     install_requires=[
         'torch',
         'torchvision>=0.8.2',
@@ -34,9 +35,11 @@
         'scikit-video',
         'transforms3d',
         'moviepy',
         'termcolor',
         'ftfy',
         'regex',
         'tqdm'
-    ]
+    ],
+    package_dir={"": "."},
+    package_data={"": ["*.sh", "*.yaml", "*.txt.gz"]}
 )
```

