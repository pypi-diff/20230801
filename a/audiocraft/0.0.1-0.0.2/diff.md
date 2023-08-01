# Comparing `tmp/audiocraft-0.0.1.tar.gz` & `tmp/audiocraft-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiocraft-0.0.1.tar", last modified: Fri Jun  9 05:33:01 2023, max compression
+gzip compressed data, was "audiocraft-0.0.2.tar", last modified: Tue Aug  1 18:20:36 2023, max compression
```

## Comparing `audiocraft-0.0.1.tar` & `audiocraft-0.0.2.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.445553 audiocraft-0.0.1/
--rw-rw-r--   0 defossez   (501) staff       (20)      228 2023-06-08 16:14:27.000000 audiocraft-0.0.1/CHANGELOG.md
--rw-r--r--   0 defossez   (501) staff       (20)     3535 2023-06-08 18:47:37.000000 audiocraft-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 defossez   (501) staff       (20)     1377 2023-06-08 18:47:37.000000 audiocraft-0.0.1/CONTRIBUTING.md
--rw-rw-r--   0 defossez   (501) staff       (20)     1088 2023-06-08 16:14:27.000000 audiocraft-0.0.1/LICENSE
--rw-rw-r--   0 defossez   (501) staff       (20)    17529 2023-06-08 16:14:27.000000 audiocraft-0.0.1/LICENSE_weights
--rw-rw-r--   0 defossez   (501) staff       (20)      158 2023-06-08 16:14:27.000000 audiocraft-0.0.1/MANIFEST.in
--rw-r--r--   0 defossez   (501) staff       (20)     5970 2023-06-09 05:32:25.000000 audiocraft-0.0.1/MODEL_CARD.md
--rw-rw-r--   0 defossez   (501) staff       (20)      340 2023-06-08 16:14:27.000000 audiocraft-0.0.1/Makefile
--rw-r--r--   0 defossez   (501) staff       (20)     5992 2023-06-09 05:33:01.445794 audiocraft-0.0.1/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)     4696 2023-06-09 05:32:17.000000 audiocraft-0.0.1/README.md
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.352525 audiocraft-0.0.1/assets/
--rw-rw-r--   0 defossez   (501) staff       (20)   160496 2023-06-08 16:14:27.000000 audiocraft-0.0.1/assets/bach.mp3
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.355327 audiocraft-0.0.1/audiocraft/
--rw-rw-r--   0 defossez   (501) staff       (20)      273 2023-06-08 16:21:54.000000 audiocraft-0.0.1/audiocraft/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.366753 audiocraft-0.0.1/audiocraft/data/
--rw-rw-r--   0 defossez   (501) staff       (20)      249 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/data/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     8818 2023-06-08 19:47:47.000000 audiocraft-0.0.1/audiocraft/data/audio.py
--rw-rw-r--   0 defossez   (501) staff       (20)    21890 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/data/audio_dataset.py
--rw-rw-r--   0 defossez   (501) staff       (20)     7224 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/data/audio_utils.py
--rw-rw-r--   0 defossez   (501) staff       (20)     2122 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/data/zip.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.378973 audiocraft-0.0.1/audiocraft/models/
--rw-rw-r--   0 defossez   (501) staff       (20)      321 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/__init__.py
--rw-rw-r--   0 defossez   (501) staff       (20)     8591 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/builders.py
--rw-rw-r--   0 defossez   (501) staff       (20)    10268 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/encodec.py
--rw-rw-r--   0 defossez   (501) staff       (20)    26480 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/lm.py
--rw-rw-r--   0 defossez   (501) staff       (20)     2278 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/models/loaders.py
--rw-r--r--   0 defossez   (501) staff       (20)    13532 2023-06-08 20:16:11.000000 audiocraft-0.0.1/audiocraft/models/musicgen.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.397448 audiocraft-0.0.1/audiocraft/modules/
--rw-rw-r--   0 defossez   (501) staff       (20)      497 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/__init__.py
--rw-rw-r--   0 defossez   (501) staff       (20)     3270 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/activations.py
--rw-rw-r--   0 defossez   (501) staff       (20)    27613 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/codebooks_patterns.py
--rw-rw-r--   0 defossez   (501) staff       (20)    41366 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/conditioners.py
--rw-rw-r--   0 defossez   (501) staff       (20)    10506 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/conv.py
--rw-rw-r--   0 defossez   (501) staff       (20)      759 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/lstm.py
--rw-rw-r--   0 defossez   (501) staff       (20)     5436 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/rope.py
--rw-rw-r--   0 defossez   (501) staff       (20)    13868 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/seanet.py
--rw-rw-r--   0 defossez   (501) staff       (20)     4530 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/streaming.py
--rw-rw-r--   0 defossez   (501) staff       (20)    35079 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/modules/transformer.py
--rw-rw-r--   0 defossez   (501) staff       (20)        0 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/py.typed
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.403631 audiocraft-0.0.1/audiocraft/quantization/
--rw-rw-r--   0 defossez   (501) staff       (20)      319 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/quantization/__init__.py
--rw-rw-r--   0 defossez   (501) staff       (20)     3386 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/quantization/base.py
--rw-rw-r--   0 defossez   (501) staff       (20)    14354 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/quantization/core_vq.py
--rw-rw-r--   0 defossez   (501) staff       (20)     4657 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/quantization/vq.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.418171 audiocraft-0.0.1/audiocraft/utils/
--rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/utils/__init__.py
--rw-rw-r--   0 defossez   (501) staff       (20)     1377 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/utils/autocast.py
--rw-rw-r--   0 defossez   (501) staff       (20)     1907 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/utils/export.py
--rw-r--r--   0 defossez   (501) staff       (20)      885 2023-06-08 18:47:37.000000 audiocraft-0.0.1/audiocraft/utils/notebook.py
--rw-rw-r--   0 defossez   (501) staff       (20)     8571 2023-06-08 16:14:27.000000 audiocraft-0.0.1/audiocraft/utils/utils.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.359730 audiocraft-0.0.1/audiocraft.egg-info/
--rw-r--r--   0 defossez   (501) staff       (20)     5992 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)     1752 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/SOURCES.txt
--rw-r--r--   0 defossez   (501) staff       (20)        1 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/dependency_links.txt
--rw-r--r--   0 defossez   (501) staff       (20)      219 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/requires.txt
--rw-r--r--   0 defossez   (501) staff       (20)       17 2023-06-09 05:33:01.000000 audiocraft-0.0.1/audiocraft.egg-info/top_level.txt
--rw-rw-r--   0 defossez   (501) staff       (20)      134 2023-06-08 16:14:27.000000 audiocraft-0.0.1/mypy.ini
--rw-rw-r--   0 defossez   (501) staff       (20)      254 2023-06-08 16:14:27.000000 audiocraft-0.0.1/requirements.txt
--rw-rw-r--   0 defossez   (501) staff       (20)      100 2023-06-09 05:33:01.447012 audiocraft-0.0.1/setup.cfg
--rw-rw-r--   0 defossez   (501) staff       (20)     1778 2023-06-08 16:14:27.000000 audiocraft-0.0.1/setup.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.420122 audiocraft-0.0.1/tests/
--rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.424188 audiocraft-0.0.1/tests/common_utils/
--rw-rw-r--   0 defossez   (501) staff       (20)      323 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/common_utils/__init__.py
--rw-rw-r--   0 defossez   (501) staff       (20)     1744 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/common_utils/temp_utils.py
--rw-rw-r--   0 defossez   (501) staff       (20)      872 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/common_utils/wav_utils.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.430116 audiocraft-0.0.1/tests/data/
--rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/data/__init__.py
--rw-rw-r--   0 defossez   (501) staff       (20)    10518 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/data/test_audio.py
--rw-rw-r--   0 defossez   (501) staff       (20)    15055 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/data/test_audio_dataset.py
--rw-rw-r--   0 defossez   (501) staff       (20)     3738 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/data/test_audio_utils.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.443528 audiocraft-0.0.1/tests/modules/
--rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/__init__.py
--rw-rw-r--   0 defossez   (501) staff       (20)    10986 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_codebooks_patterns.py
--rw-rw-r--   0 defossez   (501) staff       (20)     7383 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_conv.py
--rw-rw-r--   0 defossez   (501) staff       (20)      781 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_lstm.py
--rw-rw-r--   0 defossez   (501) staff       (20)     4719 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_rope.py
--rw-rw-r--   0 defossez   (501) staff       (20)     4874 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_seanet.py
--rw-rw-r--   0 defossez   (501) staff       (20)     8788 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/modules/test_transformer.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-06-09 05:33:01.444718 audiocraft-0.0.1/tests/utils/
--rw-rw-r--   0 defossez   (501) staff       (20)      198 2023-06-08 16:14:27.000000 audiocraft-0.0.1/tests/utils/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.428130 audiocraft-0.0.2/
+-rw-r--r--   0 defossez   (501) staff       (20)      741 2023-08-01 18:17:09.000000 audiocraft-0.0.2/CHANGELOG.md
+-rw-r--r--   0 defossez   (501) staff       (20)     3535 2023-07-03 08:49:34.000000 audiocraft-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 defossez   (501) staff       (20)     1377 2023-07-03 08:49:34.000000 audiocraft-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 defossez   (501) staff       (20)     1088 2023-07-03 08:49:34.000000 audiocraft-0.0.2/LICENSE
+-rw-r--r--   0 defossez   (501) staff       (20)    17529 2023-07-03 08:49:34.000000 audiocraft-0.0.2/LICENSE_weights
+-rw-r--r--   0 defossez   (501) staff       (20)      158 2023-07-03 08:49:34.000000 audiocraft-0.0.2/MANIFEST.in
+-rw-r--r--   0 defossez   (501) staff       (20)     5973 2023-07-03 08:49:34.000000 audiocraft-0.0.2/MODEL_CARD.md
+-rw-r--r--   0 defossez   (501) staff       (20)      340 2023-07-03 08:49:34.000000 audiocraft-0.0.2/Makefile
+-rw-r--r--   0 defossez   (501) staff       (20)    10021 2023-08-01 18:20:36.428763 audiocraft-0.0.2/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     8069 2023-08-01 18:16:30.000000 audiocraft-0.0.2/README.md
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.223730 audiocraft-0.0.2/assets/
+-rw-r--r--   0 defossez   (501) staff       (20)   160496 2023-07-03 08:49:34.000000 audiocraft-0.0.2/assets/bach.mp3
+-rw-r--r--   0 defossez   (501) staff       (20)   161280 2023-07-03 08:49:34.000000 audiocraft-0.0.2/assets/bolero_ravel.mp3
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.227562 audiocraft-0.0.2/audiocraft/
+-rw-r--r--   0 defossez   (501) staff       (20)      273 2023-08-01 18:16:50.000000 audiocraft-0.0.2/audiocraft/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.239075 audiocraft-0.0.2/audiocraft/data/
+-rw-r--r--   0 defossez   (501) staff       (20)      249 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/data/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8990 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/data/audio.py
+-rw-r--r--   0 defossez   (501) staff       (20)    21890 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/data/audio_dataset.py
+-rw-r--r--   0 defossez   (501) staff       (20)     7540 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/data/audio_utils.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2122 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/data/zip.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.250158 audiocraft-0.0.2/audiocraft/models/
+-rw-r--r--   0 defossez   (501) staff       (20)      321 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/models/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8591 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/models/builders.py
+-rw-r--r--   0 defossez   (501) staff       (20)    10268 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/models/encodec.py
+-rw-r--r--   0 defossez   (501) staff       (20)    26600 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/models/lm.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3432 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/models/loaders.py
+-rw-r--r--   0 defossez   (501) staff       (20)    17779 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/models/musicgen.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.334764 audiocraft-0.0.2/audiocraft/modules/
+-rw-r--r--   0 defossez   (501) staff       (20)      497 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3270 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/activations.py
+-rw-r--r--   0 defossez   (501) staff       (20)    27613 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/codebooks_patterns.py
+-rw-r--r--   0 defossez   (501) staff       (20)    41550 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/conditioners.py
+-rw-r--r--   0 defossez   (501) staff       (20)    10506 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/conv.py
+-rw-r--r--   0 defossez   (501) staff       (20)      759 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/lstm.py
+-rw-r--r--   0 defossez   (501) staff       (20)     5436 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/rope.py
+-rw-r--r--   0 defossez   (501) staff       (20)    13868 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/seanet.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4530 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/streaming.py
+-rw-r--r--   0 defossez   (501) staff       (20)    36832 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/modules/transformer.py
+-rw-r--r--   0 defossez   (501) staff       (20)        0 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/py.typed
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.341954 audiocraft-0.0.2/audiocraft/quantization/
+-rw-r--r--   0 defossez   (501) staff       (20)      319 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/quantization/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3386 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/quantization/base.py
+-rw-r--r--   0 defossez   (501) staff       (20)    14354 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/quantization/core_vq.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4657 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/quantization/vq.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.374529 audiocraft-0.0.2/audiocraft/utils/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/utils/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1377 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/utils/autocast.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1907 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/utils/export.py
+-rw-r--r--   0 defossez   (501) staff       (20)      885 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/utils/notebook.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8570 2023-07-03 08:49:34.000000 audiocraft-0.0.2/audiocraft/utils/utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.233481 audiocraft-0.0.2/audiocraft.egg-info/
+-rw-r--r--   0 defossez   (501) staff       (20)    10021 2023-08-01 18:20:36.000000 audiocraft-0.0.2/audiocraft.egg-info/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     1776 2023-08-01 18:20:36.000000 audiocraft-0.0.2/audiocraft.egg-info/SOURCES.txt
+-rw-r--r--   0 defossez   (501) staff       (20)        1 2023-08-01 18:20:36.000000 audiocraft-0.0.2/audiocraft.egg-info/dependency_links.txt
+-rw-r--r--   0 defossez   (501) staff       (20)      242 2023-08-01 18:20:36.000000 audiocraft-0.0.2/audiocraft.egg-info/requires.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       17 2023-08-01 18:20:36.000000 audiocraft-0.0.2/audiocraft.egg-info/top_level.txt
+-rw-r--r--   0 defossez   (501) staff       (20)      150 2023-07-03 08:49:34.000000 audiocraft-0.0.2/mypy.ini
+-rw-r--r--   0 defossez   (501) staff       (20)      277 2023-07-03 08:49:34.000000 audiocraft-0.0.2/requirements.txt
+-rw-r--r--   0 defossez   (501) staff       (20)      100 2023-08-01 18:20:36.430435 audiocraft-0.0.2/setup.cfg
+-rw-r--r--   0 defossez   (501) staff       (20)     1802 2023-08-01 18:20:11.000000 audiocraft-0.0.2/setup.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.376293 audiocraft-0.0.2/tests/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.383274 audiocraft-0.0.2/tests/common_utils/
+-rw-r--r--   0 defossez   (501) staff       (20)      323 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/common_utils/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1744 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/common_utils/temp_utils.py
+-rw-r--r--   0 defossez   (501) staff       (20)      872 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/common_utils/wav_utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.393092 audiocraft-0.0.2/tests/data/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/data/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)    10518 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/data/test_audio.py
+-rw-r--r--   0 defossez   (501) staff       (20)    15055 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/data/test_audio_dataset.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3738 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/data/test_audio_utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.425676 audiocraft-0.0.2/tests/modules/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/modules/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)    10986 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/modules/test_codebooks_patterns.py
+-rw-r--r--   0 defossez   (501) staff       (20)     7383 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/modules/test_conv.py
+-rw-r--r--   0 defossez   (501) staff       (20)      781 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/modules/test_lstm.py
+-rw-r--r--   0 defossez   (501) staff       (20)     5136 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/modules/test_rope.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4874 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/modules/test_seanet.py
+-rw-r--r--   0 defossez   (501) staff       (20)     9193 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/modules/test_transformer.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-08-01 18:20:36.427136 audiocraft-0.0.2/tests/utils/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-0.0.2/tests/utils/__init__.py
```

### Comparing `audiocraft-0.0.1/CODE_OF_CONDUCT.md` & `audiocraft-0.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/CONTRIBUTING.md` & `audiocraft-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/LICENSE` & `audiocraft-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/LICENSE_weights` & `audiocraft-0.0.2/LICENSE_weights`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/MODEL_CARD.md` & `audiocraft-0.0.2/MODEL_CARD.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,25 +48,25 @@
 
 ## Evaluation datasets
 
 The model was evaluated on the [MusicCaps benchmark](https://www.kaggle.com/datasets/googleai/musiccaps) and on an in-domain held-out evaluation set, with no artist overlap with the training set.
 
 ## Training datasets
 
-The model was trained using the following sources: the [Meta Music Initiative Sound Collection](https://www.fb.com/sound),  [Shutterstock music collection](https://www.shutterstock.com/music) and the [Pond5 music collection](https://www.pond5.com/). See the paper for more details about the training set and corresponding preprocessing.
+The model was trained on licensed data using the following sources: the [Meta Music Initiative Sound Collection](https://www.fb.com/sound),  [Shutterstock music collection](https://www.shutterstock.com/music) and the [Pond5 music collection](https://www.pond5.com/). See the paper for more details about the training set and corresponding preprocessing.
 
 ## Quantitative analysis
 
 More information can be found in the paper [Simple and Controllable Music Generation][arxiv], in the Experimental Setup section.
 
 ## Limitations and biases
 
 **Data:** The data sources used to train the model are created by music professionals and covered by legal agreements with the right holders. The model is trained on 20K hours of data, we believe that scaling the model on larger datasets can further improve the performance of the model.
 
-**Mitigations:** All vocals have been removed from the data source using a state-of-the-art music source separation method, namely using the open source [Hybrid Transformer for Music Source Separation](https://github.com/facebookresearch/demucs) (HT-Demucs). The model is therefore not able to produce vocals.
+**Mitigations:** Vocals have been removed from the data source using corresponding tags, and then using using a state-of-the-art music source separation method, namely using the open source [Hybrid Transformer for Music Source Separation](https://github.com/facebookresearch/demucs) (HT-Demucs).
 
 **Limitations:**
 
 - The model is not able to generate realistic vocals.
 - The model has been trained with English descriptions and will not perform as well in other languages.
 - The model does not perform equally well for all music styles and cultures.
 - The model sometimes generates end of songs, collapsing to silence.
```

### Comparing `audiocraft-0.0.1/assets/bach.mp3` & `audiocraft-0.0.2/assets/bach.mp3`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/data/audio.py` & `audiocraft-0.0.2/audiocraft/data/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 
 
 def audio_write(stem_name: tp.Union[str, Path],
                 wav: torch.Tensor, sample_rate: int,
                 format: str = 'wav', mp3_rate: int = 320, normalize: bool = True,
                 strategy: str = 'peak', peak_clip_headroom_db: float = 1,
                 rms_headroom_db: float = 18, loudness_headroom_db: float = 14,
+                loudness_compressor: bool = False,
                 log_clipping: bool = True, make_parent_dir: bool = True,
                 add_suffix: bool = True) -> Path:
     """Convenience function for saving audio to disk. Returns the filename the audio was written to.
 
     Args:
         stem_name (str or Path): Filename without extension which will be added automatically.
         format (str): Either "wav" or "mp3".
@@ -169,15 +170,16 @@
         strategy (str): Can be either 'clip', 'peak', or 'rms'. Default is 'peak',
             i.e. audio is normalized by its largest value. RMS normalizes by root-mean-square
             with extra headroom to avoid clipping. 'clip' just clips.
         peak_clip_headroom_db (float): Headroom in dB when doing 'peak' or 'clip' strategy.
         rms_headroom_db (float): Headroom in dB when doing 'rms' strategy. This must be much larger
             than the `peak_clip` one to avoid further clipping.
         loudness_headroom_db (float): Target loudness for loudness normalization.
-        log_clipping (bool): If True, basic logging on stderr when clipping still
+        loudness_compressor (bool): Uses tanh for soft clipping when strategy is 'loudness'.
+         when strategy is 'loudness'log_clipping (bool): If True, basic logging on stderr when clipping still
             occurs despite strategy (only for 'rms').
         make_parent_dir (bool): Make parent directory if it doesn't exist.
     Returns:
         Path: Path of the saved audio.
     """
     assert wav.dtype.is_floating_point, "wav is not floating point"
     if wav.dim() == 1:
```

### Comparing `audiocraft-0.0.1/audiocraft/data/audio_dataset.py` & `audiocraft-0.0.2/audiocraft/data/audio_dataset.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/data/audio_utils.py` & `audiocraft-0.0.2/audiocraft/data/audio_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,36 +50,39 @@
     """Convert audio to new sample rate and number of audio channels.
     """
     wav = julius.resample_frac(wav, int(from_rate), int(to_rate))
     wav = convert_audio_channels(wav, to_channels)
     return wav
 
 
-def normalize_loudness(wav: torch.Tensor, sample_rate: int, loudness_headroom_db: float = 12,
-                       energy_floor: float = 2e-3):
+def normalize_loudness(wav: torch.Tensor, sample_rate: int, loudness_headroom_db: float = 14,
+                       loudness_compressor: bool = False, energy_floor: float = 2e-3):
     """Normalize an input signal to a user loudness in dB LKFS.
     Audio loudness is defined according to the ITU-R BS.1770-4 recommendation.
 
     Args:
         wav (torch.Tensor): Input multichannel audio data.
         sample_rate (int): Sample rate.
         loudness_headroom_db (float): Target loudness of the output in dB LUFS.
+        loudness_compressor (bool): Uses tanh for soft clipping.
         energy_floor (float): anything below that RMS level will not be rescaled.
     Returns:
         output (torch.Tensor): Loudness normalized output data.
     """
     energy = wav.pow(2).mean().sqrt().item()
     if energy < energy_floor:
         return wav
     transform = torchaudio.transforms.Loudness(sample_rate)
     input_loudness_db = transform(wav).item()
     # calculate the gain needed to scale to the desired loudness level
     delta_loudness = -loudness_headroom_db - input_loudness_db
     gain = 10.0 ** (delta_loudness / 20.0)
     output = gain * wav
+    if loudness_compressor:
+        output = torch.tanh(output)
     assert output.isfinite().all(), (input_loudness_db, wav.pow(2).mean().sqrt())
     return output
 
 
 def _clip_wav(wav: torch.Tensor, log_clipping: bool = False, stem_name: tp.Optional[str] = None) -> None:
     """Utility function to clip the audio with logging if specified."""
     max_scale = wav.abs().max()
@@ -89,15 +92,16 @@
               clamp_prob, "maximum scale: ", max_scale.item(), file=sys.stderr)
     wav.clamp_(-1, 1)
 
 
 def normalize_audio(wav: torch.Tensor, normalize: bool = True,
                     strategy: str = 'peak', peak_clip_headroom_db: float = 1,
                     rms_headroom_db: float = 18, loudness_headroom_db: float = 14,
-                    log_clipping: bool = False, sample_rate: tp.Optional[int] = None,
+                    loudness_compressor: bool = False, log_clipping: bool = False,
+                    sample_rate: tp.Optional[int] = None,
                     stem_name: tp.Optional[str] = None) -> torch.Tensor:
     """Normalize the audio according to the prescribed strategy (see after).
 
     Args:
         wav (torch.Tensor): Audio data.
         normalize (bool): if `True` (default), normalizes according to the prescribed
             strategy (see after). If `False`, the strategy is only used in case clipping
@@ -105,14 +109,15 @@
         strategy (str): Can be either 'clip', 'peak', or 'rms'. Default is 'peak',
             i.e. audio is normalized by its largest value. RMS normalizes by root-mean-square
             with extra headroom to avoid clipping. 'clip' just clips.
         peak_clip_headroom_db (float): Headroom in dB when doing 'peak' or 'clip' strategy.
         rms_headroom_db (float): Headroom in dB when doing 'rms' strategy. This must be much larger
             than the `peak_clip` one to avoid further clipping.
         loudness_headroom_db (float): Target loudness for loudness normalization.
+        loudness_compressor (bool): If True, uses tanh based soft clipping.
         log_clipping (bool): If True, basic logging on stderr when clipping still
             occurs despite strategy (only for 'rms').
         sample_rate (int): Sample rate for the audio data (required for loudness).
         stem_name (Optional[str]): Stem name for clipping logging.
     Returns:
         torch.Tensor: Normalized audio.
     """
@@ -128,15 +133,15 @@
         mono = wav.mean(dim=0)
         rescaling = scale_rms / mono.pow(2).mean().sqrt()
         if normalize or rescaling < 1:
             wav = wav * rescaling
         _clip_wav(wav, log_clipping=log_clipping, stem_name=stem_name)
     elif strategy == 'loudness':
         assert sample_rate is not None, "Loudness normalization requires sample rate."
-        wav = normalize_loudness(wav, sample_rate, loudness_headroom_db)
+        wav = normalize_loudness(wav, sample_rate, loudness_headroom_db, loudness_compressor)
         _clip_wav(wav, log_clipping=log_clipping, stem_name=stem_name)
     else:
         assert wav.abs().max() < 1
         assert strategy == '' or strategy == 'none', f"Unexpected strategy: '{strategy}'"
     return wav
```

### Comparing `audiocraft-0.0.1/audiocraft/data/zip.py` & `audiocraft-0.0.2/audiocraft/data/zip.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/models/builders.py` & `audiocraft-0.0.2/audiocraft/models/builders.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/models/encodec.py` & `audiocraft-0.0.2/audiocraft/models/encodec.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/models/lm.py` & `audiocraft-0.0.2/audiocraft/models/lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,15 +359,16 @@
                 logits = uncond_logits + (cond_logits - uncond_logits) * cfg_coef
             else:
                 logits = all_logits
 
         logits = logits.permute(0, 1, 3, 2)  # [B, K, card, T]
         logits = logits[..., -1]  # [B x K x card]
 
-        if use_sampling:
+        # Apply softmax for sampling if temp > 0. Else, do greedy sampling to avoid zero division error.
+        if use_sampling and temp > 0.0:
             probs = torch.softmax(logits / temp, dim=-1)
             if top_p > 0.0:
                 next_token = utils.sample_top_p(probs, p=top_p)
             elif top_k > 0:
                 next_token = utils.sample_top_k(probs, k=top_k)
             else:
                 next_token = utils.multinomial(probs, num_samples=1)
```

### Comparing `audiocraft-0.0.1/audiocraft/models/musicgen.py` & `audiocraft-0.0.2/audiocraft/models/musicgen.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import typing as tp
 
 import torch
 
 from .encodec import CompressionModel
 from .lm import LMModel
 from .builders import get_debug_compression_model, get_debug_lm_model
-from .loaders import load_compression_model, load_lm_model
+from .loaders import load_compression_model, load_lm_model, HF_MODEL_CHECKPOINTS_MAP
 from ..data.audio_utils import convert_audio
 from ..modules.conditioners import ConditioningAttributes, WavCondition
 from ..utils.autocast import TorchAutocast
 
 
 MelodyList = tp.List[tp.Optional[torch.Tensor]]
 MelodyType = tp.Union[torch.Tensor, MelodyList]
@@ -32,21 +32,24 @@
 
     Args:
         name (str): name of the model.
         compression_model (CompressionModel): Compression model
             used to map audio to invertible discrete representations.
         lm (LMModel): Language model over discrete representations.
     """
-    def __init__(self, name: str, compression_model: CompressionModel, lm: LMModel):
+    def __init__(self, name: str, compression_model: CompressionModel, lm: LMModel,
+                 max_duration: float = 30):
         self.name = name
         self.compression_model = compression_model
         self.lm = lm
+        self.max_duration = max_duration
         self.device = next(iter(lm.parameters())).device
         self.generation_params: dict = {}
         self.set_generation_params(duration=15)  # 15 seconds by default
+        self._progress_callback: tp.Optional[tp.Callable[[int, int], None]] = None
         if self.device.type == 'cpu':
             self.autocast = TorchAutocast(enabled=False)
         else:
             self.autocast = TorchAutocast(
                 enabled=True, device_type=self.device.type, dtype=torch.float16)
 
     @property
@@ -61,73 +64,85 @@
 
     @property
     def audio_channels(self) -> int:
         """Audio channels of the generated audio."""
         return self.compression_model.channels
 
     @staticmethod
-    def get_pretrained(name: str = 'melody', device='cuda'):
+    def get_pretrained(name: str = 'melody', device=None):
         """Return pretrained model, we provide four models:
-        - small (300M), text to music,
-        - medium (1.5B), text to music,
-        - melody (1.5B) text to music and text+melody to music,
-        - large (3.3B), text to music.
+        - small (300M), text to music, # see: https://huggingface.co/facebook/musicgen-small
+        - medium (1.5B), text to music, # see: https://huggingface.co/facebook/musicgen-medium
+        - melody (1.5B) text to music and text+melody to music, # see: https://huggingface.co/facebook/musicgen-melody
+        - large (3.3B), text to music, # see: https://huggingface.co/facebook/musicgen-large
         """
 
+        if device is None:
+            if torch.cuda.device_count():
+                device = 'cuda'
+            else:
+                device = 'cpu'
+
         if name == 'debug':
             # used only for unit tests
             compression_model = get_debug_compression_model(device)
             lm = get_debug_lm_model(device)
             return MusicGen(name, compression_model, lm)
 
-        if 'MUSICGEN_ROOT' in os.environ:
-            ROOT = os.environ['MUSICGEN_ROOT']
-            if not ROOT.endswith('/'):
-                ROOT += '/'
-        else:
-            ROOT = 'https://dl.fbaipublicfiles.com/audiocraft/musicgen/v0/'
-        compression_model = load_compression_model(ROOT + 'b0dbef54-37d256b525.th', device=device)
-        names = {
-            'small': 'ba7a97ba-830fe5771e',
-            'medium': 'aa73ae27-fbc9f401db',
-            'large': '9b6e835c-1f0cf17b5e',
-            'melody': 'f79af192-61305ffc49',
-        }
-        sig = names[name]
-        lm = load_lm_model(ROOT + f'{sig}.th', device=device)
+        if name not in HF_MODEL_CHECKPOINTS_MAP:
+            if not os.path.isfile(name) and not os.path.isdir(name):
+                raise ValueError(
+                    f"{name} is not a valid checkpoint name. "
+                    f"Choose one of {', '.join(HF_MODEL_CHECKPOINTS_MAP.keys())}"
+                )
+
+        cache_dir = os.environ.get('MUSICGEN_ROOT', None)
+        compression_model = load_compression_model(name, device=device, cache_dir=cache_dir)
+        lm = load_lm_model(name, device=device, cache_dir=cache_dir)
+        if name == 'melody':
+            lm.condition_provider.conditioners['self_wav'].match_len_on_eval = True
+
         return MusicGen(name, compression_model, lm)
 
     def set_generation_params(self, use_sampling: bool = True, top_k: int = 250,
                               top_p: float = 0.0, temperature: float = 1.0,
                               duration: float = 30.0, cfg_coef: float = 3.0,
-                              two_step_cfg: bool = False):
+                              two_step_cfg: bool = False, extend_stride: float = 18):
         """Set the generation parameters for MusicGen.
 
         Args:
             use_sampling (bool, optional): Use sampling if True, else do argmax decoding. Defaults to True.
             top_k (int, optional): top_k used for sampling. Defaults to 250.
             top_p (float, optional): top_p used for sampling, when set to 0 top_k is used. Defaults to 0.0.
             temperature (float, optional): Softmax temperature parameter. Defaults to 1.0.
             duration (float, optional): Duration of the generated waveform. Defaults to 30.0.
             cfg_coef (float, optional): Coefficient used for classifier free guidance. Defaults to 3.0.
             two_step_cfg (bool, optional): If True, performs 2 forward for Classifier Free Guidance,
                 instead of batching together the two. This has some impact on how things
                 are padded but seems to have little impact in practice.
+            extend_stride: when doing extended generation (i.e. more than 30 seconds), by how much
+                should we extend the audio each time. Larger values will mean less context is
+                preserved, and shorter value will require extra computations.
         """
-        assert duration <= 30, "The MusicGen cannot generate more than 30 seconds"
+        assert extend_stride < self.max_duration, "Cannot stride by more than max generation duration."
+        self.extend_stride = extend_stride
+        self.duration = duration
         self.generation_params = {
-            'max_gen_len': int(duration * self.frame_rate),
             'use_sampling': use_sampling,
             'temp': temperature,
             'top_k': top_k,
             'top_p': top_p,
             'cfg_coef': cfg_coef,
             'two_step_cfg': two_step_cfg,
         }
 
+    def set_custom_progress_callback(self, progress_callback: tp.Optional[tp.Callable[[int, int], None]] = None):
+        """Override the default progress callback."""
+        self._progress_callback = progress_callback
+
     def generate_unconditional(self, num_samples: int, progress: bool = False) -> torch.Tensor:
         """Generate samples in an unconditional manner.
 
         Args:
             num_samples (int): Number of samples to be generated.
             progress (bool, optional): Flag to display progress of the generation process. Defaults to False.
         """
@@ -262,27 +277,86 @@
         Args:
             attributes (tp.List[ConditioningAttributes]): Conditions used for generation (text/melody).
             prompt_tokens (tp.Optional[torch.Tensor]): Audio prompt used for continuation.
             progress (bool, optional): Flag to display progress of the generation process. Defaults to False.
         Returns:
             torch.Tensor: Generated audio, of shape [B, C, T], T is defined by the generation params.
         """
+        total_gen_len = int(self.duration * self.frame_rate)
+        max_prompt_len = int(min(self.duration, self.max_duration) * self.frame_rate)
+        current_gen_offset: int = 0
+
         def _progress_callback(generated_tokens: int, tokens_to_generate: int):
-            print(f'{generated_tokens: 6d} / {tokens_to_generate: 6d}', end='\r')
+            generated_tokens += current_gen_offset
+            if self._progress_callback is not None:
+                # Note that total_gen_len might be quite wrong depending on the
+                # codebook pattern used, but with delay it is almost accurate.
+                self._progress_callback(generated_tokens, total_gen_len)
+            else:
+                print(f'{generated_tokens: 6d} / {total_gen_len: 6d}', end='\r')
 
         if prompt_tokens is not None:
-            assert self.generation_params['max_gen_len'] > prompt_tokens.shape[-1], \
+            assert max_prompt_len >= prompt_tokens.shape[-1], \
                 "Prompt is longer than audio to generate"
 
         callback = None
         if progress:
             callback = _progress_callback
 
-        # generate by sampling from LM
-        with self.autocast:
-            gen_tokens = self.lm.generate(prompt_tokens, attributes, callback=callback, **self.generation_params)
+        if self.duration <= self.max_duration:
+            # generate by sampling from LM, simple case.
+            with self.autocast:
+                gen_tokens = self.lm.generate(
+                    prompt_tokens, attributes,
+                    callback=callback, max_gen_len=total_gen_len, **self.generation_params)
+
+        else:
+            # now this gets a bit messier, we need to handle prompts,
+            # melody conditioning etc.
+            ref_wavs = [attr.wav['self_wav'] for attr in attributes]
+            all_tokens = []
+            if prompt_tokens is None:
+                prompt_length = 0
+            else:
+                all_tokens.append(prompt_tokens)
+                prompt_length = prompt_tokens.shape[-1]
+
+            stride_tokens = int(self.frame_rate * self.extend_stride)
+
+            while current_gen_offset + prompt_length < total_gen_len:
+                time_offset = current_gen_offset / self.frame_rate
+                chunk_duration = min(self.duration - time_offset, self.max_duration)
+                max_gen_len = int(chunk_duration * self.frame_rate)
+                for attr, ref_wav in zip(attributes, ref_wavs):
+                    wav_length = ref_wav.length.item()
+                    if wav_length == 0:
+                        continue
+                    # We will extend the wav periodically if it not long enough.
+                    # we have to do it here rather than in conditioners.py as otherwise
+                    # we wouldn't have the full wav.
+                    initial_position = int(time_offset * self.sample_rate)
+                    wav_target_length = int(self.max_duration * self.sample_rate)
+                    print(initial_position / self.sample_rate, wav_target_length / self.sample_rate)
+                    positions = torch.arange(initial_position,
+                                             initial_position + wav_target_length, device=self.device)
+                    attr.wav['self_wav'] = WavCondition(
+                        ref_wav[0][:, positions % wav_length],
+                        torch.full_like(ref_wav[1], wav_target_length))
+                with self.autocast:
+                    gen_tokens = self.lm.generate(
+                        prompt_tokens, attributes,
+                        callback=callback, max_gen_len=max_gen_len, **self.generation_params)
+                if prompt_tokens is None:
+                    all_tokens.append(gen_tokens)
+                else:
+                    all_tokens.append(gen_tokens[:, :, prompt_tokens.shape[-1]:])
+                prompt_tokens = gen_tokens[:, :, stride_tokens:]
+                prompt_length = prompt_tokens.shape[-1]
+                current_gen_offset += stride_tokens
+
+            gen_tokens = torch.cat(all_tokens, dim=-1)
 
         # generate audio
         assert gen_tokens.dim() == 3
         with torch.no_grad():
             gen_audio = self.compression_model.decode(gen_tokens, None)
         return gen_audio
```

### Comparing `audiocraft-0.0.1/audiocraft/modules/activations.py` & `audiocraft-0.0.2/audiocraft/modules/activations.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/modules/codebooks_patterns.py` & `audiocraft-0.0.2/audiocraft/modules/codebooks_patterns.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/modules/conditioners.py` & `audiocraft-0.0.2/audiocraft/modules/conditioners.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass, field
 from itertools import chain
 import logging
+import math
 import random
 import re
 import typing as tp
 import warnings
 
 from einops import rearrange
 from num2words import num2words
@@ -480,15 +481,15 @@
             conditions during eval (for cases where we don't want to leak test conditions like MusicCaps).
             Defaults to None.
         n_eval_wavs (int, optional): Limits the number of waveforms used for conditioning. Defaults to 0.
         device (tp.Union[torch.device, str], optional): Device for the conditioner.
         **kwargs: Additional parameters for the chroma extractor.
     """
     def __init__(self, output_dim: int, sample_rate: int, n_chroma: int, radix2_exp: int,
-                 duration: float, match_len_on_eval: bool = False, eval_wavs: tp.Optional[str] = None,
+                 duration: float, match_len_on_eval: bool = True, eval_wavs: tp.Optional[str] = None,
                  n_eval_wavs: int = 0, device: tp.Union[torch.device, str] = "cpu", **kwargs):
         from demucs import pretrained
         super().__init__(dim=n_chroma, output_dim=output_dim, device=device)
         self.autocast = TorchAutocast(enabled=device != "cpu", device_type=self.device, dtype=torch.float32)
         self.sample_rate = sample_rate
         self.match_len_on_eval = match_len_on_eval
         self.duration = duration
@@ -531,15 +532,18 @@
 
         if self.match_len_on_eval:
             b, t, c = chroma.shape
             if t > self.chroma_len:
                 chroma = chroma[:, :self.chroma_len]
                 logger.debug(f'chroma was truncated! ({t} -> {chroma.shape[1]})')
             elif t < self.chroma_len:
-                chroma = F.pad(chroma, (0, 0, 0, self.chroma_len - t))
+                # chroma = F.pad(chroma, (0, 0, 0, self.chroma_len - t))
+                n_repeat = int(math.ceil(self.chroma_len / t))
+                chroma = chroma.repeat(1, n_repeat, 1)
+                chroma = chroma[:, :self.chroma_len]
                 logger.debug(f'chroma was zero-padded! ({t} -> {chroma.shape[1]})')
         return chroma
 
 
 class ChromaExtractor(nn.Module):
     """Chroma extraction class, handles chroma extraction and quantization.
```

### Comparing `audiocraft-0.0.1/audiocraft/modules/conv.py` & `audiocraft-0.0.2/audiocraft/modules/conv.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/modules/lstm.py` & `audiocraft-0.0.2/audiocraft/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/modules/rope.py` & `audiocraft-0.0.2/audiocraft/modules/rope.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/modules/seanet.py` & `audiocraft-0.0.2/audiocraft/modules/seanet.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/modules/streaming.py` & `audiocraft-0.0.2/audiocraft/modules/streaming.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/modules/transformer.py` & `audiocraft-0.0.2/audiocraft/modules/transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,30 @@
 from torch.nn import functional as F
 from torch.utils.checkpoint import checkpoint as torch_checkpoint
 from xformers import ops
 
 from .rope import RotaryEmbedding
 from .streaming import StreamingModule
 
+_efficient_attention_backend: str = 'torch'
+
+
+def set_efficient_attention_backend(backend: str = 'torch'):
+    # Using torch by default, it seems a bit faster on older P100 GPUs (~20% faster).
+    global _efficient_attention_backend
+    assert _efficient_attention_backend in ['xformers', 'torch']
+    _efficient_attention_backend = backend
+
+
+def _get_attention_time_dimension() -> int:
+    if _efficient_attention_backend == 'torch':
+        return 2
+    else:
+        return 1
+
 
 def _is_profiled() -> bool:
     # Return true if we are currently running with a xformers profiler activated.
     try:
         from xformers.profiler import profiler
     except ImportError:
         return False
@@ -71,22 +87,30 @@
     max_period_tensor = torch.full([], max_period, device=positions.device, dtype=dtype)  # avoid sync point
     phase = positions / (max_period_tensor ** (adim / (half_dim - 1)))
     return torch.cat([torch.cos(phase), torch.sin(phase)], dim=-1)
 
 
 def expand_repeated_kv(x: torch.Tensor, n_rep: int) -> torch.Tensor:
     """torch.repeat_interleave(x, dim=2, repeats=n_rep) from xlformers"""
-    bs, slen, n_kv_heads, head_dim = x.shape
     if n_rep == 1:
         return x
-    return (
-        x[:, :, :, None, :]
-        .expand(bs, slen, n_kv_heads, n_rep, head_dim)
-        .reshape(bs, slen, n_kv_heads * n_rep, head_dim)
-    )
+    if _efficient_attention_backend == 'torch':
+        bs, n_kv_heads, slen, head_dim = x.shape
+        return (
+            x[:, :, None, :, :]
+            .expand(bs, n_kv_heads, n_rep, slen, head_dim)
+            .reshape(bs, n_kv_heads * n_rep, slen, head_dim)
+        )
+    else:
+        bs, slen, n_kv_heads, head_dim = x.shape
+        return (
+            x[:, :, :, None, :]
+            .expand(bs, slen, n_kv_heads, n_rep, head_dim)
+            .reshape(bs, slen, n_kv_heads * n_rep, head_dim)
+        )
 
 
 class LayerScale(nn.Module):
     """Layer scale from [Touvron et al 2021] (https://arxiv.org/pdf/2103.17239.pdf).
     This rescales diagonaly the residual outputs close to 0, with a learnt scale.
 
     Args:
@@ -206,27 +230,28 @@
                     state_dict[prefix + "mha." + key] = state_dict.pop(prefix + key)
         super()._load_from_state_dict(state_dict, prefix, *args, **kwargs)
 
     def _get_mask(self, current_steps: int, device: torch.device, dtype: torch.dtype):
         # Return a causal mask, accounting for potentially stored past keys/values
         # We actually return a bias for the attention score, as this has the same
         # convention both in the builtin MHA in Pytorch, and Xformers functions.
+        time_dim = _get_attention_time_dimension()
         if self.memory_efficient:
             from xformers.ops import LowerTriangularMask
             if current_steps == 1:
                 # If we only have one step, then we do not need a mask.
                 return None
             elif 'past_keys' in self._streaming_state:
                 raise RuntimeError('Not supported at the moment')
             else:
                 # Then we can safely use a lower triangular mask
                 return LowerTriangularMask()
         if self._streaming_state:
             past_keys = self._streaming_state['past_keys']
-            past_steps = past_keys.shape[1]
+            past_steps = past_keys.shape[time_dim]
         else:
             past_steps = 0
 
         queries_pos = torch.arange(
             past_steps, current_steps + past_steps, device=device).view(-1, 1)
         keys_pos = torch.arange(past_steps + current_steps, device=device).view(1, -1)
         delta = queries_pos - keys_pos
@@ -235,47 +260,50 @@
             valid &= (delta <= self.past_context)
         return torch.where(
             valid,
             torch.zeros([], device=device, dtype=dtype),
             torch.full([], float('-inf'), device=device, dtype=dtype))
 
     def _complete_kv(self, k, v):
+        time_dim = _get_attention_time_dimension()
         if self.cross_attention:
             # With cross attention we assume all keys and values
             # are already available, and streaming is with respect
             # to the queries only.
             return k, v
         # Complete the key/value pair using the streaming state.
         if self._streaming_state:
             pk = self._streaming_state['past_keys']
-            nk = torch.cat([pk, k], dim=1)
+            nk = torch.cat([pk, k], dim=time_dim)
             if v is k:
                 nv = nk
             else:
                 pv = self._streaming_state['past_values']
-                nv = torch.cat([pv, v], dim=1)
+                nv = torch.cat([pv, v], dim=time_dim)
         else:
             nk = k
             nv = v
 
-        assert nk.shape[1] == nv.shape[1]
+        assert nk.shape[time_dim] == nv.shape[time_dim]
         offset = 0
         if self.past_context is not None:
-            offset = max(0, nk.shape[1] - self.past_context)
+            offset = max(0, nk.shape[time_dim] - self.past_context)
         if self._is_streaming:
             self._streaming_state['past_keys'] = nk[:, offset:]
             if v is not k:
                 self._streaming_state['past_values'] = nv[:, offset:]
             if 'offset' in self._streaming_state:
                 self._streaming_state['offset'] += offset
             else:
                 self._streaming_state['offset'] = torch.tensor(0)
         return nk, nv
 
     def _apply_rope(self, query: torch.Tensor, key: torch.Tensor):
+        # TODO: fix and verify layout.
+        assert _efficient_attention_backend == 'xformers', 'Rope not supported with torch attn.'
         # Apply rope embeddings to query and key tensors.
         assert self.rope is not None
         if 'past_keys' in self._streaming_state:
             past_keys_offset = self._streaming_state['past_keys'].shape[1]
         else:
             past_keys_offset = 0
         if 'offset' in self._streaming_state:
@@ -288,14 +316,19 @@
     def forward(self, query: torch.Tensor, key: torch.Tensor, value: torch.Tensor,
                 key_padding_mask=None, need_weights=False, attn_mask=None,
                 average_attn_weights=True, is_causal=False):
         assert attn_mask is None
         assert not is_causal, ("new param added in torch 2.0.1 not supported, "
                                "use the causal args in the constructor.")
 
+        time_dim = _get_attention_time_dimension()
+        if time_dim == 2:
+            layout = "b h t d"
+        else:
+            layout = "b t h d"
         dtype = query.dtype
         if self._is_streaming:
             assert self.causal or self.cross_attention, \
                 "Streaming only available for causal or cross attention"
 
         if self.causal:
             # At the moment we specialize only for the self-attention case.
@@ -320,76 +353,86 @@
                 q = nn.functional.linear(query, self.in_proj_weight[:dim], bias_q)
                 # todo: when streaming, we could actually save k, v and check the shape actually match.
                 k = nn.functional.linear(key, self.in_proj_weight[dim: 2 * dim], bias_k)
                 v = nn.functional.linear(value, self.in_proj_weight[2 * dim:], bias_v)
                 if self.qk_layer_norm is True:
                     q = self.q_layer_norm(q)
                     k = self.k_layer_norm(k)
-                # q, k, v = [rearrange(x, "b t (h d) -> (b h) t d", h=self.num_heads) for x in [q, k, v]]
-                q, k, v = [rearrange(x, "b t (h d) -> b t h d", h=self.num_heads) for x in [q, k, v]]
+                q, k, v = [rearrange(x, f"b t (h d) -> {layout}", h=self.num_heads) for x in [q, k, v]]
             else:
                 if not _is_profiled():
                     # profiling breaks that propertysomehow.
                     assert query is key, "specialized implementation"
                     assert value is key, "specialized implementation"
                 projected = nn.functional.linear(query, self.in_proj_weight, self.in_proj_bias)
                 if self.kv_repeat == 1:
-                    packed = rearrange(projected, "b t (p h d) -> b t p h d", p=3, h=self.num_heads)
+                    if time_dim == 2:
+                        bound_layout = "b h p t d"
+                    else:
+                        bound_layout = "b t p h d"
+                    packed = rearrange(projected, f"b t (p h d) -> {bound_layout}", p=3, h=self.num_heads)
                     q, k, v = ops.unbind(packed, dim=2)
                 else:
                     embed_dim = self.embed_dim
                     per_head_dim = (embed_dim // self.num_heads)
                     kv_heads = self.num_heads // self.kv_repeat
                     q = projected[:, :, :embed_dim]
                     start = embed_dim
                     end = start + per_head_dim * kv_heads
                     k = projected[:, :, start: end]
                     v = projected[:, :, end:]
-                    q = rearrange(q, "b t (h d) -> b t h d", h=self.num_heads)
-                    k = rearrange(k, "b t (h d) -> b t h d", h=kv_heads)
-                    v = rearrange(v, "b t (h d) -> b t h d", h=kv_heads)
+                    q = rearrange(q, f"b t (h d) -> {layout}", h=self.num_heads)
+                    k = rearrange(k, f"b t (h d) -> {layout}", h=kv_heads)
+                    v = rearrange(v, f"b t (h d) -> {layout}", h=kv_heads)
 
                 if self.qk_layer_norm is True:
                     assert self.kv_repeat == 1
-                    q, k = [rearrange(x, "b t h d -> b t (h d)") for x in [q, k]]
+                    q, k = [rearrange(x, f"{layout} -> b t (h d)") for x in [q, k]]
                     q = self.q_layer_norm(q)
                     k = self.k_layer_norm(k)
-                    q, k = [rearrange(x, "b t (h d) -> b t h d", h=self.num_heads) for x in [q, k]]
+                    q, k = [rearrange(x, f"b t (h d) -> {layout}", h=self.num_heads) for x in [q, k]]
                 if self.rope:
                     q, k = self._apply_rope(q, k)
                 k, v = self._complete_kv(k, v)
                 if self.kv_repeat > 1:
                     k = expand_repeated_kv(k, self.kv_repeat)
                     v = expand_repeated_kv(v, self.kv_repeat)
             if self.attention_as_float32:
                 q, k, v = [x.float() for x in [q, k, v]]
             if self.memory_efficient:
                 p = self.dropout if self.training else 0
-                x = ops.memory_efficient_attention(q, k, v, attn_mask, p=p)
+                if _efficient_attention_backend == 'torch':
+                    x = torch.nn.functional.scaled_dot_product_attention(
+                        q, k, v, is_causal=attn_mask is not None, dropout_p=p)
+                else:
+                    x = ops.memory_efficient_attention(q, k, v, attn_mask, p=p)
             else:
                 # We include the dot product as float32, for consistency
                 # with the other implementations that include that step
                 # as part of the attention. Note that when using `autocast`,
                 # the einsums would be done as bfloat16, but the softmax
                 # would be done as bfloat16, so `attention_as_float32` will
                 # extend a bit the range of operations done in float32,
                 # although this should make no difference.
                 q = q / q.shape[-1] ** 0.5
+                key_layout = layout.replace('t', 'k')
+                query_layout = layout
                 if self._is_streaming and self.safe_streaming and q.device.type == 'cuda':
                     with torch.autocast(device_type=q.device.type, dtype=torch.float32):
-                        pre_w = torch.einsum("bqhc,bkhc->bhqk", q, k)
+                        pre_w = torch.einsum(f"{query_layout},{key_layout}-> b h t k", q, k)
                 else:
-                    pre_w = torch.einsum("bqhc,bkhc->bhqk", q, k)
+                    pre_w = torch.einsum(f"{query_layout},{key_layout}-> b h t k", q, k)
                 if attn_mask is not None:
                     pre_w = pre_w + attn_mask
                 w = torch.softmax(pre_w, dim=-1)
                 w = F.dropout(w, self.dropout, training=self.training).to(v)
-                x = torch.einsum("bhqk,bkhc->bqhc", w, v)
+                # Key and value have the same format.
+                x = torch.einsum(f"b h t k, {key_layout} -> {layout}", w, v)
             x = x.to(dtype)
-            x = rearrange(x, "b t h d -> b t (h d)", h=self.num_heads)
+            x = rearrange(x, f"{layout} -> b t (h d)", h=self.num_heads)
             x = self.out_proj(x)
         else:
             key, value = self._complete_kv(key, value)
             if self.attention_as_float32:
                 query, key, value = [x.float() for x in [query, key, value]]
             x, _ = self.mha(
                 query, key, value, key_padding_mask,
```

### Comparing `audiocraft-0.0.1/audiocraft/quantization/base.py` & `audiocraft-0.0.2/audiocraft/quantization/base.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/quantization/core_vq.py` & `audiocraft-0.0.2/audiocraft/quantization/core_vq.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/quantization/vq.py` & `audiocraft-0.0.2/audiocraft/quantization/vq.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/utils/autocast.py` & `audiocraft-0.0.2/audiocraft/utils/autocast.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/utils/export.py` & `audiocraft-0.0.2/audiocraft/utils/export.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/utils/notebook.py` & `audiocraft-0.0.2/audiocraft/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/audiocraft/utils/utils.py` & `audiocraft-0.0.2/audiocraft/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         p (int): The p in “top-p”.
     Returns:
         torch.Tensor: Sampled tokens.
     """
     probs_sort, probs_idx = torch.sort(probs, dim=-1, descending=True)
     probs_sum = torch.cumsum(probs_sort, dim=-1)
     mask = probs_sum - probs_sort > p
-    probs_sort *= (~mask).float(0)
+    probs_sort *= (~mask).float()
     probs_sort.div_(probs_sort.sum(dim=-1, keepdim=True))
     next_token = multinomial(probs_sort, num_samples=1)
     next_token = torch.gather(probs_idx, -1, next_token)
     return next_token
 
 
 class DummyPoolExecutor:
```

### Comparing `audiocraft-0.0.1/audiocraft.egg-info/SOURCES.txt` & `audiocraft-0.0.2/audiocraft.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Makefile
 README.md
 mypy.ini
 requirements.txt
 setup.cfg
 setup.py
 assets/bach.mp3
+assets/bolero_ravel.mp3
 audiocraft/__init__.py
 audiocraft/py.typed
 audiocraft.egg-info/PKG-INFO
 audiocraft.egg-info/SOURCES.txt
 audiocraft.egg-info/dependency_links.txt
 audiocraft.egg-info/requires.txt
 audiocraft.egg-info/top_level.txt
```

### Comparing `audiocraft-0.0.1/setup.py` & `audiocraft-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 from setuptools import setup, find_packages
 
 
 NAME = 'audiocraft'
 DESCRIPTION = 'Audio research library for PyTorch'
 
-URL = 'https://github.com/fairinternal/audiocraft'
+URL = 'https://github.com/facebookresearch/audiocraft'
 AUTHOR = 'FAIR Speech & Audio'
-EMAIL = 'defossez@meta.com'
+EMAIL = 'defossez@meta.com, jadecopet@meta.com'
 REQUIRES_PYTHON = '>=3.8.0'
 
 for line in open('audiocraft/__init__.py'):
     line = line.strip()
     if '__version__' in line:
         context = {}
         exec(line, context)
```

### Comparing `audiocraft-0.0.1/tests/common_utils/temp_utils.py` & `audiocraft-0.0.2/tests/common_utils/temp_utils.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/common_utils/wav_utils.py` & `audiocraft-0.0.2/tests/common_utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/data/test_audio.py` & `audiocraft-0.0.2/tests/data/test_audio.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/data/test_audio_dataset.py` & `audiocraft-0.0.2/tests/data/test_audio_dataset.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/data/test_audio_utils.py` & `audiocraft-0.0.2/tests/data/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/modules/test_codebooks_patterns.py` & `audiocraft-0.0.2/tests/modules/test_codebooks_patterns.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/modules/test_conv.py` & `audiocraft-0.0.2/tests/modules/test_conv.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/modules/test_lstm.py` & `audiocraft-0.0.2/tests/modules/test_lstm.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/modules/test_rope.py` & `audiocraft-0.0.2/tests/modules/test_rope.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 #
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 
 from audiocraft.modules.rope import RotaryEmbedding
-from audiocraft.modules.transformer import StreamingTransformer
+from audiocraft.modules.transformer import StreamingTransformer, set_efficient_attention_backend
 
 
 def test_rope():
+    set_efficient_attention_backend('xformers')
     B, T, H, C = 8, 75, 16, 128
 
     rope = RotaryEmbedding(dim=C)
     xq = torch.rand((B, T, H, C))
     xk = torch.rand((B, T, H, C))
     xq_out, xk_out = rope.rotate_qk(xq, xk, start=7)
 
     assert list(xq_out.shape) == [B, T, H, C]
     assert list(xk_out.shape) == [B, T, H, C]
 
 
 def test_rope_io_dtypes():
+    set_efficient_attention_backend('xformers')
     B, T, H, C = 8, 75, 16, 128
 
     rope_32 = RotaryEmbedding(dim=C, dtype=torch.float32)
     rope_64 = RotaryEmbedding(dim=C, dtype=torch.float64)
 
     # Test bfloat16 inputs w/ both 32 and 64 precision rope.
     xq_16 = torch.rand((B, T, H, C)).to(torch.bfloat16)
@@ -42,14 +44,15 @@
     xq_out, xk_out = rope_32.rotate_qk(xq_32, xk_32)
     assert xq_out.dtype == torch.float32
     xq_out, xk_out = rope_64.rotate_qk(xq_32, xk_32)
     assert xq_out.dtype == torch.float32
 
 
 def test_transformer_with_rope():
+    set_efficient_attention_backend('xformers')
     torch.manual_seed(1234)
     for pos in ['rope', 'sin_rope']:
         tr = StreamingTransformer(
             16, 4, 2, custom=True, dropout=0., layer_scale=0.1,
             positional_embedding=pos)
         tr.eval()
         steps = 12
@@ -57,14 +60,15 @@
 
         out = tr(x)
         assert list(out.shape) == list(x.shape)
 
 
 @torch.no_grad()
 def test_rope_streaming():
+    set_efficient_attention_backend('xformers')
     torch.manual_seed(1234)
     tr = StreamingTransformer(
         16, 4, 2, causal=True, dropout=0.,
         custom=True, positional_embedding='rope')
     tr.eval()
     steps = 12
     x = torch.randn(3, steps, 16)
@@ -84,14 +88,15 @@
     assert list(out.shape) == [3, steps, 16]
     delta = torch.norm(out - ref) / torch.norm(out)
     assert delta < 1e-6, delta
 
 
 @torch.no_grad()
 def test_rope_streaming_past_context():
+    set_efficient_attention_backend('xformers')
     torch.manual_seed(1234)
 
     for context in [None, 10]:
         tr = StreamingTransformer(
             16, 4, 1 if context else 2,
             causal=True, past_context=context, custom=True,
             dropout=0., positional_embedding='rope')
@@ -113,14 +118,15 @@
         out = torch.cat(outs, dim=1)
         assert list(out.shape) == [3, steps, 16]
         delta = torch.norm(out - ref) / torch.norm(out)
         assert delta < 1e-6, delta
 
 
 def test_rope_memory_efficient():
+    set_efficient_attention_backend('xformers')
     torch.manual_seed(1234)
     tr = StreamingTransformer(
         16, 4, 2, custom=True, dropout=0., layer_scale=0.1,
         positional_embedding='rope')
     tr_mem_efficient = StreamingTransformer(
         16, 4, 2, dropout=0., memory_efficient=True, layer_scale=0.1,
         positional_embedding='rope')
@@ -133,26 +139,28 @@
         y = tr(x)
         y2 = tr_mem_efficient(x)
         # Check at float precision b/c this is the rope default.
         assert torch.allclose(y, y2, atol=1e-7), (y - y2).norm()
 
 
 def test_rope_with_xpos():
+    set_efficient_attention_backend('xformers')
     B, T, H, C = 8, 75, 16, 128
 
     rope = RotaryEmbedding(dim=C, xpos=True)
     xq = torch.rand((B, T, H, C))
     xk = torch.rand((B, T, H, C))
     xq_out, xk_out = rope.rotate_qk(xq, xk, start=7)
 
     assert list(xq_out.shape) == [B, T, H, C]
     assert list(xk_out.shape) == [B, T, H, C]
 
 
 def test_positional_scale():
+    set_efficient_attention_backend('xformers')
     B, T, H, C = 8, 75, 16, 128
 
     rope = RotaryEmbedding(dim=C, xpos=True, scale=0.0)
     xq = torch.rand((B, T, H, C))
     xk = torch.rand((B, T, H, C))
     xq_out, xk_out = rope.rotate_qk(xq, xk, start=7)
```

### Comparing `audiocraft-0.0.1/tests/modules/test_seanet.py` & `audiocraft-0.0.2/tests/modules/test_seanet.py`

 * *Files identical despite different names*

### Comparing `audiocraft-0.0.1/tests/modules/test_transformer.py` & `audiocraft-0.0.2/tests/modules/test_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # LICENSE file in the root directory of this source tree.
 
 from itertools import product
 
 import pytest
 import torch
 
-from audiocraft.modules.transformer import StreamingMultiheadAttention, StreamingTransformer
+from audiocraft.modules.transformer import (
+    StreamingMultiheadAttention, StreamingTransformer, set_efficient_attention_backend)
 
 
 def test_transformer_causal_streaming():
     torch.manual_seed(1234)
 
     for context, custom in product([None, 10], [False, True]):
         # Test that causality and receptive fields are properly handled.
@@ -81,28 +82,31 @@
             tr.set_streaming_state(state)
             y2 = tr(x[:, 1:2])
             assert torch.allclose(y, y2), (y - y2).norm()
             assert tr.flush() is None
 
 
 def test_memory_efficient():
-    torch.manual_seed(1234)
-    tr = StreamingTransformer(
-        16, 4, 2, custom=True, dropout=0., layer_scale=0.1)
-    tr_mem_efficient = StreamingTransformer(
-        16, 4, 2, dropout=0., memory_efficient=True, layer_scale=0.1)
-    tr_mem_efficient.load_state_dict(tr.state_dict())
-    tr.eval()
-    steps = 12
-    x = torch.randn(3, steps, 16)
+    for backend in ['torch', 'xformers']:
+        torch.manual_seed(1234)
+        set_efficient_attention_backend(backend)
 
-    with torch.no_grad():
-        y = tr(x)
-        y2 = tr_mem_efficient(x)
-        assert torch.allclose(y, y2), (y - y2).norm()
+        tr = StreamingTransformer(
+            16, 4, 2, custom=True, dropout=0., layer_scale=0.1)
+        tr_mem_efficient = StreamingTransformer(
+            16, 4, 2, dropout=0., memory_efficient=True, layer_scale=0.1)
+        tr_mem_efficient.load_state_dict(tr.state_dict())
+        tr.eval()
+        steps = 12
+        x = torch.randn(3, steps, 16)
+
+        with torch.no_grad():
+            y = tr(x)
+            y2 = tr_mem_efficient(x)
+            assert torch.allclose(y, y2), ((y - y2).norm(), backend)
 
 
 def test_attention_as_float32():
     torch.manual_seed(1234)
     cases = [
         {'custom': True},
         {'custom': False},
@@ -124,39 +128,41 @@
             y = tr(x)
             y2 = tr_float32(x)
             assert not torch.allclose(y, y2), (y - y2).norm()
 
 
 @torch.no_grad()
 def test_streaming_memory_efficient():
-    torch.manual_seed(1234)
-    tr = StreamingTransformer(16, 4, 2, causal=True, dropout=0., custom=True)
-    tr_mem_efficient = StreamingTransformer(
-        16, 4, 2, dropout=0., memory_efficient=True, causal=True)
-    tr.load_state_dict(tr_mem_efficient.state_dict())
-    tr.eval()
-    tr_mem_efficient.eval()
-    steps = 12
-    x = torch.randn(3, steps, 16)
+    for backend in ['torch', 'xformers']:
+        torch.manual_seed(1234)
+        set_efficient_attention_backend(backend)
+        tr = StreamingTransformer(16, 4, 2, causal=True, dropout=0., custom=True)
+        tr_mem_efficient = StreamingTransformer(
+            16, 4, 2, dropout=0., memory_efficient=True, causal=True)
+        tr.load_state_dict(tr_mem_efficient.state_dict())
+        tr.eval()
+        tr_mem_efficient.eval()
+        steps = 12
+        x = torch.randn(3, steps, 16)
 
-    ref = tr(x)
+        ref = tr(x)
 
-    with tr_mem_efficient.streaming():
-        outs = []
-        # frame_sizes = [2] + [1] * (steps - 2)
-        frame_sizes = [1] * steps
-
-        for frame_size in frame_sizes:
-            frame = x[:, :frame_size]
-            x = x[:, frame_size:]
-            outs.append(tr_mem_efficient(frame))
-
-    out = torch.cat(outs, dim=1)
-    delta = torch.norm(out - ref) / torch.norm(out)
-    assert delta < 1e-6, delta
+        with tr_mem_efficient.streaming():
+            outs = []
+            # frame_sizes = [2] + [1] * (steps - 2)
+            frame_sizes = [1] * steps
+
+            for frame_size in frame_sizes:
+                frame = x[:, :frame_size]
+                x = x[:, frame_size:]
+                outs.append(tr_mem_efficient(frame))
+
+        out = torch.cat(outs, dim=1)
+        delta = torch.norm(out - ref) / torch.norm(out)
+        assert delta < 1e-6, delta
 
 
 def test_cross_attention():
     torch.manual_seed(1234)
     for norm_first in [True, False]:
         m = StreamingTransformer(
             16, 4, 2, cross_attention=False, norm_first=norm_first, dropout=0., custom=True)
@@ -200,15 +206,15 @@
 
     queries = torch.randn(3, 7, dim)
     keys = torch.randn(3, 9, dim)
     values = torch.randn(3, 9, dim)
 
     y = cross_attn(queries, keys, values)[0]
     y_ref = ref_attn(queries, keys, values)[0]
-    assert torch.allclose(y, y_ref, atol=1e-7)
+    assert torch.allclose(y, y_ref, atol=1e-7), (y - y_ref).norm() / y_ref.norm()
 
     # Now let's check that streaming is working properly.
     with cross_attn.streaming():
         ys = []
         for step in range(queries.shape[1]):
             ys.append(cross_attn(queries[:, step: step + 1], keys, values)[0])
     y_streaming = torch.cat(ys, dim=1)
```

