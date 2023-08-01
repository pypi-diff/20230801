# Comparing `tmp/django-friendly-captcha-0.1.7.tar.gz` & `tmp/django-friendly-captcha-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-friendly-captcha-0.1.7.tar", last modified: Sun Apr  2 10:32:30 2023, max compression
+gzip compressed data, was "django-friendly-captcha-0.1.8.tar", last modified: Tue Aug  1 18:16:37 2023, max compression
```

## Comparing `django-friendly-captcha-0.1.7.tar` & `django-friendly-captcha-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:30.284582 django-friendly-captcha-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-02 10:32:30.284582 django-friendly-captcha-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:30.284582 django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-02 10:32:30.000000 django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-02 10:32:30.000000 django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 10:32:30.000000 django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 10:32:30.000000 django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-02 10:32:30.000000 django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-02 10:32:30.000000 django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:30.284582 django-friendly-captcha-0.1.7/friendly_captcha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:30.280582 django-friendly-captcha-0.1.7/friendly_captcha/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:30.280582 django-friendly-captcha-0.1.7/friendly_captcha/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:30.284582 django-friendly-captcha-0.1.7/friendly_captcha/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:30.280582 django-friendly-captcha-0.1.7/friendly_captcha/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:32:30.284582 django-friendly-captcha-0.1.7/friendly_captcha/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/friendly_captcha/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 10:32:30.284582 django-friendly-captcha-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-02 10:32:21.000000 django-friendly-captcha-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:16:36.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/friendly_captcha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.031075 django-friendly-captcha-0.1.8/friendly_captcha/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.031075 django-friendly-captcha-0.1.8/friendly_captcha/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/friendly_captcha/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.031075 django-friendly-captcha-0.1.8/friendly_captcha/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/friendly_captcha/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/setup.py
```

### Comparing `django-friendly-captcha-0.1.7/LICENSE` & `django-friendly-captcha-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.7/PKG-INFO` & `django-friendly-captcha-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-friendly-captcha
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django library for friendly captcha
 Home-page: https://github.com/christianwgd/django-friendly-captcha
 Download-URL: 
 Author: Christian Wiegand
 Author-email: christianwgd@gmail.com
 Maintainer: Christian Wiegand
 Maintainer-email: christianwgd@gmail.com
@@ -80,15 +80,15 @@
                 'name', 'email', 'subject', 'text'
             )
 
         captcha = FrcCaptchaField()
 
 As of version 0.1.7 the javascript static assets are included in
 the widget, so there is no need to do that in your project templates.
-Version 0.1.7 includes friendly captcha version 0.9.11 javascript files.
+Version 0.1.8 includes friendly captcha version 0.9.12 javascript files.
 If you need a different version you can set these by providing
 them in your settings:
 
 .. code-block::
 
     FRC_WIDGET_MODULE_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.module.min.js'
     FRC_WIDGET_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.min.js'
```

### Comparing `django-friendly-captcha-0.1.7/README.rst` & `django-friendly-captcha-0.1.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 'name', 'email', 'subject', 'text'
             )
 
         captcha = FrcCaptchaField()
 
 As of version 0.1.7 the javascript static assets are included in
 the widget, so there is no need to do that in your project templates.
-Version 0.1.7 includes friendly captcha version 0.9.11 javascript files.
+Version 0.1.8 includes friendly captcha version 0.9.12 javascript files.
 If you need a different version you can set these by providing
 them in your settings:
 
 .. code-block::
 
     FRC_WIDGET_MODULE_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.module.min.js'
     FRC_WIDGET_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.min.js'
```

### Comparing `django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/PKG-INFO` & `django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-friendly-captcha
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django library for friendly captcha
 Home-page: https://github.com/christianwgd/django-friendly-captcha
 Download-URL: 
 Author: Christian Wiegand
 Author-email: christianwgd@gmail.com
 Maintainer: Christian Wiegand
 Maintainer-email: christianwgd@gmail.com
@@ -80,15 +80,15 @@
                 'name', 'email', 'subject', 'text'
             )
 
         captcha = FrcCaptchaField()
 
 As of version 0.1.7 the javascript static assets are included in
 the widget, so there is no need to do that in your project templates.
-Version 0.1.7 includes friendly captcha version 0.9.11 javascript files.
+Version 0.1.8 includes friendly captcha version 0.9.12 javascript files.
 If you need a different version you can set these by providing
 them in your settings:
 
 .. code-block::
 
     FRC_WIDGET_MODULE_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.module.min.js'
     FRC_WIDGET_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.min.js'
```

### Comparing `django-friendly-captcha-0.1.7/django_friendly_captcha.egg-info/SOURCES.txt` & `django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.7/friendly_captcha/fields.py` & `django-friendly-captcha-0.1.8/friendly_captcha/fields.py`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.7/friendly_captcha/locale/de/LC_MESSAGES/django.po` & `django-friendly-captcha-0.1.8/friendly_captcha/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.7/friendly_captcha/locale/en/LC_MESSAGES/django.po` & `django-friendly-captcha-0.1.8/friendly_captcha/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.7/friendly_captcha/widgets.py` & `django-friendly-captcha-0.1.8/friendly_captcha/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 class FrcCaptchaWidget(Widget):
 
     def __init__(self):
         super().__init__()
         self.site_key = getattr(settings, 'FRC_CAPTCHA_SITE_KEY', None)
         self.frc_widget_module_js = getattr(
             settings, 'FRC_WIDGET_MODULE_JS',
-            'https://unpkg.com/friendly-challenge@0.9.11/widget.module.min.js',
+            'https://unpkg.com/friendly-challenge@0.9.12/widget.module.min.js',
         )
-        self.frc_widget_js = (
+        self.frc_widget_js = getattr(
             settings, 'FRC_WIDGET_JS',
-            'https://unpkg.com/friendly-challenge@0.9.11/widget.min.js'
+            'https://unpkg.com/friendly-challenge@0.9.12/widget.min.js'
         )
 
     def render(self, name, value, attrs=None, renderer=None):
         attrs['data-lang'] = translation.get_language()
         attrs['data-sitekey'] = self.site_key
         attrs['data-solution-field-name'] = name
         attrs['class'] = 'frc-captcha'
```

### Comparing `django-friendly-captcha-0.1.7/setup.py` & `django-friendly-captcha-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='django-friendly-captcha',
-    version='0.1.7',
+    version='0.1.8',
     description='Django library for friendly captcha',
     long_description=read('README.rst'),
     url='https://github.com/christianwgd/django-friendly-captcha',
     download_url='',
     author='Christian Wiegand',
     author_email='christianwgd@gmail.com',
     maintainer='Christian Wiegand',
```

