# Comparing `tmp/pretix-sumup-1.0.6.tar.gz` & `tmp/pretix-sumup-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sumup-1.0.6.tar", last modified: Tue Aug  1 13:34:29 2023, max compression
+gzip compressed data, was "pretix-sumup-1.0.7.tar", last modified: Tue Aug  1 16:56:49 2023, max compression
```

## Comparing `pretix-sumup-1.0.6.tar` & `pretix-sumup-1.0.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-08-01 13:34:29.427721 pretix-sumup-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/static/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/static/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.419721 pretix-sumup-1.0.6/pretix_sumup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/control.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/email/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/not_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/pending.html
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/prepare.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/pretix_sumup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 13:34:29.000000 pretix-sumup-1.0.6/pretix_sumup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-01 13:34:29.427721 pretix-sumup-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:34:29.423721 pretix-sumup-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 13:33:04.000000 pretix-sumup-1.0.6/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.991945 pretix-sumup-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-08-01 16:56:49.991945 pretix-sumup-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.983945 pretix-sumup-1.0.7/pretix_sumup/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/locale/de_Informal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.983945 pretix-sumup-1.0.7/pretix_sumup/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.983945 pretix-sumup-1.0.7/pretix_sumup/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.983945 pretix-sumup-1.0.7/pretix_sumup/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.983945 pretix-sumup-1.0.7/pretix_sumup/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup/static/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/static/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.983945 pretix-sumup-1.0.7/pretix_sumup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.991945 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/control.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.991945 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/email/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/not_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/pending.html
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/prepare.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.987945 pretix-sumup-1.0.7/pretix_sumup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-08-01 16:56:49.000000 pretix-sumup-1.0.7/pretix_sumup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-01 16:56:49.000000 pretix-sumup-1.0.7/pretix_sumup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:56:49.000000 pretix-sumup-1.0.7/pretix_sumup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 16:56:49.000000 pretix-sumup-1.0.7/pretix_sumup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 16:56:49.000000 pretix-sumup-1.0.7/pretix_sumup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-01 16:56:49.991945 pretix-sumup-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:56:49.991945 pretix-sumup-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 16:55:09.000000 pretix-sumup-1.0.7/tests/test_main.py
```

### Comparing `pretix-sumup-1.0.6/LICENSE` & `pretix-sumup-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.6/PKG-INFO` & `pretix-sumup-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.6
+Version: 1.0.7
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.6/README.md` & `pretix-sumup-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.6/pretix_sumup/apps.py` & `pretix-sumup-1.0.7/pretix_sumup/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.6/pretix_sumup/locale/de/LC_MESSAGES/django.po` & `pretix-sumup-1.0.7/pretix_sumup/locale/de/LC_MESSAGES/django.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2017-03-07 19:01+0100\n"
-"PO-Revision-Date: 2023-07-22 08:57+0000\n"
+"PO-Revision-Date: 2023-08-01 16:53+0000\n"
 "Last-Translator: admin <ronan@highcanfly.club>\n"
-"Language-Team: German <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/"
-"de/>\n"
+"Language-Team: German <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18.2\n"
 
@@ -19,22 +18,18 @@
 msgid "Sumup Payment"
 msgstr "Sumup Zahlung"
 
 msgid "Please fill and click on Pay in the Sumup widget"
 msgstr "Bitte füllen Sie das Sumup-Widget aus und klicken Sie auf Bezahlen"
 
 msgid "In test mode, you can just manually mark this order as paid in the backend after it has been created."
-msgstr ""
-"Im Testmodus können Sie diese Bestellung nach der Erstellung im Backend "
-"einfach manuell als bezahlt markieren."
+msgstr "Im Testmodus können Sie diese Bestellung nach der Erstellung im Backend einfach manuell als bezahlt markieren."
 
 msgid "This is Sumup Client ID (under your name on the top right of the main Sumup screen)"
-msgstr ""
-"Dies ist die Sumup Client-ID (unter Ihrem Namen oben rechts auf dem Sumup "
-"Hauptbildschirm)"
+msgstr "Dies ist die Sumup Client-ID (unter Ihrem Namen oben rechts auf dem Sumup Hauptbildschirm)"
 
 msgid "This is Sumup OAuth app Client Secret"
 msgstr "Dies ist der geheime Clientschlüssel der Sumup OAuth-App"
 
 msgid "Sumup Oauth App Client ID"
 msgstr "Sumup Oauth-App-Client-ID"
 
@@ -44,15 +39,32 @@
 msgid "Payment OK, get your ticket"
 msgstr "Bezahlung OK, holen Sie sich Ihr Ticket"
 
 msgid "You will see the Sumup form after clicking on Continue"
 msgstr "Sie sehen das Sumup Formular, nachdem Sie auf Weiter geklickt haben"
 
 msgid "Sumup plugin is a payment plugin for enabling online payment via Sumup. Note that you will need to register an OAuth application and require to the Sumup team to add the 'payment' scope"
-msgstr ""
-"Das Sumup Plugin ist ein Zahlungs-Plugin zur Ermöglichung von Online-"
-"Zahlungen über Sumup. Beachten Sie, dass Sie eine OAuth-Anwendung "
-"registrieren und das Sumup Team auffordern müssen, den Bereich \"Zahlung\" "
-"hinzuzufügen"
+msgstr "Das Sumup Plugin ist ein Zahlungs-Plugin zur Ermöglichung von Online-Zahlungen über Sumup. Beachten Sie, dass Sie eine OAuth-Anwendung registrieren und das Sumup Team auffordern müssen, den Bereich \"Zahlung\" hinzuzufügen"
 
 msgid "If you have any question don't hesitate to contact us."
 msgstr "Wenn Sie Fragen haben, zögern Sie nicht, uns zu kontaktieren."
+
+msgid "This order has been marked as paid via Sumup Payment manually."
+msgstr "Diese Bestellung wurde manuell über Sumup Payment als bezahlt markiert."
+
+msgid "This order has been paid via Sumup Payment."
+msgstr "Diese Bestellung wurde über Sumup Payment bezahlt."
+
+msgid "This order has been planned to be paid via Sumup Payment, but no payment has been received yet."
+msgstr "Diese Bestellung sollte über Sumup Payment bezahlt werden, aber es ist noch keine Zahlung eingegangen."
+
+msgid "Merchant ID"
+msgstr "Händler-ID"
+
+msgid "Payment date"
+msgstr "Zahlungstermin"
+
+msgid "Transaction"
+msgstr "Transaktion"
+
+msgid "Currency"
+msgstr "Währung"
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-sumup-1.0.7/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2017-03-07 19:01+0100\n"
-"PO-Revision-Date: 2023-07-22 08:57+0000\n"
+"PO-Revision-Date: 2023-08-01 16:53+0000\n"
 "Last-Translator: admin <ronan@highcanfly.club>\n"
-"Language-Team: German <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/"
-"de_INFORMAL/>\n"
+"Language-Team: German <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/de_INFORMAL/>\n"
 "Language: de_Informal\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18.2\n"
 
@@ -19,22 +18,18 @@
 msgid "Sumup Payment"
 msgstr "Sumup Zahlung"
 
 msgid "Please fill and click on Pay in the Sumup widget"
 msgstr "Bitte füllen Sie das Sumup-Widget aus und klicken Sie auf Bezahlen"
 
 msgid "In test mode, you can just manually mark this order as paid in the backend after it has been created."
-msgstr ""
-"Im Testmodus können Sie diese Bestellung nach der Erstellung im Backend "
-"einfach manuell als bezahlt markieren."
+msgstr "Im Testmodus können Sie diese Bestellung nach der Erstellung im Backend einfach manuell als bezahlt markieren."
 
 msgid "This is Sumup Client ID (under your name on the top right of the main Sumup screen)"
-msgstr ""
-"Dies ist die Sumup-Client-ID (unter Ihrem Namen oben rechts auf dem Sumup-"
-"Hauptbildschirm)"
+msgstr "Dies ist die Sumup-Client-ID (unter Ihrem Namen oben rechts auf dem Sumup-Hauptbildschirm)"
 
 msgid "This is Sumup OAuth app Client Secret"
 msgstr "Dies ist der geheime Clientschlüssel der Sumup OAuth-App"
 
 msgid "Sumup Oauth App Client ID"
 msgstr "Sumup Oauth-App-Client-ID"
 
@@ -44,15 +39,32 @@
 msgid "Payment OK, get your ticket"
 msgstr "Bezahlung OK, holen Sie sich Ihr Ticket"
 
 msgid "You will see the Sumup form after clicking on Continue"
 msgstr "Sie sehen das Sumup-Formular, nachdem Sie auf Weiter geklickt haben"
 
 msgid "Sumup plugin is a payment plugin for enabling online payment via Sumup. Note that you will need to register an OAuth application and require to the Sumup team to add the 'payment' scope"
-msgstr ""
-"Das Sumup-Plugin ist ein Zahlungs-Plugin zur Ermöglichung von Online-"
-"Zahlungen über Sumup. Beachten Sie, dass Sie eine OAuth-Anwendung "
-"registrieren und das Sumup-Team auffordern müssen, den Bereich \"Zahlung\" "
-"hinzuzufügen"
+msgstr "Das Sumup-Plugin ist ein Zahlungs-Plugin zur Ermöglichung von Online-Zahlungen über Sumup. Beachten Sie, dass Sie eine OAuth-Anwendung registrieren und das Sumup-Team auffordern müssen, den Bereich \"Zahlung\" hinzuzufügen"
 
 msgid "If you have any question don't hesitate to contact us."
 msgstr "Wenn Sie Fragen haben, zögern Sie nicht, uns zu kontaktieren."
+
+msgid "This order has been marked as paid via Sumup Payment manually."
+msgstr "Diese Bestellung wurde manuell über Sumup Payment als bezahlt markiert."
+
+msgid "This order has been paid via Sumup Payment."
+msgstr "Diese Bestellung wurde über Sumup Payment bezahlt."
+
+msgid "This order has been planned to be paid via Sumup Payment, but no payment has been received yet."
+msgstr "Diese Bestellung sollte über Sumup Payment bezahlt werden, aber es ist noch keine Zahlung eingegangen."
+
+msgid "Merchant ID"
+msgstr "Händler-ID"
+
+msgid "Payment date"
+msgstr "Zahlungstermin"
+
+msgid "Transaction"
+msgstr "Transaktion"
+
+msgid "Currency"
+msgstr "Währung"
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup/locale/es/LC_MESSAGES/django.po` & `pretix-sumup-1.0.7/pretix_sumup/locale/es/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2017-03-07 19:01+0100\n"
-"PO-Revision-Date: 2023-07-22 08:57+0000\n"
+"PO-Revision-Date: 2023-08-01 16:53+0000\n"
 "Last-Translator: admin <ronan@highcanfly.club>\n"
-"Language-Team: Spanish <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/"
-"es/>\n"
+"Language-Team: Spanish <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18.2\n"
 
@@ -19,22 +18,18 @@
 msgid "Sumup Payment"
 msgstr "Pago Sumup"
 
 msgid "Please fill and click on Pay in the Sumup widget"
 msgstr "Por favor, rellene y haga clic en Pagar en el widget Sumup"
 
 msgid "In test mode, you can just manually mark this order as paid in the backend after it has been created."
-msgstr ""
-"En el modo de prueba, puede marcar manualmente este pedido como pagado en el "
-"backend después de que se haya creado."
+msgstr "En el modo de prueba, puede marcar manualmente este pedido como pagado en el backend después de que se haya creado."
 
 msgid "This is Sumup Client ID (under your name on the top right of the main Sumup screen)"
-msgstr ""
-"Este es el ID de cliente de Sumup (debajo de su nombre en la parte superior "
-"derecha de la pantalla principal de Sumup)"
+msgstr "Este es el ID de cliente de Sumup (debajo de su nombre en la parte superior derecha de la pantalla principal de Sumup)"
 
 msgid "This is Sumup OAuth app Client Secret"
 msgstr "Este es el secreto de cliente de la aplicación Sumup OAuth"
 
 msgid "Sumup Oauth App Client ID"
 msgstr "ID de cliente de la aplicación Sumup Oauth"
 
@@ -44,14 +39,32 @@
 msgid "Payment OK, get your ticket"
 msgstr "Pago OK, obtenga su boleto"
 
 msgid "You will see the Sumup form after clicking on Continue"
 msgstr "Verá el formulario de resumen después de hacer clic en Continuar"
 
 msgid "Sumup plugin is a payment plugin for enabling online payment via Sumup. Note that you will need to register an OAuth application and require to the Sumup team to add the 'payment' scope"
-msgstr ""
-"El complemento Sumup es un complemento de pago para habilitar el pago en "
-"línea a través de Sumup. Tenga en cuenta que deberá registrar una aplicación "
-"OAuth y solicitar al equipo de Sumup que agregue el ámbito de \"pago\""
+msgstr "El complemento Sumup es un complemento de pago para habilitar el pago en línea a través de Sumup. Tenga en cuenta que deberá registrar una aplicación OAuth y solicitar al equipo de Sumup que agregue el ámbito de \"pago\""
 
 msgid "If you have any question don't hesitate to contact us."
 msgstr "Si tiene alguna pregunta no dude en ponerse en contacto con nosotros."
+
+msgid "This order has been marked as paid via Sumup Payment manually."
+msgstr "Este pedido se ha marcado como pagado a través de Sumup Payment manualmente."
+
+msgid "This order has been paid via Sumup Payment."
+msgstr "Este pedido ha sido pagado a través de Sumup Payment."
+
+msgid "This order has been planned to be paid via Sumup Payment, but no payment has been received yet."
+msgstr "Se ha planeado que este pedido se pague a través de Sumup Payment, pero aún no se ha recibido ningún pago."
+
+msgid "Merchant ID"
+msgstr "ID de comerciante"
+
+msgid "Payment date"
+msgstr "Fecha de pago"
+
+msgid "Transaction"
+msgstr "Transacción"
+
+msgid "Currency"
+msgstr "Divisa"
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup/locale/fr/LC_MESSAGES/django.po` & `pretix-sumup-1.0.7/pretix_sumup/locale/fr/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2017-03-07 19:01+0100\n"
-"PO-Revision-Date: 2023-07-30 16:08+0000\n"
+"PO-Revision-Date: 2023-08-01 16:53+0000\n"
 "Last-Translator: admin <ronan@highcanfly.club>\n"
-"Language-Team: French <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/"
-"fr/>\n"
+"Language-Team: French <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.18.2\n"
 
@@ -41,14 +40,32 @@
 msgid "Payment OK, get your ticket"
 msgstr "Paiement ok, obtenez votre billet"
 
 msgid "You will see the Sumup form after clicking on Continue"
 msgstr "Vous verrez le formulaire Sumup après avoir cliqué sur Continuer"
 
 msgid "Sumup plugin is a payment plugin for enabling online payment via Sumup. Note that you will need to register an OAuth application and require to the Sumup team to add the 'payment' scope"
-msgstr ""
-"Le plugin Sumup est un plugin de paiement pour activer le paiement en ligne "
-"via Sumup. Notez que vous devrez enregistrer une application OAuth et "
-"demander à l'équipe Sumup pour ajouter le scope 'payment'"
+msgstr "Le plugin Sumup est un plugin de paiement pour activer le paiement en ligne via Sumup. Notez que vous devrez enregistrer une application OAuth et demander à l'équipe Sumup pour ajouter le scope 'payment'"
 
 msgid "If you have any question don't hesitate to contact us."
 msgstr "Si vous avez des questions, n’hésitez pas à nous contacter."
+
+msgid "This order has been marked as paid via Sumup Payment manually."
+msgstr "Cette commande a été marquée comme payée manuellement via un paiement Sumup."
+
+msgid "This order has been paid via Sumup Payment."
+msgstr "Cette commande a été payée via un paiement Sumup."
+
+msgid "This order has been planned to be paid via Sumup Payment, but no payment has been received yet."
+msgstr "Cette commande a été planifiée pour être payée via un paiement Sumup, mais aucun paiement n’a encore été reçu."
+
+msgid "Merchant ID"
+msgstr "Numéro d’identification du commerçant"
+
+msgid "Payment date"
+msgstr "Date de paiement"
+
+msgid "Transaction"
+msgstr "Transaction"
+
+msgid "Currency"
+msgstr "Monnaie"
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup/locale/it/LC_MESSAGES/django.po` & `pretix-sumup-1.0.7/pretix_sumup/locale/it/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2017-03-07 19:01+0100\n"
-"PO-Revision-Date: 2023-07-22 09:29+0000\n"
+"PO-Revision-Date: 2023-08-01 16:53+0000\n"
 "Last-Translator: admin <ronan@highcanfly.club>\n"
-"Language-Team: Italian <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/"
-"it/>\n"
+"Language-Team: Italian <http://oci.sctg.eu.org/projects/pretix-sumup/plugin/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18.2\n"
 
@@ -19,22 +18,18 @@
 msgid "Sumup Payment"
 msgstr "Pagamento Sumup"
 
 msgid "Please fill and click on Pay in the Sumup widget"
 msgstr "Si prega di compilare e fare clic su Paga nel widget Sumup"
 
 msgid "In test mode, you can just manually mark this order as paid in the backend after it has been created."
-msgstr ""
-"In modalità test, puoi semplicemente contrassegnare manualmente questo "
-"ordine come pagato nel back-end dopo che è stato creato."
+msgstr "In modalità test, puoi semplicemente contrassegnare manualmente questo ordine come pagato nel back-end dopo che è stato creato."
 
 msgid "This is Sumup Client ID (under your name on the top right of the main Sumup screen)"
-msgstr ""
-"Questo è l'ID client Sumup (sotto il tuo nome in alto a destra nella "
-"schermata principale di Sumup)"
+msgstr "Questo è l'ID client Sumup (sotto il tuo nome in alto a destra nella schermata principale di Sumup)"
 
 msgid "This is Sumup OAuth app Client Secret"
 msgstr "Questo è il segreto client dell'app Sumup OAuth"
 
 msgid "Sumup Oauth App Client ID"
 msgstr "ID client dell'app Sumup Oauth"
 
@@ -44,14 +39,32 @@
 msgid "Payment OK, get your ticket"
 msgstr "Pagamento OK, prendi il tuo biglietto"
 
 msgid "You will see the Sumup form after clicking on Continue"
 msgstr "Vedrai il modulo Sumup dopo aver cliccato su Continua"
 
 msgid "Sumup plugin is a payment plugin for enabling online payment via Sumup. Note that you will need to register an OAuth application and require to the Sumup team to add the 'payment' scope"
-msgstr ""
-"Sumup plugin è un plugin di pagamento per abilitare il pagamento online "
-"tramite Sumup. Tieni presente che dovrai registrare un'applicazione OAuth e "
-"richiedere al team di Sumup di aggiungere l'ambito di \"pagamento\""
+msgstr "Sumup plugin è un plugin di pagamento per abilitare il pagamento online tramite Sumup. Tieni presente che dovrai registrare un'applicazione OAuth e richiedere al team di Sumup di aggiungere l'ambito di \"pagamento\""
 
 msgid "If you have any question don't hesitate to contact us."
 msgstr "Se hai qualche domanda non esitare a contattarci."
+
+msgid "This order has been marked as paid via Sumup Payment manually."
+msgstr "Questo ordine è stato contrassegnato come pagato manualmente tramite Sumup Payment."
+
+msgid "This order has been paid via Sumup Payment."
+msgstr "Questo ordine è stato pagato tramite Sumup Payment."
+
+msgid "This order has been planned to be paid via Sumup Payment, but no payment has been received yet."
+msgstr "Questo ordine è stato pianificato per essere pagato tramite Sumup Payment, ma nessun pagamento è stato ancora ricevuto."
+
+msgid "Merchant ID"
+msgstr "ID commerciante"
+
+msgid "Payment date"
+msgstr "Data di pagamento"
+
+msgid "Transaction"
+msgstr "Transazione"
+
+msgid "Currency"
+msgstr "Valuta"
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup/payment.py` & `pretix-sumup-1.0.7/pretix_sumup/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             "Accept": "application/json",
             "Authorization": "Bearer " + merchantToken,
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
         return response
 
-    def check_sumup_payment_done(self, sumupToken, sumupCheckout):
+    def check_sumup_payment_response(self, sumupToken, sumupCheckout):
         print("SumupPayment.check_sumup_payment_done", file=sys.stderr)
         url = "https://api.sumup.com/v0.1/checkouts/" + sumupCheckout["id"]
         headers = {
             "Content-Type": "application/json",
             "Accept": "application/json",
             "Authorization": "Bearer " + sumupToken,
         }
@@ -125,18 +125,15 @@
         sumupResponse = json.loads(response.content)
         print(
             "Sumup checkout:{} status: {}".format(
                 sumupCheckout["id"], sumupResponse["status"]
             ),
             file=sys.stderr,
         )
-        if sumupResponse["status"] == "PAID":
-            return True
-        else:
-            return False
+        return sumupResponse
 
     def payment_form_render(self, request: HttpRequest, total: Decimal, order: Order = None) -> str:
         def get_invoice_address():
             if order and getattr(order, 'invoice_address', None):
                 request._checkout_flow_invoice_address = order.invoice_address
             if not hasattr(request, '_checkout_flow_invoice_address'):
                 cs = cart_session(request)
@@ -203,18 +200,23 @@
     def payment_is_valid_session(self, request):
         print("SumupPayment.payment_is_valid_session", file=sys.stderr)
         return True
 
     def execute_payment(self, request: HttpRequest, payment: OrderPayment):
         print("SumupPayment.execute_payment", file=sys.stderr)
         if ("sumupCheckout" in request.session) and ("sumupToken" in request.session):
-            if self.check_sumup_payment_done(
+            sumupResponse = self.check_sumup_payment_response(
                 request.session["sumupToken"], request.session["sumupCheckout"]
-            ):
+            )
+            if sumupResponse["status"] == "PAID":
+                payment.info_data = sumupResponse
                 payment.confirm()
+            else:
+                payment.fail()
+                
 
     def get_sumup_locale(self, request):
         languageDjango = get_language()
         localeDjango = to_locale(languageDjango)
         baseLocale = localeDjango[0:2]
         subLocale = localeDjango[3:5].upper()
         if subLocale == "":
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup/signals.py` & `pretix-sumup-1.0.7/pretix_sumup/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.6/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg` & `pretix-sumup-1.0.7/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html` & `pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html`

 * *Files 11% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 console.log('Body', body);
                 if (type == "success") {
                     document.getElementById('help-text').innerHTML = "";
                     sumupCard.unmount();
                     submitElm.classList.remove('hidden');
                     submitElm.disabled = false;
                     submitElm.innerHTML = "{{btn_text}}";
-                    document.querySelector("body > div.container.main-box > main > form").submit();
+                    submitElm.closest('form').submit()
                 }
             }
         });
     })
 
 
 </script>
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup/templates/pretix_sumup/control.html` & `pretix-sumup-1.0.7/pretix_sumup/templates/pretix_sumup/control.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 {% load i18n %}
-
-{% if payment_info and order.status == "p" %}
-    <p>{% blocktrans trimmed %}
-        This order has been paid via Sumup Payment.
+{% if payment_info.status == "PAID" and order.status == "p" %}
+<p>{% blocktrans trimmed %}
+    This order has been paid via Sumup Payment.
     {% endblocktrans %}</p>
 
-    <dl class="dl-horizontal">
-        <dt>{% trans "Payer" %}</dt>
-        <dd>{{ payment_info.payer }}</dd>
-        <dt>{% trans "Payment date" %}</dt>
-        <dd>{{ payment_info.date }}</dd>
-        <dt>{% trans "Reference" %}</dt>
-        <dd>{{ payment_info.reference }}</dd>
-    </dl>
+<dl class="dl-horizontal">
+    <dt>{% trans "Merchant ID" %}</dt>
+    <dd>{{ payment_info.merchant_code }}</dd>
+    <dt>{% trans "Payment date" %}</dt>
+    <dd>{{ payment_info.date }}</dd>
+    <dt>{% trans "Transaction" %}</dt>
+    <dd>{{ payment_info.transaction_code }}</dd>
+    <dt>{% trans "Currency" %}</dt>
+    <dd>{{ payment_info.currency }}</dd>
+</dl>
 {% else %}
-    {% if order.status == "p" %}
-        <p>{% blocktrans trimmed %}
-            This order has been marked as paid via Sumup Payment manually.
-        {% endblocktrans %}</p>
-    {% else %}
-        <p>{% blocktrans trimmed %}
-            This order has been planned to be paid via Sumup Payment, but no payment has been received yet.
-        {% endblocktrans %}</p>
-    {% endif %}
-    <dl class="dl-horizontal">
-        <dt>{% trans "Reference code" %}</dt>
-        <dd>{{ order.full_code }}</dd>
-    </dl>
+<p>{% blocktrans trimmed %}
+    This order has been planned to be paid via Sumup Payment, but no payment has been received yet.
+    {% endblocktrans %}</p>
+<dl class="dl-horizontal">
+    <dt>{% trans "Reference code" %}</dt>
+    <dd>{{ order.full_code }}</dd>
+</dl>
 {% endif %}
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup.egg-info/PKG-INFO` & `pretix-sumup-1.0.7/pretix_sumup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.6
+Version: 1.0.7
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.6/pretix_sumup.egg-info/SOURCES.txt` & `pretix-sumup-1.0.7/pretix_sumup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.6/pyproject.toml` & `pretix-sumup-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.6/setup.cfg` & `pretix-sumup-1.0.7/setup.cfg`

 * *Files identical despite different names*

