# Comparing `tmp/django-webstack-1.5.3.tar.gz` & `tmp/django-webstack-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webstack-1.5.3.tar", last modified: Sat Jul 29 08:46:18 2023, max compression
+gzip compressed data, was "django-webstack-1.5.4.tar", last modified: Tue Aug  1 05:27:27 2023, max compression
```

## Comparing `django-webstack-1.5.3.tar` & `django-webstack-1.5.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.833848 django-webstack-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-29 08:46:05.000000 django-webstack-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-29 08:46:05.000000 django-webstack-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-29 08:46:18.833848 django-webstack-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-29 08:46:05.000000 django-webstack-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.825848 django-webstack-1.5.3/django_webstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-29 08:46:18.000000 django-webstack-1.5.3/django_webstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-29 08:46:18.000000 django-webstack-1.5.3/django_webstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:46:18.000000 django-webstack-1.5.3/django_webstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 08:46:18.000000 django-webstack-1.5.3/django_webstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 08:46:18.000000 django-webstack-1.5.3/django_webstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:46:18.833848 django-webstack-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-29 08:46:16.000000 django-webstack-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.829848 django-webstack-1.5.3/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.829848 django-webstack-1.5.3/webstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/migrations/0002_auto_20230724_1835.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/migrations/0003_auto_20230725_1401.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.825848 django-webstack-1.5.3/webstack/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.825848 django-webstack-1.5.3/webstack/static/webstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.825848 django-webstack-1.5.3/webstack/static/webstack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.829848 django-webstack-1.5.3/webstack/static/webstack/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/css/nav.css
--rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon-components.css
--rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon-core.css
--rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon-forms.css
--rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon-skins.css
--rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.829848 django-webstack-1.5.3/webstack/static/webstack/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/images/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/images/logo-collapsed@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/images/logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/images/preview.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.833848 django-webstack-1.5.3/webstack/static/webstack/assets/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/js/TweenMax.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/js/joinable.js
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/js/lozad.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/js/resizeable.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/js/xenon-api.js
--rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/js/xenon-custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/static/webstack/assets/js/xenon-toggles.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.825848 django-webstack-1.5.3/webstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:46:18.833848 django-webstack-1.5.3/webstack/templates/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/templates/webstack/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/templates/webstack/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 08:46:05.000000 django-webstack-1.5.3/webstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.583584 django-webstack-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 05:27:18.000000 django-webstack-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-01 05:27:18.000000 django-webstack-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-01 05:27:27.583584 django-webstack-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-08-01 05:27:18.000000 django-webstack-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.575584 django-webstack-1.5.4/django_webstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-01 05:27:27.000000 django-webstack-1.5.4/django_webstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-01 05:27:27.000000 django-webstack-1.5.4/django_webstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:27:27.000000 django-webstack-1.5.4/django_webstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 05:27:27.000000 django-webstack-1.5.4/django_webstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 05:27:27.000000 django-webstack-1.5.4/django_webstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 05:27:27.583584 django-webstack-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-01 05:27:26.000000 django-webstack-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.575584 django-webstack-1.5.4/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.575584 django-webstack-1.5.4/webstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/migrations/0002_auto_20230724_1835.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/migrations/0003_auto_20230725_1401.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.575584 django-webstack-1.5.4/webstack/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.575584 django-webstack-1.5.4/webstack/static/webstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.575584 django-webstack-1.5.4/webstack/static/webstack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.579584 django-webstack-1.5.4/webstack/static/webstack/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/css/nav.css
+-rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon-components.css
+-rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon-forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon-skins.css
+-rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.579584 django-webstack-1.5.4/webstack/static/webstack/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/images/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/images/logo-collapsed@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/images/logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/images/preview.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.583584 django-webstack-1.5.4/webstack/static/webstack/assets/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/js/TweenMax.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/js/joinable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/js/lozad.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/js/resizeable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/js/xenon-api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/js/xenon-custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/static/webstack/assets/js/xenon-toggles.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.575584 django-webstack-1.5.4/webstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:27:27.583584 django-webstack-1.5.4/webstack/templates/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/templates/webstack/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/templates/webstack/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-01 05:27:18.000000 django-webstack-1.5.4/webstack/views.py
```

### Comparing `django-webstack-1.5.3/LICENSE` & `django-webstack-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/PKG-INFO` & `django-webstack-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.5.3
+Version: 1.5.4
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-webstack Version: 1.5.3 Summary: webstack of
+Metadata-Version: 2.1 Name: django-webstack Version: 1.5.4 Summary: webstack of
 Django Home-page: https://github.com/Hopetree/django-webstack Author: Hopetree
 Author-email: zlwork2014@163.com Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-webstack-1.5.3/README.md` & `django-webstack-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/django_webstack.egg-info/PKG-INFO` & `django-webstack-1.5.4/django_webstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.5.3
+Version: 1.5.4
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-webstack Version: 1.5.3 Summary: webstack of
+Metadata-Version: 2.1 Name: django-webstack Version: 1.5.4 Summary: webstack of
 Django Home-page: https://github.com/Hopetree/django-webstack Author: Hopetree
 Author-email: zlwork2014@163.com Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-webstack-1.5.3/django_webstack.egg-info/SOURCES.txt` & `django-webstack-1.5.4/django_webstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/setup.py` & `django-webstack-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 # Author: https://github.com/Hopetree
 # Date: 2023/7/24
 from setuptools import find_packages, setup
 
 # 这里的版本号根据tag去动态设置
-VERSION = '1.5.3'
+VERSION = '1.5.4'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='django-webstack',
     version=VERSION,
```

### Comparing `django-webstack-1.5.3/webstack/admin.py` & `django-webstack-1.5.4/webstack/admin.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/migrations/0001_initial.py` & `django-webstack-1.5.4/webstack/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/migrations/0002_auto_20230724_1835.py` & `django-webstack-1.5.4/webstack/migrations/0002_auto_20230724_1835.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/migrations/0003_auto_20230725_1401.py` & `django-webstack-1.5.4/webstack/migrations/0003_auto_20230725_1401.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/models.py` & `django-webstack-1.5.4/webstack/models.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/css/nav.css` & `django-webstack-1.5.4/webstack/static/webstack/assets/css/nav.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon-components.css` & `django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon-components.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon-core.css` & `django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon-core.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon-forms.css` & `django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon-forms.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon-skins.css` & `django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon-skins.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/css/xenon.css` & `django-webstack-1.5.4/webstack/static/webstack/assets/css/xenon.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/images/favicon.png` & `django-webstack-1.5.4/webstack/static/webstack/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/images/logo-collapsed@2x.png` & `django-webstack-1.5.4/webstack/static/webstack/assets/images/logo-collapsed@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/images/logo@2x.png` & `django-webstack-1.5.4/webstack/static/webstack/assets/images/logo@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/images/preview.gif` & `django-webstack-1.5.4/webstack/static/webstack/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/js/TweenMax.min.js` & `django-webstack-1.5.4/webstack/static/webstack/assets/js/TweenMax.min.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/js/joinable.js` & `django-webstack-1.5.4/webstack/static/webstack/assets/js/joinable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/js/lozad.js` & `django-webstack-1.5.4/webstack/static/webstack/assets/js/lozad.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/js/resizeable.js` & `django-webstack-1.5.4/webstack/static/webstack/assets/js/resizeable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/js/xenon-api.js` & `django-webstack-1.5.4/webstack/static/webstack/assets/js/xenon-api.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/js/xenon-custom.js` & `django-webstack-1.5.4/webstack/static/webstack/assets/js/xenon-custom.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/static/webstack/assets/js/xenon-toggles.js` & `django-webstack-1.5.4/webstack/static/webstack/assets/js/xenon-toggles.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.5.3/webstack/templates/webstack/base.html` & `django-webstack-1.5.4/webstack/templates/webstack/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 <head>
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
     <title>{% block title %}{% endblock %}</title>
     {% block meta %}{% endblock %}
-    <link href="https://cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
-    <link href="https://cdn.bootcss.com/twitter-bootstrap/3.0.2/css/bootstrap.min.css" rel="stylesheet">
+    <link rel="stylesheet" href="https://cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.min.css">
+    <link rel="stylesheet" href="https://cdn.bootcss.com/twitter-bootstrap/3.0.2/css/bootstrap.min.css">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-core.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-components.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-skins.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/nav.css' %}">
     <script src="https://cdn.bootcss.com/jquery/1.11.1/jquery.min.js"></script>
     <style>
         .sidebar-menu {
@@ -134,15 +134,15 @@
                 {% if second_menu.get_site_list %}
                     <h4 class="text-gray" id="{{ second_menu.name }}">
                         <i class="{{ second_menu.icon }}" style="margin-right: 7px;"></i>
                         {{ second_menu.name }}
                     </h4>
                     <div class="row">
                         {% for web in second_menu.get_site_list %}
-                            <div class="col-sm-2">
+                            <div class="col-xs-6 col-sm-4 col-md-3 col-lg-2">
                                 <div class="xe-widget xe-conversations box2 label-info"
                                      onclick="window.open('{{ web.link }}', '_blank')" data-toggle="tooltip"
                                      data-placement="bottom" title="" data-original-title="{{ web.description }}">
                                     <div class="xe-comment-entry">
                                         <a class="xe-user-img">
                                             <img data-src="{{ web.logo.url }}"
                                                  class="lozad img-circle"
```

### Comparing `django-webstack-1.5.3/webstack/templates/webstack/index.html` & `django-webstack-1.5.4/webstack/templates/webstack/index.html`

 * *Files identical despite different names*

