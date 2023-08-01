# Comparing `tmp/psychopy-whisper-0.0.1.tar.gz` & `tmp/psychopy-whisper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy-whisper-0.0.1.tar", last modified: Thu Jul 13 12:50:03 2023, max compression
+gzip compressed data, was "psychopy-whisper-0.0.2.tar", last modified: Tue Aug  1 19:59:31 2023, max compression
```

## Comparing `psychopy-whisper-0.0.1.tar` & `psychopy-whisper-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-07-13 12:50:03.611816 psychopy-whisper-0.0.1/
--rw-r--r--   0 mdc        (501) staff       (20)    35138 2023-07-12 08:42:45.000000 psychopy-whisper-0.0.1/LICENSE
--rw-r--r--   0 mdc        (501) staff       (20)     1753 2023-07-13 12:50:03.611917 psychopy-whisper-0.0.1/PKG-INFO
--rw-r--r--   0 mdc        (501) staff       (20)      586 2023-07-12 08:42:45.000000 psychopy-whisper-0.0.1/README.md
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-07-13 12:50:03.609997 psychopy-whisper-0.0.1/psychopy_whisper/
--rw-r--r--   0 mdc        (501) staff       (20)    12157 2023-07-13 12:19:31.000000 psychopy-whisper-0.0.1/psychopy_whisper/__init__.py
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-07-13 12:50:03.611361 psychopy-whisper-0.0.1/psychopy_whisper.egg-info/
--rw-r--r--   0 mdc        (501) staff       (20)     1753 2023-07-13 12:50:03.000000 psychopy-whisper-0.0.1/psychopy_whisper.egg-info/PKG-INFO
--rw-r--r--   0 mdc        (501) staff       (20)      355 2023-07-13 12:50:03.000000 psychopy-whisper-0.0.1/psychopy_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 mdc        (501) staff       (20)        1 2023-07-13 12:50:03.000000 psychopy-whisper-0.0.1/psychopy_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 mdc        (501) staff       (20)       85 2023-07-13 12:50:03.000000 psychopy-whisper-0.0.1/psychopy_whisper.egg-info/entry_points.txt
--rw-r--r--   0 mdc        (501) staff       (20)       23 2023-07-13 12:50:03.000000 psychopy-whisper-0.0.1/psychopy_whisper.egg-info/requires.txt
--rw-r--r--   0 mdc        (501) staff       (20)       28 2023-07-13 12:50:03.000000 psychopy-whisper-0.0.1/psychopy_whisper.egg-info/top_level.txt
--rw-r--r--   0 mdc        (501) staff       (20)     1433 2023-07-12 08:43:06.000000 psychopy-whisper-0.0.1/pyproject.toml
--rw-r--r--   0 mdc        (501) staff       (20)      103 2023-07-13 12:50:03.612267 psychopy-whisper-0.0.1/setup.cfg
-drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-07-13 12:50:03.611495 psychopy-whisper-0.0.1/tests/
--rw-r--r--   0 mdc        (501) staff       (20)      195 2023-07-12 08:46:51.000000 psychopy-whisper-0.0.1/tests/test_sound_transcription_whisper.py
+drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-08-01 19:59:31.118888 psychopy-whisper-0.0.2/
+-rw-r--r--   0 mdc        (501) staff       (20)    35138 2023-05-03 20:00:34.000000 psychopy-whisper-0.0.2/LICENSE
+-rw-r--r--   0 mdc        (501) staff       (20)     1753 2023-08-01 19:59:31.119004 psychopy-whisper-0.0.2/PKG-INFO
+-rw-r--r--   0 mdc        (501) staff       (20)      586 2023-05-03 20:00:34.000000 psychopy-whisper-0.0.2/README.md
+drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-08-01 19:59:31.117163 psychopy-whisper-0.0.2/psychopy_whisper/
+-rw-r--r--   0 mdc        (501) staff       (20)    12157 2023-08-01 19:57:50.000000 psychopy-whisper-0.0.2/psychopy_whisper/__init__.py
+drwxr-xr-x   0 mdc        (501) staff       (20)        0 2023-08-01 19:59:31.118733 psychopy-whisper-0.0.2/psychopy_whisper.egg-info/
+-rw-r--r--   0 mdc        (501) staff       (20)     1753 2023-08-01 19:59:31.000000 psychopy-whisper-0.0.2/psychopy_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 mdc        (501) staff       (20)      313 2023-08-01 19:59:31.000000 psychopy-whisper-0.0.2/psychopy_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 mdc        (501) staff       (20)        1 2023-08-01 19:59:31.000000 psychopy-whisper-0.0.2/psychopy_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 mdc        (501) staff       (20)       85 2023-08-01 19:59:31.000000 psychopy-whisper-0.0.2/psychopy_whisper.egg-info/entry_points.txt
+-rw-r--r--   0 mdc        (501) staff       (20)       41 2023-08-01 19:59:31.000000 psychopy-whisper-0.0.2/psychopy_whisper.egg-info/requires.txt
+-rw-r--r--   0 mdc        (501) staff       (20)       22 2023-08-01 19:59:31.000000 psychopy-whisper-0.0.2/psychopy_whisper.egg-info/top_level.txt
+-rw-r--r--   0 mdc        (501) staff       (20)     1456 2023-08-01 19:57:43.000000 psychopy-whisper-0.0.2/pyproject.toml
+-rw-r--r--   0 mdc        (501) staff       (20)      103 2023-08-01 19:59:31.119363 psychopy-whisper-0.0.2/setup.cfg
```

### Comparing `psychopy-whisper-0.0.1/LICENSE` & `psychopy-whisper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy-whisper-0.0.1/PKG-INFO` & `psychopy-whisper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-whisper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extension for transcription using OpenAI Whisper.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/psychopy/psychopy-whisper
 Project-URL: changelog, https://github.com/psychopy/psychopy-whisper/blob/main/CHANGELOG.txt
 Project-URL: documentation, https://pages.github.com/psychopy/psychopy-whisper
 Project-URL: repository, https://github.com/psychopy/psychopy-whisper
```

### Comparing `psychopy-whisper-0.0.1/README.md` & `psychopy-whisper-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `psychopy-whisper-0.0.1/psychopy_whisper/__init__.py` & `psychopy-whisper-0.0.2/psychopy_whisper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """Speech-to-text transcription using OpenAI Whisper.
 """
 
 __all__ = [
     "WhisperTranscriber",
     "recognizeWhisper"
 ]
-__version__ = '0.0.1'  # plugin version
+__version__ = '0.0.2'  # plugin version
 
 import os
 import json
 import psychopy.logging as logging
 from psychopy.preferences import prefs
 from psychopy.sound.audioclip import AudioClip
 from psychopy.sound.transcribe import TranscriptionResult, BaseTranscriber
```

### Comparing `psychopy-whisper-0.0.1/psychopy_whisper.egg-info/PKG-INFO` & `psychopy-whisper-0.0.2/psychopy_whisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-whisper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extension for transcription using OpenAI Whisper.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/psychopy/psychopy-whisper
 Project-URL: changelog, https://github.com/psychopy/psychopy-whisper/blob/main/CHANGELOG.txt
 Project-URL: documentation, https://pages.github.com/psychopy/psychopy-whisper
 Project-URL: repository, https://github.com/psychopy/psychopy-whisper
```

### Comparing `psychopy-whisper-0.0.1/pyproject.toml` & `psychopy-whisper-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psychopy-whisper"
-version = "0.0.1"
+version = "0.0.2"
 description = "Extension for transcription using OpenAI Whisper."
 readme = "README.md"
 requires-python = ">= 3.7"
 license = {text = "GNU General Public License v3 (GPLv3)"}
 authors = [
   { name = "Jon Peirce", email = "jon@opensceincetools.org" },
   { name = "Matthew Cutone", email = "mcutone@opensceincetools.org" },
@@ -27,14 +27,15 @@
 urls.homepage = "https://github.com/psychopy/psychopy-whisper"
 urls.changelog = "https://github.com/psychopy/psychopy-whisper/blob/main/CHANGELOG.txt"
 urls.documentation = "https://pages.github.com/psychopy/psychopy-whisper"
 urls.repository = "https://github.com/psychopy/psychopy-whisper"
 dependencies = [
   "faster-whisper",
   "librosa",
+  "typing-extensions",
 ]
 
 [tool.setuptools.packages.find]
 where = ["",]
 
 [project.entry-points."psychopy.sound.transcribe"]
 WhisperTranscriber = "psychopy_whisper:WhisperTranscriber"
```

