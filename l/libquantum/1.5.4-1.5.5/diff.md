# Comparing `tmp/libquantum-1.5.4.tar.gz` & `tmp/libquantum-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libquantum-1.5.4.tar", last modified: Tue Aug  1 19:48:25 2023, max compression
+gzip compressed data, was "libquantum-1.5.5.tar", last modified: Tue Aug  1 19:53:32 2023, max compression
```

## Comparing `libquantum-1.5.4.tar` & `libquantum-1.5.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.112970 libquantum-1.5.4/
--rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.4/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-08-01 19:48:25.112970 libquantum-1.5.4/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     2989 2023-04-28 19:47:14.000000 libquantum-1.5.4/README.md
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.110970 libquantum-1.5.4/libquantum/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.4/libquantum/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    22119 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/atoms.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/atoms_inverse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/blast_pulse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/doppler.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3104 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/dyadics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/entropy.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/export.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4322 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/gabor_box.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.111970 libquantum-1.5.4/libquantum/plot_templates/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.4/libquantum/plot_templates/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_picks.py
--rw-r--r--   0 opq       (1000) opq       (1000)    41024 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_reps.py
--rw-r--r--   0 opq       (1000) opq       (1000)    42082 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_reps_black.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4092 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/rms_envelope.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/scales.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.4/libquantum/spectra.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10324 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/stockwell_orig.py
--rw-r--r--   0 opq       (1000) opq       (1000)    33732 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/styx_cwt.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19514 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/styx_fft.py
--rw-r--r--   0 opq       (1000) opq       (1000)    11380 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/styx_stx.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8438 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/styx_stx_loopy.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14611 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/synthetics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.4/libquantum/tfr_gate_pick.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19522 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum/utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.111970 libquantum-1.5.4/libquantum.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     1039 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      110 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       23 2023-08-01 19:48:25.000000 libquantum-1.5.4/libquantum.egg-info/top_level.txt
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.111970 libquantum-1.5.4/libquantum2/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum2/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15727 2023-04-28 19:47:14.000000 libquantum-1.5.4/libquantum2/benchmark_signals.py
--rw-r--r--   0 opq       (1000) opq       (1000)      892 2023-08-01 19:47:39.000000 libquantum-1.5.4/pyproject.toml
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-08-01 19:48:25.112970 libquantum-1.5.4/setup.cfg
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:48:25.112970 libquantum-1.5.4/tests/
--rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.4/tests/test_quantum.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.4/tests/test_spectra.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:53:32.848486 libquantum-1.5.5/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.5/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-08-01 19:53:32.848486 libquantum-1.5.5/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     2989 2023-04-28 19:47:14.000000 libquantum-1.5.5/README.md
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:53:32.846486 libquantum-1.5.5/libquantum/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.5/libquantum/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    22119 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/atoms.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/atoms_inverse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/blast_pulse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/doppler.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3104 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/dyadics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/entropy.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/export.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4322 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/gabor_box.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:53:32.847486 libquantum-1.5.5/libquantum/plot_templates/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.5/libquantum/plot_templates/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/plot_templates/plot_time_frequency_picks.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    41024 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/plot_templates/plot_time_frequency_reps.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    42082 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/plot_templates/plot_time_frequency_reps_black.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4092 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/rms_envelope.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/scales.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.5/libquantum/spectra.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    10324 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/stockwell_orig.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    33732 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/styx_cwt.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19514 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/styx_fft.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    11380 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/styx_stx.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     8438 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/styx_stx_loopy.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14611 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/synthetics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.5/libquantum/tfr_gate_pick.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19522 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum/utils.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:53:32.847486 libquantum-1.5.5/libquantum.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-08-01 19:53:32.000000 libquantum-1.5.5/libquantum.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     1039 2023-08-01 19:53:32.000000 libquantum-1.5.5/libquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-08-01 19:53:32.000000 libquantum-1.5.5/libquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       96 2023-08-01 19:53:32.000000 libquantum-1.5.5/libquantum.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       23 2023-08-01 19:53:32.000000 libquantum-1.5.5/libquantum.egg-info/top_level.txt
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:53:32.848486 libquantum-1.5.5/libquantum2/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum2/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    15727 2023-04-28 19:47:14.000000 libquantum-1.5.5/libquantum2/benchmark_signals.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      871 2023-08-01 19:53:02.000000 libquantum-1.5.5/pyproject.toml
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-08-01 19:53:32.848486 libquantum-1.5.5/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:53:32.848486 libquantum-1.5.5/tests/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.5/tests/test_quantum.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.5/tests/test_spectra.py
```

### Comparing `libquantum-1.5.4/LICENSE` & `libquantum-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/PKG-INFO` & `libquantum-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.4
+Version: 1.5.5
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libquantum-1.5.4/README.md` & `libquantum-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/atoms.py` & `libquantum-1.5.5/libquantum/atoms.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/atoms_inverse.py` & `libquantum-1.5.5/libquantum/atoms_inverse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/blast_pulse.py` & `libquantum-1.5.5/libquantum/blast_pulse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/doppler.py` & `libquantum-1.5.5/libquantum/doppler.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/dyadics.py` & `libquantum-1.5.5/libquantum/dyadics.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/entropy.py` & `libquantum-1.5.5/libquantum/entropy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/export.py` & `libquantum-1.5.5/libquantum/export.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/gabor_box.py` & `libquantum-1.5.5/libquantum/gabor_box.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/plot_templates/plot_geo_scatter_2d_3d.py` & `libquantum-1.5.5/libquantum/plot_templates/plot_geo_scatter_2d_3d.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_picks.py` & `libquantum-1.5.5/libquantum/plot_templates/plot_time_frequency_picks.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_reps.py` & `libquantum-1.5.5/libquantum/plot_templates/plot_time_frequency_reps.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/plot_templates/plot_time_frequency_reps_black.py` & `libquantum-1.5.5/libquantum/plot_templates/plot_time_frequency_reps_black.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/rms_envelope.py` & `libquantum-1.5.5/libquantum/rms_envelope.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/scales.py` & `libquantum-1.5.5/libquantum/scales.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/spectra.py` & `libquantum-1.5.5/libquantum/spectra.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/stockwell_orig.py` & `libquantum-1.5.5/libquantum/stockwell_orig.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/styx_cwt.py` & `libquantum-1.5.5/libquantum/styx_cwt.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/styx_fft.py` & `libquantum-1.5.5/libquantum/styx_fft.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/styx_stx.py` & `libquantum-1.5.5/libquantum/styx_stx.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/styx_stx_loopy.py` & `libquantum-1.5.5/libquantum/styx_stx_loopy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/synthetics.py` & `libquantum-1.5.5/libquantum/synthetics.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/tfr_gate_pick.py` & `libquantum-1.5.5/libquantum/tfr_gate_pick.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum/utils.py` & `libquantum-1.5.5/libquantum/utils.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum.egg-info/PKG-INFO` & `libquantum-1.5.5/libquantum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.4
+Version: 1.5.5
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `libquantum-1.5.4/libquantum.egg-info/SOURCES.txt` & `libquantum-1.5.5/libquantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/libquantum2/benchmark_signals.py` & `libquantum-1.5.5/libquantum2/benchmark_signals.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.4/pyproject.toml` & `libquantum-1.5.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # See:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "libquantum"
-version = "1.5.4"
+version = "1.5.5"
 authors = [
     { name = "RedVox, Inc", email = "support@redvox.io" }
 ]
 description = "Library for implementing standardized time-frequency representations."
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file = "LICENSE" }
 
 dependencies = [
     "librosa==0.10.0.post2",
     "libwwz==1.3.1",
     "matplotlib==3.7.1",
     "numpy==1.23.5",
     "pandas==2.0.1",
-    "pandas==2.0.1",
     "redvox==3.5.2",
 ]
 
 [project.urls]
 homepage = "https://github.com/RedVoxInc/libquantum"
 PyPI = "https://pypi.org/project/libquantum/"
```

### Comparing `libquantum-1.5.4/tests/test_spectra.py` & `libquantum-1.5.5/tests/test_spectra.py`

 * *Files identical despite different names*

