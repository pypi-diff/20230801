# Comparing `tmp/palettepal-0.1.tar.gz` & `tmp/palettepal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palettepal-0.1.tar", last modified: Mon Jul 31 02:19:44 2023, max compression
+gzip compressed data, was "palettepal-0.1.1.tar", last modified: Tue Aug  1 00:56:12 2023, max compression
```

## Comparing `palettepal-0.1.tar` & `palettepal-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-07-31 02:19:44.831854 palettepal-0.1/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1070 2023-07-31 01:43:03.000000 palettepal-0.1/LICENSE
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      775 2023-07-31 02:19:44.831854 palettepal-0.1/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      213 2023-07-31 01:59:57.000000 palettepal-0.1/README.md
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-07-31 02:19:44.826854 palettepal-0.1/palettepal/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       20 2023-07-31 01:34:20.000000 palettepal-0.1/palettepal/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      105 2023-07-31 01:16:26.000000 palettepal-0.1/palettepal/__main__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    23463 2023-07-31 02:03:06.000000 palettepal-0.1/palettepal/colorapp.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8874 2023-07-31 01:34:06.000000 palettepal-0.1/palettepal/palette.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7654 2023-07-31 01:35:31.000000 palettepal-0.1/palettepal/slider.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-07-31 02:19:44.830854 palettepal-0.1/palettepal.egg-info/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      775 2023-07-31 02:19:44.000000 palettepal-0.1/palettepal.egg-info/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      352 2023-07-31 02:19:44.000000 palettepal-0.1/palettepal.egg-info/SOURCES.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-07-31 02:19:44.000000 palettepal-0.1/palettepal.egg-info/dependency_links.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       24 2023-07-31 02:19:44.000000 palettepal-0.1/palettepal.egg-info/requires.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       11 2023-07-31 02:19:44.000000 palettepal-0.1/palettepal.egg-info/top_level.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-07-31 02:19:44.000000 palettepal-0.1/palettepal.egg-info/zip-safe
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       80 2023-07-15 18:32:34.000000 palettepal-0.1/pyproject.toml
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      734 2023-07-31 02:19:44.837854 palettepal-0.1/setup.cfg
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-08-01 00:56:12.114833 palettepal-0.1.1/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1070 2023-07-31 01:43:03.000000 palettepal-0.1.1/LICENSE
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1549 2023-08-01 00:56:12.114833 palettepal-0.1.1/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      985 2023-08-01 00:53:57.000000 palettepal-0.1.1/README.md
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-08-01 00:56:12.110834 palettepal-0.1.1/palettepal/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       22 2023-08-01 00:48:33.000000 palettepal-0.1.1/palettepal/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      105 2023-07-31 01:16:26.000000 palettepal-0.1.1/palettepal/__main__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    23598 2023-07-31 02:31:29.000000 palettepal-0.1.1/palettepal/colorapp.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8874 2023-07-31 01:34:06.000000 palettepal-0.1.1/palettepal/palette.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7654 2023-07-31 01:35:31.000000 palettepal-0.1.1/palettepal/slider.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2023-08-01 00:56:12.114833 palettepal-0.1.1/palettepal.egg-info/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1549 2023-08-01 00:56:12.000000 palettepal-0.1.1/palettepal.egg-info/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      389 2023-08-01 00:56:12.000000 palettepal-0.1.1/palettepal.egg-info/SOURCES.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-08-01 00:56:12.000000 palettepal-0.1.1/palettepal.egg-info/dependency_links.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       56 2023-08-01 00:56:12.000000 palettepal-0.1.1/palettepal.egg-info/entry_points.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       24 2023-08-01 00:56:12.000000 palettepal-0.1.1/palettepal.egg-info/requires.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       11 2023-08-01 00:56:12.000000 palettepal-0.1.1/palettepal.egg-info/top_level.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2023-07-31 02:19:44.000000 palettepal-0.1.1/palettepal.egg-info/zip-safe
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       80 2023-07-15 18:32:34.000000 palettepal-0.1.1/pyproject.toml
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      816 2023-08-01 00:56:12.115833 palettepal-0.1.1/setup.cfg
```

### Comparing `palettepal-0.1/LICENSE` & `palettepal-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `palettepal-0.1/palettepal/colorapp.py` & `palettepal-0.1.1/palettepal/colorapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,19 @@
                 Binding('f1', 'select_swatch(1)', 'Color 1', show=False),
                 Binding('f2', 'select_swatch(2)', 'Color 2', show=False),
                 Binding('f3', 'select_swatch(3)', 'Color 3', show=False),
                 Binding('f4', 'select_swatch(4)', 'Color 4', show=False),
                 Binding('f5', 'select_swatch(5)', 'Color 5', show=False),
                 Binding('h', 'copy("hsl")', 'Copy HSL', show=True),
                 Binding('r', 'copy("rgb")', 'Copy RGB', show=True),
-                Binding('x', 'copy("hex")', 'Copy Hex', show=True)]
+                Binding('x', 'copy("hex")', 'Copy Hex', show=True),
+                Binding('?', 'screenshot', 'Screenshot', show=False)]
+
+    def action_screenshot(self):
+        self.save_screenshot()
 
     def compose(self) -> ComposeResult:
         yield Header()
         yield ColorPicker()
         with Horizontal():
             yield ColorNumbers()
             yield ColorSwatch(color=palette.Color(0,100,50), label='<F1>', id='color1')
```

### Comparing `palettepal-0.1/palettepal/palette.py` & `palettepal-0.1.1/palettepal/palette.py`

 * *Files identical despite different names*

### Comparing `palettepal-0.1/palettepal/slider.py` & `palettepal-0.1.1/palettepal/slider.py`

 * *Files identical despite different names*

