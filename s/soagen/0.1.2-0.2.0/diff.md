# Comparing `tmp/soagen-0.1.2.tar.gz` & `tmp/soagen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soagen-0.1.2.tar", last modified: Mon Jul 31 15:16:20 2023, max compression
+gzip compressed data, was "soagen-0.2.0.tar", last modified: Tue Aug  1 19:13:18 2023, max compression
```

## Comparing `soagen-0.1.2.tar` & `soagen-0.2.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.330018 soagen-0.1.2/
--rw-rw-rw-   0        0        0      128 2023-07-31 15:15:43.000000 soagen-0.1.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1445 2023-07-31 15:16:20.330018 soagen-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.1.2/README.md
--rw-rw-rw-   0        0        0     1893 2023-07-29 16:15:31.000000 soagen-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 15:16:20.330018 soagen-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.287018 soagen-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.308019 soagen-0.1.2/src/soagen/
--rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/__init__.py
--rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.1.2/src/soagen/column.py
--rw-rw-rw-   0        0        0     4923 2023-07-31 13:43:35.000000 soagen-0.1.2/src/soagen/config.py
--rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/configurable.py
--rw-rw-rw-   0        0        0    19129 2023-07-30 10:56:14.000000 soagen-0.1.2/src/soagen/cpp.py
--rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/errors.py
--rw-rw-rw-   0        0        0    10586 2023-07-31 14:13:28.000000 soagen-0.1.2/src/soagen/header_file.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.324019 soagen-0.1.2/src/soagen/hpp/
--rw-rw-rw-   0        0        0     5621 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/hpp/.clang-format
--rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/allocator.hpp
--rw-rw-rw-   0        0        0    31484 2023-07-31 13:53:03.000000 soagen-0.1.2/src/soagen/hpp/column_traits.hpp
-drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.328019 soagen-0.1.2/src/soagen/hpp/generated/
--rw-rw-rw-   0        0        0     9857 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/hpp/generated/compressed_pair.hpp
--rw-rw-rw-   0        0        0     2935 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/hpp/generated/core.hpp
--rw-rw-rw-   0        0        0     7897 2023-07-31 15:15:21.000000 soagen-0.1.2/src/soagen/hpp/generated/functions.hpp
--rw-rw-rw-   0        0        0    43678 2023-07-31 15:15:23.000000 soagen-0.1.2/src/soagen/hpp/generated/preprocessor.hpp
--rw-rw-rw-   0        0        0      420 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/hpp/generated/version.hpp
--rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/header_end.hpp
--rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/header_start.hpp
--rw-rw-rw-   0        0        0    15153 2023-07-31 14:45:32.000000 soagen-0.1.2/src/soagen/hpp/iterator.hpp
--rw-rw-rw-   0        0        0    25186 2023-07-31 12:16:29.000000 soagen-0.1.2/src/soagen/hpp/meta.hpp
--rw-rw-rw-   0        0        0     5469 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/mixins.hpp
--rw-rw-rw-   0        0        0     7280 2023-07-31 12:16:29.000000 soagen-0.1.2/src/soagen/hpp/row.hpp
-drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.328019 soagen-0.1.2/src/soagen/hpp/single/
--rw-rw-rw-   0        0        0   234186 2023-07-31 15:15:23.000000 soagen-0.1.2/src/soagen/hpp/single/soagen.hpp
--rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/soagen.hpp
--rw-rw-rw-   0        0        0    53592 2023-07-30 10:14:59.000000 soagen-0.1.2/src/soagen/hpp/table.hpp
--rw-rw-rw-   0        0        0    41432 2023-07-30 10:23:24.000000 soagen-0.1.2/src/soagen/hpp/table_traits.hpp
--rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.1.2/src/soagen/includes.py
--rw-rw-rw-   0        0        0     1103 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/injectors.py
--rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/log.py
--rw-rw-rw-   0        0        0    23157 2023-07-31 14:18:44.000000 soagen-0.1.2/src/soagen/main.py
--rw-rw-rw-   0        0        0     3018 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/metavars.py
--rw-rw-rw-   0        0        0     5174 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/natvis_file.py
--rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/paths.py
--rw-rw-rw-   0        0        0     6128 2023-07-30 10:13:46.000000 soagen-0.1.2/src/soagen/preprocessor.py
--rw-rw-rw-   0        0        0     2494 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/schemas.py
--rw-rw-rw-   0        0        0    66634 2023-07-31 14:13:37.000000 soagen-0.1.2/src/soagen/struct.py
--rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/type_list.py
--rw-rw-rw-   0        0        0     2697 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/utils.py
--rw-rw-rw-   0        0        0     3576 2023-07-30 14:09:00.000000 soagen-0.1.2/src/soagen/variable.py
--rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/version.py
--rw-rw-rw-   0        0        0        6 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/version.txt
--rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.1.2/src/soagen/writer.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.315019 soagen-0.1.2/src/soagen.egg-info/
--rw-rw-rw-   0        0        0     1445 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1387 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.1.2/src/soagen.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.831808 soagen-0.2.0/
+-rw-rw-rw-   0        0        0      515 2023-08-01 18:55:45.000000 soagen-0.2.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1844 2023-08-01 19:13:18.830810 soagen-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1893 2023-07-29 16:15:31.000000 soagen-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 19:13:18.831808 soagen-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.788809 soagen-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.810808 soagen-0.2.0/src/soagen/
+-rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/__init__.py
+-rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.2.0/src/soagen/column.py
+-rw-rw-rw-   0        0        0     5029 2023-08-01 15:35:54.000000 soagen-0.2.0/src/soagen/config.py
+-rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/configurable.py
+-rw-rw-rw-   0        0        0    19130 2023-08-01 16:02:29.000000 soagen-0.2.0/src/soagen/cpp.py
+-rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/errors.py
+-rw-rw-rw-   0        0        0    10577 2023-08-01 13:38:11.000000 soagen-0.2.0/src/soagen/header_file.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.824809 soagen-0.2.0/src/soagen/hpp/
+-rw-rw-rw-   0        0        0     5621 2023-08-01 18:58:28.000000 soagen-0.2.0/src/soagen/hpp/.clang-format
+-rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/allocator.hpp
+-rw-rw-rw-   0        0        0    31484 2023-08-01 17:51:18.000000 soagen-0.2.0/src/soagen/hpp/column_traits.hpp
+drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.828811 soagen-0.2.0/src/soagen/hpp/generated/
+-rw-rw-rw-   0        0        0     9857 2023-08-01 18:58:28.000000 soagen-0.2.0/src/soagen/hpp/generated/compressed_pair.hpp
+-rw-rw-rw-   0        0        0     2935 2023-08-01 18:58:28.000000 soagen-0.2.0/src/soagen/hpp/generated/core.hpp
+-rw-rw-rw-   0        0        0     7897 2023-08-01 18:58:29.000000 soagen-0.2.0/src/soagen/hpp/generated/functions.hpp
+-rw-rw-rw-   0        0        0    43876 2023-08-01 18:58:31.000000 soagen-0.2.0/src/soagen/hpp/generated/preprocessor.hpp
+-rw-rw-rw-   0        0        0      420 2023-08-01 15:39:54.000000 soagen-0.2.0/src/soagen/hpp/generated/version.hpp
+-rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/header_end.hpp
+-rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/header_start.hpp
+-rw-rw-rw-   0        0        0    15734 2023-08-01 12:49:39.000000 soagen-0.2.0/src/soagen/hpp/iterator.hpp
+-rw-rw-rw-   0        0        0    25587 2023-08-01 15:53:13.000000 soagen-0.2.0/src/soagen/hpp/meta.hpp
+-rw-rw-rw-   0        0        0     5469 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/mixins.hpp
+-rw-rw-rw-   0        0        0     7841 2023-08-01 16:10:41.000000 soagen-0.2.0/src/soagen/hpp/row.hpp
+drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.829811 soagen-0.2.0/src/soagen/hpp/single/
+-rw-rw-rw-   0        0        0   239553 2023-08-01 18:58:31.000000 soagen-0.2.0/src/soagen/hpp/single/soagen.hpp
+-rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/hpp/soagen.hpp
+-rw-rw-rw-   0        0        0    56712 2023-08-01 18:52:09.000000 soagen-0.2.0/src/soagen/hpp/table.hpp
+-rw-rw-rw-   0        0        0    42558 2023-08-01 18:52:19.000000 soagen-0.2.0/src/soagen/hpp/table_traits.hpp
+-rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.2.0/src/soagen/includes.py
+-rw-rw-rw-   0        0        0     1534 2023-08-01 12:05:38.000000 soagen-0.2.0/src/soagen/injectors.py
+-rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/log.py
+-rw-rw-rw-   0        0        0    22887 2023-08-01 15:36:32.000000 soagen-0.2.0/src/soagen/main.py
+-rw-rw-rw-   0        0        0     3018 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/metavars.py
+-rw-rw-rw-   0        0        0     5174 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/natvis_file.py
+-rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/paths.py
+-rw-rw-rw-   0        0        0     6128 2023-07-30 10:13:46.000000 soagen-0.2.0/src/soagen/preprocessor.py
+-rw-rw-rw-   0        0        0     2516 2023-08-01 12:07:40.000000 soagen-0.2.0/src/soagen/schemas.py
+-rw-rw-rw-   0        0        0    69042 2023-08-01 18:41:49.000000 soagen-0.2.0/src/soagen/struct.py
+-rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/type_list.py
+-rw-rw-rw-   0        0        0     2879 2023-08-01 11:51:16.000000 soagen-0.2.0/src/soagen/utils.py
+-rw-rw-rw-   0        0        0     3576 2023-07-30 14:09:00.000000 soagen-0.2.0/src/soagen/variable.py
+-rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.2.0/src/soagen/version.py
+-rw-rw-rw-   0        0        0        6 2023-08-01 15:39:54.000000 soagen-0.2.0/src/soagen/version.txt
+-rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.2.0/src/soagen/writer.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:13:18.815808 soagen-0.2.0/src/soagen.egg-info/
+-rw-rw-rw-   0        0        0     1844 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1387 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 19:13:18.000000 soagen-0.2.0/src/soagen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.2.0/src/soagen.egg-info/zip-safe
```

### Comparing `soagen-0.1.2/LICENSE.txt` & `soagen-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/PKG-INFO` & `soagen-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.1.2
+Version: 0.2.0
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,26 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.2.0
+
+-   Added `structs.annotations`
+-   Added `structs.attributes`
+-   Added `auto` option for `structs.default_constructible`
+-   Added `soagen::row_base`
+-   Added `soagen::table_base`
+-   Added `soagen::iterator_base`
+-   Added `Base` template argument to `soagen::table` for CRTP
+-   Added `swap_columns<>()`
+-   Made `column_indices` member struct into `enum class columns`
+
 ## v0.1.2
 
 -   Minor refactors.
 
 ## v0.1.1
 
 -   Minor refactors.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.1.2 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.2.0 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,9 +13,14 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor
-refactors. ## v0.1.0 - First public release ð&#xFE0F;
+sponsors/marzer # Changelog ## v0.2.0 - Added `structs.annotations` - Added
+`structs.attributes` - Added `auto` option for `structs.default_constructible`
+- Added `soagen::row_base` - Added `soagen::table_base` - Added `soagen::
+iterator_base` - Added `Base` template argument to `soagen::table` for CRTP -
+Added `swap_columns<>()` - Made `column_indices` member struct into `enum class
+columns` ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor refactors. ## v0.1.0 -
+First public release ð&#xFE0F;
```

### Comparing `soagen-0.1.2/pyproject.toml` & `soagen-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/column.py` & `soagen-0.2.0/src/soagen/column.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/config.py` & `soagen-0.2.0/src/soagen/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             for i in range(len(self.structs)):
                 with SchemaContext(rf"struct '{self.structs[i][0]}'"):
                     self.structs[i] = Struct(self, self.structs[i][0], self.structs[i][1])
             self.structs.sort(key=lambda s: s.name)
             self.struct_types = TypeList([s.type for s in self.structs])
             self.meta.push('struct_names', ', '.join([s.name for s in self.structs]))
             self.meta.push('struct_types', ', '.join([s.type for s in self.structs]))
+            self.meta.push('qualified_struct_names', ', '.join([s.qualified_type for s in self.structs]))
             self.meta.push('qualified_struct_types', ', '.join([s.qualified_type for s in self.structs]))
             index = 0
             for struct in self.structs:
                 struct.set_index(index)
                 index += 1
 
             # output file configs
```

### Comparing `soagen-0.1.2/src/soagen/configurable.py` & `soagen-0.2.0/src/soagen/configurable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/cpp.py` & `soagen-0.2.0/src/soagen/cpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -803,15 +803,15 @@
     # table machinery:
     r'aligned_stride',
     r'column_indices',
     r'column_name',
     r'column_traits',
     r'column_type',
     r'column',
-    r'column',
+    r'columns',
     r'emplacer',
     r'for_each_column',
     r'forward_type',
     r'get',
     r'param_type',
     r'row_type',
     r'row',
```

### Comparing `soagen-0.1.2/src/soagen/errors.py` & `soagen-0.2.0/src/soagen/errors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/header_file.py` & `soagen-0.2.0/src/soagen/header_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             #error soagen version mismatch - expected v{VERSION[0]}.{VERSION[1]}.X
           #endif
           '''
         )
 
         # external/system includes (#include <blah.h>)
         # (deferred until later so we can take advantage of detect_includes() for the whole file)
-        o('\n\n// #### SOAGEN_EXTERNAL_HEADERS #### \n\n')
+        o('\n\n// __SOAGEN_EXTERNAL_HEADERS\n\n')
 
         # misc preprocessor boilerplate
         o(
             rf'''
         SOAGEN_PUSH_WARNINGS;
         SOAGEN_DISABLE_SPAM_WARNINGS;
         #if SOAGEN_CLANG >= 16
```

### Comparing `soagen-0.1.2/src/soagen/hpp/.clang-format` & `soagen-0.2.0/src/soagen/hpp/.clang-format`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/allocator.hpp` & `soagen-0.2.0/src/soagen/hpp/allocator.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/column_traits.hpp` & `soagen-0.2.0/src/soagen/hpp/column_traits.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/generated/compressed_pair.hpp` & `soagen-0.2.0/src/soagen/hpp/generated/compressed_pair.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/generated/core.hpp` & `soagen-0.2.0/src/soagen/hpp/generated/core.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/generated/functions.hpp` & `soagen-0.2.0/src/soagen/hpp/generated/functions.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/generated/preprocessor.hpp` & `soagen-0.2.0/src/soagen/hpp/generated/preprocessor.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,16 @@
 		#define SOAGEN_HIDDEN_CONSTRAINT(condition, ...)
 	#endif
 #endif
 
 /// @cond
 #ifndef SOAGEN_CONSTRAINED_COLUMN
 	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)                                                                          \
-		SOAGEN_CONSTRAINED_TEMPLATE(sfinae_col_idx == (I) && (__VA_ARGS__), size_t sfinae_col_idx = (I))
+		SOAGEN_CONSTRAINED_TEMPLATE(sfinae_col_idx == static_cast<std::size_t>(I) && (__VA_ARGS__),                    \
+									std::size_t sfinae_col_idx = static_cast<std::size_t>(I))
 #endif
 /// @endcond
 #ifndef SOAGEN_CONSTRAINED_COLUMN
 	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)
 #endif
 
 #ifndef SOAGEN_PUSH_WARNINGS
@@ -929,15 +930,16 @@
 		SOAGEN_PURE_INLINE_GETTER                                                                                      \
 		SOAGEN_ATTR(returns_nonnull)
 #endif
 
 #ifndef SOAGEN_ALIGNED_COLUMN
 	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
 		SOAGEN_COLUMN(I)                                                                                               \
-		SOAGEN_ATTR(assume_aligned(soagen::detail::actual_column_alignment<table_traits, allocator_type, I>))
+		SOAGEN_ATTR(assume_aligned(                                                                                    \
+			soagen::detail::actual_column_alignment<table_traits, allocator_type, static_cast<std::size_t>(I)>))
 #endif
 
 #ifndef SOAGEN_ALWAYS_OPTIMIZE
 	#define SOAGEN_ALWAYS_OPTIMIZE 1
 #endif
 
 #ifndef SOAGEN_COMMA
```

### Comparing `soagen-0.1.2/src/soagen/hpp/header_end.hpp` & `soagen-0.2.0/src/soagen/hpp/header_end.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/header_start.hpp` & `soagen-0.2.0/src/soagen/hpp/header_start.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/iterator.hpp` & `soagen-0.2.0/src/soagen/hpp/iterator.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -87,19 +87,31 @@
 		{
 			std::add_const_t<remove_cvref<Table>>* table;
 			typename remove_cvref<Table>::difference_type offset;
 		};
 	}
 	/// @endcond
 
+	/// @brief		Base class for soagen::iterator.
+	/// @details	Specialize this to add functionality to all iterators of a particular type via CRTP.
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES iterator_base
+	{};
+
 	/// @brief RandomAccessIterator for soagen-generated table types.
 	template <typename Table, size_t... Columns>
-	class iterator ///
-		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>)
+	class SOAGEN_EMPTY_BASES iterator ///
+		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>,
+						   public iterator_base<iterator<Table, Columns...>>)
 	{
+		static_assert(std::is_empty_v<iterator_base<iterator<Table, Columns...>>>,
+					  "iterator_base specializations may not have data members");
+		static_assert(std::is_trivial_v<iterator_base<iterator<Table, Columns...>>>,
+					  "iterator_base specializations must be trivial");
+
 	  public:
 		/// @brief Base SoA table type for this iterator.
 		using table_type = remove_cvref<Table>;
 		static_assert(is_soa<table_type>, "soagen iterators are for use with soagen-generated SoA table types.");
 
 		/// @brief Cvref-qualified version of #table_type.
 		using table_ref = Table;
```

### Comparing `soagen-0.1.2/src/soagen/hpp/meta.hpp` & `soagen-0.2.0/src/soagen/hpp/meta.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -59,35 +59,37 @@
 			}                                                                                                          \
 		}
 #endif
 
 #ifndef SOAGEN_MAKE_COLUMN
 	#define SOAGEN_MAKE_COLUMN(Table, Column, Name)                                                                    \
 		template <>                                                                                                    \
-		struct column_name_<Table, Column> : name_constant_##Name                                                      \
+		struct column_name<Table, Column> : name_constant_##Name                                                       \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct col_ref_<Table&, Column>                                                                                \
-			: named_member_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, Column>>>                      \
+		struct column_ref<Table&, Column>                                                                              \
+			: named_member_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>> \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct col_ref_<Table&&, Column>                                                                               \
-			: named_member_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, Column>>>                      \
+		struct column_ref<Table&&, Column>                                                                             \
+			: named_member_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>> \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct col_ref_<const Table&, Column>                                                                          \
-			: named_member_##Name<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>    \
+		struct column_ref<const Table&, Column>                                                                        \
+			: named_member_##Name<std::add_lvalue_reference_t<                                                         \
+				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct col_ref_<const Table&&, Column>                                                                         \
-			: named_member_##Name<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>    \
+		struct column_ref<const Table&&, Column>                                                                       \
+			: named_member_##Name<std::add_rvalue_reference_t<                                                         \
+				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{}
 #endif
 
 namespace soagen
 {
 	/// @brief	Equivalent to C+20's std::remove_cvref_t.
 	template <typename T>
@@ -101,14 +103,19 @@
 	template <typename T>
 	using coerce_ref = std::conditional_t<std::is_reference_v<T>, T, std::add_lvalue_reference_t<T>>;
 
 	/// @brief	The identity type transformation.
 	template <typename T>
 	using identity_type = T;
 
+	/// @brief	The 'identity' base for CRTP scenarios (adds nothing to the interface).
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES identity_base
+	{};
+
 	/// @brief	True if `T` is `const` or `volatile` qualified.
 	template <typename T>
 	inline constexpr bool is_cv = !std::is_same_v<std::remove_cv_t<T>, T>;
 
 	/// @brief	True if `T` is (or is a reference to something that is) `const` or `volatile` qualified.
 	template <typename T>
 	inline constexpr bool is_cvref = !std::is_same_v<remove_cvref<T>, T>;
@@ -377,16 +384,17 @@
 	/// @endcond
 
 	/// @brief Gets the allocator being used by the #soagen::table of an SoA type.
 	template <typename T>
 	using allocator_type = POXY_IMPLEMENTATION_DETAIL(typename detail::allocator_type_<std::remove_cv_t<T>>::type);
 
 	/// @brief Gets the #soagen::column_traits::value_type for the selected column of an SoA type.
-	template <typename T, size_t Column>
-	using value_type = POXY_IMPLEMENTATION_DETAIL(typename table_traits_type<T>::template column<Column>::value_type);
+	template <typename T, auto Column>
+	using value_type = POXY_IMPLEMENTATION_DETAIL(
+		typename table_traits_type<T>::template column<static_cast<size_t>(Column)>::value_type);
 
 	/// @cond
 	namespace detail
 	{
 		template <typename ValueType>
 		struct storage_type_
 		{
@@ -592,17 +600,17 @@
 		}
 	}
 
 	/// @cond
 	namespace detail
 	{
 		template <typename Table, size_t ColumnIndex>
-		struct column_name_;
+		struct column_name;
 		template <typename Table, size_t ColumnIndex>
-		struct col_ref_;
+		struct column_ref;
 
 		template <typename A, typename B>
 		inline constexpr bool same_table_type =
 			std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>;
 	}
 	/// @endcond
 }
```

### Comparing `soagen-0.1.2/src/soagen/hpp/mixins.hpp` & `soagen-0.2.0/src/soagen/hpp/mixins.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/row.hpp` & `soagen-0.2.0/src/soagen/hpp/row.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -5,42 +5,52 @@
 #pragma once
 
 #include "meta.hpp"
 #include "header_start.hpp"
 
 namespace soagen
 {
+	/// @brief		Base class for soagen::row.
+	/// @details	Specialize this to add functionality to all rows of a particular type via CRTP.
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES row_base
+	{};
+
 	/// @brief A proxy type for treating (some subset of) an SoA row as if it were a regular AoS struct.
 	template <typename Table, size_t... Columns>
 	struct SOAGEN_EMPTY_BASES row //
-	SOAGEN_HIDDEN_BASE(public detail::col_ref_<Table, Columns>...)
+	SOAGEN_HIDDEN_BASE(public detail::column_ref<Table, Columns>..., public row_base<row<Table, Columns...>>)
 	{
 		static_assert(std::is_reference_v<Table>,
 					  "Table must be a reference so row members can derive their reference category");
+		static_assert(std::is_empty_v<row_base<row<Table, Columns...>>>,
+					  "row_base specializations may not have data members");
+		static_assert(std::is_trivial_v<row_base<row<Table, Columns...>>>, "row_base specializations must be trivial");
 
 		// columns:
 
-		template <size_t Column>
+		template <auto Column>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) column() const noexcept
 		{
-			static_assert(Column < table_traits_type<remove_cvref<Table>>::column_count, "column index out of range");
+			static_assert(static_cast<size_t>(Column) < table_traits_type<remove_cvref<Table>>::column_count,
+						  "column index out of range");
 
-			return detail::col_ref_<Table, Column>::get_named_member();
+			return detail::column_ref<Table, static_cast<size_t>(Column)>::get_named_member();
 		}
 
 		// tuple protocol:
 
-		template <size_t Member>
+		template <auto Member>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) get() const noexcept
 		{
 			static_assert(Member < sizeof...(Columns), "member index out of range");
 
-			return type_at_index<Member, detail::col_ref_<Table, Columns>...>::get_named_member();
+			return type_at_index<Member, detail::column_ref<Table, Columns>...>::get_named_member();
 		}
 
 		/// @name Equality
 		/// @availability These operators are only available when all the column types are equality-comparable.
 		/// @{
 
 		/// @brief Returns true if all of the elements in two rows are equal.
@@ -179,17 +189,17 @@
 		struct row_type_<Table, std::index_sequence<>>
 			: row_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
 		{};
 	}
 	/// @endcond
 
 	/// @brief		The #soagen::row for a given SoA type and (some subset of) its columns.
-	template <typename Table, size_t... Columns>
+	template <typename Table, auto... Columns>
 	using row_type = POXY_IMPLEMENTATION_DETAIL(
-		typename detail::row_type_<coerce_ref<Table>, std::index_sequence<Columns...>>::type);
+		typename detail::row_type_<coerce_ref<Table>, std::index_sequence<static_cast<size_t>(Columns)...>>::type);
 }
 
 /// @cond
 namespace std
 {
 	template <typename Table, size_t... Columns>
 	struct tuple_size<soagen::row<Table, Columns...>> //
```

### Comparing `soagen-0.1.2/src/soagen/hpp/single/soagen.hpp` & `soagen-0.2.0/src/soagen/hpp/single/soagen.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 //----------------------------------------------------------------------------------------------------------------------
 //
-// soagen.hpp v0.1.2
+// soagen.hpp v0.2.0
 // https://github.com/marzer/soagen
 // SPDX-License-Identifier: MIT
 //
 //----------------------------------------------------------------------------------------------------------------------
 //     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //----------------------------------------------------------------------------------------------------------------------
 //
@@ -28,17 +28,17 @@
 //----------------------------------------------------------------------------------------------------------------------
 #ifndef SOAGEN_HPP
 #define SOAGEN_HPP
 
 //********  generated/version.hpp  *************************************************************************************
 
 #define SOAGEN_VERSION_MAJOR 0
-#define SOAGEN_VERSION_MINOR 1
-#define SOAGEN_VERSION_PATCH 2
-#define SOAGEN_VERSION_STRING "0.1.2"
+#define SOAGEN_VERSION_MINOR 2
+#define SOAGEN_VERSION_PATCH 0
+#define SOAGEN_VERSION_STRING "0.2.0"
 
 //********  generated/preprocessor.hpp  ********************************************************************************
 
 #ifndef SOAGEN_CPP
 	#ifdef _MSVC_LANG
 		#if _MSVC_LANG > __cplusplus
 			#define SOAGEN_CPP _MSVC_LANG
@@ -511,15 +511,16 @@
 	#else
 		#define SOAGEN_HIDDEN_CONSTRAINT(condition, ...)
 	#endif
 #endif
 
 #ifndef SOAGEN_CONSTRAINED_COLUMN
 	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)                                                                          \
-		SOAGEN_CONSTRAINED_TEMPLATE(sfinae_col_idx == (I) && (__VA_ARGS__), size_t sfinae_col_idx = (I))
+		SOAGEN_CONSTRAINED_TEMPLATE(sfinae_col_idx == static_cast<std::size_t>(I) && (__VA_ARGS__),                    \
+									std::size_t sfinae_col_idx = static_cast<std::size_t>(I))
 #endif
 #ifndef SOAGEN_CONSTRAINED_COLUMN
 	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)
 #endif
 
 #ifndef SOAGEN_PUSH_WARNINGS
 	#if SOAGEN_CLANG
@@ -958,15 +959,16 @@
 		SOAGEN_PURE_INLINE_GETTER                                                                                      \
 		SOAGEN_ATTR(returns_nonnull)
 #endif
 
 #ifndef SOAGEN_ALIGNED_COLUMN
 	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
 		SOAGEN_COLUMN(I)                                                                                               \
-		SOAGEN_ATTR(assume_aligned(soagen::detail::actual_column_alignment<table_traits, allocator_type, I>))
+		SOAGEN_ATTR(assume_aligned(                                                                                    \
+			soagen::detail::actual_column_alignment<table_traits, allocator_type, static_cast<std::size_t>(I)>))
 #endif
 
 #ifndef SOAGEN_ALWAYS_OPTIMIZE
 	#define SOAGEN_ALWAYS_OPTIMIZE 1
 #endif
 
 #ifndef SOAGEN_COMMA
@@ -1220,35 +1222,37 @@
 			}                                                                                                          \
 		}
 #endif
 
 #ifndef SOAGEN_MAKE_COLUMN
 	#define SOAGEN_MAKE_COLUMN(Table, Column, Name)                                                                    \
 		template <>                                                                                                    \
-		struct column_name_<Table, Column> : name_constant_##Name                                                      \
+		struct column_name<Table, Column> : name_constant_##Name                                                       \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct col_ref_<Table&, Column>                                                                                \
-			: named_member_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, Column>>>                      \
+		struct column_ref<Table&, Column>                                                                              \
+			: named_member_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>> \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct col_ref_<Table&&, Column>                                                                               \
-			: named_member_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, Column>>>                      \
+		struct column_ref<Table&&, Column>                                                                             \
+			: named_member_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, static_cast<size_t>(Column)>>> \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct col_ref_<const Table&, Column>                                                                          \
-			: named_member_##Name<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>    \
+		struct column_ref<const Table&, Column>                                                                        \
+			: named_member_##Name<std::add_lvalue_reference_t<                                                         \
+				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
-		struct col_ref_<const Table&&, Column>                                                                         \
-			: named_member_##Name<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>    \
+		struct column_ref<const Table&&, Column>                                                                       \
+			: named_member_##Name<std::add_rvalue_reference_t<                                                         \
+				  std::add_const_t<soagen::value_type<Table, static_cast<size_t>(Column)>>>>                           \
 		{}
 #endif
 
 namespace soagen
 {
 	template <typename T>
 	using remove_cvref = std::remove_cv_t<std::remove_reference_t<T>>;
@@ -1258,14 +1262,18 @@
 
 	template <typename T>
 	using coerce_ref = std::conditional_t<std::is_reference_v<T>, T, std::add_lvalue_reference_t<T>>;
 
 	template <typename T>
 	using identity_type = T;
 
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES identity_base
+	{};
+
 	template <typename T>
 	inline constexpr bool is_cv = !std::is_same_v<std::remove_cv_t<T>, T>;
 
 	template <typename T>
 	inline constexpr bool is_cvref = !std::is_same_v<remove_cvref<T>, T>;
 
 	template <typename T>
@@ -1477,16 +1485,17 @@
 		{
 			using type = typename T::allocator_type;
 		};
 	}
 	template <typename T>
 	using allocator_type = POXY_IMPLEMENTATION_DETAIL(typename detail::allocator_type_<std::remove_cv_t<T>>::type);
 
-	template <typename T, size_t Column>
-	using value_type = POXY_IMPLEMENTATION_DETAIL(typename table_traits_type<T>::template column<Column>::value_type);
+	template <typename T, auto Column>
+	using value_type = POXY_IMPLEMENTATION_DETAIL(
+		typename table_traits_type<T>::template column<static_cast<size_t>(Column)>::value_type);
 
 	namespace detail
 	{
 		template <typename ValueType>
 		struct storage_type_
 		{
 			using type = ValueType;
@@ -1652,17 +1661,17 @@
 			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg));
 		}
 	}
 
 	namespace detail
 	{
 		template <typename Table, size_t ColumnIndex>
-		struct column_name_;
+		struct column_name;
 		template <typename Table, size_t ColumnIndex>
-		struct col_ref_;
+		struct column_ref;
 
 		template <typename A, typename B>
 		inline constexpr bool same_table_type =
 			std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>;
 	}
 }
 
@@ -1714,41 +1723,49 @@
 		#pragma GCC push_options
 		#pragma GCC optimize("O2")
 	#endif
 #endif
 
 namespace soagen
 {
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES row_base
+	{};
+
 	template <typename Table, size_t... Columns>
 	struct SOAGEN_EMPTY_BASES row //
-	SOAGEN_HIDDEN_BASE(public detail::col_ref_<Table, Columns>...)
+	SOAGEN_HIDDEN_BASE(public detail::column_ref<Table, Columns>..., public row_base<row<Table, Columns...>>)
 	{
 		static_assert(std::is_reference_v<Table>,
 					  "Table must be a reference so row members can derive their reference category");
+		static_assert(std::is_empty_v<row_base<row<Table, Columns...>>>,
+					  "row_base specializations may not have data members");
+		static_assert(std::is_trivial_v<row_base<row<Table, Columns...>>>, "row_base specializations must be trivial");
 
 		// columns:
 
-		template <size_t Column>
+		template <auto Column>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) column() const noexcept
 		{
-			static_assert(Column < table_traits_type<remove_cvref<Table>>::column_count, "column index out of range");
+			static_assert(static_cast<size_t>(Column) < table_traits_type<remove_cvref<Table>>::column_count,
+						  "column index out of range");
 
-			return detail::col_ref_<Table, Column>::get_named_member();
+			return detail::column_ref<Table, static_cast<size_t>(Column)>::get_named_member();
 		}
 
 		// tuple protocol:
 
-		template <size_t Member>
+		template <auto Member>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) get() const noexcept
 		{
 			static_assert(Member < sizeof...(Columns), "member index out of range");
 
-			return type_at_index<Member, detail::col_ref_<Table, Columns>...>::get_named_member();
+			return type_at_index<Member, detail::column_ref<Table, Columns>...>::get_named_member();
 		}
 
 		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
 									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator==(const row& lhs, const row<T, Columns...>& rhs) //
@@ -1859,17 +1876,17 @@
 			using type = row<Table, Columns...>;
 		};
 		template <typename Table>
 		struct row_type_<Table, std::index_sequence<>>
 			: row_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
 		{};
 	}
-	template <typename Table, size_t... Columns>
+	template <typename Table, auto... Columns>
 	using row_type = POXY_IMPLEMENTATION_DETAIL(
-		typename detail::row_type_<coerce_ref<Table>, std::index_sequence<Columns...>>::type);
+		typename detail::row_type_<coerce_ref<Table>, std::index_sequence<static_cast<size_t>(Columns)...>>::type);
 }
 
 namespace std
 {
 	template <typename Table, size_t... Columns>
 	struct tuple_size<soagen::row<Table, Columns...>> //
 		: std::integral_constant<size_t, sizeof...(Columns)>
@@ -3581,19 +3598,22 @@
 	{
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		// columns
 
-		template <size_t Index>
-		using column = type_at_index<Index, Columns...>;
+		template <auto Index>
+		using column = type_at_index<static_cast<size_t>(Index), Columns...>;
 
 		template <typename IndexConstant>
-		using column_from_ic = type_at_index<IndexConstant::value, Columns...>;
+		using column_from_ic = type_at_index<static_cast<size_t>(IndexConstant::value), Columns...>;
+
+		template <auto Index>
+		using storage_type = typename column<static_cast<size_t>(Index)>::storage_type;
 
 		using column_pointers		= std::byte* [column_count];
 		using const_column_pointers = std::byte* const[column_count];
 
 		static constexpr size_t column_sizes[column_count] = { sizeof(typename Columns::storage_type)... };
 
 		// default constructibility
@@ -3810,15 +3830,15 @@
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
 					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
 
-					if constexpr (!std::is_trivially_destructible_v<typename column<column_index>::storage_type>)
+					if constexpr (!std::is_trivially_destructible_v<storage_type<column_index>>)
 					{
 						SOAGEN_ASSUME(columns[column_index]);
 						SOAGEN_ASSUME(leftmost_column <= rightmost_column);
 						SOAGEN_ASSUME(leftmost_column < column_count);
 						SOAGEN_ASSUME(rightmost_column < column_count);
 
 						if (column_index >= leftmost_column && column_index <= rightmost_column)
@@ -3844,15 +3864,15 @@
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
 					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
 
-					if constexpr (!std::is_trivially_destructible_v<typename column<column_index>::storage_type>)
+					if constexpr (!std::is_trivially_destructible_v<storage_type<column_index>>)
 					{
 						SOAGEN_ASSUME(columns[column_index]);
 
 						column<column_index>::destruct(columns[column_index], index);
 					}
 				};
 
@@ -3914,16 +3934,15 @@
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor = [&](auto ic) //
-					noexcept(
-						std::is_nothrow_default_constructible_v<typename column<decltype(ic)::value>::storage_type>)
+					noexcept(std::is_nothrow_default_constructible_v<storage_type<decltype(ic)::value>>)
 				{
 					column_from_ic<decltype(ic)>::default_construct(columns[decltype(ic)::value], index);
 
 					constructed_columns++;
 				};
 
 				try
@@ -4033,16 +4052,15 @@
 				{
 					// machinery to provide strong-exception guarantee
 
 					size_t constructed_columns = {};
 
 					const auto constructor =
 						[&](auto ic, auto&& arg) noexcept(
-							std::is_nothrow_constructible_v<typename column_from_ic<decltype(ic)>::storage_type,
-															decltype(arg)&&>)
+							std::is_nothrow_constructible_v<storage_type<decltype(ic)::value>, decltype(arg)&&>)
 					{
 						column_from_ic<decltype(ic)>::construct_at(columns[decltype(ic)::value],
 																   index,
 																   static_cast<decltype(arg)&&>(arg));
 
 						constructed_columns++;
 					};
@@ -4105,16 +4123,15 @@
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
-					[&](auto ic) noexcept(
-						std::is_nothrow_move_constructible_v<typename column_from_ic<decltype(ic)>::storage_type>)
+					[&](auto ic) noexcept(std::is_nothrow_move_constructible_v<storage_type<decltype(ic)::value>>)
 				{
 					column_from_ic<decltype(ic)>::move_construct(dest_columns[decltype(ic)::value],
 																 dest_index,
 																 source_columns[decltype(ic)::value],
 																 source_index);
 
 					constructed_columns++;
@@ -4238,16 +4255,15 @@
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
-					[&](auto ic) noexcept(
-						std::is_nothrow_copy_constructible_v<typename column_from_ic<decltype(ic)>::storage_type>)
+					[&](auto ic) noexcept(std::is_nothrow_copy_constructible_v<storage_type<decltype(ic)::value>>)
 				{
 					column_from_ic<decltype(ic)>::copy_construct(dest_columns[decltype(ic)::value],
 																 dest_index,
 																 source_columns[decltype(ic)::value],
 																 source_index);
 
 					constructed_columns++;
@@ -4480,15 +4496,15 @@
 				{
 					for (size_t i = 0; i < count; i++)
 						copy_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
 				}
 			}
 		}
 
-		//--- swap -----------------------------------------------------------------------------------------------------
+		//--- swap rows ------------------------------------------------------------------------------------------------
 
 	  private:
 		template <typename... Args, size_t... Cols>
 		SOAGEN_CPP20_CONSTEXPR
 		static void swap_rows(column_pointers& lhs_columns,
 							  size_t lhs_index,
 							  column_pointers& rhs_columns,
@@ -4510,14 +4526,43 @@
 							  column_pointers& rhs_columns,
 							  size_t rhs_index) //
 			noexcept(all_nothrow_swappable)
 		{
 			swap_rows(lhs_columns, lhs_index, rhs_columns, rhs_index, std::make_index_sequence<column_count>{});
 		}
 
+		//--- swap columns ---------------------------------------------------------------------------------------------
+
+		template <size_t A, size_t B>
+		static constexpr bool can_swap_columns =
+			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_swappable);
+
+		template <size_t A, size_t B>
+		static constexpr bool can_nothrow_swap_columns =
+			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_nothrow_swappable);
+
+		SOAGEN_HIDDEN_CONSTRAINT((can_swap_columns<A, B>), size_t A, size_t B)
+		SOAGEN_CPP20_CONSTEXPR
+		static void swap_columns([[maybe_unused]] column_pointers& columns,
+								 [[maybe_unused]] size_t start,
+								 [[maybe_unused]] size_t count) //
+			noexcept(can_nothrow_swap_columns<A, B>)
+		{
+			if constexpr (A != B)
+			{
+				static_assert(std::is_same_v<storage_type<A>, storage_type<B>>);
+				static_assert(column<A>::is_swappable);
+				static_assert(column<B>::is_swappable);
+
+				count += start;
+				for (; start < count; start++)
+					column<A>::swap(columns[A], start, columns[B], start);
+			}
+		}
+
 		//--- equality -------------------------------------------------------------------------------------------------
 
 	  private:
 		template <typename... Args, size_t... Cols>
 		SOAGEN_NODISCARD
 		constexpr static bool equal(const const_column_pointers& lhs_columns,
 									size_t lhs_start_index,
@@ -4622,19 +4667,19 @@
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		static constexpr size_t aligned_stride = lcm(size_t{ 1 }, Columns::aligned_stride...);
 
 		// columns
 		// (note that these hide the base class typedefs - this is intentional)
 
-		template <size_t Index>
-		using column = type_at_index<Index, Columns...>;
+		template <auto Index>
+		using column = type_at_index<static_cast<size_t>(Index), Columns...>;
 
 		template <typename IndexConstant>
-		using column_from_ic = type_at_index<IndexConstant::value, Columns...>;
+		using column_from_ic = type_at_index<static_cast<size_t>(IndexConstant::value), Columns...>;
 
 		static constexpr size_t column_alignments[column_count] = { Columns::alignment... };
 
 		static constexpr size_t largest_alignment = max(size_t{ 1 }, Columns::alignment...);
 
 		static constexpr bool rvalue_type_list_is_distinct = POXY_IMPLEMENTATION_DETAIL(
 			!(std::is_same_v<typename Columns::param_type, typename Columns::rvalue_type> && ...));
@@ -4765,39 +4810,44 @@
 #if SOAGEN_CLANG >= 16
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
 namespace soagen::detail
 {
 	SOAGEN_CONSTRAINED_TEMPLATE(is_unsigned<T>, typename T)
-	[[nodiscard]]
+	SOAGEN_NODISCARD
 	constexpr bool add_without_overflowing(T lhs, T rhs, T& result) noexcept
 	{
 		if (lhs > static_cast<T>(-1) - rhs)
 			return false;
 
 		result = lhs + rhs;
 		return true;
 	};
 
+	inline static constexpr size_t min_actual_column_alignment =
+		max(size_t{ __STDCPP_DEFAULT_NEW_ALIGNMENT__ }, alignof(std::max_align_t), size_t{ 16 });
+
 	// trait for determining the _actual_ alignment of a table column, taking the allocator and
 	// table-allocation semantics into account (since the full allocation for a table always has
 	// alignment == table_traits::largest_alignment).
 	//
 	// note that this has absolutely nothing to do with the aligned_stride; that is still calculated
 	// according to the user's specified alignment requirements. this trait is _only_ used
 	// to help the compiler via assume_aligned.
-	template <typename Traits, typename Allocator, size_t ColumnIndex>
-	inline constexpr size_t actual_column_alignment = Traits::template column<ColumnIndex>::alignment;
+	template <typename Traits, typename Allocator, size_t Column>
+	inline constexpr size_t actual_column_alignment =
+		max(Traits::template column<Column>::alignment, min_actual_column_alignment);
 
 	template <typename Traits, typename Allocator>
 	inline constexpr size_t actual_column_alignment<Traits, Allocator, 0> =
 		max(Traits::template column<0>::alignment,
 			allocator_traits<Allocator>::min_alignment,
-			Traits::largest_alignment);
+			Traits::largest_alignment,
+			min_actual_column_alignment);
 
 	//------------------------------------------------------------------------------------------------------------------
 	// generic allocation class for tracking the column pointers and the actual size in bytes
 	//------------------------------------------------------------------------------------------------------------------
 
 	template <size_t ColumnCount>
 	struct table_allocation
@@ -4816,15 +4866,15 @@
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// base class for handling most allocation-related boilerplate
 	//------------------------------------------------------------------------------------------------------------------
 
 	template <size_t ColumnCount, typename Allocator>
-	class table_base
+	class table_storage
 	{
 		static_assert(ColumnCount, "tables must have at least one column");
 		static_assert(!is_cvref<Allocator>, "allocators may not be cvref-qualified");
 
 	  public:
 		using size_type		  = size_t;
 		using difference_type = ptrdiff_t;
@@ -4835,46 +4885,46 @@
 
 		allocation alloc_ = {};
 		size_t count_	  = {};
 		compressed_pair<size_t, Allocator> capacity_;
 
 	  public:
 		SOAGEN_NODISCARD_CTOR
-		explicit constexpr table_base(const Allocator& alloc) noexcept //
+		explicit constexpr table_storage(const Allocator& alloc) noexcept //
 			: capacity_{ size_t{}, alloc }
 		{
 			static_assert(std::is_nothrow_copy_constructible_v<Allocator>,
 						  "allocators must be nothrow copy-constructible");
 		}
 
 		SOAGEN_NODISCARD_CTOR
-		explicit constexpr table_base(Allocator&& alloc) noexcept //
+		explicit constexpr table_storage(Allocator&& alloc) noexcept //
 			: capacity_{ size_t{}, static_cast<Allocator&&>(alloc) }
 		{
 			static_assert(std::is_nothrow_move_constructible_v<Allocator>,
 						  "allocators must be nothrow move-constructible");
 		}
 
 		SOAGEN_NODISCARD_CTOR
-		constexpr table_base(table_base&& other) noexcept //
+		constexpr table_storage(table_storage&& other) noexcept //
 			: alloc_{ std::exchange(other.alloc_, allocation{}) },
 			  count_{ std::exchange(other.count_, size_t{}) },
 			  capacity_{ std::exchange(other.capacity_.first(), size_t{}), static_cast<Allocator&&>(other.allocator()) }
 		{
 			static_assert(std::is_nothrow_move_constructible_v<Allocator>,
 						  "allocators must be nothrow move-constructible");
 		}
 
 		// conditionally-implemented in specialized child classes:
-		table_base()							 = delete;
-		table_base& operator=(table_base&&)		 = delete;
-		table_base(const table_base&)			 = delete;
-		table_base& operator=(const table_base&) = delete;
+		table_storage()								   = delete;
+		table_storage& operator=(table_storage&&)	   = delete;
+		table_storage(const table_storage&)			   = delete;
+		table_storage& operator=(const table_storage&) = delete;
 
-		~table_base() noexcept
+		~table_storage() noexcept
 		{
 			static_assert(std::is_nothrow_destructible_v<Allocator>, "allocators must be nothrow destructible");
 
 			// element destructors are run in a more specialized child class
 
 			if (alloc_)
 				deallocate(alloc_);
@@ -4926,26 +4976,28 @@
 
 		static constexpr bool allocate_is_nothrow =
 			noexcept(allocator_traits<Allocator>::allocate(std::declval<Allocator&>(), size_t{}, std::align_val_t{}));
 
 		// guard against allocators with incorrect pointer typedefs where possible
 		using allocator_pointer_type = std::remove_reference_t<
 			decltype(allocator_traits<Allocator>::allocate(std::declval<Allocator&>(), size_t{}, std::align_val_t{}))>;
+		static_assert(std::is_pointer_v<allocator_pointer_type>);
 
 		SOAGEN_NODISCARD
 		constexpr allocation allocate(size_t n_bytes, size_t alignment) noexcept(allocate_is_nothrow)
 		{
 			SOAGEN_ASSUME(n_bytes);
 			SOAGEN_ASSUME((static_cast<size_t>(alignment) & (static_cast<size_t>(alignment) - 1u)) == 0u);
 
 			const auto ptr = soagen::assume_aligned<allocator_traits<Allocator>::min_alignment>(
 				allocator_traits<Allocator>::allocate(
 					allocator(),
 					n_bytes,
 					std::align_val_t{ max(alignment, allocator_traits<Allocator>::min_alignment) }));
+
 			SOAGEN_ASSUME(ptr != nullptr);
 			std::memset(ptr, 0, n_bytes);
 
 			if constexpr (std::is_same_v<allocator_pointer_type, std::byte*>)
 				return { { ptr }, n_bytes };
 			else
 				return { { reinterpret_cast<std::byte*>(ptr) }, n_bytes };
@@ -4966,15 +5018,15 @@
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: default-constructibility
 	//------------------------------------------------------------------------------------------------------------------
 
 #undef SOAGEN_BASE_NAME
-#define SOAGEN_BASE_NAME table_base
+#define SOAGEN_BASE_NAME table_storage
 #undef SOAGEN_BASE_TYPE
 #define SOAGEN_BASE_TYPE SOAGEN_BASE_NAME<ColumnCount, Allocator>
 
 	template <size_t ColumnCount,
 			  typename Allocator,
 			  bool = std::is_default_constructible_v<Allocator>>
 	class SOAGEN_EMPTY_BASES table_default_construct //
@@ -5179,39 +5231,36 @@
 
 		static constexpr void calc_column_ends(column_ends& ends, size_t capacity) noexcept
 		{
 			// pad ends so the next column starts at the right alignment for the storage type
 			size_t prev = {};
 			for (size_t i = 0; i < Traits::column_count - 1u; i++)
 			{
-				ends[i] = prev + Traits::column_sizes[i] * capacity;
-				ends[i] = (ends[i] + Traits::column_alignments[i + 1u] - 1u) //
-						& ~(Traits::column_alignments[i + 1u] - 1u);
+				const auto align = max(Traits::column_alignments[i + 1u], min_actual_column_alignment);
 
-				SOAGEN_ASSUME(ends[i] % Traits::column_alignments[i + 1u] == 0u);
-				prev = ends[i];
+				ends[i] = prev + Traits::column_sizes[i] * capacity;
+				ends[i] = (ends[i] + align - 1u) & ~(align - 1u);
+				prev	= ends[i];
 			}
 
 			// last end doesn't need to be aligned (it's just the total buffer size)
 			ends[Traits::column_count - 1u] = prev + Traits::column_sizes[Traits::column_count - 1u] * capacity;
 		}
 
+		SOAGEN_NODISCARD
 		constexpr allocation allocate(const column_ends& ends) noexcept(base::allocate_is_nothrow)
 		{
 			SOAGEN_ASSUME(ends[Traits::column_count - 1u]);
 
-			auto alloc = base::allocate(ends[Traits::column_count - 1u], Traits::largest_alignment);
+			auto alloc = base::allocate(ends[Traits::column_count - 1u], actual_column_alignment<Traits, Allocator, 0>);
 			SOAGEN_ASSUME(alloc.columns[0]);
 			SOAGEN_ASSUME(alloc.size_in_bytes == ends[Traits::column_count - 1u]);
 
 			for (size_t i = 1; i < Traits::column_count; i++)
-			{
 				alloc.columns[i] = alloc.columns[0] + ends[i - 1u];
-				SOAGEN_ASSUME(reinterpret_cast<uintptr_t>(alloc.columns[i]) % Traits::column_alignments[i] == 0u);
-			}
 
 			return alloc;
 		}
 
 		SOAGEN_CPP20_CONSTEXPR
 		void adjust_capacity(size_t new_capacity) noexcept(
 			base::allocate_is_nothrow
@@ -5405,17 +5454,19 @@
 				constexpr auto capacity_ok = [](size_t cap) noexcept
 				{
 					size_t buf_end = {};
 					for (size_t i = 0u; i < Traits::column_count; i++)
 					{
 						if (i)
 						{
-							if (const size_t rem = buf_end % Traits::column_alignments[i - 1u]; rem > 0u)
+							const auto align = max(Traits::column_alignments[i - 1u], min_actual_column_alignment);
+
+							if (const size_t rem = buf_end % align; rem > 0u)
 							{
-								if (!add_without_overflowing(buf_end, Traits::column_alignments[i - 1u] - rem, buf_end))
+								if (!add_without_overflowing(buf_end, align - rem, buf_end))
 									return false;
 							}
 						}
 						if (!add_without_overflowing(buf_end, Traits::column_sizes[i] * cap, buf_end))
 							return false;
 					}
 					return true;
@@ -5529,14 +5580,56 @@
 
 			// todo: there might be some inputs that allow us to move-assign instead of destruct+construct
 			Traits::destruct_row(base::alloc_.columns, position);
 			Traits::construct_row(base::alloc_.columns, position, static_cast<Args&&>(args)...);
 
 			base::count_++;
 		}
+
+	  private:
+		template <size_t A, size_t B>
+		static constexpr bool can_swap_columns =
+			Traits::template can_swap_columns<A, B>
+			|| (std::is_same_v<typename Traits::template storage_type<A>, typename Traits::template storage_type<B>>
+				&& actual_column_alignment<Traits, Allocator, A> == actual_column_alignment<Traits, Allocator, B>);
+
+		template <size_t A, size_t B>
+		static constexpr bool can_nothrow_swap_columns =
+			Traits::template can_nothrow_swap_columns<A, B>
+			|| (std::is_same_v<typename Traits::template storage_type<A>, typename Traits::template storage_type<B>>
+				&& actual_column_alignment<Traits, Allocator, A> == actual_column_alignment<Traits, Allocator, B>);
+
+	  public:
+		template <size_t A, size_t B>
+		SOAGEN_CPP20_CONSTEXPR
+		void swap_columns() //
+			noexcept(can_nothrow_swap_columns<A, B>)
+		{
+			static_assert(can_swap_columns<A, B>);
+
+			if constexpr (A != B)
+			{
+				using storage_a = typename Traits::template storage_type<A>;
+				using storage_b = typename Traits::template storage_type<B>;
+				static_assert(std::is_same_v<storage_a, storage_b>);
+
+				// if they have the same base alignment, we can just swap the two pointers
+				// rather than having to do an element-wise swap
+				if constexpr (actual_column_alignment<Traits, Allocator, A>
+							  == actual_column_alignment<Traits, Allocator, B>)
+				{
+					std::swap(base::alloc_.columns[A], base::alloc_.columns[B]);
+				}
+
+				else
+				{
+					Traits::template swap_columns<A, B>(base::alloc_.columns, {}, base::count_);
+				}
+			}
+		}
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: default-constructible column types
 	//------------------------------------------------------------------------------------------------------------------
 
 #undef SOAGEN_BASE_NAME
@@ -6122,39 +6215,57 @@
 #undef SOAGEN_BASE_NAME
 #define SOAGEN_BASE_NAME table_data_ptr
 #undef SOAGEN_BASE_TYPE
 #define SOAGEN_BASE_TYPE detail::SOAGEN_BASE_NAME<Traits, Allocator>
 
 namespace soagen
 {
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES table_base
+	{};
+
 	template <typename Traits,
-			  typename Allocator = soagen::allocator>
+			  typename Allocator				= soagen::allocator,
+			  template <typename> typename Base = soagen::identity_base>
 	class SOAGEN_EMPTY_BASES table //
-		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE)
+		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE,
+						   public table_base<table<Traits, Allocator, Base>>,
+						   public Base<table<Traits, Allocator, Base>>)
 	{
 		static_assert(is_table_traits<Traits>, "Traits must be an instance of soagen::table_traits");
 		static_assert(!is_cvref<Traits>, "table traits may not be cvref-qualified");
 		static_assert(!is_cvref<Allocator>, "allocators may not be cvref-qualified");
 
+		static_assert(!std::is_same_v<table_base<table<Traits, Allocator, Base>>, Base<table<Traits, Allocator, Base>>>,
+					  "table_base and Base may not be the same type");
+
+		static_assert(std::is_empty_v<table_base<table<Traits, Allocator, Base>>>,
+					  "table_base specializations may not have data members");
+		static_assert(std::is_trivial_v<table_base<table<Traits, Allocator, Base>>>,
+					  "table_base specializations must be trivial");
+
+		static_assert(std::is_empty_v<Base<table<Traits, Allocator, Base>>>, "CRTP bases may not have data members");
+		static_assert(std::is_trivial_v<Base<table<Traits, Allocator, Base>>>, "CRTP bases must be trivial");
+
 	  private:
 		using base = SOAGEN_BASE_TYPE;
 
 	  public:
 		using size_type		  = size_t;
 		using difference_type = ptrdiff_t;
 
 		using table_traits = Traits;
 
 		using allocator_type = Allocator;
 
-		template <size_type Column>
-		using column_traits = typename table_traits::template column<Column>;
+		template <auto Column>
+		using column_traits = typename table_traits::template column<static_cast<size_t>(Column)>;
 
-		template <size_type Column>
-		using column_type = typename column_traits<Column>::value_type;
+		template <auto Column>
+		using column_type = typename column_traits<static_cast<size_t>(Column)>::value_type;
 
 		static constexpr size_t aligned_stride = Traits::aligned_stride;
 
 		SOAGEN_NODISCARD_CTOR
 		table() = default;
 
 		SOAGEN_NODISCARD_CTOR
@@ -6167,32 +6278,36 @@
 
 		table& operator=(const table&) = default;
 
 		~table() = default;
 
 		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
-		template <size_t Column>
+		template <auto Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
 		column_type<Column>* column() noexcept
 		{
-			static_assert(Column < table_traits::column_count, "column index out of range");
+			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
 
-			return soagen::assume_aligned<detail::actual_column_alignment<table_traits, allocator_type, Column>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<Column>*>(base::alloc_.columns[Column])));
+			return soagen::assume_aligned<
+				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>>(
+				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
+					base::alloc_.columns[static_cast<size_t>(Column)])));
 		}
 
-		template <size_t Column>
+		template <auto Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
 		std::add_const_t<column_type<Column>>* column() const noexcept
 		{
-			static_assert(Column < table_traits::column_count, "column index out of range");
+			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
 
-			return soagen::assume_aligned<detail::actual_column_alignment<table_traits, allocator_type, Column>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<Column>*>(base::alloc_.columns[Column])));
+			return soagen::assume_aligned<
+				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>>(
+				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
+					base::alloc_.columns[static_cast<size_t>(Column)])));
 		}
 	};
 
 	template <typename>
 	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(false);
 	template <typename... Args>
 	inline constexpr bool is_table<table<Args...>> = true;
@@ -6206,18 +6321,18 @@
 	{
 		template <typename... Args>
 		struct table_type_<table<Args...>>
 		{
 			using type = table<Args...>;
 		};
 	}
-	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Traits, Allocator>>), typename Traits, typename Allocator)
+	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Args...>>), typename... Args)
 	SOAGEN_ALWAYS_INLINE
-	constexpr void swap(table<Traits, Allocator>& lhs, table<Traits, Allocator>& rhs) //
-		noexcept(soagen::has_nothrow_swap_member<table<Traits, Allocator>>)
+	constexpr void swap(table<Args...>& lhs, table<Args...>& rhs) //
+		noexcept(soagen::has_nothrow_swap_member<table<Args...>>)
 	{
 		lhs.swap(rhs);
 	}
 }
 
 #undef SOAGEN_BASE_NAME
 #undef SOAGEN_BASE_TYPE
@@ -6505,18 +6620,28 @@
 		template <typename Table>
 		struct iterator_storage
 		{
 			std::add_const_t<remove_cvref<Table>>* table;
 			typename remove_cvref<Table>::difference_type offset;
 		};
 	}
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES iterator_base
+	{};
+
 	template <typename Table, size_t... Columns>
-	class iterator
-		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>)
-	{
+	class SOAGEN_EMPTY_BASES iterator
+		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>,
+						   public iterator_base<iterator<Table, Columns...>>)
+	{
+		static_assert(std::is_empty_v<iterator_base<iterator<Table, Columns...>>>,
+					  "iterator_base specializations may not have data members");
+		static_assert(std::is_trivial_v<iterator_base<iterator<Table, Columns...>>>,
+					  "iterator_base specializations must be trivial");
+
 	  public:
 		using table_type = remove_cvref<Table>;
 		static_assert(is_soa<table_type>, "soagen iterators are for use with soagen-generated SoA table types.");
 
 		using table_ref = Table;
 		static_assert(std::is_reference_v<table_ref>,
 					  "Table must be a reference so row members can derive their reference category");
```

### Comparing `soagen-0.1.2/src/soagen/hpp/soagen.hpp` & `soagen-0.2.0/src/soagen/hpp/soagen.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/hpp/table.hpp` & `soagen-0.2.0/src/soagen/hpp/table.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -13,39 +13,44 @@
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
 /// @cond
 namespace soagen::detail
 {
 	SOAGEN_CONSTRAINED_TEMPLATE(is_unsigned<T>, typename T)
-	[[nodiscard]]
+	SOAGEN_NODISCARD
 	constexpr bool add_without_overflowing(T lhs, T rhs, T& result) noexcept
 	{
 		if (lhs > static_cast<T>(-1) - rhs)
 			return false;
 
 		result = lhs + rhs;
 		return true;
 	};
 
+	inline static constexpr size_t min_actual_column_alignment =
+		max(size_t{ __STDCPP_DEFAULT_NEW_ALIGNMENT__ }, alignof(std::max_align_t), size_t{ 16 });
+
 	// trait for determining the _actual_ alignment of a table column, taking the allocator and
 	// table-allocation semantics into account (since the full allocation for a table always has
 	// alignment == table_traits::largest_alignment).
 	//
 	// note that this has absolutely nothing to do with the aligned_stride; that is still calculated
 	// according to the user's specified alignment requirements. this trait is _only_ used
 	// to help the compiler via assume_aligned.
-	template <typename Traits, typename Allocator, size_t ColumnIndex>
-	inline constexpr size_t actual_column_alignment = Traits::template column<ColumnIndex>::alignment;
+	template <typename Traits, typename Allocator, size_t Column>
+	inline constexpr size_t actual_column_alignment =
+		max(Traits::template column<Column>::alignment, min_actual_column_alignment);
 
 	template <typename Traits, typename Allocator>
 	inline constexpr size_t actual_column_alignment<Traits, Allocator, 0> =
 		max(Traits::template column<0>::alignment,
 			allocator_traits<Allocator>::min_alignment,
-			Traits::largest_alignment);
+			Traits::largest_alignment,
+			min_actual_column_alignment);
 
 	//------------------------------------------------------------------------------------------------------------------
 	// generic allocation class for tracking the column pointers and the actual size in bytes
 	//------------------------------------------------------------------------------------------------------------------
 
 	template <size_t ColumnCount>
 	struct table_allocation
@@ -64,15 +69,15 @@
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// base class for handling most allocation-related boilerplate
 	//------------------------------------------------------------------------------------------------------------------
 
 	template <size_t ColumnCount, typename Allocator>
-	class table_base
+	class table_storage
 	{
 		static_assert(ColumnCount, "tables must have at least one column");
 		static_assert(!is_cvref<Allocator>, "allocators may not be cvref-qualified");
 
 	  public:
 		using size_type		  = size_t;
 		using difference_type = ptrdiff_t;
@@ -83,46 +88,46 @@
 
 		allocation alloc_ = {};
 		size_t count_	  = {};
 		compressed_pair<size_t, Allocator> capacity_;
 
 	  public:
 		SOAGEN_NODISCARD_CTOR
-		explicit constexpr table_base(const Allocator& alloc) noexcept //
+		explicit constexpr table_storage(const Allocator& alloc) noexcept //
 			: capacity_{ size_t{}, alloc }
 		{
 			static_assert(std::is_nothrow_copy_constructible_v<Allocator>,
 						  "allocators must be nothrow copy-constructible");
 		}
 
 		SOAGEN_NODISCARD_CTOR
-		explicit constexpr table_base(Allocator&& alloc) noexcept //
+		explicit constexpr table_storage(Allocator&& alloc) noexcept //
 			: capacity_{ size_t{}, static_cast<Allocator&&>(alloc) }
 		{
 			static_assert(std::is_nothrow_move_constructible_v<Allocator>,
 						  "allocators must be nothrow move-constructible");
 		}
 
 		SOAGEN_NODISCARD_CTOR
-		constexpr table_base(table_base&& other) noexcept //
+		constexpr table_storage(table_storage&& other) noexcept //
 			: alloc_{ std::exchange(other.alloc_, allocation{}) },
 			  count_{ std::exchange(other.count_, size_t{}) },
 			  capacity_{ std::exchange(other.capacity_.first(), size_t{}), static_cast<Allocator&&>(other.allocator()) }
 		{
 			static_assert(std::is_nothrow_move_constructible_v<Allocator>,
 						  "allocators must be nothrow move-constructible");
 		}
 
 		// conditionally-implemented in specialized child classes:
-		table_base()							 = delete;
-		table_base& operator=(table_base&&)		 = delete;
-		table_base(const table_base&)			 = delete;
-		table_base& operator=(const table_base&) = delete;
+		table_storage()								   = delete;
+		table_storage& operator=(table_storage&&)	   = delete;
+		table_storage(const table_storage&)			   = delete;
+		table_storage& operator=(const table_storage&) = delete;
 
-		~table_base() noexcept
+		~table_storage() noexcept
 		{
 			static_assert(std::is_nothrow_destructible_v<Allocator>, "allocators must be nothrow destructible");
 
 			// element destructors are run in a more specialized child class
 
 			if (alloc_)
 				deallocate(alloc_);
@@ -174,26 +179,28 @@
 
 		static constexpr bool allocate_is_nothrow =
 			noexcept(allocator_traits<Allocator>::allocate(std::declval<Allocator&>(), size_t{}, std::align_val_t{}));
 
 		// guard against allocators with incorrect pointer typedefs where possible
 		using allocator_pointer_type = std::remove_reference_t<
 			decltype(allocator_traits<Allocator>::allocate(std::declval<Allocator&>(), size_t{}, std::align_val_t{}))>;
+		static_assert(std::is_pointer_v<allocator_pointer_type>);
 
 		SOAGEN_NODISCARD
 		constexpr allocation allocate(size_t n_bytes, size_t alignment) noexcept(allocate_is_nothrow)
 		{
 			SOAGEN_ASSUME(n_bytes);
 			SOAGEN_ASSUME((static_cast<size_t>(alignment) & (static_cast<size_t>(alignment) - 1u)) == 0u);
 
 			const auto ptr = soagen::assume_aligned<allocator_traits<Allocator>::min_alignment>(
 				allocator_traits<Allocator>::allocate(
 					allocator(),
 					n_bytes,
 					std::align_val_t{ max(alignment, allocator_traits<Allocator>::min_alignment) }));
+
 			SOAGEN_ASSUME(ptr != nullptr);
 			std::memset(ptr, 0, n_bytes);
 
 			if constexpr (std::is_same_v<allocator_pointer_type, std::byte*>)
 				return { { ptr }, n_bytes };
 			else
 				return { { reinterpret_cast<std::byte*>(ptr) }, n_bytes };
@@ -214,15 +221,15 @@
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: default-constructibility
 	//------------------------------------------------------------------------------------------------------------------
 
 #undef SOAGEN_BASE_NAME
-#define SOAGEN_BASE_NAME table_base
+#define SOAGEN_BASE_NAME table_storage
 #undef SOAGEN_BASE_TYPE
 #define SOAGEN_BASE_TYPE SOAGEN_BASE_NAME<ColumnCount, Allocator>
 
 	template <size_t ColumnCount,
 			  typename Allocator,
 			  bool = std::is_default_constructible_v<Allocator>>
 	class SOAGEN_EMPTY_BASES table_default_construct //
@@ -427,39 +434,36 @@
 
 		static constexpr void calc_column_ends(column_ends& ends, size_t capacity) noexcept
 		{
 			// pad ends so the next column starts at the right alignment for the storage type
 			size_t prev = {};
 			for (size_t i = 0; i < Traits::column_count - 1u; i++)
 			{
-				ends[i] = prev + Traits::column_sizes[i] * capacity;
-				ends[i] = (ends[i] + Traits::column_alignments[i + 1u] - 1u) //
-						& ~(Traits::column_alignments[i + 1u] - 1u);
+				const auto align = max(Traits::column_alignments[i + 1u], min_actual_column_alignment);
 
-				SOAGEN_ASSUME(ends[i] % Traits::column_alignments[i + 1u] == 0u);
-				prev = ends[i];
+				ends[i] = prev + Traits::column_sizes[i] * capacity;
+				ends[i] = (ends[i] + align - 1u) & ~(align - 1u);
+				prev	= ends[i];
 			}
 
 			// last end doesn't need to be aligned (it's just the total buffer size)
 			ends[Traits::column_count - 1u] = prev + Traits::column_sizes[Traits::column_count - 1u] * capacity;
 		}
 
+		SOAGEN_NODISCARD
 		constexpr allocation allocate(const column_ends& ends) noexcept(base::allocate_is_nothrow)
 		{
 			SOAGEN_ASSUME(ends[Traits::column_count - 1u]);
 
-			auto alloc = base::allocate(ends[Traits::column_count - 1u], Traits::largest_alignment);
+			auto alloc = base::allocate(ends[Traits::column_count - 1u], actual_column_alignment<Traits, Allocator, 0>);
 			SOAGEN_ASSUME(alloc.columns[0]);
 			SOAGEN_ASSUME(alloc.size_in_bytes == ends[Traits::column_count - 1u]);
 
 			for (size_t i = 1; i < Traits::column_count; i++)
-			{
 				alloc.columns[i] = alloc.columns[0] + ends[i - 1u];
-				SOAGEN_ASSUME(reinterpret_cast<uintptr_t>(alloc.columns[i]) % Traits::column_alignments[i] == 0u);
-			}
 
 			return alloc;
 		}
 
 		SOAGEN_CPP20_CONSTEXPR
 		void adjust_capacity(size_t new_capacity) noexcept(
 			base::allocate_is_nothrow
@@ -653,17 +657,19 @@
 				constexpr auto capacity_ok = [](size_t cap) noexcept
 				{
 					size_t buf_end = {};
 					for (size_t i = 0u; i < Traits::column_count; i++)
 					{
 						if (i)
 						{
-							if (const size_t rem = buf_end % Traits::column_alignments[i - 1u]; rem > 0u)
+							const auto align = max(Traits::column_alignments[i - 1u], min_actual_column_alignment);
+
+							if (const size_t rem = buf_end % align; rem > 0u)
 							{
-								if (!add_without_overflowing(buf_end, Traits::column_alignments[i - 1u] - rem, buf_end))
+								if (!add_without_overflowing(buf_end, align - rem, buf_end))
 									return false;
 							}
 						}
 						if (!add_without_overflowing(buf_end, Traits::column_sizes[i] * cap, buf_end))
 							return false;
 					}
 					return true;
@@ -777,14 +783,56 @@
 
 			// todo: there might be some inputs that allow us to move-assign instead of destruct+construct
 			Traits::destruct_row(base::alloc_.columns, position);
 			Traits::construct_row(base::alloc_.columns, position, static_cast<Args&&>(args)...);
 
 			base::count_++;
 		}
+
+	  private:
+		template <size_t A, size_t B>
+		static constexpr bool can_swap_columns =
+			Traits::template can_swap_columns<A, B>
+			|| (std::is_same_v<typename Traits::template storage_type<A>, typename Traits::template storage_type<B>>
+				&& actual_column_alignment<Traits, Allocator, A> == actual_column_alignment<Traits, Allocator, B>);
+
+		template <size_t A, size_t B>
+		static constexpr bool can_nothrow_swap_columns =
+			Traits::template can_nothrow_swap_columns<A, B>
+			|| (std::is_same_v<typename Traits::template storage_type<A>, typename Traits::template storage_type<B>>
+				&& actual_column_alignment<Traits, Allocator, A> == actual_column_alignment<Traits, Allocator, B>);
+
+	  public:
+		template <size_t A, size_t B>
+		SOAGEN_CPP20_CONSTEXPR
+		void swap_columns() //
+			noexcept(can_nothrow_swap_columns<A, B>)
+		{
+			static_assert(can_swap_columns<A, B>);
+
+			if constexpr (A != B)
+			{
+				using storage_a = typename Traits::template storage_type<A>;
+				using storage_b = typename Traits::template storage_type<B>;
+				static_assert(std::is_same_v<storage_a, storage_b>);
+
+				// if they have the same base alignment, we can just swap the two pointers
+				// rather than having to do an element-wise swap
+				if constexpr (actual_column_alignment<Traits, Allocator, A>
+							  == actual_column_alignment<Traits, Allocator, B>)
+				{
+					std::swap(base::alloc_.columns[A], base::alloc_.columns[B]);
+				}
+
+				else
+				{
+					Traits::template swap_columns<A, B>(base::alloc_.columns, {}, base::count_);
+				}
+			}
+		}
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: default-constructible column types
 	//------------------------------------------------------------------------------------------------------------------
 
 #undef SOAGEN_BASE_NAME
@@ -1372,31 +1420,52 @@
 #undef SOAGEN_BASE_TYPE
 #define SOAGEN_BASE_TYPE detail::SOAGEN_BASE_NAME<Traits, Allocator>
 
 /// @endcond
 
 namespace soagen
 {
+	/// @brief		Base class for soagen::table.
+	/// @details	Specialize this to add functionality to all tables of a particular type via CRTP.
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES table_base
+	{};
+
 	/// @brief		A table.
 	/// @details	Effectively a multi-column std::vector.
 	/// @tparam		Traits		The #soagen::table_traits for the table.
 	/// @tparam		Allocator	The allocator used by the table.
+	/// @tparam		Base		Base class hook allowing you to add more functionality to the table via CRTP.
 	///
 	///	@attention	This class is the backing data structure for the soagen-generated Structure-of-arrays classes.
 	///				You don't need to know anything about it unless you are implementing your own SoA machinery
 	///				without using the soagen generator.
 	template <typename Traits,
-			  typename Allocator = soagen::allocator>
+			  typename Allocator				= soagen::allocator,
+			  template <typename> typename Base = soagen::identity_base>
 	class SOAGEN_EMPTY_BASES table //
-		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE)
+		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE,
+						   public table_base<table<Traits, Allocator, Base>>,
+						   public Base<table<Traits, Allocator, Base>>)
 	{
 		static_assert(is_table_traits<Traits>, "Traits must be an instance of soagen::table_traits");
 		static_assert(!is_cvref<Traits>, "table traits may not be cvref-qualified");
 		static_assert(!is_cvref<Allocator>, "allocators may not be cvref-qualified");
 
+		static_assert(!std::is_same_v<table_base<table<Traits, Allocator, Base>>, Base<table<Traits, Allocator, Base>>>,
+					  "table_base and Base may not be the same type");
+
+		static_assert(std::is_empty_v<table_base<table<Traits, Allocator, Base>>>,
+					  "table_base specializations may not have data members");
+		static_assert(std::is_trivial_v<table_base<table<Traits, Allocator, Base>>>,
+					  "table_base specializations must be trivial");
+
+		static_assert(std::is_empty_v<Base<table<Traits, Allocator, Base>>>, "CRTP bases may not have data members");
+		static_assert(std::is_trivial_v<Base<table<Traits, Allocator, Base>>>, "CRTP bases must be trivial");
+
 	  private:
 		/// @cond
 		using base = SOAGEN_BASE_TYPE;
 		/// @endcond
 
 	  public:
 		using size_type		  = size_t;
@@ -1405,20 +1474,20 @@
 		/// @brief	The #soagen::table_traits for the the table.
 		using table_traits = Traits;
 
 		/// @brief	The allocator used by the table.
 		using allocator_type = Allocator;
 
 		/// @brief	Returns the #soagen::column_traits for the column at the specified index.
-		template <size_type Column>
-		using column_traits = typename table_traits::template column<Column>;
+		template <auto Column>
+		using column_traits = typename table_traits::template column<static_cast<size_t>(Column)>;
 
 		/// @brief	Returns the `value_type` for the column at the specified index.
-		template <size_type Column>
-		using column_type = typename column_traits<Column>::value_type;
+		template <auto Column>
+		using column_type = typename column_traits<static_cast<size_t>(Column)>::value_type;
 
 		/// @copydoc	table_traits::aligned_stride
 		static constexpr size_t aligned_stride = Traits::aligned_stride;
 
 		/// @brief Default constructor.
 		SOAGEN_NODISCARD_CTOR
 		table() = default;
@@ -1573,33 +1642,37 @@
 		/// @brief Returns a const pointer to the raw byte backing array.
 		///
 		/// @availability This method is only available when all the column types are trivially-copyable.
 		constexpr const std::byte* data() const noexcept;
 #endif
 
 		/// @brief Returns a pointer to the elements of a specific column.
-		template <size_t Column>
+		template <auto Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
 		column_type<Column>* column() noexcept
 		{
-			static_assert(Column < table_traits::column_count, "column index out of range");
+			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
 
-			return soagen::assume_aligned<detail::actual_column_alignment<table_traits, allocator_type, Column>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<Column>*>(base::alloc_.columns[Column])));
+			return soagen::assume_aligned<
+				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>>(
+				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
+					base::alloc_.columns[static_cast<size_t>(Column)])));
 		}
 
 		/// @brief Returns a pointer to the elements of a specific column.
-		template <size_t Column>
+		template <auto Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
 		std::add_const_t<column_type<Column>>* column() const noexcept
 		{
-			static_assert(Column < table_traits::column_count, "column index out of range");
+			static_assert(static_cast<size_t>(Column) < table_traits::column_count, "column index out of range");
 
-			return soagen::assume_aligned<detail::actual_column_alignment<table_traits, allocator_type, Column>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<Column>*>(base::alloc_.columns[Column])));
+			return soagen::assume_aligned<
+				detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_t>(Column)>>(
+				SOAGEN_LAUNDER(reinterpret_cast<column_type<static_cast<size_t>(Column)>*>(
+					base::alloc_.columns[static_cast<size_t>(Column)])));
 		}
 
 		/// @}
 	};
 
 	/// @brief True if `T` is an instance of #soagen::table.
 	template <typename>
@@ -1621,19 +1694,19 @@
 			using type = table<Args...>;
 		};
 	}
 	/// @endcond
 
 	/// @brief Swaps the contents of two tables.
 	///
-	/// @availability This method is only available when Allocator is swappable or non-propagating.
-	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Traits, Allocator>>), typename Traits, typename Allocator)
+	/// @availability This method is only available when the table's `allocator_type` is swappable or non-propagating.
+	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Args...>>), typename... Args)
 	SOAGEN_ALWAYS_INLINE
-	constexpr void swap(table<Traits, Allocator>& lhs, table<Traits, Allocator>& rhs) //
-		noexcept(soagen::has_nothrow_swap_member<table<Traits, Allocator>>)
+	constexpr void swap(table<Args...>& lhs, table<Args...>& rhs) //
+		noexcept(soagen::has_nothrow_swap_member<table<Args...>>)
 	{
 		lhs.swap(rhs);
 	}
 }
 
 #undef SOAGEN_BASE_NAME
 #undef SOAGEN_BASE_TYPE
```

### Comparing `soagen-0.1.2/src/soagen/hpp/table_traits.hpp` & `soagen-0.2.0/src/soagen/hpp/table_traits.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,22 @@
 	{
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		// columns
 
-		template <size_t Index>
-		using column = type_at_index<Index, Columns...>;
+		template <auto Index>
+		using column = type_at_index<static_cast<size_t>(Index), Columns...>;
 
 		template <typename IndexConstant>
-		using column_from_ic = type_at_index<IndexConstant::value, Columns...>;
+		using column_from_ic = type_at_index<static_cast<size_t>(IndexConstant::value), Columns...>;
+
+		template <auto Index>
+		using storage_type = typename column<static_cast<size_t>(Index)>::storage_type;
 
 		using column_pointers		= std::byte* [column_count];
 		using const_column_pointers = std::byte* const[column_count];
 
 		static constexpr size_t column_sizes[column_count] = { sizeof(typename Columns::storage_type)... };
 
 		// default constructibility
@@ -250,15 +253,15 @@
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
 					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
 
-					if constexpr (!std::is_trivially_destructible_v<typename column<column_index>::storage_type>)
+					if constexpr (!std::is_trivially_destructible_v<storage_type<column_index>>)
 					{
 						SOAGEN_ASSUME(columns[column_index]);
 						SOAGEN_ASSUME(leftmost_column <= rightmost_column);
 						SOAGEN_ASSUME(leftmost_column < column_count);
 						SOAGEN_ASSUME(rightmost_column < column_count);
 
 						if (column_index >= leftmost_column && column_index <= rightmost_column)
@@ -284,15 +287,15 @@
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
 					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
 
-					if constexpr (!std::is_trivially_destructible_v<typename column<column_index>::storage_type>)
+					if constexpr (!std::is_trivially_destructible_v<storage_type<column_index>>)
 					{
 						SOAGEN_ASSUME(columns[column_index]);
 
 						column<column_index>::destruct(columns[column_index], index);
 					}
 				};
 
@@ -354,16 +357,15 @@
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor = [&](auto ic) //
-					noexcept(
-						std::is_nothrow_default_constructible_v<typename column<decltype(ic)::value>::storage_type>)
+					noexcept(std::is_nothrow_default_constructible_v<storage_type<decltype(ic)::value>>)
 				{
 					column_from_ic<decltype(ic)>::default_construct(columns[decltype(ic)::value], index);
 
 					constructed_columns++;
 				};
 
 				try
@@ -473,16 +475,15 @@
 				{
 					// machinery to provide strong-exception guarantee
 
 					size_t constructed_columns = {};
 
 					const auto constructor =
 						[&](auto ic, auto&& arg) noexcept(
-							std::is_nothrow_constructible_v<typename column_from_ic<decltype(ic)>::storage_type,
-															decltype(arg)&&>)
+							std::is_nothrow_constructible_v<storage_type<decltype(ic)::value>, decltype(arg)&&>)
 					{
 						column_from_ic<decltype(ic)>::construct_at(columns[decltype(ic)::value],
 																   index,
 																   static_cast<decltype(arg)&&>(arg));
 
 						constructed_columns++;
 					};
@@ -545,16 +546,15 @@
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
-					[&](auto ic) noexcept(
-						std::is_nothrow_move_constructible_v<typename column_from_ic<decltype(ic)>::storage_type>)
+					[&](auto ic) noexcept(std::is_nothrow_move_constructible_v<storage_type<decltype(ic)::value>>)
 				{
 					column_from_ic<decltype(ic)>::move_construct(dest_columns[decltype(ic)::value],
 																 dest_index,
 																 source_columns[decltype(ic)::value],
 																 source_index);
 
 					constructed_columns++;
@@ -678,16 +678,15 @@
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
-					[&](auto ic) noexcept(
-						std::is_nothrow_copy_constructible_v<typename column_from_ic<decltype(ic)>::storage_type>)
+					[&](auto ic) noexcept(std::is_nothrow_copy_constructible_v<storage_type<decltype(ic)::value>>)
 				{
 					column_from_ic<decltype(ic)>::copy_construct(dest_columns[decltype(ic)::value],
 																 dest_index,
 																 source_columns[decltype(ic)::value],
 																 source_index);
 
 					constructed_columns++;
@@ -920,15 +919,15 @@
 				{
 					for (size_t i = 0; i < count; i++)
 						copy_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
 				}
 			}
 		}
 
-		//--- swap -----------------------------------------------------------------------------------------------------
+		//--- swap rows ------------------------------------------------------------------------------------------------
 
 	  private:
 		template <typename... Args, size_t... Cols>
 		SOAGEN_CPP20_CONSTEXPR
 		static void swap_rows(column_pointers& lhs_columns,
 							  size_t lhs_index,
 							  column_pointers& rhs_columns,
@@ -950,14 +949,43 @@
 							  column_pointers& rhs_columns,
 							  size_t rhs_index) //
 			noexcept(all_nothrow_swappable)
 		{
 			swap_rows(lhs_columns, lhs_index, rhs_columns, rhs_index, std::make_index_sequence<column_count>{});
 		}
 
+		//--- swap columns ---------------------------------------------------------------------------------------------
+
+		template <size_t A, size_t B>
+		static constexpr bool can_swap_columns =
+			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_swappable);
+
+		template <size_t A, size_t B>
+		static constexpr bool can_nothrow_swap_columns =
+			A == B || (std::is_same_v<storage_type<A>, storage_type<B>> && column<A>::is_nothrow_swappable);
+
+		SOAGEN_HIDDEN_CONSTRAINT((can_swap_columns<A, B>), size_t A, size_t B)
+		SOAGEN_CPP20_CONSTEXPR
+		static void swap_columns([[maybe_unused]] column_pointers& columns,
+								 [[maybe_unused]] size_t start,
+								 [[maybe_unused]] size_t count) //
+			noexcept(can_nothrow_swap_columns<A, B>)
+		{
+			if constexpr (A != B)
+			{
+				static_assert(std::is_same_v<storage_type<A>, storage_type<B>>);
+				static_assert(column<A>::is_swappable);
+				static_assert(column<B>::is_swappable);
+
+				count += start;
+				for (; start < count; start++)
+					column<A>::swap(columns[A], start, columns[B], start);
+			}
+		}
+
 		//--- equality -------------------------------------------------------------------------------------------------
 
 	  private:
 		template <typename... Args, size_t... Cols>
 		SOAGEN_NODISCARD
 		constexpr static bool equal(const const_column_pointers& lhs_columns,
 									size_t lhs_start_index,
@@ -1079,20 +1107,20 @@
 		///				type. This is for over-alignment scenarios where you need to do things in batches (e.g. SIMD).
 		static constexpr size_t aligned_stride = lcm(size_t{ 1 }, Columns::aligned_stride...);
 
 		// columns
 		// (note that these hide the base class typedefs - this is intentional)
 
 		/// @brief	Returns the #soagen::column_traits for the column at the specified index.
-		template <size_t Index>
-		using column = type_at_index<Index, Columns...>;
+		template <auto Index>
+		using column = type_at_index<static_cast<size_t>(Index), Columns...>;
 
 		/// @brief	Same as #column but takes an #index_constant.
 		template <typename IndexConstant>
-		using column_from_ic = type_at_index<IndexConstant::value, Columns...>;
+		using column_from_ic = type_at_index<static_cast<size_t>(IndexConstant::value), Columns...>;
 
 		/// @brief Array containing the `alignment` for each column.
 		static constexpr size_t column_alignments[column_count] = { Columns::alignment... };
 
 		/// @brief The max `alignment` of all columns in the table.
 		static constexpr size_t largest_alignment = max(size_t{ 1 }, Columns::alignment...);
```

### Comparing `soagen-0.1.2/src/soagen/includes.py` & `soagen-0.2.0/src/soagen/includes.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/log.py` & `soagen-0.2.0/src/soagen/log.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/main.py` & `soagen-0.2.0/src/soagen/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,50 +189,47 @@
                             f.write(new_text)
 
     # copy .clang-format
     if update_templated_hpps or update_soagen_hpp or update_tests or update_examples:
         utils.copy_file(Path(paths.REPOSITORY, r'.clang-format'), paths.HPP, logger=log.i)
 
     # regenerate the generated headers from their templates
-    if update_templated_hpps:
-        if paths.MAKE_SINGLE.exists():
-            for template in utils.enumerate_files(paths.HPP_TEMPLATES, all='*.hpp.in', recursive=True):
-                output = Path(paths.HPP_GENERATED, template.stem)
-                os.makedirs(str(paths.HPP_GENERATED), exist_ok=True)
-                utils.run_python_script(
-                    *(
-                        [
-                            paths.MAKE_SINGLE,
-                            str(template),
-                            r'--output',
-                            output,
-                            r'--namespaces',
-                            r'soagen',
-                            r'detail',
-                            r'--macros',
-                            r'SOAGEN',
-                        ]
-                        + ([r'--no-strip-hidden-bases'] if template.name not in (r'compressed_pair.hpp.in',) else [])
-                        + (
-                            [r'--no-strip-doxygen-from-snippets']
-                            if template.name not in (r'compressed_pair.hpp.in', r'preprocessor.hpp.in')
-                            else []
-                        )
+    if update_templated_hpps and paths.MAKE_SINGLE.exists():
+        for template in utils.enumerate_files(paths.HPP_TEMPLATES, all='*.hpp.in', recursive=True):
+            output = Path(paths.HPP_GENERATED, template.stem)
+            os.makedirs(str(paths.HPP_GENERATED), exist_ok=True)
+            utils.run_python_script(
+                *(
+                    [
+                        paths.MAKE_SINGLE,
+                        str(template),
+                        r'--output',
+                        output,
+                        r'--namespaces',
+                        r'soagen',
+                        r'detail',
+                        r'--macros',
+                        r'SOAGEN',
+                    ]
+                    + ([r'--no-strip-hidden-bases'] if template.name not in (r'compressed_pair.hpp.in',) else [])
+                    + (
+                        [r'--no-strip-doxygen-from-snippets']
+                        if template.name not in (r'compressed_pair.hpp.in', r'preprocessor.hpp.in')
+                        else []
                     )
                 )
-                text = utils.read_all_text_from_file(output, logger=log.i)
-                try:
-                    text = utils.clang_format(text, cwd=output.parent)
-                except:
-                    pass
-                log.i(rf'Writing {output}')
-                with open(output, 'w', encoding='utf-8', newline='\n') as f:
-                    f.write(text)
-        else:
-            log.w(rf'could not regenerate headers using muu: {paths.MAKE_SINGLE.name} did not exist or was not a file')
+            )
+            text = utils.read_all_text_from_file(output, logger=log.i)
+            try:
+                text = utils.clang_format(text, cwd=output.parent)
+            except:
+                pass
+            log.i(rf'Writing {output}')
+            with open(output, 'w', encoding='utf-8', newline='\n') as f:
+                f.write(text)
 
     # read soagen.hpp + preprocess into single header
     if update_soagen_hpp:
         soagen_hpp_in = Path(paths.HPP, 'soagen.hpp')
         soagen_hpp_out = Path(paths.HPP_SINGLE, 'soagen.hpp')
         text = str(Preprocessor(soagen_hpp_in))
         text = utils.replace_metavar(r'version', VERSION_STRING, text)
@@ -455,21 +452,21 @@
             for src in (config.hpp,):
 
                 def on_flush(o: Writer, s: str) -> str:
                     nonlocal src
                     # sub in external headers
                     includes = sorted(set(src.includes.external + cpp.detect_includes(s)))
                     includes = cpp.remove_implicit_includes(includes)
-                    PATTERN = r'\n[ \t]*//[ \t]*####[ \t]+SOAGEN_EXTERNAL_HEADERS[ \t]+####[ \t]*\n'
+                    EXTERNAL_HEADERS = r'\n[ \t]*//[ \t]*__SOAGEN_EXTERNAL_HEADERS[ \t]*\n'
                     rep = '\nSOAGEN_DISABLE_WARNINGS;'
                     for inc in includes:
                         rep += f'\n#include <{inc}>'
                     rep += '\n#if SOAGEN_HAS_EXCEPTIONS\n\t#include <stdexcept>\n#endif'
                     rep += '\nSOAGEN_ENABLE_WARNINGS;\n'
-                    s = re.sub(PATTERN, rep, s)
+                    s = re.sub(EXTERNAL_HEADERS, rep, s)
                     # strip doxygen stuff if we have that disabled
                     if not o.doxygen:
                         s = re.sub(
                             r'\n[ \t]*#[ \t]*if[ \t]*SOAGEN_DOXYGEN[ \t]*\n.+?\n[ \t]*#[ \t]*endif[ \t]*\n',
                             '\n',
                             s,
                             flags=re.DOTALL,
```

### Comparing `soagen-0.1.2/src/soagen/metavars.py` & `soagen-0.2.0/src/soagen/metavars.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/natvis_file.py` & `soagen-0.2.0/src/soagen/natvis_file.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/paths.py` & `soagen-0.2.0/src/soagen/paths.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/preprocessor.py` & `soagen-0.2.0/src/soagen/preprocessor.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/schemas.py` & `soagen-0.2.0/src/soagen/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     )
 
 
 def ValueOrArray(typ, name='', length=None):
     global py2toml
     inner = None
     if length is None:
-        inner = Or(typ, [typ], error=rf'{name + ": " if name else ""}expected {py2toml[typ]} or array of {py2toml[typ]}s')
+        inner = Or(
+            typ, [typ], error=rf'{name + ": " if name else ""}expected {py2toml[typ]} or array of {py2toml[typ]}s'
+        )
     else:
         err = rf'{name + ": " if name else ""}expected {py2toml[typ]} or array of {length} {py2toml[typ]}{"s" if length != 1 else ""}'
         inner = And(Or(typ, [typ], error=err), lambda v: not isinstance(v, list) or len(v) == length, error=err)
     return And(inner, Use(lambda x: x if isinstance(x, list) else [x]))
 
 
 def Stripped(typ, allow_empty=True, name=''):
```

### Comparing `soagen-0.1.2/src/soagen/struct.py` & `soagen-0.2.0/src/soagen/struct.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,25 @@
 TAB_SPACES = '    '
 
 
 class Struct(Configurable):
     __schema = Schema(
         {
             Optional(r'allocator', default=''): Stripped(str),
+            Optional(r'annotations', default=[]): And(
+                ValueOrArray(str, name=r'annotations'),
+                Use(lambda x: utils.remove_duplicates([s.strip() for s in x if s.strip()])),
+            ),
+            Optional(r'attributes', default=[]): And(
+                ValueOrArray(str, name=r'attributes'),
+                Use(lambda x: utils.remove_duplicates([s.strip() for s in x if s.strip()])),
+            ),
             Optional(r'brief', default=''): Stripped(str),
             Optional(r'copyable', default=True): bool,
-            Optional(r'default_constructible', default=True): bool,
+            Optional(r'default_constructible', default=True): Or(bool, 'auto'),
             Optional(r'details', default=''): Stripped(str),
             Optional(r'epilogue', default=''): Stripped(str),
             Optional(r'footer', default=''): Stripped(str),
             Optional(r'header', default=''): Stripped(str),
             Optional(r'includes', default=dict): {object: object},
             Optional(r'iterators', default=True): bool,
             Optional(r'movable', default=True): bool,
@@ -62,23 +70,34 @@
 
         self.qualified_type = rf'{self.config.namespace}::{self.type}' if self.config.namespace else self.type
         self.qualified_name = self.qualified_type
         self.index = -1  # set by the config
         self.meta = MetaVars()
         self.meta.push(r'name', self.name)
         self.meta.push(r'type', self.type)
+        self.meta.push(r'qualified_name', self.qualified_name)
+        self.meta.push(r'qualified_type', self.qualified_type)
         self.meta.push(r'struct::name', self.name)
         self.meta.push(r'struct::type', self.type)
+        self.meta.push(r'struct::qualified_name', self.qualified_name)
+        self.meta.push(r'struct::qualified_type', self.qualified_type)
         self.meta.push(r'struct::scope', '')
 
         if not self.allocator:
             self.allocator = self.config.allocator
         if self.allocator == r'std::allocator':
             self.allocator = r'std::allocator<std::byte>'
 
+        self.annotations = utils.remove_duplicates(self.config.all_structs.annotations + self.annotations)
+        self.attributes = utils.remove_duplicates(self.config.all_structs.attributes + self.attributes)
+        if r'SOAGEN_EMPTY_BASES' not in self.attributes:
+            self.attributes.append(r'SOAGEN_EMPTY_BASES')
+        if r'__declspec(empty_bases)' in self.attributes:
+            self.attributes.remove(r'__declspec(empty_bases)')
+
         with SchemaContext('includes'):
             self.includes = Includes(cfg, self.includes)
 
         has_defaults = False
         for i in range(len(self.variables)):
             with SchemaContext(
                 rf"variable '{self.variables[i]['name']}'" if r'name' in self.variables[i] else rf"variable [{i}]"
@@ -267,17 +286,19 @@
                 @brief {self.brief}
 
                 @details {self.details}
 
                 @note The code and documentation for this class were generated by soagen - https://marzer.github.io/soagen'''
                 )
             )
+            for annotation in self.annotations:
+                o(annotation)
             with ClassDefinition(
                 o,
-                f'class SOAGEN_EMPTY_BASES {self.name}',
+                f'class {" ".join(self.attributes)} {self.name}',
                 hidden_base_classes=[
                     rf'public soagen::mixins::resizable<{self.name}>',
                     rf'public soagen::mixins::equality_comparable<{self.name}>',
                     rf'public soagen::mixins::less_than_comparable<{self.name}>',
                     rf'public soagen::mixins::data_ptr<{self.name}>',
                     rf'public soagen::mixins::const_data_ptr<{self.name}>',
                 ]
@@ -298,23 +319,23 @@
                     {doxygen(r"@brief This class's underlying soagen::table type.")}
                     using table_type = soagen::table_type<{self.name}>;
 
                     {doxygen(r"@brief The soagen::table_traits for the underlying table.")}
                     using table_traits = soagen::table_traits_type<{self.name}>;
 
                     {doxygen(r"@brief The number of columns in the table.")}
-                    static constexpr size_t column_count = soagen::table_traits_type<{self.name}>::column_count;
+                    static constexpr size_type column_count = soagen::table_traits_type<{self.name}>::column_count;
 
                     {doxygen(r"@brief Gets the soagen::column_traits for a specific column of the table.")}
-                    template <size_type Column>
-                    using column_traits = typename table_traits::template column<Column>;
+                    template <auto Column>
+                    using column_traits = typename table_traits::template column<static_cast<size_type>(Column)>;
 
                     {doxygen(r"@brief Gets the type of a specific column in the table.")}
-                    template <size_type Column>
-                    using column_type = typename column_traits<Column>::value_type;
+                    template <auto Column>
+                    using column_type = typename column_traits<static_cast<size_type>(Column)>::value_type;
 
                     '''
                     )
 
                     if self.iterators:
                         o(
                             rf'''
@@ -380,30 +401,30 @@
                     )
 
                     if o.doxygen:
                         o(
                             rf'''
                          #if SOAGEN_DOXYGEN
                         /// @brief Named index constants for all of the columns in the table.
-                        using column_indices = POXY_IMPLEMENTATION_DETAIL(struct dummy_t);
+                        using columns = POXY_IMPLEMENTATION_DETAIL(struct dummy_t);
                         #else'''
                         )
 
-                    with ClassDefinition(o, 'struct column_indices'):
+                    with ClassDefinition(o, 'enum class columns : size_type'):
                         for col in self.columns:
-                            o(rf'static constexpr size_type {col.name} = {col.index};')
+                            o(rf'{col.name} = {col.index},')
 
                     if o.doxygen:
                         o('#endif')
 
                     o(
                         rf'''
 
                     {doxygen(r"@brief Gets the name of the specified column as a null-terminated string.")}
-                    template <size_type Column> static constexpr auto& column_name = soagen::detail::column_name_<{self.name}, Column>::value;
+                    template <auto Column> static constexpr auto& column_name = soagen::detail::column_name<{self.name}, static_cast<size_type>(Column)>::value;
 
                     {self.header}
 
                     '''
                     )
 
                 for access in (r'public', r'protected', r'private'):
@@ -418,20 +439,25 @@
                         rf'''
                     table_type table_;
                     '''
                     )
 
                 with Public(o):
                     ctor_attrs = 'SOAGEN_NODISCARD_CTOR'
-                    o(
-                        rf'''
 
-                    {doxygen(r"@brief Default constructor.")}
-                    {ctor_attrs if self.default_constructible else ""} {self.name}() = {"default" if self.default_constructible else "delete"};
+                    if isinstance(self.default_constructible, bool) or self.default_constructible != 'auto':
+                        o(
+                            rf'''
+                        {doxygen(r"@brief Default constructor.")}
+                        {ctor_attrs if self.default_constructible else ""} {self.name}() = {"default" if self.default_constructible else "delete"};
+                        '''
+                        )
 
+                    o(
+                        rf'''
                     {doxygen(r"@brief Move constructor.")}
                     {ctor_attrs if self.movable else ""} {self.name}({self.name}&&) = {"default" if self.movable else "delete"};
 
                     {doxygen(r"@brief Move-assignment operator.")}
                     {self.name}& operator=({self.name}&&) = {"default" if self.movable else "delete"};
 
                     {doxygen(r"@brief Copy constructor.")}
@@ -672,14 +698,28 @@
                         {self.name}& pop_back(size_type num = 1) //
                             noexcept(noexcept(std::declval<table_type&>().pop_back(size_type{{}})))
                         {{
                             table_.pop_back(num);
                             return *this;
                         }}
 
+                        {doxygen(r"""
+                        @brief Swaps two columns.
+
+                        @availability The two columns must have the same underlying value_type.""")}
+                        template <auto A, auto B>
+                        SOAGEN_ALWAYS_INLINE
+                        SOAGEN_CPP20_CONSTEXPR
+                        {self.name}& swap_columns() //
+                            noexcept(noexcept(std::declval<table_type&>().template swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>()))
+                        {{
+                            table_.template swap_columns<static_cast<size_t>(A), static_cast<size_t>(B)>();
+                            return *this;
+                        }}
+
                         #if SOAGEN_DOXYGEN
 
                         {doxygen(r"""
                         @brief Resizes the table to the given number of rows.
 
                         @availability This method is only available when all the column types are default-constructible.""")}
                         {self.name}& resize(size_type new_size) //
@@ -747,15 +787,15 @@
                                                     types.append(r'size_type')
                                                     names.append(r'index_')
                                                     forwards.append(names[-1])
                                                     deduced.append(False)
 
                                             if row_overload:
                                                 template_params.append(r'typename Table')
-                                                template_params.append(r'size_t... Columns')
+                                                template_params.append(r'auto... Columns')
                                                 template_defaults += ['', '']
                                                 types.append(r'const soagen::row<Table, Columns...>&')
                                                 names.append(r'row_')
                                                 deduced.append(True)
                                                 defaults.append('')
                                                 forwards.append(names[-1])
                                             else:
@@ -1055,31 +1095,31 @@
                         @availability This method is only available when all the column types are trivially-copyable.""")}
                         constexpr const std::byte* const data() //
                             noexcept(soagen::has_nothrow_data_member<const table_type>);
 
                         #endif
 
                         {doxygen(r"@brief Returns a pointer to the elements of a specific column.")}
-                        template <size_type Column>
+                        template <auto Column>
                         SOAGEN_ALIGNED_COLUMN(Column)
                         constexpr column_type<Column>* column() noexcept
                         {{
-                            static_assert(Column < table_traits::column_count, "column index out of range");
+                            static_assert(static_cast<size_type>(Column) < table_traits::column_count, "column index out of range");
 
-                            return soagen::assume_aligned<soagen::detail::actual_column_alignment<table_traits, allocator_type, Column>>(table_.template column<Column>());
+                            return soagen::assume_aligned<soagen::detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_type>(Column)>>(table_.template column<static_cast<size_type>(Column)>());
                         }}
 
                         {doxygen(r"@brief Returns a pointer to the elements of a specific column.")}
-                        template <size_type Column>
+                        template <auto Column>
                         SOAGEN_ALIGNED_COLUMN(Column)
                         constexpr std::add_const_t<column_type<Column>>* column() const noexcept
                         {{
-                            static_assert(Column < table_traits::column_count, "column index out of range");
+                            static_assert(static_cast<size_type>(Column) < table_traits::column_count, "column index out of range");
 
-                            return soagen::assume_aligned<soagen::detail::actual_column_alignment<table_traits, allocator_type, Column>>(table_.template column<Column>());
+                            return soagen::assume_aligned<soagen::detail::actual_column_alignment<table_traits, allocator_type, static_cast<size_type>(Column)>>(table_.template column<static_cast<size_type>(Column)>());
                         }}'''
                         )
                         for i in range(len(self.columns)):
                             o(
                                 rf'''
                              {doxygen(rf"@brief Returns a pointer to the elements in column [{i}]: {self.columns[i].name}.")}
                             SOAGEN_ALIGNED_COLUMN({i})
@@ -1126,22 +1166,22 @@
                             row_type = ('rvalue_' if ref == '&&' else ('const_' if const else '')) + r'row_type'
                             o(
                                 rf'''
                                 {doxygen(r"""
                                 @brief Returns the row at the given index.
 
                                 @tparam Columns Indices of the columns to include in the row. Leave the list empty for all columns.""")}
-                                template <size_type... Columns>
+                                template <auto... Columns>
                                 SOAGEN_PURE_GETTER
                                 SOAGEN_CPP20_CONSTEXPR
                                 soagen::row_type<{const}{self.name}{ref}, Columns...> row(size_type index) {const}{ref} noexcept
                                 {{
                                     if constexpr (sizeof...(Columns))
                                     {{
-                                        return {{ {{ {move_l}this->template column<Columns>()[index]{move_r} }}... }};
+                                        return {{ {{ {move_l}this->template column<static_cast<size_type>(Columns)>()[index]{move_r} }}... }};
                                     }}
                                     else
                                     {{
                                         return {move}(*this).template row<{self.column_indices}>(index);
                                     }}
                                 }}
```

### Comparing `soagen-0.1.2/src/soagen/type_list.py` & `soagen-0.2.0/src/soagen/type_list.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/utils.py` & `soagen-0.2.0/src/soagen/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,7 +93,15 @@
     text = text.replace('\n\n', '\b')
     text = text.replace('\n', ' ')
     text = text.replace('\b', '\n')
     text = text.split('\n')
     for i in range(len(text)):
         text[i] = '\n'.join(textwrap.wrap(text[i], width=int(line_length), tabsize=int(tab_size)))
     return '\n\n'.join(text)
+
+
+def remove_duplicates(vals: list) -> list:
+    new_vals = []
+    for v in coerce_collection(vals):
+        if v not in new_vals:
+            new_vals.append(v)
+    return new_vals
```

### Comparing `soagen-0.1.2/src/soagen/variable.py` & `soagen-0.2.0/src/soagen/variable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/version.py` & `soagen-0.2.0/src/soagen/version.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen/writer.py` & `soagen-0.2.0/src/soagen/writer.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.2/src/soagen.egg-info/PKG-INFO` & `soagen-0.2.0/src/soagen.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.1.2
+Version: 0.2.0
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,26 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.2.0
+
+-   Added `structs.annotations`
+-   Added `structs.attributes`
+-   Added `auto` option for `structs.default_constructible`
+-   Added `soagen::row_base`
+-   Added `soagen::table_base`
+-   Added `soagen::iterator_base`
+-   Added `Base` template argument to `soagen::table` for CRTP
+-   Added `swap_columns<>()`
+-   Made `column_indices` member struct into `enum class columns`
+
 ## v0.1.2
 
 -   Minor refactors.
 
 ## v0.1.1
 
 -   Minor refactors.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.1.2 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.2.0 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,9 +13,14 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor
-refactors. ## v0.1.0 - First public release ð&#xFE0F;
+sponsors/marzer # Changelog ## v0.2.0 - Added `structs.annotations` - Added
+`structs.attributes` - Added `auto` option for `structs.default_constructible`
+- Added `soagen::row_base` - Added `soagen::table_base` - Added `soagen::
+iterator_base` - Added `Base` template argument to `soagen::table` for CRTP -
+Added `swap_columns<>()` - Made `column_indices` member struct into `enum class
+columns` ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor refactors. ## v0.1.0 -
+First public release ð&#xFE0F;
```

### Comparing `soagen-0.1.2/src/soagen.egg-info/SOURCES.txt` & `soagen-0.2.0/src/soagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

