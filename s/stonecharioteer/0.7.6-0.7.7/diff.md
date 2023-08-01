# Comparing `tmp/stonecharioteer-0.7.6.tar.gz` & `tmp/stonecharioteer-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stonecharioteer-0.7.6.tar", max compression
+gzip compressed data, was "stonecharioteer-0.7.7.tar", max compression
```

## Comparing `stonecharioteer-0.7.6.tar` & `stonecharioteer-0.7.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0      708 2023-05-17 06:32:29.401878 stonecharioteer-0.7.6/pyproject.toml
--rw-r--r--   0        0        0       64 2023-05-17 06:32:34.642209 stonecharioteer-0.7.6/stonecharioteer/__init__.py
--rw-r--r--   0        0        0      586 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/constants.py
--rw-r--r--   0        0        0     1118 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/logger.py
--rw-r--r--   0        0        0     1922 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/qtile/__init__.py
--rw-r--r--   0        0        0      422 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/qtile/groups.py
--rw-r--r--   0        0        0      573 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/qtile/inputs.py
--rwxr-xr-x   0        0        0     4934 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/qtile/keymaps.py
--rw-r--r--   0        0        0      150 2023-02-14 06:50:42.458837 stonecharioteer-0.7.6/stonecharioteer/qtile/layouts.py
--rwxr-xr-x   0        0        0     6013 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/qtile/panels.py
--rw-r--r--   0        0        0     2499 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/qtile/screens.py
--rw-r--r--   0        0        0     1324 2022-12-19 06:25:17.895784 stonecharioteer-0.7.6/stonecharioteer/utils/displays.py
--rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 stonecharioteer-0.7.6/setup.py
--rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 stonecharioteer-0.7.6/PKG-INFO
+-rwxr-xr-x   0        0        0      694 2023-08-01 06:58:44.361308 stonecharioteer-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-05-17 06:34:36.239890 stonecharioteer-0.7.7/stonecharioteer/__init__.py
+-rw-r--r--   0        0        0      586 2022-12-19 06:25:17.895784 stonecharioteer-0.7.7/stonecharioteer/constants.py
+-rw-r--r--   0        0        0     1118 2022-12-19 06:25:17.895784 stonecharioteer-0.7.7/stonecharioteer/logger.py
+-rw-r--r--   0        0        0     1922 2022-12-19 06:25:17.895784 stonecharioteer-0.7.7/stonecharioteer/qtile/__init__.py
+-rw-r--r--   0        0        0      422 2022-12-19 06:25:17.895784 stonecharioteer-0.7.7/stonecharioteer/qtile/groups.py
+-rw-r--r--   0        0        0      573 2022-12-19 06:25:17.895784 stonecharioteer-0.7.7/stonecharioteer/qtile/inputs.py
+-rwxr-xr-x   0        0        0     4934 2022-12-19 06:25:17.895784 stonecharioteer-0.7.7/stonecharioteer/qtile/keymaps.py
+-rw-r--r--   0        0        0      150 2023-05-17 06:34:36.239890 stonecharioteer-0.7.7/stonecharioteer/qtile/layouts.py
+-rwxr-xr-x   0        0        0     5273 2023-08-01 06:57:14.245544 stonecharioteer-0.7.7/stonecharioteer/qtile/panels.py
+-rw-r--r--   0        0        0     2499 2022-12-19 06:25:17.895784 stonecharioteer-0.7.7/stonecharioteer/qtile/screens.py
+-rw-r--r--   0        0        0     1324 2022-12-19 06:25:17.895784 stonecharioteer-0.7.7/stonecharioteer/utils/displays.py
+-rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 stonecharioteer-0.7.7/setup.py
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 stonecharioteer-0.7.7/PKG-INFO
```

### Comparing `stonecharioteer-0.7.6/pyproject.toml` & `stonecharioteer-0.7.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stonecharioteer"
-version = "0.7.6"
+version = "0.7.7"
 description = "My personal utils and configs, managed via python library"
 authors = ["Vinay Keerthi <11478411+stonecharioteer@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
 qtile = ">=0.18.1"
@@ -16,16 +16,16 @@
 python-xlib = "^0.31"
 typeguard = "^2.13.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pre-commit = "^2.15.0"
 ipython = "^7.29.0"
-black = "^21.12b0"
+black = "*"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
-black = "^22.12.0"
+black = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stonecharioteer-0.7.6/stonecharioteer/constants.py` & `stonecharioteer-0.7.7/stonecharioteer/constants.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.6/stonecharioteer/logger.py` & `stonecharioteer-0.7.7/stonecharioteer/logger.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.6/stonecharioteer/qtile/__init__.py` & `stonecharioteer-0.7.7/stonecharioteer/qtile/__init__.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.6/stonecharioteer/qtile/inputs.py` & `stonecharioteer-0.7.7/stonecharioteer/qtile/inputs.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.6/stonecharioteer/qtile/keymaps.py` & `stonecharioteer-0.7.7/stonecharioteer/qtile/keymaps.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.6/stonecharioteer/qtile/panels.py` & `stonecharioteer-0.7.7/stonecharioteer/qtile/panels.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,50 +97,27 @@
             TextBox(
                 text="]",
                 foreground=colors[6],
                 background=colors[0],
                 font=cfg.get("font", FONT),
                 fontsize=cfg.get("font_size", FONT_SIZE),
             ),
-            quick_exit,
             get_sep(cfg),
             Spacer(length=STRETCH, foreground=colors[2], background=colors[0]),
-            cpu_indicator,
             get_sep(cfg),
-            memory_indicator,
-            get_sep(cfg),
-            TextBox(
-                text="HDD:",
-                foreground=colors[6],
-                background=colors[0],
-                font=cfg.get("font", FONT),
-                fontsize=cfg.get("font_size", FONT_SIZE),
-            ),
-            hdd_indicator,
-            get_sep(cfg),
-            system_tray,
             TextBox(
                 text="Net:",
                 foreground=colors[6],
                 background=colors[0],
                 font=cfg.get("font", FONT),
                 fontsize=cfg.get("font_size", FONT_SIZE),
             ),
             network_indicator,
             get_sep(cfg),
-            TextBox(
-                text="Vol:",
-                foreground=colors[6],
-                background=colors[0],
-                font=cfg.get("font", FONT),
-                fontsize=cfg.get("font_size", FONT_SIZE),
-            ),
-            volume_control,
-            get_sep(cfg),
-            capslock_numlock_indicator,
+            system_tray,
             Sep(linewidth=0, padding=5, foreground=colors[2], background=colors[0]),
         ],
         default_size,
     )
     return default_top_bar
```

### Comparing `stonecharioteer-0.7.6/stonecharioteer/qtile/screens.py` & `stonecharioteer-0.7.7/stonecharioteer/qtile/screens.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.6/stonecharioteer/utils/displays.py` & `stonecharioteer-0.7.7/stonecharioteer/utils/displays.py`

 * *Files identical despite different names*

### Comparing `stonecharioteer-0.7.6/setup.py` & `stonecharioteer-0.7.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'rich>=10.12.0,<11.0.0',
  'toml>=0.10.2,<0.11.0',
  'typeguard>=2.13.3,<3.0.0',
  'types-toml>=0.10.1,<0.11.0']
 
 setup_kwargs = {
     'name': 'stonecharioteer',
-    'version': '0.7.6',
+    'version': '0.7.7',
     'description': 'My personal utils and configs, managed via python library',
     'long_description': 'None',
     'author': 'Vinay Keerthi',
     'author_email': '11478411+stonecharioteer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stonecharioteer-0.7.6/PKG-INFO` & `stonecharioteer-0.7.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stonecharioteer
-Version: 0.7.6
+Version: 0.7.7
 Summary: My personal utils and configs, managed via python library
 Author: Vinay Keerthi
 Author-email: 11478411+stonecharioteer@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

