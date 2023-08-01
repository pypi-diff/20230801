# Comparing `tmp/odoo14-addon-energy_selfconsumption-14.0.1.1.1.tar.gz` & `tmp/odoo14-addon-energy_selfconsumption-14.0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_selfconsumption-14.0.1.1.1.tar", last modified: Wed Jun 14 09:42:16 2023, max compression
+gzip compressed data, was "odoo14-addon-energy_selfconsumption-14.0.1.1.2.tar", last modified: Tue Aug  1 07:50:43 2023, max compression
```

## Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1.tar` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.862158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      426 2023-06-14 09:42:16.862158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/PKG-INFO
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.854158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.854158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.858158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       21 2023-06-14 08:16:02.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      869 2023-06-14 09:38:27.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/__manifest__.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.858158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/data/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      507 2023-06-12 15:44:22.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/data/ir_sequence_data.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      247 2023-05-16 12:14:37.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/data/project_type_data.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.858158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    34646 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/ca_ES.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    32006 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/energy_selfconsumption.pot
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    34700 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/es.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    34485 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/eu_ES.po
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.858158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      151 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2431 2023-06-12 15:44:22.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/distribution_table.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      864 2023-06-12 15:44:22.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/partner.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2066 2023-06-14 08:16:02.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/selfconsumption.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1195 2023-05-30 09:24:38.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/supply_point.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2312 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/supply_point_assignation.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.858158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/security/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1535 2023-06-14 08:16:02.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/security/ir.model.access.csv
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1461 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/security/ir_rule_data.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.858158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/static/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.858158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/static/description/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3721 2023-05-16 12:14:37.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/static/description/icon.png
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.862158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     5349 2023-06-12 15:44:22.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/distribution_table_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1597 2023-06-12 15:44:22.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/res_partner_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     8495 2023-06-14 08:16:02.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1770 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/supply_point_assignation_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     4057 2023-06-12 15:44:22.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/supply_point_views.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:42:16.862158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo14_addon_energy_selfconsumption.egg-info/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      426 2023-06-14 09:42:16.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo14_addon_energy_selfconsumption.egg-info/PKG-INFO
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1680 2023-06-14 09:42:16.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo14_addon_energy_selfconsumption.egg-info/SOURCES.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 09:42:16.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo14_addon_energy_selfconsumption.egg-info/dependency_links.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 09:42:16.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo14_addon_energy_selfconsumption.egg-info/not-zip-safe
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       61 2023-06-14 09:42:16.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo14_addon_energy_selfconsumption.egg-info/requires.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        5 2023-06-14 09:42:16.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo14_addon_energy_selfconsumption.egg-info/top_level.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       38 2023-06-14 09:42:16.862158 odoo14-addon-energy_selfconsumption-14.0.1.1.1/setup.cfg
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      215 2023-06-14 09:41:48.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.1/setup.py
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.352609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      489 2023-08-01 07:50:43.352609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/PKG-INFO
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.344609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.344609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.348609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)       21 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/__init__.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      869 2023-08-01 07:48:31.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/__manifest__.py
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.348609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/data/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      507 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/data/ir_sequence_data.xml
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      247 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/data/project_type_data.xml
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.348609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)    34646 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/ca_ES.po
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)    32006 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/energy_selfconsumption.pot
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)    34700 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/es.po
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)    34485 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/eu_ES.po
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.348609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      151 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/__init__.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     2431 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/distribution_table.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      864 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/partner.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     3093 2023-07-28 09:57:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/selfconsumption.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     1195 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/supply_point.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     2606 2023-07-28 09:57:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/supply_point_assignation.py
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.348609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/security/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     1535 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/security/ir.model.access.csv
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     1461 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/security/ir_rule_data.xml
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.344609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/static/
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.348609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/static/description/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     2758 2023-07-28 09:57:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/static/description/icon.png
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.352609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     5349 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/distribution_table_views.xml
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     1597 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/res_partner_views.xml
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     8763 2023-07-28 09:57:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     1770 2023-07-05 09:12:08.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/supply_point_assignation_views.xml
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     4809 2023-07-28 09:57:25.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/supply_point_views.xml
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:50:43.352609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo14_addon_energy_selfconsumption.egg-info/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      489 2023-08-01 07:50:43.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo14_addon_energy_selfconsumption.egg-info/PKG-INFO
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     1680 2023-08-01 07:50:43.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo14_addon_energy_selfconsumption.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)        1 2023-08-01 07:50:43.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo14_addon_energy_selfconsumption.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)        1 2023-08-01 07:50:43.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo14_addon_energy_selfconsumption.egg-info/not-zip-safe
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)       61 2023-08-01 07:50:43.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo14_addon_energy_selfconsumption.egg-info/requires.txt
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)        5 2023-08-01 07:50:43.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo14_addon_energy_selfconsumption.egg-info/top_level.txt
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)       38 2023-08-01 07:50:43.352609 odoo14-addon-energy_selfconsumption-14.0.1.1.2/setup.cfg
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      215 2023-08-01 07:47:06.000000 odoo14-addon-energy_selfconsumption-14.0.1.1.2/setup.py
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/__manifest__.py` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         """,
     "description": """
         Module for energetic self-consumption projects.
     """,
     "author": "Coopdevs Treball SCCL & Som Energia SCCL",
     "website": "https://somcomunitats.coop/",
     "category": "Customizations",
-    "version": "14.0.1.1.1",
+    "version": "14.0.1.1.2",
     "depends": [
         "base",
         "mail",
         "energy_project",
     ],
     "data": [
         "security/ir.model.access.csv",
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/ca_ES.po` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/ca_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/energy_selfconsumption.pot` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/energy_selfconsumption.pot`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/es.po` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/i18n/eu_ES.po` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/i18n/eu_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/distribution_table.py` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/distribution_table.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/partner.py` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/partner.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/selfconsumption.py` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/selfconsumption.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,40 +10,61 @@
     }
     _description = "Self-consumption Energy Project"
 
     def _compute_distribution_table_count(self):
         for record in self:
             record.distribution_table_count = len(record.distribution_table_ids)
 
+    def _compute_inscription_count(self):
+        for record in self:
+            record.inscription_count = len(record.inscription_ids)
+
     project_id = fields.Many2one(
         "energy_project.project", required=True, ondelete="cascade"
     )
     code = fields.Char(string="CAU")
-    power = fields.Float(string="Generation Power (kWh)")
+    cil = fields.Char(string="CIL", help="Production facility code for liquidation purposes")
+    owner_id = fields.Many2one("res.partner", string="Owner", required=True, default=lambda self: self.env.company.partner_id)
+    power = fields.Float(string="Generation Power (kW)")
     distribution_table_ids = fields.One2many('energy_selfconsumption.distribution_table', 'selfconsumption_project_id',
                                              readonly=True)
-    distribution_table_count = fields.Integer(compute=_compute_distribution_table_count)
+    distribution_table_count = fields.Integer(compute=_compute_distribution_table_count) 
+    inscription_ids = fields.One2many('energy_project.inscription', 'project_id', readonly=True)
+    inscription_count = fields.Integer(compute=_compute_inscription_count)
 
     def get_distribution_tables(self):
         self.ensure_one()
         return {
             'type': 'ir.actions.act_window',
             'name': 'Distribution Tables',
             'view_mode': 'tree,form',
             'res_model': 'energy_selfconsumption.distribution_table',
             'domain': [('selfconsumption_project_id', '=', self.id)],
             'context': {'create': True, 'default_selfconsumption_project_id': self.id},
         }
+    
+    def get_inscriptions(self):
+        self.ensure_one()
+        return {
+            'type': 'ir.actions.act_window',
+            'name': 'Inscriptions',
+            'view_mode': 'tree,form',
+            'res_model': 'energy_project.inscription',
+            'domain': [('project_id', '=', self.id)],
+            'context': {'create': True, 'default_project_id': self.id},
+        }
 
     def set_activation(self):
         for record in self:
             record.write({"state": "activation"})
 
     def activate(self):
         for record in self:
             if not record.code:
                 raise ValidationError(_("Project must have a valid Code."))
+            if not record.cil:
+                raise ValidationError(_("Project must have a valid CIL."))
             if not record.power or record.power <= 0:
                 raise ValidationError(_("Project must have a valid Generation Power."))
             if not record.distribution_table_ids.filtered_domain([('state', '=', 'validated')]):
                 raise ValidationError(_("Must have a valid Distribution Table."))
             record.write({"state": "active"})
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/supply_point.py` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/supply_point.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/models/supply_point_assignation.py` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/models/supply_point_assignation.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         for record in self:
             record.supply_point_filtered_ids = \
                 record.distribution_table_id.selfconsumption_project_id.inscription_ids.mapped('partner_id.supply_ids') \
                     .filtered_domain([('id', 'not in', record.distribution_table_id.supply_point_assignation_ids.mapped(
                     'supply_point_id.id'))])
 
     distribution_table_id = fields.Many2one('energy_selfconsumption.distribution_table', required=True)
+    selfconsumption_project_id = fields.Many2one(related='distribution_table_id.selfconsumption_project_id')
+    distribution_table_state = fields.Selection(related='distribution_table_id.state')
+    distribution_table_create_date = fields.Datetime(related='distribution_table_id.create_date')
     supply_point_id = fields.Many2one('energy_selfconsumption.supply_point', required=True)
     coefficient = fields.Float(string='Distribution coefficient', digits=(1, 5), required=True,
                                help="The sum of all the coefficients must result in 1")
     owner_id = fields.Many2one("res.partner", related='supply_point_id.owner_id')
     code = fields.Char(related='supply_point_id.code')
     table_coefficient_is_valid = fields.Boolean(related='distribution_table_id.coefficient_is_valid')
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/security/ir.model.access.csv` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/security/ir_rule_data.xml` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/security/ir_rule_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/distribution_table_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/distribution_table_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/res_partner_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/res_partner_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml`

 * *Files 3% similar despite different names*

#### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/selfconsumption_views.xml`

```diff
@@ -9,14 +9,17 @@
           <header>
             <button type="object" string="Set in activation" name="set_activation" attrs="{'invisible':[('state','not in',['draft'])]}"/>
             <button type="object" string="Activate" name="activate" attrs="{'invisible':[('state','not in',['activation'])]}"/>
             <field name="state" widget="statusbar" readonly="True" statusbar_visible="draft,activation,active"/>
           </header>
           <sheet>
             <div class="oe_button_box" name="button_box">
+              <button class="oe_stat_button" type="object" name="get_inscriptions" icon="fa-pencil-square-o" context="{'default_effective_date': today}">
+                <field string="Inscriptions" name="inscription_count" widget="statinfo"/>
+              </button>
               <button class="oe_stat_button" type="object" name="get_distribution_tables" icon="fa-table" context="{'default_owner_id': id}" attrs="{'invisible': [('state', '==', 'draft')]}">
                 <field string="Distribution Tables" name="distribution_table_count" widget="statinfo"/>
               </button>
             </div>
             <widget name="web_ribbon" text="Archived" bg_color="bg-danger" attrs="{'invisible': [('active', '=', True)]}"/>
             <field name="active" invisible="True"/>
             <div class="oe_title">
@@ -27,15 +30,17 @@
             </div>
             <group>
               <group>
                 <field name="company_id" invisible="True"/>
                 <field name="id" invisible="True"/>
                 <field name="type" invisible="True"/>
                 <field name="code" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
+                <field name="cil" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
                 <field name="power" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
+                <field name="owner_id" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
               </group>
               <group>
                 <span class="o_form_label o_td_label" name="address_name">
                   <b>Address</b>
                 </span>
                 <div class="o_address_format">
                   <field name="street" placeholder="Street..." class="o_address_street" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
@@ -43,22 +48,14 @@
                   <field name="city" placeholder="City" class="o_address_city" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
                   <field name="state_id" class="o_address_state" placeholder="State" options="{'no_open': True, 'no_quick_create': True}" context="{'country_id': country_id, 'default_country_id': country_id, 'zip': zip}" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
                   <field name="zip" placeholder="ZIP" class="o_address_zip" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
                   <field name="country_id" placeholder="Country" class="o_address_country" options="{&quot;no_open&quot;: True, &quot;no_create&quot;: True}" attrs="{'readonly': [('state', 'not in', ['draft', 'activation'])]}"/>
                 </div>
               </group>
             </group>
-            <group>
-              <field name="inscription_ids" widget="one2many" mode="list" context="{'default_project_id':id, 'default_effective_date': today}">
-                <tree editable="bottom">
-                  <field name="partner_id" options="{'no_create': True}"/>
-                  <field name="effective_date"/>
-                </tree>
-              </field>
-            </group>
           </sheet>
           <div class="oe_chatter">
             <field name="message_follower_ids" widget="mail_followers"/>
             <field name="activity_ids" widget="mail_activity"/>
             <field name="message_ids" widget="mail_thread"/>
           </div>
         </form>
@@ -66,14 +63,20 @@
     </record>
     <record id="selfconsumption_tree_view" model="ir.ui.view">
       <field name="name">energy_selfconsumption.selfconsumption.tree</field>
       <field name="model">energy_selfconsumption.selfconsumption</field>
       <field name="arch" type="xml">
         <tree string="Self-Consumption Projects">
           <field name="name"/>
+          <field name="street"/>
+          <field name="street2"/>
+          <field name="state_id"/>
+          <field name="zip"/>
+          <field name="country_id"/>
+          <field name="power"/>
           <field name="state"/>
         </tree>
       </field>
     </record>
     <record id="selfconsumption_form_view_act_window" model="ir.actions.act_window">
       <field name="name">Self-consumption Project</field>
       <field name="type">ir.actions.act_window</field>
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/supply_point_assignation_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/supply_point_assignation_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/supply_point_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/supply_point_views.xml`

 * *Files 10% similar despite different names*

#### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo/addons/energy_selfconsumption/views/supply_point_views.xml` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo/addons/energy_selfconsumption/views/supply_point_views.xml`

```diff
@@ -28,14 +28,25 @@
                   <field name="city" placeholder="City" class="o_address_city"/>
                   <field name="state_id" class="o_address_state" placeholder="State" options="{'no_open': True, 'no_quick_create': True}" context="{'country_id': country_id, 'default_country_id': country_id, 'zip': zip}"/>
                   <field name="zip" placeholder="ZIP" class="o_address_zip"/>
                   <field name="country_id" placeholder="Country" class="o_address_country" options="{&quot;no_open&quot;: True, &quot;no_create&quot;: True}"/>
                 </div>
               </group>
             </group>
+            <notebook>
+              <page string="Self-consumption Projects" name="selfconsumption_project" autofocus="autofocus">
+                <field name="supply_point_assignation_ids">
+                  <tree default_order="distribution_table_create_date desc">
+                    <field name="selfconsumption_project_id" string="Name"/>
+                    <field name="distribution_table_state"/>
+                    <field name="distribution_table_create_date"/>
+                  </tree>
+                </field>
+              </page>
+            </notebook>
           </sheet>
           <div class="oe_chatter">
             <field name="message_follower_ids" widget="mail_followers"/>
             <field name="activity_ids" widget="mail_activity"/>
             <field name="message_ids" widget="mail_thread"/>
           </div>
         </form>
```

### Comparing `odoo14-addon-energy_selfconsumption-14.0.1.1.1/odoo14_addon_energy_selfconsumption.egg-info/SOURCES.txt` & `odoo14-addon-energy_selfconsumption-14.0.1.1.2/odoo14_addon_energy_selfconsumption.egg-info/SOURCES.txt`

 * *Files identical despite different names*

