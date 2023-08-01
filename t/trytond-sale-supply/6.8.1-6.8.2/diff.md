# Comparing `tmp/trytond_sale_supply-6.8.1.tar.gz` & `tmp/trytond_sale_supply-6.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply-6.8.1.tar", last modified: Wed Jun 21 17:14:33 2023, max compression
+gzip compressed data, was "trytond_sale_supply-6.8.2.tar", last modified: Tue Aug  1 19:48:41 2023, max compression
```

## Comparing `trytond_sale_supply-6.8.1.tar` & `trytond_sale_supply-6.8.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.143788 trytond_sale_supply-6.8.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2204 2023-06-21 17:14:30.000000 trytond_sale_supply-6.8.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-06-21 17:14:29.000000 trytond_sale_supply-6.8.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-06-21 17:14:33.143788 trytond_sale_supply-6.8.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.140454 trytond_sale_supply-6.8.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.137121 trytond_sale_supply-6.8.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1885 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1898 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1743 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1906 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1601 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1553 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1684 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1809 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1852 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1628 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1711 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1699 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1728 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1596 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3438 2023-06-10 09:48:45.000000 trytond_sale_supply-6.8.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3494 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11814 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:14:33.143788 trytond_sale_supply-6.8.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4391 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2873 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.140454 trytond_sale_supply-6.8.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7845 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/scenario_sale_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1550 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/scenario_sale_supply_notifications.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3849 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/scenario_sale_supply_shipment_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3356 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/scenario_sale_supply_stock_first.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      174 2023-05-01 12:18:02.000000 trytond_sale_supply-6.8.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.143788 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1867 2023-06-21 17:14:33.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:18.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:14:32.000000 trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:14:33.140454 trytond_sale_supply-6.8.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.1/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:48:41.741337 trytond_sale_supply-6.8.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2305 2023-08-01 19:48:37.000000 trytond_sale_supply-6.8.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-08-01 19:48:37.000000 trytond_sale_supply-6.8.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-08-01 19:48:41.741337 trytond_sale_supply-6.8.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:48:41.738004 trytond_sale_supply-6.8.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:48:41.734670 trytond_sale_supply-6.8.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1885 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1898 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1743 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1906 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1601 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1553 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1684 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1809 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1852 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1628 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1711 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1699 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1728 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2023-07-22 21:31:37.000000 trytond_sale_supply-6.8.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3494 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11814 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-08-01 19:48:41.741337 trytond_sale_supply-6.8.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4391 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2873 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:48:41.734670 trytond_sale_supply-6.8.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7845 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/tests/scenario_sale_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1550 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/tests/scenario_sale_supply_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3849 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/tests/scenario_sale_supply_shipment_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3356 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/tests/scenario_sale_supply_stock_first.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      174 2023-06-21 17:14:42.000000 trytond_sale_supply-6.8.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:48:41.741337 trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2825 2023-08-01 19:48:40.000000 trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1867 2023-08-01 19:48:41.000000 trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-08-01 19:48:40.000000 trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-08-01 19:48:40.000000 trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:18.000000 trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-08-01 19:48:40.000000 trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-08-01 19:48:40.000000 trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:48:41.738004 trytond_sale_supply-6.8.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-05-01 12:17:31.000000 trytond_sale_supply-6.8.2/view/template_form.xml
```

### Comparing `trytond_sale_supply-6.8.1/CHANGELOG` & `trytond_sale_supply-6.8.2/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_sale_supply-6.8.1/COPYRIGHT` & `trytond_sale_supply-6.8.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/LICENSE` & `trytond_sale_supply-6.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/PKG-INFO` & `trytond_sale_supply-6.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply
-Version: 6.8.1
+Version: 6.8.2
 Summary: Tryton module for sale supply
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_supply-6.8.1/README.rst` & `trytond_sale_supply-6.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/__init__.py` & `trytond_sale_supply-6.8.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/doc/conf.py` & `trytond_sale_supply-6.8.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/doc/index.rst` & `trytond_sale_supply-6.8.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/bg.po` & `trytond_sale_supply-6.8.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/ca.po` & `trytond_sale_supply-6.8.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/cs.po` & `trytond_sale_supply-6.8.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/de.po` & `trytond_sale_supply-6.8.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/es.po` & `trytond_sale_supply-6.8.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/es_419.po` & `trytond_sale_supply-6.8.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/et.po` & `trytond_sale_supply-6.8.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/fa.po` & `trytond_sale_supply-6.8.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/fi.po` & `trytond_sale_supply-6.8.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/fr.po` & `trytond_sale_supply-6.8.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/hu.po` & `trytond_sale_supply-6.8.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/id.po` & `trytond_sale_supply-6.8.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/it.po` & `trytond_sale_supply-6.8.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/lo.po` & `trytond_sale_supply-6.8.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/lt.po` & `trytond_sale_supply-6.8.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/nl.po` & `trytond_sale_supply-6.8.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/pl.po` & `trytond_sale_supply-6.8.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/pt.po` & `trytond_sale_supply-6.8.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/ro.po` & `trytond_sale_supply-6.8.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/ru.po` & `trytond_sale_supply-6.8.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/sl.po` & `trytond_sale_supply-6.8.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/tr.po` & `trytond_sale_supply-6.8.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/uk.po` & `trytond_sale_supply-6.8.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/locale/zh_CN.po` & `trytond_sale_supply-6.8.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/message.xml` & `trytond_sale_supply-6.8.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/product.py` & `trytond_sale_supply-6.8.2/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         migrate_supply_on_sale = (
             table_h.column_exist('supply_on_sale')
             and table_h.column_is_type('supply_on_sale', 'BOOL'))
         if migrate_supply_on_sale:
             table_h.column_rename('supply_on_sale', '_temp_supply_on_sale')
         if cls._history:
             h_table_h = cls.__table_handler__(module, history=True)
-            h_table = cls.__table__()
+            h_table = cls.__table_history__()
             h_migrate_supply_on_sale = (
                 h_table_h.column_exist('supply_on_sale')
                 and h_table_h.column_is_type('supply_on_sale', 'BOOL'))
             if h_migrate_supply_on_sale:
                 h_table_h.column_rename(
                     'supply_on_sale', '_temp_supply_on_sale')
```

### Comparing `trytond_sale_supply-6.8.1/purchase.py` & `trytond_sale_supply-6.8.2/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/sale.py` & `trytond_sale_supply-6.8.2/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/sale.xml` & `trytond_sale_supply-6.8.2/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/setup.py` & `trytond_sale_supply-6.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/stock.py` & `trytond_sale_supply-6.8.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/tests/scenario_sale_supply.rst` & `trytond_sale_supply-6.8.2/tests/scenario_sale_supply.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/tests/scenario_sale_supply_notifications.rst` & `trytond_sale_supply-6.8.2/tests/scenario_sale_supply_notifications.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/tests/scenario_sale_supply_shipment_on_invoice.rst` & `trytond_sale_supply-6.8.2/tests/scenario_sale_supply_shipment_on_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/tests/scenario_sale_supply_stock_first.rst` & `trytond_sale_supply-6.8.2/tests/scenario_sale_supply_stock_first.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/tox.ini` & `trytond_sale_supply-6.8.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/PKG-INFO` & `trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-sale-supply
-Version: 6.8.1
+Version: 6.8.2
 Summary: Tryton module for sale supply
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale_supply-6.8.1/trytond_sale_supply.egg-info/SOURCES.txt` & `trytond_sale_supply-6.8.2/trytond_sale_supply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

