# Comparing `tmp/metloom-0.3.8.tar.gz` & `tmp/metloom-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metloom-0.3.8.tar", last modified: Tue May  9 16:54:42 2023, max compression
+gzip compressed data, was "metloom-0.3.9.tar", last modified: Tue Aug  1 20:44:10 2023, max compression
```

## Comparing `metloom-0.3.8.tar` & `metloom-0.3.9.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:42.551843 metloom-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 16:54:24.000000 metloom-0.3.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-09 16:54:24.000000 metloom-0.3.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-09 16:54:24.000000 metloom-0.3.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-09 16:54:24.000000 metloom-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 16:54:24.000000 metloom-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-09 16:54:42.551843 metloom-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-09 16:54:24.000000 metloom-0.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:42.543842 metloom-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4999 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-09 16:54:24.000000 metloom-0.3.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:42.543842 metloom-0.3.8/metloom/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/dataframe_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:42.547842 metloom-0.3.8/metloom/pointdata/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/pointdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/pointdata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/pointdata/cdec.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/pointdata/mesowest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/pointdata/snotel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/pointdata/snotel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/pointdata/usgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-09 16:54:24.000000 metloom-0.3.8/metloom/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:42.543842 metloom-0.3.8/metloom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-09 16:54:42.000000 metloom-0.3.8/metloom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 16:54:42.000000 metloom-0.3.8/metloom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:54:42.000000 metloom-0.3.8/metloom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 16:54:42.000000 metloom-0.3.8/metloom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:54:42.000000 metloom-0.3.8/metloom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 16:54:42.000000 metloom-0.3.8/metloom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 16:54:42.000000 metloom-0.3.8/metloom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 16:54:42.551843 metloom-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-09 16:54:24.000000 metloom-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:42.547842 metloom-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:42.551843 metloom-0.3.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:54:42.551843 metloom-0.3.8/tests/data/cdec_mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/cdec_mocks/raw_tny_locations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/cdec_mocks/raw_tny_notes.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/cdec_mocks/raw_tny_sensors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/daily_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/platoro_meta.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/station_search_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/testing.cpg
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/testing.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/testing.prj
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/testing.shp
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/testing.shx
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/triangle.cpg
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/triangle.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/triangle.prj
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/triangle.shp
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/data/triangle.shx
--rw-r--r--   0 runner    (1001) docker     (123)    22665 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/test_cdec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/test_dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/test_mesowest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/test_point_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/test_snotel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/test_usgs.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 16:54:24.000000 metloom-0.3.8/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.616397 metloom-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 20:43:56.000000 metloom-0.3.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-01 20:43:56.000000 metloom-0.3.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-01 20:43:56.000000 metloom-0.3.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-01 20:43:56.000000 metloom-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-01 20:43:56.000000 metloom-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-08-01 20:44:10.616397 metloom-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-08-01 20:43:56.000000 metloom-0.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.608396 metloom-0.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-01 20:43:56.000000 metloom-0.3.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-01 20:43:56.000000 metloom-0.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 20:43:56.000000 metloom-0.3.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4999 2023-08-01 20:43:56.000000 metloom-0.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 20:43:56.000000 metloom-0.3.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 20:43:56.000000 metloom-0.3.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-01 20:43:56.000000 metloom-0.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-01 20:43:57.000000 metloom-0.3.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-01 20:43:57.000000 metloom-0.3.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 20:43:57.000000 metloom-0.3.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-08-01 20:43:57.000000 metloom-0.3.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.608396 metloom-0.3.9/metloom/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/dataframe_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.612397 metloom-0.3.9/metloom/pointdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/pointdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/pointdata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/pointdata/cdec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/pointdata/mesowest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/pointdata/snotel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/pointdata/snotel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/pointdata/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-08-01 20:43:57.000000 metloom-0.3.9/metloom/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.608396 metloom-0.3.9/metloom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-08-01 20:44:10.000000 metloom-0.3.9/metloom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-01 20:44:10.000000 metloom-0.3.9/metloom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:44:10.000000 metloom-0.3.9/metloom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 20:44:10.000000 metloom-0.3.9/metloom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:44:10.000000 metloom-0.3.9/metloom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 20:44:10.000000 metloom-0.3.9/metloom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 20:44:10.000000 metloom-0.3.9/metloom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-01 20:44:10.616397 metloom-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-01 20:43:57.000000 metloom-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.612397 metloom-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.616397 metloom-0.3.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.616397 metloom-0.3.9/tests/data/cdec_mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/cdec_mocks/raw_tny_locations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/cdec_mocks/raw_tny_notes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/cdec_mocks/raw_tny_sensors.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/testing.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/testing.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/testing.prj
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/testing.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/testing.shx
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/triangle.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/triangle.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/triangle.prj
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/triangle.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/triangle.shx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:44:10.616397 metloom-0.3.9/tests/data/usgs_mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/usgs_mocks/daily_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/usgs_mocks/hourly_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/usgs_mocks/platoro_meta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/data/usgs_mocks/station_search_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22665 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/test_cdec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/test_dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/test_mesowest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/test_point_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/test_snotel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/test_usgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-01 20:43:57.000000 metloom-0.3.9/tests/test_variables.py
```

### Comparing `metloom-0.3.8/CONTRIBUTING.rst` & `metloom-0.3.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/HISTORY.rst` & `metloom-0.3.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/LICENSE` & `metloom-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/PKG-INFO` & `metloom-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metloom
-Version: 0.3.8
+Version: 0.3.9
 Summary: Location Oriented Observed Meteorology (LOOM)
 Home-page: https://github.com/M3Works/metloom
 Author: M3Works
 Author-email: m3worksllc@gmail.com
 License: BSD license
 Keywords: metloom
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `metloom-0.3.8/README.rst` & `metloom-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/docs/Makefile` & `metloom-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/docs/conf.py` & `metloom-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/docs/installation.rst` & `metloom-0.3.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/docs/make.bat` & `metloom-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/docs/usage.rst` & `metloom-0.3.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/cli.py` & `metloom-0.3.9/metloom/cli.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/dataframe_utils.py` & `metloom-0.3.9/metloom/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/pointdata/base.py` & `metloom-0.3.9/metloom/pointdata/base.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/pointdata/cdec.py` & `metloom-0.3.9/metloom/pointdata/cdec.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/pointdata/mesowest.py` & `metloom-0.3.9/metloom/pointdata/mesowest.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/pointdata/snotel.py` & `metloom-0.3.9/metloom/pointdata/snotel.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/pointdata/snotel_client.py` & `metloom-0.3.9/metloom/pointdata/snotel_client.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/pointdata/usgs.py` & `metloom-0.3.9/metloom/pointdata/usgs.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import requests
 import logging
 from io import StringIO
 from bs4 import BeautifulSoup
+from geopandas import GeoDataFrame
 
 from .base import PointData
 from ..variables import USGSVariables, SensorDescription
-from ..dataframe_utils import merge_df, append_df
+from ..dataframe_utils import merge_df, append_df, resample_whole_df
 
 LOG = logging.getLogger(__name__)
 
 
 class USGSPointData(PointData):
     """
     Implement PointData methods for USGS data source.
@@ -31,15 +32,17 @@
     META_URL = USGS_URL + "site/"
     DATASOURCE = "USGS"
 
     def __init__(self, station_id, name, metadata=None, duration=None):
         """
         See docstring for PointData.__init__
         """
-        super(USGSPointData, self).__init__(station_id, name, metadata=metadata)
+        super(USGSPointData, self).__init__(
+            str(station_id), name, metadata=metadata
+        )
         self._tzinfo = None
         self._raw_metadata = None
         self.duration = duration
 
     def _get_all_metadata(self):
         if self._raw_metadata is None:
             params = {
@@ -91,15 +94,15 @@
             end_date: datetime, date only
         """
         if hasattr(start_date, 'hour'):
             start_date = start_date.date()
         if hasattr(end_date, 'hour'):
             end_date = end_date.date()
 
-        if not end_date > start_date:
+        if not end_date >= start_date:
             LOG.error(
                 f" end_date '{end_date}' must be later than start_date '{start_date}'"
             )
             raise ValueError("end_date must be later than start_date")
 
         return start_date, end_date
 
@@ -161,25 +164,27 @@
                     "returned."
                 )
                 data = []
 
         return data
 
     def _sensor_response_to_df(
-        self, response_data, sensor, final_columns, site_id
+        self, response_data, sensor, final_columns, site_id,
+        resample_duration=None
     ):
         """
         Convert the response data from the API to a GeoDataFrame Format and map columns
         in the dataframe
 
         Args:
             response_data: JSON list response from API
             sensor: SensorDescription obj
             final_columns: List of columns used for filtering
             site_id: site id
+            resample_duration: To resample the array. [None, 'D', 'H']
         Returns:
             GeoDataFrame
         """
 
         if "values" not in response_data:
             LOG.warning(" Response does not contain expected data")
             raise ValueError("Failed parsing response for data")
@@ -196,21 +201,50 @@
             LOG.warning(" Data request resulted in no data returned")
             return []
 
         sensor_df.replace(no_data_value, np.nan, inplace=True)
         sensor_df["site"] = site_id
         sensor_df[f"{sensor.name}_units"] = units
 
+        # cast values to float
+        sensor_df["value"] = sensor_df["value"].astype('float32')
+
         final_columns += [sensor.name, f"{sensor.name}_units"]
         column_map = {"dateTime": "datetime", "value": sensor.name}
         sensor_df.rename(columns=column_map, inplace=True)
-        sensor_df["datetime"] = pd.to_datetime(sensor_df["datetime"])
 
-        if sensor_df["datetime"][0].tzinfo is None:
-            sensor_df["datetime"] = sensor_df["datetime"].apply(self._handle_df_tz)
+        # Daily data doesn't have timezone built in
+        if pd.to_datetime(sensor_df["datetime"])[0].tzinfo is None:
+            sensor_df["datetime"] = pd.DatetimeIndex(
+                pd.to_datetime(sensor_df["datetime"])
+            )
+            # We will handle the timezone after resample to avoid
+            # the case where resampling resets values to 0 hour of the day
+            # for daily data
+            handle_tz_after_resample = True
+
+        # convert hourly or instantaneous data to utc prior to resample
+        else:
+            sensor_df["datetime"] = pd.to_datetime(
+                sensor_df["datetime"], utc=True
+            )
+            handle_tz_after_resample = False
+
+        if resample_duration:
+            sensor_df = resample_whole_df(
+                sensor_df.set_index("datetime"), sensor,
+                interval=resample_duration
+            ).reset_index()
+            sensor_df = GeoDataFrame(sensor_df, geometry=sensor_df["geometry"])
+
+        if handle_tz_after_resample:
+            # handle the timezone if we didn't already
+            sensor_df["datetime"] = sensor_df["datetime"].apply(
+                self._handle_df_tz
+            )
 
         # set index so joining works
         sensor_df.set_index("datetime", inplace=True)
         sensor_df.index = sensor_df.index.tz_convert(self.desired_tzinfo)
         sensor_df = sensor_df.filter(final_columns)
         sensor_df = sensor_df.loc[pd.notna(sensor_df[sensor.name])]
         return sensor_df
@@ -230,49 +264,60 @@
         return response_data, duration
 
     def _get_data(
         self,
         start_date: datetime,
         end_date: datetime,
         variables: List[SensorDescription],
-        duration: str
+        duration_list: List[str],
+        resample_duration=None
     ):
         """
         Args:
             start_date: datetime object for start of data collection period
             end_date: datetime object for end of data collection period
             variables: List of metloom.variables.SensorDescription object
                 from self.ALLOWED_VARIABLES
-            duration: USGS duration code, "dv" or "iv"
+            duration_list: list of USGS duration code, "dv" or "iv"
+            resample_duration: optional if we need to resample the data
         Returns:
             GeoDataFrame of data, indexed on datetime, site
         """
+        if not isinstance(duration_list, list):
+            raise ValueError("duration list must be a list")
 
         start_date, end_date = self._check_dates(start_date, end_date)
 
         params = {
             'startDT': start_date.isoformat(),
             'endDT': end_date.isoformat(),
             'sites': self.id,
             'format': 'json',
-            'siteType': 'ST',
             'siteStatus': 'all'
         }
 
         df = None
         final_columns = ["geometry", "site"]
 
         for sensor in variables:
             params["parameterCd"] = sensor.code
-            response_data, response_duration = self._get_data_fallback(
-                params, duration
-            )
+            response_data = None
+            for duration in duration_list:
+                response_data, response_duration = self._get_data_fallback(
+                    params, duration
+                )
+                # Break if we got data
+                if response_data:
+                    break
+
+            # format the data if we have any
             if response_data:
                 sensor_df = self._sensor_response_to_df(
-                    response_data, sensor, final_columns, self.id
+                    response_data, sensor, final_columns, self.id,
+                    resample_duration=resample_duration
                 )
                 df = merge_df(df, sensor_df)
                 df[sensor.name] = df[sensor.name].astype(float)
 
         if df is not None:
             if len(df.index) > 0:
                 # Set the datasource
@@ -291,26 +336,39 @@
         start_date: datetime,
         end_date: datetime,
         variables: List[SensorDescription],
     ):
         """
         See docstring for PointData.get_daily_data
         """
-        return self._get_data(start_date, end_date, variables, "dv")
+        return self._get_data(
+            start_date, end_date, variables, ["dv", "iv"],
+            resample_duration="24H"
+        )
+
+    def get_hourly_data(
+        self,
+        start_date: datetime,
+        end_date: datetime,
+        variables: List[SensorDescription],
+    ):
+        return self._get_data(
+            start_date, end_date, variables, ["iv"], resample_duration="H"
+        )
 
     def get_instantaneous_data(
         self,
         start_date: datetime,
         end_date: datetime,
         variables: List[SensorDescription],
     ):
         """
         USGS 'instantaneous' data, which is generally 15 minutes.
         """
-        return self._get_data(start_date, end_date, variables, "iv")
+        return self._get_data(start_date, end_date, variables, ["iv"])
 
     @staticmethod
     def _get_url_response(url, params=None, parse='text'):
         """
         Get url response from USGS
 
         Args:
@@ -350,15 +408,15 @@
             else:
                 raise ValueError(f"Format '{parse}' not supported")
 
         return result
 
     @classmethod
     def _station_sensor_search(
-        cls, meta_url, bounds, sensor: SensorDescription, dur="dv", buffer=0.0
+        cls, meta_url, bounds, sensor: SensorDescription, dur="dv,iv", buffer=0.0
     ):
         """
         Search for USGS stations within a bounding box for the given sensor description.
 
         Args:
             meta_url: base url for metadata
             bounds: dictionary of lat/long bounds with keys minx, miny, maxx, maxy
```

### Comparing `metloom-0.3.8/metloom/request_utils.py` & `metloom-0.3.9/metloom/request_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/metloom/variables.py` & `metloom-0.3.9/metloom/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,7 +174,11 @@
     To add more sensors:
     https://help.waterdata.usgs.gov/codes-and-parameters/parameters
     """
     DISCHARGE = SensorDescription("00060", "DISCHARGE", "DISCHARGE (CFS)")
     STREAMFLOW = SensorDescription(
         "74082", "STREAMFLOW", "STREAMFLOW, DAILY VOLUME (AC-FT)"
     )
+    SNOWDEPTH = SensorDescription("72189", "SNOWDEPTH", "Snow depth, Meters")
+    SWE = SensorDescription(
+        "72341", "SWE", "Water content of snow, millimeters"
+    )
```

### Comparing `metloom-0.3.8/metloom.egg-info/PKG-INFO` & `metloom-0.3.9/metloom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metloom
-Version: 0.3.8
+Version: 0.3.9
 Summary: Location Oriented Observed Meteorology (LOOM)
 Home-page: https://github.com/M3Works/metloom
 Author: M3Works
 Author-email: m3worksllc@gmail.com
 License: BSD license
 Keywords: metloom
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `metloom-0.3.8/metloom.egg-info/SOURCES.txt` & `metloom-0.3.9/metloom.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -40,24 +40,25 @@
 tests/test_cdec.py
 tests/test_dataframe_utils.py
 tests/test_mesowest.py
 tests/test_point_data.py
 tests/test_snotel.py
 tests/test_usgs.py
 tests/test_variables.py
-tests/data/daily_response.txt
-tests/data/platoro_meta.txt
-tests/data/station_search_response.txt
 tests/data/testing.cpg
 tests/data/testing.dbf
 tests/data/testing.prj
 tests/data/testing.shp
 tests/data/testing.shx
 tests/data/triangle.cpg
 tests/data/triangle.dbf
 tests/data/triangle.prj
 tests/data/triangle.py
 tests/data/triangle.shp
 tests/data/triangle.shx
 tests/data/cdec_mocks/raw_tny_locations.csv
 tests/data/cdec_mocks/raw_tny_notes.csv
-tests/data/cdec_mocks/raw_tny_sensors.csv
+tests/data/cdec_mocks/raw_tny_sensors.csv
+tests/data/usgs_mocks/daily_response.txt
+tests/data/usgs_mocks/hourly_response.json
+tests/data/usgs_mocks/platoro_meta.txt
+tests/data/usgs_mocks/station_search_response.txt
```

### Comparing `metloom-0.3.8/setup.py` & `metloom-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     include_package_data=True,
     keywords='metloom',
     name='metloom',
     packages=find_packages(include=['metloom', 'metloom.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/M3Works/metloom',
-    version='0.3.8',
+    version='0.3.9',
     zip_safe=False,
 )
```

### Comparing `metloom-0.3.8/tests/data/cdec_mocks/raw_tny_sensors.csv` & `metloom-0.3.9/tests/data/cdec_mocks/raw_tny_sensors.csv`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/data/daily_response.txt` & `metloom-0.3.9/tests/data/usgs_mocks/daily_response.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/data/platoro_meta.txt` & `metloom-0.3.9/tests/data/usgs_mocks/platoro_meta.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/data/station_search_response.txt` & `metloom-0.3.9/tests/data/usgs_mocks/station_search_response.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/test_cdec.py` & `metloom-0.3.9/tests/test_cdec.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/test_dataframe_utils.py` & `metloom-0.3.9/tests/test_dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/test_mesowest.py` & `metloom-0.3.9/tests/test_mesowest.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/test_point_data.py` & `metloom-0.3.9/tests/test_point_data.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/test_snotel.py` & `metloom-0.3.9/tests/test_snotel.py`

 * *Files identical despite different names*

### Comparing `metloom-0.3.8/tests/test_usgs.py` & `metloom-0.3.9/tests/test_usgs.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pandas as pd
 import pytest
 
 from metloom.pointdata import USGSPointData
 from metloom.variables import USGSVariables
 from tests.test_point_data import BasePointDataTest
 
-DATA_DIR = str(Path(__file__).parent.joinpath("data"))
+DATA_DIR = str(Path(__file__).parent.joinpath("data/usgs_mocks"))
 
 
 class TestUSGSStation(BasePointDataTest):
 
     @staticmethod
     def station_search_response():
         with open(join(DATA_DIR, "station_search_response.txt")) as fp:
@@ -91,17 +91,22 @@
         return Response
 
     @classmethod
     def get_url_response(cls, resp="daily"):
         if resp == 'daily':
             with open(join(DATA_DIR, "daily_response.txt")) as fp:
                 data = json.load(fp)
-        if resp == 'metadata':
+        elif resp == 'metadata':
             with open(join(DATA_DIR, "platoro_meta.txt")) as fp:
                 data = fp.read()
+        elif resp == 'hourly':
+            with open(join(DATA_DIR, "hourly_response.json")) as fp:
+                data = json.load(fp)
+        else:
+            raise RuntimeError(f"{resp} is an unknown option")
 
         return data
 
     def test_get_metadata(self, crp_station):
         with patch("metloom.pointdata.usgs.USGSPointData._get_url_response") \
                 as mock_request:
             mock_request.return_value = self.get_url_response(resp="metadata")
@@ -120,18 +125,40 @@
             response = crp_station.get_daily_data(
                 datetime(2020, 7, 1),
                 datetime(2020, 7, 2),
                 [USGSVariables.DISCHARGE],
             )
         pd.testing.assert_frame_equal(response, crp_daily_expected)
 
+    def test_get_hourly_data(self, crp_station, crp_daily_expected):
+        """
+        Test that we resample from 15m to 1 hour correctly
+        """
+        with patch("metloom.pointdata.usgs.USGSPointData._get_url_response") \
+                as mock_requests:
+            mock_requests.side_effect = [
+                self.get_url_response(resp='hourly'),
+                self.get_url_response(resp='metadata')
+            ]
+            response = crp_station.get_hourly_data(
+                datetime(2023, 1, 13),
+                datetime(2023, 1, 13),
+                [USGSVariables.DISCHARGE],
+            )
+        response = response.reset_index()
+        assert response["datetime"].values[0] == pd.to_datetime("2023-01-13 07")
+        assert response["datetime"].values[-1] == pd.to_datetime("2023-01-14 06")
+        assert response["DISCHARGE"].values[0] == 300.0
+        assert response["DISCHARGE"].values[-1] == 283.25
+        assert all(response["site"].values == "08245000")
+
     def test_points_from_geometry(self, shape_obj):
         expected_url = (
             'https://waterservices.usgs.gov/nwis/site/?format=rdb&bBox=-119.8%2C37.7'
-            '%2C-119.2%2C38.2&siteStatus=active&hasDataTypeCd=dv&parameterCd=00060'
+            '%2C-119.2%2C38.2&siteStatus=active&hasDataTypeCd=dv,iv&parameterCd=00060'
         )
         names = [
             'TUOLUMNER NR HETCH HETCHY CA',
             'TUOLUMNE R A GRAND CYN OF TUOLUMNE AB HETCH HETCHY',
             'MILL C BL LUNDY LK NR LEE VINING CA',
             'LEE VINING C BL SADDLEBAG LK NR LEE VINING CA'
         ]
@@ -143,15 +170,15 @@
             assert mock_tb.call_args[0][0] == expected_url
             assert len(result) == 10
             assert [x.name in names for x in result.points]
 
     def test_points_from_geometry_failure(self, shape_obj):
         expected_url = (
             'https://waterservices.usgs.gov/nwis/site/?format=rdb&bBox=-119.8%2C37.7'
-            '%2C-119.2%2C38.2&siteStatus=active&hasDataTypeCd=dv&parameterCd=74082'
+            '%2C-119.2%2C38.2&siteStatus=active&hasDataTypeCd=dv,iv&parameterCd=74082'
         )
         with patch("metloom.pointdata.usgs.requests.get") as mock_request:
             mock_request.return_value = self.failure_response()
             result = USGSPointData.points_from_geometry(
                 shape_obj, [USGSVariables.STREAMFLOW]
             )
             assert result.points == []
```

### Comparing `metloom-0.3.8/tests/test_variables.py` & `metloom-0.3.9/tests/test_variables.py`

 * *Files identical despite different names*

