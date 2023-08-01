# Comparing `tmp/libquantum-1.5.3.tar.gz` & `tmp/libquantum-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libquantum-1.5.3.tar", last modified: Tue Aug  1 19:08:03 2023, max compression
+gzip compressed data, was "libquantum-1.5.4.tar", last modified: Tue Aug  1 19:48:25 2023, max compression
```

## Comparing `libquantum-1.5.3.tar` & `libquantum-1.5.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:08:03.909389 libquantum-1.5.3/
--rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.3/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-08-01 19:08:03.909389 libquantum-1.5.3/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     2989 2023-04-28 19:47:14.000000 libquantum-1.5.3/README.md
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:08:03.907389 libquantum-1.5.3/libquantum/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.3/libquantum/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    22119 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/atoms.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/atoms_inverse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/blast_pulse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/doppler.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3104 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/dyadics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/entropy.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/export.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4322 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/gabor_box.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:08:03.908389 libquantum-1.5.3/libquantum/plot_templates/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.3/libquantum/plot_templates/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/plot_templates/plot_time_frequency_picks.py
--rw-r--r--   0 opq       (1000) opq       (1000)    41024 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/plot_templates/plot_time_frequency_reps.py
--rw-r--r--   0 opq       (1000) opq       (1000)    42082 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/plot_templates/plot_time_frequency_reps_black.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4092 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/rms_envelope.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/scales.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.3/libquantum/spectra.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10324 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/stockwell_orig.py
--rw-r--r--   0 opq       (1000) opq       (1000)    33732 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/styx_cwt.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19514 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/styx_fft.py
--rw-r--r--   0 opq       (1000) opq       (1000)    11380 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/styx_stx.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8438 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/styx_stx_loopy.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14611 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/synthetics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.3/libquantum/tfr_gate_pick.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19522 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum/utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:08:03.908389 libquantum-1.5.3/libquantum.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-08-01 19:08:03.000000 libquantum-1.5.3/libquantum.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     1039 2023-08-01 19:08:03.000000 libquantum-1.5.3/libquantum.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-08-01 19:08:03.000000 libquantum-1.5.3/libquantum.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      104 2023-08-01 19:08:03.000000 libquantum-1.5.3/libquantum.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       23 2023-08-01 19:08:03.000000 libquantum-1.5.3/libquantum.egg-info/top_level.txt
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:08:03.909389 libquantum-1.5.3/libquantum2/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum2/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15727 2023-04-28 19:47:14.000000 libquantum-1.5.3/libquantum2/benchmark_signals.py
--rw-r--r--   0 opq       (1000) opq       (1000)      864 2023-08-01 19:06:22.000000 libquantum-1.5.3/pyproject.toml
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-08-01 19:08:03.909389 libquantum-1.5.3/setup.cfg
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:08:03.909389 libquantum-1.5.3/tests/
--rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.3/tests/test_quantum.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.3/tests/test_spectra.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.112970 libquantum-1.5.4/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.4/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-08-01 19:48:25.112970 libquantum-1.5.4/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     2989 2023-04-28 19:47:14.000000 libquantum-1.5.4/README.md
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.110970 libquantum-1.5.4/libquantum/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.4/libquantum/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    22119 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/atoms.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/atoms_inverse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/blast_pulse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/doppler.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3104 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/dyadics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/entropy.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/export.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4322 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/gabor_box.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.111970 libquantum-1.5.4/libquantum/plot_templates/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.4/libquantum/plot_templates/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_picks.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    41024 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_reps.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    42082 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_reps_black.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4092 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/rms_envelope.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/scales.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.4/libquantum/spectra.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    10324 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/stockwell_orig.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    33732 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/styx_cwt.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19514 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/styx_fft.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    11380 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/styx_stx.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     8438 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/styx_stx_loopy.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14611 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/synthetics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/tfr_gate_pick.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19522 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/utils.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.111970 libquantum-1.5.4/libquantum.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     1039 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      110 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       23 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/top_level.txt
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.111970 libquantum-1.5.4/libquantum2/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum2/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    15727 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum2/benchmark_signals.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      892 2023-08-01 19:47:39.000000 libquantum-1.5.4/pyproject.toml
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-08-01 19:48:25.112970 libquantum-1.5.4/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.112970 libquantum-1.5.4/tests/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.4/tests/test_quantum.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.4/tests/test_spectra.py
```

### Comparing `libquantum-1.5.3/LICENSE` & `libquantum-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/PKG-INFO` & `libquantum-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.3
+Version: 1.5.4
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libquantum-1.5.3/README.md` & `libquantum-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/atoms.py` & `libquantum-1.5.4/libquantum/atoms.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/atoms_inverse.py` & `libquantum-1.5.4/libquantum/atoms_inverse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/blast_pulse.py` & `libquantum-1.5.4/libquantum/blast_pulse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/doppler.py` & `libquantum-1.5.4/libquantum/doppler.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/dyadics.py` & `libquantum-1.5.4/libquantum/dyadics.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/entropy.py` & `libquantum-1.5.4/libquantum/entropy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/export.py` & `libquantum-1.5.4/libquantum/export.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/gabor_box.py` & `libquantum-1.5.4/libquantum/gabor_box.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/plot_templates/plot_geo_scatter_2d_3d.py` & `libquantum-1.5.4/libquantum/plot_templates/plot_geo_scatter_2d_3d.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/plot_templates/plot_time_frequency_picks.py` & `libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_picks.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/plot_templates/plot_time_frequency_reps.py` & `libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_reps.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/plot_templates/plot_time_frequency_reps_black.py` & `libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_reps_black.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/rms_envelope.py` & `libquantum-1.5.4/libquantum/rms_envelope.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/scales.py` & `libquantum-1.5.4/libquantum/scales.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/spectra.py` & `libquantum-1.5.4/libquantum/spectra.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/stockwell_orig.py` & `libquantum-1.5.4/libquantum/stockwell_orig.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/styx_cwt.py` & `libquantum-1.5.4/libquantum/styx_cwt.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/styx_fft.py` & `libquantum-1.5.4/libquantum/styx_fft.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/styx_stx.py` & `libquantum-1.5.4/libquantum/styx_stx.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/styx_stx_loopy.py` & `libquantum-1.5.4/libquantum/styx_stx_loopy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/synthetics.py` & `libquantum-1.5.4/libquantum/synthetics.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/tfr_gate_pick.py` & `libquantum-1.5.4/libquantum/tfr_gate_pick.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum/utils.py` & `libquantum-1.5.4/libquantum/utils.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum.egg-info/PKG-INFO` & `libquantum-1.5.4/libquantum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.3
+Version: 1.5.4
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libquantum-1.5.3/libquantum.egg-info/SOURCES.txt` & `libquantum-1.5.4/libquantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/libquantum2/benchmark_signals.py` & `libquantum-1.5.4/libquantum2/benchmark_signals.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.3/tests/test_spectra.py` & `libquantum-1.5.4/tests/test_spectra.py`

 * *Files identical despite different names*

