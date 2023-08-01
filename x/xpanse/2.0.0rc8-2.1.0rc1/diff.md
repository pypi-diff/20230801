# Comparing `tmp/xpanse-2.0.0rc8.tar.gz` & `tmp/xpanse-2.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanse-2.0.0rc8.tar", last modified: Wed Jul  5 14:44:34 2023, max compression
+gzip compressed data, was "xpanse-2.1.0rc1.tar", last modified: Tue Aug  1 13:31:30 2023, max compression
```

## Comparing `xpanse-2.0.0rc8.tar` & `xpanse-2.1.0rc1.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/docs/_source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/docs/_source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/_static/xpanse_banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/cover.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.asset_management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.attack_surface_rules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.incident_management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.261893 xpanse-2.0.0rc8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/examples/asset_management/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/asset_management/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/asset_management/get_services_by_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/asset_management/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/examples/incident_management/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/incident_management/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/incident_management/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/incident_management/update_incidents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/examples/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/tags/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/tags/assign_and_remove_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/tags/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/xpanse/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/asset_management/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/assets_management_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/owned_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/incident_management/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/incident_management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/v1/incidents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/incident_management/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/v2/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/tags/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/tags/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/tags/v1/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.974094 xpanse-2.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.958094 xpanse-2.1.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.962093 xpanse-2.1.0rc1/docs/_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.962093 xpanse-2.1.0rc1/docs/_source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/_static/xpanse_banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/cover.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/xpanse.api.asset_management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/xpanse.api.attack_surface_rules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/xpanse.api.incident_management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/xpanse.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/xpanse.api.tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/_source/xpanse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.958094 xpanse-2.1.0rc1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.962093 xpanse-2.1.0rc1/examples/asset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/asset_management/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/asset_management/get_services_by_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/asset_management/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.962093 xpanse-2.1.0rc1/examples/incident_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/incident_management/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/incident_management/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/incident_management/update_incidents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.962093 xpanse-2.1.0rc1/examples/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/tags/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/tags/assign_and_remove_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/examples/tags/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:31:30.974094 xpanse-2.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.966094 xpanse-2.1.0rc1/xpanse/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.966094 xpanse-2.1.0rc1/xpanse/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.966094 xpanse-2.1.0rc1/xpanse/api/asset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/asset_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/asset_management/assets_management_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/xpanse/api/asset_management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/asset_management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/asset_management/v1/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/asset_management/v1/owned_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/asset_management/v1/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/xpanse/api/attack_surface_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/attack_surface_rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/xpanse/api/attack_surface_rules/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/attack_surface_rules/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/xpanse/api/incident_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/incident_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/xpanse/api/incident_management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/incident_management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/incident_management/v1/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/incident_management/v1/incidents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/xpanse/api/incident_management/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/incident_management/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/incident_management/v2/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/xpanse/api/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.970094 xpanse-2.1.0rc1/xpanse/api/tags/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/tags/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/api/tags/v1/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-01 13:30:52.000000 xpanse-2.1.0rc1/xpanse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:31:30.966094 xpanse-2.1.0rc1/xpanse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-08-01 13:31:30.000000 xpanse-2.1.0rc1/xpanse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-08-01 13:31:30.000000 xpanse-2.1.0rc1/xpanse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:31:30.000000 xpanse-2.1.0rc1/xpanse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 13:31:30.000000 xpanse-2.1.0rc1/xpanse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 13:31:30.000000 xpanse-2.1.0rc1/xpanse.egg-info/top_level.txt
```

### Comparing `xpanse-2.0.0rc8/LICENSE` & `xpanse-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/PKG-INFO` & `xpanse-2.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanse
-Version: 2.0.0rc8
+Version: 2.1.0rc1
 Summary: Python library is an interface to the Cortex Xpanse API.
 Home-page: UNKNOWN
 Author: Palo Alto Cortex Xpanse
 Author-email: xpanse-integrations@paloaltonetworks.com
 License: ISC
 Keywords: xpanse iom
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc8 Summary: Python library is
+Metadata-Version: 2.1 Name: xpanse Version: 2.1.0rc1 Summary: Python library is
 an interface to the Cortex Xpanse API. Home-page: UNKNOWN Author: Palo Alto
 Cortex Xpanse Author-email: xpanse-integrations@paloaltonetworks.com License:
 ISC Keywords: xpanse iom Platform: UNKNOWN Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `xpanse-2.0.0rc8/README.md` & `xpanse-2.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/Makefile` & `xpanse-2.1.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/README.md` & `xpanse-2.1.0rc1/docs/README.md`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/_source/_static/xpanse_banner.png` & `xpanse-2.1.0rc1/docs/_source/_static/xpanse_banner.png`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/_source/conf.py` & `xpanse-2.1.0rc1/docs/_source/conf.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/_source/cover.rst` & `xpanse-2.1.0rc1/docs/_source/cover.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/_source/xpanse.api.asset_management.rst` & `xpanse-2.1.0rc1/docs/_source/xpanse.api.asset_management.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/_source/xpanse.api.incident_management.rst` & `xpanse-2.1.0rc1/docs/_source/xpanse.api.incident_management.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/_source/xpanse.api.rst` & `xpanse-2.1.0rc1/docs/_source/xpanse.api.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/_source/xpanse.rst` & `xpanse-2.1.0rc1/docs/_source/xpanse.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/docs/requirements-docs.txt` & `xpanse-2.1.0rc1/docs/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/examples/asset_management/get_services_by_asset.py` & `xpanse-2.1.0rc1/examples/asset_management/get_services_by_asset.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/examples/incident_management/update_incidents.py` & `xpanse-2.1.0rc1/examples/incident_management/update_incidents.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/examples/tags/assign_and_remove_tags.py` & `xpanse-2.1.0rc1/examples/tags/assign_and_remove_tags.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/setup.py` & `xpanse-2.1.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/asset_management/__init__.py` & `xpanse-2.1.0rc1/xpanse/api/asset_management/__init__.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/asset_management/assets_management_base.py` & `xpanse-2.1.0rc1/xpanse/api/asset_management/assets_management_base.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/asset_management/v1/assets.py` & `xpanse-2.1.0rc1/xpanse/api/asset_management/v1/assets.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/asset_management/v1/owned_ip_ranges.py` & `xpanse-2.1.0rc1/xpanse/api/asset_management/v1/owned_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/asset_management/v1/services.py` & `xpanse-2.1.0rc1/xpanse/api/asset_management/v1/services.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py` & `xpanse-2.1.0rc1/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/incident_management/__init__.py` & `xpanse-2.1.0rc1/xpanse/api/incident_management/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from xpanse.api.incident_management.v1.incidents import IncidentsEndpoint
 from xpanse.api.incident_management.v2.alerts import AlertsEndpoint
+from xpanse.api.incident_management.v1.alerts import AlertsEndpointV1
 
 
 class IncidentsApi(IncidentsEndpoint):
     def __init__(self, session):
         super().__init__(session)
 
     @property
@@ -22,7 +23,11 @@
     @property
     def current_version(self):
         return "v2"
 
     @property
     def v2(self):
         return AlertsEndpoint(self._api)
+
+    @property
+    def v1(self):
+        return AlertsEndpointV1(self._api)
```

### Comparing `xpanse-2.0.0rc8/xpanse/api/incident_management/v1/incidents.py` & `xpanse-2.1.0rc1/xpanse/api/incident_management/v1/incidents.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/incident_management/v2/alerts.py` & `xpanse-2.1.0rc1/xpanse/api/incident_management/v2/alerts.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/api/tags/v1/tags.py` & `xpanse-2.1.0rc1/xpanse/api/tags/v1/tags.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/client.py` & `xpanse-2.1.0rc1/xpanse/client.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/const.py` & `xpanse-2.1.0rc1/xpanse/const.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/endpoint.py` & `xpanse-2.1.0rc1/xpanse/endpoint.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/error.py` & `xpanse-2.1.0rc1/xpanse/error.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/iterator.py` & `xpanse-2.1.0rc1/xpanse/iterator.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/response.py` & `xpanse-2.1.0rc1/xpanse/response.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/types.py` & `xpanse-2.1.0rc1/xpanse/types.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse/utils.py` & `xpanse-2.1.0rc1/xpanse/utils.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc8/xpanse.egg-info/PKG-INFO` & `xpanse-2.1.0rc1/xpanse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanse
-Version: 2.0.0rc8
+Version: 2.1.0rc1
 Summary: Python library is an interface to the Cortex Xpanse API.
 Home-page: UNKNOWN
 Author: Palo Alto Cortex Xpanse
 Author-email: xpanse-integrations@paloaltonetworks.com
 License: ISC
 Keywords: xpanse iom
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc8 Summary: Python library is
+Metadata-Version: 2.1 Name: xpanse Version: 2.1.0rc1 Summary: Python library is
 an interface to the Cortex Xpanse API. Home-page: UNKNOWN Author: Palo Alto
 Cortex Xpanse Author-email: xpanse-integrations@paloaltonetworks.com License:
 ISC Keywords: xpanse iom Platform: UNKNOWN Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `xpanse-2.0.0rc8/xpanse.egg-info/SOURCES.txt` & `xpanse-2.1.0rc1/xpanse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,13 +46,14 @@
 xpanse/api/asset_management/v1/owned_ip_ranges.py
 xpanse/api/asset_management/v1/services.py
 xpanse/api/attack_surface_rules/__init__.py
 xpanse/api/attack_surface_rules/v1/__init__.py
 xpanse/api/attack_surface_rules/v1/attack_surface_rules.py
 xpanse/api/incident_management/__init__.py
 xpanse/api/incident_management/v1/__init__.py
+xpanse/api/incident_management/v1/alerts.py
 xpanse/api/incident_management/v1/incidents.py
 xpanse/api/incident_management/v2/__init__.py
 xpanse/api/incident_management/v2/alerts.py
 xpanse/api/tags/__init__.py
 xpanse/api/tags/v1/__init__.py
 xpanse/api/tags/v1/tags.py
```

