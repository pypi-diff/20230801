# Comparing `tmp/remotion_lambda-4.0.14.tar.gz` & `tmp/remotion_lambda-4.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotion_lambda-4.0.14.tar", last modified: Mon Jul 31 14:22:10 2023, max compression
+gzip compressed data, was "remotion_lambda-4.0.15.tar", last modified: Tue Aug  1 07:01:51 2023, max compression
```

## Comparing `remotion_lambda-4.0.14.tar` & `remotion_lambda-4.0.15.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-07-31 14:22:10.391688 remotion_lambda-4.0.14/
--rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/LICENSE
--rw-r--r--   0 jonathanburger   (501) staff       (20)      391 2023-07-31 14:22:10.391490 remotion_lambda-4.0.14/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/README.md
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-07-31 14:22:10.388298 remotion_lambda-4.0.14/remotion_lambda/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/remotion_lambda/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-07-31 13:42:06.000000 remotion_lambda-4.0.14/remotion_lambda/models.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-07-31 14:14:39.000000 remotion_lambda-4.0.14/remotion_lambda/remotionclient.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2023-07-31 13:27:17.000000 remotion_lambda-4.0.14/remotion_lambda/version.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-07-31 14:22:10.390027 remotion_lambda-4.0.14/remotion_lambda.egg-info/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      391 2023-07-31 14:22:10.000000 remotion_lambda-4.0.14/remotion_lambda.egg-info/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-07-31 14:22:10.000000 remotion_lambda-4.0.14/remotion_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-07-31 14:22:10.000000 remotion_lambda-4.0.14/remotion_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-07-31 14:22:10.000000 remotion_lambda-4.0.14/remotion_lambda.egg-info/top_level.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-07-31 14:22:10.391730 remotion_lambda-4.0.14/setup.cfg
--rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/setup.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-07-31 14:22:10.390959 remotion_lambda-4.0.14/tests/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/tests/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/tests/test_get_render_progress_client.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/tests/test_render_client.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-01 07:01:51.957916 remotion_lambda-4.0.15/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/LICENSE
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      427 2023-08-01 07:01:51.957801 remotion_lambda-4.0.15/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/README.md
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-01 07:01:51.956724 remotion_lambda-4.0.15/remotion_lambda/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/remotion_lambda/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/remotion_lambda/models.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/remotion_lambda/remotionclient.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2023-08-01 06:56:26.000000 remotion_lambda-4.0.15/remotion_lambda/version.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-01 07:01:51.957153 remotion_lambda-4.0.15/remotion_lambda.egg-info/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      427 2023-08-01 07:01:51.000000 remotion_lambda-4.0.15/remotion_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-08-01 07:01:51.000000 remotion_lambda-4.0.15/remotion_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-08-01 07:01:51.000000 remotion_lambda-4.0.15/remotion_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-01 07:01:51.000000 remotion_lambda-4.0.15/remotion_lambda.egg-info/top_level.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-01 07:01:51.958026 remotion_lambda-4.0.15/setup.cfg
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/setup.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-01 07:01:51.957584 remotion_lambda-4.0.15/tests/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/tests/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/tests/test_get_render_progress_client.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-07-31 17:59:07.000000 remotion_lambda-4.0.15/tests/test_render_client.py
```

### Comparing `remotion_lambda-4.0.14/LICENSE` & `remotion_lambda-4.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.14/remotion_lambda/models.py` & `remotion_lambda-4.0.15/remotion_lambda/models.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.14/remotion_lambda/remotionclient.py` & `remotion_lambda-4.0.15/remotion_lambda/remotionclient.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.14/setup.py` & `remotion_lambda-4.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="remotion_lambda",
     version=VERSION,
-    author="Johny Burger",
+    author="Jonny Burger",
     author_email="jonny@remotion.dev",
     description="Remotion Lambda client",
     long_description_content_type="text/markdown",
     url="https://github.com/remotion-dev/remotion/tree/main/packages/lambda-python",
     classifiers=[
 
     ],
```

### Comparing `remotion_lambda-4.0.14/tests/test_render_client.py` & `remotion_lambda-4.0.15/tests/test_render_client.py`

 * *Files identical despite different names*

