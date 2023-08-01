# Comparing `tmp/cubicweb-book-0.8.2.tar.gz` & `tmp/cubicweb-book-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-book-0.8.2.tar", last modified: Wed Oct 16 06:59:38 2019, max compression
+gzip compressed data, was "cubicweb-book-0.8.3.tar", last modified: Tue Aug  1 15:11:45 2023, max compression
```

## Comparing `cubicweb-book-0.8.2.tar` & `cubicweb-book-0.8.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      312 2018-12-11 11:38:28.000000 cubicweb-book-0.8.2/MANIFEST.in
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2610 2019-02-28 09:17:08.000000 cubicweb-book-0.8.2/setup.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book.egg-info/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       39 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book.egg-info/entry_points.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       14 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book.egg-info/top_level.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book.egg-info/not-zip-safe
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1321 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book.egg-info/SOURCES.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       68 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book.egg-info/requires.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book.egg-info/dependency_links.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      840 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book.egg-info/PKG-INFO
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     5161 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/hooks.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2511 2019-10-15 17:29:41.000000 cubicweb-book-0.8.2/cubicweb_book/entities.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1083 2019-10-16 06:56:19.000000 cubicweb-book-0.8.2/cubicweb_book/__pkginfo__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book/bin/
--rwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)      981 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/bin/import-openlibrary.py
--rwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)     1316 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/bin/add-books.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book/i18n/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     6453 2018-12-11 11:38:28.000000 cubicweb-book-0.8.2/cubicweb_book/i18n/fr.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     5297 2018-12-11 11:38:28.000000 cubicweb-book-0.8.2/cubicweb_book/i18n/es.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     5627 2018-12-11 11:38:28.000000 cubicweb-book-0.8.2/cubicweb_book/i18n/en.po
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       93 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/uiprops.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2532 2019-10-15 17:29:49.000000 cubicweb-book-0.8.2/cubicweb_book/schema.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2725 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/olapi.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      390 2019-02-28 09:17:08.000000 cubicweb-book-0.8.2/cubicweb_book/site_cubicweb.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book/views/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2596 2019-05-07 08:58:42.000000 cubicweb-book-0.8.2/cubicweb_book/views/secondaries.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2131 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/views/bibo.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     4987 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/views/primaries.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      768 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/views/facet.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      746 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/views/urls.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1209 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/views/boxes.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      965 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/views/__init__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book/migration/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2649 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/migration/import_freebase.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     6777 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/migration/import_dbpedia.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       26 2019-02-28 09:17:08.000000 cubicweb-book-0.8.2/cubicweb_book/migration/0.7.1_Any.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       26 2019-02-28 09:17:08.000000 cubicweb-book-0.8.2/cubicweb_book/migration/0.5.0_Any.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       65 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/migration/postcreate.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      290 2019-02-28 09:17:08.000000 cubicweb-book-0.8.2/cubicweb_book/migration/0.3.0_Any.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     9273 2019-04-23 14:04:58.000000 cubicweb-book-0.8.2/cubicweb_book/migration/import_ol.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)        0 2019-02-28 09:17:08.000000 cubicweb-book-0.8.2/cubicweb_book/migration/__init__.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       20 2019-02-28 09:17:08.000000 cubicweb-book-0.8.2/cubicweb_book/__init__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/cubicweb_book/data/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      975 2018-12-11 11:38:28.000000 cubicweb-book-0.8.2/cubicweb_book/data/blue_arrow.png
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      156 2018-12-11 11:38:28.000000 cubicweb-book-0.8.2/cubicweb_book/data/cubes.book.css
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     3910 2018-12-11 11:38:28.000000 cubicweb-book-0.8.2/cubicweb_book/data/default-cover.png
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       45 2018-12-11 11:38:28.000000 cubicweb-book-0.8.2/cubicweb_book/data/cubes.book.js
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       38 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/setup.cfg
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      840 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/PKG-INFO
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      320 2018-12-11 11:37:50.000000 cubicweb-book-0.8.2/README.rst
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-16 06:59:38.000000 cubicweb-book-0.8.2/test/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1077 2019-05-07 08:58:43.000000 cubicweb-book-0.8.2/test/test_book.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.329392 cubicweb-book-0.8.3/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      452 2023-08-01 15:09:16.000000 cubicweb-book-0.8.3/MANIFEST.in
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      729 2023-08-01 15:11:45.329392 cubicweb-book-0.8.3/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      320 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/README.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.325392 cubicweb-book-0.8.3/cubicweb_book/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       20 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1065 2023-08-01 15:09:13.000000 cubicweb-book-0.8.3/cubicweb_book/__pkginfo__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.325392 cubicweb-book-0.8.3/cubicweb_book/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      975 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/data/blue_arrow.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      156 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/data/cubes.book.css
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       45 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/data/cubes.book.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3910 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/data/default-cover.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2511 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5161 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/hooks.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.325392 cubicweb-book-0.8.3/cubicweb_book/i18n/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5627 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/i18n/en.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5297 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/i18n/es.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6453 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/i18n/fr.po
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.329392 cubicweb-book-0.8.3/cubicweb_book/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      290 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/migration/0.3.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       26 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/migration/0.5.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       26 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/migration/0.7.1_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/migration/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6777 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/migration/import_dbpedia.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2649 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/migration/import_freebase.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9273 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/migration/import_ol.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       65 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2725 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/olapi.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2532 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      390 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/site_cubicweb.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       93 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/uiprops.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.329392 cubicweb-book-0.8.3/cubicweb_book/views/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      965 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/views/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2131 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/views/bibo.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1209 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/views/boxes.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      768 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/views/facet.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4987 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/views/primaries.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2596 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/views/secondaries.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      746 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/cubicweb_book/views/urls.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.325392 cubicweb-book-0.8.3/cubicweb_book.egg-info/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      729 2023-08-01 15:11:45.000000 cubicweb-book-0.8.3/cubicweb_book.egg-info/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1284 2023-08-01 15:11:45.000000 cubicweb-book-0.8.3/cubicweb_book.egg-info/SOURCES.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2023-08-01 15:11:45.000000 cubicweb-book-0.8.3/cubicweb_book.egg-info/dependency_links.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       38 2023-08-01 15:11:45.000000 cubicweb-book-0.8.3/cubicweb_book.egg-info/entry_points.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2023-08-01 15:08:41.000000 cubicweb-book-0.8.3/cubicweb_book.egg-info/not-zip-safe
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      102 2023-08-01 15:11:45.000000 cubicweb-book-0.8.3/cubicweb_book.egg-info/requires.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       14 2023-08-01 15:11:45.000000 cubicweb-book-0.8.3/cubicweb_book.egg-info/top_level.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       38 2023-08-01 15:11:45.329392 cubicweb-book-0.8.3/setup.cfg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2610 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/setup.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.329392 cubicweb-book-0.8.3/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2023-08-01 15:11:45.329392 cubicweb-book-0.8.3/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        5 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/test/data/bootstrap_cubes
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1077 2023-08-01 15:05:09.000000 cubicweb-book-0.8.3/test/test_book.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      886 2023-08-01 15:10:32.000000 cubicweb-book-0.8.3/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-book-0.8.2/setup.py` & `cubicweb-book-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book.egg-info/SOURCES.txt` & `cubicweb-book-0.8.3/cubicweb_book.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MANIFEST.in
 README.rst
 setup.py
+tox.ini
 cubicweb_book/__init__.py
 cubicweb_book/__pkginfo__.py
 cubicweb_book/entities.py
 cubicweb_book/hooks.py
 cubicweb_book/olapi.py
 cubicweb_book/schema.py
 cubicweb_book/site_cubicweb.py
@@ -12,16 +13,14 @@
 cubicweb_book.egg-info/PKG-INFO
 cubicweb_book.egg-info/SOURCES.txt
 cubicweb_book.egg-info/dependency_links.txt
 cubicweb_book.egg-info/entry_points.txt
 cubicweb_book.egg-info/not-zip-safe
 cubicweb_book.egg-info/requires.txt
 cubicweb_book.egg-info/top_level.txt
-cubicweb_book/bin/add-books.py
-cubicweb_book/bin/import-openlibrary.py
 cubicweb_book/data/blue_arrow.png
 cubicweb_book/data/cubes.book.css
 cubicweb_book/data/cubes.book.js
 cubicweb_book/data/default-cover.png
 cubicweb_book/i18n/en.po
 cubicweb_book/i18n/es.po
 cubicweb_book/i18n/fr.po
@@ -36,8 +35,9 @@
 cubicweb_book/views/__init__.py
 cubicweb_book/views/bibo.py
 cubicweb_book/views/boxes.py
 cubicweb_book/views/facet.py
 cubicweb_book/views/primaries.py
 cubicweb_book/views/secondaries.py
 cubicweb_book/views/urls.py
-test/test_book.py
+test/test_book.py
+test/data/bootstrap_cubes
```

### Comparing `cubicweb-book-0.8.2/cubicweb_book/hooks.py` & `cubicweb-book-0.8.3/cubicweb_book/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/entities.py` & `cubicweb-book-0.8.3/cubicweb_book/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/__pkginfo__.py` & `cubicweb-book-0.8.3/cubicweb_book/__pkginfo__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # pylint: disable-msg=W0622
 """cubicweb-book application packaging information"""
 
-modname = 'book'
-distname = 'cubicweb-%s' % modname
+modname = "book"
+distname = "cubicweb-%s" % modname
 
-numversion = (0, 8, 2)
-version = '.'.join(str(num) for num in numversion)
+numversion = (0, 8, 3)
+version = ".".join(str(num) for num in numversion)
 
-license = 'LGPL'
-description = 'component to describe books for the CubicWeb framework'
-author = 'Logilab'
-author_email = 'contact@logilab.fr'
+license = "LGPL"
+description = "component to describe books for the CubicWeb framework"
+author = "Logilab"
+author_email = "contact@logilab.fr"
 long_desc = """
 This cube provides the entity type ``Book`` and uses the OpenLibrary API_
 to automatically fill the book's description
 
 Check out : `Fetching book descriptions and covers`_
 
 .. _`Fetching book descriptions and covers` : http://www.logilab.org/blogentry/9138
 .. _API : http://openlibrary.org/dev/docs/api
 """
-web = 'http://www.cubicweb.org/project/%s' % distname
+web = "http://www.cubicweb.org/project/%s" % distname
 
 classifiers = [
-    'Environment :: Web Environment',
-    'Framework :: CubicWeb',
-    'Programming Language :: Python',
-    'Programming Language :: JavaScript',
-    ]
-
-__depends__ = {'cubicweb': '>= 3.24.0',
-               'cubicweb-addressbook': None,
-               'cubicweb-person': None,
-               'cubicweb-file': None,
-               }
+    "Environment :: Web Environment",
+    "Framework :: CubicWeb",
+    "Programming Language :: Python",
+    "Programming Language :: JavaScript",
+]
+
+__depends__ = {
+    "cubicweb": ">= 3.24.0, <4.0.0",
+    "cubicweb-addressbook": ">=1.13.0,<2.0.0",
+    "cubicweb-person": "<2.0.0",
+    "cubicweb-file": "<4.0.0",
+}
```

### Comparing `cubicweb-book-0.8.2/cubicweb_book/i18n/fr.po` & `cubicweb-book-0.8.3/cubicweb_book/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/i18n/es.po` & `cubicweb-book-0.8.3/cubicweb_book/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/i18n/en.po` & `cubicweb-book-0.8.3/cubicweb_book/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/schema.py` & `cubicweb-book-0.8.3/cubicweb_book/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/olapi.py` & `cubicweb-book-0.8.3/cubicweb_book/olapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/views/secondaries.py` & `cubicweb-book-0.8.3/cubicweb_book/views/secondaries.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/views/bibo.py` & `cubicweb-book-0.8.3/cubicweb_book/views/bibo.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/views/primaries.py` & `cubicweb-book-0.8.3/cubicweb_book/views/primaries.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/views/facet.py` & `cubicweb-book-0.8.3/cubicweb_book/views/facet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/views/urls.py` & `cubicweb-book-0.8.3/cubicweb_book/views/urls.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/views/boxes.py` & `cubicweb-book-0.8.3/cubicweb_book/views/boxes.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/views/__init__.py` & `cubicweb-book-0.8.3/cubicweb_book/views/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/migration/import_freebase.py` & `cubicweb-book-0.8.3/cubicweb_book/migration/import_freebase.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/migration/import_dbpedia.py` & `cubicweb-book-0.8.3/cubicweb_book/migration/import_dbpedia.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/migration/import_ol.py` & `cubicweb-book-0.8.3/cubicweb_book/migration/import_ol.py`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/data/blue_arrow.png` & `cubicweb-book-0.8.3/cubicweb_book/data/blue_arrow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/cubicweb_book/data/default-cover.png` & `cubicweb-book-0.8.3/cubicweb_book/data/default-cover.png`

 * *Files identical despite different names*

### Comparing `cubicweb-book-0.8.2/test/test_book.py` & `cubicweb-book-0.8.3/test/test_book.py`

 * *Files identical despite different names*

