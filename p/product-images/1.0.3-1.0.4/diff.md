# Comparing `tmp/product-images-1.0.3.tar.gz` & `tmp/product-images-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "product-images-1.0.3.tar", last modified: Thu Jul  6 07:36:20 2023, max compression
+gzip compressed data, was "product-images-1.0.4.tar", last modified: Tue Aug  1 12:57:23 2023, max compression
```

## Comparing `product-images-1.0.3.tar` & `product-images-1.0.4.tar`

### file list

```diff
@@ -1,45 +1,42 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.033166 product-images-1.0.3/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 product-images-1.0.3/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 product-images-1.0.3/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      339 2023-07-06 07:36:20.033166 product-images-1.0.3/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-14 15:22:21.000000 product-images-1.0.3/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      270 2022-09-07 19:14:03.000000 product-images-1.0.3/product_images/actions.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      668 2022-09-07 19:14:03.000000 product-images-1.0.3/product_images/fields.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2081 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/forms.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images/locale/ru/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)      518 2022-07-21 04:00:27.000000 product-images-1.0.3/product_images/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     1803 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1319 2022-07-21 04:00:27.000000 product-images-1.0.3/product_images/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     2024 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1102 2023-07-06 07:35:21.000000 product-images-1.0.3/product_images/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:13.000000 product-images-1.0.3/product_images/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2577 2022-09-07 19:14:03.000000 product-images-1.0.3/product_images/models.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images/static/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.033166 product-images-1.0.3/product_images/static/dropzone/
--rw-rw-r--   0 dev       (1000) dev       (1000)     9717 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/static/dropzone/dropzone.min.css
--rw-rw-r--   0 dev       (1000) dev       (1000)    43003 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/static/dropzone/dropzone.min.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.033166 product-images-1.0.3/product_images/static/file-manager/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1090 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/static/file-manager/file-manager.css
--rw-rw-r--   0 dev       (1000) dev       (1000)     2953 2023-01-15 17:09:23.000000 product-images-1.0.3/product_images/static/file-manager/file-manager.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.033166 product-images-1.0.3/product_images/templates/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1034 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/templates/product-images-form.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      393 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      354 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/utils.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1585 2022-09-07 19:14:03.000000 product-images-1.0.3/product_images/views.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      402 2022-07-21 03:58:58.000000 product-images-1.0.3/product_images/widgets.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-06 07:36:20.029166 product-images-1.0.3/product_images.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      339 2023-07-06 07:36:19.000000 product-images-1.0.3/product_images.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      994 2023-07-06 07:36:19.000000 product-images-1.0.3/product_images.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-07-06 07:36:19.000000 product-images-1.0.3/product_images.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       25 2023-07-06 07:36:19.000000 product-images-1.0.3/product_images.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       15 2023-07-06 07:36:19.000000 product-images-1.0.3/product_images.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       25 2023-01-15 17:10:32.000000 product-images-1.0.3/requirements.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-07-06 07:36:20.033166 product-images-1.0.3/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      537 2023-07-06 07:35:53.000000 product-images-1.0.3/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 product-images-1.0.4/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 product-images-1.0.4/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      339 2023-08-01 12:57:23.316405 product-images-1.0.4/PKG-INFO
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      270 2022-09-07 19:14:03.000000 product-images-1.0.4/product_images/actions.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      668 2022-09-07 19:14:03.000000 product-images-1.0.4/product_images/fields.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2081 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/forms.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/locale/ru/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      518 2022-07-21 04:00:27.000000 product-images-1.0.4/product_images/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1803 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1319 2022-07-21 04:00:27.000000 product-images-1.0.4/product_images/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2024 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1102 2023-07-06 07:35:21.000000 product-images-1.0.4/product_images/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-06-10 13:48:13.000000 product-images-1.0.4/product_images/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2569 2023-08-01 12:53:41.000000 product-images-1.0.4/product_images/models.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/static/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/static/dropzone/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     9717 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/static/dropzone/dropzone.min.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)    43003 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/static/dropzone/dropzone.min.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/static/file-manager/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1090 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/static/file-manager/file-manager.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2953 2023-01-15 17:09:23.000000 product-images-1.0.4/product_images/static/file-manager/file-manager.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images/templates/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1034 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/templates/product-images-form.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      393 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      354 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/utils.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1585 2022-09-07 19:14:03.000000 product-images-1.0.4/product_images/views.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      402 2022-07-21 03:58:58.000000 product-images-1.0.4/product_images/widgets.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-01 12:57:23.316405 product-images-1.0.4/product_images.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      339 2023-08-01 12:57:23.000000 product-images-1.0.4/product_images.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      920 2023-08-01 12:57:23.000000 product-images-1.0.4/product_images.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-08-01 12:57:23.000000 product-images-1.0.4/product_images.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       15 2023-08-01 12:57:23.000000 product-images-1.0.4/product_images.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       38 2023-08-01 12:57:23.316405 product-images-1.0.4/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      431 2023-08-01 12:56:53.000000 product-images-1.0.4/setup.py
```

### Comparing `product-images-1.0.3/LICENSE` & `product-images-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/fields.py` & `product-images-1.0.4/product_images/fields.py`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/forms.py` & `product-images-1.0.4/product_images/forms.py`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/locale/ru/LC_MESSAGES/django.mo` & `product-images-1.0.4/product_images/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/locale/ru/LC_MESSAGES/django.po` & `product-images-1.0.4/product_images/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/locale/uk/LC_MESSAGES/django.mo` & `product-images-1.0.4/product_images/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/locale/uk/LC_MESSAGES/django.po` & `product-images-1.0.4/product_images/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/migrations/0001_initial.py` & `product-images-1.0.4/product_images/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/models.py` & `product-images-1.0.4/product_images/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 from PIL import Image
-from watermarks.utils import insert_watermark
 
 from os.path import basename
 from urllib.request import urlretrieve
 
 from django.db import models
 from django.urls import reverse
 from django.core.files import File
@@ -89,21 +88,22 @@
             blank=blank,
             null=null,
             max_length=max_length,
             editable=editable,
             *args, **kwargs)
 
 
-def add_product_image_watermark(sender, instance, created, **kwargs):
+def _post_process_image(sender, instance, created, **kwargs):
 
     if not created:
         return
 
     instance.compress()
 
     try:
+        from watermarks.utils import insert_watermark
         insert_watermark('product', instance.file.path)
     except Exception as e:
         pass
 
 
-post_save.connect(add_product_image_watermark, sender=ProductImage)
+post_save.connect(_post_process_image, sender=ProductImage)
```

### Comparing `product-images-1.0.3/product_images/static/dropzone/dropzone.min.css` & `product-images-1.0.4/product_images/static/dropzone/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/static/dropzone/dropzone.min.js` & `product-images-1.0.4/product_images/static/dropzone/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/static/file-manager/file-manager.css` & `product-images-1.0.4/product_images/static/file-manager/file-manager.css`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/static/file-manager/file-manager.js` & `product-images-1.0.4/product_images/static/file-manager/file-manager.js`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/templates/product-images-form.html` & `product-images-1.0.4/product_images/templates/product-images-form.html`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images/views.py` & `product-images-1.0.4/product_images/views.py`

 * *Files identical despite different names*

### Comparing `product-images-1.0.3/product_images.egg-info/SOURCES.txt` & `product-images-1.0.4/product_images.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 LICENSE
 MANIFEST.in
-README.md
-requirements.txt
-setup.cfg
 setup.py
 product_images/__init__.py
 product_images/actions.py
 product_images/fields.py
 product_images/forms.py
 product_images/models.py
 product_images/urls.py
 product_images/utils.py
 product_images/views.py
 product_images/widgets.py
 product_images.egg-info/PKG-INFO
 product_images.egg-info/SOURCES.txt
 product_images.egg-info/dependency_links.txt
-product_images.egg-info/requires.txt
 product_images.egg-info/top_level.txt
 product_images/locale/ru/LC_MESSAGES/django.mo
 product_images/locale/ru/LC_MESSAGES/django.po
 product_images/locale/uk/LC_MESSAGES/django.mo
 product_images/locale/uk/LC_MESSAGES/django.po
 product_images/migrations/0001_initial.py
 product_images/migrations/__init__.py
```

