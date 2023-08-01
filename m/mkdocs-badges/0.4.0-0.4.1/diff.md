# Comparing `tmp/mkdocs-badges-0.4.0.tar.gz` & `tmp/mkdocs-badges-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-badges-0.4.0.tar", last modified: Sat Oct 22 18:00:00 2022, max compression
+gzip compressed data, was "mkdocs-badges-0.4.1.tar", last modified: Tue Aug  1 16:43:16 2023, max compression
```

## Comparing `mkdocs-badges-0.4.0.tar` & `mkdocs-badges-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-10-22 18:00:00.828169 mkdocs-badges-0.4.0/
--rw-r--r--   0 user       (501) staff       (20)     1063 2022-08-04 17:39:49.000000 mkdocs-badges-0.4.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      160 2022-08-04 17:39:49.000000 mkdocs-badges-0.4.0/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     2592 2022-10-22 18:00:00.828218 mkdocs-badges-0.4.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     2043 2022-10-22 17:59:37.000000 mkdocs-badges-0.4.0/README.md
--rw-r--r--   0 user       (501) staff       (20)       85 2022-08-04 17:39:49.000000 mkdocs-badges-0.4.0/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)      801 2022-10-22 18:00:00.828467 mkdocs-badges-0.4.0/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-10-22 18:00:00.824219 mkdocs-badges-0.4.0/src/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-10-22 18:00:00.826483 mkdocs-badges-0.4.0/src/mkdocs_badges/
--rw-r--r--   0 user       (501) staff       (20)      453 2022-08-05 13:12:48.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-10-22 18:00:00.827981 mkdocs-badges-0.4.0/src/mkdocs_badges/assets/
--rw-r--r--   0 user       (501) staff       (20)     1071 2022-08-04 17:39:49.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/assets/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1470 2022-10-22 17:35:51.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/assets/badge.css
--rw-r--r--   0 user       (501) staff       (20)     2942 2022-08-04 17:39:49.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/assets/badge.js
--rw-r--r--   0 user       (501) staff       (20)     1859 2022-08-04 17:47:59.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/assets/install_badge_data.json
--rw-r--r--   0 user       (501) staff       (20)     5404 2022-10-22 17:54:11.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/badge_handler.py
--rw-r--r--   0 user       (501) staff       (20)     2586 2022-08-07 15:24:42.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/badge_html.py
--rw-r--r--   0 user       (501) staff       (20)     1758 2022-08-05 13:02:24.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/install_badge.py
--rwxr-xr-x   0 user       (501) staff       (20)    10719 2022-08-07 15:23:40.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/parser.py
--rw-r--r--   0 user       (501) staff       (20)     3508 2022-10-22 17:54:27.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/plugin.py
--rw-r--r--   0 user       (501) staff       (20)     1748 2022-08-05 13:04:17.000000 mkdocs-badges-0.4.0/src/mkdocs_badges/tag_badge.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-10-22 18:00:00.827326 mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     2592 2022-10-22 18:00:00.000000 mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      676 2022-10-22 18:00:00.000000 mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2022-10-22 18:00:00.000000 mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       53 2022-10-22 18:00:00.000000 mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       14 2022-10-22 18:00:00.000000 mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       14 2022-10-22 18:00:00.000000 mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:43:16.129646 mkdocs-badges-0.4.1/
+-rw-r--r--   0 user       (501) staff       (20)     1063 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      160 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     2895 2023-08-01 16:43:16.129694 mkdocs-badges-0.4.1/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     2295 2023-08-01 16:41:27.000000 mkdocs-badges-0.4.1/README.md
+-rw-r--r--   0 user       (501) staff       (20)       85 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)      841 2023-08-01 16:43:16.129924 mkdocs-badges-0.4.1/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:43:16.125954 mkdocs-badges-0.4.1/src/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:43:16.128047 mkdocs-badges-0.4.1/src/mkdocs_badges/
+-rw-r--r--   0 user       (501) staff       (20)      380 2023-08-01 15:47:22.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:43:16.129294 mkdocs-badges-0.4.1/src/mkdocs_badges/assets/
+-rw-r--r--   0 user       (501) staff       (20)     1071 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/assets/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1470 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/assets/badge.css
+-rw-r--r--   0 user       (501) staff       (20)     2942 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/assets/badge.js
+-rw-r--r--   0 user       (501) staff       (20)     2173 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/assets/install_badge_data.json
+-rw-r--r--   0 user       (501) staff       (20)     5404 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/badge_handler.py
+-rw-r--r--   0 user       (501) staff       (20)     2586 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/badge_html.py
+-rw-r--r--   0 user       (501) staff       (20)     1758 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/install_badge.py
+-rwxr-xr-x   0 user       (501) staff       (20)    10719 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/parser.py
+-rw-r--r--   0 user       (501) staff       (20)     3933 2023-08-01 16:38:04.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/plugin.py
+-rw-r--r--   0 user       (501) staff       (20)     1748 2023-08-01 15:46:26.000000 mkdocs-badges-0.4.1/src/mkdocs_badges/tag_badge.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:43:16.128753 mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     2895 2023-08-01 16:43:16.000000 mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      697 2023-08-01 16:43:16.000000 mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-08-01 16:43:16.000000 mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       53 2023-08-01 16:43:16.000000 mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-08-01 16:43:16.000000 mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-08-01 16:43:16.000000 mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 16:43:16.129436 mkdocs-badges-0.4.1/tests/
+-rw-r--r--   0 user       (501) staff       (20)     2952 2022-08-04 18:04:40.000000 mkdocs-badges-0.4.1/tests/test_parser.py
```

### Comparing `mkdocs-badges-0.4.0/LICENSE` & `mkdocs-badges-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/PKG-INFO` & `mkdocs-badges-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: mkdocs-badges
-Version: 0.4.0
-Summary: Add badges to your mkdocs page
+Version: 0.4.1
+Summary: Add badges to your MkDocs page
 Home-page: https://github.com/six-two/mkdocs-badges
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mkdocs-badges
 [![PyPI version](https://img.shields.io/pypi/v/mkdocs-badges)](https://pypi.org/project/mkdocs-badges/)
 ![License](https://img.shields.io/pypi/l/mkdocs-badges)
@@ -48,15 +49,20 @@
 ```bash
 pip install . && python -m unittest
 ```
 
 
 ## Notable changes
 
-### 0.4.0
+### Version 0.4.1
+
+- Now requires MkDocs 1.5 or newer
+- The included script is now marked as `async` by default, maybe improving loading times a tiny bit. This can be disabled by adding `async: False` to the plugin config in your `mkdocs.yml`
+
+### Version 0.4.0
 
 - Now requires MkDocs 1.4 or newer
 - Updated the layout rules for badges. This should better handle oversized contents (like images or very long texts).
 
 ### Version 0.3.4
 
 - Added single element badges
```

### Comparing `mkdocs-badges-0.4.0/README.md` & `mkdocs-badges-0.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,20 @@
 ```bash
 pip install . && python -m unittest
 ```
 
 
 ## Notable changes
 
-### 0.4.0
+### Version 0.4.1
+
+- Now requires MkDocs 1.5 or newer
+- The included script is now marked as `async` by default, maybe improving loading times a tiny bit. This can be disabled by adding `async: False` to the plugin config in your `mkdocs.yml`
+
+### Version 0.4.0
 
 - Now requires MkDocs 1.4 or newer
 - Updated the layout rules for badges. This should better handle oversized contents (like images or very long texts).
 
 ### Version 0.3.4
 
 - Added single element badges
```

### Comparing `mkdocs-badges-0.4.0/setup.cfg` & `mkdocs-badges-0.4.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [metadata]
 name = mkdocs-badges
-version = 0.4.0
+version = 0.4.1
 author = six-two
 author_email = pip@six-two.dev
-description = Add badges to your mkdocs page
+description = Add badges to your MkDocs page
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/six-two/mkdocs-badges
 license = MIT License
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
 scripts = 
 install_requires = 
-	mkdocs>=1.4.0
+	mkdocs>=1.5.0
 
 [options.entry_points]
 mkdocs.plugins = 
 	badges = mkdocs_badges:BadgesPlugin
 
 [options.packages.find]
 where = src
```

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/assets/__init__.py` & `mkdocs-badges-0.4.1/src/mkdocs_badges/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/assets/badge.css` & `mkdocs-badges-0.4.1/src/mkdocs_badges/assets/badge.css`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/assets/badge.js` & `mkdocs-badges-0.4.1/src/mkdocs_badges/assets/badge.js`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/assets/install_badge_data.json` & `mkdocs-badges-0.4.1/src/mkdocs_badges/assets/install_badge_data.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7692307692307693%*

 * *Differences: {"'pip_github'": "OrderedDict([('title', 'Python package (Github)'), ('link_template', "*

 * *                 "'https://github.com/{{value}}'), ('command_template', 'pip install "*

 * *                 "git+https://github.com/six-two/mkdocs-badges')])",*

 * * "'pip_gitlab'": "OrderedDict([('title', 'Python package (Gitlab)'), ('link_template', "*

 * *                 "'https://gitlab.com/{{value}}'), ('command_template', 'pip install "*

 * *                 "git+https://gitlab.com/six-two/mkdocs-badges')])",*

 * * 'delete': "['']"}*

```diff
@@ -1,13 +1,8 @@
 {
-    "": {
-        "command_template": "{{value}}",
-        "link_template": "{{value}}",
-        "title": ""
-    },
     "aur": {
         "command_template": "sudo pacaur -S {{value}}",
         "link_template": "https://aur.archlinux.org/packages/{{value}}",
         "title": "Arch Linux (AUR)"
     },
     "brew": {
         "command_template": "brew install {{value}}",
@@ -45,13 +40,23 @@
         "title": "npm"
     },
     "pacman": {
         "command_template": "sudo pacman -S {{value}}",
         "link_template": "https://archlinux.org/packages/?name={{value}}",
         "title": "Arch Linux"
     },
+    "pip_github": {
+        "command_template": "pip install git+https://github.com/six-two/mkdocs-badges",
+        "link_template": "https://github.com/{{value}}",
+        "title": "Python package (Github)"
+    },
+    "pip_gitlab": {
+        "command_template": "pip install git+https://gitlab.com/six-two/mkdocs-badges",
+        "link_template": "https://gitlab.com/{{value}}",
+        "title": "Python package (Gitlab)"
+    },
     "pypi": {
         "command_template": "pip install {{value}}",
         "link_template": "https://pypi.org/project/{{value}}",
         "title": "PyPI"
     }
 }
```

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/badge_handler.py` & `mkdocs-badges-0.4.1/src/mkdocs_badges/badge_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/badge_html.py` & `mkdocs-badges-0.4.1/src/mkdocs_badges/badge_html.py`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/install_badge.py` & `mkdocs-badges-0.4.1/src/mkdocs_badges/install_badge.py`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/parser.py` & `mkdocs-badges-0.4.1/src/mkdocs_badges/parser.py`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/plugin.py` & `mkdocs-badges-0.4.1/src/mkdocs_badges/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pip dependency
 import mkdocs
-from mkdocs.config.config_options import Type
-from mkdocs.plugins import BasePlugin
+from mkdocs.config.config_options import Type, ExtraScriptValue
+from mkdocs.plugins import BasePlugin # , event_priority
 from mkdocs.config.base import Config
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 from mkdocs.structure.files import Files
 # local files
 from . import warning
 from .install_badge import InstallBadgeManager
@@ -18,44 +18,52 @@
 
 
 class BadgesPluginConfig(Config):
     enabled = Type(bool, default=True)
     # Options to allow overwriting CSS and/or JS files
     badge_css = Type(str, default="")
     badge_js = Type(str, default="")
+    # Load script as async? You can deactivate it if it causes trouble
+    async_ = Type(bool, default=True)
     # Allow overwriting the install badge data
     install_badge_data = Type(str, default="")
     # Base link for the tag links
     tag_page_link = Type(str, default="/index.html")
 
 
 class BadgesPlugin(BasePlugin[BadgesPluginConfig]):
-    def on_config(self, config: MkDocsConfig, **kwargs) -> Config:
+    def on_config(self, config: MkDocsConfig, **kwargs) -> MkDocsConfig:
         """
         Called once when the config is loaded.
         It will make modify the config and initialize this plugin.
         """
         # Make sure that the CSS and JS badge files are included on every page
         badge_css_path = self.config.badge_css or DEFAULT_BADGE_CSS_PATH
         extra_css = config.extra_css
         if badge_css_path not in extra_css:
             extra_css.append(badge_css_path)
 
-        badge_js_path = self.config.badge_js or DEFAULT_BADGE_JS_PATH
+        badge_js_path = ExtraScriptValue(self.config.badge_js or DEFAULT_BADGE_JS_PATH)
+        if self.config.async_:
+            badge_js_path.async_ = True
+        
         extra_js = config.extra_javascript
         if badge_js_path not in extra_js:
             extra_js.append(badge_js_path)
 
         # Load the install badge data from the data file
         install_badge_data_path = self.config.install_badge_data or INSTALL_BADGE_DATA
         self.install_badge_manager = InstallBadgeManager(install_badge_data_path)
         self.tag_badge_manager = TagBadgeManager(self.config.tag_page_link)
 
         return config
 
+    # @event_priority(50)
+    # Earlier than most other plugins to update the tags properly. Did not work
+    # SEE https://www.mkdocs.org/dev-guide/plugins/#event-priorities
     def on_page_markdown(self, markdown: str, page: Page, config: MkDocsConfig, files: Files) -> str:
         """
         The page_markdown event is called after the page's markdown is loaded from file and can be used to alter the Markdown source text. The meta- data has been stripped off and is available as page.meta at this point.
         See: https://www.mkdocs.org/dev-guide/plugins/#on_page_markdown
         """
         try:
             if self.config.enabled:
```

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges/tag_badge.py` & `mkdocs-badges-0.4.1/src/mkdocs_badges/tag_badge.py`

 * *Files identical despite different names*

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/PKG-INFO` & `mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: mkdocs-badges
-Version: 0.4.0
-Summary: Add badges to your mkdocs page
+Version: 0.4.1
+Summary: Add badges to your MkDocs page
 Home-page: https://github.com/six-two/mkdocs-badges
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mkdocs-badges
 [![PyPI version](https://img.shields.io/pypi/v/mkdocs-badges)](https://pypi.org/project/mkdocs-badges/)
 ![License](https://img.shields.io/pypi/l/mkdocs-badges)
@@ -48,15 +49,20 @@
 ```bash
 pip install . && python -m unittest
 ```
 
 
 ## Notable changes
 
-### 0.4.0
+### Version 0.4.1
+
+- Now requires MkDocs 1.5 or newer
+- The included script is now marked as `async` by default, maybe improving loading times a tiny bit. This can be disabled by adding `async: False` to the plugin config in your `mkdocs.yml`
+
+### Version 0.4.0
 
 - Now requires MkDocs 1.4 or newer
 - Updated the layout rules for badges. This should better handle oversized contents (like images or very long texts).
 
 ### Version 0.3.4
 
 - Added single element badges
```

### Comparing `mkdocs-badges-0.4.0/src/mkdocs_badges.egg-info/SOURCES.txt` & `mkdocs-badges-0.4.1/src/mkdocs_badges.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 src/mkdocs_badges.egg-info/dependency_links.txt
 src/mkdocs_badges.egg-info/entry_points.txt
 src/mkdocs_badges.egg-info/requires.txt
 src/mkdocs_badges.egg-info/top_level.txt
 src/mkdocs_badges/assets/__init__.py
 src/mkdocs_badges/assets/badge.css
 src/mkdocs_badges/assets/badge.js
-src/mkdocs_badges/assets/install_badge_data.json
+src/mkdocs_badges/assets/install_badge_data.json
+tests/test_parser.py
```

