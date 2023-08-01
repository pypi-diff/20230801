# Comparing `tmp/tsuchinoko-1.1.0.tar.gz` & `tmp/tsuchinoko-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsuchinoko-1.1.0.tar", last modified: Tue Jul 25 20:48:31 2023, max compression
+gzip compressed data, was "tsuchinoko-1.1.1.tar", last modified: Tue Aug  1 19:00:51 2023, max compression
```

## Comparing `tsuchinoko-1.1.0.tar` & `tsuchinoko-1.1.1.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.547758 tsuchinoko-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.547758 tsuchinoko-1.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.547758 tsuchinoko-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tests/test_graphics_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tests/test_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/adaptive/
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/acquisition_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/gpCAM_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/quadtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/random_in_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/core/
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/core/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/IRBL_server_demo_LC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/_launch_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/adaptive_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/bluesky_adaptive_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/client_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/grid_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/headless_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/high_dimensionality_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/ir_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/multi_task_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/quadtree_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/server_demo_bluesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/vector_metric_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/execution/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/bluesky_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/bluesky_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/threaded_in_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/graphics_items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphics_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphics_items/clouditem.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphics_items/indicatoritem.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphics_items/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphs/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/patches/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/patches/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/patches/pyqode.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/patches/pyqtgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/plan_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/plan_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/mutex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/runengine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/debugmenubar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/graph_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/server_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.547758 tsuchinoko-1.1.0/tsuchinoko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.891714 tsuchinoko-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.891714 tsuchinoko-1.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.895714 tsuchinoko-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tests/test_graphics_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/tsuchinoko/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/tsuchinoko/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.899714 tsuchinoko-1.1.1/tsuchinoko/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/acquisition_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/gpCAM_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/quadtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/adaptive/random_in_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.899714 tsuchinoko-1.1.1/tsuchinoko/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.899714 tsuchinoko-1.1.1/tsuchinoko/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/core/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.899714 tsuchinoko-1.1.1/tsuchinoko/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/IRBL_server_demo_LC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/_launch_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/adaptive_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/bluesky_adaptive_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/client_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/grid_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/headless_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/high_dimensionality_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/ir_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/multi_task_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/quadtree_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/server_demo_bluesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112760 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/sombrero_pug.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/examples/vector_metric_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/bluesky_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/bluesky_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/execution/threaded_in_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/graphics_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphics_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphics_items/clouditem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphics_items/indicatoritem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphics_items/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/graphs/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/patches/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/patches/pyqode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/patches/pyqtgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.903714 tsuchinoko-1.1.1/tsuchinoko/plan_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/plan_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/tsuchinoko/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/mutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/runengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/utils/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.907714 tsuchinoko-1.1.1/tsuchinoko/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/debugmenubar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/graph_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/server_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/tsuchinoko/widgets/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:00:51.895714 tsuchinoko-1.1.1/tsuchinoko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 19:00:51.000000 tsuchinoko-1.1.1/tsuchinoko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-08-01 19:00:40.000000 tsuchinoko-1.1.1/versioneer.py
```

### Comparing `tsuchinoko-1.1.0/CONTRIBUTING.rst` & `tsuchinoko-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/LICENSE` & `tsuchinoko-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/PKG-INFO` & `tsuchinoko-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsuchinoko
-Version: 1.1.0
+Version: 1.1.1
 Summary: An adaptive optics alignment tool for ALS beamlines utilizing gpCAM.
 Home-page: https://github.com/lbl-camera/tsuchinoko
 Author: Ronald J Pandolfi
 Author-email: ronpandolfi@lbl.gov
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tsuchinoko-1.1.0/README.md` & `tsuchinoko-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/docs/Makefile` & `tsuchinoko-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/docs/make.bat` & `tsuchinoko-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/docs/source/conf.py` & `tsuchinoko-1.1.1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,10 +199,11 @@
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3/', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/stable', None),
     'matplotlib': ('https://matplotlib.org/stable', None),
     'pyqtgraph': ("https://pyqtgraph.readthedocs.io/en/latest/", None),
+    'bluesky-adaptive': ("https://blueskyproject.io/bluesky-adaptive/", None),
 }
 
 autoclass_content = 'both'
```

### Comparing `tsuchinoko-1.1.0/legal.txt` & `tsuchinoko-1.1.1/legal.txt`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/setup.py` & `tsuchinoko-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tests/test_core.py` & `tsuchinoko-1.1.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tests/test_graphics_items.py` & `tsuchinoko-1.1.1/tests/test_graphics_items.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tests/test_gui.py` & `tsuchinoko-1.1.1/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/__init__.py` & `tsuchinoko-1.1.1/tsuchinoko/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/adaptive/__init__.py` & `tsuchinoko-1.1.1/tsuchinoko/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/adaptive/acquisition_functions.py` & `tsuchinoko-1.1.1/tsuchinoko/adaptive/acquisition_functions.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/adaptive/adaptive.py` & `tsuchinoko-1.1.1/tsuchinoko/adaptive/adaptive.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py` & `tsuchinoko-1.1.1/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/adaptive/gpCAM_in_process.py` & `tsuchinoko-1.1.1/tsuchinoko/adaptive/gpCAM_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/adaptive/grid.py` & `tsuchinoko-1.1.1/tsuchinoko/adaptive/grid.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/adaptive/quadtree.py` & `tsuchinoko-1.1.1/tsuchinoko/adaptive/quadtree.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/adaptive/random_in_process.py` & `tsuchinoko-1.1.1/tsuchinoko/adaptive/random_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/core/__init__.py` & `tsuchinoko-1.1.1/tsuchinoko/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/core/messages.py` & `tsuchinoko-1.1.1/tsuchinoko/core/messages.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/IRBL_server_demo_LC.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/IRBL_server_demo_LC.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/adaptive_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/adaptive_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/bluesky_adaptive_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/bluesky_adaptive_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/grid_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/grid_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/headless_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/headless_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/high_dimensionality_server_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/high_dimensionality_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/ir_server_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/ir_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/multi_task_server_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/multi_task_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/quadtree_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/quadtree_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/server_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/server_demo_bluesky.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/server_demo_bluesky.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/examples/vector_metric_demo.py` & `tsuchinoko-1.1.1/tsuchinoko/examples/vector_metric_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/execution/__init__.py` & `tsuchinoko-1.1.1/tsuchinoko/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/execution/bluesky_adaptive.py` & `tsuchinoko-1.1.1/tsuchinoko/execution/bluesky_adaptive.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/execution/bluesky_in_process.py` & `tsuchinoko-1.1.1/tsuchinoko/execution/bluesky_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/execution/simple.py` & `tsuchinoko-1.1.1/tsuchinoko/execution/simple.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/execution/threaded_in_process.py` & `tsuchinoko-1.1.1/tsuchinoko/execution/threaded_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/graphics_items/clouditem.py` & `tsuchinoko-1.1.1/tsuchinoko/graphics_items/clouditem.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/graphics_items/mixins.py` & `tsuchinoko-1.1.1/tsuchinoko/graphics_items/mixins.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/graphs/__init__.py` & `tsuchinoko-1.1.1/tsuchinoko/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/graphs/common.py` & `tsuchinoko-1.1.1/tsuchinoko/graphs/common.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/patches/pyqode.py` & `tsuchinoko-1.1.1/tsuchinoko/patches/pyqode.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/patches/pyqtgraph.py` & `tsuchinoko-1.1.1/tsuchinoko/patches/pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/plan_stubs/__init__.py` & `tsuchinoko-1.1.1/tsuchinoko/plan_stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/utils/__init__.py` & `tsuchinoko-1.1.1/tsuchinoko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/utils/coverage.py` & `tsuchinoko-1.1.1/tsuchinoko/utils/coverage.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/utils/dependencies.py` & `tsuchinoko-1.1.1/tsuchinoko/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/utils/logging.py` & `tsuchinoko-1.1.1/tsuchinoko/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/utils/mutex.py` & `tsuchinoko-1.1.1/tsuchinoko/utils/mutex.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/utils/runengine.py` & `tsuchinoko-1.1.1/tsuchinoko/utils/runengine.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/utils/threads.py` & `tsuchinoko-1.1.1/tsuchinoko/utils/threads.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/widgets/debugmenubar.py` & `tsuchinoko-1.1.1/tsuchinoko/widgets/debugmenubar.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/widgets/displays.py` & `tsuchinoko-1.1.1/tsuchinoko/widgets/displays.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/widgets/graph_widgets.py` & `tsuchinoko-1.1.1/tsuchinoko/widgets/graph_widgets.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/widgets/mainwindow.py` & `tsuchinoko-1.1.1/tsuchinoko/widgets/mainwindow.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/widgets/server_editor.py` & `tsuchinoko-1.1.1/tsuchinoko/widgets/server_editor.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko/widgets/simple.py` & `tsuchinoko-1.1.1/tsuchinoko/widgets/simple.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.1.0/tsuchinoko.egg-info/PKG-INFO` & `tsuchinoko-1.1.1/tsuchinoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsuchinoko
-Version: 1.1.0
+Version: 1.1.1
 Summary: An adaptive optics alignment tool for ALS beamlines utilizing gpCAM.
 Home-page: https://github.com/lbl-camera/tsuchinoko
 Author: Ronald J Pandolfi
 Author-email: ronpandolfi@lbl.gov
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tsuchinoko-1.1.0/tsuchinoko.egg-info/SOURCES.txt` & `tsuchinoko-1.1.1/tsuchinoko.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 tsuchinoko/examples/headless_demo.py
 tsuchinoko/examples/high_dimensionality_server_demo.py
 tsuchinoko/examples/ir_server_demo.py
 tsuchinoko/examples/multi_task_server_demo.py
 tsuchinoko/examples/quadtree_demo.py
 tsuchinoko/examples/server_demo.py
 tsuchinoko/examples/server_demo_bluesky.py
+tsuchinoko/examples/sombrero_pug.jpg
 tsuchinoko/examples/vector_metric_demo.py
 tsuchinoko/execution/__init__.py
 tsuchinoko/execution/bluesky_adaptive.py
 tsuchinoko/execution/bluesky_in_process.py
 tsuchinoko/execution/simple.py
 tsuchinoko/execution/threaded_in_process.py
 tsuchinoko/extensions/__init__.py
```

### Comparing `tsuchinoko-1.1.0/versioneer.py` & `tsuchinoko-1.1.1/versioneer.py`

 * *Files identical despite different names*

