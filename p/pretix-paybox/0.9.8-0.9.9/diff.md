# Comparing `tmp/pretix-paybox-0.9.8.tar.gz` & `tmp/pretix-paybox-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-paybox-0.9.8.tar", last modified: Mon Jul 31 18:32:56 2023, max compression
+gzip compressed data, was "pretix-paybox-0.9.9.tar", last modified: Tue Aug  1 16:13:57 2023, max compression
```

## Comparing `pretix-paybox-0.9.8.tar` & `pretix-paybox-0.9.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.860541 pretix-paybox-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    33895 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-31 18:32:56.860541 pretix-paybox-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.856541 pretix-paybox-0.9.8/pretix_paybox/
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/Paybox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/PayboxCheck.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.856541 pretix-paybox-0.9.8/pretix_paybox/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.852541 pretix-paybox-0.9.8/pretix_paybox/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.856541 pretix-paybox-0.9.8/pretix_paybox/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.852541 pretix-paybox-0.9.8/pretix_paybox/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.856541 pretix-paybox-0.9.8/pretix_paybox/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.852541 pretix-paybox-0.9.8/pretix_paybox/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.856541 pretix-paybox-0.9.8/pretix_paybox/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.852541 pretix-paybox-0.9.8/pretix_paybox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.856541 pretix-paybox-0.9.8/pretix_paybox/static/pretix_paybox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/static/pretix_paybox/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/static/pretix_paybox/Up2Pay_eTransactions.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.852541 pretix-paybox-0.9.8/pretix_paybox/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.860541 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/checkout_payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/control.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.860541 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/email/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/email/order_pending.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/pending.html
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/prepare.html
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/templates/pretix_paybox/redirect.html
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pretix_paybox/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.856541 pretix-paybox-0.9.8/pretix_paybox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-31 18:32:56.000000 pretix-paybox-0.9.8/pretix_paybox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-31 18:32:56.000000 pretix-paybox-0.9.8/pretix_paybox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:32:56.000000 pretix-paybox-0.9.8/pretix_paybox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 18:32:56.000000 pretix-paybox-0.9.8/pretix_paybox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 18:32:56.000000 pretix-paybox-0.9.8/pretix_paybox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 18:32:56.000000 pretix-paybox-0.9.8/pretix_paybox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-31 18:32:56.860541 pretix-paybox-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:32:56.860541 pretix-paybox-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 18:31:10.000000 pretix-paybox-0.9.8/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.651370 pretix-paybox-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    33895 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-01 16:13:57.651370 pretix-paybox-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.647370 pretix-paybox-0.9.9/pretix_paybox/
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/Paybox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/PayboxCheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.647370 pretix-paybox-0.9.9/pretix_paybox/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.639370 pretix-paybox-0.9.9/pretix_paybox/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.647370 pretix-paybox-0.9.9/pretix_paybox/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.639370 pretix-paybox-0.9.9/pretix_paybox/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.647370 pretix-paybox-0.9.9/pretix_paybox/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.639370 pretix-paybox-0.9.9/pretix_paybox/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.647370 pretix-paybox-0.9.9/pretix_paybox/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    16255 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.639370 pretix-paybox-0.9.9/pretix_paybox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.647370 pretix-paybox-0.9.9/pretix_paybox/static/pretix_paybox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/static/pretix_paybox/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/static/pretix_paybox/Up2Pay_eTransactions.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.643370 pretix-paybox-0.9.9/pretix_paybox/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.651370 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/checkout_payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/control.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.651370 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/email/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/email/order_pending.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/pending.html
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/prepare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/templates/pretix_paybox/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pretix_paybox/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.647370 pretix-paybox-0.9.9/pretix_paybox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-01 16:13:57.000000 pretix-paybox-0.9.9/pretix_paybox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-01 16:13:57.000000 pretix-paybox-0.9.9/pretix_paybox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:13:57.000000 pretix-paybox-0.9.9/pretix_paybox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 16:13:57.000000 pretix-paybox-0.9.9/pretix_paybox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 16:13:57.000000 pretix-paybox-0.9.9/pretix_paybox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 16:13:57.000000 pretix-paybox-0.9.9/pretix_paybox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 16:13:57.651370 pretix-paybox-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:13:57.651370 pretix-paybox-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 16:12:10.000000 pretix-paybox-0.9.9/tests/test_main.py
```

### Comparing `pretix-paybox-0.9.8/LICENSE` & `pretix-paybox-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/MANIFEST.in` & `pretix-paybox-0.9.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/PKG-INFO` & `pretix-paybox-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-paybox
-Version: 0.9.8
+Version: 0.9.9
 Summary: Paybox payment plugin for Pretix 4
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: AGPLv3
 Project-URL: homepage, https://github.com/highcanfly-club/pretix-paybox
 Project-URL: repository, https://github.com/highcanfly-club/pretix-paybox
 Keywords: pretix
```

### Comparing `pretix-paybox-0.9.8/README.md` & `pretix-paybox-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/pretix_paybox/Paybox.py` & `pretix-paybox-0.9.9/pretix_paybox/Paybox.py`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/pretix_paybox/apps.py` & `pretix-paybox-0.9.9/pretix_paybox/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/pretix_paybox/locale/de/LC_MESSAGES/django.po` & `pretix-paybox-0.9.9/pretix_paybox/locale/django.pot`

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,151 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2017-03-07 19:01+0100\n"
-"PO-Revision-Date: 2023-07-31 17:58+0000\n"
-"Last-Translator: admin <ronan@highcanfly.club>\n"
-"Language-Team: German <http://oci.sctg.eu.org/projects/pretix-paybox/plugin/"
-"de/>\n"
-"Language: de\n"
+"PO-Revision-Date: \n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"Plural-Forms: \n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18.2\n"
+""
 
 msgid "Paybox for Pretix"
-msgstr "Paybox für Pretix"
+msgstr ""
 
 msgid "Paybox Payment"
-msgstr "Paybox-Zahlung"
+msgstr ""
 
 msgid "Paybox payment plugin for Pretix 4"
-msgstr "Paybox-Zahlungs-Plugin für Pretix 4"
+msgstr ""
 
 msgid "Paybox production HMAC"
-msgstr "Paybox-Produktion HMAC"
+msgstr ""
 
 msgid "The production HMAC key"
-msgstr "Der HMAC-Schlüssel für die Produktion"
+msgstr ""
 
 msgid "The sandbox HMAC key"
-msgstr "Der Sandbox-HMAC-Schlüssel"
+msgstr ""
 
 msgid "This is the Paybox site ID"
-msgstr "Dies ist die Paybox-Site-ID"
+msgstr ""
 
 msgid "Paybox rank"
-msgstr "Paybox-Rang"
+msgstr ""
 
 msgid "This is the two characters rank ID"
-msgstr "Dies ist die Rang-ID der beiden Zeichen"
+msgstr ""
 
 msgid "Endpoint"
-msgstr "Endpunkt"
+msgstr ""
 
 msgid "Live"
-msgstr "Leben"
+msgstr ""
 
 msgid "Sandbox"
-msgstr "Sandkasten"
+msgstr ""
 
 msgid "This is the main Paybox ID"
-msgstr "Dies ist die Haupt-Paybox-ID"
+msgstr ""
 
 msgid "Production server"
-msgstr "Produktionsserver"
+msgstr ""
 
 msgid "Sandbox server"
-msgstr "Sandbox-Server"
+msgstr ""
 
 msgid "Application path"
-msgstr "Pfad der Bewerbung"
+msgstr ""
 
 msgid "The path part of the complete URL (server+path)"
-msgstr "Der Pfadteil der vollständigen URL (Server+Pfad)"
+msgstr ""
 
 msgid "Card Holder Last Name"
-msgstr "Nachname des Karteninhabers"
+msgstr ""
 
 msgid "Card Holder First Name"
-msgstr "Vorname des Karteninhabers"
+msgstr ""
 
 msgid "Card Holder Street"
-msgstr "Kartenhalter Straße"
+msgstr ""
 
 msgid "Card Holder Address Complement"
-msgstr "Adressergänzung des Karteninhabers"
+msgstr ""
 
 msgid "Card Holder Postal Code"
-msgstr "Postleitzahl des Karteninhabers"
+msgstr ""
 
 msgid "Card Holder City"
-msgstr "Karteninhaber Stadt"
+msgstr ""
 
 msgid "Card Holder Country"
-msgstr "Land des Karteninhabers"
+msgstr ""
 
 msgid "The production server base URL"
-msgstr "Die Basis-URL des Produktionsservers"
+msgstr ""
 
 msgid "The sandbox server base URL"
-msgstr "Die Basis-URL des Sandbox-Servers"
+msgstr ""
 
 msgid "Paybox identifier"
-msgstr "Paybox-Kennung"
+msgstr ""
 
 msgid "Server Error"
-msgstr "Server-Fehler"
+msgstr ""
 
 msgid "Go to Paybox/Up2Pay secured website"
-msgstr "Gehen Sie zur gesicherten Website von Paybox/Up2Pay"
+msgstr ""
 
 msgid "refused"
-msgstr "abgewiesen"
+msgstr ""
 
 msgid "answer to"
-msgstr "Antwort auf"
+msgstr ""
 
 msgid "unkown error"
-msgstr "Unbekannter Fehler"
+msgstr ""
 
 msgid "canceled"
-msgstr "abgebrochen"
+msgstr ""
 
 msgid "pending"
-msgstr "anhängig"
+msgstr ""
+
+msgid "You will redirected to the Paybox/Up2Pay secured website after clicking on 'Place binding order'"
+msgstr ""
+
+msgid "This order has been paid via Paybox/Up2Pay Payment."
+msgstr ""
+
+msgid "This order has been marked as paid via Paybox/Up2Pay Payment manually."
+msgstr ""
+
+msgid "This order has been planned to be paid via Paybox/Up2Pay Payment, but no payment has been received yet."
+msgstr ""
+
+msgid "Payment is pending"
+msgstr ""
+
+msgid "Transaction"
+msgstr ""
+
+msgid "Authorization"
+msgstr ""
+
+msgid "Card type"
+msgstr ""
+
+msgid "Card number"
+msgstr ""
+
+msgid "Card expiration"
+msgstr ""
+
+msgid "Payment date"
+msgstr ""
+
+msgid "Reference"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pretix-paybox-0.9.8/pretix_paybox/locale/fr/LC_MESSAGES/django.po` & `pretix-paybox-0.9.9/pretix_paybox/locale/fr/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 msgid ""
-msgstr ""
-"Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-03-07 19:01+0100\n"
-"PO-Revision-Date: 2023-07-31 17:58+0000\n"
-"Last-Translator: admin <ronan@highcanfly.club>\n"
-"Language-Team: French <http://oci.sctg.eu.org/projects/pretix-paybox/plugin/"
-"fr/>\n"
-"Language: fr\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.18.2\n"
+msgstr "Report-Msgid-Bugs-To: \nPOT-Creation-Date: 2017-03-07 19:01+0100\nPO-Revision-Date: 2023-08-01 16:01+0000\nLast-Translator: admin <ronan@highcanfly.club>\nLanguage-Team: French <http://oci.sctg.eu.org/projects/pretix-paybox/plugin/fr/>\nLanguage: fr\nMIME-Version: 1.0\nContent-Type: text/plain; charset=UTF-8\nContent-Transfer-Encoding: 8bit\nPlural-Forms: nplurals=2; plural=n > 1;\nX-Generator: Weblate 4.18.2\n"
 
 msgid "Paybox for Pretix"
 msgstr "Paybox pour Pretix"
 
 msgid "Paybox Payment"
 msgstr "Paiement Paybox"
 
@@ -111,23 +99,55 @@
 
 msgid "canceled"
 msgstr "Annulé"
 
 msgid "pending"
 msgstr "en instance"
 
+msgid "You will redirected to the Paybox/Up2Pay secured website after clicking on 'Place binding order'"
+msgstr "Vous serez redirigé vers le site sécurisé Paybox/Up2Pay après avoir cliqué sur 'Passer une commande'"
+
+msgid "This order has been paid via Paybox/Up2Pay Payment."
+msgstr "Cette commande a été payée via un paiement Paybox/Up2Pay."
+
+msgid "This order has been marked as paid via Paybox/Up2Pay Payment manually."
+msgstr "Cette commande a été marquée comme payée manuellement via un paiement Paybox/Up2Pay."
+
+msgid "This order has been planned to be paid via Paybox/Up2Pay Payment, but no payment has been received yet."
+msgstr "Cette commande a été planifiée pour être payée via un paiement Paybox/Up2Pay, mais aucun paiement n’a encore été reçu."
+
+msgid "Payment is pending"
+msgstr "Le paiement est en attente"
+
+msgid "Transaction"
+msgstr "Transaction"
+
+msgid "Authorization"
+msgstr "Autorisation"
+
+msgid "Card type"
+msgstr "Type de carte"
+
+msgid "Card number"
+msgstr "Numéro de carte"
+
+msgid "Card expiration"
+msgstr "Expiration de la carte"
+
+msgid "Payment date"
+msgstr "Date de paiement"
+
+msgid "Reference"
+msgstr "Référence"
+
 #~ msgid "Paybox plugin"
 #~ msgstr "Plugin Paybox"
 
-#~ msgid ""
-#~ "In test mode, you can just manually mark this order as paid in the "
-#~ "backend after it has been created."
-#~ msgstr ""
-#~ "En mode test, vous pouvez simplement marquer manuellement cette commande "
-#~ "comme payée dans le backend après sa création."
+#~ msgid "In test mode, you can just manually mark this order as paid in the backend after it has been created."
+#~ msgstr "En mode test, vous pouvez simplement marquer manuellement cette commande comme payée dans le backend après sa création."
 
 #~ msgid "Paybox sandbox HMAC"
 #~ msgstr "HMAC bac à sable Paybox"
 
 #, fuzzy
 #~| msgid "Paybox Payment"
 #~ msgid "Paybox site"
```

### Comparing `pretix-paybox-0.9.8/pretix_paybox/payment.py` & `pretix-paybox-0.9.9/pretix_paybox/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,47 +102,51 @@
             (
                 "sandbox_secret",
                 forms.CharField(
                     label=_("Paybox sandbox HMAC"),
                     max_length=128,
                     min_length=128,
                     help_text=_("The sandbox HMAC key"),
+                    initial="0123456789ABCDEF0123456789ABCDEF0123456789ABCDEF0123456789ABCDEF0123456789ABCDEF0123456789ABCDEF0123456789ABCDEF0123456789ABCDEF"
                 ),
             ),
             (
                 "paybox_site",
                 forms.CharField(
                     label=_("Paybox site"),
                     max_length=8,
                     min_length=6,
                     help_text=_(
                         "This is the Paybox site ID"
                     ),
+                    initial="1999888"
                 ),
             ),
             (
                 "paybox_rank",
                 forms.CharField(
                     label=_("Paybox rank"),
                     max_length=2,
                     min_length=2,
                     help_text=_(
                         "This is the two characters rank ID"
                     ),
+                    initial="32"
                 ),
             ),
             (
                 "paybox_id",
                 forms.CharField(
                     label=_("Paybox identifier"),
                     max_length=9,
                     min_length=1,
                     help_text=_(
                         "This is the main Paybox ID"
                     ),
+                    initial="2"
                 ),
             ),
         ]
         return OrderedDict(fields + list(super().settings_form_fields.items()))
 
     def payment_form_render(self, request: HttpRequest, total: Decimal, order: Order = None) -> str:
         def get_invoice_address():
@@ -323,14 +327,19 @@
         }
         return template.render(ctx)
 
     def payment_control_render(self, request: HttpRequest, payment: OrderPayment):
         print("PayboxPayment.payment_control_render", file=sys.stderr)
         template = get_template("pretix_paybox/control.html")
         ctx = {
+            "request": request,
+            "event": self.event,
+            "payment": payment,
+            "payment_info": payment.info_data,
+            "order": payment.order,
         }
         return template.render(ctx)
 
     def payment_form(self, request: HttpRequest) -> Form:
         """
         This is called by the default implementation of :py:meth:`payment_form_render`
         to obtain the form that is displayed to the user during the checkout
```

### Comparing `pretix-paybox-0.9.8/pretix_paybox/signals.py` & `pretix-paybox-0.9.9/pretix_paybox/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/pretix_paybox/static/pretix_paybox/Up2Pay_eTransactions.svg` & `pretix-paybox-0.9.9/pretix_paybox/static/pretix_paybox/Up2Pay_eTransactions.svg`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/pretix_paybox/urls.py` & `pretix-paybox-0.9.9/pretix_paybox/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/pretix_paybox/views.py` & `pretix-paybox-0.9.9/pretix_paybox/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,87 @@
 import sys
 from django.http import HttpResponse
+from django.shortcuts import redirect, render
 from django.urls import resolve
-from .payment import check_signed_uuid4, PayboxPayment, getNonce
-from pretix.base.models import Event, Organizer, OrderPayment
+from django.utils.translation import gettext_lazy as _
 from django_scopes import scope
-from django.shortcuts import redirect, render
+from pretix.base.models import Event, OrderPayment, Organizer
 from pretix.multidomain.urlreverse import eventreverse
-from django.utils.translation import gettext_lazy as _
-from .PayboxCheck import verify_response
+from urllib.parse import parse_qs, urlparse
+
+from .PayboxCheck import get_object_response, verify_response
+from .payment import PayboxPayment, check_signed_uuid4, getNonce
 
 
-def refuse(request):
+def refuse(request, *args, **kwargs):
     print('views.refuse', file=sys.stderr)
-    pid = request.GET.get('paymentId')
-    return HttpResponse(_('refused'), status=500)
+    return annule(request, kwargs)
 
 
-def repondre_a(request):
+def repondre_a(request, *args, **kwargs):
     print('views.repondre_a', file=sys.stderr)
-    pid = request.GET.get('paymentId')
-    return HttpResponse(_("answer to"), status=500)
+    return annule(request, kwargs)
+
+
+def get_response_code(request):
+    uri = request.build_absolute_uri()
+    url_parsed = urlparse(uri)
+    query = parse_qs(url_parsed.query)  # dictionnary
+    error = query["error"][0]
+    return error
 
 
 def effectue(request, *args, **kwargs):
     print('views.effectue', file=sys.stderr)
     pid = request.GET.get('paymentId')
-    print(pid, file=sys.stderr)
     if pid == request.session['payment_payboxpayment_uuid4']:
         if request.session.get('paybox_payment_info'):
             paybox_payment_info = request.session.get('paybox_payment_info')
             payment = OrderPayment.objects.get(pk=paybox_payment_info["payment_id"])
         else:
             payment = None
         if payment:
             check = verify_response(request.build_absolute_uri())
             if check:
-                payment.confirm()
-                return redirect(eventreverse(request.event, 'presale:event.order', kwargs={
-                    'order': payment.order.code,
-                    'secret': payment.order.secret
-                }) + '?paid=yes')
+                if get_response_code(request) == "00000":
+                    payment.info_data = get_object_response(request.build_absolute_uri())
+                    payment.confirm()
+                    return redirect(eventreverse(request.event, 'presale:event.order', kwargs={
+                        'order': payment.order.code,
+                        'secret': payment.order.secret
+                    }) + '?paid=yes')
+                else:
+                    payment.fail()
+                    return redirect(eventreverse(request.event, 'presale:event.order', kwargs={
+                        'order': payment.order.code,
+                        'secret': payment.order.secret
+                    }))
     return HttpResponse(_("unkown error"), status=200)
 
 
-def annule(request):
+def annule(request, *args, **kwargs):
     print('views.annule', file=sys.stderr)
     pid = request.GET.get('paymentId')
+    if pid == request.session['payment_payboxpayment_uuid4']:
+        check = verify_response(request.build_absolute_uri())
+        if check:
+            if request.session.get('paybox_payment_info'):
+                paybox_payment_info = request.session.get('paybox_payment_info')
+                payment = OrderPayment.objects.get(pk=paybox_payment_info["payment_id"])
+                payment.fail()
+                return redirect(eventreverse(request.event, 'presale:event.order', kwargs={
+                    'order': payment.order.code,
+                    'secret': payment.order.secret
+                }))
     return HttpResponse(_("canceled"), status=500)
 
 
-def attente(request):
+def attente(request, *args, **kwargs):
     print('views.attente', file=sys.stderr)
-    pid = request.GET.get('paymentId')
-    return HttpResponse(_("pending"), status=500)
+    return annule(request, kwargs)
 
 
 def redirectview(request, *args, **kwargs):
     print('views.redirect', file=sys.stderr)
     url = resolve(request.path_info)
     print("PayboxPayment.redirectview {}".format(url.url_name), file=sys.stderr)
     spid = request.GET.get('suuid4')
```

### Comparing `pretix-paybox-0.9.8/pretix_paybox.egg-info/PKG-INFO` & `pretix-paybox-0.9.9/pretix_paybox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-paybox
-Version: 0.9.8
+Version: 0.9.9
 Summary: Paybox payment plugin for Pretix 4
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: AGPLv3
 Project-URL: homepage, https://github.com/highcanfly-club/pretix-paybox
 Project-URL: repository, https://github.com/highcanfly-club/pretix-paybox
 Keywords: pretix
```

### Comparing `pretix-paybox-0.9.8/pretix_paybox.egg-info/SOURCES.txt` & `pretix-paybox-0.9.9/pretix_paybox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/pyproject.toml` & `pretix-paybox-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-paybox-0.9.8/setup.cfg` & `pretix-paybox-0.9.9/setup.cfg`

 * *Files identical despite different names*

