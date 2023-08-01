# Comparing `tmp/pretix-sumup-1.0.5.tar.gz` & `tmp/pretix-sumup-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sumup-1.0.5.tar", last modified: Mon Jul 31 13:26:43 2023, max compression
+gzip compressed data, was "pretix-sumup-1.0.6.tar", last modified: Tue Aug  1 13:34:29 2023, max compression
```

## Comparing `pretix-sumup-1.0.5.tar` & `pretix-sumup-1.0.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.196086 pretix-sumup-1.0.5/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.196086 pretix-sumup-1.0.5/pretix_sumup/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/locale/de_Informal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.196086 pretix-sumup-1.0.5/pretix_sumup/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.196086 pretix-sumup-1.0.5/pretix_sumup/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.196086 pretix-sumup-1.0.5/pretix_sumup/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.196086 pretix-sumup-1.0.5/pretix_sumup/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/static/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/static/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.196086 pretix-sumup-1.0.5/pretix_sumup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/control.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/email/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/not_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/pending.html
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/prepare.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/pretix_sumup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-31 13:26:43.000000 pretix-sumup-1.0.5/pretix_sumup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 13:26:43.000000 pretix-sumup-1.0.5/pretix_sumup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:26:43.000000 pretix-sumup-1.0.5/pretix_sumup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 13:26:43.000000 pretix-sumup-1.0.5/pretix_sumup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 13:26:43.000000 pretix-sumup-1.0.5/pretix_sumup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:26:43.200085 pretix-sumup-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 13:25:21.000000 pretix-sumup-1.0.5/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-08-01 13:34:29.427721 pretix-sumup-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/static/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/static/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/control.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/email/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/not_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/pending.html
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/prepare.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-01 13:34:29.427721 pretix-sumup-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/tests/test_main.py
```

### Comparing `pretix-sumup-1.0.5/LICENSE` & `pretix-sumup-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/PKG-INFO` & `pretix-sumup-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.5
+Version: 1.0.6
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.5/README.md` & `pretix-sumup-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/apps.py` & `pretix-sumup-1.0.6/pretix_sumup/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/locale/de/LC_MESSAGES/django.po` & `pretix-sumup-1.0.6/pretix_sumup/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/locale/django.pot` & `pretix-sumup-1.0.6/pretix_sumup/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/locale/es/LC_MESSAGES/django.po` & `pretix-sumup-1.0.6/pretix_sumup/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/locale/fr/LC_MESSAGES/django.po` & `pretix-sumup-1.0.6/pretix_sumup/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/locale/it/LC_MESSAGES/django.po` & `pretix-sumup-1.0.6/pretix_sumup/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/payment.py` & `pretix-sumup-1.0.6/pretix_sumup/payment.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import requests
 import sys
 import uuid
 from collections import OrderedDict
 from django import forms
 from django.http import HttpRequest
 from django.template.loader import get_template
+from django.urls import resolve
 from django.utils.crypto import get_random_string
 from django.utils.translation import get_language, gettext_lazy as _, to_locale
 from i18nfield.strings import LazyI18nString
 from pretix.base.models import InvoiceAddress, Order, OrderPayment
 from pretix.base.payment import BasePaymentProvider
 from pretix.presale.views.cart import cart_session
 
@@ -144,34 +145,33 @@
                     request._checkout_flow_invoice_address = InvoiceAddress()
                 else:
                     try:
                         request._checkout_flow_invoice_address = InvoiceAddress.objects.get(pk=iapk, order__isnull=True)
                     except InvoiceAddress.DoesNotExist:
                         request._checkout_flow_invoice_address = InvoiceAddress()
             return request._checkout_flow_invoice_address
-        
+
         print("SumupPayment.payment_form_render", file=sys.stderr)
         self.ia = get_invoice_address()
         ctx = {}
         template = get_template("pretix_sumup/prepare.html")
         return template.render(ctx)
 
-    def checkout_prepare(self, request, cart):
+    def sumup_prepare(self, request, email, total):
         print("SumupPayment.checkout_prepare", file=sys.stderr)
         client_id = self.settings.get("client_id")
         secret = self.settings.get("secret")
         sumupid = self.settings.get("sumupid")
         sumupToken = self.sumup_get_token(client_id, secret)
-        cs = cart_session(request)
         if isinstance(sumupToken, str):
             sumupCheckoutResponse = self.sumup_create_checkout(
                 sumupToken,
                 sumupid,
-                str(cart["total"]),
-                cs["email"],
+                str(total),
+                email,
                 self.ia.name_parts["given_name"] if "given_name" in self.ia.name_parts else "John",
                 self.ia.name_parts["family_name"] if "family_name" in self.ia.name_parts else "Doe",
             )
             if sumupCheckoutResponse.status_code == 201:
                 print(
                     "SumupPayment.checkout_prepare OK: "
                     + str(sumupCheckoutResponse.content),
@@ -186,19 +186,23 @@
                 request.session["sumupCheckout"] = ""
                 request.session["sumupToken"] = ""
                 return False
         request.session["sumupCheckout"] = ""
         request.session["sumupToken"] = ""
         return False
 
+    def checkout_prepare(self, request, cart):
+        cs = cart_session(request)
+        return self.sumup_prepare(request, cs["email"], cart["total"])
+
     def payment_prepare(
         self, request: HttpRequest, payment: OrderPayment
     ) -> bool | str:
         print("SumupPayment.payment_prepare", file=sys.stderr)
-        return True
+        return self.sumup_prepare(request, payment.order.email, payment.order.total)
 
     def payment_is_valid_session(self, request):
         print("SumupPayment.payment_is_valid_session", file=sys.stderr)
         return True
 
     def execute_payment(self, request: HttpRequest, payment: OrderPayment):
         print("SumupPayment.execute_payment", file=sys.stderr)
@@ -215,15 +219,16 @@
         subLocale = localeDjango[3:5].upper()
         if subLocale == "":
             subLocale = baseLocale.upper()
         locale = "{}-{}".format(baseLocale, subLocale)
         return locale
 
     def checkout_confirm_render(self, request):
-        print("SumupPayment.checkout_confirm_render", file=sys.stderr)
+        url = resolve(request.path_info)
+        print("SumupPayment.checkout_confirm_render name:{}".format(url.url_name), file=sys.stderr)
         ctx = {
             "request": request,
             "event": self.event,
             "sumupCheckout": request.session["sumupCheckout"],
             "nonce": getNonce(request),
             "locale": self.get_sumup_locale(request),
             "btn_text": _("Payment OK, get your ticket"),
```

### Comparing `pretix-sumup-1.0.5/pretix_sumup/signals.py` & `pretix-sumup-1.0.6/pretix_sumup/signals.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 @receiver(signal=process_response, dispatch_uid="payment_sumup_middleware_resp")
 def signal_process_response(
     sender, request: HttpRequest, response: HttpResponse, **kwargs
 ):
     url = resolve(request.path_info)
-    if url.url_name == "event.checkout":
+    if url.url_name == "event.checkout" or url.url_name == "event.order.pay.confirm":
         if "Content-Security-Policy" in response:
             h = _parse_csp(response["Content-Security-Policy"])
         else:
             h = {}
 
         csps = {
             "script-src": [
```

### Comparing `pretix-sumup-1.0.5/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg` & `pretix-sumup-1.0.6/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html` & `pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup/templates/pretix_sumup/control.html` & `pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pretix_sumup.egg-info/PKG-INFO` & `pretix-sumup-1.0.6/pretix_sumup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.5
+Version: 1.0.6
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.5/pretix_sumup.egg-info/SOURCES.txt` & `pretix-sumup-1.0.6/pretix_sumup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/pyproject.toml` & `pretix-sumup-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.5/setup.cfg` & `pretix-sumup-1.0.6/setup.cfg`

 * *Files identical despite different names*

