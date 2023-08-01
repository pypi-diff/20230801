# Comparing `tmp/charidotella-1.2.0.tar.gz` & `tmp/charidotella-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charidotella-1.2.0.tar", last modified: Sun May 28 11:10:07 2023, max compression
+gzip compressed data, was "charidotella-2.0.0.tar", last modified: Mon Jul 31 22:27:52 2023, max compression
```

## Comparing `charidotella-1.2.0.tar` & `charidotella-2.0.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-28 11:10:06.000000 charidotella-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-28 11:10:07.009798 charidotella-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-28 11:09:03.000000 charidotella-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.001798 charidotella-1.2.0/charidotella/
--rw-r--r--   0 runner    (1001) docker     (123)    45110 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/animals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.005798 charidotella-1.2.0/charidotella/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/assets/configuration-schema.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-05-28 11:09:36.000000 charidotella-1.2.0/charidotella/assets/es_to_frames
--rwxr-xr-x   0 runner    (1001) docker     (123)   286032 2023-05-28 11:09:44.000000 charidotella-1.2.0/charidotella/assets/event_rate
--rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-05-28 11:09:46.000000 charidotella-1.2.0/charidotella/assets/size
--rwxr-xr-x   0 runner    (1001) docker     (123)  1011024 2023-05-28 11:09:55.000000 charidotella-1.2.0/charidotella/assets/spatiospectrogram
--rwxr-xr-x   0 runner    (1001) docker     (123)   396632 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella/assets/spectrogram
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/charidotella_extension_placeholder.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.005798 charidotella-1.2.0/charidotella/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/arbiter_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/hot_pixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/refractory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/filters/transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.005798 charidotella-1.2.0/charidotella/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/colourtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/event_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/spatiospectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/tasks/wiggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:09:03.000000 charidotella-1.2.0/charidotella/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.001798 charidotella-1.2.0/charidotella.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 11:10:06.000000 charidotella-1.2.0/charidotella.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.005798 charidotella-1.2.0/command_line_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/premake4.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/crop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/cut.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/dat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/dat_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/es_to_csv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/es_to_frames.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/es_to_ply.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/event_rate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/evt3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/evt3_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/font.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/html.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/rainbow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/rainmaker.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/spatiospectrogram.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26665 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/spectrogram.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/statistics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/synth.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/source/timecode.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/lodepng/
--rw-r--r--   0 runner    (1001) docker     (123)   260001 2023-05-28 11:09:05.000000 charidotella-1.2.0/command_line_tools/third_party/lodepng/lodepng.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    93636 2023-05-28 11:09:05.000000 charidotella-1.2.0/command_line_tools/third_party/lodepng/lodepng.h
--rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/third_party/monaco.ttf.base64.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:06.997798 charidotella-1.2.0/command_line_tools/third_party/pontella/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/pontella/source/
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-28 11:09:05.000000 charidotella-1.2.0/command_line_tools/third_party/pontella/source/pontella.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.001798 charidotella-1.2.0/command_line_tools/third_party/sepia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/sepia/source/
--rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-05-28 11:09:07.000000 charidotella-1.2.0/command_line_tools/third_party/sepia/source/sepia.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-05-28 11:09:03.000000 charidotella-1.2.0/command_line_tools/third_party/stb_truetype.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.001798 charidotella-1.2.0/command_line_tools/third_party/tarsier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:10:07.009798 charidotella-1.2.0/command_line_tools/third_party/tarsier/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-28 11:09:09.000000 charidotella-1.2.0/command_line_tools/third_party/tarsier/source/replicate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-28 11:09:09.000000 charidotella-1.2.0/command_line_tools/third_party/tarsier/source/stitch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-05-28 11:09:03.000000 charidotella-1.2.0/configuration-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-28 11:09:03.000000 charidotella-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 11:10:07.009798 charidotella-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-28 11:09:03.000000 charidotella-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 22:27:52.000000 charidotella-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-31 22:27:52.666162 charidotella-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-31 22:26:25.000000 charidotella-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.646162 charidotella-2.0.0/charidotella/
+-rw-r--r--   0 runner    (1001) docker     (123)    44465 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/animals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.654162 charidotella-2.0.0/charidotella/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/assets/configuration-schema.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-07-31 22:27:14.000000 charidotella-2.0.0/charidotella/assets/es_to_frames
+-rwxr-xr-x   0 runner    (1001) docker     (123)   286032 2023-07-31 22:27:24.000000 charidotella-2.0.0/charidotella/assets/event_rate
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-07-31 22:27:26.000000 charidotella-2.0.0/charidotella/assets/size
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1011024 2023-07-31 22:27:37.000000 charidotella-2.0.0/charidotella/assets/spatiospectrogram
+-rwxr-xr-x   0 runner    (1001) docker     (123)   396632 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella/assets/spectrogram
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/charidotella_extension_placeholder.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.654162 charidotella-2.0.0/charidotella/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/arbiter_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/hot_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/refractory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/filters/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.658162 charidotella-2.0.0/charidotella/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/colourtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/event_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/spatiospectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/tasks/wiggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 22:26:25.000000 charidotella-2.0.0/charidotella/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.646162 charidotella-2.0.0/charidotella.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 22:27:52.000000 charidotella-2.0.0/charidotella.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.658162 charidotella-2.0.0/command_line_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/premake4.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.662162 charidotella-2.0.0/command_line_tools/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/crop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/cut.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/dat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/dat_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/es_to_csv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/es_to_frames.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/es_to_ply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/event_rate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/evt3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/evt3_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/font.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/html.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/rainbow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/rainmaker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/spatiospectrogram.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26665 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/spectrogram.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/statistics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/synth.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/source/timecode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/lodepng/
+-rw-r--r--   0 runner    (1001) docker     (123)   260001 2023-07-31 22:26:32.000000 charidotella-2.0.0/command_line_tools/third_party/lodepng/lodepng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    93636 2023-07-31 22:26:32.000000 charidotella-2.0.0/command_line_tools/third_party/lodepng/lodepng.h
+-rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/third_party/monaco.ttf.base64.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.642162 charidotella-2.0.0/command_line_tools/third_party/pontella/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/pontella/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-07-31 22:26:33.000000 charidotella-2.0.0/command_line_tools/third_party/pontella/source/pontella.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.642162 charidotella-2.0.0/command_line_tools/third_party/sepia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/sepia/source/
+-rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-07-31 22:26:35.000000 charidotella-2.0.0/command_line_tools/third_party/sepia/source/sepia.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-07-31 22:26:27.000000 charidotella-2.0.0/command_line_tools/third_party/stb_truetype.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.642162 charidotella-2.0.0/command_line_tools/third_party/tarsier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:27:52.666162 charidotella-2.0.0/command_line_tools/third_party/tarsier/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-31 22:26:40.000000 charidotella-2.0.0/command_line_tools/third_party/tarsier/source/replicate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-31 22:26:40.000000 charidotella-2.0.0/command_line_tools/third_party/tarsier/source/stitch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-07-31 22:26:25.000000 charidotella-2.0.0/configuration-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-31 22:26:25.000000 charidotella-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 22:27:52.670163 charidotella-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-31 22:26:25.000000 charidotella-2.0.0/setup.py
```

### Comparing `charidotella-1.2.0/MANIFEST.in` & `charidotella-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/PKG-INFO` & `charidotella-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: charidotella
-Version: 1.2.0
-Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
-Home-page: https://github.com/neuromorphicsystems/charidotella
-Author: Alexandre Marcireau
-Author-email: alexandre.marcireau@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 ![banner](banner.png)
 
 Charidotella (https://en.wikipedia.org/wiki/Charidotella_sexpunctata) is a toolbox to organise and visualise Event Stream (.es) recordings.
 
 It supports Python 3.9, 3.10, and 3.11.
 
 - [Dependencies](#dependencies)
@@ -137,22 +125,22 @@
     my-wonderful-project
     ├── recordings
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     ├── renders
-    │   ├── adjective-animal-1
+    │   ├── file_1
     │   │    ├── filtered-recording.es
     │   │    ├── rendered-file-1.es
     │   │    ├── ...
     │   │    └── rendered-file-m.es
-    │   ├── adjective-animal-2
+    │   ├── file_2
     │   ├── ...
-    │   └── adjective-animal-n
+    │   └── file_n
     └── charidotella-configuration.toml
     ```
 
 6.  (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
```

### Comparing `charidotella-1.2.0/README.md` & `charidotella-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: charidotella
+Version: 2.0.0
+Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
+Home-page: https://github.com/neuromorphicsystems/charidotella
+Author: Alexandre Marcireau
+Author-email: alexandre.marcireau@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 ![banner](banner.png)
 
 Charidotella (https://en.wikipedia.org/wiki/Charidotella_sexpunctata) is a toolbox to organise and visualise Event Stream (.es) recordings.
 
 It supports Python 3.9, 3.10, and 3.11.
 
 - [Dependencies](#dependencies)
@@ -125,22 +137,22 @@
     my-wonderful-project
     ├── recordings
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     ├── renders
-    │   ├── adjective-animal-1
+    │   ├── file_1
     │   │    ├── filtered-recording.es
     │   │    ├── rendered-file-1.es
     │   │    ├── ...
     │   │    └── rendered-file-m.es
-    │   ├── adjective-animal-2
+    │   ├── file_2
     │   ├── ...
-    │   └── adjective-animal-n
+    │   └── file_n
     └── charidotella-configuration.toml
     ```
 
 6.  (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
```

### Comparing `charidotella-1.2.0/charidotella/__init__.py` & `charidotella-2.0.0/charidotella/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,18 +87,18 @@
     init_parser.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Replace the configuration if it exists",
     )
     init_parser.add_argument(
-        "--preserve-names",
-        "-p",
+        "--generate-names",
+        "-g",
         action="store_true",
-        help="Do not generate new names for the recordings",
+        help="Generate new names (adjective + animal) for the recordings",
     )
     init_parser.add_argument(
         "--spatiospectrograms",
         "-s",
         action="store_true",
         help="Generate spatio-spectrogram tasks",
     )
@@ -336,26 +336,26 @@
             path.resolve()
             for path in pathlib.Path(".").glob(args.glob)
             if path.is_file() and path.suffix == ".es"
         ]
         paths.sort(key=lambda path: (path.stem, path.parent))
         if len(paths) == 0:
             utilities.error(f'no .es files match "{args.glob}"')
-        if args.preserve_names:
+        if args.generate_names:
+            names = animals.generate_names(len(paths))
+        else:
             names = sorted([path.stem for path in paths])
             if len(names) != len(set(names)):
                 name_to_path: dict[str, pathlib.Path] = {}
                 for path in paths:
                     if path.stem in name_to_path:
                         utilities.error(
                             f'two files have the same name ("{name_to_path[path.stem]}" and "{path}"), rename one or do *not* use the flag --preserve-name'
                         )
                     name_to_path[path.stem] = path
-        else:
-            names = animals.generate_names(len(paths))
         attachments: dict[str, list[dict[str, str]]] = {}
         for name, path in zip(names, paths):
             for sibling in path.parent.iterdir():
                 if sibling != path and sibling.stem == path.stem:
                     if not name in attachments:
                         attachments[name] = []
                     attachments[name].append(
@@ -557,44 +557,61 @@
                             "tau": utilities.timestamp_to_timecode(100000),
                             "mode": "all",
                             "maximum": 10000.0,
                             "frequencies": 100,
                             "times": 1000,
                             "gamma": 0.5,
                         },
-                        "video-real-time": {
+                        "video-1x": {
                             "type": "video",
                             "icon": "🎬",
                             "frametime": utilities.timestamp_to_timecode(20000),
                             "tau": utilities.timestamp_to_timecode(200000),
                             "style": "exponential",
                             "on_color": "#F4C20D",
                             "off_color": "#1E88E5",
                             "idle_color": "#191919",
                             "cumulative_ratio": 0.01,
                             "timecode": True,
                             "h264_crf": 15,
                             "ffmpeg": "ffmpeg",
                             "scale": 1,
                         },
-                        "video-slow-motion": {
+                        "video-0.1x": {
                             "type": "video",
                             "icon": "🎬",
                             "frametime": utilities.timestamp_to_timecode(2000),
                             "tau": utilities.timestamp_to_timecode(20000),
                             "style": "exponential",
                             "on_color": "#F4C20D",
                             "off_color": "#1E88E5",
                             "idle_color": "#191919",
                             "cumulative_ratio": 0.01,
                             "timecode": True,
                             "h264_crf": 15,
                             "ffmpeg": "ffmpeg",
                             "scale": 1,
                         },
+                        "wiggle": {
+                            "type": "wiggle",
+                            "icon": "👋",
+                            "forward_duration": utilities.timestamp_to_timecode(
+                                1000000
+                            ),
+                            "tau_to_frametime_ratio": 3.0,
+                            "style": "cumulative",
+                            "idle_color": "#191919",
+                            "on_color": "#F4C20D",
+                            "off_color": "#1E88E5",
+                            "idle_color": "#191919",
+                            "cumulative_ratio": 0.01,
+                            "timecode": True,
+                            "ffmpeg": "ffmpeg",
+                            "scale": 1,
+                        },
                     },
                 },
                 configuration_file,
                 encoder=Encoder(),
             )
 
             configuration_file.write(
@@ -616,22 +633,22 @@
                                 "png_compression_level": 6,
                                 "background_color": "#191919",
                                 "scale": 1,
                             },
                         },
                         {
                             "parameters": {
-                                "suffix": ["100000-10000", "1000-100"],
+                                "suffix": ["100000-10000", "10000-1000"],
                                 "long_tau": [
                                     utilities.timestamp_to_timecode(100000),
-                                    utilities.timestamp_to_timecode(1000),
+                                    utilities.timestamp_to_timecode(10000),
                                 ],
                                 "short_tau": [
                                     utilities.timestamp_to_timecode(10000),
-                                    utilities.timestamp_to_timecode(100),
+                                    utilities.timestamp_to_timecode(1000),
                                 ],
                             },
                             "template": {
                                 "name": "event-rate-@suffix",
                                 "type": "event_rate",
                                 "icon": "🎢",
                                 "long_tau": "@long_tau",
@@ -641,41 +658,14 @@
                                 "axis_color": "#000000",
                                 "main_grid_color": "#555555",
                                 "secondary_grid_color": "#DDDDDD",
                                 "width": 1280,
                                 "height": 720,
                             },
                         },
-                        {
-                            "parameters": {
-                                "suffix": ["4s", "2s", "1s", "0.5s"],
-                                "forward_duration": [
-                                    utilities.timestamp_to_timecode(2000000),
-                                    utilities.timestamp_to_timecode(1000000),
-                                    utilities.timestamp_to_timecode(500000),
-                                    utilities.timestamp_to_timecode(250000),
-                                ],
-                            },
-                            "template": {
-                                "name": "wiggle-@suffix",
-                                "type": "wiggle",
-                                "icon": "👋",
-                                "forward_duration": "@raw(forward_duration)",
-                                "tau_to_frametime_ratio": 3.0,
-                                "style": "cumulative",
-                                "idle_color": "#191919",
-                                "on_color": "#F4C20D",
-                                "off_color": "#1E88E5",
-                                "idle_color": "#191919",
-                                "cumulative_ratio": 0.01,
-                                "timecode": True,
-                                "ffmpeg": "ffmpeg",
-                                "scale": 1,
-                            },
-                        },
                     ]
                 },
                 configuration_file,
                 encoder=Encoder(),
             )
 
             configuration_file.write(
@@ -715,16 +705,16 @@
                                         "begin": "job-begin",
                                         "end": "job-end",
                                         "filters": ["arbiter-saturation-@threshold"],
                                         "tasks": [
                                             "colourtime-.+",
                                             "event-rate-.+",
                                             "spectrogram",
-                                            "wiggle-.+",
-                                            "video-real-time",
+                                            "wiggle",
+                                            "video-1x",
                                         ]
                                         + (
                                             ["spatiospectrogram"]
                                             if args.spatiospectrograms
                                             else []
                                         ),
                                     },
```

### Comparing `charidotella-1.2.0/charidotella/animals.py` & `charidotella-2.0.0/charidotella/animals.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/assets/configuration-schema.json` & `charidotella-2.0.0/charidotella/assets/configuration-schema.json`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/assets/es_to_frames` & `charidotella-2.0.0/charidotella/assets/es_to_frames`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -27,14 +27,14 @@
   [22] .init_array       INIT_ARRAY      00000000000fbd28 0fad28 000010 08  WA  0   0  8
   [23] .fini_array       FINI_ARRAY      00000000000fbd38 0fad38 000008 08  WA  0   0  8
   [24] .data.rel.ro      PROGBITS        00000000000fbd40 0fad40 000c48 00  WA  0   0 32
   [25] .dynamic          DYNAMIC         00000000000fc988 0fb988 000220 10  WA  7   0  8
   [26] .got              PROGBITS        00000000000fcba8 0fbba8 000440 08  WA  0   0  8
   [27] .data             PROGBITS        00000000000fd000 0fc000 000438 00  WA  0   0 32
   [28] .bss              NOBITS          00000000000fd440 0fc438 000420 00  WA  0   0 64
-  [29] .comment          PROGBITS        0000000000000000 0fc438 00002b 01  MS  0   0  1
-  [30] .shstrtab         STRTAB          0000000000000000 0fc463 000129 00      0   0  1
+  [29] .comment          PROGBITS        0000000000000000 0fc438 00002d 01  MS  0   0  1
+  [30] .shstrtab         STRTAB          0000000000000000 0fc465 000129 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000020	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK, x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 26f4b2b098ac44acf13aa41ea8d532bb7e7b4ae1
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 04141307f889f6d1633422fc5001eeade128c4e1
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -649,15 +649,15 @@
 NSt8__detail12_CharMatcherINSt7__cxx1112regex_traitsIcEELb1ELb0EEE
 NSt8__detail12_CharMatcherINSt7__cxx1112regex_traitsIcEELb1ELb1EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb0ELb0EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb0ELb1EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb1ELb0EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb1ELb1EEE
 00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 .shstrtab
 .note.gnu.property
 .note.gnu.build-id
 .note.ABI-tag
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

### Comparing `charidotella-1.2.0/charidotella/assets/event_rate` & `charidotella-2.0.0/charidotella/assets/event_rate`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -27,14 +27,14 @@
   [22] .init_array       INIT_ARRAY      0000000000044be8 043be8 000010 08  WA  0   0  8
   [23] .fini_array       FINI_ARRAY      0000000000044bf8 043bf8 000008 08  WA  0   0  8
   [24] .data.rel.ro      PROGBITS        0000000000044c00 043c00 000df0 00  WA  0   0 32
   [25] .dynamic          DYNAMIC         00000000000459f0 0449f0 000220 10  WA  7   0  8
   [26] .got              PROGBITS        0000000000045c10 044c10 0003e8 08  WA  0   0  8
   [27] .data             PROGBITS        0000000000046000 045000 000438 00  WA  0   0 32
   [28] .bss              NOBITS          0000000000046440 045438 000198 00  WA  0   0 32
-  [29] .comment          PROGBITS        0000000000000000 045438 00002b 01  MS  0   0  1
-  [30] .shstrtab         STRTAB          0000000000000000 045463 000129 00      0   0  1
+  [29] .comment          PROGBITS        0000000000000000 045438 00002d 01  MS  0   0  1
+  [30] .shstrtab         STRTAB          0000000000000000 045465 000129 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000020	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK, x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 012fb5c1e0aef7fdd82e53b4fecf3e717aa44b00
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 4c05017e25ea262b1a305eb4a5b1cc938831a5fc
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -619,15 +619,15 @@
 NSt8__detail12_CharMatcherINSt7__cxx1112regex_traitsIcEELb1ELb1EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb0ELb0EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb0ELb1EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb1ELb0EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb1ELb1EEE
 00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
 00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 .shstrtab
 .note.gnu.property
 .note.gnu.build-id
 .note.ABI-tag
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

### Comparing `charidotella-1.2.0/charidotella/assets/size` & `charidotella-2.0.0/charidotella/assets/size`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -27,14 +27,14 @@
   [22] .init_array       INIT_ARRAY      000000000000f9c8 00e9c8 000010 08  WA  0   0  8
   [23] .fini_array       FINI_ARRAY      000000000000f9d8 00e9d8 000008 08  WA  0   0  8
   [24] .data.rel.ro      PROGBITS        000000000000f9e0 00e9e0 000218 00  WA  0   0 32
   [25] .dynamic          DYNAMIC         000000000000fbf8 00ebf8 000210 10  WA  7   0  8
   [26] .got              PROGBITS        000000000000fe08 00ee08 0001f0 08  WA  0   0  8
   [27] .data             PROGBITS        0000000000010000 00f000 000020 00  WA  0   0  8
   [28] .bss              NOBITS          0000000000010040 00f020 000238 00  WA  0   0 64
-  [29] .comment          PROGBITS        0000000000000000 00f020 00002b 01  MS  0   0  1
-  [30] .shstrtab         STRTAB          0000000000000000 00f04b 000129 00      0   0  1
+  [29] .comment          PROGBITS        0000000000000000 00f020 00002d 01  MS  0   0  1
+  [30] .shstrtab         STRTAB          0000000000000000 00f04d 000129 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000020	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK, x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 9dbc13f14b032f18caea7a36b1d197be067349f5
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: fa09cadf2fd907bfd0bd2570dcdc12673eda9681
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -142,15 +142,15 @@
 Unknown option name or alias '
 N5sepia15unreadable_fileE
 N5sepia15wrong_signatureE
 N5sepia19unsupported_versionE
 N5sepia17incomplete_headerE
 N5sepia22unsupported_event_typeE
 00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 .shstrtab
 .note.gnu.property
 .note.gnu.build-id
 .note.ABI-tag
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

### Comparing `charidotella-1.2.0/charidotella/assets/spatiospectrogram` & `charidotella-2.0.0/charidotella/assets/spatiospectrogram`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -27,14 +27,14 @@
   [22] .init_array       INIT_ARRAY      00000000000f5ea8 0f4ea8 000010 08  WA  0   0  8
   [23] .fini_array       FINI_ARRAY      00000000000f5eb8 0f4eb8 000008 08  WA  0   0  8
   [24] .data.rel.ro      PROGBITS        00000000000f5ec0 0f4ec0 000ac0 00  WA  0   0 32
   [25] .dynamic          DYNAMIC         00000000000f6980 0f5980 000220 10  WA  7   0  8
   [26] .got              PROGBITS        00000000000f6ba0 0f5ba0 000448 08  WA  0   0  8
   [27] .data             PROGBITS        00000000000f7000 0f6000 000438 00  WA  0   0 32
   [28] .bss              NOBITS          00000000000f7440 0f6438 000720 00  WA  0   0 64
-  [29] .comment          PROGBITS        0000000000000000 0f6438 00002b 01  MS  0   0  1
-  [30] .shstrtab         STRTAB          0000000000000000 0f6463 000129 00      0   0  1
+  [29] .comment          PROGBITS        0000000000000000 0f6438 00002d 01  MS  0   0  1
+  [30] .shstrtab         STRTAB          0000000000000000 0f6465 000129 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000020	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK, x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: fc119613b4dbacd375b0468a30b09cd16a75bbc0
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: cc01d26749221d619ac22b00f00d073c41d73822
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -608,15 +608,15 @@
 NSt8__detail12_CharMatcherINSt7__cxx1112regex_traitsIcEELb1ELb0EEE
 NSt8__detail12_CharMatcherINSt7__cxx1112regex_traitsIcEELb1ELb1EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb0ELb0EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb0ELb1EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb1ELb0EEE
 NSt8__detail15_BracketMatcherINSt7__cxx1112regex_traitsIcEELb1ELb1EEE
 00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 .shstrtab
 .note.gnu.property
 .note.gnu.build-id
 .note.ABI-tag
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

### Comparing `charidotella-1.2.0/charidotella/assets/spectrogram` & `charidotella-2.0.0/charidotella/assets/spectrogram`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -27,14 +27,14 @@
   [22] .init_array       INIT_ARRAY      000000000005fce8 05ece8 000010 08  WA  0   0  8
   [23] .fini_array       FINI_ARRAY      000000000005fcf8 05ecf8 000008 08  WA  0   0  8
   [24] .data.rel.ro      PROGBITS        000000000005fd00 05ed00 000c98 00  WA  0   0 32
   [25] .dynamic          DYNAMIC         0000000000060998 05f998 000220 10  WA  7   0  8
   [26] .got              PROGBITS        0000000000060bb8 05fbb8 000438 08  WA  0   0  8
   [27] .data             PROGBITS        0000000000061000 060000 000440 00  WA  0   0 32
   [28] .bss              NOBITS          0000000000061440 060440 0004a8 00  WA  0   0 32
-  [29] .comment          PROGBITS        0000000000000000 060440 00002b 01  MS  0   0  1
-  [30] .shstrtab         STRTAB          0000000000000000 06046b 000129 00      0   0  1
+  [29] .comment          PROGBITS        0000000000000000 060440 00002d 01  MS  0   0  1
+  [30] .shstrtab         STRTAB          0000000000000000 06046d 000129 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000020	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK, x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: d33fd77174a2c14e944ab59329daedfc9a3465aa
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0d5d264b4def163f890e97e9a5c7ddd7be0653a2
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -769,15 +769,15 @@
 integer overflow with combined idat chunk size
 invalid ICC profile color type, the PNG specification only allows RGB or GRAY
 PNG specification does not allow RGB ICC profile on gray color types and vice versa
 not allowed to set grayscale ICC profile with colored pixels by PNG specification
 invalid palette index in bKGD chunk. Maybe it came before PLTE chunk?
 invalid bKGD color while encoding (e.g. palette index out of range)
 vector::_M_default_append
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 .shstrtab
 .note.gnu.property
 .note.gnu.build-id
 .note.ABI-tag
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

### Comparing `charidotella-1.2.0/charidotella/charidotella_extension_placeholder.c` & `charidotella-2.0.0/charidotella/charidotella_extension_placeholder.c`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/filters/arbiter_saturation.py` & `charidotella-2.0.0/charidotella/filters/arbiter_saturation.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/filters/default.py` & `charidotella-2.0.0/charidotella/filters/default.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/filters/hot_pixels.py` & `charidotella-2.0.0/charidotella/filters/hot_pixels.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/filters/refractory.py` & `charidotella-2.0.0/charidotella/filters/refractory.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/filters/transpose.py` & `charidotella-2.0.0/charidotella/filters/transpose.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/tasks/colourtime.py` & `charidotella-2.0.0/charidotella/tasks/colourtime.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/tasks/event_rate.py` & `charidotella-2.0.0/charidotella/tasks/event_rate.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/tasks/spatiospectrogram.py` & `charidotella-2.0.0/charidotella/tasks/spatiospectrogram.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/tasks/spectrogram.py` & `charidotella-2.0.0/charidotella/tasks/spectrogram.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/tasks/video.py` & `charidotella-2.0.0/charidotella/tasks/video.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/tasks/wiggle.py` & `charidotella-2.0.0/charidotella/tasks/wiggle.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella/utilities.py` & `charidotella-2.0.0/charidotella/utilities.py`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/charidotella.egg-info/PKG-INFO` & `charidotella-2.0.0/charidotella.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charidotella
-Version: 1.2.0
+Version: 2.0.0
 Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
 Home-page: https://github.com/neuromorphicsystems/charidotella
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -137,22 +137,22 @@
     my-wonderful-project
     ├── recordings
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     ├── renders
-    │   ├── adjective-animal-1
+    │   ├── file_1
     │   │    ├── filtered-recording.es
     │   │    ├── rendered-file-1.es
     │   │    ├── ...
     │   │    └── rendered-file-m.es
-    │   ├── adjective-animal-2
+    │   ├── file_2
     │   ├── ...
-    │   └── adjective-animal-n
+    │   └── file_n
     └── charidotella-configuration.toml
     ```
 
 6.  (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
```

### Comparing `charidotella-1.2.0/charidotella.egg-info/SOURCES.txt` & `charidotella-2.0.0/charidotella.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/premake4.lua` & `charidotella-2.0.0/command_line_tools/premake4.lua`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/crop.cpp` & `charidotella-2.0.0/command_line_tools/source/crop.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/cut.cpp` & `charidotella-2.0.0/command_line_tools/source/cut.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/dat.hpp` & `charidotella-2.0.0/command_line_tools/source/dat.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/dat_to_es.cpp` & `charidotella-2.0.0/command_line_tools/source/dat_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/es_to_csv.cpp` & `charidotella-2.0.0/command_line_tools/source/es_to_csv.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/es_to_frames.cpp` & `charidotella-2.0.0/command_line_tools/source/es_to_frames.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/es_to_ply.cpp` & `charidotella-2.0.0/command_line_tools/source/es_to_ply.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/event_rate.cpp` & `charidotella-2.0.0/command_line_tools/source/event_rate.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/evt3.hpp` & `charidotella-2.0.0/command_line_tools/source/evt3.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/evt3_to_es.cpp` & `charidotella-2.0.0/command_line_tools/source/evt3_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/font.hpp` & `charidotella-2.0.0/command_line_tools/source/font.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/html.hpp` & `charidotella-2.0.0/command_line_tools/source/html.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/rainbow.cpp` & `charidotella-2.0.0/command_line_tools/source/rainbow.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/rainmaker.cpp` & `charidotella-2.0.0/command_line_tools/source/rainmaker.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/size.cpp` & `charidotella-2.0.0/command_line_tools/source/size.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/spatiospectrogram.cpp` & `charidotella-2.0.0/command_line_tools/source/spatiospectrogram.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/spectrogram.cpp` & `charidotella-2.0.0/command_line_tools/source/spectrogram.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/statistics.cpp` & `charidotella-2.0.0/command_line_tools/source/statistics.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/synth.cpp` & `charidotella-2.0.0/command_line_tools/source/synth.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/source/timecode.hpp` & `charidotella-2.0.0/command_line_tools/source/timecode.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/third_party/lodepng/lodepng.cpp` & `charidotella-2.0.0/command_line_tools/third_party/lodepng/lodepng.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/third_party/lodepng/lodepng.h` & `charidotella-2.0.0/command_line_tools/third_party/lodepng/lodepng.h`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/third_party/monaco.ttf.base64.hpp` & `charidotella-2.0.0/command_line_tools/third_party/monaco.ttf.base64.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/third_party/pontella/source/pontella.hpp` & `charidotella-2.0.0/command_line_tools/third_party/pontella/source/pontella.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/third_party/sepia/source/sepia.hpp` & `charidotella-2.0.0/command_line_tools/third_party/sepia/source/sepia.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/third_party/stb_truetype.hpp` & `charidotella-2.0.0/command_line_tools/third_party/stb_truetype.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/third_party/tarsier/source/replicate.hpp` & `charidotella-2.0.0/command_line_tools/third_party/tarsier/source/replicate.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/command_line_tools/third_party/tarsier/source/stitch.hpp` & `charidotella-2.0.0/command_line_tools/third_party/tarsier/source/stitch.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/configuration-schema.json` & `charidotella-2.0.0/configuration-schema.json`

 * *Files identical despite different names*

### Comparing `charidotella-1.2.0/setup.py` & `charidotella-2.0.0/setup.py`

 * *Files identical despite different names*

