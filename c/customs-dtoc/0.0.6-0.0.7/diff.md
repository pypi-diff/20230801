# Comparing `tmp/customs_dtoc-0.0.6.tar.gz` & `tmp/customs_dtoc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customs_dtoc-0.0.6.tar", last modified: Sun Jul 30 13:55:15 2023, max compression
+gzip compressed data, was "customs_dtoc-0.0.7.tar", last modified: Tue Aug  1 11:07:59 2023, max compression
```

## Comparing `customs_dtoc-0.0.6.tar` & `customs_dtoc-0.0.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.960966 customs_dtoc-0.0.6/
--rw-rw-rw-   0        0        0     1083 2023-07-22 15:27:03.000000 customs_dtoc-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3053 2023-07-30 13:55:15.960966 customs_dtoc-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2334 2023-07-30 12:38:03.000000 customs_dtoc-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-30 13:55:15.960966 customs_dtoc-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1050 2023-07-30 13:54:25.000000 customs_dtoc-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.333769 customs_dtoc-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.521272 customs_dtoc-0.0.6/src/customs_dtoc/
--rw-rw-rw-   0        0        0     1388 2023-07-30 13:12:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.599394 customs_dtoc-0.0.6/src/customs_dtoc/csf/
--rw-rw-rw-   0        0        0       57 2023-07-23 10:17:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/csf/__init__.py
--rw-rw-rw-   0        0        0     1217 2023-07-22 15:27:03.000000 customs_dtoc-0.0.6/src/customs_dtoc/csf/csf.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.599394 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/
--rw-rw-rw-   0        0        0      978 2023-07-30 13:12:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.615021 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/
--rw-rw-rw-   0        0        0      956 2023-07-30 13:15:53.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.615021 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/
--rw-rw-rw-   0        0        0      380 2023-07-30 11:15:51.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.630646 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/outports/
--rw-rw-rw-   0        0        0       85 2023-07-30 11:15:51.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/outports/__init__.py
--rw-rw-rw-   0        0        0      931 2023-07-30 11:53:46.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/outports/ac_outports.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.646271 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/
--rw-rw-rw-   0        0        0      355 2023-07-23 10:17:45.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.661898 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/
--rw-rw-rw-   0        0        0      135 2023-07-23 10:17:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/__init__.py
--rw-rw-rw-   0        0        0     2383 2023-07-30 12:32:55.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.661898 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/
--rw-rw-rw-   0        0        0      150 2023-07-23 10:29:01.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/__init__.py
--rw-rw-rw-   0        0        0     2996 2023-07-30 12:20:55.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/full_containerized_cargo.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.677520 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/lcl/
--rw-rw-rw-   0        0        0      105 2023-07-23 10:17:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/lcl/__init__.py
--rw-rw-rw-   0        0        0     5232 2023-07-30 12:52:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/lcl/bulk_break_bulk_cargo.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.693146 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/bc/
--rw-rw-rw-   0        0        0       35 2023-07-23 10:17:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/bc/__init__.py
--rw-rw-rw-   0        0        0      295 2023-07-30 10:55:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/bc/bc.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.708769 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/bf/
--rw-rw-rw-   0        0        0       61 2023-07-23 10:17:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/bf/__init__.py
--rw-rw-rw-   0        0        0     1547 2023-07-30 10:55:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/bf/bf_formal_entry.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.724396 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/cds/
--rw-rw-rw-   0        0        0       49 2023-07-23 10:17:48.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/cds/__init__.py
--rw-rw-rw-   0        0        0      438 2023-07-30 10:55:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/cds/cds.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.740020 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/cud/
--rw-rw-rw-   0        0        0       37 2023-07-23 10:17:46.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/cud/__init__.py
--rw-rw-rw-   0        0        0      373 2023-07-22 15:27:03.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/cud/cud.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.755645 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/dv/
--rw-rw-rw-   0        0        0       70 2023-07-23 10:17:46.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/dv/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-07-30 10:55:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/dv/dv.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.771273 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ipf/
--rw-rw-rw-   0        0        0       45 2023-07-23 10:17:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ipf/__init__.py
--rw-rw-rw-   0        0        0      873 2023-07-30 10:55:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ipf/ipf.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.771273 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/
--rw-rw-rw-   0        0        0      338 2023-07-30 13:12:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.786897 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/outports/
--rw-rw-rw-   0        0        0       95 2023-07-30 13:12:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/outports/__init__.py
--rw-rw-rw-   0        0        0      858 2023-07-30 13:12:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/outports/wharfage_due_outports.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.802521 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/
--rw-rw-rw-   0        0        0      313 2023-07-23 10:17:46.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.818151 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/
--rw-rw-rw-   0        0        0      135 2023-07-23 10:19:01.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-07-30 13:13:40.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.833772 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/
--rw-rw-rw-   0        0        0      230 2023-07-23 10:19:01.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/__init__.py
--rw-rw-rw-   0        0        0     2132 2023-07-30 13:14:38.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/full_containerized_load.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.849400 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/lcl/
--rw-rw-rw-   0        0        0      105 2023-07-23 10:17:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/lcl/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-07-30 13:12:36.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/lcl/bulk_break_bulk_cargo.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.849400 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/
--rw-rw-rw-   0        0        0      167 2023-07-23 10:17:46.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.865023 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/formal_entry/
--rw-rw-rw-   0        0        0      109 2023-07-23 10:29:01.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/formal_entry/__init__.py
--rw-rw-rw-   0        0        0     1905 2023-07-22 15:27:03.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/formal_entry/lc_via_formal_entry.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.865023 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/informal_entry/
--rw-rw-rw-   0        0        0       70 2023-07-23 10:29:01.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/informal_entry/__init__.py
--rw-rw-rw-   0        0        0      666 2023-07-22 15:27:03.000000 customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/informal_entry/lc_via_informal_entry.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.892943 customs_dtoc-0.0.6/src/customs_dtoc/pro_rata/
--rw-rw-rw-   0        0        0      167 2023-07-23 10:17:47.000000 customs_dtoc-0.0.6/src/customs_dtoc/pro_rata/__init__.py
--rw-rw-rw-   0        0        0     2025 2023-07-22 15:27:03.000000 customs_dtoc-0.0.6/src/customs_dtoc/pro_rata/pro_rata.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.905945 customs_dtoc-0.0.6/src/customs_dtoc/sop/
--rw-rw-rw-   0        0        0      147 2023-07-23 10:17:48.000000 customs_dtoc-0.0.6/src/customs_dtoc/sop/__init__.py
--rw-rw-rw-   0        0        0     2908 2023-07-22 15:27:03.000000 customs_dtoc-0.0.6/src/customs_dtoc/sop/sop.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.918946 customs_dtoc-0.0.6/src/customs_dtoc/vat/
--rw-rw-rw-   0        0        0       62 2023-07-23 10:17:48.000000 customs_dtoc-0.0.6/src/customs_dtoc/vat/__init__.py
--rw-rw-rw-   0        0        0      753 2023-07-28 15:53:22.000000 customs_dtoc-0.0.6/src/customs_dtoc/vat/vat.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.583768 customs_dtoc-0.0.6/src/customs_dtoc.egg-info/
--rw-rw-rw-   0        0        0     3053 2023-07-30 13:55:15.000000 customs_dtoc-0.0.6/src/customs_dtoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-07-30 13:55:15.000000 customs_dtoc-0.0.6/src/customs_dtoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 13:55:15.000000 customs_dtoc-0.0.6/src/customs_dtoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-30 13:55:15.000000 customs_dtoc-0.0.6/src/customs_dtoc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 13:55:15.945333 customs_dtoc-0.0.6/tests/
--rw-rw-rw-   0        0        0      572 2023-07-30 12:47:49.000000 customs_dtoc-0.0.6/tests/test_csf.py
--rw-rw-rw-   0        0        0     1364 2023-07-30 12:47:48.000000 customs_dtoc-0.0.6/tests/test_landed_cost.py
--rw-rw-rw-   0        0        0     1625 2023-07-30 12:47:48.000000 customs_dtoc-0.0.6/tests/test_pro_rata.py
--rw-rw-rw-   0        0        0     1464 2023-07-30 12:47:48.000000 customs_dtoc-0.0.6/tests/test_sop.py
--rw-rw-rw-   0        0        0      556 2023-07-30 12:47:48.000000 customs_dtoc-0.0.6/tests/test_vat.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:59.875703 customs_dtoc-0.0.7/
+-rw-rw-rw-   0        0        0     1083 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3053 2023-08-01 11:07:59.875703 customs_dtoc-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2334 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 11:07:59.891332 customs_dtoc-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2023-08-01 10:27:53.000000 customs_dtoc-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.211643 customs_dtoc-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.383517 customs_dtoc-0.0.7/src/customs_dtoc/
+-rw-rw-rw-   0        0        0     1388 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.524143 customs_dtoc-0.0.7/src/customs_dtoc/csf/
+-rw-rw-rw-   0        0        0       57 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/csf/__init__.py
+-rw-rw-rw-   0        0        0     1217 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/csf/csf.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.539768 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/
+-rw-rw-rw-   0        0        0      978 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.555397 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/
+-rw-rw-rw-   0        0        0      956 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.586642 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/
+-rw-rw-rw-   0        0        0      380 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.633521 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/outports/
+-rw-rw-rw-   0        0        0       85 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/outports/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/outports/ac_outports.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.664771 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/
+-rw-rw-rw-   0        0        0      355 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.711646 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/
+-rw-rw-rw-   0        0        0      135 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/__init__.py
+-rw-rw-rw-   0        0        0     1662 2023-08-01 09:50:49.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.727267 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/
+-rw-rw-rw-   0        0        0      145 2023-08-01 08:46:15.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/__init__.py
+-rw-rw-rw-   0        0        0     2257 2023-08-01 10:57:35.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/containerized_cargo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.742895 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/lcl/
+-rw-rw-rw-   0        0        0      105 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/lcl/__init__.py
+-rw-rw-rw-   0        0        0     1583 2023-08-01 08:38:13.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/lcl/bulk_break_bulk_cargo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.789769 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/bc/
+-rw-rw-rw-   0        0        0       35 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/bc/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/bc/bc.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.852271 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/bf/
+-rw-rw-rw-   0        0        0       61 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/bf/__init__.py
+-rw-rw-rw-   0        0        0     1547 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/bf/bf_formal_entry.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.899141 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/cds/
+-rw-rw-rw-   0        0        0       49 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/cds/__init__.py
+-rw-rw-rw-   0        0        0      549 2023-08-01 10:25:49.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/cds/cds.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.930396 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/cud/
+-rw-rw-rw-   0        0        0       37 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/cud/__init__.py
+-rw-rw-rw-   0        0        0      373 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/cud/cud.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.992894 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/dv/
+-rw-rw-rw-   0        0        0       70 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/dv/__init__.py
+-rw-rw-rw-   0        0        0      920 2023-08-01 10:25:49.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/dv/dv.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.024140 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ipf/
+-rw-rw-rw-   0        0        0       45 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ipf/__init__.py
+-rw-rw-rw-   0        0        0      873 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ipf/ipf.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.051338 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/
+-rw-rw-rw-   0        0        0      338 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.129462 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/outports/
+-rw-rw-rw-   0        0        0       95 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/outports/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/outports/wharfage_due_outports.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.160715 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/
+-rw-rw-rw-   0        0        0      313 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.284151 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/
+-rw-rw-rw-   0        0        0      135 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.397114 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/
+-rw-rw-rw-   0        0        0      226 2023-08-01 10:57:36.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-08-01 10:57:36.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/containerized_cargo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.584622 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/lcl/
+-rw-rw-rw-   0        0        0      105 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/lcl/__init__.py
+-rw-rw-rw-   0        0        0     1233 2023-08-01 10:58:42.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/lcl/bulk_break_bulk_cargo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.700525 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/
+-rw-rw-rw-   0        0        0      167 2023-07-30 14:42:54.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:58.919285 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/formal_entry/
+-rw-rw-rw-   0        0        0      109 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/formal_entry/__init__.py
+-rw-rw-rw-   0        0        0     1905 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/formal_entry/lc_via_formal_entry.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:59.013035 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/informal_entry/
+-rw-rw-rw-   0        0        0       70 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/informal_entry/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/informal_entry/lc_via_informal_entry.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:59.231922 customs_dtoc-0.0.7/src/customs_dtoc/pro_rata/
+-rw-rw-rw-   0        0        0      167 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/pro_rata/__init__.py
+-rw-rw-rw-   0        0        0     2025 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/pro_rata/pro_rata.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:59.419428 customs_dtoc-0.0.7/src/customs_dtoc/sop/
+-rw-rw-rw-   0        0        0      147 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/sop/__init__.py
+-rw-rw-rw-   0        0        0     2910 2023-08-01 10:27:53.000000 customs_dtoc-0.0.7/src/customs_dtoc/sop/sop.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:59.560059 customs_dtoc-0.0.7/src/customs_dtoc/vat/
+-rw-rw-rw-   0        0        0       62 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/vat/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/src/customs_dtoc/vat/vat.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:57.446016 customs_dtoc-0.0.7/src/customs_dtoc.egg-info/
+-rw-rw-rw-   0        0        0     3053 2023-08-01 11:07:57.000000 customs_dtoc-0.0.7/src/customs_dtoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3374 2023-08-01 11:07:57.000000 customs_dtoc-0.0.7/src/customs_dtoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 11:07:57.000000 customs_dtoc-0.0.7/src/customs_dtoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 11:07:57.000000 customs_dtoc-0.0.7/src/customs_dtoc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 11:07:59.875703 customs_dtoc-0.0.7/tests/
+-rw-rw-rw-   0        0        0      572 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/tests/test_csf.py
+-rw-rw-rw-   0        0        0     1364 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/tests/test_landed_cost.py
+-rw-rw-rw-   0        0        0     1625 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/tests/test_pro_rata.py
+-rw-rw-rw-   0        0        0     1464 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/tests/test_sop.py
+-rw-rw-rw-   0        0        0      556 2023-07-30 14:42:55.000000 customs_dtoc-0.0.7/tests/test_vat.py
```

### Comparing `customs_dtoc-0.0.6/LICENSE` & `customs_dtoc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/PKG-INFO` & `customs_dtoc-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customs_dtoc
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for calculating customs duties, taxes, and other charges.
 Home-page: https://github.com/iaaan05/python-customs-tax-package
 Author: Iaaan05
 Author-email: iaaan100500@gmail.com
 License: MIT
 Keywords: customs,duties,taxes,charges
 Classifier: Intended Audience :: Information Technology
```

### Comparing `customs_dtoc-0.0.6/README.md` & `customs_dtoc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/setup.py` & `customs_dtoc-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='customs_dtoc',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[],
     python_requires='>=3.11',
     license='MIT',
     author='Iaaan05',
     author_email='iaaan100500@gmail.com',
```

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/__init__.py` & `customs_dtoc-0.0.7/src/customs_dtoc/__init__.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/csf/csf.py` & `customs_dtoc-0.0.7/src/customs_dtoc/csf/csf.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/__init__.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/__init__.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/__init__.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/__init__.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/outports/ac_outports.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/outports/ac_outports.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,38 @@
+import json
+
+
+def get_rate_for_dangerous_cargo(class_dangerous_cargo: str, file_name: str) -> float:
+    with open(file_name, 'r') as f:
+        rates = json.load(f)
+    return rates.get(class_dangerous_cargo, 0.0)
+
+
 class ContainerizedDangerousCargoClass:
+    CLASS_DANGEROUS_CARGO = {
+        1.0: 'Class 1, 6, and 8', 2.0: 'Class 2, 3, 4, and 7', 3.0: 'Class 5 and 9'
+    }
+
     def __init__(self, classification_of_dangerous_cargo: float, total_number_of_containers: float) -> None:
-        self.classification_of_dangerous_cargo = classification_of_dangerous_cargo
+        self.class_dangerous_cargo = classification_of_dangerous_cargo
         self.total_number_of_containers = total_number_of_containers
         self.ac_rate = float
-        self.class_1_6_8 = 1
-        self.class_2_3_4_7 = 2
-        self.class_5_9 = 3
 
     def calculate_fcl_footer(self, ac_rate) -> float:
         total_ac = round(
             self.total_number_of_containers * ac_rate, 2
         )
         return total_ac
 
 
 class ACContainerizedDangerousCargo20Footer(ContainerizedDangerousCargoClass):
-    def __init__(self, classification_of_dangerous_cargo: float, total_number_of_containers: float) -> None:
-        super().__init__(classification_of_dangerous_cargo, total_number_of_containers)
-        self.class_1_6_8_rate = 5590.50
-        self.class_2_3_4_7_rate = 4658.75
-        self.class_5_9_rate = 4099.70
-
     def calculate_fcl_20_footer(self) -> float:
-        if self.classification_of_dangerous_cargo == self.class_1_6_8:
-            self.ac_rate = self.class_1_6_8_rate
-
-        elif self.classification_of_dangerous_cargo == self.class_2_3_4_7:
-            self.ac_rate = self.class_2_3_4_7_rate
-
-        elif self.classification_of_dangerous_cargo == self.class_5_9:
-            self.ac_rate = self.class_5_9_rate
-
+        class_dangerous_cargo = ContainerizedDangerousCargoClass.CLASS_DANGEROUS_CARGO[self.class_dangerous_cargo]
+        self.ac_rate = get_rate_for_dangerous_cargo(class_dangerous_cargo, '20_footer_rates.json')
         return self.calculate_fcl_footer(self.ac_rate)
 
 
 class ACContainerizedDangerousCargo40Footer(ContainerizedDangerousCargoClass):
-    def __init__(self, classification_of_dangerous_cargo: float, total_number_of_containers: float) -> None:
-        super().__init__(classification_of_dangerous_cargo, total_number_of_containers)
-        self.class_1_6_8_rate = 12826.00
-        self.class_2_3_4_7_rate = 10688.75
-        self.class_5_9_rate = 9406.10
-
     def calculate_fcl_40_footer(self) -> float:
-        if self.classification_of_dangerous_cargo == self.class_1_6_8:
-            self.ac_rate = self.class_1_6_8_rate
-
-        elif self.classification_of_dangerous_cargo == self.class_2_3_4_7:
-            self.ac_rate = self.class_2_3_4_7_rate
-
-        elif self.classification_of_dangerous_cargo == self.class_5_9:
-            self.ac_rate = self.class_5_9_rate
-
+        class_dangerous_cargo = ContainerizedDangerousCargoClass.CLASS_DANGEROUS_CARGO[self.class_dangerous_cargo]
+        self.ac_rate = get_rate_for_dangerous_cargo(class_dangerous_cargo, '40_footer_rates.json')
         return self.calculate_fcl_footer(self.ac_rate)
```

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/bf/bf_formal_entry.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/bf/bf_formal_entry.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/dv/dv.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/dv/dv.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,22 +14,14 @@
             self.fob_fca_value, self.dutiable_ins, self.dutiable_frt,
         )
         dutiable_value = round(math.fsum(dutiable_value) * self.rate_of_exchange, 2)
         return dutiable_value
 
 
 class DutiableValueBySea(DutiableValue):
-    def __init__(self, fob_fca_value: float, dutiable_ins: float, dutiable_frt: float,
-                 rate_of_exchange: float) -> None:
-        super().__init__(fob_fca_value, dutiable_ins, dutiable_frt, rate_of_exchange)
-
     def calculate_dutiable_value_by_sea(self):
         return self.calculate_dutiable_value()
 
 
 class DutiableValueByAir(DutiableValue):
-    def __init__(self, fob_fca_value: float, dutiable_ins: float, dutiable_frt: float,
-                 rate_of_exchange: float) -> None:
-        super().__init__(fob_fca_value, dutiable_ins, dutiable_frt, rate_of_exchange)
-
     def calculate_dutiable_value_by_air(self):
         return self.calculate_dutiable_value()
```

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/ipf/ipf.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/ipf/ipf.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/outports/wharfage_due_outports.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/outports/wharfage_due_outports.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/full_containerized_load.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/containerized_cargo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,38 @@
+import json
+
+
+def get_rate_of_container_size(container_size: str, file_name: str) -> float:
+    with open(file_name, 'r') as f:
+        rates = json.load(f)
+    return rates.get(container_size, 0.0)
+
+
 class WDContainerizedCargo:
+    CONTAINER_SIZE = {
+        20.0: 'Twenty Footer', 40.0: 'Forty Footer', 45.0: 'Forty-Five Footer'
+    }
+
     def __init__(self, size_of_container: float, total_number_of_containers: float) -> None:
         self.size_of_container = size_of_container
         self.total_number_of_containers = total_number_of_containers
-        self.twenty_footer = 20
-        self.forty_footer = 40
-        self.forty_five_footer = 45
+        self.wd_rate = float
 
     def calculate_fcl(self, wd_rate) -> float:
         total_wd = round(
             self.total_number_of_containers * wd_rate, 2
         )
         return total_wd
 
 
 class WDContainerizedCargoImport(WDContainerizedCargo):
-    def __init__(self, size_of_container, total_number_of_containers) -> None:
-        super().__init__(size_of_container, total_number_of_containers)
-        self.wd_rate = float
-        self.twenty_footer_rate = 519.35
-        self.forty_footer_rate = 779.05
-        self.forty_five_footer_rate = 916.50
-
     def calculate_fcl_import(self):
-        if self.size_of_container == self.twenty_footer:
-            self.wd_rate = self.twenty_footer_rate
-
-        elif self.size_of_container == self.forty_footer:
-            self.wd_rate = self.forty_footer_rate
-
-        elif self.size_of_container == self.forty_five_footer:
-            self.wd_rate = self.forty_five_footer_rate
-
+        container_size = WDContainerizedCargo.CONTAINER_SIZE[self.size_of_container]
+        self.wd_rate = get_rate_of_container_size(container_size, 'import_rates.json')
         return self.calculate_fcl(self.wd_rate)
 
 
 class WDContainerizedCargoExport(WDContainerizedCargo):
-    def __init__(self, size_of_container, total_number_of_containers) -> None:
-        super().__init__(size_of_container, total_number_of_containers)
-        self.wd_rate = float
-        self.twenty_footer_rate = 259.70
-        self.forty_footer_rate = 391.05
-        self.forty_five_footer_rate = 458.25
-
     def calculate_fcl_export(self):
-        if self.size_of_container == self.twenty_footer:
-            self.wd_rate = self.twenty_footer_rate
-
-        elif self.size_of_container == self.forty_footer:
-            self.wd_rate = self.forty_footer_rate
-
-        elif self.size_of_container == self.forty_five_footer:
-            self.wd_rate = self.forty_five_footer_rate
-
+        container_size = WDContainerizedCargo.CONTAINER_SIZE[self.size_of_container]
+        self.wd_rate = get_rate_of_container_size(container_size, 'export_rates.json')
         return self.calculate_fcl(self.wd_rate)
```

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/formal_entry/lc_via_formal_entry.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/formal_entry/lc_via_formal_entry.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/landed_cost/entry_type/informal_entry/lc_via_informal_entry.py` & `customs_dtoc-0.0.7/src/customs_dtoc/landed_cost/entry_type/informal_entry/lc_via_informal_entry.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/pro_rata/pro_rata.py` & `customs_dtoc-0.0.7/src/customs_dtoc/pro_rata/pro_rata.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/sop/sop.py` & `customs_dtoc-0.0.7/src/customs_dtoc/sop/sop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import math
 
 
 class SummaryOfPaymentsWithLetterOfCredit:
     def __init__(self, customs_duty: float, value_added_tax: float, excise_tax: float, import_processing_fee: float,
                  customs_documentary_stamps: float, container_security_fee: float, advance_deposit: float) -> None:
         self.customs_duty = customs_duty
```

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc/vat/vat.py` & `customs_dtoc-0.0.7/src/customs_dtoc/vat/vat.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc.egg-info/PKG-INFO` & `customs_dtoc-0.0.7/src/customs_dtoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customs-dtoc
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for calculating customs duties, taxes, and other charges.
 Home-page: https://github.com/iaaan05/python-customs-tax-package
 Author: Iaaan05
 Author-email: iaaan100500@gmail.com
 License: MIT
 Keywords: customs,duties,taxes,charges
 Classifier: Intended Audience :: Information Technology
```

### Comparing `customs_dtoc-0.0.6/src/customs_dtoc.egg-info/SOURCES.txt` & `customs_dtoc-0.0.7/src/customs_dtoc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 src/customs_dtoc/landed_cost/components_of_lc/ac/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/ac/outports/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/ac/outports/ac_outports.py
 src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py
 src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/__init__.py
-src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/full_containerized_cargo.py
+src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/fcl/containerized_cargo.py
 src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/lcl/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/ac/pom_micp/lcl/bulk_break_bulk_cargo.py
 src/customs_dtoc/landed_cost/components_of_lc/bc/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/bc/bc.py
 src/customs_dtoc/landed_cost/components_of_lc/bf/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/bf/bf_formal_entry.py
 src/customs_dtoc/landed_cost/components_of_lc/cds/__init__.py
@@ -35,15 +35,15 @@
 src/customs_dtoc/landed_cost/components_of_lc/wd/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/wd/outports/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/wd/outports/wharfage_due_outports.py
 src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/containerized_dangerous_cargo/containerized_dangerous_cargo.py
 src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/__init__.py
-src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/full_containerized_load.py
+src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/fcl/containerized_cargo.py
 src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/lcl/__init__.py
 src/customs_dtoc/landed_cost/components_of_lc/wd/pom_micp/lcl/bulk_break_bulk_cargo.py
 src/customs_dtoc/landed_cost/entry_type/__init__.py
 src/customs_dtoc/landed_cost/entry_type/formal_entry/__init__.py
 src/customs_dtoc/landed_cost/entry_type/formal_entry/lc_via_formal_entry.py
 src/customs_dtoc/landed_cost/entry_type/informal_entry/__init__.py
 src/customs_dtoc/landed_cost/entry_type/informal_entry/lc_via_informal_entry.py
```

### Comparing `customs_dtoc-0.0.6/tests/test_csf.py` & `customs_dtoc-0.0.7/tests/test_csf.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/tests/test_landed_cost.py` & `customs_dtoc-0.0.7/tests/test_landed_cost.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/tests/test_pro_rata.py` & `customs_dtoc-0.0.7/tests/test_pro_rata.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/tests/test_sop.py` & `customs_dtoc-0.0.7/tests/test_sop.py`

 * *Files identical despite different names*

### Comparing `customs_dtoc-0.0.6/tests/test_vat.py` & `customs_dtoc-0.0.7/tests/test_vat.py`

 * *Files identical despite different names*

