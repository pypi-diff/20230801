# Comparing `tmp/audioscrape-0.3.0.tar.gz` & `tmp/audioscrape-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioscrape-0.3.0.tar", last modified: Wed Jul 26 22:55:33 2023, max compression
+gzip compressed data, was "audioscrape-0.3.1.tar", last modified: Tue Aug  1 00:34:05 2023, max compression
```

## Comparing `audioscrape-0.3.0.tar` & `audioscrape-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:33.597864 audioscrape-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 22:55:23.000000 audioscrape-0.3.0/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:33.589864 audioscrape-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:33.589864 audioscrape-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-26 22:55:23.000000 audioscrape-0.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-26 22:55:23.000000 audioscrape-0.3.0/.github/workflows/pre-commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 22:55:23.000000 audioscrape-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 22:55:23.000000 audioscrape-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 22:55:23.000000 audioscrape-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-26 22:55:33.597864 audioscrape-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-26 22:55:23.000000 audioscrape-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:33.593864 audioscrape-0.3.0/audioscrape/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-26 22:55:23.000000 audioscrape-0.3.0/audioscrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-26 22:55:23.000000 audioscrape-0.3.0/audioscrape/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 22:55:23.000000 audioscrape-0.3.0/audioscrape/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 22:55:23.000000 audioscrape-0.3.0/audioscrape/freesound.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 22:55:23.000000 audioscrape-0.3.0/audioscrape/soundcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 22:55:33.000000 audioscrape-0.3.0/audioscrape/version.py
--rw-r--r--   0 runner    (1001) docker     (123)  4126810 2023-07-26 22:55:23.000000 audioscrape-0.3.0/audioscrape/yamnet.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-26 22:55:23.000000 audioscrape-0.3.0/audioscrape/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:33.597864 audioscrape-0.3.0/audioscrape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-26 22:55:33.000000 audioscrape-0.3.0/audioscrape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-26 22:55:33.000000 audioscrape-0.3.0/audioscrape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:55:33.000000 audioscrape-0.3.0/audioscrape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 22:55:33.000000 audioscrape-0.3.0/audioscrape.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-26 22:55:33.000000 audioscrape-0.3.0/audioscrape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 22:55:33.000000 audioscrape-0.3.0/audioscrape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-26 22:55:23.000000 audioscrape-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:55:33.597864 audioscrape-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:33.597864 audioscrape-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   320991 2023-07-26 22:55:23.000000 audioscrape-0.3.0/tests/example.mp3
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-26 22:55:23.000000 audioscrape-0.3.0/tests/test_audioscrape.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 22:55:23.000000 audioscrape-0.3.0/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:34:05.924122 audioscrape-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 00:33:50.000000 audioscrape-0.3.1/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:34:05.916122 audioscrape-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:34:05.916122 audioscrape-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-01 00:33:50.000000 audioscrape-0.3.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 00:33:50.000000 audioscrape-0.3.1/.github/workflows/pre-commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 00:33:50.000000 audioscrape-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 00:33:50.000000 audioscrape-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 00:33:50.000000 audioscrape-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-08-01 00:34:05.924122 audioscrape-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 00:33:50.000000 audioscrape-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:34:05.924122 audioscrape-0.3.1/audioscrape/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 00:33:50.000000 audioscrape-0.3.1/audioscrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-01 00:33:50.000000 audioscrape-0.3.1/audioscrape/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 00:33:50.000000 audioscrape-0.3.1/audioscrape/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 00:33:50.000000 audioscrape-0.3.1/audioscrape/freesound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-01 00:33:50.000000 audioscrape-0.3.1/audioscrape/soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 00:34:05.000000 audioscrape-0.3.1/audioscrape/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4126810 2023-08-01 00:33:50.000000 audioscrape-0.3.1/audioscrape/yamnet.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-01 00:33:50.000000 audioscrape-0.3.1/audioscrape/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:34:05.924122 audioscrape-0.3.1/audioscrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-08-01 00:34:05.000000 audioscrape-0.3.1/audioscrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-01 00:34:05.000000 audioscrape-0.3.1/audioscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:34:05.000000 audioscrape-0.3.1/audioscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 00:34:05.000000 audioscrape-0.3.1/audioscrape.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 00:34:05.000000 audioscrape-0.3.1/audioscrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 00:34:05.000000 audioscrape-0.3.1/audioscrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-01 00:33:50.000000 audioscrape-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:34:05.924122 audioscrape-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:34:05.924122 audioscrape-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   320991 2023-08-01 00:33:50.000000 audioscrape-0.3.1/tests/example.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-01 00:33:50.000000 audioscrape-0.3.1/tests/test_audioscrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 00:33:50.000000 audioscrape-0.3.1/tests/test_classify.py
```

### Comparing `audioscrape-0.3.0/.github/workflows/ci.yaml` & `audioscrape-0.3.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/.pre-commit-config.yaml` & `audioscrape-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/LICENSE` & `audioscrape-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/PKG-INFO` & `audioscrape-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioscrape
-Version: 0.3.0
+Version: 0.3.1
 Summary: Scrape online audio with a simple command-line interface.
 Author-email: Carl Thomé <carlthome@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Thomé
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `audioscrape-0.3.0/README.md` & `audioscrape-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/audioscrape/__main__.py` & `audioscrape-0.3.1/audioscrape/__main__.py`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/audioscrape/classify.py` & `audioscrape-0.3.1/audioscrape/classify.py`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/audioscrape/soundcloud.py` & `audioscrape-0.3.1/audioscrape/soundcloud.py`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/audioscrape/yamnet.tflite` & `audioscrape-0.3.1/audioscrape/yamnet.tflite`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/audioscrape/youtube.py` & `audioscrape-0.3.1/audioscrape/youtube.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             "nooverwrites": not overwrite,
             "writeinfojson": True,
             "writethumbnail": True,
             "writedescription": True,
             "postprocessors": [
                 {
                     "key": "FFmpegExtractAudio",
-                    "preferredcodec": "ogg",
+                    "preferredcodec": "vorbis",
                     "preferredquality": "192",
                 }
             ],
         }
         ydl = yt.YoutubeDL(download_options)
 
         # Fetch metadata.
```

### Comparing `audioscrape-0.3.0/audioscrape.egg-info/PKG-INFO` & `audioscrape-0.3.1/audioscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioscrape
-Version: 0.3.0
+Version: 0.3.1
 Summary: Scrape online audio with a simple command-line interface.
 Author-email: Carl Thomé <carlthome@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Thomé
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `audioscrape-0.3.0/audioscrape.egg-info/SOURCES.txt` & `audioscrape-0.3.1/audioscrape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audioscrape-0.3.0/pyproject.toml` & `audioscrape-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 [project.urls]
 Homepage = "https://github.com/carlthome/audio-scraper"
 Bugs = "https://github.com/carlthome/audioscrape/issues"
 
 [tool.setuptools_scm]
 write_to = "audioscrape/version.py"
-version_scheme = "release-branch-semver"
 local_scheme = "no-local-version"
 
 [tool.black]
 line-length = 120
 
 [tool.pytest.ini_options]
 log_cli = true
```

### Comparing `audioscrape-0.3.0/tests/example.mp3` & `audioscrape-0.3.1/tests/example.mp3`

 * *Files identical despite different names*

