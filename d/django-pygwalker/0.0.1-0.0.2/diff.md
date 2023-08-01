# Comparing `tmp/django-pygwalker-0.0.1.tar.gz` & `tmp/django-pygwalker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pygwalker-0.0.1.tar", last modified: Tue Aug  1 01:42:26 2023, max compression
+gzip compressed data, was "django-pygwalker-0.0.2.tar", last modified: Tue Aug  1 02:14:12 2023, max compression
```

## Comparing `django-pygwalker-0.0.1.tar` & `django-pygwalker-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46845 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46845 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 01:42:26.000000 django-pygwalker-0.0.1/src/django_pygwalker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.899128 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.899128 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/pygwalker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:42:26.903128 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-01 01:42:08.000000 django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46845 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.706181 django-pygwalker-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46845 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.706181 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.706181 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/pygwalker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/views.py
```

### Comparing `django-pygwalker-0.0.1/LICENSE` & `django-pygwalker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.1/PKG-INFO` & `django-pygwalker-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pygwalker
-Version: 0.0.1
+Version: 0.0.2
 Author-email: David Slusser <dbslusser@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `django-pygwalker-0.0.1/README.md` & `django-pygwalker-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.1/pyproject.toml` & `django-pygwalker-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.1/src/django_pygwalker.egg-info/PKG-INFO` & `django-pygwalker-0.0.2/src/django_pygwalker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pygwalker
-Version: 0.0.1
+Version: 0.0.2
 Author-email: David Slusser <dbslusser@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html` & `django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.1/src/djangoaddicts/pygwalker/views.py` & `django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,17 +21,48 @@
         from djangoaddicts.pygwalker.views import PygWalkerView
         class MyPygView(PygWalkerView):
             queryset = Order.objects.all()
             title = "Order Data Analysis"
             theme = "light"
             field_list = ["status__name", "customer", "order_id", "created_at", "updated_at", "products"]
     """
+
     field_list: list = []
     queryset: QuerySet = None
     template_name: str = "pygwalker/bs5/pygwalker.html"
     theme: str = "media"
     title: str = "Data Analysis"
 
     def get(self, request):
         pd_data = pd.DataFrame(list(self.queryset.values(*self.field_list)))
         context = {"pyg": pyg.walk(pd_data, return_html=True, dark=self.theme), "title": self.title}
         return render(request, self.template_name, context)
+
+
+class StaticCsvPygWalkerView(View):
+    """View to create a PyGWalker visualization interface from a statically definied csv file.
+    See https://github.com/Kanaries/pygwalker for more information on PyGWalker.
+
+    class parameters:
+        csv_file      - csv file containing data to visualize
+        theme         - PyGWalker theme to use for pyg html (defaults to "media")
+        title         - title used on html render
+        template_name - template used when rendering page; defaults to: pygwalker/bs5/pyg.html
+
+    example:
+
+        from djangoaddicts.pygwalker.views import StaticCsvPygWalkerView
+        class MyPygView(StaticCsvPygWalkerView):
+            csv_file = "my_csv_file.csv
+            title = "Order Data Analysis"
+            theme = "light"
+    """
+
+    csv_file: str | None = None
+    template_name: str = "pygwalker/bs5/pygwalker.html"
+    theme: str = "media"
+    title: str = "Data Analysis"
+
+    def get(self, request):
+        pd_data = pd.read_csv(self.csv_file)
+        context = {"pyg": pyg.walk(pd_data, return_html=True, dark=self.theme), "title": self.title}
+        return render(request, self.template_name, context)
```

