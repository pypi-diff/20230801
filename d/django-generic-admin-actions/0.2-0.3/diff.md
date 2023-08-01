# Comparing `tmp/django-generic-admin-actions-0.2.tar.gz` & `tmp/django-generic-admin-actions-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-generic-admin-actions-0.2.tar", last modified: Fri Jul 28 20:28:11 2023, max compression
+gzip compressed data, was "django-generic-admin-actions-0.3.tar", last modified: Tue Aug  1 14:29:26 2023, max compression
```

## Comparing `django-generic-admin-actions-0.2.tar` & `django-generic-admin-actions-0.3.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2023-07-27 09:35:02.000000 django-generic-admin-actions-0.2/LICENCE
--rw-r--r--   0 thomas    (1000) thomas    (1000)      136 2023-07-27 11:11:22.000000 django-generic-admin-actions-0.2/MANIFEST.in
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3401 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2091 2023-07-27 19:56:06.000000 django-generic-admin-actions-0.2/README.rst
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3401 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1086 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       12 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       39 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-27 19:30:57.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/zip-safe
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/generic_admin_actions/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.2/generic_admin_actions/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      660 2023-07-28 20:26:55.000000 django-generic-admin-actions-0.2/generic_admin_actions/__version__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1603 2023-07-28 15:49:22.000000 django-generic-admin-actions-0.2/generic_admin_actions/admin.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      172 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.2/generic_admin_actions/apps.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      200 2023-07-27 13:31:59.000000 django-generic-admin-actions-0.2/generic_admin_actions/forms.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/generic_admin_actions/migrations/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.2/generic_admin_actions/migrations/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.484400 django-generic-admin-actions-0.2/generic_admin_actions/templates/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/generic_admin_actions/templates/admin/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      454 2023-07-27 13:33:18.000000 django-generic-admin-actions-0.2/generic_admin_actions/templates/admin/change-list.html
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2192 2023-07-27 19:41:58.000000 django-generic-admin-actions-0.2/setup.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.484400 django-generic-admin-actions-0.2/tests/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      215 2023-07-27 13:35:43.000000 django-generic-admin-actions-0.2/tests/testapp/actions.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      388 2023-07-27 13:40:59.000000 django-generic-admin-actions-0.2/tests/testapp/admin.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      114 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/apps.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/management/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/management/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/management/commands/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/management/commands/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1290 2023-07-27 19:52:51.000000 django-generic-admin-actions-0.2/tests/testapp/management/commands/testapp.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/migrations/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      509 2023-07-27 12:32:31.000000 django-generic-admin-actions-0.2/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 12:32:29.000000 django-generic-admin-actions-0.2/tests/testapp/migrations/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      204 2023-07-27 13:41:08.000000 django-generic-admin-actions-0.2/tests/testapp/models.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3167 2023-07-27 12:43:08.000000 django-generic-admin-actions-0.2/tests/testapp/settings.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/tests/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/tests/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1083 2023-07-27 14:04:55.000000 django-generic-admin-actions-0.2/tests/testapp/tests/test_generic_admin_actions.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      758 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/urls.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      391 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/wsgi.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2023-07-27 09:35:02.000000 django-generic-admin-actions-0.3/LICENCE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      136 2023-07-27 11:11:22.000000 django-generic-admin-actions-0.3/MANIFEST.in
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3874 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2564 2023-08-01 14:18:44.000000 django-generic-admin-actions-0.3/README.rst
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.496989 django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3874 2023-08-01 14:29:26.000000 django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1205 2023-08-01 14:29:26.000000 django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-08-01 14:29:26.000000 django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       12 2023-08-01 14:29:26.000000 django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       39 2023-08-01 14:29:26.000000 django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-27 19:30:57.000000 django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/zip-safe
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/generic_admin_actions/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-08-01 14:01:33.000000 django-generic-admin-actions-0.3/generic_admin_actions/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      660 2023-08-01 13:52:08.000000 django-generic-admin-actions-0.3/generic_admin_actions/__version__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5154 2023-08-01 14:02:33.000000 django-generic-admin-actions-0.3/generic_admin_actions/admin.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      172 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.3/generic_admin_actions/apps.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      187 2023-08-01 13:11:24.000000 django-generic-admin-actions-0.3/generic_admin_actions/forms.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/generic_admin_actions/migrations/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.3/generic_admin_actions/migrations/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.496989 django-generic-admin-actions-0.3/generic_admin_actions/templates/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/generic_admin_actions/templates/admin/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      316 2023-08-01 13:11:24.000000 django-generic-admin-actions-0.3/generic_admin_actions/templates/admin/change_list.html
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      588 2023-08-01 13:11:24.000000 django-generic-admin-actions-0.3/generic_admin_actions/templates/admin/generic_actions.html
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/generic_admin_actions/templatetags/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      639 2023-08-01 13:11:24.000000 django-generic-admin-actions-0.3/generic_admin_actions/templatetags/generic_admin_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2192 2023-07-27 19:41:58.000000 django-generic-admin-actions-0.3/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.496989 django-generic-admin-actions-0.3/tests/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/tests/testapp/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.3/tests/testapp/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      259 2023-08-01 14:25:05.000000 django-generic-admin-actions-0.3/tests/testapp/actions.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      396 2023-08-01 14:03:00.000000 django-generic-admin-actions-0.3/tests/testapp/admin.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      114 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.3/tests/testapp/apps.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/tests/testapp/management/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.3/tests/testapp/management/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/tests/testapp/management/commands/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.3/tests/testapp/management/commands/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1290 2023-07-29 14:39:44.000000 django-generic-admin-actions-0.3/tests/testapp/management/commands/testapp.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/tests/testapp/migrations/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      509 2023-07-27 12:32:31.000000 django-generic-admin-actions-0.3/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 12:32:29.000000 django-generic-admin-actions-0.3/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      204 2023-07-27 13:41:08.000000 django-generic-admin-actions-0.3/tests/testapp/models.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3167 2023-07-30 07:35:25.000000 django-generic-admin-actions-0.3/tests/testapp/settings.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-01 14:29:26.500989 django-generic-admin-actions-0.3/tests/testapp/tests/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.3/tests/testapp/tests/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1544 2023-08-01 13:11:24.000000 django-generic-admin-actions-0.3/tests/testapp/tests/test_generic_admin_actions.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      758 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.3/tests/testapp/urls.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      391 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.3/tests/testapp/wsgi.py
```

### Comparing `django-generic-admin-actions-0.2/LICENCE` & `django-generic-admin-actions-0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.2/PKG-INFO` & `django-generic-admin-actions-0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-generic-admin-actions
-Version: 0.2
+Version: 0.3
 Summary: TODO
 Home-page: https://github.com/thomst/django-generic-admin-actions
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,53 +50,57 @@
 .. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
    :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
    :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
-Django-generic-admin-actions provides an easy way to add an action form to a
-change-list to run generic actions for a specific model independently from the
-item selection.
+Django-generic-admin-actions are admin actions without an item selection. They
+work exactly like original admin actions but without taking a queryset. This is
+useful for actions that are model (and not object) related or that should
+manipulate model objects as a whole.
 
 
 Installation
 ============
 Install from pypi.org::
 
     pip install django-generic-admin-actions
 
-Setup
-=====
 
+Getting started
+===============
 Add generic_admin_actions to your installed apps::
 
     INSTALLED_APPS = [
         'generic_admin_actions',
+        'django.contrib.admin',
         ...
     ]
 
-Use the GenericActionsModelAdmin class and add a generic action::
+Since we overwrite the change_list.html template the app must be listed before
+django's admin-site.
+
+Use the GenericActionsMixin for your ModelAdmin classes and add some actions::
 
-    from generic_admin_actions import GenericActionsModelAdmin
+    from django.contrib import admin
+    from generic_admin_actions import GenericActionsMixin
 
     def my_action(modeladmin, request):
         # Do some stuff here.
 
-    class MyModelAdmin(GenericActionsModelAdmin):
+    class MyModelAdmin(GenericActionsMixin, admin.ModelAdmin):
         ...
         generic_actions = [
             my_action,
             ...
         ]
 
-Setup with an intermediate page
-===============================
-
-TODO
+Generic admin actions working all the same as original admin actions with the
+difference that their don't take a queryset. So for more advanced setups like
+actions with intermediate pages please follow django's official documentation.
 
 
 Usage
 =====
-
 On your model's change-list-view choose the generic action from the dropdown and
 press the "Go" button.
```

### Comparing `django-generic-admin-actions-0.2/README.rst` & `django-generic-admin-actions-0.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -17,53 +17,57 @@
 .. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
    :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
    :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
-Django-generic-admin-actions provides an easy way to add an action form to a
-change-list to run generic actions for a specific model independently from the
-item selection.
+Django-generic-admin-actions are admin actions without an item selection. They
+work exactly like original admin actions but without taking a queryset. This is
+useful for actions that are model (and not object) related or that should
+manipulate model objects as a whole.
 
 
 Installation
 ============
 Install from pypi.org::
 
     pip install django-generic-admin-actions
 
-Setup
-=====
 
+Getting started
+===============
 Add generic_admin_actions to your installed apps::
 
     INSTALLED_APPS = [
         'generic_admin_actions',
+        'django.contrib.admin',
         ...
     ]
 
-Use the GenericActionsModelAdmin class and add a generic action::
+Since we overwrite the change_list.html template the app must be listed before
+django's admin-site.
+
+Use the GenericActionsMixin for your ModelAdmin classes and add some actions::
 
-    from generic_admin_actions import GenericActionsModelAdmin
+    from django.contrib import admin
+    from generic_admin_actions import GenericActionsMixin
 
     def my_action(modeladmin, request):
         # Do some stuff here.
 
-    class MyModelAdmin(GenericActionsModelAdmin):
+    class MyModelAdmin(GenericActionsMixin, admin.ModelAdmin):
         ...
         generic_actions = [
             my_action,
             ...
         ]
 
-Setup with an intermediate page
-===============================
-
-TODO
+Generic admin actions working all the same as original admin actions with the
+difference that their don't take a queryset. So for more advanced setups like
+actions with intermediate pages please follow django's official documentation.
 
 
 Usage
 =====
-
 On your model's change-list-view choose the generic action from the dropdown and
 press the "Go" button.
```

### Comparing `django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/PKG-INFO` & `django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-generic-admin-actions
-Version: 0.2
+Version: 0.3
 Summary: TODO
 Home-page: https://github.com/thomst/django-generic-admin-actions
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,53 +50,57 @@
 .. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
    :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
    :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
 
 
 Description
 ===========
-Django-generic-admin-actions provides an easy way to add an action form to a
-change-list to run generic actions for a specific model independently from the
-item selection.
+Django-generic-admin-actions are admin actions without an item selection. They
+work exactly like original admin actions but without taking a queryset. This is
+useful for actions that are model (and not object) related or that should
+manipulate model objects as a whole.
 
 
 Installation
 ============
 Install from pypi.org::
 
     pip install django-generic-admin-actions
 
-Setup
-=====
 
+Getting started
+===============
 Add generic_admin_actions to your installed apps::
 
     INSTALLED_APPS = [
         'generic_admin_actions',
+        'django.contrib.admin',
         ...
     ]
 
-Use the GenericActionsModelAdmin class and add a generic action::
+Since we overwrite the change_list.html template the app must be listed before
+django's admin-site.
+
+Use the GenericActionsMixin for your ModelAdmin classes and add some actions::
 
-    from generic_admin_actions import GenericActionsModelAdmin
+    from django.contrib import admin
+    from generic_admin_actions import GenericActionsMixin
 
     def my_action(modeladmin, request):
         # Do some stuff here.
 
-    class MyModelAdmin(GenericActionsModelAdmin):
+    class MyModelAdmin(GenericActionsMixin, admin.ModelAdmin):
         ...
         generic_actions = [
             my_action,
             ...
         ]
 
-Setup with an intermediate page
-===============================
-
-TODO
+Generic admin actions working all the same as original admin actions with the
+difference that their don't take a queryset. So for more advanced setups like
+actions with intermediate pages please follow django's official documentation.
 
 
 Usage
 =====
-
 On your model's change-list-view choose the generic action from the dropdown and
 press the "Go" button.
```

### Comparing `django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/SOURCES.txt` & `django-generic-admin-actions-0.3/django_generic_admin_actions.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 django_generic_admin_actions.egg-info/zip-safe
 generic_admin_actions/__init__.py
 generic_admin_actions/__version__.py
 generic_admin_actions/admin.py
 generic_admin_actions/apps.py
 generic_admin_actions/forms.py
 generic_admin_actions/migrations/__init__.py
-generic_admin_actions/templates/admin/change-list.html
+generic_admin_actions/templates/admin/change_list.html
+generic_admin_actions/templates/admin/generic_actions.html
+generic_admin_actions/templatetags/generic_admin_actions.py
 tests/testapp/__init__.py
 tests/testapp/actions.py
 tests/testapp/admin.py
 tests/testapp/apps.py
 tests/testapp/models.py
 tests/testapp/settings.py
 tests/testapp/urls.py
```

### Comparing `django-generic-admin-actions-0.2/generic_admin_actions/__version__.py` & `django-generic-admin-actions-0.3/generic_admin_actions/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 internal code changes that do not affect the API. Development versions are
 incomplete states of a release .
 
 Version 0.x should be considered a development version with an unstable API,
 and backwards compatibility is not guaranteed for minor versions.
 """
 
-__version__ = "0.2"
+__version__ = "0.3"
```

### Comparing `django-generic-admin-actions-0.2/setup.py` & `django-generic-admin-actions-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.2/tests/testapp/management/commands/testapp.py` & `django-generic-admin-actions-0.3/tests/testapp/management/commands/testapp.py`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.2/tests/testapp/settings.py` & `django-generic-admin-actions-0.3/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.2/tests/testapp/tests/test_generic_admin_actions.py` & `django-generic-admin-actions-0.3/tests/testapp/tests/test_generic_admin_actions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from django.test import TestCase
+from django.test import Client
 from django.contrib.auth.models import User
 from django.urls import reverse
 
 from ..admin import ModelOneAdmin
 from ..management.commands.testapp import create_test_data
 
 
@@ -12,20 +13,32 @@
     def setUpTestData(cls):
         create_test_data()
 
     def setUp(self):
         self.admin = User.objects.get(username='admin')
         self.client.force_login(self.admin)
         self.url = reverse('admin:testapp_modelone_changelist')
-        self.action_url = f'{self.url}run_generic_action/'
+        self.post_data = dict(
+            generic_action_index=0,
+            generic_action=None
+        )
 
     def test_form(self):
         resp = self.client.get(self.url)
         self.assertEqual(resp.status_code, 200)
         for action in ModelOneAdmin.generic_actions:
             self.assertIn(action.__name__, resp.content.decode('utf-8'))
 
     def test_actions(self):
-        post_data = dict(generic_action='action_one')
-        resp = self.client.post(self.action_url, post_data, follow=True)
+        post_data = self.post_data.copy()
+        post_data['generic_action'] = 'action_one'
+        resp = self.client.post(self.url, post_data, follow=True)
         self.assertEqual(resp.status_code, 200)
         self.assertIn('Go with action_one!', resp.content.decode('utf-8'))
+
+    def test_action_permission(self):
+        client = Client()
+        client.force_login(User.objects.get(username='anyuser'))
+        resp = client.get(self.url)
+        self.assertEqual(resp.status_code, 200)
+        self.assertNotIn('action_one', resp.content.decode('utf-8'))
+        self.assertIn('action_two', resp.content.decode('utf-8'))
```

### Comparing `django-generic-admin-actions-0.2/tests/testapp/urls.py` & `django-generic-admin-actions-0.3/tests/testapp/urls.py`

 * *Files identical despite different names*

