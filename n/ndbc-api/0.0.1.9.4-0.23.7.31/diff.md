# Comparing `tmp/ndbc-api-0.0.1.9.4.tar.gz` & `tmp/ndbc-api-0.23.7.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ndbc-api-0.0.1.9.4.tar", last modified: Sun Jan  8 07:09:15 2023, max compression
+gzip compressed data, was "ndbc-api-0.23.7.31.tar", last modified: Tue Aug  1 05:31:21 2023, max compression
```

## Comparing `ndbc-api-0.0.1.9.4.tar` & `ndbc-api-0.23.7.31.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:15.312001 ndbc-api-0.0.1.9.4/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1069 2022-06-04 17:46:07.000000 ndbc-api-0.0.1.9.4/LICENSE
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      100 2022-09-04 04:37:56.000000 ndbc-api-0.0.1.9.4/MANIFEST.in
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)    10739 2023-01-08 07:09:15.312996 ndbc-api-0.0.1.9.4/PKG-INFO
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     8111 2022-10-03 05:29:03.000000 ndbc-api-0.0.1.9.4/README.md
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:14.929994 ndbc-api-0.0.1.9.4/ndbc_api/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      112 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/__init__.py
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:14.979997 ndbc-api-0.0.1.9.4/ndbc_api/api/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2022-06-05 13:54:43.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/__init__.py
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:15.016996 ndbc-api-0.0.1.9.4/ndbc_api/api/handlers/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2022-08-03 23:38:02.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/handlers/__init__.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)       30 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/handlers/_base.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)    11910 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/handlers/data.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     4873 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/handlers/stations.py
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:15.155997 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2022-07-30 23:18:38.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/__init__.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     3357 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/_base.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      625 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/_html.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1822 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/_station.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     2620 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/adcp.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      454 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/cwind.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      404 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/ocean.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      463 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/spec.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1152 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/station_historical.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1686 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/station_metadata.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      938 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/station_realtime.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1045 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/stations.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      456 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/stdmet.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      494 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/supl.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1415 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swden.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1410 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swdir.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1469 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swdir2.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1408 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swr1.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1408 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swr2.py
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:15.272996 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2022-07-30 23:18:25.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/__init__.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     4154 2023-01-08 05:43:45.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/_base.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      152 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/_core.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      517 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/adcp.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      522 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/cwind.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      522 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/ocean.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      484 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/spec.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      306 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/station_historical.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      285 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/station_metadata.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      307 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/station_realtime.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      238 2023-01-07 20:48:08.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/stations.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      491 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/stdmet.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      517 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/supl.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      522 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swden.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      522 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swdir.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      527 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swdir2.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      517 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swr1.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      517 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swr2.py
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:15.278996 ndbc-api-0.0.1.9.4/ndbc_api/config/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      988 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/config/__init__.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      810 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/exceptions.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)    20865 2022-09-19 17:20:00.000000 ndbc-api-0.0.1.9.4/ndbc_api/ndbc_api.py
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:15.306999 ndbc-api-0.0.1.9.4/ndbc_api/utilities/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2022-06-04 17:54:09.000000 ndbc-api-0.0.1.9.4/ndbc_api/utilities/__init__.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1538 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/utilities/req_cache.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     8337 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/utilities/req_handler.py
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      337 2022-09-19 17:20:01.000000 ndbc-api-0.0.1.9.4/ndbc_api/utilities/singleton.py
-drwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        0 2023-01-08 07:09:14.972996 ndbc-api-0.0.1.9.4/ndbc_api.egg-info/
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)    10739 2023-01-08 07:09:14.000000 ndbc-api-0.0.1.9.4/ndbc_api.egg-info/PKG-INFO
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1790 2023-01-08 07:09:14.000000 ndbc-api-0.0.1.9.4/ndbc_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        1 2023-01-08 07:09:14.000000 ndbc-api-0.0.1.9.4/ndbc_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)       29 2023-01-08 07:09:14.000000 ndbc-api-0.0.1.9.4/ndbc_api.egg-info/requires.txt
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)        9 2023-01-08 07:09:14.000000 ndbc-api-0.0.1.9.4/ndbc_api.egg-info/top_level.txt
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)      245 2023-01-08 07:09:15.328996 ndbc-api-0.0.1.9.4/setup.cfg
--rwxrwxrwx   0 cjellen   (1000) cjellen   (1000)     1236 2023-01-08 07:09:08.000000 ndbc-api-0.0.1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.990890 ndbc-api-0.23.7.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-08-01 05:31:21.990890 ndbc-api-0.23.7.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.986890 ndbc-api-0.23.7.31/ndbc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.986890 ndbc-api-0.23.7.31/ndbc_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.986890 ndbc-api-0.23.7.31/ndbc_api/api/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/handlers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/handlers/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/handlers/stations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.986890 ndbc-api-0.23.7.31/ndbc_api/api/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/adcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/cwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/station_historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/station_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/station_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/stdmet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/supl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/swden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/swdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/swdir2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/swr1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/parsers/swr2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.990890 ndbc-api-0.23.7.31/ndbc_api/api/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/adcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/cwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/station_historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/station_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/station_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/stdmet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/supl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/swden.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/swdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/swdir2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/swr1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/api/requests/swr2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.990890 ndbc-api-0.23.7.31/ndbc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20892 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/ndbc_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.990890 ndbc-api-0.23.7.31/ndbc_api/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/utilities/req_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/utilities/req_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/ndbc_api/utilities/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:31:21.986890 ndbc-api-0.23.7.31/ndbc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-08-01 05:31:21.000000 ndbc-api-0.23.7.31/ndbc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-01 05:31:21.000000 ndbc-api-0.23.7.31/ndbc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:31:21.000000 ndbc-api-0.23.7.31/ndbc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 05:31:21.000000 ndbc-api-0.23.7.31/ndbc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 05:31:21.000000 ndbc-api-0.23.7.31/ndbc_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 05:31:21.990890 ndbc-api-0.23.7.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-01 05:31:11.000000 ndbc-api-0.23.7.31/setup.py
```

### Comparing `ndbc-api-0.0.1.9.4/LICENSE` & `ndbc-api-0.23.7.31/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Chris Jellen
+Copyright (c) 2023 Chris Jellen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ndbc-api-0.0.1.9.4/PKG-INFO` & `ndbc-api-0.23.7.31/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,241 +1,240 @@
 Metadata-Version: 2.1
 Name: ndbc-api
-Version: 0.0.1.9.4
+Version: 0.23.7.31
 Summary: A Python API for the National Data Buoy Center.
 Home-page: https://github.com/cdjellen/ndbc-api
+Download-URL: https://github.com/cdjellen/ndbc-api/tarball/main
 Author: Chris Jellen
-Author-email: contact.cdjellen@gmail.com
+Author-email: cdjellen@gmail.com
 License: MIT
-Download-URL: https://github.com/cdjellen/ndbc-api/tarball/main
-Description: <div align="center">
-            <h2>NDBC API</h2>
-        </div>
-        
-        
-        [![Coverage Status](https://coveralls.io/repos/github/CDJellen/ndbc-api/badge.svg?branch=main)](https://coveralls.io/github/CDJellen/ndbc-api?branch=main)
-        [![PyPI](https://img.shields.io/pypi/v/ndbc-api)](https://pypi.org/project/ndbc-api/#history)
-        [![PyPI - Status](https://img.shields.io/pypi/status/ndbc-api)](https://pypi.org/project/ndbc-api/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ndbc-api)](https://pypi.org/project/ndbc-api/)
-        [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/cdjellen/)
-        [![GitHub](https://img.shields.io/github/license/cdjellen/ndbc-api)](https://github.com/cdjellen/ndbc-api/blob/main/LICENSE)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/ndbc-api)](https://pypi.org/project/ndbc-api/)
-        
-        
-        <div align="center">
-            <h3>A Python API for the National Data Buoy Center</h3>
-        </div>
-        
-        
-        The National Oceanic and Atmospheric Association's National Data Buoy Center maintains marine monitoring and observation stations around the world[^1]. These stations report atmospheric, oceanographic, and other meterological data at regular intervals to the NDBC. Measurements are made available over HTTP through the NDBC's data service.
-        
-        The ndbc-api is a python library that makes this data more widely accessible.
-        
-        The ndbc-api is primarily built to parse whitespace-delimited oceanographic and atmospheric data distributed as text files for available time ranges, on a station-by-station basis[^2]. Measurements are typically distributed as `utf-8` encoded, station-by-station, fixed-period text files. More information on the measurements and methodology are available [on the NDBC website](https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf)[^3].
-        
-        Please read the documentation for more information:
-        https://ndbc-api.readthedocs.io
-        
-        [^1]: https://www.ndbc.noaa.gov/
-        [^2]: https://www.ndbc.noaa.gov/obs.shtml
-        [^3]: https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf
-        
-        
-        #### Installation
-        The `ndbc-api` can be installed via PIP:
-        
-        ```sh
-        pip install ndbc-api
-        ```
-        
-        #### Requirements
-        The `ndbc-api` has been tested on Python 3.6, 3.7, 3.8, 3.9, and 3.10. Python 2 support is not currently planned, but could be implemented based on the needs of the atmospheric research community.
-        
-        The API uses synchronous HTTP requests to compile data matching the user-supplied parameters. The `ndbc-api` package depends on:
-        * requests>=2.10.0
-        * pandas
-        * bs4
-        * html5lib>=1.1
-        
-        ##### Development
-        If you would like to contribute to the growth and maintenance of the `ndbc-api`, please feel free to open a PR with tests covering your changes. The tests leverage `pytest` and depend on the above requirements, as well as:
-        * coveralls
-        * httpretty
-        * pytest
-        * pytest-cov
-        * pyyaml
-        * pyarrow
-        
-        Breaking changes will be considered, especially in the current `alpha` state of the package on `PyPi`.  As the API further matures, breaking changes will only be considered with new major versions (e.g. `N.0.0`).
-        
-        #### Example
-        
-        The `ndbc-api` exposes public methods through the `NdbcApi` class.
-        
-        ```python3
-        from ndbc_api import NdbcApi
-        
-        api = NdbcApi()
-        ```
-        
-        The `api` is a singleton, such that the underlying `RequestHandler` and NDBC station-level `RequestCache`s are shared between instances. Both the singleton metaclass and `RequestHandler` are implemented to reduce the likelihood of repeat requests to the NDBC's data service, and to converse NDBC resources. This is balanced by a station-level `cache_limit`, implemented as an LRU cache, which seeks to respect user resources.
-        
-        Data made available by the NDBC falls into two broad catagories.
-        
-        1. Station metadata
-        2. Station measurements
-        
-        The `api` supports a range of public methods for accessing data from the above catagories.
-        
-        ##### Station metadata
-        
-        The `api` has five key public methods for accessing NDBC metadata.
-        
-        1. The `stations` method, which returns all NDBC stations.
-        2. The `nearest_staion` method, which returns the station ID of the nearest station.
-        3. The `station` method, which returns station metadata from a given station ID.
-        4. The `available_realtime` method, which returns hyperlinks and measurement names for realtime measurements captured by a given station.
-        5. The `available_historical` method, which returns hyperlinks and measurement names for historical measurements captured by a given station.
-        
-        ###### `stations`
-        
-        ```python3
-        # get all stations and some metadata as a Pandas DataFrame
-        stations_df = api.stations()
-        # parse the response as a dictionary
-        stations_dict = api.stations(as_df=False)
-        ```
-        
-        ###### `nearest_station`
-        
-        ```python3
-        # specify desired latitude and longitude
-        lat = '38.88N'
-        lon = '76.43W'
-        
-        # find the station ID of the nearest NDBC station
-        nearest = api.nearest_station(lat=lat, lon=lon)
-        print(nearest_station)
-        ```
-        
-        ```python3
-        'tplm2'
-        ```
-        
-        ###### `station`
-        
-        ```python3
-        # get staion metadata
-        tplm2_meta = api.station(station_id='tplm2')
-        # parse the response as a Pandas DataFrame
-        tplm2_df = api.station(station_id='tplm2', as_df=True)
-        ```
-        
-        ###### `available_realtime`
-        
-        ```python3
-        # get all available realtime measurements, periods, and hyperlinks
-        tplm2_realtime = api.available_realtime(station_id='tplm2')
-        # parse the response as a Pandas DataFrame
-        tplm2_realtime_df = api.available_realtime(station_id='tplm2', as_df=True)
-        ```
-        
-        ###### `available_historical`
-        
-        ```python3
-        # get all available historical measurements, periods, and hyperlinks
-        tplm2_historical = api.available_historical(station_id='tplm2')
-        # parse the response as a Pandas DataFrame
-        tplm2_historical_df = api.available_historical(station_id='tplm2', as_df=True)
-        ```
-        
-        ##### Station measurements
-        
-        The `api` has two public method which support accessing supported NDBC station measurements.
-        
-        1. The `get_modes` method, which returns a list of supported `mode`s, coresponding to the data formats provided by the NDBC data service. 
-        
-        Note that not all stations provide the same set of measurements. The `available_realtime` and `available_historical` methods can be called on a station-by station basis to ensure a station has the desired data available, before building and executing requests with `get_data`. 
-        
-        2. The `get_data` method, which returns measurements of a given type for a given station.
-        
-        ###### `get_modes`
-        
-        ```python3
-        # get the list of supported meterological measurement modes
-        modes = api.get_modes()
-        print(modes)
-        ```
-        
-        ```python3
-        [
-            'adcp',
-            'cwind',
-            'ocean',
-            'spec',
-            'stdmet',
-            'supl',
-            'swden',
-            'swdir',
-            'swdir2,
-            'swr1',
-            'swr2'
-        ]
-        ```
-        
-        ###### `get_data`
-        
-        ```python3
-        # get all continuous wind measurements for station tplm2
-        cwind_df = api.get_data(
-            station_id='tplm2',
-            mode='cwind',
-            start_time='2020-01-01',
-            end_time='2022-09-15',
-        )
-        # return data as a dictionary
-        cwind_dict = api.get_data(
-            station_id='tplm2',
-            mode='cwind',
-            start_time='2020-01-01',
-            end_time='2022-09-15',
-            as_df=False
-        )
-        # get only the wind speed measurements
-        wspd_df = api.get_data(
-            station_id='tplm2',
-            mode='cwind',
-            start_time='2020-01-01',
-            end_time='2022-09-15',
-            as_df=True,
-            cols=['WSPD']
-        )
-        ```
-        
-        #### More Information
-        see the [documentation](https://ndbc-api.readthedocs.io/en/latest/) for more info.
-        
-        
-        #### Questions
-        If you have questions regarding the library please post them into
-        the [GitHub discussion forum](https://github.com/cdjellen/ndbc-api/discussions).
-        
-        
-        #### Contributing
-        The `ndbc-api` is actively maintained, please feel free to open a pull request if you have any suggested improvements, test coverage is strongly preferred.
-        
-        As a reminder, breaking changes will be considered, especially in the current `alpha` state of the package on `PyPi`.  As the API further matures, breaking changes will only be considered with new major versions (e.g. `N.0.0`).
-        
-        Alternatively, if you have an idea for a new capability or improvement, feel free to open a feature request issue outlining your suggestion and the ways in which it will empower the atmospheric research community.
-        
 Keywords: ndbc,python3,api,oceanography,buoy,atmospheric
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+    <h2>NDBC API</h2>
+</div>
+
+
+[![Coverage Status](https://coveralls.io/repos/github/CDJellen/ndbc-api/badge.svg?branch=main)](https://coveralls.io/github/CDJellen/ndbc-api?branch=main)
+[![PyPI](https://img.shields.io/pypi/v/ndbc-api)](https://pypi.org/project/ndbc-api/#history)
+[![PyPI - Status](https://img.shields.io/pypi/status/ndbc-api)](https://pypi.org/project/ndbc-api/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ndbc-api)](https://pypi.org/project/ndbc-api/)
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/cdjellen/)
+[![GitHub](https://img.shields.io/github/license/cdjellen/ndbc-api)](https://github.com/cdjellen/ndbc-api/blob/main/LICENSE)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ndbc-api)](https://pypi.org/project/ndbc-api/)
+
+
+<div align="center">
+    <h3>A Python API for the National Data Buoy Center</h3>
+</div>
+
+
+The National Oceanic and Atmospheric Association's National Data Buoy Center maintains marine monitoring and observation stations around the world[^1]. These stations report atmospheric, oceanographic, and other meterological data at regular intervals to the NDBC. Measurements are made available over HTTP through the NDBC's data service.
+
+The ndbc-api is a python library that makes this data more widely accessible.
+
+The ndbc-api is primarily built to parse whitespace-delimited oceanographic and atmospheric data distributed as text files for available time ranges, on a station-by-station basis[^2]. Measurements are typically distributed as `utf-8` encoded, station-by-station, fixed-period text files. More information on the measurements and methodology are available [on the NDBC website](https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf)[^3].
+
+Please see [the included example notebook](/notebooks/overview.ipynb) for a more detailed walkthrough of the API's capabilities.
+
+[^1]: https://www.ndbc.noaa.gov/
+[^2]: https://www.ndbc.noaa.gov/obs.shtml
+[^3]: https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf
+
+
+#### Installation
+The `ndbc-api` can be installed via PIP:
+
+```sh
+pip install ndbc-api
+```
+
+#### Requirements
+The `ndbc-api` has been tested on Python 3.6, 3.7, 3.8, 3.9, and 3.10. Python 2 support is not currently planned, but could be implemented based on the needs of the atmospheric research community.
+
+The API uses synchronous HTTP requests to compile data matching the user-supplied parameters. The `ndbc-api` package depends on:
+* requests>=2.10.0
+* pandas
+* bs4
+* html5lib>=1.1
+
+##### Development
+If you would like to contribute to the growth and maintenance of the `ndbc-api`, please feel free to open a PR with tests covering your changes. The tests leverage `pytest` and depend on the above requirements, as well as:
+* coveralls
+* httpretty
+* pytest
+* pytest-cov
+* pyyaml
+* pyarrow
+
+Breaking changes will be considered, especially in the current `alpha` state of the package on `PyPi`.  As the API further matures, breaking changes will only be considered with new major versions (e.g. `N.0.0`).
+
+#### Example
+
+The `ndbc-api` exposes public methods through the `NdbcApi` class.
+
+```python3
+from ndbc_api import NdbcApi
+
+api = NdbcApi()
+```
+
+The `api` is a singleton, such that the underlying `RequestHandler` and NDBC station-level `RequestCache`s are shared between instances. Both the singleton metaclass and `RequestHandler` are implemented to reduce the likelihood of repeat requests to the NDBC's data service, and to converse NDBC resources. This is balanced by a station-level `cache_limit`, implemented as an LRU cache, which seeks to respect user resources.
+
+Data made available by the NDBC falls into two broad catagories.
+
+1. Station metadata
+2. Station measurements
+
+The `api` supports a range of public methods for accessing data from the above catagories.
+
+##### Station metadata
+
+The `api` has five key public methods for accessing NDBC metadata.
+
+1. The `stations` method, which returns all NDBC stations.
+2. The `nearest_staion` method, which returns the station ID of the nearest station.
+3. The `station` method, which returns station metadata from a given station ID.
+4. The `available_realtime` method, which returns hyperlinks and measurement names for realtime measurements captured by a given station.
+5. The `available_historical` method, which returns hyperlinks and measurement names for historical measurements captured by a given station.
+
+###### `stations`
+
+```python3
+# get all stations and some metadata as a Pandas DataFrame
+stations_df = api.stations()
+# parse the response as a dictionary
+stations_dict = api.stations(as_df=False)
+```
+
+###### `nearest_station`
+
+```python3
+# specify desired latitude and longitude
+lat = '38.88N'
+lon = '76.43W'
+
+# find the station ID of the nearest NDBC station
+nearest = api.nearest_station(lat=lat, lon=lon)
+print(nearest_station)
+```
+
+```python3
+'tplm2'
+```
+
+###### `station`
+
+```python3
+# get staion metadata
+tplm2_meta = api.station(station_id='tplm2')
+# parse the response as a Pandas DataFrame
+tplm2_df = api.station(station_id='tplm2', as_df=True)
+```
+
+###### `available_realtime`
+
+```python3
+# get all available realtime measurements, periods, and hyperlinks
+tplm2_realtime = api.available_realtime(station_id='tplm2')
+# parse the response as a Pandas DataFrame
+tplm2_realtime_df = api.available_realtime(station_id='tplm2', as_df=True)
+```
+
+###### `available_historical`
+
+```python3
+# get all available historical measurements, periods, and hyperlinks
+tplm2_historical = api.available_historical(station_id='tplm2')
+# parse the response as a Pandas DataFrame
+tplm2_historical_df = api.available_historical(station_id='tplm2', as_df=True)
+```
+
+##### Station measurements
+
+The `api` has two public method which support accessing supported NDBC station measurements.
+
+1. The `get_modes` method, which returns a list of supported `mode`s, coresponding to the data formats provided by the NDBC data service. 
+
+Note that not all stations provide the same set of measurements. The `available_realtime` and `available_historical` methods can be called on a station-by station basis to ensure a station has the desired data available, before building and executing requests with `get_data`. 
+
+2. The `get_data` method, which returns measurements of a given type for a given station.
+
+###### `get_modes`
+
+```python3
+# get the list of supported meterological measurement modes
+modes = api.get_modes()
+print(modes)
+```
+
+```python3
+[
+    'adcp',
+    'cwind',
+    'ocean',
+    'spec',
+    'stdmet',
+    'supl',
+    'swden',
+    'swdir',
+    'swdir2,
+    'swr1',
+    'swr2'
+]
+```
+
+###### `get_data`
+
+```python3
+# get all continuous wind measurements for station tplm2
+cwind_df = api.get_data(
+    station_id='tplm2',
+    mode='cwind',
+    start_time='2020-01-01',
+    end_time='2022-09-15',
+)
+# return data as a dictionary
+cwind_dict = api.get_data(
+    station_id='tplm2',
+    mode='cwind',
+    start_time='2020-01-01',
+    end_time='2022-09-15',
+    as_df=False
+)
+# get only the wind speed measurements
+wspd_df = api.get_data(
+    station_id='tplm2',
+    mode='cwind',
+    start_time='2020-01-01',
+    end_time='2022-09-15',
+    as_df=True,
+    cols=['WSPD']
+)
+```
+
+#### More Information
+Please see [the included example notebook](/notebooks/overview.ipynb) for a more detailed walkthrough of the API's capabilities.
+
+
+#### Questions
+If you have questions regarding the library please post them into
+the [GitHub discussion forum](https://github.com/cdjellen/ndbc-api/discussions).
+
+
+#### Contributing
+The `ndbc-api` is actively maintained, please feel free to open a pull request if you have any suggested improvements, test coverage is strongly preferred.
+
+As a reminder, breaking changes will be considered, especially in the current `alpha` state of the package on `PyPi`.  As the API further matures, breaking changes will only be considered with new major versions (e.g. `N.0.0`).
+
+Alternatively, if you have an idea for a new capability or improvement, feel free to open a feature request issue outlining your suggestion and the ways in which it will empower the atmospheric research community.
```

### Comparing `ndbc-api-0.0.1.9.4/README.md` & `ndbc-api-0.23.7.31/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 The National Oceanic and Atmospheric Association's National Data Buoy Center maintains marine monitoring and observation stations around the world[^1]. These stations report atmospheric, oceanographic, and other meterological data at regular intervals to the NDBC. Measurements are made available over HTTP through the NDBC's data service.
 
 The ndbc-api is a python library that makes this data more widely accessible.
 
 The ndbc-api is primarily built to parse whitespace-delimited oceanographic and atmospheric data distributed as text files for available time ranges, on a station-by-station basis[^2]. Measurements are typically distributed as `utf-8` encoded, station-by-station, fixed-period text files. More information on the measurements and methodology are available [on the NDBC website](https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf)[^3].
 
-Please read the documentation for more information:
-https://ndbc-api.readthedocs.io
+Please see [the included example notebook](/notebooks/overview.ipynb) for a more detailed walkthrough of the API's capabilities.
 
 [^1]: https://www.ndbc.noaa.gov/
 [^2]: https://www.ndbc.noaa.gov/obs.shtml
 [^3]: https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf
 
 
 #### Installation
@@ -199,15 +198,15 @@
     end_time='2022-09-15',
     as_df=True,
     cols=['WSPD']
 )
 ```
 
 #### More Information
-see the [documentation](https://ndbc-api.readthedocs.io/en/latest/) for more info.
+Please see [the included example notebook](/notebooks/overview.ipynb) for a more detailed walkthrough of the API's capabilities.
 
 
 #### Questions
 If you have questions regarding the library please post them into
 the [GitHub discussion forum](https://github.com/cdjellen/ndbc-api/discussions).
```

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/handlers/data.py` & `ndbc-api-0.23.7.31/ndbc_api/api/handlers/data.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/handlers/stations.py` & `ndbc-api-0.23.7.31/ndbc_api/api/handlers/stations.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/_base.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from ndbc_api.exceptions import ParserException
 
 
 class BaseParser:
 
     HEADER_PREFIX = '#'
     NAN_VALUES = ['MM']
-    DATE_PARSER = lambda x: datetime.strptime(x, '%Y %m %d %H %M')
+    DATE_PARSER = '%Y %m %d %H %M'
     PARSE_DATES = ['YY', 'MM', 'DD', 'hh', 'mm']
-    INDEX_COL = None
+    INDEX_COL = False
     REVERT_COL_NAMES = []
 
     @classmethod
     def df_from_responses(cls,
                           responses: List[dict],
                           use_timestamp: bool = True) -> pd.DataFrame:
         components = []
@@ -43,32 +43,37 @@
         if not data:
             return pd.DataFrame()
         # check that parsed names match parsed values or revert
         if len([v.strip() for v in data[0].split(' ') if v]) != len(names):
             names = cls.REVERT_COL_NAMES
         if '(' in data[0]:
             data = cls._clean_data(data)
-        # check whether to parse dates
-        if use_timestamp:
-            parse_dates = {'timestamp': cls.PARSE_DATES}
-        else:
-            parse_dates = False
+        
         try:
+            parse_dates = False
+            date_format = None
+            if use_timestamp:
+                parse_dates = [cls.PARSE_DATES]
+                date_format = cls.DATE_PARSER
             df = pd.read_csv(
                 StringIO('\n'.join(data)),
                 names=names,
                 delim_whitespace=True,
                 na_values=cls.NAN_VALUES,
-                parse_dates=parse_dates,
-                date_parser=cls.DATE_PARSER,
                 index_col=cls.INDEX_COL,
+                parse_dates=parse_dates,
+                date_format=date_format,
             )
+            if use_timestamp:
+                df.index.name = 'timestamp'
+            
         except (NotImplementedError, TypeError, ValueError) as e:
             return pd.DataFrame()
-
+        
+        # check whether to parse dates
         return df
 
     @staticmethod
     def _parse_body(body: str) -> Tuple[List[str], List[str]]:
         buf = StringIO(body)
         data = []
         header = []
```

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/_html.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/_html.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/_station.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/_station.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/adcp.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/adcp.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/station_historical.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/station_historical.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/station_metadata.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/station_metadata.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/station_realtime.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/station_realtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 class RealtimeParser(StationParser):
 
     @classmethod
     def available_measurements(cls, response: dict) -> dict:
         if response.get('status') == 200:
             soup = bs4.BeautifulSoup(response.get('body'), 'html.parser')
-            line_items = soup.find_all('li')
+            items = soup.find('section', {"class": "data"})
+            line_items = items.find_all('li')
             return cls._build_available_measurements(line_items=line_items)
         else:
             return dict()
 
     @classmethod
     def _parse_list_item(cls, li: bs4.element.Tag) -> dict:
         measurement_item = dict()
```

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/stations.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/stations.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swden.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/swden.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swdir.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/swdir.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swdir2.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/swdir2.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swr1.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/swr1.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/parsers/swr2.py` & `ndbc-api-0.23.7.31/ndbc_api/api/parsers/swr2.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/_base.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/_base.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/adcp.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/adcp.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/cwind.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/cwind.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/ocean.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/ocean.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/supl.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/supl.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swden.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/swden.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swdir.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/swdir.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swdir2.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/swdir2.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swr1.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/swr1.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/api/requests/swr2.py` & `ndbc-api-0.23.7.31/ndbc_api/api/requests/swr2.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/config/__init__.py` & `ndbc-api-0.23.7.31/ndbc_api/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
     HTTP_DELAY (:int:) The delay between requests submitted to the NDBC data
         service, in milliseconds.
     HTTP_DEBUG (:bool:): Whether to log requests and responses to the NDBC API's
         log (a `logging.Logger`) as debug messages.
 """
 LOGGER_NAME = 'NDBC-API'
 DEFAULT_CACHE_LIMIT = 36
-VERIFY_HTTPS = False
+VERIFY_HTTPS = True
 HTTP_RETRY = 5
 HTTP_BACKOFF_FACTOR = 0.8
 HTTP_DELAY = 2000
 HTTP_DEBUG = True
```

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/exceptions.py` & `ndbc-api-0.23.7.31/ndbc_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/ndbc_api.py` & `ndbc-api-0.23.7.31/ndbc_api/ndbc_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,13 +467,13 @@
                     'Failed to parse column selection.') from e
         if as_df and isinstance(data, pd.DataFrame):
             return data
         elif isinstance(data, pd.DataFrame) and not as_df:
             return data.to_dict()
         elif as_df:
             try:
-                return pd.DataFrame().from_dict(data)
-            except (NotImplementedError, ValueError) as e:
+                return pd.DataFrame().from_dict(data, orient='index')
+            except (NotImplementedError, ValueError, TypeError) as e:
                 raise HandlerException(
                     'Failed to convert `pd.DataFrame` to `dict`.') from e
         else:
             return data
```

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/utilities/req_cache.py` & `ndbc-api-0.23.7.31/ndbc_api/utilities/req_cache.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api/utilities/req_handler.py` & `ndbc-api-0.23.7.31/ndbc_api/utilities/req_handler.py`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api.egg-info/PKG-INFO` & `ndbc-api-0.23.7.31/ndbc_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,241 +1,240 @@
 Metadata-Version: 2.1
 Name: ndbc-api
-Version: 0.0.1.9.4
+Version: 0.23.7.31
 Summary: A Python API for the National Data Buoy Center.
 Home-page: https://github.com/cdjellen/ndbc-api
+Download-URL: https://github.com/cdjellen/ndbc-api/tarball/main
 Author: Chris Jellen
-Author-email: contact.cdjellen@gmail.com
+Author-email: cdjellen@gmail.com
 License: MIT
-Download-URL: https://github.com/cdjellen/ndbc-api/tarball/main
-Description: <div align="center">
-            <h2>NDBC API</h2>
-        </div>
-        
-        
-        [![Coverage Status](https://coveralls.io/repos/github/CDJellen/ndbc-api/badge.svg?branch=main)](https://coveralls.io/github/CDJellen/ndbc-api?branch=main)
-        [![PyPI](https://img.shields.io/pypi/v/ndbc-api)](https://pypi.org/project/ndbc-api/#history)
-        [![PyPI - Status](https://img.shields.io/pypi/status/ndbc-api)](https://pypi.org/project/ndbc-api/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ndbc-api)](https://pypi.org/project/ndbc-api/)
-        [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/cdjellen/)
-        [![GitHub](https://img.shields.io/github/license/cdjellen/ndbc-api)](https://github.com/cdjellen/ndbc-api/blob/main/LICENSE)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/ndbc-api)](https://pypi.org/project/ndbc-api/)
-        
-        
-        <div align="center">
-            <h3>A Python API for the National Data Buoy Center</h3>
-        </div>
-        
-        
-        The National Oceanic and Atmospheric Association's National Data Buoy Center maintains marine monitoring and observation stations around the world[^1]. These stations report atmospheric, oceanographic, and other meterological data at regular intervals to the NDBC. Measurements are made available over HTTP through the NDBC's data service.
-        
-        The ndbc-api is a python library that makes this data more widely accessible.
-        
-        The ndbc-api is primarily built to parse whitespace-delimited oceanographic and atmospheric data distributed as text files for available time ranges, on a station-by-station basis[^2]. Measurements are typically distributed as `utf-8` encoded, station-by-station, fixed-period text files. More information on the measurements and methodology are available [on the NDBC website](https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf)[^3].
-        
-        Please read the documentation for more information:
-        https://ndbc-api.readthedocs.io
-        
-        [^1]: https://www.ndbc.noaa.gov/
-        [^2]: https://www.ndbc.noaa.gov/obs.shtml
-        [^3]: https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf
-        
-        
-        #### Installation
-        The `ndbc-api` can be installed via PIP:
-        
-        ```sh
-        pip install ndbc-api
-        ```
-        
-        #### Requirements
-        The `ndbc-api` has been tested on Python 3.6, 3.7, 3.8, 3.9, and 3.10. Python 2 support is not currently planned, but could be implemented based on the needs of the atmospheric research community.
-        
-        The API uses synchronous HTTP requests to compile data matching the user-supplied parameters. The `ndbc-api` package depends on:
-        * requests>=2.10.0
-        * pandas
-        * bs4
-        * html5lib>=1.1
-        
-        ##### Development
-        If you would like to contribute to the growth and maintenance of the `ndbc-api`, please feel free to open a PR with tests covering your changes. The tests leverage `pytest` and depend on the above requirements, as well as:
-        * coveralls
-        * httpretty
-        * pytest
-        * pytest-cov
-        * pyyaml
-        * pyarrow
-        
-        Breaking changes will be considered, especially in the current `alpha` state of the package on `PyPi`.  As the API further matures, breaking changes will only be considered with new major versions (e.g. `N.0.0`).
-        
-        #### Example
-        
-        The `ndbc-api` exposes public methods through the `NdbcApi` class.
-        
-        ```python3
-        from ndbc_api import NdbcApi
-        
-        api = NdbcApi()
-        ```
-        
-        The `api` is a singleton, such that the underlying `RequestHandler` and NDBC station-level `RequestCache`s are shared between instances. Both the singleton metaclass and `RequestHandler` are implemented to reduce the likelihood of repeat requests to the NDBC's data service, and to converse NDBC resources. This is balanced by a station-level `cache_limit`, implemented as an LRU cache, which seeks to respect user resources.
-        
-        Data made available by the NDBC falls into two broad catagories.
-        
-        1. Station metadata
-        2. Station measurements
-        
-        The `api` supports a range of public methods for accessing data from the above catagories.
-        
-        ##### Station metadata
-        
-        The `api` has five key public methods for accessing NDBC metadata.
-        
-        1. The `stations` method, which returns all NDBC stations.
-        2. The `nearest_staion` method, which returns the station ID of the nearest station.
-        3. The `station` method, which returns station metadata from a given station ID.
-        4. The `available_realtime` method, which returns hyperlinks and measurement names for realtime measurements captured by a given station.
-        5. The `available_historical` method, which returns hyperlinks and measurement names for historical measurements captured by a given station.
-        
-        ###### `stations`
-        
-        ```python3
-        # get all stations and some metadata as a Pandas DataFrame
-        stations_df = api.stations()
-        # parse the response as a dictionary
-        stations_dict = api.stations(as_df=False)
-        ```
-        
-        ###### `nearest_station`
-        
-        ```python3
-        # specify desired latitude and longitude
-        lat = '38.88N'
-        lon = '76.43W'
-        
-        # find the station ID of the nearest NDBC station
-        nearest = api.nearest_station(lat=lat, lon=lon)
-        print(nearest_station)
-        ```
-        
-        ```python3
-        'tplm2'
-        ```
-        
-        ###### `station`
-        
-        ```python3
-        # get staion metadata
-        tplm2_meta = api.station(station_id='tplm2')
-        # parse the response as a Pandas DataFrame
-        tplm2_df = api.station(station_id='tplm2', as_df=True)
-        ```
-        
-        ###### `available_realtime`
-        
-        ```python3
-        # get all available realtime measurements, periods, and hyperlinks
-        tplm2_realtime = api.available_realtime(station_id='tplm2')
-        # parse the response as a Pandas DataFrame
-        tplm2_realtime_df = api.available_realtime(station_id='tplm2', as_df=True)
-        ```
-        
-        ###### `available_historical`
-        
-        ```python3
-        # get all available historical measurements, periods, and hyperlinks
-        tplm2_historical = api.available_historical(station_id='tplm2')
-        # parse the response as a Pandas DataFrame
-        tplm2_historical_df = api.available_historical(station_id='tplm2', as_df=True)
-        ```
-        
-        ##### Station measurements
-        
-        The `api` has two public method which support accessing supported NDBC station measurements.
-        
-        1. The `get_modes` method, which returns a list of supported `mode`s, coresponding to the data formats provided by the NDBC data service. 
-        
-        Note that not all stations provide the same set of measurements. The `available_realtime` and `available_historical` methods can be called on a station-by station basis to ensure a station has the desired data available, before building and executing requests with `get_data`. 
-        
-        2. The `get_data` method, which returns measurements of a given type for a given station.
-        
-        ###### `get_modes`
-        
-        ```python3
-        # get the list of supported meterological measurement modes
-        modes = api.get_modes()
-        print(modes)
-        ```
-        
-        ```python3
-        [
-            'adcp',
-            'cwind',
-            'ocean',
-            'spec',
-            'stdmet',
-            'supl',
-            'swden',
-            'swdir',
-            'swdir2,
-            'swr1',
-            'swr2'
-        ]
-        ```
-        
-        ###### `get_data`
-        
-        ```python3
-        # get all continuous wind measurements for station tplm2
-        cwind_df = api.get_data(
-            station_id='tplm2',
-            mode='cwind',
-            start_time='2020-01-01',
-            end_time='2022-09-15',
-        )
-        # return data as a dictionary
-        cwind_dict = api.get_data(
-            station_id='tplm2',
-            mode='cwind',
-            start_time='2020-01-01',
-            end_time='2022-09-15',
-            as_df=False
-        )
-        # get only the wind speed measurements
-        wspd_df = api.get_data(
-            station_id='tplm2',
-            mode='cwind',
-            start_time='2020-01-01',
-            end_time='2022-09-15',
-            as_df=True,
-            cols=['WSPD']
-        )
-        ```
-        
-        #### More Information
-        see the [documentation](https://ndbc-api.readthedocs.io/en/latest/) for more info.
-        
-        
-        #### Questions
-        If you have questions regarding the library please post them into
-        the [GitHub discussion forum](https://github.com/cdjellen/ndbc-api/discussions).
-        
-        
-        #### Contributing
-        The `ndbc-api` is actively maintained, please feel free to open a pull request if you have any suggested improvements, test coverage is strongly preferred.
-        
-        As a reminder, breaking changes will be considered, especially in the current `alpha` state of the package on `PyPi`.  As the API further matures, breaking changes will only be considered with new major versions (e.g. `N.0.0`).
-        
-        Alternatively, if you have an idea for a new capability or improvement, feel free to open a feature request issue outlining your suggestion and the ways in which it will empower the atmospheric research community.
-        
 Keywords: ndbc,python3,api,oceanography,buoy,atmospheric
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+    <h2>NDBC API</h2>
+</div>
+
+
+[![Coverage Status](https://coveralls.io/repos/github/CDJellen/ndbc-api/badge.svg?branch=main)](https://coveralls.io/github/CDJellen/ndbc-api?branch=main)
+[![PyPI](https://img.shields.io/pypi/v/ndbc-api)](https://pypi.org/project/ndbc-api/#history)
+[![PyPI - Status](https://img.shields.io/pypi/status/ndbc-api)](https://pypi.org/project/ndbc-api/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ndbc-api)](https://pypi.org/project/ndbc-api/)
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/cdjellen/)
+[![GitHub](https://img.shields.io/github/license/cdjellen/ndbc-api)](https://github.com/cdjellen/ndbc-api/blob/main/LICENSE)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ndbc-api)](https://pypi.org/project/ndbc-api/)
+
+
+<div align="center">
+    <h3>A Python API for the National Data Buoy Center</h3>
+</div>
+
+
+The National Oceanic and Atmospheric Association's National Data Buoy Center maintains marine monitoring and observation stations around the world[^1]. These stations report atmospheric, oceanographic, and other meterological data at regular intervals to the NDBC. Measurements are made available over HTTP through the NDBC's data service.
+
+The ndbc-api is a python library that makes this data more widely accessible.
+
+The ndbc-api is primarily built to parse whitespace-delimited oceanographic and atmospheric data distributed as text files for available time ranges, on a station-by-station basis[^2]. Measurements are typically distributed as `utf-8` encoded, station-by-station, fixed-period text files. More information on the measurements and methodology are available [on the NDBC website](https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf)[^3].
+
+Please see [the included example notebook](/notebooks/overview.ipynb) for a more detailed walkthrough of the API's capabilities.
+
+[^1]: https://www.ndbc.noaa.gov/
+[^2]: https://www.ndbc.noaa.gov/obs.shtml
+[^3]: https://www.ndbc.noaa.gov/docs/ndbc_web_data_guide.pdf
+
+
+#### Installation
+The `ndbc-api` can be installed via PIP:
+
+```sh
+pip install ndbc-api
+```
+
+#### Requirements
+The `ndbc-api` has been tested on Python 3.6, 3.7, 3.8, 3.9, and 3.10. Python 2 support is not currently planned, but could be implemented based on the needs of the atmospheric research community.
+
+The API uses synchronous HTTP requests to compile data matching the user-supplied parameters. The `ndbc-api` package depends on:
+* requests>=2.10.0
+* pandas
+* bs4
+* html5lib>=1.1
+
+##### Development
+If you would like to contribute to the growth and maintenance of the `ndbc-api`, please feel free to open a PR with tests covering your changes. The tests leverage `pytest` and depend on the above requirements, as well as:
+* coveralls
+* httpretty
+* pytest
+* pytest-cov
+* pyyaml
+* pyarrow
+
+Breaking changes will be considered, especially in the current `alpha` state of the package on `PyPi`.  As the API further matures, breaking changes will only be considered with new major versions (e.g. `N.0.0`).
+
+#### Example
+
+The `ndbc-api` exposes public methods through the `NdbcApi` class.
+
+```python3
+from ndbc_api import NdbcApi
+
+api = NdbcApi()
+```
+
+The `api` is a singleton, such that the underlying `RequestHandler` and NDBC station-level `RequestCache`s are shared between instances. Both the singleton metaclass and `RequestHandler` are implemented to reduce the likelihood of repeat requests to the NDBC's data service, and to converse NDBC resources. This is balanced by a station-level `cache_limit`, implemented as an LRU cache, which seeks to respect user resources.
+
+Data made available by the NDBC falls into two broad catagories.
+
+1. Station metadata
+2. Station measurements
+
+The `api` supports a range of public methods for accessing data from the above catagories.
+
+##### Station metadata
+
+The `api` has five key public methods for accessing NDBC metadata.
+
+1. The `stations` method, which returns all NDBC stations.
+2. The `nearest_staion` method, which returns the station ID of the nearest station.
+3. The `station` method, which returns station metadata from a given station ID.
+4. The `available_realtime` method, which returns hyperlinks and measurement names for realtime measurements captured by a given station.
+5. The `available_historical` method, which returns hyperlinks and measurement names for historical measurements captured by a given station.
+
+###### `stations`
+
+```python3
+# get all stations and some metadata as a Pandas DataFrame
+stations_df = api.stations()
+# parse the response as a dictionary
+stations_dict = api.stations(as_df=False)
+```
+
+###### `nearest_station`
+
+```python3
+# specify desired latitude and longitude
+lat = '38.88N'
+lon = '76.43W'
+
+# find the station ID of the nearest NDBC station
+nearest = api.nearest_station(lat=lat, lon=lon)
+print(nearest_station)
+```
+
+```python3
+'tplm2'
+```
+
+###### `station`
+
+```python3
+# get staion metadata
+tplm2_meta = api.station(station_id='tplm2')
+# parse the response as a Pandas DataFrame
+tplm2_df = api.station(station_id='tplm2', as_df=True)
+```
+
+###### `available_realtime`
+
+```python3
+# get all available realtime measurements, periods, and hyperlinks
+tplm2_realtime = api.available_realtime(station_id='tplm2')
+# parse the response as a Pandas DataFrame
+tplm2_realtime_df = api.available_realtime(station_id='tplm2', as_df=True)
+```
+
+###### `available_historical`
+
+```python3
+# get all available historical measurements, periods, and hyperlinks
+tplm2_historical = api.available_historical(station_id='tplm2')
+# parse the response as a Pandas DataFrame
+tplm2_historical_df = api.available_historical(station_id='tplm2', as_df=True)
+```
+
+##### Station measurements
+
+The `api` has two public method which support accessing supported NDBC station measurements.
+
+1. The `get_modes` method, which returns a list of supported `mode`s, coresponding to the data formats provided by the NDBC data service. 
+
+Note that not all stations provide the same set of measurements. The `available_realtime` and `available_historical` methods can be called on a station-by station basis to ensure a station has the desired data available, before building and executing requests with `get_data`. 
+
+2. The `get_data` method, which returns measurements of a given type for a given station.
+
+###### `get_modes`
+
+```python3
+# get the list of supported meterological measurement modes
+modes = api.get_modes()
+print(modes)
+```
+
+```python3
+[
+    'adcp',
+    'cwind',
+    'ocean',
+    'spec',
+    'stdmet',
+    'supl',
+    'swden',
+    'swdir',
+    'swdir2,
+    'swr1',
+    'swr2'
+]
+```
+
+###### `get_data`
+
+```python3
+# get all continuous wind measurements for station tplm2
+cwind_df = api.get_data(
+    station_id='tplm2',
+    mode='cwind',
+    start_time='2020-01-01',
+    end_time='2022-09-15',
+)
+# return data as a dictionary
+cwind_dict = api.get_data(
+    station_id='tplm2',
+    mode='cwind',
+    start_time='2020-01-01',
+    end_time='2022-09-15',
+    as_df=False
+)
+# get only the wind speed measurements
+wspd_df = api.get_data(
+    station_id='tplm2',
+    mode='cwind',
+    start_time='2020-01-01',
+    end_time='2022-09-15',
+    as_df=True,
+    cols=['WSPD']
+)
+```
+
+#### More Information
+Please see [the included example notebook](/notebooks/overview.ipynb) for a more detailed walkthrough of the API's capabilities.
+
+
+#### Questions
+If you have questions regarding the library please post them into
+the [GitHub discussion forum](https://github.com/cdjellen/ndbc-api/discussions).
+
+
+#### Contributing
+The `ndbc-api` is actively maintained, please feel free to open a pull request if you have any suggested improvements, test coverage is strongly preferred.
+
+As a reminder, breaking changes will be considered, especially in the current `alpha` state of the package on `PyPi`.  As the API further matures, breaking changes will only be considered with new major versions (e.g. `N.0.0`).
+
+Alternatively, if you have an idea for a new capability or improvement, feel free to open a feature request issue outlining your suggestion and the ways in which it will empower the atmospheric research community.
```

### Comparing `ndbc-api-0.0.1.9.4/ndbc_api.egg-info/SOURCES.txt` & `ndbc-api-0.23.7.31/ndbc_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ndbc-api-0.0.1.9.4/setup.py` & `ndbc-api-0.23.7.31/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='ndbc-api',
     packages=setuptools.find_packages(exclude=['*tests*']),
-    version='0.0.1.9.4',
+    version='0.23.7.31',
     license='MIT',
     description='A Python API for the National Data Buoy Center.',
     author='Chris Jellen',
-    author_email='contact.cdjellen@gmail.com',
+    author_email='cdjellen@gmail.com',
     url='https://github.com/cdjellen/ndbc-api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     download_url='https://github.com/cdjellen/ndbc-api/tarball/main',
     keywords=['ndbc', 'python3', 'api', 'oceanography', 'buoy', 'atmospheric'],
     install_requires=['requests', 'pandas', 'bs4', 'html5lib'],
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

