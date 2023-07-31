# Comparing `tmp/lollms-2.2.6.tar.gz` & `tmp/lollms-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.2.6.tar", last modified: Mon Jul 31 22:28:50 2023, max compression
+gzip compressed data, was "lollms-2.2.7.tar", last modified: Mon Jul 31 22:47:11 2023, max compression
```

## Comparing `lollms-2.2.6.tar` & `lollms-2.2.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.439445 lollms-2.2.6/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.6/LICENSE
--rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0    11076 2023-07-31 22:28:50.438445 lollms-2.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.391922 lollms-2.2.6/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.6/lollms/__init__.py
--rw-rw-rw-   0        0        0     9679 2023-07-31 20:58:01.000000 lollms-2.2.6/lollms/app.py
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.414927 lollms-2.2.6/lollms/apps/
--rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.6/lollms/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.415926 lollms-2.2.6/lollms/apps/console/
--rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.6/lollms/apps/console/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.416927 lollms-2.2.6/lollms/apps/playground/
--rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.6/lollms/apps/playground/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.428436 lollms-2.2.6/lollms/apps/playground/static/
--rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.6/lollms/apps/playground/static/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.6/lollms/apps/playground/static/README.md
--rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.6/lollms/apps/playground/static/index.html
--rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.6/lollms/apps/playground/static/logo.png
--rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.6/lollms/apps/playground/static/lollms_playground.html
--rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.6/lollms/apps/playground/static/package.json
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.430445 lollms-2.2.6/lollms/apps/server/
--rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.2.6/lollms/apps/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.431443 lollms-2.2.6/lollms/apps/settings/
--rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.2.6/lollms/apps/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.433445 lollms-2.2.6/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.6/lollms/assets/logo.png
--rw-rw-rw-   0        0        0    11094 2023-07-31 22:09:20.000000 lollms-2.2.6/lollms/binding.py
--rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.6/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.436445 lollms-2.2.6/lollms/configs/
--rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.6/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.6/lollms/data.py
--rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.6/lollms/extension.py
--rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.6/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.6/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.6/lollms/main_config.py
--rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.6/lollms/paths.py
--rw-rw-rw-   0        0        0    50348 2023-07-31 22:28:37.000000 lollms-2.2.6/lollms/personality.py
--rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.6/lollms/terminal.py
--rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.6/lollms/types.py
--rw-rw-rw-   0        0        0    26797 2023-07-31 20:27:41.000000 lollms-2.2.6/lollms/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-31 22:28:50.413927 lollms-2.2.6/lollms.egg-info/
--rw-rw-rw-   0        0        0    11076 2023-07-31 22:28:50.000000 lollms-2.2.6/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-07-31 22:28:50.000000 lollms-2.2.6/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 22:28:50.000000 lollms-2.2.6/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-07-31 22:28:50.000000 lollms-2.2.6/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      245 2023-07-31 22:28:50.000000 lollms-2.2.6/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 22:28:50.000000 lollms-2.2.6/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 22:28:50.439445 lollms-2.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-07-31 22:28:47.000000 lollms-2.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.419954 lollms-2.2.7/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.7/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-07-31 22:47:11.419954 lollms-2.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.226384 lollms-2.2.7/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.7/lollms/__init__.py
+-rw-rw-rw-   0        0        0     9679 2023-07-31 20:58:01.000000 lollms-2.2.7/lollms/app.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.252990 lollms-2.2.7/lollms/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.7/lollms/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.263848 lollms-2.2.7/lollms/apps/console/
+-rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.7/lollms/apps/console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.285157 lollms-2.2.7/lollms/apps/playground/
+-rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.7/lollms/apps/playground/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.385020 lollms-2.2.7/lollms/apps/playground/static/
+-rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.7/lollms/apps/playground/static/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.7/lollms/apps/playground/static/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.7/lollms/apps/playground/static/index.html
+-rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.7/lollms/apps/playground/static/logo.png
+-rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.7/lollms/apps/playground/static/lollms_playground.html
+-rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.7/lollms/apps/playground/static/package.json
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.399499 lollms-2.2.7/lollms/apps/server/
+-rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.2.7/lollms/apps/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.408675 lollms-2.2.7/lollms/apps/settings/
+-rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.2.7/lollms/apps/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.409680 lollms-2.2.7/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.7/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0    11094 2023-07-31 22:09:20.000000 lollms-2.2.7/lollms/binding.py
+-rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.7/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.417800 lollms-2.2.7/lollms/configs/
+-rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.7/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.7/lollms/data.py
+-rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.7/lollms/extension.py
+-rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.7/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.7/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.7/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.7/lollms/paths.py
+-rw-rw-rw-   0        0        0    50348 2023-07-31 22:28:37.000000 lollms-2.2.7/lollms/personality.py
+-rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.7/lollms/terminal.py
+-rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.7/lollms/types.py
+-rw-rw-rw-   0        0        0    26875 2023-07-31 22:43:18.000000 lollms-2.2.7/lollms/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:47:11.251978 lollms-2.2.7/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-07-31 22:47:10.000000 lollms-2.2.7/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-07-31 22:47:11.000000 lollms-2.2.7/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 22:47:10.000000 lollms-2.2.7/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-07-31 22:47:10.000000 lollms-2.2.7/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      245 2023-07-31 22:47:10.000000 lollms-2.2.7/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 22:47:10.000000 lollms-2.2.7/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 22:47:11.420959 lollms-2.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-07-31 22:41:55.000000 lollms-2.2.7/setup.py
```

### Comparing `lollms-2.2.6/LICENSE` & `lollms-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/PKG-INFO` & `lollms-2.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.6
+Version: 2.2.7
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.6/README.md` & `lollms-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/app.py` & `lollms-2.2.7/lollms/app.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/apps/console/__init__.py` & `lollms-2.2.7/lollms/apps/console/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/apps/playground/static/LICENSE` & `lollms-2.2.7/lollms/apps/playground/static/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/apps/playground/static/README.md` & `lollms-2.2.7/lollms/apps/playground/static/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/apps/playground/static/index.html` & `lollms-2.2.7/lollms/apps/playground/static/index.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/apps/playground/static/logo.png` & `lollms-2.2.7/lollms/apps/playground/static/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/apps/playground/static/lollms_playground.html` & `lollms-2.2.7/lollms/apps/playground/static/lollms_playground.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/apps/server/__init__.py` & `lollms-2.2.7/lollms/apps/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/apps/settings/__init__.py` & `lollms-2.2.7/lollms/apps/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/assets/logo.png` & `lollms-2.2.7/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/binding.py` & `lollms-2.2.7/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/config.py` & `lollms-2.2.7/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/configs/config.yaml` & `lollms-2.2.7/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/data.py` & `lollms-2.2.7/lollms/data.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/extension.py` & `lollms-2.2.7/lollms/extension.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/helpers.py` & `lollms-2.2.7/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/langchain_integration.py` & `lollms-2.2.7/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/main_config.py` & `lollms-2.2.7/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/paths.py` & `lollms-2.2.7/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/personality.py` & `lollms-2.2.7/lollms/personality.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/terminal.py` & `lollms-2.2.7/lollms/terminal.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/types.py` & `lollms-2.2.7/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/lollms/utilities.py` & `lollms-2.2.7/lollms/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,16 @@
             import io
             import base64
         except:
             PackageManager.install_package("pillow")
             from PIL import Image
             import io
             import base64        
-        Image.open(io.BytesIO(base64.b64decode(b64img)))  
+        image_data = re.sub('^data:image/.+;base64,', '', b64img)
+        return Image.open(io.BytesIO(base64.b64decode(image_data)))  
 
 
 class TFIDFLoader:
     @staticmethod
     def create_vectorizer_from_dict(tfidf_info):
         vectorizer = TfidfVectorizer(**tfidf_info['params'])
         vectorizer.vocabulary_ = tfidf_info['vocabulary']
```

### Comparing `lollms-2.2.6/lollms.egg-info/PKG-INFO` & `lollms-2.2.7/lollms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.6
+Version: 2.2.7
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.6/lollms.egg-info/SOURCES.txt` & `lollms-2.2.7/lollms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lollms-2.2.6/setup.py` & `lollms-2.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.2.6",
+    version="2.2.7",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

