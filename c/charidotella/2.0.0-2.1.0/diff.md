# Comparing `tmp/charidotella-2.0.0.tar.gz` & `tmp/charidotella-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charidotella-2.0.0.tar", last modified: Mon Jul 31 22:27:52 2023, max compression
+gzip compressed data, was "charidotella-2.1.0.tar", last modified: Tue Aug  1 20:37:30 2023, max compression
```

## Comparing `charidotella-2.0.0.tar` & `charidotella-2.1.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 22:27:52.000000 charidotella-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-31 22:27:52.666162 charidotella-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-31 22:26:25.000000 charidotella-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.646162 charidotella-2.0.0/charidotella/
--rw-r--r--   0 runner    (1001) docker     (123)    44465 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/animals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.654162 charidotella-2.0.0/charidotella/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/assets/configuration-schema.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-07-31 22:27:14.000000 charidotella-2.0.0/charidotella/assets/es_to_frames
--rwxr-xr-x   0 runner    (1001) docker     (123)   286032 2023-07-31 22:27:24.000000 charidotella-2.0.0/charidotella/assets/event_rate
--rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-07-31 22:27:26.000000 charidotella-2.0.0/charidotella/assets/size
--rwxr-xr-x   0 runner    (1001) docker     (123)  1011024 2023-07-31 22:27:37.000000 charidotella-2.0.0/charidotella/assets/spatiospectrogram
--rwxr-xr-x   0 runner    (1001) docker     (123)   396632 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella/assets/spectrogram
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/charidotella_extension_placeholder.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.654162 charidotella-2.0.0/charidotella/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/arbiter_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/hot_pixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/refractory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.658162 charidotella-2.0.0/charidotella/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/colourtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/event_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/spatiospectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/wiggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.646162 charidotella-2.0.0/charidotella.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.658162 charidotella-2.0.0/command_line_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/premake4.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.662162 charidotella-2.0.0/command_line_tools/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/crop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/cut.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/dat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/dat_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/es_to_csv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/es_to_frames.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/es_to_ply.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/event_rate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/evt3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/evt3_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/font.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/html.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/rainbow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/rainmaker.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/spatiospectrogram.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26665 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/spectrogram.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/statistics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/synth.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/timecode.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/lodepng/
--rw-r--r--   0 runner    (1001) docker     (123)   260001 2023-07-31 22:26:32.000000 charidotella-2.0.0/command_line_tools/third_party/lodepng/lodepng.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    93636 2023-07-31 22:26:32.000000 charidotella-2.0.0/command_line_tools/third_party/lodepng/lodepng.h
--rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/third_party/monaco.ttf.base64.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.642162 charidotella-2.0.0/command_line_tools/third_party/pontella/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/pontella/source/
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-07-31 22:26:33.000000 charidotella-2.0.0/command_line_tools/third_party/pontella/source/pontella.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.642162 charidotella-2.0.0/command_line_tools/third_party/sepia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/sepia/source/
--rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-07-31 22:26:35.000000 charidotella-2.0.0/command_line_tools/third_party/sepia/source/sepia.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/third_party/stb_truetype.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.642162 charidotella-2.0.0/command_line_tools/third_party/tarsier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/tarsier/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-31 22:26:40.000000 charidotella-2.0.0/command_line_tools/third_party/tarsier/source/replicate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-31 22:26:40.000000 charidotella-2.0.0/command_line_tools/third_party/tarsier/source/stitch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-07-31 22:26:25.000000 charidotella-2.0.0/configuration-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-31 22:26:25.000000 charidotella-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 22:27:52.670163 charidotella-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-31 22:26:25.000000 charidotella-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.378506 charidotella-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 20:37:30.000000 charidotella-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-01 20:37:30.374506 charidotella-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-01 20:35:57.000000 charidotella-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.362505 charidotella-2.1.0/charidotella/
+-rw-r--r--   0 runner    (1001) docker     (123)    44506 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/animals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.366505 charidotella-2.1.0/charidotella/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/assets/configuration-schema.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-08-01 20:36:49.000000 charidotella-2.1.0/charidotella/assets/es_to_frames
+-rwxr-xr-x   0 runner    (1001) docker     (123)   286032 2023-08-01 20:37:00.000000 charidotella-2.1.0/charidotella/assets/event_rate
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-08-01 20:37:03.000000 charidotella-2.1.0/charidotella/assets/size
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1011024 2023-08-01 20:37:14.000000 charidotella-2.1.0/charidotella/assets/spatiospectrogram
+-rwxr-xr-x   0 runner    (1001) docker     (123)   396632 2023-08-01 20:37:30.000000 charidotella-2.1.0/charidotella/assets/spectrogram
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/charidotella_extension_placeholder.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.366505 charidotella-2.1.0/charidotella/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/filters/arbiter_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/filters/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/filters/hot_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/filters/refractory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/filters/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.370505 charidotella-2.1.0/charidotella/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/tasks/colourtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/tasks/event_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/tasks/spatiospectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/tasks/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/tasks/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/tasks/wiggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 20:35:57.000000 charidotella-2.1.0/charidotella/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.362505 charidotella-2.1.0/charidotella.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-01 20:37:30.000000 charidotella-2.1.0/charidotella.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-08-01 20:37:30.000000 charidotella-2.1.0/charidotella.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:37:30.000000 charidotella-2.1.0/charidotella.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 20:37:30.000000 charidotella-2.1.0/charidotella.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 20:37:30.000000 charidotella-2.1.0/charidotella.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 20:37:30.000000 charidotella-2.1.0/charidotella.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.370505 charidotella-2.1.0/command_line_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/premake4.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.374506 charidotella-2.1.0/command_line_tools/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/crop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/cut.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/dat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/dat_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/es_to_csv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/es_to_frames.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/es_to_ply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/event_rate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/evt3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/evt3_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/font.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/html.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/rainbow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/rainmaker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/spatiospectrogram.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26665 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/spectrogram.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/statistics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/synth.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/source/timecode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.374506 charidotella-2.1.0/command_line_tools/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.374506 charidotella-2.1.0/command_line_tools/third_party/lodepng/
+-rw-r--r--   0 runner    (1001) docker     (123)   260001 2023-08-01 20:36:04.000000 charidotella-2.1.0/command_line_tools/third_party/lodepng/lodepng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    93636 2023-08-01 20:36:04.000000 charidotella-2.1.0/command_line_tools/third_party/lodepng/lodepng.h
+-rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/third_party/monaco.ttf.base64.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.358505 charidotella-2.1.0/command_line_tools/third_party/pontella/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.374506 charidotella-2.1.0/command_line_tools/third_party/pontella/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-01 20:36:06.000000 charidotella-2.1.0/command_line_tools/third_party/pontella/source/pontella.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.358505 charidotella-2.1.0/command_line_tools/third_party/sepia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.374506 charidotella-2.1.0/command_line_tools/third_party/sepia/source/
+-rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-08-01 20:36:09.000000 charidotella-2.1.0/command_line_tools/third_party/sepia/source/sepia.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-08-01 20:35:59.000000 charidotella-2.1.0/command_line_tools/third_party/stb_truetype.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.358505 charidotella-2.1.0/command_line_tools/third_party/tarsier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:37:30.374506 charidotella-2.1.0/command_line_tools/third_party/tarsier/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-01 20:36:13.000000 charidotella-2.1.0/command_line_tools/third_party/tarsier/source/replicate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-01 20:36:13.000000 charidotella-2.1.0/command_line_tools/third_party/tarsier/source/stitch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-08-01 20:35:57.000000 charidotella-2.1.0/configuration-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 20:35:57.000000 charidotella-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:37:30.378506 charidotella-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-01 20:35:57.000000 charidotella-2.1.0/setup.py
```

### Comparing `charidotella-2.0.0/MANIFEST.in` & `charidotella-2.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/PKG-INFO` & `charidotella-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charidotella
-Version: 2.0.0
+Version: 2.1.0
 Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
 Home-page: https://github.com/neuromorphicsystems/charidotella
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -104,15 +104,15 @@
         └── file_n.es
     ```
 
 3.  Generate a configuration file
 
     ```sh
     cd my-wonderful-project
-    charidotella init 'recordings/*.es'
+    charidotella init
     ```
 
     The directory now has the following structure
 
     ```txt
     my-wonderful-project
     ├── recordings
```

### Comparing `charidotella-2.0.0/README.md` & `charidotella-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         └── file_n.es
     ```
 
 3.  Generate a configuration file
 
     ```sh
     cd my-wonderful-project
-    charidotella init 'recordings/*.es'
+    charidotella init
     ```
 
     The directory now has the following structure
 
     ```txt
     my-wonderful-project
     ├── recordings
```

### Comparing `charidotella-2.0.0/charidotella/__init__.py` & `charidotella-2.1.0/charidotella/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,17 @@
     )
     parser.add_argument(
         "--version", "-v", action="store_true", help="show the version and exit"
     )
     subparsers = parser.add_subparsers(dest="command")
     init_parser = subparsers.add_parser("init", help="Generate a configuration file")
     init_parser.add_argument(
-        "glob",
+        "--glob",
+        "-g",
+        default="recordings/*.es",
         help="Glob pattern used to search for Event Stream files",
     )
     init_parser.add_argument(
         "--configuration",
         "-c",
         default="charidotella-configuration.toml",
         help="Render configuration file path",
@@ -391,16 +393,16 @@
                     "begin": utilities.timestamp_to_timecode(begin),
                     "end": utilities.timestamp_to_timecode(end),
                     "filters": ["default"],
                     "tasks": [
                         "colourtime-.+",
                         "event-rate-.+",
                         "spectrogram",
-                        "wiggle-.+",
-                        "video-real-time",
+                        "wiggle",
+                        "video-1x",
                     ]
                     + (["spatiospectrogram"] if args.spatiospectrograms else []),
                 }
             )
         with open(
             utilities.with_suffix(configuration_path, ".part"),
             "w",
```

### Comparing `charidotella-2.0.0/charidotella/animals.py` & `charidotella-2.1.0/charidotella/animals.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/assets/configuration-schema.json` & `charidotella-2.1.0/charidotella/assets/configuration-schema.json`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/assets/es_to_frames` & `charidotella-2.1.0/charidotella/assets/es_to_frames`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/assets/event_rate` & `charidotella-2.1.0/charidotella/assets/event_rate`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/assets/size` & `charidotella-2.1.0/charidotella/assets/size`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/assets/spatiospectrogram` & `charidotella-2.1.0/charidotella/assets/spatiospectrogram`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/assets/spectrogram` & `charidotella-2.1.0/charidotella/assets/spectrogram`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/charidotella_extension_placeholder.c` & `charidotella-2.1.0/charidotella/charidotella_extension_placeholder.c`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/filters/arbiter_saturation.py` & `charidotella-2.1.0/charidotella/filters/arbiter_saturation.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/filters/default.py` & `charidotella-2.1.0/charidotella/filters/default.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/filters/hot_pixels.py` & `charidotella-2.1.0/charidotella/filters/hot_pixels.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/filters/refractory.py` & `charidotella-2.1.0/charidotella/filters/refractory.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/filters/transpose.py` & `charidotella-2.1.0/charidotella/filters/transpose.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/tasks/colourtime.py` & `charidotella-2.1.0/charidotella/tasks/colourtime.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/tasks/event_rate.py` & `charidotella-2.1.0/charidotella/tasks/event_rate.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/tasks/spatiospectrogram.py` & `charidotella-2.1.0/charidotella/tasks/spatiospectrogram.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/tasks/spectrogram.py` & `charidotella-2.1.0/charidotella/tasks/spectrogram.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/tasks/video.py` & `charidotella-2.1.0/charidotella/tasks/video.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/tasks/wiggle.py` & `charidotella-2.1.0/charidotella/tasks/wiggle.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella/utilities.py` & `charidotella-2.1.0/charidotella/utilities.py`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/charidotella.egg-info/PKG-INFO` & `charidotella-2.1.0/charidotella.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charidotella
-Version: 2.0.0
+Version: 2.1.0
 Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
 Home-page: https://github.com/neuromorphicsystems/charidotella
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -104,15 +104,15 @@
         └── file_n.es
     ```
 
 3.  Generate a configuration file
 
     ```sh
     cd my-wonderful-project
-    charidotella init 'recordings/*.es'
+    charidotella init
     ```
 
     The directory now has the following structure
 
     ```txt
     my-wonderful-project
     ├── recordings
```

### Comparing `charidotella-2.0.0/charidotella.egg-info/SOURCES.txt` & `charidotella-2.1.0/charidotella.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/premake4.lua` & `charidotella-2.1.0/command_line_tools/premake4.lua`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/crop.cpp` & `charidotella-2.1.0/command_line_tools/source/crop.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/cut.cpp` & `charidotella-2.1.0/command_line_tools/source/cut.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/dat.hpp` & `charidotella-2.1.0/command_line_tools/source/dat.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/dat_to_es.cpp` & `charidotella-2.1.0/command_line_tools/source/dat_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/es_to_csv.cpp` & `charidotella-2.1.0/command_line_tools/source/es_to_csv.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/es_to_frames.cpp` & `charidotella-2.1.0/command_line_tools/source/es_to_frames.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/es_to_ply.cpp` & `charidotella-2.1.0/command_line_tools/source/es_to_ply.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/event_rate.cpp` & `charidotella-2.1.0/command_line_tools/source/event_rate.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/evt3.hpp` & `charidotella-2.1.0/command_line_tools/source/evt3.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/evt3_to_es.cpp` & `charidotella-2.1.0/command_line_tools/source/evt3_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/font.hpp` & `charidotella-2.1.0/command_line_tools/source/font.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/html.hpp` & `charidotella-2.1.0/command_line_tools/source/html.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/rainbow.cpp` & `charidotella-2.1.0/command_line_tools/source/rainbow.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/rainmaker.cpp` & `charidotella-2.1.0/command_line_tools/source/rainmaker.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/size.cpp` & `charidotella-2.1.0/command_line_tools/source/size.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/spatiospectrogram.cpp` & `charidotella-2.1.0/command_line_tools/source/spatiospectrogram.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/spectrogram.cpp` & `charidotella-2.1.0/command_line_tools/source/spectrogram.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/statistics.cpp` & `charidotella-2.1.0/command_line_tools/source/statistics.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/synth.cpp` & `charidotella-2.1.0/command_line_tools/source/synth.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/source/timecode.hpp` & `charidotella-2.1.0/command_line_tools/source/timecode.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/third_party/lodepng/lodepng.cpp` & `charidotella-2.1.0/command_line_tools/third_party/lodepng/lodepng.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/third_party/lodepng/lodepng.h` & `charidotella-2.1.0/command_line_tools/third_party/lodepng/lodepng.h`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/third_party/monaco.ttf.base64.hpp` & `charidotella-2.1.0/command_line_tools/third_party/monaco.ttf.base64.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/third_party/pontella/source/pontella.hpp` & `charidotella-2.1.0/command_line_tools/third_party/pontella/source/pontella.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/third_party/sepia/source/sepia.hpp` & `charidotella-2.1.0/command_line_tools/third_party/sepia/source/sepia.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/third_party/stb_truetype.hpp` & `charidotella-2.1.0/command_line_tools/third_party/stb_truetype.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/third_party/tarsier/source/replicate.hpp` & `charidotella-2.1.0/command_line_tools/third_party/tarsier/source/replicate.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/command_line_tools/third_party/tarsier/source/stitch.hpp` & `charidotella-2.1.0/command_line_tools/third_party/tarsier/source/stitch.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/configuration-schema.json` & `charidotella-2.1.0/configuration-schema.json`

 * *Files identical despite different names*

### Comparing `charidotella-2.0.0/setup.py` & `charidotella-2.1.0/setup.py`

 * *Files identical despite different names*

