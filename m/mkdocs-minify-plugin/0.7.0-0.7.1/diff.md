# Comparing `tmp/mkdocs-minify-plugin-0.7.0.tar.gz` & `tmp/mkdocs-minify-plugin-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-minify-plugin-0.7.0.tar", last modified: Wed Jul 26 00:05:31 2023, max compression
+gzip compressed data, was "mkdocs-minify-plugin-0.7.1.tar", last modified: Tue Aug  1 16:33:19 2023, max compression
```

## Comparing `mkdocs-minify-plugin-0.7.0.tar` & `mkdocs-minify-plugin-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-07-26 00:05:31.930965 mkdocs-minify-plugin-0.7.0/
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1057 2021-01-16 01:26:07.000000 mkdocs-minify-plugin-0.7.0/LICENSE
--rw-r--r--   0 byrne.reese   (502) staff       (20)      946 2023-07-26 00:05:31.930840 mkdocs-minify-plugin-0.7.0/PKG-INFO
--rw-r--r--   0 byrne.reese   (502) staff       (20)     2894 2023-03-14 17:07:06.000000 mkdocs-minify-plugin-0.7.0/README.md
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-07-26 00:05:31.929664 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin/
--rw-r--r--   0 byrne.reese   (502) staff       (20)        0 2021-01-16 01:26:07.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin/__init__.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     8814 2023-07-26 00:05:18.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin/plugin.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-07-26 00:05:31.930414 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/
--rw-r--r--   0 byrne.reese   (502) staff       (20)      946 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/PKG-INFO
--rw-r--r--   0 byrne.reese   (502) staff       (20)      376 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)        1 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       67 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/entry_points.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       65 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/requires.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       21 2023-07-26 00:05:31.000000 mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/top_level.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       38 2023-07-26 00:05:31.931003 mkdocs-minify-plugin-0.7.0/setup.cfg
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1346 2023-07-26 00:05:18.000000 mkdocs-minify-plugin-0.7.0/setup.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-07-26 00:05:31.930532 mkdocs-minify-plugin-0.7.0/tests/
--rw-r--r--   0 byrne.reese   (502) staff       (20)     8589 2022-11-28 18:27:18.000000 mkdocs-minify-plugin-0.7.0/tests/test_basic.py
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-08-01 16:33:19.376576 mkdocs-minify-plugin-0.7.1/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     1057 2021-01-16 01:26:07.000000 mkdocs-minify-plugin-0.7.1/LICENSE
+-rw-r--r--   0 byrne.reese   (502) staff       (20)      946 2023-08-01 16:33:19.376449 mkdocs-minify-plugin-0.7.1/PKG-INFO
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     2894 2023-03-14 17:07:06.000000 mkdocs-minify-plugin-0.7.1/README.md
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-08-01 16:33:19.375139 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)        0 2021-01-16 01:26:07.000000 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin/__init__.py
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     9248 2023-08-01 16:08:38.000000 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin/plugin.py
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-08-01 16:33:19.375857 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin.egg-info/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)      946 2023-08-01 16:33:19.000000 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 byrne.reese   (502) staff       (20)      376 2023-08-01 16:33:19.000000 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)        1 2023-08-01 16:33:19.000000 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       67 2023-08-01 16:33:19.000000 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       65 2023-08-01 16:33:19.000000 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin.egg-info/requires.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       21 2023-08-01 16:33:19.000000 mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin.egg-info/top_level.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       38 2023-08-01 16:33:19.376613 mkdocs-minify-plugin-0.7.1/setup.cfg
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     1346 2023-08-01 16:08:38.000000 mkdocs-minify-plugin-0.7.1/setup.py
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2023-08-01 16:33:19.375979 mkdocs-minify-plugin-0.7.1/tests/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     8589 2022-11-28 18:27:18.000000 mkdocs-minify-plugin-0.7.1/tests/test_basic.py
```

### Comparing `mkdocs-minify-plugin-0.7.0/LICENSE` & `mkdocs-minify-plugin-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-minify-plugin-0.7.0/PKG-INFO` & `mkdocs-minify-plugin-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-minify-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: An MkDocs plugin to minify HTML, JS or CSS files prior to being written to disk
 Home-page: https://github.com/byrnereese/mkdocs-minify-plugin
 Author: Byrne Reese, Lars Wilhelmer
 Author-email: byrne@majordojo.com
 License: MIT
 Keywords: mkdocs minify publishing documentation html css
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-minify-plugin-0.7.0/README.md` & `mkdocs-minify-plugin-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin/plugin.py` & `mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,22 +154,29 @@
             file_hash: str = ""
 
             # When `cache_safe`, the hash is needed before the build,
             # so it's generated from the data from the source file.
             # A valid path in a custom_dir takes priority.
             if self.config["cache_safe"]:
                 docs_file_path: str = f"{config['docs_dir']}/{file_path}".replace("\\", "/")
+                theme = config.theme
 
-                for user_config in config.user_configs:
-                    user_config: Dict
-                    custom_dir: str = user_config.get("theme", {}).get("custom_dir", "")
-                    temp_path: str = f"{custom_dir}/{file_path}".replace("\\", "/")
-                    if custom_dir and os.path.exists(temp_path):
+                # Since MkDocs 1.5.0, theme.custom_dir is available for direct access
+                if not hasattr(theme, "custom_dir"):
+                    for user_config in config.user_configs:
+                        user_config: Dict
+                        custom_dir: str = user_config.get("theme", {}).get("custom_dir", "")
+                        temp_path: str = f"{custom_dir}/{file_path}".replace("\\", "/")
+                        if custom_dir and os.path.exists(temp_path):
+                            docs_file_path = temp_path
+                            break
+                elif theme.custom_dir:
+                    temp_path: str = f"{theme.custom_dir}/{file_path}".replace("\\", "/")
+                    if os.path.exists(temp_path):
                         docs_file_path = temp_path
-                        break
 
                 with open(docs_file_path, encoding="utf8") as file:
                     file_data: str = file.read()
 
                     if minify_flag:
                         file_data = self._minify_file_data_with_func(file_data, minify_func)
```

### Comparing `mkdocs-minify-plugin-0.7.0/mkdocs_minify_plugin.egg-info/PKG-INFO` & `mkdocs-minify-plugin-0.7.1/mkdocs_minify_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-minify-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: An MkDocs plugin to minify HTML, JS or CSS files prior to being written to disk
 Home-page: https://github.com/byrnereese/mkdocs-minify-plugin
 Author: Byrne Reese, Lars Wilhelmer
 Author-email: byrne@majordojo.com
 License: MIT
 Keywords: mkdocs minify publishing documentation html css
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-minify-plugin-0.7.0/setup.py` & `mkdocs-minify-plugin-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="mkdocs-minify-plugin",
-    version="0.7.0",
+    version="0.7.1",
     description="An MkDocs plugin to minify HTML, JS or CSS files prior to being written to disk",
     long_description="",
     keywords="mkdocs minify publishing documentation html css",
     url="https://github.com/byrnereese/mkdocs-minify-plugin",
     author="Byrne Reese, Lars Wilhelmer",
     author_email="byrne@majordojo.com",
     license="MIT",
```

### Comparing `mkdocs-minify-plugin-0.7.0/tests/test_basic.py` & `mkdocs-minify-plugin-0.7.1/tests/test_basic.py`

 * *Files identical despite different names*

