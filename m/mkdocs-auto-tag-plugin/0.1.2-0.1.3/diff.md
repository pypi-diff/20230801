# Comparing `tmp/mkdocs-auto-tag-plugin-0.1.2.tar.gz` & `tmp/mkdocs-auto-tag-plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-auto-tag-plugin-0.1.2.tar", last modified: Sat Dec 31 14:43:19 2022, max compression
+gzip compressed data, was "mkdocs-auto-tag-plugin-0.1.3.tar", last modified: Tue Aug  1 16:57:59 2023, max compression
```

## Comparing `mkdocs-auto-tag-plugin-0.1.2.tar` & `mkdocs-auto-tag-plugin-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-12-31 14:43:19.287958 mkdocs-auto-tag-plugin-0.1.2/
--rw-r--r--   0 user       (501) staff       (20)     1063 2022-08-04 17:39:49.000000 mkdocs-auto-tag-plugin-0.1.2/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       18 2022-12-17 13:02:02.000000 mkdocs-auto-tag-plugin-0.1.2/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     1938 2022-12-31 14:43:19.288008 mkdocs-auto-tag-plugin-0.1.2/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1340 2022-12-31 14:41:42.000000 mkdocs-auto-tag-plugin-0.1.2/README.md
--rw-r--r--   0 user       (501) staff       (20)       85 2022-08-04 17:39:49.000000 mkdocs-auto-tag-plugin-0.1.2/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)      854 2022-12-31 14:43:19.288262 mkdocs-auto-tag-plugin-0.1.2/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-12-31 14:43:19.286298 mkdocs-auto-tag-plugin-0.1.2/src/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-12-31 14:43:19.287156 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin/
--rw-r--r--   0 user       (501) staff       (20)      538 2022-12-18 16:03:33.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     6558 2022-12-18 17:01:52.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin/plugin.py
--rwxr-xr-x   0 user       (501) staff       (20)     1230 2022-12-31 14:35:24.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin/utils.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-12-31 14:43:19.287830 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     1938 2022-12-31 14:43:19.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      468 2022-12-31 14:43:19.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2022-12-31 14:43:19.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       57 2022-12-31 14:43:19.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       14 2022-12-31 14:43:19.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       23 2022-12-31 14:43:19.000000 mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:57:59.417615 mkdocs-auto-tag-plugin-0.1.3/
+-rw-r--r--   0 user       (501) staff       (20)     1063 2022-08-04 17:39:49.000000 mkdocs-auto-tag-plugin-0.1.3/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       18 2022-12-17 13:02:02.000000 mkdocs-auto-tag-plugin-0.1.3/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     1999 2023-08-01 16:57:59.417667 mkdocs-auto-tag-plugin-0.1.3/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     1401 2023-08-01 16:55:28.000000 mkdocs-auto-tag-plugin-0.1.3/README.md
+-rw-r--r--   0 user       (501) staff       (20)       85 2022-08-04 17:39:49.000000 mkdocs-auto-tag-plugin-0.1.3/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)      854 2023-08-01 16:57:59.417899 mkdocs-auto-tag-plugin-0.1.3/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:57:59.414422 mkdocs-auto-tag-plugin-0.1.3/src/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:57:59.416514 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin/
+-rw-r--r--   0 user       (501) staff       (20)      465 2023-08-01 16:52:59.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     6564 2023-08-01 16:57:27.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin/plugin.py
+-rwxr-xr-x   0 user       (501) staff       (20)     1230 2022-12-31 14:35:24.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin/utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:57:59.417521 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     1999 2023-08-01 16:57:59.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      468 2023-08-01 16:57:59.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-08-01 16:57:59.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       57 2023-08-01 16:57:59.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-08-01 16:57:59.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       23 2023-08-01 16:57:59.000000 mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin.egg-info/top_level.txt
```

### Comparing `mkdocs-auto-tag-plugin-0.1.2/LICENSE` & `mkdocs-auto-tag-plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-auto-tag-plugin-0.1.2/PKG-INFO` & `mkdocs-auto-tag-plugin-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-auto-tag-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add tags to your MkDocs pages based on their path / file name
 Home-page: https://github.com/six-two/mkdocs-auto-tag-plugin
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -32,15 +32,17 @@
 
 The files in the `docs/test/` directory implicitely work as tests.
 They should be tagged correctly.
 
 
 ## Notable changes
 
-### HEAD
+### 0.1.3
+
+- Just fixed the `DeprecationWarning` for `warning_filter`
 
 ### 0.1.2
 
 - Just small documentation changes. But I needed to increase the version number to remove the `!!! Warning: Pre alpha: This is currently just a PoC for myself` line from the PyPI site
 
 ### 0.1.1
```

### Comparing `mkdocs-auto-tag-plugin-0.1.2/README.md` & `mkdocs-auto-tag-plugin-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 The files in the `docs/test/` directory implicitely work as tests.
 They should be tagged correctly.
 
 
 ## Notable changes
 
-### HEAD
+### 0.1.3
+
+- Just fixed the `DeprecationWarning` for `warning_filter`
 
 ### 0.1.2
 
 - Just small documentation changes. But I needed to increase the version number to remove the `!!! Warning: Pre alpha: This is currently just a PoC for myself` line from the PyPI site
 
 ### 0.1.1
```

### Comparing `mkdocs-auto-tag-plugin-0.1.2/setup.cfg` & `mkdocs-auto-tag-plugin-0.1.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-auto-tag-plugin
-version = 0.1.2
+version = 0.1.3
 author = six-two
 author_email = pip@six-two.dev
 description = Add tags to your MkDocs pages based on their path / file name
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/six-two/mkdocs-auto-tag-plugin
 license = MIT License
```

### Comparing `mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin/plugin.py` & `mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 
 def replace_placeholders(string_with_placeholders: str, values: list[str]) -> str:
     debug("replace_placeholders - %r - %r", string_with_placeholders, values)
     return string_with_placeholders.format(*values)
 
 class Plugin(BasePlugin[MyConfig]):
-    def on_config(self, config: MkDocsConfig, **kwargs) -> Config:
+    def on_config(self, config: MkDocsConfig, **kwargs) -> MkDocsConfig:
         """
         Called once when the config is loaded.
         It will make modify the config and initialize this plugin.
         """
         self.rules: list[Rule] = []
 
         for key, value in self.config.globs.items():
```

### Comparing `mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin/utils.py` & `mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-auto-tag-plugin-0.1.2/src/mkdocs_auto_tag_plugin.egg-info/PKG-INFO` & `mkdocs-auto-tag-plugin-0.1.3/src/mkdocs_auto_tag_plugin.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-auto-tag-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add tags to your MkDocs pages based on their path / file name
 Home-page: https://github.com/six-two/mkdocs-auto-tag-plugin
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -32,15 +32,17 @@
 
 The files in the `docs/test/` directory implicitely work as tests.
 They should be tagged correctly.
 
 
 ## Notable changes
 
-### HEAD
+### 0.1.3
+
+- Just fixed the `DeprecationWarning` for `warning_filter`
 
 ### 0.1.2
 
 - Just small documentation changes. But I needed to increase the version number to remove the `!!! Warning: Pre alpha: This is currently just a PoC for myself` line from the PyPI site
 
 ### 0.1.1
```

