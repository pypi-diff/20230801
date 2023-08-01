# Comparing `tmp/blechpy-2.2.1.tar.gz` & `tmp/blechpy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blechpy-2.2.1.tar", last modified: Mon Jul 31 16:13:57 2023, max compression
+gzip compressed data, was "dist/blechpy-2.2.2.tar", last modified: Tue Aug  1 18:12:09 2023, max compression
```

## Comparing `blechpy-2.2.1.tar` & `blechpy-2.2.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1055 2021-06-14 16:20:28.000000 blechpy-2.2.1/LICENSE
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      122 2021-06-14 16:20:28.000000 blechpy-2.2.1/MANIFEST.in
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8844 2023-07-31 16:13:57.000000 blechpy-2.2.1/PKG-INFO
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8228 2022-10-24 17:39:20.000000 blechpy-2.2.1/README.md
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      430 2023-06-28 22:29:28.000000 blechpy-2.2.1/blechpy/__init__.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/analysis/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    65368 2021-11-18 18:57:35.000000 blechpy-2.2.1/blechpy/analysis/blech_clustering.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    11522 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/circus_interface.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2734 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/clustering.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/analysis/defaults/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      850 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/defaults/bilateral32.prb
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2797 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/defaults/default_config.params
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    12715 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/held_unit_analysis.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    25063 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/palatability_analysis.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    67026 2023-06-28 22:25:59.000000 blechpy-2.2.1/blechpy/analysis/poissonHMM.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    55747 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/poissonHMM_deprecated.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     9485 2022-07-14 00:49:50.000000 blechpy-2.2.1/blechpy/analysis/spike_analysis.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      516 2021-11-12 15:27:15.000000 blechpy-2.2.1/blechpy/analysis/spike_detection.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10253 2022-08-24 19:14:57.000000 blechpy-2.2.1/blechpy/analysis/spike_sorting.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1220 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/analysis/stat_tests.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/datastructures/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/datastructures/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    63858 2023-06-16 18:07:52.000000 blechpy-2.2.1/blechpy/datastructures/dataset.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    18325 2022-08-09 19:53:31.000000 blechpy-2.2.1/blechpy/datastructures/experiment.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5165 2021-11-12 15:27:15.000000 blechpy-2.2.1/blechpy/datastructures/objects.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8334 2022-12-09 16:30:22.000000 blechpy-2.2.1/blechpy/datastructures/project.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/dio/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      118 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10654 2022-05-23 16:45:59.000000 blechpy-2.2.1/blechpy/dio/blech_params.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/dio/defaults/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1395 2023-02-02 18:51:46.000000 blechpy-2.2.1/blechpy/dio/defaults/CAR_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2053 2022-05-23 18:04:09.000000 blechpy-2.2.1/blechpy/dio/defaults/clustering_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      205 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/defaults/pal_id_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      100 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/defaults/psth_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      124 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/defaults/spike_array_params.json
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    49150 2022-10-14 16:51:23.000000 blechpy-2.2.1/blechpy/dio/h5io.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10722 2023-03-09 19:13:34.000000 blechpy-2.2.1/blechpy/dio/hmmIO.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/dio/intanutil/
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/intanutil/__init__.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     2710 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/intanutil/data_to_result.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1642 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/intanutil/get_bytes_per_data_block.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1467 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/intanutil/notch_filter.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1036 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/intanutil/qstring.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     6858 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/intanutil/read_header.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     3649 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/intanutil/read_one_data_block.py
--rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)    10224 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/dio/load_intan_rhd_format.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8453 2021-11-12 15:27:15.000000 blechpy-2.2.1/blechpy/dio/rawIO.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3168 2022-02-10 19:18:13.000000 blechpy-2.2.1/blechpy/environment.yml
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/plotting/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      149 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/plotting/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2822 2022-08-11 19:05:52.000000 blechpy-2.2.1/blechpy/plotting/blech_waveforms_datashader.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    29972 2023-03-24 15:16:51.000000 blechpy-2.2.1/blechpy/plotting/data_plot.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    17524 2023-06-28 22:11:05.000000 blechpy-2.2.1/blechpy/plotting/hmm_plot.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    34279 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/plotting/palatability_plot.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy/utils/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      208 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/utils/__init__.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      736 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/utils/cluster_filters.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      970 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/utils/data_reset.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1418 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/utils/decorators.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1311 2021-11-18 19:01:07.000000 blechpy-2.2.1/blechpy/utils/math_tools.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1100 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/utils/memory_monitor.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3547 2021-11-12 15:27:15.000000 blechpy-2.2.1/blechpy/utils/particles.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3752 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/utils/print_tools.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    20821 2023-04-10 17:57:49.000000 blechpy-2.2.1/blechpy/utils/spike_sorting_GUI.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5082 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/utils/tk_widgets.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    19601 2022-08-11 19:06:02.000000 blechpy-2.2.1/blechpy/utils/userIO.py
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1535 2021-06-14 16:20:28.000000 blechpy-2.2.1/blechpy/utils/write_tools.py
-drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy.egg-info/
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8844 2023-07-31 16:13:56.000000 blechpy-2.2.1/blechpy.egg-info/PKG-INFO
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2076 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy.egg-info/SOURCES.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        1 2023-07-31 16:13:56.000000 blechpy-2.2.1/blechpy.egg-info/dependency_links.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      399 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy.egg-info/requires.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        8 2023-07-31 16:13:57.000000 blechpy-2.2.1/blechpy.egg-info/top_level.txt
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       38 2023-07-31 16:13:57.000000 blechpy-2.2.1/setup.cfg
--rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1280 2023-07-31 15:56:16.000000 blechpy-2.2.1/setup.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1055 2021-06-14 16:20:28.000000 blechpy-2.2.2/LICENSE
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      122 2021-06-14 16:20:28.000000 blechpy-2.2.2/MANIFEST.in
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    14465 2023-08-01 18:12:09.000000 blechpy-2.2.2/PKG-INFO
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    13849 2023-08-01 16:45:44.000000 blechpy-2.2.2/README.md
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      430 2023-06-28 22:29:28.000000 blechpy-2.2.2/blechpy/__init__.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/analysis/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    65368 2021-11-18 18:57:35.000000 blechpy-2.2.2/blechpy/analysis/blech_clustering.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    11522 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/circus_interface.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2734 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/clustering.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/analysis/defaults/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      850 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/defaults/bilateral32.prb
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2797 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/defaults/default_config.params
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    12715 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/held_unit_analysis.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    25063 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/palatability_analysis.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    67304 2023-07-31 19:56:18.000000 blechpy-2.2.2/blechpy/analysis/poissonHMM.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    55747 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/poissonHMM_deprecated.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     9485 2022-07-14 00:49:50.000000 blechpy-2.2.2/blechpy/analysis/spike_analysis.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      516 2021-11-12 15:27:15.000000 blechpy-2.2.2/blechpy/analysis/spike_detection.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10253 2022-08-24 19:14:57.000000 blechpy-2.2.2/blechpy/analysis/spike_sorting.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1220 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/analysis/stat_tests.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/datastructures/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/datastructures/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    63858 2023-06-16 18:07:52.000000 blechpy-2.2.2/blechpy/datastructures/dataset.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    18325 2022-08-09 19:53:31.000000 blechpy-2.2.2/blechpy/datastructures/experiment.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5165 2021-11-12 15:27:15.000000 blechpy-2.2.2/blechpy/datastructures/objects.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8334 2022-12-09 16:30:22.000000 blechpy-2.2.2/blechpy/datastructures/project.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/dio/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      118 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10654 2022-05-23 16:45:59.000000 blechpy-2.2.2/blechpy/dio/blech_params.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/dio/defaults/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1395 2023-02-02 18:51:46.000000 blechpy-2.2.2/blechpy/dio/defaults/CAR_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2053 2022-05-23 18:04:09.000000 blechpy-2.2.2/blechpy/dio/defaults/clustering_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      205 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/defaults/pal_id_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      100 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/defaults/psth_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      124 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/defaults/spike_array_params.json
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    49150 2022-10-14 16:51:23.000000 blechpy-2.2.2/blechpy/dio/h5io.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    10722 2023-03-09 19:13:34.000000 blechpy-2.2.2/blechpy/dio/hmmIO.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/dio/intanutil/
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/intanutil/__init__.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     2710 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/intanutil/data_to_result.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1642 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/intanutil/get_bytes_per_data_block.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1467 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/intanutil/notch_filter.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     1036 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/intanutil/qstring.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     6858 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/intanutil/read_header.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)     3649 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/intanutil/read_one_data_block.py
+-rwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)    10224 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/dio/load_intan_rhd_format.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     8453 2021-11-12 15:27:15.000000 blechpy-2.2.2/blechpy/dio/rawIO.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3168 2022-02-10 19:18:13.000000 blechpy-2.2.2/blechpy/environment.yml
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/plotting/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      149 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/plotting/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2822 2022-08-11 19:05:52.000000 blechpy-2.2.2/blechpy/plotting/blech_waveforms_datashader.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    29972 2023-03-24 15:16:51.000000 blechpy-2.2.2/blechpy/plotting/data_plot.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    17524 2023-06-28 22:11:05.000000 blechpy-2.2.2/blechpy/plotting/hmm_plot.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    34279 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/plotting/palatability_plot.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy/utils/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      208 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/utils/__init__.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      736 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/utils/cluster_filters.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      970 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/utils/data_reset.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1418 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/utils/decorators.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1311 2021-11-18 19:01:07.000000 blechpy-2.2.2/blechpy/utils/math_tools.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1100 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/utils/memory_monitor.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3547 2021-11-12 15:27:15.000000 blechpy-2.2.2/blechpy/utils/particles.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     3752 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/utils/print_tools.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    20821 2023-04-10 17:57:49.000000 blechpy-2.2.2/blechpy/utils/spike_sorting_GUI.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     5082 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/utils/tk_widgets.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    19601 2022-08-11 19:06:02.000000 blechpy-2.2.2/blechpy/utils/userIO.py
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1535 2021-06-14 16:20:28.000000 blechpy-2.2.2/blechpy/utils/write_tools.py
+drwxrwxr-x   0 dsvedberg  (1000) dsvedberg  (1000)        0 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy.egg-info/
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)    14465 2023-08-01 18:12:08.000000 blechpy-2.2.2/blechpy.egg-info/PKG-INFO
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     2076 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        1 2023-08-01 18:12:08.000000 blechpy-2.2.2/blechpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)      399 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy.egg-info/requires.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)        8 2023-08-01 18:12:09.000000 blechpy-2.2.2/blechpy.egg-info/top_level.txt
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)       38 2023-08-01 18:12:09.000000 blechpy-2.2.2/setup.cfg
+-rw-rw-r--   0 dsvedberg  (1000) dsvedberg  (1000)     1280 2023-07-31 20:14:38.000000 blechpy-2.2.2/setup.py
```

### Comparing `blechpy-2.2.1/LICENSE` & `blechpy-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/blech_clustering.py` & `blechpy-2.2.2/blechpy/analysis/blech_clustering.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/circus_interface.py` & `blechpy-2.2.2/blechpy/analysis/circus_interface.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/clustering.py` & `blechpy-2.2.2/blechpy/analysis/clustering.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/defaults/bilateral32.prb` & `blechpy-2.2.2/blechpy/analysis/defaults/bilateral32.prb`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/defaults/default_config.params` & `blechpy-2.2.2/blechpy/analysis/defaults/default_config.params`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/held_unit_analysis.py` & `blechpy-2.2.2/blechpy/analysis/held_unit_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/palatability_analysis.py` & `blechpy-2.2.2/blechpy/analysis/palatability_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/poissonHMM.py` & `blechpy-2.2.2/blechpy/analysis/poissonHMM.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,35 +362,35 @@
         pass
     else:
         bestPaths, path_probs = compute_best_paths(spikes, dt, PI, A, B)
         maxLogProb = np.sum(path_probs)
         n_time_steps = spikes.shape[-1]
 
     BIC = -2 * maxLogProb + nParams * np.log(n_time_steps)
-    return BIC, bestPaths, maxLogProb
-#TODO add compute_AIC method and integrate
-
+    AIC = -2 * maxLogProb + 2 * nParams
+    return BIC, AIC, bestPaths, maxLogProb
 
 def compute_hmm_cost(spikes, dt, PI, A, B, win_size=0.25, true_rates=None):
     if true_rates is None:
         true_rates = convert_spikes_to_rates(spikes, dt, win_size,
                                              step_size=win_size)
 
-    BIC, bestPaths, maxLogProb = compute_BIC(PI, A, B, spikes=spikes, dt=dt)
+    BIC, AIC, bestPaths, maxLogProb = compute_BIC(PI, A, B, spikes=spikes, dt=dt)
     hmm_rates = generate_rate_array_from_state_seq(bestPaths, B, dt, win_size,
                                                    step_size=win_size)
     RMSE = compute_rate_rmse(true_rates, hmm_rates)
-    return RMSE, BIC, bestPaths, maxLogProb
+    return RMSE, BIC, AIC, bestPaths, maxLogProb
 
 
 def compute_best_paths(spikes, dt, PI, A, B):
     if len(spikes.shape) == 2:
         spikes = np.array([spikes])
 
-    nTrials, nCells, nTimeSteps = spikes.shape
+    nTrials, nCells, nTimeSteps = spikes.shapeg
+    nTrials, nCells, nTimeSteps = spikes.shapeg
     bestPaths = np.zeros((nTrials, nTimeSteps))-1
     pathProbs = np.zeros((nTrials,))
 
     for i, trial in enumerate(spikes):
         bestPaths[i,:], pathProbs[i], _, _ = poisson_viterbi(trial, dt, PI,
                                                              A, B)
     return bestPaths, pathProbs
@@ -777,14 +777,15 @@
     for k,v in stat_arrays.items():
         if k in hmm.stat_arrays.keys() and isinstance(hmm.stat_arrays[k], list):
             hmm.stat_arrays[k] = list(v)
         else:
             hmm.stat_arrays[k] = v
 
     hmm.BIC = params.pop('BIC')
+    hmm.AIC = params.pop('AIC')
     hmm.converged = params.pop('converged')
     hmm.fitted = params.pop('fitted')
     hmm.cost = params.pop('cost')
     hmm.fit_LL = params.pop('log_likelihood')
     hmm.max_log_prob = params.pop('max_log_prob')
     if stat_arrays.get('trial_nums') is not None:
         params['trial_nums'] = list(stat_arrays['trial_nums'])
@@ -895,14 +896,15 @@
         self.initial_distribution = None
 
         self.fitted = False
         self.converged = False
 
         self.cost = None
         self.BIC = None
+        self.AIC = None
         self.max_log_prob = None
         self.fit_LL = None
 
     def randomize(self, spikes, dt, time, row_id=None, constraint_func=None):
         '''Initialize and randomize HMM matrices: initial_distribution (PI),
         transition (A) and emission/rates (B)
         Parameters
@@ -972,28 +974,30 @@
         self._update_cost(spikes, dt)
         self.fit_LL = self.max_log_prob
         self._update_history()
 
     def _init_history(self):
         self.stat_arrays['cost'] = []
         self.stat_arrays['BIC'] = []
+        self.stat_arrays['AIC'] = []
         self.stat_arrays['max_log_prob'] = []
         self.stat_arrays['fit_LL'] = []
         self.stat_arrays['iterations'] = []
         self.history = {'A': [], 'B': [], 'PI': [], 'iterations':[]}
 
     def _update_history(self):
         itr = self.iteration
         self.history['A'].append(self.transition)
         self.history['B'].append(self.emission)
         self.history['PI'].append(self.initial_distribution)
         self.history['iterations'].append(itr)
 
         self.stat_arrays['cost'].append(self.cost)
         self.stat_arrays['BIC'].append(self.BIC)
+        self.stat_arrays['AIC'].append(self.AIC)
         self.stat_arrays['max_log_prob'].append(self.max_log_prob)
         self.stat_arrays['fit_LL'].append(self.fit_LL)
         self.stat_arrays['iterations'].append(itr)
 
     def fit(self, spikes, dt, time, max_iter = 500, threshold=1e-5, parallel=False):
         '''using parallels for processing trials actually seems to slow down
         processing (with 15 trials). Might still be useful if there is a very
@@ -1147,17 +1151,18 @@
         return np.array(gammas)
 
     def _update_cost(self, spikes, dt):
         spikes = spikes.astype('int')
         PI = self.initial_distribution
         A  = self.transition
         B  = self.emission
-        cost, BIC, bestPaths, maxLogProb = compute_hmm_cost(spikes, dt, PI, A, B)
+        cost, BIC, AIC, bestPaths, maxLogProb = compute_hmm_cost(spikes, dt, PI, A, B)
         self.cost = cost
         self.BIC = BIC
+        self.AIC = AIC
         self.max_log_prob = maxLogProb
         self.stat_arrays['best_sequences'] = bestPaths
 
     def roll_back(self, iteration, spikes=None, dt=None):
         itrs = self.history['iterations']
         idx = np.where(itrs == iteration)[0]
         if len(idx) == 0:
@@ -1170,14 +1175,15 @@
         self.iteration = iteration
 
         itrs = self.stat_arrays['iterations']
         idx = np.where(itrs == iteration)[0][0]
         self.fit_LL = self.stat_arrays['fit_LL'][idx]
         self.max_log_prob = self.stat_arrays['max_log_prob'][idx]
         self.BIC = self.stat_arrays['BIC'][idx]
+        self.AIC = self.stat_arrays['AIC'][idx]
         self.cost = self.stat_arrays['cost'][idx]
         if spikes is not None and dt is not None:
             self.stat_arrays['gamma_probabilities'] = self.get_gamma_probabilities(spikes, dt)
             self._update_cost(spikes, dt)
 
         self._update_history()
```

### Comparing `blechpy-2.2.1/blechpy/analysis/poissonHMM_deprecated.py` & `blechpy-2.2.2/blechpy/analysis/poissonHMM_deprecated.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/spike_analysis.py` & `blechpy-2.2.2/blechpy/analysis/spike_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/spike_detection.py` & `blechpy-2.2.2/blechpy/analysis/spike_detection.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/spike_sorting.py` & `blechpy-2.2.2/blechpy/analysis/spike_sorting.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/analysis/stat_tests.py` & `blechpy-2.2.2/blechpy/analysis/stat_tests.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/datastructures/dataset.py` & `blechpy-2.2.2/blechpy/datastructures/dataset.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/datastructures/experiment.py` & `blechpy-2.2.2/blechpy/datastructures/experiment.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/datastructures/objects.py` & `blechpy-2.2.2/blechpy/datastructures/objects.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/datastructures/project.py` & `blechpy-2.2.2/blechpy/datastructures/project.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/blech_params.py` & `blechpy-2.2.2/blechpy/dio/blech_params.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/defaults/CAR_params.json` & `blechpy-2.2.2/blechpy/dio/defaults/CAR_params.json`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/defaults/clustering_params.json` & `blechpy-2.2.2/blechpy/dio/defaults/clustering_params.json`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/h5io.py` & `blechpy-2.2.2/blechpy/dio/h5io.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/hmmIO.py` & `blechpy-2.2.2/blechpy/dio/hmmIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/intanutil/data_to_result.py` & `blechpy-2.2.2/blechpy/dio/intanutil/data_to_result.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/intanutil/get_bytes_per_data_block.py` & `blechpy-2.2.2/blechpy/dio/intanutil/get_bytes_per_data_block.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/intanutil/notch_filter.py` & `blechpy-2.2.2/blechpy/dio/intanutil/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/intanutil/qstring.py` & `blechpy-2.2.2/blechpy/dio/intanutil/qstring.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/intanutil/read_header.py` & `blechpy-2.2.2/blechpy/dio/intanutil/read_header.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/intanutil/read_one_data_block.py` & `blechpy-2.2.2/blechpy/dio/intanutil/read_one_data_block.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/load_intan_rhd_format.py` & `blechpy-2.2.2/blechpy/dio/load_intan_rhd_format.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/dio/rawIO.py` & `blechpy-2.2.2/blechpy/dio/rawIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/environment.yml` & `blechpy-2.2.2/blechpy/environment.yml`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/plotting/blech_waveforms_datashader.py` & `blechpy-2.2.2/blechpy/plotting/blech_waveforms_datashader.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/plotting/data_plot.py` & `blechpy-2.2.2/blechpy/plotting/data_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/plotting/hmm_plot.py` & `blechpy-2.2.2/blechpy/plotting/hmm_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/plotting/palatability_plot.py` & `blechpy-2.2.2/blechpy/plotting/palatability_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/cluster_filters.py` & `blechpy-2.2.2/blechpy/utils/cluster_filters.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/data_reset.py` & `blechpy-2.2.2/blechpy/utils/data_reset.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/decorators.py` & `blechpy-2.2.2/blechpy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/math_tools.py` & `blechpy-2.2.2/blechpy/utils/math_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/memory_monitor.py` & `blechpy-2.2.2/blechpy/utils/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/particles.py` & `blechpy-2.2.2/blechpy/utils/particles.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/print_tools.py` & `blechpy-2.2.2/blechpy/utils/print_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/spike_sorting_GUI.py` & `blechpy-2.2.2/blechpy/utils/spike_sorting_GUI.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/tk_widgets.py` & `blechpy-2.2.2/blechpy/utils/tk_widgets.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/userIO.py` & `blechpy-2.2.2/blechpy/utils/userIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy/utils/write_tools.py` & `blechpy-2.2.2/blechpy/utils/write_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/blechpy.egg-info/SOURCES.txt` & `blechpy-2.2.2/blechpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blechpy-2.2.1/setup.py` & `blechpy-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = [] # Examples: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirementPath):
     with open(requirementPath) as f:
         install_requires = f.read().splitlines()
 
 setuptools.setup(
     name='blechpy',
-    version='2.2.1',
+    version='2.2.2',
     author='Roshan Nanu, Daniel Svedberg',
     author_email='roshan.nanu@gmail.com, dan.ake.svedberg@gmail.com',
     description='Package for exrtacting, processing and analyzing Intan and OpenEphys data',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/nubs01/blechpy',
     packages=setuptools.find_packages(),
```

