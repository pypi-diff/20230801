# Comparing `tmp/django-pygwalker-0.0.0.dev1.tar.gz` & `tmp/django-pygwalker-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pygwalker-0.0.0.dev1.tar", last modified: Mon Jul 31 00:04:04 2023, max compression
+gzip compressed data, was "django-pygwalker-0.0.1.tar", last modified: Tue Aug  1 01:42:26 2023, max compression
```

## Comparing `django-pygwalker-0.0.0.dev1.tar` & `django-pygwalker-0.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46857 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46857 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/pygwalker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46845 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46845 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.899128 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.899128 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/pygwalker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/views.py
```

### Comparing `django-pygwalker-0.0.0.dev1/LICENSE` & `django-pygwalker-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.0.dev1/PKG-INFO` & `django-pygwalker-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pygwalker
-Version: 0.0.0.dev1
+Version: 0.0.1
 Author-email: David Slusser <dbslusser@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -703,15 +703,15 @@
 # django-pygwalker
 [![Downloads](https://static.pepy.tech/badge/django-pygwalker)](https://pepy.tech/project/django-pygwalker)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7682/badge)](https://bestpractices.coreinfrastructure.org/projects/7682)
 
 ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-pygwalker)
 ![PyPI - Django](https://img.shields.io/pypi/djversions/django-pygwalker)
 
-Turn your Django querysets into a user interfaces for visual analysis with PyGWalker.
+Turn your Django querysets into user interfaces for visual analysis with PyGWalker.
 
 This utility creates user interfaces based on your Django querysets for visual analysis using PyGwalker. 
 For more information on PyGWalker see the github repo available here: https://github.com/Kanaries/pygwalker 
 
 
 <br/>
 
@@ -770,15 +770,15 @@
     ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates.* 
 
 <br/>
 
 ## Features
 
 ### PygWalkerView
-The PygWalkerView view renders a page containing PyGWalker html. This view takes a queryset parameter and included all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.  
+The PygWalkerView renders a page containing PyGWalker html. This view takes a queryset parameter and includes all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.  
 
 A Bootstrap 5 template is included, but can be overwritten using the template_name parameter. 
 
 #### Parameters
 - **field_list:** list of model fields to include (defaults to fields defined in the model)
 - **queryset:** queryset providing data available to visualization
 - **theme:** PyGWalker theme to use for pyg html (defaults to "media")
```

### Comparing `django-pygwalker-0.0.0.dev1/README.md` & `django-pygwalker-0.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # django-pygwalker
 [![Downloads](https://static.pepy.tech/badge/django-pygwalker)](https://pepy.tech/project/django-pygwalker)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7682/badge)](https://bestpractices.coreinfrastructure.org/projects/7682)
 
 ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-pygwalker)
 ![PyPI - Django](https://img.shields.io/pypi/djversions/django-pygwalker)
 
-Turn your Django querysets into a user interfaces for visual analysis with PyGWalker.
+Turn your Django querysets into user interfaces for visual analysis with PyGWalker.
 
 This utility creates user interfaces based on your Django querysets for visual analysis using PyGwalker. 
 For more information on PyGWalker see the github repo available here: https://github.com/Kanaries/pygwalker 
 
 
 <br/>
 
@@ -68,15 +68,15 @@
     ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates.* 
 
 <br/>
 
 ## Features
 
 ### PygWalkerView
-The PygWalkerView view renders a page containing PyGWalker html. This view takes a queryset parameter and included all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.  
+The PygWalkerView renders a page containing PyGWalker html. This view takes a queryset parameter and includes all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.  
 
 A Bootstrap 5 template is included, but can be overwritten using the template_name parameter. 
 
 #### Parameters
 - **field_list:** list of model fields to include (defaults to fields defined in the model)
 - **queryset:** queryset providing data available to visualization
 - **theme:** PyGWalker theme to use for pyg html (defaults to "media")
```

### Comparing `django-pygwalker-0.0.0.dev1/pyproject.toml` & `django-pygwalker-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/PKG-INFO` & `django-pygwalker-0.0.1/src/django_pygwalker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pygwalker
-Version: 0.0.0.dev1
+Version: 0.0.1
 Author-email: David Slusser <dbslusser@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -703,15 +703,15 @@
 # django-pygwalker
 [![Downloads](https://static.pepy.tech/badge/django-pygwalker)](https://pepy.tech/project/django-pygwalker)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7682/badge)](https://bestpractices.coreinfrastructure.org/projects/7682)
 
 ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-pygwalker)
 ![PyPI - Django](https://img.shields.io/pypi/djversions/django-pygwalker)
 
-Turn your Django querysets into a user interfaces for visual analysis with PyGWalker.
+Turn your Django querysets into user interfaces for visual analysis with PyGWalker.
 
 This utility creates user interfaces based on your Django querysets for visual analysis using PyGwalker. 
 For more information on PyGWalker see the github repo available here: https://github.com/Kanaries/pygwalker 
 
 
 <br/>
 
@@ -770,15 +770,15 @@
     ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates.* 
 
 <br/>
 
 ## Features
 
 ### PygWalkerView
-The PygWalkerView view renders a page containing PyGWalker html. This view takes a queryset parameter and included all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.  
+The PygWalkerView renders a page containing PyGWalker html. This view takes a queryset parameter and includes all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.  
 
 A Bootstrap 5 template is included, but can be overwritten using the template_name parameter. 
 
 #### Parameters
 - **field_list:** list of model fields to include (defaults to fields defined in the model)
 - **queryset:** queryset providing data available to visualization
 - **theme:** PyGWalker theme to use for pyg html (defaults to "media")
```

### Comparing `django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html` & `django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/views.py` & `django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/views.py`

 * *Files identical despite different names*

