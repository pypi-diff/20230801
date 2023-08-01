# Comparing `tmp/adm-boundary-manager-0.0.4.tar.gz` & `tmp/adm-boundary-manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adm-boundary-manager-0.0.4.tar", last modified: Mon Jul 31 10:54:41 2023, max compression
+gzip compressed data, was "adm-boundary-manager-0.0.5.tar", last modified: Tue Aug  1 11:30:50 2023, max compression
```

## Comparing `adm-boundary-manager-0.0.4.tar` & `adm-boundary-manager-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.494392 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.494392 adm-boundary-manager-0.0.4/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/boundary_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.494392 adm-boundary-manager-0.0.4/adminboundarymanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20604 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.528252 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20604 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/cod_abs_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/gadm_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/generic_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0005_alter_country_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.528252 adm-boundary-manager-0.0.5/adminboundarymanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/setup.cfg
```

### Comparing `adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/SOURCES.txt` & `adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,25 +6,30 @@
 adm_boundary_manager.egg-info/SOURCES.txt
 adm_boundary_manager.egg-info/dependency_links.txt
 adm_boundary_manager.egg-info/requires.txt
 adm_boundary_manager.egg-info/top_level.txt
 adminboundarymanager/__init__.py
 adminboundarymanager/admin.py
 adminboundarymanager/apps.py
-adminboundarymanager/boundary_loader.py
 adminboundarymanager/countries.py
 adminboundarymanager/errors.py
 adminboundarymanager/forms.py
 adminboundarymanager/models.py
 adminboundarymanager/serializers.py
 adminboundarymanager/tests.py
 adminboundarymanager/urls.py
 adminboundarymanager/utils.py
 adminboundarymanager/views.py
 adminboundarymanager/wagtail_hooks.py
+adminboundarymanager/loaders/__init__.py
+adminboundarymanager/loaders/cod_abs_loader.py
+adminboundarymanager/loaders/gadm_loader.py
+adminboundarymanager/loaders/generic_loader.py
 adminboundarymanager/migrations/0001_initial.py
 adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
 adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
 adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
+adminboundarymanager/migrations/0005_alter_country_country.py
+adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py
 adminboundarymanager/migrations/__init__.py
 adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
 adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
```

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/boundary_loader.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/loaders/cod_abs_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 
 from adminboundarymanager.errors import (
     MissingBoundaryField,
     NoMatchingBoundaryData,
     InvalidBoundaryGeomType,
     UnsupportedBoundaryLevel
 )
-from .models import AdminBoundary
-from .utils import extract_zipped_shapefile
+from adminboundarymanager.models import AdminBoundary
+from adminboundarymanager.utils import extract_zipped_shapefile
 
 COMMON_FIELDS = {
     "level": "LEVEL"
 }
 
 LEVEL0_BOUNDARY_FIELDS = {
-    **COMMON_FIELDS,
     "name_0": "ADM0_EN",
     "gid_0": "ADM0_PCODE",
 }
 LEVEL1_BOUNDARY_FIELDS = {
     **LEVEL0_BOUNDARY_FIELDS,
     "name_1": "ADM1_EN",
     "gid_1": "ADM1_PCODE",
@@ -49,17 +48,24 @@
 
 GEOM_FIELD = {
     "geom": "MULTIPOLYGON",
 }
 
 VALID_GEOM_TYPES = ["Polygon", "MultiPolygon"]
 
+COD_ABS_FIELDS = {
+    "level_0": LEVEL0_BOUNDARY_FIELDS,
+    "level_1": LEVEL1_BOUNDARY_FIELDS,
+    "level_2": LEVEL2_BOUNDARY_FIELDS,
+    "level_3": LEVEL3_BOUNDARY_FIELDS,
+}
+
 
 @transaction.atomic
-def check_and_load_boundaries(shp_path, country_code, level, remove_existing=True):
+def check_and_load_boundaries(shp_path, country, level, remove_existing=True):
     # set required layermapping fields
     if level == 0:
         required_fields = LEVEL0_BOUNDARY_FIELDS
     elif level == 1:
         required_fields = LEVEL1_BOUNDARY_FIELDS
     elif level == 2:
         required_fields = LEVEL2_BOUNDARY_FIELDS
@@ -67,14 +73,17 @@
         required_fields = LEVEL3_BOUNDARY_FIELDS
     elif level == 4:
         required_fields = LEVEL4_BOUNDARY_FIELDS
     else:
         raise UnsupportedBoundaryLevel(
             f"Unsupported admin boundary level : '{level}'. Supported levels are 0, 1, 2, 3 and 4.")
 
+    # add common fields
+    required_fields.update({**COMMON_FIELDS})
+
     # read shapefile first layer
     gdf = gpd.read_file(shp_path, layer=0)
 
     # assign level
     gdf = gdf.assign(LEVEL=level)
 
     # get geom types
@@ -113,21 +122,22 @@
         layer_mapping_fields = {
             **required_fields,
             **GEOM_FIELD,
         }
 
         if remove_existing:
             # delete existing boundary data for given country iso and level
-            AdminBoundary.objects.filter(gid_0=country_code, level=level).delete()
+            AdminBoundary.objects.filter(gid_0=country.code, level=level).delete()
+            AdminBoundary.objects.filter(gid_0=country.alpha3, level=level).delete()
 
         # do layermapping and save
         lm = LayerMapping(AdminBoundary, temp_shapefile_path, layer_mapping_fields)
         lm.save(verbose=True)
 
 
-def load_cod_abs_boundary(shp_zip_path, country_code, level, remove_existing=True):
+def load_cod_abs_boundary(shp_zip_path, country, level, remove_existing=True, **kwargs):
     with tempfile.TemporaryDirectory() as tmpdir:
         # extract shapefile to get .shp file
         shp_path = extract_zipped_shapefile(shp_zip_path, tmpdir)
 
         # load boundaries
-        check_and_load_boundaries(shp_path, country_code, level, remove_existing)
+        check_and_load_boundaries(shp_path, country, level, remove_existing)
```

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/countries.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/countries.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/errors.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/errors.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/forms.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/forms.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 from django import forms
 
 from django.utils.translation import gettext_lazy as _
 
 
-class CodAbsBoundaryUploadForm(forms.Form):
+class GenericBoundaryUploadForm(forms.Form):
     LEVEL_CHOICES = (
         ("0", _("Level 0")),
         ("1", _("Level 1")),
         ("2", _("Level 2")),
         ("3", _("Level 3")),
         ("4", _("Level 4")),
     )
+
     country = forms.ChoiceField(required=True, label=_("Country"))
     level = forms.ChoiceField(required=True, choices=LEVEL_CHOICES, label=_("Admin Boundary Level"))
-    shp_zip = forms.FileField(required=True, label=_("Country Shapefile ZIP"),
-                              widget=forms.FileInput(attrs={'accept': '.zip'}))
+    file = forms.FileField(required=True, label=_("Country Shapefile ZIP"),
+                           widget=forms.FileInput(attrs={'accept': '.zip'}))
+
+    def __init__(self, country_choices=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # set country options
+        if country_choices:
+            self.fields['country'].choices = [(country.code, country.name) for country in country_choices]
+
+
+class CodAbsBoundaryUploadForm(GenericBoundaryUploadForm):
+    pass
+
+
+class GADMBoundaryUploadForm(forms.Form):
+    country = forms.ChoiceField(required=True, label=_("Country"))
+    file = forms.FileField(required=True, label=_("GADM Country Geopackage"),
+                           help_text=_("The uploaded file should be a geopackage, "
+                                       "downloaded from https://gadm.org/download_country.html"),
+                           widget=forms.FileInput(attrs={'accept': '.gpkg'}))
 
     def __init__(self, country_choices=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # set country options
         if country_choices:
             self.fields['country'].choices = [(country.code, country.name) for country in country_choices]
```

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0001_initial.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/models.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 from django.contrib.gis.db import models
-from django.db.models.signals import post_save
+from django.db.models.signals import post_save, post_delete
 from django.dispatch import receiver
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from django_countries.fields import CountryField
 from django_countries.widgets import CountrySelectWidget
 from modelcluster.fields import ParentalKey
@@ -31,15 +31,14 @@
     name_4 = models.CharField(max_length=100, blank=True, null=True)
     gid_0 = models.CharField(max_length=100, blank=True, null=True)
     gid_1 = models.CharField(max_length=100, blank=True, null=True)
     gid_2 = models.CharField(max_length=100, blank=True, null=True)
     gid_3 = models.CharField(max_length=100, blank=True, null=True)
     gid_4 = models.CharField(max_length=100, blank=True, null=True)
     level = models.IntegerField(blank=True, null=True)
-    size = models.CharField(max_length=100, blank=True, null=True)
 
     geom = models.MultiPolygonField(srid=4326)
 
     class Meta:
         verbose_name_plural = _("Administrative Boundaries")
 
     def __str__(self):
@@ -87,56 +86,58 @@
         return info
 
 
 class AdminBoundaryForm(WagtailAdminModelForm):
     def is_valid(self):
         form_is_valid = super().is_valid()
 
-        countries_formset = self.formsets.get("countries")
-        countries_cleaned_data = countries_formset.cleaned_data
+        if form_is_valid:
+            countries_formset = self.formsets.get("countries")
+            countries_cleaned_data = countries_formset.cleaned_data
+
+            countries = []
+            for country in countries_cleaned_data:
+                to_delete = country.get("DELETE")
+
+                if not to_delete:
+                    country_obj = Country(country=country.get("country"))
+                    countries.append(country_obj)
+
+            cleaned_data = self.cleaned_data
+            countries_must_share_boundaries = cleaned_data.get("countries_must_share_boundaries")
+
+            if countries_must_share_boundaries and len(countries) > 1:
+                bounds_polygons = []
+                for country in countries:
+                    bounds_polygons.append(country.country_bounds_polygon)
+
+                union_polygon = bounds_polygons[0]
+                for polygon in bounds_polygons[1:]:
+                    union_polygon = union_polygon.union(polygon)
+
+                connected = isinstance(union_polygon, Polygon)
+                if not connected:
+                    error = _("One or more selected countries do not share boundaries. "
+                              "Please make sure all the countries are in one region and share boundaries")
+                    # add error
+                    self.formsets.get("countries")._non_form_errors.append(error)
 
-        countries = []
-        for country in countries_cleaned_data:
-            to_delete = country.get("DELETE")
-
-            if not to_delete:
-                country_obj = Country(country=country.get("country"))
-                countries.append(country_obj)
-
-        cleaned_data = self.cleaned_data
-        countries_must_share_boundaries = cleaned_data.get("countries_must_share_boundaries")
-
-        if countries_must_share_boundaries and len(countries) > 1:
-            bounds_polygons = []
-            for country in countries:
-                bounds_polygons.append(country.country_bounds_polygon)
-
-            union_polygon = bounds_polygons[0]
-            for polygon in bounds_polygons[1:]:
-                union_polygon = union_polygon.union(polygon)
-
-            connected = isinstance(union_polygon, Polygon)
-            if not connected:
-                error = _("One or more selected countries do not share boundaries. "
-                          "Please make sure all the countries are in one region and share boundaries")
-                # add error
-                self.formsets.get("countries")._non_form_errors.append(error)
-
-                return False
+                    return False
 
         return form_is_valid
 
 
 @register_setting
 class AdminBoundarySettings(BaseSiteSetting, ClusterableModel):
     base_form_class = AdminBoundaryForm
 
     DATA_SOURCE_CHOICES = (
         ("codabs", "OCHA Administrative Boundary Common Operational Datasets (COD-ABS)"),
-        ("gadm41", "Global Administrative Areas 4.1 (GADM)")
+        ("gadm41", "Global Administrative Areas 4.1 (GADM)"),
+        ("generic", "Generic Data Source")
     )
 
     data_source = models.CharField(max_length=100, choices=DATA_SOURCE_CHOICES, default="codabs",
                                    verbose_name=_("Boundary Data Source"), help_text="Source of the boundaries data")
     countries_must_share_boundaries = models.BooleanField(default=True,
                                                           verbose_name=_(
                                                               "Countries must share boundaries - If more than one"),
@@ -144,15 +145,15 @@
                                                               "Validation to ensure that the selected countries share "
                                                               "boundaries with each other. Used if two or more "
                                                               "countries are set."))
 
     panels = [
         FieldPanel("data_source"),
         FieldPanel("countries_must_share_boundaries"),
-        InlinePanel("countries", heading=_("Countries"), label=_("Country")),
+        InlinePanel("countries", heading=_("Countries"), label=_("Country Detail")),
     ]
 
     @cached_property
     def countries_list(self):
         countries = []
         for country in self.countries.all():
             countries.append({
@@ -182,15 +183,15 @@
     @cached_property
     def boundary_tiles_url(self):
         return reverse("admin_boundary_tiles", args=[0, 0, 0]).replace("/0/0/0", r"/{z}/{x}/{y}")
 
 
 class Country(Orderable):
     parent = ParentalKey(AdminBoundarySettings, on_delete=models.CASCADE, related_name='countries')
-    country = CountryField(blank_label=_("Select Country"), verbose_name=_("country"))
+    country = CountryField(blank_label=_("Select Country"), verbose_name=_("country"), unique=True)
 
     panels = [
         FieldPanel("country", widget=CountrySelectWidget()),
     ]
 
     @cached_property
     def country_info(self):
@@ -212,7 +213,19 @@
         return {}
 
 
 # clear cache after saving boundary settings
 @receiver(post_save, sender=AdminBoundarySettings)
 def handle_clear_wagtail_cache(sender, **kwargs):
     clear_cache()
+
+
+# delete any existing country boundaries after deleting a country
+@receiver(post_delete, sender=Country)
+def after_country_delete(sender, instance, **kwargs):
+    country = instance.country
+
+    # delete by 2-letter code
+    AdminBoundary.objects.filter(gid_0=country.code).delete()
+
+    # delete by 3-letter code
+    AdminBoundary.objects.filter(gid_0=country.alpha3).delete()
```

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/serializers.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/serializers.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html` & `adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html`

 * *Files 14% similar despite different names*

```diff
@@ -13,57 +13,76 @@
 
 {% block content %}
     {% trans "Boundary Loader" as header_str %}
 
     {% include "wagtailadmin/shared/header.html" with title=header_str icon="upload" %}
 
     <div class="nice-padding">
+        {% if data_source %}
+            <div class="help-block help-info">
+                <svg class="icon icon-help icon" aria-hidden="true">
+                    <use href="#icon-help"></use>
+                </svg>
+                <p><b>Selected Source: {{ data_source.title }}</b></p>
+                <div>
+                    {{ data_source.description }}
+                </div>
+
+                {% if data_source.data_detail_urls %}
+                    <div style="margin-top: 10px">
+                        <b>You can learn more here:</b>
+                        <ul>
+                            {% for link in data_source.data_detail_urls %}
+                                <li>
+                                    <a href="{{ link.url }}" target="_blank"
+                                       rel="noreferrer noopener">{{ link.label }}</a>
+                                </li>
+                            {% endfor %}
+                        </ul>
+                    </div>
+                {% endif %}
+                {% if data_source.data_download_url %}
+                    <div style="margin-top: 10px">
+                        <b>You can access and download data from the source: </b>
+                        <ul>
+                            <li>
+                                <a href="{{ data_source.data_download_url }}" target="_blank"
+                                   rel="noreferrer noopener">Download from source</a>
+                            </li>
+
+                        </ul>
+                    </div>
+                {% endif %}
+            </div>
+        {% endif %}
         <div style="margin-top: 40px;"
              id="upload_form_wrapper">
-            {% if data_source_unimplemented %}
-                <div class="help-block help-info">
-                    <svg class="icon icon-help icon" aria-hidden="true">
-                        <use href="#icon-help"></use>
-                    </svg>
-                    <p>The boundary source you selected in boundary settings is not yet implemented.</p>
-                    <div>
-                        <p>Please select <b>OCHA COD ABS</b> source for now as we work to implement other sources</p>
+            <form action="{% url 'adminboundarymanager_load_boundary' %}" method="POST"
+                  enctype="multipart/form-data">
+                {% if form.non_field_errors %}
+                    <div class="non-field_errors" style="margin-bottom: 20px">
+                        {% include "wagtailadmin/shared/non_field_errors.html" with form=form %}
                     </div>
-                </div>
-                <a href="{{ settings_url }}" class="button bicolor button--icon button-secondary"><span
-                        class="icon-wrapper">
-                    <svg class="icon icon-edit icon" aria-hidden="true">
-                        <use href="#icon-edit"></use>
-                    </svg>
-                </span>Change Source
-                </a>
-            {% else %}
-                <form action="{% url 'adminboundarymanager_load_boundary' %}" method="POST"
-                      enctype="multipart/form-data">
-                    {% if form.non_field_errors %}
-                        <div class="non-field_errors" style="margin-bottom: 20px">
-                            {% include "wagtailadmin/shared/non_field_errors.html" with form=form %}
-                        </div>
-                    {% endif %}
-                    <ul class="fields">
-                        {% csrf_token %}
-                        {% for field in form %}
-                            {% if field.is_hidden %}
-                                {{ field }}
-                            {% else %}
-                                {% include "wagtailadmin/shared/field_as_li.html" %}
-                            {% endif %}
-                        {% endfor %}
-                        <li>
-                            <button type="submit" class="button"> {% trans 'Upload' %}</button>
-                        </li>
-                    </ul>
-                </form>
-            {% endif %}
+                {% endif %}
+                <ul class="fields">
+                    {% csrf_token %}
+                    {% for field in form %}
+                        {% if field.is_hidden %}
+                            {{ field }}
+                        {% else %}
+                            {% include "wagtailadmin/shared/field_as_li.html" %}
+                        {% endif %}
+                    {% endfor %}
+                    <li>
+                        <button type="submit" class="button"> {% trans 'Upload' %}</button>
+                    </li>
+                </ul>
+            </form>
         </div>
+
     </div>
 {% endblock %}
 
 {% block extra_js %}
     {{ block.super }}
     {{ form_media.js }}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,22 +1,30 @@
 {% extends "wagtailadmin/base.html" %} {% load i18n %} {% load l10n %} {% load
 wagtailadmin_tags wagtailimages_tags static %} {% block titletag %}{%
 blocktrans with title=page.get_admin_display_title %}Boundary Loader {{ title
 }} {% endblocktrans %}{% endblock %} {% block extra_css %} {{ block.super }} {
 { form_media.css }} {% endblock %} {% block content %} {% trans "Boundary
 Loader" as header_str %} {% include "wagtailadmin/shared/header.html" with
 title=header_str icon="upload" %}
-{% if data_source_unimplemented %}
+{% if data_source %}
 
-The boundary source you selected in boundary settings is not yet implemented.
-Please select OCHA COD ABS source for now as we work to implement other sources
-___Change_Source {% else %}
+Selected Source: {{ data_source.title }}
+{{ data_source.description }}
+{% if data_source.data_detail_urls %}
+You can learn more here:
+    * {% for link in data_source.data_detail_urls %}
+    * {{_link.label_}}
+    * {% endfor %}
+{% endif %} {% if data_source.data_download_url %}
+You can access and download data from the source:
+    * Download_from_source
+{% endif %}
+{% endif %}
 {% if form.non_field_errors %}
 {% include "wagtailadmin/shared/non_field_errors.html" with form=form %}
 {% endif %}
     * {% csrf_token %} {% for field in form %} {% if field.is_hidden %} {
       { field }} {% else %} {% include "wagtailadmin/shared/field_as_li.html"
       %} {% endif %} {% endfor %}
     *  {% trans 'Upload' %}
-{% endif %}
 {% endblock %} {% block extra_js %} {{ block.super }} {{ form_media.js }} {%
 endblock %}
```

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html` & `adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     <div class="nice-padding">
         <div style="margin-top: 40px;">
             {% if countries %}
                 <div class="w-field__input" style="margin-bottom: 20px">
                     <select id="country_selector">
                         <option value="all">All Countries</option>
                         {% for country in countries %}
-                            <option value="{{ country.country.code }}"
+                            <option value="{% if use_country_alpha3 %}{{ country.country.alpha3 }}{% else %}
+                                {{ country.country.code }}{% endif %}"
                                     data-info="{{ country.country_info_str }}">{{ country.country.name }}</option>
                         {% endfor %}
                     </select>
                 </div>
             {% endif %}
             <div id="preview-map" style="height: 600px;width: 100%"></div>
         </div>
```

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/urls.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/urls.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/utils.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/utils.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/views.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from rest_framework.filters import SearchFilter
 from rest_framework.generics import ListAPIView, RetrieveAPIView
 from wagtail.admin import messages
 from wagtail.admin.auth import user_passes_test, user_has_any_page_permission
 from wagtailcache.cache import cache_page
 from wagtailcache.cache import clear_cache
 
-from .boundary_loader import load_cod_abs_boundary
-from .forms import CodAbsBoundaryUploadForm
-from .models import AdminBoundarySettings, AdminBoundary
+from .forms import CodAbsBoundaryUploadForm, GADMBoundaryUploadForm, GenericBoundaryUploadForm
+from .loaders import load_cod_abs_boundary, load_gadm_boundary, load_generic_boundary, data_sources
+from .models import AdminBoundarySettings, AdminBoundary, Country
 from .serializers import AdminBoundarySerializer
 
 
 @user_passes_test(user_has_any_page_permission)
 def load_boundary(request):
     template = "adminboundarymanager/boundary_loader.html"
 
@@ -29,41 +29,50 @@
         "wagtailsettings:edit",
         args=[AdminBoundarySettings._meta.app_label, AdminBoundarySettings._meta.model_name, ],
     )
     context.update({"settings_url": settings_url})
 
     abm_settings = AdminBoundarySettings.for_request(request)
 
-    if abm_settings.data_source != "codabs":
-        context.update({"data_source_unimplemented": True})
-        return render(request, template_name=template, context=context)
+    context.update({"data_source": data_sources.get(abm_settings.data_source)})
 
-    countries = [obj.country for obj in abm_settings.countries.all()]
+    if abm_settings.data_source == "codabs":
+        form_class = CodAbsBoundaryUploadForm
+        loader_fn = load_cod_abs_boundary
+    elif abm_settings.data_source == "gadm41":
+        form_class = GADMBoundaryUploadForm
+        loader_fn = load_gadm_boundary
+    else:
+        form_class = GenericBoundaryUploadForm
+        loader_fn = load_generic_boundary
 
-    FormClass = CodAbsBoundaryUploadForm
+    countries = [obj.country for obj in abm_settings.countries.all()]
 
     if request.POST:
-        form = FormClass(countries, request.POST, request.FILES)
+        form = form_class(countries, request.POST, request.FILES)
 
         if form.is_valid():
-            shp_zip = form.cleaned_data.get("shp_zip")
+            file = form.cleaned_data.get("file")
             country_code = form.cleaned_data.get("country")
-            level = form.cleaned_data.get("level")
+            level = None
+
+            if abm_settings.data_source != "gadm41":
+                level = int(form.cleaned_data.get("level"))
 
             if not country_code:
                 form.add_error(None, "Please select a country in layer manager settings and try again")
 
-            with tempfile.NamedTemporaryFile(delete=False, suffix=f"_{shp_zip.name}") as temp_file:
-                for chunk in shp_zip.chunks():
+            country_option = Country.objects.get(country=country_code)
+
+            with tempfile.NamedTemporaryFile(delete=False, suffix=f"_{file.name}") as temp_file:
+                for chunk in file.chunks():
                     temp_file.write(chunk)
 
                 try:
-                    load_cod_abs_boundary(shp_zip_path=temp_file.name,
-                                          country_code=country_code,
-                                          level=int(level))
+                    loader_fn(temp_file.name, country=country_option.country, level=level)
                 except Exception as e:
                     form.add_error(None, str(e))
                     context.update({"form": form, "has_error": True})
                     countries = AdminBoundary.objects.filter(level=0)
 
                     if countries.exists():
                         context.update({"existing_countries": countries})
@@ -76,37 +85,39 @@
             clear_cache()
 
             return redirect(reverse("adminboundarymanager_preview_boundary"))
         else:
             context.update({"form": form})
             return render(request, template_name=template, context=context)
     else:
-        form = FormClass(countries)
+        form = form_class(countries)
         context["form"] = form
 
         return render(request, template_name=template, context=context)
 
 
 @user_passes_test(user_has_any_page_permission)
 def preview_boundary(request):
     template = "adminboundarymanager/boundary_preview.html"
 
     abm_settings = AdminBoundarySettings.for_request(request)
     countries = abm_settings.countries.all()
+    boundary_data_source = abm_settings.data_source
 
     boundary_tiles_url = abm_settings.boundary_tiles_url
 
     boundary_tiles_url = request.scheme + '://' + request.get_host() + boundary_tiles_url
 
     context = {
         "mapConfig": {
             "boundaryTilesUrl": boundary_tiles_url,
             "combinedBbox": abm_settings.combined_countries_bounds
         },
         "countries": countries,
+        "use_country_alpha3": boundary_data_source == "gadm41",
         "load_boundary_url": reverse("adminboundarymanager_load_boundary")
     }
 
     return render(request, template, context=context)
 
 
 @method_decorator(cache_page, name='get')
```

### Comparing `adm-boundary-manager-0.0.4/adminboundarymanager/wagtail_hooks.py` & `adm-boundary-manager-0.0.5/adminboundarymanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.4/setup.cfg` & `adm-boundary-manager-0.0.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = adm-boundary-manager
-version = 0.0.4
+version = 0.0.5
 description = Load, manage and visualize Administrative Boundaries Data in Wagtail
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/adm-boundary-manager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
@@ -26,13 +26,13 @@
 python_requires = >=3.9
 install_requires = 
 	wagtail>=4.2.2
 	shapely>=2.0.1
 	geopandas>=0.12.2
 	django-filter>=22.1
 	django-countries>=7.5.1
-	wagtail-cache>=2.2.0
+	wagtail-cache>=2.3.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

