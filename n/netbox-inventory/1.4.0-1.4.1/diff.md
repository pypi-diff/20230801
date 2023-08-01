# Comparing `tmp/netbox-inventory-1.4.0.tar.gz` & `tmp/netbox-inventory-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.4.0.tar", last modified: Wed Jul 26 12:59:12 2023, max compression
+gzip compressed data, was "netbox-inventory-1.4.1.tar", last modified: Tue Aug  1 11:42:02 2023, max compression
```

## Comparing `netbox-inventory-1.4.0.tar` & `netbox-inventory-1.4.1.tar`

### file list

```diff
@@ -1,116 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.170005 netbox-inventory-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-26 12:59:12.170005 netbox-inventory-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.146005 netbox-inventory-1.4.0/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.150005 netbox-inventory-1.4.0/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    14749 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.150005 netbox-inventory-1.4.0/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/forms/reassign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.154005 netbox-inventory-1.4.0/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18297 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.142005 netbox-inventory-1.4.0/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.154005 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/delivery.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.154005 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.158005 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.158005 netbox-inventory-1.4.0/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.158005 netbox-inventory-1.4.0/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.162005 netbox-inventory-1.4.0/netbox_inventory/tests/delivery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/delivery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/delivery/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/delivery/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.162005 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.162005 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.162005 netbox-inventory-1.4.0/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.166005 netbox-inventory-1.4.0/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.166005 netbox-inventory-1.4.0/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:59:12.146005 netbox-inventory-1.4.0/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-26 12:59:12.000000 netbox-inventory-1.4.0/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-26 12:59:12.000000 netbox-inventory-1.4.0/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:59:12.000000 netbox-inventory-1.4.0/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 12:59:12.000000 netbox-inventory-1.4.0/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-26 12:58:59.000000 netbox-inventory-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:59:12.170005 netbox-inventory-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.052806 netbox-inventory-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-08-01 11:42:02.052806 netbox-inventory-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.040804 netbox-inventory-1.4.1/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.044805 netbox-inventory-1.4.1/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14749 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.044805 netbox-inventory-1.4.1/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/forms/reassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.044805 netbox-inventory-1.4.1/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/migrations/0005_delivery_asset_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.040804 netbox-inventory-1.4.1/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.048805 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/delivery.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.048805 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.048805 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.048805 netbox-inventory-1.4.1/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.048805 netbox-inventory-1.4.1/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.048805 netbox-inventory-1.4.1/netbox_inventory/tests/delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/delivery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/delivery/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/delivery/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.052806 netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.052806 netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.052806 netbox-inventory-1.4.1/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.052806 netbox-inventory-1.4.1/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.052806 netbox-inventory-1.4.1/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:42:02.044805 netbox-inventory-1.4.1/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-08-01 11:42:02.000000 netbox-inventory-1.4.1/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-01 11:42:02.000000 netbox-inventory-1.4.1/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:42:02.000000 netbox-inventory-1.4.1/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:42:02.000000 netbox-inventory-1.4.1/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:41:45.000000 netbox-inventory-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:42:02.052806 netbox-inventory-1.4.1/setup.cfg
```

### Comparing `netbox-inventory-1.4.0/LICENSE` & `netbox-inventory-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/PKG-INFO` & `netbox-inventory-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.4.0
+Version: 1.4.1
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -166,14 +166,15 @@
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 | `asset_custom_fields_search_filters` | `{}` | A dictionary of custom fields and lookup types that will be added to the search filters for assets. The dictionary is in the form of `{field: [lookup_type]}`. Example: `{'asset_mac': ['icontains', 'exact']}`. |
+| `asset_warranty_expire_warning_days` | `90` | Days from warranty expiration to show as warning in Warranty remaining field |
 | `prefill_asset_name_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the InventoryItem name to match the asset name. |
 | `prefill_asset_tag_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the tags to match the tags associated to the asset. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
```

### Comparing `netbox-inventory-1.4.0/README.md` & `netbox-inventory-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 | `asset_custom_fields_search_filters` | `{}` | A dictionary of custom fields and lookup types that will be added to the search filters for assets. The dictionary is in the form of `{field: [lookup_type]}`. Example: `{'asset_mac': ['icontains', 'exact']}`. |
+| `asset_warranty_expire_warning_days` | `90` | Days from warranty expiration to show as warning in Warranty remaining field |
 | `prefill_asset_name_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the InventoryItem name to match the asset name. |
 | `prefill_asset_tag_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the tags to match the tags associated to the asset. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/__init__.py` & `netbox-inventory-1.4.1/netbox_inventory/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         'asset_import_create_device_type': False,
         'asset_import_create_module_type': False,
         'asset_import_create_inventoryitem_type': False,
         'asset_import_create_tenant': False,
         'asset_disable_editing_fields_for_tags': {},
         'asset_disable_deletion_for_tags': [],
         'asset_custom_fields_search_filters': {},
+        'asset_warranty_expire_warning_days': 90,
         'prefill_asset_name_create_inventoryitem': False,
         'prefill_asset_tag_create_inventoryitem': False,
     }
 
     def ready(self):
         super().ready()
         import netbox_inventory.signals
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/analyzers.py` & `netbox-inventory-1.4.1/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.4.1/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/api/serializers.py` & `netbox-inventory-1.4.1/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/api/urls.py` & `netbox-inventory-1.4.1/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/api/views.py` & `netbox-inventory-1.4.1/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/filtersets.py` & `netbox-inventory-1.4.1/netbox_inventory/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/forms/assign.py` & `netbox-inventory-1.4.1/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.4.1/netbox_inventory/forms/bulk.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/forms/bulk_add.py` & `netbox-inventory-1.4.1/netbox_inventory/forms/bulk_add.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/forms/create.py` & `netbox-inventory-1.4.1/netbox_inventory/forms/create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/forms/filters.py` & `netbox-inventory-1.4.1/netbox_inventory/forms/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/forms/models.py` & `netbox-inventory-1.4.1/netbox_inventory/forms/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/forms/reassign.py` & `netbox-inventory-1.4.1/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.4.1/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.4.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.4.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py` & `netbox-inventory-1.4.1/netbox_inventory/migrations/0005_delivery_asset_delivery.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/models.py` & `netbox-inventory-1.4.1/netbox_inventory/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,22 +242,19 @@
         else:
             return None
 
     @property
     def warranty_remaining(self):
         """
             How many days are left in warranty period.
-            Returns negative duration if period has not started yet
+            Returns negative duration if warranty expired
             Return None if warranty_end not defined
         """
         if self.warranty_end:
-            if self.warranty_start and self.warranty_start > date.today():
-                return date.today() - self.warranty_start
-            else:
-                return self.warranty_end - date.today()
+            return self.warranty_end - date.today()
         return None
 
     @property
     def warranty_elapsed(self):
         """
             How many days have passed in warranty period.
             Returns negative duration if period has not started yet
@@ -269,14 +266,25 @@
 
     @property
     def warranty_total(self):
         if self.warranty_end and self.warranty_start:
             return self.warranty_end - self.warranty_start
         return None
 
+    @property
+    def warranty_progress(self):
+        """
+        Percentage of warranty elapsed
+        Returns > 100 if warranty has expired, < 0 if not started yet and None
+        if warranty_start or warranty_end not set.
+        """
+        if not self.warranty_start or not self.warranty_end:
+            return None
+        return int(100 * (self.warranty_elapsed / self.warranty_total))
+
     def clean(self):
         self.clean_delivery()
         self.validate_hardware_types()
         self.validate_hardware()
         self.update_status()
         return super().clean()
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/navigation.py` & `netbox-inventory-1.4.1/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/search.py` & `netbox-inventory-1.4.1/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/signals.py` & `netbox-inventory-1.4.1/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tables.py` & `netbox-inventory-1.4.1/netbox_inventory/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.db.models.functions import Coalesce
 import django_tables2 as tables
 
 from netbox.tables import columns, NetBoxTable
 from tenancy.tables import ContactsColumnMixin
 from .models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
+from .template_content import WARRANTY_PROGRESSBAR
 
 __all__ = (
     'AssetTable',
     'SupplierTable',
     'PurchaseTable',
     'DeliveryTable',
     'InventoryItemTypeTable',
@@ -85,14 +86,21 @@
     purchase_date = columns.DateColumn(
         accessor='purchase__date',
         verbose_name='Purchase Date',
     )
     delivery_date = columns.DateColumn(
         accessor='delivery__date',
         verbose_name='Delivery Date',
+
+    )
+    warranty_progress = columns.TemplateColumn(
+        template_code=WARRANTY_PROGRESSBAR,
+        order_by='warranty_end',
+        #orderable=False,
+        verbose_name='Warranty remaining',
     )
     comments = columns.MarkdownColumn()
     tags = columns.TagColumn()
     actions = columns.ActionsColumn(
         extra_buttons="""
             {% if record.hardware %}
             <a href="#" class="btn btn-sm btn-outline-dark disabled">
@@ -226,14 +234,15 @@
             'supplier',
             'purchase',
             'delivery',
             'purchase_date',
             'delivery_date',
             'warranty_start',
             'warranty_end',
+            'warranty_progress',
             'comments',
             'tags',
             'created',
             'last_updated',
             'actions',
         )
         default_columns = (
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             <tr>
               <th scope="row">Warranty end</th>
               <td>{{ object.warranty_end|annotated_date|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Warranty remaining</th>
               <td>
-                {% include "netbox_inventory/inc/asset_warranty.html" with asset=object %}
+                {% include warranty_progressbar with record=object %}
               </td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
```

#### html2text {}

```diff
@@ -51,14 +51,13 @@
 Purchase           object.purchase.date %} on {
                    { object.purchase.date|annotated_date }}{% endif %}
                    {{ object.delivery|linkify:'name'|placeholder }}{% if
 Delivery           object.delivery.date %} on {
                    { object.delivery.date|annotated_date }}{% endif %}
 Warranty start     {{ object.warranty_start|annotated_date|placeholder }}
 Warranty end       {{ object.warranty_end|annotated_date|placeholder }}
-Warranty remaining {% include "netbox_inventory/inc/asset_warranty.html" with
-                   asset=object %}
+Warranty remaining {% include warranty_progressbar with record=object %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% include 'inc/panels/image_attachments.html' %} {% plugin_right_page object
 %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_edit.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/delivery.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/delivery.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       <tr>
         <th scope="row">Purchase</th>
         <td>{{ asset.purchase|linkify|placeholder }}</td>
       </tr>
       <tr>
         <th>Warranty remaining</th>
         <td>
-          {% include "netbox_inventory/inc/asset_warranty.html" with asset=asset %}
+          {% include warranty_progressbar with record=asset %}
         </td>
       </tr>
     </table>
   {% else %}
     <div class="text-muted">None assigned</div>
   {% endif %}
   </div>
```

#### html2text {}

```diff
@@ -3,16 +3,15 @@
 {% if asset %}
 Name                asset.pk %}">{{ asset.hardware_type.manufacturer }} {
                    { asset }}{% if asset.name %} ({{ asset.name }}){% endif %}
 Status             {% badge asset.get_status_display
                    bg_color=asset.get_status_color %}
 Owner              {{ asset.owner|linkify|placeholder }}
 Purchase           {{ asset.purchase|linkify|placeholder }}
-Warranty remaining {% include "netbox_inventory/inc/asset_warranty.html" with
-                   asset=asset %}
+Warranty remaining {% include warranty_progressbar with record=asset %}
 {% else %}
 None assigned
 {% endif %}
 {# only show reassign button if user has change permissions on asset #} {% if
 perms.netbox_inventory.change_asset %} {% with object|meta:"model_name" as
 object_type %} {% if object_type == "device" %} {%_elif_object_type_==_"module"
 %}_{%_elif_object_type_==_"inventoryitem"_%}_{%_endif_%}_{%_endwith_%}__Edit
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.4.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views_create.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/custom.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/delivery/test_api.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/delivery/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/delivery/test_views.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/delivery/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/settings.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.4.1/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.4.0"
+        assert __version__ == "1.4.1"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/urls.py` & `netbox-inventory-1.4.1/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/utils.py` & `netbox-inventory-1.4.1/netbox_inventory/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,14 @@
 from django.core.exceptions import ImproperlyConfigured
 from django.db.models.signals import pre_save
 
 from dcim.models import Device, Module, InventoryItem
 from .choices import AssetStatusChoices
 
 
-def get_asset_warranty_context(asset):
-    warranty_progress = None
-    bar_class = 'bg-success'
-    if asset.warranty_elapsed and asset.warranty_elapsed.total_seconds() > 0 and asset.warranty_total:
-        warranty_progress = asset.warranty_elapsed / asset.warranty_total
-    if warranty_progress is not None:
-        warranty_progress = warranty_progress * 100
-        if asset.warranty_remaining.days < 7:
-            bar_class = 'bg-danger'
-        elif asset.warranty_remaining.days < 30:
-            bar_class = 'bg-warning'
-    return dict(
-        warranty_progress=warranty_progress,
-        bar_class=bar_class
-    )
-
-
 def get_prechange_field(obj, field_name):
     """Get value from obj._prechange_snapshot. If field is a relation,
     return object instance.
     """
     value = getattr(obj, '_prechange_snapshot', {}).get(field_name)
     if value is None:
         return None
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/asset.py` & `netbox-inventory-1.4.1/netbox_inventory/views/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 
 from django.contrib import messages
 from django.db import IntegrityError
 from django.shortcuts import redirect
+from django.template import Template
 from netbox.views import generic
 from utilities.forms import ConfirmationForm, restrict_form_fields
 
 from .. import filtersets, forms, models, tables
+from ..template_content import WARRANTY_PROGRESSBAR
 from ..utils import (
-    get_asset_warranty_context,
     get_tags_and_edit_protected_asset_fields,
     get_tags_that_protect_asset_from_deletion,
 )
 
 __all__ = (
     'AssetView',
     'AssetListView',
@@ -26,15 +27,15 @@
 
 
 class AssetView(generic.ObjectView):
     queryset = models.Asset.objects.all()
 
     def get_extra_context(self, request, instance):
         context = super().get_extra_context(request, instance)
-        context.update(get_asset_warranty_context(instance))
+        context['warranty_progressbar'] = Template(WARRANTY_PROGRESSBAR)
         return context
 
 
 class AssetListView(generic.ObjectListView):
     queryset = models.Asset.objects.prefetch_related(
         'device_type__manufacturer',
         'module_type__manufacturer',
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.4.1/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.4.1/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/asset_reassign.py` & `netbox-inventory-1.4.1/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/delivery.py` & `netbox-inventory-1.4.1/netbox_inventory/views/delivery.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/inventoryitem_group.py` & `netbox-inventory-1.4.1/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.4.1/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/purchase.py` & `netbox-inventory-1.4.1/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/supplier.py` & `netbox-inventory-1.4.1/netbox_inventory/views/supplier.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory/views/tabs.py` & `netbox-inventory-1.4.1/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.4.0/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.4.1/netbox_inventory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.4.0
+Version: 1.4.1
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -166,14 +166,15 @@
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 | `asset_custom_fields_search_filters` | `{}` | A dictionary of custom fields and lookup types that will be added to the search filters for assets. The dictionary is in the form of `{field: [lookup_type]}`. Example: `{'asset_mac': ['icontains', 'exact']}`. |
+| `asset_warranty_expire_warning_days` | `90` | Days from warranty expiration to show as warning in Warranty remaining field |
 | `prefill_asset_name_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the InventoryItem name to match the asset name. |
 | `prefill_asset_tag_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the tags to match the tags associated to the asset. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
```

### Comparing `netbox-inventory-1.4.0/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.4.1/netbox_inventory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
 netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
 netbox_inventory/templates/netbox_inventory/purchase.html
 netbox_inventory/templates/netbox_inventory/supplier.html
 netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
 netbox_inventory/templates/netbox_inventory/inc/asset_info.html
 netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
-netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
 netbox_inventory/tests/__init__.py
 netbox_inventory/tests/custom.py
 netbox_inventory/tests/settings.py
```

### Comparing `netbox-inventory-1.4.0/pyproject.toml` & `netbox-inventory-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

