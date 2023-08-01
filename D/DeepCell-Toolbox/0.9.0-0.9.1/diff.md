# Comparing `tmp/Deepcell_Toolbox-0.9.0.tar.gz` & `tmp/Deepcell_Toolbox-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Deepcell_Toolbox-0.9.0.tar", last modified: Tue Mar  2 20:34:48 2021, max compression
+gzip compressed data, was "Deepcell_Toolbox-0.9.1.tar", last modified: Wed Jun  2 20:14:08 2021, max compression
```

## Comparing `Deepcell_Toolbox-0.9.0.tar` & `Deepcell_Toolbox-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 20:34:48.564785 Deepcell_Toolbox-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 20:34:48.560785 Deepcell_Toolbox-0.9.0/Deepcell_Toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2021-03-02 20:34:47.000000 Deepcell_Toolbox-0.9.0/Deepcell_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-02 20:34:48.000000 Deepcell_Toolbox-0.9.0/Deepcell_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-02 20:34:47.000000 Deepcell_Toolbox-0.9.0/Deepcell_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-03-02 20:34:47.000000 Deepcell_Toolbox-0.9.0/Deepcell_Toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-03-02 20:34:47.000000 Deepcell_Toolbox-0.9.0/Deepcell_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2021-03-02 20:34:48.564785 Deepcell_Toolbox-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      897 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 20:34:48.560785 Deepcell_Toolbox-0.9.0/deepcell_toolbox/
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/compute_overlap.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/compute_overlap_3D.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    11472 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/deep_watershed.py
--rw-r--r--   0 runner    (1001) docker     (121)     5195 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/deep_watershed_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    49422 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    29795 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11126 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/processing_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    29463 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    15985 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/deepcell_toolbox/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-02 20:34:48.564785 Deepcell_Toolbox-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4627 2021-03-02 20:34:40.000000 Deepcell_Toolbox-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 20:14:08.934091 Deepcell_Toolbox-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 20:14:08.934091 Deepcell_Toolbox-0.9.1/Deepcell_Toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1725 2021-06-02 20:14:08.000000 Deepcell_Toolbox-0.9.1/Deepcell_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-06-02 20:14:08.000000 Deepcell_Toolbox-0.9.1/Deepcell_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-02 20:14:08.000000 Deepcell_Toolbox-0.9.1/Deepcell_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2021-06-02 20:14:08.000000 Deepcell_Toolbox-0.9.1/Deepcell_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-06-02 20:14:08.000000 Deepcell_Toolbox-0.9.1/Deepcell_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11691 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1725 2021-06-02 20:14:08.934091 Deepcell_Toolbox-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 20:14:08.934091 Deepcell_Toolbox-0.9.1/deepcell_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1672 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1677 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/compute_overlap.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     2089 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/compute_overlap_3D.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)    11472 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/deep_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5195 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/deep_watershed_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49584 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29961 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11126 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/processing_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29613 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15985 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/deepcell_toolbox/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-02 20:14:08.934091 Deepcell_Toolbox-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4627 2021-06-02 20:14:03.000000 Deepcell_Toolbox-0.9.1/setup.py
```

### Comparing `Deepcell_Toolbox-0.9.0/Deepcell_Toolbox.egg-info/PKG-INFO` & `Deepcell_Toolbox-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: Deepcell-Toolbox
-Version: 0.9.0
+Name: Deepcell_Toolbox
+Version: 0.9.1
 Summary: The pre- and post-processing functions module for deepcell-tf.
 Home-page: https://github.com/vanvalenlab/deepcell-toolbox
 Author: Van Valen Lab
 Author-email: vanvalenlab@gmail.com
 License: LICENSE
-Download-URL: https://github.com/vanvalenlab/deepcell-toolbox/tarball/0.9.0
+Download-URL: https://github.com/vanvalenlab/deepcell-toolbox/tarball/0.9.1
 Description: # ![DeepCell Toolbox Banner](https://raw.githubusercontent.com/vanvalenlab/deepcell-toolbox/master/docs/images/DeepCell_toolbox_Banner.png)
         
         [![Build Status](https://github.com/vanvalenlab/deepcell-toolbox/workflows/build/badge.svg)](https://github.com/vanvalenlab/deepcell-toolbox/actions)
         [![Coverage Status](https://coveralls.io/repos/github/vanvalenlab/deepcell-toolbox/badge.svg?branch=master)](https://coveralls.io/github/vanvalenlab/deepcell-toolbox?branch=master)
         [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](/LICENSE)
         [![PyPI version](https://badge.fury.io/py/Deepcell-Toolbox.svg)](https://badge.fury.io/py/deepcell-toolbox)
         [![Python Versions](https://img.shields.io/pypi/pyversions/deepcell_toolbox.svg)](https://pypi.org/project/deepcell_toolbox/)
```

### Comparing `Deepcell_Toolbox-0.9.0/Deepcell_Toolbox.egg-info/SOURCES.txt` & `Deepcell_Toolbox-0.9.1/Deepcell_Toolbox.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 Deepcell_Toolbox.egg-info/PKG-INFO
 Deepcell_Toolbox.egg-info/SOURCES.txt
 Deepcell_Toolbox.egg-info/dependency_links.txt
 Deepcell_Toolbox.egg-info/requires.txt
```

### Comparing `Deepcell_Toolbox-0.9.0/PKG-INFO` & `Deepcell_Toolbox-0.9.1/Deepcell_Toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: Deepcell_Toolbox
-Version: 0.9.0
+Name: Deepcell-Toolbox
+Version: 0.9.1
 Summary: The pre- and post-processing functions module for deepcell-tf.
 Home-page: https://github.com/vanvalenlab/deepcell-toolbox
 Author: Van Valen Lab
 Author-email: vanvalenlab@gmail.com
 License: LICENSE
-Download-URL: https://github.com/vanvalenlab/deepcell-toolbox/tarball/0.9.0
+Download-URL: https://github.com/vanvalenlab/deepcell-toolbox/tarball/0.9.1
 Description: # ![DeepCell Toolbox Banner](https://raw.githubusercontent.com/vanvalenlab/deepcell-toolbox/master/docs/images/DeepCell_toolbox_Banner.png)
         
         [![Build Status](https://github.com/vanvalenlab/deepcell-toolbox/workflows/build/badge.svg)](https://github.com/vanvalenlab/deepcell-toolbox/actions)
         [![Coverage Status](https://coveralls.io/repos/github/vanvalenlab/deepcell-toolbox/badge.svg?branch=master)](https://coveralls.io/github/vanvalenlab/deepcell-toolbox?branch=master)
         [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](/LICENSE)
         [![PyPI version](https://badge.fury.io/py/Deepcell-Toolbox.svg)](https://badge.fury.io/py/deepcell-toolbox)
         [![Python Versions](https://img.shields.io/pypi/pyversions/deepcell_toolbox.svg)](https://pypi.org/project/deepcell_toolbox/)
```

### Comparing `Deepcell_Toolbox-0.9.0/README.md` & `Deepcell_Toolbox-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/__init__.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/__version__.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 # limitations under the License.
 # ============================================================================
 
 __title__ = 'Deepcell_Toolbox'
 __description__ = 'The pre- and post-processing functions module for ' \
     'deepcell-tf.'
 __url__ = 'https://github.com/vanvalenlab/deepcell-toolbox'
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 __author__ = 'Van Valen Lab'
 __author_email__ = 'vanvalenlab@gmail.com'
 __license__ = 'LICENSE'
 __copyright__ = 'Copyright 2016-2021 The Van Valen Lab at the ' \
     'California Institute of Technology (Caltech)'
```

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/compute_overlap.pyx` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/compute_overlap.pyx`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/compute_overlap_3D.pyx` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/compute_overlap_3D.pyx`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/deep_watershed.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/deep_watershed.py`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/deep_watershed_test.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/deep_watershed_test.py`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/metrics.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,17 +595,24 @@
 
     def save_to_dataframe(self):
         """Save error results to a pandas dataframe
 
         Returns:
             pandas.DataFrame: Single row dataframe with error types as columns
         """
+        try:
+            self.precision = self.correct_detections / self.n_pred
+        except ZeroDivisionError:
+            self.precision = 0
+
+        try:
+            self.recall = self.correct_detections / self.n_true
+        except ZeroDivisionError:
+            self.recall = 0
 
-        self.precision = self.correct_detections / self.n_pred
-        self.recall = self.correct_detections / self.n_true
         self.f1 = hmean([self.recall, self.precision])
 
         D = {
             'n_pred': self.n_pred,
             'n_true': self.n_true,
             'correct_detections': self.correct_detections,
             'missed_detections': self.missed_detections,
```

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/metrics_test.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/metrics_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,14 +364,18 @@
         before = len(m.output)
 
         m.calc_object_stats(y_true, y_pred)
 
         # Check data added to output
         assert before != len(m.output)
 
+        m.calc_object_stats(np.zeros_like(y_true), np.zeros_like(y_pred))
+        assert m.stats['precision'].sum() == 0
+        assert m.stats['recall'].sum() == 0
+
         # Raise input size error
         with testing.assert_raises(ValueError):
             m.calc_object_stats(np.random.rand(10, 10), np.random.rand(10, 10))
 
         # data that needs to be relabeled raises a warning
         with pytest.warns(UserWarning):
             y_pred[0, 0, 0] = 40
```

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/processing.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/processing.py`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/processing_test.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/processing_test.py`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/utils.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,25 +418,30 @@
     x_pad = tiles_info['pad_x']
     y_pad = tiles_info['pad_y']
 
     image_shape = [image_shape[0], image_shape[1], image_shape[2], tiles.shape[-1]]
     window_size = (tile_size_x, tile_size_y)
     image = np.zeros(image_shape, dtype=np.float)
 
+    window_cache = {}
+    for x, y in zip(overlaps_x, overlaps_y):
+        if (x, y) not in window_cache:
+            w = window_2D(window_size, overlap_x=x, overlap_y=y, power=power)
+            window_cache[(x, y)] = w
+
     for tile, batch, x_start, x_end, y_start, y_end, overlap_x, overlap_y in zip(
             tiles, batches, x_starts, x_ends, y_starts, y_ends, overlaps_x, overlaps_y):
 
         # Conditions under which to use spline interpolation
         # A tile size or stride ratio that is too small gives inconsistent results,
         # so in these cases we skip interpolation and just return the raw tiles
         if (min_tile_size <= tile_size_x < image_shape[1] and
                 min_tile_size <= tile_size_y < image_shape[2] and
                 stride_ratio >= min_stride_ratio):
-            window = window_2D(window_size, overlap_x=overlap_x,
-                               overlap_y=overlap_y, power=power)
+            window = window_cache[(overlap_x, overlap_y)]
             image[batch, x_start:x_end, y_start:y_end, :] += tile * window
         else:
             image[batch, x_start:x_end, y_start:y_end, :] = tile
 
     image = image.astype(tiles.dtype)
 
     x_start = x_pad[0]
```

### Comparing `Deepcell_Toolbox-0.9.0/deepcell_toolbox/utils_test.py` & `Deepcell_Toolbox-0.9.1/deepcell_toolbox/utils_test.py`

 * *Files identical despite different names*

### Comparing `Deepcell_Toolbox-0.9.0/setup.py` & `Deepcell_Toolbox-0.9.1/setup.py`

 * *Files identical despite different names*

