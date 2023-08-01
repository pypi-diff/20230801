# Comparing `tmp/json-tools2-0.0.8.tar.gz` & `tmp/json-tools2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-tools2-0.0.8.tar", last modified: Fri Jul 28 10:53:52 2023, max compression
+gzip compressed data, was "json-tools2-0.0.9.tar", last modified: Tue Aug  1 02:09:41 2023, max compression
```

## Comparing `json-tools2-0.0.8.tar` & `json-tools2-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 10:53:52.099943 json-tools2-0.0.8/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1067 2021-10-05 22:07:19.000000 json-tools2-0.0.8/LICENSE
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       18 2021-10-05 22:07:19.000000 json-tools2-0.0.8/MANIFEST.in
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4044 2023-07-28 10:53:52.095943 json-tools2-0.0.8/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3675 2023-07-28 10:19:42.000000 json-tools2-0.0.8/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-28 10:53:52.099943 json-tools2-0.0.8/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      987 2023-07-28 10:13:24.000000 json-tools2-0.0.8/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 10:53:52.095943 json-tools2-0.0.8/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 10:53:52.095943 json-tools2-0.0.8/src/json_tools2/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      118 2023-07-28 09:44:32.000000 json-tools2-0.0.8/src/json_tools2/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    13180 2021-10-05 22:07:19.000000 json-tools2-0.0.8/src/json_tools2/flat_json.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     9370 2023-07-28 10:52:13.000000 json-tools2-0.0.8/src/json_tools2/schema.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1045 2021-11-02 22:26:53.000000 json-tools2-0.0.8/src/json_tools2/spark.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      637 2021-10-05 22:07:19.000000 json-tools2-0.0.8/src/json_tools2/util.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 10:53:52.095943 json-tools2-0.0.8/src/json_tools2.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4044 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      364 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       11 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       12 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-08-01 02:09:41.602162 json-tools2-0.0.9/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1067 2021-10-05 22:07:19.000000 json-tools2-0.0.9/LICENSE
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       18 2021-10-05 22:07:19.000000 json-tools2-0.0.9/MANIFEST.in
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6346 2023-08-01 02:09:41.602162 json-tools2-0.0.9/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5977 2023-08-01 01:40:10.000000 json-tools2-0.0.9/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-08-01 02:09:41.602162 json-tools2-0.0.9/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      987 2023-08-01 02:09:16.000000 json-tools2-0.0.9/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-08-01 02:09:41.602162 json-tools2-0.0.9/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-08-01 02:09:41.602162 json-tools2-0.0.9/src/json_tools2/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      207 2023-08-01 00:28:32.000000 json-tools2-0.0.9/src/json_tools2/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    13180 2021-10-05 22:07:19.000000 json-tools2-0.0.9/src/json_tools2/flat_json.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     9370 2023-07-28 10:52:13.000000 json-tools2-0.0.9/src/json_tools2/schema.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1045 2021-11-02 22:26:53.000000 json-tools2-0.0.9/src/json_tools2/spark.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3506 2023-08-01 01:28:04.000000 json-tools2-0.0.9/src/json_tools2/transform.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      637 2021-10-05 22:07:19.000000 json-tools2-0.0.9/src/json_tools2/util.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-08-01 02:09:41.602162 json-tools2-0.0.9/src/json_tools2.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6346 2023-08-01 02:09:41.000000 json-tools2-0.0.9/src/json_tools2.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      393 2023-08-01 02:09:41.000000 json-tools2-0.0.9/src/json_tools2.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-08-01 02:09:41.000000 json-tools2-0.0.9/src/json_tools2.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       11 2023-08-01 02:09:41.000000 json-tools2-0.0.9/src/json_tools2.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       12 2023-08-01 02:09:41.000000 json-tools2-0.0.9/src/json_tools2.egg-info/top_level.txt
```

### Comparing `json-tools2-0.0.8/LICENSE` & `json-tools2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.8/setup.py` & `json-tools2-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="json-tools2",
-    version="0.0.8",
+    version="0.0.9",
     description="JSON Tools Library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/json_tools2",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `json-tools2-0.0.8/src/json_tools2/flat_json.py` & `json-tools2-0.0.9/src/json_tools2/flat_json.py`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.8/src/json_tools2/schema.py` & `json-tools2-0.0.9/src/json_tools2/schema.py`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.8/src/json_tools2/spark.py` & `json-tools2-0.0.9/src/json_tools2/spark.py`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.8/src/json_tools2/util.py` & `json-tools2-0.0.9/src/json_tools2/util.py`

 * *Files identical despite different names*

