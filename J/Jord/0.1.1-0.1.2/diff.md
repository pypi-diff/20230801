# Comparing `tmp/Jord-0.1.1.tar.gz` & `tmp/Jord-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jord-0.1.1.tar", last modified: Wed Jul 26 11:10:25 2023, max compression
+gzip compressed data, was "Jord-0.1.2.tar", last modified: Tue Aug  1 06:14:07 2023, max compression
```

## Comparing `Jord-0.1.1.tar` & `Jord-0.1.2.tar`

### file list

```diff
@@ -1,149 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.532286 Jord-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-26 11:10:18.000000 Jord-0.1.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-26 11:10:18.000000 Jord-0.1.1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 11:10:18.000000 Jord-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:18.000000 Jord-0.1.1/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 11:10:25.000000 Jord-0.1.1/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 11:10:18.000000 Jord-0.1.1/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-26 11:10:18.000000 Jord-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-26 11:10:18.000000 Jord-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-26 11:10:25.532286 Jord-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-26 11:10:18.000000 Jord-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-26 11:10:18.000000 Jord-0.1.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 11:10:18.000000 Jord-0.1.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/jord/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.516286 Jord-0.1.1/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geojson_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geojson_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geopandas_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geopandas_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geopandas_utilities/geometry_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/geopandas_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/pillow_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/pillow_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/pillow_utilities/exif.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/configuration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/configuration/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.520286 Jord-0.1.1/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/conversion/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/conversion/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/helpers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/numpy_utilities/rasters.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/plugin_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qgis_utilities/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.524286 Jord-0.1.1/jord/qlive_utilities/clients/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/clients/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/clients/interfaced.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/qt_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qt_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/rasterio_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/shapely_utilities/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/analysis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/analysis/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/clamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/mirroring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/sanitise_poly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/shapely_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/serialisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/serialisation/well_known_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/serialisation/well_known_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/spatialite_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/spatialite_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.528286 Jord-0.1.1/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/torch_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-26 11:10:18.000000 Jord-0.1.1/jord/torch_utilities/geodata_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-26 11:10:18.000000 Jord-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 11:10:18.000000 Jord-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 11:10:25.532286 Jord-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-07-26 11:10:18.000000 Jord-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.532286 Jord-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:10:25.532286 Jord-0.1.1/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 11:10:18.000000 Jord-0.1.1/tests/qgis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-26 11:10:18.000000 Jord-0.1.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 11:10:18.000000 Jord-0.1.1/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.328316 Jord-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.308315 Jord-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-01 06:13:58.000000 Jord-0.1.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 06:13:58.000000 Jord-0.1.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 06:13:58.000000 Jord-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:13:58.000000 Jord-0.1.2/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 06:13:58.000000 Jord-0.1.2/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-01 06:13:58.000000 Jord-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 06:13:58.000000 Jord-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-01 06:14:07.328316 Jord-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 06:13:58.000000 Jord-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-01 06:13:58.000000 Jord-0.1.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:13:58.000000 Jord-0.1.2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/jord/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geojson_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geojson_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geopandas_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geopandas_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geopandas_utilities/geometry_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/pillow_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/pillow_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/pillow_utilities/exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/configuration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/configuration/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/conversion/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/rasters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/plugin_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qgis_utilities/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qlive_utilities/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/clients/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/clients/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/qgis_layer_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qt_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qt_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/rasterio_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/shapely_utilities/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/analysis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/analysis/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/mirroring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/sanitise_poly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/shapely_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/serialisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/serialisation/well_known_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/serialisation/well_known_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/spatialite_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/spatialite_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/torch_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/torch_utilities/geodata_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-01 06:13:58.000000 Jord-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 06:13:58.000000 Jord-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-01 06:14:07.328316 Jord-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-08-01 06:13:58.000000 Jord-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.328316 Jord-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.328316 Jord-0.1.2/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 06:13:58.000000 Jord-0.1.2/tests/qgis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-01 06:13:58.000000 Jord-0.1.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 06:13:58.000000 Jord-0.1.2/tests/test_sanity.py
```

### Comparing `Jord-0.1.1/.github/CODE_OF_CONDUCT.md` & `Jord-0.1.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/.github/CONTRIBUTING.md` & `Jord-0.1.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/Jord.egg-info/PKG-INFO` & `Jord-0.1.2/Jord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.1.1 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.1.2 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
```

### Comparing `Jord-0.1.1/Jord.egg-info/SOURCES.txt` & `Jord-0.1.2/Jord.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,19 @@
 jord/qgis_utilities/shapely_utilities/README.md
 jord/qgis_utilities/shapely_utilities/__init__.py
 jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
 jord/qlive_utilities/README.md
 jord/qlive_utilities/__init__.py
 jord/qlive_utilities/client.py
 jord/qlive_utilities/procedures.py
+jord/qlive_utilities/qgis_layer_creation.py
 jord/qlive_utilities/serialisation.py
 jord/qlive_utilities/uri_utilities.py
 jord/qlive_utilities/clients/__init__.py
+jord/qlive_utilities/clients/arguments.py
 jord/qlive_utilities/clients/auto.py
 jord/qlive_utilities/clients/interfaced.py
 jord/qt_utilities/__init__.py
 jord/qt_utilities/enums.py
 jord/rasterio_utilities/README.md
 jord/rasterio_utilities/__init__.py
 jord/shapely_utilities/README.md
```

### Comparing `Jord-0.1.1/Jord.egg-info/requires.txt` & `Jord-0.1.2/Jord.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 numpy>=1.20.2
 warg>=1.1.6
 apppath>=1.0.2
 sorcery
 pyzmq
+tqdm
 
 [all]
-sphinxcontrib-programoutput
-Pillow
-pip>=22.1.2
-wheel>=0.33.0
-pre-commit>=2.17.0
-sphinx>=4.0.1
-pyzmq
 pytest>=4.4.1
-apppath>=1.0.2
 coveralls>=1.6.0
-pytest>=4.3.0
+furo
+Pillow
+numpy>=1.20.2
+warg>=1.1.6
 mock
-black[jupyter]>=21.5b0
+apppath>=1.0.2
 sorcery
+pre-commit>=2.17.0
+tqdm
+sphinxcontrib-programoutput
 twine>=1.13.0
+sphinx>=4.0.1
+wheel>=0.33.0
+black[jupyter]>=21.5b0
+pip>=22.1.2
+pytest>=4.3.0
+pyzmq
 pytest-cov>=2.11.1
-furo
-warg>=1.1.6
-numpy>=1.20.2
 
 [dev]
-sphinxcontrib-programoutput
-pytest>=4.3.0
-mock
-wheel>=0.33.0
-black[jupyter]>=21.5b0
-furo
+pytest>=4.4.1
 coveralls>=1.6.0
-pre-commit>=2.17.0
-sphinx>=4.0.1
-warg>=1.1.6
+furo
+mock
 numpy>=1.20.2
+warg>=1.1.6
+apppath>=1.0.2
 sorcery
+pre-commit>=2.17.0
+sphinxcontrib-programoutput
+tqdm
 twine>=1.13.0
-pytest>=4.4.1
-pytest-cov>=2.11.1
-pyzmq
-apppath>=1.0.2
+sphinx>=4.0.1
+wheel>=0.33.0
+black[jupyter]>=21.5b0
 pip>=22.1.2
+pytest>=4.3.0
+pyzmq
+pytest-cov>=2.11.1
 
 [docs]
+sphinx>=4.0.1
 sphinxcontrib-programoutput
 furo
-sphinx>=4.0.1
 
 [extra]
 
 [gdal]
 
 [pil]
 Pillow
 
 [samples]
 
 [setup]
 
 [tests]
-mock
 pytest>=4.4.1
+mock
```

### Comparing `Jord-0.1.1/LICENSE.md` & `Jord-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/PKG-INFO` & `Jord-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.1.1 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.1.2 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
```

### Comparing `Jord-0.1.1/README.md` & `Jord-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/SECURITY.md` & `Jord-0.1.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/__init__.py` & `Jord-0.1.2/jord/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 
 import datetime
 import os
 from pathlib import Path
 from typing import Any
 from warnings import warn
 
-import pkg_resources
+from importlib import resources
+from importlib.metadata import PackageNotFoundError
+from warg import package_is_editable
 from apppath import AppPath
 from warg import dist_is_editable
 
 __project__ = "Jord"
 __author__ = "Christian Heider Nielsen"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Nielsen <christian.heider@alexandra.dk>
 
@@ -31,22 +33,21 @@
 
 PROJECT_NAME = __project__.lower().strip().replace(" ", "_")
 PROJECT_VERSION = __version__
 PROJECT_YEAR = 2018
 PROJECT_AUTHOR = __author__.lower().strip().replace(" ", "_")
 PROJECT_ORGANISATION = "Automaps"
 PROJECT_APP_PATH = AppPath(app_name=PROJECT_NAME, app_author=PROJECT_AUTHOR)
-PACKAGE_DATA_PATH = Path(pkg_resources.resource_filename(PROJECT_NAME, "data"))
 INCLUDE_PROJECT_READMES = False
 
-distributions = {v.key: v for v in pkg_resources.working_set}
-if PROJECT_NAME in distributions:
-    distribution = distributions[PROJECT_NAME]
-    DEVELOP = dist_is_editable(distribution)
-else:
+PACKAGE_DATA_PATH = resources.files(PROJECT_NAME) / "data"
+
+try:
+    DEVELOP = package_is_editable(PROJECT_NAME)
+except PackageNotFoundError as e:
     DEVELOP = True
 
 
 def get_version(append_time: Any = DEVELOP) -> str:
     """
       :param append_time:
 
@@ -92,7 +93,11 @@
     return version
 
 
 if __version__ is None:
     __version__ = get_version(append_time=True)
 
 __version_info__ = tuple(int(segment) for segment in __version__.split("."))
+
+
+if __name__ == "__main__":
+    print(PROJECT_APP_PATH.user_cache)
```

### Comparing `Jord-0.1.1/jord/gdal_utilities/__init__.py` & `Jord-0.1.2/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/gdal_utilities/cloning.py` & `Jord-0.1.2/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/gdal_utilities/context.py` & `Jord-0.1.2/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/gdal_utilities/conversion.py` & `Jord-0.1.2/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/gdal_utilities/importing.py` & `Jord-0.1.2/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/gdal_utilities/persistence.py` & `Jord-0.1.2/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/geojson_utilities/geometry_types.py` & `Jord-0.1.2/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/geopandas_utilities/geometry_filtering.py` & `Jord-0.1.2/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/qgis_utilities/__init__.py` & `Jord-0.1.2/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/qgis_utilities/categorisation.py` & `Jord-0.1.2/jord/qgis_utilities/categorisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import random
 from itertools import cycle
 from typing import Iterable, Sized, Callable, Generator
 
 from PyQt5.Qt import QColor
+
+# noinspection PyUnresolvedReferences
 from qgis.core import (
     QgsVectorLayer,
     QgsSymbol,
     QgsRendererCategory,
     QgsCategorizedSymbolRenderer,
 )
+
 from warg import TripleNumber, QuadNumber, n_uint_mix_generator_builder
 
 __all__ = ["categorise_layer"]
 
 
 def random_rgb(mix: TripleNumber = (255, 255, 255)) -> TripleNumber:
     red = random.randrange(0, mix[0])
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/configuration/plugin_settings.py` & `Jord-0.1.2/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,39 +7,44 @@
            Created on 02-12-2020
            """
 
 __all__ = ["store_plugin_setting", "read_plugin_setting"]
 
 from typing import Any
 
-from qgis.core import QgsSettings
 
 from jord import PROJECT_NAME
 
 
 def store_plugin_setting(key: str, value: Any, *, project_name: str = PROJECT_NAME):
     """
 
     :param key:
     :param value:
     :param project_name:
     :return:
     """
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsSettings
+
     QgsSettings().setValue(f"{project_name}/{key}", value)
 
 
 def read_plugin_setting(
     key: str, *, default_value: Any = None, project_name: str = PROJECT_NAME
 ):
     """
 
     :param key:
     :param default_value:
     :param project_name:
     :return:
     """
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsSettings
+
     return QgsSettings().value(f"{project_name}/{key}", default_value)
 
 
 if __name__ == "__main__":
     store_plugin_setting("mytext", "hello world")
     print(read_plugin_setting("mytext"))
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/configuration/project_settings.py` & `Jord-0.1.2/jord/qgis_utilities/configuration/project_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,17 @@
     "read_project_setting",
     "restore_default_project_settings",
 ]
 
 from logging import warning
 from typing import Any, Mapping, Optional
 
-from qgis.core import QgsProject
 
 from jord import PROJECT_NAME
 
-qgis_project = QgsProject.instance()
-
 
 def restore_default_project_settings(
     defaults: Optional[Mapping] = None, *, project_name: str = PROJECT_NAME
 ):
     """
 
     :param defaults:
@@ -42,14 +39,19 @@
     """
 
     :param key:
     :param value:
     :param project_name:
     :return:
     """
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsProject
+
+    qgis_project = QgsProject.instance()
+
     if isinstance(value, bool):
         qgis_project.writeEntryBool(project_name, key, value)
     elif isinstance(value, float):
         qgis_project.writeEntryDouble(project_name, key, value)
     # elif isinstance(value, int): # DOES NOT EXIST!
     #    qgis_project.writeEntryNum(project_name, key, value)
     else:
@@ -70,14 +72,18 @@
 
     :param key:
     :param type_hint:
     :param defaults:
     :param project_name:
     :return:
     """
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsProject
+
+    qgis_project = QgsProject.instance()
 
     # read values (returns a tuple with the value, and a status boolean
     # which communicates whether the value retrieved could be converted to
     # its type, in these cases a string, an integer, a double and a boolean
     # respectively)
 
     if defaults is None:
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/geometry_types.py` & `Jord-0.1.2/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/qgis_utilities/helpers/actions.py` & `Jord-0.1.2/jord/qgis_utilities/helpers/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 from PyQt5.QtGui import QIcon
 from PyQt5.QtWidgets import QAction, QWidget
+
 from jord.qgis_utilities.helpers.signals import reconnect_signal
 
 
 __all__ = ["create_action"]
 
 
 def create_action(
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/helpers/drawing.py` & `Jord-0.1.2/jord/qgis_utilities/helpers/drawing.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,24 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 02-12-2020
            """
 
+# noinspection PyUnresolvedReferences
 from qgis.PyQt import QtGui
+
+# noinspection PyUnresolvedReferences
 from qgis.PyQt.QtCore import Qt
+
+# noinspection PyUnresolvedReferences
 from qgis.core import QgsWkbTypes
+
+# noinspection PyUnresolvedReferences
 from qgis.gui import QgsMapCanvas, QgsRubberBand
 
 __all__ = ["make_rubber_band"]
 
 
 def make_rubber_band(canvas: QgsMapCanvas) -> QgsRubberBand:
     """
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/helpers/environment.py` & `Jord-0.1.2/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/qgis_utilities/helpers/models.py` & `Jord-0.1.2/jord/qgis_utilities/helpers/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 __doc__ = r"""
 
            Created on 02-12-2020
            """
 
 from typing import Any, Optional, Tuple
 
+# noinspection PyUnresolvedReferences
 from qgis.PyQt import QtCore
 
 __all__ = ["MyTableModel"]
 
 
 # noinspection PyPep8Naming
 class MyTableModel(QtCore.QAbstractTableModel):
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/helpers/progress_bar.py` & `Jord-0.1.2/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 __doc__ = r"""
 
            Created on 02-12-2020
            """
 
 from typing import Tuple
 
+# noinspection PyUnresolvedReferences
 from qgis.PyQt import QtGui, QtWidgets
 
 __all__ = ["dialog_progress_bar"]
 
 
 def dialog_progress_bar(
     progress: int = 0, *, minimum_width: int = 300
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/helpers/signals.py` & `Jord-0.1.2/jord/qgis_utilities/helpers/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
            Created on 02-12-2020
            """
 
 __all__ = ["disconnect_signal", "connect_signal", "reconnect_signal"]
 
 from logging import warning
 
+# noinspection PyUnresolvedReferences
 from qgis.PyQt import QtCore
 
 IS_DEBUGGING = False
 
 
 def connect_signal(signal: QtCore.pyqtSignal, new_handler: callable = None) -> None:
     """
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/numpy_utilities/conversion.py` & `Jord-0.1.2/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,19 @@
            Created on 02-12-2020
            """
 
 from typing import Sequence
 
 import numpy
 from PIL import Image
+
+# noinspection PyUnresolvedReferences
 from qgis.PyQt import QtGui
+
+# noinspection PyUnresolvedReferences
 from qgis.core import (
     QgsCoordinateReferenceSystem,
     QgsCoordinateTransform,
     QgsPoint,
     QgsVectorLayer,
 )
 
@@ -92,15 +96,15 @@
 
 
     :param layer:
     :return:
 
     """
 
-    layerRectangle = layer.extent()
+    layer_rectangle = layer.extent()
 
     return [
-        layerRectangle.xMinimum(),
-        layerRectangle.yMinimum(),
-        layerRectangle.xMaximum(),
-        layerRectangle.yMaximum(),
+        layer_rectangle.xMinimum(),
+        layer_rectangle.yMinimum(),
+        layer_rectangle.xMaximum(),
+        layer_rectangle.yMaximum(),
     ]
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/numpy_utilities/data_type.py` & `Jord-0.1.2/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from enum import Enum
 from typing import Any
 
 import numpy
-from qgis.core import (
-    Qgis,
-)
+from qgis.core import Qgis
 
 
 class QgisDataTypeEnum(Enum):
     unknown = Qgis.UnknownDataType  # Unknown or unspecified type.
 
     # int8 = Qgis.Int8  # Eight bit signed integer (qint8) (added in QGIS 3.30)
     int16 = Qgis.Int16  # Sixteen bit signed integer (qint16)
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `Jord-0.1.2/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py` & `Jord-0.1.2/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+# noinspection PyUnresolvedReferences
 from qgis.core import *  # attach main QGIS library
+
+# noinspection PyUnresolvedReferences
 from qgis.utils import *  # attach main python library
 
 
 def single_vector_layer():
     # Attach libraries
 
     import os  # attach operating system library
```

### Comparing `Jord-0.1.1/jord/qgis_utilities/styling.py` & `Jord-0.1.2/jord/qgis_utilities/styling.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from typing import Mapping
 
-from PyQt5.QtGui import QColor
-from warg import TripleNumber
-import random
-from itertools import cycle
-from typing import Any, Iterable, Sized
 
 from PyQt5.Qt import QColor
+
+# noinspection PyUnresolvedReferences
 from qgis.core import (
     QgsVectorLayer,
     QgsSymbol,
     QgsRendererCategory,
     QgsCategorizedSymbolRenderer,
     QgsLineSymbol,
 )
```

### Comparing `Jord-0.1.1/jord/qlive_utilities/client.py` & `Jord-0.1.2/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/qlive_utilities/clients/auto.py` & `Jord-0.1.2/jord/qlive_utilities/clients/auto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 from functools import partial
 from typing import Callable
-import inspect
-from enum import Enum
 from jord.qlive_utilities import (
     QliveClient,
     QliveRPCMethodEnum,
     QliveRPCMethodMap,
     build_package,
 )
 
 
 __all__ = ["AutoQliveClient"]
 
-
-class DisSatisfactionEnum(Enum):
-    none = "none"
-    args = "args"
-    kws = "kws"
-    argskws = "argskws"
-
-
-def partial_satisfied(partial_fn: Callable) -> bool:
-    signature = inspect.signature(partial_fn.func)
-    try:
-        signature.bind(*partial_fn.args, **partial_fn.keywords)
-        return True
-    except TypeError:
-        return False
+from jord.qlive_utilities.clients.arguments import partial_satisfied
 
 
 class AutoQliveClient(QliveClient):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         for method in QliveRPCMethodEnum:
```

### Comparing `Jord-0.1.1/jord/qlive_utilities/procedures.py` & `Jord-0.1.2/jord/qlive_utilities/procedures.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-import json
 import time
+import uuid
 from enum import Enum
-
-from typing import Mapping, Any, Tuple, Optional
-
+from typing import Mapping, Any, Tuple
 
 import numpy
 import shapely.geometry.base
-from warg import passes_kws_to, Number
-from jord.geojson_utilities import GeoJsonGeometryTypesEnum
+import tqdm
 from pandas import DataFrame
 from shapely.geometry.base import BaseGeometry
-from shapely.geometry import GeometryCollection
+from warg import ensure_existence
+from warg import passes_kws_to, Number
 
+from jord import PROJECT_APP_PATH
+from jord.qlive_utilities.qgis_layer_creation import add_qgis_geometry
 
 APPEND_TIMESTAMP = True
 SKIP_MEMORY_LAYER_CHECK_AT_CLOSE = True
 PIXEL_SIZE = 1
 DEFAULT_NUMBER = 0
 CONTRAST_ENHANCE = True
 DEFAULT_LAYER_NAME = "TemporaryLayer"
 DEFAULT_LAYER_CRS = "EPSG:4326"
 VERBOSE = False
 
 __all__ = [
     "add_raster",
-    "add_wkb",
-    "add_wkts",
-    "add_wkbs",
     "add_rasters",
     "add_wkt",
+    "add_wkts",
+    "add_wkb",
+    "add_wkbs",
     "add_dataframe",
+    "add_dataframes",
     "add_geojson",
+    "add_shapely_geometry",
+    "add_shapely_geometries",
     "clear_all",
     "remove_layers",
     "QliveRPCMethodEnum",
     "QliveRPCMethodMap",
 ]
 
 
@@ -45,42 +48,45 @@
     name: str = DEFAULT_LAYER_NAME,
     centroid: Tuple[Number, Number] = None,
     extent_tuple: Tuple[Number, Number, Number, Number] = None,
     pixel_size: Tuple[Number, Number] = PIXEL_SIZE,
     crs_str: str = DEFAULT_LAYER_CRS,
     default_value: Number = DEFAULT_NUMBER,
     field: str = None,
+    no_data_value: int = -1,
 ) -> None:
     """
+    add a raster
 
     :param qgis_instance_handle:
     :param raster:
     :param name:
     :param centroid:
     :param extent_tuple:
     :param pixel_size:
     :param crs_str:
     :param default_value:
     :param field:
     :return: None
     :rtype: None
     """
+    # noinspection PyUnresolvedReferences
     from qgis.core import (
         QgsRectangle,
         QgsCoordinateReferenceSystem,
-        QgsRasterBlock,
         QgsRasterBandStats,
         QgsSingleBandGrayRenderer,
         QgsMultiBandColorRenderer,
         QgsContrastEnhancement,
         QgsRasterLayer,
-        QgsProcessing,
+        QgsRasterFileWriter,
+        Qgis,
     )
     from jord.qgis_utilities.numpy_utilities.data_type import get_qgis_type
-    from qgis import processing
+    from jord.qgis_utilities import RasterDataProviderEditSession
 
     x_size, y_size, *rest_size = raster.shape
 
     if len(rest_size) == 0:
         raster = numpy.expand_dims(raster, axis=-1)
 
     *_, num_bands = raster.shape
@@ -104,78 +110,65 @@
             raster_half_size = raster_half_size[1], raster_half_size[0]
 
         extent.setXMinimum(centroid[0] - raster_half_size[0])
         extent.setYMinimum(centroid[1] - raster_half_size[1])
         extent.setXMaximum(centroid[0] + raster_half_size[0])
         extent.setYMaximum(centroid[1] + raster_half_size[1])
 
-    raster_output = processing.run(
-        "qgis:createconstantrasterlayer",
-        {
-            "EXTENT": extent,
-            "TARGET_CRS": QgsCoordinateReferenceSystem(crs_str),  # ("EPSG:2180")
-            "PIXEL_SIZE": pixel_size,
-            "NUMBER": default_value,
-            "OUTPUT_TYPE": data_type.value,
-            "IGNORE_NODATA": True,
-            "OUTPUT_NODATA_VALUE": DEFAULT_NUMBER,
-            "OUTPUT": QgsProcessing.TEMPORARY_OUTPUT,
-        },
-    )["OUTPUT"]
-
     if APPEND_TIMESTAMP:
         name += f"_{time.time()}"
 
-    layer = QgsRasterLayer(raster_output, name, "gdal")
-    provider = layer.dataProvider()
+    temp_file = (
+        ensure_existence(PROJECT_APP_PATH.user_data / "rasters") / f"{uuid.uuid4()}.tif"
+    )
+    writer = QgsRasterFileWriter(temp_file)
+    provider = writer.createMultiBandRaster(
+        dataType=data_type.value,
+        width=x_size,
+        height=y_size,
+        extent=extent,
+        crs=QgsCoordinateReferenceSystem(crs_str),
+        nBands=num_bands,
+    )
 
-    if False:
-        location = None
-        extent = provider.extent()
-        xres = (extent.width()) / provider.xSize()
-        yres = (extent.height()) / provider.ySize()
-        col = int((location.x() - extent.xMinimum()) / xres)
-        row = int((location.y() - extent.yMinimum()) / yres)
-    elif False:
-        raster_extent = provider.extent()
-        raster_width = provider.xSize()
-        raster_height = provider.ySize()
-        no_data_value = provider.srcNoDataValue(1)
-    else:
-        w = layer.width()
-        h = layer.height()
+    if VERBOSE:
+        print("drawing")
 
-    provider.setEditable(True)
-    block = QgsRasterBlock(data_type, w, h)
-    # block = provider.block(1, extent, w, h)
+    w_pixels, h_pixels = x_size, y_size
 
-    for ith_band in range(0, num_bands):
-        if False:
-            for i in range(0, w):
-                for j in range(0, h):
-                    value = raster[i][j][ith_band]
+    with RasterDataProviderEditSession(provider):
+        progress = range(0, num_bands)
+
+        if VERBOSE:
+            progress = tqdm.tqdm(progress)
+
+        for ith_band in progress:
+            block = provider.block(
+                bandNo=ith_band + 1, boundingBox=extent, width=w_pixels, height=h_pixels
+            )
+            provider.setNoDataValue(bandNo=ith_band + 1, noDataValue=no_data_value)
+
+            for wp in range(0, w_pixels):
+                for hp in range(0, h_pixels):
+                    value = raster[wp][hp][ith_band]
                     if value == numpy.nan:
-                        block.setIsNoData(i, j)
+                        block.setIsNoData(wp, hp)
                         continue
-                    value = int(value) * 255
-                    block.setValue(i, j, value)
-        elif True:
-            for i in range(0, w):
-                for j in range(0, h):
-                    block.setValue(i, j, raster[i][j][ith_band])
-        else:
-            block.setData(bytearray(numpy.array(map(lambda x: int(x * 255), raster))))
+                    if False:
+                        value = int(value) * 255
+                    block.setValue(wp, hp, value)
 
-        if VERBOSE:
-            print("writing block on band", ith_band + 1)
+            if VERBOSE:
+                print("writing block on band", ith_band + 1)
+
+            provider.writeBlock(block, band=ith_band + 1, xOffset=0, yOffset=0)
 
-        provider.writeBlock(block, band=ith_band + 1)
+            del block
 
-    provider.setEditable(False)
-    provider.reload()
+    layer = QgsRasterLayer(temp_file, name, "gdal")
 
     if num_bands == 1:
         # this is needed for the min and max value to refresh in the layer panel
         renderer = layer.renderer()
 
         gray_renderer = QgsSingleBandGrayRenderer(provider, 1)
 
@@ -189,21 +182,23 @@
                 QgsContrastEnhancement.StretchToMinimumMaximum, True
             )
             my_enhancement.setMinimumValue(min_value)
             my_enhancement.setMaximumValue(max_value)
             gray_renderer.setContrastEnhancement(my_enhancement)
 
         layer.setRenderer(gray_renderer)
+
     elif num_bands != 4:
         multi_color_renderer = QgsMultiBandColorRenderer(provider, 1, 2, 3)
 
         layer.setRenderer(multi_color_renderer)
         layer.setDefaultContrastEnhancement()
         layer.triggerRepaint()
         # iface.legendInterface().refreshLayerSymbology(layer)
+
     else:
         multi_color_renderer = QgsMultiBandColorRenderer(provider, 1, 2, 3)
 
         layer.setRenderer(multi_color_renderer)
         layer.setDefaultContrastEnhancement()
         layer.triggerRepaint()
 
@@ -223,208 +218,78 @@
     :param kwargs:
     :return:
     """
     for layer_name, raster in rasters.items():
         add_raster(qgis_instance_handle, raster, name=layer_name, **kwargs)
 
 
-def add_geometries(qgis_instance_handle: Any):
-    ...
-
-
-def add_geometry(
-    qgis_instance_handle: Any,
-    geom,  #: QgsGeometry,
-    name: Optional[str] = None,
-    crs: Optional[str] = None,
-    fields: Mapping = None,
-    index: bool = False,
-    categorise_by_attribute: Optional[str] = None,
-) -> None:
-    """
-
-    An example url is “Point?crs=epsg:4326&field=id:integer&field=name:string(20)&index=yes”
-
-    :param fields: Field=name:type(length,precision) Defines an attribute of the layer. Multiple field parameters can be added to the data provider definition. Type is one of “integer”, “double”, “string”.
-    :param index:     index=yes Specifies that the layer will be constructed with a spatial index
-    :param qgis_instance_handle:
-    :param geom:
-    :param name:
-    :param crs: Crs=definition Defines the coordinate reference system to use for the layer. Definition is any string accepted by QgsCoordinateReferenceSystem.createFromString()
-    :return: None
-    :rtype: None
-    """
-
-    from qgis.core import QgsVectorLayer, QgsFeature
-
-    # uri = geom.type()
-    # uri = geom.wkbType()
-    # uri = geom.wktTypeStr()
-
-    geom_type = json.loads(geom.asJson())["type"]
-    uri = geom_type
-
-    if name is None:
-        name = DEFAULT_LAYER_NAME
-
-    if crs is None:
-        crs = DEFAULT_LAYER_CRS
-
-    layer_name = f"{name}"
-    if APPEND_TIMESTAMP:
-        layer_name += f"_{time.time()}"
-
-    if geom_type == GeoJsonGeometryTypesEnum.geometry_collection.value.__name__:
-        gm_group = qgis_instance_handle.temporary_group.addGroup(layer_name)
-
-        for g in geom.asGeometryCollection():  # TODO: Look into recursion?
-            uri = json.loads(g.asJson())["type"]
-            sub_type = uri
-
-            if crs:
-                uri += f"?crs={crs}"
-
-            if fields:
-                for k, v in fields.items():
-                    uri += f"&field={k}:{v}"
-
-            uri += f'&index={"yes" if index else "no"}'
-
-            feat = QgsFeature()
-            feat.setGeometry(g)
-
-            sub_layer = QgsVectorLayer(uri, f"{layer_name}_{sub_type}", "memory")
-            sub_layer.dataProvider().addFeatures([feat])
-
-            if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
-                sub_layer.setCustomProperty("skipMemoryLayersCheck", 1)
-
-            qgis_instance_handle.qgis_project.addMapLayer(sub_layer, False)
-            gm_group.insertLayer(0, sub_layer)
-    elif geom_type == GeoJsonGeometryTypesEnum.multi_point.value.__name__:
-        ...
-    elif geom_type == GeoJsonGeometryTypesEnum.multi_line_string.value.__name__:
-        ...
-    elif geom_type == "CurvePolygon":
-        ...
-    elif geom_type == "MultiSurface":
-        ...
-    elif geom_type == "CompoundCurve":
-        ...
-    elif geom_type == "MultiCurve":
-        ...
-    elif geom_type == GeoJsonGeometryTypesEnum.multi_polygon.value.__name__:
-        gm_group = qgis_instance_handle.temporary_group.addGroup(layer_name)
-
-        g = geom
-        uri = json.loads(g.asJson())["type"]
-        sub_type = uri
-
-        if crs:
-            uri += f"?crs={crs}"
-
-        if fields:
-            for k, v in fields.items():
-                uri += f"&field={k}:{v}"
-
-        uri += f'&index={"yes" if index else "no"}'
-
-        sub_layer = QgsVectorLayer(uri, f"{layer_name}_{sub_type}", "memory")
-
-        features = []
-        for g_ in [g]:
-            feat = QgsFeature()
-            feat.setGeometry(g)
-            features.append(feat)
-
-        sub_layer.dataProvider().addFeatures(features)
-
-        if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
-            sub_layer.setCustomProperty("skipMemoryLayersCheck", 1)
-
-        qgis_instance_handle.qgis_project.addMapLayer(sub_layer, False)
-        gm_group.insertLayer(0, sub_layer)
-    else:
-        if crs:
-            uri += f"?crs={crs}"
-
-        if fields:
-            for k, v in fields.items():
-                uri += f"&field={k}:{v}"
-
-        uri += f'&index={"yes" if index else "no"}'
-
-        feat = QgsFeature()
-        feat.setGeometry(geom)
-
-        layer = QgsVectorLayer(uri, layer_name, "memory")
-        layer.dataProvider().addFeatures([feat])
-
-        if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
-            layer.setCustomProperty("skipMemoryLayersCheck", 1)
-
-        qgis_instance_handle.qgis_project.addMapLayer(layer, False)
-        qgis_instance_handle.temporary_group.insertLayer(0, layer)
-
-
-@passes_kws_to(add_geometry)
+@passes_kws_to(add_qgis_geometry)
 def add_wkb(qgis_instance_handle: Any, wkb: str, **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param wkb:
     :param kwargs:
     :return:
     """
+    # noinspection PyUnresolvedReferences
     from qgis.core import QgsGeometry
 
-    add_geometry(qgis_instance_handle, QgsGeometry.fromWkb(wkb), **kwargs)
+    add_qgis_geometry(qgis_instance_handle, QgsGeometry.fromWkb(wkb), **kwargs)
 
 
-@passes_kws_to(add_geometry)
+@passes_kws_to(add_qgis_geometry)
 def add_wkt(qgis_instance_handle: Any, wkt: str, **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param wkt:
     :param kwargs:
     :return:
     """
+    # noinspection PyUnresolvedReferences
     from qgis.core import QgsGeometry
 
-    add_geometry(qgis_instance_handle, QgsGeometry.fromWkt(wkt), **kwargs)
+    add_qgis_geometry(qgis_instance_handle, QgsGeometry.fromWkt(wkt), **kwargs)
 
 
 @passes_kws_to(add_wkb)
-def add_wkbs(qgis_instance_handle: Any, wkbs: Mapping, **kwargs) -> None:
+def add_wkbs(qgis_instance_handle: Any, wkbs: Mapping[str, str], **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param wkbs:
     :param kwargs:
     :return:
     """
     for layer_name, wkb in wkbs.items():
         add_wkb(qgis_instance_handle, wkb, name=layer_name, **kwargs)
 
 
 @passes_kws_to(add_wkt)
-def add_wkts(qgis_instance_handle: Any, wkts: Mapping, **kwargs) -> None:
+def add_wkts(qgis_instance_handle: Any, wkts: Mapping[str, str], **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param wkts:
     :param kwargs:
     :return:
     """
     for layer_name, wkt in wkts.items():
         add_wkt(qgis_instance_handle, wkt, name=layer_name, **kwargs)
 
 
-@passes_kws_to(add_geometry)
+@passes_kws_to(add_qgis_geometry)
+def add_dataframes(
+    qgis_instance_handle: Any, dataframes: Mapping[str, DataFrame], **kwargs
+) -> None:
+    ...
+
+
+@passes_kws_to(add_qgis_geometry)
 def add_dataframe(qgis_instance_handle: Any, dataframe: DataFrame, **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param dataframe:
     :param kwargs:
     :return:
@@ -460,25 +325,25 @@
         for row in wkts:
             add_wkt(qgis_instance_handle, row)
     else:
         if VERBOSE:
             print("SKIP!")
 
 
-@passes_kws_to(add_geometry)
+@passes_kws_to(add_qgis_geometry)
 def add_geojson(qgis_instance_handle: Any, geojson: str, **kwargs) -> None:
     """
 
     :param qgis_instance_handle:
     :param dataframe:
     :param kwargs:
     :return:
     """
     geom = shapely.from_geojson(geojson)
-    add_shapely(geom)
+    add_shapely_geometry(geom)
 
 
 def remove_layers(qgis_instance_handle: Any, *args) -> None:
     """
     clear all the added layers
 
     :param qgis_instance_handle:
@@ -496,35 +361,54 @@
     :return:
     """
     remove_layers(qgis_instance_handle)
     if VERBOSE:
         print("CLEAR ALL!")
 
 
-def add_shapely(qgis_instance_handle: Any, geom: BaseGeometry, **kwargs) -> None:
+def add_shapely_geometry(
+    qgis_instance_handle: Any, geom: BaseGeometry, **kwargs
+) -> None:
     """
     Add a shapely geometry
 
     :param qgis_instance_handle:
     :param args:
     :return:
     """
 
     add_wkt(qgis_instance_handle, geom.wkt)
 
 
+@passes_kws_to(add_shapely_geometry)
+def add_shapely_geometries(
+    qgis_instance_handle: Any, geometries: Mapping, **kwargs
+) -> None:
+    """
+
+    :param qgis_instance_handle:
+    :param wkbs:
+    :param kwargs:
+    :return:
+    """
+    for layer_name, geometry in geometries.items():
+        add_shapely_geometry(qgis_instance_handle, geometry, name=layer_name, **kwargs)
+
+
 class QliveRPCMethodEnum(Enum):
     # add_layers = add_layers.__name__
     remove_layers = remove_layers.__name__
     clear_all = clear_all.__name__
     add_wkt = add_wkt.__name__
     add_wkb = add_wkb.__name__
     add_wkts = add_wkts.__name__
     add_wkbs = add_wkbs.__name__
     add_dataframe = add_dataframe.__name__
-    add_shapely = add_shapely.__name__
+    add_dataframes = add_dataframes.__name__
+    add_shapely_geometry = add_shapely_geometry.__name__
+    add_shapely_geometries = add_shapely_geometries.__name__
     add_raster = add_raster.__name__
     add_rasters = add_rasters.__name__
 
 
 funcs = locals()  # In local scope for name
 QliveRPCMethodMap = {e: funcs[e.value] for e in QliveRPCMethodEnum}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Jord-0.1.1/jord/qlive_utilities/serialisation.py` & `Jord-0.1.2/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/qlive_utilities/uri_utilities.py` & `Jord-0.1.2/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/qt_utilities/enums.py` & `Jord-0.1.2/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/__init__.py` & `Jord-0.1.2/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/clamp.py` & `Jord-0.1.2/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/geometry_types.py` & `Jord-0.1.2/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/iteration.py` & `Jord-0.1.2/jord/shapely_utilities/iteration.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/lines.py` & `Jord-0.1.2/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/mirroring.py` & `Jord-0.1.2/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/morphology.py` & `Jord-0.1.2/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/points.py` & `Jord-0.1.2/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/projection.py` & `Jord-0.1.2/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/sanitise_poly.py` & `Jord-0.1.2/jord/shapely_utilities/sanitise_poly.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/serialisation/well_known_binary.py` & `Jord-0.1.2/jord/shapely_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/serialisation/well_known_text.py` & `Jord-0.1.2/jord/shapely_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/jord/shapely_utilities/transformation.py` & `Jord-0.1.2/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.1/setup.py` & `Jord-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from pathlib import Path
 from typing import List, Sequence, Union
 
 from setuptools import find_packages, setup
 
 
-def python_version_check(major: int = 3, minor: int = 7) -> None:
+def python_version_check(major: int = 3, minor: int = 8) -> None:
     """
       :param major:
     :param minor:
     """
     import sys
 
     assert sys.version_info.major == major and sys.version_info.minor >= minor, (
```

### Comparing `Jord-0.1.1/tests/test_import.py` & `Jord-0.1.2/tests/test_import.py`

 * *Files identical despite different names*

