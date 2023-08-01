# Comparing `tmp/django-form-action-1.0.4.tar.gz` & `tmp/django-form-action-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-form-action-1.0.4.tar", last modified: Sat Jul 29 20:17:55 2023, max compression
+gzip compressed data, was "django-form-action-1.0.5.tar", last modified: Tue Aug  1 18:22:54 2023, max compression
```

## Comparing `django-form-action-1.0.4.tar` & `django-form-action-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:17:55.448672 django-form-action-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 20:17:45.000000 django-form-action-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-29 20:17:55.448672 django-form-action-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-29 20:17:45.000000 django-form-action-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:17:55.448672 django-form-action-1.0.4/django_form_action.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 20:17:55.000000 django-form-action-1.0.4/django_form_action.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:17:55.448672 django-form-action-1.0.4/form_action/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-29 20:17:45.000000 django-form-action-1.0.4/form_action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-29 20:17:45.000000 django-form-action-1.0.4/form_action/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-29 20:17:45.000000 django-form-action-1.0.4/form_action/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 20:17:45.000000 django-form-action-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:17:55.448672 django-form-action-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-29 20:17:45.000000 django-form-action-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:22:54.389175 django-form-action-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 18:22:44.000000 django-form-action-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 18:22:54.389175 django-form-action-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-01 18:22:44.000000 django-form-action-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:22:54.389175 django-form-action-1.0.5/django_form_action.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 18:22:54.000000 django-form-action-1.0.5/django_form_action.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 18:22:54.000000 django-form-action-1.0.5/django_form_action.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:22:54.000000 django-form-action-1.0.5/django_form_action.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 18:22:54.000000 django-form-action-1.0.5/django_form_action.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 18:22:54.000000 django-form-action-1.0.5/django_form_action.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:22:54.389175 django-form-action-1.0.5/form_action/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 18:22:44.000000 django-form-action-1.0.5/form_action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-08-01 18:22:44.000000 django-form-action-1.0.5/form_action/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-01 18:22:44.000000 django-form-action-1.0.5/form_action/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 18:22:44.000000 django-form-action-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:22:54.389175 django-form-action-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-01 18:22:44.000000 django-form-action-1.0.5/setup.py
```

### Comparing `django-form-action-1.0.4/LICENSE` & `django-form-action-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-form-action-1.0.4/PKG-INFO` & `django-form-action-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-action
-Version: 1.0.4
+Version: 1.0.5
 Summary: Django action to add an intermediate page to parse form data
 Home-page: https://github.com/sandbox-pokhara/django-form-action
 Author: Pradish Bijukchhe
 Author-email: pradishbijukchhe@gmail.com
 Project-URL: Bug Tracker, https://github.com/sandbox-pokhara/django-form-action/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-form-action-1.0.4/README.md` & `django-form-action-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django-form-action-1.0.4/django_form_action.egg-info/PKG-INFO` & `django-form-action-1.0.5/django_form_action.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-action
-Version: 1.0.4
+Version: 1.0.5
 Summary: Django action to add an intermediate page to parse form data
 Home-page: https://github.com/sandbox-pokhara/django-form-action
 Author: Pradish Bijukchhe
 Author-email: pradishbijukchhe@gmail.com
 Project-URL: Bug Tracker, https://github.com/sandbox-pokhara/django-form-action/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-form-action-1.0.4/form_action/decorators.py` & `django-form-action-1.0.5/form_action/decorators.py`

 * *Files identical despite different names*

### Comparing `django-form-action-1.0.4/form_action/mixins.py` & `django-form-action-1.0.5/form_action/mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from urllib.parse import urljoin
+
 from django.template import engines
 from django.urls import path
 
 template = engines["django"].from_string("""
 {% extends "admin/change_list.html" %}
-{% load add_preserved_filters from admin_urls %}
 {% block object-tools-items %}
   {% for button in extra_buttons %}
     <li>
-      <a href="{% add_preserved_filters action_url %}actions/{{ button.name }}/">
+      <a href="{{ button.url }}">
         {{ button.title }}
       </a>
     </li>
   {% endfor %}
   {{ block.super }}
 {% endblock %}
 """)
@@ -19,15 +20,22 @@
 
 class ExtraButtonMixin:
     change_list_template = template
 
     def changelist_view(self, request, extra_context=None):
         extra_context = extra_context or {}
         extra_buttons = getattr(self, "extra_buttons", [])
-        extra_buttons = [{"name": b.name, "title": b.title} for b in extra_buttons]
+        extra_buttons = [
+            {
+                "name": b.name,
+                "title": b.title,
+                "url": urljoin(request.path, f"actions/{b.name}/"),
+            }
+            for b in extra_buttons
+        ]
         extra_context.update({"extra_buttons": extra_buttons})
         return super().changelist_view(request, extra_context)
 
     def get_urls(self):
         urls = super().get_urls()
         return self.get_extra_urls() + urls
```

### Comparing `django-form-action-1.0.4/setup.py` & `django-form-action-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-form-action",
-    version="1.0.4",
+    version="1.0.5",
     author="Pradish Bijukchhe",
     author_email="pradishbijukchhe@gmail.com",
     description="Django action to add an intermediate page to parse form data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sandbox-pokhara/django-form-action",
     project_urls={
```

