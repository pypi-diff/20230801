# Comparing `tmp/odoo14-addon-energy_project-14.0.1.1.1.tar.gz` & `tmp/odoo14-addon-energy_project-14.0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_project-14.0.1.1.1.tar", last modified: Wed Jun 14 09:34:40 2023, max compression
+gzip compressed data, was "odoo14-addon-energy_project-14.0.1.1.2.tar", last modified: Tue Aug  1 07:43:56 2023, max compression
```

## Comparing `odoo14-addon-energy_project-14.0.1.1.1.tar` & `odoo14-addon-energy_project-14.0.1.1.2.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.541595 odoo14-addon-energy_project-14.0.1.1.1/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      398 2023-06-14 09:34:40.541595 odoo14-addon-energy_project-14.0.1.1.1/PKG-INFO
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.537595 odoo14-addon-energy_project-14.0.1.1.1/odoo/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.537595 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.537595 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       21 2023-05-19 10:06:31.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      547 2023-06-14 09:33:54.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/__manifest__.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.537595 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     7521 2023-05-30 07:52:25.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/ca_ES.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     7056 2023-05-16 16:06:50.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/energy_project.pot
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     7545 2023-05-30 07:52:25.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/es.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     7538 2023-05-30 07:52:25.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/eu_ES.po
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.537595 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/models/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       75 2023-05-16 12:14:37.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/models/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      859 2023-05-16 12:14:37.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/models/inscription.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1237 2023-05-16 12:14:37.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/models/project.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      193 2023-05-16 12:14:37.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/models/project_type.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.537595 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/security/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      806 2023-05-16 12:14:37.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/security/ir.model.access.csv
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      439 2023-05-19 10:06:31.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/security/ir_rule_data.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      549 2023-05-16 12:14:37.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/security/res_groups.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.537595 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/static/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.537595 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/static/description/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3721 2023-05-16 12:14:37.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/static/description/icon.png
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:34:40.541595 odoo14-addon-energy_project-14.0.1.1.1/odoo14_addon_energy_project.egg-info/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      398 2023-06-14 09:34:40.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo14_addon_energy_project.egg-info/PKG-INFO
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      970 2023-06-14 09:34:40.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo14_addon_energy_project.egg-info/SOURCES.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 09:34:40.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo14_addon_energy_project.egg-info/dependency_links.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 09:34:40.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo14_addon_energy_project.egg-info/not-zip-safe
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       21 2023-06-14 09:34:40.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo14_addon_energy_project.egg-info/requires.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        5 2023-06-14 09:34:40.000000 odoo14-addon-energy_project-14.0.1.1.1/odoo14_addon_energy_project.egg-info/top_level.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       38 2023-06-14 09:34:40.541595 odoo14-addon-energy_project-14.0.1.1.1/setup.cfg
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      100 2023-05-16 12:14:37.000000 odoo14-addon-energy_project-14.0.1.1.1/setup.py
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.009990 odoo14-addon-energy_project-14.0.1.1.2/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      461 2023-08-01 07:43:56.009990 odoo14-addon-energy_project-14.0.1.1.2/PKG-INFO
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.005990 odoo14-addon-energy_project-14.0.1.1.2/odoo/
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.005990 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.005990 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)       21 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/__init__.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      586 2023-08-01 07:39:31.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/__manifest__.py
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.005990 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     7521 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/ca_ES.po
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     7056 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/energy_project.pot
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     7545 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/es.po
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     7538 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/eu_ES.po
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.005990 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/models/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)       75 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/models/__init__.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      859 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/models/inscription.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     1278 2023-07-28 09:57:25.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/models/project.py
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      193 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/models/project_type.py
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.009990 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/security/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      806 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/security/ir.model.access.csv
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      439 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/security/ir_rule_data.xml
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      549 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/security/res_groups.xml
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.005990 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/static/
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.009990 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/static/description/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     3721 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/static/description/icon.png
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.009990 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/views/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      570 2023-07-28 09:57:25.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/views/inscription_views.xml
+drwxrwxr-x   0 benjami   (1000) benjami   (1000)        0 2023-08-01 07:43:56.009990 odoo14-addon-energy_project-14.0.1.1.2/odoo14_addon_energy_project.egg-info/
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      461 2023-08-01 07:43:55.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo14_addon_energy_project.egg-info/PKG-INFO
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)     1025 2023-08-01 07:43:55.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo14_addon_energy_project.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)        1 2023-08-01 07:43:55.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo14_addon_energy_project.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)        1 2023-08-01 07:43:55.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo14_addon_energy_project.egg-info/not-zip-safe
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)       21 2023-08-01 07:43:55.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo14_addon_energy_project.egg-info/requires.txt
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)        5 2023-08-01 07:43:55.000000 odoo14-addon-energy_project-14.0.1.1.2/odoo14_addon_energy_project.egg-info/top_level.txt
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)       38 2023-08-01 07:43:56.009990 odoo14-addon-energy_project-14.0.1.1.2/setup.cfg
+-rw-rw-r--   0 benjami   (1000) benjami   (1000)      100 2023-07-05 09:12:08.000000 odoo14-addon-energy_project-14.0.1.1.2/setup.py
```

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/__manifest__.py` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/__manifest__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,19 @@
         """,
     "description": """
             Base module for energetic projects.
     """,
     "author": "Coopdevs Treball SCCL & Som Energia SCCL",
     "website": "https://somcomunitats.coop/",
     "category": "Customizations",
-    "version": "14.0.1.1.1",
+    "version": "14.0.1.1.2",
     "depends": [
         "base",
         "mail",
     ],
     "data": [
         "security/res_groups.xml",
         "security/ir.model.access.csv",
         "security/ir_rule_data.xml",
+        "views/inscription_views.xml",
     ],
 }
```

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/ca_ES.po` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/ca_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/energy_project.pot` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/energy_project.pot`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/es.po` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/i18n/eu_ES.po` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/i18n/eu_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/models/inscription.py` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/models/inscription.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/models/project.py` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/models/project.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,20 +20,21 @@
     inscription_ids = fields.One2many(
         "energy_project.inscription", "project_id", required=True
     )
     active = fields.Boolean(default=True)
 
     # address fields
     street = fields.Char(required=True)
-    street2 = fields.Char(required=True)
+    street2 = fields.Char()
     zip = fields.Char(change_default=True, required=True)
     city = fields.Char(required=True)
     state_id = fields.Many2one(
         "res.country.state",
         string="State",
         ondelete="restrict",
         domain="[('country_id', '=?', country_id)]",
         required=True,
     )
     country_id = fields.Many2one(
-        "res.country", string="Country", ondelete="restrict", required=True
+        "res.country", string="Country", ondelete="restrict", required=True,
+        default=lambda self: self.env.ref('base.es')
     )
```

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/security/ir.model.access.csv` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/security/res_groups.xml` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/security/res_groups.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo/addons/energy_project/static/description/icon.png` & `odoo14-addon-energy_project-14.0.1.1.2/odoo/addons/energy_project/static/description/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_project-14.0.1.1.1/odoo14_addon_energy_project.egg-info/SOURCES.txt` & `odoo14-addon-energy_project-14.0.1.1.2/odoo14_addon_energy_project.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 odoo/addons/energy_project/models/inscription.py
 odoo/addons/energy_project/models/project.py
 odoo/addons/energy_project/models/project_type.py
 odoo/addons/energy_project/security/ir.model.access.csv
 odoo/addons/energy_project/security/ir_rule_data.xml
 odoo/addons/energy_project/security/res_groups.xml
 odoo/addons/energy_project/static/description/icon.png
+odoo/addons/energy_project/views/inscription_views.xml
 odoo14_addon_energy_project.egg-info/PKG-INFO
 odoo14_addon_energy_project.egg-info/SOURCES.txt
 odoo14_addon_energy_project.egg-info/dependency_links.txt
 odoo14_addon_energy_project.egg-info/not-zip-safe
 odoo14_addon_energy_project.egg-info/requires.txt
 odoo14_addon_energy_project.egg-info/top_level.txt
```

