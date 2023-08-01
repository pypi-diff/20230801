# Comparing `tmp/discovery-capability-0.5.1.tar.gz` & `tmp/discovery-capability-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.5.1.tar", last modified: Thu Jul 27 22:07:54 2023, max compression
+gzip compressed data, was "discovery-capability-0.5.2.tar", last modified: Tue Aug  1 15:55:57 2023, max compression
```

## Comparing `discovery-capability-0.5.1.tar` & `discovery-capability-0.5.2.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.476600 discovery-capability-0.5.1/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.1/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.1/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 22:07:54.476837 discovery-capability-0.5.1/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.1/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.311444 discovery-capability-0.5.1/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.311968 discovery-capability-0.5.1/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-27 20:11:45.000000 discovery-capability-0.5.1/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.314744 discovery-capability-0.5.1/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.1/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14475 2023-07-27 16:49:58.000000 discovery-capability-0.5.1/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.1/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)    10567 2023-07-27 21:55:26.000000 discovery-capability-0.5.1/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.1/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.315818 discovery-capability-0.5.1/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.1/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.320032 discovery-capability-0.5.1/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.1/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.1/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.1/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.5.1/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    68036 2023-07-27 21:19:07.000000 discovery-capability-0.5.1/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.5.1/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.323302 discovery-capability-0.5.1/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.1/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.1/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.1/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.1/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.464525 discovery-capability-0.5.1/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.1/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-27 22:07:54.477535 discovery-capability-0.5.1/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.1/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.468546 discovery-capability-0.5.1/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.1/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.470077 discovery-capability-0.5.1/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.1/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3000 2023-07-27 21:49:45.000000 discovery-capability-0.5.1/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.1/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.471174 discovery-capability-0.5.1/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.1/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.475674 discovery-capability-0.5.1/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.1/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.1/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.1/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-27 20:05:03.000000 discovery-capability-0.5.1/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.1/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.301634 discovery-capability-0.5.2/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.2/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.2/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 15:55:57.301855 discovery-capability-0.5.2/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.2/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.133343 discovery-capability-0.5.2/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-01 15:55:57.000000 discovery-capability-0.5.2/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.133860 discovery-capability-0.5.2/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-27 22:41:13.000000 discovery-capability-0.5.2/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.137040 discovery-capability-0.5.2/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.2/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14475 2023-07-27 16:49:58.000000 discovery-capability-0.5.2/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.2/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20338 2023-08-01 15:46:02.000000 discovery-capability-0.5.2/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.2/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.137784 discovery-capability-0.5.2/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.2/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.141549 discovery-capability-0.5.2/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.2/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.2/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.2/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11239 2023-07-30 18:52:11.000000 discovery-capability-0.5.2/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.2/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20903 2023-07-27 23:20:42.000000 discovery-capability-0.5.2/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.143846 discovery-capability-0.5.2/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.2/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.2/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.2/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.2/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.293834 discovery-capability-0.5.2/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.2/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.2/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-01 15:55:57.302514 discovery-capability-0.5.2/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.2/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.294753 discovery-capability-0.5.2/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.2/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.295624 discovery-capability-0.5.2/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.2/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.2/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.2/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.296390 discovery-capability-0.5.2/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.2/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 15:55:57.299515 discovery-capability-0.5.2/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.2/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.2/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3099 2023-07-29 22:54:26.000000 discovery-capability-0.5.2/test/intent/fb_correlate_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.2/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.2/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.2/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.5.1/LICENSE.txt` & `discovery-capability-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/PKG-INFO` & `discovery-capability-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.1
+Version: 0.5.2
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.1/README.rst` & `discovery-capability-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.5.2/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.1
+Version: 0.5.2
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.1/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.5.2/discovery_capability.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -50,10 +50,11 @@
 test/__init__.py
 test/component/__init__.py
 test/component/discovery_test.py
 test/component/synthetic_test.py
 test/handlers/__init__.py
 test/intent/__init__.py
 test/intent/fb_analysis_intent_test.py
+test/intent/fb_correlate_intent_test.py
 test/intent/fb_diff_intent_test.py
 test/intent/fb_intent_test.py
 test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.5.1/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.5.2/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/components/commons.py` & `discovery-capability-0.5.2/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/components/feature_build.py` & `discovery-capability-0.5.2/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.5.2/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/intent/common_intent.py` & `discovery-capability-0.5.2/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.5.2/ds_capability/intent/feature_build_intent.py`

 * *Files 2% similar despite different names*

```diff
@@ -911,18 +911,19 @@
         canonical = Commons.table_append(canonical, _)
         # string
         _ = self.get_sample(sample_name='us_street_names', size=size, seed=seed, column_name='string',  save_intent=False)
         canonical = Commons.table_append(canonical, _)
 
         if isinstance(inc_nulls, bool) and inc_nulls:
             gen = np.random.default_rng()
-            # cat_null
             prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
-            _ = self.get_category(selection=['M', 'F', 'U'], relative_freq=[9,8,4], quantity=1 - prob_nulls,
-                                  column_name='cat_null', size=size, seed=seed, save_intent=False)
+            # cat_null
+            _ = self.get_category(selection=['High', 'Med', 'Low'], relative_freq=[9,8,4], quantity=1 - prob_nulls,
+                                  column_name='cat_null', size=size, encode=category_encode, seed=seed,
+                                  save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # num_null
             prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
             _ = self.get_number(start=-1.0, stop=1.0, relative_freq=[1, 1, 2, 3, 5, 8, 13, 21], size=size,
                                 quantity=1 - prob_nulls, column_name='num_null', seed=seed, save_intent=False)
             canonical = Commons.table_append(canonical, _)
             # int_null
```

### Comparing `discovery-capability-0.5.1/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.5.2/ds_capability/intent/feature_build_model_intent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import inspect
 import pandas as pd
 import pyarrow as pa
+from aistac.handlers.abstract_handlers import HandlerFactory
+
+from ds_capability.components.discovery import DataDiscovery
 from ds_capability.intent.abstract_feature_build_intent import AbstractFeatureBuildIntentModel
 from ds_capability.intent.common_intent import CommonsIntentModel
 from ds_capability.components.commons import Commons
 from ds_capability.managers.feature_build_property_manager import FeatureBuildPropertyManager
 
 
 # noinspection PyArgumentList
@@ -125,15 +128,15 @@
                     - if int: added to the level specified, overwriting any that already exist
 
         :param replace_intent: (optional) if the intent method exists at the level, or default level
                     - True - replaces the current intent method with the new
                     - False - leaves it untouched, disregarding the new intent
 
         :param remove_duplicates: (optional) removes any duplicate intent in any level that is identical
-        :return: a pd.DataFrame
+        :return: a pa.Table
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # intent action
         canonical = self._get_canonical(canonical)
@@ -143,29 +146,24 @@
         flagged_connector = self._extract_value(flagged_connector)
         summary_connector = self._extract_value(summary_connector)
         detail_connector = self._extract_value(detail_connector)
         unmatched_connector = self._extract_value(unmatched_connector)
         on_key = Commons.list_formatter(self._extract_value(on_key))
         left_diff = Commons.list_diff(canonical.column_names, other.column_names, symmetric=False)
         right_diff = Commons.list_diff(other.column_names, canonical.column_names, symmetric=False)
-
-
-
-
-        df_canonical = canonical.to_pandas()
-        df_other = other.to_pandas()
-        # remove not matching columns
-        left_diff = Commons.list_diff(df_canonical.columns.to_list(), df_other.columns.to_list(), symmetric=False)
-        right_diff = Commons.list_diff(df_other.columns.to_list(), df_canonical.columns.to_list(), symmetric=False)
-        _canonical = df_canonical.drop(left_diff, axis=1)
-        _other = df_other.drop(right_diff, axis=1)
+        # drop columns
+        tbl_canonical = canonical.drop_columns(left_diff)
+        tbl_other = other.drop_columns(right_diff)
+        # pandas
+        df_canonical = tbl_canonical.to_pandas()
+        df_other = tbl_other.to_pandas()
         # sort
-        _canonical.sort_values(on_key, inplace=True)
-        _other.sort_values(on_key, inplace=True)
-        _other = _other.loc[:, _canonical.columns.to_list()]
+        df_canonical.sort_values(on_key, inplace=True)
+        df_other.sort_values(on_key, inplace=True)
+        df_other = df_other.loc[:, df_canonical.columns.to_list()]
 
         # unmatched report
         if isinstance(unmatched_connector, str):
             if self._pm.has_connector(unmatched_connector):
                 left_merge = pd.merge(df_canonical, df_other, on=on_key, how='left', suffixes=('', '_y'), indicator=True)
                 left_merge = left_merge[left_merge['_merge'] == 'left_only']
                 left_merge = left_merge[left_merge.columns[~left_merge.columns.str.endswith('_y')]]
@@ -177,15 +175,15 @@
                 unmatched.insert(0, 'found_in', unmatched.pop('_merge'))
                 handler = self._pm.get_connector_handler(unmatched_connector)
                 handler.persist_canonical(pa.Table.from_pandas(unmatched), **kwargs)
             else:
                 raise ValueError(f"The connector name {unmatched_connector} has been given but no Connect Contract added")
 
         # remove non-matching rows
-        df = pd.merge(_canonical, _other, on=on_key, how='inner', suffixes=('_x', '_y'))
+        df = pd.merge(df_canonical, df_other, on=on_key, how='inner', suffixes=('_x', '_y'))
         df_x = df.filter(regex='(_x$)', axis=1)
         df_y = df.filter(regex='(_y$)', axis=1)
         df_x.columns = df_x.columns.str.removesuffix('_x')
         df_y.columns = df_y.columns.str.removesuffix('_y')
         # flag the differences
         diff = df_x.ne(df_y).astype(int)
         if drop_zero_sum:
@@ -237,7 +235,78 @@
             raise ValueError(f"The connector name {flagged_connector} has been given but no Connect Contract added")
 
         if drop_zero_sum:
             diff = diff.sort_values(on_key)
             diff = diff.reset_index(drop=True)
 
         return pa.Table.from_pandas(diff)
+
+    def model_profiling(self, canonical: pa.Table, profiling: str, headers: [str, list]=None, drop: bool=None,
+                         dtype: [str, list]=None, exclude: bool=None, regex: [str, list]=None,
+                         re_ignore_case: bool=None, connector_name: str=None, seed: int=None, save_intent: bool=None,
+                         column_name: [int, str]=None, intent_order: int=None, replace_intent: bool=None,
+                         remove_duplicates: bool=None, **kwargs) -> pa.Table:
+        """ Data profiling provides, analyzing, and creating useful summaries of data. The process yields a high-level
+        overview which aids in the discovery of data quality issues, risks, and overall trends. It can be used to
+        identify any errors, anomalies, or patterns that may exist within the data. There are three types of data
+        profiling available 'dictionary', 'schema' or 'quality'
+
+        :param canonical: a direct or generated pd.DataFrame. see context notes below
+        :param profiling: The profiling name. Options are 'dictionary', 'schema' or 'quality'
+        :param headers: (optional) a filter of headers from the 'other' dataset
+        :param drop: (optional) to drop or not drop the headers if specified
+        :param dtype: (optional) a filter on data type for the 'other' dataset. int, float, bool, object
+        :param exclude: (optional) to exclude or include the data types if specified
+        :param regex: (optional) a regular expression to search the headers. example '^((?!_amt).)*$)' excludes '_amt'
+        :param re_ignore_case: (optional) true if the regex should ignore case. Default is False
+        :param connector_name::(optional) a connector name where the outcome is sent
+        :param seed:(optional) this is a placeholder, here for compatibility across methods
+        :param save_intent: (optional) if the intent contract should be saved to the property manager
+        :param column_name: (optional) the column name that groups intent to create a column
+        :param intent_order: (optional) the order in which each intent should run.
+                    - If None: default's to -1
+                    - if -1: added to a level above any current instance of the intent section, level 0 if not found
+                    - if int: added to the level specified, overwriting any that already exist
+
+        :param replace_intent: (optional) if the intent method exists at the level, or default level
+                    - True - replaces the current intent method with the new
+                    - False - leaves it untouched, disregarding the new intent
+
+        :param remove_duplicates: (optional) removes any duplicate intent in any level that is identical
+        :return: a pa.Table
+        """
+        # intent persist options
+        self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
+                                   column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
+                                   remove_duplicates=remove_duplicates, save_intent=save_intent)
+        # intent action
+        canonical = self._get_canonical(canonical)
+        columns = Commons.filter_headers(canonical, headers=headers, drop=drop, dtype=dtype, exclude=exclude,
+                                        regex=regex, re_ignore_case=re_ignore_case)
+        _seed = self._seed() if seed is None else seed
+        if profiling == 'dictionary':
+            result =  DataDiscovery.data_dictionary(canonical=canonical, table_cast=True, stylise=False)
+        elif profiling == 'quality':
+            result =  DataDiscovery.data_quality(canonical=canonical, stylise=False)
+        # elif profiling == 'schema':
+        #     blob = DataDiscovery.analyse_association(df=canonical, columns_list=columns)
+        #     report = pd.DataFrame(columns=['root', 'section', 'element', 'value'])
+        #     root_list = DataAnalytics.get_tree_roots(analytics_blob=blob)
+        #     for root_items in root_list:
+        #         data_analysis = DataAnalytics.from_root(analytics_blob=blob, root=root_items)
+        #         for section in data_analysis.section_names:
+        #             for element, value in data_analysis.get(section).items():
+        #                 to_append = [root_items, section, element, value]
+        #                 a_series = pd.Series(to_append, index=report.columns)
+        #                 report = pd.concat([report, a_series.to_frame().transpose()], ignore_index=True)
+        #     result = report
+        else:
+            raise ValueError(f"The report name '{profiling}' is not recognised. Use 'dictionary', 'schema' or 'quality'")
+        if isinstance(connector_name, str):
+            if self._pm.has_connector(connector_name):
+                handler = self._pm.get_connector_handler(connector_name)
+                handler.persist_canonical(result, **kwargs)
+                return canonical
+            raise ValueError(f"The connector name {connector_name} has been given but no Connect Contract added")
+        # set the index
+        return result
+
```

### Comparing `discovery-capability-0.5.1/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.5.2/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.5.2/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.5.2/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.5.2/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.5.2/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.5.2/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.5.2/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.5.2/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.5.2/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.5.2/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.5.2/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.5.2/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.5.2/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.5.2/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.5.2/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/ds_capability/sample/sample_data.py` & `discovery-capability-0.5.2/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/setup.py` & `discovery-capability-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/test/component/discovery_test.py` & `discovery-capability-0.5.2/test/component/discovery_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,21 +74,23 @@
         result = DataDiscovery.data_dictionary(tbl, stylise=True)
         pprint(result.to_string())
 
     def test_data_quality(self):
         sb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = sb.tools
         tbl = tools.get_synthetic_data_types(1000, inc_nulls=True)
-        result = DataDiscovery.data_quality(tbl)
-        print(result.column_names)
-        # c = result.column('summary').combine_chunks()
-        # print(c)
         result = DataDiscovery.data_quality(tbl, stylise=True)
         pprint(result.to_string())
 
+    def test_data_schema(self):
+        sb = FeatureBuild.from_memory()
+        tools: FeatureBuildIntentModel = sb.tools
+        tbl = tools.get_synthetic_data_types(1000, inc_nulls=True)
+        result = DataDiscovery.data_schema(tbl, stylise=True)
+        pprint(result.to_string())
 
 
     def test_raise(self):
         with self.assertRaises(KeyError) as context:
             env = os.environ['NoEnvValueTest']
         self.assertTrue("'NoEnvValueTest'" in str(context.exception))
```

### Comparing `discovery-capability-0.5.1/test/component/synthetic_test.py` & `discovery-capability-0.5.2/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.5.2/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.5.2/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.1/test/intent/fb_intent_test.py` & `discovery-capability-0.5.2/test/intent/fb_intent_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         except OSError:
             pass
 
     def test_for_smoke(self):
         fb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = fb.tools
         tbl = tools.get_synthetic_data_types(100)
-        self.assertEqual((100, 7), tbl.shape)
+        self.assertEqual((100, 6), tbl.shape)
         tbl = tools.get_synthetic_data_types(100, inc_nulls=True, prob_nulls=0.03)
         self.assertEqual((100, 19), tbl.shape)
 
     def test_run_component_pipeline(self):
         fb = FeatureBuild.from_env('test', has_contract=False)
         tools: FeatureBuildIntentModel = fb.tools
         # reload the properties
```

### Comparing `discovery-capability-0.5.1/test/intent/fb_model_intent_test.py` & `discovery-capability-0.5.2/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

