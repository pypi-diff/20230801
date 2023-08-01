# Comparing `tmp/tomoscan-1.3.0a4.tar.gz` & `tmp/tomoscan-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomoscan-1.3.0a4.tar", last modified: Mon Jul 31 13:43:32 2023, max compression
+gzip compressed data, was "tomoscan-1.3.1.tar", last modified: Tue Aug  1 07:13:36 2023, max compression
```

## Comparing `tomoscan-1.3.0a4.tar` & `tomoscan-1.3.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/
--rw-r--r--   0 payno     (1000) payno     (1000)     1253 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)      953 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      609 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     1213 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)     1486 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.170681 tomoscan-1.3.0a4/tomoscan/
--rw-r--r--   0 payno     (1000) payno     (1000)       67 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.170681 tomoscan-1.3.0a4/tomoscan/esrf/
--rw-r--r--   0 payno     (1000) payno     (1000)     1992 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      263 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/edfscan.py
--rw-r--r--   0 payno     (1000) payno     (1000)      266 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/hdf5scan.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.170681 tomoscan-1.3.0a4/tomoscan/esrf/identifier/
--rw-r--r--   0 payno     (1000) payno     (1000)     1765 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2926 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/edfidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5467 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/folderidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5781 2023-07-20 08:59:28.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/hdf5Identifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2302 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/jp2kidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2732 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/rawidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3621 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/tiffidentifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2431 2023-07-20 08:59:28.000000 tomoscan-1.3.0a4/tomoscan/esrf/identifier/url_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)      254 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/mock.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.174681 tomoscan-1.3.0a4/tomoscan/esrf/scan/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    44382 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/edfscan.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.174681 tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/
--rw-r--r--   0 payno     (1000) payno     (1000)      118 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    25256 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/edfframereducer.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8542 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
--rw-r--r--   0 payno     (1000) payno     (1000)    58068 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/hdf5scan.py
--rw-r--r--   0 payno     (1000) payno     (1000)    37157 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/mock.py
--rw-r--r--   0 payno     (1000) payno     (1000)    22858 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/esrf/scan/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)      257 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.174681 tomoscan-1.3.0a4/tomoscan/esrf/volume/
--rw-r--r--   0 payno     (1000) payno     (1000)     1637 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5369 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/edfvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)    19300 2023-07-20 08:59:28.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/hdf5volume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8962 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/jp2kvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3035 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/mock.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17047 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/rawvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15152 2023-07-20 08:50:33.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/singleframebase.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17517 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/tiffvolume.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9222 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/esrf/volume/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)    10102 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/factory.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3757 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/framereducerbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2434 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/identifier.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6006 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/io.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.178681 tomoscan-1.3.0a4/tomoscan/nexus/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.178681 tomoscan-1.3.0a4/tomoscan/nexus/paths/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      831 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)      406 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)      250 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)      540 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)      276 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11151 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/nexus/paths/nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5438 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3214 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/progress.py
--rw-r--r--   0 payno     (1000) payno     (1000)    67365 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/scanbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)      303 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/scanfactory.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8224 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/serie.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/tomoscan/test/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)      266 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/conftest.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1732 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_framereducerbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)      451 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_hdf5_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2850 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_io.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7466 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_normalization.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2013 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_progress.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8996 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_scanbase.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4569 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_scanfactory.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6223 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_serie.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1611 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_tomoobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3704 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11616 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_validator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1502 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_version.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2933 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_volume_base.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6186 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/test_volume_utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8574 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/test/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2341 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/tomoobject.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/tomoscan/unitsystem/
--rw-r--r--   0 payno     (1000) payno     (1000)     1657 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2447 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/electriccurrentsystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3270 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/energysystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6542 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/metricsystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3165 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/timesystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1846 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/unit.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1975 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/unitsystem/voltagesystem.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.182681 tomoscan-1.3.0a4/tomoscan/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)      175 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1120 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/decorator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2976 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/geometry.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2666 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/hdf5.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1512 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/io.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8884 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/utils/volume.py
--rw-r--r--   0 payno     (1000) payno     (1000)    17014 2023-07-19 15:24:18.000000 tomoscan-1.3.0a4/tomoscan/validator.py
--rw-r--r--   0 payno     (1000) payno     (1000)     4346 2023-07-31 13:42:16.000000 tomoscan-1.3.0a4/tomoscan/version.py
--rw-r--r--   0 payno     (1000) payno     (1000)    21318 2023-07-27 11:43:47.000000 tomoscan-1.3.0a4/tomoscan/volumebase.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-07-31 13:43:32.170681 tomoscan-1.3.0a4/tomoscan.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)      953 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)     2741 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      300 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        9 2023-07-31 13:43:31.000000 tomoscan-1.3.0a4/tomoscan.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.959406 tomoscan-1.3.1/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1253 2023-07-19 15:24:18.000000 tomoscan-1.3.1/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)      951 2023-08-01 07:13:36.959406 tomoscan-1.3.1/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      609 2023-07-19 15:24:18.000000 tomoscan-1.3.1/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     1221 2023-08-01 07:13:36.959406 tomoscan-1.3.1/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1486 2023-07-19 15:24:18.000000 tomoscan-1.3.1/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.955406 tomoscan-1.3.1/tomoscan/
+-rw-r--r--   0 payno     (1000) payno     (1000)       67 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.955406 tomoscan-1.3.1/tomoscan/esrf/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1992 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      263 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/edfscan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      266 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/hdf5scan.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.955406 tomoscan-1.3.1/tomoscan/esrf/identifier/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1765 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/identifier/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2926 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/identifier/edfidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5467 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/identifier/folderidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5781 2023-07-20 08:59:28.000000 tomoscan-1.3.1/tomoscan/esrf/identifier/hdf5Identifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2302 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/identifier/jp2kidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2732 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/identifier/rawidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3621 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/identifier/tiffidentifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2431 2023-07-20 08:59:28.000000 tomoscan-1.3.1/tomoscan/esrf/identifier/url_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      254 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/mock.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.955406 tomoscan-1.3.1/tomoscan/esrf/scan/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/scan/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    44382 2023-08-01 06:16:45.000000 tomoscan-1.3.1/tomoscan/esrf/scan/edfscan.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.955406 tomoscan-1.3.1/tomoscan/esrf/scan/framereducer/
+-rw-r--r--   0 payno     (1000) payno     (1000)      118 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/scan/framereducer/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    25256 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/scan/framereducer/edfframereducer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8542 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    60107 2023-08-01 06:16:48.000000 tomoscan-1.3.1/tomoscan/esrf/scan/hdf5scan.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    37157 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/scan/mock.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    25675 2023-08-01 06:16:48.000000 tomoscan-1.3.1/tomoscan/esrf/scan/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      257 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.959406 tomoscan-1.3.1/tomoscan/esrf/volume/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1637 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/volume/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5369 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/volume/edfvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19300 2023-07-20 08:59:28.000000 tomoscan-1.3.1/tomoscan/esrf/volume/hdf5volume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8962 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/volume/jp2kvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3035 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/volume/mock.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17047 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/volume/rawvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15152 2023-07-20 08:50:33.000000 tomoscan-1.3.1/tomoscan/esrf/volume/singleframebase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17517 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/volume/tiffvolume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9222 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/esrf/volume/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10102 2023-08-01 06:16:45.000000 tomoscan-1.3.1/tomoscan/factory.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3757 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/framereducerbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2434 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/identifier.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6006 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/io.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.959406 tomoscan-1.3.1/tomoscan/nexus/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/nexus/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.959406 tomoscan-1.3.1/tomoscan/nexus/paths/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/nexus/paths/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      831 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/nexus/paths/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      406 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/nexus/paths/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      250 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/nexus/paths/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      540 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/nexus/paths/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      276 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/nexus/paths/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11151 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/nexus/paths/nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5438 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3214 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/progress.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    67365 2023-08-01 06:16:45.000000 tomoscan-1.3.1/tomoscan/scanbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      303 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/scanfactory.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8224 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/serie.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.959406 tomoscan-1.3.1/tomoscan/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      266 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/conftest.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1732 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_framereducerbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      451 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_hdf5_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2850 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_io.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7466 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_normalization.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2013 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_progress.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8996 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_scanbase.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4569 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_scanfactory.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6223 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_serie.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1611 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_tomoobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3704 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11616 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_validator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1502 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_version.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2933 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_volume_base.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6186 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/test_volume_utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8574 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/test/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2341 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/tomoobject.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.959406 tomoscan-1.3.1/tomoscan/unitsystem/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1657 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/unitsystem/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2447 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/unitsystem/electriccurrentsystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3270 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/unitsystem/energysystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6542 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/unitsystem/metricsystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3165 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/unitsystem/timesystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1846 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/unitsystem/unit.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1975 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/unitsystem/voltagesystem.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.959406 tomoscan-1.3.1/tomoscan/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)      175 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1120 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/utils/decorator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2976 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/utils/geometry.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2666 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/utils/hdf5.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1512 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/utils/io.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8884 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/utils/volume.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17014 2023-07-19 15:24:18.000000 tomoscan-1.3.1/tomoscan/validator.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4346 2023-08-01 07:13:20.000000 tomoscan-1.3.1/tomoscan/version.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    21318 2023-07-27 11:43:47.000000 tomoscan-1.3.1/tomoscan/volumebase.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-01 07:13:36.955406 tomoscan-1.3.1/tomoscan.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)      951 2023-08-01 07:13:36.000000 tomoscan-1.3.1/tomoscan.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     2741 2023-08-01 07:13:36.000000 tomoscan-1.3.1/tomoscan.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-08-01 07:13:36.000000 tomoscan-1.3.1/tomoscan.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      307 2023-08-01 07:13:36.000000 tomoscan-1.3.1/tomoscan.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        9 2023-08-01 07:13:36.000000 tomoscan-1.3.1/tomoscan.egg-info/top_level.txt
```

### Comparing `tomoscan-1.3.0a4/LICENSE` & `tomoscan-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/PKG-INFO` & `tomoscan-1.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.3.0a4
+Version: 1.3.1
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.3.0a4/README.md` & `tomoscan-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/setup.cfg` & `tomoscan-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 install_requires = 
 	setuptools
 	h5py>=3.0
 	silx>=0.14a
 	lxml
 	dicttoxml
 	packaging
+	psutil
 
 [options.extras_require]
 doc = 
 	Sphinx>=4.0.0, <5.2.0
 	nbsphinx
 	pandoc
 	ipykernel
```

### Comparing `tomoscan-1.3.0a4/setup.py` & `tomoscan-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/__init__.py` & `tomoscan-1.3.1/tomoscan/esrf/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/identifier/__init__.py` & `tomoscan-1.3.1/tomoscan/esrf/identifier/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/identifier/edfidentifier.py` & `tomoscan-1.3.1/tomoscan/esrf/identifier/edfidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/identifier/folderidentifier.py` & `tomoscan-1.3.1/tomoscan/esrf/identifier/folderidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/identifier/hdf5Identifier.py` & `tomoscan-1.3.1/tomoscan/esrf/identifier/hdf5Identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/identifier/jp2kidentifier.py` & `tomoscan-1.3.1/tomoscan/esrf/identifier/jp2kidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/identifier/rawidentifier.py` & `tomoscan-1.3.1/tomoscan/esrf/identifier/rawidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/identifier/tiffidentifier.py` & `tomoscan-1.3.1/tomoscan/esrf/identifier/tiffidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/identifier/url_utils.py` & `tomoscan-1.3.1/tomoscan/esrf/identifier/url_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/scan/edfscan.py` & `tomoscan-1.3.1/tomoscan/esrf/scan/edfscan.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/edfframereducer.py` & `tomoscan-1.3.1/tomoscan/esrf/scan/framereducer/edfframereducer.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/scan/framereducer/hdf5framereducer.py` & `tomoscan-1.3.1/tomoscan/esrf/scan/framereducer/hdf5framereducer.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/scan/hdf5scan.py` & `tomoscan-1.3.1/tomoscan/esrf/scan/hdf5scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 from tomoscan.io import HDF5File
 from tomoscan.nexus.paths.nxtomo import get_paths as _get_nexus_paths
 from tomoscan.scanbase import FOV, Source, TomoScanBase
 from tomoscan.unitsystem import electriccurrentsystem, energysystem, timesystem
 from tomoscan.unitsystem.metricsystem import MetricSystem
 from tomoscan.unitsystem.unit import Unit
 from tomoscan.utils import BoundingBox1D, BoundingBox3D, docstring
+from tomoscan.esrf.scan.utils import (
+    dataset_has_broken_vds,
+    check_possible_issue_with_rlimit,
+)
 
 from .utils import get_compacted_dataslices
 
 _logger = logging.getLogger(__name__)
 
 
 class ImageKey(_Enum):
@@ -205,14 +209,36 @@
         self._end_time = None
         self._x_translations = None
         self._y_translations = None
         self._z_translations = None
         self._nexus_paths = None
         self._nexus_version = None
         self._user_nx_version = nx_version
+        self.__detector_broken_vds_behavior = {
+            "run_check": True,  # check vds
+            "raise_error": False,  # if met an error raise it
+            "log_level": logging.WARNING,  # if met an error log it with the following level
+        }
+        # behavior to get when check detector vds
+
+    def set_check_behavior(
+        self, run_check=True, raise_error=False, log_level=logging.WARNING
+    ):
+        """
+        when user require to access to scan frames HDF5TomoScan build them (`frames` property).
+        Some check can be made during this stage to know if the scan has some broken virtual-dataset (vds) or
+        if the vds is linked to more file than the system might handle.
+
+        In this case the 'vds-check' can either raise an error or log potential issues with a specific log level
+        """
+        self.__detector_broken_vds_behavior = {
+            "run_check": run_check,
+            "raise_error": raise_error,
+            "log_level": log_level,
+        }
 
     @staticmethod
     def get_master_file(scan_path):
         if os.path.isfile(scan_path):
             master_file = scan_path
         else:
             master_file = os.path.join(scan_path, os.path.basename(scan_path))
@@ -993,14 +1019,16 @@
                 intensity_monitor = [None] * len(image_keys)
             if image_keys is not None and len(image_keys) != len(rotation_angles):
                 raise ValueError(
                     "`rotation_angle` and `image_key` have incoherent size "
                     f"({len(rotation_angles)} vs {len(image_keys)}). Unable to deduce frame properties"
                 )
             self._frames = []
+            if self.__detector_broken_vds_behavior["run_check"]:
+                self._checkDetectorDataset()
 
             if image_keys is None:
                 # in the case there is no frame / image keys registered at all
                 return self._frames
 
             for i_frame, rot_a, img_key, x_tr, y_tr, z_tr, i_m in zip(
                 range(len(rotation_angles)),
@@ -1188,24 +1216,42 @@
             unit = default_unit
         # handle Diamond dataset where unit is stored as bytes
         if hasattr(unit, "decode"):
             unit = unit.decode()
         return value * default_unit.from_value(unit).value
 
     def _check_hdf5scan_validity(self):
+        """some basic check to make sure both the master file (.nx file) and requested entry (data_path) exists"""
         if self.master_file is None:
             raise ValueError("No master file provided")
         if self.entry is None:
             raise ValueError("No entry provided")
         with HDF5File(self.master_file, "r") as h5_file:
             if self._entry not in h5_file:
                 raise ValueError(
                     f"Given entry {self._entry} is not in the master file {self.master_file}"
                 )
 
+    def _checkDetectorDataset(self):
+        """check that detector dataset is valid - especially in the case this is a vds"""
+        url = DataUrl(
+            file_path=os.path.abspath(self.master_file),
+            data_path=self.get_detector_data_path(),
+        )
+        dataset_has_broken_vds(
+            url=url,
+            raise_error=self.__detector_broken_vds_behavior["raise_error"],
+            log_level=self.__detector_broken_vds_behavior["log_level"],
+        )
+        check_possible_issue_with_rlimit(
+            url=url,
+            raise_error=self.__detector_broken_vds_behavior["raise_error"],
+            log_level=self.__detector_broken_vds_behavior["log_level"],
+        )
+
     def get_flat_expected_location(self):
         return DataUrl(
             file_path=self.master_file,
             data_path=_get_nexus_paths(self.nexus_version).PROJ_PATH,
         ).path()
 
     def get_dark_expected_location(self):
```

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/scan/mock.py` & `tomoscan-1.3.1/tomoscan/esrf/scan/mock.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/scan/utils.py` & `tomoscan-1.3.1/tomoscan/esrf/scan/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 
 
 import contextlib
 import fnmatch
 import logging
 import os
 import sys
+import psutil
 import warnings
 from typing import Iterable, Union
+import resource
 
 import fabio
 import h5py
 import numpy
 from silx.io.dictdump import h5todict
 from silx.io.url import DataUrl
 from silx.io.utils import get_data as silx_get_data
@@ -281,32 +283,112 @@
 @deprecated(replacement="tomoscan.serie.serie_is_complete", since_version="0.8.0")
 def grp_is_complete(scans: Iterable) -> bool:
     from tomoscan.serie import serie_is_complete_from_group_size
 
     return serie_is_complete_from_group_size(scans)
 
 
-def dataset_has_broken_vds(url: DataUrl):
+def __get_log_fct(log_level):
+    if log_level is logging.WARNING:
+        return _logger.warning
+    elif log_level is logging.ERROR:
+        return _logger.error
+    elif log_level is logging.DEBUG:
+        return _logger.debug
+    elif log_level is logging.INFO:
+        return _logger.info
+    elif log_level is logging.CRITICAL:
+        return _logger.critical
+    else:
+        raise ValueError("logging level unrecognized")
+
+
+def dataset_has_broken_vds(
+    url: DataUrl, raise_error=False, log_level=logging.WARNING
+) -> bool:
     """
     check that the provided url is not a VDS with broken links.
     """
     if not isinstance(url, DataUrl):
         raise TypeError(f"{url} is expected to be an instance of {DataUrl}")
     with HDF5File(url.file_path(), mode="r") as h5f:
-        dataset = h5f[url.data_path()]
+        dataset = h5f.get(url.data_path(), None)
+        if dataset is None:
+            msg = f"no data found at {url.file_path()}://{url.data_path()}"
+            if raise_error:
+                raise ValueError(msg)
+            else:
+                __get_log_fct(log_level)(msg)
+            return True
+
         if not dataset.is_virtual:
             return False
         else:
-            for file_ in get_unique_files_linked(url=url):
-                if not os.path.exists(file_):
-                    _logger.warning(f"{file_} does not exists")
-                    return True
+            missing_files = tuple(
+                filter(
+                    lambda file_: not os.path.exists(file_),
+                    get_unique_files_linked(url=url),
+                )
+            )
+            if len(missing_files) > 0:
+                msg = f"dataset {url.file_path()} has broken virtual-dataset at {url.data_path()}. {missing_files} missing"
+
+                __get_log_fct(log_level)(msg)
+                if raise_error:
+                    raise OSError(msg)
+                return True
+
     return False
 
 
+def check_possible_issue_with_rlimit(
+    url: DataUrl,
+    raise_error=False,
+    log_level=logging.WARNING,
+    delta_n_file=0,
+    substract_current_open=True,
+) -> bool:
+    """
+    check that the provided url does not contain more external file than (ulimit - delta_ulimit).
+    Else if this limit is reached we will probably met some troubles when reading data.
+    Once this limit is reached - vds data will return 0 only - silently
+    """
+    # first check if dataset is virtual, else skip test
+    with HDF5File(url.file_path(), mode="r") as h5f:
+        dataset = h5f.get(url.data_path(), None)
+        if dataset is None:
+            msg = f"no data found at {url.file_path()}://{url.data_path()}"
+            if raise_error:
+                raise ValueError(msg)
+            else:
+                __get_log_fct(log_level)(msg)
+            return True
+
+        if not dataset.is_virtual:
+            return False
+
+    n_files = len(get_unique_files_linked(url=url))
+    if substract_current_open:
+        current_process = psutil.Process()
+        n_open_file_currently = len(current_process.open_files())
+    else:
+        n_open_file_currently = 0
+    try:
+        rlimit = resource.getrlimit(resource.RLIMIT_NOFILE)[0]
+    except (ValueError, OSError):
+        _logger.warning("Failed to check_possible_issue_with_rlimit")
+    else:
+        might_met_troubles = n_files > (rlimit - delta_n_file - n_open_file_currently)
+        if might_met_troubles:
+            msg = f"too much external files to open from {url.path()} - contains {n_files} external files. OS rlimit is set to {rlimit}"
+            __get_log_fct(log_level)(msg)
+            if raise_error:
+                raise OSError(msg)
+
+
 def get_datasets_linked_to_vds(url: DataUrl):
     """
     Return set([file-path, data_path]) linked to the provided url
     """
     if not isinstance(url, DataUrl):
         raise TypeError(f"{url} is expected to be an instance of {DataUrl}")
     start_file_path = url.file_path()
```

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/__init__.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/edfvolume.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/edfvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/hdf5volume.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/hdf5volume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/jp2kvolume.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/jp2kvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/mock.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/mock.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/rawvolume.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/rawvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/singleframebase.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/singleframebase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/tiffvolume.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/tiffvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/esrf/volume/utils.py` & `tomoscan-1.3.1/tomoscan/esrf/volume/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/factory.py` & `tomoscan-1.3.1/tomoscan/factory.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/framereducerbase.py` & `tomoscan-1.3.1/tomoscan/framereducerbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/identifier.py` & `tomoscan-1.3.1/tomoscan/identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/io.py` & `tomoscan-1.3.1/tomoscan/io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/nexus/paths/nxdetector.py` & `tomoscan-1.3.1/tomoscan/nexus/paths/nxdetector.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/nexus/paths/nxsample.py` & `tomoscan-1.3.1/tomoscan/nexus/paths/nxsample.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/nexus/paths/nxtomo.py` & `tomoscan-1.3.1/tomoscan/nexus/paths/nxtomo.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/normalization.py` & `tomoscan-1.3.1/tomoscan/normalization.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/progress.py` & `tomoscan-1.3.1/tomoscan/progress.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/scanbase.py` & `tomoscan-1.3.1/tomoscan/scanbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/serie.py` & `tomoscan-1.3.1/tomoscan/serie.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_framereducerbase.py` & `tomoscan-1.3.1/tomoscan/test/test_framereducerbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_io.py` & `tomoscan-1.3.1/tomoscan/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_normalization.py` & `tomoscan-1.3.1/tomoscan/test/test_normalization.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_progress.py` & `tomoscan-1.3.1/tomoscan/test/test_progress.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_scanbase.py` & `tomoscan-1.3.1/tomoscan/test/test_scanbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_scanfactory.py` & `tomoscan-1.3.1/tomoscan/test/test_scanfactory.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_serie.py` & `tomoscan-1.3.1/tomoscan/test/test_serie.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_tomoobject.py` & `tomoscan-1.3.1/tomoscan/test/test_tomoobject.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_utils.py` & `tomoscan-1.3.1/tomoscan/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_validator.py` & `tomoscan-1.3.1/tomoscan/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_version.py` & `tomoscan-1.3.1/tomoscan/test/test_version.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_volume_base.py` & `tomoscan-1.3.1/tomoscan/test/test_volume_base.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/test_volume_utils.py` & `tomoscan-1.3.1/tomoscan/test/test_volume_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/test/utils.py` & `tomoscan-1.3.1/tomoscan/test/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/tomoobject.py` & `tomoscan-1.3.1/tomoscan/tomoobject.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/unitsystem/__init__.py` & `tomoscan-1.3.1/tomoscan/unitsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/unitsystem/electriccurrentsystem.py` & `tomoscan-1.3.1/tomoscan/unitsystem/electriccurrentsystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/unitsystem/energysystem.py` & `tomoscan-1.3.1/tomoscan/unitsystem/energysystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/unitsystem/metricsystem.py` & `tomoscan-1.3.1/tomoscan/unitsystem/metricsystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/unitsystem/timesystem.py` & `tomoscan-1.3.1/tomoscan/unitsystem/timesystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/unitsystem/unit.py` & `tomoscan-1.3.1/tomoscan/unitsystem/unit.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/unitsystem/voltagesystem.py` & `tomoscan-1.3.1/tomoscan/unitsystem/voltagesystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/utils/decorator.py` & `tomoscan-1.3.1/tomoscan/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/utils/geometry.py` & `tomoscan-1.3.1/tomoscan/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/utils/hdf5.py` & `tomoscan-1.3.1/tomoscan/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/utils/io.py` & `tomoscan-1.3.1/tomoscan/utils/io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/utils/volume.py` & `tomoscan-1.3.1/tomoscan/utils/volume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/validator.py` & `tomoscan-1.3.1/tomoscan/validator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan/version.py` & `tomoscan-1.3.1/tomoscan/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
     "gamma": 12,
     "rc": 13,
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 3
-MICRO = 0
-RELEV = "alpha"  # <16
+MICRO = 1
+RELEV = "final"  # <16
 SERIAL = 4  # <16
 
 date = __date__
 
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
```

### Comparing `tomoscan-1.3.0a4/tomoscan/volumebase.py` & `tomoscan-1.3.1/tomoscan/volumebase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a4/tomoscan.egg-info/PKG-INFO` & `tomoscan-1.3.1/tomoscan.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.3.0a4
+Version: 1.3.1
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.3.0a4/tomoscan.egg-info/SOURCES.txt` & `tomoscan-1.3.1/tomoscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

