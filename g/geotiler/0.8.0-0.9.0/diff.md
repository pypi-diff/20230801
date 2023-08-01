# Comparing `tmp/geotiler-0.8.0.tar.bz2` & `tmp/geotiler-0.9.0.tar.bz2`

## Comparing `geotiler-0.8.0.tar` & `geotiler-0.9.0.tar`

### file list

```diff
@@ -1,76 +1,73 @@
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/bin/
--rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)     3114 2016-03-06 01:57:23.000000 geotiler-0.8.0/bin/geotiler-fetch
--rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)     4005 2016-02-17 09:34:35.000000 geotiler-0.8.0/bin/geotiler-lint
--rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)     4343 2016-03-06 01:46:30.000000 geotiler-0.8.0/bin/geotiler-route
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/data/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     7147 2016-03-06 01:31:19.000000 geotiler-0.8.0/data/path.gpx
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/doc/
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/doc/static/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   319264 2014-04-10 20:56:07.000000 geotiler-0.8.0/doc/static/bluemarble.png
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      633 2014-04-12 10:12:07.000000 geotiler-0.8.0/doc/static/geotiler.css
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      687 2015-05-01 17:48:50.000000 geotiler-0.8.0/doc/api.rst
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1353 2016-02-27 08:01:32.000000 geotiler-0.8.0/doc/changelog.rst
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1534 2016-03-06 01:57:07.000000 geotiler-0.8.0/doc/cmd.rst
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      693 2014-04-08 18:26:41.000000 geotiler-0.8.0/doc/conf.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      896 2016-02-27 08:03:51.000000 geotiler-0.8.0/doc/index.rst
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1770 2015-11-21 09:17:36.000000 geotiler-0.8.0/doc/intro.rst
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5532 2016-02-27 08:04:04.000000 geotiler-0.8.0/doc/usage.rst
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/examples/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2510 2016-02-17 09:34:35.000000 geotiler-0.8.0/examples/ex-async-gps.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2060 2016-02-17 09:34:35.000000 geotiler-0.8.0/examples/ex-basemap.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2085 2016-02-17 09:34:35.000000 geotiler-0.8.0/examples/ex-cairo.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1478 2016-02-17 09:34:35.000000 geotiler-0.8.0/examples/ex-geocoder.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1859 2016-02-17 09:34:35.000000 geotiler-0.8.0/examples/ex-matplotlib.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5182 2016-02-27 07:40:54.000000 geotiler-0.8.0/examples/ex-opencv.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     7234 2016-02-17 09:34:35.000000 geotiler-0.8.0/examples/ex-qt-gps.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1825 2016-02-17 09:34:35.000000 geotiler-0.8.0/examples/ex-redis-cache.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler/
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler/provider/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1097 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2868 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/base.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1878 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/bluemarble.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1276 2015-11-04 07:55:59.000000 geotiler-0.8.0/geotiler/provider/chartbundle.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3216 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/cloudmade.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2687 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/conf.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2375 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/mapquest.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4535 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/ms.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1977 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/osm.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2809 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/stamen.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4569 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/provider/yahoo.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler/tests/
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler/tests/provider/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1108 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/provider/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2934 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/provider/test_ms.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2920 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/provider/test_yahoo.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1094 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4162 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/test_cache.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3158 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/test_geo.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10492 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/test_map.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2883 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/test_tile_img.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4213 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tests/test_tile_io.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler/tile/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1064 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/tile/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3059 2016-03-05 19:49:32.000000 geotiler-0.8.0/geotiler/tile/img.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3052 2016-02-17 14:37:29.000000 geotiler-0.8.0/geotiler/tile/io.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1180 2016-02-17 14:37:16.000000 geotiler-0.8.0/geotiler/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3239 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/cache.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5127 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/geo.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    15303 2016-02-17 09:34:35.000000 geotiler-0.8.0/geotiler/map.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler.egg-info/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      597 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler.egg-info/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1407 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler.egg-info/SOURCES.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler.egg-info/dependency_links.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        7 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler.egg-info/requires.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        9 2016-03-06 02:03:14.000000 geotiler-0.8.0/geotiler.egg-info/top_level.txt
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-03-06 02:03:14.000000 geotiler-0.8.0/scripts/
--rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)     2911 2014-04-07 23:20:21.000000 geotiler-0.8.0/scripts/map-origin
--rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)      708 2014-04-06 19:08:43.000000 geotiler-0.8.0/scripts/test-all
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)       32 2014-03-30 13:42:07.000000 geotiler-0.8.0/.gitignore
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)       95 2014-04-06 15:14:46.000000 geotiler-0.8.0/.travis.yml
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      681 2016-03-06 01:38:01.000000 geotiler-0.8.0/Makefile
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      531 2014-04-06 18:12:21.000000 geotiler-0.8.0/README
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      128 2015-04-28 20:25:54.000000 geotiler-0.8.0/requirements.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1940 2016-03-06 01:42:09.000000 geotiler-0.8.0/setup.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      597 2016-03-06 02:03:14.000000 geotiler-0.8.0/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      200 2016-03-06 02:03:14.000000 geotiler-0.8.0/setup.cfg
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/bin/
+-rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)     3034 2016-08-14 14:10:10.000000 geotiler-0.9.0/bin/geotiler-fetch
+-rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)     3136 2016-08-14 14:01:58.000000 geotiler-0.9.0/bin/geotiler-lint
+-rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)     4210 2016-08-14 13:58:03.000000 geotiler-0.9.0/bin/geotiler-route
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/data/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     7147 2016-03-06 01:31:19.000000 geotiler-0.9.0/data/path.gpx
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/doc/
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/doc/static/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   319264 2014-04-10 20:56:07.000000 geotiler-0.9.0/doc/static/bluemarble.png
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      633 2014-04-12 10:12:07.000000 geotiler-0.9.0/doc/static/geotiler.css
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      746 2016-08-14 14:18:27.000000 geotiler-0.9.0/doc/api.rst
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1769 2016-08-14 14:26:25.000000 geotiler-0.9.0/doc/changelog.rst
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1537 2016-08-14 14:02:56.000000 geotiler-0.9.0/doc/cmd.rst
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      693 2014-04-08 18:26:41.000000 geotiler-0.9.0/doc/conf.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      896 2016-02-27 08:03:51.000000 geotiler-0.9.0/doc/index.rst
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1770 2015-11-21 09:17:36.000000 geotiler-0.9.0/doc/intro.rst
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5633 2016-08-14 14:17:46.000000 geotiler-0.9.0/doc/usage.rst
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/examples/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2510 2016-02-17 09:34:35.000000 geotiler-0.9.0/examples/ex-async-gps.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2060 2016-02-17 09:34:35.000000 geotiler-0.9.0/examples/ex-basemap.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2085 2016-02-17 09:34:35.000000 geotiler-0.9.0/examples/ex-cairo.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1478 2016-02-17 09:34:35.000000 geotiler-0.9.0/examples/ex-geocoder.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1859 2016-02-17 09:34:35.000000 geotiler-0.9.0/examples/ex-matplotlib.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5182 2016-02-27 07:40:54.000000 geotiler-0.9.0/examples/ex-opencv.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     7234 2016-02-17 09:34:35.000000 geotiler-0.9.0/examples/ex-qt-gps.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1825 2016-02-17 09:34:35.000000 geotiler-0.9.0/examples/ex-redis-cache.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3447 2016-03-11 21:58:43.000000 geotiler-0.9.0/examples/ex-shelvecache.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler/
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler/source/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      247 2016-08-14 13:48:10.000000 geotiler-0.9.0/geotiler/source/bluemarble.json
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      255 2016-08-14 13:39:56.000000 geotiler-0.9.0/geotiler/source/osm-cycle.json
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      249 2016-08-14 13:39:51.000000 geotiler-0.9.0/geotiler/source/osm.json
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      250 2016-08-14 13:44:04.000000 geotiler-0.9.0/geotiler/source/stamen-terrain.json
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      256 2016-08-14 13:44:19.000000 geotiler-0.9.0/geotiler/source/stamen-toner-lite.json
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      246 2016-08-14 13:44:13.000000 geotiler-0.9.0/geotiler/source/stamen-toner.json
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      260 2016-08-14 13:43:27.000000 geotiler-0.9.0/geotiler/source/stamen-watercolor.json
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler/tests/
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler/tests/provider/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1108 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/tests/provider/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1094 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/tests/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4162 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/tests/test_cache.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3158 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/tests/test_geo.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10492 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/tests/test_map.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2996 2016-08-14 13:24:43.000000 geotiler-0.9.0/geotiler/tests/test_provider.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2883 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/tests/test_tile_img.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4213 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/tests/test_tile_io.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler/tile/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1064 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/tile/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3059 2016-03-05 19:49:32.000000 geotiler-0.9.0/geotiler/tile/img.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3052 2016-02-17 14:37:29.000000 geotiler-0.9.0/geotiler/tile/io.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1186 2016-08-14 14:19:31.000000 geotiler-0.9.0/geotiler/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3239 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/cache.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5127 2016-02-17 09:34:35.000000 geotiler-0.9.0/geotiler/geo.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    15330 2016-08-14 14:23:29.000000 geotiler-0.9.0/geotiler/map.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3672 2016-08-14 14:24:20.000000 geotiler-0.9.0/geotiler/provider.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler.egg-info/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      597 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler.egg-info/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1338 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler.egg-info/SOURCES.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler.egg-info/dependency_links.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        7 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler.egg-info/requires.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        9 2016-08-14 14:28:40.000000 geotiler-0.9.0/geotiler.egg-info/top_level.txt
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2016-08-14 14:28:40.000000 geotiler-0.9.0/scripts/
+-rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)     2911 2014-04-07 23:20:21.000000 geotiler-0.9.0/scripts/map-origin
+-rwxr-xr-x   0 wrobell   (1000) wrobell   (1000)      768 2016-08-14 14:07:24.000000 geotiler-0.9.0/scripts/test-all
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)       32 2014-03-30 13:42:07.000000 geotiler-0.9.0/.gitignore
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)       95 2016-08-10 21:25:39.000000 geotiler-0.9.0/.travis.yml
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      683 2016-08-14 14:03:37.000000 geotiler-0.9.0/Makefile
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      531 2014-04-06 18:12:21.000000 geotiler-0.9.0/README
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      128 2015-04-28 20:25:54.000000 geotiler-0.9.0/requirements.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      200 2016-08-14 14:28:40.000000 geotiler-0.9.0/setup.cfg
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1971 2016-08-14 13:55:31.000000 geotiler-0.9.0/setup.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      597 2016-08-14 14:28:40.000000 geotiler-0.9.0/PKG-INFO
```

### Comparing `geotiler-0.8.0/bin/geotiler-fetch` & `geotiler-0.9.0/bin/geotiler-fetch`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 """
 
 parser = argparse.ArgumentParser(description=desc)
 parser.add_argument(
     '-v', '--verbose', dest='verbose', help='explain what is being done',
     action='store_true'
 )
-providers = list(sorted(geotiler.provider.conf.PROVIDERS.keys()))
+providers = geotiler.providers()
 parser.add_argument(
     '-p', '--provider', dest='provider', choices=providers, default='osm',
-    help='map provider name'
+    help='map provider id'
 )
 parser.add_argument(
     '--cache', dest='cache', choices=['redis'], default='redis',
     help='specify caching strategy'
 )
 parser.add_argument(
     '-x', '--min-zoom', dest='min_zoom', default=1, type=int,
@@ -69,27 +69,25 @@
 )
 
 args = parser.parse_args()
 
 if args.verbose:
     logging.basicConfig(level=logging.DEBUG)
 
-provider = geotiler.find_provider(args.provider)
-
 if args.cache == 'redis':
     import redis
     from geotiler.cache import redis_downloader
 
     client = redis.Redis('localhost')
     downloader = redis_downloader(client)
 
 
 render_map = functools.partial(geotiler.render_map, downloader=downloader)
 for zoom in range(args.min_zoom, args.max_zoom + 1):
-    map = geotiler.Map(extent=args.extent, zoom=zoom, provider=provider)
+    map = geotiler.Map(extent=args.extent, zoom=zoom, provider=args.provider)
     map.zoom = zoom
     if map.size[0] < 256 or map.size[1] < 256:
         print(
             'map image size for zoom {} is less than 256x256,' \
             ' skipping'.format(zoom),
             file=sys.stderr
         )
```

### Comparing `geotiler-0.8.0/bin/geotiler-route` & `geotiler-0.9.0/bin/geotiler-route`

 * *Files 10% similar despite different names*

```diff
@@ -75,30 +75,30 @@
 """
 
 parser = argparse.ArgumentParser(description=desc)
 parser.add_argument(
     '-v', '--verbose', dest='verbose', help='Make a bunch of noise',
     action='store_true'
 )
-providers = list(sorted(geotiler.provider.conf.PROVIDERS.keys()))
+providers = geotiler.providers()
 parser.add_argument(
     '-p', '--provider', dest='provider', choices=providers, default='osm',
-    help='Map provider or URL template like "http://example.com/{z}/{x}/{y}.png".'
+    help='map provider id'
 )
 parser.add_argument(
     '-s', '--size', dest='size', nargs=2, type=int, default=(1920, 1080),
-    help='Size of map image'
+    help='size of map image'
 )
 parser.add_argument(
     '-r', '--radius', dest='radius', type=float, default=0.5,
-    help='Radius of drawn point of a position'
+    help='radius of drawn point of a position'
 )
 parser.add_argument(
     '-a', '--alpha', dest='alpha', type=float, default=0.5,
-    help='Color alpha of drawn point of a position'
+    help='color alpha of drawn point of a position'
 )
 parser.add_argument(
     '--cache', dest='cache', choices=['redis'], default='redis',
     help='specify caching strategy'
 )
 parser.add_argument('filename', nargs='+', help='GPX file')
 parser.add_argument('output', help='Output PNG file')
@@ -119,16 +119,15 @@
 positions = list(positions)
 x, y = zip(*positions)
 extent = min(x), min(y), max(x), max(y)
 
 #
 # render map image
 #
-provider = geotiler.find_provider(args.provider)
-mm = geotiler.Map(size=args.size, extent=extent, provider=provider)
+mm = geotiler.Map(size=args.size, extent=extent, provider=args.provider)
 if mm.zoom > 18: # FIXME: max zoom in API missing
     mm = geotiler.Map(zoom=18, extent=extent)
 
 render_map = functools.partial(geotiler.render_map, downloader=downloader)
 img = render_map(mm)
 
 #
```

### Comparing `geotiler-0.8.0/data/path.gpx` & `geotiler-0.9.0/data/path.gpx`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/doc/static/bluemarble.png` & `geotiler-0.9.0/doc/static/bluemarble.png`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/doc/static/geotiler.css` & `geotiler-0.9.0/doc/static/geotiler.css`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/doc/api.rst` & `geotiler-0.9.0/doc/api.rst`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 Map Rendering
 -------------
 .. autosummary::
 
    geotiler.Map
    geotiler.render_map
    geotiler.render_map_async
+   geotiler.providers
    geotiler.find_provider
 
 .. autoclass:: geotiler.Map
    :members:
    :special-members:
 
 .. autofunction:: geotiler.render_map
 .. autofunction:: geotiler.render_map_async
+.. autofunction:: geotiler.providers
 .. autofunction:: geotiler.find_provider
 
 
 Tile Downloading and Caching
 ----------------------------
 .. autosummary::
```

### Comparing `geotiler-0.8.0/doc/changelog.rst` & `geotiler-0.9.0/doc/changelog.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 Changelog
 =========
+0.9.0
+-----
+- replace python based map providers configuration with JSON file
+  configuration (inspired by poor-maps project tile source definition
+  https://github.com/otsaloma/poor-maps/tree/master/tilesources)
+- `geotiler-lint` map provider argument is optional now
+- `geotiler.Map` provider constructor parameter should be string now
+- added caching example using `shelve` Python module (thanks to matthijs876)
+
 0.8.0
 -----
 - implemented `geotiler-fetch` script to cache map tiles upfront
 - implemented `geotiler-route` script to draw GPX track on a map
 - OpenCV example added, thanks to `matthijs876`
 
 0.7.0
```

### Comparing `geotiler-0.8.0/doc/cmd.rst` & `geotiler-0.9.0/doc/cmd.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 --------------------
 GeoTiler provides `geotiler-lint` script, which can be used to create a map
 image from command line.
 
 For example, to create a map image using Blue Marble map tiles provider,
 map center, zoom and map image size::
 
-    geotiler-lint -c -6.069 53.390 -z 8 -s 512 512 bluemarble map-bluemarble.png
+    geotiler-lint -c -6.069 53.390 -z 8 -s 512 512 -p bluemarble map-bluemarble.png
 
 .. figure:: map-bluemarble.png
    :align: center
 
 The script supports all implemented map tiles providers. Map can be
 specified with any of the required map parameters combination. It allows to
 switch map tiles caching strategy to use Redis cache.
```

### Comparing `geotiler-0.8.0/doc/conf.py` & `geotiler-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/doc/index.rst` & `geotiler-0.9.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/doc/intro.rst` & `geotiler-0.9.0/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/doc/usage.rst` & `geotiler-0.9.0/doc/usage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -87,24 +87,27 @@
      Stamen Terrain            stamen-terrain        as above
      Stamen Water Color        stamen-watercolor     as above
      Modest Maps Blue Marble   bluemarble            see `NASA guideline <http://www.nasa.gov/audience/formedia/features/MP_Photo_Guidelines.html>`_
     ========================= ===================== ==================
 
 The default map provider is OpenStreetMap.
 
-GeoTiler implements more map providers. Some of them will be fully
-supported in next GeoTiler releases. The :py:mod:`geotiler.provider.conf` module
-lists all implemented map providers.
-
-A map provider instance can be created with :py:func:`geotiler.find_provider`
-function and the instance can be passed to :py:class:`geotiler.Map` class
+Identificators of GeoTiler map providers can be listed with
+:py:func:`geotiler.providers` function. Map provider identificator can be
+used with :py:func:`geotiler.find_provider` function to create instance of
+map provider or it can be passed to :py:class:`geotiler.Map` class
 constructor::
 
-    >>> toner = geotiler.find_provider('stamen-toner')
-    >>> map = geotiler.Map(center=(-6.069, 53.390), zoom=16, size=(512, 512), provider=toner)
+    >>> map = geotiler.Map(center=(-6.069, 53.390), zoom=16, size=(512, 512), provider='stamen-toner')
+    >>> image = geotiler.render_map(map) # doctest: +SKIP
+
+    # or
+
+    >>> map = geotiler.Map(center=(-6.069, 53.390), zoom=16, size=(512, 512))
+    >>> map.provider = geotiler.find_provider('stamen-toner')
     >>> image = geotiler.render_map(map) # doctest: +SKIP
 
 .. figure:: map-stamen-toner.png
    :align: center
 
 .. _integrate:
```

### Comparing `geotiler-0.8.0/examples/ex-async-gps.py` & `geotiler-0.9.0/examples/ex-async-gps.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/examples/ex-basemap.py` & `geotiler-0.9.0/examples/ex-basemap.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/examples/ex-cairo.py` & `geotiler-0.9.0/examples/ex-cairo.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/examples/ex-geocoder.py` & `geotiler-0.9.0/examples/ex-geocoder.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/examples/ex-matplotlib.py` & `geotiler-0.9.0/examples/ex-matplotlib.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/examples/ex-opencv.py` & `geotiler-0.9.0/examples/ex-opencv.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/examples/ex-qt-gps.py` & `geotiler-0.9.0/examples/ex-qt-gps.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/examples/ex-redis-cache.py` & `geotiler-0.9.0/examples/ex-redis-cache.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/provider/__init__.py` & `geotiler-0.9.0/geotiler/tile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,12 +21,8 @@
 # permission notice (restored, based on setup.py file from
 # https://github.com/stamen/modestmaps-py):
 #
 #   Copyright (C) 2007-2013 by Michal Migurski and other contributors
 #   License: BSD
 #
 
-"""
-Map tiles providers.
-"""
-
-# vim:et sts=4 sw=4:
+# vim: sw=4:et:ai
```

### Comparing `geotiler-0.8.0/geotiler/tests/provider/__init__.py` & `geotiler-0.9.0/geotiler/tests/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/tests/__init__.py` & `geotiler-0.9.0/geotiler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/tests/test_cache.py` & `geotiler-0.9.0/geotiler/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/tests/test_geo.py` & `geotiler-0.9.0/geotiler/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/tests/test_map.py` & `geotiler-0.9.0/geotiler/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/tests/test_tile_img.py` & `geotiler-0.9.0/geotiler/tests/test_tile_img.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/tests/test_tile_io.py` & `geotiler-0.9.0/geotiler/tests/test_tile_io.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/tile/__init__.py` & `geotiler-0.9.0/geotiler/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,13 @@
 # permission notice (restored, based on setup.py file from
 # https://github.com/stamen/modestmaps-py):
 #
 #   Copyright (C) 2007-2013 by Michal Migurski and other contributors
 #   License: BSD
 #
 
+__version__ = '0.9.0'
+
+from .map import Map, render_map, render_map_async
+from .provider import find_provider, providers
+
 # vim: sw=4:et:ai
```

### Comparing `geotiler-0.8.0/geotiler/tile/img.py` & `geotiler-0.9.0/geotiler/tile/img.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/tile/io.py` & `geotiler-0.9.0/geotiler/tile/io.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/cache.py` & `geotiler-0.9.0/geotiler/cache.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/geo.py` & `geotiler-0.9.0/geotiler/geo.py`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/geotiler/map.py` & `geotiler-0.9.0/geotiler/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 """
 
 import asyncio
 import itertools
 import math
 import logging
 
-from .provider.conf import DEFAULT_PROVIDER
+from .provider import DEFAULT_PROVIDER, find_provider
 from .geo import zoom_to
 from .tile.io import fetch_tiles
 from .tile.img import render_image
 
 logger = logging.getLogger(__name__)
 
 MAX_ZOOM = 25
@@ -46,15 +46,15 @@
 class Map(object):
     """
     Map created from tiles and to be drawn as an image.
 
     The extent, zoom, center and image size can be changed at any time with
     appropriate properties.
 
-    :var provider: Map tiles provider (default OpenStreetMap).
+    :var provider: Map tiles provider identificator (default `osm`).
     :var _zoom: Map zoom attribute accessed via `zoom` property.
     :var _size: Map image size accessed via `size` property.
     :var origin: Tile coordinates at map zoom level of base tile.
     :var offset: Position of base tile relative to map center.
     """
     def __init__(
         self, extent=None, center=None, zoom=None, size=None,
@@ -75,15 +75,15 @@
         :param extent: Map geographical extent.
         :param center: Map geographical center.
         :param zoom: Map zoom.
         :param size: Map image size.
         :param provider: Map tiles provider.
         """
         super().__init__()
-        self.provider = provider
+        self.provider = find_provider(provider)
         self.origin = None
         self.offset = None
 
         self._zoom = zoom
         self._size = size
 
         if center and extent:
@@ -364,16 +364,15 @@
     get_url = map.provider.get_tile_urls
 
     # NOTE: consider having origin tile at top-left tile instead of the
     # center, then we could skip this step
     coord, offset = _find_top_left_tile(map)
 
     coords = _tile_coords(map, coord, offset)
-    urls = tuple(get_url(c, map.zoom)[0] for c in coords)
-
+    urls = tuple(get_url(c, map.zoom) for c in coords)
     tile_data = yield from downloader(urls, **kw)
 
     offsets = _tile_offsets(map, offset)
     return render_image(map, tile_data, offsets)
 
 
 def _tile_coords(map, coord, offset):
```

### Comparing `geotiler-0.8.0/geotiler.egg-info/PKG-INFO` & `geotiler-0.9.0/geotiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: geotiler
-Version: 0.8.0
+Version: 0.9.0
 Summary: GeoTiler - library to create maps using tiles from a map provider
 Home-page: http://wrobell.it-zone.org/geotiler/
 Author: Artur Wroblewski
 Author-email: wrobell@pld-linux.org
 License: GPL (includes BSD licensed code)
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `geotiler-0.8.0/scripts/map-origin` & `geotiler-0.9.0/scripts/map-origin`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/scripts/test-all` & `geotiler-0.9.0/scripts/test-all`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/bin/sh
 
 #
 # render map via all supported map tiles providers; redis is required
 #
 
-PROVIDERS="osm osm-cycle stamen-toner bluemarble"
+PROVIDERS="osm osm-cycle stamen-toner stamen-toner-lite stamen-terrain stamen-watercolor bluemarble"
 EXTENT="-10.854492187499988 35.20972164522138 41.8798828125 71.37110941823617"
 CENTER="15.512695312500005 57.49221366670073"
 ZOOM=5
 SIZE="1200 1500"
 GEOTILER='./bin/geotiler-lint -v --cache redis'
 
 i=1
 for p in $PROVIDERS; do
     ii=$(printf "%03d" $i)
-    $GEOTILER -c $CENTER -z $ZOOM -s $SIZE $p test-all-$ii-$p-center-zoom-size.png
-    $GEOTILER -e $EXTENT -s $SIZE $p test-all-$ii-$p--extent-size.png
-    $GEOTILER -e $EXTENT -z $ZOOM $p test-all-$ii-$p-extent-zoom.png
+    $GEOTILER -c $CENTER -z $ZOOM -s $SIZE -p $p test-all-$ii-$p-center-zoom-size.png
+    $GEOTILER -e $EXTENT -s $SIZE -p $p test-all-$ii-$p--extent-size.png
+    $GEOTILER -e $EXTENT -z $ZOOM -p $p test-all-$ii-$p-extent-zoom.png
     i=$((i + 1))
 done
 gm montage -geometry '1200x1500>+2+2' -tile 3x test-all-*.png test-all.png
```

### Comparing `geotiler-0.8.0/Makefile` & `geotiler-0.9.0/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 upload-doc:
 	$(RSYNC) build/doc/ wrobell@wrobell.it-zone.org:~/public_html/geotiler
 
 .sphinx-stamp: .map-stamp
 	sphinx-build doc build/doc
 
 .map-stamp:
-	./bin/geotiler-lint --cache redis -c -6.069 53.390 -s 512 512 -z 15 osm doc/map-osm.png
-	./bin/geotiler-lint --cache redis -c -6.069 53.390 -s 512 512 -z 15 stamen-toner doc/map-stamen-toner.png
-	./bin/geotiler-lint --cache redis -c -6.069 53.390 -z 8 -s 512 512 bluemarble doc/map-bluemarble.png
+	./bin/geotiler-lint --cache redis -c -6.069 53.390 -s 512 512 -z 15 doc/map-osm.png
+	./bin/geotiler-lint --cache redis -c -6.069 53.390 -s 512 512 -z 15 -p stamen-toner doc/map-stamen-toner.png
+	./bin/geotiler-lint --cache redis -c -6.069 53.390 -z 8 -s 512 512 -p bluemarble doc/map-bluemarble.png
 	./bin/geotiler-route -r 5 -a 1 --cache redis data/path.gpx doc/map-path.png
```

### Comparing `geotiler-0.8.0/README` & `geotiler-0.9.0/README`

 * *Files identical despite different names*

### Comparing `geotiler-0.8.0/setup.py` & `geotiler-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 #
 
 from setuptools import setup, find_packages
 
 setup(
     name='geotiler',
     packages=find_packages('.'),
+    include_package_data=True,
     scripts=('bin/geotiler-lint', 'bin/geotiler-route', 'bin/geotiler-fetch'),
-    version='0.8.0',
+    version='0.9.0',
     description='GeoTiler - library to create maps using tiles'
         ' from a map provider',
     author='Artur Wroblewski',
     author_email='wrobell@pld-linux.org',
     url='http://wrobell.it-zone.org/geotiler/',
     setup_requires = ['setuptools_git >= 1.0'],
     install_requires=['Pillow'],
```

### Comparing `geotiler-0.8.0/PKG-INFO` & `geotiler-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: geotiler
-Version: 0.8.0
+Version: 0.9.0
 Summary: GeoTiler - library to create maps using tiles from a map provider
 Home-page: http://wrobell.it-zone.org/geotiler/
 Author: Artur Wroblewski
 Author-email: wrobell@pld-linux.org
 License: GPL (includes BSD licensed code)
 Description: UNKNOWN
 Platform: UNKNOWN
```

