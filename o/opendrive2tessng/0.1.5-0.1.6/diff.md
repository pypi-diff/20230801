# Comparing `tmp/opendrive2tessng-0.1.5.tar.gz` & `tmp/opendrive2tessng-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\opendrive2tessng-0.1.5.tar", last modified: Mon Jul 31 09:16:17 2023, max compression
+gzip compressed data, was "dist\opendrive2tessng-0.1.6.tar", last modified: Tue Aug  1 01:20:26 2023, max compression
```

## Comparing `opendrive2tessng-0.1.5.tar` & `opendrive2tessng-0.1.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/
--rw-rw-rw-   0        0        0     1091 2022-07-04 06:28:49.000000 opendrive2tessng-0.1.5/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/
--rw-rw-rw-   0        0        0      720 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/main.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/
--rw-rw-rw-   0        0        0    12909 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/conversion_lanelet.py
--rw-rw-rw-   0        0        0    38355 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/conversion_lanelet_network.py
--rw-rw-rw-   0        0        0     9412 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/converter.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/
--rw-rw-rw-   0        0        0     7920 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/gui.py
--rw-rw-rw-   0        0        0     3585 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/opendrive_convert.py
--rw-rw-rw-   0        0        0     4854 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/osm_convert.py
--rw-rw-rw-   0        0        0    13250 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/viewer.py
--rw-rw-rw-   0        0        0     1720 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/visualize_commonroad.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/__init__.py
--rw-rw-rw-   0        0        0    14324 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/network.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/
--rw-rw-rw-   0        0        0     2632 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/eulerspiral.py
--rw-rw-rw-   0        0        0     7137 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/geometry.py
--rw-rw-rw-   0        0        0     3909 2023-05-06 02:10:21.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/junction.py
--rw-rw-rw-   0        0        0     2286 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/opendrive.py
--rw-rw-rw-   0        0        0     2616 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road.py
--rw-rw-rw-   0        0        0      920 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadElevationProfile.py
--rw-rw-rw-   0        0        0     7954 2023-05-08 01:38:23.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLanes.py
--rw-rw-rw-   0        0        0     4099 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLateralProfile.py
--rw-rw-rw-   0        0        0     5726 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLink.py
--rw-rw-rw-   0        0        0     8934 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadPlanView.py
--rw-rw-rw-   0        0        0     2165 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadtype.py
--rw-rw-rw-   0        0        0     1495 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road_record.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/__init__.py
--rw-rw-rw-   0        0        0    18715 2023-07-01 14:13:19.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/parser.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/
--rw-rw-rw-   0        0        0    12247 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/lanelet2osm.py
--rw-rw-rw-   0        0        0     4085 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/osm.py
--rw-rw-rw-   0        0        0    23038 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/osm2lanelet.py
--rw-rw-rw-   0        0        0     1872 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/parser.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/
--rw-rw-rw-   0        0        0     4222 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/border.py
--rw-rw-rw-   0        0        0    14407 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/plane.py
--rw-rw-rw-   0        0        0    17452 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/plane_group.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/utils.py
--rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/
--rw-rw-rw-   0        0        0     1982 2023-07-31 09:11:10.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/config.py
--rw-rw-rw-   0        0        0    11765 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/convert_utils.py
--rw-rw-rw-   0        0        0     8363 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/external_utils.py
--rw-rw-rw-   0        0        0    11529 2023-07-31 03:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/functions.py
--rw-rw-rw-   0        0        0    42188 2023-07-31 09:07:26.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/network_utils.py
--rw-rw-rw-   0        0        0    10707 2023-03-14 07:15:21.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/unity_utils.py
--rw-rw-rw-   0        0        0      228 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/utils/__init__.py
--rw-rw-rw-   0        0        0      688 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.5/opendrive2tessng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      583 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2756 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/opendrive2tessng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      583 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      118 2022-07-04 07:03:18.000000 opendrive2tessng-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 09:16:17.000000 opendrive2tessng-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      829 2023-07-31 09:14:39.000000 opendrive2tessng-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2022-07-04 06:28:49.000000 opendrive2tessng-0.1.6/LICENSE
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng/
+-rw-rw-rw-   0        0        0      720 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/
+-rw-rw-rw-   0        0        0    12909 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/conversion_lanelet.py
+-rw-rw-rw-   0        0        0    38355 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/conversion_lanelet_network.py
+-rw-rw-rw-   0        0        0     9412 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/converter.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/
+-rw-rw-rw-   0        0        0     7920 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/gui.py
+-rw-rw-rw-   0        0        0     3585 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/opendrive_convert.py
+-rw-rw-rw-   0        0        0     4854 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/osm_convert.py
+-rw-rw-rw-   0        0        0    13250 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/viewer.py
+-rw-rw-rw-   0        0        0     1720 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/visualize_commonroad.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/__init__.py
+-rw-rw-rw-   0        0        0    14324 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/network.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/
+-rw-rw-rw-   0        0        0     2632 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/eulerspiral.py
+-rw-rw-rw-   0        0        0     7137 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/geometry.py
+-rw-rw-rw-   0        0        0     3909 2023-05-06 02:10:21.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/junction.py
+-rw-rw-rw-   0        0        0     2286 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/opendrive.py
+-rw-rw-rw-   0        0        0     2616 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road.py
+-rw-rw-rw-   0        0        0      920 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadElevationProfile.py
+-rw-rw-rw-   0        0        0     7954 2023-05-08 01:38:23.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLanes.py
+-rw-rw-rw-   0        0        0     4099 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLateralProfile.py
+-rw-rw-rw-   0        0        0     5726 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLink.py
+-rw-rw-rw-   0        0        0     8934 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadPlanView.py
+-rw-rw-rw-   0        0        0     2165 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadtype.py
+-rw-rw-rw-   0        0        0     1495 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road_record.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/__init__.py
+-rw-rw-rw-   0        0        0    18715 2023-07-01 14:13:19.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/
+-rw-rw-rw-   0        0        0    12247 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/lanelet2osm.py
+-rw-rw-rw-   0        0        0     4085 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/osm.py
+-rw-rw-rw-   0        0        0    23038 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/osm2lanelet.py
+-rw-rw-rw-   0        0        0     1872 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/plane_elements/
+-rw-rw-rw-   0        0        0     4222 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/plane_elements/border.py
+-rw-rw-rw-   0        0        0    14407 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/plane_elements/plane.py
+-rw-rw-rw-   0        0        0    17452 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/plane_elements/plane_group.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/plane_elements/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/utils.py
+-rw-rw-rw-   0        0        0        0 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng/utils/
+-rw-rw-rw-   0        0        0     2108 2023-08-01 01:18:24.000000 opendrive2tessng-0.1.6/opendrive2tessng/utils/config.py
+-rw-rw-rw-   0        0        0    11765 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/utils/convert_utils.py
+-rw-rw-rw-   0        0        0     8363 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/utils/external_utils.py
+-rw-rw-rw-   0        0        0    11529 2023-07-31 03:16:17.000000 opendrive2tessng-0.1.6/opendrive2tessng/utils/functions.py
+-rw-rw-rw-   0        0        0    42190 2023-08-01 01:18:24.000000 opendrive2tessng-0.1.6/opendrive2tessng/utils/network_utils.py
+-rw-rw-rw-   0        0        0    10707 2023-03-14 07:15:21.000000 opendrive2tessng-0.1.6/opendrive2tessng/utils/unity_utils.py
+-rw-rw-rw-   0        0        0      228 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/utils/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-03-13 03:59:50.000000 opendrive2tessng-0.1.6/opendrive2tessng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      583 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     2756 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/opendrive2tessng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      583 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      118 2022-07-04 07:03:18.000000 opendrive2tessng-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 01:20:26.000000 opendrive2tessng-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-08-01 01:20:22.000000 opendrive2tessng-0.1.6/setup.py
```

### Comparing `opendrive2tessng-0.1.5/LICENSE` & `opendrive2tessng-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/main.py` & `opendrive2tessng-0.1.6/opendrive2tessng/main.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/conversion_lanelet.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/conversion_lanelet.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/conversion_lanelet_network.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/conversion_lanelet_network.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/converter.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/converter.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/gui.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/gui.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/opendrive_convert.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/opendrive_convert.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/osm_convert.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/osm_convert.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/viewer.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/viewer.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/io/visualize_commonroad.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/io/visualize_commonroad.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/network.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/network.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/eulerspiral.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/eulerspiral.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/geometry.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/geometry.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/junction.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/junction.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/opendrive.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/opendrive.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadElevationProfile.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadElevationProfile.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLanes.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLanes.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLateralProfile.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLateralProfile.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLink.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadLink.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadPlanView.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadPlanView.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadtype.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/roadtype.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road_record.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/elements/road_record.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/opendriveparser/parser.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/opendriveparser/parser.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/lanelet2osm.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/lanelet2osm.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/osm.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/osm.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/osm2lanelet.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/osm2lanelet.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/osm/parser.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/osm/parser.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/border.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/plane_elements/border.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/plane.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/plane_elements/plane.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/plane_elements/plane_group.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/plane_elements/plane_group.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/opendrive2lanelet/utils.py` & `opendrive2tessng-0.1.6/opendrive2tessng/opendrive2lanelet/utils.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/utils/config.py` & `opendrive2tessng-0.1.6/opendrive2tessng/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     # 'median': '',
     # 'curb': '',
 }
 
 # 当前后几个点的向量夹角小于 default_angle 且点距小于 max_length(除非夹角为0 ) 时，抹除过渡点
 default_angle = 1
 max_length = 50
+# 如果是opendrive导入的路网，会主动进行简化(仅路段)，避免创建过慢
+simplify_network_force = True
+
 
 # 连续次数后可视为正常车道，或者连续次数后可视为连接段,最小值为2
 point_require = 2
 POINT_REQUIRE = max(2, point_require)
 
 # 当 opendrive 连接段的首尾连接长度低于此值时，抛弃原有的点序列，使用自动连接
 MIN_CONNECTOR_LENGTH = None
```

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/utils/convert_utils.py` & `opendrive2tessng-0.1.6/opendrive2tessng/utils/convert_utils.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/utils/external_utils.py` & `opendrive2tessng-0.1.6/opendrive2tessng/utils/external_utils.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/utils/functions.py` & `opendrive2tessng-0.1.6/opendrive2tessng/utils/functions.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/utils/network_utils.py` & `opendrive2tessng-0.1.6/opendrive2tessng/utils/network_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import numpy as np
 
 # 使用此功能必须依赖 TESS 安装包
 from Tessng import *
 from PySide2.QtGui import *
 from typing import List, Dict
 from opendrive2tessng import send_signal
-from opendrive2tessng.utils.config import LANE_TYPE_MAPPING, MIN_CONNECTOR_LENGTH, is_center, default_angle
+from opendrive2tessng.utils.config import LANE_TYPE_MAPPING, MIN_CONNECTOR_LENGTH, is_center, default_angle, \
+    simplify_network_force
 from opendrive2tessng.utils.convert_utils import convert_opendrive, convert_roads_info, convert_lanes_info
 from opendrive2tessng.utils.functions import get_inter, get_section_childs, connect_childs, get_new_point_indexs
 from opendrive2tessng.opendrive2lanelet.opendriveparser.elements.opendrive import OpenDrive
 from opendrive2tessng.opendrive2lanelet.opendriveparser.elements.roadLanes import Lane
 
 
 class Section:
@@ -244,15 +245,14 @@
         road_mapping = self.create_links(netiface, roads_info, connector_mapping, error_junction)
         # 记录路段间及section间的连接关系
         self.convert_link_connect(roads_info, lanes_info, connector_mapping, road_mapping, error_junction)
         # 记录交叉口的连接关系
         self.convert_junction(roads_info, lanes_info, connector_mapping, road_mapping, error_junction)
         # 实现所有的连接关系
         self.create_connects(netiface, connector_mapping)
-        # print("路网创建成功")
         return error_junction
 
     def create_links(self, netiface: TessInterface.netInterface, roads_info: Dict, connector_mapping: Dict,
                      error_junction: List) -> Dict:
         """
            在 TessNg 中创建 opendrive 所有的基础路段(Link),如果 子section被打断，同时将连接关系记录在 connector_mapping 中
         Args:
@@ -295,53 +295,54 @@
                     # 右车道id为负，越小的越先在tess中创建，左车道id为正，越大的越先创建
                     reverse = True if direction == 'left' else False
                     for index in range(len(childs)):
                         child = childs[index]
                         # 步长过大，可能会导致在分段时 child 只包含了一个点
                         start_index, end_index = child['start'], child['end'] + 1
                         land_ids = sorted(child['lanes'], reverse=reverse)  # 列表内多点的的数据是一样的，取第一个即可
-                        lCenterLinePoint = self.get_coo_list(
-                            [point["position"] for point in points][start_index:end_index])
-                        lanesWithPoints = [
-                            {
-                                'left': self.get_coo_list(
-                                    road_info['sections'][section_id]["lanes"][lane_id]['left_vertices'][
-                                    start_index:end_index]),
-                                'center': self.get_coo_list(
-                                    road_info['sections'][section_id]["lanes"][lane_id]['center_vertices'][
-                                    start_index:end_index]),
-                                'right': self.get_coo_list(
-                                    road_info['sections'][section_id]["lanes"][lane_id]['right_vertices'][
-                                    start_index:end_index]),
-                            }
-                            for lane_id in land_ids
-                        ]
-
-                        # # TODO 当前后两点的空间向量夹角小于某值时，可以将此点忽略
-                        # center_points = [point["position"] for point in points][start_index:end_index]
-                        # new_point_indexs = get_new_point_indexs(center_points, default_angle)
-                        # new_center_points = [center_points[index] for index in new_point_indexs]
-                        # # print(len(center_points), len(new_point_indexs), new_point_indexs)
-                        # lCenterLinePoint = self.get_coo_list(new_center_points)
-                        # lanesWithPoints = []
-                        # for lane_id in land_ids:
-                        #     lane_left_points = road_info['sections'][section_id]["lanes"][lane_id]['left_vertices'][start_index:end_index]
-                        #     lane_center_points = road_info['sections'][section_id]["lanes"][lane_id]['center_vertices'][start_index:end_index]
-                        #     lane_right_points = road_info['sections'][section_id]["lanes"][lane_id]['right_vertices'][start_index:end_index]
-                        #
-                        #     new_lane_left_points = [lane_left_points[index] for index in new_point_indexs]
-                        #     new_lane_center_points = [lane_center_points[index] for index in new_point_indexs]
-                        #     new_lane_right_points = [lane_right_points[index] for index in new_point_indexs]
-                        #     lanesWithPoints.append(
-                        #         {
-                        #             'left': self.get_coo_list(new_lane_left_points),
-                        #             'center': self.get_coo_list(new_lane_center_points),
-                        #             'right': self.get_coo_list(new_lane_right_points),
-                        #         }
-                        #     )
+
+                        # 是否需要简化路网
+                        if not simplify_network_force:
+                            lCenterLinePoint = self.get_coo_list(
+                                [point["position"] for point in points][start_index:end_index])
+                            lanesWithPoints = [
+                                {
+                                    'left': self.get_coo_list(
+                                        road_info['sections'][section_id]["lanes"][lane_id]['left_vertices'][
+                                        start_index:end_index]),
+                                    'center': self.get_coo_list(
+                                        road_info['sections'][section_id]["lanes"][lane_id]['center_vertices'][
+                                        start_index:end_index]),
+                                    'right': self.get_coo_list(
+                                        road_info['sections'][section_id]["lanes"][lane_id]['right_vertices'][
+                                        start_index:end_index]),
+                                }
+                                for lane_id in land_ids
+                            ]
+                        else:
+                            center_points = [point["position"] for point in points][start_index:end_index]
+                            new_point_indexs = get_new_point_indexs(center_points, default_angle)
+                            new_center_points = [center_points[index] for index in new_point_indexs]
+                            lCenterLinePoint = self.get_coo_list(new_center_points)
+                            lanesWithPoints = []
+                            for lane_id in land_ids:
+                                lane_left_points = road_info['sections'][section_id]["lanes"][lane_id]['left_vertices'][start_index:end_index]
+                                lane_center_points = road_info['sections'][section_id]["lanes"][lane_id]['center_vertices'][start_index:end_index]
+                                lane_right_points = road_info['sections'][section_id]["lanes"][lane_id]['right_vertices'][start_index:end_index]
+
+                                new_lane_left_points = [lane_left_points[index] for index in new_point_indexs]
+                                new_lane_center_points = [lane_center_points[index] for index in new_point_indexs]
+                                new_lane_right_points = [lane_right_points[index] for index in new_point_indexs]
+                                lanesWithPoints.append(
+                                    {
+                                        'left': self.get_coo_list(new_lane_left_points),
+                                        'center': self.get_coo_list(new_lane_center_points),
+                                        'right': self.get_coo_list(new_lane_right_points),
+                                    }
+                                )
 
                         lLaneType = [LANE_TYPE_MAPPING[section_info['lanes'][lane_id]['type']] for lane_id in land_ids]
                         lAttr = [{} for _ in land_ids]
                         link_name = f"{road_id}_{section_id}_{index}_{direction}_{self.file_name}"
 
                         link_obj = netiface.createLink3DWithLanePointsAndAttrs(lCenterLinePoint, lanesWithPoints,
                                                                                lLaneType, lAttr, link_name)
```

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/utils/unity_utils.py` & `opendrive2tessng-0.1.6/opendrive2tessng/utils/unity_utils.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng/__init__.py` & `opendrive2tessng-0.1.6/opendrive2tessng/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng.egg-info/PKG-INFO` & `opendrive2tessng-0.1.6/opendrive2tessng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendrive2tessng
-Version: 0.1.5
+Version: 0.1.6
 Summary: convert opendrive to road_network
 Home-page: UNKNOWN
 Author: Author
 Author-email: 17315487709@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opendrive2tessng-0.1.5/opendrive2tessng.egg-info/SOURCES.txt` & `opendrive2tessng-0.1.6/opendrive2tessng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opendrive2tessng-0.1.5/PKG-INFO` & `opendrive2tessng-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendrive2tessng
-Version: 0.1.5
+Version: 0.1.6
 Summary: convert opendrive to road_network
 Home-page: UNKNOWN
 Author: Author
 Author-email: 17315487709@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opendrive2tessng-0.1.5/setup.py` & `opendrive2tessng-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="opendrive2tessng",
-    version="0.1.5",
+    version="0.1.6",
     author="Author",
     author_email="17315487709@163.com",
     description="convert opendrive to road_network",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     install_requires=[
```

