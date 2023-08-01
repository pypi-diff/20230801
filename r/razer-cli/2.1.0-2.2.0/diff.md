# Comparing `tmp/razer-cli-2.1.0.tar.gz` & `tmp/razer-cli-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "razer-cli-2.1.0.tar", last modified: Fri Jul 16 17:11:53 2021, max compression
+gzip compressed data, was "razer-cli-2.2.0.tar", last modified: Tue Aug  1 05:55:36 2023, max compression
```

## Comparing `razer-cli-2.1.0.tar` & `razer-cli-2.2.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.899592 razer-cli-2.1.0/
--rw-r--r--   0 me        (1000) me        (1000)    35149 2019-03-13 15:54:55.000000 razer-cli-2.1.0/LICENSE
--rw-r--r--   0 me        (1000) me        (1000)       50 2021-02-12 14:33:30.000000 razer-cli-2.1.0/MANIFEST.in
--rw-r--r--   0 me        (1000) me        (1000)     8137 2021-07-16 17:11:53.899592 razer-cli-2.1.0/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     7631 2021-06-03 07:58:41.000000 razer-cli-2.1.0/README.md
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.896259 razer-cli-2.1.0/razer_cli/
--rw-r--r--   0 me        (1000) me        (1000)        0 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/__init__.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.896259 razer-cli-2.1.0/razer_cli/razer_cli/
--rw-r--r--   0 me        (1000) me        (1000)        0 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/__init__.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.899592 razer-cli-2.1.0/razer_cli/razer_cli/handler/
--rw-r--r--   0 me        (1000) me        (1000)        0 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/handler/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     1066 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/handler/brightness_handler.py
--rw-r--r--   0 me        (1000) me        (1000)     1156 2021-07-16 17:08:10.000000 razer-cli-2.1.0/razer_cli/razer_cli/handler/color_effect_handler.py
--rw-r--r--   0 me        (1000) me        (1000)      489 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/handler/handler.py
--rw-r--r--   0 me        (1000) me        (1000)      606 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/handler/version_handler.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.899592 razer-cli-2.1.0/razer_cli/razer_cli/lister/
--rw-r--r--   0 me        (1000) me        (1000)        0 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/lister/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     6694 2021-06-03 08:16:40.000000 razer-cli-2.1.0/razer_cli/razer_cli/lister/device_lister.py
--rw-r--r--   0 me        (1000) me        (1000)      328 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/lister/lister.py
--rwxr-xr-x   0 me        (1000) me        (1000)      800 2021-07-16 17:10:41.000000 razer-cli-2.1.0/razer_cli/razer_cli/main.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.899592 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/
--rw-r--r--   0 me        (1000) me        (1000)      243 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/automatic
--rw-r--r--   0 me        (1000) me        (1000)      293 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/battery
--rw-r--r--   0 me        (1000) me        (1000)      466 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/brightness
--rw-r--r--   0 me        (1000) me        (1000)      622 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/color
--rw-r--r--   0 me        (1000) me        (1000)      173 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/device
--rw-r--r--   0 me        (1000) me        (1000)      249 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/dpi
--rw-r--r--   0 me        (1000) me        (1000)     1973 2021-07-16 17:08:10.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/effect
--rw-r--r--   0 me        (1000) me        (1000)     2537 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/example
--rw-r--r--   0 me        (1000) me        (1000)      306 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/list_devices
--rw-r--r--   0 me        (1000) me        (1000)      166 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/poll
--rw-r--r--   0 me        (1000) me        (1000)      685 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/man_pages/zone
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.899592 razer-cli-2.1.0/razer_cli/razer_cli/parser/
--rw-r--r--   0 me        (1000) me        (1000)        0 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/parser/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     3372 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/parser/argument_parser.py
--rw-r--r--   0 me        (1000) me        (1000)     2173 2021-07-16 17:08:10.000000 razer-cli-2.1.0/razer_cli/razer_cli/parser/color_parser.py
--rw-r--r--   0 me        (1000) me        (1000)      372 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/parser/zone_parser.py
--rw-r--r--   0 me        (1000) me        (1000)     3487 2021-06-04 17:13:13.000000 razer-cli-2.1.0/razer_cli/razer_cli/rc.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.899592 razer-cli-2.1.0/razer_cli/razer_cli/setter/
--rw-r--r--   0 me        (1000) me        (1000)        0 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/setter/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     2160 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/setter/battery_setter.py
--rw-r--r--   0 me        (1000) me        (1000)     2541 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/setter/brightness_setter.py
--rw-r--r--   0 me        (1000) me        (1000)    14099 2021-07-16 17:08:10.000000 razer-cli-2.1.0/razer_cli/razer_cli/setter/color_effect_setter.py
--rw-r--r--   0 me        (1000) me        (1000)     1790 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/setter/dpi_setter.py
--rw-r--r--   0 me        (1000) me        (1000)     1484 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/setter/poll_rate_setter.py
--rw-r--r--   0 me        (1000) me        (1000)      346 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/setter/resetter.py
--rw-r--r--   0 me        (1000) me        (1000)      337 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/razer_cli/setter/setter.py
--rw-r--r--   0 me        (1000) me        (1000)     1255 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/razer_cli/settings.py
--rw-r--r--   0 me        (1000) me        (1000)     9265 2021-07-16 17:08:10.000000 razer-cli-2.1.0/razer_cli/razer_cli/util.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.899592 razer-cli-2.1.0/razer_cli/tests/
--rw-r--r--   0 me        (1000) me        (1000)        0 2021-02-12 14:33:30.000000 razer-cli-2.1.0/razer_cli/tests/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      626 2021-02-15 17:37:21.000000 razer-cli-2.1.0/razer_cli/tests/test_argument_parser.py
--rw-r--r--   0 me        (1000) me        (1000)     2461 2021-07-16 17:08:10.000000 razer-cli-2.1.0/razer_cli/tests/test_util.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2021-07-16 17:11:53.896259 razer-cli-2.1.0/razer_cli.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     8137 2021-07-16 17:11:53.000000 razer-cli-2.1.0/razer_cli.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     1759 2021-07-16 17:11:53.000000 razer-cli-2.1.0/razer_cli.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2021-07-16 17:11:53.000000 razer-cli-2.1.0/razer_cli.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       61 2021-07-16 17:11:53.000000 razer-cli-2.1.0/razer_cli.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       10 2021-07-16 17:11:53.000000 razer-cli-2.1.0/razer_cli.egg-info/top_level.txt
--rw-r--r--   0 me        (1000) me        (1000)      116 2021-07-16 17:11:53.899592 razer-cli-2.1.0/setup.cfg
--rw-r--r--   0 me        (1000) me        (1000)      854 2021-07-16 17:10:35.000000 razer-cli-2.1.0/setup.py
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.213003 razer-cli-2.2.0/
+-rw-r--r--   0 lleitner   (503) staff       (20)    35149 2023-07-25 07:34:15.000000 razer-cli-2.2.0/LICENSE
+-rw-r--r--   0 lleitner   (503) staff       (20)       50 2023-07-25 07:34:15.000000 razer-cli-2.2.0/MANIFEST.in
+-rw-r--r--   0 lleitner   (503) staff       (20)     8807 2023-08-01 05:55:36.213410 razer-cli-2.2.0/PKG-INFO
+-rw-r--r--   0 lleitner   (503) staff       (20)     8338 2023-07-25 07:34:15.000000 razer-cli-2.2.0/README.md
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.179848 razer-cli-2.2.0/razer_cli/
+-rw-r--r--   0 lleitner   (503) staff       (20)        0 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/__init__.py
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.185148 razer-cli-2.2.0/razer_cli/razer_cli/
+-rw-r--r--   0 lleitner   (503) staff       (20)        0 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/__init__.py
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.189707 razer-cli-2.2.0/razer_cli/razer_cli/handler/
+-rw-r--r--   0 lleitner   (503) staff       (20)        0 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/handler/__init__.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     1066 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/handler/brightness_handler.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     1156 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/handler/color_effect_handler.py
+-rw-r--r--   0 lleitner   (503) staff       (20)      489 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/handler/handler.py
+-rw-r--r--   0 lleitner   (503) staff       (20)      606 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/handler/version_handler.py
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.191706 razer-cli-2.2.0/razer_cli/razer_cli/lister/
+-rw-r--r--   0 lleitner   (503) staff       (20)        0 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/lister/__init__.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     6822 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/lister/device_lister.py
+-rw-r--r--   0 lleitner   (503) staff       (20)      328 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/lister/lister.py
+-rwxr-xr-x   0 lleitner   (503) staff       (20)      800 2023-08-01 05:51:57.000000 razer-cli-2.2.0/razer_cli/razer_cli/main.py
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.198475 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/
+-rw-r--r--   0 lleitner   (503) staff       (20)      243 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/automatic
+-rw-r--r--   0 lleitner   (503) staff       (20)      293 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/battery
+-rw-r--r--   0 lleitner   (503) staff       (20)      466 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/brightness
+-rw-r--r--   0 lleitner   (503) staff       (20)      622 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/color
+-rw-r--r--   0 lleitner   (503) staff       (20)      173 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/device
+-rw-r--r--   0 lleitner   (503) staff       (20)      249 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/dpi
+-rw-r--r--   0 lleitner   (503) staff       (20)     1973 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/effect
+-rw-r--r--   0 lleitner   (503) staff       (20)     2537 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/example
+-rw-r--r--   0 lleitner   (503) staff       (20)      306 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/list_devices
+-rw-r--r--   0 lleitner   (503) staff       (20)      166 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/poll
+-rw-r--r--   0 lleitner   (503) staff       (20)      685 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/man_pages/zone
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.201074 razer-cli-2.2.0/razer_cli/razer_cli/parser/
+-rw-r--r--   0 lleitner   (503) staff       (20)        0 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/parser/__init__.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     3372 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/parser/argument_parser.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     2173 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/parser/color_parser.py
+-rw-r--r--   0 lleitner   (503) staff       (20)      372 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/parser/zone_parser.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     3487 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/rc.py
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.209298 razer-cli-2.2.0/razer_cli/razer_cli/setter/
+-rw-r--r--   0 lleitner   (503) staff       (20)        0 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/setter/__init__.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     2518 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/setter/battery_setter.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     2541 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/setter/brightness_setter.py
+-rw-r--r--   0 lleitner   (503) staff       (20)    14099 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/setter/color_effect_setter.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     1790 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/setter/dpi_setter.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     1484 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/setter/poll_rate_setter.py
+-rw-r--r--   0 lleitner   (503) staff       (20)      346 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/setter/resetter.py
+-rw-r--r--   0 lleitner   (503) staff       (20)      337 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/setter/setter.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     1255 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/settings.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     9265 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/razer_cli/util.py
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.212052 razer-cli-2.2.0/razer_cli/tests/
+-rw-r--r--   0 lleitner   (503) staff       (20)        0 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/tests/__init__.py
+-rw-r--r--   0 lleitner   (503) staff       (20)      626 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/tests/test_argument_parser.py
+-rw-r--r--   0 lleitner   (503) staff       (20)     2461 2023-07-25 07:34:15.000000 razer-cli-2.2.0/razer_cli/tests/test_util.py
+drwxr-xr-x   0 lleitner   (503) staff       (20)        0 2023-08-01 05:55:36.181900 razer-cli-2.2.0/razer_cli.egg-info/
+-rw-r--r--   0 lleitner   (503) staff       (20)     8807 2023-08-01 05:55:36.000000 razer-cli-2.2.0/razer_cli.egg-info/PKG-INFO
+-rw-r--r--   0 lleitner   (503) staff       (20)     1759 2023-08-01 05:55:36.000000 razer-cli-2.2.0/razer_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 lleitner   (503) staff       (20)        1 2023-08-01 05:55:36.000000 razer-cli-2.2.0/razer_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 lleitner   (503) staff       (20)       60 2023-08-01 05:55:36.000000 razer-cli-2.2.0/razer_cli.egg-info/entry_points.txt
+-rw-r--r--   0 lleitner   (503) staff       (20)       10 2023-08-01 05:55:36.000000 razer-cli-2.2.0/razer_cli.egg-info/top_level.txt
+-rw-r--r--   0 lleitner   (503) staff       (20)      116 2023-08-01 05:55:36.214556 razer-cli-2.2.0/setup.cfg
+-rw-r--r--   0 lleitner   (503) staff       (20)      854 2023-08-01 05:51:49.000000 razer-cli-2.2.0/setup.py
```

### Comparing `razer-cli-2.1.0/LICENSE` & `razer-cli-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/PKG-INFO` & `razer-cli-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: razer-cli
-Version: 2.1.0
+Version: 2.2.0
 Summary: Control Razer devices from the command line
 Home-page: https://github.com/lolei/razer-cli
 Author: Lorenz Leitner
 Author-email: lrnz.ltnr@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # razer-cli
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 Command line interface for controlling Razer devices on Linux
 
 ## About
 With this command line interface you can configure your Razer peripherals, such
 as keyboard and mouse, set their colors and effects, etc.
 
@@ -100,14 +98,17 @@
 
 ### Example usage with Pywal
 To get your mouse and keyboard to use Pywal's colors, simply start `razer-cli`
 with the `-a` flag, after having executed `wal`: `razer-cli -a`  
 Example in action 
 [here](https://github.com/LoLei/dotfiles/blob/master/exec-wal.sh).
 
+Another option is to use `razer-cli -e multicolor,xpalette`, which not only 
+uses a single color from pywal, but uses the entire 16 color palette.
+
 #### Other examples
 `$ razer-cli -e ripple -c ff0000`  
 `$ razer-cli -e static -c ffffff`  
 
 You can also leave out the color or the effect:  
 `$ razer-cli -e breath_single`  
 `$ razer-cli -c 55ff99`
@@ -149,23 +150,24 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://github.com/Ansis100"><img src="https://avatars2.githubusercontent.com/u/35926716?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ansis</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=Ansis100" title="Code">💻</a></td>
-    <td align="center"><a href="https://t1c.dev"><img src="https://avatars0.githubusercontent.com/u/44733677?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kainoa Kanter</b></sub></a><br /><a href="#ideas-ThatOneCalculator" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://ifohancroft.com"><img src="https://avatars0.githubusercontent.com/u/3461282?v=4?s=100" width="100px;" alt=""/><br /><sub><b>IFo Hancroft</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/issues?q=author%3Aifohancroft" title="Bug reports">🐛</a> <a href="#userTesting-ifohancroft" title="User Testing">📓</a> <a href="https://github.com/LoLei/razer-cli/commits?author=ifohancroft" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/GM-Script-Writer-62850"><img src="https://avatars2.githubusercontent.com/u/564653?v=4?s=100" width="100px;" alt=""/><br /><sub><b>GM-Script-Writer-62850</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=GM-Script-Writer-62850" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ansis100"><img src="https://avatars2.githubusercontent.com/u/35926716?v=4?s=100" width="100px;" alt="Ansis"/><br /><sub><b>Ansis</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=Ansis100" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://t1c.dev"><img src="https://avatars0.githubusercontent.com/u/44733677?v=4?s=100" width="100px;" alt="Kainoa Kanter"/><br /><sub><b>Kainoa Kanter</b></sub></a><br /><a href="#ideas-ThatOneCalculator" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.ifohancroft.com"><img src="https://avatars0.githubusercontent.com/u/3461282?v=4?s=100" width="100px;" alt="IFo Hancroft"/><br /><sub><b>IFo Hancroft</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/issues?q=author%3Aifohancroft" title="Bug reports">🐛</a> <a href="#userTesting-ifohancroft" title="User Testing">📓</a> <a href="https://github.com/LoLei/razer-cli/commits?author=ifohancroft" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/GM-Script-Writer-62850"><img src="https://avatars2.githubusercontent.com/u/564653?v=4?s=100" width="100px;" alt="GM-Script-Writer-62850"/><br /><sub><b>GM-Script-Writer-62850</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=GM-Script-Writer-62850" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sk8ersteve"><img src="https://avatars.githubusercontent.com/u/10476999?v=4?s=100" width="100px;" alt="Stephen Thomas-Dorin"/><br /><sub><b>Stephen Thomas-Dorin</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=sk8ersteve" title="Code">💻</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
-
-
```

### Comparing `razer-cli-2.1.0/README.md` & `razer-cli-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # razer-cli
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 Command line interface for controlling Razer devices on Linux
 
 ## About
 With this command line interface you can configure your Razer peripherals, such
 as keyboard and mouse, set their colors and effects, etc.
 
@@ -84,14 +84,17 @@
 
 ### Example usage with Pywal
 To get your mouse and keyboard to use Pywal's colors, simply start `razer-cli`
 with the `-a` flag, after having executed `wal`: `razer-cli -a`  
 Example in action 
 [here](https://github.com/LoLei/dotfiles/blob/master/exec-wal.sh).
 
+Another option is to use `razer-cli -e multicolor,xpalette`, which not only 
+uses a single color from pywal, but uses the entire 16 color palette.
+
 #### Other examples
 `$ razer-cli -e ripple -c ff0000`  
 `$ razer-cli -e static -c ffffff`  
 
 You can also leave out the color or the effect:  
 `$ razer-cli -e breath_single`  
 `$ razer-cli -c 55ff99`
@@ -133,20 +136,23 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://github.com/Ansis100"><img src="https://avatars2.githubusercontent.com/u/35926716?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ansis</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=Ansis100" title="Code">💻</a></td>
-    <td align="center"><a href="https://t1c.dev"><img src="https://avatars0.githubusercontent.com/u/44733677?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kainoa Kanter</b></sub></a><br /><a href="#ideas-ThatOneCalculator" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://ifohancroft.com"><img src="https://avatars0.githubusercontent.com/u/3461282?v=4?s=100" width="100px;" alt=""/><br /><sub><b>IFo Hancroft</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/issues?q=author%3Aifohancroft" title="Bug reports">🐛</a> <a href="#userTesting-ifohancroft" title="User Testing">📓</a> <a href="https://github.com/LoLei/razer-cli/commits?author=ifohancroft" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/GM-Script-Writer-62850"><img src="https://avatars2.githubusercontent.com/u/564653?v=4?s=100" width="100px;" alt=""/><br /><sub><b>GM-Script-Writer-62850</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=GM-Script-Writer-62850" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ansis100"><img src="https://avatars2.githubusercontent.com/u/35926716?v=4?s=100" width="100px;" alt="Ansis"/><br /><sub><b>Ansis</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=Ansis100" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://t1c.dev"><img src="https://avatars0.githubusercontent.com/u/44733677?v=4?s=100" width="100px;" alt="Kainoa Kanter"/><br /><sub><b>Kainoa Kanter</b></sub></a><br /><a href="#ideas-ThatOneCalculator" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.ifohancroft.com"><img src="https://avatars0.githubusercontent.com/u/3461282?v=4?s=100" width="100px;" alt="IFo Hancroft"/><br /><sub><b>IFo Hancroft</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/issues?q=author%3Aifohancroft" title="Bug reports">🐛</a> <a href="#userTesting-ifohancroft" title="User Testing">📓</a> <a href="https://github.com/LoLei/razer-cli/commits?author=ifohancroft" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/GM-Script-Writer-62850"><img src="https://avatars2.githubusercontent.com/u/564653?v=4?s=100" width="100px;" alt="GM-Script-Writer-62850"/><br /><sub><b>GM-Script-Writer-62850</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=GM-Script-Writer-62850" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sk8ersteve"><img src="https://avatars.githubusercontent.com/u/10476999?v=4?s=100" width="100px;" alt="Stephen Thomas-Dorin"/><br /><sub><b>Stephen Thomas-Dorin</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=sk8ersteve" title="Code">💻</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/handler/brightness_handler.py` & `razer-cli-2.2.0/razer_cli/razer_cli/handler/brightness_handler.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/handler/color_effect_handler.py` & `razer-cli-2.2.0/razer_cli/razer_cli/handler/color_effect_handler.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/handler/version_handler.py` & `razer-cli-2.2.0/razer_cli/razer_cli/handler/version_handler.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/lister/device_lister.py` & `razer-cli-2.2.0/razer_cli/razer_cli/lister/device_lister.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,19 @@
                     print("   DPI stages:", device.dpi_stages)
                 if device.has('poll_rate'):
                     print("   polling rate:", device.poll_rate)
                 if device.has('battery'):
                     print("   battery:")
                     print("      charge:", device.battery_level)
                     print("      charging:", device.is_charging)
-                    print("      low threshold:",
-                          device.get_low_battery_threshold(), '%')
-                    print("      idle delay", device.get_idle_time(), 'seconds')
+                    if device.has('get_low_battery_threshold'):
+                        print("      low threshold:",
+                              device.get_low_battery_threshold(), '%')
+                    if device.has('get_idle_time'):
+                        print("      idle delay", device.get_idle_time(), 'seconds')
 
                 for i in settings.ZONES:
                     # Settings
                     if i == 'generic':
                         print('  ', i, 'zone:')
                         if util.rgb_support(device, effect='brightness'):
                             print("      brightness:", device.brightness)
```

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/main.py` & `razer-cli-2.2.0/razer_cli/razer_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """
 Module Docstring
 """
 
 __author__ = "Lorenz Leitner"
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 __license__ = "GPL-3.0"
 
 import sys
 
 from openrazer.client import DeviceManager
 
 from razer_cli.razer_cli import util
```

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/man_pages/color` & `razer-cli-2.2.0/razer_cli/razer_cli/man_pages/color`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/man_pages/effect` & `razer-cli-2.2.0/razer_cli/razer_cli/man_pages/effect`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/man_pages/example` & `razer-cli-2.2.0/razer_cli/razer_cli/man_pages/example`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/man_pages/zone` & `razer-cli-2.2.0/razer_cli/razer_cli/man_pages/zone`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/parser/argument_parser.py` & `razer-cli-2.2.0/razer_cli/razer_cli/parser/argument_parser.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/parser/color_parser.py` & `razer-cli-2.2.0/razer_cli/razer_cli/parser/color_parser.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/rc.py` & `razer-cli-2.2.0/razer_cli/razer_cli/rc.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/setter/battery_setter.py` & `razer-cli-2.2.0/razer_cli/razer_cli/setter/battery_setter.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,32 +10,36 @@
         for device in self.device_manager.devices:
             if (self.args.device and (device.name in self.args.device or device.serial in self.args.device)) or (not self.args.device):
                 if device.has("battery"):
                     if len(self.args.battery) < 2:
                         print(device.name, 'battery:')
                         print("   charge:", device.battery_level)
                         print("   charging:", device.is_charging)
-                        print("   low threshold:",
-                              device.get_low_battery_threshold(), '%')
-                        print("   idle delay", device.get_idle_time(), 'seconds')
+                        if device.has('get_low_battery_threshold'):
+                            print("   low threshold:",
+                                device.get_low_battery_threshold(), '%')
+                        if device.has('get_idle_time'):
+                            print("   idle delay", device.get_idle_time(), 'seconds')
                     else:
                         i = 0
                         stop = len(self.args.battery)
                         bat = {}
                         while i < stop:
                             if self.args.battery[i] == "low" and stop > i + 1:
                                 bat['low'] = int(self.args.battery[i + 1])
-                                device.set_low_battery_threshold(bat['low'])
-                                if self.args.verbose:
+                                if device.has("set_low_battery_threshold"):
+                                    device.set_low_battery_threshold(bat['low'])
+                                if self.args.verbose and device.has("get_low_battery_threshold"):
                                     print(device.name, 'low battery =',
                                           device.get_low_battery_threshold(), '%')
                             elif self.args.battery[i] == "idle" and stop > i + 1:
                                 bat['idle'] = int(self.args.battery[i + 1])
-                                device.set_idle_time(bat['idle'])
-                                if self.args.verbose:
+                                if device.has("set_idle_time"):
+                                    device.set_idle_time(bat['idle'])
+                                if self.args.verbose and device.has("get_idle_time"):
                                     print(device.name, 'idle delay =',
                                           device.get_idle_time(), 'seconds')
                             i += 1
                         # Save used settings for this device to a file
                         util.write_settings_to_file(device, battery=bat)
                 else:
                     print('Does', device.name, 'have a battery?')
```

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/setter/brightness_setter.py` & `razer-cli-2.2.0/razer_cli/razer_cli/setter/brightness_setter.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/setter/color_effect_setter.py` & `razer-cli-2.2.0/razer_cli/razer_cli/setter/color_effect_setter.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/setter/dpi_setter.py` & `razer-cli-2.2.0/razer_cli/razer_cli/setter/dpi_setter.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/setter/poll_rate_setter.py` & `razer-cli-2.2.0/razer_cli/razer_cli/setter/poll_rate_setter.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/settings.py` & `razer-cli-2.2.0/razer_cli/razer_cli/settings.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/razer_cli/util.py` & `razer-cli-2.2.0/razer_cli/razer_cli/util.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/tests/test_argument_parser.py` & `razer-cli-2.2.0/razer_cli/tests/test_argument_parser.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli/tests/test_util.py` & `razer-cli-2.2.0/razer_cli/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/razer_cli.egg-info/PKG-INFO` & `razer-cli-2.2.0/razer_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: razer-cli
-Version: 2.1.0
+Version: 2.2.0
 Summary: Control Razer devices from the command line
 Home-page: https://github.com/lolei/razer-cli
 Author: Lorenz Leitner
 Author-email: lrnz.ltnr@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # razer-cli
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 Command line interface for controlling Razer devices on Linux
 
 ## About
 With this command line interface you can configure your Razer peripherals, such
 as keyboard and mouse, set their colors and effects, etc.
 
@@ -100,14 +98,17 @@
 
 ### Example usage with Pywal
 To get your mouse and keyboard to use Pywal's colors, simply start `razer-cli`
 with the `-a` flag, after having executed `wal`: `razer-cli -a`  
 Example in action 
 [here](https://github.com/LoLei/dotfiles/blob/master/exec-wal.sh).
 
+Another option is to use `razer-cli -e multicolor,xpalette`, which not only 
+uses a single color from pywal, but uses the entire 16 color palette.
+
 #### Other examples
 `$ razer-cli -e ripple -c ff0000`  
 `$ razer-cli -e static -c ffffff`  
 
 You can also leave out the color or the effect:  
 `$ razer-cli -e breath_single`  
 `$ razer-cli -c 55ff99`
@@ -149,23 +150,24 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://github.com/Ansis100"><img src="https://avatars2.githubusercontent.com/u/35926716?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ansis</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=Ansis100" title="Code">💻</a></td>
-    <td align="center"><a href="https://t1c.dev"><img src="https://avatars0.githubusercontent.com/u/44733677?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kainoa Kanter</b></sub></a><br /><a href="#ideas-ThatOneCalculator" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://ifohancroft.com"><img src="https://avatars0.githubusercontent.com/u/3461282?v=4?s=100" width="100px;" alt=""/><br /><sub><b>IFo Hancroft</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/issues?q=author%3Aifohancroft" title="Bug reports">🐛</a> <a href="#userTesting-ifohancroft" title="User Testing">📓</a> <a href="https://github.com/LoLei/razer-cli/commits?author=ifohancroft" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/GM-Script-Writer-62850"><img src="https://avatars2.githubusercontent.com/u/564653?v=4?s=100" width="100px;" alt=""/><br /><sub><b>GM-Script-Writer-62850</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=GM-Script-Writer-62850" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ansis100"><img src="https://avatars2.githubusercontent.com/u/35926716?v=4?s=100" width="100px;" alt="Ansis"/><br /><sub><b>Ansis</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=Ansis100" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://t1c.dev"><img src="https://avatars0.githubusercontent.com/u/44733677?v=4?s=100" width="100px;" alt="Kainoa Kanter"/><br /><sub><b>Kainoa Kanter</b></sub></a><br /><a href="#ideas-ThatOneCalculator" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.ifohancroft.com"><img src="https://avatars0.githubusercontent.com/u/3461282?v=4?s=100" width="100px;" alt="IFo Hancroft"/><br /><sub><b>IFo Hancroft</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/issues?q=author%3Aifohancroft" title="Bug reports">🐛</a> <a href="#userTesting-ifohancroft" title="User Testing">📓</a> <a href="https://github.com/LoLei/razer-cli/commits?author=ifohancroft" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/GM-Script-Writer-62850"><img src="https://avatars2.githubusercontent.com/u/564653?v=4?s=100" width="100px;" alt="GM-Script-Writer-62850"/><br /><sub><b>GM-Script-Writer-62850</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=GM-Script-Writer-62850" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sk8ersteve"><img src="https://avatars.githubusercontent.com/u/10476999?v=4?s=100" width="100px;" alt="Stephen Thomas-Dorin"/><br /><sub><b>Stephen Thomas-Dorin</b></sub></a><br /><a href="https://github.com/LoLei/razer-cli/commits?author=sk8ersteve" title="Code">💻</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
-
-
```

### Comparing `razer-cli-2.1.0/razer_cli.egg-info/SOURCES.txt` & `razer-cli-2.2.0/razer_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `razer-cli-2.1.0/setup.py` & `razer-cli-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """razer-cli - setup.py"""
 from setuptools import setup, find_packages
 
 LONG_DESC = open('README.md').read()
 
 setup(
     name="razer-cli",
-    version="2.1.0",
+    version="2.2.0",
     author="Lorenz Leitner",
     author_email="lrnz.ltnr@gmail.com",
     description="Control Razer devices from the command line",
     long_description_content_type="text/markdown",
     long_description=LONG_DESC,
     url="https://github.com/lolei/razer-cli",
     classifiers=[
```

