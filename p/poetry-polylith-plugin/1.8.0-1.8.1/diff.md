# Comparing `tmp/poetry_polylith_plugin-1.8.0.tar.gz` & `tmp/poetry_polylith_plugin-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_polylith_plugin-1.8.0.tar", max compression
+gzip compressed data, was "poetry_polylith_plugin-1.8.1.tar", max compression
```

## Comparing `poetry_polylith_plugin-1.8.0.tar` & `poetry_polylith_plugin-1.8.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1475 2023-04-01 08:55:53.793699 poetry_polylith_plugin-1.8.0/README.md
--rw-r--r--   0        0        0      244 2022-11-22 16:34:48.997679 poetry_polylith_plugin-1.8.0/polylith/bricks/__init__.py
--rw-r--r--   0        0        0      555 2023-03-13 14:27:27.458090 poetry_polylith_plugin-1.8.0/polylith/bricks/base.py
--rw-r--r--   0        0        0     1045 2023-03-13 14:27:27.458215 poetry_polylith_plugin-1.8.0/polylith/bricks/brick.py
--rw-r--r--   0        0        0     1096 2023-03-14 14:29:50.224158 poetry_polylith_plugin-1.8.0/polylith/bricks/component.py
--rw-r--r--   0        0        0       98 2023-07-29 11:51:13.391379 poetry_polylith_plugin-1.8.0/polylith/check/__init__.py
--rw-r--r--   0        0        0     1347 2023-07-29 11:51:13.391711 poetry_polylith_plugin-1.8.0/polylith/check/collect.py
--rw-r--r--   0        0        0     1051 2023-03-13 14:27:27.458511 poetry_polylith_plugin-1.8.0/polylith/check/grouping.py
--rw-r--r--   0        0        0     2516 2023-07-29 11:51:13.391873 poetry_polylith_plugin-1.8.0/polylith/check/report.py
--rw-r--r--   0        0        0       98 2022-11-04 07:17:35.622947 poetry_polylith_plugin-1.8.0/polylith/development/__init__.py
--rw-r--r--   0        0        0      211 2022-11-22 16:34:48.998071 poetry_polylith_plugin-1.8.0/polylith/development/development.py
--rw-r--r--   0        0        0       75 2022-11-22 16:34:48.998183 poetry_polylith_plugin-1.8.0/polylith/diff/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-05 14:32:20.927245 poetry_polylith_plugin-1.8.0/polylith/diff/collect.py
--rw-r--r--   0        0        0     2670 2023-04-23 13:53:29.379615 poetry_polylith_plugin-1.8.0/polylith/diff/report.py
--rw-r--r--   0        0        0       68 2022-11-04 07:17:35.623197 poetry_polylith_plugin-1.8.0/polylith/dirs/__init__.py
--rw-r--r--   0        0        0      273 2022-11-22 16:34:48.998517 poetry_polylith_plugin-1.8.0/polylith/dirs/dirs.py
--rw-r--r--   0        0        0       72 2022-11-04 07:17:35.623423 poetry_polylith_plugin-1.8.0/polylith/files/__init__.py
--rw-r--r--   0        0        0      145 2022-11-04 07:17:35.623526 poetry_polylith_plugin-1.8.0/polylith/files/files.py
--rw-r--r--   0        0        0      151 2023-04-23 13:53:29.379732 poetry_polylith_plugin-1.8.0/polylith/imports/__init__.py
--rw-r--r--   0        0        0     1730 2023-07-29 11:51:13.392045 poetry_polylith_plugin-1.8.0/polylith/imports/parser.py
--rw-r--r--   0        0        0      426 2023-04-01 08:55:53.790585 poetry_polylith_plugin-1.8.0/polylith/info/__init__.py
--rw-r--r--   0        0        0     1692 2023-04-01 08:55:53.790905 poetry_polylith_plugin-1.8.0/polylith/info/collect.py
--rw-r--r--   0        0        0     2458 2023-08-01 13:54:57.805503 poetry_polylith_plugin-1.8.0/polylith/info/report.py
--rw-r--r--   0        0        0       91 2022-11-04 07:17:35.623663 poetry_polylith_plugin-1.8.0/polylith/interface/__init__.py
--rw-r--r--   0        0        0      876 2023-03-13 14:27:27.458927 poetry_polylith_plugin-1.8.0/polylith/interface/interfaces.py
--rw-r--r--   0        0        0      201 2023-04-23 13:53:29.380600 poetry_polylith_plugin-1.8.0/polylith/libs/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-23 13:53:29.380732 poetry_polylith_plugin-1.8.0/polylith/libs/grouping.py
--rw-r--r--   0        0        0     3677 2023-07-28 17:52:12.877081 poetry_polylith_plugin-1.8.0/polylith/libs/report.py
--rw-r--r--   0        0        0     4156 2023-04-23 13:53:29.381083 poetry_polylith_plugin-1.8.0/polylith/libs/stdlib.py
--rw-r--r--   0        0        0      790 2023-04-23 13:53:29.381323 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/__init__.py
--rw-r--r--   0        0        0     2532 2023-07-29 11:51:13.392333 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/check.py
--rw-r--r--   0        0        0      552 2023-03-13 14:27:27.461635 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create.py
--rw-r--r--   0        0        0      634 2023-03-13 14:27:27.461785 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create_base.py
--rw-r--r--   0        0        0      674 2023-03-13 14:27:27.461919 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create_component.py
--rw-r--r--   0        0        0      680 2023-03-13 14:27:27.462039 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create_project.py
--rw-r--r--   0        0        0      949 2022-11-22 16:34:48.999505 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create_workspace.py
--rw-r--r--   0        0        0     1744 2023-04-05 14:32:20.927796 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/diff.py
--rw-r--r--   0        0        0     1162 2023-08-01 13:54:57.805710 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/info.py
--rw-r--r--   0        0        0     2328 2023-04-01 08:55:53.792609 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/libs.py
--rw-r--r--   0        0        0     1803 2023-07-29 11:51:13.392698 poetry_polylith_plugin-1.8.0/polylith/poetry/commands/sync.py
--rw-r--r--   0        0        0       87 2022-11-04 07:17:35.621247 poetry_polylith_plugin-1.8.0/polylith/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      959 2023-04-23 13:53:29.378523 poetry_polylith_plugin-1.8.0/polylith/poetry_plugin/plugin.py
--rw-r--r--   0        0        0      331 2023-04-23 13:53:29.381659 poetry_polylith_plugin-1.8.0/polylith/project/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-05 14:32:20.927943 poetry_polylith_plugin-1.8.0/polylith/project/create.py
--rw-r--r--   0        0        0     1433 2023-04-23 13:53:29.381846 poetry_polylith_plugin-1.8.0/polylith/project/get.py
--rw-r--r--   0        0        0      433 2023-04-01 08:55:53.793395 poetry_polylith_plugin-1.8.0/polylith/project/parser.py
--rw-r--r--   0        0        0      142 2023-03-13 14:27:27.462643 poetry_polylith_plugin-1.8.0/polylith/readme/__init__.py
--rw-r--r--   0        0        0     1067 2023-04-05 14:32:20.928603 poetry_polylith_plugin-1.8.0/polylith/readme/readme.py
--rw-r--r--   0        0        0      374 2022-11-22 16:34:49.000462 poetry_polylith_plugin-1.8.0/polylith/repo/__init__.py
--rw-r--r--   0        0        0      985 2022-11-22 16:34:49.000581 poetry_polylith_plugin-1.8.0/polylith/repo/repo.py
--rw-r--r--   0        0        0       58 2023-04-23 13:53:29.381960 poetry_polylith_plugin-1.8.0/polylith/reporting/__init__.py
--rw-r--r--   0        0        0      172 2023-07-27 12:41:39.939902 poetry_polylith_plugin-1.8.0/polylith/reporting/theme.py
--rw-r--r--   0        0        0      188 2023-04-23 13:53:29.382161 poetry_polylith_plugin-1.8.0/polylith/sync/__init__.py
--rw-r--r--   0        0        0     1853 2023-07-29 11:51:13.393013 poetry_polylith_plugin-1.8.0/polylith/sync/collect.py
--rw-r--r--   0        0        0      971 2023-07-29 11:51:13.393395 poetry_polylith_plugin-1.8.0/polylith/sync/report.py
--rw-r--r--   0        0        0     1787 2023-04-23 13:53:29.382434 poetry_polylith_plugin-1.8.0/polylith/sync/update.py
--rw-r--r--   0        0        0       71 2022-11-04 07:17:35.625873 poetry_polylith_plugin-1.8.0/polylith/test/__init__.py
--rw-r--r--   0        0        0      859 2022-11-22 16:34:49.000744 poetry_polylith_plugin-1.8.0/polylith/test/tests.py
--rw-r--r--   0        0        0       94 2023-03-13 14:27:27.463180 poetry_polylith_plugin-1.8.0/polylith/workspace/__init__.py
--rw-r--r--   0        0        0     1089 2023-03-13 14:27:27.463863 poetry_polylith_plugin-1.8.0/polylith/workspace/create.py
--rw-r--r--   0        0        0     1832 2023-05-22 11:03:54.995273 poetry_polylith_plugin-1.8.0/polylith/workspace/parser.py
--rw-r--r--   0        0        0      949 2023-03-13 14:27:27.464047 poetry_polylith_plugin-1.8.0/polylith/workspace/paths.py
--rw-r--r--   0        0        0      781 2023-08-01 13:55:15.191528 poetry_polylith_plugin-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1475 2023-04-01 08:55:53.793699 poetry_polylith_plugin-1.8.1/README.md
+-rw-r--r--   0        0        0      244 2022-11-22 16:34:48.997679 poetry_polylith_plugin-1.8.1/polylith/bricks/__init__.py
+-rw-r--r--   0        0        0      555 2023-03-13 14:27:27.458090 poetry_polylith_plugin-1.8.1/polylith/bricks/base.py
+-rw-r--r--   0        0        0     1045 2023-03-13 14:27:27.458215 poetry_polylith_plugin-1.8.1/polylith/bricks/brick.py
+-rw-r--r--   0        0        0     1096 2023-03-14 14:29:50.224158 poetry_polylith_plugin-1.8.1/polylith/bricks/component.py
+-rw-r--r--   0        0        0       98 2023-07-29 11:51:13.391379 poetry_polylith_plugin-1.8.1/polylith/check/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-29 11:51:13.391711 poetry_polylith_plugin-1.8.1/polylith/check/collect.py
+-rw-r--r--   0        0        0     1051 2023-03-13 14:27:27.458511 poetry_polylith_plugin-1.8.1/polylith/check/grouping.py
+-rw-r--r--   0        0        0     2516 2023-07-29 11:51:13.391873 poetry_polylith_plugin-1.8.1/polylith/check/report.py
+-rw-r--r--   0        0        0       98 2022-11-04 07:17:35.622947 poetry_polylith_plugin-1.8.1/polylith/development/__init__.py
+-rw-r--r--   0        0        0      211 2022-11-22 16:34:48.998071 poetry_polylith_plugin-1.8.1/polylith/development/development.py
+-rw-r--r--   0        0        0       75 2022-11-22 16:34:48.998183 poetry_polylith_plugin-1.8.1/polylith/diff/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-05 14:32:20.927245 poetry_polylith_plugin-1.8.1/polylith/diff/collect.py
+-rw-r--r--   0        0        0     1997 2023-08-01 15:25:09.532718 poetry_polylith_plugin-1.8.1/polylith/diff/report.py
+-rw-r--r--   0        0        0       68 2022-11-04 07:17:35.623197 poetry_polylith_plugin-1.8.1/polylith/dirs/__init__.py
+-rw-r--r--   0        0        0      273 2022-11-22 16:34:48.998517 poetry_polylith_plugin-1.8.1/polylith/dirs/dirs.py
+-rw-r--r--   0        0        0       72 2022-11-04 07:17:35.623423 poetry_polylith_plugin-1.8.1/polylith/files/__init__.py
+-rw-r--r--   0        0        0      145 2022-11-04 07:17:35.623526 poetry_polylith_plugin-1.8.1/polylith/files/files.py
+-rw-r--r--   0        0        0      151 2023-04-23 13:53:29.379732 poetry_polylith_plugin-1.8.1/polylith/imports/__init__.py
+-rw-r--r--   0        0        0     1730 2023-07-29 11:51:13.392045 poetry_polylith_plugin-1.8.1/polylith/imports/parser.py
+-rw-r--r--   0        0        0      528 2023-08-01 15:25:09.532901 poetry_polylith_plugin-1.8.1/polylith/info/__init__.py
+-rw-r--r--   0        0        0     1692 2023-04-01 08:55:53.790905 poetry_polylith_plugin-1.8.1/polylith/info/collect.py
+-rw-r--r--   0        0        0     3116 2023-08-01 15:25:09.533076 poetry_polylith_plugin-1.8.1/polylith/info/report.py
+-rw-r--r--   0        0        0       91 2022-11-04 07:17:35.623663 poetry_polylith_plugin-1.8.1/polylith/interface/__init__.py
+-rw-r--r--   0        0        0      876 2023-03-13 14:27:27.458927 poetry_polylith_plugin-1.8.1/polylith/interface/interfaces.py
+-rw-r--r--   0        0        0      201 2023-04-23 13:53:29.380600 poetry_polylith_plugin-1.8.1/polylith/libs/__init__.py
+-rw-r--r--   0        0        0     1220 2023-04-23 13:53:29.380732 poetry_polylith_plugin-1.8.1/polylith/libs/grouping.py
+-rw-r--r--   0        0        0     3677 2023-07-28 17:52:12.877081 poetry_polylith_plugin-1.8.1/polylith/libs/report.py
+-rw-r--r--   0        0        0     4156 2023-04-23 13:53:29.381083 poetry_polylith_plugin-1.8.1/polylith/libs/stdlib.py
+-rw-r--r--   0        0        0      790 2023-04-23 13:53:29.381323 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/__init__.py
+-rw-r--r--   0        0        0     2532 2023-07-29 11:51:13.392333 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/check.py
+-rw-r--r--   0        0        0      552 2023-03-13 14:27:27.461635 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create.py
+-rw-r--r--   0        0        0      634 2023-03-13 14:27:27.461785 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create_base.py
+-rw-r--r--   0        0        0      674 2023-03-13 14:27:27.461919 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create_component.py
+-rw-r--r--   0        0        0      680 2023-03-13 14:27:27.462039 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create_project.py
+-rw-r--r--   0        0        0      949 2022-11-22 16:34:48.999505 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create_workspace.py
+-rw-r--r--   0        0        0     1744 2023-04-05 14:32:20.927796 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/diff.py
+-rw-r--r--   0        0        0     1381 2023-08-01 15:25:09.533257 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/info.py
+-rw-r--r--   0        0        0     2328 2023-04-01 08:55:53.792609 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/libs.py
+-rw-r--r--   0        0        0     1803 2023-07-29 11:51:13.392698 poetry_polylith_plugin-1.8.1/polylith/poetry/commands/sync.py
+-rw-r--r--   0        0        0       87 2022-11-04 07:17:35.621247 poetry_polylith_plugin-1.8.1/polylith/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      959 2023-04-23 13:53:29.378523 poetry_polylith_plugin-1.8.1/polylith/poetry_plugin/plugin.py
+-rw-r--r--   0        0        0      331 2023-04-23 13:53:29.381659 poetry_polylith_plugin-1.8.1/polylith/project/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-05 14:32:20.927943 poetry_polylith_plugin-1.8.1/polylith/project/create.py
+-rw-r--r--   0        0        0     1433 2023-04-23 13:53:29.381846 poetry_polylith_plugin-1.8.1/polylith/project/get.py
+-rw-r--r--   0        0        0      433 2023-04-01 08:55:53.793395 poetry_polylith_plugin-1.8.1/polylith/project/parser.py
+-rw-r--r--   0        0        0      142 2023-03-13 14:27:27.462643 poetry_polylith_plugin-1.8.1/polylith/readme/__init__.py
+-rw-r--r--   0        0        0     1067 2023-04-05 14:32:20.928603 poetry_polylith_plugin-1.8.1/polylith/readme/readme.py
+-rw-r--r--   0        0        0      374 2022-11-22 16:34:49.000462 poetry_polylith_plugin-1.8.1/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      985 2022-11-22 16:34:49.000581 poetry_polylith_plugin-1.8.1/polylith/repo/repo.py
+-rw-r--r--   0        0        0       58 2023-04-23 13:53:29.381960 poetry_polylith_plugin-1.8.1/polylith/reporting/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-27 12:41:39.939902 poetry_polylith_plugin-1.8.1/polylith/reporting/theme.py
+-rw-r--r--   0        0        0      188 2023-04-23 13:53:29.382161 poetry_polylith_plugin-1.8.1/polylith/sync/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-29 11:51:13.393013 poetry_polylith_plugin-1.8.1/polylith/sync/collect.py
+-rw-r--r--   0        0        0      971 2023-07-29 11:51:13.393395 poetry_polylith_plugin-1.8.1/polylith/sync/report.py
+-rw-r--r--   0        0        0     1787 2023-04-23 13:53:29.382434 poetry_polylith_plugin-1.8.1/polylith/sync/update.py
+-rw-r--r--   0        0        0       71 2022-11-04 07:17:35.625873 poetry_polylith_plugin-1.8.1/polylith/test/__init__.py
+-rw-r--r--   0        0        0      859 2022-11-22 16:34:49.000744 poetry_polylith_plugin-1.8.1/polylith/test/tests.py
+-rw-r--r--   0        0        0       94 2023-03-13 14:27:27.463180 poetry_polylith_plugin-1.8.1/polylith/workspace/__init__.py
+-rw-r--r--   0        0        0     1089 2023-03-13 14:27:27.463863 poetry_polylith_plugin-1.8.1/polylith/workspace/create.py
+-rw-r--r--   0        0        0     1832 2023-05-22 11:03:54.995273 poetry_polylith_plugin-1.8.1/polylith/workspace/parser.py
+-rw-r--r--   0        0        0      949 2023-03-13 14:27:27.464047 poetry_polylith_plugin-1.8.1/polylith/workspace/paths.py
+-rw-r--r--   0        0        0      781 2023-08-01 15:25:54.485807 poetry_polylith_plugin-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.8.1/PKG-INFO
```

### Comparing `poetry_polylith_plugin-1.8.0/README.md` & `poetry_polylith_plugin-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/bricks/base.py` & `poetry_polylith_plugin-1.8.1/polylith/bricks/base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/bricks/brick.py` & `poetry_polylith_plugin-1.8.1/polylith/bricks/brick.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/bricks/component.py` & `poetry_polylith_plugin-1.8.1/polylith/bricks/component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/check/collect.py` & `poetry_polylith_plugin-1.8.1/polylith/check/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/check/grouping.py` & `poetry_polylith_plugin-1.8.1/polylith/check/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/check/report.py` & `poetry_polylith_plugin-1.8.1/polylith/check/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/diff/collect.py` & `poetry_polylith_plugin-1.8.1/polylith/diff/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/diff/report.py` & `poetry_polylith_plugin-1.8.1/polylith/diff/report.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,27 @@
 from typing import List
 
+from polylith import info
 from polylith.reporting import theme
-from rich import box
-from rich.columns import Columns
 from rich.console import Console
 from rich.padding import Padding
-from rich.table import Table
-
-
-def brick_status(brick, bricks) -> str:
-    status = ":gear:" if brick in bricks else "-"
-
-    return f"[data]{status}[/]"
 
 
 def print_diff_details(
     projects_data: List[dict], bases: List[str], components: List[str]
 ) -> None:
-
     if not bases and not components:
         return
 
     console = Console(theme=theme.poly_theme)
-    table = Table(box=box.SIMPLE_HEAD)
-    table.add_column("[data]changed brick[/]")
-
-    proj_cols = [f"[proj]{project['name']}[/]" for project in projects_data]
-    table.add_column(Columns(proj_cols, align="center", expand=True))
 
-    for brick in sorted(components):
-        cols = [brick_status(brick, p.get("components")) for p in projects_data]
-        table.add_row(f"[comp]{brick}[/]", Columns(cols, align="center", expand=True))
-
-    for brick in sorted(bases):
-        cols = [brick_status(brick, p.get("bases")) for p in projects_data]
-        table.add_row(f"[base]{brick}[/]", Columns(cols, align="center", expand=True))
+    options = {"command": "diff"}
+    table = info.report.build_bricks_in_projects_table(
+        projects_data, bases, components, options
+    )
 
     console.print(table, overflow="ellipsis")
 
 
 def print_detected_changes_in_projects(projects: List[str]) -> None:
     if not projects:
         return
@@ -78,15 +61,14 @@
 
 def print_short_diff(
     projects_data: List[dict],
     projects: List[str],
     bases: List[str],
     components: List[str],
 ) -> None:
-
     a = _changed_projects(projects_data, "components", components)
     b = _changed_projects(projects_data, "bases", bases)
     c = set(projects)
 
     res = {*a, *b, *c}
 
     console = Console(theme=theme.poly_theme)
```

### Comparing `poetry_polylith_plugin-1.8.0/polylith/imports/parser.py` & `poetry_polylith_plugin-1.8.1/polylith/imports/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/info/collect.py` & `poetry_polylith_plugin-1.8.1/polylith/info/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/info/report.py` & `poetry_polylith_plugin-1.8.1/polylith/info/report.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from polylith.reporting import theme
 from rich import box
 from rich.console import Console
 from rich.padding import Padding
 from rich.table import Table
 
 
-def brick_status(brick, bricks) -> str:
-    status = ":heavy_check_mark:" if brick in bricks else "-"
+def brick_status(brick, bricks, command: str) -> str:
+    emoji = ":heavy_check_mark:" if command == "info" else ":gear:"
+
+    status = emoji if brick in bricks else "-"
 
     return f"[data]{status}[/]"
 
 
 def is_project(project: dict) -> bool:
     return project["type"] == "project"
 
@@ -27,46 +29,72 @@
 
     if short:
         return template.format(name="\n".join(name))
 
     return template.format(name=name)
 
 
-def construct_brick_columns(brick: str, brick_type: str, projects_data: List[dict]):
-    statuses = [brick_status(brick, p.get(brick_type)) for p in projects_data]
-
-    return [f"[comp]{brick}[/]"] + statuses
-
-
-def print_bricks_in_projects(
-    projects_data: List[dict], bases: List[str], components: List[str], short: bool
-) -> None:
-    if not components and not bases:
-        return
+def build_bricks_in_projects_table(
+    projects_data: List[dict],
+    bases: List[str],
+    components: List[str],
+    options: dict,
+) -> Table:
+    short = options.get("short", False)
+    command = options.get("command", "info")
 
-    console = Console(theme=theme.poly_theme)
     table = Table(box=box.SIMPLE_HEAD)
     table.add_column("[data]brick[/]")
 
     proj_cols = [printable_name(project, short) for project in projects_data]
 
     for col in proj_cols:
         table.add_column(col, justify="center")
 
     for brick in sorted(components):
-        cols = construct_brick_columns(brick, "components", projects_data)
+        statuses = [
+            brick_status(brick, p.get("components"), command) for p in projects_data
+        ]
+        cols = [f"[comp]{brick}[/]"] + statuses
+
         table.add_row(*cols)
 
     for brick in sorted(bases):
-        cols = construct_brick_columns(brick, "bases", projects_data)
+        statuses = [brick_status(brick, p.get("bases"), command) for p in projects_data]
+        cols = [f"[base]{brick}[/]"] + statuses
+
         table.add_row(*cols)
 
+    return table
+
+
+def print_table(table: Table) -> None:
+    console = Console(theme=theme.poly_theme)
+
     console.print(table, overflow="ellipsis")
 
 
+def print_compressed_view_for_bricks_in_projects(
+    projects_data: List[dict], bases: List[str], components: List[str]
+) -> None:
+    options = {"short": True}
+    table = build_bricks_in_projects_table(projects_data, bases, components, options)
+
+    print_table(table)
+
+
+def print_bricks_in_projects(
+    projects_data: List[dict], bases: List[str], components: List[str]
+) -> None:
+    options = {"short": False}
+    table = build_bricks_in_projects_table(projects_data, bases, components, options)
+
+    print_table(table)
+
+
 def print_workspace_summary(
     projects_data: List[dict], bases: List[str], components: List[str]
 ) -> None:
     console = Console(theme=theme.poly_theme)
 
     console.print(Padding("[data]Workspace summary[/]", (1, 0, 1, 0)))
```

### Comparing `poetry_polylith_plugin-1.8.0/polylith/interface/interfaces.py` & `poetry_polylith_plugin-1.8.1/polylith/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/libs/grouping.py` & `poetry_polylith_plugin-1.8.1/polylith/libs/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/libs/report.py` & `poetry_polylith_plugin-1.8.1/polylith/libs/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/libs/stdlib.py` & `poetry_polylith_plugin-1.8.1/polylith/libs/stdlib.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/__init__.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/check.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/check.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create_base.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create_base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create_component.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create_component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create_project.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create_project.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/create_workspace.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/create_workspace.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/diff.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/diff.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/info.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/info.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,10 +29,19 @@
 
         ns = workspace.parser.get_namespace_from_config(root)
         bases = info.get_bases(root, ns)
         components = info.get_components(root, ns)
         projects_data = info.get_bricks_in_projects(root, components, bases, ns)
 
         info.print_workspace_summary(projects_data, bases, components)
-        info.print_bricks_in_projects(projects_data, bases, components, short)
+
+        if not components and not bases:
+            return 0
+
+        if short:
+            info.print_compressed_view_for_bricks_in_projects(
+                projects_data, bases, components
+            )
+        else:
+            info.print_bricks_in_projects(projects_data, bases, components)
 
         return 0
```

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/libs.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/libs.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry/commands/sync.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry/commands/sync.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/poetry_plugin/plugin.py` & `poetry_polylith_plugin-1.8.1/polylith/poetry_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/project/create.py` & `poetry_polylith_plugin-1.8.1/polylith/project/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/project/get.py` & `poetry_polylith_plugin-1.8.1/polylith/project/get.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/readme/readme.py` & `poetry_polylith_plugin-1.8.1/polylith/readme/readme.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/repo/repo.py` & `poetry_polylith_plugin-1.8.1/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/sync/collect.py` & `poetry_polylith_plugin-1.8.1/polylith/sync/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/sync/report.py` & `poetry_polylith_plugin-1.8.1/polylith/sync/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/sync/update.py` & `poetry_polylith_plugin-1.8.1/polylith/sync/update.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/test/tests.py` & `poetry_polylith_plugin-1.8.1/polylith/test/tests.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/workspace/create.py` & `poetry_polylith_plugin-1.8.1/polylith/workspace/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/workspace/parser.py` & `poetry_polylith_plugin-1.8.1/polylith/workspace/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/polylith/workspace/paths.py` & `poetry_polylith_plugin-1.8.1/polylith/workspace/paths.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.8.0/pyproject.toml` & `poetry_polylith_plugin-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-polylith-plugin"
-version = "1.8.0"
+version = "1.8.1"
 description = "A Poetry plugin that adds tooling support for the Polylith Architecture"
 authors = ["David Vujic"]
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 readme = "README.md"
 packages = [
     {include = "polylith"},
```

### Comparing `poetry_polylith_plugin-1.8.0/PKG-INFO` & `poetry_polylith_plugin-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-polylith-plugin
-Version: 1.8.0
+Version: 1.8.1
 Summary: A Poetry plugin that adds tooling support for the Polylith Architecture
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

