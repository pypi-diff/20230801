# Comparing `tmp/trytond_sale_point-6.8.1.tar.gz` & `tmp/trytond_sale_point-6.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_point-6.8.1.tar", last modified: Wed Jun 21 17:15:09 2023, max compression
+gzip compressed data, was "trytond_sale_point-6.8.2.tar", last modified: Tue Aug  1 19:50:02 2023, max compression
```

## Comparing `trytond_sale_point-6.8.1.tar` & `trytond_sale_point-6.8.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:15:09.640950 trytond_sale_point-6.8.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-06-21 17:15:06.000000 trytond_sale_point-6.8.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-06-21 17:15:06.000000 trytond_sale_point-6.8.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-06-21 17:15:09.637617 trytond_sale_point-6.8.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:15:09.627617 trytond_sale_point-6.8.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4049 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:15:09.517615 trytond_sale_point-6.8.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17178 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17597 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17215 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17446 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14479 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14154 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17042 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2741 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1870 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    45308 2023-06-10 09:38:21.000000 trytond_sale_point-6.8.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24915 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1996 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:15:09.640950 trytond_sale_point-6.8.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:15:09.544283 trytond_sale_point-6.8.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5832 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tests/scenario_sale_point.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3674 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tests/scenario_sale_point_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4456 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tests/scenario_sale_point_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4996 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tests/scenario_sale_point_session.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3928 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tests/scenario_sale_point_tax_excluded.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-05-01 12:18:02.000000 trytond_sale_point-6.8.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:15:09.637617 trytond_sale_point-6.8.1/trytond_sale_point.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-06-21 17:15:08.000000 trytond_sale_point-6.8.1/trytond_sale_point.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2894 2023-06-21 17:15:09.000000 trytond_sale_point-6.8.1/trytond_sale_point.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:15:08.000000 trytond_sale_point-6.8.1/trytond_sale_point.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-06-21 17:15:08.000000 trytond_sale_point-6.8.1/trytond_sale_point.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:22.000000 trytond_sale_point-6.8.1/trytond_sale_point.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-06-21 17:15:08.000000 trytond_sale_point-6.8.1/trytond_sale_point.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:15:08.000000 trytond_sale_point-6.8.1/trytond_sale_point.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:15:09.610950 trytond_sale_point-6.8.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/cash_session_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/cash_session_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/cash_transfer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/cash_transfer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/cash_transfer_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/cash_transfer_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/payment_form_wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      276 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/payment_method_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/point_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1878 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/sale_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/sale_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.1/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:50:02.588993 trytond_sale_point-6.8.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)      759 2023-08-01 19:49:58.000000 trytond_sale_point-6.8.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-08-01 19:49:58.000000 trytond_sale_point-6.8.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-08-01 19:50:02.588993 trytond_sale_point-6.8.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      936 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:50:02.585660 trytond_sale_point-6.8.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4049 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      180 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:50:02.575660 trytond_sale_point-6.8.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17178 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17597 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17215 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17446 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14479 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14154 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17042 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14040 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2741 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1870 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    45343 2023-07-03 21:19:17.000000 trytond_sale_point-6.8.2/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24915 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1996 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-08-01 19:50:02.592327 trytond_sale_point-6.8.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:50:02.578993 trytond_sale_point-6.8.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5832 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tests/scenario_sale_point.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3674 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tests/scenario_sale_point_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4456 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tests/scenario_sale_point_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4996 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tests/scenario_sale_point_session.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3928 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tests/scenario_sale_point_tax_excluded.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      182 2023-06-21 17:15:17.000000 trytond_sale_point-6.8.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:50:02.588993 trytond_sale_point-6.8.2/trytond_sale_point.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2421 2023-08-01 19:50:01.000000 trytond_sale_point-6.8.2/trytond_sale_point.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2894 2023-08-01 19:50:02.000000 trytond_sale_point-6.8.2/trytond_sale_point.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-08-01 19:50:01.000000 trytond_sale_point-6.8.2/trytond_sale_point.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2023-08-01 19:50:01.000000 trytond_sale_point-6.8.2/trytond_sale_point.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:22.000000 trytond_sale_point-6.8.2/trytond_sale_point.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-08-01 19:50:01.000000 trytond_sale_point-6.8.2/trytond_sale_point.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-08-01 19:50:01.000000 trytond_sale_point-6.8.2/trytond_sale_point.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:50:02.585660 trytond_sale_point-6.8.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      914 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/cash_session_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/cash_session_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/cash_transfer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/cash_transfer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/cash_transfer_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/cash_transfer_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/payment_form_wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      276 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/payment_method_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/point_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1878 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/sale_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/sale_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 12:17:31.000000 trytond_sale_point-6.8.2/view/template_tree.xml
```

### Comparing `trytond_sale_point-6.8.1/CHANGELOG` & `trytond_sale_point-6.8.2/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 6.8.2 - 2023-08-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 6.8.1 - 2023-06-21
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 6.8.0 - 2023-05-01
 --------------------------
```

### Comparing `trytond_sale_point-6.8.1/COPYRIGHT` & `trytond_sale_point-6.8.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/LICENSE` & `trytond_sale_point-6.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/PKG-INFO` & `trytond_sale_point-6.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_point
-Version: 6.8.1
+Version: 6.8.2
 Summary: Tryton module for Point of Sales
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_point-6.8.1/__init__.py` & `trytond_sale_point-6.8.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/account.py` & `trytond_sale_point-6.8.2/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/doc/conf.py` & `trytond_sale_point-6.8.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/doc/design.rst` & `trytond_sale_point-6.8.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/bg.po` & `trytond_sale_point-6.8.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/ca.po` & `trytond_sale_point-6.8.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/cs.po` & `trytond_sale_point-6.8.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/de.po` & `trytond_sale_point-6.8.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/es.po` & `trytond_sale_point-6.8.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/es_419.po` & `trytond_sale_point-6.8.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/et.po` & `trytond_sale_point-6.8.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/fa.po` & `trytond_sale_point-6.8.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/fi.po` & `trytond_sale_point-6.8.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/fr.po` & `trytond_sale_point-6.8.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/hu.po` & `trytond_sale_point-6.8.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/id.po` & `trytond_sale_point-6.8.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/it.po` & `trytond_sale_point-6.8.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/lo.po` & `trytond_sale_point-6.8.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/lt.po` & `trytond_sale_point-6.8.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/nl.po` & `trytond_sale_point-6.8.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/pl.po` & `trytond_sale_point-6.8.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/pt.po` & `trytond_sale_point-6.8.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/ro.po` & `trytond_sale_point-6.8.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/ru.po` & `trytond_sale_point-6.8.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/sl.po` & `trytond_sale_point-6.8.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/tr.po` & `trytond_sale_point-6.8.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/uk.po` & `trytond_sale_point-6.8.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/locale/zh_CN.po` & `trytond_sale_point-6.8.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/message.xml` & `trytond_sale_point-6.8.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/product.py` & `trytond_sale_point-6.8.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/product.xml` & `trytond_sale_point-6.8.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/sale.py` & `trytond_sale_point-6.8.2/sale.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,14 +266,15 @@
         if default is None:
             default = {}
         else:
             default = default.copy()
         default.setdefault('employee')
         default.setdefault('number')
         default.setdefault('payments')
+        default.setdefault('move')
         return super().copy(sales, default=default)
 
     @classmethod
     def delete(cls, sales):
         for sale in sales:
             if sale.number:
                 raise AccessError(
```

### Comparing `trytond_sale_point-6.8.1/sale.xml` & `trytond_sale_point-6.8.2/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/sale_reporting.py` & `trytond_sale_point-6.8.2/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/setup.py` & `trytond_sale_point-6.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/tests/scenario_sale_point.rst` & `trytond_sale_point-6.8.2/tests/scenario_sale_point.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/tests/scenario_sale_point_reporting.rst` & `trytond_sale_point-6.8.2/tests/scenario_sale_point_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/tests/scenario_sale_point_return.rst` & `trytond_sale_point-6.8.2/tests/scenario_sale_point_return.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/tests/scenario_sale_point_session.rst` & `trytond_sale_point-6.8.2/tests/scenario_sale_point_session.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/tests/scenario_sale_point_tax_excluded.rst` & `trytond_sale_point-6.8.2/tests/scenario_sale_point_tax_excluded.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/tox.ini` & `trytond_sale_point-6.8.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/trytond_sale_point.egg-info/PKG-INFO` & `trytond_sale_point-6.8.2/trytond_sale_point.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-sale-point
-Version: 6.8.1
+Version: 6.8.2
 Summary: Tryton module for Point of Sales
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_point-6.8.1/trytond_sale_point.egg-info/SOURCES.txt` & `trytond_sale_point-6.8.2/trytond_sale_point.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/view/cash_session_form.xml` & `trytond_sale_point-6.8.2/view/cash_session_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/view/cash_transfer_form.xml` & `trytond_sale_point-6.8.2/view/cash_transfer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/view/point_form.xml` & `trytond_sale_point-6.8.2/view/point_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/view/sale_form.xml` & `trytond_sale_point-6.8.2/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_point-6.8.1/view/sale_line_form.xml` & `trytond_sale_point-6.8.2/view/sale_line_form.xml`

 * *Files identical despite different names*

