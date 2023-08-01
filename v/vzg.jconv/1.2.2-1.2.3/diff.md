# Comparing `tmp/vzg.jconv-1.2.2.tar.gz` & `tmp/vzg.jconv-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vzg.jconv-1.2.2.tar", last modified: Fri Jul 28 14:01:32 2023, max compression
+gzip compressed data, was "vzg.jconv-1.2.3.tar", last modified: Tue Aug  1 07:36:14 2023, max compression
```

## Comparing `vzg.jconv-1.2.2.tar` & `vzg.jconv-1.2.3.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/
--rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.2.2/LICENSE.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.2.2/MANIFEST.in
--rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.2.2/README.md
--rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-07-28 14:00:41.000000 vzg.jconv-1.2.2/VERSION.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/setup.cfg
--rw-rw-r--   0 teg       (1000) teg       (1000)     1679 2023-02-16 10:38:51.000000 vzg.jconv-1.2.2/setup.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.391660 vzg.jconv-1.2.2/src/
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/
--rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.2.2/src/vzg/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/
--rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.2.2/src/vzg/jconv/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/converter/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.2.2/src/vzg/jconv/converter/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    21834 2023-07-24 11:52:45.000000 vzg.jconv-1.2.2/src/vzg/jconv/converter/jats.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.2.2/src/vzg/jconv/errors.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1278 2023-07-24 11:43:22.000000 vzg.jconv-1.2.2/src/vzg/jconv/gapi.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      875 2020-02-08 12:51:55.000000 vzg.jconv-1.2.2/src/vzg/jconv/interfaces.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/langcode/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.2.2/src/vzg/jconv/langcode/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.2.2/src/vzg/jconv/langcode/language-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/person/
--rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-07-21 15:51:03.000000 vzg.jconv-1.2.2/src/vzg/jconv/person/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/publisher/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1314 2023-07-28 13:58:32.000000 vzg.jconv-1.2.2/src/vzg/jconv/publisher/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.2.2/src/vzg/jconv/publisher/publisher-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/schema/
--rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.2.2/src/vzg/jconv/schema/article_schema.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/test/
--rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.2.2/src/vzg/jconv/test/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 15:51:03.000000 vzg.jconv-1.2.2/src/vzg/jconv/test/conftest.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:51:03.000000 vzg.jconv-1.2.2/src/vzg/jconv/test/test_jats_article.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     3151 2023-07-21 15:51:03.000000 vzg.jconv-1.2.2/src/vzg/jconv/test/test_jats_converter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     4936 2023-07-21 15:51:03.000000 vzg.jconv-1.2.2/src/vzg/jconv/test/test_jats_degruyter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.2.2/src/vzg/jconv/test/test_langcode.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.2.2/src/vzg/jconv/test/test_person.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.2.2/src/vzg/jconv/test/test_publisher.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/tools/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.2.2/src/vzg/jconv/tools/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-07-21 15:51:03.000000 vzg.jconv-1.2.2/src/vzg/jconv/tools/simple_conv.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg/jconv/utils/
--rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-07-24 11:56:32.000000 vzg.jconv-1.2.2/src/vzg/jconv/utils/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1644 2020-09-25 10:34:55.000000 vzg.jconv-1.2.2/src/vzg/jconv/utils/date.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-28 14:01:32.395660 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/
--rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-07-28 14:01:32.000000 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)     1211 2023-07-28 14:01:32.000000 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/SOURCES.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-07-28 14:01:32.000000 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/dependency_links.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-07-28 14:01:32.000000 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/entry_points.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-07-28 14:01:32.000000 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/namespace_packages.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/not-zip-safe
--rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-07-28 14:01:32.000000 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/requires.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-07-28 14:01:32.000000 vzg.jconv-1.2.2/src/vzg.jconv.egg-info/top_level.txt
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.2.3/LICENSE.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.2.3/MANIFEST.in
+-rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.2.3/README.md
+-rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-08-01 07:35:40.000000 vzg.jconv-1.2.3/VERSION.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/setup.cfg
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1679 2023-02-16 10:38:51.000000 vzg.jconv-1.2.3/setup.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.025975 vzg.jconv-1.2.3/src/
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/
+-rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.2.3/src/vzg/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.2.3/src/vzg/jconv/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/converter/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.2.3/src/vzg/jconv/converter/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    15018 2023-07-31 15:01:19.000000 vzg.jconv-1.2.3/src/vzg/jconv/converter/jats.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.2.3/src/vzg/jconv/errors.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4144 2023-07-31 15:01:19.000000 vzg.jconv-1.2.3/src/vzg/jconv/gapi.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1112 2023-07-31 15:01:19.000000 vzg.jconv-1.2.3/src/vzg/jconv/interfaces.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/journal/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6603 2023-07-31 15:28:18.000000 vzg.jconv-1.2.3/src/vzg/jconv/journal/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/langcode/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.2.3/src/vzg/jconv/langcode/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.2.3/src/vzg/jconv/langcode/language-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/person/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-07-21 15:51:03.000000 vzg.jconv-1.2.3/src/vzg/jconv/person/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/publisher/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1314 2023-07-28 13:58:32.000000 vzg.jconv-1.2.3/src/vzg/jconv/publisher/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.2.3/src/vzg/jconv/publisher/publisher-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/schema/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.2.3/src/vzg/jconv/schema/article_schema.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/test/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 15:51:03.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/conftest.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:51:03.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/test_jats_article.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     3627 2023-08-01 07:25:20.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/test_jats_converter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     7302 2023-08-01 07:22:39.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/test_jats_degruyter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4008 2023-07-31 15:20:44.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/test_journal.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/test_langcode.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/test_person.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.2.3/src/vzg/jconv/test/test_publisher.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/tools/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.2.3/src/vzg/jconv/tools/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-07-21 15:51:03.000000 vzg.jconv-1.2.3/src/vzg/jconv/tools/simple_conv.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg/jconv/utils/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-07-24 11:56:32.000000 vzg.jconv-1.2.3/src/vzg/jconv/utils/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1644 2020-09-25 10:34:55.000000 vzg.jconv-1.2.3/src/vzg/jconv/utils/date.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-01 07:36:14.029975 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-08-01 07:36:14.000000 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1280 2023-08-01 07:36:14.000000 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-08-01 07:36:14.000000 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-08-01 07:36:14.000000 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/entry_points.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-01 07:36:14.000000 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/namespace_packages.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/not-zip-safe
+-rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-08-01 07:36:14.000000 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/requires.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-01 07:36:14.000000 vzg.jconv-1.2.3/src/vzg.jconv.egg-info/top_level.txt
```

### Comparing `vzg.jconv-1.2.2/LICENSE.txt` & `vzg.jconv-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/PKG-INFO` & `vzg.jconv-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
```

### Comparing `vzg.jconv-1.2.2/setup.py` & `vzg.jconv-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/interfaces.py` & `vzg.jconv-1.2.3/src/vzg/jconv/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: UTF-8 -*-
 """Interfaces
 ##############################################################################
 #
-# Copyright (c) 2020 Verbundzentrale des GBV.
+# Copyright (c) 2020-2023 Verbundzentrale des GBV.
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
 # Imports
 from zope.interface import Attribute, Interface
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
-__docformat__ = 'plaintext'
+__docformat__ = "plaintext"
 
 
 class IArticle(Interface):
     """VZG Article"""
 
     journal = Attribute("Journal")
     json = Attribute("Article as JSON object")
@@ -28,7 +28,18 @@
 class IConverter(Interface):
     """Converter"""
 
     articles = Attribute("List of IArticle objects")
 
     def run(self):
         """Start the conversion"""
+
+
+class IJournal(Interface):
+    """Journal"""
+
+    def as_dict(self):
+        """Dict representation"""
+
+    journal_ids = Attribute("List of journal identifier")
+    title = Attribute("Journal title")
+    year = Attribute("Year")
```

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/langcode/__init__.py` & `vzg.jconv-1.2.3/src/vzg/jconv/langcode/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/langcode/language-codes.json` & `vzg.jconv-1.2.3/src/vzg/jconv/langcode/language-codes.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/person/__init__.py` & `vzg.jconv-1.2.3/src/vzg/jconv/person/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/publisher/__init__.py` & `vzg.jconv-1.2.3/src/vzg/jconv/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/schema/article_schema.json` & `vzg.jconv-1.2.3/src/vzg/jconv/schema/article_schema.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/test/__init__.py` & `vzg.jconv-1.2.3/src/vzg/jconv/test/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/test/conftest.py` & `vzg.jconv-1.2.3/src/vzg/jconv/test/conftest.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/test/test_jats_article.py` & `vzg.jconv-1.2.3/src/vzg/jconv/test/test_jats_article.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/test/test_jats_converter.py` & `vzg.jconv-1.2.3/src/vzg/jconv/test/test_jats_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class AricleConverter(unittest.TestCase):
     def setUp(self):
         unittest.TestCase.setUp(self)
 
         self.fpaths = {
             "emerald": Path("data/tests/emerald/article_emerald.xml"),
             "degruyter": Path("data/tests/degruyter/article.xml"),
+            "degruyter_abbrev": Path("data/tests/degruyter/article_abbrev.xml"),
             "springer": Path("data/tests/springer/article.xml"),
         }
 
         self.fpath = self.fpaths["springer"]
 
     def tearDown(self):
         unittest.TestCase.tearDown(self)
@@ -102,14 +103,27 @@
 
         self.assertTrue(len(jconv.articles) == 0, "articles")
 
         jconv.run()
 
         self.assertTrue(len(jconv.articles) == 2, "articles")
 
+        for article in jconv.articles:
+            self.assertIsInstance(article, JatsArticle, "article")
+
+    def test07(self):
+        """validate degruyter abbrev"""
+        jconv = JatsConverter(self.fpaths["degruyter_abbrev"], validate=True)
+
+        self.assertTrue(len(jconv.articles) == 0, "articles")
+
+        jconv.run()
+
+        self.assertTrue(len(jconv.articles) == 2, "articles")
+
         for article in jconv.articles:
             self.assertIsInstance(article, JatsArticle, "article")
 
 
 # if __name__ == "__main__":
 #     suite = unittest.TestSuite()
 #     suite.addTest(unittest.makeSuite(AricleConverter))
```

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/test/test_jats_degruyter.py` & `vzg.jconv-1.2.3/src/vzg/jconv/test/test_jats_degruyter.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         """primary_id"""
         self.assertEqual(
             self.jobj.primary_id, self.testdata["primary_id"], "primary_id"
         )
 
     def test04(self):
         """journal"""
+        print(self.jobj.journal)
         self.assertEqual(self.jobj.journal, self.testdata["journal"], "journal")
 
     def test05(self):
         """other_ids"""
         self.assertEqual(self.jobj.other_ids, self.testdata["other_ids"], "other_ids")
 
     def test06(self):
@@ -162,7 +163,84 @@
         """dateOfProduction"""
         self.assertNotIn("dateOfProduction", self.jobj.jdict, "dateOfProduction")
 
     def test12(self):
         """eissn überprüfen"""
         itypes = [entry["type"] for entry in self.jobj.journal["journal_ids"]]
         self.assertIn("eissn", itypes, "eissn")
+
+
+class PPubAbbrevArticle(unittest.TestCase):
+    def setUp(self):
+        unittest.TestCase.setUp(self)
+
+        self.fpath = Path("data/tests/degruyter/article_abbrev.xml")
+        self.jpath = Path("data/tests/degruyter/article_abbrev_ppub.json")
+
+        with open(self.jpath) as fh:
+            self.testdata = json.load(fh)
+
+        with open(self.fpath, "rb") as fh:
+            self.dom = etree.parse(fh)
+
+        self.jobj = JatsArticle(
+            self.dom,
+            JATS_SPRINGER_PUBTYPE.print,
+            pubtype_source=PUBTYPE_SOURCES.degruyter,
+        )
+
+    def tearDown(self):
+        unittest.TestCase.tearDown(self)
+
+    def test01(self):
+        """title"""
+        self.assertEqual(self.jobj.title, self.testdata["title"], "title")
+
+    def test02(self):
+        """lang_code"""
+        self.assertEqual(self.jobj.lang_code, self.testdata["lang_code"], "lang_code")
+
+    def test03(self):
+        """primary_id"""
+        self.assertEqual(
+            self.jobj.primary_id, self.testdata["primary_id"], "primary_id"
+        )
+
+    def test04(self):
+        """journal"""
+        self.assertEqual(self.jobj.journal, self.testdata["journal"], "journal")
+
+    def test05(self):
+        """other_ids"""
+        self.assertEqual(self.jobj.other_ids, self.testdata["other_ids"], "other_ids")
+
+    def test06(self):
+        """persons"""
+        self.assertEqual(self.jobj.persons, self.testdata["persons"], "persons")
+
+    def test07(self):
+        """copyright"""
+        self.assertEqual(self.jobj.copyright, self.testdata["copyright"], "copyright")
+
+    def test08(self):
+        """abstracts"""
+        self.assertEqual(self.jobj.abstracts, self.testdata["abstracts"], "abstracts")
+
+    def test09(self):
+        """urls"""
+        self.assertNotIn("urls", self.testdata, "urls")
+
+    def test10(self):
+        """subjects"""
+        self.assertEqual(
+            self.jobj.subjects, self.testdata["subject_terms"], "subject_terms"
+        )
+
+    def test11(self):
+        """dateOfProduction"""
+        self.assertNotIn("dateOfProduction", self.jobj.jdict, "dateOfProduction")
+
+    def test12(self):
+        """eissn überprüfen"""
+        itypes = [entry["type"] for entry in self.jobj.journal["journal_ids"]]
+        self.assertIn("eissn", itypes, "eissn")
+        self.assertIn("pissn", itypes, "pissn")
```

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/test/test_langcode.py` & `vzg.jconv-1.2.3/src/vzg/jconv/test/test_langcode.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/test/test_person.py` & `vzg.jconv-1.2.3/src/vzg/jconv/test/test_person.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/test/test_publisher.py` & `vzg.jconv-1.2.3/src/vzg/jconv/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/tools/simple_conv.py` & `vzg.jconv-1.2.3/src/vzg/jconv/tools/simple_conv.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/utils/__init__.py` & `vzg.jconv-1.2.3/src/vzg/jconv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg/jconv/utils/date.py` & `vzg.jconv-1.2.3/src/vzg/jconv/utils/date.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.2/src/vzg.jconv.egg-info/PKG-INFO` & `vzg.jconv-1.2.3/src/vzg.jconv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
```

### Comparing `vzg.jconv-1.2.2/src/vzg.jconv.egg-info/SOURCES.txt` & `vzg.jconv-1.2.3/src/vzg.jconv.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 src/vzg.jconv.egg-info/top_level.txt
 src/vzg/jconv/__init__.py
 src/vzg/jconv/errors.py
 src/vzg/jconv/gapi.py
 src/vzg/jconv/interfaces.py
 src/vzg/jconv/converter/__init__.py
 src/vzg/jconv/converter/jats.py
+src/vzg/jconv/journal/__init__.py
 src/vzg/jconv/langcode/__init__.py
 src/vzg/jconv/langcode/language-codes.json
 src/vzg/jconv/person/__init__.py
 src/vzg/jconv/publisher/__init__.py
 src/vzg/jconv/publisher/publisher-codes.json
 src/vzg/jconv/schema/article_schema.json
 src/vzg/jconv/test/__init__.py
 src/vzg/jconv/test/conftest.py
 src/vzg/jconv/test/test_jats_article.py
 src/vzg/jconv/test/test_jats_converter.py
 src/vzg/jconv/test/test_jats_degruyter.py
+src/vzg/jconv/test/test_journal.py
 src/vzg/jconv/test/test_langcode.py
 src/vzg/jconv/test/test_person.py
 src/vzg/jconv/test/test_publisher.py
 src/vzg/jconv/tools/__init__.py
 src/vzg/jconv/tools/simple_conv.py
 src/vzg/jconv/utils/__init__.py
 src/vzg/jconv/utils/date.py
```

