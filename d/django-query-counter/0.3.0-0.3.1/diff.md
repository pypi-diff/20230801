# Comparing `tmp/django-query-counter-0.3.0.tar.gz` & `tmp/django-query-counter-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-query-counter-0.3.0.tar", last modified: Thu Jun 29 19:14:07 2023, max compression
+gzip compressed data, was "django-query-counter-0.3.1.tar", last modified: Tue Aug  1 13:47:27 2023, max compression
```

## Comparing `django-query-counter-0.3.0.tar` & `django-query-counter-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 oleh       (501) staff       (20)        0 2023-06-29 19:14:07.741719 django-query-counter-0.3.0/
--rw-r--r--   0 oleh       (501) staff       (20)      110 2023-06-28 12:41:24.000000 django-query-counter-0.3.0/AUTHORS.md
--rw-r--r--   0 oleh       (501) staff       (20)     1069 2023-02-27 12:40:15.000000 django-query-counter-0.3.0/LICENSE
--rw-r--r--   0 oleh       (501) staff       (20)     3956 2023-06-29 19:14:07.741082 django-query-counter-0.3.0/PKG-INFO
--rw-r--r--   0 oleh       (501) staff       (20)     3219 2023-06-28 12:53:20.000000 django-query-counter-0.3.0/README.md
-drwxr-xr-x   0 oleh       (501) staff       (20)        0 2023-06-29 19:14:07.730721 django-query-counter-0.3.0/django_query_counter.egg-info/
--rw-r--r--   0 oleh       (501) staff       (20)     3956 2023-06-29 19:14:07.000000 django-query-counter-0.3.0/django_query_counter.egg-info/PKG-INFO
--rw-r--r--   0 oleh       (501) staff       (20)      420 2023-06-29 19:14:07.000000 django-query-counter-0.3.0/django_query_counter.egg-info/SOURCES.txt
--rw-r--r--   0 oleh       (501) staff       (20)        1 2023-06-29 19:14:07.000000 django-query-counter-0.3.0/django_query_counter.egg-info/dependency_links.txt
--rw-r--r--   0 oleh       (501) staff       (20)        9 2023-06-29 19:14:07.000000 django-query-counter-0.3.0/django_query_counter.egg-info/requires.txt
--rw-r--r--   0 oleh       (501) staff       (20)       14 2023-06-29 19:14:07.000000 django-query-counter-0.3.0/django_query_counter.egg-info/top_level.txt
--rw-r--r--   0 oleh       (501) staff       (20)     1086 2023-06-29 18:09:26.000000 django-query-counter-0.3.0/pyproject.toml
-drwxr-xr-x   0 oleh       (501) staff       (20)        0 2023-06-29 19:14:07.735679 django-query-counter-0.3.0/query_counter/
--rw-r--r--   0 oleh       (501) staff       (20)      181 2023-06-29 17:33:20.000000 django-query-counter-0.3.0/query_counter/__init__.py
--rw-r--r--   0 oleh       (501) staff       (20)      372 2023-02-27 12:40:15.000000 django-query-counter-0.3.0/query_counter/apps.py
--rw-r--r--   0 oleh       (501) staff       (20)     6238 2023-06-27 19:24:23.000000 django-query-counter-0.3.0/query_counter/decorators.py
--rw-r--r--   0 oleh       (501) staff       (20)      255 2023-05-25 14:17:44.000000 django-query-counter-0.3.0/query_counter/middleware.py
--rw-r--r--   0 oleh       (501) staff       (20)      364 2023-02-27 12:40:15.000000 django-query-counter-0.3.0/query_counter/settings.py
--rw-r--r--   0 oleh       (501) staff       (20)       38 2023-06-29 19:14:07.741962 django-query-counter-0.3.0/setup.cfg
--rw-r--r--   0 oleh       (501) staff       (20)     1048 2023-06-28 13:33:44.000000 django-query-counter-0.3.0/setup.py
-drwxr-xr-x   0 oleh       (501) staff       (20)        0 2023-06-29 19:14:07.738309 django-query-counter-0.3.0/tests/
--rw-r--r--   0 oleh       (501) staff       (20)      660 2023-06-29 19:12:27.000000 django-query-counter-0.3.0/tests/test_main.py
+drwxr-xr-x   0 oleh       (501) staff       (20)        0 2023-08-01 13:47:27.744554 django-query-counter-0.3.1/
+-rw-r--r--   0 oleh       (501) staff       (20)      110 2023-06-29 19:49:27.000000 django-query-counter-0.3.1/AUTHORS.md
+-rw-r--r--   0 oleh       (501) staff       (20)     1069 2023-02-27 12:40:15.000000 django-query-counter-0.3.1/LICENSE
+-rw-r--r--   0 oleh       (501) staff       (20)     3963 2023-08-01 13:47:27.744114 django-query-counter-0.3.1/PKG-INFO
+-rw-r--r--   0 oleh       (501) staff       (20)     3226 2023-08-01 13:47:03.000000 django-query-counter-0.3.1/README.md
+drwxr-xr-x   0 oleh       (501) staff       (20)        0 2023-08-01 13:47:27.739618 django-query-counter-0.3.1/django_query_counter.egg-info/
+-rw-r--r--   0 oleh       (501) staff       (20)     3963 2023-08-01 13:47:27.000000 django-query-counter-0.3.1/django_query_counter.egg-info/PKG-INFO
+-rw-r--r--   0 oleh       (501) staff       (20)      420 2023-08-01 13:47:27.000000 django-query-counter-0.3.1/django_query_counter.egg-info/SOURCES.txt
+-rw-r--r--   0 oleh       (501) staff       (20)        1 2023-08-01 13:47:27.000000 django-query-counter-0.3.1/django_query_counter.egg-info/dependency_links.txt
+-rw-r--r--   0 oleh       (501) staff       (20)        9 2023-08-01 13:47:27.000000 django-query-counter-0.3.1/django_query_counter.egg-info/requires.txt
+-rw-r--r--   0 oleh       (501) staff       (20)       14 2023-08-01 13:47:27.000000 django-query-counter-0.3.1/django_query_counter.egg-info/top_level.txt
+-rw-r--r--   0 oleh       (501) staff       (20)     1086 2023-06-29 19:49:27.000000 django-query-counter-0.3.1/pyproject.toml
+drwxr-xr-x   0 oleh       (501) staff       (20)        0 2023-08-01 13:47:27.742554 django-query-counter-0.3.1/query_counter/
+-rw-r--r--   0 oleh       (501) staff       (20)      181 2023-08-01 13:47:03.000000 django-query-counter-0.3.1/query_counter/__init__.py
+-rw-r--r--   0 oleh       (501) staff       (20)      372 2023-02-27 12:40:15.000000 django-query-counter-0.3.1/query_counter/apps.py
+-rw-r--r--   0 oleh       (501) staff       (20)     6238 2023-06-29 19:49:27.000000 django-query-counter-0.3.1/query_counter/decorators.py
+-rw-r--r--   0 oleh       (501) staff       (20)      255 2023-05-25 14:17:44.000000 django-query-counter-0.3.1/query_counter/middleware.py
+-rw-r--r--   0 oleh       (501) staff       (20)      364 2023-02-27 12:40:15.000000 django-query-counter-0.3.1/query_counter/settings.py
+-rw-r--r--   0 oleh       (501) staff       (20)       38 2023-08-01 13:47:27.744711 django-query-counter-0.3.1/setup.cfg
+-rw-r--r--   0 oleh       (501) staff       (20)     1048 2023-06-29 19:49:27.000000 django-query-counter-0.3.1/setup.py
+drwxr-xr-x   0 oleh       (501) staff       (20)        0 2023-08-01 13:47:27.743404 django-query-counter-0.3.1/tests/
+-rw-r--r--   0 oleh       (501) staff       (20)      660 2023-06-29 19:49:27.000000 django-query-counter-0.3.1/tests/test_main.py
```

### Comparing `django-query-counter-0.3.0/LICENSE` & `django-query-counter-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-query-counter-0.3.0/PKG-INFO` & `django-query-counter-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-query-counter
-Version: 0.3.0
+Version: 0.3.1
 Summary: Debug tool to print sql queries count to the console
 Home-page: https://github.com/conformist-mw/django-query-counter
 Author: Oleg Smedyuk
 Author-email: oleg.smedyuk@gmail.com
 License: MIT
 Keywords: django sql query count management commands
 Classifier: Development Status :: 4 - Beta
@@ -126,14 +126,15 @@
     'DQC_PYGMENTS_STYLE': 'tango',
     'DQC_PRINT_ALL_QUERIES': False,
     'DQC_COUNT_QTY_MAP': {
         5: 'green',
         10: 'white',
         20: 'yellow',
         30: 'red',
+    },
 }
 ```
 
 Feel free to override any of them.
 
 Tabulate tables formats you can find [here](https://github.com/astanin/python-tabulate#table-format).
 Pygments styles available [here](https://pygments.org/demo/).
```

### Comparing `django-query-counter-0.3.0/README.md` & `django-query-counter-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     'DQC_PYGMENTS_STYLE': 'tango',
     'DQC_PRINT_ALL_QUERIES': False,
     'DQC_COUNT_QTY_MAP': {
         5: 'green',
         10: 'white',
         20: 'yellow',
         30: 'red',
+    },
 }
 ```
 
 Feel free to override any of them.
 
 Tabulate tables formats you can find [here](https://github.com/astanin/python-tabulate#table-format).
 Pygments styles available [here](https://pygments.org/demo/).
```

### Comparing `django-query-counter-0.3.0/django_query_counter.egg-info/PKG-INFO` & `django-query-counter-0.3.1/django_query_counter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-query-counter
-Version: 0.3.0
+Version: 0.3.1
 Summary: Debug tool to print sql queries count to the console
 Home-page: https://github.com/conformist-mw/django-query-counter
 Author: Oleg Smedyuk
 Author-email: oleg.smedyuk@gmail.com
 License: MIT
 Keywords: django sql query count management commands
 Classifier: Development Status :: 4 - Beta
@@ -126,14 +126,15 @@
     'DQC_PYGMENTS_STYLE': 'tango',
     'DQC_PRINT_ALL_QUERIES': False,
     'DQC_COUNT_QTY_MAP': {
         5: 'green',
         10: 'white',
         20: 'yellow',
         30: 'red',
+    },
 }
 ```
 
 Feel free to override any of them.
 
 Tabulate tables formats you can find [here](https://github.com/astanin/python-tabulate#table-format).
 Pygments styles available [here](https://pygments.org/demo/).
```

### Comparing `django-query-counter-0.3.0/pyproject.toml` & `django-query-counter-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-query-counter-0.3.0/query_counter/decorators.py` & `django-query-counter-0.3.1/query_counter/decorators.py`

 * *Files identical despite different names*

### Comparing `django-query-counter-0.3.0/setup.py` & `django-query-counter-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-query-counter-0.3.0/tests/test_main.py` & `django-query-counter-0.3.1/tests/test_main.py`

 * *Files identical despite different names*

