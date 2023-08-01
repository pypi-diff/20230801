# Comparing `tmp/aotpy-0.8.2.tar.gz` & `tmp/aotpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.8.2.tar", last modified: Wed Jul 26 16:34:13 2023, max compression
+gzip compressed data, was "aotpy-1.0.0.tar", last modified: Tue Aug  1 16:38:04 2023, max compression
```

## Comparing `aotpy-0.8.2.tar` & `aotpy-1.0.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.174644 aotpy-0.8.2/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.8.2/LICENSE
--rw-rw-rw-   0        0        0     3108 2023-07-26 16:34:13.174644 aotpy-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     2309 2023-07-26 16:33:12.000000 aotpy-0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.122675 aotpy-0.8.2/aotpy/
--rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.8.2/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.138676 aotpy-0.8.2/aotpy/core/
--rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.8.2/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.8.2/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     5304 2023-07-17 15:33:42.000000 aotpy-0.8.2/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     3050 2023-07-17 15:15:05.000000 aotpy-0.8.2/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0     1162 2023-07-17 10:40:27.000000 aotpy-0.8.2/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1338 2023-07-17 12:24:43.000000 aotpy-0.8.2/aotpy/core/image.py
--rw-rw-rw-   0        0        0     5293 2023-07-17 15:13:26.000000 aotpy-0.8.2/aotpy/core/loop.py
--rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.8.2/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-0.8.2/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-0.8.2/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-0.8.2/aotpy/core/time.py
--rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-0.8.2/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.142674 aotpy-0.8.2/aotpy/data/
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.142674 aotpy-0.8.2/aotpy/data/ERIS/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.2/aotpy/data/ERIS/ho_subap.fits
--rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-0.8.2/aotpy/data/ERIS/lo_subap.fits
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.142674 aotpy-0.8.2/aotpy/data/GALACSI/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.2/aotpy/data/GALACSI/subap.fits
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.146679 aotpy-0.8.2/aotpy/data/NAOMI/
--rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.8.2/aotpy/data/NAOMI/zernike_control_modes.fits
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.154652 aotpy-0.8.2/aotpy/data/PAPYRUS/
--rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-0.8.2/aotpy/data/PAPYRUS/T152_pupil.fits
--rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.8.2/aotpy/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.158644 aotpy-0.8.2/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-0.8.2/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-0.8.2/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.162644 aotpy-0.8.2/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.8.2/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    26722 2023-07-25 11:24:17.000000 aotpy-0.8.2/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    40528 2023-07-25 15:30:54.000000 aotpy-0.8.2/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     9313 2023-07-24 13:06:09.000000 aotpy-0.8.2/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31347 2023-07-26 14:41:33.000000 aotpy-0.8.2/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.174644 aotpy-0.8.2/aotpy/translators/
--rw-rw-rw-   0        0        0      440 2023-06-28 16:02:08.000000 aotpy-0.8.2/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-0.8.2/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     7166 2023-07-25 17:10:27.000000 aotpy-0.8.2/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0    18440 2023-07-26 15:13:13.000000 aotpy-0.8.2/aotpy/translators/eris.py
--rw-rw-rw-   0        0        0    10740 2023-07-26 16:13:22.000000 aotpy-0.8.2/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0    11473 2023-07-25 17:13:23.000000 aotpy-0.8.2/aotpy/translators/galacsi.py
--rw-rw-rw-   0        0        0     7574 2023-07-25 17:10:28.000000 aotpy-0.8.2/aotpy/translators/naomi.py
--rw-rw-rw-   0        0        0    12588 2023-07-26 10:27:29.000000 aotpy-0.8.2/aotpy/translators/papyrus.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.126675 aotpy-0.8.2/aotpy.egg-info/
--rw-rw-rw-   0        0        0     3108 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.8.2/pyproject.toml
--rw-rw-rw-   0        0        0     1029 2023-07-26 16:34:13.174644 aotpy-0.8.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.935191 aotpy-1.0.0/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3108 2023-08-01 16:38:04.935191 aotpy-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2309 2023-07-26 16:33:12.000000 aotpy-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.845614 aotpy-1.0.0/aotpy/
+-rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-1.0.0/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.886179 aotpy-1.0.0/aotpy/core/
+-rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-1.0.0/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-1.0.0/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     5304 2023-07-17 15:33:42.000000 aotpy-1.0.0/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     3050 2023-07-17 15:15:05.000000 aotpy-1.0.0/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0     1162 2023-08-01 14:14:59.000000 aotpy-1.0.0/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1338 2023-07-31 08:42:20.000000 aotpy-1.0.0/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     5293 2023-07-17 15:13:26.000000 aotpy-1.0.0/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-1.0.0/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-1.0.0/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-1.0.0/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-1.0.0/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-1.0.0/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.889161 aotpy-1.0.0/aotpy/data/
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.891156 aotpy-1.0.0/aotpy/data/ERIS/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-1.0.0/aotpy/data/ERIS/ho_subap.fits
+-rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-1.0.0/aotpy/data/ERIS/lo_subap.fits
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.894158 aotpy-1.0.0/aotpy/data/GALACSI/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-1.0.0/aotpy/data/GALACSI/subap.fits
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.895157 aotpy-1.0.0/aotpy/data/NAOMI/
+-rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-1.0.0/aotpy/data/NAOMI/zernike_control_modes.fits
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.908618 aotpy-1.0.0/aotpy/data/PAPYRUS/
+-rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-1.0.0/aotpy/data/PAPYRUS/T152_pupil.fits
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-1.0.0/aotpy/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.912624 aotpy-1.0.0/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-1.0.0/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-1.0.0/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.918642 aotpy-1.0.0/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-1.0.0/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    26722 2023-07-25 11:24:17.000000 aotpy-1.0.0/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    40530 2023-07-28 15:36:51.000000 aotpy-1.0.0/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     9760 2023-08-01 15:07:29.000000 aotpy-1.0.0/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31140 2023-08-01 14:05:38.000000 aotpy-1.0.0/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.930647 aotpy-1.0.0/aotpy/translators/
+-rw-rw-rw-   0        0        0      440 2023-06-28 16:02:08.000000 aotpy-1.0.0/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-1.0.0/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     7166 2023-07-25 17:10:27.000000 aotpy-1.0.0/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0    18590 2023-08-01 16:25:41.000000 aotpy-1.0.0/aotpy/translators/eris.py
+-rw-rw-rw-   0        0        0    11377 2023-08-01 15:46:15.000000 aotpy-1.0.0/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0    11574 2023-08-01 16:28:10.000000 aotpy-1.0.0/aotpy/translators/galacsi.py
+-rw-rw-rw-   0        0        0     7616 2023-08-01 15:46:15.000000 aotpy-1.0.0/aotpy/translators/naomi.py
+-rw-rw-rw-   0        0        0    12598 2023-08-01 16:31:56.000000 aotpy-1.0.0/aotpy/translators/papyrus.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:38:04.860354 aotpy-1.0.0/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     3108 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 16:38:04.000000 aotpy-1.0.0/aotpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1029 2023-08-01 16:38:04.938203 aotpy-1.0.0/setup.cfg
```

### Comparing `aotpy-0.8.2/LICENSE` & `aotpy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/PKG-INFO` & `aotpy-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.8.2
+Version: 1.0.0
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.8.2/README.md` & `aotpy-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/__init__.py` & `aotpy-1.0.0/aotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/__init__.py` & `aotpy-1.0.0/aotpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/aberration.py` & `aotpy-1.0.0/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/ao_system.py` & `aotpy-1.0.0/aotpy/core/ao_system.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/atmosphere.py` & `aotpy-1.0.0/aotpy/core/atmosphere.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/base.py` & `aotpy-1.0.0/aotpy/core/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/image.py` & `aotpy-1.0.0/aotpy/core/image.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/loop.py` & `aotpy-1.0.0/aotpy/core/loop.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/optical_sensor.py` & `aotpy-1.0.0/aotpy/core/optical_sensor.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/source.py` & `aotpy-1.0.0/aotpy/core/source.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/telescope.py` & `aotpy-1.0.0/aotpy/core/telescope.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/time.py` & `aotpy-1.0.0/aotpy/core/time.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/core/wavefront_corrector.py` & `aotpy-1.0.0/aotpy/core/wavefront_corrector.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/data/ERIS/ho_subap.fits` & `aotpy-1.0.0/aotpy/data/ERIS/ho_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/data/ERIS/lo_subap.fits` & `aotpy-1.0.0/aotpy/data/ERIS/lo_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/data/GALACSI/subap.fits` & `aotpy-1.0.0/aotpy/data/GALACSI/subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/data/NAOMI/zernike_control_modes.fits` & `aotpy-1.0.0/aotpy/data/NAOMI/zernike_control_modes.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/data/PAPYRUS/T152_pupil.fits` & `aotpy-1.0.0/aotpy/data/PAPYRUS/T152_pupil.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/io/base.py` & `aotpy-1.0.0/aotpy/io/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/io/fits/_keywords.py` & `aotpy-1.0.0/aotpy/io/fits/_keywords.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/io/fits/reader.py` & `aotpy-1.0.0/aotpy/io/fits/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import aotpy
 from . import _keywords as kw
 from .utils import FITSURLImage, FITSFileImage, image_from_hdu, keyword_is_relevant, metadatum_from_card
 from ..base import SystemReader
 
 _reference_pattern = re.compile(r'([^<]+)<(.+)>(\d+)?')
 
+
 def read_system_from_fits(filename: str, extra_data: bool = False, **kwargs) -> aotpy.AOSystem:
     """
     Get `AOSystem` from FITS file specified by `filename`.
 
     Parameters
     ----------
     filename
```

### Comparing `aotpy-0.8.2/aotpy/io/fits/utils.py` & `aotpy-1.0.0/aotpy/io/fits/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
 from . import _keywords as kw
 
-__all__ = ['FITSFileImage', 'FITSURLImage', 'image_from_file', 'image_from_hdus', 'image_from_hdu',
-           'metadatum_from_card', 'metadata_from_hdu', 'datetime_to_iso', 'keyword_is_relevant']
+__all__ = ['FITSFileImage', 'FITSURLImage', 'image_from_fits_file', 'image_from_hdus', 'image_from_hdu',
+           'card_from_metadatum', 'metadatum_from_card', 'metadata_from_hdu', 'datetime_to_iso', 'keyword_is_relevant']
 
 
 def keyword_is_relevant(keyword):
     """Check if keyword is relevant. Keywords are considered "irrelevant" if they are already reflected elsewhere in the
      object produced by Astropy."""
     _standard_keywords = {'SIMPLE', 'EXTEND', 'BSCALE', 'BZERO', 'XTENSION', 'BITPIX',
                           'PCOUNT', 'GCOUNT', 'EXTNAME', 'CHECKSUM', 'DATASUM'}
@@ -84,17 +84,17 @@
         self.index = index
         self.name, self.data, self.unit, self._time, self.metadata = _get_image_fields_from_file(url, index, **kwargs)
 
     def __eq__(self, other):
         return self.url == other.url and self.index == other.index and self.time == other.time
 
 
-def image_from_file(path: str | os.PathLike, index: int = None, *, name: str = None, **kwargs) -> aotpy.Image:
+def image_from_fits_file(path: str | os.PathLike, index: int = None, *, name: str = None, **kwargs) -> aotpy.Image:
     """
-    Get `Image` from specified path or URL.
+    Get `Image` from FITS file specified on path or URL.
 
     Parameters
     ----------
     path
         Path/URL to FITS file that contains multidimensional data.
     index: int, optional
         Index of the HDU that contains the image data. If omitted, the first HDU containing image data is assumed.
@@ -195,15 +195,29 @@
     _time = None
     if (md := next((x for x in metadata if x.key == kw.TIME_REFERENCE), None)) is not None:
         _time = md.value
         metadata.remove(md)
     return hdu.name, hdu.data, unit, _time, metadata
 
 
-def metadatum_from_card(card: fits.Card):
+def card_from_metadatum(md: aotpy.Metadatum) -> fits.Card:
+    """
+    Get `Card` from `Metadatum`.
+
+    Parameters
+    ----------
+    md
+        `Metadatum` to convert to `Card`.
+    """
+    return fits.Card(f'HIERARCH {md.key}' if (len(md.key) > 8 and not md.key.startswith('HIERARCH')) else md.key,
+                     md.value,
+                     md.comment)
+
+
+def metadatum_from_card(card: fits.Card) -> aotpy.Metadatum:
     """
     Get `Metadatum` from `Card`.
 
     Parameters
     ----------
     card
         `Card` to convert to `Metadatum`.
```

### Comparing `aotpy-0.8.2/aotpy/io/fits/writer.py` & `aotpy-1.0.0/aotpy/io/fits/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
 from . import _keywords as kw
-from .utils import FITSFileImage, FITSURLImage, datetime_to_iso
+from .utils import FITSFileImage, FITSURLImage, datetime_to_iso, card_from_metadatum
 from ..base import SystemWriter
 
 # NaN is defined here as a single precision float (32-bits), which is the lowest possible float precision in FITS.
 # The goal is to ensure that low precision numpy arrays aren't unnecessarily upcasted just because of NaN.
 _nan = np.single(np.nan)
 
 # Given that integer values in AOT cannot be negative, we assume the lowest integer in a signed 16-bit integer is null.
@@ -533,17 +533,15 @@
         if self._system.strehl_ratio is not None:
             hdr[kw.AOT_STREHL_RATIO] = self._system.strehl_ratio
         if self._system.temporal_error is not None:
             hdr[kw.AOT_TEMPORAL_ERROR] = self._system.temporal_error
         if self._system.config is not None:
             hdr[kw.AOT_CONFIG] = self._system.config
 
-        hdr.extend([(f'HIERARCH {md.key}' if len(md.key) > 8 else md.key,
-                            md.value,
-                            md.comment) for md in self._system.metadata])
+        hdr.extend([card_from_metadatum(md) for md in self._system.metadata])
         return fits.PrimaryHDU(header=hdr)
 
     def _create_bintable_hdus(self) -> list[fits.BinTableHDU]:
         hdus = []
         for table_name in kw.TABLE_SEQUENCE:
             try:
                 table = self._tables[table_name]
@@ -607,16 +605,14 @@
                 columns.append(col)
             hdus.append(fits.BinTableHDU.from_columns(name=table_name, columns=columns))
         return hdus
 
     def _create_image_hdus(self) -> list[fits.ImageHDU]:
         hdus = []
         for image in self._images.values():
-            hdr = fits.Header([(f'HIERARCH {md.key}' if len(md.key) > 8 else md.key,
-                                md.value,
-                                md.comment) for md in image.metadata])
+            hdr = fits.Header([card_from_metadatum(md) for md in image.metadata])
             if image.time is not None:
                 hdr[kw.TIME_REFERENCE] = self._create_row_reference(image.time.uid)
             if image.unit is not None:
                 hdr[kw.IMAGE_UNIT] = image.unit
             hdus.append(fits.ImageHDU(name=image.name, data=image.data, header=hdr))
         return hdus
```

### Comparing `aotpy-0.8.2/aotpy/translators/base.py` & `aotpy-1.0.0/aotpy/translators/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/translators/ciao.py` & `aotpy-1.0.0/aotpy/translators/ciao.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/aotpy/translators/eris.py` & `aotpy-1.0.0/aotpy/translators/eris.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
-from aotpy.io import image_from_file
+from aotpy.io import image_from_fits_file
 from .eso import ESOTranslator
 
 
 # TODO set image units
 
 
 class ERISTranslator(ESOTranslator):
@@ -78,15 +78,15 @@
         active_laser = fits.getheader(self._path / 'JitCtr.CFG.DYNAMIC.fits')['ACTIVE_JITTER']
         llt = aotpy.LaserLaunchTelescope(f'LLT{active_laser}')
         lgs = aotpy.SodiumLaserGuideStar(uid='LGS', laser_launch_telescope=llt)
         self.system.sources.append(lgs)
 
         eris_data_path = importlib.resources.files('aotpy.data') / 'ERIS'
         with importlib.resources.as_file(eris_data_path / 'ho_subap.fits') as p:
-            subaperture_mask = image_from_file(p, name='LGS WFS SUBAPERTURE MASK')
+            subaperture_mask = image_from_fits_file(p, name='LGS WFS SUBAPERTURE MASK')
         n_valid_subapertures = np.count_nonzero(subaperture_mask.data != -1)
 
         reference = self._stack_slopes(fits.getdata(self._path / 'LGSAcq.DET1.REFSLP_WITH_OFFSETS.fits'),
                                        slope_axis=1)[0]
         lgs_wfs = aotpy.ShackHartmann(
             uid='LGS WFS',
             source=lgs,
@@ -97,17 +97,17 @@
             mask_offsets=[aotpy.Coordinates(0, 0)],
             subaperture_intensities=aotpy.Image('LGS Intensities', lgs_loop_frame['Intensities'])
         )
         self.system.wavefront_sensors.append(lgs_wfs)
 
         lgs_wfs.detector = aotpy.Detector(
             uid='LGS DET1',
-            dark=image_from_file(self._path / 'LGSAcq.DET1.DARK.fits'),
-            weight_map=image_from_file(self._path / 'LGSAcq.DET1.WEIGHT.fits'),
-            sky_background=image_from_file(self._path / 'LGSAcq.DET1.BACKGROUND.fits'),
+            dark=self._image_from_eso_file(self._path / 'LGSAcq.DET1.DARK.fits'),
+            weight_map=self._image_from_eso_file(self._path / 'LGSAcq.DET1.WEIGHT.fits'),
+            sky_background=self._image_from_eso_file(self._path / 'LGSAcq.DET1.BACKGROUND.fits'),
             pixel_intensities=aotpy.Image(name='LGS Pixels',
                                           data=self._get_pixel_data_from_table(lgs_pix_frame),
                                           time=aotpy.Time('LGS Pixel Time',
                                                           frame_numbers=lgs_pix_frame['FrameCounter'].tolist()))
         )
         lgs_wfs.subaperture_size = \
             lgs_wfs.detector.pixel_intensities.data.shape[0] // lgs_wfs.subaperture_mask.data.shape[0]
@@ -124,16 +124,16 @@
             ref_commands=aotpy.Image('LGSCtr.ACT_POS_REF_MAP_WITH_OFFSETS',
                                      fits.getdata(self._path / 'LGSCtr.ACT_POS_REF_MAP_WITH_OFFSETS.fits')[:, 0]),
             time=lgs_time,
             framerate=lgs_freq,
             time_filter_num=aotpy.Image('LGSCtr.A_TERMS', fits.getdata(self._path / 'LGSCtr.A_TERMS.fits').T),
             time_filter_den=aotpy.Image('LGSCtr.B_TERMS', fits.getdata(self._path / 'LGSCtr.B_TERMS.fits').T),
             measurements_to_modes=aotpy.Image('CLMatrixOptimiser.S2M', s2m),
-            modes_to_commands=image_from_file(self._path / 'CLMatrixOptimiser.M2V.fits'),
-            commands_to_modes=image_from_file(self._path / 'CLMatrixOptimiser.V2M.fits'),
+            modes_to_commands=self._image_from_eso_file(self._path / 'CLMatrixOptimiser.M2V.fits'),
+            commands_to_modes=self._image_from_eso_file(self._path / 'CLMatrixOptimiser.V2M.fits'),
             modes_to_measurements=aotpy.Image('CLMatrixOptimiser.M2S', m2s),
         ))
 
         jit = aotpy.TipTiltMirror(
             uid='Jitter',
             telescope=llt
         )
@@ -185,15 +185,15 @@
             lo_timestamps_list = []
         else:
             lo_timestamps_list = lo_timestamps.tolist()
         ho_frame_numbers = lo_loop_frame['HO_FrameCounter']
         lo_time = aotpy.Time('LO Loop Time', timestamps=lo_timestamps_list, frame_numbers=ho_frame_numbers.tolist())
 
         with importlib.resources.as_file(eris_data_path / 'lo_subap.fits') as p:
-            subaperture_mask = image_from_file(p, name='LO WFS SUBAPERTURE MASK')
+            subaperture_mask = image_from_fits_file(p, name='LO WFS SUBAPERTURE MASK')
         n_valid_subapertures = np.count_nonzero(subaperture_mask.data != -1)
 
         reference = self._stack_slopes(fits.getdata(self._path / 'LOAcq.DET1.REFSLP_WITH_OFFSETS.fits'),
                                        slope_axis=1)[0]
         lo_wfs = aotpy.ShackHartmann(
             uid='LO WFS',
             source=ngs,
@@ -242,17 +242,17 @@
             cur = last + diff
             if cur > aux_fc.size - 1:
                 break
             aux_fc[cur] = masked_lgs[-1] + diff * step
 
         lo_wfs.detector = aotpy.Detector(
             uid='LO DET1',
-            dark=image_from_file(self._path / 'LOAcq.DET1.DARK.fits'),
-            weight_map=image_from_file(self._path / 'LOAcq.DET1.WEIGHT.fits'),
-            sky_background=image_from_file(self._path / 'LOAcq.DET1.BACKGROUND.fits'),
+            dark=self._image_from_eso_file(self._path / 'LOAcq.DET1.DARK.fits'),
+            weight_map=self._image_from_eso_file(self._path / 'LOAcq.DET1.WEIGHT.fits'),
+            sky_background=self._image_from_eso_file(self._path / 'LOAcq.DET1.BACKGROUND.fits'),
             pixel_intensities=aotpy.Image(name='LO Pixels',
                                           data=self._get_pixel_data_from_table(lo_pix_frame),
                                           time=aotpy.Time('LO Pixel Time',
                                                           frame_numbers=aux_fc.tolist()))
         )
         self.system.wavefront_sensors.append(lo_wfs)
         lo_wfs.subaperture_size = \
@@ -304,15 +304,15 @@
                              frame_numbers=ho_frame_numbers.tolist())
 
         ngs = aotpy.NaturalGuideStar('NGS')
         self.system.sources.append(ngs)
 
         eris_data_path = importlib.resources.files('aotpy.data') / 'ERIS'
         with importlib.resources.as_file(eris_data_path / 'ho_subap.fits') as p:
-            subaperture_mask = image_from_file(p, name='HO WFS SUBAPERTURE MASK')
+            subaperture_mask = image_from_fits_file(p, name='HO WFS SUBAPERTURE MASK')
         n_valid_subapertures = np.count_nonzero(subaperture_mask.data != -1)
 
         reference = self._stack_slopes(fits.getdata(self._path / 'HOAcq.DET1.REFSLP_WITH_OFFSETS.fits'),
                                        slope_axis=1)[0]
         ho_wfs = aotpy.ShackHartmann(
             uid='HO WFS',
             source=ngs,
@@ -323,17 +323,17 @@
             mask_offsets=[aotpy.Coordinates(0, 0)],
             subaperture_intensities=aotpy.Image('Intensities', ho_loop_frame['Intensities'])
         )
         self.system.wavefront_sensors.append(ho_wfs)
 
         ho_wfs.detector = aotpy.Detector(
             uid='DET1',
-            dark=image_from_file(self._path / 'HOAcq.DET1.DARK.fits'),
-            weight_map=image_from_file(self._path / 'HOAcq.DET1.WEIGHT.fits'),
-            sky_background=image_from_file(self._path / 'HOAcq.DET1.BACKGROUND.fits'),
+            dark=self._image_from_eso_file(self._path / 'HOAcq.DET1.DARK.fits'),
+            weight_map=self._image_from_eso_file(self._path / 'HOAcq.DET1.WEIGHT.fits'),
+            sky_background=self._image_from_eso_file(self._path / 'HOAcq.DET1.BACKGROUND.fits'),
             pixel_intensities=aotpy.Image(name='HO Pixels',
                                           data=self._get_pixel_data_from_table(ho_pix_frame),
                                           time=aotpy.Time('HO Pixel Time',
                                                           frame_numbers=ho_pix_frame['FrameCounter'].tolist()))
         )
         ho_wfs.subaperture_size = \
             ho_wfs.detector.pixel_intensities.data.shape[0] // ho_wfs.subaperture_mask.data.shape[0]
@@ -349,16 +349,16 @@
             ref_commands=aotpy.Image('HOCtr.ACT_POS_REF_MAP_WITH_OFFSETS',
                                      fits.getdata(self._path / 'HOCtr.ACT_POS_REF_MAP_WITH_OFFSETS.fits')[:, 0]),
             time=ho_time,
             framerate=fits.getheader(self._path / 'HODet.CFG.DYNAMIC.fits')['FREQ'],
             time_filter_num=aotpy.Image('HOCtr.A_TERMS', fits.getdata(self._path / 'HOCtr.A_TERMS.fits').T),
             time_filter_den=aotpy.Image('HOCtr.B_TERMS', fits.getdata(self._path / 'HOCtr.B_TERMS.fits').T),
             measurements_to_modes=aotpy.Image('CLMatrixOptimiser.S2M', s2m),
-            modes_to_commands=image_from_file(self._path / 'CLMatrixOptimiser.M2V.fits'),
-            commands_to_modes=image_from_file(self._path / 'CLMatrixOptimiser.V2M.fits'),
+            modes_to_commands=self._image_from_eso_file(self._path / 'CLMatrixOptimiser.M2V.fits'),
+            commands_to_modes=self._image_from_eso_file(self._path / 'CLMatrixOptimiser.V2M.fits'),
             modes_to_measurements=aotpy.Image('CLMatrixOptimiser.M2S', m2s),
         ))
 
     def _get_eso_telescope_name(self) -> str:
         return 'ESO-VLT-U4'
 
     def _get_eso_ao_name(self) -> str:
```

### Comparing `aotpy-0.8.2/aotpy/translators/eso.py` & `aotpy-1.0.0/aotpy/translators/eso.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 It also provides tools that enable users to automatically add the necessary metadata for compatibility with ESO's
 science archive. This is done by querying the archive via programmatic access (pyvo is necessary for this
 functionality).
 
 """
 
+import os
 import warnings
 from abc import abstractmethod
 from datetime import timedelta, datetime, timezone
 
 import astropy.table
 import numpy as np
 from astropy.io import fits
@@ -94,15 +95,15 @@
         Get the run ID (prog ID) that refers to the data, as defined by ESO.
         """
         pass
 
     @abstractmethod
     def _get_chip_id(self) -> str:
         """
-        Get HIERARCH ESO DET CHIP1 ID for the specific data. This is an ESO archive requirement to ensure compatibility
+        Get ESO DET CHIP1 ID for the specific data. This is an ESO archive requirement to ensure compatibility
         when there are simultaneous recordings of the same instrument on different telescopes.
         """
         pass
 
     def add_archive_metadata(self, query_archive: bool = False) -> None:
         """
         Adds necessary metadata for ESO Archive to AOSystem.
@@ -114,31 +115,31 @@
         """
         telescope = self._get_eso_telescope_name()
         metadata = {
             'ORIGIN': 'ESO-PARANAL',
             'DATE': datetime.now().isoformat(timespec='milliseconds'),
             'TELESCOP': telescope.replace('%', ''),
             'INSTRUME': self._get_eso_ao_name(),
-            'HIERARCH ESO DET CHIP1 ID': self._get_chip_id(),
-            'HIERARCH ESO OBS PROG ID': self._get_run_id(),
+            'ESO DET CHIP1 ID': self._get_chip_id(),
+            'ESO OBS PROG ID': self._get_run_id(),
             'OBJECT': 'AO-TELEM',
             'OBSERVER': 'I, Condor',
             'DATE-OBS': self.system.date_beginning.astimezone(timezone.utc).replace(tzinfo=None).isoformat(
                 timespec='milliseconds'),
             'MJD-OBS': Time(self.system.date_beginning, scale='utc').mjd,
             'MJD-END': Time(self.system.date_end, scale='utc').mjd,
             'EXPTIME': (self.system.date_end - self.system.date_beginning).total_seconds(),
-            'HIERARCH ESO DPR CATG': 'CALIB',
-            'HIERARCH ESO DPR TYPE': f'AO-TELEM,AOT,{self._get_eso_ao_name()}',
-            'HIERARCH ESO DPR TECH': self.system.ao_mode,
+            'ESO DPR CATG': 'CALIB',
+            'ESO DPR TYPE': f'AO-TELEM,AOT,{self._get_eso_ao_name()}',
+            'ESO DPR TECH': self.system.ao_mode,
         }
         if self.system.main_telescope.azimuth is not None:
-            metadata['HIERARCH ESO TEL AZ'] = self.system.main_telescope.azimuth
+            metadata['ESO TEL AZ'] = self.system.main_telescope.azimuth
         if self.system.main_telescope.elevation is not None:
-            metadata['HIERARCH ESO TEL ALT'] = self.system.main_telescope.elevation
+            metadata['ESO TEL ALT'] = self.system.main_telescope.elevation
 
         if query_archive:
             if tap is None:
                 raise ImportError("Querying the ESO archive requires the pyvo module."
                                   "You can set the 'query_archive' option to False to skip querying the archive.")
             beg = Time(self.system.date_beginning, scale='utc')
 
@@ -161,21 +162,21 @@
                 res = res[0]
                 metadata |= {
                     'INSTRUME': res['instrument'],
                     'RA': res['ra'],
                     'DEC': res['dec'],
                     # 'PI-COI': res['pi_coi'],
                     # we do not store PI-COI because it is not needed and can cause issues with special chars
-                    'HIERARCH ESO OBS PROG ID': res['prog_id'],
-                    'HIERARCH ESO INS MODE': res['ins_mode'],
+                    'ESO OBS PROG ID': res['prog_id'],
+                    'ESO INS MODE': res['ins_mode'],
                 }
-                if 'HIERARCH ESO TEL AZ' not in metadata:
-                    metadata['HIERARCH ESO TEL AZ'] = res['tel_az']
-                if 'HIERARCH ESO TEL ALT' not in metadata:
-                    metadata['HIERARCH ESO TEL ALT'] = res['tel_alt']
+                if 'ESO TEL AZ' not in metadata:
+                    metadata['ESO TEL AZ'] = res['tel_az']
+                if 'ESO TEL ALT' not in metadata:
+                    metadata['ESO TEL ALT'] = res['tel_alt']
             else:
                 warnings.warn(f"Could not find data from telescope '{telescope}' near mjd_obs {beg.mjd} at the "
                               f"ESO Archive")
         self.system.metadata.extend([aotpy.Metadatum(k, v) for k, v in metadata.items()])
 
     def get_atmospheric_parameters_from_archive(self) -> astropy.table.Table:
         """
@@ -243,7 +244,22 @@
             tilt = data[1::2]
         elif slope_axis == 1:
             tip = data[:, ::2]
             tilt = data[:, 1::2]
         else:
             raise NotImplementedError
         return np.stack([tip, tilt], axis=1)
+
+    @staticmethod
+    def _fix_pointing_format(time: float):
+        # TODO test this and add to translators
+        # Old ESO pointing data was stored using a pseudo-float format such that e.g. 100526.90157 -> +10h 05m 26.90157s
+        # This function converts from this format into decimal degrees
+        t = str(time)
+        return int(t[:2]) + int(t[2:4]) / 60 + float(t[4:]) / 3600
+
+    @staticmethod
+    def _image_from_eso_file(filename: str | os.PathLike) -> aotpy.Image:
+        image = aotpy.image_from_fits_file(filename)
+        image.metadata = [md for md in image.metadata if not md.key.startswith("ESO DPR") and md.key != 'ORIGIN' and
+                          md.key != 'RA' and md.key != 'DEC']
+        return image
```

### Comparing `aotpy-0.8.2/aotpy/translators/galacsi.py` & `aotpy-1.0.0/aotpy/translators/galacsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
-from aotpy.io import image_from_file
+from aotpy.io import image_from_fits_file
 from .eso import ESOTranslator
 
 
 # TODO set image units
 
 
 class GALACSITranslator(ESOTranslator):
@@ -59,21 +59,21 @@
         lgs_timestamps = lgs_loop_frame['Seconds'] + lgs_loop_frame['USeconds'] / 1.e6
         self.system.date_beginning = datetime.utcfromtimestamp(lgs_timestamps[0])
         self.system.date_end = datetime.utcfromtimestamp(lgs_timestamps[-1])
         lgs_frame_numbers = lgs_loop_frame['FrameCounter']
         lgs_time = aotpy.Time('LGS Loop Time', timestamps=lgs_timestamps.tolist(),
                               frame_numbers=lgs_frame_numbers.tolist())
 
-        aof_data_path = importlib.resources.files('aotpy.data') / 'GALACSI'
-        with importlib.resources.as_file(aof_data_path / 'subap.fits') as p:
-            subaperture_mask = image_from_file(p)
+        galacsi_data_path = importlib.resources.files('aotpy.data') / 'GALACSI'
+        with importlib.resources.as_file(galacsi_data_path / 'subap.fits') as p:
+            subaperture_mask = image_from_fits_file(p, name='LGS WFS SUBAPERTURE MASK')
         n_valid_subapertures = np.count_nonzero(subaperture_mask.data != -1)
 
         dsm_positions = aotpy.Image('DSM_positions', lgs_loop_frame['DSM_Positions'][:, self.dsm_valid])
-        m2c = image_from_file(path_lgs / 'LGSCtr.ACT_POS_MODAL_PROJECTION.fits')
+        m2c = self._image_from_eso_file(path_lgs / 'LGSCtr.ACT_POS_MODAL_PROJECTION.fits')
         lgs_tfz_num = aotpy.Image('LGSCtr.A_TERMS', fits.getdata(path_lgs / 'LGSCtr.A_TERMS.fits').T)
         lgs_tfz_den = aotpy.Image('LGSCtr.B_TERMS', fits.getdata(path_lgs / 'LGSCtr.B_TERMS.fits').T)
         jit_tfz_num = fits.getdata(path_lgs / 'JitCtr.A_TERMS.fits').T
         jit_tfz_den = fits.getdata(path_lgs / 'JitCtr.B_TERMS.fits').T
         jit_ref = fits.getdata(path_lgs / 'JitCtr.ACT_POS_REF_MAP_WITH_OFFSETS.fits')[:, 0]
         off_ref = fits.getdata(path_lgs / 'JitCtr.OACT_POS_REF_MAP.fits')[0, :]
         proj_map = fits.getdata(path_lgs / f'JitCtr.PROJ_MAP_SCALED.fits')
@@ -94,16 +94,16 @@
                 ref_measurements=aotpy.Image(f'LGSAcq.DET{i}.REFSLP_WITH_OFFSETS', reference),
                 subaperture_mask=subaperture_mask,
                 subaperture_intensities=aotpy.Image(f'WFS{i}_Intensities', lgs_loop_frame[f'WFS{i}_Intensities'])
             )
 
             wfs.detector = aotpy.Detector(
                 uid=f'LGS DET{i}',
-                dark=image_from_file(path_lgs / f'LGSAcq.DET{i}.DARK.fits'),
-                weight_map=image_from_file(path_lgs / f'LGSAcq.DET{i}.WEIGHT.fits')
+                dark=self._image_from_eso_file(path_lgs / f'LGSAcq.DET{i}.DARK.fits'),
+                weight_map=self._image_from_eso_file(path_lgs / f'LGSAcq.DET{i}.WEIGHT.fits')
             )
             self.system.wavefront_sensors.append(wfs)
 
             cm = self._stack_slopes(fits.getdata(path_lgs / f'LGSRecn.REC{i}.HOCM.fits')[self.dsm_valid], slope_axis=1)
             im = self._stack_slopes(im_list[i - 1], slope_axis=0)
             self.system.loops.append(aotpy.ControlLoop(
                 uid=f'High-order loop {i}',
@@ -174,17 +174,17 @@
         self.system.sources.append(ngs)
 
         gradients = self._stack_slopes(ir_loop_frame['WFS_Gradients'], slope_axis=1)
         reference = self._stack_slopes(fits.getdata(path_ir / 'IRAcq.DET1.REFSLP_WITH_OFFSETS.fits'), slope_axis=1)[0]
         ngs_wfs = aotpy.ShackHartmann(
             uid='NGS WFS1',
             n_valid_subapertures=4,  # All subapertures are valid
-            subaperture_mask=aotpy.Image('NGS_WFS_SUBAPERTURE_MASK', np.array([[1, 3], [2, 4]])),
+            subaperture_mask=aotpy.Image('NGS WFS SUBAPERTURE MASK', np.array([[1, 3], [2, 4]])),
             source=ngs,
-            measurements=aotpy.Image('NGS_WFS_Gradients', gradients),
+            measurements=aotpy.Image('NGS WFS_Gradients', gradients),
             ref_measurements=aotpy.Image('IRAcq.DET1.REFSLP_WITH_OFFSETS', reference),
             subaperture_intensities=aotpy.Image('WFS_Intensities', ir_loop_frame['WFS_Intensities'])
         )
         self.system.wavefront_sensors.append(ngs_wfs)
 
         # Find the indexes where the counter for pixels matches the counter for ngs
         # Assumes the frames for pixel are contained in the frames for ngs
@@ -201,16 +201,16 @@
             pix_timestamps_list = pix_timestamps.tolist()
 
         pix_time = aotpy.Time('Pixel Time', timestamps=pix_timestamps_list,
                               frame_numbers=ho_frame_numbers[pix_time_mask].tolist())
 
         ngs_wfs.detector = aotpy.Detector(
             uid='NGS DET1',
-            dark=image_from_file(path_ir / 'IRAcq.DET1.DARK.fits'),
-            weight_map=image_from_file(path_ir / 'IRAcq.DET1.WEIGHT.fits'),
+            dark=self._image_from_eso_file(path_ir / 'IRAcq.DET1.DARK.fits'),
+            weight_map=self._image_from_eso_file(path_ir / 'IRAcq.DET1.WEIGHT.fits'),
             pixel_intensities=aotpy.Image(name='NGS Pixels',
                                           data=self._get_pixel_data_from_table(pix_loop_frame),
                                           time=pix_time)
         )
 
         s2m = self._stack_slopes(fits.getdata(path_ir / 'IRCtr.SENSOR_2_MODES.fits'), slope_axis=1)
         m2c = fits.getdata(path_ir / 'IRCtr.MODES_2_ACT.fits')[self.dsm_valid]
```

### Comparing `aotpy-0.8.2/aotpy/translators/naomi.py` & `aotpy-1.0.0/aotpy/translators/naomi.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 from astropy.io import fits
 
 import aotpy
-from aotpy.io import image_from_file
 from .eso import ESOTranslator
 
 
 # TODO set image units
 
 
 class NAOMITranslator(ESOTranslator):
@@ -75,24 +74,24 @@
             ref_measurements=aotpy.Image('Acq.DET1.REFSLP_WITH_OFFSETS', reference),
             subaperture_intensities=aotpy.Image(f'Intensities', main_loop_frame['Intensities'], time=loop_time)
         )
 
         wfs.non_common_path_aberration = aotpy.Aberration(
             uid='NCPA',
             modes=control_modes,
-            coefficients=image_from_file(path / 'Ctr.MODAL_OFFSETS_ROTATED_0001.fits')  # in DM modal space
+            coefficients=self._image_from_eso_file(path / 'Ctr.MODAL_OFFSETS_ROTATED_0001.fits')  # in DM modal space
         )
 
         wfs.detector = aotpy.Detector(
             uid='DET',
-            weight_map=image_from_file(path / 'Acq.DET1.WEIGHT_0001.fits'),
-            dark=image_from_file(path / 'Acq.DET1.DARK_0001.fits'),
-            flat_field=image_from_file(path / 'Acq.DET1.FLAT_0001.fits'),
-            bad_pixel_map=image_from_file(path / 'Acq.DET1.DEAD_0001.fits'),
-            sky_background=image_from_file(path / 'Acq.DET1.BACKGROUND_0001.fits')
+            weight_map=self._image_from_eso_file(path / 'Acq.DET1.WEIGHT_0001.fits'),
+            dark=self._image_from_eso_file(path / 'Acq.DET1.DARK_0001.fits'),
+            flat_field=self._image_from_eso_file(path / 'Acq.DET1.FLAT_0001.fits'),
+            bad_pixel_map=self._image_from_eso_file(path / 'Acq.DET1.DEAD_0001.fits'),
+            sky_background=self._image_from_eso_file(path / 'Acq.DET1.BACKGROUND_0001.fits')
         )
 
         pix_loop_frame = fits.getdata(path / 'NAOMI_PIXELS_0001.fits')
         wfs.detector.pixel_intensities = aotpy.Image(
             'Pixels',
             data=self._get_pixel_data_from_table(pix_loop_frame),
             time=aotpy.Time('Pixel time', frame_numbers=pix_loop_frame['FrameCounter'].tolist())
@@ -122,16 +121,16 @@
             time_filter_num=aotpy.Image('Ctr.TERM_A', fits.getdata(path / 'Ctr.TERM_A_0001.fits')),
             time_filter_den=aotpy.Image('Ctr.TERM_B', fits.getdata(path / 'Ctr.TERM_B_0001.fits')),
             commands=aotpy.Image('DM positions', main_loop_frame['Positions'], time=loop_time),
             ref_commands=ref_commands,
             modes=control_modes,
             modal_coefficients=aotpy.Image('Modal Coefficients', modal_coefficients, time=loop_time),
             measurements_to_modes=aotpy.Image('Recn.REC1.CM', s2m),
-            modes_to_commands=image_from_file(path / 'RTC.M2DM_SCALED_0001.fits'),
-            commands_to_modes=image_from_file(path / 'RTC.DM2M_SCALED_0001.fits'),
+            modes_to_commands=self._image_from_eso_file(path / 'RTC.M2DM_SCALED_0001.fits'),
+            commands_to_modes=self._image_from_eso_file(path / 'RTC.DM2M_SCALED_0001.fits'),
             modes_to_measurements=aotpy.Image('ModalRecnCalibrat.REF_IM', m2s),
             closed=main_hdr['ESO AOS LOOP ST'],
             framerate=main_hdr['ESO AOS LOOP RATE']
         )
 
         asm = aotpy.AtmosphericParameters(
             'ESO ASM (Astronomical Site Monitor)',
```

### Comparing `aotpy-0.8.2/aotpy/translators/papyrus.py` & `aotpy-1.0.0/aotpy/translators/papyrus.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 This module contains a class for translating telemetry data produced by the ALPAO RTC, part of the PAPYRUS system. 
 It assumes the MATLAB files produced by ALPAO RTC have been converted to use struct objects instead of classes. 
 The custom MATLAB function makeTelemetryFileReadable is made for this.
 Note that the use of scipy.io.loadmat to read the .mat files in python suppose that these .mat files were 
 saved with the version -v7 of matlab or anterior. scipy.io.loadmat does not work for files saved with matlab -v7.3.
 """
 
+import datetime
 import importlib.resources
 
-import datetime
 import numpy as np
 
 import aotpy
-from aotpy.io import image_from_file
+from aotpy.io import image_from_fits_file
 from .base import BaseTranslator
 
 try:
     from scipy.io import loadmat
 except (ImportError, ModuleNotFoundError):
     loadmat = None
 
@@ -29,15 +29,15 @@
 
         # common fields between SH and PYWFS telemetry
 
         self.system = aotpy.AOSystem(ao_mode='SCAO', name='PAPYRUS')
 
         papyrus_data_path = importlib.resources.files('aotpy.data') / 'PAPYRUS'
         with importlib.resources.as_file(papyrus_data_path / 'T152_pupil.fits') as p:
-            pupil_mask = image_from_file(p, name='T152 PUPIL')
+            pupil_mask = image_from_fits_file(p, name='T152 PUPIL')
 
         self.system.main_telescope = aotpy.MainTelescope(
             uid="T152",
             enclosing_diameter=1.5,
             inscribed_diameter=1.5,
             pupil_mask=pupil_mask)
```

### Comparing `aotpy-0.8.2/aotpy.egg-info/PKG-INFO` & `aotpy-1.0.0/aotpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.8.2
+Version: 1.0.0
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.8.2/aotpy.egg-info/SOURCES.txt` & `aotpy-1.0.0/aotpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.2/setup.cfg` & `aotpy-1.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6f74 7079 0d0a 7665 7273 696f   = aotpy..versio
-00000020: 6e20 3d20 302e 382e 320d 0a61 7574 686f  n = 0.8.2..autho
+00000020: 6e20 3d20 312e 302e 300d 0a61 7574 686f  n = 1.0.0..autho
 00000030: 7220 3d20 5469 6167 6f20 476f 6d65 730d  r = Tiago Gomes.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7469 6167 6f67 6f6d 6573 4066 652e 7570  tiagogomes@fe.up
 00000060: 2e70 740d 0a64 6573 6372 6970 7469 6f6e  .pt..description
 00000070: 203d 2048 656c 7065 7220 7061 636b 6167   = Helper packag
 00000080: 6520 666f 7220 6861 6e64 6c69 6e67 2041  e for handling A
 00000090: 6461 7074 6976 6520 4f70 7469 6373 2054  daptive Optics T
```

