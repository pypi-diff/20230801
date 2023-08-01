# Comparing `tmp/trytond_web_shop_shopify-6.8.0.tar.gz` & `tmp/trytond_web_shop_shopify-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop_shopify-6.8.0.tar", last modified: Mon May  1 11:35:59 2023, max compression
+gzip compressed data, was "trytond_web_shop_shopify-6.8.1.tar", last modified: Tue Aug  1 19:42:07 2023, max compression
```

## Comparing `trytond_web_shop_shopify-6.8.0.tar` & `trytond_web_shop_shopify-6.8.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.064897 trytond_web_shop_shopify-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      683 2023-05-01 10:57:24.000000 trytond_web_shop_shopify-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-05-01 10:57:24.000000 trytond_web_shop_shopify-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2546 2023-05-01 11:35:59.064897 trytond_web_shop_shopify-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2282 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5112 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5642 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.061563 trytond_web_shop_shopify-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.054896 trytond_web_shop_shopify-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10064 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:38.000000 trytond_web_shop_shopify-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10405 2023-04-29 08:02:38.000000 trytond_web_shop_shopify-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10110 2023-04-29 08:02:38.000000 trytond_web_shop_shopify-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:38.000000 trytond_web_shop_shopify-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10355 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7363 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7351 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10006 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-04-29 08:02:39.000000 trytond_web_shop_shopify-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4138 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4339 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21438 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      790 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17299 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:35:59.064897 trytond_web_shop_shopify-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4993 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/shopify_retry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6220 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2852 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.054896 trytond_web_shop_shopify-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20068 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/scenario_web_shop_shopify.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7234 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/scenario_web_shop_shopify_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-05-01 10:57:19.000000 trytond_web_shop_shopify-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.064897 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2546 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2742 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:35:58.000000 trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:59.058230 trytond_web_shop_shopify-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/product_attribute_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_shopify_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_shopify_identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_shopify_payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_shopify_payment_journal_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_stock_location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/shop_stock_location_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/stock_shipment_shopify_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/view/stock_shipment_shopify_identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    28233 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-6.8.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:42:07.619845 trytond_web_shop_shopify-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-08-01 19:42:02.000000 trytond_web_shop_shopify-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-08-01 19:42:02.000000 trytond_web_shop_shopify-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2546 2023-08-01 19:42:07.616511 trytond_web_shop_shopify-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2282 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5112 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5642 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:42:07.613178 trytond_web_shop_shopify-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:42:07.606511 trytond_web_shop_shopify-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10064 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10405 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10110 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10355 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7363 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7351 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10006 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4138 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4339 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21434 2023-07-03 21:16:51.000000 trytond_web_shop_shopify-6.8.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      790 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17299 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-08-01 19:42:07.619845 trytond_web_shop_shopify-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4993 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/shopify_retry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6220 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2852 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:42:07.609845 trytond_web_shop_shopify-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20068 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/tests/scenario_web_shop_shopify.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7234 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/tests/scenario_web_shop_shopify_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-05-01 12:18:02.000000 trytond_web_shop_shopify-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:42:07.616511 trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2546 2023-08-01 19:42:06.000000 trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2742 2023-08-01 19:42:07.000000 trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-08-01 19:42:06.000000 trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-08-01 19:42:06.000000 trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:15.000000 trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2023-08-01 19:42:06.000000 trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-08-01 19:42:06.000000 trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-08-01 19:42:07.613178 trytond_web_shop_shopify-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/product_attribute_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/shop_shopify_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/shop_shopify_identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/shop_shopify_payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/shop_shopify_payment_journal_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/shop_stock_location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/shop_stock_location_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/stock_shipment_shopify_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/view/stock_shipment_shopify_identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    28233 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-05-01 12:17:32.000000 trytond_web_shop_shopify-6.8.1/web.xml
```

### Comparing `trytond_web_shop_shopify-6.8.0/CHANGELOG` & `trytond_web_shop_shopify-6.8.1/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 6.8.1 - 2023-08-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.7
 * Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
```

### Comparing `trytond_web_shop_shopify-6.8.0/COPYRIGHT` & `trytond_web_shop_shopify-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/LICENSE` & `trytond_web_shop_shopify-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/PKG-INFO` & `trytond_web_shop_shopify-6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_shopify
-Version: 6.8.0
+Version: 6.8.1
 Summary: Module to integrate Tryton with Shopify
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_shop_shopify-6.8.0/__init__.py` & `trytond_web_shop_shopify-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/account.py` & `trytond_web_shop_shopify-6.8.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/common.py` & `trytond_web_shop_shopify-6.8.1/common.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/doc/conf.py` & `trytond_web_shop_shopify-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/doc/design.rst` & `trytond_web_shop_shopify-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/doc/usage.rst` & `trytond_web_shop_shopify-6.8.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/ir.py` & `trytond_web_shop_shopify-6.8.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/ir.xml` & `trytond_web_shop_shopify-6.8.1/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/bg.po` & `trytond_web_shop_shopify-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/ca.po` & `trytond_web_shop_shopify-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/cs.po` & `trytond_web_shop_shopify-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/de.po` & `trytond_web_shop_shopify-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/es.po` & `trytond_web_shop_shopify-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/es_419.po` & `trytond_web_shop_shopify-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/et.po` & `trytond_web_shop_shopify-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/fa.po` & `trytond_web_shop_shopify-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/fi.po` & `trytond_web_shop_shopify-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/fr.po` & `trytond_web_shop_shopify-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/hu.po` & `trytond_web_shop_shopify-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/id.po` & `trytond_web_shop_shopify-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/it.po` & `trytond_web_shop_shopify-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/lo.po` & `trytond_web_shop_shopify-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/lt.po` & `trytond_web_shop_shopify-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/nl.po` & `trytond_web_shop_shopify-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/pl.po` & `trytond_web_shop_shopify-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/pt.po` & `trytond_web_shop_shopify-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/ro.po` & `trytond_web_shop_shopify-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/ru.po` & `trytond_web_shop_shopify-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/sl.po` & `trytond_web_shop_shopify-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/tr.po` & `trytond_web_shop_shopify-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/uk.po` & `trytond_web_shop_shopify-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/locale/zh_CN.po` & `trytond_web_shop_shopify-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/message.xml` & `trytond_web_shop_shopify-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/party.py` & `trytond_web_shop_shopify-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/product.py` & `trytond_web_shop_shopify-6.8.1/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,15 +608,15 @@
 
 
 class Image_Attribute(metaclass=PoolMeta):
     __name__ = 'product.image'
 
     @property
     def shopify_name(self):
-        name = super().shopify_filename
+        name = super().shopify_name
         if self.product:
             attributes_name = self.product.attributes_name
         else:
             attributes_name = self.attributes_name
         if attributes_name:
             name += ' ' + attributes_name
         return name
```

### Comparing `trytond_web_shop_shopify-6.8.0/product.xml` & `trytond_web_shop_shopify-6.8.1/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/routes.py` & `trytond_web_shop_shopify-6.8.1/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/sale.py` & `trytond_web_shop_shopify-6.8.1/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/setup.py` & `trytond_web_shop_shopify-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/shopify_retry.py` & `trytond_web_shop_shopify-6.8.1/shopify_retry.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/stock.py` & `trytond_web_shop_shopify-6.8.1/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/stock.xml` & `trytond_web_shop_shopify-6.8.1/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/tests/scenario_web_shop_shopify.rst` & `trytond_web_shop_shopify-6.8.1/tests/scenario_web_shop_shopify.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/tests/scenario_web_shop_shopify_secondary_unit.rst` & `trytond_web_shop_shopify-6.8.1/tests/scenario_web_shop_shopify_secondary_unit.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/tox.ini` & `trytond_web_shop_shopify-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/PKG-INFO` & `trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-web-shop-shopify
-Version: 6.8.0
+Version: 6.8.1
 Summary: Module to integrate Tryton with Shopify
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/SOURCES.txt` & `trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/trytond_web_shop_shopify.egg-info/requires.txt` & `trytond_web_shop_shopify-6.8.1/trytond_web_shop_shopify.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/view/shop_form.xml` & `trytond_web_shop_shopify-6.8.1/view/shop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/web.py` & `trytond_web_shop_shopify-6.8.1/web.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-6.8.0/web.xml` & `trytond_web_shop_shopify-6.8.1/web.xml`

 * *Files identical despite different names*

