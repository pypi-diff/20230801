# Comparing `tmp/lollms-2.2.4.tar.gz` & `tmp/lollms-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.2.4.tar", last modified: Mon Jul 31 20:27:53 2023, max compression
+gzip compressed data, was "lollms-2.2.5.tar", last modified: Mon Jul 31 22:15:30 2023, max compression
```

## Comparing `lollms-2.2.4.tar` & `lollms-2.2.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.400930 lollms-2.2.4/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.4/LICENSE
--rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0    11076 2023-07-31 20:27:53.400930 lollms-2.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.358996 lollms-2.2.4/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.4/lollms/__init__.py
--rw-rw-rw-   0        0        0     9442 2023-07-31 19:53:45.000000 lollms-2.2.4/lollms/app.py
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.384893 lollms-2.2.4/lollms/apps/
--rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.4/lollms/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.386067 lollms-2.2.4/lollms/apps/console/
--rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.4/lollms/apps/console/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.386901 lollms-2.2.4/lollms/apps/playground/
--rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.4/lollms/apps/playground/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.394418 lollms-2.2.4/lollms/apps/playground/static/
--rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.4/lollms/apps/playground/static/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.4/lollms/apps/playground/static/README.md
--rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.4/lollms/apps/playground/static/index.html
--rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.4/lollms/apps/playground/static/logo.png
--rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.4/lollms/apps/playground/static/lollms_playground.html
--rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.4/lollms/apps/playground/static/package.json
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.394924 lollms-2.2.4/lollms/apps/server/
--rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.2.4/lollms/apps/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.395933 lollms-2.2.4/lollms/apps/settings/
--rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.2.4/lollms/apps/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.397929 lollms-2.2.4/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.4/lollms/assets/logo.png
--rw-rw-rw-   0        0        0    10963 2023-07-27 19:45:11.000000 lollms-2.2.4/lollms/binding.py
--rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.4/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.399934 lollms-2.2.4/lollms/configs/
--rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.4/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.4/lollms/data.py
--rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.4/lollms/extension.py
--rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.4/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.4/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.4/lollms/main_config.py
--rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.4/lollms/paths.py
--rw-rw-rw-   0        0        0    50149 2023-07-30 23:55:31.000000 lollms-2.2.4/lollms/personality.py
--rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.4/lollms/terminal.py
--rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.4/lollms/types.py
--rw-rw-rw-   0        0        0    26797 2023-07-31 20:27:41.000000 lollms-2.2.4/lollms/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-31 20:27:53.384039 lollms-2.2.4/lollms.egg-info/
--rw-rw-rw-   0        0        0    11076 2023-07-31 20:27:53.000000 lollms-2.2.4/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-07-31 20:27:53.000000 lollms-2.2.4/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 20:27:53.000000 lollms-2.2.4/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-07-31 20:27:53.000000 lollms-2.2.4/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      245 2023-07-31 20:27:53.000000 lollms-2.2.4/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 20:27:53.000000 lollms-2.2.4/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 20:27:53.401931 lollms-2.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-07-31 20:27:49.000000 lollms-2.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.956790 lollms-2.2.5/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.5/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-07-31 22:15:30.956790 lollms-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.804825 lollms-2.2.5/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.5/lollms/__init__.py
+-rw-rw-rw-   0        0        0     9679 2023-07-31 20:58:01.000000 lollms-2.2.5/lollms/app.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.829346 lollms-2.2.5/lollms/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.5/lollms/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.830347 lollms-2.2.5/lollms/apps/console/
+-rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.5/lollms/apps/console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.841978 lollms-2.2.5/lollms/apps/playground/
+-rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.5/lollms/apps/playground/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.927531 lollms-2.2.5/lollms/apps/playground/static/
+-rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.5/lollms/apps/playground/static/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.5/lollms/apps/playground/static/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.5/lollms/apps/playground/static/index.html
+-rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.5/lollms/apps/playground/static/logo.png
+-rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.5/lollms/apps/playground/static/lollms_playground.html
+-rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.5/lollms/apps/playground/static/package.json
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.938531 lollms-2.2.5/lollms/apps/server/
+-rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.2.5/lollms/apps/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.946536 lollms-2.2.5/lollms/apps/settings/
+-rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.2.5/lollms/apps/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.947531 lollms-2.2.5/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.5/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0    11094 2023-07-31 22:09:20.000000 lollms-2.2.5/lollms/binding.py
+-rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.5/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.954792 lollms-2.2.5/lollms/configs/
+-rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.5/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.5/lollms/data.py
+-rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.5/lollms/extension.py
+-rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.5/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.5/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.5/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.5/lollms/paths.py
+-rw-rw-rw-   0        0        0    50341 2023-07-31 20:55:31.000000 lollms-2.2.5/lollms/personality.py
+-rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.5/lollms/terminal.py
+-rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.5/lollms/types.py
+-rw-rw-rw-   0        0        0    26797 2023-07-31 20:27:41.000000 lollms-2.2.5/lollms/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-31 22:15:30.828349 lollms-2.2.5/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-07-31 22:15:30.000000 lollms-2.2.5/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-07-31 22:15:30.000000 lollms-2.2.5/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 22:15:30.000000 lollms-2.2.5/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-07-31 22:15:30.000000 lollms-2.2.5/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      245 2023-07-31 22:15:30.000000 lollms-2.2.5/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 22:15:30.000000 lollms-2.2.5/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 22:15:30.956790 lollms-2.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-07-31 22:15:27.000000 lollms-2.2.5/setup.py
```

### Comparing `lollms-2.2.4/LICENSE` & `lollms-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/PKG-INFO` & `lollms-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.4
+Version: 2.2.5
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.4/README.md` & `lollms-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/app.py` & `lollms-2.2.5/lollms/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from lollms.helpers import ASCIIColors
 from lollms.paths import LollmsPaths
 from lollms.personality import PersonalityBuilder
 from lollms.binding import LLMBinding, BindingBuilder, ModelBuilder
 from lollms.config import InstallOption
 from lollms.helpers import trace_exception
 from lollms.terminal import MainMenu
+from typing import Callable
 
 import subprocess
 
 class LollmsApplication:
     def __init__(
                     self, 
                     app_name:str, 
@@ -147,15 +148,19 @@
                 to_remove.append(i)
         to_remove.sort(reverse=True)
         for i in to_remove:
             self.unmount_personality(i)
 
         self.personality = self.mounted_personalities[self.config.active_personality_id]
 
+    def set_personalities_callbacks(self, callback: Callable[[str, int, dict], bool]=None):
+        for personality in self.mount_personalities:
+            personality.setCallback(callback)
 
+            
     def unmount_personality(self, id:int)->bool:
         if id<len(self.config.personalities):
             del self.config.personalities[id]
             del self.mounted_personalities[id]
             if self.config.active_personality_id>=id:
                 self.config.active_personality_id-=1
```

### Comparing `lollms-2.2.4/lollms/apps/console/__init__.py` & `lollms-2.2.5/lollms/apps/console/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/apps/playground/static/LICENSE` & `lollms-2.2.5/lollms/apps/playground/static/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/apps/playground/static/README.md` & `lollms-2.2.5/lollms/apps/playground/static/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/apps/playground/static/index.html` & `lollms-2.2.5/lollms/apps/playground/static/index.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/apps/playground/static/logo.png` & `lollms-2.2.5/lollms/apps/playground/static/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/apps/playground/static/lollms_playground.html` & `lollms-2.2.5/lollms/apps/playground/static/lollms_playground.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/apps/server/__init__.py` & `lollms-2.2.5/lollms/apps/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/apps/settings/__init__.py` & `lollms-2.2.5/lollms/apps/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/assets/logo.png` & `lollms-2.2.5/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/binding.py` & `lollms-2.2.5/lollms/binding.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,17 +143,21 @@
             str: The path of the model.
         """
         if self.config.model_name is None:
             return None
         
         if self.config.model_name.endswith(".reference"):
             ASCIIColors.yellow("Loading a reference model:")
-            with open(str(self.lollms_paths.personal_models_path / f"{self.binding_folder_name}/{self.config.model_name}"), 'r') as f:
-                model_path = Path(f.read())
-            ASCIIColors.yellow(model_path)
+            file_path = self.lollms_paths.personal_models_path / f"{self.binding_folder_name}/{self.config.model_name}"
+            if file_path.exists():
+                with open(str(file_path), 'r') as f:
+                    model_path = Path(f.read())
+                ASCIIColors.yellow(model_path)
+            else:
+                return None
         else:
             model_path = Path(self.lollms_paths.personal_models_path / f"{self.binding_folder_name}/{self.config.model_name}")
 
         return model_path
 
     
     def get_current_seed(self):
```

### Comparing `lollms-2.2.4/lollms/config.py` & `lollms-2.2.5/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/configs/config.yaml` & `lollms-2.2.5/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/data.py` & `lollms-2.2.5/lollms/data.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/extension.py` & `lollms-2.2.5/lollms/extension.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/helpers.py` & `lollms-2.2.5/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/langchain_integration.py` & `lollms-2.2.5/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/main_config.py` & `lollms-2.2.5/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/paths.py` & `lollms-2.2.5/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/personality.py` & `lollms-2.2.5/lollms/personality.py`

 * *Files 1% similar despite different names*

```diff
@@ -943,15 +943,20 @@
             self.personality_config.config.save_config()
         else:
             self.load_personality_config()
 
         self.models_folder = self.personality.lollms_paths.personal_models_path / self.personality.personality_folder_name
         self.models_folder.mkdir(parents=True, exist_ok=True)
 
+    def setCallback(self, callback: Callable[[str, int, dict], bool]):
+        self.callback = callback
+        if self.process:
+            self.process.callback = callback
 
+            
     def load_personality_config(self):
         """
         Load the content of local_config.yaml file.
 
         The function reads the content of the local_config.yaml file and returns it as a Python dictionary.
 
         Args:
```

### Comparing `lollms-2.2.4/lollms/terminal.py` & `lollms-2.2.5/lollms/terminal.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/types.py` & `lollms-2.2.5/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms/utilities.py` & `lollms-2.2.5/lollms/utilities.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/lollms.egg-info/PKG-INFO` & `lollms-2.2.5/lollms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.4
+Version: 2.2.5
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.4/lollms.egg-info/SOURCES.txt` & `lollms-2.2.5/lollms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lollms-2.2.4/setup.py` & `lollms-2.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.2.4",
+    version="2.2.5",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

