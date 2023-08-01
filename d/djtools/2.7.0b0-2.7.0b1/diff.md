# Comparing `tmp/djtools-2.7.0b0.tar.gz` & `tmp/djtools-2.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djtools-2.7.0b0.tar", last modified: Sat Jul 29 19:28:59 2023, max compression
+gzip compressed data, was "djtools-2.7.0b1.tar", last modified: Tue Aug  1 16:32:28 2023, max compression
```

## Comparing `djtools-2.7.0b0.tar` & `djtools-2.7.0b1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.196725 djtools-2.7.0b0/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 djtools-2.7.0b0/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 djtools-2.7.0b0/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2864 2023-07-29 19:28:59.196855 djtools-2.7.0b0/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1632 2023-07-29 18:53:45.000000 djtools-2.7.0b0/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.166823 djtools-2.7.0b0/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2621 2023-07-29 19:17:36.000000 djtools-2.7.0b0/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-29 19:17:36.000000 djtools-2.7.0b0/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.180351 djtools-2.7.0b0/djtools/collection/
--rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2914 2023-07-26 18:56:00.000000 djtools-2.7.0b0/djtools/collection/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27429 2023-07-26 18:56:00.000000 djtools-2.7.0b0/djtools/collection/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7697 2023-07-26 18:56:00.000000 djtools-2.7.0b0/djtools/collection/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13886 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/collection/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.185634 djtools-2.7.0b0/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 djtools-2.7.0b0/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-26 18:24:13.000000 djtools-2.7.0b0/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1495 2023-07-29 19:18:55.000000 djtools-2.7.0b0/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    22288 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 djtools-2.7.0b0/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:30.000000 djtools-2.7.0b0/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.186326 djtools-2.7.0b0/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.7.0b0/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.189214 djtools-2.7.0b0/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.191517 djtools-2.7.0b0/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-22 20:25:43.000000 djtools-2.7.0b0/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5343 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.196253 djtools-2.7.0b0/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)     1441 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4233 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2130 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9264 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1719 2023-07-29 19:24:52.000000 djtools-2.7.0b0/djtools/utils/normalize_audio.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5138 2023-07-29 19:24:55.000000 djtools-2.7.0b0/djtools/utils/process_recording.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 djtools-2.7.0b0/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-29 18:53:45.000000 djtools-2.7.0b0/djtools/version.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:59.172909 djtools-2.7.0b0/djtools.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2864 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1277 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      278 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-29 19:28:59.000000 djtools-2.7.0b0/djtools.egg-info/top_level.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 djtools-2.7.0b0/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-29 19:28:59.197283 djtools-2.7.0b0/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2361 2023-07-29 19:17:36.000000 djtools-2.7.0b0/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.806547 djtools-2.7.0b1/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 djtools-2.7.0b1/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 djtools-2.7.0b1/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2864 2023-08-01 16:32:28.806641 djtools-2.7.0b1/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1632 2023-07-29 18:53:45.000000 djtools-2.7.0b1/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.767990 djtools-2.7.0b1/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2621 2023-07-29 19:17:36.000000 djtools-2.7.0b1/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-29 19:17:36.000000 djtools-2.7.0b1/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.786082 djtools-2.7.0b1/djtools/collection/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2914 2023-07-26 18:56:00.000000 djtools-2.7.0b1/djtools/collection/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27429 2023-07-26 18:56:00.000000 djtools-2.7.0b1/djtools/collection/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7697 2023-07-26 18:56:00.000000 djtools-2.7.0b1/djtools/collection/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13886 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.793626 djtools-2.7.0b1/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 djtools-2.7.0b1/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-26 18:24:13.000000 djtools-2.7.0b1/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1485 2023-08-01 16:23:50.000000 djtools-2.7.0b1/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    22278 2023-08-01 15:46:44.000000 djtools-2.7.0b1/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 djtools-2.7.0b1/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:30.000000 djtools-2.7.0b1/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.794478 djtools-2.7.0b1/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.7.0b1/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.797211 djtools-2.7.0b1/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.799890 djtools-2.7.0b1/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5343 2023-07-29 18:53:45.000000 djtools-2.7.0b1/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.806016 djtools-2.7.0b1/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1441 2023-07-29 18:53:45.000000 djtools-2.7.0b1/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4233 2023-07-29 18:53:45.000000 djtools-2.7.0b1/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2120 2023-08-01 15:47:39.000000 djtools-2.7.0b1/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9264 2023-07-29 18:53:45.000000 djtools-2.7.0b1/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1859 2023-08-01 16:20:25.000000 djtools-2.7.0b1/djtools/utils/normalize_audio.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5098 2023-08-01 15:47:27.000000 djtools-2.7.0b1/djtools/utils/process_recording.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 djtools-2.7.0b1/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-08-01 16:15:23.000000 djtools-2.7.0b1/djtools/version.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.775431 djtools-2.7.0b1/djtools.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2864 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1277 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      278 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/top_level.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 djtools-2.7.0b1/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-08-01 16:32:28.807159 djtools-2.7.0b1/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2361 2023-07-29 19:17:36.000000 djtools-2.7.0b1/setup.py
```

### Comparing `djtools-2.7.0b0/LICENSE` & `djtools-2.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/PKG-INFO` & `djtools-2.7.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djtools
-Version: 2.7.0b0
+Version: 2.7.0b1
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `djtools-2.7.0b0/README.md` & `djtools-2.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/__init__.py` & `djtools-2.7.0b1/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/__main__.py` & `djtools-2.7.0b1/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/__init__.py` & `djtools-2.7.0b1/djtools/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/collections.py` & `djtools-2.7.0b1/djtools/collection/collections.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/config.py` & `djtools-2.7.0b1/djtools/collection/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/copy_playlists.py` & `djtools-2.7.0b1/djtools/collection/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/helpers.py` & `djtools-2.7.0b1/djtools/collection/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/playlist_builder.py` & `djtools-2.7.0b1/djtools/collection/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/playlists.py` & `djtools-2.7.0b1/djtools/collection/playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/shuffle_playlists.py` & `djtools-2.7.0b1/djtools/collection/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/collection/tracks.py` & `djtools-2.7.0b1/djtools/collection/tracks.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/configs/collection_playlists.yaml` & `djtools-2.7.0b1/djtools/configs/collection_playlists.yaml`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/configs/config.py` & `djtools-2.7.0b1/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/configs/config.yaml` & `djtools-2.7.0b1/djtools/configs/config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -43,18 +43,18 @@
   UPLOAD_INCLUDE_DIRS: []
   UPLOAD_MUSIC: false
   USB_PATH: null
   USER: ''
 utils:
   AUDIO_BITRATE: 320k
   AUDIO_FORMAT: mp3
+  AUDIO_HEADROOM: 0.0
   CHECK_TRACKS: false
   CHECK_TRACKS_FUZZ_RATIO: 80
   CHECK_TRACKS_SPOTIFY_PLAYLISTS: []
   LOCAL_DIRS: []
   NORMALIZE_AUDIO: false
-  NORMALIZE_AUDIO_HEADROOM: 0.0
   PROCESS_RECORDING: false
   RECORDING_FILE: null
   RECORDING_PLAYLIST: ''
   URL_DOWNLOAD: ''
   URL_DOWNLOAD_DESTINATION: null
```

### Comparing `djtools-2.7.0b0/djtools/configs/helpers.py` & `djtools-2.7.0b1/djtools/configs/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,14 +440,19 @@
     )
     utils_parser.add_argument(
         "--audio-format",
         type=str,
         help='File format to save files output by "--process-recording"',
     )
     utils_parser.add_argument(
+        "--audio-headroom",
+        type=float,
+        help="Amount of headroom in decibels to leave when normalizing audio.",
+    )
+    utils_parser.add_argument(
         "--check-tracks",
         action="store_true",
         help=(
             "Flag to trigger checking for track overlap between the Beatcloud "
             'and "--local-dirs" and / or "--check-tracks-spotify-playlists".'
         ),
     )
@@ -474,19 +479,14 @@
     )
     utils_parser.add_argument(
         "--normalize-audio",
         action="store_true",
         help='Flag to trigger normalizing audio files at "--local-dirs".',
     )
     utils_parser.add_argument(
-        "--normalize-audio-headroom",
-        type=float,
-        help="Amount of headroom in decibels to leave when normalizing audio.",
-    )
-    utils_parser.add_argument(
         "--process-recording",
         action="store_true",
         help=(
             "Flag to trigger processing an audio recording using a Spotify "
             "playlist."
         ),
     )
```

### Comparing `djtools-2.7.0b0/djtools/spotify/__init__.py` & `djtools-2.7.0b1/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/spotify/config.py` & `djtools-2.7.0b1/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/spotify/helpers.py` & `djtools-2.7.0b1/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/spotify/playlist_builder.py` & `djtools-2.7.0b1/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/sync/__init__.py` & `djtools-2.7.0b1/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/sync/config.py` & `djtools-2.7.0b1/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/sync/helpers.py` & `djtools-2.7.0b1/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/sync/sync_operations.py` & `djtools-2.7.0b1/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/utils/__init__.py` & `djtools-2.7.0b1/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/utils/check_tracks.py` & `djtools-2.7.0b1/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/utils/config.py` & `djtools-2.7.0b1/djtools/utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
 
 class UtilsConfig(BaseConfig):
     """Configuration object for the utils package."""
 
     AUDIO_BITRATE: str = '320k'
     AUDIO_FORMAT: str = 'mp3'
+    AUDIO_HEADROOM: NonNegativeFloat = 0.0
     CHECK_TRACKS: bool = False
     CHECK_TRACKS_FUZZ_RATIO: NonNegativeInt = 80
     CHECK_TRACKS_SPOTIFY_PLAYLISTS:  List[str] = []
     LOCAL_DIRS: List[Path] = []
     NORMALIZE_AUDIO: bool = False
-    NORMALIZE_AUDIO_HEADROOM: NonNegativeFloat = 0.0
     PROCESS_RECORDING: bool = False
     RECORDING_FILE: Path = None
     RECORDING_PLAYLIST: str = ""
     URL_DOWNLOAD: str = ""
     URL_DOWNLOAD_DESTINATION: Path = None
 
     def __init__(self, *args, **kwargs):
```

### Comparing `djtools-2.7.0b0/djtools/utils/helpers.py` & `djtools-2.7.0b1/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools/utils/normalize_audio.py` & `djtools-2.7.0b1/djtools/utils/normalize_audio.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def normalize(config: BaseConfig):
     """Gets local tracks and normalizes them.
 
-    Tracks will be overwritten and have a headroom equal to
-    NORMALIZE_AUDIO_HEADROOM.
+    Tracks will be overwritten and have a headroom equal to AUDIO_HEADROOM.
 
     Args:
         config: Configuration object.
 
     Raises:
         RuntimeError: Must have local tracks to normalize.
     """
@@ -28,30 +27,32 @@
         raise RuntimeError(
             "There are no local tracks; make sure LOCAL_DIRS has one or "
             "more directories containing one or more tracks"
         )
 
     for track in [
         track for tracks in folder_tracks.values() for track in tracks
+        if track.is_file() and not track.name.startswith(".")
     ]:
-        audio = AudioSegment.from_file(track)
+        try:
+            audio = AudioSegment.from_file(track)
+        except Exception as exc:
+            logger.error(f"Couldn't decode {track}: {exc}")
+            continue
 
-        if abs(audio.max_dBFS + config.NORMALIZE_AUDIO_HEADROOM) > 0.001:
+        if abs(audio.max_dBFS + config.AUDIO_HEADROOM) > 0.001:
             logger.info(
                 f"{track} has a max dB of {audio.max_dBFS}, normalizing to "
-                f"have a headroom of {config.NORMALIZE_AUDIO_HEADROOM}..."
-            )
-            audio = effects.normalize(
-                audio, headroom=config.NORMALIZE_AUDIO_HEADROOM
+                f"have a headroom of {config.AUDIO_HEADROOM}..."
             )
+            audio = effects.normalize(audio, headroom=config.AUDIO_HEADROOM)
             audio.export(
-                track,
+                track.parent / f"{track.stem}.{config.AUDIO_FORMAT}",
                 tags=utils.mediainfo(track).get("TAG", {}),
                 bitrate=config.AUDIO_BITRATE,
                 format=config.AUDIO_FORMAT,
             )
             continue
 
         logger.info(
-            f"{track} already has a headroom of "
-            f"{config.NORMALIZE_AUDIO_HEADROOM}"
+            f"{track} already has a headroom of {config.AUDIO_HEADROOM}"
         )
```

### Comparing `djtools-2.7.0b0/djtools/utils/process_recording.py` & `djtools-2.7.0b1/djtools/utils/process_recording.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Given a recording of multiple tracks and a Spotify playlist, use the
 information from the Spotify API to:
 
 - split the recording into individual files
 - name these files with the title and artist(s)
 - populate the title, artist, and album tags
-- normalize the audio so the headroom is NORMALIZE_AUDIO_HEADROOM decibels
+- normalize the audio so the headroom is AUDIO_HEADROOM decibels
 - export the files with the configured AUDIO_BITRATE and AUDIO_FORMAT
 """
 from datetime import datetime
 import logging
 
 from pydub import AudioSegment, effects
 
@@ -85,18 +85,18 @@
     write_path.mkdir(parents=True, exist_ok=True)
     for track in track_data:
         # Slice the portion of the recording for the track.
         track_audio = audio[:track["duration"]]
         audio = audio[track["duration"]:]
 
         # Normalize the audio such that the headroom is
-        # NORMALIZE_AUDIO_HEADROOM dB.
-        if abs(track_audio.max_dBFS + config.NORMALIZE_AUDIO_HEADROOM) > 0.001:
+        # AUDIO_HEADROOM dB.
+        if abs(track_audio.max_dBFS + config.AUDIO_HEADROOM) > 0.001:
             track_audio = effects.normalize(
-                track_audio, headroom=config.NORMALIZE_AUDIO_HEADROOM
+                track_audio, headroom=config.AUDIO_HEADROOM
             )
 
         # Build the filename using the title, artist(s) and configured format.
         filename = (
             f'{track["artist"]} - {track["title"]}' if config.ARTIST_FIRST
             else f'{track["title"]} - {track["artist"]}'
         )
```

### Comparing `djtools-2.7.0b0/djtools/utils/url_download.py` & `djtools-2.7.0b1/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/djtools.egg-info/PKG-INFO` & `djtools-2.7.0b1/djtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djtools
-Version: 2.7.0b0
+Version: 2.7.0b1
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `djtools-2.7.0b0/djtools.egg-info/SOURCES.txt` & `djtools-2.7.0b1/djtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b0/setup.py` & `djtools-2.7.0b1/setup.py`

 * *Files identical despite different names*

