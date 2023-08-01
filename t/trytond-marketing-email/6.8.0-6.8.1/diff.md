# Comparing `tmp/trytond_marketing_email-6.8.0.tar.gz` & `tmp/trytond_marketing_email-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_marketing_email-6.8.0.tar", last modified: Mon May  1 11:58:01 2023, max compression
+gzip compressed data, was "trytond_marketing_email-6.8.1.tar", last modified: Tue Aug  1 19:52:31 2023, max compression
```

## Comparing `trytond_marketing_email-6.8.0.tar` & `trytond_marketing_email-6.8.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.051302 trytond_marketing_email-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      660 2023-05-01 11:12:18.000000 trytond_marketing_email-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-05-01 11:12:17.000000 trytond_marketing_email-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3636 2023-05-01 11:58:01.051302 trytond_marketing_email-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      729 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.047969 trytond_marketing_email-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1785 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/email_subscribe.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/email_unsubscribe.html
--rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/empty.gif
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-29 22:04:03.000000 trytond_marketing_email-6.8.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.047969 trytond_marketing_email-6.8.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/icons/tryton-marketing-mail.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.041302 trytond_marketing_email-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6184 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6124 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6249 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6061 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5373 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5205 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6014 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-04-29 08:02:48.000000 trytond_marketing_email-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18644 2023-04-29 22:04:03.000000 trytond_marketing_email-6.8.0/marketing.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10433 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/marketing.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      603 2023-04-29 22:04:03.000000 trytond_marketing_email-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:58:01.051302 trytond_marketing_email-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4311 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.041302 trytond_marketing_email-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5610 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-05-01 11:12:12.000000 trytond_marketing_email-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.047969 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3636 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1955 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:58:00.000000 trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:58:01.044635 trytond_marketing_email-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-28 07:46:16.000000 trytond_marketing_email-6.8.0/view/email_list_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1066 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/email_message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/view/send_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-04-15 07:12:15.000000 trytond_marketing_email-6.8.0/web.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:52:31.020811 trytond_marketing_email-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-08-01 19:52:27.000000 trytond_marketing_email-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      725 2023-08-01 19:52:27.000000 trytond_marketing_email-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3636 2023-08-01 19:52:31.020811 trytond_marketing_email-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      729 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:52:31.017477 trytond_marketing_email-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1446 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1785 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/email_subscribe.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/email_unsubscribe.html
+-rw-r--r--   0 ced       (1000) ced       (1000)       43 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/empty.gif
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:52:31.017477 trytond_marketing_email-6.8.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/icons/tryton-marketing-mail.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      464 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:52:31.014144 trytond_marketing_email-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6184 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6124 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6249 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6061 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5373 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5205 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6014 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4979 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18906 2023-07-22 21:26:26.000000 trytond_marketing_email-6.8.1/marketing.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10433 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/marketing.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      603 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-08-01 19:52:31.020811 trytond_marketing_email-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4311 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:52:31.014144 trytond_marketing_email-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5610 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-05-01 12:18:02.000000 trytond_marketing_email-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:52:31.020811 trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3636 2023-08-01 19:52:30.000000 trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1955 2023-08-01 19:52:30.000000 trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-08-01 19:52:30.000000 trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-08-01 19:52:30.000000 trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:21.000000 trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      137 2023-08-01 19:52:30.000000 trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-08-01 19:52:30.000000 trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:52:31.017477 trytond_marketing_email-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/view/email_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/view/email_list_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1066 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/view/email_message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/view/email_message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/view/send_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-05-01 12:17:31.000000 trytond_marketing_email-6.8.1/web.py
```

### Comparing `trytond_marketing_email-6.8.0/COPYRIGHT` & `trytond_marketing_email-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/LICENSE` & `trytond_marketing_email-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/PKG-INFO` & `trytond_marketing_email-6.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_marketing_email
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module to manage marketing mailing lists
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_marketing_email-6.8.0/README.rst` & `trytond_marketing_email-6.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/__init__.py` & `trytond_marketing_email-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/doc/conf.py` & `trytond_marketing_email-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/doc/index.rst` & `trytond_marketing_email-6.8.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/email_subscribe.html` & `trytond_marketing_email-6.8.1/email_subscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/email_unsubscribe.html` & `trytond_marketing_email-6.8.1/email_unsubscribe.html`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/icons/LICENSE` & `trytond_marketing_email-6.8.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/bg.po` & `trytond_marketing_email-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/ca.po` & `trytond_marketing_email-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/cs.po` & `trytond_marketing_email-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/de.po` & `trytond_marketing_email-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/es.po` & `trytond_marketing_email-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/es_419.po` & `trytond_marketing_email-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/et.po` & `trytond_marketing_email-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/fa.po` & `trytond_marketing_email-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/fi.po` & `trytond_marketing_email-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/fr.po` & `trytond_marketing_email-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/hu.po` & `trytond_marketing_email-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/id.po` & `trytond_marketing_email-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/it.po` & `trytond_marketing_email-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/lo.po` & `trytond_marketing_email-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/lt.po` & `trytond_marketing_email-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/nl.po` & `trytond_marketing_email-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/pl.po` & `trytond_marketing_email-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/pt.po` & `trytond_marketing_email-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/ro.po` & `trytond_marketing_email-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/ru.po` & `trytond_marketing_email-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/sl.po` & `trytond_marketing_email-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/tr.po` & `trytond_marketing_email-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/uk.po` & `trytond_marketing_email-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/locale/zh_CN.po` & `trytond_marketing_email-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/marketing.py` & `trytond_marketing_email-6.8.1/marketing.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     @classmethod
     def __setup__(cls):
         super().__setup__()
 
         t = cls.__table__()
         cls._sql_constraints = [
             ('email_list_unique', Unique(t, t.email, t.list_),
-                'marketing.msg_email_list_unique'),
+                'marketing_email.msg_email_list_unique'),
             ]
         cls._sql_indexes.add(Index(
                 t,
                 (t.list_, Index.Equality()),
                 (t.email, Index.Equality())))
 
     @classmethod
@@ -131,14 +131,19 @@
             email = record.email.lower()
             if email != record.email:
                 record.email = email
         cls.save(records)
 
     @classmethod
     def create(cls, vlist):
+        vlist = [v.copy() for v in vlist]
+        for values in vlist:
+            # Ensure to get a different token for each record
+            # default methods are called only once
+            values.setdefault('email_token', cls.default_email_token())
         records = super().create(vlist)
         cls._format_email(records)
         return records
 
     @classmethod
     def write(cls, *args):
         super().write(*args)
```

### Comparing `trytond_marketing_email-6.8.0/marketing.xml` & `trytond_marketing_email-6.8.1/marketing.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/message.xml` & `trytond_marketing_email-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/setup.py` & `trytond_marketing_email-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/tests/test_module.py` & `trytond_marketing_email-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/tox.ini` & `trytond_marketing_email-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/PKG-INFO` & `trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-marketing-email
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module to manage marketing mailing lists
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_marketing_email-6.8.0/trytond_marketing_email.egg-info/SOURCES.txt` & `trytond_marketing_email-6.8.1/trytond_marketing_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_marketing_email-6.8.0/view/email_message_form.xml` & `trytond_marketing_email-6.8.1/view/email_message_form.xml`

 * *Files identical despite different names*

