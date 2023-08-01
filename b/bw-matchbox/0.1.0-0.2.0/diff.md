# Comparing `tmp/bw_matchbox-0.1.0.tar.gz` & `tmp/bw_matchbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.1.0.tar", last modified: Wed Jul 26 22:17:02 2023, max compression
+gzip compressed data, was "bw_matchbox-0.2.0.tar", last modified: Tue Aug  1 11:50:34 2023, max compression
```

## Comparing `bw_matchbox-0.1.0.tar` & `bw_matchbox-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,62 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.196186 bw_matchbox-0.1.0/
--rw-r--r--   0 cmutel     (501) staff       (20)     1067 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)      181 2023-07-26 22:12:03.000000 bw_matchbox-0.1.0/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     6221 2023-07-26 22:17:02.196250 bw_matchbox-0.1.0/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     5197 2023-07-26 21:58:12.000000 bw_matchbox-0.1.0/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.191197 bw_matchbox-0.1.0/bw_matchbox/
--rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/VERSION
--rw-r--r--   0 cmutel     (501) staff       (20)      215 2023-07-26 20:50:48.000000 bw_matchbox-0.1.0/bw_matchbox/__init__.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.189766 bw_matchbox-0.1.0/bw_matchbox/assets/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.192433 bw_matchbox-0.1.0/bw_matchbox/assets/css/
--rw-r--r--   0 cmutel     (501) staff       (20)     1322 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 cmutel     (501) staff       (20)     7797 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 cmutel     (501) staff       (20)    11452 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 cmutel     (501) staff       (20)      960 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.192558 bw_matchbox-0.1.0/bw_matchbox/assets/images/
--rw-r--r--   0 cmutel     (501) staff       (20)    32038 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.195290 bw_matchbox-0.1.0/bw_matchbox/assets/templates/
--rw-r--r--   0 cmutel     (501) staff       (20)    11832 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2566 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 cmutel     (501) staff       (20)      461 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 cmutel     (501) staff       (20)    11784 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/file.html
--rw-r--r--   0 cmutel     (501) staff       (20)       16 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1792 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1738 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 cmutel     (501) staff       (20)      733 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1711 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 cmutel     (501) staff       (20)      798 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 cmutel     (501) staff       (20)     3507 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 cmutel     (501) staff       (20)      599 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 cmutel     (501) staff       (20)      399 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 cmutel     (501) staff       (20)      850 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 cmutel     (501) staff       (20)      947 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1243 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.190987 bw_matchbox-0.1.0/bw_matchbox/bin/
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/bin/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2769 2023-07-26 21:52:48.000000 bw_matchbox-0.1.0/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.196067 bw_matchbox-0.1.0/bw_matchbox/data/
--rw-r--r--   0 cmutel     (501) staff       (20)   123245 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 cmutel     (501) staff       (20)    93862 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 cmutel     (501) staff       (20)   116071 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 cmutel     (501) staff       (20)      603 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/data/dare.json
--rw-r--r--   0 cmutel     (501) staff       (20)      364 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/bw_matchbox/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)    16666 2023-07-26 19:15:48.000000 bw_matchbox-0.1.0/bw_matchbox/webapp.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.191975 bw_matchbox-0.1.0/bw_matchbox.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     6221 2023-07-26 22:17:02.000000 bw_matchbox-0.1.0/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     1584 2023-07-26 22:17:02.000000 bw_matchbox-0.1.0/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-26 22:17:02.000000 bw_matchbox-0.1.0/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       59 2023-07-26 22:17:02.000000 bw_matchbox-0.1.0/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 11:26:00.000000 bw_matchbox-0.1.0/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 cmutel     (501) staff       (20)      155 2023-07-26 22:17:02.000000 bw_matchbox-0.1.0/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       12 2023-07-26 22:17:02.000000 bw_matchbox-0.1.0/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-07-26 22:17:02.191095 bw_matchbox-0.1.0/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     1145 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/docs/conf.py
--rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 11:16:50.000000 bw_matchbox-0.1.0/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)     1721 2023-07-26 22:17:02.196625 bw_matchbox-0.1.0/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.836134 bw_matchbox-0.2.0/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.2.0/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)      216 2023-08-01 11:41:22.000000 bw_matchbox-0.2.0/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-01 11:50:34.836212 bw_matchbox-0.2.0/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.826388 bw_matchbox-0.2.0/bw_matchbox/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-01 11:50:13.000000 bw_matchbox-0.2.0/bw_matchbox/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-07-29 11:35:17.000000 bw_matchbox-0.2.0/bw_matchbox/__init__.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.823835 bw_matchbox-0.2.0/bw_matchbox/assets/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.828361 bw_matchbox-0.2.0/bw_matchbox/assets/css/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4955 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1501 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      146 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/css/layout.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.828484 bw_matchbox-0.2.0/bw_matchbox/assets/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.2.0/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.829473 bw_matchbox-0.2.0/bw_matchbox/assets/js/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1534 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/js/common-helpers.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    18008 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/js/compare-core.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      946 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/js/compare-row-click.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    10108 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/js/compare-rows-helpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.833053 bw_matchbox-0.2.0/bw_matchbox/assets/templates/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3929 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11784 2023-06-20 12:27:44.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/file.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2336 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1751 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-06-21 09:42:53.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.2.0/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.826004 bw_matchbox-0.2.0/bw_matchbox/bin/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.2.0/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2913 2023-08-01 07:14:42.000000 bw_matchbox-0.2.0/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.835898 bw_matchbox-0.2.0/bw_matchbox/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   123245 2023-06-13 11:22:50.000000 bw_matchbox-0.2.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.2.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)   116071 2023-06-13 11:23:32.000000 bw_matchbox-0.2.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.2.0/bw_matchbox/data/dare.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      346 2023-08-01 07:14:42.000000 bw_matchbox-0.2.0/bw_matchbox/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    20933 2023-08-01 07:14:48.000000 bw_matchbox-0.2.0/bw_matchbox/webapp.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.827208 bw_matchbox-0.2.0/bw_matchbox.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-01 11:50:34.000000 bw_matchbox-0.2.0/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1820 2023-08-01 11:50:34.000000 bw_matchbox-0.2.0/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-01 11:50:34.000000 bw_matchbox-0.2.0/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-01 11:50:34.000000 bw_matchbox-0.2.0/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.2.0/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      155 2023-08-01 11:50:34.000000 bw_matchbox-0.2.0/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-01 11:50:34.000000 bw_matchbox-0.2.0/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-01 11:50:34.826180 bw_matchbox-0.2.0/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.2.0/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.2.0/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-01 11:50:34.836587 bw_matchbox-0.2.0/setup.cfg
```

### Comparing `bw_matchbox-0.1.0/LICENSE` & `bw_matchbox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/PKG-INFO` & `bw_matchbox-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.1.0
+Version: 0.2.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
@@ -59,14 +59,20 @@
 
 You can install _bw_matchbox_ via [pip] from [PyPI]:
 
 ```console
 pip install bw_matchbox
 ```
 
+It's possible to install the library itself for development purposes (in the cloned project):
+
+```console
+pip install -e .
+```
+
 This library depends on:
 
 * Brightway 2.5 (`brightway25`)
 * `docopt-ng`
 * `flask` and `flask_httpauth`
 * `tomli`
 * `werkzeug`
```

### Comparing `bw_matchbox-0.1.0/README.md` & `bw_matchbox-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 
 You can install _bw_matchbox_ via [pip] from [PyPI]:
 
 ```console
 pip install bw_matchbox
 ```
 
+It's possible to install the library itself for development purposes (in the cloned project):
+
+```console
+pip install -e .
+```
+
 This library depends on:
 
 * Brightway 2.5 (`brightway25`)
 * `docopt-ng`
 * `flask` and `flask_httpauth`
 * `tomli`
 * `werkzeug`
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.2.0/bw_matchbox/assets/css/customizations.css`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,46 @@
+/* stylelint-disable number-max-precision, declaration-block-single-line-max-declarations, comment-empty-line-before, rule-empty-line-before */
+
 .shift-right {
   position: relative;
   animation-name: shift-right-anim;
   animation-duration: 0.5s;
 }
 
 @keyframes shift-right-anim {
-  0%   {background-color:white; left:0px;}
-  50%  {background-color:DeepSkyBlue; left:10px;}
-  100% {background-color:white; left:0px;}
+  0% {
+    background-color: white;
+    left: 0;
+  }
+  50% {
+    background-color: deepskyblue;
+    left: 10px;
+  }
+  100% {
+    background-color: white;
+    left: 0;
+  }
 }
 
 .tight {
-  margin-bottom: .5rem;
+  margin-bottom: 0.5rem;
 }
 
 .model-wrapper {
   position: relative;
 }
 
 .modal {
   display: none; /* Hidden by default */
   position: absolute;
   z-index: 1; /* Sit on top */
   /*  left: 0;*/
   /*  top: 0;*/
   width: 100%; /* Full width */
-  /*  height: 100%; /* Full height */*/
+  /*  height: 100%; /* Full height */
   overflow: auto; /* Enable scroll if needed */
   background-color: white;
   border: 2px solid #888;
 }
 
 /* Modal Content/Box */
 .modal-content {
@@ -56,25 +67,25 @@
 
 .checkbox-grid li {
   display: block;
   float: left;
 }
 
 .narrower {
-  color: #592A71;
+  color: #592a71;
 }
 
 .broader {
-  color: #AA3C39;
+  color: #aa3c39;
 }
 
 .exact {
-  color: #2D8632;
+  color: #2d8632;
 }
 
 .approximate {
-  color: #A8AA39;
+  color: #a8aa39;
 }
 
 .selected-element {
-  box-shadow: 0 0 5px 5px #33C3F0;
+  box-shadow: 0 0 5px 5px #33c3f0;
 }
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.2.0/bw_matchbox/assets/css/normalize.css`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,15 @@
  * 1. Set default font family to sans-serif.
  * 2. Prevent iOS text size adjust after orientation change, without disabling
  *    user zoom.
  */
 
 html {
   font-family: sans-serif; /* 1 */
-  -ms-text-size-adjust: 100%; /* 2 */
-  -webkit-text-size-adjust: 100%; /* 2 */
+  text-size-adjust: 100%; /* 2 */
 }
 
 /**
  * Remove default margin.
  */
 
 body {
@@ -205,15 +204,14 @@
 }
 
 /**
  * Address differences between Firefox and other browsers.
  */
 
 hr {
-  -moz-box-sizing: content-box;
   box-sizing: content-box;
   height: 0;
 }
 
 /**
  * Contain overflow in all browsers.
  */
@@ -226,15 +224,15 @@
  * Address odd `em`-unit font size rendering in all browsers.
  */
 
 code,
 kbd,
 pre,
 samp {
-  font-family: monospace, monospace;
+  font-family: monospace;
   font-size: 1em;
 }
 
 /* Forms
    ========================================================================== */
 
 /**
@@ -287,15 +285,15 @@
  *    `input` and others.
  */
 
 button,
 html input[type="button"], /* 1 */
 input[type="reset"],
 input[type="submit"] {
-  -webkit-appearance: button; /* 2 */
+  appearance: button; /* 2 */
   cursor: pointer; /* 3 */
 }
 
 /**
  * Re-set default cursor for disabled elements.
  */
 
@@ -327,53 +325,51 @@
  * It's recommended that you don't attempt to style these elements.
  * Firefox's implementation doesn't respect box-sizing, padding, or width.
  *
  * 1. Address box sizing set to `content-box` in IE 8/9/10.
  * 2. Remove excess padding in IE 8/9/10.
  */
 
-input[type="checkbox"],
-input[type="radio"] {
+input[type='checkbox'],
+input[type='radio'] {
   box-sizing: border-box; /* 1 */
   padding: 0; /* 2 */
 }
 
 /**
  * Fix the cursor style for Chrome's increment/decrement buttons. For certain
  * `font-size` values of the `input`, it causes the cursor style of the
  * decrement button to change from `default` to `text`.
  */
 
-input[type="number"]::-webkit-inner-spin-button,
-input[type="number"]::-webkit-outer-spin-button {
+input[type='number']::-webkit-inner-spin-button,
+input[type='number']::-webkit-outer-spin-button {
   height: auto;
 }
 
 /**
  * 1. Address `appearance` set to `searchfield` in Safari and Chrome.
  * 2. Address `box-sizing` set to `border-box` in Safari and Chrome
  *    (include `-moz` to future-proof).
  */
 
-input[type="search"] {
-  -webkit-appearance: textfield; /* 1 */
-  -moz-box-sizing: content-box;
-  -webkit-box-sizing: content-box; /* 2 */
-  box-sizing: content-box;
+input[type='search'] {
+  appearance: textfield; /* 1 */
+  box-sizing: content-box; /* 2 */
 }
 
 /**
  * Remove inner padding and search cancel button in Safari and Chrome on OS X.
  * Safari (but not Chrome) clips the cancel button when the search input has
  * padding (and `textfield` appearance).
  */
 
-input[type="search"]::-webkit-search-cancel-button,
-input[type="search"]::-webkit-search-decoration {
-  -webkit-appearance: none;
+input[type='search']::-webkit-search-cancel-button,
+input[type='search']::-webkit-search-decoration {
+  appearance: none;
 }
 
 /**
  * Define consistent border, margin, and padding.
  */
 
 fieldset {
@@ -420,8 +416,8 @@
   border-collapse: collapse;
   border-spacing: 0;
 }
 
 td,
 th {
   padding: 0;
-}
+}
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.2.0/bw_matchbox/assets/css/skeleton.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+/* stylelint-disable number-max-precision, declaration-block-single-line-max-declarations */
+
 /*
 * Skeleton V2.0.4
 * Copyright 2014, Dave Gamache
 * www.getskeleton.com
 * Free to use under the MIT license.
 * http://www.opensource.org/licenses/mit-license.php
 * 12/29/2014
@@ -30,38 +32,47 @@
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 .container {
   position: relative;
   width: 100%;
   max-width: 960px;
   margin: 0 auto;
   padding: 0 20px;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 .column,
 .columns {
   width: 100%;
   float: left;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
 
 /* For devices larger than 400px */
-@media (min-width: 400px) {
+@media (width>= 400px) {
   .container {
     width: 85%;
-    padding: 0; }
+    padding: 0;
+  }
 }
 
 /* For devices larger than 550px */
-@media (min-width: 550px) {
+@media (width>= 550px) {
   .container {
-    width: 80%; }
+    width: 80%;
+  }
+
   .column,
   .columns {
-    margin-left: 4%; }
+    margin-left: 4%;
+  }
+
   .column:first-child,
   .columns:first-child {
-    margin-left: 0; }
+    margin-left: 0;
+  }
 
   .one.column,
   .one.columns                    { width: 4.66666666667%; }
   .two.columns                    { width: 13.3333333333%; }
   .three.columns                  { width: 22%;            }
   .four.columns                   { width: 30.6666666667%; }
   .five.columns                   { width: 39.3333333333%; }
@@ -77,94 +88,114 @@
   .two-thirds.column              { width: 65.3333333333%; }
 
   .one-half.column                { width: 48%; }
 
   /* Offsets */
   .offset-by-one.column,
   .offset-by-one.columns          { margin-left: 8.66666666667%; }
+
   .offset-by-two.column,
   .offset-by-two.columns          { margin-left: 17.3333333333%; }
+
   .offset-by-three.column,
   .offset-by-three.columns        { margin-left: 26%;            }
+
   .offset-by-four.column,
   .offset-by-four.columns         { margin-left: 34.6666666667%; }
+
   .offset-by-five.column,
   .offset-by-five.columns         { margin-left: 43.3333333333%; }
+
   .offset-by-six.column,
   .offset-by-six.columns          { margin-left: 52%;            }
+
   .offset-by-seven.column,
   .offset-by-seven.columns        { margin-left: 60.6666666667%; }
+
   .offset-by-eight.column,
   .offset-by-eight.columns        { margin-left: 69.3333333333%; }
+
   .offset-by-nine.column,
   .offset-by-nine.columns         { margin-left: 78.0%;          }
+
   .offset-by-ten.column,
   .offset-by-ten.columns          { margin-left: 86.6666666667%; }
+
   .offset-by-eleven.column,
   .offset-by-eleven.columns       { margin-left: 95.3333333333%; }
 
   .offset-by-one-third.column,
   .offset-by-one-third.columns    { margin-left: 34.6666666667%; }
+
   .offset-by-two-thirds.column,
   .offset-by-two-thirds.columns   { margin-left: 69.3333333333%; }
 
   .offset-by-one-half.column,
   .offset-by-one-half.columns     { margin-left: 52%; }
 
 }
 
 
 /* Base Styles
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
+
 /* NOTE
 html is set to 62.5% so that all the REM measurements throughout Skeleton
 are based on 10px sizing. So basically 1.5rem = 15px :) */
 html {
-  font-size: 62.5%; }
+  font-size: 62.5%;
+}
+
 body {
   font-size: 1.5em; /* currently ems cause chrome bug misinterpreting rems on body element */
   line-height: 1.6;
   font-weight: 400;
-  font-family: "Raleway", "HelveticaNeue", "Helvetica Neue", Helvetica, Arial, sans-serif;
-  color: #222; }
+  font-family: Raleway, HelveticaNeue, "Helvetica Neue", Helvetica, Arial, sans-serif;
+  color: #222;
+}
 
 
 /* Typography
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 h1, h2, h3, h4, h5, h6 {
   margin-top: 0;
   margin-bottom: 2rem;
-  font-weight: 300; }
+  font-weight: 300;
+}
 h1 { font-size: 4.0rem; line-height: 1.2;  letter-spacing: -.1rem;}
 h2 { font-size: 3.6rem; line-height: 1.25; letter-spacing: -.1rem; }
 h3 { font-size: 3.0rem; line-height: 1.3;  letter-spacing: -.1rem; }
 h4 { font-size: 2.4rem; line-height: 1.35; letter-spacing: -.08rem; }
 h5 { font-size: 1.8rem; line-height: 1.5;  letter-spacing: -.05rem; }
 h6 { font-size: 1.5rem; line-height: 1.6;  letter-spacing: 0; }
 
 /* Larger than phablet */
-@media (min-width: 550px) {
+@media (width>= 550px) {
   h1 { font-size: 5.0rem; }
   h2 { font-size: 4.2rem; }
   h3 { font-size: 3.6rem; }
   h4 { font-size: 3.0rem; }
   h5 { font-size: 2.4rem; }
   h6 { font-size: 1.5rem; }
 }
 
 p {
-  margin-top: 0; }
+  margin-top: 0;
+}
 
 
 /* Links
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 a {
-  color: #1EAEDB; }
+  color: #1EAEDB;
+}
+
 a:hover {
-  color: #0FA0CE; }
+  color: #0FA0CE;
+}
 
 
 /* Buttons
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 .button,
 button,
 input[type="submit"],
@@ -182,49 +213,56 @@
   text-transform: uppercase;
   text-decoration: none;
   white-space: nowrap;
   background-color: transparent;
   border-radius: 4px;
   border: 1px solid #bbb;
   cursor: pointer;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 .button:hover,
 button:hover,
 input[type="submit"]:hover,
 input[type="reset"]:hover,
 input[type="button"]:hover,
 .button:focus,
 button:focus,
 input[type="submit"]:focus,
 input[type="reset"]:focus,
 input[type="button"]:focus {
   color: #333;
   border-color: #888;
-  outline: 0; }
+  outline: 0;
+}
+
 .button.button-primary,
 button.button-primary,
 input[type="submit"].button-primary,
 input[type="reset"].button-primary,
 input[type="button"].button-primary {
   color: #FFF;
   background-color: #33C3F0;
-  border-color: #33C3F0; }
+  border-color: #33C3F0;
+}
+
 .button.button-primary:hover,
 button.button-primary:hover,
 input[type="submit"].button-primary:hover,
 input[type="reset"].button-primary:hover,
 input[type="button"].button-primary:hover,
 .button.button-primary:focus,
 button.button-primary:focus,
 input[type="submit"].button-primary:focus,
 input[type="reset"].button-primary:focus,
 input[type="button"].button-primary:focus {
   color: #FFF;
   background-color: #1EAEDB;
-  border-color: #1EAEDB; }
+  border-color: #1EAEDB;
+}
 
 
 /* Forms
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 input[type="email"],
 input[type="number"],
 input[type="search"],
@@ -236,183 +274,230 @@
 select {
   height: 38px;
   padding: 6px 10px; /* The 6px vertically centers text on FF, ignored by Webkit */
   background-color: #fff;
   border: 1px solid #D1D1D1;
   border-radius: 4px;
   box-shadow: none;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 /* Removes awkward default styles on some inputs for iOS */
 input[type="email"],
 input[type="number"],
 input[type="search"],
 input[type="text"],
 input[type="tel"],
 input[type="url"],
 input[type="password"],
 textarea {
-  -webkit-appearance: none;
-     -moz-appearance: none;
-          appearance: none; }
+  appearance: none;
+}
+
 textarea {
   min-height: 65px;
   padding-top: 6px;
-  padding-bottom: 6px; }
+  padding-bottom: 6px;
+}
+
 input[type="email"]:focus,
 input[type="number"]:focus,
 input[type="search"]:focus,
 input[type="text"]:focus,
 input[type="tel"]:focus,
 input[type="url"]:focus,
 input[type="password"]:focus,
 textarea:focus,
 select:focus {
   border: 1px solid #33C3F0;
-  outline: 0; }
+  outline: 0;
+}
+
 label,
 legend {
   display: block;
   margin-bottom: .5rem;
-  font-weight: 600; }
+  font-weight: 600;
+}
+
 fieldset {
   padding: 0;
-  border-width: 0; }
+  border-width: 0;
+}
+
 input[type="checkbox"],
 input[type="radio"] {
-  display: inline; }
+  display: inline;
+}
+
 label > .label-body {
   display: inline-block;
   margin-left: .5rem;
-  font-weight: normal; }
+  font-weight: normal;
+}
 
 
 /* Lists
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 ul {
-  list-style: circle inside; }
+  list-style: circle inside;
+}
+
 ol {
-  list-style: decimal inside; }
+  list-style: decimal inside;
+}
+
 ol, ul {
   padding-left: 0;
-  margin-top: 0; }
+  margin-top: 0;
+}
+
 ul ul,
 ul ol,
 ol ol,
 ol ul {
   margin: 1.5rem 0 1.5rem 3rem;
-  font-size: 90%; }
+  font-size: 90%;
+}
+
 li {
-  margin-bottom: 1rem; }
+  margin-bottom: 1rem;
+}
 
 
 /* Code
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 code {
   padding: .2rem .5rem;
   margin: 0 .2rem;
   font-size: 90%;
   white-space: nowrap;
   background: #F1F1F1;
   border: 1px solid #E1E1E1;
-  border-radius: 4px; }
+  border-radius: 4px;
+}
+
 pre > code {
   display: block;
   padding: 1rem 1.5rem;
-  white-space: pre; }
+  white-space: pre;
+}
 
 
 /* Tables
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 th,
 td {
   padding: 12px 15px;
   text-align: left;
-  border-bottom: 1px solid #E1E1E1; }
+  border-bottom: 1px solid rgb(0 0 0 / 10%);
+
+  /* border-bottom: 1px solid #E1E1E1; */
+}
+
 th:first-child,
 td:first-child {
-  padding-left: 0; }
+  padding-left: 0;
+}
+
 th:last-child,
 td:last-child {
-  padding-right: 0; }
+  padding-right: 0;
+}
 
 
 /* Spacing
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 button,
 .button {
-  margin-bottom: 1rem; }
+  margin-bottom: 1rem;
+}
+
 input,
 textarea,
 select,
 fieldset {
-  margin-bottom: 1.5rem; }
+  margin-bottom: 1.5rem;
+}
+
 pre,
 blockquote,
 dl,
 figure,
 table,
 p,
 ul,
 ol,
 form {
-  margin-bottom: 2.5rem; }
+  margin-bottom: 2.5rem;
+}
 
 
 /* Utilities
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 .u-full-width {
   width: 100%;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 .u-max-full-width {
   max-width: 100%;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 .u-pull-right {
-  float: right; }
+  float: right;
+}
+
 .u-pull-left {
-  float: left; }
+  float: left;
+}
 
 
 /* Misc
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 hr {
   margin-top: 3rem;
   margin-bottom: 3.5rem;
   border-width: 0;
-  border-top: 1px solid #E1E1E1; }
+  border-top: 1px solid #E1E1E1;
+}
 
 
 /* Clearing
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 
 /* Self Clearing Goodness */
-.container:after,
-.row:after,
+.container::after,
+.row::after,
 .u-cf {
   content: "";
   display: table;
-  clear: both; }
+  clear: both;
+}
 
 
 /* Media Queries
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
+
 /*
 Note: The best way to structure the use of media queries is to create the queries
 near the relevant code. For example, if you wanted to change the styles for buttons
 on small devices, paste the mobile query code up in the buttons section and style it
 there.
 */
 
 
 /* Larger than mobile */
-@media (min-width: 400px) {}
+@media (width>= 400px) {}
 
 /* Larger than phablet (also point when grid becomes active) */
-@media (min-width: 550px) {}
+@media (width>= 550px) {}
 
 /* Larger than tablet */
-@media (min-width: 750px) {}
+@media (width>= 750px) {}
 
 /* Larger than desktop */
-@media (min-width: 1000px) {}
+@media (width>= 1000px) {}
 
 /* Larger than Desktop HD */
-@media (min-width: 1200px) {}
+@media (width>= 1200px) {}
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.2.0/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/file.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/file.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/header.html`

 * *Files 22% similar despite different names*

```diff
@@ -13,21 +13,29 @@
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <meta name="viewport" content="width=device-width, initial-scale=1">
 
   <!-- FONT
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link href="//fonts.googleapis.com/css?family=Raleway:400,300,600" rel="stylesheet" type="text/css">
 
+  <!-- ICONS
+  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
+  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
+
   <!-- CSS
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link rel="stylesheet" href="{{ url_for('static', filename='css/normalize.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/tooltip.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/skeleton.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/customizations.css') }}">
-  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
+  <link rel="stylesheet" href="{{ url_for('static', filename='css/layout.css') }}">
+
+  <!-- Scripts (TODO: to move to the body end?)
+  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
+  <script src="{{ url_for('static', filename='js/common-helpers.js') }}"></script>
 
   <!-- Favicon
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link rel="icon" type="image/png" href="{{ url_for('static', filename='images/favicon.ico') }}">
 
 </head>
 <body>
```

#### html2text {}

```diff
@@ -4,7 +4,9 @@
 
 
 
 
 
 
 
+
+
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/index.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <div class="column">
       <h1>
         {% if unmatched_link %}Source Database <a href="{{ url_for('unmatched') }}">(Only unmatched)</a>
         {% else %}Unmatched in Source Database
         {% endif %}
       </h1>
       <p><input class="u-full-width" placeholder="{{ query_string }}" id="query_string"></p>
-      <table>
+      <table width="100%">
         <tr>
           <th>Name</th>
           <th>Location</th>
           <th>Unit</th>
           <th>Matched</th>
         </tr>
         {% for row in table_data %}
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/process_detail.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 {% include 'header.html' %}
 <div class="container">
   {% include 'navigation.html' %}
   <div class="row">
     <div class="column">
       <h1>{{ ds.name }}
         {% if ds.database == source %}
-          {% if not ds.matched %}<button onclick="markMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-match">Mark matched</button> <a style="vertical-align: middle" class="button button-primary" href="{{ url_for('match', source=ds.id)}}">Match</a>{% else %}<button id="manual-match" style="vertical-align: middle">Matched</button>{% endif %}
+          {% if not ds.matched %}<button onclick="markMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-match">No match needed</button> <a style="vertical-align: middle" class="button button-primary" href="{{ url_for('match', source=ds.id)}}">Match</a>{% else %}<button id="manual-match" style="vertical-align: middle">Matched</button>{% endif %}
         {% endif %}
       </h1>
       <ul>
           <li>Database: {{ ds.database }}</li>
           <li>Location: {{ ds.location }}</li>
           <li>Unit: {{ ds.unit }}</li>
           <li>Comment: {{ds.comment }}</li>
           {% if same_name_count %}
               <li>Datasets with same name: {{ same_name_count }}: {% for obj in same_name %}<a href="{{ url_for('process_detail', id=obj.id) }}">{{obj.location}}</a> {% endfor %}</li>
           {% endif %}
 
       </ul>
       <h2>Technosphere Inputs</h2>
-      <table>
+      <table width="100%">
         <tr>
           <th>Amount</th>
           <th>Name</th>
           <th>Location</th>
           <th>Unit</th>
           {% if show_matching %}
             <th>Matched</th>
@@ -56,15 +56,15 @@
         </tr>
         {% endfor %}
       </table>
       <h2>Biosphere Inputs</h2>
       {% if biosphere|length > 50 or not biosphere|length %}
       <p>{{ biosphere|length }} biosphere exchanges</p>
       {% else %}
-      <table>
+      <table width="100%">
         <tr>
           <th>Amount</th>
           <th>Name</th>
           <th>Categories</th>
           <th>Unit</th>
         </tr>
         {% for exc in biosphere %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% include 'header.html' %}
 {% include 'navigation.html' %}
-****** {{ ds.name }} {% if ds.database == source %} {% if not ds.matched %}Mark
-matched Match{% else %}Matched{% endif %} {% endif %} ******
+****** {{ ds.name }} {% if ds.database == source %} {% if not ds.matched %}No
+match needed Match{% else %}Matched{% endif %} {% endif %} ******
     * Database: {{ ds.database }}
     * Location: {{ ds.location }}
     * Unit: {{ ds.unit }}
     * Comment: {{ds.comment }}
     * {% if same_name_count %}
     * Datasets with same name: {{ same_name_count }}: {% for obj in same_name
       %}{{obj.location}} {% endfor %}
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.2.0/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.2.0/bw_matchbox/bin/matchbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,67 +33,73 @@
 
 CHANGES_TEMPLATE = {
     "name": "<change-this-please>",
     "licenses": [
         {
             "name": "CC BY 4.0",
             "path": "https://creativecommons.org/licenses/by/4.0/",
-            "title": "Creative Commons Attribution 4.0 International"
+            "title": "Creative Commons Attribution 4.0 International",
         }
     ],
     "version": "1.0.0",
     "description": "<change-this-please>",
     "created": None,
     "contributors": [
         {
-          "title": "<change-this-please>",
-          "path": "<change-this-please>",
-          "role": "author"
+            "title": "<change-this-please>",
+            "path": "<change-this-please>",
+            "role": "author",
         }
     ],
     "create-datasets": [],
     "create-exchanges": [],
     "delete": [],
     "disaggregate": [],
     "replace": [],
-    "update": []
+    "update": [],
 }
 
 
 def create_setup_files(filename, changesfile):
     if not filename.lower().endswith(".toml"):
         filename += ".toml"
     if not changesfile.lower().endswith(".json"):
         changesfile += ".json"
     with open(CWD / filename, "w") as f:
         f.write(CONFIG_TEMPLATE.format(CWD / changesfile))
         print("Created config file {}".format(CWD / filename))
     with open(CWD / changesfile, "w") as f:
-        CHANGES_TEMPLATE['created'] = datetime.datetime.now().isoformat()
+        CHANGES_TEMPLATE["created"] = datetime.datetime.now().isoformat()
         json.dump(CHANGES_TEMPLATE, f, ensure_ascii=False, indent=2)
         print("Created changes file {}".format(CWD / changesfile))
 
 
 def main():
     args = docopt(__doc__, version="bw_matchbox app 1.0")
 
-    if args['setup']:
+    if args["setup"]:
         create_setup_files("config.toml", "changes.json")
-    elif args['example_project']:
-        name = args['<project_name>'] or 'matchbox-example'
-        bi.install_project('USEEIO-1.1', name)
+    elif args["example_project"]:
+        name = args["<project_name>"] or "matchbox-example"
+        bi.install_project("USEEIO-1.1", name)
         bd.projects.set_current(name)
         bd.Database("USEEIO-1.1").copy("USEEIO-copy")
-        print(f"Create project {name}. Make sure to select `USEEIO-1.1` for one database and `USEEIO-copy` for the other.")
-    elif args['webapp']:
-        filepath = args['<config>']
+        print(
+            f"Create project {name}. Make sure to select `USEEIO-1.1` for one database and `USEEIO-copy` for the other."
+        )
+    elif args["webapp"]:
+        filepath = args["<config>"]
         port = int(args.get("--port", False) or 5000)
         host = "localhost" if args.get("--localhost", False) else "0.0.0.0"
 
-        app = configure_app(filepath, matchbox_app)
+        try:
+            app = configure_app(filepath, matchbox_app)
 
-        print("bw_matchbox webapp started on {}:{}".format(host, port))
-        app.run(host=host, port=port, debug=True)
+            print("bw_matchbox webapp started on {}:{}".format(host, port))
+            app.run(host=host, port=port, debug=True)
+        except Exception as err:
+            print("Error:", err)
+            raise err
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.2.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.2.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.2.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/data/dare.json` & `bw_matchbox-0.2.0/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/bw_matchbox/webapp.py` & `bw_matchbox-0.2.0/bw_matchbox/webapp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,83 @@
+from functools import total_ordering
 from bw2data.backends import ActivityDataset as AD
 from flask_httpauth import HTTPBasicAuth
 from pathlib import Path
+from peewee import fn
 from werkzeug.security import check_password_hash, generate_password_hash
 import bw2data as bd
 import flask
 import json
+import math
 import os
-import uuid
+import random
+import string
 import tomli
+import uuid
 
 
 BASE_DIR = Path(__file__).resolve().parent
 DATA_DIR = BASE_DIR / "data"
 
 matchbox_app = flask.Flask(
     "matchbox_app",
     static_folder=BASE_DIR / "assets",
-    template_folder=BASE_DIR / "assets" / "templates"
+    template_folder=BASE_DIR / "assets" / "templates",
 )
 matchbox_app.config["SECRET_KEY"] = os.urandom(24)
 
 auth = HTTPBasicAuth()
 
 
 @auth.verify_password
 def verify_password(username, password):
-    users = matchbox_app.config['mb_users']
+    users = matchbox_app.config["mb_users"]
     if username in users and check_password_hash(users.get(username), password):
         return username
 
 
 def configure_app(filepath, app):
     try:
         config_fp = Path(filepath)
         assert config_fp.exists
         with open(config_fp, "rb") as f:
             config = tomli.load(f)
-        assert 'users' in config
+        assert "users" in config
     except:
+        # NOTE: If you got this exception, make sure first you don't have
+        # windows-style backslahes in your config file for file names (no
+        # double `\\`).
         raise ValueError("Invalid or unreadable config file")
 
     app.config["mb_users"] = {
         user: generate_password_hash(password)
-        for user, password in config['users'].items()
+        for user, password in config["users"].items()
     }
-    app.config["mb_changes_file"] = config['files']['changes_file']
+    app.config["mb_changes_file"] = config["files"]["changes_file"]
     try:
         json.load(open(app.config["mb_changes_file"], "rb"))
     except:
         raise ValueError("Can't read changes file")
     return app
 
 
 def get_context():
-    project = flask.request.cookies.get('project')
+    project = flask.request.cookies.get("project")
     if not project:
         return flask.redirect(flask.url_for("select_project"))
-    source = flask.request.cookies.get('source')
-    target = flask.request.cookies.get('target')
+    source = flask.request.cookies.get("source")
+    target = flask.request.cookies.get("target")
     if not (source and target):
         return flask.redirect(flask.url_for("select_databases"))
-    proxy = flask.request.cookies.get('proxy')
+    proxy = flask.request.cookies.get("proxy")
     return project, source, target, proxy
 
 
 def get_files():
-    files = flask.request.cookies.get('files')
+    files = flask.request.cookies.get("files")
     if files:
         files = json.loads(files)
     else:
         included = filter(lambda x: x.suffix.lower() == ".json", DATA_DIR.iterdir())
         files = [
             {
                 "index": str(index),
@@ -79,127 +87,136 @@
                 "enabled": True,
             }
             for index, path in enumerate(included)
         ]
     return files
 
 
-@matchbox_app.route('/project', methods = ['POST', 'GET'])
+@matchbox_app.route("/project", methods=["POST", "GET"])
 @auth.login_required
 def select_project():
     files = get_files()
 
-    if flask.request.method == 'POST':
-        project = flask.request.form['project']
+    if flask.request.method == "POST":
+        project = flask.request.form["project"]
         resp = flask.make_response(flask.redirect(flask.url_for("select_databases")))
-        resp.set_cookie('project', project)
+        resp.set_cookie("project", project)
         return resp
     else:
-        resp = flask.make_response(flask.render_template(
-            "project.html",
-            file_number=sum(1 for obj in files if obj['enabled']),
-            projects=[o for o in bd.projects],
-            user=auth.current_user(),
-            changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
-        ))
+        resp = flask.make_response(
+            flask.render_template(
+                "project.html",
+                file_number=sum(1 for obj in files if obj["enabled"]),
+                projects=[o for o in bd.projects],
+                user=auth.current_user(),
+                changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
+            )
+        )
         resp.delete_cookie("project")
         resp.delete_cookie("source")
         resp.delete_cookie("target")
         return resp
 
 
-@matchbox_app.route('/databases', methods = ['POST', 'GET'])
+@matchbox_app.route("/databases", methods=["POST", "GET"])
 @auth.login_required
 def select_databases():
-    project = flask.request.cookies.get('project')
+    project = flask.request.cookies.get("project")
     if not project:
         return flask.redirect(flask.url_for("select_project"))
     bd.projects.set_current(project)
 
     files = get_files()
 
-    if flask.request.method == 'POST':
-        source = flask.request.form['source']
-        target = flask.request.form['target']
-        use_proxy = 'use-proxy' in flask.request.form
-        proxy_existing = flask.request.form['proxy-existing']
-        proxy_new = flask.request.form['proxy-new'].strip()
+    if flask.request.method == "POST":
+        source = flask.request.form["source"]
+        target = flask.request.form["target"]
+        use_proxy = "use-proxy" in flask.request.form
+        proxy_existing = flask.request.form["proxy-existing"]
+        proxy_new = flask.request.form["proxy-new"].strip()
         if source != target:
             resp = flask.make_response(flask.redirect(flask.url_for("index")))
-            resp.set_cookie('source', source)
-            resp.set_cookie('target', target)
+            resp.set_cookie("source", source)
+            resp.set_cookie("target", target)
 
             if use_proxy:
                 if proxy_new:
                     bd.Database(proxy_new).register()
-                    resp.set_cookie('proxy', proxy_new)
+                    resp.set_cookie("proxy", proxy_new)
                 else:
-                    resp.set_cookie('proxy', proxy_existing)
+                    resp.set_cookie("proxy", proxy_existing)
             else:
-                resp.set_cookie('proxy', "")
+                resp.set_cookie("proxy", "")
 
             return resp
 
-    resp = flask.make_response(flask.render_template(
-        "databases.html",
-        project=project,
-        file_number=sum(1 for obj in files if obj['enabled']),
-        user=auth.current_user(),
-        changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
-        databases=bd.databases,
-    ))
+    resp = flask.make_response(
+        flask.render_template(
+            "databases.html",
+            project=project,
+            file_number=sum(1 for obj in files if obj["enabled"]),
+            user=auth.current_user(),
+            changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
+            databases=bd.databases,
+        )
+    )
     resp.delete_cookie("source")
     resp.delete_cookie("target")
     return resp
 
 
-@matchbox_app.route('/files', methods = ['POST', 'GET'])
+@matchbox_app.route("/files", methods=["POST", "GET"])
 @auth.login_required
 def select_matching_files():
     context = get_context()
     if isinstance(context, flask.Response):
         proj, s, t, proxy = None, None, None, None
     else:
         proj, s, t, proxy = context
 
     files = get_files()
 
-    if flask.request.method == 'POST':
+    if flask.request.method == "POST":
         # Don't get unchecked elements in forms
         for line in files:
-            line['enabled'] = False
+            line["enabled"] = False
 
         for key, value in flask.request.form.items():
             index = key.replace("enabled-", "")
             for line in files:
-                if line['index'] == index:
-                    line['enabled'] = value == "on"
+                if line["index"] == index:
+                    line["enabled"] = value == "on"
 
             resp = flask.make_response(flask.redirect(flask.url_for("index")))
-            resp.set_cookie('files', json.dumps(files))
+            resp.set_cookie("files", json.dumps(files))
             return resp
 
     # Format file cookie data for nicer form
     files_formatted = [
-        sorted([obj for obj in files if obj['dirpath'] == dirpath], key=lambda x: x['filename'])
-        for dirpath in sorted({obj['dirpath'] for obj in files})
+        sorted(
+            [obj for obj in files if obj["dirpath"] == dirpath],
+            key=lambda x: x["filename"],
+        )
+        for dirpath in sorted({obj["dirpath"] for obj in files})
     ]
 
-    resp = flask.make_response(flask.render_template(
-        "select_files.html",
-        files=files_formatted,
-        file_number=sum(1 for obj in files if obj['enabled']),
-        project=proj,
-        proxy=proxy,
-        source=s,
-        target=t,
-        user=auth.current_user(),
-        changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
-    ))
-    resp.set_cookie('files', json.dumps(files))
+    resp = flask.make_response(
+        flask.render_template(
+            "select_files.html",
+            files=files_formatted,
+            file_number=sum(1 for obj in files if obj["enabled"]),
+            project=proj,
+            proxy=proxy,
+            source=s,
+            target=t,
+            user=auth.current_user(),
+            changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
+        )
+    )
+    resp.set_cookie("files", json.dumps(files))
     return resp
 
 
 @matchbox_app.route("/", methods=["GET"])
 @auth.login_required
 def index():
     context = get_context()
@@ -213,24 +230,98 @@
     return flask.render_template(
         "index.html",
         title="bw_matchbox Index Page",
         unmatched_link=True,
         project=proj,
         source=s,
         target=t,
-        file_number=sum(1 for obj in files if obj['enabled']),
+        file_number=sum(1 for obj in files if obj["enabled"]),
         table_data=[obj for obj, _ in zip(bd.Database(s), range(50))],
         query_string="",
         database=s,
         proxy=proxy,
         user=auth.current_user(),
         changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
     )
 
 
+@matchbox_app.route("/processes", methods=["GET"])
+@auth.login_required
+def processes():
+    """API Endpoint to get process data for dynamic table population.
+
+    GET args:
+
+        * database (str): Name of database to draw processes from. Defaults to source database (stored in cookie) if not given.
+        * order_by (str): Parameter to sort by. Random if not provided. Valid parameters:
+            * name (will be used 99% of the time)
+            * location
+            * product (short name for reference product)
+        * offset (int): Offset from beginning of sorted values. Zero-indexed. Only used if sorting.
+        * limit (int): Number of results to return
+
+    Response data format (JSON):
+
+    ```
+        [
+            {
+                'details_url': 'URL for `process_detail` page for this activity',
+                'match_url': 'URL for `match` page for this activity',
+                'matched': 'Boolean. Whether or not process is already matched.',
+                'id': 'Integer process ID',
+                'name': 'Process name',
+                'location': 'Process location',
+                'unit': 'Unit of reference product',
+            }
+        ]
+    ```
+    """
+    context = get_context()
+    proj, s, t, proxy = context
+    bd.projects.set_current(proj)
+
+    database_label = flask.request.args.get("database") or s
+    qs = AD.select().where(AD.database == database_label)
+
+    total_records = qs.count()
+
+    order_by = flask.request.args.get("order_by")
+    if order_by and order_by in ("name", "location", "product"):
+        qs = qs.order_by(getattr(AD, order_by))
+    else:
+        qs = qs.order_by(fn.Random())
+
+    offset = flask.request.args.get("offset")
+    if offset:
+        qs = qs.offset(int(offset))
+
+    limit = flask.request.args.get("limit")
+    if limit:
+        qs = qs.limit(int(limit))
+    else:
+        qs = qs.limit(50)
+
+    payload = {
+        "total_records": total_records,
+        "data": [
+            {
+                "details_url": flask.url_for("process_detail", id=obj.id),
+                "match_url": flask.url_for("match", source=obj.id),
+                "matched": bool(obj.data.get("matched")),
+                "id": obj.id,
+                "name": obj.name,
+                "location": obj.location,
+                "unit": obj.data["unit"],
+            }
+            for obj in qs
+        ],
+    }
+    return flask.jsonify(payload)
+
+
 @matchbox_app.route("/unmatched", methods=["GET"])
 @auth.login_required
 def unmatched():
     context = get_context()
     if isinstance(context, flask.Response):
         return context
     proj, s, t, proxy = context
@@ -242,15 +333,15 @@
         "index.html",
         title="Unmatched Processes",
         unmatched_link=False,
         project=proj,
         proxy=proxy,
         source=s,
         target=t,
-        file_number=sum(1 for obj in files if obj['enabled']),
+        file_number=sum(1 for obj in files if obj["enabled"]),
         table_data=[obj for obj, _ in zip(bd.Database(s), range(50))],
         query_string="",
         database=s,
         user=auth.current_user(),
         changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
     )
 
@@ -311,15 +402,15 @@
     else:
         search_db = flask.request.args.get("database")
         return flask.render_template(
             "index.html",
             project=proj,
             source=s,
             target=t,
-            file_number=sum(1 for obj in files if obj['enabled']),
+            file_number=sum(1 for obj in files if obj["enabled"]),
             proxy=proxy,
             user=auth.current_user(),
             title="bw_matchbox Search Result",
             table_data=bd.Database(search_db).search(q, limit=100),
             query_string=q,
             database=s,
         )
@@ -328,15 +419,15 @@
 @matchbox_app.route("/mark-matched/<id>", methods=["GET"])
 @auth.login_required
 def mark_matched(id):
     context = get_context()
     proj, s, t, proxy = context
     bd.projects.set_current(proj)
     node = bd.get_node(id=id)
-    node['matched'] = True
+    node["matched"] = True
     node.save()
     return ""
 
 
 @matchbox_app.route("/process/<id>", methods=["GET"])
 @auth.login_required
 def process_detail(id):
@@ -344,28 +435,30 @@
     if isinstance(context, flask.Response):
         return context
     proj, s, t, proxy = context
     files = get_files()
     bd.projects.set_current(proj)
 
     node = bd.get_node(id=id)
-    same_name = AD.select().where(AD.name == node['name'], AD.database == node['database'], AD.id != node.id)
+    same_name = AD.select().where(
+        AD.name == node["name"], AD.database == node["database"], AD.id != node.id
+    )
     same_name_count = same_name.count()
-    technosphere = sorted(node.technosphere(), key=lambda x: x.input['name'])
-    biosphere = sorted(node.biosphere(), key=lambda x: x.input['name'])
+    technosphere = sorted(node.technosphere(), key=lambda x: x.input["name"])
+    biosphere = sorted(node.biosphere(), key=lambda x: x.input["name"])
 
     return flask.render_template(
         "process_detail.html",
         title="bw_matchbox Detail Page",
         ds=node,
         project=proj,
         proxy=proxy,
         source=s,
         target=t,
-        file_number=sum(1 for obj in files if obj['enabled']),
+        file_number=sum(1 for obj in files if obj["enabled"]),
         user=auth.current_user(),
         changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
         same_name_count=same_name_count,
         same_name=same_name,
         technosphere=technosphere,
         biosphere=biosphere,
         show_matching=False,
@@ -380,32 +473,73 @@
         return context
     proj, s, t, proxy = context
     files = get_files()
     bd.projects.set_current(proj)
 
     node = bd.get_node(id=source)
 
-    matches = bd.Database(t).search(node['name'] + " " + node.get('location', ''))
+    matches = bd.Database(t).search(node["name"] + " " + node.get("location", ""))
 
     return flask.render_template(
         "match.html",
         title="Database Matching Page",
         ds=node,
         project=proj,
         proxy=proxy,
         source=s,
         target=t,
-        file_number=sum(1 for obj in files if obj['enabled']),
+        file_number=sum(1 for obj in files if obj["enabled"]),
         user=auth.current_user(),
         changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
-        query_string=node['name'] + " " + node.get('location', ''),
-        matches=matches
+        query_string=node["name"] + " " + node.get("location", ""),
+        matches=matches,
+    )
+
+
+def normalize_name(string):
+    return (
+        string.lower()
+        .replace("market group for", "")
+        .replace("market for", "")
+        .replace(", at plant", "")
+        .strip()
     )
 
 
+def similar_location(a, b):
+    return any(
+        [
+            (b == a),
+            (b == "CH" and a in ("CH", "RER", "GLO", "RoW")),
+            (len(b) == 2 and a in ("GLO", "RoW")),
+            (b == "RER" and a in ("GLO", "RoW", "RoE")),
+        ]
+    )
+
+
+def check_similar(node, candidates):
+    for index, candidate in enumerate(candidates):
+        if node.get("collapsed") or candidate.get("collapsed"):
+            continue
+        if (
+            normalize_name(node["name"]) == normalize_name(candidate["name"])
+            and similar_location(node["location"], candidate["location"])
+            and node["unit"] == candidate["unit"]
+            and math.isclose(
+                node["amount"], candidate["amount"], rel_tol=0.025, abs_tol=1e-6
+            )
+        ):
+            node["collapsed"] = candidate["collapsed"] = True
+            node["collapsed-group"] = candidate[
+                "collapsed-group"
+            ] = "Collapsed-{}-{}".format(
+                index, "".join(random.choices(string.ascii_letters, k=6))
+            )
+
+
 @matchbox_app.route("/compare/<source>/<target>", methods=["GET"])
 @auth.login_required
 def compare(source, target):
     context = get_context()
     if isinstance(context, flask.Response):
         return context
     proj, s, t, proxy = context
@@ -414,57 +548,61 @@
     bd.projects.set_current(proj)
 
     source = bd.get_node(id=int(source))
     target = bd.get_node(id=int(target))
 
     source_technosphere = [
         {
-            'amount': exc['amount'],
-            'amount_display': '{:0.2g}'.format(exc['amount']),
-            'name': exc.input['name'],
-            'unit': exc.input['unit'],
-            'location': exc.input['location'],
-            'input_id': exc.input.id,
-            'url': flask.url_for("process_detail", id=exc.input.id),
+            "amount": exc["amount"],
+            "amount_display": "{:0.2g}".format(exc["amount"]),
+            "name": exc.input["name"],
+            "unit": exc.input["unit"],
+            "location": exc.input["location"],
+            "input_id": exc.input.id,
+            "url": flask.url_for("process_detail", id=exc.input.id),
         }
         for exc in source.technosphere()
     ]
     target_itself = {
-        'amount': 1,
-        'amount_display': "1.0",
-        'name': target['name'],
-        'unit': target['unit'],
-        'location': target.get('location', ''),
-        'input_id': target.id,
-        'url': flask.url_for("process_detail", id=target.id),
+        "amount": 1,
+        "amount_display": "1.0",
+        "name": target["name"],
+        "unit": target["unit"],
+        "location": target.get("location", ""),
+        "input_id": target.id,
+        "url": flask.url_for("process_detail", id=target.id),
     }
     target_technosphere = [
         {
-            'amount': exc['amount'],
-            'amount_display': '{:0.2g}'.format(exc['amount']),
-            'name': exc.input['name'],
-            'unit': exc.input['unit'],
-            'location': exc.input['location'],
-            'input_id': exc.input.id,
-            'url': flask.url_for("process_detail", id=exc.input.id),
+            "amount": exc["amount"],
+            "amount_display": "{:0.2g}".format(exc["amount"]),
+            "name": exc.input["name"],
+            "unit": exc.input["unit"],
+            "location": exc.input["location"],
+            "input_id": exc.input.id,
+            "url": flask.url_for("process_detail", id=exc.input.id),
         }
         for exc in target.technosphere()
     ]
 
+    for obj in target_technosphere:
+        # Modifies in place
+        check_similar(obj, source_technosphere)
+
     return flask.render_template(
         "compare.html",
         title="Database Comparison Page",
         project=proj,
         proxy=proxy,
         source=s,
         target=t,
         target_json=json.dumps(target_itself),
         user=auth.current_user(),
         changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
-        file_number=sum(1 for obj in files if obj['enabled']),
+        file_number=sum(1 for obj in files if obj["enabled"]),
         source_node=source,
         source_data_json=json.dumps(source_technosphere),
         target_node=target,
         target_data_json=json.dumps(target_technosphere),
     )
 
 
@@ -478,58 +616,60 @@
 
     bd.projects.set_current(proj)
     node = bd.get_activity(id=int(id))
     scale = float(scale)
 
     exchanges = list(node.technosphere())
     for exc in exchanges:
-        exc['amount'] *= scale
+        exc["amount"] *= scale
 
     payload = [
         {
-            'amount': exc['amount'],
-            'amount_display': '{:0.2g}'.format(exc['amount']),
-            'name': exc.input['name'],
-            'unit': exc.input['unit'],
-            'location': exc.input['location'],
-            'input_id': exc.input.id,
-            'url': flask.url_for("process_detail", id=exc.input.id),
+            "amount": exc["amount"],
+            "amount_display": "{:0.2g}".format(exc["amount"]),
+            "name": exc.input["name"],
+            "unit": exc.input["unit"],
+            "location": exc.input["location"],
+            "input_id": exc.input.id,
+            "url": flask.url_for("process_detail", id=exc.input.id),
         }
         for exc in exchanges
     ]
     return flask.jsonify(payload)
 
 
 @matchbox_app.route("/create-proxy/", methods=["POST"])
 @auth.login_required
 def create_proxy():
     content = flask.request.get_json()
     proj, s, t, proxy = get_context()
     # files = get_files()
     bd.projects.set_current(proj)
 
-    source = bd.get_activity(id=content['source'])
+    source = bd.get_activity(id=content["source"])
     process = bd.Database(proxy).new_activity(
-        name=content['name'],
+        name=content["name"],
         code=uuid.uuid4().hex,
-        comment=content['comment'],
-        unit=source['unit'],
-        location=source['location'],
-        original_name=source['name'],
+        comment=content["comment"],
+        unit=source["unit"],
+        location=source["location"],
+        original_name=source["name"],
         original_id=source.id,
-        **{'reference product': source.get('reference product')}
+        **{"reference product": source.get("reference product")}
     )
     process.save()
 
     source_rp = source.rp_exchange()
-    process.new_edge(input=process, amount=source_rp['amount'], type="production").save()
-    for exc in content['exchanges']:
+    process.new_edge(
+        input=process, amount=source_rp["amount"], type="production"
+    ).save()
+    for exc in content["exchanges"]:
         process.new_edge(
             type="technosphere",
-            input=bd.get_activity(id=exc['input_id']),
-            amount=exc['amount'],
+            input=bd.get_activity(id=exc["input_id"]),
+            amount=exc["amount"],
         ).save()
 
-    source['matched'] = True
+    source["matched"] = True
     source.save()
 
     return flask.redirect(flask.url_for("process_detail", id=process.id))
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.2.0/bw_matchbox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.1.0
+Version: 0.2.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
@@ -59,14 +59,20 @@
 
 You can install _bw_matchbox_ via [pip] from [PyPI]:
 
 ```console
 pip install bw_matchbox
 ```
 
+It's possible to install the library itself for development purposes (in the cloned project):
+
+```console
+pip install -e .
+```
+
 This library depends on:
 
 * Brightway 2.5 (`brightway25`)
 * `docopt-ng`
 * `flask` and `flask_httpauth`
 * `tomli`
 * `werkzeug`
```

### Comparing `bw_matchbox-0.1.0/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.2.0/bw_matchbox.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,25 @@
 bw_matchbox.egg-info/PKG-INFO
 bw_matchbox.egg-info/SOURCES.txt
 bw_matchbox.egg-info/dependency_links.txt
 bw_matchbox.egg-info/entry_points.txt
 bw_matchbox.egg-info/not-zip-safe
 bw_matchbox.egg-info/requires.txt
 bw_matchbox.egg-info/top_level.txt
+bw_matchbox/assets/css/compare.css
 bw_matchbox/assets/css/customizations.css
+bw_matchbox/assets/css/layout.css
 bw_matchbox/assets/css/normalize.css
 bw_matchbox/assets/css/skeleton.css
 bw_matchbox/assets/css/tooltip.css
 bw_matchbox/assets/images/favicon.ico
+bw_matchbox/assets/js/common-helpers.js
+bw_matchbox/assets/js/compare-core.js
+bw_matchbox/assets/js/compare-row-click.js
+bw_matchbox/assets/js/compare-rows-helpers.js
 bw_matchbox/assets/templates/compare.html
 bw_matchbox/assets/templates/databases.html
 bw_matchbox/assets/templates/expand.html
 bw_matchbox/assets/templates/file.html
 bw_matchbox/assets/templates/footer.html
 bw_matchbox/assets/templates/header.html
 bw_matchbox/assets/templates/index.html
```

### Comparing `bw_matchbox-0.1.0/docs/conf.py` & `bw_matchbox-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.1.0/setup.cfg` & `bw_matchbox-0.2.0/setup.cfg`

 * *Files identical despite different names*

