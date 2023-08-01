# Comparing `tmp/micrologai-1.3.3.tar.gz` & `tmp/micrologai-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micrologai-1.3.3.tar", last modified: Thu Jul 27 20:14:28 2023, max compression
+gzip compressed data, was "micrologai-1.3.4.tar", last modified: Tue Aug  1 09:56:51 2023, max compression
```

## Comparing `micrologai-1.3.3.tar` & `micrologai-1.3.4.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.968997 micrologai-1.3.3/
--rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.3/LICENSE
--rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.3/MANIFEST.in
--rw-r--r--   0 laffra     (501) staff       (20)    46678 2023-07-27 20:14:28.971424 micrologai-1.3.3/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)    11038 2023-07-26 18:33:07.000000 micrologai-1.3.3/README.md
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.384308 micrologai-1.3.3/dashboard/
--rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    12401 2023-07-27 20:00:40.000000 micrologai-1.3.3/dashboard/canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.3/dashboard/colors.py
--rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     8571 2023-07-27 07:37:34.000000 micrologai-1.3.3/dashboard/design.py
--rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/dialog.py
--rw-r--r--   0 laffra     (501) staff       (20)    13720 2023-07-27 19:59:14.000000 micrologai-1.3.3/dashboard/main.py
--rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/markdown.py
--rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.3/dashboard/profiler.py
--rw-r--r--   0 laffra     (501) staff       (20)     2218 2023-07-27 07:38:32.000000 micrologai-1.3.3/dashboard/tips.py
--rw-r--r--   0 laffra     (501) staff       (20)     4245 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/treeview.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.411112 micrologai-1.3.3/dashboard/views/
--rw-r--r--   0 laffra     (501) staff       (20)     2165 2023-07-26 09:43:49.000000 micrologai-1.3.3/dashboard/views/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    15841 2023-07-27 19:32:02.000000 micrologai-1.3.3/dashboard/views/call.py
--rw-r--r--   0 laffra     (501) staff       (20)     5010 2023-07-27 20:05:28.000000 micrologai-1.3.3/dashboard/views/marker.py
--rw-r--r--   0 laffra     (501) staff       (20)     4416 2023-07-26 13:59:52.000000 micrologai-1.3.3/dashboard/views/status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.3/dashboard/views/timeline.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.501963 micrologai-1.3.3/examples/
--rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.3/examples/binaryTrees.py
--rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.3/examples/books.json
--rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.3/examples/bookstore.py
--rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.3/examples/dataframes.py
--rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.3/examples/example.py
--rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.3/examples/files.py
--rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.3/examples/go.py
--rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.3/examples/helloworld.py
--rw-r--r--   0 laffra     (501) staff       (20)     1127 2023-07-08 12:02:09.000000 micrologai-1.3.3/examples/memory.py
--rw-r--r--   0 laffra     (501) staff       (20)     1178 2023-07-24 10:45:34.000000 micrologai-1.3.3/examples/modules.py
--rwxr-xr-x   0 laffra     (501) staff       (20)      410 2023-07-24 11:06:15.000000 micrologai-1.3.3/examples/runall.sh
--rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.3/examples/startstop.py
--rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.3/examples/threads.py
--rw-r--r--   0 laffra     (501) staff       (20)    93813 2023-07-24 11:09:29.000000 micrologai-1.3.3/examples/treemap.ipynb
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.557129 micrologai-1.3.3/microlog/
--rw-r--r--   0 laffra     (501) staff       (20)      302 2023-07-27 20:13:48.000000 micrologai-1.3.3/microlog/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)     2798 2023-07-24 11:03:18.000000 micrologai-1.3.3/microlog/api.py
--rw-r--r--   0 laffra     (501) staff       (20)      769 2023-07-24 11:11:41.000000 micrologai-1.3.3/microlog/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.3/microlog/explain.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.738247 micrologai-1.3.3/microlog/images/
--rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.3/microlog/images/anomaly.png
--rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.3/microlog/images/apple-touch-icon.png
--rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.3/microlog/images/chatgpt.png
--rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.3/microlog/images/design-go.png
--rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.3/microlog/images/dialog.png
--rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.3/microlog/images/error-log.png
--rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.3/microlog/images/favicon-16x16.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.3/microlog/images/favicon-32x32.png
--rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.3/microlog/images/fd-leak.png
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.875154 micrologai-1.3.3/microlog/images/icons/
--rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.3/microlog/images/icons/asyncio.png
--rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.3/microlog/images/icons/dataclasses.png
--rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.3/microlog/images/icons/email.png
--rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.3/microlog/images/icons/google.png
--rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.3/microlog/images/icons/guppy.png
--rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.3/microlog/images/icons/http.png
--rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.3/microlog/images/icons/jupyter.png
--rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.3/microlog/images/icons/matplotlib.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.3/microlog/images/icons/microlog.png
--rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.3/microlog/images/icons/networkx.png
--rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.3/microlog/images/icons/numpy.png
--rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.3/microlog/images/icons/pandas.png
--rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.3/microlog/images/icons/pyparsing.png
--rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.3/microlog/images/icons/pytest.png
--rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.3/microlog/images/icons/python.png
--rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.3/microlog/images/icons/re.png
--rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.3/microlog/images/icons/squarify.png
--rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.3/microlog/images/icons/ssl.png
--rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.3/microlog/images/icons/tornado.png
--rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.3/microlog/images/icons/urllib.png
--rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.3/microlog/images/icons/wsgi.png
--rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.3/microlog/images/icons/zmq.png
--rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.3/microlog/images/log.png
--rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.3/microlog/images/logo-bing.png
--rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.3/microlog/images/logo-brave.png
--rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.3/microlog/images/logo-duckduckgo.png
--rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.3/microlog/images/logo-google.png
--rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.3/microlog/images/logo-hackernews.png
--rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.3/microlog/images/logo-sourcegraph.png
--rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.3/microlog/images/logo-stackoverflow.png
--rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.3/microlog/images/logo-twitter.png
--rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.3/microlog/images/markdown.png
--rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.3/microlog/images/memory-leak.png
--rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.3/microlog/images/overview.png
--rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.3/microlog/images/spinner.png
--rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.3/microlog/images/status.png
--rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.3/microlog/images/tips.png
--rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.3/microlog/images/zoomedin.png
--rw-r--r--   0 laffra     (501) staff       (20)     4844 2023-07-26 12:10:57.000000 micrologai-1.3.3/microlog/log.py
--rw-r--r--   0 laffra     (501) staff       (20)     9743 2023-07-24 10:08:40.000000 micrologai-1.3.3/microlog/models.py
--rw-r--r--   0 laffra     (501) staff       (20)     6102 2023-07-27 20:12:14.000000 micrologai-1.3.3/microlog/server.py
--rw-r--r--   0 laffra     (501) staff       (20)      538 2023-07-19 13:49:13.000000 micrologai-1.3.3/microlog/sitecustomize.py
--rw-r--r--   0 laffra     (501) staff       (20)    17190 2023-07-24 10:07:20.000000 micrologai-1.3.3/microlog/tracer.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.915794 micrologai-1.3.3/micrologai.egg-info/
--rw-r--r--   0 laffra     (501) staff       (20)    46678 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)     2768 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/SOURCES.txt
--rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/dependency_links.txt
--rw-r--r--   0 laffra     (501) staff       (20)       48 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/entry_points.txt
--rw-r--r--   0 laffra     (501) staff       (20)       41 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/requires.txt
--rw-r--r--   0 laffra     (501) staff       (20)       19 2023-07-27 20:14:28.000000 micrologai-1.3.3/micrologai.egg-info/top_level.txt
--rw-r--r--   0 laffra     (501) staff       (20)      893 2023-07-27 20:13:48.000000 micrologai-1.3.3/pyproject.toml
--rw-r--r--   0 laffra     (501) staff       (20)       79 2023-07-27 20:14:28.981920 micrologai-1.3.3/setup.cfg
--rw-r--r--   0 laffra     (501) staff       (20)     1560 2023-07-27 20:13:48.000000 micrologai-1.3.3/setup.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-27 20:14:28.966525 micrologai-1.3.3/tests/
--rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.3/tests/test_call_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.3/tests/test_canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.3/tests/test_log.py
--rw-r--r--   0 laffra     (501) staff       (20)     1755 2023-07-26 09:43:39.000000 micrologai-1.3.3/tests/test_marker_view.py
--rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.3/tests/test_print.py
--rw-r--r--   0 laffra     (501) staff       (20)      727 2023-07-02 20:31:07.000000 micrologai-1.3.3/tests/test_status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.3/tests/test_status_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.3/tests/test_tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:51.387175 micrologai-1.3.4/
+-rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.4/LICENSE
+-rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.4/MANIFEST.in
+-rw-r--r--   0 laffra     (501) staff       (20)    46802 2023-08-01 09:56:51.391488 micrologai-1.3.4/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)    11162 2023-07-31 16:21:51.000000 micrologai-1.3.4/README.md
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:50.524849 micrologai-1.3.4/dashboard/
+-rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.4/dashboard/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    12401 2023-07-27 20:00:40.000000 micrologai-1.3.4/dashboard/canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.4/dashboard/colors.py
+-rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.4/dashboard/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     8571 2023-07-27 07:37:34.000000 micrologai-1.3.4/dashboard/design.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.4/dashboard/dialog.py
+-rw-r--r--   0 laffra     (501) staff       (20)    13803 2023-07-31 18:51:03.000000 micrologai-1.3.4/dashboard/main.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.4/dashboard/markdown.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.4/dashboard/profiler.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2233 2023-07-31 16:28:15.000000 micrologai-1.3.4/dashboard/tips.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4396 2023-07-30 20:29:02.000000 micrologai-1.3.4/dashboard/treeview.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:50.569634 micrologai-1.3.4/dashboard/views/
+-rw-r--r--   0 laffra     (501) staff       (20)     2165 2023-07-26 09:43:49.000000 micrologai-1.3.4/dashboard/views/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    15841 2023-08-01 09:55:10.000000 micrologai-1.3.4/dashboard/views/call.py
+-rw-r--r--   0 laffra     (501) staff       (20)     5222 2023-07-29 10:41:01.000000 micrologai-1.3.4/dashboard/views/marker.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4416 2023-07-26 13:59:52.000000 micrologai-1.3.4/dashboard/views/status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.4/dashboard/views/timeline.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:50.697675 micrologai-1.3.4/examples/
+-rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.4/examples/binaryTrees.py
+-rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.4/examples/books.json
+-rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.4/examples/bookstore.py
+-rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.4/examples/dataframes.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.4/examples/example.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.4/examples/files.py
+-rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.4/examples/go.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.4/examples/helloworld.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1361 2023-08-01 08:23:56.000000 micrologai-1.3.4/examples/memory.py
+-rw-r--r--   0 laffra     (501) staff       (20)      970 2023-07-29 20:25:44.000000 micrologai-1.3.4/examples/modules.py
+-rwxr-xr-x   0 laffra     (501) staff       (20)      729 2023-08-01 08:27:55.000000 micrologai-1.3.4/examples/runall.sh
+-rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.4/examples/startstop.py
+-rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.4/examples/threads.py
+-rw-r--r--   0 laffra     (501) staff       (20)    94019 2023-07-31 09:16:43.000000 micrologai-1.3.4/examples/treemap.ipynb
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:50.776531 micrologai-1.3.4/microlog/
+-rw-r--r--   0 laffra     (501) staff       (20)      302 2023-08-01 09:56:29.000000 micrologai-1.3.4/microlog/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2841 2023-07-30 08:16:55.000000 micrologai-1.3.4/microlog/api.py
+-rw-r--r--   0 laffra     (501) staff       (20)      873 2023-08-01 08:27:24.000000 micrologai-1.3.4/microlog/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.4/microlog/explain.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:51.025656 micrologai-1.3.4/microlog/images/
+-rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.4/microlog/images/anomaly.png
+-rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.4/microlog/images/apple-touch-icon.png
+-rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.4/microlog/images/chatgpt.png
+-rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.4/microlog/images/design-go.png
+-rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.4/microlog/images/dialog.png
+-rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.4/microlog/images/error-log.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.4/microlog/images/favicon-16x16.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.4/microlog/images/favicon-32x32.png
+-rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.4/microlog/images/fd-leak.png
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:51.239629 micrologai-1.3.4/microlog/images/icons/
+-rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.4/microlog/images/icons/asyncio.png
+-rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.4/microlog/images/icons/dataclasses.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.4/microlog/images/icons/email.png
+-rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.4/microlog/images/icons/google.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.4/microlog/images/icons/guppy.png
+-rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.4/microlog/images/icons/http.png
+-rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.4/microlog/images/icons/jupyter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.4/microlog/images/icons/matplotlib.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.4/microlog/images/icons/microlog.png
+-rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.4/microlog/images/icons/networkx.png
+-rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.4/microlog/images/icons/numpy.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.4/microlog/images/icons/pandas.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.4/microlog/images/icons/pyparsing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.4/microlog/images/icons/pytest.png
+-rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.4/microlog/images/icons/python.png
+-rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.4/microlog/images/icons/re.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.4/microlog/images/icons/squarify.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.4/microlog/images/icons/ssl.png
+-rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.4/microlog/images/icons/tornado.png
+-rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.4/microlog/images/icons/urllib.png
+-rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.4/microlog/images/icons/wsgi.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.4/microlog/images/icons/zmq.png
+-rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.4/microlog/images/log.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.4/microlog/images/logo-bing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.4/microlog/images/logo-brave.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.4/microlog/images/logo-duckduckgo.png
+-rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.4/microlog/images/logo-google.png
+-rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.4/microlog/images/logo-hackernews.png
+-rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.4/microlog/images/logo-sourcegraph.png
+-rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.4/microlog/images/logo-stackoverflow.png
+-rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.4/microlog/images/logo-twitter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.4/microlog/images/markdown.png
+-rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.4/microlog/images/memory-leak.png
+-rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.4/microlog/images/overview.png
+-rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.4/microlog/images/spinner.png
+-rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.4/microlog/images/status.png
+-rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.4/microlog/images/tips.png
+-rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.4/microlog/images/zoomedin.png
+-rw-r--r--   0 laffra     (501) staff       (20)     5029 2023-08-01 07:51:23.000000 micrologai-1.3.4/microlog/log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     9741 2023-07-28 08:12:21.000000 micrologai-1.3.4/microlog/models.py
+-rw-r--r--   0 laffra     (501) staff       (20)     6190 2023-07-31 18:51:32.000000 micrologai-1.3.4/microlog/server.py
+-rw-r--r--   0 laffra     (501) staff       (20)      595 2023-07-30 16:11:01.000000 micrologai-1.3.4/microlog/sitecustomize.py
+-rw-r--r--   0 laffra     (501) staff       (20)    19471 2023-08-01 08:21:14.000000 micrologai-1.3.4/microlog/tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:51.304984 micrologai-1.3.4/micrologai.egg-info/
+-rw-r--r--   0 laffra     (501) staff       (20)    46802 2023-08-01 09:56:50.000000 micrologai-1.3.4/micrologai.egg-info/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)     2801 2023-08-01 09:56:50.000000 micrologai-1.3.4/micrologai.egg-info/SOURCES.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        1 2023-08-01 09:56:50.000000 micrologai-1.3.4/micrologai.egg-info/dependency_links.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       48 2023-08-01 09:56:50.000000 micrologai-1.3.4/micrologai.egg-info/entry_points.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-30 10:03:22.000000 micrologai-1.3.4/micrologai.egg-info/not-zip-safe
+-rw-r--r--   0 laffra     (501) staff       (20)       41 2023-08-01 09:56:50.000000 micrologai-1.3.4/micrologai.egg-info/requires.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       19 2023-08-01 09:56:50.000000 micrologai-1.3.4/micrologai.egg-info/top_level.txt
+-rw-r--r--   0 laffra     (501) staff       (20)      893 2023-08-01 09:56:29.000000 micrologai-1.3.4/pyproject.toml
+-rw-r--r--   0 laffra     (501) staff       (20)       79 2023-08-01 09:56:51.403141 micrologai-1.3.4/setup.cfg
+-rw-r--r--   0 laffra     (501) staff       (20)     1765 2023-08-01 09:56:29.000000 micrologai-1.3.4/setup.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-08-01 09:56:51.382395 micrologai-1.3.4/tests/
+-rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.4/tests/test_call_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.4/tests/test_canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.4/tests/test_log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1755 2023-07-26 09:43:39.000000 micrologai-1.3.4/tests/test_marker_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.4/tests/test_print.py
+-rw-r--r--   0 laffra     (501) staff       (20)      740 2023-07-30 08:56:08.000000 micrologai-1.3.4/tests/test_status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.4/tests/test_status_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.4/tests/test_tracer.py
```

### Comparing `micrologai-1.3.3/LICENSE` & `micrologai-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/PKG-INFO` & `micrologai-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.3
+Version: 1.3.4
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
         
@@ -569,14 +569,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # microlog.ai
 
+A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). 
+
 _Microlog_ is a continuous profiler and logger for the Python language that
 explains application behavior using interactive graphs and AI. 
 It makes understanding complex applications easy, reducing support costs
 and shortening production problems, increasing application quality, and minimizing outages.
 
 _Microlog_ has extremely low runtime overhead (~1%) and exceptionally fast rendering (~20ms).
 It saves logs and performance profiles on the local file system. The logs are
@@ -642,15 +644,15 @@
 
 # The Microlog.ai UI 
 
 A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). The UI is
 written almost entirely in Python, see [dashboard](dashboard). The _Microlog_ UI runs in the browser using PyScript. 
 
 To describe the UI features of _Microlog_, we will look at the output of the [examples\memory.py](examples\memory.py) example (the live preview is at
-[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_26_14_11_38/)):
+[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_31_11_16_19/)):
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
 
 The main elements of the UI are:
 
  - `Log list`, at the left, showing currently available logs on the local machine.
  - `Timeline`, the starting point for analysis of your application:
```

### Comparing `micrologai-1.3.3/README.md` & `micrologai-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # microlog.ai
 
+A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). 
+
 _Microlog_ is a continuous profiler and logger for the Python language that
 explains application behavior using interactive graphs and AI. 
 It makes understanding complex applications easy, reducing support costs
 and shortening production problems, increasing application quality, and minimizing outages.
 
 _Microlog_ has extremely low runtime overhead (~1%) and exceptionally fast rendering (~20ms).
 It saves logs and performance profiles on the local file system. The logs are
@@ -69,15 +71,15 @@
 
 # The Microlog.ai UI 
 
 A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). The UI is
 written almost entirely in Python, see [dashboard](dashboard). The _Microlog_ UI runs in the browser using PyScript. 
 
 To describe the UI features of _Microlog_, we will look at the output of the [examples\memory.py](examples\memory.py) example (the live preview is at
-[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_26_14_11_38/)):
+[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_31_11_16_19/)):
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
 
 The main elements of the UI are:
 
  - `Log list`, at the left, showing currently available logs on the local machine.
  - `Timeline`, the starting point for analysis of your application:
```

### Comparing `micrologai-1.3.3/dashboard/canvas.py` & `micrologai-1.3.4/dashboard/canvas.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/colors.py` & `micrologai-1.3.4/dashboard/colors.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/config.py` & `micrologai-1.3.4/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/design.py` & `micrologai-1.3.4/dashboard/design.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/dialog.py` & `micrologai-1.3.4/dashboard/dialog.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/main.py` & `micrologai-1.3.4/dashboard/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,32 +92,32 @@
 
     @profiler.profile("Flamegraph.convertLog")
     def convertLog(self, log):
         self.calls = [ CallView(self.flameCanvas, model) for model in log.log.calls ]
         self.statuses = [ StatusView(self.timelineCanvas, model) for model in log.log.statuses ]
         self.markers = [ MarkerView(self.timelineCanvas, model) for model in log.log.markers ]
 
-    @profiler.profile("Flamegraph.showStatus")
-    def showStatus(self, logEntries, index):
+    @profiler.profile("Flamegraph.addMarkerToLogTab")
+    def addMarkerToLogTab(self, logEntries, index):
         if self.statuses and index < len(self.statuses):
             logEntries.append((self.statuses[index].when, str(self.statuses[index]), ""))
 
     @profiler.report("Flamegraph.load")
     def load(self, log):
         self.convertLog(log)
         statusIndex = 0
         logEntries = []
-        self.showStatus(logEntries, 0)
+        self.addMarkerToLogTab(logEntries, 0)
         for marker in self.markers:
             while self.statuses[statusIndex].when < marker.when and statusIndex < len(self.statuses) - 1:
                 statusIndex += 1
             logEntries.append((marker.when, markdown.toHTML(marker.message), marker.formatStack(full=False)))
-            self.showStatus(logEntries, statusIndex)
+            self.addMarkerToLogTab(logEntries, statusIndex)
         self.addLogEntries(logEntries)
-        self.showStatus(logEntries, -1)
+        self.addMarkerToLogTab(logEntries, -1)
         self.hover = None
         js.jQuery(self.flameElementId).empty()
         js.jQuery(self.timelineElementId).empty()
    
     @profiler.report("Redrawing the whole UI.")
     def redraw(self, event=None):
         if self.currentTab == "Timeline":
@@ -247,15 +247,14 @@
     def clickTimeline(self, x, y):
         self.clickCanvas(self.timelineCanvas, self.markers, x, y)
 
     def clickCanvas(self, canvas, views, x, y):
         x, y, _, _ = canvas.absolute(x, y)
         for view in views:
             if view.inside(x, y):
-                print("click", x, y, view)
                 view.click(x, y)
                 return True
         dialog.hide()
 
 
 def setUrl(log=None):
     if not "Electron" in js.navigator.userAgent:
@@ -326,17 +325,20 @@
     if not any(logList):
         js.jQuery(".logs").empty().append(js.jQuery("<span>").css("color", "pink").text("No matching logs found")),
         return
     def tree():
         return defaultdict(tree)
     logs = tree()
     for log in [log for log in reversed(logList) if log]:
-        application, name = log.split("/")
-        if application != "-":
-            logs[application][name.replace(".log", "")]
+        try:
+            application, name = log.split("/")
+            if application != "-":
+                logs[application][name.replace(".log", "")]
+        except:
+            print("Error: Cannot handle", log)
     TreeView(
         js.jQuery(".logs").empty(),
         logs,
         getLogFromUrl(),
         lambda path: showLog(path),
         lambda path, doneHandler: deleteLog(path, doneHandler),
         refreshLogs
@@ -359,28 +361,28 @@
 def setupLogHandlers():
     js.jQuery(".refresh").click(pyodide.ffi.create_proxy(refreshLogs))
     js.jQuery(".filter").keyup(pyodide.ffi.create_proxy(refreshLogs))
 
 
 def resize(event=None):
     flamegraph.reset()
-    height = js.jQuery(js.window).height() - 55
+    height = js.jQuery(js.window).height() - 2
     filterHeight = js.jQuery("#filter").height() + 36
     tabHeight = height - js.jQuery(".tabs-header").height()
     padding = 24
     js.jQuery("body").css("height", height)
     js.jQuery(".main").css("height", height)
     js.jQuery(".tabs").css("height", height)
     width = js.jQuery(".tabs").width()
     flamegraph.resize(width, tabHeight - padding)
     js.jQuery("#tabs-tracing").css("height", tabHeight)
     js.jQuery("#tabs-design").css("height", tabHeight)
     js.jQuery("#tabs-log").css("height", tabHeight)
     js.jQuery("#tabs-explain").css("height", tabHeight)
-    js.jQuery(".logs").css("height", height - filterHeight)
+    js.jQuery(".logs").css("height", height - filterHeight - 2)
     js.jQuery(".tree").css("height", height - filterHeight - padding)
 
 def main():
     setupLogHandlers()
     showAllLogs()
     loadLog(getLogFromUrl())
     js.jQuery(js.window).on("resize", pyodide.ffi.create_proxy(resize))
```

### Comparing `micrologai-1.3.3/dashboard/markdown.py` & `micrologai-1.3.4/dashboard/markdown.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/profiler.py` & `micrologai-1.3.4/dashboard/profiler.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/tips.py` & `micrologai-1.3.4/dashboard/tips.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 for provider, url in SEARCH_URLS.items()
             ])
     
     def createButton(self, provider, logo, url):
         return (js.jQuery("<button>")
             .addClass("tips-button")
             .append(
-                js.jQuery("<img>").addClass("tips-logo").attr("src", logo),
+                js.jQuery("<img>").addClass("tips-logo").attr("src", f"/microlog/{logo}"),
                 js.jQuery("<span>").text(provider),
             )
             .click(pyodide.ffi.create_proxy(lambda event: self.open(url)))
         )
 
     def open(self, url):
         print("Tips", self.modules, url)
```

### Comparing `micrologai-1.3.3/dashboard/treeview.py` & `micrologai-1.3.4/dashboard/treeview.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 #
 # Microlog. Copyright (c) 2023 laffra, dcharbon. All rights reserved.
 #
 
 from __future__ import annotations
 
-import builtins
 import js # type: ignore
-import json
 import pyodide # type: ignore
-import traceback
 
 from typing import List
 
 
 class TreeView():
     instance = None
 
@@ -49,14 +46,15 @@
                             .addClass("tree-delete-icon") \
                             .html(f"🗑") \
                             .click(pyodide.ffi.create_proxy(lambda event: self.delete(js.jQuery(event.target).parent()))) 
                     )
                 )
                 add(js.jQuery("<div>").appendTo(node), path + [label], children, depth+1)
         add(parent, [], items)
+        self.scrollIntoView(js.jQuery(".tree-selected"))
 
     def keyDown(self, event):
         if event.keyCode in [38, 40]: 
             index = int(js.jQuery(".tree-selected").attr("index")) or 0
             direction = -1 if event.keyCode == 38 else 1
             index += direction
             selected = js.jQuery(f".tree-leaf[index='{index}']")
@@ -89,16 +87,20 @@
         if int(node.attr("children")):
             if node.hasClass("closed"):
                 self.openNode(node)
             else:
                 self.closeNode(node)
         else:
             self.selectNode(node)
-        
 
     def selectNode(self, node):
         js.jQuery(".tree-selected").removeClass("tree-selected")
         node.addClass("tree-selected")
         self.selectionHandler(f"{node.attr('path')}/{node.attr('label')}")
+        self.scrollIntoView(node)
+    
+    def scrollIntoView(self, node):
+        if not node.isInViewport():
+            node[0].scrollIntoView()
     
 
 js.jQuery("body").on("keydown", pyodide.ffi.create_proxy(lambda event: TreeView.instance.keyDown(event)))
```

### Comparing `micrologai-1.3.3/dashboard/views/__init__.py` & `micrologai-1.3.4/dashboard/views/__init__.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/views/call.py` & `micrologai-1.3.4/dashboard/views/call.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/views/marker.py` & `micrologai-1.3.4/dashboard/views/marker.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     images = {
         api.config.EVENT_KIND_INFO:  js.jQuery("#marker-info"),
         api.config.EVENT_KIND_WARN:  js.jQuery("#marker-warn"),
         api.config.EVENT_KIND_DEBUG: js.jQuery("#marker-debug"),
         api.config.EVENT_KIND_ERROR: js.jQuery("#marker-error"),
     }
     offset = {
-        api.config.EVENT_KIND_INFO:  0,
-        api.config.EVENT_KIND_ERROR: 24,
-        api.config.EVENT_KIND_WARN:  48,
-        api.config.EVENT_KIND_DEBUG: 72,
+        api.config.EVENT_KIND_INFO:  4,
+        api.config.EVENT_KIND_ERROR: 28,
+        api.config.EVENT_KIND_WARN:  53,
+        api.config.EVENT_KIND_DEBUG: 76,
     }
     instances = []
 
     @profiler.profile("StatusView.__init__")
     def __init__(self, canvas, model):
         View.__init__(self, canvas, model)
         self.image = self.images[self.kind]
@@ -84,17 +84,17 @@
     def mouseenter(self, x, y):
         View.mouseenter(self, x, y)
         self.select()
     
     def select(self):
         self.draw()
         (js.jQuery("#marker-highlight")
+            .attr("index", self.index)
             .css("left", self.canvas.toScreenX(self.x))
             .css("top", self.canvas.toScreenY(self.y) + 42)
-            .click(pyodide.ffi.create_proxy(lambda event: self.click(0, 0)))
             .appendTo(self.canvas.canvas.parent()))
 
     def mouseleave(self, x, y):
         View.mouseleave(self, x, y)
 
     def formatStack(self, full=True):
         def shortFile(filename):
@@ -106,15 +106,14 @@
             return f"<a href=vscode://file/{callSite.filename}:{callSite.lineno}:1>{shortFile(callSite.filename)}:{callSite.lineno}</a>\n"
         return ''.join([
               addLink(callSite)
               for callSite in self.stack
         ])
 
     def click(self, x, y):
-        # self.canvas.redraw()
         self.select()
         formattedStack = self.formatStack()
         stack = f"""
             <h2>Callstack</h2>
             <pre>{formattedStack}</pre>
         """ if formattedStack else ""
 
@@ -141,7 +140,17 @@
         js.jQuery("#show-log").click(
             pyodide.ffi.create_proxy(lambda event:
                 self.showLog()))
     
     def showLog(self):
         dialog.hide()
         js.jQuery('a[href="#tabs-log"]').click()
+
+
+def clickMarker(event):
+    index = int(js.jQuery("#marker-highlight").attr("index"))
+    x = event.originalEvent.offsetX
+    y = event.originalEvent.offsetY
+    MarkerView.instances[index].click(x, y)
+
+
+js.jQuery("#marker-highlight").click(pyodide.ffi.create_proxy(clickMarker))
```

### Comparing `micrologai-1.3.3/dashboard/views/status.py` & `micrologai-1.3.4/dashboard/views/status.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/dashboard/views/timeline.py` & `micrologai-1.3.4/dashboard/views/timeline.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/binaryTrees.py` & `micrologai-1.3.4/examples/binaryTrees.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/books.json` & `micrologai-1.3.4/examples/books.json`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/bookstore.py` & `micrologai-1.3.4/examples/bookstore.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/dataframes.py` & `micrologai-1.3.4/examples/dataframes.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/example.py` & `micrologai-1.3.4/examples/example.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/files.py` & `micrologai-1.3.4/examples/files.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/go.py` & `micrologai-1.3.4/examples/go.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/helloworld.py` & `micrologai-1.3.4/examples/helloworld.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/memory.py` & `micrologai-1.3.4/examples/memory.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,33 +2,37 @@
 # Microlog. Copyright (c) 2023 laffra, dcharbon. All rights reserved.
 #
 
 import sys
 sys.path.insert(0, ".")
 
 from collections import Counter
+from collections import defaultdict
 import gc
 import time
 import microlog
 
+start_counter = Counter(type(obj).__name__ for obj in gc.get_objects())
+
 def showMemoryInfo():
     top10 = "\n".join(
-        f"- {name}: {count:,}"
+        f"- {count} objects of type \"{name}\", which is {count - start_counter[name]:+,} since the start"
         for name, count in Counter(type(obj).__name__ for obj in gc.get_objects()).most_common(10)
     )
     print(f"# Python Heap Details\n\nThe top ten of {len(gc.get_objects()):,} live objects:\n{top10}")
 
 
 class MemoryLeak():
     def __init__(self):
         self.memory = f"{time.time()}" * 10000
 
 
 def allocate1GB(run):
     takeShortPauze()
+    showMemoryInfo()
     return [MemoryLeak() for n in range(10000)]
 
 
 def takeShortPauze():
     time.sleep(0.2)
 
 
@@ -52,8 +56,10 @@
         gc.collect()
         showMemoryInfo()
 
     gc.collect()
     showMemoryInfo()
 
 
+forced_leak = MemoryLeak()
+
 main()
```

### Comparing `micrologai-1.3.3/examples/modules.py` & `micrologai-1.3.4/examples/modules.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,47 +20,34 @@
         loadModule(name)
         duration = round(time.time() - start, 1)
         msg = api.info if duration < 0.3 else api.error
         msg(f"{name} - {len(sys.modules) - moduleCount} modules - {duration}s")
     except:
         pass
 
-load('attrs')
 load('bleach')
 load('certifi')
 load('click')
 load('cycler')
 load('decorator')
 load('docutils')
 load('exceptiongroup')
 load('fsspec')
 load('idna')
 load('iniconfig')
 load('jedi')
-load('joblib')
 load('kiwisolver')
 load('matplotlib')
 load('mpmath')
 load('multidict')
 load('networkx')
 load('nltk')
-load('numpy')
-load('packaging')
 load('pandas')
-load('parso')
 load('pluggy')
 load('py')
 load('pydantic')
-load('pyparsing')
 load('pytest')
-load('pytz')
-load('regex')
-load('scipy')
-load('setuptools')
-load('six')
 load('sqlalchemy')
 load('sympy')
-load('threadpoolctl')
 load('tomli')
 load('tqdm')
-load('webencodings')
 load('yarl')
```

### Comparing `micrologai-1.3.3/examples/startstop.py` & `micrologai-1.3.4/examples/startstop.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/threads.py` & `micrologai-1.3.4/examples/threads.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/examples/treemap.ipynb` & `micrologai-1.3.4/examples/treemap.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992283950617284%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': "*

 * *            "['/Users/laffra/microlog/logs/ipykernel_launcher/2023_07_31_11_16_32.log\\n', '📈 "*

 * *            'Microlog ··· 3.9s ··· 8.9KB ··· ipykernel_launcher ··· '*

 * *            "http://127.0.0.1:4000/log/ipykernel_launcher/2023_07_31_11_16_32 🚀\\n']}}}, 1: "*

 * *            "{'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAgMAAAGbCAYAAABZBpPkAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAA […]*

```diff
@@ -5,15 +5,16 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\ud83d\udcc8 Microlog \u00b7\u00b7\u00b7 2.2s \u00b7\u00b7\u00b7 4.1KB \u00b7\u00b7\u00b7 ipykernel_launcher \u00b7\u00b7\u00b7 http://127.0.0.1:4000/log/ipykernel_launcher/0.0.0/2023_07_24_13_09_18 \ud83d\ude80\n"
+                        "/Users/laffra/microlog/logs/ipykernel_launcher/2023_07_31_11_16_32.log\n",
+                        "\ud83d\udcc8 Microlog \u00b7\u00b7\u00b7 3.9s \u00b7\u00b7\u00b7 8.9KB \u00b7\u00b7\u00b7 ipykernel_launcher \u00b7\u00b7\u00b7 http://127.0.0.1:4000/log/ipykernel_launcher/2023_07_31_11_16_32 \ud83d\ude80\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
                 "import microlog\n",
                 "microlog.start(\"Treemap-Jupyter-Notebook\")"
@@ -22,25 +23,24 @@
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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7dpVLVu21KJFizRgwAB17NhRo0aNUtOmTZWdna2srCzFxMTorbfeuqg5p6ena/369Ro4cKASExN17NgxzZ8/X82aNdNNN91U7uMee+wxDRgwQDfeeKPGjBnju7SwTp06mjlz5kXN4Up45JFHlJWVpa5du+ruu+9Whw4ddPLkSW3evFlr1671RdBdd92l5cuXa9y4ccrKylKPHj1UXFysXbt2afny5crMzKySL5JKSkpS69at9atf/UrZ2dmKiYnRypUrA84dKFWjRg2tWbNGqamp6tq1q1avXq23335bDz30ULmfo5+rXbt2GjNmjD755BM1atRIL774oo4eParFixcHbDty5Ej99re/VVZWVqUv9Vy2bJkyMjI0ZMgQdenSRREREdq5c6defPFF1ahRw+97Ks43atQoSdKPf/xjvfTSS373lf6/MnnyZK1atUqDBg1SWlqaunTpovz8fG3fvl2vv/66Dhw4oLi4uErNFbigIF3FgKvQhS4t1L8uySsqKnLXX3+9a9asWcDlV08//bST5F577TXf2Jtvvuk6dOjgwsLCAi7r++yzz9ytt97q6tev7yIjI11iYqIbPny4e++993zblF7Sd/5laKVzLb3k7b333nO33HKLa9KkiYuIiHBNmjRxt99+u98lXWVdWuicc2vXrnU9evRwNWvWdDExMW7w4MHuiy++8NumsvOojPIuLZwwYUKZ2x89etRNmDDBNW/e3IWHh7vGjRu7lJQUt2DBAr/tCgsL3dy5c13Hjh1dZGSkq1u3ruvSpYubNWuWO3369AWPVfrcPPbYY37jWVlZTpJbsWKFb+yLL75wffr0cbVq1XJxcXHu7rvvdlu3bg14blNTU110dLT78ssv3U9+8hMXFRXlGjVq5GbMmOGKi4srfJ4SExPdwIEDXWZmpuvcubOLjIx0SUlJfnM5X8eOHV1ISIj76quvKty/c85t27bNTZ482f3oRz9y9erVc2FhYS4+Pt4NGzbMbd682W/b8y8tLL30sbz/V0p98803burUqa5NmzYuIiLCxcXFue7du7vHH3/cFRYWVmqeQEU8zlXBmUsAUMXS0tL0+uuvV+s/9nPttdeqXr16Ad+OCVztOGcAACT97W9/05YtW/xObASs4JwBAKbt2LFDn376qZ544gnFx8drxIgRwZ4SUO1YGQBg2uuvv65Ro0bp7NmzeuWVV/iXHmES5wwAAGAcKwMAABhHDAAAYFylTyDsX2f0lZwHAFxxO59oH+wpAOX6c7/yv4nzcnRq/lWF27AyAACAccQAAADGEQMAABhHDAAAYBwxAACAccQAAAD/YTonZKtzQnaV7Y8YAADAOGIAAADj+FcLAQA+h+6eUuZ43NMzlTNxpiQpYeGjZT6mdLysfZz/GFTOtS2zVVzsPzb7iTq+2+d/VPDq23XVoVPURR+HlQEAQJlCmzby3c6ZOFORP0iSJP3j/87yjX81+X8lSeGtEiX5h0Bos3h5akdXx1SvSg9MyPGFwHXdwtQsoeQl+2yh/78v2KZdqML+9db+5wNPXdKxWBkAAASIe3qmoqJK3mGWvsA3mjhah+6eIvdNvm87b26eJCl+6gS/x7MScPk+/bhQktS1e7gWvtrQ7770qSXP+58/qKuEhJK/p8s5oZCVAQBAgNIQkCSFlLxUFOTkfH972+cq2LPf7zHHFy8vuRERXi1zvNq9uDJWkvTRprO+qweeeSzXb5vSELhcxAAAoNLipk2SJOU8u1Q5j78gSao/7i5JUnhCk2BN66qUkBClv+6qq9ox348tfCZfabcdrfJjEQMAgAvzeiVJUXFxikpoXDLmvh+P7tJJkhSbclPJfYVnq3uGV62oqCht3NFU2w411Z8/qCtJ2vxJUZUfh3MGAAABDt09RaFNG6n4cOC70NDmTVT8j8MlP0SXvUx96O4pCm3eRO6bb+TN/YZzCC7Bj5OzlXtSqt9AuqZ9uD7aWBJZ4RHS2cKqPRYrAwCAMhVnHy1ZAVDJCYWlmk6f5LudMG+m32POfdEv/sdheXO/uYIzvLrVqxcqSTpxXNq0/qzvyoJP9zat8mOxMgAACHChd/IFBQWX/FhU3p/WNS73vm2HAoOgrLHKIgYAAJWW89JKFfy/jyRJtX7aO8izQVXhYwIAQKWVhoAk1RvSP4gzQVViZQAA4FPREj8fAVydWBkAAMA4YgAAAOOIAQAAjOOcAQBmRMb+M9hTAMp120e/uCL73d284m1YGQAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAXLQ9w6Zrz7DpwZ4GqkhYsCcAAPjPE3tHitzZ4mBPA1WEGAAAXLQGQ3oFewqoQsQAAOCilX5E0HZFuvaMmCF5nd/9ceP/S3V7/0gFOd8qe/yj/g8OD1Xbl2dIkg5OX6TCnYekkBDJ6/Vt4omuoTZLHrqyvwR8OGcAAHDJsp96zRcCEe0TFNqoriTJFZV8hOALAY8U3rxhye2zxTowZb7/jrxeKSxE4YmNSh6f/08VHDp+5X8BSGJlAABwGf6586AkKbJjCyXMHF3udm2Xp/tu7xk2XWf3Hwnc5pWZkqT9//1bFX2do6PzXlXLJ39ZtRNGmVgZAABcsvjflATAd58f8F1hcPTVtZKknLc+kCR5akZUuB9PnWjf7ajuHSRJxTmnq3q6KAcxAAC4ZFEN4tR06YPyREX6xvJWrtfBXy+8qP2EhIX6bntCSl6anHPlbY4qRgwAAC5LVFSU2iydprYr0tV0/n9Lkgp3/UNxg2+SJLkzhcGcHiqBcwYAAJds75iH5fLOKKROtMITGum7z/eX3BHm/15zz/DpCm/WUGf/cUySFN6ycXVPFRfAygAA4JKF1ir5rN97Ol/fbd/nu7Kg9GTAps9NKdnQyRcCCg9Vi0fvre6p4gI8rpIfyvSvU/5ZogDwn2Df71sGewpXjXO/ZwD/3nYP/XWF2/AxAQCg0goOHdfRx18J9jRQxYgBAEClHZmzVMUn8iRJMbf9OMizQVUhBgAAldbq+V8Fewq4AjiBEAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGMBly8xbrMy8xUE45pJqPSYAXK3Cgj0B/OdLCOuoSEUHexoAgEtEDOCytY+6IdhTAABcBmIAl630I4J+MaPK/bigX8yogG1L5RTk6NOityq9j++587b1qF9M2sX/AgBgHOcM4IqJVqzv9jt5SyVJoYqQJH32bZbvvk+L/ixJSgrrVsY+6gbso/zjOG3IW3kZMwYAm1gZwBVx7rv4zLzFcvJKkvrE/B9l5i3WMe+Bc7Z2kqTEqPaV2seFtilQXhXMHgBsYWUAQbX12/WSpFC6FACChhhAtWseWrICsDYvQ0e8X0qS+sTcFcwpAYBpxACqXYfoknMDilUY5JkAACTOGcAVkpm3WNGKVb5yJUme87rToxDfOQANPIlVdpwo1b7kfQGAVawM4IopfYGWpJ/EpPrdd1PYMN/tH9XuXWXH6Rkz9LL2BQAWsTKAyxZ4/X/ZY+c6roP/uuW5pP1VtH+gLEVnQ4M9BeDfEjGAalVQUKC93k/1tXevJOnGsEFBnhEAgBhAtdpelKVcHZMkhShUMVFxQZ4RAIAYQJWqaPm+a8zAapoJAKCyOIEQAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMC4s2BMAAFwd9t8xrczxRoum6ejY30iSWr78mzIfc/44qhcrAwCAKhfWrKHv9tGxv1Hkte0kSQfGzfGNH7zvEUlSeNtm1Ts5BCAGAABVqtGiaWr+6ES/d/tNJqdKklxevm/Me/IbSVKzWeOrd4IIwMcEAIAqFRUV9f0PISGS16uCnBzf7fzNO+WJqhm8CSIAKwMAgGrRaM4vJUnHnnhJR/93kSQpbuLtwZwS/oWVAQDAleP1SpKi4uK+H3OSnJMk1e76gyBMCucjBgAAVWr/HdMU1qyhirKPBdwX1qKxig4cKfmhVlTA/QgOPiYAAFS5oq+OlawAqOSEwlLN//VRgSS1XFD2pYiofqwMAACq1IW+M6CgoKAaZ4LKIgYAANXi2O//pPz3PpEk1b6lV5Bng3PxMQEAoFqUhoA8UtyInwR3MvDDygAAoEpU9JXCfOXwvy9WBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMI4YAADAOGIAAADjiAEAAIwjBgAAMM7jnHPBngQAAAgeVgYAADCOGAAAwDhiAAAA44gBAACMIwYAADCOGAAAwDhiAAAA44gBAACMIwYAADDu/wNo1zb13/iLjAAAAABJRU5ErkJggg==",
+                        "image/png": "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b76pqVOnaufOnUpNTdWkSZM0evRoxcbG+p0KuFhOTo569eql3NxcffTRRwoLC/Ou27lzpzZv3lzqvxfgchEDCJj09HTvG3vBxWelUfCT+4svvljkLYcFt3MVCA4OLnS7gp/cKlWqpFWrViktLU2fffaZlixZog8//FCdO3fW0qVLi3z+pSppHFfiwp+4pfOv00MPPVRkOLVq1cq77XXXXafJkycXut3Fb/JFfR8lfX+5ubnq0qWLjh8/rqeffloJCQmKiIjQgQMHlJycHLCL4nr37q358+dr7dq1uu6667Ro0SINHjy4yBAsjMfjUdOmTdW0aVN1795d11xzjVJSUkqMgWHDhumLL77Q8uXLVa9ePZ91eXl56tKli4YPH17ocwvCBrhSxAACIi8vT8nJyYqMjNTjjz+u5557Tvfee6/uvvtu7zZFfZBO48aNJeVP+d52221lNqagoCAlJSUpKSlJkydP1nPPPadRo0YpLS2t0OPExcVJkr799lu/ddu3b1d0dLTPrEB5i4mJUZUqVZSbm1vi69S4cWNt2rRJSUlJV/UDjLZs2aIdO3Zozpw56t27t3f5smXLCt0+Ly9P6enpPm96O3bskKRSfZrfrl275Jzz+Z4Ke/4dd9yhmJgYpaSkqG3btsrKytLDDz98Kd+aj/j4eFWrVk2HDh0qdrsPPvhAr7zyil555RV16tTJb33jxo115syZMv13DhSGawYQEJMnT9batWs1ffp0TZgwQe3bt9egQYN87kIoeCM9efKkz3Nbt26txo0b66WXXir0E96OHTt2yeM5fvy437KCWYeLb60rEBsbq8TERM2ZM8dnjFu3btXSpUv1i1/84pLHUZaCg4N1zz33aOHChdq6davf+gtfp169eunAgQN6++23/bY7d+6czp49W2ZjknxnQpxzevXVV4t8zuuvv+6z7euvv64KFSooKSmpxOMdPHhQf/nLX7xfnz59Wu+8844SExNVu3Zt7/KQkBA98MADmjdvnmbPnq3rrrvOO2tSnHXr1hX62qxfv16ZmZmFnkIqsHXrVg0YMEAPPfSQHnvssUK36dWrl7744gulpqb6rTt58qRycnJKHCNQGswMoMwtXrxY27dv91vevn17xcfHa9u2bXr22WeVnJysnj17Ssr/KOPExEQNHjxY8+bNk5T/U1FUVJSmTZumKlWqKCIiQm3b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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "import sys\n",
                 "import squarify\n",
                 "import folderstats\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "\n",
                 "for n in range(10):\n",
                 "    df = folderstats.folderstats('./', ignore_hidden=True)\n",
@@ -89,15 +89,15 @@
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjkAAAHkCAYAAADcoz4BAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABEwklEQVR4nO3deVxWdd7/8ffFomwioiIqiltolkLllpoglhumWJYz2mhptmjdLTNNVnab3TZm5czUWOnkfmepkUuu5YKODm65oJiKigsuJE6CIqYs5/eHP67bS0DBxOviy+v5ePDQ65zvOedznS/C2+8553vZLMuyBAAAYBg3ZxcAAABQFgg5AADASIQcAABgJEIOAAAwEiEHAAAYiZADAACMRMgBAABGIuQAAAAjEXIAAICRCDmAi1q7dq1sNpveeecdZ5dyy9hsNkVFRTnt+A0aNFCDBg0cls2YMUM2m00zZsxwSk0FnH1urnXkyBHZbDY9+eSTzi6lRFylH+FaCDlwKTab7YZfa9euven9P/nkk7LZbDpy5Mgtq7kiKQheV3/5+Piodu3a6tSpk1577TXt2LGjTI5d3n7pXquogIXi5eXl6YsvvlBkZKQCAwPl6empoKAgtWzZUk8//bS+++47Z5eIcsDD2QUARRk9enSx6yrKL4o2bdpo7969qlGjhrNLKSQ0NNQeNi5fvqz09HRt375dH330kT766CMNGDBAkydPlp+fn8N2e/fulY+PjxMqvmL16tVOO/aNOPvcuJK8vDz16tVLK1asUEBAgGJiYhQSEqLLly9rz549+uqrr7Rv3z717t3bvk3fvn3Vrl071a5d24mVw9UQcuCSTLpEc7N8fHzUrFkzZ5dRpAYNGhTZRzt37tSgQYP01Vdf6ZdfftHy5csd1jv7/TRu3Nipx78eZ58bV/L1119rxYoVCg8P17p161S1alWH9dnZ2dq8ebPDsqpVqxZqB3C5CuXW4cOHFRAQoMDAQB09etRh3YULF3TnnXfK3d3dfnnLZrNp5syZkqSGDRvaL7dcOzL0yy+/6I033tCdd94pb29vVa1aVV26dNEPP/xQqIar7wOIj49XVFSUqlSpIn9/f8XExGjv3r2Ftvn555/1pz/9SU2bNpWvr68CAgLUtGlTPfnkk0pJSbG3u949OQcOHNCgQYNUt25dVapUSXXq1NGgQYN04MCBQm3feecd+2W+uLg4tWnTRj4+PgoMDNTvfvc7nThx4kanusQiIiK0atUq1axZUytWrNDChQsd1hd138n58+f1P//zP7r77rvl7++vKlWqqHHjxurfv7+2bdtmfw8NGzaUJM2cOdPhclnBPRhXn68tW7YoJiZGgYGBDpcnb3TJaOnSpWrfvr18fX1VrVo19evXr8hzGhUVJZvNVuQ+rr03pKCuo0eP6ujRow61X33prbh7cjIzM/XGG2+oadOm8vLyUrVq1dStWzetWrWqUNurz8HOnTsVExOjgIAA+fj4KDIyUgkJCcW+9+vZt2+fYmNjFRgYKF9fX3Xs2LHQv4fJkyfLZrNpzJgxRe4jLS1Nnp6eatGixQ2PV1Dnk08+WWRw8fHxUefOnR2WFXVPTsHl6eK+ivpe+Prrr9W5c2cFBATIy8tLd955p8aOHatLly7dsG64HkZyUG41bNhQU6ZM0WOPPaYBAwZo3bp18vC48i09fPhw7du3T++88479F8fo0aO1cOFCJSYm6qWXXlJAQIAk2f+UpKNHjyoqKkpHjhzRAw88oO7du+vChQtasmSJunfvrsmTJ2vYsGGFalmyZIkWLVqkHj166LnnntNPP/2kZcuWaevWrfrpp5/sl5yys7PVoUMHHTp0SA899JAefvhhWZalo0ePatGiRerXr58aNWp03fe9detWPfjggzp//rx69+6t5s2ba9++ffryyy+1aNEirVq1Sq1bty603WeffabvvvtOvXv3VmRkpDZv3qy5c+cqMTFRO3fuVOXKlW+iFwoLCgrSs88+q7Fjx2r27NmKjY0ttq1lWerevbsSEhJ0//336+mnn5aHh4eOHz+u+Ph4PfDAA7rvvvsUFRWljIwMffzxxwoPD3fYZ0REhMM+N27cqHHjxqljx44aMmSIzpw5o0qVKt2w7vnz52v58uXq27evoqKitHPnTn377beKj49XQkKCmjZtelPno0GDBho9erT+/ve/S5JefvnlYmu/VkZGhjp06KCffvpJrVu31ssvv6wzZ85o3rx56tq1qz7//HM9++yzhbb78ccf9cEHH9jP6bFjx/Ttt9+qS5cu2rlzZ6ney+HDh3X//ferRYsWevbZZ3Xq1CnNnTtXPXr00FdffaX+/ftLkgYOHKg///nPmjp1qkaNGiV3d3eH/UybNk25ublF1nut6tWrS5KSk5NLXGdRYmNjiwwyu3fv1vz58wtdHhwyZIimT5+ukJAQPfroowoICNCmTZv09ttva/Xq1Vq5cqX9ZwzKCQtwIZIsSdbo0aOL/Bo3blyhbZ5//nlLkjVy5EjLsixrxowZliSrc+fOVl5enkPbwYMHW5Ksw4cPF3n8yMhIy2azWV9//bXD8rNnz1rh4eGWl5eXlZaWZl8+ffp0S5Ll7u5urVq1ymGbkSNHWpKs8ePH25d99913liTr5ZdfLnTsS5cuWefOnbO/jo+Pt5+LAvn5+VazZs0sSdaXX37psP2cOXMsSVbTpk0d3vfo0aMtSVaVKlWsXbt2OWzz+9//3pJkzZ07t8jzca2CmiIjI6/bbtWqVZYkq379+g7Lr912165dliQrNja20D7y8vKsX375xf768OHDliRr8ODB161NkjVp0qQi24SGhlqhoaEOywr6UJK1ePFih3V///vfLUlWdHS0w/LIyEiruB+fBfubPn36DY99taLO6zPPPGNJsp555hkrPz/fvjw5Odny9/e3KlWq5PC9fPU5uPb4kyZNsiRZzz//fLE1XK3gfEuy/vSnPzms27p1q+Xh4WEFBARYmZmZ9uUjRowo8jzm5+dbDRs2tHx8fKyMjIwbHnv79u2Wp6enZbPZrCeeeML69ttvrSNHjlx3m+LO+7VSU1OtunXrWl5eXtbGjRsLbd+3b18rOzvbYZuCf0N///vfb1g7XAshBy6l4IdqcV9Vq1YttM3Fixet8PBwy2azWf/4xz8sX19fq2bNmtbJkycLtb1eyNm5c6clyerXr1+RtS1cuNCSZH366af2ZQU/GAcOHFiofUpKiiXJevTRR+3LCkLOG2+8ccNzUVTI2bBhgyXJuv/++4vcpmPHjpYka926dfZlBT+g33rrrULt16xZY0my/vjHP96wnqtrulHI2bt3ryXJ8vb2dlheXMj5/e9/f8NjlzTkREREFLuP64Wca4OMZVlWbm6u1bhxY0uSwy/Z2xFyLl26ZPn4+Fh+fn7Wf/7zn0LtR40aZUmyxowZY19WcA46dOhQqP3ly5ctDw8P67777iu2hqsVnO+qVas6hO8CBf+WZsyYYV+WlJRkSbJ69erl0HbFihWWJOupp54q0bEty7Lmzp1rBQcHO/z7DwwMtGJjY63vvvuuUPuShJxz585ZLVu2tGw2m/XNN984rIuIiLA8PDyss2fPFtouNzfXql69utW6desS1w/XwLgbXJJlWSVu6+Xlpblz56pVq1Z68cUXZbPZFBcXV+qnLDZu3Cjpyj0QRd0Hk56eLklF3mfTqlWrQsvq1asnSTp79qx9WWRkpOrWrav3339f27dvV8+ePdWhQwdFREQUGt4vyvbt2yVJ0dHRRa6Pjo7Whg0btGPHDnXq1OmmarwVCvqvuPtWCjRv3lwRERH6+uuvdfToUfXp00cdO3ZUq1atSnSJqSht2rS5qe0iIyMLLXN3d1fHjh116NAh7dixQ6GhoTe175uxf/9+++XNwMDAQuujo6M1duzYIh/ZL6qvPT09VatWrVL39b333qsqVaoUWh4VFaWZM2dqx44dGjx4sCTprrvuUqdOnbR8+XKlpqbav7/++c9/SpKee+65Eh/38ccfV9++fRUfH2//nt6wYYMWLlyohQsXatCgQfb7cEoiLy9Pjz/+uHbt2qUPPvhA/fr1s6/Lzs5WYmKiatSoYb+seK3KlSsX+W8fro2QAyOEhYWpZcuWSkhIUPPmzdW1a9dS7+M///mPJGnlypVauXJlse2ysrIKLbv6vp4CBdfu8/Ly7Mv8/f21adMmjR49Wt99952+//57SVKNGjU0fPhwjRo1Sp6ensUeOzMzU5KKDXAFyzMyMm66xlvh5MmTkqSaNWtet527u7vWrFmjd999V3FxcXr99dclSVWqVNHgwYM1bty4Qo+h30hwcPBN1VyrVq3r7q/g3N8ut7qvpSv9Xdq+Lu15GT58uP71r39pypQpGjNmjNLS0vTdd98pIiKi1AHU09NTXbt2tf97zsvL07fffqshQ4Zo1qxZ6tu373Xv+braiBEjtGLFCj377LN67bXXHNadPXtWlmUpPT292BunUT7xdBWM8P777yshIUE1atTQnj17NG7cuFLvo+Apjo8//ljWlUu5RX5Nnz79N9UaEhKiqVOn6vTp00pKStInn3yi6tWr691339W7775bohrT0tKKXH/q1CmHds4SHx8vSWrbtu0N21arVk1/+9vflJqaqgMHDmjKlClq1qyZJk6cqOeff77Uxy7p/+yv9fPPPxe5vOBcX31O3dyu/OjMzc0t1L6o0HEzXKWvS3NeJOmRRx5RrVq1NHXqVOXl5ZXqhuMbcXd31+OPP65XXnlFkrRmzZoSbffBBx9o8uTJ6tGjhz799NNC6wvewz333HPdf/ulGWGGayDkoNxLSEjQf//3f6tp06ZKSkpS06ZNNXr0aG3YsKFQ24JLQkX9b7Zdu3aSpPXr15dtwf+fzWbTXXfdpRdffNE+cnTtI9fXuueeeySp2FmfC8LFvffee8vqLK3Tp09r8uTJkq48cVMaTZo00dChQ7Vu3Tr5+flp0aJF9nXX67tbYd26dYWW5eXl2b+PCs69dCWYSVJqamqhbX788cci9+/u7l6q2ps2bSofHx8lJiYWGZxuV19v375d58+fL7S84Hvw6vMiXRl9efrpp3XixAktXrxYU6ZMkZ+fX6m/F66n4PJZSUJHXFycRo4cqfDwcM2dO7fIy8J+fn666667tGfPHv3yyy+3rE44HyEH5drZs2f1+9//Xu7u7pozZ45q1aqluXPnysPDQwMGDCj0A6vg0dRjx44V2lerVq30wAMPaP78+Zo2bVqRx9u9e7dOnz590/Xu2bOnyP8ZFyy70Yy3HTp0UNOmTbVhwwbFxcU5rIuLi9P69esVFhamjh073nSNv0ViYqIeeughnTlzRj179nSYkbYohw8fdpgbqMDZs2d16dIleXt725dVq1ZNNputyL67FdasWaMlS5Y4LJs4caIOHTqkzp07O9yPU3DZ5YsvvnBov3r1an399ddF7r969epKT0/XxYsXS1RPpUqVNHDgQJ0/f15vv/22w7pDhw7pk08+kaenp/7whz+UaH83KzMzs9AI448//qjZs2eratWq6tu3b6FtnnnmGbm7u+uFF17Q4cOHNWDAgCLv6ynO119/rZUrVyo/P7/QurS0NPt5v/a+s2tt3LhRf/jDH1SnTh0tXbr0ujW8+uqrunz5soYMGVJkqDx79qz9njiUH9yTA5d0vRmPY2Nj7fOLDBkyRMeOHdMnn3xiXxYeHq4JEybohRde0JNPPunwGTddunTRhx9+qGHDhunRRx9VlSpVFBAQoBdeeEGS9NVXXyk6OlpDhw7VJ598orZt2yogIEDHjx/Xrl27lJSUpI0bNyooKOim3tfKlSv12muv6f7771dYWJiCgoJ0/PhxLVq0SG5uboXuFbhWwYSGDz30kPr3768+ffqoWbNm2r9/vxYuXKgqVapo1qxZ9sspZeXIkSP2PsrJydGZM2e0bds2++R9TzzxhCZNmnTD/SQmJuqRRx5R69atdeedd6pOnTpKT0/XokWLlJOTY79HR7ryv+22bdtq/fr1GjhwoMLCwuTu7q7evXurZcuWv/k9Pfzww+rbt6/69u2rJk2aaOfOnVq+fLkCAwP12WefObR96qmn9OGHH2rcuHFKTExU8+bNlZycbJ9n59tvvy20/y5dumjr1q3q3r27OnXqpMqVKys8PFwPP/xwsTW9//77Wr9+vSZOnKitW7eqc+fO9nlyzp8/r4kTJ9onSSwrnTp10pQpU7R582Z16NDBPk9Ofn6+Jk+eLH9//0Lb1K9fXzExMfZ/e6W9VLV582Z9/PHHCg4OVseOHe3v8fDhw1q6dKkuXryoPn36ONw8XJShQ4fq119/Vdu2bQsFUunKvUsF8xYNGTJE27Zt02effabGjRurW7duql+/vn755RcdPnxY//rXv/TUU0+V6PsaLuQ2P80FXJdu8Ai5rnpE9JNPPrEkWb179y5yX3379rUkWX/9618dlk+YMMFq1qyZValSJUtSocd6z507Z7333nvWvffea/n6+lpeXl5WgwYNrJ49e1qTJ0+2srKy7G1v9Niqrnks+KeffrJeeeUV67777rNq1KhhVapUyQoNDbUeffRR69///rfDtkU9Ql5g37591hNPPGEFBwdbHh4eVnBwsDVw4EBr3759hdoWPEIeHx9faN2NHsu+1tXzsBR8eXl5WcHBwdYDDzxg/elPf7J27NhR7PbXno/U1FTrjTfesNq3b2/VqlXLqlSpklW3bl2re/fu1rJlywptf+DAAatXr15WYGCgZbPZHM799c5Xges9Qj59+nRr8eLFVrt27SwfHx+ratWq1iOPPGLt37+/yH0lJSVZPXr0sPz8/CxfX18rMjLSWrt2bbHfE1lZWdZzzz1n1a1b13J3dy903q89NwXOnj1r/fnPf7aaNGliVapUyapatar14IMPWt9//32htjc6Bzd6jP1qV39v/PTTT1bv3r2tgIAAy9vb22rfvr21YsWK625fMOVCq1atSnS8qx07dsyaOHGiFRsba4WFhVlVqlSxPD09reDgYKtHjx7W//7v/xaaA6uo8x4aGnrdnyVFnYvFixdbMTExVs2aNS1PT0+rVq1aVuvWra233nrL2rt3b6nfC5zLZlncSQUAuLXeeecdjRkzRlOmTNHQoUOdXQ4qKEIOAOCWOn/+vO644w7l5OQoNTWVT1eH03BPDgDglli6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Z968eercubNq1uTTg53ltddeU+3atfX444+rWrVqstlsDut9fHycVFnFNW3aNAUHB6tnz54Oy1esWKG0tDQ9+eSTzimsAsrPz9fatWu1e/fuIkc6R48e7aTKyh735JRDmzZt0h//+EelpKQoNDRUoaGhOnz4sP74xz9q06ZNzi6vwtm6datefPFFvfvuu9qwYUO5/2T78igtLU0DBgxQSEiIfH195ePj4/CF22/z5s1q1qxZoeVhYWH8nLrNpk+frunTpys/P1/16tWz/94o+DIZl6vKodmzZys2Nlb9+/d3WD5v3jzNnj1b7dq1c1JlFdOHH36ow4cPKz4+XtOnT9fUqVPVvn17de7cWU2aNHF2eRVCkyZNlJaWpuDgYGeXgv8vKyuryIDp4+Oj8+fPO6GiiishIUGvvPKK7r33XmeXctsRcsqhs2fPKjIystDyBx54QN99950TKkLDhg3VsGFDDRo0SNu2bVN8fLzefvtt1a1bV9HR0YqKimJEoQz16NFDs2bNUkZGhurXry93d3eH9ab/b9UVBQcHa+fOnerevbvD8h07digoKMhJVVVMHh4eFfY/AISccuiuu+7S3r17C33T7tu3T3feeaeTqkKBvLw85eXlSZJ8fX21YsUKzZ07V88++6zat2/v5OrMNGHCBEnS559/XuR6bjy+/WJiYjRt2jSdO3dOd999tyRp9+7dWrJkiQYPHuzk6iqWXr16admyZRo6dGih+9VMx43H5cSPP/5o//svv/yiefPm6f7779cdd9whSTpw4IA2bdqkxx57TF27dnVWmRVWSkqK4uPj9e9//1uenp7q1KmTunTpYg+iy5cv1/z58/XFF184uVIzFfdUVQFuCneOH374QfPnz9fZs2clXemHxx57rMiRaNxaH330kcPrpKQk+fn5KSQkRB4ejuMbf/rTn25nabcVIaecuPb+m+vhf6231x//+EedPHlSLVu2VJcuXdSqVSu5uTne03/u3DkNGzaMvkGFdO7cOVWqVEleXl7OLqXC+Oyzz0rcdvjw4WVYiXMRcoDfKC4uTtHR0QoMDFTBP6eKNiTsCtLS0rRs2TKHaRV69uxZYe9FcDamVnAdly9fVn5+vj1knj59Wlu3blXdunUVERHh3OLKGCEHuAXWrFmjpUuX6tSpU5Kk2rVrq2fPnurSpYuTK6sYdu7cqQ8++EANGjRQ06ZNJUn79+/X0aNH9frrr6tly5ZOrrDiee2115SamqrmzZsrOjpabdu2laenp7PLqpDGjh2rNm3aqGvXrrpw4YJefvlleXh46Ny5cxo8eLDRtzhw43E5tXv37mIndjJ56NEVzZ07V0uWLFGPHj0UFhYm6coMvDNnztSZM2dKdakRN+err75STEyMBg4c6LB89uzZmj17NiHHCZhawXUcPnzYfrP3pk2bFBAQoPHjx2vz5s2aN28eIQeu5ZtvvlFcXJwaN26sgIAALo042Q8//KBnn31WHTt2tC9r1aqV6tevr+nTpxNyboMTJ07olVdeKbS8c+fOWrZsmRMqgsTUCq7i0qVL8vb2liQlJiaqTZs2cnNz0x133HHDm/bLO0JOObRy5UqNGDFCnTp1cnYp0JVHxhs3blxoeaNGjeyPkqNs+fv768iRI6pdu7bD8iNHjsjf399JVeFqTK3gPMHBwdqyZYvatGmjxMRE9erVS9KVG8ILwo+pCDnlUG5urv2yCJyvU6dO+uGHHwrN/bFq1SqH0R2UnS5duuif//ynfv75Z4d7chYtWqSYmBgnV1dxFTW1wtChQx2mVpg+fTohp4z169dPH3/8sWbOnKkWLVrYf38kJiaqYcOGTq6ubHHjcTn05ZdfysvLS/369XN2KdCVDyJct26datSo4TBv0ZkzZxQZGekw+y6ToJUNy7K0dOlSLVmyxD4nS7Vq1dS7d2/16NGDS7pOwNQKriUjI0Nnz55VaGiovR8OHjwob29v1a1b18nVlR1CTjk0ffp0/etf/1L9+vUVGhpaaAp7fpHeXmPGjClxW5M/7ddVXLx4UZKMH4Z3dUytAFdAyCmHbvRLlV+kqGguX74sy7JUuXJlSVdmQN6yZYtCQkIUHh7u5OoqLqZWgLMRcgCUexV5HhBXVdzUCitWrFBMTAxPHeK2cLtxE7ia+Ph4Xb582dllAC7j8OHD9g+nLZgH5NNPP9ULL7yg5cuXO7m6iqlgaoUBAwaoVatWatWqlQYMGKBnnnlGP/zwg7PLQwVByCmHvvrqKw0bNkyff/659u/f7+xyAKeryPOAuCqmVoArIOSUQ5MmTdKIESN0/vx5vfPOO3r55Ze1cOFCZWRkOLs0wCkK5gE5c+aMEhMT7ffhVIR5QFxVwdQK12JqBdxO3JNTzmVkZGj9+vVat26dTpw4oYiICEVHR+u+++4r9LgmYKpNmzbp448/Vn5+vu6++269/fbbkqQFCxZo7969evPNN51cYcXD1ApwBYQcAxw4cEDx8fFat26dAgICdOHCBfn6+mr48OG66667nF0ecFsUzAPSoEED+6PKBw8elI+Pj+rUqePk6ioeplaAKyDklFMZGRn617/+pbVr1+rnn39W69atFR0drZYtW+rXX39VXFycEhIS9Nlnnzm7VKBMfPTRRxo+fLh8fHz00UcfXbetl5eXQkJC1LVrVz4rCahA+FiHcuj9999XYmKi6tSpoy5duigyMlJ+fn729V5eXnr44Ye1ePFiJ1YJlC0fHx/7iM2NgktOTo5Wrlyp/fv36/XXX78d5QFwAYzklEOff/65unTpct3Pr7IsS2fOnFHNmjVvY2WA6zp+/LjeeOMN/e///q+zSwFwmxByAFQI+fn5OnbsmBo0aODsUgDcJoSccmr37t1aunSpTpw4IUmqW7euevbsqZYtWzq5MgAAXAMhpxz6/vvvNWPGDLVt29Z+yerAgQPatGmTBg8erO7duzu5QgAAnI8bj8uhBQsWFBlmmjZtqgULFhByAAAQMx6XSxcuXFBERESh5eHh4crOzr79BQEA4IIIOeVQq1attGXLlkLLt27dqvvuu88JFQEA4Hq4J6cc+vbbb7V48WI1bdrU4Z6c/fv3q1evXg6f1dOzZ09nlQkAgFMRcsqhESNGlKidzWbTxIkTy7gaAABcEyEHAAAYiaeryomZM2eqf//+8vLy0syZM4ttZ7PZNGjQoNtYGQAAromQU04cOXJEeXl59r8DAIDr43IVAAAwEo+QAwAAIxFyAACAkQg5AADASIQcAABgJEIOABRj3rx5evzxx51dBoCbRMgB4DK2b9+uefPmObsMAIbgEXIALmPq1Kn6/vvvXSbo5OXlKS8vT5UqVXJ2KQBuApMBAkAx3N3d5e7u7uwyANwkRnIA/Ga//PKL5syZox07dujChQsKDg5Wr169FB0drcuXL+vPf/6zJOmDDz6wj4pkZWXp1VdfVVBQkN599119/vnnWrduXaF9F4zq5Ofna/ny5Vq9erV+/vln+fj4qHXr1howYID8/Pzs7UeMGKF69eopNjZWM2fO1LFjx1StWjU99thjioyMtLfLzc3VggULtH79ev3nP/9R5cqVVbduXT322GNq2bKl/dhxcXEO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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjkAAAHkCAYAAADcoz4BAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABE4ElEQVR4nO3deXxOd97/8feVhWwitghCIgjVkrS1FZWIKSFKtFoz9KalWqW9p+1Mp9rqrTo6rbZmph1tmdrvatHUUnstYZjYaglRBLGTiiEhomQ5vz/8ct0uiSUqrivfvJ6PRx5c53zPOZ/rfCN5+55zvpfNsixLAAAAhnFzdgEAAAClgZADAACMRMgBAABGIuQAAAAjEXIAAICRCDkAAMBIhBwAAGAkQg4AADASIQcAABiJkAO4qNWrV8tms+mdd95xdil3jM1mU3R0tNOOHxoaqtDQUIdlU6dOlc1m09SpU51SUyFnn5trHTp0SDabTU8//bSzS7klrtKPcC2EHLgUm81206/Vq1ff9v6ffvpp2Ww2HTp06I7VXJ4UBq+rv3x8fFSrVi116NBBr732mrZt21Yqxy5rv3SvVVzAwvXl5+fryy+/VFRUlKpWrSpPT08FBgaqefPmevbZZ/X99987u0SUAR7OLgAozsiRI6+7rrz8omjVqpV2796t6tWrO7uUIkJCQuxh4/Lly8rIyNDWrVv18ccf6+OPP1bfvn01YcIE+fn5OWy3e/du+fj4OKHiK1auXOm0Y9+Ms8+NK8nPz1f37t21dOlSBQQEKC4uTsHBwbp8+bJ27dqlr7/+Wnv27FGPHj3s2/Tq1Utt2rRRrVq1nFg5XA0hBy7JpEs0t8vHx0dNmjRxdhnFCg0NLbaPtm/frv79++vrr7/WmTNntGTJEof1zn4/DRo0cOrxb8TZ58aVfPPNN1q6dKkiIiK0Zs0aVa5c2WF9Tk6ONm7c6LCscuXKRdoBXK5CmXXw4EEFBASoatWqOnz4sMO6Cxcu6J577pG7u7v98pbNZtO0adMkSfXr17dfbrl2ZOjMmTN64403dM8998jb21uVK1dWp06d9MMPPxSp4er7ABITExUdHa1KlSrJ399fcXFx2r17d5Ftfv75Z/3xj39U48aN5evrq4CAADVu3FhPP/200tLS7O1udE/Ovn371L9/f9WpU0cVKlRQ7dq11b9/f+3bt69I23feecd+mS8hIUGtWrWSj4+Pqlatqt/+9rc6fvz4zU71LYuMjNSKFStUo0YNLV26VPPmzXNYX9x9J+fPn9ef//xn3XffffL391elSpXUoEED9enTR1u2bLG/h/r160uSpk2b5nC5rPAejKvP16ZNmxQXF6eqVas6XJ682SWjRYsWqW3btvL19VWVKlXUu3fvYs9pdHS0bDZbsfu49t6QwroOHz6sw4cPO9R+9aW3692Tk5WVpTfeeEONGzeWl5eXqlSpoi5dumjFihVF2l59DrZv3664uDgFBATIx8dHUVFRSkpKuu57v5E9e/YoPj5eVatWla+vr9q3b1/k38OECRNks9k0atSoYveRnp4uT09PNWvW7KbHK6zz6aefLja4+Pj4qGPHjg7Lirsnp/Dy9PW+ivte+Oabb9SxY0cFBATIy8tL99xzj0aPHq1Lly7dtG64HkZyUGbVr19fEydO1BNPPKG+fftqzZo18vC48i09dOhQ7dmzR++88479F8fIkSM1b948JScn6/e//70CAgIkyf6nJB0+fFjR0dE6dOiQHn74YcXGxurChQtauHChYmNjNWHCBA0ePLhILQsXLtT8+fPVtWtXDRkyRD/99JMWL16szZs366effrJfcsrJyVG7du104MABPfLII3r00UdlWZYOHz6s+fPnq3fv3goLC7vh+968ebN+85vf6Pz58+rRo4eaNm2qPXv26KuvvtL8+fO1YsUKtWzZssh2n3/+ub7//nv16NFDUVFR2rhxo2bNmqXk5GRt375dFStWvI1eKCowMFDPP/+8Ro8erRkzZig+Pv66bS3LUmxsrJKSkvTQQw/p2WeflYeHh44dO6bExEQ9/PDDevDBBxUdHa3MzEx98sknioiIcNhnZGSkwz7Xr1+v999/X+3bt9fAgQN1+vRpVahQ4aZ1z5kzR0uWLFGvXr0UHR2t7du367vvvlNiYqKSkpLUuHHj2zofoaGhGjlypP7+979Lkl5++eXr1n6tzMxMtWvXTj/99JNatmypl19+WadPn9bs2bPVuXNnffHFF3r++eeLbPfjjz/qww8/tJ/TI0eO6LvvvlOnTp20ffv2Er2XgwcP6qGHHlKzZs30/PPP6+TJk5o1a5a6du2qr7/+Wn369JEk9evXT3/60580adIkjRgxQu7u7g77mTx5svLy8oqt91rVqlWTJKWmpt5yncWJj48vNsjs3LlTc+bMKXJ5cODAgZoyZYqCg4P1+OOPKyAgQBs2bNDbb7+tlStXavny5fafMSgjLMCFSLIkWSNHjiz26/333y+yzQsvvGBJsoYPH25ZlmVNnTrVkmR17NjRys/Pd2g7YMAAS5J18ODBYo8fFRVl2Ww265tvvnFYfvbsWSsiIsLy8vKy0tPT7cunTJliSbLc3d2tFStWOGwzfPhwS5I1ZswY+7Lvv//ekmS9/PLLRY596dIl69y5c/bXiYmJ9nNRqKCgwGrSpIklyfrqq68ctp85c6YlyWrcuLHD+x45cqQlyapUqZK1Y8cOh21+97vfWZKsWbNmFXs+rlVYU1RU1A3brVixwpJk1atXz2H5tdvu2LHDkmTFx8cX2Ud+fr515swZ++uDBw9akqwBAwbcsDZJ1vjx44ttExISYoWEhDgsK+xDSdaCBQsc1v3973+3JFkxMTEOy6Oioqzr/fgs3N+UKVNueuyrFXden3vuOUuS9dxzz1kFBQX25ampqZa/v79VoUIFh+/lq8/BtccfP368Jcl64YUXrlvD1QrPtyTrj3/8o8O6zZs3Wx4eHlZAQICVlZVlXz5s2LBiz2NBQYFVv359y8fHx8rMzLzpsbdu3Wp5enpaNpvNeuqpp6zvvvvOOnTo0A23ud55v9bRo0etOnXqWF5eXtb69euLbN+rVy8rJyfHYZvCf0N///vfb1o7XAshBy6l8Ifq9b4qV65cZJuLFy9aERERls1ms/7xj39Yvr6+Vo0aNawTJ04UaXujkLN9+3ZLktW7d+9ia5s3b54lyfrss8/sywp/MPbr169I+7S0NEuS9fjjj9uXFYacN95446bnoriQs27dOkuS9dBDDxW7Tfv27S1J1po1a+zLCn9Av/XWW0Xar1q1ypJk/eEPf7hpPVfXdLOQs3v3bkuS5e3t7bD8eiHnd7/73U2PfashJzIy8rr7uFHIuTbIWJZl5eXlWQ0aNLAkOfySvRsh59KlS5aPj4/l5+dn/ec//ynSfsSIEZYka9SoUfZlheegXbt2RdpfvnzZ8vDwsB588MHr1nC1wvNduXJlh/BdqPDf0tSpU+3LUlJSLElW9+7dHdouXbrUkmQ988wzt3Rsy7KsWbNmWUFBQQ7//qtWrWrFx8db33//fZH2txJyzp07ZzVv3tyy2WzWt99+67AuMjLS8vDwsM6ePVtku7y8PKtatWpWy5Ytb7l+uAbG3eCSLMu65bZeXl6aNWuWWrRooZdeekk2m00JCQklfspi/fr1kq7cA1HcfTAZGRmSVOx9Ni1atCiyrG7dupKks2fP2pdFRUWpTp06+uCDD7R161Z169ZN7dq1U2RkZJHh/eJs3bpVkhQTE1Ps+piYGK1bt07btm1Thw4dbqvGO6Gw/65330qhpk2bKjIyUt98840OHz6snj17qn379mrRosUtXWIqTqtWrW5ru6ioqCLL3N3d1b59ex04cEDbtm1TSEjIbe37duzdu9d+ebNq1apF1sfExGj06NHFPrJfXF97enqqZs2aJe7rBx54QJUqVSqyPDo6WtOmTdO2bds0YMAASdK9996rDh06aMmSJTp69Kj9++uf//ynJGnIkCG3fNwnn3xSvXr1UmJiov17et26dZo3b57mzZun/v372+/DuRX5+fl68skntWPHDn344Yfq3bu3fV1OTo6Sk5NVvXp1+2XFa1WsWLHYf/twbYQcGCE8PFzNmzdXUlKSmjZtqs6dO5d4H//5z38kScuXL9fy5cuv2y47O7vIsqvv6ylUeO0+Pz/fvszf318bNmzQyJEj9f3332vZsmWSpOrVq2vo0KEaMWKEPD09r3vsrKwsSbpugCtcnpmZeds13gknTpyQJNWoUeOG7dzd3bVq1Sq9++67SkhI0Ouvvy5JqlSpkgYMGKD333+/yGPoNxMUFHRbNdesWfOG+ys893fLne5r6Up/l7SvS3pehg4dqn/961+aOHGiRo0apfT0dH3//feKjIwscQD19PRU586d7f+e8/Pz9d1332ngwIGaPn26evXqdcN7vq42bNgwLV26VM8//7xee+01h3Vnz56VZVnKyMi47o3TKJt4ugpG+OCDD5SUlKTq1atr165dev/990u8j8KnOD755BNZVy7lFvs1ZcqUX1VrcHCwJk2apFOnTiklJUWffvqpqlWrpnfffVfvvvvuLdWYnp5e7PqTJ086tHOWxMRESVLr1q1v2rZKlSr629/+pqNHj2rfvn2aOHGimjRponHjxumFF14o8bFv9X/21/r555+LXV54rq8+p25uV3505uXlFWlfXOi4Ha7S1yU5L5L02GOPqWbNmpo0aZLy8/NLdMPxzbi7u+vJJ5/UK6+8IklatWrVLW334YcfasKECeratas+++yzIusL38P9999/w3/7JRlhhmsg5KDMS0pK0v/8z/+ocePGSklJUePGjTVy5EitW7euSNvCS0LF/W+2TZs2kqS1a9eWbsH/n81m07333quXXnrJPnJ07SPX17r//vsl6bqzPheGiwceeOCO1VlSp06d0oQJEyRdeeKmJBo2bKhBgwZpzZo18vPz0/z58+3rbtR3d8KaNWuKLMvPz7d/HxWee+lKMJOko0ePFtnmxx9/LHb/7u7uJaq9cePG8vHxUXJycrHB6W719datW3X+/Pkiywu/B68+L9KV0Zdnn31Wx48f14IFCzRx4kT5+fmV+HvhRgovn91K6EhISNDw4cMVERGhWbNmFXtZ2M/PT/fee6927dqlM2fO3LE64XyEHJRpZ8+e1e9+9zu5u7tr5syZqlmzpmbNmiUPDw/17du3yA+swkdTjxw5UmRfLVq00MMPP6w5c+Zo8uTJxR5v586dOnXq1G3Xu2vXrmL/Z1y47GYz3rZr106NGzfWunXrlJCQ4LAuISFBa9euVXh4uNq3b3/bNf4aycnJeuSRR3T69Gl169bNYUba4hw8eNBhbqBCZ8+e1aVLl+Tt7W1fVqVKFdlstmL77k5YtWqVFi5c6LBs3LhxOnDggDp27OhwP07hZZcvv/zSof3KlSv1zTffFLv/atWqKSMjQxcvXryleipUqKB+/frp/Pnzevvttx3WHThwQJ9++qk8PT31X//1X7e0v9uVlZVVZITxxx9/1IwZM1S5cmX16tWryDbPPfec3N3d9eKLL+rgwYPq27dvsff1XM8333yj5cuXq6CgoMi69PR0+3m/9r6za61fv17/9V//pdq1a2vRokU3rOHVV1/V5cuXNXDgwGJD5dmzZ+33xKHs4J4cuKQbzXgcHx9vn19k4MCBOnLkiD799FP7soiICI0dO1Yvvviinn76aYfPuOnUqZM++ugjDR48WI8//rgqVaqkgIAAvfjii5Kkr7/+WjExMRo0aJA+/fRTtW7dWgEBATp27Jh27NihlJQUrV+/XoGBgbf1vpYvX67XXntNDz30kMLDwxUYGKhjx45p/vz5cnNzK3KvwLUKJzR85JFH1KdPH/Xs2VNNmjTR3r17NW/ePFWqVEnTp0+3X04pLYcOHbL3UW5urk6fPq0tW7bYJ+976qmnNH78+JvuJzk5WY899phatmype+65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d67Wrl2r//znP6pYsaLq1KmjJ554Qs2bN7cfOyEhwWFkKT8/X3PnztWaNWv0n//8R1WqVFG7du30xBNPyNPTs8R1ACg9jOQA+FUyMzP11ltvSZK6dOkif39/bd++XePHj9fFixcVFxenYcOG6e2339Y333yjAQMGSJImTpyonJwcDR06VG5ubnrkkUd09uxZ7dixQy+++GKR4/zzn//UmjVrFB0dra5du+rUqVNaunSpDh48qD//+c/y8Pi/H2fp6ekaO3asYmJiFBUVpcTERH3++ecKCwtT3bp1JUnffvut5s2bp5iYGDVs2FAXL17UgQMHlJaWZg85xRk/frzWrFmjNm3aqHv37tq3b5/mzZun48eP67XXXnNoeyt1ACg9hBwAv8rMmTNVUFCgjz/+WJUqVZIkde7cWX//+9/17bff6pFHHlGjRo3Uo0cPzZ8/X61atVJWVpaSkpL09NNPq3bt2pKk8PBw1apVSzt27FCHDh0cjrFnzx6tWrVK//3f/6327dvbl9977736y1/+og0bNjgsP3HihEaNGqV77rlHktS2bVu98MILSkxMtH+A7datW3X//ffr+eefv+X3eujQIa1Zs0YxMTEaMmSIpCvBrnLlylqwYIFSUlJ03333lagOAKWHp6sA3DbLsrRx40Y9+OCDsixL586ds39FRkYqJydHaWlpkqQnn3xSdevW1WeffaaJEyeqadOm6tq16y0dZ/369fLx8VHz5s0djhEWFiYvLy+lpKQ4tA8ODrYHC0ny9/dX7dq1derUKfsyX19fHT16VCdPnrzl97tt2zZJUvfu3R2WP/roo5KuBKeS1gGg9DCSA+C2nTt3ThcuXNCKFSu0YsWK67aRJA8PD73wwgt644035OnpqaFDh8pms93ScdLT05WTk6Nnn332hscoVL169SJtfH19deHCBfvrJ598Uh999JF+//vfq27duoqMjFSHDh0UEhJy3ToyMjJks9kUFBTksDwgIEC+vr46ffp0iesAUHoIOQBuW+FzCw8//PB1b6a9OjQkJydLknJzc3Xy5EkFBgbe0nEKCgpUuXJlvfTSS8Wu9/f3d3jt5lb8IPXVz1k0bdpU//jHP7R582YlJydr1apVWrRokQYPHqxOnTrdsJ5bDWe3UgeA0kPIAXDb/P395e3trYKCghverCtJhw8fVkJCgqKjo3X48GGNHz9eY8eOlY+Pj73N9cJDzZo1tXPnTjVp0uSOzlnj5+enjh07qmPHjvrll180cuRIffvtt9cNOTVq1JBlWTp58qSCg4PtyzMzM3XhwoViR24AOA/35AC4bW5ubmrdurU2btyoI0eOFFlfeBkpLy9Pn3/+uapUqaJnnnlGQ4cOVVZWlqZOnerQvmLFipJU5HJO27ZtVVBQoISEhCLHyM/Pv63LP+fPn3d47eXlpZo1ayo3N/e629x///2SpMWLFzssX7hwoSTpgQceKHEdAEoPIzkAfpW+fftq165deuutt9SpUycFBwcrOztbaWlp2rlzp6ZMmaI5c+bo0KFDevvtt+Xt7a2QkBD17t1bM2fOVJs2bezhICwsTJI0ZcoURUREyM3NTe3atVPTpk31m9/8RvPmzdPhw4fVvHlzubu7Kz09XevXr9czzzyjNm3alKjuV199VU2bNlVYWJj8/Px04MABbdy4UV26dLnuNqGhoYqKitKKFSt04cIFNW3aVPv379eaNWvUsmVLhyerADgfIQfArxIQEKC//OUvSkhI0MaNG7Vs2TJVqlRJdevWVb9+/ZSWlqa5c+eqS5cuDiEgPj5emzdv1oQJE/TXv/5Vvr6+at26tWJjY5WUlKS1a9fKsiy1a9dOkvTcc88pLCxMK1as0DfffCN3d3fVqFFDDz/8sBo3blziurt27aoff/xRO3bsUG5urmrUqKE+ffqoR48eN9xuyJAhqlmzplavXq1NmzYpICBA8fHxeuKJJ0pcA4DSxYzHAADASNyTAwAAjETIAQAARiLkAAAAIxFyAACAkQg5AADASIQcAABgJEIOAAAwEiEHAAAYiZADAACMRMgBAABGIuQAAAAjEXIAAICR/h/iL7CfMKuo+QAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -117,15 +117,15 @@
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAkIAAAIUCAYAAAD2cEPqAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABBzElEQVR4nO3deViU1/3//9cIo4KI4EKAoCAiwRoF06iJ2Gi0iYjGJUtjYz4xQb1q1W5p+q1tbVNbTaVpNmv6iU20xiwfRatBDRqXaBoDqcbEBaMi4oKKcajOUMCFgfn94Y+7GUGjKTg45/m4Lq8w55w59/sm91y+PPcyNo/H4xEAAICBmvm6AAAAAF8hCAEAAGMRhAAAgLEIQgAAwFgEIQAAYCyCEAAAMBZBCAAAGIsgBAAAjEUQAgAAxiIIAbhuDh8+LJvNpscff/yq37Nw4ULZbDYtXLiw0epqDDabTQMHDvR1GQC+AkEIQB02m+2Kf260UNIQtm3bprFjxyo2NlYtWrRQaGiounTpovvuu09//OMfVVFR4esSAXwNgb4uAEDT9fTTT9fbnpKScn0L8bE333xT48aNk8fj0aBBgzR69GgFBQXpyJEj2rJli1avXq37779fCQkJ1nv27t2r4OBgH1YN4GoQhABc1m9/+1tfl+BzlZWVmjJlimw2m9atW6fBgwfXGZObm6v27dt7tSUlJV2vEgH8Fzg1BuC/cv78ec2ePVs9evRQcHCwQkND9a1vfUtZWVnXNE9hYaEeeughhYeHq1WrVurXr5/efffdK77n2LFjmjp1quLj49WiRQu1a9dOI0aM0LZt2+qM/e1vfyubzabNmzfr7bffVt++fRUSEqK4uLgrbiM/P19lZWW69dZb6w1BktSvXz+FhYV5tV16jdDmzZu/8pTj5s2bvebYt2+fHn/8cXXs2FHNmzfXTTfdpEceeUT79++vU8MXX3yhp556SrfccotatWqlsLAw3XLLLXr88cdVVFR0xX0ETMaKEICv7cKFCxoyZIg++OADJSUlacqUKaqsrNSyZcv08MMPa8eOHXrmmWe+cp4DBw7ozjvv1L/+9S8NHTpUKSkpKiws1KhRozR06NB63/Ppp5/q3nvv1enTpzVkyBDdf//9Ki0t1TvvvKP+/ftrxYoVSk9Pr/O+5557TuvXr9d9992nu+++Wy6X64q1tWvXTpJ04sQJVVRUqFWrVlfxm6krLi6u3lONVVVVev7553Xu3DmvU2lr167V/fffr6qqKt13331KSEjQsWPHtHz5cr377rvatGmTbrvtNkkXV61SU1N18OBB3XPPPbrvvvvk8Xh05MgRZWdn68EHH1R8fPzXqhvwex4AuIQkjyTP008/XefP3/72N2vcM88845HkGTp0qKeqqspq/+KLLzyxsbEeSZ6PPvrIaj906JBHkmfcuHFe27vnnns8kjwvvviiV/s777xj1fLl7VZVVXm6dOniadGihWfz5s1e7zl+/LgnOjraExkZ6Tl37pzV/vTTT3skeYKDgz2ffvrpVf8uampqPL179/ZI8iQnJ3vmzp3r+fTTTz3nz5+/4vskeQYMGPCV848bN84jyfPjH//Yajt9+rQnLCzM065dO8+ePXu8xu/evdvTqlUrT69evay2lStX1pmj1vnz5z1lZWVfWQdgKoIQgDpqw0d9f778l3tCQoLHZrN59u7dW2eO1157zSPJ88QTT1ht9QWh4uJijyRP586dPW63u848AwYMqBOEagPSU089VW/9L774okeS591337XaaoNQfWHhqxw5csQzcOBAr9+D3W739OnTxzN79myPy+Wq856rCUIzZszwSPKMHDnSU11dXaf+uXPn1vu+H//4xx5JVkiqDUK/+MUvrnnfANNxagzAZXk8nsv2/fvf/1ZhYaFuvvnmei8MHjRokCTps88+u+I2avv79++vgICAOv0DBw7UBx984NWWl5cnSTpy5Ei9F3QfOHBA0sU7ty49PdanT58r1lOfTp06adOmTdq7d6/Wr1+vTz75RFu3brX+/OUvf9HmzZvVuXPnq57zrbfe0tNPP63bb79db7/9tpo1+88lm7X7t3Pnznr3r6CgwNq/b3zjGxowYIBuvvlmzZ49W59++qnS09OVmpqqlJSUen+nAP6DIATga6m9tiYqKqre/tp2p9N5VfPcdNNN9fZHRkbWafvXv/4lSVq6dOkV5y4vL7+q+a5Wt27d1K1bN+v1vn37lJGRoby8PP3kJz/RO++8c1XzfPDBB8rIyFBsbKxWr15d5zb72v179dVXrzhP7f6Fhobq448/1tNPP62VK1fqvffekyS1b99ekydP1vTp02W32692NwGjEIQAfC1t2rSRJJ08ebLe/pKSEq9xXzXPF198UW9/ffPXvic7O1sjRoy4uoL/fzab7ZrGX0lSUpLeeOMNJSQk6P3337+q9+zbt896DlFOTk69AbB2/3bu3KmePXte1bwxMTGaP3++PB6PPv/8c73//vt6+eWX9bvf/U41NTX6/e9/f/U7BhiE2+cBfC2tW7dWly5ddPz4cetU1Jdt2rRJkqw7my6nV69ekqQtW7aourq6Tv+lt5RL0h133CFJ+vDDD6+17AbXunVrSVc+jVjL4XBo2LBhKi8v19///nd94xvfqHfcf7N/NptN3bt31w9+8AOtX79ekq56pQowEUEIwNeWkZEhj8ejn/3sZ14hprS01FqByMjIuOIcMTExuueee3To0CHNnTvXqy87O7vO9UGSNHLkSHXp0kUvv/yycnJy6p03Ly9PlZWV17pLdRw6dEhz5syp9zZ7j8ejWbNmSZLuuuuuK85z7tw5jRgxQkVFRZo3b95ln0kkSU888YTCwsI0Y8YMbd26tU5/TU2NV0Dcs2dPvStqtW084Rq4PE6NAfjannrqKa1Zs0bZ2dlKTk5Wenq6KisrtXTpUp06dUr/7//9P/Xv3/8r53n55Zd155136sc//rHWrVun5ORkFRYWasWKFbrvvvu0atUqr/F2u13Lly/XkCFDNGzYMPXr108pKSkKDg5WcXGxtm3bpqKiIpWUlPzXIcDlculHP/qRfvaznyk1NVW33nqrWrdurVOnTun9999XUVGRIiIi9Nxzz11xnjlz5ujjjz9WfHz8ZS/yfvzxxxUXF6d27dpp2bJlGj16tO644w4NHjxY3bt3l81mU3FxsfLy8vSvf/1L586dkyStX79eP/vZz3TnnXcqMTFREREROnbsmLKzs9WsWTP97Gc/+69+B4A/IwgB+NqaN2+u9evX6/nnn9fbb7+tP//5zwoMDFRycrJefPFFffe7372qebp27aqPP/5Y06ZN04YNG7R582b17NlT77zzjhwOR50gJEk9e/bUzp079fzzz2v16tX629/+pmbNmikqKkq9evXSjBkz6nztxdfRrVs3rVixQuvWrdPHH3+sJUuW6PTp0woODlZCQoJ+9atf6Uc/+pE6dOhwxXlqV6eKioo0Y8aMescMHDjQetL14MGDtWvXLv3pT3/Se++9pw8//FDNmzdXdHS0Bg0apAceeMB635AhQ3T06FH94x//UHZ2tsrKyhQVFaV77rlHTz75pPr1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i4v1q1/9SsePH9eoUaP0P//zP2rRooWeffZZbd269br8LgA0DFaEANww4uLi9P3vf996XV5erk2bNunRRx+VJM2YMUPNmze3+tPS0jRr1iy9++67SktL85rrxIkTmjlzphITEyVJMTExmjVrlubNm6cXX3xR7du3lySFhITor3/9q/bu3avu3btLkhYuXKj27dvrD3/4g+x2uyRpyJAh+s1vfqO33npLffr0abxfAoAGxYoQgBvGPffc4/U6KSlJ//73v1VZWSlJXiGosrJSZWVl+sY3vqEvvvjCGlMrJibGCkGS1LVrV0nSrbfeaoUgSUpISJAkffHFF5Iuhq/8/HzdeeedOnv2rMrKylRWVqZ///vfSk5OVklJiU6fPt2Aew2gMbEiBOCG8eWAIl1crZGkiooKBQcHa9++fVq6dKkKCgp0/vx5r7GVlZUKDg6+7Fy1fe3atau3vaKiQtLFU2oej0dLlizRkiVL6q3T5XKpbdu217p7AHyAIATghnG5bwj3eDw6efKkfv/73ys6OlqPPfaY2rVrp8DAQH322Wd69913va7xudJcV9qGJGue++67T8nJyfWOjYyMvKr9AeB7BCEAfmH79u2qqqrSz3/+c6/Vnj179jTodm666SZJUkBAgHr27NmgcwO4/rhGCIBfqF3JqV25kS6eDtu8eXODbqdNmzbq3r27NmzYoDNnztTpLysra9DtAWhcrAgB8AvJyckKDAxUZmamvv3tb+vcuXPauHGjQkND6w0s/43x48fr17/+tZ566ikNHjxYERERcrlcKigo0OnTp/Xss8826PYANB5WhAD4hejoaD355JOy2Wx64403tH79en37299Wenp6g28rJiZGs2fPVq9evbR582bNnz9f69evl81m0wMPPNDg2wPQeGyeL68jAwAAGIQVIQAAYCyCEAAAMBZBCAAAGIsgBAAAjEUQAgAAxiIIAQAAYxGEAACAsQhCAADAWAQhAABgLIIQAAAwFkEIAAAYiyAEAACMRRACAADG+v8AzrIJQCiCoTwAAAAASUVORK5CYII=",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAkIAAAIUCAYAAAD2cEPqAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABB1klEQVR4nO3de1RU1/3//9cIo4KI4IUAQUFEgjUKplETsdFoExGNl1waG/OJCeqqVXtL02/9tLaprabSNDdr+olNtMZcqmg1qEHjJZrGQKox8YJREfGCinGozlDACwPz+8MfpxlBoyk4OPv5WMsVzt579nkfcmb5cp8zZ2wej8cjAAAAAzXzdQEAAAC+QhACAADGIggBAABjEYQAAICxCEIAAMBYBCEAAGAsghAAADAWQQgAABiLIAQAAIxFEAJw3Rw+fFg2m02PP/74Vb9m4cKFstlsWrhwYaPV1RhsNpsGDhzo6zIAfAWCEIA6bDbbFf/caKGkIWzbtk1jx45VbGysWrRoodDQUHXp0kX33Xef/vCHP6iiosLXJQL4GgJ9XQCApuvpp5+utz0lJeX6FuJjb775psaNGyePx6NBgwZp9OjRCgoK0pEjR7RlyxatXr1a999/vxISEqzX7N27V8HBwT6sGsDVIAgBuKzf/OY3vi7B5yorKzVlyhTZbDatW7dOgwcPrjMmNzdX7du392pLSkq6XiUC+C9waQzAf+X8+fOaPXu2evTooeDgYIWGhupb3/qWsrKyrmmewsJCPfTQQwoPD1erVq3Ur18/vfvuu1d8zbFjxzR16lTFx8erRYsWateunUaMGKFt27bVGfub3/xGNptNmzdv1ttvv62+ffsqJCREcXFxV9xHfn6+ysrKdOutt9YbgiSpX79+CgsL82q79B6hzZs3f+Ulx82bN3vNsW/fPj3++OPq2LGjmjdvrptuukmPPPKI9u/fX6eGL774Qk899ZRuueUWtWrVSmFhYbrlllv0+OOPq6io6IrHCJiMFSEAX9uFCxc0ZMgQffDBB0pKStKUKVNUWVmpZcuW6eGHH9aOHTv0zDPPfOU8Bw4c0J133ql//etfGjp0qFJSUlRYWKhRo0Zp6NCh9b7m008/1b333qvTp09ryJAhuv/++1VaWqp33nlH/fv314oVK5Senl7ndc8995zWr1+v++67T3fffbdcLtcVa2vXrp0k6cSJE6qoqFCrVq2u4jdTV1xcXL2XGquqqvT888/r3LlzXpfS1q5dq/vvv19VVVW67777lJCQoGPHjmn58uV69913tWnTJt12222SLq5apaam6uDBg7rnnnt03333yePx6MiRI8rOztaDDz6o+Pj4r1U34Pc8AHAJSR5JnqeffrrOn7/+9a/WuGeeecYjyTN06FBPVVWV1f7FF194YmNjPZI8H330kdV+6NAhjyTPuHHjvPZ3zz33eCR5XnzxRa/2d955x6rly/utqqrydOnSxdOiRQvP5s2bvV5z/PhxT3R0tCcyMtJz7tw5q/3pp5/2SPIEBwd7Pv3006v+XdTU1Hh69+7tkeRJTk72zJ071/Ppp596zp8/f8XXSfIMGDDgK+cfN26cR5Lnxz/+sdV2+vRpT1hYmKddu3aePXv2eI3fvXu3p1WrVp5evXpZbStXrqwzR63z5897ysrKvrIOwFQEIQB11IaP+v58+S/3hIQEj81m8+zdu7fOHK+99ppHkueJJ56w2uoLQsXFxR5Jns6dO3vcbnedeQYMGFAnCNUGpKeeeqre+l988UWPJM+7775rtdUGofrCwlc5cuSIZ+DAgV6/B7vd7unTp49n9uzZHpfLVec1VxOEZsyY4ZHkGTlypKe6urpO/XPnzq33dT/+8Y89kqyQVBuE/vd///eajw0wHZfGAFyWx+O5bN+///1vFRYW6uabb673xuBBgwZJkj777LMr7qO2v3///goICKjTP3DgQH3wwQdebXl5eZKkI0eO1HtD94EDByRd/OTWpZfH+vTpc8V66tOpUydt2rRJe/fu1fr16/XJJ59o69at1p8///nP2rx5szp37nzVc7711lt6+umndfvtt+vtt99Ws2b/uWWz9vh27txZ7/EVFBRYx/eNb3xDAwYM0M0336zZs2fr008/VXp6ulJTU5WSklLv7xTAfxCEAHwttffWREVF1dtf2+50Oq9qnptuuqne/sjIyDpt//rXvyRJS5cuveLc5eXlVzXf1erWrZu6detmbe/bt08ZGRnKy8vTT37yE73zzjtXNc8HH3ygjIwMxcbGavXq1XU+Zl97fK+++uoV56k9vtDQUH388cd6+umntXLlSr333nuSpPbt22vy5MmaPn267Hb71R4mYBSCEICvpU2bNpKkkydP1ttfUlLiNe6r5vniiy/q7a9v/trX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0AsvvKCamhrrtcXFxfrlL3+p48ePa9SoUfqf//kftWjRQs8++6y2bt16XX4XABoGK0IAbhhxcXH6/ve/b22Xl5dr06ZNevTRRyVJM2bMUPPmza3+tLQ0zZo1S++++67S0tK85jpx4oRmzpypxMRESVJMTIxmzZqlefPm6cUXX1T79u0lSSEhIfrLX/6ivXv3qnv37pKkhQsXqn379vr9738vu90uSRoyZIh+/etf66233lKfPn0a75cAoEGxIgTghnHPPfd4bSclJenf//63KisrJckrBFVWVqqsrEzf+MY39MUXX1hjasXExFghSJK6du0qSbr11lutECRJCQkJkqQvvvhC0sXwlZ+frzvvvFNnz55VWVmZysrK9O9//1vJyckqKSnR6dOnG/CoATQmVoQA3DC+HFCki6s1klRRUaHg4GDt27dPS5cuVUFBgc6fP+81trKyUsHBwZedq7avXbt29bZXVFRIunhJzePxaMmSJVqyZEm9dbpcLrVt2/ZaDw+ADxCEANwwLvcN4R6PRydPntTvfvc7RUdH67HHHlO7du0UGBiozz77TO+++67XPT5XmutK+5BkzXPfffcpOTm53rGRkZFXdTwAfI8gBMAvbN++XVVVVfr5z3/utdqzZ8+eBt3PTTfdJEkKCAhQz549G3RuANcf9wgB8Au1Kzm1KzfSxcthmzdvbtD9tGnTRt27d9eGDRt05syZOv1lZWUNuj8AjYsVIQB+ITk5WYGBgcrMzNS3v/1tnTt3Ths3blRoaGi9geW/MX78eP3qV7/SU089pcGDBysiIkIul0sFBQU6ffq0nn322QbdH4DGw4oQAL8QHR2tJ598UjabTW+88YbWr1+vb3/720pPT2/wfcXExGj27Nnq1auXNm/erPnz52v9+vWy2Wx64IEHGnx/ABqPzfPldWQAAACDsCIEAACMRRACAADGIggBAABjEYQAAICxCEIAAMBYBCEAAGAsghAAADAWQQgAABiLIAQAAIxFEAIAAMYiCAEAAGMRhAAAgLEIQgAAwFj/H+dNCc1K3SGBAAAAAElFTkSuQmCC",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -147,15 +147,15 @@
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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2qOPPhonTpyIu+66K2/7doHH4THc/0FCvlnDFLvRsoaH5QKPFwqeJUuWxK/8yq9c8ENm8620tDSqq6ujqampN4y6u7ujqakpstnssM0BABSvQZ98fT6TJk3K+xWl29vbo6Wlpff24cOHo7m5OcrLy2Pq1KmxbNmy2Lx5c1RXV0dNTU08++yz0dHREYsXL87rHADA6JRzGD322GORyWTij//4j6OkpCQee+yxj3xOJpOJW2+9dVADnum1116LdevW9d6ur6+PiIhFixbFmjVr4uqrr462trZ44oknorW1NWbNmhX33nvvWSdkAwCcS85htGfPnshkMtHd3R0lJSWxZ8+ej3xOfy+q9FHmzZsXTzzxxAUfk81m837orKGhIRobG6OysjLq6uryum0AYOQY8MnXY5mTr4fHaDnpj7HLGqbYjZY1PCwnX3/Y22+/Hf/xH/8Rra2tcfnll8fixYtj4sSJ+do8AMCQ61cYNTQ0xHPPPRfr16/v89EfL730UnznO9/pczXo5557LjZs2DCkHxECAJBP/bry9UsvvRTTp0/vEzunTp2K73//+1FSUhK33nprbNq0KW688cY4evRoPPXUU3kfGABgqPQrjN56662YM2dOn/v27NkTbW1t8du//duxePHiuOKKK+IrX/lKLFy4MH7yk5/kdVgAgKHUrzD63//93/j4xz/e577//u//jojoc7XpiIhf+IVfiKNHjw5yPACA4dOvMDrzA1lPe+WVV2LcuHFRVVXV5/7S0tIoLR2y60cCAORdv8Kouro6nn/++Th58mRERLz55puxf//+uOqqq+Kiiy7q89i33377rHeXAABGsn69pXPdddfFPffcE1//+tfjiiuuiAMHDkRExIoVK8567Isvvhjz5s3Lz5QF5gKPADA29CuMPvGJT8S3vvWteOqpp+Lw4cMxZ86c+PKXvxzV1dV9Hrdnz564+OKLY+HChXkdtlCG4mraAMDI48rXA+DK18NjtFxxlbHLGqbYjZY13J8rX/frHCMAgNFMGAEAJMIIACARRgAAiTACAEiEEQBA4jM7cuACjwAwNgijHLjAIwCMDQ6lAQAkwggAIBFGAACJMAIASIQRAEAijAAAEmEEAJAIIwCARBgBACTCCAAg8ZEgOfBZaQAwNgijHPisNAAYGxxKAwBIhBEAQCKMAAASYQQAkAgjAIBEGAEA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",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -194,15 +194,16 @@
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\ud83d\udcc8 Microlog \u00b7\u00b7\u00b7 9.7s \u00b7\u00b7\u00b7 10.9KB \u00b7\u00b7\u00b7 Treemap-Jupyter-Notebook \u00b7\u00b7\u00b7 http://127.0.0.1:4000/log/Treemap-Jupyter-Notebook/0.0.0/2023_07_24_13_09_28 \ud83d\ude80\n"
+                        "/Users/laffra/microlog/logs/Treemap-Jupyter-Notebook/2023_07_31_11_16_42.log\n",
+                        "\ud83d\udcc8 Microlog \u00b7\u00b7\u00b7 9.6s \u00b7\u00b7\u00b7 19.4KB \u00b7\u00b7\u00b7 Treemap-Jupyter-Notebook \u00b7\u00b7\u00b7 http://127.0.0.1:4000/log/Treemap-Jupyter-Notebook/2023_07_31_11_16_42 \ud83d\ude80\n"
                     ]
                 }
             ],
             "source": [
                 "microlog.stop()"
             ]
         }
```

### Comparing `micrologai-1.3.3/microlog/api.py` & `micrologai-1.3.4/microlog/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 
     def stop(self):
         if not self.running:
             return
         from microlog import log
         try:
             self.tracer.stop()
-            self.tracer.join()
+            if self.tracer.is_alive():
+                self.tracer.join()
             log.log.stop()
             self.startServer()
         except Exception as e:
             sys.stderr.write(f"microlog.stop, error {e}")
             raise e
         finally:
             self.running = False
```

### Comparing `micrologai-1.3.3/microlog/config.py` & `micrologai-1.3.4/microlog/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #
 # Microlog. Copyright (c) 2023 laffra, dcharbon. All rights reserved.
 #
 
 import os
-import time
+import signal
 
 EVENT_KIND_SECTION = "#"
 EVENT_KIND_CALL = 1
 EVENT_KIND_STATUS = 2
 EVENT_KIND_INFO = 3
 EVENT_KIND_WARN = 4
 EVENT_KIND_DEBUG = 5
@@ -27,18 +27,22 @@
     "Error",
     "Callsite",
     "Marker",
     "Stack",
     "Symbol",
 ]
 
-statusDelay: float = float(os.environ.get("MICROLOG_STATUS_DELAY", 0.1))
-sampleDelay: float = float(os.environ.get("MICROLOG_SAMPLE_DELAY", 0.1))
+TRACER_STATUS_DELAY = float(os.environ.get("MICROLOG_STATUS_DELAY", 0.1))
+TRACER_SAMPLE_DELAY = float(os.environ.get("MICROLOG_SAMPLE_DELAY", 0.05))
+TRACER_SIGNAL_KIND = signal.SIGPROF
+TRACER_TIMER_KIND = signal.ITIMER_PROF
+
 
 IGNORE_MODULES = [
     "microlog.api",
     "microlog.tracer",
     "microlog.microlog",
+    "microlog.models",
     "microlog",
 ] 
 
 application = ""
```

### Comparing `micrologai-1.3.3/microlog/explain.py` & `micrologai-1.3.4/microlog/explain.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/anomaly.png` & `micrologai-1.3.4/microlog/images/anomaly.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/apple-touch-icon.png` & `micrologai-1.3.4/microlog/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/chatgpt.png` & `micrologai-1.3.4/microlog/images/chatgpt.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/design-go.png` & `micrologai-1.3.4/microlog/images/design-go.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/dialog.png` & `micrologai-1.3.4/microlog/images/dialog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/error-log.png` & `micrologai-1.3.4/microlog/images/error-log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/favicon-32x32.png` & `micrologai-1.3.4/microlog/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/fd-leak.png` & `micrologai-1.3.4/microlog/images/fd-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/asyncio.png` & `micrologai-1.3.4/microlog/images/icons/asyncio.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/dataclasses.png` & `micrologai-1.3.4/microlog/images/icons/dataclasses.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/email.png` & `micrologai-1.3.4/microlog/images/icons/email.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/google.png` & `micrologai-1.3.4/microlog/images/icons/google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/guppy.png` & `micrologai-1.3.4/microlog/images/icons/guppy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/http.png` & `micrologai-1.3.4/microlog/images/icons/http.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/jupyter.png` & `micrologai-1.3.4/microlog/images/icons/jupyter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/matplotlib.png` & `micrologai-1.3.4/microlog/images/icons/matplotlib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/microlog.png` & `micrologai-1.3.4/microlog/images/icons/microlog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/networkx.png` & `micrologai-1.3.4/microlog/images/icons/networkx.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/numpy.png` & `micrologai-1.3.4/microlog/images/icons/numpy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/pandas.png` & `micrologai-1.3.4/microlog/images/icons/pandas.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/pyparsing.png` & `micrologai-1.3.4/microlog/images/icons/pyparsing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/pytest.png` & `micrologai-1.3.4/microlog/images/icons/pytest.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/python.png` & `micrologai-1.3.4/microlog/images/icons/python.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/re.png` & `micrologai-1.3.4/microlog/images/icons/re.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/squarify.png` & `micrologai-1.3.4/microlog/images/icons/squarify.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/ssl.png` & `micrologai-1.3.4/microlog/images/icons/ssl.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/tornado.png` & `micrologai-1.3.4/microlog/images/icons/tornado.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/urllib.png` & `micrologai-1.3.4/microlog/images/icons/urllib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/wsgi.png` & `micrologai-1.3.4/microlog/images/icons/wsgi.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/icons/zmq.png` & `micrologai-1.3.4/microlog/images/icons/zmq.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/log.png` & `micrologai-1.3.4/microlog/images/log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/logo-bing.png` & `micrologai-1.3.4/microlog/images/logo-bing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/logo-brave.png` & `micrologai-1.3.4/microlog/images/logo-brave.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/logo-duckduckgo.png` & `micrologai-1.3.4/microlog/images/logo-duckduckgo.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/logo-google.png` & `micrologai-1.3.4/microlog/images/logo-google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/logo-hackernews.png` & `micrologai-1.3.4/microlog/images/logo-hackernews.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/logo-sourcegraph.png` & `micrologai-1.3.4/microlog/images/logo-sourcegraph.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/logo-stackoverflow.png` & `micrologai-1.3.4/microlog/images/logo-stackoverflow.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/logo-twitter.png` & `micrologai-1.3.4/microlog/images/logo-twitter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/markdown.png` & `micrologai-1.3.4/microlog/images/markdown.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/memory-leak.png` & `micrologai-1.3.4/microlog/images/memory-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/overview.png` & `micrologai-1.3.4/microlog/images/overview.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/status.png` & `micrologai-1.3.4/microlog/images/status.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/tips.png` & `micrologai-1.3.4/microlog/images/tips.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/images/zoomedin.png` & `micrologai-1.3.4/microlog/images/zoomedin.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/microlog/log.py` & `micrologai-1.3.4/microlog/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     def now(self):
         return time.perf_counter() - self.begin
 
     def addCall(self, call: Call):
         if not self.running: 
             return
         self.calls.append(call)
+        if len(self.calls) % 10000 == 0:
+            sys.stdout.write(f"{len(self.calls)} calls\n")
 
     def addStatus(self, status: Status):
         self.statuses.append(status)
 
     def addMarker(self, marker: Marker):
         self.markers.append(marker)
 
@@ -126,17 +128,21 @@
     return filename.replace("/", "_")
 
 
 def getApplication():
     from microlog import config
     if config.application:
          return config.application
-    name = sys.argv[0] if sys.argv[0] != "-c" else sys.argv[1] if sys.argv[0] == "-m" else "python"
+    name = sys.argv[0]
+    if name == "-c": name = "python"
+    if name == "-m": name = sys.argv[1]
     name = "-".join(name.split("/")[-3:])
     name = name.replace("python-site-packages-", "").replace(".py", "")
+    name = name.replace("python3 -m ", "")
+    name = name.replace("python -m ", "")
     return name
 
 def getIdentifier():
     date = datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
     return f"{getApplication()}/{date}"
```

### Comparing `micrologai-1.3.3/microlog/models.py` & `micrologai-1.3.4/microlog/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
     def walkStack(self, startFrame):
         stack = [
             (frame, lineno)
             for frame, lineno in reversed(list(traceback.walk_stack(startFrame)))
         ]
         return stack
             
+    @classmethod
     def callSiteFromFrame(self, frame, lineno):
         filename = frame.f_globals.get("__file__", "")
         module = frame.f_globals.get("__name__", "")
         if module == "__main__":
             module = sys.argv[0].replace(".py", "").replace("/", ".")
         instance = frame.f_locals["self"] if "self" in frame.f_locals else None
         clazz = ""
@@ -155,16 +156,16 @@
             clazz = instance.__class__.__name__
             module = instance.__module__
         name = frame.f_code.co_name
         if self.ignore(module):
             return None
         return CallSite(filename, lineno, f"{module}.{clazz}.{name}")
         
+    @classmethod
     def ignore(self, module):
-        from microlog import config
         return module in config.IGNORE_MODULES
 
     def __iter__(self):
         return iter(self.callSites)
 
     def __len__(self):
         return len(self.callSites)
```

### Comparing `micrologai-1.3.3/microlog/server.py` & `micrologai-1.3.4/microlog/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,17 @@
                 explanation = explain.explainLog(name.split("/")[0], log.decode("utf-8"))
                 print(explanation)
                 return self.sendData("text/html", bytes(explanation, encoding="utf-8"))
 
             if self.path in ["/stop"]:
                 return 
 
-            if self.path.startswith("/microlog/images/"):
+            if "/images/" in self.path:
+                while self.path.startswith("/microlog//"):
+                    self.path = self.path[10:]
                 with open(self.path[1:], "rb") as fd:
                     return self.sendData("image/png", fd.read())
 
             if self.path in ["", "/"]:
                 with open('index.html') as fd:
                     return self.sendData("text/html", bytes(f"{fd.read()}", encoding="utf-8"))
```

### Comparing `micrologai-1.3.3/microlog/sitecustomize.py` & `micrologai-1.3.4/microlog/sitecustomize.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 #
 
 def install_microlog_as_a_continuous_profiler():
     try:
         import psutil
         try:
             import logging
+            import sys
+
+            sys.path.append(".")
             import microlog
 
             logging.Logger("Microlog").info("Microlog has been enabled in", __file__)
             microlog.start()
         except:
             import traceback
             traceback.print_exc()
```

### Comparing `micrologai-1.3.3/microlog/tracer.py` & `micrologai-1.3.4/microlog/tracer.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 
 import collections
 
 import gc
 import inspect
 import logging
 import os
+import signal
 import sys
 import threading
-import time
+from time import time, sleep
 
 from microlog import config
 from microlog import log
+from microlog import warn
+from microlog import debug
+from microlog import info
+from microlog import error
 from microlog.models import Status
 from microlog.models import Call
 from microlog.models import CallSite
 from microlog.models import Stack
 
 
 KB = 1024
@@ -29,65 +34,63 @@
     memoryWarning = 0
 
     def __init__(self):
         import psutil # type: ignore
         self.daemon = True
         self.running = False
         self.lastCpuSample = (log.log.now(), psutil.Process().cpu_times())
-        self.delay = config.statusDelay
-        self.tick()
+        self.delay = config.TRACER_STATUS_DELAY
+        self.tick(log.log.now())
 
     def checkMemory(self, memory):
         gb = int(memory / GB)
         if gb > StatusGenerator.memoryWarning:
-            from microlog.api import warn
             StatusGenerator.memoryWarning = gb
             warn(f"WARNING: Python process memory grew to {memory / GB:.1f} GB")
     
-    def tick(self) -> None:
+    def tick(self, when) -> None:
         import psutil # type: ignore
         vm = psutil.virtual_memory()
         process = psutil.Process()
         systemCpu = psutil.cpu_percent() / psutil.cpu_count()
         memoryTotal = vm.total
         memoryFree = vm.free
-        now = log.log.now()
         with process.oneshot():
             memory = process.memory_info()
             cpuTimes = process.cpu_times()
 
         def getCpu():
             lastCpuSampleTime, lastCpuTimes = self.lastCpuSample
             user = cpuTimes.user - lastCpuTimes.user
             system = cpuTimes.system - lastCpuTimes.system
-            duration = now - lastCpuSampleTime
-            cpu = min(100, (user + system) * 100 / duration)
-            self.lastCpuSample = (now, cpuTimes)
+            duration = when - lastCpuSampleTime
+            cpu = min(100, (user + system) * 100 / duration) if duration else 0
+            self.lastCpuSample = (when, cpuTimes)
             return cpu
 
         def getMemory():
             self.checkMemory(memory.rss)
             return memory.rss
 
         cpu = getCpu()
         memory = getMemory()
 
         log.log.addStatus(Status(
-            log.log.now(), 
+            when,
             cpu,
             systemCpu,
             memory,
             memoryTotal,
             memoryFree,
             len(sys.modules),
         ))
 
     def stop(self):
-        self.tick()
-        self.tick()
+        self.tick(log.log.now())
+        self.tick(log.log.now())
 
 
 class Tracer(threading.Thread):
     def __init__(self):
         threading.Thread.__init__(self)
         self.statusGenerator = StatusGenerator()
         self.openFiles = {}
@@ -101,48 +104,99 @@
 
     Functionality:
     - Starts a background daemon thread running tick() at a regular interval.
     - For each thread, merges the current stack trace with a new one.
     - At the end, generates a final stack trace with the current timestamp.
     """
     def start(self) -> None:
-        from microlog import config
+        self.delay = config.TRACER_SAMPLE_DELAY
+        if not self.delay:
+            return
         self.setDaemon(True)
         self.stacks = collections.defaultdict(Stack)
-        self.delay = config.sampleDelay
         self.track_print()
         self.track_logging()
         self.track_gc()
         self.track_files()
+        self.lastSample = 0
         self.lastStatus = 0
+        self.sampleCount = 0
         self.running = True
-        return threading.Thread.start(self)
+        self.setupTimer()
+    
+    def setupTimer(self):
+        try:
+            # The peferred choice as this is the least amount of overhead 
+            # Only works on Linux, UNIX, and MacOSs
+            signal.signal(config.TRACER_SIGNAL_KIND, self.signal_handler)
+            signal.setitimer(config.TRACE_TIMER_KIND, self.delay)
+            info(f"Microlog: Using a signal timer with a sample delay of {self.delay}s")
+            return
+        except Exception as e:
+            error(f"Microlog: Cannot use a signal timer: {e}")
+
+        try:
+            # The second-best choice, use a thread that sleeps
+            # Does not work on PyScript/PyOdide as WebAssembly makes threads hard
+            threading.Thread.start(self) # use thread if signals do not work
+            info(f"Microlog: Using a background thread with a sample delay of {self.delay}s")
+            return 
+        except Exception as e:
+            error(f"Microlog: Cannot use a background thread timer: {e}")
+
+        try:
+            # The final choice, this is needed for PyScript.
+            # This has serious overhead, making Python run around 4X slower.
+            sys.setprofile(lambda frame, event, arg: self.sample() if event == "call" else None)
+            info(f"Microlog: Using sys.setprofile with a sample delay of {self.delay}s")
+            return
+        except Exception as e:
+            error(f"Microlog: Cannot use a sys.profile timer: {e}")
+
+
+    def signal_handler(self, sig, frame):
+        try:
+            self.sample()
+            signal.setitimer(signal.ITIMER_PROF, self.delay)
+        except:
+            pass
+
+    def profile(self, frame, event, arg, delay=config.TRACER_SAMPLE_DELAY):
+        # This is to generate a timer if signals don't work (on PyScript?)
+        # Needs the following during start:
+        #  - self.lastProfile = log.log.now()
+        #  - sys.setprofile(self.profile)
+        if self.running and event == "c_exception":
+            now = time()
+            if now - self.lastProfile > delay:
+                self.sample()
+                self.lastProfile = time()
+            return self.profile
 
     def run(self) -> None:
         while self.running:
-            self.tick()
-            time.sleep(self.delay)
+            self.tick(log.log.now())
+            sleep(self.delay)
 
     def track_gc(self):
         self.gc_info = {
             "duration": 0.0,
             "count": 0,
             "collected": 0,
             "uncollectable": 0,
         }
         gc.callbacks.append(self.gc_ran)
         
     def gc_ran(self, phase, info):
         if not self.running:
             return
-        from microlog.api import debug
         if phase == "start":
-            self.gc_info["start"] = time.time()
+            self.gc_info["start"] = time()
         elif phase == "stop":
-            duration = time.time() - self.gc_info["start"]
+            duration = time() - self.gc_info["start"]
             self.gc_info["duration"] += duration
             self.gc_info["count"] += 1
             self.gc_info["collected"] += info["collected"]
             self.gc_info["uncollectable"] += info["uncollectable"]
             if duration > 1.0:
                 debug(f"GC took {duration:.1}s for {info['collected']} objects.")
 
@@ -176,25 +230,23 @@
                     del self.openFiles[io]
                     io.__exit__ = __exit__
 
             return io
         __builtins__["open"] = microlog_open
 
     def track_print(self):
-        from microlog.api import info
-        from microlog.api import error
-        original_print = print
+        self.original_print = print
         def microlog_print(
             *values: object,
             sep: str | None = " ",
             end: str | None = "\n",
             file=None,
             flush=False,
         ) -> None: 
-            original_print(*values, sep=sep, end=end, file=file, flush=flush)
+            self.original_print(*values, sep=sep, end=end, file=file, flush=flush)
             if self.running:
                 log = error if file == sys.stderr else info if file in [None, sys.stdout] else None
                 if log:
                     log(" ".join(map(str, values)))
                 self.sample()
         __builtins__["print"] = microlog_print
 
@@ -204,62 +256,63 @@
         class LogStreamHandler(logging.StreamHandler):
             def __init__(self):
                 logging.StreamHandler.__init__(self)
                 self.setLevel(logging.DEBUG)
                 self.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s'))
 
             def emit(self, record):
-                from microlog.api import debug
-                from microlog.api import info
-                from microlog.api import warn
-                from microlog.api import error
                 message = self.format(record)
                 if record.levelno == logging.INFO:
                     info(message)
                 elif record.levelno == logging.DEBUG:
                     debug(message)
                 elif record.levelno == logging.WARN:
                     warn(message)
                 elif record.levelno == logging.ERROR:
                     error(message)
                 tracer.sample()
 
         logging.getLogger().addHandler(LogStreamHandler())
 
-    def tick(self) -> None:
+    def tick(self, when) -> None:
         """
         Runs every `delay` seconds. Generates a call stack sample.
         """
         self.sample()
-        from microlog import config
-        from microlog import log
-        when = log.log.now()
-        if when - self.lastStatus > config.statusDelay:
-            self.lastStatus = when
-            self.statusGenerator.tick()
+        self.generateStatus(when)
+
+    def generateStatus(self, when):
+        if when - self.lastStatus < config.TRACER_STATUS_DELAY:
+            return
+        self.lastStatus = when
+        self.statusGenerator.tick(when)
 
     def sample(self, function=None) -> None:
         """
         Samples all threads.
 
         Parameters:
         - function: The function to add to the current stack trace, when using a decorator.
         """
         if not self.running:
             return
-        from microlog import log
         when = log.log.now()
+        if when - self.lastSample < config.TRACER_STATUS_DELAY:
+            return
+        self.sampleCount += 1
+        self.lastSample = when
         frames = sys._current_frames()
         for threadId, frame in frames.items():
             if threadId != self.ident:
                 self.merge(threadId, self.getStack(when, threadId, frame, function))
         for threadId in list(self.stacks.keys()):
             if threadId not in frames:
                 self.merge(threadId, Stack(log.log.now(), threadId))
                 del self.stacks[threadId]
+        self.generateStatus(when)
 
     def getStack(self, when, threadId, frame, function):
         """
         Generates a new stack trace with the given timestamp and starting frame.  
 
         Parameters:
         - when: The timestamp for the new stack trace. 
@@ -328,22 +381,27 @@
         self.stacks[threadId] = stack
 
     def stop(self):
         """
         Generates a final stack trace for all threads with the current timestamp.  
         """
         self.running = False
-        self.addFinalStack()
-        self.addOpenFilesWarning()
-        self.showStats()
+        if self.delay:
+            try:
+                # cancel the most recent signal timer
+                signal.setitimer(signal.ITIMER_PROF, 0)
+                time.sleep(self.delay)
+            except:
+                pass
+            self.addFinalStack()
+            self.addOpenFilesWarning()
+            self.showStats()
     
     def addOpenFilesWarning(self):
         if self.openFiles:
-            from microlog import warn
-
             def shortFile(filename):
                 parts = filename.split("/")
                 if parts[-1] == "__init__.py":
                     parts.pop()
                 return parts[-1]
 
             def link(frame):
@@ -358,20 +416,20 @@
             warn(f"""
                 # File Descriptors Leaked
                 Found {len(self.openFiles)} files that were opened, but never closed:
                 {files}
                 """)
     
     def addFinalStack(self):
-        from microlog import log
-        self.statusGenerator.tick()
         now = log.log.now()
+        self.statusGenerator.tick(now)
         for threadId in sys._current_frames():
             if threadId != self.ident:
                 self.merge(threadId, Stack(now, threadId))
+        self.generateStatus(now)
      
     def interesting(self, obj: any) -> bool:
         BUILTIN_MODULES = set([
             "http", "_frozen_importlib", "_frozen_importlib_external", "builtins",
             "weakref", "_weakrefset", "functools", "threading", "re", "__future__", "socketserver",
             "_thread", "encodings.utf_8", "os", "operator", "calendar", "email.charset", "email._policybase",
             "json.encoder", "json.decoder", "_json", "string", "psutil", "appdata", "pathlib", "ast",
@@ -395,22 +453,18 @@
         parts = name.split(os.path.sep)
         for n, part in enumerate(parts):
             if part.startswith("python"):
                 return ".".join(parts[n + 1:]).replace("site-packages.", "")
         return ".".join(parts)
     
     def showStats(self):
-        from collections import Counter
-        from microlog import log
-        from microlog.api import debug
-        from microlog.api import error
         now = log.log.now()
         gc.collect()
         objects = [obj for obj in gc.get_objects() if self.interesting(obj)]
-        typeCounts = Counter(type(obj).__name__ for obj in objects)
+        typeCounts = collections.Counter(type(obj).__name__ for obj in objects)
         top10Types = dict(typeCounts.most_common(10))
         top10 = []
         for obj in objects:
             typeName = type(obj).__name__
             if typeName in top10Types:
                 del top10Types[typeName]
                 top10.append(obj)
@@ -423,14 +477,16 @@
         uncollectable = f"A total of {self.gc_info['uncollectable']:,} objects were leaked (uncollectable) during runtime." if self.gc_info["uncollectable"] else ""
         count = self.gc_info["count"]
         count = "once" if count == 1 else f"{count} times"
         duration = self.gc_info["duration"]
         percentage = self.gc_info["duration"] / now * 100
         average = self.gc_info["duration"] / self.gc_info["count"] if self.gc_info["count"] else 0.0
         (error if leaks else debug)(f"""
+# General Statistics
+- Performed {self.sampleCount} samples
 # GC Statistics
 GC ran {count} for {duration:.3f}s ({percentage:.1f}% of {now:.3f}s), averaging {average:.3f}s per collection.
 In total, {self.gc_info["collected"]:,} objects were collected.
 {uncollectable}
 {leaks}""")
 
     def describeReference(self, obj, value):
```

### Comparing `micrologai-1.3.3/micrologai.egg-info/PKG-INFO` & `micrologai-1.3.4/micrologai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.3
+Version: 1.3.4
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
         
@@ -569,14 +569,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # microlog.ai
 
+A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). 
+
 _Microlog_ is a continuous profiler and logger for the Python language that
 explains application behavior using interactive graphs and AI. 
 It makes understanding complex applications easy, reducing support costs
 and shortening production problems, increasing application quality, and minimizing outages.
 
 _Microlog_ has extremely low runtime overhead (~1%) and exceptionally fast rendering (~20ms).
 It saves logs and performance profiles on the local file system. The logs are
@@ -642,15 +644,15 @@
 
 # The Microlog.ai UI 
 
 A live demo of the _Microlog_ UI can be found at [micrologai.github.io/microlog](https://micrologai.github.io/microlog/). The UI is
 written almost entirely in Python, see [dashboard](dashboard). The _Microlog_ UI runs in the browser using PyScript. 
 
 To describe the UI features of _Microlog_, we will look at the output of the [examples\memory.py](examples\memory.py) example (the live preview is at
-[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_26_14_11_38/)):
+[GitHub Pages](https://micrologai.github.io/microlog/#examples-memory/2023_07_31_11_16_19/)):
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
 
 The main elements of the UI are:
 
  - `Log list`, at the left, showing currently available logs on the local machine.
  - `Timeline`, the starting point for analysis of your application:
```

### Comparing `micrologai-1.3.3/micrologai.egg-info/SOURCES.txt` & `micrologai-1.3.4/micrologai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 microlog/images/icons/urllib.png
 microlog/images/icons/wsgi.png
 microlog/images/icons/zmq.png
 micrologai.egg-info/PKG-INFO
 micrologai.egg-info/SOURCES.txt
 micrologai.egg-info/dependency_links.txt
 micrologai.egg-info/entry_points.txt
+micrologai.egg-info/not-zip-safe
 micrologai.egg-info/requires.txt
 micrologai.egg-info/top_level.txt
 tests/test_call_view.py
 tests/test_canvas.py
 tests/test_log.py
 tests/test_marker_view.py
 tests/test_print.py
```

### Comparing `micrologai-1.3.3/pyproject.toml` & `micrologai-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micrologai"
-version = "1.3.3"
+version = "1.3.4"
 description = "A continuous profiler and logger for Python written entirely in Python"
 readme = "README.md"
 authors = [{ name = "Chris Laffra", email = "chris@chrislaffra.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `micrologai-1.3.3/setup.py` & `micrologai-1.3.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,36 +14,41 @@
 os.system(pip)
 
 def _post_install():
     sitepackages = site.getsitepackages()[0]
     original = sitecustomize.__file__
     target = os.path.join(sitepackages, os.path.basename(original))
     if os.path.exists(target):
+        with open(target) as file:
+            if "Microlog" in file.read():
+                print("Microlog was already installed in", target)
+                return
         with open(target, "a") as file:
             file.write("#\n")
             file.write(f"# Microlog installation time: {datetime.datetime.now()}\n")
             file.write(f"# Microlog location: {original}\n")
             file.write(open(sitecustomize.__file__).read())
     else:
         shutil.copy(sitecustomize.__file__, sitepackages)
-    print('Installed', sitecustomize.__file__, "into", target)
+    print('Microlog has been installed', sitecustomize.__file__, "into", target)
 
 
 atexit.register(_post_install)
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='Microlog',
     description='A continuous profiler and logger for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="1.3.3",
+    version="1.3.4",
+    zip_safe=False,
     author='Chris Laffra',
     author_email='laffra@gmail.com',
     url='https://www.chrislaffra.org/',
     packages=setuptools.find_packages(include=[
         'microlog',
         'dashboard',
     ]),
```

### Comparing `micrologai-1.3.3/tests/test_call_view.py` & `micrologai-1.3.4/tests/test_call_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/tests/test_canvas.py` & `micrologai-1.3.4/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/tests/test_marker_view.py` & `micrologai-1.3.4/tests/test_marker_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/tests/test_print.py` & `micrologai-1.3.4/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/tests/test_status.py` & `micrologai-1.3.4/tests/test_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from microlog import log
 from microlog.tracer import StatusGenerator
 
 
 class StatusTest(unittest.TestCase):
     def test_sample(self):
         status = StatusGenerator()
-        status.tick()
+        status.tick(log.log.now())
         self.assertGreaterEqual(len(log.log.statuses), 2)
 
         status = log.log.statuses[0]
         self.assertGreaterEqual(status.cpu, 0)
         self.assertGreater(status.memoryTotal, 0)
         self.assertGreater(status.memoryFree, 0)
         self.assertGreaterEqual(status.systemCpu, 0)
```

### Comparing `micrologai-1.3.3/tests/test_status_view.py` & `micrologai-1.3.4/tests/test_status_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.3/tests/test_tracer.py` & `micrologai-1.3.4/tests/test_tracer.py`

 * *Files identical despite different names*

