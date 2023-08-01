# Comparing `tmp/wagtail-icon-chooser-0.0.4.tar.gz` & `tmp/wagtail-icon-chooser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-icon-chooser-0.0.4.tar", last modified: Mon Jul 10 08:25:52 2023, max compression
+gzip compressed data, was "wagtail-icon-chooser-0.0.5.tar", last modified: Tue Aug  1 12:53:33 2023, max compression
```

## Comparing `wagtail-icon-chooser-0.0.4.tar` & `wagtail-icon-chooser-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 08:25:52.000000 wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/css/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/js/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.456918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/wagtailiconchooser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/wagtailiconchooser/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:52.460918 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-10 08:25:35.000000 wagtail-icon-chooser-0.0.4/wagtailiconchooser/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.245140 wagtail-icon-chooser-0.0.5/wagtail_icon_chooser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-08-01 12:53:33.000000 wagtail-icon-chooser-0.0.5/wagtail_icon_chooser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-01 12:53:33.000000 wagtail-icon-chooser-0.0.5/wagtail_icon_chooser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:53:33.000000 wagtail-icon-chooser-0.0.5/wagtail_icon_chooser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 12:53:33.000000 wagtail-icon-chooser-0.0.5/wagtail_icon_chooser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 12:53:33.000000 wagtail-icon-chooser-0.0.5/wagtail_icon_chooser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.241140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.245140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/wagtailiconchooser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/wagtailiconchooser/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/wagtailiconchooser/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.245140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.245140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/templates/wagtailiconchooser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/templates/wagtailiconchooser/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:33.249140 wagtail-icon-chooser-0.0.5/wagtailiconchooser/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-01 12:53:14.000000 wagtail-icon-chooser-0.0.5/wagtailiconchooser/widgets.py
```

### Comparing `wagtail-icon-chooser-0.0.4/PKG-INFO` & `wagtail-icon-chooser-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-icon-chooser
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wagtail Icon Chooser
 Home-page: https://github.com/wmo-raf/wagtail-icon-chooser
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
@@ -170,7 +170,44 @@
     <use href="#icon-{{ page.icon }}"></use>
 </svg>
 ```
 
 `NOTE` This approach will load all the icons added to Wagtail (using the `register_icons` hook) to your template. If you
 have registered many SVG icons, this might increase your page's loading bandwidth and might not be efficient since you
 might not use all the icons.
+
+If you have a list of icons that are known, you can create a svg sprite containing only those icons, by using the
+function `get_svg_sprite_for_icons`. This can be used in a view. For example:
+
+```python
+from django.shortcuts import render
+from wagtailiconchooser.utils import get_svg_sprite_for_icons
+
+
+def my_view(request):
+    icons = ["some-icon", "some-other-icon", ...]
+    svg_sprite = get_svg_sprite_for_icons(icons)
+
+    context = {
+        "svg_sprite": svg_sprite
+    }
+
+    return render(request, "template.html", context=context)
+```
+
+In your `template.html` you will have access to the `svg_sprite` context, and you can render and use as below:
+
+```html
+
+<div>
+    {{ svg_sprite|safe }}
+</div>
+
+<svg class="icon">
+    <use href="#icon-some-icon"></use>
+</svg>
+
+<svg class="icon">
+    <use href="#icon-some-other-icon"></use>
+</svg>
+
+```
```

### Comparing `wagtail-icon-chooser-0.0.4/README.md` & `wagtail-icon-chooser-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -149,7 +149,44 @@
     <use href="#icon-{{ page.icon }}"></use>
 </svg>
 ```
 
 `NOTE` This approach will load all the icons added to Wagtail (using the `register_icons` hook) to your template. If you
 have registered many SVG icons, this might increase your page's loading bandwidth and might not be efficient since you
 might not use all the icons.
+
+If you have a list of icons that are known, you can create a svg sprite containing only those icons, by using the
+function `get_svg_sprite_for_icons`. This can be used in a view. For example:
+
+```python
+from django.shortcuts import render
+from wagtailiconchooser.utils import get_svg_sprite_for_icons
+
+
+def my_view(request):
+    icons = ["some-icon", "some-other-icon", ...]
+    svg_sprite = get_svg_sprite_for_icons(icons)
+
+    context = {
+        "svg_sprite": svg_sprite
+    }
+
+    return render(request, "template.html", context=context)
+```
+
+In your `template.html` you will have access to the `svg_sprite` context, and you can render and use as below:
+
+```html
+
+<div>
+    {{ svg_sprite|safe }}
+</div>
+
+<svg class="icon">
+    <use href="#icon-some-icon"></use>
+</svg>
+
+<svg class="icon">
+    <use href="#icon-some-other-icon"></use>
+</svg>
+
+```
```

### Comparing `wagtail-icon-chooser-0.0.4/setup.cfg` & `wagtail-icon-chooser-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-icon-chooser
-version = 0.0.4
+version = 0.0.5
 description = Wagtail Icon Chooser
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-icon-chooser
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/PKG-INFO` & `wagtail-icon-chooser-0.0.5/wagtail_icon_chooser.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-icon-chooser
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wagtail Icon Chooser
 Home-page: https://github.com/wmo-raf/wagtail-icon-chooser
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
@@ -170,7 +170,44 @@
     <use href="#icon-{{ page.icon }}"></use>
 </svg>
 ```
 
 `NOTE` This approach will load all the icons added to Wagtail (using the `register_icons` hook) to your template. If you
 have registered many SVG icons, this might increase your page's loading bandwidth and might not be efficient since you
 might not use all the icons.
+
+If you have a list of icons that are known, you can create a svg sprite containing only those icons, by using the
+function `get_svg_sprite_for_icons`. This can be used in a view. For example:
+
+```python
+from django.shortcuts import render
+from wagtailiconchooser.utils import get_svg_sprite_for_icons
+
+
+def my_view(request):
+    icons = ["some-icon", "some-other-icon", ...]
+    svg_sprite = get_svg_sprite_for_icons(icons)
+
+    context = {
+        "svg_sprite": svg_sprite
+    }
+
+    return render(request, "template.html", context=context)
+```
+
+In your `template.html` you will have access to the `svg_sprite` context, and you can render and use as below:
+
+```html
+
+<div>
+    {{ svg_sprite|safe }}
+</div>
+
+<svg class="icon">
+    <use href="#icon-some-icon"></use>
+</svg>
+
+<svg class="icon">
+    <use href="#icon-some-other-icon"></use>
+</svg>
+
+```
```

### Comparing `wagtail-icon-chooser-0.0.4/wagtail_icon_chooser.egg-info/SOURCES.txt` & `wagtail-icon-chooser-0.0.5/wagtail_icon_chooser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.4/wagtailiconchooser/blocks.py` & `wagtail-icon-chooser-0.0.5/wagtailiconchooser/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css` & `wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.4/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js` & `wagtail-icon-chooser-0.0.5/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.4/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html` & `wagtail-icon-chooser-0.0.5/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.4/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py` & `wagtail-icon-chooser-0.0.5/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.4/wagtailiconchooser/utils.py` & `wagtail-icon-chooser-0.0.5/wagtailiconchooser/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,23 +28,39 @@
                         if icon_id.startswith("icon-"):
                             icon_id = icon_id.replace("icon-", "")
                         _svg_icons[icon_id] = svg_str
                 else:
                     symbol = doc.getElementsByTagName("symbol")
                     if symbol:
                         symbol = symbol[0]
-                        icon_id = symbol.getAttribute("id")
-                        if icon_id:
-                            if icon_id.startswith("icon-"):
-                                icon_id = icon_id.replace("icon-", "")
+                        symbol_icon_id = symbol.getAttribute("id")
+                        if symbol_icon_id:
+                            if symbol_icon_id.startswith("icon-"):
+                                icon_id = symbol_icon_id.replace("icon-", "")
                                 svg_str = symbol.toxml().replace("symbol", "svg")
                                 doc = minidom.parseString(svg_str)
                                 svg = doc.getElementsByTagName("svg")
                                 if svg:
                                     svg = svg[0]
                                     svg.setAttribute('xmlns', 'http://www.w3.org/2000/svg')
-                                    svg.setAttribute("id", icon_id)
+                                    svg.setAttribute("id", symbol_icon_id)
                                     _svg_icons[icon_id] = mark_safe(svg.toxml())
             except Exception:
                 pass
 
     return _svg_icons
+
+
+def get_svg_sprite_for_icons(icons_list):
+    svg_icons = get_svg_icons()
+    combined_icon_markup = ""
+    for icon in icons_list:
+        svg_str = svg_icons.get(icon)
+        if svg_str:
+            combined_icon_markup += (
+                svg_str.replace('xmlns="http://www.w3.org/2000/svg"', "").replace("svg", "symbol")
+            )
+    _icons_html = render_to_string(
+        "wagtailadmin/shared/icons.html", {"icons": combined_icon_markup}
+    )
+
+    return _icons_html
```

### Comparing `wagtail-icon-chooser-0.0.4/wagtailiconchooser/widgets.py` & `wagtail-icon-chooser-0.0.5/wagtailiconchooser/widgets.py`

 * *Files identical despite different names*

