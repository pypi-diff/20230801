# Comparing `tmp/bw_matchbox-0.2.1.tar.gz` & `tmp/bw_matchbox-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.2.1.tar", last modified: Tue Aug  1 12:25:20 2023, max compression
+gzip compressed data, was "bw_matchbox-0.2.2.tar", last modified: Tue Aug  1 12:30:23 2023, max compression
```

## Comparing `bw_matchbox-0.2.1.tar` & `bw_matchbox-0.2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.278352 bw_matchbox-0.2.1/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.2.1/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      216 2023-08-01 11:41:22.000000 bw_matchbox-0.2.1/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-01 12:25:20.278412 bw_matchbox-0.2.1/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.266921 bw_matchbox-0.2.1/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-01 12:24:59.000000 bw_matchbox-0.2.1/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-07-29 11:35:17.000000 bw_matchbox-0.2.1/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.265124 bw_matchbox-0.2.1/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.268399 bw_matchbox-0.2.1/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4955 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1501 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      146 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/css/layout.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.268570 bw_matchbox-0.2.1/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.2.1/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.269641 bw_matchbox-0.2.1/bw_matchbox/assets/js/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1534 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/js/common-helpers.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    18008 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/js/compare-core.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      946 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/js/compare-row-click.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    10108 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/js/compare-rows-helpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.273388 bw_matchbox-0.2.1/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3929 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)    11784 2023-06-20 12:27:44.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/file.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2336 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1751 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-06-21 09:42:53.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.2.1/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.273844 bw_matchbox-0.2.1/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.2.1/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2913 2023-08-01 07:14:42.000000 bw_matchbox-0.2.1/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.278129 bw_matchbox-0.2.1/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123245 2023-06-13 11:22:50.000000 bw_matchbox-0.2.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.2.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116071 2023-06-13 11:23:32.000000 bw_matchbox-0.2.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.2.1/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      346 2023-08-01 07:14:42.000000 bw_matchbox-0.2.1/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    20933 2023-08-01 07:14:48.000000 bw_matchbox-0.2.1/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.274984 bw_matchbox-0.2.1/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-01 12:25:20.000000 bw_matchbox-0.2.1/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     3017 2023-08-01 12:25:20.000000 bw_matchbox-0.2.1/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-01 12:25:20.000000 bw_matchbox-0.2.1/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-01 12:25:20.000000 bw_matchbox-0.2.1/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.2.1/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      155 2023-08-01 12:25:20.000000 bw_matchbox-0.2.1/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-01 12:25:20.000000 bw_matchbox-0.2.1/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:25:20.274060 bw_matchbox-0.2.1/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.2.1/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.2.1/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1849 2023-08-01 12:25:20.278771 bw_matchbox-0.2.1/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.156120 bw_matchbox-0.2.2/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.2.2/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)      216 2023-08-01 11:41:22.000000 bw_matchbox-0.2.2/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-01 12:30:23.156182 bw_matchbox-0.2.2/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.146602 bw_matchbox-0.2.2/bw_matchbox/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-01 12:29:57.000000 bw_matchbox-0.2.2/bw_matchbox/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-07-29 11:35:17.000000 bw_matchbox-0.2.2/bw_matchbox/__init__.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.144765 bw_matchbox-0.2.2/bw_matchbox/assets/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.148184 bw_matchbox-0.2.2/bw_matchbox/assets/css/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4955 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1501 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      146 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/layout.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.148305 bw_matchbox-0.2.2/bw_matchbox/assets/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.149133 bw_matchbox-0.2.2/bw_matchbox/assets/js/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1534 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/js/common-helpers.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    18008 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-core.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      946 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-row-click.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    10108 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-rows-helpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.151810 bw_matchbox-0.2.2/bw_matchbox/assets/templates/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3929 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11784 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/file.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2336 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1751 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-06-21 09:42:53.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.2.2/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.152079 bw_matchbox-0.2.2/bw_matchbox/bin/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.2.2/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2913 2023-08-01 07:14:42.000000 bw_matchbox-0.2.2/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.154140 bw_matchbox-0.2.2/bw_matchbox/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   123245 2023-06-13 11:22:50.000000 bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)   116071 2023-06-13 11:23:32.000000 bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.2.2/bw_matchbox/data/dare.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      346 2023-08-01 07:14:42.000000 bw_matchbox-0.2.2/bw_matchbox/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    20933 2023-08-01 07:14:48.000000 bw_matchbox-0.2.2/bw_matchbox/webapp.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.155315 bw_matchbox-0.2.2/bw_matchbox.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3256 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      155 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-01 12:30:23.000000 bw_matchbox-0.2.2/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 12:30:23.154376 bw_matchbox-0.2.2/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.2.2/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.2.2/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1862 2023-08-01 12:30:23.156547 bw_matchbox-0.2.2/setup.cfg
```

### Comparing `bw_matchbox-0.2.1/LICENSE` & `bw_matchbox-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/PKG-INFO` & `bw_matchbox-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.2.1
+Version: 0.2.2
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.2.1/README.md` & `bw_matchbox-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/css/compare.css` & `bw_matchbox-0.2.2/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.2.2/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.2.2/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.2.2/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.2.2/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.2.2/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/js/common-helpers.js` & `bw_matchbox-0.2.2/bw_matchbox/assets/js/common-helpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/js/compare-core.js` & `bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-core.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/js/compare-row-click.js` & `bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-row-click.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/js/compare-rows-helpers.js` & `bw_matchbox-0.2.2/bw_matchbox/assets/js/compare-rows-helpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/compare.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/file.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/file.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/index.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/process_detail.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.2.2/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.2.2/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.2.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/data/dare.json` & `bw_matchbox-0.2.2/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox/webapp.py` & `bw_matchbox-0.2.2/bw_matchbox/webapp.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.2.2/bw_matchbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.2.1
+Version: 0.2.2
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.2.1/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.2.2/bw_matchbox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 ./bw_matchbox/assets/templates/project.html
 ./bw_matchbox/assets/templates/search-embedded.html
 ./bw_matchbox/assets/templates/search.html
 ./bw_matchbox/assets/templates/search_result.html
 ./bw_matchbox/assets/templates/select_files.html
 ./bw_matchbox/bin/__init__.py
 ./bw_matchbox/bin/matchbox.py
+./bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+./bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+./bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+./bw_matchbox/data/dare.json
 ./docs/conf.py
 bw_matchbox/VERSION
 bw_matchbox.egg-info/PKG-INFO
 bw_matchbox.egg-info/SOURCES.txt
 bw_matchbox.egg-info/dependency_links.txt
 bw_matchbox.egg-info/entry_points.txt
 bw_matchbox.egg-info/not-zip-safe
```

### Comparing `bw_matchbox-0.2.1/docs/conf.py` & `bw_matchbox-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.2.1/setup.cfg` & `bw_matchbox-0.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 [options.package_data]
 bw_matchbox = 
 	assets/js/*.js
 	assets/images/*.ico
 	assets/templates/*.html
 	assets/css/*.css
+	data/*.json
 	VERSION
 
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
 	pytest-cov
```

