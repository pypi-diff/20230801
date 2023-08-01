# Comparing `tmp/coastalhazardstoolkit-0.1.0.tar.gz` & `tmp/coastalhazardstoolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coastalhazardstoolkit-0.1.0.tar", last modified: Mon Feb 20 16:53:48 2023, max compression
+gzip compressed data, was "coastalhazardstoolkit-0.2.0.tar", last modified: Tue Aug  1 13:46:12 2023, max compression
```

## Comparing `coastalhazardstoolkit-0.1.0.tar` & `coastalhazardstoolkit-0.2.0.tar`

### file list

```diff
@@ -1,108 +1,133 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.888436 coastalhazardstoolkit-0.1.0/
--rw-rw-rw-   0        0        0    35823 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      367 2023-02-20 16:53:48.888436 coastalhazardstoolkit-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      887 2023-02-20 16:53:32.000000 coastalhazardstoolkit-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-20 16:53:48.888436 coastalhazardstoolkit-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.762188 coastalhazardstoolkit-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.762188 coastalhazardstoolkit-0.1.0/src/cht/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.762188 coastalhazardstoolkit-0.1.0/src/cht/bathymetry/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/bathymetry/__init__.py
--rw-rw-rw-   0        0        0    26263 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/bathymetry/bathymetry_database.py
--rw-rw-rw-   0        0        0    26344 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/bathymetry/tiling.py
--rw-rw-rw-   0        0        0      803 2022-11-13 13:13:28.000000 coastalhazardstoolkit-0.1.0/src/cht/bathymetry/tiling_example.py
--rw-rw-rw-   0        0        0     1324 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/bathymetry/tiling_example_gebco22.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.777200 coastalhazardstoolkit-0.1.0/src/cht/beware/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/beware/__init__.py
--rw-rw-rw-   0        0        0    33085 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/beware/beware.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.780265 coastalhazardstoolkit-0.1.0/src/cht/delft3dfm/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/delft3dfm/__init__.py
--rw-rw-rw-   0        0        0    45459 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/delft3dfm/delft3dfm.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.792872 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/bathymetry.py
--rw-rw-rw-   0        0        0    12328 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/boundary_conditions.py
--rw-rw-rw-   0        0        0     2701 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/grid.py
--rw-rw-rw-   0        0        0    31734 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/hurrywave.py
--rw-rw-rw-   0        0        0     4763 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/hurrywave_builder.py
--rw-rw-rw-   0        0        0     6804 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/hurrywave_domain.py
--rw-rw-rw-   0        0        0     4893 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/input.py
--rw-rw-rw-   0        0        0     5454 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/mask.py
--rw-rw-rw-   0        0        0     5793 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/hurrywave/observation_points.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.808510 coastalhazardstoolkit-0.1.0/src/cht/meteo/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/__init__.py
--rw-rw-rw-   0        0        0    11578 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/coamps_analysis.py
--rw-rw-rw-   0        0        0    26632 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/coamps_tc_forecast.py
--rw-rw-rw-   0        0        0    23025 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/coamps_tc_hindcast.py
--rw-rw-rw-   0        0        0     4688 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/coamps_tc_ufl_d01.py
--rw-rw-rw-   0        0        0    12331 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_anl_0p50.py
--rw-rw-rw-   0        0        0     9220 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_anl_0p50_02.py
--rw-rw-rw-   0        0        0    14130 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_anl_0p50_03.py
--rw-rw-rw-   0        0        0    15644 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_anl_0p50_04.py
--rw-rw-rw-   0        0        0     6399 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_forecast_0p25.py
--rw-rw-rw-   0        0        0     4146 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_forecast_0p25_02.py
--rw-rw-rw-   0        0        0    54411 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/meteo.py
--rw-rw-rw-   0        0        0     1939 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/meteo/test_coamps.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.808510 coastalhazardstoolkit-0.1.0/src/cht/misc/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/__init__.py
--rw-rw-rw-   0        0        0     9328 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/deltares_ini.py
--rw-rw-rw-   0        0        0     2871 2022-10-26 08:55:26.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/fileops.py
--rw-rw-rw-   0        0        0     4434 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/geometry.py
--rw-rw-rw-   0        0        0     2901 2023-02-18 19:02:25.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/misc_tools.py
--rw-rw-rw-   0        0        0      886 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/pli_file.py
--rw-rw-rw-   0        0        0     6472 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/sftp.py
--rw-rw-rw-   0        0        0     9845 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/tekal.py
--rw-rw-rw-   0        0        0     5112 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/misc/xmlkit.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.821732 coastalhazardstoolkit-0.1.0/src/cht/model_builder/
--rw-rw-rw-   0        0        0    22614 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/model_builder/model_builder.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.828369 coastalhazardstoolkit-0.1.0/src/cht/nesting/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/nesting/__init__.py
--rw-rw-rw-   0        0        0     7791 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/nesting/nest1.py
--rw-rw-rw-   0        0        0    31037 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/nesting/nest2.py
--rw-rw-rw-   0        0        0    37211 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/nesting/nesting.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.834080 coastalhazardstoolkit-0.1.0/src/cht/observation_stations/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/observation_stations/__init__.py
--rw-rw-rw-   0        0        0      503 2023-02-20 16:03:50.000000 coastalhazardstoolkit-0.1.0/src/cht/observation_stations/_ndbc.py
--rw-rw-rw-   0        0        0     1127 2023-02-20 16:04:24.000000 coastalhazardstoolkit-0.1.0/src/cht/observation_stations/_noaa_coops.py
--rw-rw-rw-   0        0        0      667 2023-02-20 16:07:26.000000 coastalhazardstoolkit-0.1.0/src/cht/observation_stations/observation_stations.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.840163 coastalhazardstoolkit-0.1.0/src/cht/physics/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/physics/__init__.py
--rw-rw-rw-   0        0        0      590 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/physics/deshoal.py
--rw-rw-rw-   0        0        0     1238 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/physics/disper.py
--rw-rw-rw-   0        0        0     7860 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/physics/vo21.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.840163 coastalhazardstoolkit-0.1.0/src/cht/sfincs/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/sfincs/__init__.py
--rw-rw-rw-   0        0        0    60163 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/sfincs/quadtree.py
--rw-rw-rw-   0        0        0    11167 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/sfincs/regulargrid.py
--rw-rw-rw-   0        0        0    44061 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/sfincs/sfincs.py
--rw-rw-rw-   0        0        0    11701 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/sfincs/sfincs_builder.py
--rw-rw-rw-   0        0        0    48185 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/sfincs/subgrid.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.849549 coastalhazardstoolkit-0.1.0/src/cht/snapwave/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/snapwave/__init__.py
--rw-rw-rw-   0        0        0    24908 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/snapwave/mesh.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.856201 coastalhazardstoolkit-0.1.0/src/cht/tide/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/tide/__init__.py
--rw-rw-rw-   0        0        0     7255 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/tide/astro.py
--rw-rw-rw-   0        0        0     7524 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/tide/constituent.py
--rw-rw-rw-   0        0        0     4860 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/tide/nodal_corrections.py
--rw-rw-rw-   0        0        0    15386 2022-10-26 08:55:26.000000 coastalhazardstoolkit-0.1.0/src/cht/tide/tide.py
--rw-rw-rw-   0        0        0      965 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/tide/tide_predict.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.856201 coastalhazardstoolkit-0.1.0/src/cht/tiling/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/tiling/__init__.py
--rw-rw-rw-   0        0        0    26436 2022-10-26 08:55:26.000000 coastalhazardstoolkit-0.1.0/src/cht/tiling/tiling.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.856201 coastalhazardstoolkit-0.1.0/src/cht/tropical_cyclone/
--rw-rw-rw-   0        0        0     1517 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/tropical_cyclone/testje.py
--rw-rw-rw-   0        0        0     1091 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/tropical_cyclone/testje_forecasting.py
--rw-rw-rw-   0        0        0    92252 2023-02-18 16:24:10.000000 coastalhazardstoolkit-0.1.0/src/cht/tropical_cyclone/tropical_cyclone.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.856201 coastalhazardstoolkit-0.1.0/src/cht/watersheds/
--rw-rw-rw-   0        0        0       92 2022-11-13 13:13:28.000000 coastalhazardstoolkit-0.1.0/src/cht/watersheds/__init__.py
--rw-rw-rw-   0        0        0     7923 2022-11-13 13:13:28.000000 coastalhazardstoolkit-0.1.0/src/cht/watersheds/watersheds.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.856201 coastalhazardstoolkit-0.1.0/src/cht/xbeach/
--rw-rw-rw-   0        0        0       92 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/xbeach/__init__.py
--rw-rw-rw-   0        0        0    28049 2022-10-06 02:48:18.000000 coastalhazardstoolkit-0.1.0/src/cht/xbeach/xbeach.py
-drwxrwxrwx   0        0        0        0 2023-02-20 16:53:48.888436 coastalhazardstoolkit-0.1.0/src/coastalhazardstoolkit.egg-info/
--rw-rw-rw-   0        0        0      367 2023-02-20 16:53:48.000000 coastalhazardstoolkit-0.1.0/src/coastalhazardstoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2023-02-20 16:53:48.000000 coastalhazardstoolkit-0.1.0/src/coastalhazardstoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 16:53:48.000000 coastalhazardstoolkit-0.1.0/src/coastalhazardstoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-02-20 16:53:48.000000 coastalhazardstoolkit-0.1.0/src/coastalhazardstoolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-20 16:53:48.000000 coastalhazardstoolkit-0.1.0/src/coastalhazardstoolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.482195 coastalhazardstoolkit-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      367 2023-08-01 13:46:12.482195 coastalhazardstoolkit-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-08-01 13:45:59.000000 coastalhazardstoolkit-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 13:46:12.483194 coastalhazardstoolkit-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.394109 coastalhazardstoolkit-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.395109 coastalhazardstoolkit-0.2.0/src/cht/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.401115 coastalhazardstoolkit-0.2.0/src/cht/bathymetry/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/bathymetry/__init__.py
+-rw-rw-rw-   0        0        0    26958 2023-06-09 14:37:46.000000 coastalhazardstoolkit-0.2.0/src/cht/bathymetry/bathymetry_database.py
+-rw-rw-rw-   0        0        0    26344 2023-01-03 18:41:58.000000 coastalhazardstoolkit-0.2.0/src/cht/bathymetry/tiling.py
+-rw-rw-rw-   0        0        0      803 2022-11-09 17:01:21.000000 coastalhazardstoolkit-0.2.0/src/cht/bathymetry/tiling_example.py
+-rw-rw-rw-   0        0        0     1324 2023-01-03 19:45:23.000000 coastalhazardstoolkit-0.2.0/src/cht/bathymetry/tiling_example_gebco22.py
+-rw-rw-rw-   0        0        0     1645 2023-06-05 18:25:14.000000 coastalhazardstoolkit-0.2.0/src/cht/bathymetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.403109 coastalhazardstoolkit-0.2.0/src/cht/beware/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/beware/__init__.py
+-rw-rw-rw-   0        0        0    38019 2023-06-06 20:06:44.000000 coastalhazardstoolkit-0.2.0/src/cht/beware/beware.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.405110 coastalhazardstoolkit-0.2.0/src/cht/delft3dfm/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/delft3dfm/__init__.py
+-rw-rw-rw-   0        0        0    45459 2023-02-18 18:54:56.000000 coastalhazardstoolkit-0.2.0/src/cht/delft3dfm/delft3dfm.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.413515 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-02-16 02:20:58.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/bathymetry.py
+-rw-rw-rw-   0        0        0    17214 2023-07-18 19:58:54.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/boundary_conditions.py
+-rw-rw-rw-   0        0        0    18023 2023-06-09 15:38:31.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/grid.py
+-rw-rw-rw-   0        0        0    31446 2023-06-07 17:46:39.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/hurrywave.py
+-rw-rw-rw-   0        0        0     4763 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/hurrywave_builder.py
+-rw-rw-rw-   0        0        0     6804 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/hurrywave_domain.py
+-rw-rw-rw-   0        0        0     5288 2023-05-15 15:51:19.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/input.py
+-rw-rw-rw-   0        0        0     5454 2023-02-16 02:34:58.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/mask.py
+-rw-rw-rw-   0        0        0     7393 2023-05-19 15:46:00.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/observation_points.py
+-rw-rw-rw-   0        0        0     4004 2023-05-22 15:09:37.000000 coastalhazardstoolkit-0.2.0/src/cht/hurrywave/to_xugrid.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.425674 coastalhazardstoolkit-0.2.0/src/cht/meteo/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/__init__.py
+-rw-rw-rw-   0        0        0    11578 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/coamps_analysis.py
+-rw-rw-rw-   0        0        0    26632 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/coamps_tc_forecast.py
+-rw-rw-rw-   0        0        0    23025 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/coamps_tc_hindcast.py
+-rw-rw-rw-   0        0        0     4688 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/coamps_tc_ufl_d01.py
+-rw-rw-rw-   0        0        0    12331 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_anl_0p50.py
+-rw-rw-rw-   0        0        0     9220 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_anl_0p50_02.py
+-rw-rw-rw-   0        0        0    14130 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_anl_0p50_03.py
+-rw-rw-rw-   0        0        0    15644 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_anl_0p50_04.py
+-rw-rw-rw-   0        0        0     6399 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_forecast_0p25.py
+-rw-rw-rw-   0        0        0     4146 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_forecast_0p25_02.py
+-rw-rw-rw-   0        0        0    58037 2023-07-18 19:58:54.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/meteo.py
+-rw-rw-rw-   0        0        0     2074 2023-07-18 19:58:54.000000 coastalhazardstoolkit-0.2.0/src/cht/meteo/test_coamps.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.432685 coastalhazardstoolkit-0.2.0/src/cht/misc/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/__init__.py
+-rw-rw-rw-   0        0        0     9328 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/deltares_ini.py
+-rw-rw-rw-   0        0        0     3138 2023-06-06 20:06:44.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/fileops.py
+-rw-rw-rw-   0        0        0     4434 2023-02-16 02:05:36.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/geometry.py
+-rw-rw-rw-   0        0        0     2901 2023-02-12 05:38:17.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/misc_tools.py
+-rw-rw-rw-   0        0        0     4440 2023-06-07 20:21:34.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/pli_file.py
+-rw-rw-rw-   0        0        0     3831 2023-07-25 20:21:34.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/prob_maps.py
+-rw-rw-rw-   0        0        0     6472 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/sftp.py
+-rw-rw-rw-   0        0        0     9845 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/tekal.py
+-rw-rw-rw-   0        0        0     5317 2023-05-17 17:18:05.000000 coastalhazardstoolkit-0.2.0/src/cht/misc/xmlkit.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.432685 coastalhazardstoolkit-0.2.0/src/cht/model_builder/
+-rw-rw-rw-   0        0        0    22934 2023-03-02 18:25:09.000000 coastalhazardstoolkit-0.2.0/src/cht/model_builder/model_builder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.435195 coastalhazardstoolkit-0.2.0/src/cht/nesting/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/nesting/__init__.py
+-rw-rw-rw-   0        0        0     7791 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/nesting/nest1.py
+-rw-rw-rw-   0        0        0    33815 2023-07-28 19:48:45.000000 coastalhazardstoolkit-0.2.0/src/cht/nesting/nest2.py
+-rw-rw-rw-   0        0        0    37037 2023-07-18 19:58:54.000000 coastalhazardstoolkit-0.2.0/src/cht/nesting/nesting.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.438195 coastalhazardstoolkit-0.2.0/src/cht/observation_stations/
+-rw-rw-rw-   0        0        0       92 2023-03-02 18:25:09.000000 coastalhazardstoolkit-0.2.0/src/cht/observation_stations/__init__.py
+-rw-rw-rw-   0        0        0      993 2023-05-17 17:26:56.000000 coastalhazardstoolkit-0.2.0/src/cht/observation_stations/_ndbc.py
+-rw-rw-rw-   0        0        0     1127 2023-03-02 18:25:09.000000 coastalhazardstoolkit-0.2.0/src/cht/observation_stations/_noaa_coops.py
+-rw-rw-rw-   0        0        0     1181 2023-05-17 17:33:01.000000 coastalhazardstoolkit-0.2.0/src/cht/observation_stations/observation_stations.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.440202 coastalhazardstoolkit-0.2.0/src/cht/physics/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/physics/__init__.py
+-rw-rw-rw-   0        0        0      590 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/physics/deshoal.py
+-rw-rw-rw-   0        0        0     1238 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/physics/disper.py
+-rw-rw-rw-   0        0        0     7860 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/physics/vo21.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.444194 coastalhazardstoolkit-0.2.0/src/cht/sfincs/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs/__init__.py
+-rw-rw-rw-   0        0        0    66271 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs/quadtree.py
+-rw-rw-rw-   0        0        0    11167 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs/regulargrid.py
+-rw-rw-rw-   0        0        0    46392 2023-07-25 20:52:10.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs/sfincs.py
+-rw-rw-rw-   0        0        0    12920 2023-07-18 19:58:54.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs/sfincs_builder.py
+-rw-rw-rw-   0        0        0    48185 2023-01-05 19:25:34.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs/subgrid.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.454194 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/
+-rw-rw-rw-   0        0        0       92 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/__init__.py
+-rw-rw-rw-   0        0        0    12996 2023-06-14 15:50:17.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/boundary_conditions.py
+-rw-rw-rw-   0        0        0    46524 2023-07-18 19:58:54.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/grid.py
+-rw-rw-rw-   0        0        0     8587 2023-06-07 20:03:21.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/input.py
+-rw-rw-rw-   0        0        0    22639 2023-07-18 19:58:54.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/mask.py
+-rw-rw-rw-   0        0        0     3308 2023-05-27 14:29:58.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/observation_points.py
+-rw-rw-rw-   0        0        0    78823 2023-06-01 20:37:42.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/quadtree_grid.py
+-rw-rw-rw-   0        0        0    25105 2023-06-02 21:09:28.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/quadtree_grid_snapwave.py
+-rw-rw-rw-   0        0        0    18022 2023-05-25 16:37:22.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/regular_grid.py
+-rw-rw-rw-   0        0        0    46298 2023-06-14 14:43:07.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/sfincs.py
+-rw-rw-rw-   0        0        0    11719 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/sfincs_builder.py
+-rw-rw-rw-   0        0        0    20663 2023-06-08 11:04:18.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/snapwave.py
+-rw-rw-rw-   0        0        0    46524 2023-06-14 15:18:38.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/subgrid.py
+-rw-rw-rw-   0        0        0     1707 2023-06-07 20:14:52.000000 coastalhazardstoolkit-0.2.0/src/cht/sfincs2/wave_makers.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.456194 coastalhazardstoolkit-0.2.0/src/cht/snapwave/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/snapwave/__init__.py
+-rw-rw-rw-   0        0        0    24908 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/snapwave/mesh.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.463194 coastalhazardstoolkit-0.2.0/src/cht/tide/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/__init__.py
+-rw-rw-rw-   0        0        0     7255 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/astro.py
+-rw-rw-rw-   0        0        0     7524 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/constituent.py
+-rw-rw-rw-   0        0        0     3542 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/fes2014.py
+-rw-rw-rw-   0        0        0     4860 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/nodal_corrections.py
+-rw-rw-rw-   0        0        0     1479 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/predict.py
+-rw-rw-rw-   0        0        0      687 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/test_tide_database.py
+-rw-rw-rw-   0        0        0    15388 2023-03-02 18:25:09.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/tide.py
+-rw-rw-rw-   0        0        0     3365 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/tide_model.py
+-rw-rw-rw-   0        0        0      965 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/tide/tide_predict.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.464205 coastalhazardstoolkit-0.2.0/src/cht/tiling/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/tiling/__init__.py
+-rw-rw-rw-   0        0        0    32567 2023-06-06 20:06:44.000000 coastalhazardstoolkit-0.2.0/src/cht/tiling/tiling.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.468195 coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/
+-rw-rw-rw-   0        0        0    10203 2023-05-17 12:40:56.000000 coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/cyclone_track_database.py
+-rw-rw-rw-   0        0        0     2406 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/test_meteo.py
+-rw-rw-rw-   0        0        0      480 2023-05-04 16:45:00.000000 coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/test_track.py
+-rw-rw-rw-   0        0        0     1517 2023-01-25 14:41:34.000000 coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/testje.py
+-rw-rw-rw-   0        0        0     1091 2023-01-25 14:41:34.000000 coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/testje_forecasting.py
+-rw-rw-rw-   0        0        0   102706 2023-07-29 20:44:35.000000 coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/tropical_cyclone.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.469194 coastalhazardstoolkit-0.2.0/src/cht/watersheds/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/watersheds/__init__.py
+-rw-rw-rw-   0        0        0     7923 2022-11-10 16:13:06.000000 coastalhazardstoolkit-0.2.0/src/cht/watersheds/watersheds.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.471195 coastalhazardstoolkit-0.2.0/src/cht/xbeach/
+-rw-rw-rw-   0        0        0       92 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/xbeach/__init__.py
+-rw-rw-rw-   0        0        0    28049 2022-10-06 18:56:32.000000 coastalhazardstoolkit-0.2.0/src/cht/xbeach/xbeach.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:46:12.481194 coastalhazardstoolkit-0.2.0/src/coastalhazardstoolkit.egg-info/
+-rw-rw-rw-   0        0        0      367 2023-08-01 13:46:12.000000 coastalhazardstoolkit-0.2.0/src/coastalhazardstoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3410 2023-08-01 13:46:12.000000 coastalhazardstoolkit-0.2.0/src/coastalhazardstoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:46:12.000000 coastalhazardstoolkit-0.2.0/src/coastalhazardstoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-08-01 13:46:12.000000 coastalhazardstoolkit-0.2.0/src/coastalhazardstoolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 13:46:12.000000 coastalhazardstoolkit-0.2.0/src/coastalhazardstoolkit.egg-info/top_level.txt
```

### Comparing `coastalhazardstoolkit-0.1.0/LICENSE` & `coastalhazardstoolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/pyproject.toml` & `coastalhazardstoolkit-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.1.0"
+version = "0.2.0"
 name = "coastalhazardstoolkit"
 authors = [
     {name = "Maarten van Ormondt", email = "maarten.vanormondt@deltares-usa.us"},
     {name = "Roel de Goede", email = "roel.degoede@deltares.nl"},
     {name = "Kees Nederhoff", email = "kees.nederhoff@deltares-usa.us"},
     {name = "Tim Leijnse", email = "tim.leijnse@deltares.nl"},
     {name = "Panos Athanasiou", email = "panos.athanasiou@deltares.nl"},
@@ -29,8 +29,10 @@
     "matplotlib",
     "noaa-coops",
     "metpy",
     "siphon",
     "netCDF4",
     "mat73",
     "tabulate",
+    "pyyaml",
+    "toml"
 ]
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/bathymetry/bathymetry_database.py` & `coastalhazardstoolkit-0.2.0/src/cht/bathymetry/bathymetry_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     """
     The main Bathymetry Database class
     
     :param pth: Path name where bathymetry tiles will be cached.
     :type pth: string            
     """
     
-    def __init__(self,pth):
+    def __init__(self, pth):
         if pth:
             self.path    = pth
             self.dataset = []
             self.read()
             self.initialized = True
         else:
-            self.initialized =False
+            self.initialized = False
     
     def initialize(self, pth):
         if not self.initialized:
             self.path    = pth
             self.dataset = []
             self.read()
         self.initialized = True
@@ -60,15 +60,15 @@
         xml_file = os.path.join(self.path, "bathymetry.xml")
         xml_root = ET.parse(xml_file).getroot()
 
         for xml_dataset in xml_root.findall('dataset'):
             
             try:
 
-                dataset = BathymetryDataset()
+                dataset = BathymetryDataset(self)
 
                 # Set attributes
                 for prop in xml_dataset:
                     setattr(dataset, prop.tag.lower(), prop.text)
                     
                 dataset.local_path = os.path.join(self.path, dataset.name)
     
@@ -120,39 +120,44 @@
         
         # Read in data from database
         # Find corresponding dataset dataset
         for d in self.dataset:
             if d.name == dataset_name:
                 return d.crs
 
-    # def get_data_on_array(self, dataset_name, xarr, yarr, crs):
-        
-    #     # Get data interpolated onto array xarr, yarr
-        
-    #     zarr = 0.0
-        
-    #     return zarr
-    
-    def get_bathymetry_on_grid(self, xz, yz, crs, bathymetry_list, method="linear"):
+    def get_bathymetry_on_points(self, xz, yz, dxmin, crs, bathymetry_list, method="linear"):
+        zz = self.get_bathymetry_on_grid(xz, yz, crs, bathymetry_list, method=method, coords="points", dxmin=dxmin)
+        return zz
 
-        if xz.ndim ==2:
+    def get_bathymetry_on_grid(self, xz, yz, crs, bathymetry_list, method="linear", coords="grid", dxmin=1.0e6):
+
+        if xz.ndim == 2:
+            # xy and yz are a grid
             zz = np.full(xz.shape, np.nan)
             dx = np.sqrt((xz[0,1] - xz[0,0])**2 + (yz[0,1] - yz[0,0])**2)
             dy = np.sqrt((xz[1,0] - xz[0,0])**2 + (yz[1,0] - yz[0,0])**2)
         else:
-            zz = np.full((len(yz), len(xz)), np.nan)
-            dx = xz[1] - xz[0]
-            dy = yz[1] - yz[0]
-            xz, yz = np.meshgrid(xz, yz)
-
-        if crs.is_geographic:
-            dx = min(111111.0 * dx,
-                     111111.0 * dy * np.cos(np.pi * np.max(np.abs(yz)) / 180.0))
+            if coords == "grid":
+                zz = np.full((len(yz), len(xz)), np.nan)
+                dx = xz[1] - xz[0]
+                dy = yz[1] - yz[0]
+                xz, yz = np.meshgrid(xz, yz)
+            else:    
+                zz = np.full(xz.shape, np.nan)
+
+        # Determine resolution to get bathy data
+        if coords == "grid":
+            # Resolution follow from grid
+            if crs.is_geographic:
+                dx = min(111111.0 * dx,
+                        111111.0 * dy * np.cos(np.pi * np.max(np.abs(yz)) / 180.0))
+            else:
+                dx = min(dx, dy)
         else:
-            dx = min(dx, dy)
+            dx = dxmin        
 
         # Loop through bathymetry datasets
         for ibathy, bathymetry in enumerate(bathymetry_list):
             dataset = bathymetry["dataset"]
             zmin    = bathymetry["zmin"]
             zmax    = bathymetry["zmax"]
             transformer = Transformer.from_crs(crs,
@@ -231,16 +236,17 @@
     """
     Bathymetry dataset class 
 
     :ivar name: initial value: ''
     :ivar nr_zoom_levels: initial value: 0
     """
 
-    def __init__(self):
+    def __init__(self, database):
         
+        self.database          = database
         self.name              = ''
         self.long_name         = ''
         self.source            = ''
         self.data_format       = '' # netcdftiles, geotiff, etc
         self.nr_zoom_levels    = 0
         self.zoom_level        = []
         self.coordinate_system = []
@@ -353,18 +359,18 @@
             ilev2 = self.nr_zoom_levels
         else:
             ilev1 = izoom
             ilev2 = izoom
         
         for ilev in range(ilev1,ilev2+1):
             
-            x0  = self.zoom_level[ilev].x0   # lower-left corner x
-            y0  = self.zoom_level[ilev].y0   # lower-left corner y
-            dx  = self.zoom_level[ilev].dx   # cell size x
-            dy  = self.zoom_level[ilev].dy   # cell size y
+            x0  = float(self.zoom_level[ilev].x0)   # lower-left corner x
+            y0  = float(self.zoom_level[ilev].y0)   # lower-left corner y
+            dx  = float(self.zoom_level[ilev].dx)   # cell size x
+            dy  = float(self.zoom_level[ilev].dy)   # cell size y
             nx  = self.pixels_in_tile        # number of pixels in tile x
             if self.name == "rws_vaklodingen":
                 ny = 625
             else:
                 ny  = self.pixels_in_tile        # number of pixels in tile y
             nnx = self.zoom_level[ilev].nr_tiles_x  # number of tiles x
             nny = self.zoom_level[ilev].nr_tiles_y  # number of tiles y
@@ -460,27 +466,30 @@
 
             # Indices of tiles to be loaded
             tiles_index_x = all_tiles_index_x[ix1:ix2 + 1]
             tiles_index_y = all_tiles_index_y[iy1:iy2 + 1]
             # Origins of tiles to be loaded
             tiles_x0 = all_tiles_x0[ix1:ix2 + 1]
             tiles_y0 = all_tiles_y0[iy1:iy2 + 1]
+            tiles_x1 = tiles_x0 + tile_size_x
+            npixx = int(np.round((tiles_x1[-1] - tiles_x0[0])/dx))
 
             if not just_get_tiles:
                 # Mesh of horizontal coordinates
                 # x = np.arange(tiles_x0[0],
                 #                tiles_x0[-1] + tile_size_x, dx)
                 # y = np.arange(tiles_y0[0],
                 #                tiles_y0[-1] + tile_size_y, dy)
 
-                x = np.linspace(tiles_x0[0], tiles_x0[-1] + tile_size_x - dx, num=nnnx*nx)
+                x = np.linspace(tiles_x0[0], tiles_x0[0] + (npixx - 1) * dx, num=npixx)
+#                x = np.linspace(tiles_x0[0], tiles_x0[-1] + tile_size_x - dx, num=nnnx*nx)
                 y = np.linspace(tiles_y0[0], tiles_y0[-1] + tile_size_y - dy, num=nnny*ny)
 
                 # Allocate z
-                z = np.empty((nnny*ny,nnnx*nx))
+                z = np.empty((nnny*ny, npixx))
                 z[:] = np.nan
 
             # Start indices for each tile in larger matrix
             istartx = []
             for i in range(nnnx):
                 iii1 = find_first(abs(x - tiles_x0[i]) == min(abs(x - tiles_x0[i])))
                 istartx.append(iii1)
@@ -640,15 +649,15 @@
                 
                 data_in_cell_centres = True
 
                 if data_in_cell_centres:
                     x = x + 0.5*dx # This really should be added as the data are defined in the cell centres!!!               
                     y = y + 0.5*dy
                 
-                z = z[iy1:iy2,ix1:ix2]
+                z = z[iy1:iy2, ix1:ix2]
                 
                 # Convert to metres
                 if self.vertical_units == 'cm':
                     z = z*0.01
                 elif self.vertical_units == 'ft':
                     z = z*0.3048
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/bathymetry/tiling.py` & `coastalhazardstoolkit-0.2.0/src/cht/bathymetry/tiling.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/bathymetry/tiling_example.py` & `coastalhazardstoolkit-0.2.0/src/cht/bathymetry/tiling_example.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/bathymetry/tiling_example_gebco22.py` & `coastalhazardstoolkit-0.2.0/src/cht/bathymetry/tiling_example_gebco22.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/beware/beware.py` & `coastalhazardstoolkit-0.2.0/src/cht/beware/beware.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,36 +35,34 @@
         self.path = os.path.dirname(input_file)
         self.read_input_file(input_file)
         
         self.flow_boundary_point = []
         self.wave_boundary_point = []
         self.testprofs = []
         
-        if os.path.isabs(self.input.profsfile) is False:
-            self.input.profsfile= os.path.join(self.path, self.input.profsfile)
-
-        self.read_profile_characteristics()              
         self.read_wave_boundary_points()
         self.read_flow_boundary_points()
                        
-    def run(self, Hs, Tp, WL, betab, testprofs, xbFile, match_runup=None, match_flooding=None):
+    def run(self, Hs, Tp, WL, betab, testprofs, xbFile):
         self.Hs = Hs
         self.Tp = Tp
         self.WL = WL
         self.betab = betab
             
         # Initialize: load matching for runup / flooding and initialize input / output vars
         BWvars=["Hs", "Tp", "WL", "betab", 'BWprof']
         outvars1 = []
-        if match_runup is not None and self.input.runup==1:
-            matchrunup = io.loadmat(match_runup, simplify_cells=True)
+        matchrunup=None
+        matchflooding=None
+        if self.input.r2matchfile:
+            matchrunup = io.loadmat(os.path.join(self.path, self.input.r2matchfile), simplify_cells=True)
             BWvars.extend(["R2pIndex", "runupComponents"])
             outvars1.extend(["R2", "R2_wl", "R2_setup", 'R2_vlf', "R2_ig", "R2_hf",  r"R2_tot"])
-        if match_flooding is not None and self.input.flooding==1:
-            matchflooding = io.loadmat(match_flooding, simplify_cells=True)
+        if self.input.flmatchfile:
+            matchflooding = io.loadmat(os.path.join(self.path, self.input.flmatchfile), simplify_cells=True)
             BWvars.extend([r"obs_05m.fp", r"obs_05m.infra_m0", r"obs_05m.fsplit",  r"obs_05m.gauss_scale", r"obs_05m.Hm0_HF", r"obs_05m.setup"])
             outvars1.extend([r"fsplit",  r"scale", r"fp", r"Hhf", r"setup", r"m0"])
 
         # Load XB results        
         ds = nc.Dataset(xbFile)
         BWdata={}
         for var in BWvars:
@@ -72,25 +70,23 @@
 
         # Initialize BEWARE profile output
         outvars2= [r"Prof", r"Xc",  r"Yc", r"Xo", r"Yo"]
         self.out={}
         for var in outvars1:
             a = np.empty((len(testprofs), len(Hs)))
             a[:] = np.nan
-#            self.out[str(var)]= np.nan((len(testprofs), (len(Hs))))
             self.out[str(var)]= a
         for var in outvars2:
             a = np.empty((len(testprofs)))
             a[:] = np.nan
             self.out[str(var)]= a
-#            self.out[str(var)]= np.nan((len(testprofs)))
 
         error=[]
         # Initialize profile id naming
-        if match_runup is not None:
+        if matchrunup:
             profid= np.zeros(len(matchrunup['ProbNS3']['profid']))
             for i in range(len(matchrunup['ProbNS3']['profid'])):
                 profid[i]= matchrunup['ProbNS3']['profid'][i]
         else:
             profid= np.zeros(len(matchflooding['ProbNS3']['profid']))
             for i in range(len(matchflooding['ProbNS3']['profid'])):
                 profid[i]= matchflooding['ProbNS3']['profid'][i]
@@ -103,15 +99,15 @@
             # Load forcing file into dictionary
             if np.shape(self.Hs)[0] == 1:
                 forcing=np.array(np.concatenate((self.Hs[:, inputprof], self.Tp[:, inputprof], self.WL[:, inputprof],self.betab[inputprof]*np.ones(np.shape(self.Hs)[0]))), ndmin=2)
             else:
                 forcing=np.transpose((self.Hs[:, inputprof], self.Tp[:, inputprof], self.WL[:, inputprof],self.betab[inputprof]*np.ones(np.shape(self.Hs)[0])))
 
             # Runup
-            if match_runup is not None and self.input.runup==1:
+            if matchrunup:
                 prob=matchrunup['ProbNS3']['ProbtoCR2'][ID]            # Get matching % of input profile to BW profiles
                 idx= [i for i,v in enumerate(prob) if v > 0.01]             # Delete profiles with less than 1% matching
                 
                 bwProfiles= matchrunup['ProbNS3']['CR2repProf'][idx]             # Get id of matched bwprofiles
                 prob=prob[idx] / sum(prob[idx])                             # correct probability of matching for deleted profiles
             
                 # try:
@@ -125,15 +121,15 @@
                     # intpData=np.zeros((16, 4))
         
                     for iforcings in range(np.shape(forcing)[0]): # Loop through forcing conditions
                             
     
                         for iprof in range(len(bwProfiles)): # Loop through matched BEWARE profiles range(len(prob))
                             if np.isnan(forcing).any():
-                                cont=1   
+                                pass
                             else:
     
                                 profval= np.where(bwProfiles[iprof]==BWdata['BWprof'])[0][0]
                                 BWforcing=np.transpose((BWdata['Hs'][:,profval], BWdata['Tp'][:,profval],
                                                                             BWdata['WL'][:,profval], BWdata['betab'][:,profval])) 
                         
                                 # Find nearest conditions (same for all profiles so only run once per forcing condition)  
@@ -197,99 +193,97 @@
            
                 # except:
                 #     error.append(inputprof)
                 #     print('error')
                     
                 
             # Flooding
-            if match_flooding is not None and self.input.flooding==1:
+            if matchflooding:
                 prob=matchflooding['ProbNS3']['ProbtoCR2'][ID]            # Get matching % of input profile to BW profiles
                 idx= [i for i,v in enumerate(prob) if v > 0.01]             # Delete profiles with less than 1% matching
                 
                 bwProfiles= matchflooding['ProbNS3']['CR2repProf'][idx]             # Get id of matched bwprofiles
                 prob=prob[idx] / sum(prob[idx])                             # correct probability of matching for deleted profiles
                   
-                try:
-                    if len(prob)>=1:
+                if len(prob)>=1:
+    
+                    savevars= [r"fsplit",  r"scale", r"fp", r"Hhf", r"setup",  r"m0"]
+                    save={}
+                    for var in savevars:
+                        save[str(var)]= np.zeros((len(self.Hs),len(prob)))
+                    
+                    #intpData=np.zeros((16, 4))
         
-                        savevars= [r"fsplit",  r"scale", r"fp", r"Hhf", r"setup",  r"m0"]
-                        save={}
-                        for var in savevars:
-                            save[str(var)]= np.zeros((len(self.Hs),len(prob)))
+                    for iforcings in range(np.shape(forcing)[0]): # Loop through forcing conditions
+                            
+    
+                        for iprof in range(len(bwProfiles)): # Loop through matched BEWARE profiles range(len(prob))
+                            if np.isnan(forcing).any():
+                                pass
+                            else:
+    
+                                profval= np.where(bwProfiles[iprof]==BWdata['BWprof'])[0][0]
+                                BWforcing=np.squeeze(np.array(np.transpose([BWdata['Hs'][:,profval], BWdata['Tp'][:,profval],
+                                                                            BWdata['WL'][:,profval], BWdata['betab'][:,profval]]))) # faster?
                         
-                        intpData=np.zeros((16, 4))
-            
-                        for iforcings in range(np.shape(forcing)[0]): # Loop through forcing conditions
+                                # Find nearest conditions
+                                df = forcing[iforcings,:]-BWforcing
+                                lims=[]
+                                for ilim in range(4):
+                                    lims.append(BWforcing[df[:,ilim]>=0, ilim].max())
+                                    lims.append(BWforcing[df[:,ilim]<0, ilim].min())
+                                BWinds=np.where(np.all(((BWforcing[:,0]==lims[0]) | (BWforcing[:,0]==lims[1]), (BWforcing[:,1]==lims[2]) | (BWforcing[:,1]==lims[3]), 
+                                    (BWforcing[:,2]==lims[4]) | (BWforcing[:,2]==lims[5]),(BWforcing[:,3]==lims[6]) | (BWforcing[:,3]==lims[7])), axis=0))
+
+                                # lims=[] # nearest upper and lower values
+                                # for ilim in range(4):
+                                #     uniquelist= list(set(BWforcing[:,ilim]))
+                                #     lims.append(next(uniquelist[i-1] for i,v in enumerate(uniquelist) if v>forcing[iforcings, ilim]))
+                                #     lims.append(next(uniquelist[i]  for i,v in enumerate(uniquelist) if v>forcing[iforcings, ilim]))
+                                # lims=np.array(lims)                                
+                                                            
+                                # BWinds=[]
+                                # for itmp in range(2):
+                                #     for itmp2 in range(2):
+                                #         for itmp3 in range(2):
+                                #             for itmp4 in range(2):
+                                #                 BWinds.append(np.argwhere(np.all((BWforcing[:,0]==lims[0+itmp], BWforcing[:,1]==lims[2+itmp2], BWforcing[:,2]==lims[4+itmp3], BWforcing[:,3]==lims[6+itmp4]), axis=0)))
+                                                        
+                                # BWinds= np.squeeze(BWinds)
+                                limsdim=[lims[1]-lims[0], lims[3]-lims[2], lims[5]-lims[4], lims[7]-lims[6]] # distance between BW conditions        
+                                intpData= np.zeros((np.shape(BWinds)[1], 4))
+                                intpData[0:np.shape(BWinds)[1], 0:4]= BWforcing[BWinds,:]
+                            
+                                # Calculate normalized geometric mean inverse distance
+                                NGM= (1-abs((forcing[iforcings,:] - intpData) / (limsdim)))
+                                NGMiD=np.prod(NGM, axis=1)**(1/len(intpData[0]))
+                                P= NGMiD/ sum(NGMiD)
                                 
-        
-                            for iprof in range(len(bwProfiles)): # Loop through matched BEWARE profiles range(len(prob))
-                                if np.isnan(forcing).any():
-                                   cont=1   
-                                else:
-        
-                                    profval= np.where(bwProfiles[iprof]==BWdata['BWprof'])[0][0]
-                                    BWforcing=np.squeeze(np.array(np.transpose([BWdata['Hs'][:,profval], BWdata['Tp'][:,profval],
-                                                                                BWdata['WL'][:,profval], BWdata['betab'][:,profval]]))) # faster?
-                           
-                                    # Find nearest conditions
-                                    df = forcing[iforcings,:]-BWforcing
-                                    lims=[]
-                                    for ilim in range(4):
-                                        lims.append(BWforcing[df[:,ilim]>=0, ilim].max())
-                                        lims.append(BWforcing[df[:,ilim]<0, ilim].min())
-                                    BWinds=np.where(np.all(((BWforcing[:,0]==lims[0]) | (BWforcing[:,0]==lims[1]), (BWforcing[:,1]==lims[2]) | (BWforcing[:,1]==lims[3]), 
-                                        (BWforcing[:,2]==lims[4]) | (BWforcing[:,2]==lims[5]),(BWforcing[:,3]==lims[6]) | (BWforcing[:,3]==lims[7])), axis=0))
-
-                                    # lims=[] # nearest upper and lower values
-                                    # for ilim in range(4):
-                                    #     uniquelist= list(set(BWforcing[:,ilim]))
-                                    #     lims.append(next(uniquelist[i-1] for i,v in enumerate(uniquelist) if v>forcing[iforcings, ilim]))
-                                    #     lims.append(next(uniquelist[i]  for i,v in enumerate(uniquelist) if v>forcing[iforcings, ilim]))
-                                    # lims=np.array(lims)                                
+                                # R2= np.squeeze(BWdata['R2pIndex'][BWinds, profval])
+                                # R2comp= np.squeeze(BWdata['runupComponents'][BWinds, :, profval])
                                                                 
-                                    # BWinds=[]
-                                    # for itmp in range(2):
-                                    #     for itmp2 in range(2):
-                                    #         for itmp3 in range(2):
-                                    #             for itmp4 in range(2):
-                                    #                 BWinds.append(np.argwhere(np.all((BWforcing[:,0]==lims[0+itmp], BWforcing[:,1]==lims[2+itmp2], BWforcing[:,2]==lims[4+itmp3], BWforcing[:,3]==lims[6+itmp4]), axis=0)))
-                                                            
-                                    # BWinds= np.squeeze(BWinds)
-                                    limsdim=[lims[1]-lims[0], lims[3]-lims[2], lims[5]-lims[4], lims[7]-lims[6]] # distance between BW conditions        
-                                    intpData[0:16,0:4]= BWforcing[BWinds,:]
+                                save['fsplit'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.fsplit'][BWinds, profval])*P*prob[iprof]) 
+                                save['scale'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.gauss_scale'][BWinds, profval])*P*prob[iprof]) 
+                                save['m0'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.infra_m0'][BWinds, profval])*P*prob[iprof])          
+                                save['fp'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.fp'][BWinds, profval])*P*prob[iprof]) 
+                                save['Hhf'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.Hm0_HF'][BWinds, profval])*P*prob[iprof])                        
+                                save['setup'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.setup'][BWinds, profval])*P*prob[iprof])        
                                 
-                                    # Calculate normalized geometric mean inverse distance
-                                    NGM= (1-abs((forcing[iforcings,:] - intpData) / (limsdim)))
-                                    NGMiD=np.prod(NGM, axis=1)**(1/len(intpData[0]))
-                                    P= NGMiD/ sum(NGMiD)
-                                    
-                                    # R2= np.squeeze(BWdata['R2pIndex'][BWinds, profval])
-                                    # R2comp= np.squeeze(BWdata['runupComponents'][BWinds, :, profval])
-                                                                    
-                                    save['fsplit'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.fsplit'][BWinds, profval])*P*prob[iprof]) 
-                                    save['scale'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.gauss_scale'][BWinds, profval])*P*prob[iprof]) 
-                                    save['m0'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.infra_m0'][BWinds, profval])*P*prob[iprof])          
-                                    save['fp'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.fp'][BWinds, profval])*P*prob[iprof]) 
-                                    save['Hhf'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.Hm0_HF'][BWinds, profval])*P*prob[iprof])                        
-                                    save['setup'][iforcings, iprof]= np.sum(np.squeeze(BWdata[r'obs_05m.setup'][BWinds, profval])*P*prob[iprof])        
-                                    
-                        # self.out['BWForcing'][inputprof,:,:] = np.squeeze(forcing[:,0:3])
-                        # self.out['Prof'][inputprof]        =  int(match['ProbNS3']['profid'][ID][12:])    
-                        # self.out['Xc'][inputprof]        = self.input.profs['x_coast'][PRoutid]
-                        # self.out['Yc'][inputprof]        = profs['y_coast'][PRoutid]
-                        # self.out['Xo'][inputprof]        = profs['x_off'][PRoutid]
-                        # self.out['Yo'][inputprof]        = profs['y_off'][PRoutid]
-        
-                        self.out['fp'][inputprof,:]  = 0.5*np.sum(save['fsplit'],1)
-                        self.out['m0'][inputprof,:]      = np.sum(save['m0'],1)
-                        self.out['scale'][inputprof,:]   = np.sum(save['scale'],1)
-                        self.out['setup'][inputprof,:]   = np.sum(save['setup'],1)
+                    # self.out['BWForcing'][inputprof,:,:] = np.squeeze(forcing[:,0:3])
+                    # self.out['Prof'][inputprof]        =  int(match['ProbNS3']['profid'][ID][12:])    
+                    # self.out['Xc'][inputprof]        = self.input.profs['x_coast'][PRoutid]
+                    # self.out['Yc'][inputprof]        = profs['y_coast'][PRoutid]
+                    # self.out['Xo'][inputprof]        = profs['x_off'][PRoutid]
+                    # self.out['Yo'][inputprof]        = profs['y_off'][PRoutid]
     
-                except:
-                    error.append(inputprof)  
+                    self.out['fp'][inputprof,:]  = 0.5*np.sum(save['fsplit'],1)
+                    self.out['m0'][inputprof,:]      = np.sum(save['m0'],1)
+                    self.out['scale'][inputprof,:]   = np.sum(save['scale'],1)
+                    self.out['setup'][inputprof,:]   = np.sum(save['setup'],1)
+
         # self.output=self.out
                         
     def write_flow_boundary_points(self, file_name=None):
     
         # Write BEWARE profs file
         if not file_name:
             if not self.input.bndfile:
@@ -321,44 +315,31 @@
         fid = open(file_name, "w")
         for point in self.wave_boundary_point:
             if point.data is not None:
                 string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}'
                 fid.write(string + r' ' + str(point.name) + '\n')
         fid.close()  
 
-    def read_profile_characteristics(self):
-
-        df = pd.read_csv(self.input.profsfile, index_col=False,
-            delim_whitespace=True)
-
-        self.input.betab= df.beachslope.values
-        self.input.xc= df.x_coast.values
-        self.input.yc= df.y_coast.values
-        self.input.xo= df.x_off.values
-        self.input.yo= df.y_off.values
-        self.input.coasttype= df.coasttype.values
-        self.input.profid= df.profid.values
-
     def read_flow_boundary_points(self):
         
         # Read BEWARE profs file
         from cht.sfincs.sfincs import FlowBoundaryPoint
         
         prof_file = os.path.join(self.path, self.input.profsfile)
         # Read the bnd file
         # df = pd.read_csv(prof_file, index_col=False, header=None,
         #      delim_whitespace=True, names=['x', 'y', 'profs', 'type'])
         df = pd.read_csv(prof_file, index_col=False,
              delim_whitespace=True)
         
         # Loop through points
-        for ind in range(len(df.x_off.values)):
+        for ind in range(len(df.x_flow.values)):
             name = df.profid.values[ind]
-            point = FlowBoundaryPoint(df.x_off.values[ind],
-                                      df.y_off.values[ind],
+            point = FlowBoundaryPoint(df.x_flow.values[ind],
+                                      df.y_flow.values[ind],
                                        name=r'transect_' + str(int(name)))
                                       # name= str(int(name))) 
             self.flow_boundary_point.append(point)
             self.testprofs.append(name)
             
     def read_wave_boundary_points(self):
         
@@ -377,24 +358,116 @@
             name = df.profid.values[ind]
             point = FlowBoundaryPoint(df.x_off.values[ind],
                                       df.y_off.values[ind],
                                        name=r'transect_' + str(int(name)))
                                       # name= str(int(name))) 
             self.wave_boundary_point.append(point)             
         
-    def write_wave_boundary_conditions(self, file_name=None):
+    def read_wave_boundary_conditions(self):
 
-        file_name = os.path.join(self.path,
-                                 self.input.bwvfile)
-                 
-        # Build a new DataFrame
+        # Hm0, Tp
+        self.read_bhs_file()
+        self.read_btp_file()
+
+    def read_bhs_file(self, file_name=None, interpolate = True):
+        
+        # Read BEWARE bhs file
+        if not file_name:
+            if not self.input.bhsfile:
+                return
+            file_name = os.path.join(self.path,
+                                     self.input.bhsfile)
+            
+        if not file_name:
+            return        
+
+        hs= pd.read_csv(file_name, index_col=0, header=None,
+                  delim_whitespace=True)
+        
+        # Interpolate to required time intervals
+        if interpolate:
+            tstart = (self.input.tstart - self.input.tref)
+            tstop  = (self.input.tstop - self.input.tref)
+
+            hs.index=pd.to_timedelta(hs.index, unit="s")
+            hs = hs.resample(self.input.dT).interpolate(method='time')
+            indexes = hs[(hs.index<tstart) | (hs.index>=tstop)].index
+            hs.drop(indexes, inplace=True)
+
+        self.hs= hs
+
+    def read_btp_file(self, file_name=None, interpolate = True):
+
+        # Read BEWARE btp file
+        if not file_name:
+            if not self.input.btpfile:
+                return
+            file_name = os.path.join(self.path,
+                                     self.input.btpfile)
+            
+        if not file_name:
+            return        
 
-        file_name = os.path.join(self.path,
-                                 'beware.bhs')
-        self.bhsfile = file_name
+        tp= pd.read_csv(file_name, index_col=0, header=None,
+                  delim_whitespace=True)
+        
+        # Interpolate to required time intervals
+        if interpolate:
+            tstart = (self.input.tstart - self.input.tref)
+            tstop  = (self.input.tstop - self.input.tref)
+
+            tp.index=pd.to_timedelta(tp.index, unit="s")
+            tp = tp.resample(self.input.dT).interpolate(method='time')
+            indexes = tp[(tp.index<tstart) | (tp.index>=tstop)].index
+            tp.drop(indexes, inplace=True)
+
+        self.tp= tp
+
+    def read_flow_boundary_conditions(self, file_name=None, interpolate = True):
+        # Read BEWARE bhs file
+        if not file_name:
+            if not self.input.bzsfile:
+                return
+            file_name = os.path.join(self.path,
+                                     self.input.bzsfile)
+            
+        if not file_name:
+            return        
+
+        wl= pd.read_csv(file_name, index_col=0, header=None,
+            delim_whitespace=True)
+
+        if interpolate:
+            tstart = (self.input.tstart - self.input.tref)
+            tstop  = (self.input.tstop - self.input.tref)
+
+            wl.index=pd.to_timedelta(wl.index, unit="s")
+            wl = wl.resample(self.input.dT).interpolate(method='time')
+            indexes = wl[(wl.index<tstart) | (wl.index>=tstop)].index
+            wl.drop(indexes, inplace=True)
+
+        self.wl=wl
+
+    def write_wave_boundary_conditions(self):
+
+        # Hm0, Tp, etc given (probably forced with SnapWave)
+        self.write_bhs_file()
+        self.write_btp_file()
+
+    def write_bhs_file(self, file_name=None):
+        
+        # Write BEWARE bhs file
+        if not file_name:
+            if not self.input.bhsfile:
+                return
+            file_name = os.path.join(self.path,
+                                     self.input.bhsfile)
+            
+        if not file_name:
+            return        
         
         point_data = []
         for point in self.wave_boundary_point:
             if point.data is not None:
                 # df = pd.concat([df, point.data['hm0']], axis=1)
                 point_data.append(point.data['hm0'])
         df = pd.concat(point_data, axis=1)
@@ -404,36 +477,51 @@
         # df=df.replace(np.NaN, 0.1)
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.3f")
         
-        file_name = os.path.join(self.path,
-                                 'beware.btp')
-        self.btpfile = file_name
+    def write_btp_file(self, file_name=None):
+
+        # Write BEWARE btp file
+        if not file_name:
+            if not self.input.btpfile:
+                return
+            file_name = os.path.join(self.path,
+                                     self.input.btpfile)
+            
+        if not file_name:
+            return
 
         point_data = []
         for point in self.wave_boundary_point:
             if point.data is not None:
                 point_data.append(point.data['tp'])
         df = pd.concat(point_data, axis=1)
+
+        tmsec = pd.to_timedelta(df.index - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
-        df=df.replace(np.NaN, 5.0)        
+        #df=df.replace(np.NaN, 5.0)        
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.3f")
         
     def write_flow_boundary_conditions(self, file_name=None):
 
-        file_name = os.path.join(self.path,
-                                 self.input.bzsfile)
-        self.input.bzsfile = file_name
+        if not file_name:
+            if not self.input.bzsfile:
+                return
+            file_name = os.path.join(self.path,
+                                     self.input.bzsfile)
+            
+        if not file_name:
+            return
 
         # Build a new DataFrame
         point_data = []
         for point in self.flow_boundary_point:
             point_data.append(point.data)
             # df = pd.concat([df, point.data], axis=1)
             
@@ -444,14 +532,40 @@
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.3f")
         print('Finish write flow data')
+    
+    def write_input_file(self, input_file=None):
+
+        if not input_file:
+            input_file = os.path.join(self.path, "beware.inp")
+            
+        fid = open(input_file, "w")
+        for key, value in self.input.__dict__.items():
+            if not value is None:
+                if type(value) == "float":
+                    string = f'{key.ljust(20)} = {float(value)}\n'
+                elif type(value) == "int":
+                    string = f'{key.ljust(20)} = {int(value)}\n'
+                elif type(value) == list:
+                    valstr = ""
+                    for v in value:
+                        valstr += str(v) + " "
+                    string = f'{key.ljust(20)} = {valstr}\n'
+                elif isinstance(value, datetime.date):
+                    dstr = value.strftime("%Y%m%d %H%M%S")
+                    string = f'{key.ljust(20)} = {dstr}\n'
+                else:
+                    string = f'{key.ljust(20)} = {value}\n'                
+                fid.write(string)
+        fid.close()    
+
         
     def read_input_file(self, inputfile):
         
         # Reads beware.inp
         
         
         fid = open(inputfile, 'r')
@@ -486,34 +600,39 @@
             if name == "tstop":
                 try:
                     val = datetime.datetime.strptime(val.rstrip(), '%Y%m%d %H%M%S')
                 except:
                     val = None
             setattr(self.input, name, val)
 
-    def read_data(self, input_file=None):
+    def read_data(self, input_file=None, prcs=None):
         if not input_file:
             output_path = os.path.join(self.cycle_path, "output\\")
-            input_file= os.path.join(output_path, 'BEWARE_output.nc')
+            input_file= os.path.join(output_path, 'beware_his.nc')
 
         ds = nc.Dataset(input_file)
         self.R2p=np.nan_to_num(ds[r"R2_tot"][:].data, copy=False, nan=0.0)
         self.setup=np.nan_to_num(ds[r"R2_set"][:].data, copy=False, nan=0.0)
         self.Hs=np.nan_to_num(ds[r"Hs"][:].data, copy=False, nan=0.0)
         self.Tp=np.nan_to_num(ds[r"Tp"][:].data, copy=False, nan=0.0)
-        self.WL=np.nan_to_num(ds[r"R2_wl"][:].data, copy=False, nan=0.0)
+        self.WL=np.nan_to_num(ds[r"WL"][:].data, copy=False, nan=0.0)
         self.filename=ds[r"Profiles"][:].data
         self.swash=self.R2p-self.setup-self.WL
 
         self.xp=ds[r"x_coast"][:].data
         self.yp=ds[r"y_coast"][:].data
         
         self.xo=ds[r"x_off"][:].data
         self.yo=ds[r"y_off"][:].data
-        
+        self.R2p_prc, self.setup_prc={},{}
+        if prcs is not None:
+            for i,v in enumerate(prcs):
+                self.R2p_prc[str(round(v*100))]= np.nan_to_num(ds[r"R2_tot_"+str(round(v*100))][:].data, copy=False, nan=0.0)
+                self.setup_prc[str(round(v*100))]= np.nan_to_num(ds[r"R2_set_"+str(round(v*100))][:].data, copy=False, nan=0.0)
+
         if not self.input.tstart:
             ttt = ds["time"][:]
             dt  = datetime.timedelta(seconds=ttt[0])
             tout = datetime.datetime(1970,1,1) + dt
             self.input.tstart = tout
         
 #     def write_to_geojson(self, output_path, scenario):
@@ -628,24 +747,60 @@
 #             runup_file = os.path.join(output_path,
 #                                     "twls.geojson.js")
 #             cht.misc.misc_tools.write_json_js(runup_file, feature_collection, "var TWL =")
             
 
 class BewareInput():
     def __init__(self):
-        self.xc = []
-        self.yc = []
-        self.xo = []
-        self.yo = []
-        self.betab = []
-        self.coasttype = []
-        self.profid = []
-        
-        self.tref = []
-        self.tstart = []
-        self.tstop = []
-        self.folder = []
-        self.dT = []
-        self.runup = []
-        self.flooding = []
+        
+        self.tref = None
+        self.tstart = None
+        self.tstop = None
+       # self.folder = []
+        self.dT = None
+        self.r2matchfile = None
+        self.flmatchfile = None
+        self.profsfile = "beware.profs"
+        self.bndfile = "beware.bnd"
+        self.bzsfile= "beware.bzs"
+        self.bwvfile= "beware.bwv"
+        self.bhsfile= "beware.bhs"
+        self.btpfile= "beware.btp"
+
+class BewareProfiles():
+    def __init__(self):
+        self.betab=None
+        self.xc= None
+        self.yc= None
+        self.xo= None
+        self.yo= None
+        self.coasttype= None
+        self.profid= None
         self.profsfile = "beware.profs"
-        
+
+    def read_profile_characteristics(self, file_name= None):
+
+        # Read profs file
+        if not file_name:
+            if not self.profsfile:
+                return
+            if not self.path:
+                return
+            file_name = os.path.join(self.path,
+                                     self.profsfile)
+
+        if not file_name:
+            return
+
+        df = pd.read_csv(file_name, index_col=False,
+            delim_whitespace=True)
+
+        self.betab= df.beachslope.values
+        self.xc= df.x_coast.values
+        self.yc= df.y_coast.values
+        self.xo= df.x_off.values
+        self.yo= df.y_off.values
+        self.xf= df.x_flow.values
+        self.yf= df.y_flow.values
+        self.coasttype= df.coasttype.values
+        self.profid= df.profid.values
+
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/delft3dfm/delft3dfm.py` & `coastalhazardstoolkit-0.2.0/src/cht/delft3dfm/delft3dfm.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/hurrywave/bathymetry.py` & `coastalhazardstoolkit-0.2.0/src/cht/hurrywave/bathymetry.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/hurrywave/boundary_conditions.py` & `coastalhazardstoolkit-0.2.0/src/cht/hurrywave/boundary_conditions.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import os
 import numpy as np
 import geopandas as gpd
 import shapely
 import pandas as pd
 from tabulate import tabulate
+from pyproj import Transformer
 
 class HurryWaveBoundaryConditions:
     def __init__(self, hw):
         self.model = hw
         self.forcing = "timeseries"
         self.gdf = gpd.GeoDataFrame()
         self.times = []
@@ -47,15 +48,15 @@
         gdf_list = []
         # Loop through points
         for ind in range(len(df.x.values)):
             name = str(ind + 1).zfill(4)
             x = df.x.values[ind]
             y = df.y.values[ind]
             point = shapely.geometry.Point(x, y)
-            d = {"name": name, "timeseries": pd.DataFrame(), "geometry": point}
+            d = {"name": name, "timeseries": pd.DataFrame(), "spectra": None, "geometry": point}
             gdf_list.append(d)
         self.gdf = gpd.GeoDataFrame(gdf_list, crs=self.model.crs)
 
 
     def write_boundary_points(self):
         # Write bnd file
 
@@ -80,25 +81,46 @@
             for index, row in self.gdf.iterrows():
                 x = row["geometry"].coords[0][0]
                 y = row["geometry"].coords[0][1]
                 string = f'{x:12.1f}{y:12.1f}\n'
                 fid.write(string)
             fid.close()
 
+    def set_timeseries_uniform(self, hs, tp, wd, ds):
+        # Applies uniform time series boundary conditions for each point
+        time = [self.model.input.variables.tstart, self.model.input.variables.tstop]
+        nt = len(time)
+        hs = [hs] * nt
+        tp = [tp] * nt
+        wd = [wd] * nt
+        ds = [ds] * nt
+        for index, point in self.gdf.iterrows():
+            df = pd.DataFrame()     
+            df["time"] = time
+            df["hs"] = hs
+            df["tp"] = tp
+            df["wd"] = wd
+            df["ds"] = ds
+            df = df.set_index("time")
+            self.gdf.at[index, "timeseries"] = df
+
+    def set_conditions_at_point(self, index, par, val):
+        df = self.gdf["timeseries"].loc[index]
+        df[par] = val
+
     def add_point(self, x, y, hs=None, tp=None, wd=None, ds=None, sp=None):
         # Add point
 
         nrp = len(self.gdf.index)
         name = str(nrp + 1).zfill(4)
         point = shapely.geometry.Point(x, y)
         df = pd.DataFrame()     
 
         if hs:
-            # Forcing by time series
-        
+            # Forcing by time series        
             if not self.model.input.variables.bndfile:
                 self.model.input.variables.bndfile = "hurrywave.bnd"
             if not self.model.input.variables.bhsfile:
                 self.model.input.variables.bhsfile = "hurrywave.bhs"
             if not self.model.input.variables.btpfile:
                 self.model.input.variables.btpfile = "hurrywave.btp"
             if not self.model.input.variables.bwdfile:
@@ -112,14 +134,15 @@
                 
             if new:
                 # Start and stop time
                 time = [self.model.input.variables.tstart, self.model.input.variables.tstop]
             else:
                 # Get times from first point
                 time = self.gdf.loc[0]["timeseries"].index    
+
             nt = len(time)
 
             hs = [hs] * nt
             tp = [tp] * nt
             wd = [wd] * nt
             ds = [ds] * nt
 
@@ -139,14 +162,17 @@
 
     def delete_point(self, index):
         # Delete boundary point by index
         if len(self.gdf.index)==0:
             return
         if index<len(self.gdf.index):
             self.gdf = self.gdf.drop(index).reset_index(drop=True)
+        # Rename points    
+        for index, point in self.gdf.iterrows():
+            self.gdf.at[index, "name"] = str(index + 1).zfill(4)
         
 
     def clear(self):
         self.gdf  = gpd.GeoDataFrame()
 
 
     def read_boundary_time_series(self):
@@ -192,15 +218,14 @@
     def read_boundary_spectra(self):
         # Read HurryWave bhs, btp, bwd and bds files
         if not self.model.input.variables.bspfile:
             return
         if len(self.gdf.index)==0:
             return
 
-        tref = self.model.input.variables.tref
         file_name = os.path.join(self.model.path, self.model.input.variables.bspfile)
         print("Reading " + file_name)
 
 
     def write_boundary_conditions_timeseries(self):
         if len(self.gdf.index)==0:
             return
@@ -270,38 +295,41 @@
         #           index=True,
         #           sep=" ",
         #           header=False,
         #           float_format="%.3f")
         to_fwf(df, file_name)
 
         
-    def write_boundary_conditions_spectra(self):
+    def write_boundary_conditions_spectra(self, file_name=None):
         # Write HurryWave bsp file
 
         import xarray as xr
 
-        file_name = os.path.join(self.model.path, self.model.input.variables.bspfile)
+        if file_name is None:
+            file_name = os.path.join(self.model.path, self.model.input.variables.bspfile)
+        
+        sp20 = self.gdf["spectra"][0]
 
-        times = self.boundary_point[0].data.point_spectrum2d.coords["time"].values
+        times = sp20.coords["time"].values
         #        tref  = np.datetime64(self.input.tref)
         #        times = np.single((times-tref)/1000000000)
 
-        sigma = self.boundary_point[0].data.point_spectrum2d.coords["sigma"].values
-        theta = self.boundary_point[0].data.point_spectrum2d.coords["theta"].values
+        sigma = sp20.coords["sigma"].values
+        theta = sp20.coords["theta"].values
 
-        sp2 = np.zeros([len(times), len(self.boundary_point), len(theta), len(sigma)])
+        sp2 = np.zeros([len(times), len(self.gdf), len(theta), len(sigma)])
 
         points = []
-        xs = np.zeros([len(self.boundary_point)])
-        ys = np.zeros([len(self.boundary_point)])
-        for ip, point in enumerate(self.boundary_point):
-            points.append(point.name)
+        xs = np.zeros([len(self.gdf)])
+        ys = np.zeros([len(self.gdf)])
+        for ip, point in self.gdf.iterrows():            
+            points.append(point["name"])
             xs[ip] = point.geometry.x
             ys[ip] = point.geometry.y
-            sp2[:, ip, :, :] = point.data.point_spectrum2d.values
+            sp2[:, ip, :, :] = point["spectra"].values
 
         # Convert to single
         xs = np.single(xs)
         ys = np.single(ys)
         sp2 = np.single(sp2)
 
         ds = xr.Dataset(
@@ -311,21 +339,126 @@
                            ),
             coords=dict(time=times,
                         stations=points,
                         theta=theta,
                         sigma=sigma)
         )
 
-        dstr = "seconds since " + self.input.tref.strftime("%Y%m%d %H%M%S")
+        dstr = "seconds since " + self.model.input.variables.tref.strftime("%Y%m%d %H%M%S")
 
         ds.to_netcdf(path=file_name,
                      mode='w',
                      encoding={'time': {'units': dstr}})
-#        ds.to_netcdf(path=file_name,
-#                     mode='w')
+
+
+    def get_boundary_points_from_mask(self, min_dist=None, bnd_dist=50000.0):
+
+        if min_dist is None:
+            # Set minimum distance between to grid boundary points on polyline to 2 * dx
+            min_dist = self.model.grid.dx * 2 
+
+        # Get coordinates of boundary points
+        da_mask = self.model.grid.ds["mask"]
+        ibnd = np.where(da_mask.values == 2)
+        xp = da_mask["x"].values[ibnd]
+        yp = da_mask["y"].values[ibnd]
+
+
+
+        # Make boolean array for points that are include in a polyline 
+        used = np.full(xp.shape, False, dtype=bool)
+
+        polylines = []
+
+        while True:
+
+            if np.all(used):
+                # All boundary grid points have been used. We can stop now.
+                break
+
+            # Find first of the unused points
+            i1 = np.where(used==False)[0][0]
+
+            # Set this point to used
+            used[i1] = True
+
+            polyline = [i1] 
+
+            while True:
+                if np.all(used):
+                    # All boundary grid points have been used. We can stop now.
+                    break
+                # Started new polyline
+                dst = np.sqrt((xp - xp[i1])**2 + (yp - yp[i1])**2)
+                dst[polyline] = np.nan
+                inear = np.nanargmin(dst)
+                if dst[inear] < min_dist:
+                    # Found next point along polyline
+                    polyline.append(inear)
+                    used[inear] = True
+                    i1 = inear
+                else:
+                    # Last point found
+                    break    
+
+            i1 = polyline[0]
+            while True:
+                if np.all(used):
+                    # All boundary grid points have been used. We can stop now.
+                    break
+                # Now we go in the other direction            
+                dst = np.sqrt((xp - xp[i1])**2 + (yp - yp[i1])**2)
+                dst[polyline] = np.nan
+                inear = np.nanargmin(dst)
+                if dst[inear] < min_dist:
+                    # Found next point along polyline
+                    polyline.insert(0, inear)
+                    used[inear] = True
+                    i1 = inear
+                else:
+                    # Last point found
+                    # On to the next polyline
+                    break    
+
+            if len(polyline) > 1:  
+                polylines.append(polyline)
+
+        gdf_list = []
+        ip = 0
+
+        # If geographic, convert to Web Mercator
+        if self.model.crs.is_geographic:
+            transformer = Transformer.from_crs(self.model.crs,
+                                               3857,
+                                               always_xy=True)
+
+        # Loop through polylines 
+        for polyline in polylines:
+            x = xp[polyline]
+            y = yp[polyline]
+            points = [(x,y) for x,y in zip(x.ravel(),y.ravel())]                
+            line = shapely.geometry.LineString(points)
+            if self.model.crs.is_geographic:
+                # Line in web mercator (to get length in metres)
+                xm, ym = transformer.transform(x, y)
+                pointsm = [(xm,ym) for xm,ym in zip(xm.ravel(),ym.ravel())]
+                linem = shapely.geometry.LineString(pointsm)
+                num_points = int(linem.length / bnd_dist) + 2
+            else:
+                num_points = int(line.length / bnd_dist) + 2
+            # If geographic, convert to Web Mercator
+            new_points = [line.interpolate(i/float(num_points - 1), normalized=True) for i in range(num_points)]
+            # Loop through points in polyline
+            for point in new_points:
+                name = str(ip + 1).zfill(4)
+                d = {"name": name, "timeseries": pd.DataFrame(), "spectra": None, "geometry": point}
+                gdf_list.append(d)
+                ip += 1
+
+        self.gdf = gpd.GeoDataFrame(gdf_list, crs=self.model.crs)
 
 def read_timeseries_file(file_name, ref_date):
     # Returns a dataframe with time series for each of the columns
     df = pd.read_csv(file_name, index_col=0, header=None,
                      delim_whitespace=True)
     ts = ref_date + pd.to_timedelta(df.index, unit="s")
     df.index = ts
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/hurrywave/hurrywave.py` & `coastalhazardstoolkit-0.2.0/src/cht/hurrywave/hurrywave.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,66 +56,57 @@
 
         if load:
             self.input.read()
             # Get CRS from input file
             self.crs = CRS(self.input.variables.crs_name)
 
         self.grid                       = HurryWaveGrid(self)
-        self.mask                       = HurryWaveMask(self)
-        self.bathymetry                 = HurryWaveBathymetry(self)
+        # self.mask                       = HurryWaveMask(self)
+        # self.bathymetry                 = HurryWaveBathymetry(self)
         self.boundary_conditions        = HurryWaveBoundaryConditions(self)
         self.observation_points_regular = HurryWaveObservationPointsRegular(self)
         self.observation_points_sp2     = HurryWaveObservationPointsSpectra(self)
         self.obstacle                   = []
 
         # Now read the attribute files
         if load:
             self.read_attribute_files()
 
+    def clear_spatial_attributes(self):
+        # Clear all spatial data
+        self.grid                       = HurryWaveGrid(self)
+        self.boundary_conditions        = HurryWaveBoundaryConditions(self)
+        self.observation_points_regular = HurryWaveObservationPointsRegular(self)
+        self.observation_points_sp2     = HurryWaveObservationPointsSpectra(self)
+
     def read(self, path=None):
         if path:
             self.path = path
         self.input.read()
         # Get CRS from input file
         self.crs = CRS(self.input.variables.crs_name)
         self.read_attribute_files()
 
     def read_input_file(self):
         self.input.read()
         # Get CRS from input file
         self.crs = CRS(self.input.variables.crs_name)
 
     def read_attribute_files(self):
-
-        # Grid
-        self.grid.build(self.input.variables.x0,
-                        self.input.variables.y0,
-                        self.input.variables.dx,
-                        self.input.variables.dy,
-                        self.input.variables.mmax,
-                        self.input.variables.nmax,
-                        self.input.variables.rotation,
-                        self.crs)
-
-        self.mask.read()
-        self.bathymetry.read()
+        self.grid.read()
         self.boundary_conditions.read()
         self.observation_points_regular.read()
         self.observation_points_sp2.read()
 
     def write(self):
         self.input.write()
         self.write_attribute_files()
         
-
     def write_attribute_files(self):
-
-        # Wave boundary conditions
-        self.mask.write()
-        self.bathymetry.write()
+        self.grid.write()
         self.boundary_conditions.write()
         self.observation_points_regular.write()
         self.observation_points_sp2.write()
 
     def write_batch_file(self):
         fid = open(os.path.join(self.path, "run.bat"), "w")
         fid.write(self.exe_path + "\\" + "hurrywave.exe")
@@ -366,15 +357,15 @@
                                parameter = "hm0"):
 
         import xarray as xr
         import pandas as pd
         import numpy as np
 
         # Returns a dataframe with timeseries    
-        
+        # parameter options: hm0, tp, wavdir, dirsp        
         if not path:
             path = self.path
 
         if not file_name:
             file_name = "hurrywave_his.nc"
 
         file_name = os.path.join(path, file_name)
@@ -393,53 +384,23 @@
         if not name_list:
             name_list = []
             for st in all_stations:
                 name_list.append(st)
         
         df = pd.DataFrame(index=times, columns=name_list)
         
-        if parameter.lower() == "hm0":
-        
-            for station in name_list:
-                for ist, st in enumerate(all_stations):
-                    if station == st:
-                        data = ddd.point_hm0.values[:,ist]
-                        data[np.isnan(data)] = -999.0
-                        df[st]=data
-                        break            
-
-        elif parameter.lower() == "tp":
-        
-            for station in name_list:
-                for ist, st in enumerate(all_stations):
-                    if station == st:
-                        data = ddd.point_tp.values[:,ist]
-                        data[np.isnan(data)] = -999.0
-                        df[st]=data
-                        break            
-
-        elif parameter.lower() == "wavdir":
-        
-            for station in name_list:
-                for ist, st in enumerate(all_stations):
-                    if station == st:
-                        data = ddd.point_wavdir.values[:,ist]
-                        data[np.isnan(data)] = -999.0
-                        df[st]=data
-                        break            
-
-        elif parameter.lower() == "dirspr":
-        
-            for station in name_list:
-                for ist, st in enumerate(all_stations):
-                    if station == st:
-                        data = ddd.point_dirsp.values[:,ist]
-                        data[np.isnan(data)] = -999.0
-                        df[st]=data
-                        break            
+        data_tmp = ddd["point_" + parameter].values
+
+        for station in name_list:
+            for ist, st in enumerate(all_stations):
+                if station == st:
+                    data = data_tmp[:,ist]
+                    data[np.isnan(data)] = -999.0
+                    df[st]=data
+                    break            
 
         ddd.close()
         
         return df    
         
         # # Returns a dataframe with timeseries
     
@@ -459,16 +420,43 @@
         # # Add column names
         # df.columns = columns
             
         # if name_list:
         #     df = df[name_list]
             
         # return df    
+    def read_map_output_max(self, time_range=None, map_file=None, parameter = "hm0"):
+    
+        if not map_file:
+            map_file = os.path.join(self.path, "hurrywave_map.nc")
+            
+        dsin = xr.open_dataset(map_file)
+
+        output_times = dsin.timemax.values
+        if time_range is None:
+
+            t0 = pd.to_datetime(str(output_times[0])).replace(tzinfo=None).to_pydatetime()
+            t1 = pd.to_datetime(str(output_times[-1])).replace(tzinfo=None).to_pydatetime()
+            time_range = [t0, t1]
 
-    def read_hm0max(self, time_range=None, hm0max_file=None):
+        it0 = -1
+        for it, time in enumerate(output_times):
+            time = pd.to_datetime(str(time)).replace(tzinfo=None).to_pydatetime()
+            if time>=time_range[0] and it0<0:
+                it0 = it
+            if time<=time_range[1]:
+                it1 = it
+        
+        zs_da = np.amax(dsin[parameter].values[it0:it1,:,:], axis=0)
+        dsin.close()
+        
+        return zs_da
+
+
+    def read_hm0max(self, time_range=None, hm0max_file=None, parameter='hm0max'):
     
         if not hm0max_file:
             hm0max_file = os.path.join(self.path, "hm0max.dat")
             
         fname, ext = os.path.splitext(hm0max_file)
         
         if ext == ".dat":
@@ -523,17 +511,17 @@
 
             it0 = -1
             for it, time in enumerate(output_times):
                 time = pd.to_datetime(str(time)).replace(tzinfo=None).to_pydatetime()
                 if time>=time_range[0] and it0<0:
                     it0 = it
                 if time<=time_range[1]:
-                    it1 = it
+                    it1 = it            
             
-            zs_da = np.transpose(np.amax(dsin.hm0max.values[it0:it1,:,:], axis=0))
+            zs_da = np.amax(dsin[parameter].values[it0:it1,:,:], axis=0)
             dsin.close()
             
         else:
             # Must be txt file
             return None
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/hurrywave/hurrywave_builder.py` & `coastalhazardstoolkit-0.2.0/src/cht/hurrywave/hurrywave_builder.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/hurrywave/hurrywave_domain.py` & `coastalhazardstoolkit-0.2.0/src/cht/hurrywave/hurrywave_domain.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/hurrywave/input.py` & `coastalhazardstoolkit-0.2.0/src/cht/hurrywave/input.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Jun 18 09:03:08 2022
 @author: ormondt
 """
 import os
 import datetime
+import copy
 
 class Variables:
     def __init__(self):
         pass
 
 class HurryWaveInput:
     def __init__(self, hw):
@@ -53,18 +54,20 @@
         self.variables.crs_type = "geographic"
         self.variables.crs_utmzone = None
         self.variables.crs_epsg = None
         self.variables.gammajsp = 3.3
         self.variables.spinup_meteo = 1
         self.variables.quadruplets = 1
         self.variables.redopt = 1
+        self.variables.redopt = 1
+        self.variables.winddrag = "zijlema"
+        self.variables.cdcap = 0.0025
 
         self.variables.depfile = None
         self.variables.mskfile = None
-        self.variables.indexfile = None
         self.variables.bndfile = None
         self.variables.bhsfile = None
         self.variables.btpfile = None
         self.variables.bwdfile = None
         self.variables.bdsfile = None
         self.variables.bspfile = None
         self.variables.rstfile = None
@@ -74,17 +77,17 @@
         self.variables.wndfile = None
         self.variables.obsfile = None
         self.variables.ospfile = None
 
         self.variables.inputformat = "bin"
         self.variables.outputformat = "net"
 
-        self.variables.cdnrb = 3
-        self.variables.cdwnd = [0.0, 28.0, 50.0]
-        self.variables.cdval = [0.001, 0.0025, 0.0015]
+        # self.variables.cdnrb = 3
+        # self.variables.cdwnd = [0.0, 28.0, 50.0]
+        # self.variables.cdval = [0.001, 0.0025, 0.0015]
 
     def read(self):
         # Reads hurrywave.inp
         file_name = os.path.join(self.model.path, "hurrywave.inp")
         fid = open(file_name, 'r')
         lines = fid.readlines()
         fid.close()
@@ -109,18 +112,28 @@
             if name == "tstart":
                 val = datetime.datetime.strptime(val.rstrip(), '%Y%m%d %H%M%S')
             if name == "tstop":
                 val = datetime.datetime.strptime(val.rstrip(), '%Y%m%d %H%M%S')
             setattr(self.variables, name, val)
 
     def write(self):
+
         file_name = os.path.join(self.model.path, "hurrywave.inp")
+        variables = copy.copy(self.variables)
+        # Remove some input variables
+        if self.model.boundary_conditions.forcing == "spectra":
+            variables.bhsfile = None
+            variables.btpfile = None
+            variables.bwdfile = None
+            variables.bdsfile = None
+        else:
+            variables.bspfile = None
+
         fid = open(file_name, "w")
-#        for key, value in self.input.__dict__.items():
-        for key, value in self.variables.__dict__.items():
+        for key, value in variables.__dict__.items():
             if not value is None:
                 if type(value) == "float":
                     string = f'{key.ljust(20)} = {float(value)}\n'
                 elif type(value) == "int":
                     string = f'{key.ljust(20)} = {int(value)}\n'
                 elif type(value) == list:
                     valstr = ""
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/hurrywave/mask.py` & `coastalhazardstoolkit-0.2.0/src/cht/hurrywave/mask.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/hurrywave/observation_points.py` & `coastalhazardstoolkit-0.2.0/src/cht/hurrywave/observation_points.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Created on Sat Jun 18 09:03:08 2022
 @author: ormondt
 """
 import os
 import geopandas as gpd
 import shapely
 import pandas as pd
+import numpy as np
+from matplotlib import path
 
 class HurryWaveObservationPointsRegular:
     def __init__(self, hw):
         self.model = hw
         self.gdf  = gpd.GeoDataFrame()
 
     def read(self):
@@ -35,14 +37,15 @@
             d = {"name": name, "long_name": None, "geometry": point}
             gdf_list.append(d)
         self.gdf = gpd.GeoDataFrame(gdf_list, crs=self.model.crs)
 
     def write(self):
 
         if not self.model.input.variables.obsfile:
+            print("No name for obs file !")
             return
         if len(self.gdf.index)==0:
             return
 
         file_name = os.path.join(self.model.path, self.model.input.variables.obsfile)
         
         if self.model.crs.is_geographic:
@@ -68,31 +71,51 @@
         point = shapely.geometry.Point(x, y)
         gdf_list = []
         d = {"name": name, "long_name": None, "geometry": point}
         gdf_list.append(d)
         gdf_new = gpd.GeoDataFrame(gdf_list, crs=self.model.crs)
         self.gdf = pd.concat([self.gdf, gdf_new], ignore_index=True)
 
-    def delete_point(self, name):
-        for index, row in self.gdf.iterrows():
-            if row["name"] == name:
-                self.gdf = self.gdf.drop(index).reset_index(drop=True)
-                return
-        print("Point " + name + " not found!")    
-        
+    def delete_point(self, name_or_index):
+        if type(name_or_index) == str:
+            name = name_or_index
+            for index, row in self.gdf.iterrows():
+                if row["name"] == name:
+                    self.gdf = self.gdf.drop(index).reset_index(drop=True)
+                    return
+            print("Point " + name + " not found!")
+        else:
+            index = name_or_index
+            self.gdf = self.gdf.drop(index).reset_index(drop=True)
+
     def clear(self):
         self.gdf  = gpd.GeoDataFrame()
 
     def list_observation_points(self):
         names = []
         for index, row in self.gdf.iterrows():
             names.append(row["name"])
         return names
 
-
+    def add_points(self, gdf, name="name"):
+        outline = self.model.grid.outline().loc[0]["geometry"]
+        gdf = gdf.to_crs(self.model.crs)
+        x = np.empty((len(gdf)))
+        y = np.empty((len(gdf)))
+        for index, row in gdf.iterrows():
+            x[index] = row["geometry"].coords[0][0]
+            y[index] = row["geometry"].coords[0][1]
+        inpol = inpolygon(x, y, outline)
+        gdf_list = []
+        for index, row in gdf.iterrows():
+            if inpol[index]:
+                d = {"name": row[name], "long_name": None, "geometry": shapely.geometry.Point(x[index], y[index])}
+                gdf_list.append(d)
+        gdf_new = gpd.GeoDataFrame(gdf_list, crs=self.model.crs)
+        self.gdf = pd.concat([self.gdf, gdf_new], ignore_index=True)
 
 class HurryWaveObservationPointsSpectra:
     def __init__(self, hw):
         self.model = hw
         self.gdf  = gpd.GeoDataFrame()
 
     def read(self):
@@ -150,22 +173,35 @@
         point = shapely.geometry.Point(x, y)
         gdf_list = []
         d = {"name": name, "long_name": None, "geometry": point}
         gdf_list.append(d)
         gdf_new = gpd.GeoDataFrame(gdf_list, crs=self.model.crs)
         self.gdf = pd.concat([self.gdf, gdf_new], ignore_index=True)
 
-    def delete_point(self, name):
-        for index, row in self.gdf.iterrows():
-            if row["name"] == name:
-                self.gdf = self.gdf.drop(index).reset_index(drop=True)
-                return
-        print("Point " + name + " not found!")    
+    def delete_point(self, name_or_index):
+        if type(name_or_index) == str:
+            name = name_or_index
+            for index, row in self.gdf.iterrows():
+                if row["name"] == name:
+                    self.gdf = self.gdf.drop(index).reset_index(drop=True)
+                    return
+            print("Point " + name + " not found!")
+        else:
+            index = name_or_index
+            self.gdf = self.gdf.drop(index).reset_index(drop=True)
         
     def clear(self):
         self.gdf  = gpd.GeoDataFrame()
 
     def list_observation_points(self):
         names = []
         for index, row in self.gdf.iterrows():
             names.append(row["name"])
         return names
+
+def inpolygon(xq, yq, p):
+    shape = xq.shape
+    xq = xq.reshape(-1)
+    yq = yq.reshape(-1)
+    q = [(xq[i], yq[i]) for i in range(xq.shape[0])]
+    p = path.Path([(crds[0], crds[1]) for i, crds in enumerate(p.exterior.coords)])
+    return p.contains_points(q).reshape(shape)
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/coamps_analysis.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/coamps_analysis.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/coamps_tc_forecast.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/coamps_tc_forecast.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/coamps_tc_hindcast.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/coamps_tc_hindcast.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/coamps_tc_ufl_d01.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/coamps_tc_ufl_d01.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_anl_0p50.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_anl_0p50.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_anl_0p50_02.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_anl_0p50_02.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_anl_0p50_03.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_anl_0p50_03.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_anl_0p50_04.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_anl_0p50_04.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_forecast_0p25.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_forecast_0p25.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/gfs_forecast_0p25_02.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/gfs_forecast_0p25_02.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/meteo.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/meteo.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import cht.misc.fileops as fo
 
 # Added for TCs
 from cht.tropical_cyclone.tropical_cyclone import TropicalCyclone
 import geopandas as gpd
 from shapely.geometry import Point
 date_format     = "%Y%m%d %H%M%S"
+import requests
 
 class MeteoSource():
     
     # e.g. GFS forecast
     def __init__(self, name, module_name, source_type,
                  crs=None, long_name=None, delay=None,
                  cycle_interval=6, time_interval=3):
@@ -351,19 +352,15 @@
                             self.last_analysis_time = t
 
             # Use earliest forecast file available for spinup (force earlier timesteps with this file)
             ID1= next(i for i,v in enumerate(requested_files) if v is not None)
             for ind in range(ID1):
                 requested_files[ind]=requested_files[ID1]
 
-            for ind, file in enumerate(requested_files):
-                if not file:
-                    times_to_remove.append(requested_times[ind])
-
-            # Get rid of None values
+                # Get rid of None values
             times_to_remove = []
             for ind, file in enumerate(requested_files):
                 if not file:
                     times_to_remove.append(requested_times[ind])
             if times_to_remove:  
                 for tr in times_to_remove:
                     requested_times.remove(tr)
@@ -907,35 +904,33 @@
     def find_cyclone_tracks(self,
                             xlim=[-1.0e9, 1.0e9],
                             ylim=[-1.0e9, 1.0e9],
                             pcyc=99000.0,
                             dist=2.0,
                             dt=6):
 
-        tstride = np.round(dt/self.source.time_interval).astype(int)  
-                
-        tracks = []
-        
-        nt = np.size(self.time)
+        # Settings of the algorithm
+        tstride     = np.round(dt/self.source.time_interval).astype(int)  
+        tracks      = []
+        nt          = np.size(self.time)
 
+        # Loop over time
         for it in range(0, nt, tstride):
-#        for it, time in enumerate(self.time[::tstride]):
             
             x = self.x
             y = self.y
             time = self.time[it]
             u = np.squeeze(self.quantity[0].u[it,:,:])
             v = np.squeeze(self.quantity[0].v[it,:,:])
             p = np.squeeze(self.quantity[1].val[it,:,:])
             
             xeye, yeye, vmax, peye = find_cyclone_eyes(x, y, u, v, p,
                                                        pcyc, dist,
                                                        xlim, ylim)
             
-
             # Check if these locations match with previous tracks
             for j in range(len(xeye)):
                 itrack = -1
                 for k, track in enumerate(tracks):
                     coords              = track.track.geometry
                     ids_coords          = track.track.geometry.size
                     dst                 = np.sqrt((coords[ids_coords-1].x - xeye[j])**2 + (coords[ids_coords-1].y - yeye[j])**2)
@@ -972,14 +967,74 @@
                     tracks[-1].track = tracks[-1].track.reset_index(drop=True)
                     tracks[-1].track = tracks[-1].track.drop([0])           # remove the dummy
                     tracks[-1].track = tracks[-1].track.reset_index(drop=True)
 
         # return tracks
         return tracks                    
 
+# Function to filter the tracks based on TCvitals
+def filter_cyclones_TCvitals(tracks):
+
+    # Settings
+    dist        = 2.0                                                       # needs to be within 2 degrees 
+    time_range  = datetime.timedelta(hours=6)
+
+    # Read TCvitals
+    url         = 'https://ftp.nhc.noaa.gov/atcf/com/tcvitals'
+    tcvitals    = requests.get(url)                                         # read data
+    tcvitals    = tcvitals.text
+    splits      = [line.split() for line in tcvitals.split('\n')[:-1]]      # last line is empty
+
+    # Is this a real track according to the TCvitals?
+    remove_eye = np.zeros(len(tracks))                                      # in principle we keep it all
+    for split in splits:
+
+        # Get subset
+        date_string         = split[3] + ' ' + split[4]
+        datetime_object     = datetime.datetime.strptime(date_string, '%Y%m%d %H%M')
+
+        # Determine latitude
+        if split[5][-1] == 'N':
+            lat_object          = float(split[5][0:-1]) / 10   # northern hemisphere
+        else:
+            lat_object          = float(split[5][0:-1]) / -10  # southern hemisphere
+
+        # Determine longitude
+        if split[6][-1] == 'W':
+            lon_object          = float(split[6][0:-1])/-10
+        else:
+            lon_object          = float(split[6][0:-1])/10
+
+        # Loop over tracks
+        for k, track in enumerate(tracks):
+
+            # Loop over time stamps
+            for tt in range(len(track.track.geometry)):
+                track_time          = track.track.datetime[tt]
+                track_time          = datetime.datetime.strptime(track_time, date_format)
+                time_difference     = datetime_object - track_time
+
+                # Within time window
+                if time_difference <= time_range:
+                    
+                    # Yes, this is TCvital that can be used
+                    xeye = track.track.geometry[tt].x
+                    yeye = track.track.geometry[tt].y
+                    dst  = np.sqrt((lon_object - xeye)**2 + (lat_object- yeye)**2)
+                    if dst>dist:
+                        remove_eye[k] = 1                   # unless, it is too far for time stamp wanted
+    
+    # Done with all this; let now really remove based on remove_eye
+    remove_tracks       = remove_eye>0
+    tracks_filtered     = [track for track, remove in zip(tracks, remove_tracks) if not remove]
+
+    # return tracks
+    return tracks_filtered         
+
+
 def merge(forcing_list):
 
     meteo_grid = MeteoGrid()
 
     return meteo_grid
 
 
@@ -1289,16 +1344,18 @@
     yeye = []
     vmax = []
     pc   = []
     
     xx, yy = np.meshgrid(x, y)
     
     vmag = np.sqrt(u**2 + v**2)
+    rot_z, av = curl(xx,yy,u,v)
     
-    ibelow = np.where(p<pcyc)
+#    ibelow = np.where(p<pcyc)
+    ibelow = np.where(rot_z>40.0)
     xb = xx[ibelow]
     yb = yy[ibelow]
     
     iin = np.where((xb>=xlim[0]) & (xb<=xlim[1]) & (yb>=ylim[0]) & (yb<=ylim[1]))
     xb = xb[iin]
     yb = yb[iin]
     
@@ -1312,16 +1369,16 @@
         for k, cluster in enumerate(clusters):
          
             # Centre of the cluster
             xc = cluster.x
             yc = cluster.y
             
             # Grid indices        
-            ix = np.where(x>xc)[0][0]
-            iy = np.where(y>yc)[0][0]
+            ix = np.where(x>=xc)[0][0]
+            iy = np.where(y>=yc)[0][0]
     
             i0 = max(iy - ng, 0)         
             i1 = min(iy + ng, np.size(y) -1)      
             j0 = max(ix - ng, 0)         
             j1 = min(ix + ng, np.size(x) -1)      
             
             xxx = x[j0:j1]
@@ -1394,8 +1451,57 @@
 
 class Cluster():
     
     def __init__(self):
         self.x     = None
         self.y     = None
         self.index = None
-        
+
+def curl(x0, y0, u0, v0):
+
+    n = np.shape(x0)[0]
+    m = np.shape(x0)[1]
+
+    x = np.empty((n, m, 2))
+    y = np.empty((n, m, 2))
+    z = np.empty((n, m, 2))
+    u = np.empty((n, m, 2))
+    v = np.empty((n, m, 2))
+    w = np.empty((n, m, 2))
+
+    x[:,:,0] = x0
+    x[:,:,1] = x0
+    y[:,:,0] = y0
+    y[:,:,1] = y0
+    z[:,:,0] = 0.0
+    z[:,:,1] = 0.0
+    u[:,:,0] = u0
+    u[:,:,1] = u0
+    v[:,:,0] = v0
+    v[:,:,1] = v0
+    w[:]     = 0.0
+
+    dx = x[0,:,0]
+    dy = y[:,0,0]
+    dz = z[0,0,:]
+
+    dummy, dFx_dy, dFx_dz = np.gradient (u, dx, dy, dz, axis=[1,0,2])
+    dFy_dx, dummy, dFy_dz = np.gradient (v, dx, dy, dz, axis=[1,0,2])
+    dFz_dx, dFz_dy, dummy = np.gradient (w, dx, dy, dz, axis=[1,0,2])
+
+    rot_x = dFz_dy - dFy_dz
+    rot_y = dFx_dz - dFz_dx
+    rot_z = dFy_dx - dFx_dy
+
+    l = np.sqrt(np.power(u,2.0) + np.power(v,2.0) + np.power(w,2.0));
+
+    m1 = np.multiply(rot_x,u)
+    m2 = np.multiply(rot_y,v)
+    m3 = np.multiply(rot_z,w)
+
+    tmp1 = (m1 + m2 + m3)
+    tmp2 = np.multiply(l,2.0)
+
+    av = np.divide(tmp1, tmp2)
+
+    rot_z = rot_z[:,:,0]
+    return rot_z, av
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/meteo/test_coamps.py` & `coastalhazardstoolkit-0.2.0/src/cht/meteo/test_coamps.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 # NOTE YOU NEED GEOPANDAS
 
 import datetime
 import matplotlib.pyplot as plt
 from cht.meteo.meteo import MeteoSource, MeteoGrid
+from cht.meteo.meteo import filter_cyclones_TCvitals
 
 # Define a track
 source = MeteoSource("coamps", "coamps_tc_forecast", "forecast",
                      delay=6)
 
 parameters = ["wind", "barometric_pressure"]
 x_range = [-100.0, -80.0]
@@ -26,14 +27,17 @@
 t0 = datetime.datetime(2017,9,17,0,0,0)
 t1 = datetime.datetime(2017,9,22,0,0,0)
 ds.collect(time_range=[t0, t1])
 
 # New determine best-track from these files
 tracks = ds.find_cyclone_tracks(pcyc=99999, dt=6)
 
+# Filter cyclone based on TCvitals
+tracks = filter_cyclones_TCvitals(tracks)
+
 # Write them out as geojson at location
 for k, track in enumerate(tracks):
     
     # Check the size - only if there are 3 timestamps
     if track.track.geometry.size > 3:
 
         # Save as cyc
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/misc/deltares_ini.py` & `coastalhazardstoolkit-0.2.0/src/cht/misc/deltares_ini.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/misc/fileops.py` & `coastalhazardstoolkit-0.2.0/src/cht/misc/fileops.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,48 +6,54 @@
 """
 
 import glob
 import shutil
 import os
 
 def move_file(src, dst):
-    
     for full_file_name in glob.glob(src):
         src_name = os.path.basename(full_file_name)        
         if os.path.exists(os.path.join(dst, src_name)):
             # Try removing existing file
             try:                
                 os.remove(os.path.join(dst, src_name))
             except:
                 print("Could not remove file " + os.path.join(dst, src_name))
         try:        
             shutil.move(full_file_name, dst)
         except:
             print("Could not move file " + full_file_name)
-            
+
 
 def copy_file(src, dst):
     
     for full_file_name in glob.glob(src):
         src_name = os.path.basename(full_file_name)        
         if os.path.exists(os.path.join(dst, src_name)):
             os.remove(os.path.join(dst, src_name))
         if os.path.isdir(full_file_name):
             dstf = os.path.join(dst, os.path.basename(full_file_name))
             shutil.copytree(full_file_name, dstf)
         else:    
             shutil.copy(full_file_name, dst)
 
 def delete_file(src):
-    
-    for file_name in glob.glob(src):
-        try:
-            os.remove(src)
-        except:
-            print("Could not delete " + src)
+    if isinstance(src, list):
+        for i,v in enumerate(src):
+            for file_name in glob.glob(v):
+                try:
+                    os.remove(v)
+                except:
+                    print("Could not delete " + v)
+    else:
+        for file_name in glob.glob(src):
+            try:
+                os.remove(src)
+            except:
+                print("Could not delete " + src)
 
 def rm(src):
     
     os.remove(src)
 
 def mkdir(path):
 
@@ -63,28 +69,28 @@
             if os.path.isfile(item):
                 file_list.append(item)                
     else:
         file_list = os.listdir(src)
 #                file_list.append(os.path.basename(item))
 #                print(it)
                 
-    return file_list
+    return sorted(file_list)
 
 def list_folders(src, basename=False):
     
     folder_list = []
     full_list = glob.glob(src)
     for item in full_list:
         if os.path.isdir(item):
             if basename:
                 folder_list.append(os.path.basename(item))
             else:
                 folder_list.append(item)                
 
-    return folder_list
+    return sorted(folder_list)
 
 def delete_folder(src):
     try:
         shutil.rmtree(src, ignore_errors=False, onerror=None)
     except:
         # Folder was probably open in another application
         print("Could not delete folder " + src)
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/misc/geometry.py` & `coastalhazardstoolkit-0.2.0/src/cht/misc/geometry.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/misc/misc_tools.py` & `coastalhazardstoolkit-0.2.0/src/cht/misc/misc_tools.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/misc/sftp.py` & `coastalhazardstoolkit-0.2.0/src/cht/misc/sftp.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/misc/tekal.py` & `coastalhazardstoolkit-0.2.0/src/cht/misc/tekal.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/misc/xmlkit.py` & `coastalhazardstoolkit-0.2.0/src/cht/misc/xmlkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Created on Wed May 12 08:59:03 2021
 
 @author: ormondt
 """
 
 import xml.etree.ElementTree as ET
 from datetime import datetime
+import urllib
 
 class XMLObject():
     def __init__(self):
         # Empty object
         pass
 
 
@@ -143,11 +144,16 @@
             elif node.attrib["type"] == "datetime":
                 val = datetime.strptime(node.text,
                                                 '%Y%m%d %H%M%S')
     return val
 
 def xml2obj(file_name):    
 
-    xml_root = ET.parse(file_name).getroot()
+    if file_name[0:4] == "http":
+        with urllib.request.urlopen(file_name) as f:
+            tree = ET.parse(f)
+            xml_root = tree.getroot()        
+    else:        
+        xml_root = ET.parse(file_name).getroot()
     obj = xml2py(xml_root)
 
     return obj
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/model_builder/model_builder.py` & `coastalhazardstoolkit-0.2.0/src/cht/model_builder/model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,20 +159,20 @@
         self.setup_config["mask"]                             = {}
         self.setup_config["mask"]["zmin"]                     = -99999.0
         self.setup_config["mask"]["zmax"]                     = 99999.0
         self.setup_config["mask"]["include_polygon"]          = []
         self.setup_config["mask"]["exclude_polygon"]          = []
         self.setup_config["mask"]["open_boundary_polygon"]    = []
         self.setup_config["mask"]["outflow_boundary_polygon"] = []
-        self.setup_config["wave_mask"]                             = {}
-        self.setup_config["wave_mask"]["zmin"]                     = -99999.0
-        self.setup_config["wave_mask"]["zmax"]                     = 99999.0
-        self.setup_config["wave_mask"]["include_polygon"]          = []
-        self.setup_config["wave_mask"]["exclude_polygon"]          = []
-        self.setup_config["wave_mask"]["open_boundary_polygon"]    = []
+        # self.setup_config["wave_mask"]                             = {}
+        # self.setup_config["wave_mask"]["zmin"]                     = -99999.0
+        # self.setup_config["wave_mask"]["zmax"]                     = 99999.0
+        # self.setup_config["wave_mask"]["include_polygon"]          = []
+        # self.setup_config["wave_mask"]["exclude_polygon"]          = []
+        # self.setup_config["wave_mask"]["open_boundary_polygon"]    = []
         self.setup_config["subgrid"]                          = {}
         self.setup_config["subgrid"]["nr_bins"]               = 5
         self.setup_config["subgrid"]["zmin"]                  = -99999.0
         self.setup_config["subgrid"]["max_gradient"]          = 5.0
         self.setup_config["subgrid"]["nr_subgrid_pixels"]     = 20
         self.setup_config["bathymetry"]                       = {}
         self.setup_config["bathymetry"]["dataset"]            = []
@@ -269,48 +269,49 @@
                     polygon["zmin"] = -99999.0
                 if "zmax" not in polygon:
                     polygon["zmax"] = 99999.0
 
 
         if "wave_mask" not in self.setup_config:
             self.setup_config["wave_mask"] = {}
-            self.setup_config["wave_mask"]["zmin"] = -99999.0
-            self.setup_config["wave_mask"]["zmax"] = 99999.0
+            # self.setup_config["wave_mask"]["zmin"] = -99999.0
+            # self.setup_config["wave_mask"]["zmax"] = 99999.0
         else:
             if "zmin" not in self.setup_config["wave_mask"]:
                 self.setup_config["wave_mask"]["zmin"] = -99999.0
             if "zmax" not in self.setup_config["wave_mask"]:
                 self.setup_config["wave_mask"]["zmax"] = 99999.0
 
-        if "include_polygon" not in self.setup_config["wave_mask"]:
-            self.setup_config["wave_mask"]["include_polygon"] = []
-        if self.setup_config["wave_mask"]["include_polygon"]:
-            for polygon in self.setup_config["wave_mask"]["include_polygon"]:
-                if "zmin" not in polygon:
-                    polygon["zmin"] = -99999.0
-                if "zmax" not in polygon:
-                    polygon["zmax"] = 99999.0
-
-        if "exclude_polygon" not in self.setup_config["wave_mask"]:
-            self.setup_config["wave_mask"]["exclude_polygon"] = []
-        if self.setup_config["wave_mask"]["exclude_polygon"]:
-            for polygon in self.setup_config["wave_mask"]["exclude_polygon"]:
-                if "zmin" not in polygon:
-                    polygon["zmin"] = -99999.0
-                if "zmax" not in polygon:
-                    polygon["zmax"] = 99999.0
-
-        if "open_boundary_polygon" not in self.setup_config["wave_mask"]:
-            self.setup_config["wave_mask"]["open_boundary_polygon"] = []
-        if self.setup_config["wave_mask"]["open_boundary_polygon"]:
-            for polygon in self.setup_config["wave_mask"]["open_boundary_polygon"]:
-                if "zmin" not in polygon:
-                    polygon["zmin"] = -99999.0
-                if "zmax" not in polygon:
-                    polygon["zmax"] = 99999.0
+        if self.setup_config["wave_mask"]:
+            if "include_polygon" not in self.setup_config["wave_mask"]:
+                self.setup_config["wave_mask"]["include_polygon"] = []
+            if self.setup_config["wave_mask"]["include_polygon"]:
+                for polygon in self.setup_config["wave_mask"]["include_polygon"]:
+                    if "zmin" not in polygon:
+                        polygon["zmin"] = -99999.0
+                    if "zmax" not in polygon:
+                        polygon["zmax"] = 99999.0
+    
+            if "exclude_polygon" not in self.setup_config["wave_mask"]:
+                self.setup_config["wave_mask"]["exclude_polygon"] = []
+            if self.setup_config["wave_mask"]["exclude_polygon"]:
+                for polygon in self.setup_config["wave_mask"]["exclude_polygon"]:
+                    if "zmin" not in polygon:
+                        polygon["zmin"] = -99999.0
+                    if "zmax" not in polygon:
+                        polygon["zmax"] = 99999.0
+    
+            if "open_boundary_polygon" not in self.setup_config["wave_mask"]:
+                self.setup_config["wave_mask"]["open_boundary_polygon"] = []
+            if self.setup_config["wave_mask"]["open_boundary_polygon"]:
+                for polygon in self.setup_config["wave_mask"]["open_boundary_polygon"]:
+                    if "zmin" not in polygon:
+                        polygon["zmin"] = -99999.0
+                    if "zmax" not in polygon:
+                        polygon["zmax"] = 99999.0
 
 
         if "subgrid" not in self.setup_config:
             self.setup_config["subgrid"] = {}
         else:
             if "nr_bins" not in self.setup_config["subgrid"]:                
                 self.setup_config["subgrid"]["nr_bins"]               = 5
@@ -422,42 +423,43 @@
             for p in polygons:
                 self.outflow_boundary_polygons.append(MaskPolygon(x=p.x,
                                                                   y=p.y,
                                                                   zmin=polygon["zmin"],
                                                                   zmax=polygon["zmax"]))            
 
         # Wave mask polygons        
-        self.wave_include_polygons = []
-        for polygon in self.setup_config["wave_mask"]["include_polygon"]:
-            polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
-            # Polygon file may include multiple polygons
-            for p in polygons:
-                self.wave_include_polygons.append(MaskPolygon(x=p.x,
-                                                         y=p.y,
-                                                         zmin=polygon["zmin"],
-                                                         zmax=polygon["zmax"]))            
-    
-        self.wave_exclude_polygons = []
-        for polygon in self.setup_config["wave_mask"]["exclude_polygon"]:
-            polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
-            # Polygon file may include multiple polygons
-            for p in polygons:
-                self.wave_exclude_polygons.append(MaskPolygon(x=p.x,
-                                                         y=p.y,
-                                                         zmin=polygon["zmin"],
-                                                         zmax=polygon["zmax"]))            
-        self.wave_open_boundary_polygons = []
-        for polygon in self.setup_config["wave_mask"]["open_boundary_polygon"]:
-            polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
-            # Polygon file may include multiple polygons
-            for p in polygons:
-                self.wave_open_boundary_polygons.append(MaskPolygon(x=p.x,
-                                                   y=p.y,
-                                                   zmin=polygon["zmin"],
-                                                   zmax=polygon["zmax"]))            
+        if self.setup_config["wave_mask"]:
+            self.wave_include_polygons = []
+            for polygon in self.setup_config["wave_mask"]["include_polygon"]:
+                polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
+                # Polygon file may include multiple polygons
+                for p in polygons:
+                    self.wave_include_polygons.append(MaskPolygon(x=p.x,
+                                                             y=p.y,
+                                                             zmin=polygon["zmin"],
+                                                             zmax=polygon["zmax"]))            
+        
+            self.wave_exclude_polygons = []
+            for polygon in self.setup_config["wave_mask"]["exclude_polygon"]:
+                polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
+                # Polygon file may include multiple polygons
+                for p in polygons:
+                    self.wave_exclude_polygons.append(MaskPolygon(x=p.x,
+                                                             y=p.y,
+                                                             zmin=polygon["zmin"],
+                                                             zmax=polygon["zmax"]))            
+            self.wave_open_boundary_polygons = []
+            for polygon in self.setup_config["wave_mask"]["open_boundary_polygon"]:
+                polygons = read_pli_file(os.path.join(self.data_path, polygon["file_name"]))
+                # Polygon file may include multiple polygons
+                for p in polygons:
+                    self.wave_open_boundary_polygons.append(MaskPolygon(x=p.x,
+                                                       y=p.y,
+                                                       zmin=polygon["zmin"],
+                                                       zmax=polygon["zmax"]))            
 
                 
         # Bathymetry and roughness
         self.bathymetry_list = []
         for dataset in self.setup_config["bathymetry"]["dataset"]:
             self.bathymetry_list.append(BathymetryDataset(name=dataset["name"],
                                                           source=dataset["source"],
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/nesting/nest1.py` & `coastalhazardstoolkit-0.2.0/src/cht/nesting/nest1.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/nesting/nest2.py` & `coastalhazardstoolkit-0.2.0/src/cht/nesting/nest2.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,52 @@
 from pyproj import CRS
 from pyproj import Transformer
 import pandas as pd
 import xarray as xr
 import numpy as np
 import glob
 import datetime 
+from cht.misc.deltares_ini import IniStruct
+from cht.tide.tide_predict import predict
 
 def nest2(overall,
           detail,
           boundary_water_level_correction=None,
           output_path=None,
           output_file=None,
 	      option=None,
-          return_maximum = False):
+          return_maximum=False,
+          ensemble=False,
+          ensemble_member_index=None,
+          bc_path=None):
 
 
     if not boundary_water_level_correction:
         # Path of the overall output time series
         boundary_water_level_correction = 0.0
     
+    if type(overall) == str:
+        overall_str = overall
+        if overall == "sfincs":
+            from cht.sfincs.sfincs import SFINCS
+            overall = SFINCS()
+        elif overall == "hurrywave":
+            from cht.hurrywave.hurrywave import HurryWave
+            overall = HurryWave()
+        elif overall == "xbeach":
+            from cht.xbeach.xbeach import XBeach
+            overall = XBeach()
+        elif overall == "beware":
+            from cht.beware.beware import Beware
+            overall = Beware()
+        elif overall == "delft3dfm":
+            from cht.delft3dfm.delft3dfm import Delft3DFM
+            overall = Delft3DFM()           
+        overall.type = overall_str
+
     if overall.type.lower() == "delft3dfm":
 
         if detail.type.lower() == "delft3dfm":
             nest2_delft3dfm_in_delft3dfm(overall,
                                          detail,
                                          output_path,
                                          output_file,
@@ -50,20 +74,22 @@
                                       output_file,
                                       boundary_water_level_correction,
                                       option)
             
     elif overall.type.lower() == "sfincs":
 
         if detail.type.lower() == "sfincs":
-            zs = nest2_sfincs_in_sfincs(overall,
+            zs = nest2_sfincs_in_sfincs(overall,    
                                         detail,
                                         output_path,
                                         output_file,
                                         boundary_water_level_correction,
-                                        return_maximum=return_maximum)
+                                        return_maximum=return_maximum,
+                                        bc_path=bc_path,
+                                        ensemble_member_index=ensemble_member_index)
             return zs
         elif detail.type.lower() == "xbeach":
             bc = nest2_xbeach_in_sfincs(overall,
                                         detail,
                                         output_path,
                                         output_file,
                                         boundary_water_level_correction,
@@ -107,15 +133,16 @@
 
         if detail.type.lower() == "sfincs":
             nest2_sfincs_in_beware(overall,
                                    detail,
                                    output_path,
                                    output_file,
                                    boundary_water_level_correction,
-                                   option)
+                                   option,
+                                   bc_path)
 
 def nest2_delft3dfm_in_delft3dfm(overall,
                                  detail,
                                  output_path,
                                  output_file,
                                  boundary_water_level_correction):
 
@@ -247,15 +274,17 @@
 
 
 def nest2_sfincs_in_sfincs(overall,
                            detail,
                            output_path,
                            output_file,
                            boundary_water_level_correction,
-                           return_maximum=False):
+                           return_maximum=False,
+                           ensemble_member_index=None,
+                           bc_path=None):
 
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
     
         
     if overall.input.outputformat[0:3] == "bin":
@@ -270,34 +299,43 @@
     point_names = []
     for point in detail.flow_boundary_point:
         point_names.append(detail.name + "_" + point.name)                    
     zstfile = os.path.join(output_path, output_file)
 
     # Return DataFrame bzs
     bzs = overall.read_timeseries_output(name_list=point_names,
-                                         file_name=zstfile)
-
+                                         file_name=zstfile,
+                                         ensemble_member_index=ensemble_member_index)
     ts  = bzs.index
+    
+    # Astro correction
+    vcor = 0.0
+    if detail.input.corfile:        
+        vcor = get_vcor(os.path.join(detail.path, detail.input.corfile), ts)
+
     for icol, point in enumerate(detail.flow_boundary_point):
-        point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction
+        point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction + vcor
+
+    # Write bzs file
+    if bc_path is not None:
+        detail.write_flow_boundary_conditions(file_name=os.path.join(bc_path, detail.input.bzsfile))
 
+    # Why do we need this?
     if return_maximum:
         zmax = -999.0
         for icol, point in enumerate(detail.flow_boundary_point):
             zx = point.data.max()
             if zx>zmax:
                 zs = point.data
                 zmax = zx
-        return zs        
-                    
+        return zs                            
     else:    
         return detail.flow_boundary_point
 
 
-
 def nest2_xbeach_in_sfincs(overall,
                            detail,
                            output_path,
                            output_file,
                            boundary_water_level_correction,
                            return_maximum=False):
 
@@ -319,21 +357,19 @@
         point_names.append(detail.name + "_" + point.name)                    
     zstfile = os.path.join(output_path, output_file)
 
     # Return DataFrame bzs
     bzs = overall.read_timeseries_output(name_list=point_names,
                                          file_name=zstfile)
 
-    
     # Interpolate on desired format for XBeach forcing
     bzs_resampled = bzs.resample('10min').mean()
     bzs_interpolated = bzs_resampled.interpolate(method='linear')
     bzs_filtered = bzs_interpolated[detail.tref:detail.tstop]
     
-
     ts  = bzs_filtered.index
     for icol, point in enumerate(detail.flow_boundary_point):
         point.data = pd.Series(bzs_filtered.iloc[:,icol].values, index=ts) + boundary_water_level_correction
 
     if return_maximum:
         zmax = -999.0
         if len(detail.flow_boundary_point) <= 2:
@@ -720,15 +756,16 @@
 
 
 def nest2_sfincs_in_beware(overall,
                            detail,
                            output_path,
                            output_file,
                            boundary_water_level_correction,
-                           option):
+                           option,
+                           bc_path):
 
     from cht.sfincs.sfincs import FlowBoundaryPoint
     from cht.sfincs.sfincs import WaveMakerForcingPoint
 
     # Get bounding box for sfincs model
     # Convert bbox to beware crs
     x_range, y_range = detail.bounding_box(crs=overall.crs)
@@ -741,26 +778,25 @@
     
     # Read BEWARE offshore locations
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
     if not output_file:
-        output_file = "BW_output.nc"
-
+        output_file = "beware_his.nc"
     file_name = os.path.join(output_path, output_file)
 
     # Open netcdf file
     ddd = xr.open_dataset(file_name)
     
     if option == "flow":
     
         xb = ddd.x_off.values
         yb = ddd.y_off.values
-        
+
         # Find beware locations in bounding box
         inear = np.where((xb>x_range[0]) & (xb<x_range[1]) & (yb>y_range[0]) & (yb<y_range[1]))    
         xb=xb[inear]
         yb=yb[inear]
         nb = xb.size
         
         # Clear existing flow boundary points
@@ -779,32 +815,34 @@
                                       name=name)
             detail.flow_boundary_point.append(point)
         
         # Extract data and set water level boundary conditions
         tref = datetime.datetime(1970,1,1)
         tsec = ddd.time.values # array of int64
         times = tref + tsec*datetime.timedelta(seconds=1)
-        
         for ip, point in enumerate(detail.flow_boundary_point):
-            point.data = pd.Series(ddd.WL.values[inear[0][ip],:], index=times) + boundary_water_level_correction
+            point.data = pd.Series(ddd.R2_set.values[inear[0][ip],:], index=times) + pd.Series(ddd.R2_wl.values[inear[0][ip],:], index=times) + boundary_water_level_correction
 
     elif option == "wave":
 
         xb = ddd.x_coast.values
         yb = ddd.y_coast.values
-        
+
         # Find beware locations in bounding box
         inear = np.where((xb>x_range[0]) & (xb<x_range[1]) & (yb>y_range[0]) & (yb<y_range[1]))    
         xb=xb[inear]
         yb=yb[inear]
         nb = xb.size
-        
+
         # Clear existing flow boundary points
         detail.wavemaker_forcing_point = []
     
+        # Find wave boundary forcing at intersection wfp file and beware transects
+        # Load sfincs.wfp, find intersect with wfp and beware transect.
+
         # Convert to coordinate system of detail model
         transformer = Transformer.from_crs(overall.crs,
                                            detail.crs,
                                            always_xy=True)
         
         for ip in range(nb):
             name = str(ip + 1).zfill(4)        
@@ -818,21 +856,47 @@
         tref = datetime.datetime(1970,1,1)
         tsec = ddd.time.values # array of int64
         times = tref + tsec*datetime.timedelta(seconds=1)
         
         for ip, point in enumerate(detail.wavemaker_forcing_point):
 
             df = pd.DataFrame()
-            df["hm0_ig"] = ddd.obs_hm0_ig.values[inear[0][ip],:]
-            df["tp_ig"]  = ddd.obs_tpig.values[inear[0][ip],:]
-            df["setup"]  = ddd.obs_setup.values[inear[0][ip],:]
+            df["hm0_ig"] = ddd.hm0_ig.values[inear[0][ip],:]
+            df["tp_ig"]  = ddd.tp_ig.values[inear[0][ip],:]
+            df["setup"]  = ddd.setup.values[inear[0][ip],:]
             df["time"]   = times
             df = df.set_index("time")
             
             df["hm0_ig"]=df["hm0_ig"].replace(np.nan, 0.1)
             df["tp_ig"]=df["tp_ig"].replace(np.nan, 60.0)
             df["setup"]=df["setup"].replace(np.nan, 0.0)
             
             point.data = df
 
     ddd.close()
+
+    if bc_path is not None:
+        detail.write_whi_file(file_name=os.path.join(bc_path, detail.input.whifile))
+        detail.write_wti_file(file_name=os.path.join(bc_path, detail.input.wtifile))
+
+
+def get_vcor(corfile, times):
+    # Add astronomic correction to time series        
+    # Read cor file
+#        corfile = os.path.join(detail.path, detail.input.corfile)
+    d = IniStruct(filename=corfile)
+    astro = d.section[0].data
+#    times = self.domain.flow_boundary_point[0].data.index
+    names = []
+    amp   = []
+    phi   = []        
+    for icmp, cmp in enumerate(astro.index):                
+        names.append(cmp)
+        amp.append(astro[1][icmp])
+        phi.append(astro[2][icmp])        
+    df = pd.DataFrame()
+    df["component"] = pd.Series(names) 
+    df["amplitude"] = pd.Series(amp) 
+    df["phase"]     = pd.Series(phi) 
+    df = df.set_index("component")
+    return predict(df, times)
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/nesting/nesting.py` & `coastalhazardstoolkit-0.2.0/src/cht/nesting/nesting.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
 
 def nest2(overall,
           detail,
           boundary_water_level_correction=None,
           output_path=None,
           output_file=None,
 	      option=None,
-          return_maximum = False):
+          return_maximum=False,
+          bc_file=None):
 
 
     if not boundary_water_level_correction:
         # Path of the overall output time series
         boundary_water_level_correction = 0.0
     
     if overall.type.lower() == "delft3dfm":
@@ -121,15 +122,17 @@
 
     elif overall.type.lower() == "hurrywave":
 
         if detail.type.lower() == "hurrywave":
             nest2_hurrywave_in_hurrywave(overall,
                                    detail,
                                    output_path,
-                                   output_file)
+                                   output_file,
+                                   bc_file)
+            pass
         elif detail.type.lower() == "xbeach":
             bc = nest2_xbeach_in_hurrywave(overall,
                                            detail,
                                            output_path,
                                            output_file,
                                            option,
                                            return_maximum=return_maximum)
@@ -244,66 +247,65 @@
         overall.add_observation_point(x, y, name)
 
 def nest1_hurrywave_in_hurrywave(overall, detail):
     
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
                                        always_xy=True)
-    
-    for ind, point in enumerate(detail.boundary_point):
 
+    for ind, row in detail.boundary_conditions.gdf.iterrows():
         name = detail.name + "_" + str(ind + 1).zfill(4)
-        x, y = transformer.transform(point.geometry.x,
-                                     point.geometry.y)
-#        obs_list.append(obspoint(x, y, name, crs=overall.crs))
-        overall.add_observation_point_sp2(x, y, name)
+        x = row["geometry"].coords[0][0]
+        y = row["geometry"].coords[0][1]
+        x, y = transformer.transform(x, y)
+        overall.observation_points_sp2.add_point(x, y, name)
 
 def nest1_xbeach_in_hurrywave(overall, detail, option="sp2"):
     
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
                                        always_xy=True)
     
     for ind, point in enumerate(detail.wave_boundary_point):
 
         name = detail.name + "_" + str(ind + 1).zfill(4)
         x, y = transformer.transform(point.geometry.x,
                                      point.geometry.y)
 #        obs_list.append(obspoint(x, y, name, crs=overall.crs))
 #        if option=="sp2":
-        overall.add_observation_point_sp2(x, y, name)
+        overall.observation_points_sp2.add_point(x, y, name)
 #        else:
-        overall.add_observation_point(x, y, name)
+        overall.observation_points_regular.add_point(x, y, name)
 
 def nest1_sfincs_in_hurrywave(overall, detail):
     
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
                                        always_xy=True)
 
     for ind, point in enumerate(detail.wave_boundary_point):
 
         name = detail.name + "_" + str(ind + 1).zfill(4)
         x, y = transformer.transform(point.geometry.x,
                                      point.geometry.y)
-        overall.add_observation_point(x, y, name)
+        overall.observation_points_regular.add_point(x, y, name)
 
 def nest1_beware_in_hurrywave(overall, detail):
     
     transformer = Transformer.from_crs(detail.crs,
                                        overall.crs,
                                        always_xy=True)
 
     for ind, point in enumerate(detail.wave_boundary_point):
 
         
         name = detail.name + "_" + point.name
         x, y = transformer.transform(point.geometry.x,
                                      point.geometry.y)
-        overall.add_observation_point(x, y, name)
+        overall.observation_points_regular.add_point(x, y, name)
 
             
 def nest2_delft3dfm_in_delft3dfm(overall,
                                  detail,
                                  output_path,
                                  output_file,
                                  boundary_water_level_correction):
@@ -564,37 +566,40 @@
             point.data = pd.Series(bzs.iloc[:,icol].values, index=bzs.index) + boundary_water_level_correction    
             
 
     
 def nest2_hurrywave_in_hurrywave(overall,
                                  detail,
                                  output_path,
-                                 output_file):
+                                 output_file,
+                                 bc_file):
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
     if not output_file:
         output_file = "hurrywave_sp2.nc"
 
     file_name = os.path.join(output_path, output_file)
+    
+    detail.boundary_conditions.forcing = "spectra"
 
     # Open netcdf file
     ddd = xr.open_dataset(file_name)
     stations=ddd.station_name.values
     all_stations = []
     for ist, st in enumerate(stations):
         st=str(st.strip())[2:-1]
         all_stations.append(st)
 
-    point_names = []    
-    if detail.boundary_point:
+    point_names = []
+    if len(detail.boundary_conditions.gdf)>0:
+        for ind, row in detail.boundary_conditions.gdf.iterrows():
         # Find required boundary points        
-        for point in detail.boundary_point:
-            point_names.append(detail.name + "_" + point.name)                    
+            point_names.append(detail.name + "_" + row["name"])                    
         
     else:
         point_names = all_stations.copy()
         
     times   = ddd.point_spectrum2d.coords["time"].values
     sigma   = ddd.point_spectrum2d.coords["sigma"].values
     theta   = ddd.point_spectrum2d.coords["theta"].values
@@ -602,39 +607,28 @@
     ireq = []    
     for ip, point in enumerate(point_names):
         for ist,st in enumerate(all_stations):
             if point.lower() == st.lower():
                 ireq.append(ist)            
                 break
 
-    for ip, point in enumerate(detail.boundary_point):
+    for ind, row in detail.boundary_conditions.gdf.iterrows():
 
-        sp2 = ddd.point_spectrum2d.values[:,ireq[ip],:,:]
+        sp2 = ddd.point_spectrum2d.values[:,ireq[ind],:,:]
 
         ds = xr.Dataset(
                 data_vars = dict(point_spectrum2d=(["time", "theta", "sigma"], sp2)),
                 coords    = dict(time=times,
                                  theta=theta,
                                  sigma=sigma)
                 )
-        
-        point.data = ds
-            
-    # point_names = []
-    # for point in detail.flow_boundary_point:
-    #     point_names.append(detail.name + "_" + point.name)                    
-    # zstfile = os.path.join(output_path, output_file)
-
-    # # Return DataFrame bzs
-    # bzs = overall.read_timeseries_output(name_list=point_names,
-    #                                      file_name=zstfile)
-
-    # ts  = bzs.index
-    # for icol, point in enumerate(detail.flow_boundary_point):
-    #     point.data = pd.Series(bzs.iloc[:,icol].values, index=ts) + boundary_water_level_correction
+        detail.boundary_conditions.gdf.loc[ind, "spectra"] = ds.to_array()
+
+    if bc_file is not None:
+        detail.boundary_conditions.write_boundary_conditions_spectra(file_name=bc_file)
      
 def nest2_xbeach_in_hurrywave(overall,
                               detail,
                               output_path,
                               output_file,
                               option,
                               return_maximum=False):
@@ -900,15 +894,15 @@
     
     # Read BEWARE offshore locations
     if not output_path:
         # Path of the overall output time series
         output_path = overall.path
         
     if not output_file:
-        output_file = "BW_output.nc"
+        output_file = "beware_his.nc"
 
     file_name = os.path.join(output_path, output_file)
 
     # Open netcdf file
     ddd = xr.open_dataset(file_name)
     
     if option == "flow":
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/observation_stations/_noaa_coops.py` & `coastalhazardstoolkit-0.2.0/src/cht/observation_stations/_noaa_coops.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/physics/deshoal.py` & `coastalhazardstoolkit-0.2.0/src/cht/physics/deshoal.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/physics/disper.py` & `coastalhazardstoolkit-0.2.0/src/cht/physics/disper.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/physics/vo21.py` & `coastalhazardstoolkit-0.2.0/src/cht/physics/vo21.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/sfincs/quadtree.py` & `coastalhazardstoolkit-0.2.0/src/cht/sfincs/quadtree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Apr 21 17:24:49 2022
 
 @author: ormondt
 """
 import time
+import os
 import numpy as np
 from matplotlib import path
 # import matplotlib.pyplot as plt
 from pyproj import CRS, Transformer
 
 from cht.misc.misc_tools import interp2
 
@@ -432,14 +433,24 @@
         self.md2 = np.fromfile(file, dtype="i4", count=self.nr_cells) - 1
         self.z   = np.fromfile(file, dtype="f4", count=self.nr_cells)
         
         file.close()
         
         self.compute_cell_centre_coordinates()
 
+        # First indices of levels
+        ilast = -1
+        self.level_index = []
+        for j in range(self.nr_cells):
+#            print(j)
+            if self.level[j] > ilast:
+                self.level_index.append(j)
+                ilast = ilast + 1
+
+
     def save(self, file_name, version=0):
         
         file = open(file_name, "wb")
         
         # File version        
         file.write(np.int8(version))
 
@@ -1340,15 +1351,153 @@
             ilev = self.level[ic]
             if ilev>last_lev:
                 # Found new level
                 self.ifirst[ilev] = ic
                 last_lev = ilev
     
         self.find_neighbors()
+
+
+    def make_index_tiles(self, path, zoom_range=None, format=0):
+        
+        import math
+        from cht.tiling.tiling import deg2num
+        from cht.tiling.tiling import num2deg
+        import cht.misc.fileops as fo
+        
+        npix = 256
+        
+        if not zoom_range:
+            zoom_range = [0, 13]
+
+        cosrot = math.cos(-self.rotation*math.pi/180)
+        sinrot = math.sin(-self.rotation*math.pi/180)       
+
+        # Compute lon/lat range
+        xmin = np.amin(self.x) - 10*self.dx
+        xmax = np.amax(self.x) + 10*self.dx
+        ymin = np.amin(self.y) - 10*self.dy
+        ymax = np.amax(self.y) + 10*self.dy
+        transformer = Transformer.from_crs(self.crs,
+                                            CRS.from_epsg(4326),
+                                            always_xy=True)
+        lon_min, lat_min = transformer.transform(xmin, ymin)
+        lon_max, lat_max = transformer.transform(xmax, ymax)
+        lon_range = [lon_min, lon_max]
+        lat_range = [lat_min, lat_max]        
+        
+        transformer_a = Transformer.from_crs(CRS.from_epsg(4326),
+                                                CRS.from_epsg(3857),
+                                                always_xy=True)
+        transformer_b = Transformer.from_crs(CRS.from_epsg(3857),
+                                                self.crs,
+                                                always_xy=True)
+        
+        i0_lev = []
+        i1_lev = []
+        nmax_lev = []
+        mmax_lev = []
+        nm_lev = []
+        for level in range(self.nr_refinement_levels):
+            i0 = self.level_index[level]
+            if level<self.nr_refinement_levels - 1:
+                i1 = self.level_index[level + 1]
+            else:
+                i1 = self.nr_cells   
+            i0_lev.append(i0)    
+            i1_lev.append(i1)    
+            nmax_lev.append(np.amax(self.n[i0:i1]) + 1)
+            mmax_lev.append(np.amax(self.m[i0:i1]) + 1)
+            mm = self.m[i0:i1]
+            nn = self.n[i0:i1]
+            nm_lev.append(mm*nmax_lev[level] + nn)
+
+        for izoom in range(zoom_range[0], zoom_range[1] + 1):
+            
+            print("Processing zoom level " + str(izoom))
+        
+            zoom_path = os.path.join(path, str(izoom))
+        
+            dxy = (40075016.686/npix) / 2 ** izoom
+            xx = np.linspace(0.0, (npix - 1)*dxy, num=npix)
+            yy = xx[:]
+            xv, yv = np.meshgrid(xx, yy)
+        
+            ix0, iy0 = deg2num(lat_range[0], lon_range[0], izoom)
+            ix1, iy1 = deg2num(lat_range[1], lon_range[1], izoom)
         
+            for i in range(ix0, ix1 + 1):
+            
+                path_okay = False
+                zoom_path_i = os.path.join(zoom_path, str(i))
+            
+                for j in range(iy0, iy1 + 1):
+            
+                    file_name = os.path.join(zoom_path_i, str(j) + ".dat")
+            
+                    # Compute lat/lon at ll corner of tile
+                    lat, lon = num2deg(i, j, izoom)
+            
+                    # Convert to Global Mercator
+                    xo, yo   = transformer_a.transform(lon,lat)
+            
+                    # Tile grid on local mercator
+                    x = xv[:] + xo + 0.5*dxy
+                    y = yv[:] + yo + 0.5*dxy
+            
+                    # Convert tile grid to crs of SFINCS model
+                    x, y = transformer_b.transform(x, y)
+
+                    # Now rotate around origin of SFINCS model
+                    x00 = x - self.x0
+                    y00 = y - self.y0
+                    xg  = x00*cosrot - y00*sinrot
+                    yg  = x00*sinrot + y00*cosrot
+
+                    indx = np.full((npix, npix), -999, dtype=int)
+
+                    for ilev in range(self.nr_refinement_levels):
+                        nmax = nmax_lev[ilev]
+                        mmax = mmax_lev[ilev]
+                        i0   = i0_lev[ilev]
+                        i1   = i1_lev[ilev]
+                        dx   = self.dx/2**ilev
+                        dy   = self.dy/2**ilev
+                        iind = np.floor(xg/dx).astype(int)
+                        jind = np.floor(yg/dy).astype(int)
+                        # Now check whether this cell exists on this level
+                        ind  = iind*nmax + jind
+                        ind[iind<0]   = -999
+                        ind[jind<0]   = -999
+                        ind[iind>=mmax] = -999
+                        ind[jind>=nmax] = -999
+
+                        ingrid = np.isin(ind, nm_lev[ilev], assume_unique=False) # return boolean for each pixel that falls inside a grid cell
+                        incell = np.where(ingrid)                                # tuple of arrays of pixel indices that fall in a cell
+
+                        if incell[0].size>0:
+                            # Now find the cell indices
+                            try:
+                                cell_indices = np.searchsorted(nm_lev[ilev], ind[incell[0], incell[1]]) + i0_lev[ilev]
+                                indx[incell[0], incell[1]] = cell_indices
+                            except:
+                                pass
+
+                    if np.any(indx>=0):                        
+                        if not path_okay:
+                            if not os.path.exists(zoom_path_i):
+                                fo.mkdir(zoom_path_i)
+                                path_okay = True
+                                
+                        # And write indices to file
+                        fid = open(file_name, "wb")
+                        fid.write(indx)
+                        fid.close()
+
+
 def get_neighbors_in_larger_cell(n, m):
     
     nnbr = [-1, -1, -1, -1]
     mnbr = [-1, -1, -1, -1]
 
     if not odd(n) and not odd(m):
         # lower left
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/sfincs/regulargrid.py` & `coastalhazardstoolkit-0.2.0/src/cht/sfincs/regulargrid.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/sfincs/sfincs.py` & `coastalhazardstoolkit-0.2.0/src/cht/sfincs/sfincs.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,18 @@
 #        self.grid = SfincsGrid()
 
         # Flow boundary conditions
         self.read_flow_boundary_points()
         self.read_flow_boundary_conditions()
         self.read_astro_boundary_conditions()
 
+        # Wave boundary conditions
+        self.read_wave_boundary_points()
+        # self.read_wave_boundary_conditions()
+
         # Observation points
         self.read_observation_points()
 
 #        self.grid.compute_coordinates(x0,y0,dx,dy,nx,ny,rotation)
     
     def read_index_file(self):
         pass
@@ -302,19 +306,19 @@
 
     def read_wave_boundary_points(self):
         
         # Read SFINCS bnd file
         
         self.wave_boundary_point = []
         
-        if not self.input.bwvfile:
+        if not self.input.snapwave_bndfile:
             return
                     
         bnd_file = os.path.join(self.path,
-                                self.input.bwvfile)
+                                self.input.snapwave_bndfile)
 
         if not os.path.exists(bnd_file):
             return
         
         # Read the bnd file
         df = pd.read_csv(bnd_file, index_col=False, header=None,
              delim_whitespace=True, names=['x', 'y'])
@@ -327,18 +331,18 @@
                                       name=name)
             self.wave_boundary_point.append(point)
 
     def write_wave_boundary_points(self, file_name=None):
 
         # Write SFINCS bnd file
         if not file_name:
-            if not self.input.bwvfile:
+            if not self.input.snapwave_bndfile:
                 return
             file_name = os.path.join(self.path,
-                                     self.input.bwvfile)
+                                     self.input.snapwave_bndfile)
             
         if not file_name:
             return
             
         fid = open(file_name, "w")
         for point in self.wave_boundary_point:
             string = f'{point.geometry.x:12.1f}{point.geometry.y:12.1f}\n'
@@ -378,72 +382,72 @@
         self.write_wti_file()
         self.write_wst_file()
 
             
     def write_bhs_file(self, file_name=None):
         # Hm0
         if not file_name:
-            if not self.input.bhsfile:
+            if not self.input.snapwave_bhsfile:
                 return
             file_name = os.path.join(self.path,
-                                      self.input.bhsfile)
+                                      self.input.snapwave_bhsfile)
         df = pd.DataFrame()
         for point in self.wave_boundary_point:
             df = pd.concat([df, point.data["hm0"]], axis=1)
         tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.3f")
 
     def write_btp_file(self, file_name=None):
         # Tp
         if not file_name:
-            if not self.input.btpfile:
+            if not self.input.snapwave_btpfile:
                 return
             file_name = os.path.join(self.path,
-                                      self.input.btpfile)
+                                      self.input.snapwave_btpfile)
         df = pd.DataFrame()
         for point in self.wave_boundary_point:
             df = pd.concat([df, point.data["tp"]], axis=1)
         tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.1f")
 
     def write_bwd_file(self, file_name=None):
         # WavDir
         if not file_name:
-            if not self.input.bwdfile:
+            if not self.input.snapwave_bwdfile:
                 return
             file_name = os.path.join(self.path,
-                                      self.input.bwdfile)
+                                      self.input.snapwave_bwdfile)
         df = pd.DataFrame()
         for point in self.wave_boundary_point:
             df = pd.concat([df, point.data["wavdir"]], axis=1)
         tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
                   sep=" ",
                   header=False,
                   float_format="%0.1f")
 
     def write_bds_file(self, file_name=None):
         # DirSpr
         if not file_name:
-            if not self.input.bdsfile:
+            if not self.input.snapwave_bdsfile:
                 return
             file_name = os.path.join(self.path,
-                                      self.input.bdsfile)
+                                      self.input.snapwave_bdsfile)
         df = pd.DataFrame()
         for point in self.wave_boundary_point:
             df = pd.concat([df, point.data["dirspr"]], axis=1)
         tmsec = pd.to_timedelta(df.index.values - self.input.tref, unit="s")
         df.index = tmsec.total_seconds()
         df.to_csv(file_name,
                   index=True,
@@ -558,23 +562,34 @@
                 string = f'{point.geometry.x:12.6f}{point.geometry.y:12.6f}  "{point.name}"\n'
                 fid.write(string)
             fid.close()
         
             
     ### Output ###
 
-    def read_timeseries_output(self, name_list = None, file_name = None):
-    
+    def read_timeseries_output(self,
+                               name_list=None,
+                               file_name=None,
+                               parameter="point_zs",
+                               path=None,
+                               ensemble_member_index=None):
+
+        if path is None:
+            if hasattr(self, "path"):
+                path = self.path
+            else:
+                path = os.getcwd()
+
         # Returns a dataframe with timeseries
         if self.input.outputformat[0:3] == "bin":
             
             # ASCII output
     
             if not file_name:
-                file_name = os.path.join(self.path, "zst.txt")
+                file_name = os.path.join(path, "zst.txt")
         
             if not self.observation_point:
                 # First read observation points
                 self.read_observation_points()
             
             columns = []
             for point in self.observation_point:
@@ -588,51 +603,63 @@
             if name_list:
                 df = df[name_list]
             
         else:
             
             # NetCDF output
             if not file_name:
-                file_name = os.path.join(self.path, "sfincs_his.nc")
+                file_name = "sfincs_his.nc"
+
+            # Check if file_name has a path
+            if not os.path.dirname(file_name):
+                # file_name has no path 
+                file_name = os.path.join(path, file_name)
                     
             # Open netcdf file
             ddd = xr.open_dataset(file_name)
 #            stations=ddd.point_zs.coords["station_name"].values
             stations=ddd.station_name.values
             all_stations = []
             for ist, st in enumerate(stations):
 #                st=str(st)[2:-1]
                 all_stations.append(st.decode().strip())
             
-            times   = ddd.point_zs.coords["time"].values
+
+            times   = ddd[parameter].coords["time"].values
     
             # If name_list is empty, add all points    
             if not name_list:
                 name_list = []
                 for st in all_stations:
                     name_list.append(st)
             
             df = pd.DataFrame(index=times, columns=name_list)
-            
+
             for station in name_list:
                 for ist, st in enumerate(all_stations):
                     if station == st:
-                        wl = ddd.point_zs.values[:,ist]
+                        if ensemble_member_index is None:
+                            wl = ddd[parameter].values[:,ist]
+                        else:
+                            wl = ddd[parameter].values[:,ist,ensemble_member_index]    
                         wl[np.isnan(wl)] = -999.0
                         df[st]=wl
                         break            
     
             ddd.close()
                     
         return df    
 
-    def read_zsmax(self, time_range=None, zsmax_file=None, output="grid"):
+    def read_zsmax(self, time_range=None, zsmax_file=None, output="grid", varname='zsmax'):
     
         if not zsmax_file:
-            zsmax_file = os.path.join(self.path, "zsmax.dat")
+            if self.input.outputformat[0:3] == "net":
+                zsmax_file = os.path.join(self.path, "sfincs_map.nc")
+            else:
+                zsmax_file = os.path.join(self.path, "zsmax.dat")
             
 
         if self.input.outputformat[0:3] == "net":
 #            ddd=xr.open_dataset(zsmax_file)
 #            zsmx=ddd.zsmax.values
 #            zsmax=np.transpose(np.nanmax(ddd.zsmax.values, axis=0))
             
@@ -648,16 +675,20 @@
             it0 = -1
             for it, time in enumerate(output_times):
                 time = pd.to_datetime(str(time)).replace(tzinfo=None).to_pydatetime()
                 if time>=time_range[0] and it0<0:
                     it0 = it
                 if time<=time_range[1]:
                     it1 = it
-            
-            zsmax = np.transpose(np.nanmax(dsin.zsmax.values[it0:it1 + 1,:,:], axis=0))
+
+            if self.input.qtrfile:
+                zsmax = np.nanmax(dsin[varname].values[it0:it1 + 1,:], axis=0)
+            else:                
+                zsmax = np.transpose(np.nanmax(dsin[varname].values[it0:it1 + 1,:,:], axis=0))
+                zsmax = np.nanmax(dsin[varname].values[it0:it1 + 1,:,:], axis=0)
             dsin.close()
 
             return zsmax
 
 
 
         else:
@@ -887,15 +918,22 @@
             xg, yg = transformer.transform(xg, yg)
         
         xp = [ xg[0,0], xg[0,-1], xg[-1,-1], xg[-1,0], xg[0,0] ]
         yp = [ yg[0,0], yg[0,-1], yg[-1,-1], yg[-1,0], yg[0,0] ]
         
         return xp, yp
         
-    def make_index_tiles(self, path, zoom_range=None):
+    def make_index_tiles(self, path, zoom_range=None, format=0):
+
+        if self.input.qtrfile:
+            from .quadtree import QuadtreeGrid
+            quadtree = QuadtreeGrid(crs=self.crs) 
+            quadtree.load(os.path.join(self.path, self.input.qtrfile))
+            quadtree.make_index_tiles(path, zoom_range=zoom_range)
+            return
         
         from cht.tiling.tiling import deg2num
         from cht.tiling.tiling import num2deg
         import cht.misc.fileops as fo
         
         if not zoom_range:
             zoom_range = [0, 13]
@@ -1001,20 +1039,21 @@
         self.nmax = 0
         self.dx   = 10.0
         self.dy   = 10.0
         self.x0   = 0.0
         self.y0   = 0.0
         self.rotation = 0.0
         self.latitude = 0.0
-        self.tref=None
-        self.tstart=None
-        self.tstop=None
+        tnow = datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)
+        self.tref=tnow
+        self.tstart=tnow
+        self.tstop=tnow + datetime.timedelta(days=1)
         self.tspinup=60.0
         self.t0out=None
-        self.dtmapout=600.0
+        self.dtmapout=3600.0
         self.dthisout=600.0
         self.dtrstout=0.0
         self.dtmaxout=0.0
         self.trstout=-999.0
         self.dtwnd=1800.0
         self.alpha=0.5
         self.theta=1.0
@@ -1036,17 +1075,19 @@
         self.baro=0
         self.pavbnd=0
         self.gapres=101200.0
         self.advlim=9999.9
         self.stopdepth=1000.0
         self.crsgeo=0
         
+        self.qtrfile=None
         self.depfile=None
         self.mskfile=None
         self.indexfile=None
+        self.qtrfile=None
         self.cstfile=None
         self.bndfile=None
         self.bzsfile=None
         self.bzifile=None
         self.bwvfile=None
         self.bhsfile=None
 #        self.bhifile=None
@@ -1081,14 +1122,29 @@
         self.inputformat="bin"
         self.outputformat="net"
         
         self.cdnrb=3
         self.cdwnd=[0.0,28.0,50.0]
         self.cdval=[0.001,0.0025,0.0015]
 
+        self.dtwave=None
+        self.snapwave=None
+        self.snapwave_gamma=None
+        self.snapwave_dtheta=None
+        self.snapwave_hmin=None
+        self.snapwave_fw0=None
+        self.snapwave_crit=None
+        self.snapwave_igwaves=None
+        self.snapwave_nrsweeps=None
+        self.snapwave_bhsfile=None
+        self.snapwave_btpfile=None
+        self.snapwave_bwdfile=None
+        self.snapwave_bdsfile=None
+        self.snapwave_encfile=None
+        self.snapwave_bndfile=None
 
 class SfincsGrid():
 
     def __init__(self, x0, y0, dx, dy, nx, ny, rotation):
         self.geometry = RegularGrid(x0, y0, dx, dy, nx, ny, rotation)
 
     # def plot(self,ax):
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/sfincs/sfincs_builder.py` & `coastalhazardstoolkit-0.2.0/src/cht/sfincs2/sfincs_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,23 +64,23 @@
             # Compute latitude   
         sf.input.crs_epsg = crs.to_epsg()
         
         # Set input parameters in sf.input
         for key in self.setup_config["input"]:
             setattr(sf.input, key, self.setup_config["input"][key])
 
-        # Copy other files to input folder
-        if os.path.exists(os.path.join(self.data_path, "sfincs.bnd")):
-            fo.copy_file(os.path.join(self.data_path, "sfincs.bnd"),
-                        self.model_path)
-            sf.input.bndfile = "sfincs.bnd"
-        if os.path.exists(os.path.join(self.data_path, "sfincs.bca")):
-            fo.copy_file(os.path.join(self.data_path, "sfincs.bca"),
-                        self.model_path)
-            sf.input.bcafile = "sfincs.bca"
+        # # Copy other files to input folder
+        # if os.path.exists(os.path.join(self.data_path, "sfincs.bnd")):
+        #     fo.copy_file(os.path.join(self.data_path, "sfincs.bnd"),
+        #                 self.model_path)
+        #     sf.input.bndfile = "sfincs.bnd"
+        # if os.path.exists(os.path.join(self.data_path, "sfincs.bca")):
+        #     fo.copy_file(os.path.join(self.data_path, "sfincs.bca"),
+        #                 self.model_path)
+        #     sf.input.bcafile = "sfincs.bca"
             
         # Check if quadtree needs to be built (may also be regular grid)
         
         if self.setup_config["quadtree"]:
             # Quadtree not empty
             
             # This is the default (qtrfile=sfincs.qtr)
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/sfincs/subgrid.py` & `coastalhazardstoolkit-0.2.0/src/cht/sfincs/subgrid.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/snapwave/mesh.py` & `coastalhazardstoolkit-0.2.0/src/cht/snapwave/mesh.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tide/astro.py` & `coastalhazardstoolkit-0.2.0/src/cht/tide/astro.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tide/constituent.py` & `coastalhazardstoolkit-0.2.0/src/cht/tide/constituent.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tide/nodal_corrections.py` & `coastalhazardstoolkit-0.2.0/src/cht/tide/nodal_corrections.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tide/tide.py` & `coastalhazardstoolkit-0.2.0/src/cht/tide/tide.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
 		Partition a sorted list of numbers (or in this case hours).
 		Arguments:
 		hours -- sorted ndarray of hours.
 		partition -- maximum partition length (default: 3600.0)
 		"""
 		partition = float(partition)
 		relative = hours - hours[0]
-		total_partitions = np.ceil(relative[-1] / partition + 10*np.finfo(np.float).eps).astype('int')
+		total_partitions = np.ceil(relative[-1] / partition + 10*np.finfo(np.float64).eps).astype('int')
 		return [hours[np.floor(np.divide(relative, partition)) == i] for i in range(total_partitions)]
 
 	@staticmethod
 	def _times(t0, hours):
 		"""
 		Return a (list of) datetime(s) given an initial time and an (list of) hourly offset(s).
 		Arguments:
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tide/tide_predict.py` & `coastalhazardstoolkit-0.2.0/src/cht/tide/tide_predict.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tiling/tiling.py` & `coastalhazardstoolkit-0.2.0/src/cht/tiling/tiling.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     :type zoom_range: list of int
     
     """
     
     if type(valg) == list:
         pass
     else:
-        valg = valg.transpose().flatten()
+        valg = valg.flatten()
 
     if not caxis:
         caxis = []
         caxis.append(np.nanmin(valg))
         caxis.append(np.nanmax(valg))
     
     for izoom in range(zoom_range[0], zoom_range[1] + 1):
@@ -241,15 +241,15 @@
     :type zoom_range: list of int
     
     """
     
     if type(valg) == list:
         pass
     else:
-        valg = valg.transpose().flatten()
+        valg = valg.flatten()
 
     if not caxis:
         caxis = []
         caxis.append(np.nanmin(valg))
         caxis.append(np.nanmax(valg))
         
     # First do highest zoom level, then derefine from there    
@@ -311,14 +311,15 @@
                                           ifolder, str(j) + ".dat")
                 if not os.path.exists(bathy_file):
                     # No bathy for this tile, continue
                     continue
                 zb  = np.fromfile(bathy_file, dtype="f4")
                 
                 valt = valg[ind]                   
+                valt[np.where(ind<0)] = np.NaN                 
                 valt = valt - zb
                 valt[valt<0.05] = np.NaN
                 valt[zb<zbmax] = np.NaN
 
             if color_values:
                 
                 rgb = np.zeros((256*256,4),'uint8')                        
@@ -461,14 +462,167 @@
     #                        rgb[rgb==0] = rgb0[rgb==0]
                             im = Image.fromarray(rgb)
     #                        im.show()
         
                     im.save(png_file)            
     
 
+def make_floodmap_overlay(valg,
+                          index_path,
+                          topo_path,
+                          npixels=[1200, 800],
+                          lon_range=None,
+                          lat_range=None,  
+                          option="deterministic",
+                          color_values=None,
+                          caxis=None,
+                          zbmax=-999.0,
+                          merge=True,
+                          depth=None,
+                          quiet=False,
+                          file_name=None):
+    """
+    Generates overlay PNG from tiles
+    
+    :param valg: Name of the scenario to be run.
+    :type valg: array
+    :param index_path: Path where the index tiles are sitting.
+    :type index_path: str
+    :param png_path: Output path where the png tiles will be created.
+    :type png_path: str
+    :param option: Option to define the type of tiles to be generated. Options are 'direct', 'floodmap', 'topography'. Defaults to 'direct', in which case the values in *valg* are used directly.
+    :type option: str
+    :param zoom_range: Zoom range for which the png tiles will be created. Defaults to [0, 23].
+    :type zoom_range: list of int
+    
+    """
+    
+    if type(valg) == list:
+        pass
+    else:
+        valg = valg.transpose().flatten()
+
+    if not caxis:
+        caxis = []
+        caxis.append(np.nanmin(valg))
+        caxis.append(np.nanmax(valg))
+
+    # Check available levels in index tiles
+    max_zoom = 0
+    levs = fo.list_folders(os.path.join(index_path, "*"), basename=True)
+    for lev in levs:
+        max_zoom = max(max_zoom, int(lev))
+
+    # Find zoom level that provides sufficient pixels    
+    for izoom in range(max_zoom + 1):
+        ix0, iy0 = deg2num(lat_range[0], lon_range[0], izoom)
+        ix1, iy1 = deg2num(lat_range[1], lon_range[1], izoom)
+        if (ix1 - ix0 + 1)*256 > npixels[0] and (iy1 - iy0 + 1)*256 > npixels[1]:
+            # Found sufficient zoom level
+            break
+
+    index_zoom_path = os.path.join(index_path, str(izoom))
+        
+#    dxy = (40075016.686/npix) / 2 ** izoom
+#    xx = np.linspace(0.0, (256 - 1)*dxy, num=npix)
+#    yy = xx[:]
+#    xv, yv = np.meshgrid(xx, yy)
+
+    nx = (ix1 - ix0 + 1)*256
+    ny = (iy1 - iy0 + 1)*256
+    zz = np.empty((ny, nx))
+    zz[:] = np.nan
+
+    if not quiet:
+        print("Processing zoom level " + str(izoom))
+
+    index_zoom_path = os.path.join(index_path, str(izoom))
+
+    for i in range(ix0, ix1 + 1):
+        ifolder = str(i)
+        index_zoom_path_i = os.path.join(index_zoom_path, ifolder)
+
+        for j in range(iy0, iy1 + 1):
+
+            index_file = os.path.join(index_zoom_path_i, str(j) + ".dat")                           
+
+            if not os.path.exists(index_file):
+                continue
+            
+            ind = np.fromfile(index_file, dtype="i4")
+            
+            if option=="probabilistic":
+
+                # valg is actually CDF interpolator to obtain probability of water level
+
+                # Read bathy
+                bathy_file = os.path.join(topo_path, str(izoom),
+                                          ifolder, str(j) + ".dat")
+
+                if not os.path.exists(bathy_file):
+                    # No bathy for this tile, continue
+                    continue
+
+                zb  = np.fromfile(bathy_file, dtype="f4")
+                zs  = zb + depth
+                
+                valt = valg[ind](zs)
+                valt[ind<0] = np.NaN
+
+            else:
+
+                # Read bathy
+                bathy_file = os.path.join(topo_path, str(izoom),
+                                          ifolder, str(j) + ".dat")
+                if not os.path.exists(bathy_file):
+                    # No bathy for this tile, continue
+                    continue
+                zb  = np.fromfile(bathy_file, dtype="f4")
+                
+                valt = valg[ind]
+                valt[np.where(ind<0)] = np.NaN                 
+                valt = valt - zb
+                valt[valt<0.05] = np.NaN
+                valt[zb<zbmax] = np.NaN
+ 
+            ii0 = (i - ix0)*256
+            ii1 = ii0 + 256  
+            jj0 = (iy1 - j)*256
+            jj1 = jj0 + 256  
+            zz[jj0:jj1, ii0:ii1] = np.flipud(valt.reshape([256, 256]))
+
+
+    if color_values:
+        # Create empty rgb array        
+        zz = zz.flatten()
+        rgb = np.zeros((ny*nx,4),'uint8')
+        # Determine value based on user-defined ranges
+        for color_value in color_values:
+            inr = np.logical_and(zz>=color_value["lower_value"],
+                                 zz<color_value["upper_value"])
+            rgb[inr,0] = color_value["rgb"][0]
+            rgb[inr,1] = color_value["rgb"][1]
+            rgb[inr,2] = color_value["rgb"][2]
+            rgb[inr,3] = 255            
+        im = Image.fromarray(rgb.reshape([ny,nx,4]))
+
+    else:
+        zz = (zz - caxis[0]) / (caxis[1] - caxis[0])
+        zz[zz<0.0] = 0.0
+        zz[zz>1.0] = 1.0                    
+        im = Image.fromarray(cm.jet(zz, bytes=True))
+
+    if file_name:
+        im.save(file_name)
+
+    lat0, lon0 = num2deg_ll(ix0, iy0, izoom) # lat/lon coordinates of lower left cell
+    lat1, lon1 = num2deg_ur(ix1, iy1, izoom) # lat/lon coordinates of lower left cell
+    return [lon0, lon1], [lat0, lat1]    
+
+
 def make_topobathy_tiles(path, dem_names, lon_range, lat_range,
                          index_path=None,
                          zoom_range=None,
                          z_range=None,
                          bathymetry_database_path="d:\\delftdashboard\\data\\bathymetry",
                          quiet=False):
 
@@ -694,12 +848,29 @@
     lat_rad = math.radians(lat_deg)
     n = 2 ** zoom
     xtile = int((lon_deg + 180.0) / 360.0 * n) 
     ytile = int((1.0 - math.asinh(math.tan(-lat_rad)) / math.pi) / 2.0 * n)
     return (xtile, ytile)
 
 def num2deg(xtile, ytile, zoom):
+    # Return lower left corner of tile
     n = 2 ** zoom
     lon_deg = xtile / n * 360.0 - 180.0
     lat_rad = math.atan(math.sinh(math.pi * (1 - 2 * ytile / n)))
     lat_deg = math.degrees(-lat_rad)
     return (lat_deg, lon_deg)
+
+def num2deg_ll(xtile, ytile, zoom):
+    # Return lower left corner of tile
+    n = 2 ** zoom
+    lon_deg = xtile / n * 360.0 - 180.0
+    lat_rad = math.atan(math.sinh(math.pi * (1 - 2 * ytile / n)))
+    lat_deg = math.degrees(-lat_rad)
+    return (lat_deg, lon_deg)
+
+def num2deg_ur(xtile, ytile, zoom):
+    # Return upper_right corner of tile
+    n = 2 ** zoom
+    lon_deg = (xtile + 1) / n * 360.0 - 180.0
+    lat_rad = math.atan(math.sinh(math.pi * (1 - 2 * (ytile + 1) / n)))
+    lat_deg = math.degrees(-lat_rad)
+    return (lat_deg, lon_deg)
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tropical_cyclone/testje.py` & `coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/testje.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tropical_cyclone/testje_forecasting.py` & `coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/testje_forecasting.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/tropical_cyclone/tropical_cyclone.py` & `coastalhazardstoolkit-0.2.0/src/cht/tropical_cyclone/tropical_cyclone.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,17 @@
 """
 Tropical Cyclone Module in the Coastal Hazards Toolkit
 
 Module supports two classes
     TropicalCyclone:             deterministic simulations
     TropicalCycloneEnsemble      probablistic simulations using the simplified DeMaria et al. (2009) approach
 
-    
     To do list - priority
-        account for wind radii / rainfall in ensembles 
-        extract btd data from time-and-spatialying varying wind fields
         netcdf spiderwebs
 
-        
     To do list - 'nice to haves'
         make reading of ddb_cyc not file size related but using actual keywords (since format are changing)
         add more reading formats (e.g. NHC, JTWC, etc.)
         enable coordinate conversions; now it is all WGS 84
 """
 
 # Modules needed
@@ -26,212 +22,293 @@
 import pandas as pd
 import geopandas as gpd
 import matplotlib.pyplot as plt
 from datetime import datetime, timedelta
 from scipy.interpolate import interp1d, CubicSpline
 from scipy.ndimage.filters import uniform_filter1d
 from shapely.geometry import Point, LineString, MultiLineString, mapping
+import shapely
+from geojson import Feature, FeatureCollection
 
 # Settings
-dateformat_module   = "%Y%m%d %H%M%S"
-knots_to_ms         = float(0.51444)
-nm_to_km            = float(1.852)
-nm_to_m             = float(1.852)*1000
+dateformat_module = "%Y%m%d %H%M%S"
+knots_to_ms = float(0.51444)
+nm_to_km = float(1.852)
+nm_to_m = float(1.852) * 1000
 pd.options.mode.chained_assignment = None
 
+
 # Classes of the Tropical Cyclone module
 class TropicalCyclone:
-    
     # Init
-    def __init__(self,name=None):
-        
+    def __init__(self, name=None):
         # Header
-        self.name                       = name                    # name of the tropical cyclone
-        self.wind_profile               = 'holland2010'           # parametric wind profile: holland2010, holland2008, holland1980
-        self.wind_pressure_relation     = 'holland2008'           # relationship used to determine pressure or wind speed if one is unknown
-        self.rmw_relation               = 'nederhoff2019'         # relationship used to determine RMW (needed for most wind profiles)
-        self.background_pressure        = 1012.0                  # background pressure in Pa
-        self.phi_spiral                 = 20.0                    # phi spiral
-        self.wind_conversion_factor     = 0.93                    # conversion factor from 1-min to 10-minute winds (if needed)
-        self.spiderweb_radius           = 1000.0                  # radius in km
-        self.nr_radial_bins             = int(500)                # number of radial bins
-        self.nr_directional_bins        = int(36)                 # number of directional bins
-        self.debug                      = 0                       # do not show prints =0; change to 1 to show prints
-        
-        self.low_wind_speeds_cut_off    = 0.0                     # float that is used to trim the track when making spiderwebs  
-        self.rho_air                    = 1.15                    # used in the determination of parametric wind field
-        self.asymmetry_option           = 'schwerdt1979'          # asymmetry_options: schwerdt1979, mvo, none
-        self.reference_time             = datetime(1900,1,1)      # used when writing out spiderweb
-        self.include_rainfall           = False                   # logic: 0 is no and 1 is yes
-        self.rainfall_relationship      = 'ipet'                  # rainfall_relationship: ipet
+        self.name = name  # name of the tropical cyclone
+        self.wind_profile = "holland2010"  # parametric wind profile: holland2010, holland2008, holland1980
+        self.wind_pressure_relation = "holland2008"  # relationship used to determine pressure or wind speed if one is unknown
+        self.rmw_relation = "nederhoff2019"  # relationship used to determine RMW (needed for most wind profiles)
+        self.background_pressure = 1012.0  # background pressure in Pa
+        self.phi_spiral = 20.0  # phi spiral
+        self.wind_conversion_factor = (
+            0.93  # conversion factor from 1-min to 10-minute winds (if needed)
+        )
+        self.spiderweb_radius = 1000.0  # radius in km
+        self.nr_radial_bins = int(500)  # number of radial bins
+        self.nr_directional_bins = int(36)  # number of directional bins
+        self.debug = 0  # do not show prints =0; change to 1 to show prints
+
+        self.low_wind_speeds_cut_off = (
+            0.0  # float that is used to trim the track when making spiderwebs
+        )
+        self.extend_track = 0.0  # with certain amount of days
+        self.rho_air = 1.15  # used in the determination of parametric wind field
+        self.asymmetry_option = (
+            "schwerdt1979"  # asymmetry_options: schwerdt1979, mvo, none
+        )
+        self.reference_time = datetime(1970, 1, 1)  # used when writing out spiderweb
+        self.include_rainfall = False  # logic: 0 is no and 1 is yes
+        self.rainfall_relationship = "ipet"  # rainfall_relationship: ipet
+        self.rainfall_factor = 1.0  # factor to calibrate rainfall
 
         # New keywords to keep track of units in intensity, wind radii and coordinate system
-        self.unit_intensity             = 'knots'                 # float 
-        self.unit_radii                 = 'nm'                    # nm
-        self.EPSG                       = 4326
-        
+        self.unit_intensity = "knots"  # float
+        self.unit_radii = "nm"  # nm
+        self.EPSG = 4326
+
         # Track itself - create a dummy point
-        point                           = Point(0,0)
-        self.track  = gpd.GeoDataFrame({"datetime": [0], "geometry": [point] , "vmax": [0], "pc": [0], "RMW": [0],
-                                        "R35_NE": [0], "R35_SE": [0],"R35_SW": [0],"R35_NW": [0],
-                                        "R50_NE": [0], "R50_SE": [0],"R50_SW": [0],"R50_NW": [0],
-                                        "R65_NE": [0], "R65_SE": [0],"R65_SW": [0],"R65_NW": [0],
-                                        "R100_NE": [0], "R100_SE": [0],"R100_SW": [0],"R100_NW": [0]})        
+        point = Point(0, 0)
+        self.track = gpd.GeoDataFrame(
+            {
+                "datetime": [0],
+                "geometry": [point],
+                "vmax": [0],
+                "pc": [0],
+                "RMW": [0],
+                "R35_NE": [0],
+                "R35_SE": [0],
+                "R35_SW": [0],
+                "R35_NW": [0],
+                "R50_NE": [0],
+                "R50_SE": [0],
+                "R50_SW": [0],
+                "R50_NW": [0],
+                "R65_NE": [0],
+                "R65_SE": [0],
+                "R65_SW": [0],
+                "R65_NW": [0],
+                "R100_NE": [0],
+                "R100_SE": [0],
+                "R100_SW": [0],
+                "R100_NW": [0],
+            }
+        )
         self.track.set_crs(epsg=self.EPSG, inplace=True)
-        
-        # Done 
-        self.creation_time= datetime.now()
-        
-        
+
+        # Done
+        self.creation_time = datetime.now()
+
     # Reading
-    def from_jmv30(self, filename):        
-        self.read_track(filename, 'jmv30')
+    def from_jmv30(self, filename):
+        self.read_track(filename, "jmv30")
 
-    def from_ddb_cyc(self, filename):        
-        self.read_track(filename, 'ddb_cyc')
+    def from_ddb_cyc(self, filename):
+        self.read_track(filename, "ddb_cyc")
 
     def read_track(self, filename, fmt):
-        
         # If ddb_cyc
-        if fmt == 'ddb_cyc':
-            
+        if fmt == "ddb_cyc":
             # Read all the lines first
-            with open(filename, 'r') as f:
+            with open(filename, "r") as f:
                 lines = f.readlines()
-            
-            
+
             # Define the name first
             for line in lines:
-                if line[0:4] == 'Name':                    
-                    string_value    = line[5:]
-                    string_value    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.name       = string_value
-            
-            
+                if line[0:4] == "Name":
+                    string_value = line[5:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.name = string_value
+
             # Define other variables names (if they exist)
             for i in range(len(lines)):
                 line = lines[i]
-                if line[0:11] == 'WindProfile':    
-                    string_value                    = line[23:]
-                    string_value                    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.wind_profile               = string_value
-                if line[0:20] == 'WindPressureRelation':    
-                    string_value                    = line[23:]
-                    string_value                    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.wind_pressure_relation     = string_value
-                if line[0:12] == 'RMaxRelation':    
-                    string_value                    = line[23:]
-                    string_value                    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.rmw_relation               = string_value
-                if line[0:18] == 'Backgroundpressure':    
-                    string_value                    = line[23:]
-                    string_value                    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.background_pressure        = float(string_value)
-                if line[0:9] == 'PhiSpiral':    
-                    string_value                    = line[23:]
-                    string_value                    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.phi_spiral                 = float(string_value)
-                if line[0:20] == 'WindConversionFactor':    
-                    string_value                    = line[23:]
-                    self.wind_conversion_factor     = float(string_value)
-                if line[0:15] == 'SpiderwebRadius':    
-                    string_value                    = line[23:]
-                    string_value                    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.spiderweb_radius           = float(string_value)
-                if line[0:12] == 'NrRadialBins':    
-                    string_value                    = line[23:]
-                    string_value                    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.nr_radial_bins             = int(string_value)
-                if line[0:17] == 'NrDirectionalBins':    
-                    string_value                    = line[23:]
-                    string_value                    = ''.join(ch for ch in string_value if ch.isalnum())
-                    self.nr_directional_bins        = int(string_value)
-                    
-                    
+                if line[0:11] == "WindProfile":
+                    string_value = line[23:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.wind_profile = string_value
+                if line[0:20] == "WindPressureRelation":
+                    string_value = line[23:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.wind_pressure_relation = string_value
+                if line[0:12] == "RMaxRelation":
+                    string_value = line[23:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.rmw_relation = string_value
+                if line[0:18] == "Backgroundpressure":
+                    string_value = line[23:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.background_pressure = float(string_value)
+                if line[0:9] == "PhiSpiral":
+                    string_value = line[23:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.phi_spiral = float(string_value)
+                if line[0:20] == "WindConversionFactor":
+                    string_value = line[23:]
+                    self.wind_conversion_factor = float(string_value)
+                if line[0:15] == "SpiderwebRadius":
+                    string_value = line[23:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.spiderweb_radius = float(string_value)
+                if line[0:12] == "NrRadialBins":
+                    string_value = line[23:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.nr_radial_bins = int(string_value)
+                if line[0:17] == "NrDirectionalBins":
+                    string_value = line[23:]
+                    string_value = "".join(ch for ch in string_value if ch.isalnum())
+                    self.nr_directional_bins = int(string_value)
+
             # Read the track
             for i in range(len(lines)):
                 line = lines[i]
-                if line[0:8] == '#   Date':                    
+                if line[0:15] == '##    Datetime ' or line[0:15] == '#   Date   Time':            
                      break
             
             # Place coordinates in Tropical Cyclone Track 
             for j in range(i+2,len(lines)):
                 
                 # Get values
-                line            = lines[j]
-                line            = line.split()
-                date_format     = "%Y%m%d %H%M%S"
-                date_string     = line[0]  + ' ' + line[1] 
-                tc_time         = datetime.strptime(date_string, date_format)
-                tc_time_string  = tc_time.strftime(date_format)
-                y               = float(line[2])
-                x               = float(line[3])
-                vmax            = float(line[4])
-                pc              = float(line[5])
-                RMW             = float(line[6])
-                
-                R35_NE          = float(line[7])
-                R35_SE          = float(line[8])
-                R35_SW          = float(line[9])
-                R35_NW          = float(line[10])
-
-                R50_NE          = float(line[11])
-                R50_SE          = float(line[12])
-                R50_SW          = float(line[13])
-                R50_NW          = float(line[14])
-
-                R65_NE          = float(line[15])
-                R65_SE          = float(line[16])
-                R65_SW          = float(line[17])
-                R65_NW          = float(line[18])
-
-                R100_NE         = float(line[19])
-                R100_SE         = float(line[20])
-                R100_SW         = float(line[21])
-                R100_NW         = float(line[22])
-
-
-                # Make GeoDataFrame     
-                point       = Point(x,y)
-                gdf         = gpd.GeoDataFrame({"datetime": [tc_time_string],"geometry": [point], "vmax": [vmax], "pc": [pc], "RMW": [RMW],
-                                        "R35_NE":  [R35_NE],  "R35_SE":  [R35_SE], "R35_SW":  [R35_SW],  "R35_NW": [R35_NW],
-                                        "R50_NE":  [R50_NE],  "R50_SE":  [R50_SE], "R50_SW":  [R50_SW],  "R50_NW": [R50_NW],
-                                        "R65_NE":  [R65_NE],  "R65_SE":  [R65_SE], "R65_SW":  [R65_SW],  "R65_NW": [R65_NW],
-                                        "R100_NE": [R100_NE], "R100_SE": [R100_SE],"R100_SW": [R100_SW], "R100_NW": [R100_NW]})    
+                line = lines[j]
+                line = line.split()
+                date_format = "%Y%m%d %H%M%S"
+                date_string = line[0] + " " + line[1]
+                tc_time = datetime.strptime(date_string, date_format)
+                tc_time_string = tc_time.strftime(date_format)
+                y = float(line[2])
+                x = float(line[3])
+                vmax = float(line[4])
+                pc = float(line[5])
+                RMW = float(line[6])
+
+                R35_NE = float(line[7])
+                R35_SE = float(line[8])
+                R35_SW = float(line[9])
+                R35_NW = float(line[10])
+
+                R50_NE = float(line[11])
+                R50_SE = float(line[12])
+                R50_SW = float(line[13])
+                R50_NW = float(line[14])
+
+                R65_NE = float(line[15])
+                R65_SE = float(line[16])
+                R65_SW = float(line[17])
+                R65_NW = float(line[18])
+
+                R100_NE = float(line[19])
+                R100_SE = float(line[20])
+                R100_SW = float(line[21])
+                R100_NW = float(line[22])
+
+                # Make GeoDataFrame
+                point = Point(x, y)
+                gdf = gpd.GeoDataFrame(
+                    {
+                        "datetime": [tc_time_string],
+                        "geometry": [point],
+                        "vmax": [vmax],
+                        "pc": [pc],
+                        "RMW": [RMW],
+                        "R35_NE": [R35_NE],
+                        "R35_SE": [R35_SE],
+                        "R35_SW": [R35_SW],
+                        "R35_NW": [R35_NW],
+                        "R50_NE": [R50_NE],
+                        "R50_SE": [R50_SE],
+                        "R50_SW": [R50_SW],
+                        "R50_NW": [R50_NW],
+                        "R65_NE": [R65_NE],
+                        "R65_SE": [R65_SE],
+                        "R65_SW": [R65_SW],
+                        "R65_NW": [R65_NW],
+                        "R100_NE": [R100_NE],
+                        "R100_SE": [R100_SE],
+                        "R100_SW": [R100_SW],
+                        "R100_NW": [R100_NW],
+                    }
+                )
                 gdf.set_crs(epsg=self.EPSG, inplace=True)
-               
+
                 # Append self
-                self.track = pd.concat([self.track,gdf]) 
-            
+                self.track = pd.concat([self.track, gdf])
+
             # Done with this
             self.track = self.track.reset_index(drop=True)
-            self.track = self.track.drop([0])           # remove the dummy
+            self.track = self.track.drop([0])  # remove the dummy
             self.track = self.track.reset_index(drop=True)
-            if self.debug == 1: print('Succesfully read track - ddb_cyc')
+            if self.debug == 1:
+                print("Succesfully read track - ddb_cyc")
 
-        elif fmt == 'jmv30':
+        elif fmt == "jmv30":
             print("to do: work on progress")
-        else: 
-            raise Exception('This file format is not supported as read track!')
+        else:
+            raise Exception("This file format is not supported as read track!")
+
+    # Providing the track (from other source)   
+    def provide_track(self, datetimes=[], lons=[], lats=[], winds=[], pressures=[], rmw=[], r35=[]):
+
+        # All variables are Python lists and we simply place them in the right structure
+        # note that value -999 is a NaN for this moduel
+        # we assume datetimes but convert them internally
+        # R35 is a matrix with time and NE, SE, SW, NW Symmetric_Circle
+        
+        # First, check if we have either a wind or a pressure
+        a=1
+
+        # Loop over the list and place them
+        for index, vmax in enumerate(winds):
+
+            # Get time ready
+            date_format     = "%Y%m%d %H%M%S"
+            tc_time         = datetimes[index]
+            tc_time_string  = tc_time.strftime(date_format)    
+
+            # Make GeoDataFrame     
+            point       = Point(lons[index],lats[index])
+            gdf         = gpd.GeoDataFrame({"datetime": [tc_time_string],"geometry": [point], "vmax": [vmax], "pc": [pressures[index]], "RMW": [rmw[index]],
+                                    "R35_NE":  [r35[index][0]],  "R35_SE":  [r35[index][1]], "R35_SW":  [r35[index][2]],  "R35_NW": [r35[index][3]],
+                                    "R50_NE":  [-999],  "R50_SE":  [-999], "R50_SW":  [-999],  "R50_NW": [-999],
+                                    "R65_NE":  [-999],  "R65_SE":  [-999], "R65_SW":  [-999],  "R65_NW": [-999],
+                                    "R100_NE": [-999], "R100_SE": [-999],"R100_SW": [-999], "R100_NW": [-999]})    
+            gdf.set_crs(epsg=self.EPSG, inplace=True)
+                    
+            # Append self
+            self.track = pd.concat([self.track,gdf]) 
+                
+        # Done with this
+        self.track = self.track.reset_index(drop=True)
+        self.track = self.track.drop([0])           # remove the dummy
+        self.track = self.track.reset_index(drop=True)
+        if self.debug == 1: print('Succesfully placed track')
 
 
     # Writing 
     def write_track(self, filename, fmt):
-        
         # If ddb_cyc
-        if fmt == 'ddb_cyc':
-            
+        if fmt == "ddb_cyc":
             # Open file
-            with open(filename, 'wt') as f:
-                
-                 # Print header
-                f.writelines('# Tropical Cyclone Toolbox - Coastal Hazards Toolkit - ' + self.creation_time.strftime(dateformat_module) + '\n')
-  
+            with open(filename, "wt") as f:
+                # Print header
+                f.writelines(
+                    "# Tropical Cyclone Toolbox - Coastal Hazards Toolkit - "
+                    + self.creation_time.strftime(dateformat_module)
+                    + "\n"
+                )
+
                 # Print rest
-                f.writelines('Name                   ' + self.name + '\n')
+                f.writelines('Name                   "' + self.name + '"\n')
                 f.writelines('WindProfile            ' + self.wind_profile + '\n')
                 f.writelines('WindPressureRelation   ' + self.wind_pressure_relation + '\n')
                 f.writelines('RMaxRelation           ' + self.rmw_relation + '\n')
                 f.writelines('Backgroundpressure     ' + str(self.background_pressure) + '\n')
                 f.writelines('PhiSpiral              ' + str(self.phi_spiral) + '\n')
                 f.writelines('WindConversionFactor   ' + str(self.wind_conversion_factor) + '\n')
                 f.writelines('SpiderwebRadius        ' + str(self.spiderweb_radius) + '\n')
@@ -240,1663 +317,2160 @@
                 epsg        = self.track.crs.name
                 f.writelines('EPSG                   ' + epsg + '\n')
                 f.writelines('UnitIntensity          ' + str(self.unit_intensity) + '\n')
                 f.writelines('UnitWindRadii          ' + str(self.unit_radii) + '\n')
 
                 # Print header for the track
                 f.writelines('#  \n')
-                f.writelines('##    Datetime               Lat        Lon         Vmax       Pc          Rmax         R35(NE)      R35(SE)     R35(SW)     R35(NW)     R50(NE)     R50(SE)    R50(SW)    R50(NW)     R65(NE)     R65(SE)     R65(SW)     R65(NW)    R100(NE)    R100(SE)    R100(SW)    R100(NE)  \n')
+                f.writelines('#   Date   Time               Lat        Lon         Vmax       Pc          Rmax         R35(NE)      R35(SE)     R35(SW)     R35(NW)     R50(NE)     R50(SE)    R50(SW)    R50(NW)     R65(NE)     R65(SE)     R65(SW)     R65(NW)    R100(NE)    R100(SE)    R100(SW)    R100(NE)  \n')
+                f.writelines('#  \n')
 
                 # Print the actual track
                 for i in range(len(self.track)):
                     f.writelines(self.track.datetime[i].rjust(20))
                     coords = self.track.geometry[i]
-                    f.writelines(str(round(coords.y,2)).rjust(12))
-                    f.writelines(str(round(coords.x,2)).rjust(12))
-                    
-                    f.writelines(str(round(self.track.vmax[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.pc[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.RMW[i],1)).rjust(12))
-                    
-                    f.writelines(str(round(self.track.R35_NE[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R35_SE[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R35_SW[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R35_NW[i],1)).rjust(12))
-                    
-                    f.writelines(str(round(self.track.R50_NE[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R50_SE[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R50_SW[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R50_NW[i],1)).rjust(12))
-
-                    f.writelines(str(round(self.track.R65_NE[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R65_SE[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R65_SW[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R65_NW[i],1)).rjust(12))
-
-                    f.writelines(str(round(self.track.R100_NE[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R100_SE[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R100_SW[i],1)).rjust(12))
-                    f.writelines(str(round(self.track.R100_NW[i],1)).rjust(12))
-                    
-                    f.writelines('\n')
+                    f.writelines(str(round(coords.y, 2)).rjust(12))
+                    f.writelines(str(round(coords.x, 2)).rjust(12))
 
-            if self.debug == 1: print('Succesfully written track - ddb_cyc')
-        else: 
-            print('For other methods of writing the track; please used the "tc.track.to_file" option')
+                    f.writelines(str(round(self.track.vmax[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.pc[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.RMW[i], 1)).rjust(12))
+
+                    f.writelines(str(round(self.track.R35_NE[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R35_SE[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R35_SW[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R35_NW[i], 1)).rjust(12))
+
+                    f.writelines(str(round(self.track.R50_NE[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R50_SE[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R50_SW[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R50_NW[i], 1)).rjust(12))
+
+                    f.writelines(str(round(self.track.R65_NE[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R65_SE[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R65_SW[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R65_NW[i], 1)).rjust(12))
+
+                    f.writelines(str(round(self.track.R100_NE[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R100_SE[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R100_SW[i], 1)).rjust(12))
+                    f.writelines(str(round(self.track.R100_NW[i], 1)).rjust(12))
 
+                    f.writelines("\n")
+
+            if self.debug == 1:
+                print("Succesfully written track - ddb_cyc")
+        else:
+            print(
+                'For other methods of writing the track; please used the "tc.track.to_file" option'
+            )
 
     # Support functions for creating spiderweb
     # 1. estimate_missing_values => still assuming imperial system
     def estimate_missing_values(self):
-        
         # Go over the track and determine missing values
         for it in range(len(self.track)):
-            
             # Get coordinates
-            coords_it       = self.track.geometry[it]            
-
+            coords_it = self.track.geometry[it]
 
             # determine wind speed
             if self.track.vmax[it] < 0:
-                if self.wind_pressure_relation == 'holland2008':
-                    
+                if self.wind_pressure_relation == "holland2008":
                     # estimate this: vmax is in m/s
-                    vmax      =  wpr_holland2008(pc     = self.track.pc[it],
-                                           pn           = self.background_pressure, 
-                                           phi          = coords_it.y,
-                                           dpcdt        = self.track.dpcdt[it],
-                                           vt           = np.sqrt(self.track.vtx[it]**2 + self.track.vty[it]**2), 
-                                           rhoa         = self.rho_air)
-                    
-                    # place this 
-                    if self.unit_intensity == 'knots':
+                    vmax = wpr_holland2008(
+                        pc=self.track.pc[it],
+                        pn=self.background_pressure,
+                        phi=coords_it.y,
+                        dpcdt=self.track.dpcdt[it],
+                        vt=np.sqrt(self.track.vtx[it] ** 2 + self.track.vty[it] ** 2),
+                        rhoa=self.rho_air,
+                    )
+
+                    # place this
+                    if self.unit_intensity == "knots":
                         self.track.vmax[it] = vmax / knots_to_ms
                     else:
                         self.track.vmax[it] = vmax
- 
-            
-            
+
             # determine pressure
             if self.track.pc[it] < 0:
-                if self.wind_pressure_relation == 'holland2008':
-                    
+                if self.wind_pressure_relation == "holland2008":
                     # estimate this
-                    if self.unit_intensity == 'knots':
-                        pc      =  wpr_holland2008(vmax     = self.track.vmax[it]*knots_to_ms,
-                                                   pn       = self.background_pressure, 
-                                                   phi      = coords_it.y,
-                                                   dpcdt        = self.track.dpcdt[it],
-                                                   vt           = np.sqrt(self.track.vtx[it]**2 + self.track.vty[it]**2), 
-                                                   rhoa     = self.rho_air)
+                    if self.unit_intensity == "knots":
+                        pc = wpr_holland2008(
+                            vmax=self.track.vmax[it] * knots_to_ms,
+                            pn=self.background_pressure,
+                            phi=coords_it.y,
+                            dpcdt=self.track.dpcdt[it],
+                            vt=np.sqrt(
+                                self.track.vtx[it] ** 2 + self.track.vty[it] ** 2
+                            ),
+                            rhoa=self.rho_air,
+                        )
                     else:
-                        pc      =  wpr_holland2008(vmax     = self.track.vmax[it],
-                                                   pn       = self.background_pressure, 
-                                                   phi      = coords_it.y,
-                                                   dpcdt    = self.track.dpcdt[it],
-                                                   vt       = np.sqrt(self.track.vtx[it]**2 + self.track.vty[it]**2), 
-                                                   rhoa     = self.rho_air)
-                            
+                        pc = wpr_holland2008(
+                            vmax=self.track.vmax[it],
+                            pn=self.background_pressure,
+                            phi=coords_it.y,
+                            dpcdt=self.track.dpcdt[it],
+                            vt=np.sqrt(
+                                self.track.vtx[it] ** 2 + self.track.vty[it] ** 2
+                            ),
+                            rhoa=self.rho_air,
+                        )
+
                     # place this
                     self.track.pc[it] = pc
 
-
             # radius of maximum winds (RMW)
             if self.track.RMW[it] < 0:
-                
                 # Nederhoff et al. 2019
-                if self.rmw_relation == 'nederhoff2019':
-                    
+                if self.rmw_relation == "nederhoff2019":
                     # Estimate: relationship assume m/s
-                    if self.unit_intensity == 'knots':
-                        [rmax, dr35]        = wind_radii_nederhoff(self.track.vmax[it]/knots_to_ms, coords_it.y, 0, 0)
+                    if self.unit_intensity == "knots":
+                        [rmax, dr35] = wind_radii_nederhoff(
+                            self.track.vmax[it] / knots_to_ms, coords_it.y, 0, 0
+                        )
                     else:
-                        [rmax, dr35]        = wind_radii_nederhoff(self.track.vmax[it], coords_it.y, 0, 0)
-                        
+                        [rmax, dr35] = wind_radii_nederhoff(
+                            self.track.vmax[it], coords_it.y, 0, 0
+                        )
+
                     # Place value: output is in km
-                    if self.unit_radii == 'nm':
-                        self.track.RMW[it]  = rmax['mode']/nm_to_km
+                    if self.unit_radii == "nm":
+                        self.track.RMW[it] = rmax["mode"] / nm_to_km
                     else:
-                        self.track.RMW[it]  = rmax['mode']
-                
-                
+                        self.track.RMW[it] = rmax["mode"]
+
                 # Gross et al. 2004
-                elif self.rmw_relation == 'gross2004':
-                    
+                elif self.rmw_relation == "gross2004":
                     # Estimate: relationship assume knots
-                    if self.unit_radii == 'knots':
-                        rmax                = 35.37 - 0.11100*self.track.vmax[it] + 0.5700*(abs(coords_it.y)-25)
+                    if self.unit_radii == "knots":
+                        rmax = (
+                            35.37
+                            - 0.11100 * self.track.vmax[it]
+                            + 0.5700 * (abs(coords_it.y) - 25)
+                        )
                     else:
-                        rmax                = 35.37 - 0.11100*self.track.vmax[it]*knots_to_ms + 0.5700*(abs(coords_it.y)-25)
-                
+                        rmax = (
+                            35.37
+                            - 0.11100 * self.track.vmax[it] * knots_to_ms
+                            + 0.5700 * (abs(coords_it.y) - 25)
+                        )
+
                     # Place value: output is in nm
-                    if self.unit_radii == 'nm':
-                        self.track.RMW[it]  = rmax
+                    if self.unit_radii == "nm":
+                        self.track.RMW[it] = rmax
                     else:
-                        self.track.RMW[it]  = rmax*nm_to_km
-                
-                
-                # Simple constant value of 25 nm    
-                elif self.rmw_relation == 'constant_25nm':
-                    
+                        self.track.RMW[it] = rmax * nm_to_km
+
+                # Simple constant value of 25 nm
+                elif self.rmw_relation == "constant_25nm":
                     # Place 25 nm
-                    if self.unit_radii == 'nm':
-                        self.track.RMW[it]  = float(25)
+                    if self.unit_radii == "nm":
+                        self.track.RMW[it] = float(25)
                     else:
-                        self.track.RMW[it]  = float(25)*nm_to_km
-                    
-                    
-                    
+                        self.track.RMW[it] = float(25) * nm_to_km
+
             # radius of gale force winds (R35)
-            if self.wind_profile == 'holland2010':
+            if self.wind_profile == "holland2010":
                 if self.track.vmax[it] >= 35:
-                    if (self.track.R35_NE[it] == -999) and (self.track.R35_SE[it] == -999) and (self.track.R35_SW[it] == -999) and (self.track.R35_NW[it] == -999) :
-                        
+                    if (
+                        (self.track.R35_NE[it] == -999)
+                        and (self.track.R35_SE[it] == -999)
+                        and (self.track.R35_SW[it] == -999)
+                        and (self.track.R35_NW[it] == -999)
+                    ):
                         # Estimate values
-                        if self.unit_radii == 'knots':
-                            [rmax, dr35]            = wind_radii_nederhoff(self.track.vmax[it]*knots_to_ms, coords_it.y, 0, 0)
+                        if self.unit_radii == "knots":
+                            [rmax, dr35] = wind_radii_nederhoff(
+                                self.track.vmax[it] * knots_to_ms, coords_it.y, 0, 0
+                            )
                         else:
-                            [rmax, dr35]        = wind_radii_nederhoff(self.track.vmax[it], coords_it.y, 0, 0)
-                            
-                        if self.unit_radii == 'nm':    
-                            self.track.R35_NE[it]   = dr35['mode']/nm_to_km + self.track.RMW[it]
-                            self.track.R35_SE[it]   = dr35['mode']/nm_to_km + self.track.RMW[it]
-                            self.track.R35_SW[it]   = dr35['mode']/nm_to_km + self.track.RMW[it]
-                            self.track.R35_NW[it]   = dr35['mode']/nm_to_km + self.track.RMW[it]
+                            [rmax, dr35] = wind_radii_nederhoff(
+                                self.track.vmax[it], coords_it.y, 0, 0
+                            )
+
+                        if self.unit_radii == "nm":
+                            self.track.R35_NE[it] = (
+                                dr35["mode"] / nm_to_km + self.track.RMW[it]
+                            )
+                            self.track.R35_SE[it] = (
+                                dr35["mode"] / nm_to_km + self.track.RMW[it]
+                            )
+                            self.track.R35_SW[it] = (
+                                dr35["mode"] / nm_to_km + self.track.RMW[it]
+                            )
+                            self.track.R35_NW[it] = (
+                                dr35["mode"] / nm_to_km + self.track.RMW[it]
+                            )
                         else:
-                            self.track.R35_NE[it]   = dr35['mode'] + self.track.RMW[it]
-                            self.track.R35_SE[it]   = dr35['mode'] + self.track.RMW[it]
-                            self.track.R35_SW[it]   = dr35['mode'] + self.track.RMW[it]
-                            self.track.R35_NW[it]   = dr35['mode'] + self.track.RMW[it]
+                            self.track.R35_NE[it] = dr35["mode"] + self.track.RMW[it]
+                            self.track.R35_SE[it] = dr35["mode"] + self.track.RMW[it]
+                            self.track.R35_SW[it] = dr35["mode"] + self.track.RMW[it]
+                            self.track.R35_NW[it] = dr35["mode"] + self.track.RMW[it]
 
-    
-    
-    # 2. cut_off_low_wind_speeds
+    # 2A. cut_off_low_wind_speeds
     def cut_off_low_wind_speeds(self):
-        
         # Only apply this when the cut_off wind is defined
         if self.low_wind_speeds_cut_off > 0.0:
-        
             # Find first
             ifirst = []
             for it in range(len(self.track)):
                 if self.track.vmax[it] >= self.low_wind_speeds_cut_off and not ifirst:
                     ifirst = it
                     break
-            if ifirst>0:
+            if ifirst > 0:
                 self.track = self.track.drop(list(range(0, ifirst)))
                 self.track = self.track.reset_index(drop=True)
-                
+
             # Find last
             ilast = []
-            for it in range(len(self.track)-1, 0-1 , -1):
+            for it in range(len(self.track) - 1, 0 - 1, -1):
                 if self.track.vmax[it] >= self.low_wind_speeds_cut_off and not ilast:
                     ilast = it
                     break
             if ilast:
-                self.track = self.track.drop(list(range(ilast+1, len(self.track))))
+                self.track = self.track.drop(list(range(ilast + 1, len(self.track))))
                 self.track = self.track.reset_index(drop=True)
-            
-            
+
         else:
-            if self.debug == 1: print('No cut_off_low_wind_speeds since wind speed is zero or lower')
-     
-    
+            if self.debug == 1:
+                print("No cut_off_low_wind_speeds since wind speed is zero or lower")
+
+    # 2B. Extent track with certain number of days
+    def extent_track(self):
+        # Only apply this when the extend days are defined
+        if self.extend_track > 0.0:
+            # Compute last gradient
+            it_last = len(self.track) - 1
+            coords2 = self.track.geometry[it_last]  # last
+            datetime2 = datetime.strptime(
+                self.track.datetime[it_last], dateformat_module
+            )
+
+            it = len(self.track) - 2
+            coords1 = self.track.geometry[it]  # first
+            datetime1 = datetime.strptime(self.track.datetime[it], dateformat_module)
+            dx = coords2.x - coords1.x
+            dy = coords2.y - coords1.y
+            dt = datetime2 - datetime1
+
+            # Extending the track
+            for i in range(1, int(self.extend_track)):
+                # Get location
+                dt_factor = 86400 / dt.seconds
+                x = coords2.x + dx * dt_factor * i
+                y = coords2.y + dy * dt_factor * i
+                point = Point(x, y)
+
+                # Make time
+                date_format = "%Y%m%d %H%M%S"
+                tc_time = datetime.strptime(self.track.datetime[it_last], date_format)
+                tc_time = tc_time + timedelta(days=i)
+                tc_time_string = tc_time.strftime(date_format)
+                # print(tc_time_string)
+
+                # Make GeoDataFrame
+                gdf = gpd.GeoDataFrame(
+                    {
+                        "datetime": [tc_time_string],
+                        "geometry": [point],
+                        "vmax": [self.track.vmax[it_last]],
+                        "pc": [self.track.pc[it_last]],
+                        "RMW": [self.track.RMW[it_last]],
+                        "R35_NE": [0],
+                        "R35_SE": [0],
+                        "R35_SW": [0],
+                        "R35_NW": [0],
+                        "R50_NE": [0],
+                        "R50_SE": [0],
+                        "R50_SW": [0],
+                        "R50_NW": [0],
+                        "R65_NE": [0],
+                        "R65_SE": [0],
+                        "R65_SW": [0],
+                        "R65_NW": [0],
+                        "R100_NE": [0],
+                        "R100_SE": [0],
+                        "R100_SW": [0],
+                        "R100_NW": [0],
+                    }
+                )
+                gdf.set_crs(epsg=self.EPSG, inplace=True)
+
+                # Append self
+                self.track = pd.concat([self.track, gdf])
+
+            # Done
+            self.track = self.track.reset_index(drop=True)
+            if self.debug == 1:
+                print("Succesfully extended track")
+
+        else:
+            if self.debug == 1:
+                print("No extending since number of days is zero or lower")
+
     # 3A. convert_units_imperial_metric
     def convert_units_imperial_metric(self):
-        
         # Convert wind speeds
-        # from  knots   - typically 1-minute averaged 
+        # from  knots   - typically 1-minute averaged
         # to    m/s     - we account for conversion here
-        if (self.unit_intensity == 'knots') and (self.unit_radii == 'nm'):
-        
+        if (self.unit_intensity == "knots") and (self.unit_radii == "nm"):
             # Intensity first
-            self.track.vmax     = self.track.vmax * knots_to_ms * self.wind_conversion_factor
-              
+            self.track.vmax = (
+                self.track.vmax * knots_to_ms * self.wind_conversion_factor
+            )
+
             # Convert radius of maximum winds
-            self.track.RMW      = self.track.RMW * nm_to_km
-    
+            self.track.RMW = self.track.RMW * nm_to_km
+
             # Convert wind radii
             for it in range(len(self.track)):
-                
                 # R35
                 if self.track.R35_NE[it] > 0:
-                    self.track.R35_NE[it]  = self.track.R35_NE[it]* nm_to_km
+                    self.track.R35_NE[it] = self.track.R35_NE[it] * nm_to_km
                 else:
-                    self.track.R35_NE[it]  = np.NaN
-            
+                    self.track.R35_NE[it] = np.NaN
+
                 if self.track.R35_SE[it] > 0:
-                    self.track.R35_SE[it]  = self.track.R35_SE[it]* nm_to_km
+                    self.track.R35_SE[it] = self.track.R35_SE[it] * nm_to_km
                 else:
-                    self.track.R35_SE[it]  = np.NaN
-            
+                    self.track.R35_SE[it] = np.NaN
+
                 if self.track.R35_SW[it] > 0:
-                    self.track.R35_SW[it]  = self.track.R35_SW[it]* nm_to_km
+                    self.track.R35_SW[it] = self.track.R35_SW[it] * nm_to_km
                 else:
-                    self.track.R35_SW[it]  = np.NaN
-            
+                    self.track.R35_SW[it] = np.NaN
+
                 if self.track.R35_NW[it] > 0:
-                    self.track.R35_NW[it]  = self.track.R35_NW[it]* nm_to_km
+                    self.track.R35_NW[it] = self.track.R35_NW[it] * nm_to_km
                 else:
-                    self.track.R35_NW[it]  = np.NaN
-                    
+                    self.track.R35_NW[it] = np.NaN
+
                 # R50
                 if self.track.R50_NE[it] > 0:
-                    self.track.R50_NE[it]  = self.track.R50_NE[it]* nm_to_km
+                    self.track.R50_NE[it] = self.track.R50_NE[it] * nm_to_km
                 else:
-                    self.track.R50_NE[it]  = np.NaN
-            
+                    self.track.R50_NE[it] = np.NaN
+
                 if self.track.R50_SE[it] > 0:
-                    self.track.R50_SE[it]  = self.track.R50_SE[it]* nm_to_km
+                    self.track.R50_SE[it] = self.track.R50_SE[it] * nm_to_km
                 else:
-                    self.track.R50_SE[it]  = np.NaN
-            
+                    self.track.R50_SE[it] = np.NaN
+
                 if self.track.R50_SW[it] > 0:
-                    self.track.R50_SW[it]  = self.track.R50_SW[it]* nm_to_km
+                    self.track.R50_SW[it] = self.track.R50_SW[it] * nm_to_km
                 else:
-                    self.track.R50_SW[it]  = np.NaN
-            
+                    self.track.R50_SW[it] = np.NaN
+
                 if self.track.R50_NW[it] > 0:
-                    self.track.R50_NW[it]  = self.track.R50_NW[it]* nm_to_km
+                    self.track.R50_NW[it] = self.track.R50_NW[it] * nm_to_km
                 else:
-                    self.track.R50_NW[it]  = np.NaN
-            
+                    self.track.R50_NW[it] = np.NaN
+
                 # R65
                 if self.track.R65_NE[it] > 0:
-                    self.track.R65_NE[it]  = self.track.R65_NE[it]* nm_to_km
+                    self.track.R65_NE[it] = self.track.R65_NE[it] * nm_to_km
                 else:
-                    self.track.R65_NE[it]  = np.NaN
-            
+                    self.track.R65_NE[it] = np.NaN
+
                 if self.track.R65_SE[it] > 0:
-                    self.track.R65_SE[it]  = self.track.R65_SE[it]* nm_to_km
+                    self.track.R65_SE[it] = self.track.R65_SE[it] * nm_to_km
                 else:
-                    self.track.R65_SE[it]  = np.NaN
-            
+                    self.track.R65_SE[it] = np.NaN
+
                 if self.track.R65_SW[it] > 0:
-                    self.track.R65_SW[it]  = self.track.R65_SW[it]* nm_to_km
+                    self.track.R65_SW[it] = self.track.R65_SW[it] * nm_to_km
                 else:
-                    self.track.R65_SW[it]  = np.NaN
-            
+                    self.track.R65_SW[it] = np.NaN
+
                 if self.track.R65_NW[it] > 0:
-                    self.track.R65_NW[it]  = self.track.R65_NW[it]* nm_to_km
+                    self.track.R65_NW[it] = self.track.R65_NW[it] * nm_to_km
                 else:
-                    self.track.R65_NW[it]  = np.NaN
-            
+                    self.track.R65_NW[it] = np.NaN
+
                 # R100
                 if self.track.R100_NE[it] > 0:
-                    self.track.R100_NE[it]  = self.track.R100_NE[it]* nm_to_km
+                    self.track.R100_NE[it] = self.track.R100_NE[it] * nm_to_km
                 else:
-                    self.track.R100_NE[it]  = np.NaN
-            
+                    self.track.R100_NE[it] = np.NaN
+
                 if self.track.R100_SE[it] > 0:
-                    self.track.R100_SE[it]  = self.track.R100_SE[it]* nm_to_km
+                    self.track.R100_SE[it] = self.track.R100_SE[it] * nm_to_km
                 else:
-                    self.track.R100_SE[it]  = np.NaN
-            
+                    self.track.R100_SE[it] = np.NaN
+
                 if self.track.R100_SW[it] > 0:
-                    self.track.R100_SW[it]  = self.track.R100_SW[it]* nm_to_km
+                    self.track.R100_SW[it] = self.track.R100_SW[it] * nm_to_km
                 else:
-                    self.track.R100_SW[it]  = np.NaN
-            
+                    self.track.R100_SW[it] = np.NaN
+
                 if self.track.R100_NW[it] > 0:
-                    self.track.R100_NW[it]  = self.track.R100_NW[it]* nm_to_km
+                    self.track.R100_NW[it] = self.track.R100_NW[it] * nm_to_km
                 else:
-                    self.track.R100_NW[it]  = np.NaN
-        
-            # Done, so set variable 
-            self.unit_intensity   = 'ms'             
-            self.unit_radii       = 'km'     
-            if self.debug == 1: print('convert units to metric system')
-            
+                    self.track.R100_NW[it] = np.NaN
+
+            # Done, so set variable
+            self.unit_intensity = "ms"
+            self.unit_radii = "km"
+            if self.debug == 1:
+                print("convert units to metric system")
+
         else:
-            if self.debug == 1: print('units are already in the metric system: no action')
- 
-        
-        
+            if self.debug == 1:
+                print("units are already in the metric system: no action")
+
     # 3B. convert_units_metric_imperial
     def convert_units_metric_imperial(self):
-        
         # Convert wind speeds
         # from  m/s     - we account for conversion here
-        # from  knots   - typically 1-minute averaged 
-        
-        if (self.unit_intensity == 'ms') and (self.unit_radii == 'km'):
-        
+        # from  knots   - typically 1-minute averaged
+
+        if (self.unit_intensity == "ms") and (self.unit_radii == "km"):
             # Intensity first
-            self.track.vmax     = self.track.vmax / knots_to_ms / self.wind_conversion_factor
-              
+            self.track.vmax = (
+                self.track.vmax / knots_to_ms / self.wind_conversion_factor
+            )
+
             # Convert radius of maximum winds
-            self.track.RMW      = self.track.RMW / nm_to_km
-    
+            self.track.RMW = self.track.RMW / nm_to_km
+
             # Convert wind radii
             for it in range(len(self.track)):
-                
                 # R35
                 if self.track.R35_NE[it] > 0:
-                    self.track.R35_NE[it]  = self.track.R35_NE[it]/ nm_to_km
+                    self.track.R35_NE[it] = self.track.R35_NE[it] / nm_to_km
                 else:
-                    self.track.R35_NE[it]  = -999
-            
+                    self.track.R35_NE[it] = -999
+
                 if self.track.R35_SE[it] > 0:
-                    self.track.R35_SE[it]  = self.track.R35_SE[it]/ nm_to_km
+                    self.track.R35_SE[it] = self.track.R35_SE[it] / nm_to_km
                 else:
-                    self.track.R35_SE[it]  = -999
-            
+                    self.track.R35_SE[it] = -999
+
                 if self.track.R35_SW[it] > 0:
-                    self.track.R35_SW[it]  = self.track.R35_SW[it]/ nm_to_km
+                    self.track.R35_SW[it] = self.track.R35_SW[it] / nm_to_km
                 else:
-                    self.track.R35_SW[it]  = -999
-            
+                    self.track.R35_SW[it] = -999
+
                 if self.track.R35_NW[it] > 0:
-                    self.track.R35_NW[it]  = self.track.R35_NW[it]/ nm_to_km
+                    self.track.R35_NW[it] = self.track.R35_NW[it] / nm_to_km
                 else:
-                    self.track.R35_NW[it]  = -999
-                    
+                    self.track.R35_NW[it] = -999
+
                 # R50
                 if self.track.R50_NE[it] > 0:
-                    self.track.R50_NE[it]  = self.track.R50_NE[it]/ nm_to_km
+                    self.track.R50_NE[it] = self.track.R50_NE[it] / nm_to_km
                 else:
-                    self.track.R50_NE[it]  = -999
-            
+                    self.track.R50_NE[it] = -999
+
                 if self.track.R50_SE[it] > 0:
-                    self.track.R50_SE[it]  = self.track.R50_SE[it]/ nm_to_km
+                    self.track.R50_SE[it] = self.track.R50_SE[it] / nm_to_km
                 else:
-                    self.track.R50_SE[it]  = -999
-            
+                    self.track.R50_SE[it] = -999
+
                 if self.track.R50_SW[it] > 0:
-                    self.track.R50_SW[it]  = self.track.R50_SW[it]/ nm_to_km
+                    self.track.R50_SW[it] = self.track.R50_SW[it] / nm_to_km
                 else:
-                    self.track.R50_SW[it]  = -999
-            
+                    self.track.R50_SW[it] = -999
+
                 if self.track.R50_NW[it] > 0:
-                    self.track.R50_NW[it]  = self.track.R50_NW[it]/ nm_to_km
+                    self.track.R50_NW[it] = self.track.R50_NW[it] / nm_to_km
                 else:
-                    self.track.R50_NW[it]  = -999
-            
+                    self.track.R50_NW[it] = -999
+
                 # R65
                 if self.track.R65_NE[it] > 0:
-                    self.track.R65_NE[it]  = self.track.R65_NE[it]/ nm_to_km
+                    self.track.R65_NE[it] = self.track.R65_NE[it] / nm_to_km
                 else:
-                    self.track.R65_NE[it]  = -999
-            
+                    self.track.R65_NE[it] = -999
+
                 if self.track.R65_SE[it] > 0:
-                    self.track.R65_SE[it]  = self.track.R65_SE[it]/ nm_to_km
+                    self.track.R65_SE[it] = self.track.R65_SE[it] / nm_to_km
                 else:
-                    self.track.R65_SE[it]  = -999
-            
+                    self.track.R65_SE[it] = -999
+
                 if self.track.R65_SW[it] > 0:
-                    self.track.R65_SW[it]  = self.track.R65_SW[it]/ nm_to_km
+                    self.track.R65_SW[it] = self.track.R65_SW[it] / nm_to_km
                 else:
-                    self.track.R65_SW[it]  = -999
-            
+                    self.track.R65_SW[it] = -999
+
                 if self.track.R65_NW[it] > 0:
-                    self.track.R65_NW[it]  = self.track.R65_NW[it]/ nm_to_km
+                    self.track.R65_NW[it] = self.track.R65_NW[it] / nm_to_km
                 else:
-                    self.track.R65_NW[it]  = -999
-            
+                    self.track.R65_NW[it] = -999
+
                 # R100
                 if self.track.R100_NE[it] > 0:
-                    self.track.R100_NE[it]  = self.track.R100_NE[it]/ nm_to_km
+                    self.track.R100_NE[it] = self.track.R100_NE[it] / nm_to_km
                 else:
-                    self.track.R100_NE[it]  = -999
-            
+                    self.track.R100_NE[it] = -999
+
                 if self.track.R100_SE[it] > 0:
-                    self.track.R100_SE[it]  = self.track.R100_SE[it]/ nm_to_km
+                    self.track.R100_SE[it] = self.track.R100_SE[it] / nm_to_km
                 else:
-                    self.track.R100_SE[it]  = -999
-            
+                    self.track.R100_SE[it] = -999
+
                 if self.track.R100_SW[it] > 0:
-                    self.track.R100_SW[it]  = self.track.R100_SW[it]/ nm_to_km
+                    self.track.R100_SW[it] = self.track.R100_SW[it] / nm_to_km
                 else:
-                    self.track.R100_SW[it]  = -999
-            
+                    self.track.R100_SW[it] = -999
+
                 if self.track.R100_NW[it] > 0:
-                    self.track.R100_NW[it]  = self.track.R100_NW[it]/ nm_to_km
+                    self.track.R100_NW[it] = self.track.R100_NW[it] / nm_to_km
                 else:
-                    self.track.R100_NW[it]  = -999
-            
-            
-            # Done, so set variable 
-            self.unit_intensity   = 'knots'             
-            self.unit_radii       = 'nm'       
-            if self.debug == 1: print('convert units to imperial system')
-            
+                    self.track.R100_NW[it] = -999
+
+            # Done, so set variable
+            self.unit_intensity = "knots"
+            self.unit_radii = "nm"
+            if self.debug == 1:
+                print("convert units to imperial system")
+
         else:
-            if self.debug == 1: print('units are already in the imperial system: no action')
-        
-        
+            if self.debug == 1:
+                print("units are already in the imperial system: no action")
+
     # 4. account_for_forward_speed
     def account_for_forward_speed(self):
-        
         # Assign variables to geopandas dataframe
-        nan_list    = [np.nan for _ in range(len(self.track))]
-        self.track  = self.track.assign(vtx=nan_list)
-        self.track  = self.track.assign(vty=nan_list)
-        self.track  = self.track.assign(dpcdt=nan_list)
-        self.track  = self.track.assign(vmax_rel=nan_list)
-        
+        nan_list = [np.nan for _ in range(len(self.track))]
+        self.track = self.track.assign(vtx=nan_list)
+        self.track = self.track.assign(vty=nan_list)
+        self.track = self.track.assign(dpcdt=nan_list)
+        self.track = self.track.assign(vmax_rel=nan_list)
+
         # Same for 4 quadrants and 4 radii
-        nan_array = [np.full((4,4), np.nan) for i in range(len(self.track))]
-        self.track  = self.track.assign(quadrants_radii=nan_array)
-        
-        speeds      = np.array([[35, 35, 35, 35], [50, 50, 50, 50], [65, 65, 65, 65], [100, 100, 100, 100]])*knots_to_ms
+        nan_array = [np.full((4, 4), np.nan) for i in range(len(self.track))]
+        self.track = self.track.assign(quadrants_radii=nan_array)
+
+        speeds = (
+            np.array(
+                [
+                    [35, 35, 35, 35],
+                    [50, 50, 50, 50],
+                    [65, 65, 65, 65],
+                    [100, 100, 100, 100],
+                ]
+            )
+            * knots_to_ms
+        )
         speed_array = [speeds for i in range(len(self.track))]
-        self.track  = self.track.assign(quadrants_speed=speed_array)
+        self.track = self.track.assign(quadrants_speed=speed_array)
 
         # Go over time steps
         for it in range(len(self.track)):
-        
             # Get basics
-            datetime_it     = datetime.strptime(self.track.datetime[it], dateformat_module)
-            coords_it       = self.track.geometry[it]            
-            geofacx         = 1
-            geofacy         = 1
-            
+            datetime_it = datetime.strptime(self.track.datetime[it], dateformat_module)
+            coords_it = self.track.geometry[it]
+            geofacx = 1
+            geofacy = 1
+
             # Determine geo factors (currently only geo support)
             if self.track.crs.name == 'WGS 84':
-                geofacy = 111111
-                geofacx = geofacy * np.cos(coords_it.y * np.pi/180)
+                geofacy = 110540
+                geofacx = 111320 * np.cos(coords_it.y * np.pi/180)
         
             if it == 0:
-                
-                # Forward 
-                datetime_forward    = datetime.strptime(self.track.datetime[it+1], dateformat_module)
-                coords_forward      = self.track.geometry[it+1] 
-                dt                  = datetime_forward - datetime_it
-                dt                  = dt.total_seconds()
-                dx                  = (coords_forward.x - coords_it.x) * geofacx
-                dy                  = (coords_forward.y - coords_it.y) * geofacy
-                dpc                 = self.track.pc[it+1] - self.track.pc[it] 
-                
-            elif it == len(self.track)-1:
-                
-                # Backward 
-                datetime_backward   = datetime.strptime(self.track.datetime[it-1], dateformat_module)
-                coords_backward     = self.track.geometry[it-1] 
-                dt                  = datetime_it - datetime_backward
-                dt                  = dt.total_seconds()
-                dx                  = (coords_it.x - coords_backward.x) * geofacx
-                dy                  = (coords_it.y - coords_backward.y) * geofacy
-                dpc                 = self.track.pc[it] - self.track.pc[it-1] 
-                
-            else: 
-    
-                # Forward           
-                datetime_forward    = datetime.strptime(self.track.datetime[it+1], dateformat_module)
-                coords_forward      = self.track.geometry[it+1] 
-                dt1                 = datetime_forward - datetime_it
-                dt1                 = dt1.total_seconds()
-                dx1                 = (coords_forward.x - coords_it.x) * geofacx
-                dy1                 = (coords_forward.y - coords_it.y) * geofacy
-                dpc1                = self.track.pc[it+1] - self.track.pc[it] 
-                
-                # Backward 
-                datetime_backward   = datetime.strptime(self.track.datetime[it-1], dateformat_module)
-                coords_backward     = self.track.geometry[it-1] 
-                dt2                 = datetime_it - datetime_backward
-                dt2                 = dt2.total_seconds()
-                dx2                 = (coords_it.x - coords_backward.x) * geofacx
-                dy2                 = (coords_it.y - coords_backward.y) * geofacy
-                dpc2                = self.track.pc[it] - self.track.pc[it-1] 
-                
+                # Forward
+                datetime_forward = datetime.strptime(
+                    self.track.datetime[it + 1], dateformat_module
+                )
+                coords_forward = self.track.geometry[it + 1]
+                dt = datetime_forward - datetime_it
+                dt = dt.total_seconds()
+                dx = (coords_forward.x - coords_it.x) * geofacx
+                dy = (coords_forward.y - coords_it.y) * geofacy
+                dpc = self.track.pc[it + 1] - self.track.pc[it]
+
+            elif it == len(self.track) - 1:
+                # Backward
+                datetime_backward = datetime.strptime(
+                    self.track.datetime[it - 1], dateformat_module
+                )
+                coords_backward = self.track.geometry[it - 1]
+                dt = datetime_it - datetime_backward
+                dt = dt.total_seconds()
+                dx = (coords_it.x - coords_backward.x) * geofacx
+                dy = (coords_it.y - coords_backward.y) * geofacy
+                dpc = self.track.pc[it] - self.track.pc[it - 1]
+
+            else:
+                # Forward
+                datetime_forward = datetime.strptime(
+                    self.track.datetime[it + 1], dateformat_module
+                )
+                coords_forward = self.track.geometry[it + 1]
+                dt1 = datetime_forward - datetime_it
+                dt1 = dt1.total_seconds()
+                dx1 = (coords_forward.x - coords_it.x) * geofacx
+                dy1 = (coords_forward.y - coords_it.y) * geofacy
+                dpc1 = self.track.pc[it + 1] - self.track.pc[it]
+
+                # Backward
+                datetime_backward = datetime.strptime(
+                    self.track.datetime[it - 1], dateformat_module
+                )
+                coords_backward = self.track.geometry[it - 1]
+                dt2 = datetime_it - datetime_backward
+                dt2 = dt2.total_seconds()
+                dx2 = (coords_it.x - coords_backward.x) * geofacx
+                dy2 = (coords_it.y - coords_backward.y) * geofacy
+                dpc2 = self.track.pc[it] - self.track.pc[it - 1]
+
                 # Combined yields central differences
-                dx                  = np.mean([dx1, dx2])
-                dy                  = np.mean([dy1, dy2])
-                dt                  = np.mean([dt1, dt2])
-                dpc                 = np.mean([dpc1, dpc2])
-                
-                
+                dx = np.mean([dx1, dx2])
+                dy = np.mean([dy1, dy2])
+                dt = np.mean([dt1, dt2])
+                dpc = np.mean([dpc1, dpc2])
+
             # Compute variables
-            ux      = dx / dt               # speed in meter per seconds
-            uy      = dy / dt   
-            dpcdt   = dpc/ (dt   / 3600)    # pressure change per hour 
-    
-    
+            ux = dx / dt  # speed in meter per seconds
+            uy = dy / dt
+            dpcdt = dpc / (dt / 3600)  # pressure change per hour
+
             # Check to limit dpc which happens when pc is not know
             if dpcdt > 100 or dpcdt < -100:
                 dpcdt = 0
-                if self.debug == 1: print(' limited dpcdt to zero for it', it)
+                if self.debug == 1:
+                    print(" limited dpcdt to zero for it", it)
 
             # Check if all is OK
             if ux == 0 and uy == 0:
-                if self.debug == 1: print('ux or uy became 0, timestep it+1 and it-1 have exactly the same coordinate for it = ', it)
-            
-            
+                if self.debug == 1:
+                    print(
+                        "ux or uy became 0, timestep it+1 and it-1 have exactly the same coordinate for it = ",
+                        it,
+                    )
+
             # Estimate asymmetry
-            if self.asymmetry_option == 'schwerdt1979':
-                uabs    = np.sqrt(ux**2 + uy**2)    # forward speed using x and y components
-                c       = uabs/knots_to_ms          # convert back to kts
-                a       = 1.5*c**0.63               # Schwerdt (1979)
-                a       = a*knots_to_ms             # Convert to m/s
-                u_prop  = a*ux/uabs               
-                v_prop  = a*uy/uabs
-            elif self.asymmetry_option == 'mvo':
-                uabs    = np.sqrt(ux**2 + uy**2)    # forward speed using x and y components
-                c2      = 0.6
-                u_prop  = a*ux/uabs               
-                v_prop  = a*uy/uabs
-            elif self.asymmetry_option == 'none':
-                u_prop  = 0.0             
-                v_prop  = 0.0
+            if self.asymmetry_option == "schwerdt1979":
+                uabs = np.sqrt(
+                    ux**2 + uy**2
+                )  # forward speed using x and y components
+                c = uabs / knots_to_ms  # convert back to kts
+                a = 1.5 * c**0.63  # Schwerdt (1979)
+                a = a * knots_to_ms  # Convert to m/s
+                u_prop = a * ux / uabs
+                v_prop = a * uy / uabs
+            elif self.asymmetry_option == "mvo":
+                uabs = np.sqrt(
+                    ux**2 + uy**2
+                )  # forward speed using x and y components
+                c2 = 0.6
+                u_prop = a * ux / uabs
+                v_prop = a * uy / uabs
+            elif self.asymmetry_option == "none":
+                u_prop = 0.0
+                v_prop = 0.0
             else:
-                raise Exception('This asymmetry_option is not supported')
-            
+                raise Exception("This asymmetry_option is not supported")
+
             # Compute relative vmax
-            vmax_rel= self.track.vmax[it] - np.sqrt(u_prop**2 + v_prop**2)
-        
+            vmax_rel = self.track.vmax[it] - np.sqrt(u_prop**2 + v_prop**2)
+
             # Save as part of the track
-            self.track.vtx[it]          = ux            # forward speed in x
-            self.track.vty[it]          = uy            # forward speed in y
-            self.track.dpcdt[it]        = dpcdt         # pressure difference in time
-            self.track.vmax_rel[it]     = vmax_rel      # vmax corrected for asymmetry
-            
-        
+            self.track.vtx[it] = ux  # forward speed in x
+            self.track.vty[it] = uy  # forward speed in y
+            self.track.dpcdt[it] = dpcdt  # pressure difference in time
+            self.track.vmax_rel[it] = vmax_rel  # vmax corrected for asymmetry
+
             # Place wind radii in special structure  (only if wind is high enough)
             if self.track.vmax[it] > 15:
-                
                 # Note  first dimension area different radii (R35, R50, etc)        - irad
                 #       second dimension are the quadrants                          - iquad
                 # Set values for R35
                 if self.track.R35_NE[it] > 0:
-                    self.track.quadrants_radii[it][0,0] = self.track.R35_NE[it]
+                    self.track.quadrants_radii[it][0, 0] = self.track.R35_NE[it]
                 if self.track.R35_SE[it] > 0:
-                    self.track.quadrants_radii[it][0,1] = self.track.R35_SE[it]
+                    self.track.quadrants_radii[it][0, 1] = self.track.R35_SE[it]
                 if self.track.R35_SW[it] > 0:
-                    self.track.quadrants_radii[it][0,2] = self.track.R35_SW[it]
+                    self.track.quadrants_radii[it][0, 2] = self.track.R35_SW[it]
                 if self.track.R35_NW[it] > 0:
-                    self.track.quadrants_radii[it][0,3] = self.track.R35_NW[it]
-            
+                    self.track.quadrants_radii[it][0, 3] = self.track.R35_NW[it]
+
                 # Set values R50
                 if self.track.R50_NE[it] > 0:
-                    self.track.quadrants_radii[it][1,0] = self.track.R50_NE[it]
+                    self.track.quadrants_radii[it][1, 0] = self.track.R50_NE[it]
                 if self.track.R50_SE[it] > 0:
-                    self.track.quadrants_radii[it][1,1] = self.track.R50_SE[it]
+                    self.track.quadrants_radii[it][1, 1] = self.track.R50_SE[it]
                 if self.track.R50_SW[it] > 0:
-                    self.track.quadrants_radii[it][1,2] = self.track.R50_SW[it]
+                    self.track.quadrants_radii[it][1, 2] = self.track.R50_SW[it]
                 if self.track.R50_NW[it] > 0:
-                    self.track.quadrants_radii[it][1,3] = self.track.R50_NW[it]
-            
+                    self.track.quadrants_radii[it][1, 3] = self.track.R50_NW[it]
+
                 # Set values R65
                 if self.track.R65_NE[it] > 0:
-                    self.track.quadrants_radii[it][2,0] = self.track.R65_NE[it]
+                    self.track.quadrants_radii[it][2, 0] = self.track.R65_NE[it]
                 if self.track.R65_SE[it] > 0:
-                    self.track.quadrants_radii[it][2,1] = self.track.R65_SE[it]
+                    self.track.quadrants_radii[it][2, 1] = self.track.R65_SE[it]
                 if self.track.R65_SW[it] > 0:
-                    self.track.quadrants_radii[it][2,2] = self.track.R65_SW[it]
+                    self.track.quadrants_radii[it][2, 2] = self.track.R65_SW[it]
                 if self.track.R65_NW[it] > 0:
-                    self.track.quadrants_radii[it][2,3] = self.track.R65_NW[it]
-            
+                    self.track.quadrants_radii[it][2, 3] = self.track.R65_NW[it]
+
                 # Set values R100
                 if self.track.R100_NE[it] > 0:
-                    self.track.quadrants_radii[it][3,0] = self.track.R100_NE[it]
+                    self.track.quadrants_radii[it][3, 0] = self.track.R100_NE[it]
                 if self.track.R100_SE[it] > 0:
-                    self.track.quadrants_radii[it][3,1] = self.track.R100_SE[it]
+                    self.track.quadrants_radii[it][3, 1] = self.track.R100_SE[it]
                 if self.track.R100_SW[it] > 0:
-                    self.track.quadrants_radii[it][3,2] = self.track.R100_SW[it]
+                    self.track.quadrants_radii[it][3, 2] = self.track.R100_SW[it]
                 if self.track.R100_NW[it] > 0:
-                    self.track.quadrants_radii[it][3,3] = self.track.R100_NW[it]
+                    self.track.quadrants_radii[it][3, 3] = self.track.R100_NW[it]
 
-                
                 # First find directions of maximum wind speed in each quadrant
-                angles0b    = {}
-                anglesb     = {}
+                angles0b = {}
+                anglesb = {}
                 for ii in range(0, 4):
                     angles0b[ii] = []
                     anglesb[ii] = []
-                angles0b[0] = np.arange(90, 180+10, 10)     # ne
-                angles0b[1] = np.arange(0, 90+10, 10)       # se
-                angles0b[2] = np.arange(270, 360+10, 10)    # sw
-                angles0b[3] = np.arange(180, 270+10, 10)    # nw
+                angles0b[0] = np.arange(90, 180 + 10, 10)  # ne
+                angles0b[1] = np.arange(0, 90 + 10, 10)  # se
+                angles0b[2] = np.arange(270, 360 + 10, 10)  # sw
+                angles0b[3] = np.arange(180, 270 + 10, 10)  # nw
                 for iquad in range(0, 4):
                     if coords_it.y > 0:
-                        anglesb[iquad] = angles0b[iquad] + self.phi_spiral        # include spiralling effect
+                        anglesb[iquad] = (
+                            angles0b[iquad] + self.phi_spiral
+                        )  # include spiralling effect
                     else:
-                        anglesb[iquad] = angles0b[iquad] - self.phi_spiral        # include spiralling effect
-                        
-                    anglesb[iquad] = anglesb[iquad] * np.pi / 180                 # convert to radians
-                
-                
+                        anglesb[iquad] = (
+                            angles0b[iquad] - self.phi_spiral
+                        )  # include spiralling effect
+
+                    anglesb[iquad] = anglesb[iquad] * np.pi / 180  # convert to radians
+
                 # Go over quadrants: find angle with maximum winds flowing
                 angles = np.zeros((len(anglesb)))
-                for iquad in range(0,4):
-                    
+                for iquad in range(0, 4):
                     # Get ready
-                    uabs            = np.zeros((len(anglesb[iquad])))
-                    vabs            = np.zeros((len(anglesb[iquad])))
-                    abs_speed       = np.zeros((len(anglesb[iquad])))
-                    counter         = 0
-                    
+                    uabs = np.zeros((len(anglesb[iquad])))
+                    vabs = np.zeros((len(anglesb[iquad])))
+                    abs_speed = np.zeros((len(anglesb[iquad])))
+                    counter = 0
+
                     # Go over angles
                     for ii in anglesb[iquad]:
-                        uabs[counter]       = (35*knots_to_ms) * np.cos(ii)
-                        vabs[counter]       = (35*knots_to_ms) * np.sin(ii)
-                        uabs[counter]       = uabs[counter] + u_prop
-                        vabs[counter]       = vabs[counter] + v_prop
-                        abs_speed[counter]  = (np.sqrt(np.dot(uabs[counter], uabs[counter]) + np.dot(vabs[counter], vabs[counter])))
-                        counter             = counter + 1
-                        
-                    imax            = np.where(abs_speed == np.max(abs_speed))
+                        uabs[counter] = (35 * knots_to_ms) * np.cos(ii)
+                        vabs[counter] = (35 * knots_to_ms) * np.sin(ii)
+                        uabs[counter] = uabs[counter] + u_prop
+                        vabs[counter] = vabs[counter] + v_prop
+                        abs_speed[counter] = np.sqrt(
+                            np.dot(uabs[counter], uabs[counter])
+                            + np.dot(vabs[counter], vabs[counter])
+                        )
+                        counter = counter + 1
+
+                    imax = np.where(abs_speed == np.max(abs_speed))
                     if imax[0].size > 1:
                         imax = 0
-                        
-                    angles[iquad]   = angles0b[iquad][imax] * np.pi / 180
-                
-                
+
+                    angles[iquad] = angles0b[iquad][imax] * np.pi / 180
+
                 # Compute relative speed of all quadrants and radii
-                for irad in range(np.size(self.track.quadrants_speed[it],0)):
-                    for iquad in range(np.size(self.track.quadrants_speed[it],1)):
-                        uabs = self.track.quadrants_speed[it][irad,iquad] * np.cos(angles[iquad])
-                        vabs = self.track.quadrants_speed[it][irad,iquad] * np.sin(angles[iquad])
+                for irad in range(np.size(self.track.quadrants_speed[it], 0)):
+                    for iquad in range(np.size(self.track.quadrants_speed[it], 1)):
+                        uabs = self.track.quadrants_speed[it][irad, iquad] * np.cos(
+                            angles[iquad]
+                        )
+                        vabs = self.track.quadrants_speed[it][irad, iquad] * np.sin(
+                            angles[iquad]
+                        )
                         urel = uabs - u_prop
                         vrel = vabs - v_prop
-                        self.track.quadrants_speed[it][irad,iquad] = np.sqrt(urel**2  + vrel**2)
+                        self.track.quadrants_speed[it][irad, iquad] = np.sqrt(
+                            urel**2 + vrel**2
+                        )
 
         # Done with the time steps
-        if self.debug == 1: print('done with accounting for forward speed')
-
+        if self.debug == 1:
+            print("done with accounting for forward speed")
 
-
-    # Create and write-out spiderweb  
-    def to_spiderweb(self, filename):
-        
+    # Create and write-out spiderweb
+    def to_spiderweb(self, filename, progress_bar=None):
         # 1. convert units to km and m/s
         self.convert_units_imperial_metric()
-        
+
         # 2. estimate missing values
         self.account_for_forward_speed()
         self.estimate_missing_values()
-        
-        # 3. cut off track points with low wind speeds at beginning and end of track
+
+        # 3. cut off track points with low wind speeds at beginning and end of track + extent track
         self.cut_off_low_wind_speeds()
-        
+        self.extent_track()
+
         # 4. account for forward speed (computes several derivate values)
         self.account_for_forward_speed()
-        
+
         # 5. Define grid and output
-        spiderweb       = []
-        dx              = self.spiderweb_radius / self.nr_radial_bins
-        r               = np.arange(dx, self.spiderweb_radius+dx, dx)
-        dphi            = 360 /self.nr_directional_bins
-        phi             = np.arange(90, -270, -dphi)
+        spiderweb = []
+        dx = self.spiderweb_radius / self.nr_radial_bins
+        r = np.arange(dx, self.spiderweb_radius + dx, dx)
+        dphi = 360 / self.nr_directional_bins
+        phi = np.arange(90, -270, -dphi)
 
         # 6. Go over time steps in the track
         for it in range(len(self.track)):
-            
+#            print(str(it + 1) + " of " + str(len(self.track)))
+            if progress_bar:
+                progress_bar.set_value(it)
+                if progress_bar.was_canceled():
+                    return
             # Get values ready
-            dp      = self.background_pressure - self.track.pc[it]
-            vmax    = self.track.vmax[it]
-            pc      = self.track.pc[it]
-            rmax    = self.track.RMW[it]
-            pn      = self.background_pressure
-            rhoa    = self.rho_air
-            xn      = 0.5
-            coords  = self.track.geometry[it]            
-            lat     = coords.y
+            dp = self.background_pressure - self.track.pc[it]
+            vmax = self.track.vmax[it]
+            pc = self.track.pc[it]
+            rmax = self.track.RMW[it]
+            pn = self.background_pressure
+            rhoa = self.rho_air
+            xn = 0.5
+            coords = self.track.geometry[it]
+            lat = coords.y
 
             # Get derivate values
-            ux      = self.track.vtx[it]                                                            # forward speed - x 
-            uy      = self.track.vty[it]                                                            # forward speed - y  
-            vt      = np.sqrt(self.track.vtx[it]**2  + self.track.vty[it]**2)                       # forward speed - magnitude
-            phit    = np.arctan2(self.track.vty[it],self.track.vtx[it]) * 180 / np.pi               # angle
-            dpcdt   = self.track.dpcdt[it]                                                          # pressure gradient in time
-            vmax_rel= self.track.vmax_rel[it]                                                       # intensity corrected for forward motion
+            ux = self.track.vtx[it]  # forward speed - x
+            uy = self.track.vty[it]  # forward speed - y
+            vt = np.sqrt(
+                self.track.vtx[it] ** 2 + self.track.vty[it] ** 2
+            )  # forward speed - magnitude
+            phit = (
+                np.arctan2(self.track.vty[it], self.track.vtx[it]) * 180 / np.pi
+            )  # angle
+            dpcdt = self.track.dpcdt[it]  # pressure gradient in time
+            vmax_rel = self.track.vmax_rel[it]  # intensity corrected for forward motion
 
             # initialize arrays
-            wind_speed              = np.zeros((len(phi), len(r)))
-            wind_to_direction_cart  = np.zeros((len(phi), len(r)))
-            pressure_drop           = np.zeros((len(phi), len(r)))
-            rainfall_rate           = np.zeros((len(phi), len(r)))
-            spiderweb_dict          = {'wind_speed': wind_speed, 'wind_from_direction': wind_speed, 'pressure_drop': wind_speed, 'pressure_drop': wind_speed, 'rainfall': rainfall_rate}
+            wind_speed = np.zeros((len(phi), len(r)))
+            wind_to_direction_cart = np.zeros((len(phi), len(r)))
+            pressure_drop = np.zeros((len(phi), len(r)))
+            rainfall_rate = np.zeros((len(phi), len(r)))
+            spiderweb_dict = {
+                "wind_speed": wind_speed,
+                "wind_from_direction": wind_speed,
+                "pressure_drop": wind_speed,
+                "pressure_drop": wind_speed,
+                "rainfall": rainfall_rate,
+            }
 
             # Holland et al. 2010
-            if self.wind_profile == 'holland2010':
+            if self.wind_profile == "holland2010":
                 # either directionally uniform, or using r35, r50, r65, r100
-                
+
                 unidir = 0
-                n      = 0
+                n = 0
                 if vmax > 20:
-                    for iq in range(np.size(self.track.quadrants_speed[it],0)):
-                        for irad in range(np.size(self.track.quadrants_speed[it],1)):
-                            if not np.isnan(self.track.quadrants_radii[it][iq,irad]):
+                    for iq in range(np.size(self.track.quadrants_speed[it], 0)):
+                        for irad in range(np.size(self.track.quadrants_speed[it], 1)):
+                            if not np.isnan(self.track.quadrants_radii[it][iq, irad]):
                                 n = n + 1
                 if n == 0:
                     unidir = 1
-                
-                
+
                 # Do fitting of Holland 2010 xn
                 if not unidir:
-                    obs                         = {}
-                    obs['quadrants_radii']      = self.track.quadrants_radii[it]
-                    obs['quadrants_speed']      = self.track.quadrants_speed[it]
-                    wrad                        = np.array([35, 50, 65, 100])*knots_to_ms
-                    [xn, vtcor, phia]           = fit_wind_field_holland2010(vmax, rmax, pc, vt, phit, pn, self.phi_spiral, lat, dpcdt, obs, wrad)
-                    ux                          = vtcor * np.cos((phit + phia) * np.pi / 180)
-                    uy                          = vtcor * np.sin((phit + phia) * np.pi / 180)
-                    vmax_rel                    = vmax - vtcor
+                    obs = {}
+                    obs["quadrants_radii"] = self.track.quadrants_radii[it]
+                    obs["quadrants_speed"] = self.track.quadrants_speed[it]
+                    wrad = np.array([35, 50, 65, 100]) * knots_to_ms
+                    [xn, vtcor, phia] = fit_wind_field_holland2010(
+                        vmax,
+                        rmax,
+                        pc,
+                        vt,
+                        phit,
+                        pn,
+                        self.phi_spiral,
+                        lat,
+                        dpcdt,
+                        obs,
+                        wrad,
+                    )
+                    ux = vtcor * np.cos((phit + phia) * np.pi / 180)
+                    uy = vtcor * np.sin((phit + phia) * np.pi / 180)
+                    vmax_rel = vmax - vtcor
                     # print(xn)
-            
+
                 # Finally, fit profile
-                [vr, pr]    = holland2010(r, vmax_rel, pc, pn, rmax, dpcdt, lat, vt, xn)
+                [vr, pr] = holland2010(r, vmax_rel, pc, pn, rmax, dpcdt, lat, vt, xn)
 
-            
             # Assume constant xn that follows a relationship decribed in 2008 paper
-            elif self.wind_profile == 'holland2008':
-               xn          = 0.6 * (1 - dp / 215)
-               [vr, pr]    = holland2010(r, vmax_rel, pc, pn, rmax, dpcdt, lat, vt, xn)
+            elif self.wind_profile == "holland2008":
+                xn = 0.6 * (1 - dp / 215)
+                [vr, pr] = holland2010(r, vmax_rel, pc, pn, rmax, dpcdt, lat, vt, xn)
 
             # Orginal Holland uses a constant xn of 0.5
-            elif self.wind_profile == 'holland1980':
-                xn          = 0.5
-                [vr, pr]    = holland2010(r, vmax_rel, pc, pn, rmax, dpcdt, lat, vt, xn)
-                
+            elif self.wind_profile == "holland1980":
+                xn = 0.5
+                [vr, pr] = holland2010(r, vmax_rel, pc, pn, rmax, dpcdt, lat, vt, xn)
+
             else:
-                raise Exception('This wind_profile is not supported')
+                raise Exception("This wind_profile is not supported")
+
+            # Compute pressure drop
+            pd = pn - pr
 
-                
-            # Compute pressure drop    
-            pd          = pn - pr  
-            
             # Go over the different phi
             for iphi in range(len(phi)):
-            
-                # Place wind speed    
-                wind_speed[iphi,:] = vr
-                
+                # Place wind speed
+                wind_speed[iphi, :] = vr
+
                 # Check which hemisphere we are
                 if lat >= 0:
                     # northern hemisphere
-                    dr  = 90 + phi[iphi]  + self.phi_spiral
+                    dr = 90 + phi[iphi] + self.phi_spiral
                 else:
                     # southern hemisphere
-                    dr  = -90 + phi[iphi] - self.phi_spiral
+                    dr = -90 + phi[iphi] - self.phi_spiral
 
                 # Wind direction and pressure drop
-                wind_to_direction_cart[iphi,:]    = dr
-                pressure_drop[iphi,:]             = pd * 100 # convert from hPa to Pa
-            
-            
+                wind_to_direction_cart[iphi, :] = dr
+                pressure_drop[iphi, :] = pd * 100  # convert from hPa to Pa
+
             # Add asymmetry
-            if self.asymmetry_option == 'schwerdt1979':
-                uabs    = np.sqrt(ux**2 + uy**2)    # forward speed using x and y components
-                c       = uabs/knots_to_ms          # convert back to kts
-                a       = 1.5*c**0.63               # Schwerdt (1979)
-                a       = a*knots_to_ms             # Convert to m/s
-                u_prop  = a*ux/uabs               
-                v_prop  = a*uy/uabs
-            elif self.asymmetry_option == 'mvo':
-                uabs    = np.sqrt(ux**2 + uy**2)    # forward speed using x and y components
-                c2      = 0.6
-                u_prop  = a*ux/uabs               
-                v_prop  = a*uy/uabs
-            elif self.asymmetry_option == 'none':
-                u_prop  = 0.0             
-                v_prop  = 0.0
+            if self.asymmetry_option == "schwerdt1979":
+                uabs = np.sqrt(
+                    ux**2 + uy**2
+                )  # forward speed using x and y components
+                c = uabs / knots_to_ms  # convert back to kts
+                a = 1.5 * c**0.63  # Schwerdt (1979)
+                a = a * knots_to_ms  # Convert to m/s
+                u_prop = a * ux / uabs
+                v_prop = a * uy / uabs
+            elif self.asymmetry_option == "mvo":
+                uabs = np.sqrt(
+                    ux**2 + uy**2
+                )  # forward speed using x and y components
+                c2 = 0.6
+                u_prop = a * ux / uabs
+                v_prop = a * uy / uabs
+            elif self.asymmetry_option == "none":
+                u_prop = 0.0
+                v_prop = 0.0
             else:
-                raise Exception('This asymmetry_option is not supported')
-                
-            # wind speed with assymetry     
+                raise Exception("This asymmetry_option is not supported")
+
+            # wind speed with assymetry
             vx = wind_speed * np.cos(wind_to_direction_cart * np.pi / 180) + u_prop
             vy = wind_speed * np.sin(wind_to_direction_cart * np.pi / 180) + v_prop
 
             # Save all values
-            dr                  = 1.5*np.pi - np.arctan2(vy,vx)
-            wind_speed          = np.sqrt(vx**2 + vy**2)
-            wind_from_direction = 180 * dr/np.pi
+            dr = 1.5 * np.pi - np.arctan2(vy, vx)
+            wind_speed = np.sqrt(vx**2 + vy**2)
+            wind_from_direction = 180 * dr / np.pi
             wind_from_direction = np.remainder(wind_from_direction, 360)
 
             # Add rainfall (if we want)
             if self.include_rainfall == True:
-
                 # Add rainfall
-                if self.rainfall_relationship == 'ipet':
-
+                if self.rainfall_relationship == "ipet":
                     # IPET is a simple rainfall model relating pressure to rainfall rate
-                    pdef = pressure_drop[0,0]/100            # % Pa to hPa
+                    pdef = pressure_drop[0, 0] / 100  # % Pa to hPa
                     for ip in range(len(r)):
                         if r[ip] < rmax:
-                            rainfall_rate[:,ip] = 1.14 + (0.12*pdef)
+                            rainfall_rate[:, ip] = 1.14 + (0.12 * pdef)
                         else:
-                            rainfall_rate[:,ip] = (1.14 + (0.12*pdef)) * np.exp(-0.3*((r[ip]-rmax)/rmax))
-                
+                            rainfall_rate[:, ip] = (1.14 + (0.12 * pdef)) * np.exp(
+                                -0.3 * ((r[ip] - rmax) / rmax)
+                            )
+
                 # More options to be added later
                 # Bader, Bacla, etc.
 
             # Save into a dictonary for spiderweb
-            spiderweb_dict['wind_speed']           = wind_speed
-            spiderweb_dict['wind_from_direction']  = wind_from_direction
-            spiderweb_dict['pressure']             = pn - pressure_drop/100     # pa - hPa
-            spiderweb_dict['pressure_drop']        = pressure_drop
-            spiderweb_dict['rainfall_rate']        = rainfall_rate
+            spiderweb_dict["wind_speed"] = wind_speed
+            spiderweb_dict["wind_from_direction"] = wind_from_direction
+            spiderweb_dict["pressure"] = pn - pressure_drop / 100  # pa - hPa
+            spiderweb_dict["pressure_drop"] = pressure_drop
+            spiderweb_dict["rainfall_rate"] = (
+                rainfall_rate * self.rainfall_factor
+            )  # multiply with a constant factor
 
             # Add spiderweb_dict to list of spiderweb
             spiderweb.append(spiderweb_dict)
-            
 
         # Actual writing (spiderweb in ascii)
         self.write_spiderweb_ascii(spiderweb, filename)
 
         # clean-up the geopandas: remove numpy arrays
-        self.track.pop('quadrants_radii')
-        self.track.pop('quadrants_speed')
-        
+        self.track.pop("quadrants_radii")
+        self.track.pop("quadrants_speed")
+
         # End
         # we are now done
 
-
     # Write spiderweb functions
     def write_spiderweb_ascii(self, spiderweb, filename):
-        
         # Header information
-        vsn             = '1.03'
-        merge_frac      = []
-        gridunit        = 'degree'
-        
+        vsn = "1.03"
+        merge_frac = []
+        gridunit = "degree"
+
         # The rows and columns need to be switched for python
-        ncols, nrows    = np.shape(spiderweb[0]['wind_speed'])
-    
+        ncols, nrows = np.shape(spiderweb[0]["wind_speed"])
+
         # Create output
-        fid             = open(filename, 'w')
-        format1         = '{:<14} {:1} {:<} {:>} \n'
-        format2         = '{:<14} {:1} {:<} \n'
-    
+        fid = open(filename, "w")
+        format1 = "{:<14} {:1} {:<} {:>} \n"
+        format2 = "{:<14} {:1} {:<} \n"
+
         # Write header information
-        fid.write(format1.format('FileVersion', '=', vsn, '                            # Version of meteo input file, to check if the newest file format is used'))
-        fid.write(format2.format('filetype', '=', 'meteo_on_spiderweb_grid          # from TRACK file: trackfile.trk'))
-        fid.write(format2.format('NODATA_value', '=', '-999.000'))
-        fid.write(format1.format('n_cols', '=', str(ncols), '                   # Number of columns used for wind datafield'))
-        fid.write(format1.format('n_rows', '=', str(nrows), '                           # Number of rows used for wind datafield'))
-        fid.write(format2.format('grid_unit', '=', gridunit))
-        fid.write(format2.format('spw_radius', '=', str(self.spiderweb_radius*1000)))                   
-        fid.write(format2.format('spw_rad_unit', '=', 'm'))
+        fid.write(
+            format1.format(
+                "FileVersion",
+                "=",
+                vsn,
+                "                            # Version of meteo input file, to check if the newest file format is used",
+            )
+        )
+        fid.write(
+            format2.format(
+                "filetype",
+                "=",
+                "meteo_on_spiderweb_grid          # from TRACK file: trackfile.trk",
+            )
+        )
+        fid.write(format2.format("NODATA_value", "=", "-999.000"))
+        fid.write(
+            format1.format(
+                "n_cols",
+                "=",
+                str(ncols),
+                "                   # Number of columns used for wind datafield",
+            )
+        )
+        fid.write(
+            format1.format(
+                "n_rows",
+                "=",
+                str(nrows),
+                "                           # Number of rows used for wind datafield",
+            )
+        )
+        fid.write(format2.format("grid_unit", "=", gridunit))
+        fid.write(format2.format("spw_radius", "=", str(self.spiderweb_radius * 1000)))
+        fid.write(format2.format("spw_rad_unit", "=", "m"))
         if merge_frac:
-            fid.write(format2.format('spw_merge_frac', '=', str(merge_frac)))   
-        if self.include_rainfall == True:     
-            fid.write(format2.format('n_quantity', '=', '4'))
+            fid.write(format2.format("spw_merge_frac", "=", str(merge_frac)))
+        if self.include_rainfall == True:
+            fid.write(format2.format("n_quantity", "=", "4"))
         else:
-            fid.write(format2.format('n_quantity', '=', '3'))
-        fid.write(format2.format('quantity1', '=', 'wind_speed'))
-        fid.write(format2.format('quantity2', '=', 'wind_from_direction'))
-        fid.write(format2.format('quantity3', '=', 'p_drop'))
-        if self.include_rainfall == True: 
-            fid.write(format2.format('quantity4', '=', 'precipitation'))
-        fid.write(format2.format('unit1', '=', 'm s-1'))
-        fid.write(format2.format('unit2', '=', 'degree'))
-        fid.write(format2.format('unit3', '=', 'Pa'))
-        if self.include_rainfall == True: 
-            fid.write(format2.format('unit4', '=', 'mm/h'))
+            fid.write(format2.format("n_quantity", "=", "3"))
+        fid.write(format2.format("quantity1", "=", "wind_speed"))
+        fid.write(format2.format("quantity2", "=", "wind_from_direction"))
+        fid.write(format2.format("quantity3", "=", "p_drop"))
+        if self.include_rainfall == True:
+            fid.write(format2.format("quantity4", "=", "precipitation"))
+        fid.write(format2.format("unit1", "=", "m s-1"))
+        fid.write(format2.format("unit2", "=", "degree"))
+        fid.write(format2.format("unit3", "=", "Pa"))
+        if self.include_rainfall == True:
+            fid.write(format2.format("unit4", "=", "mm/h"))
 
-        # Go over the time steps            
+        # Go over the time steps
         for it in range(len(spiderweb)):
-            
             # Get time
-            datetime_it         = datetime.strptime(self.track.datetime[it], dateformat_module)
-            dt                  = datetime_it - self.reference_time
-            dt                  = dt.total_seconds() / 3600             # 60 seconds per hours
-            
+            datetime_it = datetime.strptime(self.track.datetime[it], dateformat_module)
+            dt = datetime_it - self.reference_time
+            dt = dt.total_seconds() / 60  # 60 seconds per hour
+
             # Get main variables
-            wind_speed          = spiderweb[it]['wind_speed'].transpose()
-            wind_from_direction = spiderweb[it]['wind_from_direction'].transpose()
-            pressure_drop       = spiderweb[it]['pressure_drop'].transpose()
-            rainfall_rate       = spiderweb[it]['rainfall_rate'].transpose()
+            wind_speed = spiderweb[it]["wind_speed"].transpose()
+            wind_from_direction = spiderweb[it]["wind_from_direction"].transpose()
+            pressure_drop = spiderweb[it]["pressure_drop"].transpose()
+            rainfall_rate = spiderweb[it]["rainfall_rate"].transpose()
 
             # Replace NaN with -999
-            wind_speed          = np.nan_to_num(wind_speed, nan=-999)
+            wind_speed = np.nan_to_num(wind_speed, nan=-999)
             wind_from_direction = np.nan_to_num(wind_from_direction, nan=-999)
-            pressure_drop       = np.nan_to_num(pressure_drop, nan=-999)
-            rainfall_rate       = np.nan_to_num(rainfall_rate, nan=-999)
+            pressure_drop = np.nan_to_num(pressure_drop, nan=-999)
+            rainfall_rate = np.nan_to_num(rainfall_rate, nan=-999)
 
             # Get coordinates
-            coords              = self.track.geometry[it]            
-            
-            # Print 
-            reference_time_str  = self.reference_time.strftime("%Y-%m-%d %H:%M:%S")
-            fid.write('{:<14} {:1} {:^10.2f} {:} {:} {:<6}'.format('TIME', '=', int(dt), 'hours since', reference_time_str, '+00:00'))
-            fid.write('\n')
-            fid.write(format2.format('x_spw_eye', '=', (round(coords.x,2))))
-            fid.write(format2.format('y_spw_eye', '=', (round(coords.y,2))))
-            fid.write(format2.format('p_drop_spw_eye', '=', (round(np.amax(pressure_drop),2))))
-                                                 
+            coords = self.track.geometry[it]
+
+            # Print
+            reference_time_str = self.reference_time.strftime("%Y-%m-%d %H:%M:%S")
+            fid.write(
+                "{:<14} {:1} {:^10.2f} {:} {:} {:<6}".format(
+                    "TIME", "=", int(dt), "minutes since", reference_time_str, "+00:00"
+                )
+            )
+            fid.write("\n")
+            fid.write(format2.format("x_spw_eye", "=", (round(coords.x, 2))))
+            fid.write(format2.format("y_spw_eye", "=", (round(coords.y, 2))))
+            fid.write(
+                format2.format(
+                    "p_drop_spw_eye", "=", (round(np.amax(pressure_drop), 2))
+                )
+            )
+
             # Save main variables
-            np.savetxt(fid, wind_speed, fmt='%9.2f')
-            np.savetxt(fid, wind_from_direction, fmt='%9.2f')
-            np.savetxt(fid, pressure_drop, fmt='%9.2f')
-            if self.include_rainfall == True: 
-                np.savetxt(fid, rainfall_rate, fmt='%9.2f')
-         
-        # We are done here    
-        fid.close()
-        if self.debug == 1: print('Succesfully written spiderweb to ' + filename)
+            np.savetxt(fid, wind_speed, fmt="%9.2f")
+            np.savetxt(fid, wind_from_direction, fmt="%9.2f")
+            np.savetxt(fid, pressure_drop, fmt="%9.2f")
+            if self.include_rainfall == True:
+                np.savetxt(fid, rainfall_rate, fmt="%9.2f")
 
+        # We are done here
+        fid.close()
+        if self.debug == 1:
+            print("Succesfully written spiderweb to " + filename)
 
 
-# Classes of classes       
+# Classes of classes
 class TropicalCycloneEnsemble:
-    
     # Init
-    def __init__(self,name=None,TropicalCyclone=None):
-        
+    def __init__(self, name=None, TropicalCyclone=None):
         # Main variables
         self.name                       = name                      # we give the TropicalCycloneEnsemble always a name
         self.number_of_realizations     = []                        # number of realisations
-        self.dt                         = '3H'                      # 3 hours
+        self.dt                         = 3                         # 3 hours
         self.debug                      = 0                         # do not show prints
+        self.include_best_track         = 0                         # ensemble member = 0 is actually the best track
+        self.calibration_mode           = 0                         # if in calibration - seed value is 1, otherwise random/default
 
         # Error statistics - based on NHC of 2018-2021
-        self.mean_abs_cte24             = 19.0397*nm_to_m           # mean absolute error in cross-track error (CTE)
-        self.sc_cte                     = 1.3253                    # auto-regression CTE
-        self.mean_abs_ate24             = 26.224*nm_to_m            # mean absolute error in along-track error (ATE)
-        self.sc_ate                     = 1.3432                    # auto-regression ATE
-        self.mean_abs_ve24              = 6.9858                    # mean absolute error in wind error (VE)
+        self.mean_abs_cte24             = 19.0397*nm_to_m           # mean absolute error in cross-track error (CTE) in meter
+        self.sc_cte                     = 1.3253                    # auto-regression CTE; typically >1
+        self.mean_abs_ate24             = 26.224*nm_to_m            # mean absolute error in along-track error (ATE) in meter
+        self.sc_ate                     = 1.3432                    # auto-regression ATE; typically >1
+        self.mean_abs_ve24              = 6.9858                    # mean absolute error in wind error (VE) in knots
         self.sc_ve                      = 1.0000                    # auto-regression VE = 1 = no auto-regression
-        
+        self.bias_ve                    = 0.0                       # bias per hour
+
         # Define best-track
-        self.best_track                 = TropicalCyclone
-        self.tstart                     = datetime.strptime(self.best_track.track.datetime[0], dateformat_module)
-        self.tend                       = datetime.strptime(self.best_track.track.datetime[len(self.best_track.track)-1], dateformat_module)
-        
-        # The actual ensemble members
-        self.members                    = []
+        self.best_track = TropicalCyclone
+        self.tstart = datetime.strptime(
+            self.best_track.track.datetime[0], dateformat_module
+        )  # starting time of the track
+        self.tstart_ensemble = datetime.strptime(
+            self.best_track.track.datetime[0], dateformat_module
+        )  # starting time of variability
+        self.tend = datetime.strptime(
+            self.best_track.track.datetime[len(self.best_track.track) - 1],
+            dateformat_module,
+        )
 
+        # The actual ensemble members
+        self.members = []
 
     # Compute ensemble member
     def compute_ensemble(self, number_of_realizations=None):
-        
         # First set time variables based on best track
-        if self.debug == 1: print('Started with making ensembles')
+        if self.debug == 1:
+            print("Started with making ensembles")
+        self.number_of_realizations = number_of_realizations
+
+        # Go over ensemble time steps
+        ensemble_time = []
+        current_time = self.tstart  # set the current time to the start time
+        delta = timedelta(
+            hours=self.dt
+        )  # create a timedelta object representing a 1 hour time difference
+        while current_time <= self.tend:  # loop until we reach the end time
+            ensemble_time.append(current_time)  # add the current time to the list
+            current_time += delta  # increment the current time by the time difference
+        ntpred = len(ensemble_time)
 
-        self.number_of_realizations     = number_of_realizations
-        ensemble_time                   = pd.date_range(start=self.tstart, end=self.tend, freq=self.dt)
-        ensemble_time                   = ensemble_time.tolist()
-        ntpred                          = len(ensemble_time)
-        
         # Go over time steps
-        best_track_time                 = []
-        best_track_lon                  = []
-        best_track_lat                  = []
-        best_track_vmax                 = []
+        best_track_time = []
+        best_track_lon = []
+        best_track_lat = []
+        best_track_vmax = []
         for it in range(len(self.best_track.track)):
-            coords_it       = self.best_track.track.geometry[it]   
+            coords_it = self.best_track.track.geometry[it]
             best_track_lon.append(coords_it.x)
             best_track_lat.append(coords_it.y)
-            best_track_vmax.append(self.best_track.track.vmax[it] )
-            best_track_time.append(datetime.strptime(self.best_track.track.datetime[it], dateformat_module))
-
-        # Spline to requested times 
-        best_track_time2                = [date.timestamp() for date in best_track_time]
-        ensemble_time2                  = [date.timestamp() for date in ensemble_time]
-        best_track_lon2                 = CubicSpline(best_track_time2,best_track_lon)
-        best_track_lon2                 = best_track_lon2(ensemble_time2)
-        best_track_lat2                 = CubicSpline(best_track_time2,best_track_lat)
-        best_track_lat2                 = best_track_lat2(ensemble_time2)
-        best_track_vmax2                = CubicSpline(best_track_time2,best_track_vmax)
-        best_track_vmax2                = best_track_vmax2(ensemble_time2)
+            best_track_vmax.append(self.best_track.track.vmax[it])
+            best_track_time.append(
+                datetime.strptime(self.best_track.track.datetime[it], dateformat_module)
+            )
+
+        # Spline to requested times
+        best_track_time2 = [date.timestamp() for date in best_track_time]
+        ensemble_time2 = [date.timestamp() for date in ensemble_time]
+
+        best_track_lon2 = CubicSpline(best_track_time2, best_track_lon)
+        best_track_lon2 = best_track_lon2(ensemble_time2)
+        best_track_lat2 = CubicSpline(best_track_time2, best_track_lat)
+        best_track_lat2 = best_track_lat2(ensemble_time2)
+        best_track_vmax2 = CubicSpline(best_track_time2, best_track_vmax)
+        best_track_vmax2 = best_track_vmax2(ensemble_time2)
 
         # Compute heading again
-        [forward_speed, heading]        = compute_forward_speed_heading(ensemble_time2,best_track_lon2, best_track_lat2)
+        [forward_speed, heading] = compute_forward_speed_heading(
+            ensemble_time2, best_track_lon2, best_track_lat2
+        )
 
         # Second, define all members with their first time step the same
-        self.members                     = []
-        for nn in range(self.number_of_realizations+1):
-            
+        self.members = []
+        for nn in range(self.number_of_realizations + 1):
             # Add best track
-            new_member          = TropicalCyclone(name='ensemble' + str(nn).zfill(5))
+            new_member = TropicalCyclone(name="ensemble" + str(nn).zfill(5))
 
             # Use settings from BTD
-            new_member.wind_profile               = self.best_track.wind_profile
-            new_member.wind_pressure_relation     = self.best_track.wind_pressure_relation
-            new_member.rmw_relation               = self.best_track.rmw_relation    
-            new_member.background_pressure        = self.best_track.background_pressure
-            new_member.phi_spiral                 = self.best_track.phi_spiral
-            new_member.wind_conversion_factor     = self.best_track.wind_conversion_factor
-            new_member.spiderweb_radius           = self.best_track.spiderweb_radius
-            new_member.nr_radial_bins             = self.best_track.nr_radial_bins
-            new_member.nr_directional_bins        = self.best_track.nr_directional_bins
-            new_member.debug                      = self.best_track.debug
-            new_member.low_wind_speeds_cut_off    = self.best_track.low_wind_speeds_cut_off
-            new_member.rho_air                    = self.best_track.rho_air
-            new_member.asymmetry_option           = self.best_track.asymmetry_option
-            new_member.reference_time             = self.best_track.reference_time
-            new_member.include_rainfall           = self.best_track.include_rainfall
-            new_member.rainfall_relationship      = self.best_track.rainfall_relationship
-            new_member.unit_intensity             = self.best_track.unit_intensity
-            new_member.unit_radii                 = self.best_track.unit_radii
-            new_member.EPSG                       = self.best_track.EPSG
-
-            # Replace track 
-            point               = Point(best_track_lon2[0],best_track_lat2[0])
-            gdf                 = gpd.GeoDataFrame({"datetime": [ensemble_time[0].strftime(dateformat_module)],"geometry": [point], "vmax": [best_track_vmax2[0]], "pc": [-999], "RMW": [-999],
-                                        "R35_NE":  [-999],  "R35_SE":  [-999], "R35_SW":  [-999],  "R35_NW": [-999],
-                                        "R50_NE":  [-999],  "R50_SE":  [-999], "R50_SW":  [-999],  "R50_NW": [-999],
-                                        "R65_NE":  [-999],  "R65_SE":  [-999], "R65_SW":  [-999],  "R65_NW": [-999],
-                                        "R100_NE": [-999], "R100_SE": [-999],"R100_SW": [-999], "R100_NW": [-999]})    
+            new_member.wind_profile = self.best_track.wind_profile
+            new_member.wind_pressure_relation = self.best_track.wind_pressure_relation
+            new_member.rmw_relation = self.best_track.rmw_relation
+            new_member.background_pressure = self.best_track.background_pressure
+            new_member.phi_spiral = self.best_track.phi_spiral
+            new_member.wind_conversion_factor = self.best_track.wind_conversion_factor
+            new_member.spiderweb_radius = self.best_track.spiderweb_radius
+            new_member.nr_radial_bins = self.best_track.nr_radial_bins
+            new_member.nr_directional_bins = self.best_track.nr_directional_bins
+            new_member.debug = self.best_track.debug
+            new_member.low_wind_speeds_cut_off = self.best_track.low_wind_speeds_cut_off
+            new_member.rho_air = self.best_track.rho_air
+            new_member.asymmetry_option = self.best_track.asymmetry_option
+            new_member.reference_time = self.best_track.reference_time
+            new_member.include_rainfall = self.best_track.include_rainfall
+            new_member.rainfall_relationship = self.best_track.rainfall_relationship
+            new_member.unit_intensity = self.best_track.unit_intensity
+            new_member.unit_radii = self.best_track.unit_radii
+            new_member.EPSG = self.best_track.EPSG
+
+            # Replace track
+            point = Point(best_track_lon2[0], best_track_lat2[0])
+            gdf = gpd.GeoDataFrame(
+                {
+                    "datetime": [ensemble_time[0].strftime(dateformat_module)],
+                    "geometry": [point],
+                    "vmax": [best_track_vmax2[0]],
+                    "pc": [-999],
+                    "RMW": [-999],
+                    "R35_NE": [-999],
+                    "R35_SE": [-999],
+                    "R35_SW": [-999],
+                    "R35_NW": [-999],
+                    "R50_NE": [-999],
+                    "R50_SE": [-999],
+                    "R50_SW": [-999],
+                    "R50_NW": [-999],
+                    "R65_NE": [-999],
+                    "R65_SE": [-999],
+                    "R65_SW": [-999],
+                    "R65_NW": [-999],
+                    "R100_NE": [-999],
+                    "R100_SE": [-999],
+                    "R100_SW": [-999],
+                    "R100_NW": [-999],
+                }
+            )
             gdf.set_crs(epsg=new_member.EPSG, inplace=True)
-            new_member.track    = pd.concat([new_member.track,gdf]) 
-            new_member.track    = new_member.track.reset_index(drop=True)
-            new_member.track    = new_member.track.drop([0])           # remove the dummy
-            new_member.track    = new_member.track.reset_index(drop=True)
+            new_member.track = pd.concat([new_member.track, gdf])
+            new_member.track = new_member.track.reset_index(drop=True)
+            new_member.track = new_member.track.drop([0])  # remove the dummy
+            new_member.track = new_member.track.reset_index(drop=True)
 
             # Append
             self.members.append(new_member)
 
         # Third, make variations - go over time
-        # not we are making number_of_realizations+1 since the first [0] will be the best-track
+        # note we are making number_of_realizations+1 since the first [0] will be the best-track
         dt_seconds          = ensemble_time2[1] - ensemble_time2[0]
         dtd                 = dt_seconds/86400
         ate_12              = np.zeros((1, self.number_of_realizations+1))
         cte_12              = np.zeros((1, self.number_of_realizations+1))
         ve_12               = np.zeros((1, self.number_of_realizations+1))
 
+        # Set seed value
+        if self.calibration_mode == 1:
+            if self.debug == 1: print(' we are using seed 1 - same values')
+            np.random.seed(1)
+        else:
+            if self.debug == 1: print(' we are using random seed')
+            np.random.seed()
+
         # Random error matrices from normal distribution  .
-        arnd0               = np.random.randn(ntpred,self.number_of_realizations+1) 
-        crnd0               = np.random.randn(ntpred, self.number_of_realizations+1)    
-        vrnd0               = np.random.randn(ntpred,self.number_of_realizations+1) 
+        arnd0 = np.random.randn(ntpred, self.number_of_realizations + 1)
+        crnd0 = np.random.randn(ntpred, self.number_of_realizations + 1)
+        vrnd0 = np.random.randn(ntpred, self.number_of_realizations + 1)
 
         # Rest
-        ate                 = np.zeros((ntpred, self.number_of_realizations+1))
-        cte                 = np.zeros((ntpred, self.number_of_realizations+1))
-        ve                  = np.zeros((ntpred, self.number_of_realizations+1))
-        ensemble_lon        = np.zeros((ntpred, self.number_of_realizations+1))
-        ensemble_lat        = np.zeros((ntpred, self.number_of_realizations+1))
-        ensemble_vmax       = np.zeros((ntpred, self.number_of_realizations+1))
+        ate = np.zeros((ntpred, self.number_of_realizations + 1))
+        cte = np.zeros((ntpred, self.number_of_realizations + 1))
+        ve = np.zeros((ntpred, self.number_of_realizations + 1))
+        ensemble_lon = np.zeros((ntpred, self.number_of_realizations + 1))
+        ensemble_lat = np.zeros((ntpred, self.number_of_realizations + 1))
+        ensemble_vmax = np.zeros((ntpred, self.number_of_realizations + 1))
 
         # Loop over time
+        forecast_timestep   = 0.0
         for it in range(0,len(ensemble_time2)):
-            
-            # First time step
-            if it == 0:
-                ensemble_lon[it,:]  = best_track_lon2[it]
-                ensemble_lat[it,:]  = best_track_lat2[it] 
-                ensemble_vmax[it,:] = best_track_vmax2[it] 
 
-            # Otherwise
-            else:
+            # If we want the variability
+            if (ensemble_time[it] > self.tstart_ensemble):
                 
                 # Correct for time   
                 tfac                = np.sqrt(dtd)
+                forecast_timestep   = forecast_timestep + dtd*24
                 
                 # go from mean absolute error to standard deviation
                 sigma_ate           = self.mean_abs_ate24/np.sqrt(2/np.pi)
                 sigma_cte           = self.mean_abs_cte24/np.sqrt(2/np.pi)
-                sigma_ve            = self.mean_abs_ve24/np.sqrt(2/np.pi)
+
+                # Check unit of intensity
+                if self.best_track.unit_intensity == 'knots':
+                    if self.debug == 1: print(' both best-track and ensemble are in knots')
+                    sigma_ve            = self.mean_abs_ve24/np.sqrt(2/np.pi)
+                else:
+                    if self.debug == 1: print(' issue - we are assuming track is in m/s and ensemble in knots')
+                    sigma_ve            = self.mean_abs_ve24*knots_to_ms/np.sqrt(2/np.pi)
 
                 # standard deviation scales with tfac
-                arnd                = tfac*sigma_ate*arnd0[it,:]
-                crnd                = tfac*sigma_cte*crnd0[it,:]
-                vrnd                = tfac*sigma_ve*vrnd0[it,:]
-                
+                arnd = tfac * sigma_ate * arnd0[it, :]
+                crnd = tfac * sigma_cte * crnd0[it, :]
+                vrnd = tfac * sigma_ve * vrnd0[it, :]
+
                 # Limit to -2 and +2 sigma
-                arnd                = np.maximum(np.minimum(arnd, 2*tfac*sigma_ate), -2*tfac*sigma_ate)
-                crnd                = np.maximum(np.minimum(crnd, 2*tfac*sigma_cte), -2*tfac*sigma_cte)
-                vrnd                = np.maximum(np.minimum(vrnd, 2*tfac*sigma_ve), -2*tfac*sigma_ve)
+                arnd = np.maximum(
+                    np.minimum(arnd, 2 * tfac * sigma_ate), -2 * tfac * sigma_ate
+                )
+                crnd = np.maximum(
+                    np.minimum(crnd, 2 * tfac * sigma_cte), -2 * tfac * sigma_cte
+                )
+                vrnd = np.maximum(
+                    np.minimum(vrnd, 2 * tfac * sigma_ve), -2 * tfac * sigma_ve
+                )
 
                 # Compute new track errors
-                at1                 = self.sc_ate**dtd
-                ate[it,:]           = at1 * ate_12 + arnd
-                ct1                 = self.sc_cte**dtd
-                cte[it,:]           = ct1 * cte_12 + crnd
+                at1 = self.sc_ate**dtd
+                ate[it, :] = at1 * ate_12 + arnd
+                ct1 = self.sc_cte**dtd
+                cte[it, :] = ct1 * cte_12 + crnd
 
                 # Compute new positions
                 abserr              = np.sqrt(ate[it,:]**2 + cte[it,:]**2)
                 phierr              = np.arctan2(-cte[it,:], ate[it,:])
                 phitot              = heading[it] + phierr
-                ensemble_lon[it,:]  = best_track_lon2[it] + abserr * np.cos(phitot) *np.cos(best_track_lat2[it]*np.pi/180)/111111
-                ensemble_lat[it,:]  = best_track_lat2[it] + abserr * np.sin(phitot)/111111
+                dx                  = abserr*np.cos(phitot)
+                dy                  = abserr*np.sin(phitot)
+                dx                  = dx / (111320.*np.cos(np.pi*best_track_lat2[it]/180))
+                dy                  = dy / 110540
+                ensemble_lon[it,:]  = best_track_lon2[it] + dx
+                ensemble_lat[it,:]  = best_track_lat2[it] + dy
 
                 # Do wind speed too
                 ve1                 = self.sc_ve**dtd
-                ve[it,:]            = ve1*ve_12 + vrnd
-                ensemble_vmax[it,:] = best_track_vmax2[it] + ve[it,:]
-                ensemble_vmax[it,:] = np.maximum(ensemble_vmax[it,:], 0)
+                ve[it,:]            = ve1*ve_12 + vrnd 
+                ensemble_vmax[it,:] = best_track_vmax2[it] + ve[it,:] + self.bias_ve*forecast_timestep
+                ensemble_vmax[it,:] = np.maximum(ensemble_vmax[it,:], 10.0)      # low of 10 knots (Beaufort = 3)
 
                 # Save errors from last iteration
-                ate_12  = ate[it,:]
-                cte_12  = cte[it,:]
-                ve_12   = ve[it,:]
+                ate_12              = ate[it,:]
+                cte_12              = cte[it,:]
+                ve_12               = ve[it,:]
+            
+            # Else we don't
+            else:
+                # And simply place the best-track here
+                ensemble_lon[it, :] = best_track_lon2[it]
+                ensemble_lat[it, :] = best_track_lat2[it]
+                ensemble_vmax[it, :] = best_track_vmax2[it]
 
         # Apply spatial smoothing on track data
-        factor                              = round(12/(dtd*24))
+        factor = round(12 / (dtd * 24))
         if factor > 1:
             for nn in range(self.number_of_realizations):
-                ensemble_lon[:,nn]     = uniform_filter1d(ensemble_lon[:,nn], size=factor)
-                ensemble_lat[:,nn]     = uniform_filter1d(ensemble_lat[:,nn], size=factor)
+                # Only apply this for the non-best-track-period
+                idwanted = np.zeros(len(ensemble_time), dtype=bool)
+                for dt in range(len(ensemble_time)):
+                    idwanted[dt] = ensemble_time[dt] > self.tstart_ensemble
+
+                # Apply this
+                ensemble_lon[idwanted, nn] = uniform_filter1d(
+                    ensemble_lon[idwanted, nn], size=factor
+                )
+                ensemble_lat[idwanted, nn] = uniform_filter1d(
+                    ensemble_lat[idwanted, nn], size=factor
+                )
 
         # Replace first one - that is the best-track
-        ensemble_lon[:,0]   = best_track_lon2
-        ensemble_lat[:,0]   = best_track_lat2
-        ensemble_vmax[:,0]  = best_track_vmax2
-
-        # The first step is all the same too => this shouldnt be needed...
-        ensemble_lon[0,:]   = best_track_lon2[0]
-        ensemble_lat[0,:]   = best_track_lat2[0]
-        ensemble_vmax[0,:]  = best_track_vmax2[0]
+        if self.include_best_track == 1:
+            ensemble_lon[:, 0] = best_track_lon2
+            ensemble_lat[:, 0] = best_track_lat2
+            ensemble_vmax[:, 0] = best_track_vmax2
 
         # Visual check
-        if self.debug == 1: 
+        if self.debug == 1:
             plt.plot(ensemble_time2, ensemble_vmax)
-            plt.plot(best_track_time2,best_track_vmax, '-k')
+            plt.plot(best_track_time2, best_track_vmax, "-k")
 
             plt.plot(ensemble_lon, ensemble_lat)
-            plt.plot(best_track_lon2,best_track_lat2, '-k')
+            plt.plot(best_track_lon2, best_track_lat2, "-k")
 
         # Place them in their geopandas track
         for nn, member in enumerate(self.members):
-
             # Add time stamps
-            for it in range(1,len(ensemble_time2)):
-                        
+            for it in range(1, len(ensemble_time2)):
                 # Make GeoDataFrame of this timestamp and track
-                point       = Point(ensemble_lon[it,nn],ensemble_lat[it,nn])
-                gdf         = gpd.GeoDataFrame({"datetime": [ensemble_time[it].strftime(dateformat_module)],"geometry": [point], "vmax": [ensemble_vmax[it,nn]], "pc": [-999], "RMW": [-999],
-                                            "R35_NE":  [-999],  "R35_SE":  [-999], "R35_SW":  [-999],  "R35_NW": [-999],
-                                            "R50_NE":  [-999],  "R50_SE":  [-999], "R50_SW":  [-999],  "R50_NW": [-999],
-                                            "R65_NE":  [-999],  "R65_SE":  [-999], "R65_SW":  [-999],  "R65_NW": [-999],
-                                            "R100_NE": [-999], "R100_SE": [-999],"R100_SW": [-999], "R100_NW": [-999]})    
+                point = Point(ensemble_lon[it, nn], ensemble_lat[it, nn])
+                gdf = gpd.GeoDataFrame(
+                    {
+                        "datetime": [ensemble_time[it].strftime(dateformat_module)],
+                        "geometry": [point],
+                        "vmax": [ensemble_vmax[it, nn]],
+                        "pc": [-999],
+                        "RMW": [-999],
+                        "R35_NE": [-999],
+                        "R35_SE": [-999],
+                        "R35_SW": [-999],
+                        "R35_NW": [-999],
+                        "R50_NE": [-999],
+                        "R50_SE": [-999],
+                        "R50_SW": [-999],
+                        "R50_NW": [-999],
+                        "R65_NE": [-999],
+                        "R65_SE": [-999],
+                        "R65_SW": [-999],
+                        "R65_NW": [-999],
+                        "R100_NE": [-999],
+                        "R100_SE": [-999],
+                        "R100_SW": [-999],
+                        "R100_NW": [-999],
+                    }
+                )
                 gdf.set_crs(epsg=4326, inplace=True)
-                self.members[nn].track = pd.concat([self.members[nn].track,gdf]) 
-                
+                self.members[nn].track = pd.concat([self.members[nn].track, gdf])
+
             # Done with this ensemble member
             self.members[nn].track        = self.members[nn].track.reset_index(drop=True)
             if self.debug == 1: print(self.members[nn].name)
         
-        # Are we done?
-        if self.debug == 1: print(' done with making ensemble members')
+        # Compute time axis
+        time_differences = []
+        for i in range(0, len(ensemble_time)):
+            time_diff = (ensemble_time[i] - ensemble_time[0]).total_seconds()
+            time_differences.append(time_diff/3600)       
+
+        # Keep track of the errors: give user access to these values
+        self.error_statistics_time      = time_differences
+        self.error_statistics_ate_all   = ate
+        self.error_statistics_ate_mean  = np.mean(abs(ate),1)/nm_to_m
+        self.error_statistics_cte_all   = cte
+        self.error_statistics_cte_mean  = np.mean(abs(cte),1)/nm_to_m
+        self.error_statistics_ve_all    = ve
+        self.error_statistics_ve_mean   = np.mean(abs(ve),1)
 
 
-    # Write out shapefile
-    def to_shapefile(self, folder_path):  
 
+        # Are we done?
+        if self.debug == 1:
+            print(" done with making ensemble members")
+
+    # Write out shapefile
+    def to_shapefile(self, folder_path):
         # Make path (if needed)
         os.makedirs(folder_path, exist_ok=True)
 
         # Get the tracks in line format
         lines = []
-        ids   = []
+        ids = []
         for nn, member in enumerate(self.members):
             coordinates = []
             for it in range(len(member.track)):
-                coordinates.append( (member.track.geometry[it].x, member.track.geometry[it].y) )
+                coordinates.append(
+                    (member.track.geometry[it].x, member.track.geometry[it].y)
+                )
             line = LineString(coordinates)
             lines.append(line)
             ids.append(member.name)
-        multilinestring = MultiLineString(lines)     
+        multilinestring = MultiLineString(lines)
 
         # Write out as shapefile
-        filename = os.path.join(folder_path, 'ensemble_members')
-        schema      = {'geometry': 'LineString', 'properties': {'id': 'int'}}
-        with fiona.open(filename, 'w', 'ESRI Shapefile', schema) as c:
+        filename = os.path.join(folder_path, "ensemble_members")
+        schema = {"geometry": "LineString", "properties": {"id": "int"}}
+        with fiona.open(filename, "w", "ESRI Shapefile", schema) as c:
             counter = 0
             for linestring in multilinestring.geoms:
                 # Write the linestring to the shapefile
-                c.write({'geometry': mapping(linestring), 'properties': {'id': counter}})
+                c.write(
+                    {"geometry": mapping(linestring), "properties": {"id": counter}}
+                )
                 counter += 1
 
+    # Write out shapefile
+    def get_feature_collection(self):
 
-    # Write them out to a spiderweb
-    def to_spiderweb(self, folder_path):  
+        # Get the tracks in line format
+        lines = []
+        ids = []
+        for nn, member in enumerate(self.members):
+            coordinates = []
+            for it in range(len(member.track)):
+                coordinates.append(
+                    (member.track.geometry[it].x, member.track.geometry[it].y)
+                )
+            line = LineString(coordinates)
+            lines.append(line)
+            ids.append(member.name)
+        multilinestring = MultiLineString(lines)
+
+        # Write multilinestring to geojson
+        features = []
+        features.append(Feature(geometry=multilinestring))
+        feature_collection = FeatureCollection(features)
+
+        return feature_collection
 
+    # Write them out to a spiderweb
+    def to_spiderweb(self, folder_path):
         # Make path (if needed)
         os.makedirs(folder_path, exist_ok=True)
 
         # Loop over ensemble members and write them out
         for member in self.members:
-            filename = os.path.join(folder_path, member.name)
+            filename = os.path.join(folder_path, member.name)  # combine paths
+            filename = filename + ".spw"  # add spiderweb extension
             member.to_spiderweb(filename)
 
+    # Make output with cyc
+    def to_cyc(self, folder_path):
+        # Make path (if needed)
+        os.makedirs(folder_path, exist_ok=True)
+
+        # Loop over ensemble members and write them out
+        for member in self.members:
+            filename = os.path.join(folder_path, member.name)  # combine paths
+            filename = filename + ".cyc"  # add cyc extension
+            member.write_track(filename, "ddb_cyc")
+
+    def get_outline(self, buffer=300000.0):
+        # Generate gdf with outline of all ensemble members
+        pols = []
+        for member in self.members:
+            # Loop through all points to make linestring
+            coordinates = []
+            for it in range(len(member.track)):
+                coordinates.append(
+                    (member.track.geometry[it].x, member.track.geometry[it].y)
+                )
+            line = LineString(coordinates)
+            line = gpd.GeoDataFrame({"geometry": [line]}).set_crs(4326).to_crs(3857).iloc[0]["geometry"]
+            pol = line.buffer(buffer).simplify(0.1)
+            pols.append(pol)
+        outline_geom = shapely.unary_union(pols)    
+        gdf = gpd.GeoDataFrame({"geometry": [outline_geom]}).set_crs(3857).to_crs(4326)
+        self.outline = gdf
+        return gdf
+
 
-    # Make visual of all the tracks 
-    def make_figures(self, folder_path):  
 
+    # Make visual of all the tracks
+    def make_figures(self, folder_path):
         # Make path (if needed)
         os.makedirs(folder_path, exist_ok=True)
 
         # Get times
         datetime_ensemble = []
         for it in range(len(self.members[0].track)):
-            datetime_ensemble.append(datetime.strptime(self.members[0].track.datetime[it], dateformat_module))
+            datetime_ensemble.append(
+                datetime.strptime(self.members[0].track.datetime[it], dateformat_module)
+            )
 
         # Show wind speeds
         for nn, member in enumerate(self.members):
-            plt.plot(datetime_ensemble,member.track.vmax)
+            plt.plot(datetime_ensemble, member.track.vmax)
         plt.show()
 
-   
-            
+
 ######
 # Definitions that I want to be available in general
 ######
 # Definitions to compute Holland 2010 (1D)
 def holland2010(r, vms, pc, pn, rmax, dpdt, lat, vt, xn):
     """
     Returning the one-dimensional Holland et al. (2010) parametric wind profile
-    
+
     Parameters
     ----------
     r : radius in km
     etc etc.
-    
+
     """
     # calculate Holland b parameter based on Holland (2008) - assume Dvorak method
     dp = max(pn - pc, 1)
-    x = 0.6 * (1 - dp/215)
+    x = 0.6 * (1 - dp / 215)
     if np.isnan(dpdt):
         dpdt = 0
-    b = -4.4 * 10**-5 * dp**2 + 0.01 * dp + 0.03 * dpdt - 0.014 * abs(lat) + 0.15 * vt**x + 1
-    b = min(np.nanmax(np.append(b, 1)), 2) # numerical limits
-    
+    b = (
+        -4.4 * 10**-5 * dp**2
+        + 0.01 * dp
+        + 0.03 * dpdt
+        - 0.014 * abs(lat)
+        + 0.15 * vt**x
+        + 1
+    )
+    b = min(np.nanmax(np.append(b, 1)), 2)  # numerical limits
+
     # initialise
-    x   = np.zeros(np.size(r)) + xn
-    pr  = np.zeros((np.size(r)))
-    vr  = np.zeros((np.size(r)))
-    
-    # Compute 
+    x = np.zeros(np.size(r)) + xn
+    pr = np.zeros((np.size(r)))
+    vr = np.zeros((np.size(r)))
+
+    # Compute
     index = r <= rmax
     x[index] = 0.5
-    rp = (rmax/r)**b
-    pr = pc + dp*np.exp(-rp)
-    vr = vms * (rp * np.exp(1.0 - rp))**x
-        
+    rp = (rmax / r) ** b
+    pr = pc + dp * np.exp(-rp)
+    vr = vms * (rp * np.exp(1.0 - rp)) ** x
+
     # output
     return [vr, pr]
 
 
-
 # Definitiaton for wind radii
 def wind_radii_nederhoff(vmax, lat, region, probability):
     """
     Returning the estimates of radius of maximum winds (RMW)
     and estimates of gale force winds (R35)
-    
+
     Parameters
     ----------
     vmax    : wind speed intensity in m/s - 1-minute average
     lat     : latitude in degrees
     region  : see paper for details
     probability: integer - 0 only mode; 1 = 1000 values
-    
+
     Returns
     -------
     rmax    : dictonary with mode and possible more
     r35     : ''
     """
     # radius of maximum winds (rmw or rmax)
     # 1. coefficients for A
-    coefficients_a      = np.array([  0.306982540000000,
-                            0.338409237000000,
-                            0.342791450000000,
-                            0.363546490000000,
-                            0.358572938000000,
-                            0.310729085000000,
-                            0.395431764000000,
-                            0.370190027000000])
-    
-    
-    # 2. coefficients for B        
-    coefficients_b      = np.array([[132.411906200000,	14.5640379700000,	-0.00259703300000000,	20.3808036500000], 
-                         [229.245844100000,	9.53865069100000,	0.00398810500000000,	28.4457367200000], 
-                         [85.2576655100000,	30.6920872600000,	0.00243248000000000,	5.78116540600000],
-                         [127.833300700000,	11.8474757400000,	0.0159363120000000,	    25.4682000500000],
-                         [153.733294700000,	11.4788885400000,	0.00747119300000000,	28.9489788700000],
-                         [261.528874200000,	7.01151785400000,	0.0261912560000000,	    29.2022787100000],
-                         [19.0899242800000,	24.0885573100000,	0.106240340000000,	    23.1802014600000],
-                         [44.8241743300000,	23.3717128800000,	0.0304690570000000,	    22.4282036100000],
-                         ])
-
+    coefficients_a = np.array(
+        [
+            0.306982540000000,
+            0.338409237000000,
+            0.342791450000000,
+            0.363546490000000,
+            0.358572938000000,
+            0.310729085000000,
+            0.395431764000000,
+            0.370190027000000,
+        ]
+    )
+
+    # 2. coefficients for B
+    coefficients_b = np.array(
+        [
+            [
+                132.411906200000,
+                14.5640379700000,
+                -0.00259703300000000,
+                20.3808036500000,
+            ],
+            [229.245844100000, 9.53865069100000, 0.00398810500000000, 28.4457367200000],
+            [85.2576655100000, 30.6920872600000, 0.00243248000000000, 5.78116540600000],
+            [127.833300700000, 11.8474757400000, 0.0159363120000000, 25.4682000500000],
+            [153.733294700000, 11.4788885400000, 0.00747119300000000, 28.9489788700000],
+            [261.528874200000, 7.01151785400000, 0.0261912560000000, 29.2022787100000],
+            [19.0899242800000, 24.0885573100000, 0.106240340000000, 23.1802014600000],
+            [44.8241743300000, 23.3717128800000, 0.0304690570000000, 22.4282036100000],
+        ]
+    )
 
     # 3. get the best guess for a and b given wind speed and latitude
-    a_value     = coefficients_a[region]
-    b_value     = coefficients_b[region, 0] * np.exp(-vmax / coefficients_b[region, 1]) * (1 + coefficients_b[region, 2] * abs(lat)) + coefficients_b[region, 3]
-    
+    a_value = coefficients_a[region]
+    b_value = (
+        coefficients_b[region, 0]
+        * np.exp(-vmax / coefficients_b[region, 1])
+        * (1 + coefficients_b[region, 2] * abs(lat))
+        + coefficients_b[region, 3]
+    )
+
     rmax = {}
-    rmax['mode'] = {}
-    rmax['mean'] = {}
-    rmax['median'] = {}
-    rmax['lowest'] = {}
-    rmax['highest'] = {}
-    rmax['numbers'] = {}
-    
+    rmax["mode"] = {}
+    rmax["mean"] = {}
+    rmax["median"] = {}
+    rmax["lowest"] = {}
+    rmax["highest"] = {}
+    rmax["numbers"] = {}
+
     # 4. compute 1000 delta r35 values
-    rmax['mode'] = np.exp(np.log(b_value) - a_value**2)
+    rmax["mode"] = np.exp(np.log(b_value) - a_value**2)
     if probability == 1:
-        numbers             = np.sort(np.exp(np.random.normal(size = (1000, 1)) * a_value + np.log(b_value)))
-        rmax['mean']        = np.mean(numbers)
-        rmax['median']      = np.median(numbers)
-        rmax['lowest']      = numbers[int(0.05 * len(numbers))][0]
-        rmax['highest']     = numbers[int(0.95 * len(numbers))][0]
-        rmax['numbers']     = np.sort(numbers)
-            
+        numbers = np.sort(
+            np.exp(np.random.normal(size=(1000, 1)) * a_value + np.log(b_value))
+        )
+        rmax["mean"] = np.mean(numbers)
+        rmax["median"] = np.median(numbers)
+        rmax["lowest"] = numbers[int(0.05 * len(numbers))][0]
+        rmax["highest"] = numbers[int(0.95 * len(numbers))][0]
+        rmax["numbers"] = np.sort(numbers)
+
     # delta radius of 35 knots (r35)
-    dr35                = {}
-    dr35['mode']        = {}
-    dr35['mean']        = {}
-    dr35['median']      = {}
-    dr35['lowest']      = {}
-    dr35['highest']     = {}
-    dr35['numbers']     = {}
-    
+    dr35 = {}
+    dr35["mode"] = {}
+    dr35["mean"] = {}
+    dr35["median"] = {}
+    dr35["lowest"] = {}
+    dr35["highest"] = {}
+    dr35["numbers"] = {}
+
     # Only if wind speed is more than 20 m/s
     if vmax > 20:
-
         # 1. coefficients for a
-        coefficients_a = np.array([[0.121563729, -0.052184289, 0.032953813], 
-                                   [0.131188105, -0.044389473, 0.002253258], 
-                                   [0.122286754, -0.045355772, 0.013286154], 
-                                   [0.120490659, -0.035029431, -0.005249445], 
-                                   [0.156059522, -0.041685377, 0.004952978], 
-                                   [-0.251333213, -0.009072243, -0.00506365], 
-                                   [0.131903526, -0.042096876, 0.012443195], 
-                                   [0.190044585, -0.044602083, 0.006117124]])
-        
+        coefficients_a = np.array(
+            [
+                [0.121563729, -0.052184289, 0.032953813],
+                [0.131188105, -0.044389473, 0.002253258],
+                [0.122286754, -0.045355772, 0.013286154],
+                [0.120490659, -0.035029431, -0.005249445],
+                [0.156059522, -0.041685377, 0.004952978],
+                [-0.251333213, -0.009072243, -0.00506365],
+                [0.131903526, -0.042096876, 0.012443195],
+                [0.190044585, -0.044602083, 0.006117124],
+            ]
+        )
+
         # 2. coefficients for b
-        coefficients_b = np.array([[30.92867473, 0.530681714, -0.012001645], 
-                                   [30.21210133, 0.414897465, 0.021689596], 
-                                   [26.58686237, 0.425916004, 0.028547278], 
-                                   [23.88007085, 0.43109144, 0.038119083], 
-                                   [33.26829485, 0.42859578, 0.017209431], 
-                                   [18.11013691, 0.486399912, 0.02955688], 
-                                   [16.9973011, 0.453713419, 0.054643743], 
-                                   [29.61141102, 0.4132484, 0.024418947]])
-        
+        coefficients_b = np.array(
+            [
+                [30.92867473, 0.530681714, -0.012001645],
+                [30.21210133, 0.414897465, 0.021689596],
+                [26.58686237, 0.425916004, 0.028547278],
+                [23.88007085, 0.43109144, 0.038119083],
+                [33.26829485, 0.42859578, 0.017209431],
+                [18.11013691, 0.486399912, 0.02955688],
+                [16.9973011, 0.453713419, 0.054643743],
+                [29.61141102, 0.4132484, 0.024418947],
+            ]
+        )
+
         # 3. get the best guess for a and b given wind speed and latitude
-        a_value = coefficients_a[region, 0] + np.exp(vmax * coefficients_a[region, 1]) * (1 + coefficients_a[region, 2] * abs(lat))
-        b_value = coefficients_b[region, 0] + (vmax - 18)**coefficients_b[region, 1] * (1 + coefficients_b[region, 2] * abs(lat))
+        a_value = coefficients_a[region, 0] + np.exp(
+            vmax * coefficients_a[region, 1]
+        ) * (1 + coefficients_a[region, 2] * abs(lat))
+        b_value = coefficients_b[region, 0] + (vmax - 18) ** coefficients_b[
+            region, 1
+        ] * (1 + coefficients_b[region, 2] * abs(lat))
 
         # 4. compute 1000 delta r35 values
-        dr35['mode']    = np.exp(np.log(b_value) - a_value**2)
+        dr35["mode"] = np.exp(np.log(b_value) - a_value**2)
         if probability == 1:
-            numbers             = np.sort(np.exp(np.random.normal(size = (1000, 1)) * a_value + np.log(b_value)))
-            dr35['mean']        = np.mean(numbers)
-            dr35['median']      = np.median(numbers)
-            dr35['lowest']      = numbers[int(0.05 * len(numbers))][0]
-            dr35['highest']     = numbers[int(0.95 * len(numbers))][0]
-            dr35['numbers']     = np.sort(numbers)
-    
-            
+            numbers = np.sort(
+                np.exp(np.random.normal(size=(1000, 1)) * a_value + np.log(b_value))
+            )
+            dr35["mean"] = np.mean(numbers)
+            dr35["median"] = np.median(numbers)
+            dr35["lowest"] = numbers[int(0.05 * len(numbers))][0]
+            dr35["highest"] = numbers[int(0.95 * len(numbers))][0]
+            dr35["numbers"] = np.sort(numbers)
+
     # output
     return [rmax, dr35]
 
 
 # Definition to compute wind-pressure relation to determine the vmax or the pressure drop
-def wpr_holland2008(pc = None, pn = None, phi = None, vt = None, dpcdt = None, 
-        rhoa = None, SST = None, vmax = None):
-                
+def wpr_holland2008(
+    pc=None, pn=None, phi=None, vt=None, dpcdt=None, rhoa=None, SST=None, vmax=None
+):
     # used when pc needs to be determined
     if not rhoa:
         if vmax:
             dp1 = np.arange(1, 151 + 5, 5)
             pc1 = pn - dp1
         else:
             dp1 = pn - pc
             pc1 = pc
-        
+
         if not SST:
-            Ts = 28.0 - 3*(phi - 10) / 20 # surface temperature
+            Ts = 28.0 - 3 * (phi - 10) / 20  # surface temperature
         else:
             Ts = SST - 1
-        
+
         prmw = pc1 + dp1 / 3.7
-        qm = 0.9 * (3.802 / prmw) * np.exp(17.67 * Ts / (243.5 + Ts)) # vapor pressure
-        Tvs = (Ts + 273.15) * (1.0 + 0.81 * qm) # virtual surface air temperature
+        qm = 0.9 * (3.802 / prmw) * np.exp(17.67 * Ts / (243.5 + Ts))  # vapor pressure
+        Tvs = (Ts + 273.15) * (1.0 + 0.81 * qm)  # virtual surface air temperature
         Rspecific = 287.058
         rhoa = 100 * pc1 / (Rspecific * Tvs)
-        
+
     # vmax to be determined
     if not vmax:
         dp = pn - pc
         x = 0.6 * (1 - dp / 215)
-        bs = -4.4e-5 * dp**2 + 0.01 * dp + 0.03 * dpcdt - 0.014 * phi + 0.15 * vt**x + 1.0
+        bs = (
+            -4.4e-5 * dp**2
+            + 0.01 * dp
+            + 0.03 * dpcdt
+            - 0.014 * phi
+            + 0.15 * vt**x
+            + 1.0
+        )
         vmax = np.sqrt(100 * bs * dp / (rhoa * np.e))
         output = vmax
     else:
         vtkmh = vt * 3.6
         vmaxkmh = vmax * 3.6 * 0.88
-        dp = 0.00592 * (1 - 0.0687 * vtkmh**0.33) * (1 + 0.00285 * abs(phi)**1.35) * vmaxkmh**1.81
+        dp = (
+            0.00592
+            * (1 - 0.0687 * vtkmh**0.33)
+            * (1 + 0.00285 * abs(phi) ** 1.35)
+            * vmaxkmh**1.81
+        )
         output = pn - dp
-        
-    return output
 
+    return output
 
 
-# Definition to fit Holland 2010 wind field 
-def fit_wind_field_holland2010(vmax, rmax, pc, vtreal, phit, pn, phi_spiral, lat, dpdt, obs, wrad):
-    
+# Definition to fit Holland 2010 wind field
+def fit_wind_field_holland2010(
+    vmax, rmax, pc, vtreal, phit, pn, phi_spiral, lat, dpdt, obs, wrad
+):
     # Discussion
     # shouldnt we have a switch to only calibrate vt and phi_a for observed radii
     # what about limits on these variables
     # OK with xn calibration
-    
-    # function to fit wind field based on Holland 2010    
+
+    # function to fit wind field based on Holland 2010
     size_factor = 1
-    phi         = np.arange(90, -270-10, -10) # radial angles (cartesian, degrees)
-    rmax        = rmax * 1000 # convert from km to m
-    r           = np.arange(4000, 1000000+4000, 4000)
-    
+    phi = np.arange(90, -270 - 10, -10)  # radial angles (cartesian, degrees)
+    rmax = rmax * 1000  # convert from km to m
+    r = np.arange(4000, 1000000 + 4000, 4000)
+
     # first estimates
-    xn          = 0.5
-    vt          = 0.6 * vtreal
-    
+    xn = 0.5
+    vt = 0.6 * vtreal
+
     if lat > 0:
-        phia = 45 # angle with respect to track angle (cartesian degrees, i.e. couter-clockwise)
+        phia = 45  # angle with respect to track angle (cartesian degrees, i.e. couter-clockwise)
     else:
         phia = -45
-        
+
     # More variables
-    dxn     = 0.01
-    dvt     = 0.5
-    dphia   = 5
-    nrad    = 2
-    nobs    = 0
-    
-    for irad in range(np.size(obs['quadrants_radii'],0)):
-        for iquad in range(np.size(obs['quadrants_radii'],1)):
-            if not np.isnan(obs['quadrants_radii'][irad,iquad]):
-                nobs = nobs+1
-                
+    dxn = 0.01
+    dvt = 0.5
+    dphia = 5
+    nrad = 2
+    nobs = 0
+
+    for irad in range(np.size(obs["quadrants_radii"], 0)):
+        for iquad in range(np.size(obs["quadrants_radii"], 1)):
+            if not np.isnan(obs["quadrants_radii"][irad, iquad]):
+                nobs = nobs + 1
+
     # just for plotting
     xx = np.zeros((len(phi), len(r)))
     yy = np.zeros((len(phi), len(r)))
     # plt.pcolor(xx,yy,w)
-    
+
     for j in range(len(phi)):
         for h in range(len(r)):
-            xx[j,h] = 0.001 * r[h] * np.cos(phi[j] * np.pi / 180)
-            yy[j,h] = 0.001 * r[h] * np.sin(phi[j] * np.pi / 180)
-    
-    if nobs > 0 and vmax > 21:
+            xx[j, h] = 0.001 * r[h] * np.cos(phi[j] * np.pi / 180)
+            yy[j, h] = 0.001 * r[h] * np.sin(phi[j] * np.pi / 180)
 
-        # Do three fits      
+    if nobs > 0 and vmax > 21.0:
+        # Do three fits
         for irep in range(3):
-            
             # Default fit
-            w = compute_wind_field(r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn, vt, phia)
+            w = compute_wind_field(
+                r,
+                phi,
+                vmax,
+                pc,
+                rmax,
+                pn,
+                vtreal,
+                phit,
+                lat,
+                dpdt,
+                phi_spiral,
+                xn,
+                vt,
+                phia,
+            )
             [mean_error, rms_error, err] = compute_mean_error(r, w, obs, wrad)
             nit = 0
-            
+
             # 1) now first adjust size of storm with xn
             while True:
                 nit = nit + 1
-                wu = compute_wind_field(r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn+dxn, vt, phia)
-                [mean_error_u, rms_error_u, err_u] = compute_mean_error(r, wu, obs, wrad)
-                wd = compute_wind_field(r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn-dxn, vt, phia)
-                [mean_error_d, rms_error_d, err_d] = compute_mean_error(r, wd, obs, wrad)
-                
+                wu = compute_wind_field(
+                    r,
+                    phi,
+                    vmax,
+                    pc,
+                    rmax,
+                    pn,
+                    vtreal,
+                    phit,
+                    lat,
+                    dpdt,
+                    phi_spiral,
+                    xn + dxn,
+                    vt,
+                    phia,
+                )
+                [mean_error_u, rms_error_u, err_u] = compute_mean_error(
+                    r, wu, obs, wrad
+                )
+                wd = compute_wind_field(
+                    r,
+                    phi,
+                    vmax,
+                    pc,
+                    rmax,
+                    pn,
+                    vtreal,
+                    phit,
+                    lat,
+                    dpdt,
+                    phi_spiral,
+                    xn - dxn,
+                    vt,
+                    phia,
+                )
+                [mean_error_d, rms_error_d, err_d] = compute_mean_error(
+                    r, wd, obs, wrad
+                )
+
                 # better with larger value of xn
                 if rms_error_u < rms_error:
                     xn = xn + dxn
                     rms_error = rms_error_u
-                    
-                # better with smaller value of xn    
+
+                # better with smaller value of xn
                 elif rms_error_d < rms_error:
                     xn = xn - dxn
                     rms_error = rms_error_d
-                
+
                 # optimum reached
                 else:
                     break
-                
+
                 # Other criteria
                 if xn < 0.3 or xn > 1.0:
                     break
                 if nit > 100:
                     break
-                
+
             nit = 0
-            
+
             # 2) now the asymmetry magnitude
             while True:
                 nit = nit + 1
-                wu = compute_wind_field(r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn, vt+dvt, phia)
-                [mean_error_u, rms_error_u, err_u] = compute_mean_error(r, wu, obs, wrad)
-                wd = compute_wind_field(r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn, vt-dvt, phia)
-                [mean_error_d, rms_error_d, err_d] = compute_mean_error(r, wd, obs, wrad)
-                
+                wu = compute_wind_field(
+                    r,
+                    phi,
+                    vmax,
+                    pc,
+                    rmax,
+                    pn,
+                    vtreal,
+                    phit,
+                    lat,
+                    dpdt,
+                    phi_spiral,
+                    xn,
+                    vt + dvt,
+                    phia,
+                )
+                [mean_error_u, rms_error_u, err_u] = compute_mean_error(
+                    r, wu, obs, wrad
+                )
+                wd = compute_wind_field(
+                    r,
+                    phi,
+                    vmax,
+                    pc,
+                    rmax,
+                    pn,
+                    vtreal,
+                    phit,
+                    lat,
+                    dpdt,
+                    phi_spiral,
+                    xn,
+                    vt - dvt,
+                    phia,
+                )
+                [mean_error_d, rms_error_d, err_d] = compute_mean_error(
+                    r, wd, obs, wrad
+                )
+
                 # better with larger value of vt
                 if rms_error_u < rms_error:
                     vt = vt + dvt
                     rms_error = rms_error_u
-                    
-                # better with smaller value of vt    
+
+                # better with smaller value of vt
                 elif rms_error_d < rms_error:
                     vt = vt - dvt
                     rms_error = rms_error_d
-                
+
                 # optimum reached
                 else:
                     break
-                
+
                 # Other criteria
-                if vt < 0.0 or vt > 1.5*vtreal:
+                if vt < 0.0 or vt > 1.5 * vtreal:
                     break
                 if nit > 100:
                     break
-    
+
             nit = 0
-            
+
             # 3. now the asymmetry direction
             while True:
                 nit = nit + 1
-                
-                wu = compute_wind_field(r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn, vt, phia+dphia)
-                [mean_error_u, rms_error_u, err_u] = compute_mean_error(r, wu, obs, wrad)
-                wd = compute_wind_field(r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn, vt, phia-dphia)
-                [mean_error_d, rms_error_d, err_d] = compute_mean_error(r, wd, obs, wrad)
-                
+
+                wu = compute_wind_field(
+                    r,
+                    phi,
+                    vmax,
+                    pc,
+                    rmax,
+                    pn,
+                    vtreal,
+                    phit,
+                    lat,
+                    dpdt,
+                    phi_spiral,
+                    xn,
+                    vt,
+                    phia + dphia,
+                )
+                [mean_error_u, rms_error_u, err_u] = compute_mean_error(
+                    r, wu, obs, wrad
+                )
+                wd = compute_wind_field(
+                    r,
+                    phi,
+                    vmax,
+                    pc,
+                    rmax,
+                    pn,
+                    vtreal,
+                    phit,
+                    lat,
+                    dpdt,
+                    phi_spiral,
+                    xn,
+                    vt,
+                    phia - dphia,
+                )
+                [mean_error_d, rms_error_d, err_d] = compute_mean_error(
+                    r, wd, obs, wrad
+                )
+
                 if rms_error_u < rms_error:
                     # better with larger value of phia
                     phia = phia + dphia
                     rms_error = rms_error_u
-                    
+
                 elif rms_error_d < rms_error:
                     # better with smaller value of phia
                     phia = phia - dphia
                     rms_error = rms_error_d
                 else:
                     # optimum reached
                     break
-                
+
                 if phia < -180:
                     phia = phia + 360
-                    
+
                 if phia > 180:
                     phia = phia - 360
-                
+
                 if nit > 100:
                     break
-    
-    return [xn, vt, phia]           
 
+    return [xn, vt, phia]
 
 
 # defintiion to compute wind field
-def compute_wind_field(r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn, vt, phia):
-    
+def compute_wind_field(
+    r, phi, vmax, pc, rmax, pn, vtreal, phit, lat, dpdt, phi_spiral, xn, vt, phia
+):
     # Discussion
     # is asymmetry account for properly? I believe there should be a factor in front of ux/vy
     vms = vmax - vt
-    
+
     # compute wind profile (vr and pr)
     [vr, pr] = holland2010(r, vms, pc, pn, rmax, dpdt, lat, vtreal, xn)
-    
-    wind_speed = np.zeros((phi.shape[0],r.shape[0]))
-    wind_to_direction_cart = np.zeros((phi.shape[0],r.shape[0]))
+
+    wind_speed = np.zeros((phi.shape[0], r.shape[0]))
+    wind_to_direction_cart = np.zeros((phi.shape[0], r.shape[0]))
     for iphi in range(len(phi)):
-        wind_speed[iphi,:] = vr
+        wind_speed[iphi, :] = vr
         if lat >= 0:
             # northern hemisphere
             dr = 90 + phi[iphi] + phi_spiral
         else:
             # southern hemisphere
             dr = -90 + phi[iphi] - phi_spiral
-        wind_to_direction_cart[iphi,:] = dr
-        
+        wind_to_direction_cart[iphi, :] = dr
+
     ux = vt * np.cos((phit + phia) * np.pi / 180)
     uy = vt * np.sin((phit + phia) * np.pi / 180)
-    
+
     vx = wind_speed * np.cos(wind_to_direction_cart * np.pi / 180) + ux
     vy = wind_speed * np.sin(wind_to_direction_cart * np.pi / 180) + uy
-    
+
     wind_speed = np.sqrt(vx**2 + vy**2)
-    
+
     return wind_speed
 
 
 # Definition to compute mean error
 def compute_mean_error(r, w, obs, wrad):
-    
     # Discussion
     # why are we only accounting for R35?
-    
+
     # variables
-    nrad    = np.size(obs['quadrants_radii'],0)
-    nrad    = 1         # not we are only fitting R35, nothing else
-    nq      = np.size(obs['quadrants_radii'],1)     
-    iq1     = [0, 9, 18, 27]
-    iq2     = [9, 18, 27, 36]
-    err     = np.zeros((nq, nrad))
-    
+    nrad = np.size(obs["quadrants_radii"], 0)
+    nrad = 3  # not we are only fitting R35, nothing else
+    nq = np.size(obs["quadrants_radii"], 1)
+    iq1 = [0, 9, 18, 27]
+    iq2 = [9, 18, 27, 36]
+    err = np.zeros((nq, nrad))
+
     # Go over the quadrants and radii
     for irad in range(nrad):
         for iquad in range(nq):
             vrad = 0
             for j in range(iq1[iquad], iq2[iquad] + 1):
-                ww = w[j,:]
-                if not np.isnan(obs['quadrants_radii'][irad,iquad]):
+                ww = w[j, :]
+                if not np.isnan(obs["quadrants_radii"][irad, iquad]):
                     # compute wind speed vrad at required radius
-                    wf      = interp1d(r, ww, bounds_error=False, fill_value=0)
-                    w0      = wf(obs['quadrants_radii'][irad,iquad]*1000)
-                    vrad    = max(vrad, w0)
+                    wf = interp1d(r, ww, bounds_error=False, fill_value=0)
+                    w0 = wf(obs["quadrants_radii"][irad, iquad] * 1000)
+                    vrad = max(vrad, w0)
                 else:
                     # maximum wind speed must be lower than wrad
-                    w0      = max(ww)
-                    vrad    = max(vrad, w0)
-            if not np.isnan(obs['quadrants_radii'][irad,iquad]):
+                    w0 = max(ww)
+                    vrad = max(vrad, w0)
+            if not np.isnan(obs["quadrants_radii"][irad, iquad]):
                 err[iquad, irad] = vrad - wrad[irad]
             else:
                 err[iquad, irad] = np.NAN
-   
+
     # Get error values
-    mask        = ~np.isnan(err)  # Create the mask
-    err         = err[mask]
-    mean_error  = np.nanmean(err)
-    rms_error   = np.sqrt(np.mean(err**2))
-    
+    mask = ~np.isnan(err)  # Create the mask
+    err = err[mask]
+    mean_error = np.nanmean(err)
+    rms_error = np.sqrt(np.mean(err**2))
+
     # Return
     return [mean_error, rms_error, err]
 
 
-
 # Definition to compute forward speed and heading
 def compute_forward_speed_heading(t, x, y):
-    
     # variables
     forward_speed = np.zeros((len(x)))
-    heading       = np.zeros((len(x)))
+    heading = np.zeros((len(x)))
     for it in range(len(x)):
-    
         # Get basics
-        geofacy = 111111
-        geofacx = geofacy * np.cos(y[it] * np.pi/180)
+        geofacy = 110540
+        geofacx = 111320 * np.cos(y[it] * np.pi/180)
     
         if it == 0:
             
             #print('Forward')
             #datetime_forward    = 
             #dt                  = datetime_forward - datetime_it
             #dt                  = dt.total_seconds()
@@ -1911,27 +2485,26 @@
             #dt                  = datetime_it - datetime_backward
             #dt                  = dt.total_seconds()
             dx                  = (x[it] - x[it-1]) * geofacx
             dy                  = (y[it] - y[it-1]) * geofacy
             
         else: 
 
-            # Forward           
+            # Backward           
             dx1                  = (x[it] - x[it-1]) * geofacx
             dy1                  = (y[it] - y[it-1]) * geofacy
             
-            # Backward 
+            # Forward 
             dx2                  = (x[it+1] - x[it]) * geofacx
             dy2                  = (y[it+1] - y[it]) * geofacy
             
             # Combined yields central differences
-            #print('Central')
-            dx                  = np.mean([dx1, dx2])
-            dy                  = np.mean([dy1, dy2])
+            # print('Central')
+            dx = np.mean([dx1, dx2])
+            dy = np.mean([dy1, dy2])
 
         # Compute angle
-        forward_speed[it]   = 0.0
-        heading[it]         = np.arctan2(dy,dx)
-    
-        
+        forward_speed[it] = 0.0
+        heading[it] = np.arctan2(dy, dx)
+
     # Return
-    return [forward_speed, heading]
+    return [forward_speed, heading]
```

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/watersheds/watersheds.py` & `coastalhazardstoolkit-0.2.0/src/cht/watersheds/watersheds.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/cht/xbeach/xbeach.py` & `coastalhazardstoolkit-0.2.0/src/cht/xbeach/xbeach.py`

 * *Files identical despite different names*

### Comparing `coastalhazardstoolkit-0.1.0/src/coastalhazardstoolkit.egg-info/SOURCES.txt` & `coastalhazardstoolkit-0.2.0/src/coastalhazardstoolkit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 pyproject.toml
 src/cht/__init__.py
 src/cht/bathymetry/__init__.py
 src/cht/bathymetry/bathymetry_database.py
 src/cht/bathymetry/tiling.py
 src/cht/bathymetry/tiling_example.py
 src/cht/bathymetry/tiling_example_gebco22.py
+src/cht/bathymetry/utils.py
 src/cht/beware/__init__.py
 src/cht/beware/beware.py
 src/cht/delft3dfm/__init__.py
 src/cht/delft3dfm/delft3dfm.py
 src/cht/hurrywave/__init__.py
 src/cht/hurrywave/bathymetry.py
 src/cht/hurrywave/boundary_conditions.py
 src/cht/hurrywave/grid.py
 src/cht/hurrywave/hurrywave.py
 src/cht/hurrywave/hurrywave_builder.py
 src/cht/hurrywave/hurrywave_domain.py
 src/cht/hurrywave/input.py
 src/cht/hurrywave/mask.py
 src/cht/hurrywave/observation_points.py
+src/cht/hurrywave/to_xugrid.py
 src/cht/meteo/__init__.py
 src/cht/meteo/coamps_analysis.py
 src/cht/meteo/coamps_tc_forecast.py
 src/cht/meteo/coamps_tc_hindcast.py
 src/cht/meteo/coamps_tc_ufl_d01.py
 src/cht/meteo/gfs_anl_0p50.py
 src/cht/meteo/gfs_anl_0p50_02.py
@@ -35,14 +37,15 @@
 src/cht/meteo/test_coamps.py
 src/cht/misc/__init__.py
 src/cht/misc/deltares_ini.py
 src/cht/misc/fileops.py
 src/cht/misc/geometry.py
 src/cht/misc/misc_tools.py
 src/cht/misc/pli_file.py
+src/cht/misc/prob_maps.py
 src/cht/misc/sftp.py
 src/cht/misc/tekal.py
 src/cht/misc/xmlkit.py
 src/cht/model_builder/model_builder.py
 src/cht/nesting/__init__.py
 src/cht/nesting/nest1.py
 src/cht/nesting/nest2.py
@@ -57,24 +60,45 @@
 src/cht/physics/vo21.py
 src/cht/sfincs/__init__.py
 src/cht/sfincs/quadtree.py
 src/cht/sfincs/regulargrid.py
 src/cht/sfincs/sfincs.py
 src/cht/sfincs/sfincs_builder.py
 src/cht/sfincs/subgrid.py
+src/cht/sfincs2/__init__.py
+src/cht/sfincs2/boundary_conditions.py
+src/cht/sfincs2/grid.py
+src/cht/sfincs2/input.py
+src/cht/sfincs2/mask.py
+src/cht/sfincs2/observation_points.py
+src/cht/sfincs2/quadtree_grid.py
+src/cht/sfincs2/quadtree_grid_snapwave.py
+src/cht/sfincs2/regular_grid.py
+src/cht/sfincs2/sfincs.py
+src/cht/sfincs2/sfincs_builder.py
+src/cht/sfincs2/snapwave.py
+src/cht/sfincs2/subgrid.py
+src/cht/sfincs2/wave_makers.py
 src/cht/snapwave/__init__.py
 src/cht/snapwave/mesh.py
 src/cht/tide/__init__.py
 src/cht/tide/astro.py
 src/cht/tide/constituent.py
+src/cht/tide/fes2014.py
 src/cht/tide/nodal_corrections.py
+src/cht/tide/predict.py
+src/cht/tide/test_tide_database.py
 src/cht/tide/tide.py
+src/cht/tide/tide_model.py
 src/cht/tide/tide_predict.py
 src/cht/tiling/__init__.py
 src/cht/tiling/tiling.py
+src/cht/tropical_cyclone/cyclone_track_database.py
+src/cht/tropical_cyclone/test_meteo.py
+src/cht/tropical_cyclone/test_track.py
 src/cht/tropical_cyclone/testje.py
 src/cht/tropical_cyclone/testje_forecasting.py
 src/cht/tropical_cyclone/tropical_cyclone.py
 src/cht/watersheds/__init__.py
 src/cht/watersheds/watersheds.py
 src/cht/xbeach/__init__.py
 src/cht/xbeach/xbeach.py
```

