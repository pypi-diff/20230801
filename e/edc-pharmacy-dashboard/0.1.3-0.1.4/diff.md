# Comparing `tmp/edc-pharmacy-dashboard-0.1.3.tar.gz` & `tmp/edc-pharmacy-dashboard-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-pharmacy-dashboard-0.1.3.tar", last modified: Wed May 24 16:55:14 2023, max compression
+gzip compressed data, was "edc-pharmacy-dashboard-0.1.4.tar", last modified: Tue Aug  1 05:17:45 2023, max compression
```

## Comparing `edc-pharmacy-dashboard-0.1.3.tar` & `edc-pharmacy-dashboard-0.1.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.186270 edc-pharmacy-dashboard-0.1.3/
--rw-r--r--   0 erikvw     (501) staff       (20)     1354 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.3/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      150 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1480 2023-05-24 16:55:14.186360 edc-pharmacy-dashboard-0.1.3/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      616 2020-03-13 02:50:11.000000 edc-pharmacy-dashboard-0.1.3/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.178674 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1378 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      244 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      306 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/dashboard_templates.py
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/dashboard_urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      777 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/middleware.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.179416 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.179643 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/model_wrappers/
--rw-r--r--   0 erikvw     (501) staff       (20)       65 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/model_wrappers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      701 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/model_wrappers/prescription_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1143 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/navbars.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.174004 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/old/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.179918 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/old/model_wrappers/
--rw-r--r--   0 erikvw     (501) staff       (20)     1242 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/old/model_wrappers/appointment_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      738 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/old/model_wrappers/worklist_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)       60 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/patterns.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.174118 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.174167 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.180745 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      588 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/appointment_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1165 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/base_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      478 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.174419 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.181330 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/
--rw-r--r--   0 erikvw     (501) staff       (20)     2719 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)     3967 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/dispensensing_modal.html
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      214 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/results_header.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.181748 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/
--rw-r--r--   0 erikvw     (501) staff       (20)     1751 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      290 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      227 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/results_header.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.182301 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/
--rw-r--r--   0 erikvw     (501) staff       (20)      346 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/buttons_column.html
--rw-r--r--   0 erikvw     (501) staff       (20)      703 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      343 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      198 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/results_header.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2359 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      611 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/prescription_listboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)      328 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/worklist_listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.182431 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      481 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.182922 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      194 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.183611 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/
--rw-r--r--   0 erikvw     (501) staff       (20)      229 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1818 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/approve_prescription.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3418 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/base_action_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      947 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/dispense_print_label_action_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2005 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/dispensing_action_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1064 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/dispense_print_label_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2703 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/dispensing_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1134 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/home_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.184336 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_filters/
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_filters/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      454 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_filters/appointment_listboard_view_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      480 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_filters/prescription_listboard_view_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_filters/worklist_listboard_view_filters.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.184921 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_views/
--rw-r--r--   0 erikvw     (501) staff       (20)      190 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2044 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_views/base_listboard.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1473 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_views/prescribe_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1587 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_views/worklist_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.185720 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      494 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/mixins/clean_search_term_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      470 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/mixins/dispense_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/mixins/models_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      629 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/mixins/study_site_name_queryset_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      388 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/mixins/urls_view_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.179307 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1480 2023-05-24 16:55:14.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     4255 2023-05-24 16:55:14.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:55:14.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:14:02.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-05-24 16:55:14.000000 edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      829 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/manage.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1790 2023-05-24 16:55:05.000000 edc-pharmacy-dashboard-0.1.3/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)      815 2022-09-15 02:34:07.000000 edc-pharmacy-dashboard-0.1.3/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1192 2023-05-24 16:55:14.186643 edc-pharmacy-dashboard-0.1.3/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.175020 edc-pharmacy-dashboard-0.1.3/static/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.174954 edc-pharmacy-dashboard-0.1.3/static/edc_label/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.185857 edc-pharmacy-dashboard-0.1.3/static/edc_label/label_templates/
--rw-r--r--   0 erikvw     (501) staff       (20)      195 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/static/edc_label/label_templates/edc_pharma.lbl
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.175063 edc-pharmacy-dashboard-0.1.3/static/edc_pharma_dashboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:55:14.186089 edc-pharmacy-dashboard-0.1.3/static/edc_pharma_dashboard/css/
--rw-r--r--   0 erikvw     (501) staff       (20)     1772 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.3/static/edc_pharma_dashboard/css/timeline.css
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.280454 edc-pharmacy-dashboard-0.1.4/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1354 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.4/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      150 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1480 2023-08-01 05:17:45.280550 edc-pharmacy-dashboard-0.1.4/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      616 2020-03-13 02:50:11.000000 edc-pharmacy-dashboard-0.1.4/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.272134 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1378 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      244 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      306 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/dashboard_templates.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/dashboard_urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      777 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/middleware.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.272934 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.273176 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/model_wrappers/
+-rw-r--r--   0 erikvw     (501) staff       (20)       65 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/model_wrappers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      701 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/model_wrappers/prescription_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1143 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/navbars.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.267453 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/old/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.273443 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/old/model_wrappers/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1242 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/old/model_wrappers/appointment_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      738 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/old/model_wrappers/worklist_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       60 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/patterns.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.267577 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.267625 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.274339 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      588 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/appointment_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1165 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/base_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      478 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.267883 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.274938 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2719 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     3967 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/dispensensing_modal.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      214 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/results_header.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.275441 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1751 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      290 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      227 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/results_header.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.276059 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/
+-rw-r--r--   0 erikvw     (501) staff       (20)      346 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/buttons_column.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      703 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      343 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      198 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/results_header.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2359 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      611 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/prescription_listboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      328 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/worklist_listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.276225 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      481 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.276722 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      194 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.277430 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      229 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1818 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/approve_prescription.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3418 2022-06-23 20:10:24.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/base_action_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      947 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/dispense_print_label_action_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2005 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/dispensing_action_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1064 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/dispense_print_label_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2703 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/dispensing_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1134 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/home_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.278159 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_filters/
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_filters/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      454 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_filters/appointment_listboard_view_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      480 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_filters/prescription_listboard_view_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_filters/worklist_listboard_view_filters.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.278764 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      190 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2044 2022-08-25 03:23:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_views/base_listboard.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1473 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_views/prescribe_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1587 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_views/worklist_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.279744 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      494 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/mixins/clean_search_term_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      470 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/mixins/dispense_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/mixins/models_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      629 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/mixins/study_site_name_queryset_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      388 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/mixins/urls_view_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.272794 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1480 2023-08-01 05:17:45.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     4255 2023-08-01 05:17:45.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 05:17:45.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:14:02.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-08-01 05:17:45.000000 edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      829 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/manage.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1790 2023-05-24 16:55:05.000000 edc-pharmacy-dashboard-0.1.4/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)      874 2023-08-01 05:17:38.000000 edc-pharmacy-dashboard-0.1.4/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1192 2023-08-01 05:17:45.280852 edc-pharmacy-dashboard-0.1.4/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.268495 edc-pharmacy-dashboard-0.1.4/static/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.268424 edc-pharmacy-dashboard-0.1.4/static/edc_label/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.279964 edc-pharmacy-dashboard-0.1.4/static/edc_label/label_templates/
+-rw-r--r--   0 erikvw     (501) staff       (20)      195 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/static/edc_label/label_templates/edc_pharma.lbl
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.268555 edc-pharmacy-dashboard-0.1.4/static/edc_pharma_dashboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:17:45.280242 edc-pharmacy-dashboard-0.1.4/static/edc_pharma_dashboard/css/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1772 2020-03-04 23:14:01.000000 edc-pharmacy-dashboard-0.1.4/static/edc_pharma_dashboard/css/timeline.css
```

### Comparing `edc-pharmacy-dashboard-0.1.3/.gitignore` & `edc-pharmacy-dashboard-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/LICENSE` & `edc-pharmacy-dashboard-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/PKG-INFO` & `edc-pharmacy-dashboard-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-pharmacy-dashboard
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pharmacy dashboard classes in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-pharmacy-dashboard
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc pharmacy,dashboard,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-pharmacy-dashboard-0.1.3/README.rst` & `edc-pharmacy-dashboard-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/apps.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/apps.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/middleware.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/middleware.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/model_wrappers/prescription_model_wrapper.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/model_wrappers/prescription_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/navbars.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/navbars.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/old/model_wrappers/appointment_model_wrapper.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/old/model_wrappers/appointment_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/old/model_wrappers/worklist_model_wrapper.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/old/model_wrappers/worklist_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/appointment_listboard.html` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/appointment_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/base_listboard.html` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/base_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/columns.html` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/columns.html`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/dispensensing_modal.html` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/appointment/dispensensing_modal.html`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/columns.html` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/prescription/columns.html`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/columns.html` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard/worklist/columns.html`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard.html` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/listboard.html`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/prescription_listboard.html` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/templates/edc_pharmacy_dashboard/bootstrap3/prescription_listboard.html`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/approve_prescription.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/approve_prescription.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/base_action_view.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/base_action_view.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/dispense_print_label_action_view.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/dispense_print_label_action_view.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/action_views/dispensing_action_view.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/action_views/dispensing_action_view.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/dispense_print_label_mixin.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/dispense_print_label_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/dispensing_view.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/dispensing_view.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/home_view.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/home_view.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_views/base_listboard.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_views/base_listboard.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_views/prescribe_listboard_view.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_views/prescribe_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/listboard_views/worklist_listboard_view.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/listboard_views/worklist_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard/views/mixins/study_site_name_queryset_view_mixin.py` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard/views/mixins/study_site_name_queryset_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard.egg-info/PKG-INFO` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-pharmacy-dashboard
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pharmacy dashboard classes in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-pharmacy-dashboard
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc pharmacy,dashboard,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-pharmacy-dashboard-0.1.3/edc_pharmacy_dashboard.egg-info/SOURCES.txt` & `edc-pharmacy-dashboard-0.1.4/edc_pharmacy_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/manage.py` & `edc-pharmacy-dashboard-0.1.4/manage.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/pyproject.toml` & `edc-pharmacy-dashboard-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/runtests.py` & `edc-pharmacy-dashboard-0.1.4/runtests.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     calling_file=__file__,
     EDC_NAVBAR_VERIFY_ON_LOAD=IGNORE,
     EDC_AUTH_CODENAMES_WARN_ONLY=True,
     EDC_AUTH_SKIP_SITE_AUTHS=True,
     EDC_AUTH_SKIP_AUTH_UPDATER=True,
     BASE_DIR=base_dir,
     APP_NAME=app_name,
+    SUBJECT_VISIT_MODEL="edc_visit_tracking.subjectvisit",
     EXTRA_INSTALLED_APPS=[f"{app_name}.apps.AppConfig"],
     add_dashboard_middleware=True,
     add_lab_dashboard_middleware=True,
     # use_test_urls=True,
 ).settings
```

### Comparing `edc-pharmacy-dashboard-0.1.3/setup.cfg` & `edc-pharmacy-dashboard-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-dashboard-0.1.3/static/edc_pharma_dashboard/css/timeline.css` & `edc-pharmacy-dashboard-0.1.4/static/edc_pharma_dashboard/css/timeline.css`

 * *Files identical despite different names*

