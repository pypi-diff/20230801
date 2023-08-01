# Comparing `tmp/Draugr-1.0.8.tar.gz` & `tmp/Draugr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Draugr-1.0.8.tar", last modified: Thu Feb 23 07:51:52 2023, max compression
+gzip compressed data, was "Draugr-1.0.9.tar", last modified: Tue Aug  1 06:12:27 2023, max compression
```

## Comparing `Draugr-1.0.8.tar` & `Draugr-1.0.9.tar`

### file list

```diff
@@ -1,628 +1,638 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.844074 Draugr-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.768069 Draugr-1.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-02-23 07:51:44.000000 Draugr-1.0.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-23 07:51:44.000000 Draugr-1.0.8/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-23 07:51:44.000000 Draugr-1.0.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:44.000000 Draugr-1.0.8/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.768069 Draugr-1.0.8/Draugr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-02-23 07:51:52.000000 Draugr-1.0.8/Draugr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25209 2023-02-23 07:51:52.000000 Draugr-1.0.8/Draugr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 07:51:52.000000 Draugr-1.0.8/Draugr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-23 07:51:52.000000 Draugr-1.0.8/Draugr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-02-23 07:51:52.000000 Draugr-1.0.8/Draugr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-23 07:51:52.000000 Draugr-1.0.8/Draugr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 07:51:44.000000 Draugr-1.0.8/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-02-23 07:51:44.000000 Draugr-1.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-23 07:51:44.000000 Draugr-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-02-23 07:51:52.844074 Draugr-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-02-23 07:51:44.000000 Draugr-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.768069 Draugr-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-23 07:51:44.000000 Draugr-1.0.8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.772070 Draugr-1.0.8/draugr/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.772070 Draugr-1.0.8/draugr/dlib_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/dlib_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/dlib_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/dlib_utilities/dlib_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/dlib_utilities/facealigner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.772070 Draugr-1.0.8/draugr/drawers/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/drawer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.772070 Draugr-1.0.8/draugr/drawers/mpl_drawers/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/discrete_scroll_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/distribution_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/image_stream_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/mpldrawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/series_scroll_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.772070 Draugr-1.0.8/draugr/drawers/mpl_drawers/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/spectral/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/spectral/fast_fourier_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/mpl_drawers/spectral/fast_fourier_transform_spectrogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.772070 Draugr-1.0.8/draugr/drawers/opencv_drawers/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/opencv_drawers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/opencv_drawers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/opencv_drawers/opencv_image_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.776070 Draugr-1.0.8/draugr/drawers/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/terminal/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/terminal/terminal_image_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/terminal/terminal_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/terminal/terminal_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/drawers/terminal/terminal_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.776070 Draugr-1.0.8/draugr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/entry_points/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/entry_points/cpu_usage_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/entry_points/tensorboard_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/entry_points/toggle_darkmode.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/entry_points/visdom_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.776070 Draugr-1.0.8/draugr/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/extensions/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/extensions/skimage_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/extensions/sorcery_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.776070 Draugr-1.0.8/draugr/ffmpeg_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/ffmpeg_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/ffmpeg_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/ffmpeg_utilities/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/ffmpeg_utilities/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/ffmpeg_utilities/sequencify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/ffmpeg_utilities/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.776070 Draugr-1.0.8/draugr/matlab_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/matlab_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/matlab_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/matlab_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/matlab_utilities/matlab_conversion_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/matlab_utilities/singleton_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.780070 Draugr-1.0.8/draugr/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/meters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/metric_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/metric_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/metric_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.780070 Draugr-1.0.8/draugr/metrics/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/plotting/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/metrics/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.780070 Draugr-1.0.8/draugr/multiprocessing_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/multiprocessing_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/multiprocessing_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/multiprocessing_utilities/pooled_queue_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.780070 Draugr-1.0.8/draugr/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/channel_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.780070 Draugr-1.0.8/draugr/numpy_utilities/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.784070 Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/deep_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/flat_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/shallow_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/datasets/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/mixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/powers.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/raster_grid_2d_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/raster_grid_3d_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.784070 Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/signal_mixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/signal_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/signal_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/truncation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.784070 Draugr-1.0.8/draugr/opencv_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.784070 Draugr-1.0.8/draugr/opencv_utilities/bounding_boxes/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/bounding_boxes/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/bounding_boxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/bounding_boxes/boxes_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/bounding_boxes/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.784070 Draugr-1.0.8/draugr/opencv_utilities/color_space/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/gray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/color_space/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.788071 Draugr-1.0.8/draugr/opencv_utilities/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/draw_boxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.788071 Draugr-1.0.8/draugr/opencv_utilities/drawing/masks/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/masks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/masks/gauss_circles.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/masks/segment_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/opencv_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/drawing/opencv_drawing_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.788071 Draugr-1.0.8/draugr/opencv_utilities/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/namespaces/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/namespaces/color_conversion_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/namespaces/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/namespaces/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.788071 Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/async_video_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/frame_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/video_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.788071 Draugr-1.0.8/draugr/opencv_utilities/transformation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/transformation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/transformation/cropping.py
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/transformation/cv2_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/transformation/resize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.792071 Draugr-1.0.8/draugr/opencv_utilities/windows/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.792071 Draugr-1.0.8/draugr/opencv_utilities/windows/elements/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/elements/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/elements/button.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/elements/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/elements/trackbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/opencv_utilities/windows/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.792071 Draugr-1.0.8/draugr/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/cuda_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.792071 Draugr-1.0.8/draugr/os_utilities/linux_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.792071 Draugr-1.0.8/draugr/os_utilities/linux_utilities/cron_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/cron_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/cron_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.792071 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gnome_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gnome_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gnome_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gnome_utilities/dark_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.792071 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gtk_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gtk_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gtk_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gtk_utilities/gtk_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/gtk_utilities/theme_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.796071 Draugr-1.0.8/draugr/os_utilities/linux_utilities/systemd_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/systemd_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/systemd_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/systemd_utilities/service_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/systemd_utilities/service_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/linux_utilities/user_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.796071 Draugr-1.0.8/draugr/os_utilities/mac_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/mac_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/mac_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/mac_utilities/dark_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.796071 Draugr-1.0.8/draugr/os_utilities/resource_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/resource_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/resource_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/resource_utilities/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/resource_utilities/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/resource_utilities/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/resource_utilities/ram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/screen_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.796071 Draugr-1.0.8/draugr/os_utilities/windows_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.796071 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.796071 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/enums/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/enums/task_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/enums/task_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/enums/task_logon_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/enums/task_trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.800071 Draugr-1.0.8/draugr/os_utilities/windows_utilities/win32/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/win32/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/win32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/win32/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/win32/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/os_utilities/windows_utilities/windows_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.800071 Draugr-1.0.8/draugr/pandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pandas_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pandas_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pandas_utilities/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pandas_utilities/from_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pandas_utilities/latex_mean_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pandas_utilities/misc_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pandas_utilities/multi_index_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pandas_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.800071 Draugr-1.0.8/draugr/pygame_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pygame_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pygame_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/pygame_utilities/screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.800071 Draugr-1.0.8/draugr/python_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/broadcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/counter_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/function_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.804072 Draugr-1.0.8/draugr/python_utilities/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/generators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/generators/batching_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/generators/recycling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/platform_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/python_utilities/torch_like_channel_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.804072 Draugr-1.0.8/draugr/random_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/random_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/random_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/random_utilities/seeding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.804072 Draugr-1.0.8/draugr/scipy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/scipy_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/scipy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/scipy_utilities/scipy_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.804072 Draugr-1.0.8/draugr/scipy_utilities/signal_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/scipy_utilities/signal_processing/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/scipy_utilities/signal_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/scipy_utilities/subsampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.804072 Draugr-1.0.8/draugr/stopping/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/stopping/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/stopping/stopping_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.804072 Draugr-1.0.8/draugr/tensorboard_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.804072 Draugr-1.0.8/draugr/tensorboard_utilities/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/experimental/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/experimental/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/experimental/pretty_cf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.804072 Draugr-1.0.8/draugr/tensorboard_utilities/exporting/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/exporting/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/exporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/exporting/db_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/exporting/event_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/tensorboard_utilities/exporting/file_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/threading_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/threading_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/threading_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/threading_utilities/skipper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/torch_utilities/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/architecture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/torch_utilities/architectures/distributional/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/distributional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/distributional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/distributional/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/distributional/normal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/heads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/layers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/layers/radial_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/concatination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/disjunction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/experimental/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/experimental/recurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/fourier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.808072 Draugr-1.0.8/draugr/torch_utilities/architectures/recurrent/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/recurrent/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/recurrent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.812072 Draugr-1.0.8/draugr/torch_utilities/architectures/recurrent/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/recurrent/experimental/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/recurrent/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/recurrent/experimental/recurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/architectures/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.812072 Draugr-1.0.8/draugr/torch_utilities/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/non_sequential_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/random_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.812072 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/categorical_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/supervised_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.812072 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/vision_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/vision_datasets/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/vision_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/vision_datasets/dict_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.812072 Draugr-1.0.8/draugr/torch_utilities/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/distributions/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/distributions/entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.812072 Draugr-1.0.8/draugr/torch_utilities/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/evaluation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/evaluation/archetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/evaluation/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/evaluation/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.812072 Draugr-1.0.8/draugr/torch_utilities/exporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/exporting/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/exporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/exporting/latex_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/exporting/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.816072 Draugr-1.0.8/draugr/torch_utilities/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/generators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/generators/batching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/generators/to_tensor_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.816072 Draugr-1.0.8/draugr/torch_utilities/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/images/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/images/channel_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/images/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.816072 Draugr-1.0.8/draugr/torch_utilities/opencv/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/opencv/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/opencv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/opencv/torch_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.816072 Draugr-1.0.8/draugr/torch_utilities/operations/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/boxes_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.816072 Draugr-1.0.8/draugr/torch_utilities/operations/sizes/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/sizes/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/sizes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/sizes/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/sizes/max_pool2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/sizes/pad2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/sizes/transp_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.816072 Draugr-1.0.8/draugr/torch_utilities/operations/torch_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/torch_transforms/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/torch_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/operations/torch_transforms/batch_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.820073 Draugr-1.0.8/draugr/torch_utilities/optimisation/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.820073 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.820073 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.820073 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/checking/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/checking/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/checking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/checking/numerical_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/grad_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/guided.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/layer_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/opt_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.820073 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/counting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/differential_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/exporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.820073 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/freezing/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/freezing/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/freezing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/freezing/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/freezing/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.824073 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/atari_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/fan_in_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/normal_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/ortho_weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.824073 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/regularisation/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/regularisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/regularisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/regularisation/reg_loss_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/trainable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.824073 Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/learning_rate_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.824073 Draugr-1.0.8/draugr/torch_utilities/optimisation/stopping/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/stopping/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/stopping/overfitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.824073 Draugr-1.0.8/draugr/torch_utilities/optimisation/updates/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/updates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/updates/copying.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/optimisation/updates/soft_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.824073 Draugr-1.0.8/draugr/torch_utilities/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/persistence/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/persistence/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/persistence/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/persistence/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/persistence/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/persistence/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.828073 Draugr-1.0.8/draugr/torch_utilities/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/sessions/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/sessions/cache_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/sessions/determinism_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/sessions/device_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/sessions/jit_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/sessions/model_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/sessions/type_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.828073 Draugr-1.0.8/draugr/torch_utilities/system/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/system/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/system/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/system/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/system/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/system/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/system/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/system/seeding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.832073 Draugr-1.0.8/draugr/torch_utilities/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/dimension_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/normalise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/reshaping.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/tensor_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/to_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/tensors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.832073 Draugr-1.0.8/draugr/torch_utilities/writers/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.832073 Draugr-1.0.8/draugr/torch_utilities/writers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/mixins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/mixins/graph_writer_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.832073 Draugr-1.0.8/draugr/torch_utilities/writers/tensorboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/tensorboard/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/tensorboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/tensorboard/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/tensorboard/tensorboard_pytorch_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.832073 Draugr-1.0.8/draugr/torch_utilities/writers/torch_module_writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/torch_module_writer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/torch_module_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/torch_module_writer/module_parameter_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/torch_module_writer/module_writer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/torch_module_writer/module_writer_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.832073 Draugr-1.0.8/draugr/torch_utilities/writers/visdom/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/visdom/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/visdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/visdom/episode_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/visdom/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/torch_utilities/writers/visdom/visdom_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.832073 Draugr-1.0.8/draugr/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.832073 Draugr-1.0.8/draugr/visualisation/ggplot_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/ggplot_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/ggplot_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.836073 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/color_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/figure_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.836073 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/display_3d_depth_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/display_depth_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/replay_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/matplotlib_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/matplotlib_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/metric_overview_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/quirks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.836073 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/3d_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/3d_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/display_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/signal_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/spectral_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.840074 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/cyclers.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/hatching.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/monochrome.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/publish_color.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/pillow_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.840074 Draugr-1.0.8/draugr/visualisation/progress/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/progress/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/progress/eta_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/progress/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/progress/pooled_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/progress/progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.840074 Draugr-1.0.8/draugr/visualisation/seaborn_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/seaborn_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/seaborn_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/seaborn_utilities/seaborn_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/visualisation/seaborn_utilities/seaborn_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.840074 Draugr-1.0.8/draugr/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/csv_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.840074 Draugr-1.0.8/draugr/writers/databases/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/databases/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/databases/hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/databases/sqlite_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/log_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.844074 Draugr-1.0.8/draugr/writers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/audio_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/bar_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/embed_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/figure_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/histogram_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/image_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/instantiation_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/line_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/mesh_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/precision_recall_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/scalar_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/spectrogram_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mixins/video_writer_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/mock_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/standard_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.844074 Draugr-1.0.8/draugr/writers/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/terminal/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/terminal/console_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/terminal/terminal_plot_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-02-23 07:51:45.000000 Draugr-1.0.8/draugr/writers/writer_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-23 07:51:45.000000 Draugr-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-23 07:51:45.000000 Draugr-1.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.844074 Draugr-1.0.8/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-23 07:51:45.000000 Draugr-1.0.8/samples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.844074 Draugr-1.0.8/samples/tensorboard_samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:45.000000 Draugr-1.0.8/samples/tensorboard_samples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-23 07:51:52.848074 Draugr-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-02-23 07:51:45.000000 Draugr-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 07:51:52.844074 Draugr-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-02-23 07:51:45.000000 Draugr-1.0.8/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-23 07:51:45.000000 Draugr-1.0.8/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-23 07:51:45.000000 Draugr-1.0.8/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.746296 Draugr-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.670295 Draugr-1.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-01 06:12:21.000000 Draugr-1.0.9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-01 06:12:21.000000 Draugr-1.0.9/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 06:12:21.000000 Draugr-1.0.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:21.000000 Draugr-1.0.9/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.670295 Draugr-1.0.9/Draugr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-01 06:12:27.000000 Draugr-1.0.9/Draugr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25488 2023-08-01 06:12:27.000000 Draugr-1.0.9/Draugr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:12:27.000000 Draugr-1.0.9/Draugr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-01 06:12:27.000000 Draugr-1.0.9/Draugr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-01 06:12:27.000000 Draugr-1.0.9/Draugr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 06:12:27.000000 Draugr-1.0.9/Draugr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:12:21.000000 Draugr-1.0.9/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-01 06:12:21.000000 Draugr-1.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-01 06:12:21.000000 Draugr-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-01 06:12:27.746296 Draugr-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-08-01 06:12:21.000000 Draugr-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.670295 Draugr-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:12:21.000000 Draugr-1.0.9/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.670295 Draugr-1.0.9/draugr/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.670295 Draugr-1.0.9/draugr/dlib_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/dlib_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/dlib_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/dlib_utilities/dlib_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/dlib_utilities/facealigner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.670295 Draugr-1.0.9/draugr/drawers/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/drawer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.670295 Draugr-1.0.9/draugr/drawers/mpl_drawers/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/discrete_scroll_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/distribution_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/image_stream_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/mpldrawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/series_scroll_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.674295 Draugr-1.0.9/draugr/drawers/mpl_drawers/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/spectral/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/spectral/fast_fourier_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/mpl_drawers/spectral/fast_fourier_transform_spectrogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.674295 Draugr-1.0.9/draugr/drawers/opencv_drawers/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/opencv_drawers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/opencv_drawers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/opencv_drawers/opencv_image_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.674295 Draugr-1.0.9/draugr/drawers/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/terminal/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/terminal/terminal_image_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/terminal/terminal_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/terminal/terminal_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/drawers/terminal/terminal_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.674295 Draugr-1.0.9/draugr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/entry_points/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/entry_points/cpu_usage_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/entry_points/tensorboard_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/entry_points/toggle_darkmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/entry_points/visdom_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.674295 Draugr-1.0.9/draugr/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/extensions/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/extensions/skimage_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/extensions/sorcery_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.674295 Draugr-1.0.9/draugr/ffmpeg_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/ffmpeg_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/ffmpeg_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/ffmpeg_utilities/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/ffmpeg_utilities/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/ffmpeg_utilities/sequencify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/ffmpeg_utilities/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.678295 Draugr-1.0.9/draugr/matlab_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/matlab_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/matlab_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/matlab_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/matlab_utilities/matlab_conversion_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/matlab_utilities/singleton_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.678295 Draugr-1.0.9/draugr/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/meters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/metric_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/metric_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/metric_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.678295 Draugr-1.0.9/draugr/metrics/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/plotting/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/metrics/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.678295 Draugr-1.0.9/draugr/multiprocessing_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/multiprocessing_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/multiprocessing_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/multiprocessing_utilities/pooled_queue_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.678295 Draugr-1.0.9/draugr/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/channel_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.678295 Draugr-1.0.9/draugr/numpy_utilities/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.682295 Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/deep_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/flat_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/shallow_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/datasets/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/mixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/powers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/raster_grid_2d_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/raster_grid_3d_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.682295 Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/signal_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/signal_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/signal_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/truncation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.682295 Draugr-1.0.9/draugr/opencv_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.682295 Draugr-1.0.9/draugr/opencv_utilities/bounding_boxes/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/bounding_boxes/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/bounding_boxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/bounding_boxes/boxes_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/bounding_boxes/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.686295 Draugr-1.0.9/draugr/opencv_utilities/color_space/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/gray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/color_space/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.686295 Draugr-1.0.9/draugr/opencv_utilities/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/draw_boxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.686295 Draugr-1.0.9/draugr/opencv_utilities/drawing/masks/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/masks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/masks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/masks/gauss_circles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/masks/segment_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/opencv_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/drawing/opencv_drawing_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.686295 Draugr-1.0.9/draugr/opencv_utilities/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/namespaces/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/namespaces/color_conversion_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/namespaces/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/namespaces/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.686295 Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/async_video_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/frame_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/video_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.690295 Draugr-1.0.9/draugr/opencv_utilities/transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/transformation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/transformation/cropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/transformation/cv2_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/transformation/resize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.690295 Draugr-1.0.9/draugr/opencv_utilities/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.690295 Draugr-1.0.9/draugr/opencv_utilities/windows/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/elements/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/elements/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/elements/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/elements/trackbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/opencv_utilities/windows/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.690295 Draugr-1.0.9/draugr/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/cuda_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.690295 Draugr-1.0.9/draugr/os_utilities/linux_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.690295 Draugr-1.0.9/draugr/os_utilities/linux_utilities/cron_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/cron_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/cron_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.690295 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gnome_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gnome_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gnome_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gnome_utilities/dark_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.694295 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gtk_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gtk_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gtk_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gtk_utilities/gtk_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/gtk_utilities/theme_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.694295 Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/service_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/service_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/timer_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/linux_utilities/user_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.694295 Draugr-1.0.9/draugr/os_utilities/mac_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/mac_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/mac_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/mac_utilities/dark_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.694295 Draugr-1.0.9/draugr/os_utilities/resource_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/resource_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/resource_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/resource_utilities/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/resource_utilities/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/resource_utilities/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/resource_utilities/ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/screen_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.694295 Draugr-1.0.9/draugr/os_utilities/windows_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.694295 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.698295 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/enums/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/enums/task_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/enums/task_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/enums/task_logon_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/enums/task_trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.698295 Draugr-1.0.9/draugr/os_utilities/windows_utilities/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/win32/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/win32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/win32/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/win32/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/os_utilities/windows_utilities/windows_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.698295 Draugr-1.0.9/draugr/pandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pandas_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pandas_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pandas_utilities/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pandas_utilities/from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pandas_utilities/latex_mean_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pandas_utilities/misc_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pandas_utilities/multi_index_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pandas_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.698295 Draugr-1.0.9/draugr/pipeline_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pipeline_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.698295 Draugr-1.0.9/draugr/pygame_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pygame_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pygame_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/pygame_utilities/screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.702295 Draugr-1.0.9/draugr/python_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/broadcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/counter_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/function_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.702295 Draugr-1.0.9/draugr/python_utilities/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/generators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/generators/batching_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/generators/recycling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/platform_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/python_utilities/torch_like_channel_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.702295 Draugr-1.0.9/draugr/random_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/random_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/random_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/random_utilities/seeding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.702295 Draugr-1.0.9/draugr/scipy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/scipy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/scipy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/scipy_utilities/scipy_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.702295 Draugr-1.0.9/draugr/scipy_utilities/signal_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/scipy_utilities/signal_processing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/scipy_utilities/signal_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/scipy_utilities/subsampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.702295 Draugr-1.0.9/draugr/stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/stopping/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/stopping/stopping_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.706296 Draugr-1.0.9/draugr/tensorboard_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.706296 Draugr-1.0.9/draugr/tensorboard_utilities/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/experimental/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/experimental/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/experimental/pretty_cf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.706296 Draugr-1.0.9/draugr/tensorboard_utilities/exporting/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/exporting/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/exporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/exporting/db_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/exporting/event_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/tensorboard_utilities/exporting/file_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.706296 Draugr-1.0.9/draugr/threading_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/threading_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/threading_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/threading_utilities/skipper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.706296 Draugr-1.0.9/draugr/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.706296 Draugr-1.0.9/draugr/torch_utilities/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/architecture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.706296 Draugr-1.0.9/draugr/torch_utilities/architectures/distributional/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/distributional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/distributional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/distributional/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/distributional/normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.710296 Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/heads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.710296 Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/layers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/layers/radial_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.710296 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/concatination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/disjunction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.710296 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/experimental/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/experimental/recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/fourier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.710296 Draugr-1.0.9/draugr/torch_utilities/architectures/recurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/recurrent/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/recurrent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.710296 Draugr-1.0.9/draugr/torch_utilities/architectures/recurrent/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/recurrent/experimental/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/recurrent/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/recurrent/experimental/recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/architectures/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.710296 Draugr-1.0.9/draugr/torch_utilities/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/non_sequential_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/random_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.714296 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/categorical_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/supervised_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.714296 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/vision_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/vision_datasets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/vision_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/vision_datasets/dict_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.714296 Draugr-1.0.9/draugr/torch_utilities/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/distributions/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/distributions/entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.714296 Draugr-1.0.9/draugr/torch_utilities/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/evaluation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/evaluation/archetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/evaluation/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/evaluation/cross_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.714296 Draugr-1.0.9/draugr/torch_utilities/exporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/exporting/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/exporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/exporting/latex_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/exporting/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.714296 Draugr-1.0.9/draugr/torch_utilities/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/generators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/generators/batching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/generators/to_tensor_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.714296 Draugr-1.0.9/draugr/torch_utilities/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/images/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/images/channel_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/images/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.718296 Draugr-1.0.9/draugr/torch_utilities/opencv/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/opencv/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/opencv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/opencv/torch_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.718296 Draugr-1.0.9/draugr/torch_utilities/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/boxes_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.718296 Draugr-1.0.9/draugr/torch_utilities/operations/sizes/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/sizes/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/sizes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/sizes/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/sizes/max_pool2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/sizes/pad2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/sizes/transp_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.718296 Draugr-1.0.9/draugr/torch_utilities/operations/torch_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/torch_transforms/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/torch_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/operations/torch_transforms/batch_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.718296 Draugr-1.0.9/draugr/torch_utilities/optimisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.718296 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.722296 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.722296 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/checking/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/checking/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/checking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/checking/numerical_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/grad_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/guided.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/layer_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/opt_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.722296 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/counting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/differential_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/exporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.722296 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/freezing/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/freezing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/freezing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/freezing/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/freezing/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.722296 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/atari_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/fan_in_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/normal_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/ortho_weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.722296 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/regularisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/regularisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/regularisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/regularisation/reg_loss_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/trainable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.726296 Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/learning_rate_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.726296 Draugr-1.0.9/draugr/torch_utilities/optimisation/stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/stopping/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/stopping/overfitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.726296 Draugr-1.0.9/draugr/torch_utilities/optimisation/updates/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/updates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/updates/copying.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/optimisation/updates/soft_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.726296 Draugr-1.0.9/draugr/torch_utilities/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/persistence/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/persistence/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/persistence/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/persistence/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/persistence/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/persistence/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.726296 Draugr-1.0.9/draugr/torch_utilities/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/sessions/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/sessions/cache_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/sessions/determinism_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/sessions/device_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/sessions/jit_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/sessions/model_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/sessions/type_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.730296 Draugr-1.0.9/draugr/torch_utilities/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/system/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/system/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/system/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/system/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/system/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/system/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/system/seeding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.730296 Draugr-1.0.9/draugr/torch_utilities/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/dimension_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/normalise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/reshaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/tensor_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/to_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/tensors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.730296 Draugr-1.0.9/draugr/torch_utilities/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.734296 Draugr-1.0.9/draugr/torch_utilities/writers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/mixins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/mixins/graph_writer_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.734296 Draugr-1.0.9/draugr/torch_utilities/writers/tensorboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/tensorboard/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/tensorboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/tensorboard/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18308 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/tensorboard/tensorboard_pytorch_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.734296 Draugr-1.0.9/draugr/torch_utilities/writers/torch_module_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/torch_module_writer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/torch_module_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/torch_module_writer/module_parameter_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/torch_module_writer/module_writer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/torch_module_writer/module_writer_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.734296 Draugr-1.0.9/draugr/torch_utilities/writers/visdom/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/visdom/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/visdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/visdom/episode_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/visdom/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/torch_utilities/writers/visdom/visdom_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.734296 Draugr-1.0.9/draugr/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.734296 Draugr-1.0.9/draugr/visualisation/ggplot_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/ggplot_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/ggplot_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.738296 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/color_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/figure_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.738296 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/display_3d_depth_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/display_depth_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/replay_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/matplotlib_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/matplotlib_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/metric_overview_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/quirks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.738296 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/3d_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/3d_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/display_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/signal_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/spectral_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.738296 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/cyclers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/hatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/monochrome.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/publish_color.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/pillow_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.742296 Draugr-1.0.9/draugr/visualisation/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/progress/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/progress/eta_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/progress/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/progress/pooled_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/progress/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.742296 Draugr-1.0.9/draugr/visualisation/seaborn_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/seaborn_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/seaborn_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/seaborn_utilities/seaborn_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/visualisation/seaborn_utilities/seaborn_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.742296 Draugr-1.0.9/draugr/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/csv_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.742296 Draugr-1.0.9/draugr/writers/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/databases/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/databases/hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/databases/sqlite_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/log_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.742296 Draugr-1.0.9/draugr/writers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/audio_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/bar_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/embed_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/figure_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/histogram_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/image_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/instantiation_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/line_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/mesh_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/precision_recall_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/scalar_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/spectrogram_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mixins/video_writer_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/mock_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/standard_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.746296 Draugr-1.0.9/draugr/writers/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/terminal/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/terminal/console_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/terminal/terminal_plot_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 06:12:22.000000 Draugr-1.0.9/draugr/writers/writer_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 06:12:22.000000 Draugr-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 06:12:22.000000 Draugr-1.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.746296 Draugr-1.0.9/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 06:12:22.000000 Draugr-1.0.9/samples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.666295 Draugr-1.0.9/samples/temporal_samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.746296 Draugr-1.0.9/samples/temporal_samples/multi_worker_shared_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-01 06:12:22.000000 Draugr-1.0.9/samples/temporal_samples/multi_worker_shared_queue/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.746296 Draugr-1.0.9/samples/temporal_samples/parralel_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 06:12:22.000000 Draugr-1.0.9/samples/temporal_samples/parralel_pipeline/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.746296 Draugr-1.0.9/samples/temporal_samples/sequential_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 06:12:22.000000 Draugr-1.0.9/samples/temporal_samples/sequential_pipeline/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.746296 Draugr-1.0.9/samples/tensorboard_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:22.000000 Draugr-1.0.9/samples/tensorboard_samples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 06:12:27.746296 Draugr-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-08-01 06:12:22.000000 Draugr-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:12:27.746296 Draugr-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-01 06:12:22.000000 Draugr-1.0.9/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 06:12:22.000000 Draugr-1.0.9/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 06:12:22.000000 Draugr-1.0.9/tests/test_statistics.py
```

### Comparing `Draugr-1.0.8/.github/CODE_OF_CONDUCT.md` & `Draugr-1.0.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/.github/CONTRIBUTING.md` & `Draugr-1.0.9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/Draugr.egg-info/PKG-INFO` & `Draugr-1.0.9/Draugr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Draugr
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for plotting directly in your terminal
 Home-page: https://github.com/pything/draugr
 Download-URL: https://github.com/pything/draugr/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,31 +19,31 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: ja
-Provides-Extra: dlib
-Provides-Extra: writers
 Provides-Extra: dev
-Provides-Extra: windows
-Provides-Extra: linu
-Provides-Extra: visualisation
 Provides-Extra: pygame
+Provides-Extra: torch
+Provides-Extra: tests
 Provides-Extra: opencv
+Provides-Extra: drawers
+Provides-Extra: extensions
+Provides-Extra: dlib
 Provides-Extra: docs
 Provides-Extra: multiprocessing
-Provides-Extra: tqdm
-Provides-Extra: torch
-Provides-Extra: extensions
+Provides-Extra: windows
 Provides-Extra: setup
-Provides-Extra: drawers
+Provides-Extra: ja
+Provides-Extra: linu
+Provides-Extra: writers
+Provides-Extra: visualisation
+Provides-Extra: tqdm
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![valknut](.github/images/valknut.svg)-->
 
 <p align="center">
   <img src=".github/images/valknut.svg" alt='Valknut' />
```

### Comparing `Draugr-1.0.8/Draugr.egg-info/SOURCES.txt` & `Draugr-1.0.9/Draugr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
 draugr/os_utilities/linux_utilities/gtk_utilities/__init__.py
 draugr/os_utilities/linux_utilities/gtk_utilities/gtk_settings.py
 draugr/os_utilities/linux_utilities/gtk_utilities/theme_preferences.py
 draugr/os_utilities/linux_utilities/systemd_utilities/README.md
 draugr/os_utilities/linux_utilities/systemd_utilities/__init__.py
 draugr/os_utilities/linux_utilities/systemd_utilities/service_management.py
 draugr/os_utilities/linux_utilities/systemd_utilities/service_template.py
+draugr/os_utilities/linux_utilities/systemd_utilities/timer_template.py
 draugr/os_utilities/mac_utilities/README.md
 draugr/os_utilities/mac_utilities/__init__.py
 draugr/os_utilities/mac_utilities/dark_mode.py
 draugr/os_utilities/resource_utilities/README.md
 draugr/os_utilities/resource_utilities/__init__.py
 draugr/os_utilities/resource_utilities/all.py
 draugr/os_utilities/resource_utilities/cpu.py
@@ -205,14 +206,15 @@
 draugr/pandas_utilities/__init__.py
 draugr/pandas_utilities/formatting.py
 draugr/pandas_utilities/from_dict.py
 draugr/pandas_utilities/latex_mean_std.py
 draugr/pandas_utilities/misc_utilities.py
 draugr/pandas_utilities/multi_index_utilities.py
 draugr/pandas_utilities/styling.py
+draugr/pipeline_utilities/__init__.py
 draugr/pygame_utilities/README.md
 draugr/pygame_utilities/__init__.py
 draugr/pygame_utilities/screen.py
 draugr/python_utilities/README.md
 draugr/python_utilities/__init__.py
 draugr/python_utilities/broadcasting.py
 draugr/python_utilities/counter_filter.py
@@ -505,11 +507,14 @@
 draugr/writers/mixins/spectrogram_writer_mixin.py
 draugr/writers/mixins/video_writer_mixin.py
 draugr/writers/terminal/README.md
 draugr/writers/terminal/__init__.py
 draugr/writers/terminal/console_writer.py
 draugr/writers/terminal/terminal_plot_writer.py
 samples/README.md
+samples/temporal_samples/multi_worker_shared_queue/README.md
+samples/temporal_samples/parralel_pipeline/README.md
+samples/temporal_samples/sequential_pipeline/README.md
 samples/tensorboard_samples/README.md
 tests/test_imports.py
 tests/test_sanity.py
 tests/test_statistics.py
```

### Comparing `Draugr-1.0.8/LICENSE.md` & `Draugr-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/PKG-INFO` & `Draugr-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Draugr
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for plotting directly in your terminal
 Home-page: https://github.com/pything/draugr
 Download-URL: https://github.com/pything/draugr/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,31 +19,31 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: ja
-Provides-Extra: dlib
-Provides-Extra: writers
 Provides-Extra: dev
-Provides-Extra: windows
-Provides-Extra: linu
-Provides-Extra: visualisation
 Provides-Extra: pygame
+Provides-Extra: torch
+Provides-Extra: tests
 Provides-Extra: opencv
+Provides-Extra: drawers
+Provides-Extra: extensions
+Provides-Extra: dlib
 Provides-Extra: docs
 Provides-Extra: multiprocessing
-Provides-Extra: tqdm
-Provides-Extra: torch
-Provides-Extra: extensions
+Provides-Extra: windows
 Provides-Extra: setup
-Provides-Extra: drawers
+Provides-Extra: ja
+Provides-Extra: linu
+Provides-Extra: writers
+Provides-Extra: visualisation
+Provides-Extra: tqdm
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![valknut](.github/images/valknut.svg)-->
 
 <p align="center">
   <img src=".github/images/valknut.svg" alt='Valknut' />
```

### Comparing `Draugr-1.0.8/README.md` & `Draugr-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/__init__.py` & `Draugr-1.0.9/draugr/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
 __project__ = "Draugr"
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
 
 import datetime
 import os
 from logging import warning
+from pathlib import Path
 from typing import Any
+from importlib import resources
+from importlib.metadata import PackageNotFoundError
+from warg import package_is_editable
 
-import pkg_resources
-
+from warg import dist_is_editable
 from apppath import AppPath
-from pathlib import Path
 
 # from .drawers import *
 # from .writers import *
 # from .opencv_utilities import *
 # from .torch_utilities import *
 # from .stopping import *
 # from .numpy_utilities import *
 # from .visualisation import *
 # from .metrics import *
 # from .python_utilities import *
 
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 
-
 # with open(Path(__file__).parent.parent / "README.md", "r") as this_init_file:
 #    __doc__ += this_init_file.read()
 
 __all__ = [
     "PROJECT_APP_PATH",
     "PROJECT_NAME",
     "PROJECT_VERSION",
@@ -47,43 +48,29 @@
     "PROJECT_ORGANISATION",
     "PROJECT_AUTHOR",
     "PROJECT_YEAR",
     "INCLUDE_PROJECT_READMES",
     "PACKAGE_DATA_PATH",
 ]
 
-
-def dist_is_editable(dist: Any) -> bool:
-    """
-    Return True if given Distribution is an editable installation."""
-    import sys
-
-    for path_item in sys.path:
-        egg_link = Path(path_item) / f"{dist.project_name}.egg-link"
-        if egg_link.is_file():
-            return True
-    return False
-
-
 PROJECT_ORGANISATION = "Pything"
 PROJECT_NAME = __project__.lower().strip().replace(" ", "_")
 PROJECT_VERSION = __version__
 PROJECT_YEAR = 2018
 PROJECT_AUTHOR = __author__.lower().strip().replace(" ", "_")
 PROJECT_APP_PATH = AppPath(app_name=PROJECT_NAME, app_author=PROJECT_AUTHOR)
-PACKAGE_DATA_PATH = Path(pkg_resources.resource_filename(PROJECT_NAME, "data"))
 INCLUDE_PROJECT_READMES = False
 
 __url__ = f"https://github.com/{PROJECT_ORGANISATION.lower()}/{PROJECT_NAME}"
 
-distributions = {v.key: v for v in pkg_resources.working_set}
-if PROJECT_NAME in distributions:
-    distribution = distributions[PROJECT_NAME]
-    DEVELOP = dist_is_editable(distribution)
-else:
+PACKAGE_DATA_PATH = resources.files(PROJECT_NAME) / "data"
+
+try:
+    DEVELOP = package_is_editable(PROJECT_NAME)
+except PackageNotFoundError as e:
     DEVELOP = True
 
 
 def get_version(append_time: Any = DEVELOP) -> str:
     """description"""
     version = __version__
     if not version:
```

### Comparing `Draugr-1.0.8/draugr/dlib_utilities/__init__.py` & `Draugr-1.0.9/draugr/dlib_utilities/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 03-05-2021
            """
 
-
 from pathlib import Path
 
 try:
     from .dlib_utilities import *
     from .facealigner import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
```

### Comparing `Draugr-1.0.8/draugr/dlib_utilities/dlib_utilities.py` & `Draugr-1.0.9/draugr/dlib_utilities/dlib_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/dlib_utilities/facealigner.py` & `Draugr-1.0.9/draugr/dlib_utilities/facealigner.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import cv2
 import numpy
-
 from draugr.dlib_utilities.dlib_utilities import (
     Dlib5faciallandmarksindices,
     Dlib68faciallandmarksindices,
     shape_to_ndarray,
 )
+
 from warg import Number
 
 __all__ = ["align_face"]
 
 
 def align_face(
     image,
```

### Comparing `Draugr-1.0.8/draugr/drawers/__init__.py` & `Draugr-1.0.9/draugr/drawers/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/drawers/drawer.py` & `Draugr-1.0.9/draugr/drawers/drawer.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
            Created on 25-01-2021
            """
 
 __all__ = ["Drawer"]
 
 from abc import abstractmethod
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any
+
 from warg import drop_unused_kws
 
 
 class Drawer(object):
     """
     Abstract class for drawing representations of data
     """
 
     @drop_unused_kws
     def __init__(self, verbose: bool = False):
         self._verbose = verbose
 
     @abstractmethod
-    def draw(self, *args: Sequence, **kwargs: MutableMapping) -> None:
+    def draw(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]) -> None:
         """description"""
         raise NotImplementedError
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `Draugr-1.0.8/draugr/drawers/mpl_drawers/__init__.py` & `Draugr-1.0.9/draugr/drawers/mpl_drawers/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/drawers/mpl_drawers/discrete_scroll_plot.py` & `Draugr-1.0.9/draugr/drawers/mpl_drawers/discrete_scroll_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 Created on 27/04/2019
 
 @author: cnheider
 """
 
 __all__ = ["DiscreteScrollPlot", "discrete_scroll_plot"]
 
-from typing import Iterator, Sequence, Tuple, MutableMapping
+from typing import Iterator, Sequence, Tuple, MutableMapping, Any
 
 import numpy
+from draugr.drawers.mpl_drawers.mpldrawer import MplDrawer
+from draugr.numpy_utilities import recursive_flatten_numpy
 from matplotlib import animation
 from matplotlib import pyplot
 
-from draugr.drawers.mpl_drawers.mpldrawer import MplDrawer
-from draugr.numpy_utilities import recursive_flatten_numpy
 from warg import passes_kws_to
 
 
 class DiscreteScrollPlot(MplDrawer):
     """
     Waterfall plot
     only supports a single trajectory at a time, do not supply parallel trajectories to draw method, will get truncated to num actions, effectively dropping actions for other envs than the first.
@@ -253,15 +253,17 @@
             class QueueGen:
                 def __iter__(self):
                     return self
 
                 def __next__(self):
                     return self.get()
 
-                def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+                def __call__(
+                    self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]
+                ):
                     return self.__next__()
 
                 def add(self, a):
                     """description"""
                     return data.put(a)
 
                 def get(self):
```

### Comparing `Draugr-1.0.8/draugr/drawers/mpl_drawers/distribution_plot.py` & `Draugr-1.0.9/draugr/drawers/mpl_drawers/distribution_plot.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
            """
 
 __all__ = ["DistributionPlot"]
 
 from typing import Sequence
 
 import numpy
+from draugr.drawers.mpl_drawers.mpldrawer import MplDrawer
 from matplotlib import pyplot
 
-from draugr.drawers.mpl_drawers.mpldrawer import MplDrawer
 from warg import passes_kws_to
 
 
 class DistributionPlot(MplDrawer):
     """
     Distribution plot using matplotlib
     """
```

### Comparing `Draugr-1.0.8/draugr/drawers/mpl_drawers/image_stream_plot.py` & `Draugr-1.0.9/draugr/drawers/mpl_drawers/image_stream_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,21 @@
            Created on 22-01-2021
            """
 
 __all__ = ["ImageStreamPlot"]
 
 from typing import Sequence
 
-from matplotlib import pyplot
 import matplotlib
 from draugr.drawers.mpl_drawers.mpldrawer import MplDrawer
+from matplotlib import pyplot
+
 from warg import passes_kws_to
 
+
 # pyplot.switch_backend("QtAgg")  # MacOSX, QtAgg, GTK4Agg, Gtk3Agg, TkAgg, WxAgg, Agg
 
 
 class ImageStreamPlot(MplDrawer):
     """
     Image stream plot using matplotlib
     """
```

### Comparing `Draugr-1.0.8/draugr/drawers/mpl_drawers/mpldrawer.py` & `Draugr-1.0.9/draugr/drawers/mpl_drawers/mpldrawer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 
 __all__ = ["MplDrawer", "MockDrawer"]
 
 from abc import abstractmethod
 from typing import Any, Sequence, Tuple, MutableMapping
 
 import matplotlib
-from matplotlib import pyplot
-
 from draugr.drawers.drawer import Drawer
+from matplotlib import pyplot
 
 
 # TODO: implement a key for closing the plot
 # close figure with spacebar
 # fig.canvas.mpl_connect('key_press_event', lambda evt: if evt.key == ' ': plt.close())
 # global solution
 # fig.canvas.mpl_connect('key_press_event', lambda evt: print(repr(evt.key))) # print key pressed
```

### Comparing `Draugr-1.0.8/draugr/drawers/mpl_drawers/series_scroll_plot.py` & `Draugr-1.0.9/draugr/drawers/mpl_drawers/series_scroll_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,17 @@
            Created on 22/11/2019
 
            """
 
 from typing import Sequence, Union, MutableMapping
 
 import numpy
-from matplotlib import pyplot
-
 from draugr.drawers.mpl_drawers.mpldrawer import MplDrawer
 from draugr.numpy_utilities import recursive_flatten_numpy
+from matplotlib import pyplot
 
 __all__ = ["SeriesScrollPlot"]
 
 from warg import passes_kws_to
 
 
 class SeriesScrollPlot(MplDrawer):
```

### Comparing `Draugr-1.0.8/draugr/drawers/mpl_drawers/spectral/fast_fourier_transform.py` & `Draugr-1.0.9/draugr/drawers/mpl_drawers/spectral/fast_fourier_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 """
 
 __all__ = ["FastFourierTransformPlot"]
 
 import math
 
 import numpy
-from matplotlib import pyplot
-from matplotlib.gridspec import GridSpec
-
 from draugr.drawers.mpl_drawers.mpldrawer import MplDrawer
 from draugr.visualisation.progress import progress_bar
+from matplotlib import pyplot
+from matplotlib.gridspec import GridSpec
 
 FLOAT_EPS = numpy.finfo(float).eps
 
 
 class FastFourierTransformPlot(MplDrawer):
     """
     Plots last computed fft of data"""
```

### Comparing `Draugr-1.0.8/draugr/drawers/mpl_drawers/spectral/fast_fourier_transform_spectrogram.py` & `Draugr-1.0.9/draugr/drawers/mpl_drawers/spectral/fast_fourier_transform_spectrogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 """
 
 __all__ = ["FastFourierTransformSpectrogramPlot"]
 
 import math
 
 import numpy
-from matplotlib import pyplot
-from matplotlib.gridspec import GridSpec
-
 from draugr.drawers.mpl_drawers.mpldrawer import MplDrawer
 from draugr.visualisation.progress import progress_bar
+from matplotlib import pyplot
+from matplotlib.gridspec import GridSpec
 
 FLOAT_EPS = numpy.finfo(float).eps
 
 
 class FastFourierTransformSpectrogramPlot(MplDrawer):
     """
     TODO: CENTER Align fft maybe, to mimick librosa stft
```

### Comparing `Draugr-1.0.8/draugr/drawers/opencv_drawers/opencv_image_stream.py` & `Draugr-1.0.9/draugr/drawers/opencv_drawers/opencv_image_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 25-01-2021
            """
 __all__ = ["OpencvImageStream"]
 
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any
 
 import cv2
 from draugr.drawers.drawer import Drawer
 from draugr.opencv_utilities import WindowFlagEnum
 from draugr.opencv_utilities.windows.default import match_return_code
+
 from warg import drop_unused_kws, passes_kws_to
 
 
 class OpencvImageStream(Drawer):
     """
     OpenCv Image Stream
```

### Comparing `Draugr-1.0.8/draugr/drawers/terminal/terminal_image_renderer.py` & `Draugr-1.0.9/draugr/drawers/terminal/terminal_image_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 __author__ = "heider"
 __doc__ = r"""
            Render images on the command line
 
            Created on 7/5/22
            """
 
-
 import argparse
 from pathlib import Path
 from typing import Any, List, Tuple
 
 import numpy
 from PIL import Image
```

### Comparing `Draugr-1.0.8/draugr/drawers/terminal/terminal_plot.py` & `Draugr-1.0.9/draugr/drawers/terminal/terminal_plot.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from draugr.drawers.terminal.terminal_utilities import scale
+
 from warg import (
     COLORS,
     PrintStyle,
     generate_style,
     get_terminal_size,
 )
 
 __doc__ = r"""
 
            Created on 7/5/22
            """
 
-
 __author__ = "Christian Heider Nielsen"
 __all__ = ["terminal_plot", "styled_terminal_plot_stats_shared_x"]
 
-
 from typing import Sequence, Dict, MutableMapping
 
 import numpy
 
+
 # sys.stdout.write(generate_style(u'Draugr Ûnicöde Probe\n', underline=True, italic=True))
 
 
 def terminal_plot(
     y: Sequence,
     *,
     x: Sequence = None,
```

### Comparing `Draugr-1.0.8/draugr/drawers/terminal/terminal_utilities.py` & `Draugr-1.0.9/draugr/drawers/terminal/terminal_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/entry_points/cpu_usage_entry_point.py` & `Draugr-1.0.9/draugr/entry_points/cpu_usage_entry_point.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/entry_points/tensorboard_entry_point.py` & `Draugr-1.0.9/draugr/entry_points/tensorboard_entry_point.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/extensions/__init__.py` & `Draugr-1.0.9/draugr/extensions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 04-04-2021
            """
 
-
 from pathlib import Path
 
 try:
     from .skimage_utilities import *
     from .sorcery_utilities import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
```

### Comparing `Draugr-1.0.8/draugr/extensions/skimage_utilities.py` & `Draugr-1.0.9/draugr/extensions/skimage_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/ffmpeg_utilities/__init__.py` & `Draugr-1.0.9/draugr/ffmpeg_utilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 17-09-2020
            """
 
-
 from pathlib import Path
 
 try:
     from .extract import *
     from .merge import *
     from .sequencify import *
     from .split import *
```

### Comparing `Draugr-1.0.8/draugr/ffmpeg_utilities/extract.py` & `Draugr-1.0.9/draugr/ffmpeg_utilities/extract.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 from pathlib import Path
 from typing import Optional
 
-from warg import ensure_existence
 from warg import Number
+from warg import ensure_existence
 
 FORMAT_LIST = [".mp4", ".avi", ".mkv", ".flv", ".mov"]
 AUDIO_FORMAT = ".aac"
 
 __all__ = ["extract_frames"]
```

### Comparing `Draugr-1.0.8/draugr/ffmpeg_utilities/merge.py` & `Draugr-1.0.9/draugr/ffmpeg_utilities/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import os
 import subprocess
 from pathlib import Path
 from typing import Optional
 
-from warg import ensure_existence
 from draugr.ffmpeg_utilities.extract import AUDIO_FORMAT
+
 from warg import Number, identity
+from warg import ensure_existence
 
 __all__ = ["merge_frames"]
 
 
 def get_frame_format(frames_dir: Path, formats=(".jpg", ".png")) -> str:
     """
```

### Comparing `Draugr-1.0.8/draugr/ffmpeg_utilities/split.py` & `Draugr-1.0.9/draugr/ffmpeg_utilities/split.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/matlab_utilities/__init__.py` & `Draugr-1.0.9/draugr/matlab_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/matlab_utilities/conversion.py` & `Draugr-1.0.9/draugr/matlab_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/matlab_utilities/matlab_conversion_utilities.py` & `Draugr-1.0.9/draugr/matlab_utilities/matlab_conversion_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/matlab_utilities/singleton_engine.py` & `Draugr-1.0.9/draugr/matlab_utilities/singleton_engine.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/metrics/__init__.py` & `Draugr-1.0.9/draugr/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/metrics/accumulation.py` & `Draugr-1.0.9/draugr/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/metrics/meters.py` & `Draugr-1.0.9/draugr/metrics/meters.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/metrics/metric_aggregator.py` & `Draugr-1.0.9/draugr/metrics/metric_aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+import statistics
 from pathlib import Path
 from typing import List
 from warnings import warn
-import statistics
-
 
 __author__ = "Christian Heider Nielsen"
 
-
 __all__ = ["MetricAggregator", "save_metric"]
 
 MEASURES = {*statistics.__all__} - {
     "correlation",  # x,y args
     "StatisticsError",  # is an exception
     "covariance",  # x,y args
     "linear_regression",  # x,y args
     "NormalDist",  # returns list, not number
-    #'geometric_mean' # always None?
+    # 'geometric_mean' # always None?
 }
+
+
 # Check if statistics takes only one arg. TODO: Automatic function def args inspection?
 
 
 class MetricAggregator(object):
     """description"""
 
     def __init__(
@@ -165,15 +165,15 @@
                     warn(f"{e}")
                     return
         elif item == self._running_value_key:
             return self._measures[item]
         else:
             raise AttributeError
 
-    # def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+    # def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str,Any]):
     #  return self._values
 
     def __repr__(self):
         return f"<StatisticAggregator> values: {self._values}, measures: {self.measures} </StatisticAggregator>"
 
     def __str__(self):
         return str(self._values)
```

### Comparing `Draugr-1.0.8/draugr/metrics/metric_collection.py` & `Draugr-1.0.9/draugr/metrics/metric_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Christian Heider Nielsen"
 
-import statistics
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any
 
 from draugr.metrics.metric_aggregator import MetricAggregator, MEASURES
 
-
 __all__ = ["MetricCollection"]
 
 
 class MetricCollection(dict):
     """description"""
 
     def __init__(
@@ -40,15 +38,15 @@
 
         :param name:
         :type name:"""
         self._metrics[name] = MetricAggregator(
             measures=self._measures, keep_measure_history=self._keep_measure_history
         )
 
-    def append(self, *args: Sequence, **kwargs: MutableMapping):
+    def append(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """
 
         :param args:
         :type args:
         :param kwargs:
         :type kwargs:"""
         for arg, (k, v) in zip(args, self._metrics.items()):
```

### Comparing `Draugr-1.0.8/draugr/metrics/metric_summary.py` & `Draugr-1.0.9/draugr/metrics/metric_summary.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/multiprocessing_utilities/__init__.py` & `Draugr-1.0.9/draugr/multiprocessing_utilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 __author__ = "Christian Heider Nielsen"
 
 __doc__ = r"""
 """
 
 from pathlib import Path
 
-
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 
 try:
     from .pooled_queue_processor import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
```

### Comparing `Draugr-1.0.8/draugr/multiprocessing_utilities/pooled_queue_processor.py` & `Draugr-1.0.9/draugr/multiprocessing_utilities/pooled_queue_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
     def __getstate__(self):
         return cloudpickle.dumps(self._x)
 
     def __setstate__(self, x):
         self._x = pickle.loads(x)
 
-    def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         return self._x(*args, **kwargs)
 
 
 class PooledQueueTask(ABC):
     """
     Pooled queue task interface"""
 
-    def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         return self.call(*args, **kwargs)
 
     @abstractmethod
     def call(self, *args, **kwargs) -> Any:
         """
 
         :param args:
@@ -179,29 +179,29 @@
             raise exc_type(exc_val)
             # sys.exit()
 
 
 if __name__ == "__main__":
 
     class Square(PooledQueueTask):
-        def call(self, i, *args: Sequence, **kwargs: MutableMapping):
+        def call(self, i, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             """
 
             :param i:
             :type i:
             :param args:
             :type args:
             :param kwargs:
             :type kwargs:
             :return:
             :rtype:"""
             return i * 2
 
     class Exc(PooledQueueTask):
-        def call(self, *args: Sequence, **kwargs: MutableMapping):
+        def call(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             """
 
             :param args:
             :type args:
             :param kwargs:
             :type kwargs:"""
             raise NotImplementedError
```

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/__init__.py` & `Draugr-1.0.9/draugr/numpy_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/channel_transform.py` & `Draugr-1.0.9/draugr/numpy_utilities/channel_transform.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/deep_category.py` & `Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/deep_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 __author__ = "Christian Heider Nielsen"
 
 from pathlib import Path
 
 from draugr.numpy_utilities.datasets.splitting import train_valid_test_split
 from draugr.numpy_utilities.datasets.defaults import DEFAULT_ACCEPTED_FILE_FORMATS
-from typing import Iterable, Union
+from typing import Iterable, Union, Callable
 from warg import drop_unused_kws
 
 __all__ = ["build_deep_categorical_dataset"]
 
 
 @drop_unused_kws
 def build_deep_categorical_dataset(
     directory: Union[Path, str],
     *,
     validation_percentage: float = 15,
     testing_percentage: float = 0,
     extensions: Iterable = DEFAULT_ACCEPTED_FILE_FORMATS,
-    is_valid_file: callable = None,
+    is_valid_file: Callable = None,
 ) -> dict:
     """
     Builds a list of training images from the file system.
 
     Analyzes the sub folders in the image directory, splits them into stable
     training, testing, and validation sets, and returns a data structure
     describing the lists of images for each label and their paths.
```

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/flat_category.py` & `Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/flat_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 __doc__ = r"""
 
            Created on 21/07/2020
            """
 
 import os
 from pathlib import Path
-from typing import Iterable, Union
+from typing import Iterable, Union, Callable
 
 __all__ = ["build_flat_dataset"]
 
 
 def build_flat_dataset(
     directory: Union[Path, str],
     *,
     validation_percentage: float = 15,
     testing_percentage: float = 0,
     extensions: Iterable = None,
-    is_valid_file: callable = None,
+    is_valid_file: Callable = None,
 ) -> dict:
     """
 
       :param validation_percentage:
       :param testing_percentage:
     :param directory:
     :param extensions:
```

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/datasets/categorical/shallow_category.py` & `Draugr-1.0.9/draugr/numpy_utilities/datasets/categorical/shallow_category.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 import logging
 import os
 
 __author__ = "Christian Heider Nielsen"
 
 from pathlib import Path
-from typing import Dict, Sequence, Iterable, Union
+from typing import Dict, Sequence, Iterable, Union, Callable
 
 from draugr.numpy_utilities.datasets.splitting import (
     SplitEnum,
     train_valid_test_split,
 )
 from draugr.numpy_utilities.datasets.defaults import DEFAULT_ACCEPTED_FILE_FORMATS
 from warg import drop_unused_kws
@@ -21,15 +21,15 @@
 @drop_unused_kws
 def build_shallow_categorical_dataset(
     directory: Union[Path, str],
     *,
     validation_percentage: float = 15,
     testing_percentage: float = 0,
     extensions: Iterable = DEFAULT_ACCEPTED_FILE_FORMATS,
-    is_valid_file: callable = None,
+    is_valid_file: Callable = None,
     verbose: bool = False,
 ) -> Dict[str, Dict[SplitEnum, Sequence]]:
     """
     Returns:
     An OrderedDict containing an entry for each label subfolder, with images
     split into training, testing, and validation sets within each label.
     The order of items defines the class indices.
```

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/datasets/splitting.py` & `Draugr-1.0.9/draugr/numpy_utilities/datasets/splitting.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/manipulation.py` & `Draugr-1.0.9/draugr/numpy_utilities/manipulation.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/powers.py` & `Draugr-1.0.9/draugr/numpy_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/raster_grid_2d_masking.py` & `Draugr-1.0.9/draugr/numpy_utilities/raster_grid_2d_masking.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/raster_grid_3d_masking.py` & `Draugr-1.0.9/draugr/numpy_utilities/raster_grid_3d_masking.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/resize.py` & `Draugr-1.0.9/draugr/numpy_utilities/resize.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
            Created on 17/07/2020
            """
 
 from typing import Tuple
 
 import PIL.Image
 import numpy
-
 from draugr.visualisation.pillow_utilities import np_array_to_pil_img
 
 __all__ = ["resize_array"]
 
 from warg import passes_kws_to
```

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/padding.py` & `Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/padding.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/signal_mixing.py` & `Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/signal_mixing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
            Created on 17-12-2020
            """
 
 from typing import Sequence
 
 import numpy
-
-from warg import ensure_existence
 from draugr.numpy_utilities.datasets.splitting import SplitEnum
 from draugr.numpy_utilities.signal_utilities.signal_statistics import root_mean_square
 from draugr.numpy_utilities.signal_utilities.truncation import min_length_truncate_batch
 
+from warg import ensure_existence
+
 LOG_MAGNITUDE_MULTIPLIER = 20
 LOG_POWER_MULTIPLIER = 10
 
 __all__ = ["mix_ratio"]
 
 
 def mix_ratio(
```

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/signal_projection.py` & `Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/signal_projection.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/signal_statistics.py` & `Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/signal_statistics.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/numpy_utilities/signal_utilities/truncation.py` & `Draugr-1.0.9/draugr/numpy_utilities/signal_utilities/truncation.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/__init__.py` & `Draugr-1.0.9/draugr/opencv_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/bounding_boxes/boxes_2d.py` & `Draugr-1.0.9/draugr/opencv_utilities/bounding_boxes/boxes_2d.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/bounding_boxes/evaluation.py` & `Draugr-1.0.9/draugr/opencv_utilities/bounding_boxes/evaluation.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/color_space/clean.py` & `Draugr-1.0.9/draugr/opencv_utilities/color_space/clean.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum
+from typing import MutableMapping
 
 import cv2
-from sorcery import assigned_names
-from typing import MutableMapping
 from draugr.opencv_utilities.namespaces.enums import (
     MorphShapeEnum,
     MorphTypeEnum,
     BorderTypeEnum,
 )
+from sorcery import assigned_names
 
 __all__ = ["clean_up", "CleanUpMethod"]
 
 
 class CleanUpMethod(Enum):
     close, open, nclose, nopen, erode, dilate, none = assigned_names()
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/color_space/color.py` & `Draugr-1.0.9/draugr/opencv_utilities/color_space/color.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import warnings
 
 import cv2
-
 from draugr.opencv_utilities.namespaces.color_conversion_enum import (
     ColorConversionEnum,
 )
 
 __all__ = ["num_channels", "is_singular_channel", "to_color"]
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/color_space/edge.py` & `Draugr-1.0.9/draugr/opencv_utilities/color_space/edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
+from typing import MutableMapping
 
 import cv2
-from sorcery import assigned_names
-from typing import MutableMapping
 from draugr.opencv_utilities.namespaces.enums import MorphShapeEnum, MorphTypeEnum
+from sorcery import assigned_names
+
 from warg import next_odd
 
 __all__ = ["to_edge", "ToEdgeMethodEnum", "CannyApertureSize"]
 
 
 class ToEdgeMethodEnum(Enum):
     canny, laplacian, sobel_vh, sobel_h, sobel_v, morph_gradient = assigned_names()
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/color_space/gamma.py` & `Draugr-1.0.9/draugr/opencv_utilities/color_space/gamma.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/color_space/gray.py` & `Draugr-1.0.9/draugr/opencv_utilities/color_space/gray.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from enum import Enum
 
 import cv2
-from sorcery import assigned_names
-
 from draugr.opencv_utilities.color_space.color import is_singular_channel
 from draugr.opencv_utilities.namespaces.color_conversion_enum import (
     ColorConversionEnum,
 )
+from sorcery import assigned_names
 
 __all__ = ["ToGrayMethodEnum", "to_gray"]
 
 
 class ToGrayMethodEnum(Enum):
     gray, rgb, hsv, ycrcb, yuv, lab, luv = assigned_names()
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/color_space/noise.py` & `Draugr-1.0.9/draugr/opencv_utilities/color_space/noise.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/color_space/threshold.py` & `Draugr-1.0.9/draugr/opencv_utilities/color_space/threshold.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/drawing/draw_boxes.py` & `Draugr-1.0.9/draugr/opencv_utilities/drawing/draw_boxes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from pathlib import Path
 from typing import Optional, Sequence, Tuple, Union
 
 import cv2
 import numpy
 from PIL import Image, ImageDraw, ImageFont
-
 from draugr.opencv_utilities.drawing.opencv_draw import draw_masks
+
 from warg import RGB, compute_color_for_labels
 
 __all__ = ["draw_single_box", "draw_bounding_boxes", "draw_single_rect"]
 
 
 def draw_single_box(
     image: Image.Image,
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/drawing/masks/gauss_circles.py` & `Draugr-1.0.9/draugr/opencv_utilities/drawing/masks/gauss_circles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import math
 
 import cv2
 import numpy
-
 from draugr.opencv_utilities import LineTypeEnum
 
 
 # ============================================================================
 
 
 def ellipse_bbox(h, k, a, b, theta):
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/drawing/masks/segment_ellipse.py` & `Draugr-1.0.9/draugr/opencv_utilities/drawing/masks/segment_ellipse.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/drawing/opencv_draw.py` & `Draugr-1.0.9/draugr/opencv_utilities/drawing/opencv_draw.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
            """
 
 from typing import Sequence, Tuple, Union
 
 import cv2
 import numpy
 from PIL import Image
-
 from draugr.opencv_utilities.namespaces.enums import (
     LineTypeEnum,
     ContourRetrievalModeEnum,
 )
+
 from warg import RGB, compute_color_for_labels
 
 __all__ = ["find_contours", "draw_masks"]
 
 
 def find_contours(*args, **kwargs) -> Tuple:
     """
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/drawing/opencv_drawing_utilities.py` & `Draugr-1.0.9/draugr/opencv_utilities/drawing/opencv_drawing_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/namespaces/color_conversion_enum.py` & `Draugr-1.0.9/draugr/opencv_utilities/namespaces/color_conversion_enum.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/namespaces/enums.py` & `Draugr-1.0.9/draugr/opencv_utilities/namespaces/enums.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/namespaces/flags.py` & `Draugr-1.0.9/draugr/opencv_utilities/namespaces/flags.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/async_video_stream.py` & `Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/async_video_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self._stopped = True  # indicate that the thread should be stopped
 
     # noinspection PyPep8Naming
     def isOpened(self) -> bool:
         """Returns whether the stream is open"""
         return self._stream.isOpened()
 
-    def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         return self.frame
 
     def __next__(self):
         return self.frame
 
     def __iter__(self) -> "AsyncVideoStream":
         return self.start()
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/frame_annotation.py` & `Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/frame_annotation.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/frames.py` & `Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/frames.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/raster_sequences/video_sources.py` & `Draugr-1.0.9/draugr/opencv_utilities/raster_sequences/video_sources.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/transformation/__init__.py` & `Draugr-1.0.9/draugr/opencv_utilities/transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/transformation/cropping.py` & `Draugr-1.0.9/draugr/opencv_utilities/transformation/cropping.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/transformation/cv2_transforms.py` & `Draugr-1.0.9/draugr/opencv_utilities/transformation/cv2_transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import types
-from typing import Any, List, Tuple
+from typing import Any, List, Tuple, Callable
 
 import cv2
 import numpy
 from PIL.ImageTransform import Transform
 from numpy import random
 
 __all__ = [
@@ -54,15 +54,15 @@
                 boxes, labels = remove_null_boxes(boxes, labels)
         return img, boxes, labels
 
 
 class Lambda(object):
     """Applies a lambda as a transform."""
 
-    def __init__(self, lambd: callable):
+    def __init__(self, lambd: Callable):
         assert isinstance(lambd, types.LambdaType)
         self.lambd = lambd
 
     def __call__(self, img: Any, boxes: Any = None, labels: Any = None):
         return self.lambd(img, boxes, labels)
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/transformation/resize.py` & `Draugr-1.0.9/draugr/opencv_utilities/transformation/resize.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/windows/color_picker.py` & `Draugr-1.0.9/draugr/opencv_utilities/windows/color_picker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pathlib import Path
 from typing import Iterable
 
 import cv2
 import numpy
-
 from draugr.opencv_utilities.color_space.threshold import hsv_min_max_clip_mask
 from draugr.opencv_utilities.windows.elements import add_trackbar
 from draugr.opencv_utilities.windows.image import show_image
 
 __all__ = ["interactive_hsv_color_picker"]
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/windows/elements/button.py` & `Draugr-1.0.9/draugr/opencv_utilities/windows/elements/button.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Optional
+from typing import Callable
 
 import cv2
+from draugr.opencv_utilities import ButtonTypeEnum
 
 from warg import sink
-from draugr.opencv_utilities import ButtonTypeEnum
 
 __all__ = ["add_button"]
 
 
 def add_button(
-    checkbox_name: str, *, callback: callable = sink, new_line: bool = True
+    checkbox_name: str, *, callback: Callable = sink, new_line: bool = True
 ) -> None:
     """
     :param checkbox_name:
     :type checkbox_name:
     :param new_line:
     :type new_line:
     :param callback: Callback function to be called when the button is pressed.
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/windows/elements/checkbox.py` & `Draugr-1.0.9/draugr/opencv_utilities/windows/elements/checkbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Optional
+from typing import Callable
 
 import cv2
+from draugr.opencv_utilities import ButtonTypeEnum
 
 from warg import sink
-from draugr.opencv_utilities import ButtonTypeEnum
 
 __all__ = ["add_checkbox"]
 
 
 def add_checkbox(
     checkbox_name: str,
     *,
     initial_button_state: bool = False,
-    callback: callable = sink,
+    callback: Callable = sink,
     new_line: bool = True
 ) -> None:
     """
 
     :param checkbox_name:
     :type checkbox_name:
     :param initial_button_state:
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/windows/elements/trackbar.py` & `Draugr-1.0.9/draugr/opencv_utilities/windows/elements/trackbar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, Callable
 
 import cv2
 
 from warg import sink, Number
 
 __all__ = ["add_trackbar"]
 
@@ -10,15 +10,15 @@
 def add_trackbar(
     window_name: str,
     trackbar_name: str,
     default: Optional[Number] = None,
     *,
     min_val: Number = 0,
     max_val: Number = 255,
-    callback: callable = sink
+    callback: Callable = sink
 ) -> None:
     """
     Adds a trackbar to a window.
     :param default:
     :type default:
     :param min_val:
     :type min_val:
```

### Comparing `Draugr-1.0.8/draugr/opencv_utilities/windows/image.py` & `Draugr-1.0.9/draugr/opencv_utilities/windows/image.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/__init__.py` & `Draugr-1.0.9/draugr/os_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/cuda_device.py` & `Draugr-1.0.9/draugr/os_utilities/cuda_device.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/__init__.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/gnome_utilities/dark_mode.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/gnome_utilities/dark_mode.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/gtk_utilities/__init__.py` & `Draugr-1.0.9/draugr/os_utilities/mac_utilities/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
-           Created on 03/08/2020
+           Created on 30-08-2020
            """
 
 from pathlib import Path
 
-from draugr import INCLUDE_PROJECT_READMES
-
-if INCLUDE_PROJECT_READMES:
-    with open(Path(__file__).parent / "README.md", "r") as this_init_file:
-        __doc__ += this_init_file.read()
-
+with open(Path(__file__).parent / "README.md", "r") as this_init_file:
+    __doc__ += this_init_file.read()
+# del Path
 
 try:
-    from .gtk_settings import *
-    from .theme_preferences import *
+    from .dark_mode import *
+
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = (
-        Path(__file__).parent.parent.parent
+        Path(__file__).parent.parent.parent.parent
         / "requirements"
         / f"requirements_{this_package_name}.txt"
     )
     if this_package_reqs.exists():
         print(
             f"Make sure requirements is installed for {this_package_name}, see {this_package_reqs}"
         )  # TODO: PARSE WHAT is missing and print
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/gtk_utilities/gtk_settings.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/gtk_utilities/gtk_settings.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/gtk_utilities/theme_preferences.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/gtk_utilities/theme_preferences.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/systemd_utilities/__init__.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if INCLUDE_PROJECT_READMES:
     with open(Path(__file__).parent / "README.md", "r") as this_init_file:
         __doc__ += this_init_file.read()
 
 try:
     from .service_management import *
     from .service_template import *
+    from .timer_template import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = (
         Path(__file__).parent.parent.parent
         / "requirements"
         / f"requirements_{this_package_name}.txt"
     )
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/systemd_utilities/service_management.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/service_management.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 
 import getpass
 import sys
 from enum import Enum
 from pathlib import Path
 
 import sh  # pip install sh
+from draugr import PROJECT_NAME
+from draugr.os_utilities.linux_utilities.user_utilities import make_user, remove_user
 from sorcery import assigned_names
 
-from draugr import PROJECT_NAME
+from warg import ContextWrapper
 from .service_template import (
     SERVICE_TEMPLATE,
 )
-from draugr.os_utilities.linux_utilities.user_utilities import make_user, remove_user
-from warg import ContextWrapper
 
 
 class RunAsEnum(Enum):
     """description"""
 
     user, app_user, root = assigned_names()
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/systemd_utilities/service_template.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/systemd_utilities/service_template.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,14 +39,50 @@
 Type=simple
 ExecStart={app_path}
 
 [Install]
 WantedBy=default.target
 """
 
+SERVICE_TEMPLATE_USER_ONESHOT = """
+[Unit]
+Description={app} Service
+After=docker.service app.target
+Upholds=app.target
+
+
+[Service]
+Type=oneshot
+RemainAfterExit=false
+ExecStart={app_path}
+
+[Install]
+WantedBy={app}.target
+"""
+
+TARGET_TEMPLATE_USER_ONESHOT = """
+[Unit]
+Description={app} target unit
+StopWhenUnneeded=true
+"""
+
+TIMER_TEMPLATE_USER = """
+[Unit]
+Description=Try to run {app} everyday at 00:00:00
+
+[Timer]
+#every 10 minutes
+OnCalendar=*:0/10
+
+Unit={app}.target
+
+[Install]
+WantedBy=timers.target
+"""
+
 SERVICE_TEMPLATE_SIMPLE = """
 [Unit]
 Description={service_name} Service
 After=multi-user.target
 
 [Service]
 Type=simple
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/linux_utilities/user_utilities.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/user_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/mac_utilities/__init__.py` & `Draugr-1.0.9/draugr/os_utilities/windows_utilities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from pathlib import Path
 
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 # del Path
 
 try:
-    from .dark_mode import *
+    from .windows_settings import *
+    from .task_scheduler import *
 
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = (
         Path(__file__).parent.parent.parent.parent
         / "requirements"
         / f"requirements_{this_package_name}.txt"
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/mac_utilities/dark_mode.py` & `Draugr-1.0.9/draugr/os_utilities/mac_utilities/dark_mode.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/resource_utilities/__init__.py` & `Draugr-1.0.9/draugr/os_utilities/resource_utilities/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 17-05-2021
            """
 
-
 from pathlib import Path
 
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 # del Path
 
 try:
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/resource_utilities/all.py` & `Draugr-1.0.9/draugr/os_utilities/resource_utilities/all.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/resource_utilities/cpu.py` & `Draugr-1.0.9/draugr/os_utilities/resource_utilities/cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
             Small path_utilities to keep track of cores dedicated to workers threads
 
            Created on 07-12-2020
            """
 
 import os
 from typing import MutableMapping
+
 from warg import AlsoDecorator, passes_kws_to
 
 CORE_COUNT: int = os.cpu_count()
 IN_USE_BY_THIS_PROCESS: int = 0
 
 __all__ = [
     "request_worker_cores",
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/resource_utilities/ram.py` & `Draugr-1.0.9/draugr/os_utilities/resource_utilities/ram.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/screen_resolution.py` & `Draugr-1.0.9/draugr/os_utilities/screen_resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     "screen_res_pygame",
     "screen_res_gtk",
     "screen_res_xlib",
     "screen_res_mac",
     "screen_res_win",
 ]
 
-
 import sys
 
 
 def screen_res_xlib():
     """
 
     :return:
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/windows_utilities/__init__.py` & `Draugr-1.0.9/draugr/scipy_utilities/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
-           Created on 30-08-2020
+           Created on 08-02-2021
            """
 
 from pathlib import Path
 
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 # del Path
-
 try:
-    from .windows_settings import *
-    from .task_scheduler import *
-
+    from .subsampling import *
+    from .scipy_utilities import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = (
-        Path(__file__).parent.parent.parent.parent
+        Path(__file__).parent.parent.parent
         / "requirements"
         / f"requirements_{this_package_name}.txt"
     )
     if this_package_reqs.exists():
         print(
             f"Make sure requirements is installed for {this_package_name}, see {this_package_reqs}"
         )  # TODO: PARSE WHAT is missing and print
```

### Comparing `Draugr-1.0.8/draugr/os_utilities/windows_utilities/task_scheduler/api.py` & `Draugr-1.0.9/draugr/os_utilities/windows_utilities/task_scheduler/api.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/windows_utilities/win32/api.py` & `Draugr-1.0.9/draugr/os_utilities/windows_utilities/win32/api.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/windows_utilities/win32/gui.py` & `Draugr-1.0.9/draugr/os_utilities/windows_utilities/win32/gui.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/os_utilities/windows_utilities/windows_settings.py` & `Draugr-1.0.9/draugr/os_utilities/windows_utilities/windows_settings.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/pandas_utilities/__init__.py` & `Draugr-1.0.9/draugr/pandas_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/pandas_utilities/formatting.py` & `Draugr-1.0.9/draugr/pandas_utilities/formatting.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/pandas_utilities/from_dict.py` & `Draugr-1.0.9/draugr/pandas_utilities/from_dict.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/pandas_utilities/latex_mean_std.py` & `Draugr-1.0.9/draugr/pandas_utilities/latex_mean_std.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
            """
 
 import random
 from functools import partial
 
 import numpy
 import pandas
-
 from draugr.pandas_utilities.formatting import pandas_mean_std_bold_formatter
+
 from warg import Number, drop_unused_kws, passes_kws_to
 from warg import indent_lines
 
 __all__ = [
     "pandas_mean_std",
     "pandas_mean_std_to_str",
     "pandas_format_bold_max_row_latex",
@@ -223,15 +223,15 @@
             f"\\rotatebox{{{header_rotation}}}" + "{" + "\_".join(c.split("_")) + "}"
             for c in entry_provider_df.columns
         ]
     else:
         header = True
 
     with pandas.option_context("max_colwidth", max_colwidth):
-        return entry_provider_df.to_latex(
+        return entry_provider_df.to_latex(  # TODO: change to DataFrame.style.to_latex
             index=True,
             index_names=[*entry_provider_df.index.names],
             escape=False,
             formatters=formatters,
             header=header,
         )  # .replace('textbackslash ', '').replace('\$', '$')
```

### Comparing `Draugr-1.0.8/draugr/pandas_utilities/misc_utilities.py` & `Draugr-1.0.9/draugr/pandas_utilities/misc_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/pandas_utilities/multi_index_utilities.py` & `Draugr-1.0.9/draugr/pandas_utilities/multi_index_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/pandas_utilities/styling.py` & `Draugr-1.0.9/draugr/pandas_utilities/styling.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from enum import Enum
 from pathlib import Path
 from typing import List, Union
 
 from pandas.core.generic import NDFrame
 from sorcery import assigned_names
 
-from warg import ensure_existence
 from warg import Number
+from warg import ensure_existence
 
 __all__ = [
     "color_highlight_extreme",
     "ColorEnum",
     "NDFrameExtremeEnum",
     "AttrEnum",
     "color_negative_red",
```

### Comparing `Draugr-1.0.8/draugr/pygame_utilities/__init__.py` & `Draugr-1.0.9/draugr/pygame_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/__init__.py` & `Draugr-1.0.9/draugr/python_utilities/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
            Created on 14/01/2020
            """
 
 # with open(Path(__file__).parent / "README.md", "r") as this_init_file:
 #    __doc__ += this_init_file.read()  # .replace("#", "")  # .encode("ascii", "ignore")
 
 
+from .counter_filter import *
+from .display import *
 from .function_wrappers import *
 from .generators import *
 from .http import *
-from .sockets import *
-from .torch_like_channel_transformation import *
-from .counter_filter import *
-from .matrix import *
 from .iterators import *
-from .display import *
+from .matrix import *
 from .platform_context import *
+from .sockets import *
+from .torch_like_channel_transformation import *
```

### Comparing `Draugr-1.0.8/draugr/python_utilities/broadcasting.py` & `Draugr-1.0.9/draugr/python_utilities/broadcasting.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/counter_filter.py` & `Draugr-1.0.9/draugr/python_utilities/counter_filter.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/display.py` & `Draugr-1.0.9/draugr/python_utilities/display.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/function_wrappers.py` & `Draugr-1.0.9/draugr/python_utilities/function_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     "min_interval_wrapper",
     "min_interval_wrapper_global",
     "max_frequency",
     "wrap_args",
 ]
 
 from collections import namedtuple
-from typing import MutableMapping, Tuple, Any
+from typing import MutableMapping, Tuple, Any, Callable
 
 import wrapt
 
 
-def min_interval_wrapper(f: callable, min_interval: int = 100) -> callable:
+def min_interval_wrapper(f: Callable, min_interval: int = 100) -> callable:
     """
     to ensure that a function is now being called more often than max_freq, TODO: use proper naming for the interval
     :param f:
     :param min_interval:
     :return:
     """
 
@@ -50,15 +50,15 @@
 
 
 max_frequency_wrapper = min_interval_wrapper
 
 _GLOBAL_COUNTERS = {}
 
 
-def min_interval_wrapper_global(f: callable, min_interval: int = 100) -> callable:
+def min_interval_wrapper_global(f: Callable, min_interval: int = 100) -> callable:
     """
     to ensure that a function is now being called more often than max_freq, TODO: use proper naming for the interval
     :param f:
     :param min_interval:
     :return:
     """
```

### Comparing `Draugr-1.0.8/draugr/python_utilities/generators/batching_generator.py` & `Draugr-1.0.9/draugr/python_utilities/generators/batching_generator.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/generators/recycling_generator.py` & `Draugr-1.0.9/draugr/python_utilities/generators/recycling_generator.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/iterators.py` & `Draugr-1.0.9/draugr/python_utilities/iterators.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 __doc__ = r"""
 
            Created on 8/10/22
            """
 
 __all__ = ["BidirectionalIterator", "prev"]
 
-
 from typing import Iterator, Any
 
 
 class BidirectionalIterator(Iterator):
     """
     Enable iteration forward and backward
```

### Comparing `Draugr-1.0.8/draugr/python_utilities/matrix.py` & `Draugr-1.0.9/draugr/python_utilities/matrix.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/platform_context.py` & `Draugr-1.0.9/draugr/python_utilities/platform_context.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/sockets.py` & `Draugr-1.0.9/draugr/python_utilities/sockets.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/python_utilities/torch_like_channel_transformation.py` & `Draugr-1.0.9/draugr/python_utilities/torch_like_channel_transformation.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/random_utilities/seeding.py` & `Draugr-1.0.9/draugr/random_utilities/seeding.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/scipy_utilities/__init__.py` & `Draugr-1.0.9/draugr/visualisation/progress/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
-           Created on 08-02-2021
+           Created on 08-12-2020
            """
 
 from pathlib import Path
 
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 # del Path
 try:
-    from .subsampling import *
-    from .scipy_utilities import *
+    from .progress_bar import *
+    from .pooled_progress_bar import *
+
+    # from .eta_bar import # IT is super shit
+    from .pick import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = (
         Path(__file__).parent.parent.parent
         / "requirements"
         / f"requirements_{this_package_name}.txt"
     )
```

### Comparing `Draugr-1.0.8/draugr/scipy_utilities/scipy_utilities.py` & `Draugr-1.0.9/draugr/scipy_utilities/scipy_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/scipy_utilities/subsampling.py` & `Draugr-1.0.9/draugr/scipy_utilities/subsampling.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/stopping/stopping_key.py` & `Draugr-1.0.9/draugr/stopping/stopping_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = ""
 
 __all__ = ["add_early_stopping_key_combination", "CaptureEarlyStop"]
 
 import contextlib
 from time import sleep
-from typing import Callable, Iterable, Sequence, MutableMapping
+from typing import Callable, Iterable, Sequence, MutableMapping, Any
 
 from pynput.keyboard import KeyCode
 
 from warg import GDKC, drop_unused_kws, passes_kws_to, sprint
 
 # import keyboard
 
@@ -100,15 +100,15 @@
 
 
 class CaptureEarlyStop(contextlib.AbstractContextManager):
     """
     Context for early stopping a loop"""
 
     @passes_kws_to(add_early_stopping_key_combination)
-    def __init__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __init__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         self.listener = add_early_stopping_key_combination(*args, **kwargs)
 
     def __enter__(self):
         if self.listener:
             self.listener.start()
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `Draugr-1.0.8/draugr/tensorboard_utilities/__init__.py` & `Draugr-1.0.9/draugr/tensorboard_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/tensorboard_utilities/experimental/confusion_matrix.py` & `Draugr-1.0.9/draugr/tensorboard_utilities/experimental/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/tensorboard_utilities/experimental/pretty_cf.py` & `Draugr-1.0.9/draugr/tensorboard_utilities/experimental/pretty_cf.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/tensorboard_utilities/exporting/db_export.py` & `Draugr-1.0.9/draugr/tensorboard_utilities/exporting/db_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 __doc__ = r"""
 
             TODO: Finish this off, only a placeholder for now
 
            Created on 17-03-2021
            """
 
+from typing import Sequence, MutableMapping, Any
+
 from draugr.tensorboard_utilities.exporting.event_export import TensorboardEventExporter
-from typing import Sequence, MutableMapping
 
 
 class TensorboardEventExporterDatabase(TensorboardEventExporter):
-    def __init__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __init__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         super().__init__(*args, **kwargs)
         postgres_db = kwargs.get("postgres_db")
         if postgres_db is not None:
             self.database = postgres_db
         else:
             raise ValueError("No postgres_db provided")
```

### Comparing `Draugr-1.0.8/draugr/tensorboard_utilities/exporting/event_export.py` & `Draugr-1.0.9/draugr/tensorboard_utilities/exporting/event_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from itertools import zip_longest
 from pathlib import Path
 from pickle import dump
 from typing import Iterable, Mapping, Tuple, TypeVar, Union, Sequence
 
 import numpy
 import pandas
-
 from PIL.Image import Image
 from matplotlib import pyplot
 
-
 from apppath import AppPath
 
 __all__ = ["TensorboardEventExporter"]
 
 from warg import passes_kws_to, ensure_existence
 
 # TODO: implement export options using ExportMethodEnum
```

### Comparing `Draugr-1.0.8/draugr/tensorboard_utilities/exporting/file_export.py` & `Draugr-1.0.9/draugr/tensorboard_utilities/exporting/file_export.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 __doc__ = r"""
 
             TODO: Finish this off, only a placeholder for now
 
            Created on 17-03-2021
            """
 
+from typing import Sequence, MutableMapping, Any
+
 from draugr.tensorboard_utilities.exporting.event_export import TensorboardEventExporter
-from typing import Sequence, MutableMapping
 
 
 class TensorboardEventExporterFile(TensorboardEventExporter):
-    def __init__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __init__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         super().__init__(*args, **kwargs)
         self.file = kwargs.get("file")
         if self.file is not None:
             self.file.write("")
         else:
             raise ValueError("No file provided")
```

### Comparing `Draugr-1.0.8/draugr/threading_utilities/__init__.py` & `Draugr-1.0.9/draugr/threading_utilities/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
            """
 
 from pathlib import Path
 
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 
-
 try:
     from .skipper import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = (
         Path(__file__).parent.parent.parent
         / "requirements"
```

### Comparing `Draugr-1.0.8/draugr/threading_utilities/skipper.py` & `Draugr-1.0.9/draugr/threading_utilities/skipper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import queue
 import threading
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any
 
 __all__ = ["Skipper"]
 
 
 class Skipper:
     """description"""
 
@@ -30,15 +30,15 @@
         self._stop = True
         try:
             self.Q.put_nowait((None, None))
         except:
             pass
         self.thread.join()
 
-    def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         while not self.Q.empty():
             self.Q.get_nowait()
         self.Q.put((args, kwargs))
 
 
 if __name__ == "__main__":
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/__init__.py` & `Draugr-1.0.9/draugr/torch_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/architecture.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/architecture.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/distributional/categorical.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/distributional/categorical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from typing import List, Tuple
 
 import numpy
 import torch
-from torch.distributions import Categorical
-from torch.nn import functional
-
 from draugr.torch_utilities.architectures.mlp import MLP
 from draugr.torch_utilities.tensors.to_tensor import to_tensor
+from torch.distributions import Categorical
+from torch.nn import functional
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 """
 __all__ = ["MultipleCategoricalMLP", "CategoricalMLP"]
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/distributional/normal.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/distributional/normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import time
-from typing import List, Sequence, MutableMapping
+from typing import List, Sequence, MutableMapping, Callable
 
 import torch
-from torch import nn
-from torch.distributions import MultivariateNormal, Normal
-
 from draugr.torch_utilities.architectures.mlp import MLP
 from draugr.torch_utilities.optimisation.parameters.initialisation import fan_in_init
+from torch import nn
+from torch.distributions import MultivariateNormal, Normal
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = ""
 __all__ = [
     "ShallowStdNormalMLP",
     "MultiDimensionalNormalMLP",
     "MultiVariateNormalMLP",
@@ -24,15 +23,15 @@
 
 class ShallowStdNormalMLP(MLP):
     """description"""
 
     def __init__(
         self,
         output_shape: Sequence = (2,),
-        mean_head_activation: callable = None,
+        mean_head_activation: Callable = None,
         fixed_log_std: torch.Tensor = None,
         **kwargs
     ):
         super().__init__(
             output_shape=output_shape,
             mean_head_activation=mean_head_activation,
             **kwargs
@@ -74,15 +73,15 @@
 
 class ShallowStdMultiVariateNormalMLP(MLP):
     """description"""
 
     def __init__(
         self,
         output_shape: Sequence = (2,),
-        mean_head_activation: callable = None,
+        mean_head_activation: Callable = None,
         fixed_log_std: torch.Tensor = None,
         **kwargs: MutableMapping
     ):
         super().__init__(
             output_shape=output_shape,
             mean_head_activation=mean_head_activation,
             **kwargs
@@ -121,15 +120,15 @@
 
 class MultiDimensionalNormalMLP(MLP):
     """description"""
 
     def __init__(
         self,
         output_shape: Sequence = (2,),
-        mean_head_activation: callable = None,
+        mean_head_activation: Callable = None,
         **kwargs: MutableMapping
     ):
         output_shape = (*output_shape, *output_shape)
         assert len(output_shape) == 2
 
         self.mean_head_activation = mean_head_activation
         super().__init__(
@@ -162,15 +161,15 @@
 class MultiVariateNormalMLP(MLP):
     """description"""
 
     @passes_kws_to(MLP.__init__)
     def __init__(
         self,
         output_shape: Sequence = (2,),
-        mean_head_activation: callable = None,
+        mean_head_activation: Callable = None,
         **kwargs: MutableMapping
     ):
         output_shape = (*output_shape, *output_shape)
         assert len(output_shape) == 2
 
         self.mean_head_activation = mean_head_activation
         super().__init__(output_shape=output_shape, **kwargs)
@@ -202,15 +201,15 @@
 
 class MultipleNormalMLP(MLP):
     """description"""
 
     def __init__(
         self,
         output_shape: int = 2,
-        mean_head_activation: callable = None,
+        mean_head_activation: Callable = None,
         **kwargs: MutableMapping
     ):
         output_shape = (2,) * output_shape
         super().__init__(output_shape=output_shape, **kwargs)
 
         self.mean_head_activation = mean_head_activation
         fan_in_init(self)
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/heads.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/heads.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/experimental/layers/radial_basis.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/experimental/layers/radial_basis.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/mlp.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import logging
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any, Callable, Iterable
 
 import numpy
 import torch
-from numpy import prod
-from torch import nn
-from torch.nn import Module
-
 from draugr.random_utilities import seed_stack
 from draugr.torch_utilities.architectures.architecture import Architecture
 from draugr.torch_utilities.optimisation.parameters.initialisation import (
     constant_init,
     fan_in_init,
 )
 from draugr.torch_utilities.tensors.to_tensor import to_tensor
+from numpy import prod
+from torch import nn
+from torch.nn import Module
+
 from warg import NOD
 
 __author__ = "Christian Heider Nielsen"
 
 __doc__ = r"""
 Description: Multi Layer Perceptron
 Author: Christian Heider Nielsen
@@ -47,17 +47,17 @@
         output_shape: Sequence[int] = None,
         output_activation: Module = torch.nn.Identity(),
         use_bias: bool = True,
         use_dropout: bool = False,
         dropout_prob: float = 0.2,
         auto_build_hidden_layers_if_none=True,
         input_multiplier: int = 32,
-        max_layer_width=1000,
+        max_layer_width: int = 1000,
         output_multiplier: int = 16,
-        default_init: callable = fan_in_init,
+        default_init: Callable = fan_in_init,
         # prefix:str=None, #TODO name sub networks
         **kwargs: MutableMapping,
     ):
         assert input_shape is not None
         assert output_shape is not None
 
         input_shape = self.infer_input_shape(input_shape)
@@ -121,16 +121,16 @@
             )
 
         if default_init:
             default_init(self)
 
     @staticmethod
     def construct_progressive_hidden_layers(
-        _input_shape,
-        _output_shape,
+        _input_shape: Iterable,
+        _output_shape: Iterable,
         input_multiplier: float = 32,
         output_multiplier: float = 16,
         max_layer_width: int = 1000,
     ) -> Sequence[nn.Module]:
         """
 
         :param _input_shape:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/concatination.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/concatination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from typing import Iterable, List, Sequence, MutableMapping
 
 import numpy
 import torch
-
 from draugr.torch_utilities.architectures.mlp import MLP
 from draugr.torch_utilities.tensors.to_tensor import to_tensor
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = "Fusion variant of MLPs"
 
 __all__ = ["PreConcatInputMLP", "LateConcatInputMLP"]
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/disjunction.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/disjunction.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/experimental/recurrent.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/experimental/recurrent.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 __doc__ = r"""
 
            Created on 8/24/22
            """
 
 __all__ = []
 
-
-from typing import MutableMapping, Sequence, Tuple
+from typing import MutableMapping, Sequence
 
 import torch
+from draugr.torch_utilities.architectures.mlp import MLP
 from torch import nn
 from torch.nn import functional
 
-from draugr.torch_utilities.architectures.mlp import MLP
-
 
 class RecurrentCategoricalMLP(MLP):
     """
     Recurrent model base the MLP base model
     """
 
     def __init__(self, r_hidden_layers=10, **kwargs: MutableMapping):
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/mlp_variants/fourier.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/mlp_variants/fourier.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/recurrent/experimental/recurrent.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/recurrent/experimental/recurrent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = ""
 
-from typing import MutableMapping, Sequence, Tuple
+from typing import Tuple
 
 import torch
 from torch import nn
-from torch.nn import functional
-
-from draugr.torch_utilities.architectures.mlp import MLP
 
 
 class RecurrentBase(nn.Module):
     """
     A base class for Recurrent models
     """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/architectures/vae.py` & `Draugr-1.0.9/draugr/torch_utilities/architectures/vae.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 __author__ = "heider"
 __doc__ = r"""
 
            Created on 9/22/22
            """
 
-
 __all__ = ["VariationalAutoEncoder"]
 
 from abc import abstractmethod
 
 import torch
 from draugr.torch_utilities.tensors.to_tensor import to_tensor
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/datasets/non_sequential_dataset.py` & `Draugr-1.0.9/draugr/torch_utilities/datasets/non_sequential_dataset.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/datasets/random_dataset.py` & `Draugr-1.0.9/draugr/torch_utilities/datasets/random_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
            Created on 09/10/2019
            """
 
 __all__ = ["RandomDataset"]
 
 
 class RandomDataset(Dataset):
-    """description"""
+    """Random dataset on instantiation"""
 
     def __init__(self, nd_size: Sequence, length: int):
         self.len = length
         self.data = torch.randn((length, *nd_size))
 
     def __getitem__(self, index: int) -> Any:
         return self.data[index]
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/categorical_dataset.py` & `Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/categorical_dataset.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/supervised_dataset.py` & `Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/supervised_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     SplitIndexer,
 )
 from warg import drop_unused_kws
 
 
 class SupervisedDataset(Dataset):
     """
-    Supervised Dataset is comprised of separate Splits"""
+    Supervised Dataset comprises separate Splits"""
 
     @drop_unused_kws
     def __init__(self):
         pass
 
     @property
     def split_names(self) -> Dict[SplitEnum, str]:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/datasets/supervised/vision_datasets/dict_dataset.py` & `Draugr-1.0.9/draugr/torch_utilities/datasets/supervised/vision_datasets/dict_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __doc__ = r"""
 
            Created on 21/07/2020
            """
 
 import random
 from pathlib import Path
-from typing import Iterable, Tuple
+from typing import Iterable, Tuple, Callable
 
 from torch.utils.data import DataLoader
 from torchvision.datasets import VisionDataset  # TODO: Do not need to be images
 
 __all__ = ["DictDatasetFolder", "SplitDictDatasetFolder"]
 
 from torchvision.datasets.folder import has_file_allowed_extension
@@ -56,20 +56,20 @@
     _data_categories (list): List of (sample path, class_index) tuples"""
 
     def __init__(
         self,
         root: Path,
         loader: DataLoader,
         extensions: Iterable = None,
-        transform: callable = None,
-        target_transform: callable = None,
+        transform: Callable = None,
+        target_transform: Callable = None,
         split: SplitEnum = SplitEnum.training,
         valid_percentage: float = 15,
         test_percentage: float = 0,
-        is_valid_file: callable = has_file_allowed_extension,
+        is_valid_file: Callable = has_file_allowed_extension,
     ):
         super().__init__(
             str(root), transform=transform, target_transform=target_transform
         )
         # TODO: merge Split and non split common in a base class
         self._data_categories = select_split(
             build_shallow_categorical_dataset(
@@ -154,17 +154,17 @@
     _data (list): List of (sample path, class_index) tuples"""
 
     def __init__(
         self,
         root: Path,
         loader: DataLoader,
         extensions: Iterable = None,
-        transform: callable = None,
-        target_transform: callable = None,
-        is_valid_file: callable = has_file_allowed_extension,
+        transform: Callable = None,
+        target_transform: Callable = None,
+        is_valid_file: Callable = has_file_allowed_extension,
     ):
         super().__init__(
             str(root), transform=transform, target_transform=target_transform
         )
         # TODO: merge Split and non split common in a base class
         self._data = build_flat_dataset(
             self.root, extensions=extensions, is_valid_file=is_valid_file
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/distributions/entropy.py` & `Draugr-1.0.9/draugr/torch_utilities/distributions/entropy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import math
 
 import torch
-
 from draugr.torch_utilities.system.constants import torch_pi
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 09/10/2019
            """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/evaluation/archetypes.py` & `Draugr-1.0.9/draugr/torch_utilities/evaluation/archetypes.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/evaluation/classification.py` & `Draugr-1.0.9/draugr/torch_utilities/evaluation/classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 02-12-2020
            """
 
+from typing import Callable
+
 import torch
+from draugr.torch_utilities.sessions.model_sessions import TorchEvalSession
+from draugr.torch_utilities.system.device import global_torch_device
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-from draugr.torch_utilities.sessions.model_sessions import TorchEvalSession
-from draugr.torch_utilities.system.device import global_torch_device
 from warg import kws_sink
 
 __all__ = ["find_n_misclassified"]
 
 
 def find_n_misclassified(
     model: torch.nn.Module,
     evaluation_loader: DataLoader,
     *,
-    mapper: callable = kws_sink,
+    mapper: Callable = kws_sink,
     n: int = 10,
     device: torch.device = global_torch_device(),
 ) -> None:
     """description"""
     j = 0
     num_samples = len(evaluation_loader)
     with TorchEvalSession(model):
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/evaluation/cross_validation.py` & `Draugr-1.0.9/draugr/torch_utilities/evaluation/cross_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,18 @@
            """
 
 __all__ = ["cross_validation_generator"]
 
 from typing import Tuple
 
 import torch
+from draugr.torch_utilities.tensors.to_tensor import to_tensor
 from sklearn.model_selection import KFold
 from torch.utils.data import ConcatDataset, Dataset, Subset, TensorDataset
 
-from draugr.torch_utilities.tensors.to_tensor import to_tensor
-
 
 def cross_validation_generator(
     *datasets: Dataset, n_splits: int = 10
 ) -> Tuple[Subset, Subset]:
     """
     Learning the parameters of a prediction function and testing it on the same data is a methodological mistake: a model that would just repeat the labels of the samples that it has just seen would have a perfect score but would fail to predict anything useful on yet-unseen data. This situation is called overfitting. To avoid it, it is common practice when performing a (supervised) machine learning experiment to hold out part of the available data as a test set
     """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/exporting/latex_tables.py` & `Draugr-1.0.9/draugr/torch_utilities/exporting/latex_tables.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/exporting/summary.py` & `Draugr-1.0.9/draugr/torch_utilities/exporting/summary.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/generators/batching.py` & `Draugr-1.0.9/draugr/torch_utilities/generators/batching.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/generators/to_tensor_generator.py` & `Draugr-1.0.9/draugr/torch_utilities/generators/to_tensor_generator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from typing import Iterable, Iterator, Tuple, Union, MutableMapping
 
 import numpy
 import torch
-from torch.utils.data.dataloader import DataLoader
-
 from draugr.torch_utilities.datasets import NonSequentialDataset
 from draugr.torch_utilities.tensors import to_tensor
+from torch.utils.data.dataloader import DataLoader
+
 from warg import passes_kws_to
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 28/10/2019
            """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/images/channel_transform.py` & `Draugr-1.0.9/draugr/torch_utilities/images/channel_transform.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/images/conversion.py` & `Draugr-1.0.9/draugr/torch_utilities/images/conversion.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/opencv/torch_conversion.py` & `Draugr-1.0.9/draugr/torch_utilities/opencv/torch_conversion.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/operations/activations.py` & `Draugr-1.0.9/draugr/torch_utilities/operations/activations.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/operations/sizes/conv2d.py` & `Draugr-1.0.9/draugr/torch_utilities/operations/sizes/conv2d.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/operations/sizes/max_pool2d.py` & `Draugr-1.0.9/draugr/torch_utilities/operations/sizes/max_pool2d.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/operations/sizes/pad2d.py` & `Draugr-1.0.9/draugr/torch_utilities/operations/sizes/pad2d.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/operations/sizes/transp_conv2d.py` & `Draugr-1.0.9/draugr/torch_utilities/operations/sizes/transp_conv2d.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/operations/torch_transforms/batch_transforms.py` & `Draugr-1.0.9/draugr/torch_utilities/operations/torch_transforms/batch_transforms.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/checking/numerical_gradient.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/checking/numerical_gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,36 +7,37 @@
            Created on 29/07/2020
            """
 
 __all__ = []
 
 import copy
 import math
+from typing import Callable
 
 import torch
-
 from draugr.torch_utilities.optimisation.parameters import (
     named_trainable_parameters,
     normal_init_weights,
     trainable_parameters,
 )
 from draugr.torch_utilities.sessions import TorchEvalSession
+
 from warg import ContextWrapper
 
 
 def loss_grad_check(
     model: torch.nn.Module,
-    loss_fn: callable,
+    loss_fn: Callable,
     iinput: torch.Tensor,
     target: torch.Tensor,
     epsilon: float = 1e-6,
     error_tolerance: float = 1e-5,
 ) -> None:
     """
-    two sided gradient numerical approximation
+    Two sided gradient numerical approximation
     DOES not work, please refer to torch/autograd/gradcheck.py
 
     :param iinput:
     :type iinput:
     :param target:
     :type target:
     :param error_tolerance:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/flow.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,18 @@
            Created on 29/07/2020
            """
 
 __all__ = ["plot_grad_flow"]
 
 import numpy
 import torch
+from draugr.torch_utilities.optimisation.parameters import normal_init_weights
 from matplotlib import pyplot
 from matplotlib.lines import Line2D
 
-from draugr.torch_utilities.optimisation.parameters import normal_init_weights
-
 
 def plot_grad_flow(
     model: torch.nn.Module,
     lines: bool = True,
     alpha: float = 0.5,
     line_width: float = 1.0,
 ) -> None:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/grad_trace.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/grad_trace.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/gradients/guided.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/gradients/guided.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/layer_fetching.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/layer_fetching.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __doc__ = r"""
 
            Created on 07/07/2020
            """
 
 import functools
 from collections import OrderedDict
-from typing import Tuple, Sequence, MutableMapping
+from typing import Tuple, Sequence, MutableMapping, Any
 
 import torch
 from torch import nn
 
 __all__ = ["IntermediateLayerGetter"]
 
 
@@ -62,15 +62,17 @@
         :rtype:"""
 
         def _getattr(obj, attr):
             return getattr(obj, attr, *args)
 
         return functools.reduce(_getattr, (obj, *attr.split(".")))
 
-    def __call__(self, *args: Sequence, **kwargs: MutableMapping) -> Tuple:
+    def __call__(
+        self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]
+    ) -> Tuple:
         ret = OrderedDict()
         handles = []
         for name, new_name in self.return_layers:
             if name == "":
                 continue  # TODO: Fail maybe?
             layer = IntermediateLayerGetter.reduce_getattr(self._model, name)
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/debugging/opt_verification.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/debugging/opt_verification.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
            Created on 07/07/2020
            """
 
 from random import random
 
 import torch
-
 from draugr.torch_utilities.tensors import to_tensor
 
 __all__ = ["overfit_single_batch"]
 
 
 # __all__ = ['init_softmax_loss','overfit_single_batch']
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/__init__.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/complexity.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/complexity.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 25/03/2020
            """
 
 import sys
-from typing import Sequence, TextIO, Tuple, Union
+from typing import Sequence, TextIO, Tuple, Union, Callable
 
 import numpy
 import torch
-from torch import nn
-
 from draugr.torch_utilities import assume_model_dtype, assume_model_device
 from draugr.torch_utilities.optimisation.parameters.counting import get_num_parameters
+from torch import nn
 
 __all__ = ["get_model_complexity_info", "MODULES_MAPPING"]
 
 
 def get_model_complexity_info(
     model: torch.nn.Module,
     input_res: Tuple,
     print_per_layer_stat: bool = True,
     as_strings: bool = True,
-    input_constructor: callable = None,
+    input_constructor: Callable = None,
     ost: TextIO = sys.stdout,
 ) -> Union[Tuple[int, int], Tuple[str, str]]:
     """
 
     :param model:
     :type model:
     :param input_res:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/counting.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/counting.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 __doc__ = r"""
 
            Created on 27/06/2020
            """
 
 __all__ = ["get_num_parameters"]
 
-from torch import nn
-
 from draugr.torch_utilities.optimisation.parameters.trainable import (
     trainable_parameters,
 )
+from torch import nn
 
 
 def get_num_parameters(model: nn.Module, *, only_trainable: bool = False) -> int:
     """
     Returns the number of parameters of a model (trainable or all)
 
     :param only_trainable:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/differential_operators.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/differential_operators.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/exporting.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/exporting.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/freezing/models.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/freezing/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 
            Created on 02-12-2020
            """
 
 from contextlib import contextmanager
 from itertools import tee
 
-from torch.nn import Module
-
 from draugr.torch_utilities.optimisation.parameters.freezing.parameters import (
     freeze_parameters,
 )
+from torch.nn import Module
 
 __all__ = ["freeze_model", "frozen_model"]
 
 
 def freeze_model(model: Module, value: bool = None, recurse: bool = True) -> None:
     """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/freezing/parameters.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/freezing/parameters.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/atari_weight_init.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/atari_weight_init.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/fan_in_weight_init.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/fan_in_weight_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,23 @@
     Conv2d,
     Linear,
     Module,
     Sigmoid,
     Tanh,
     ReLU,
     LeakyReLU,
-    BatchNorm2d,
-    BatchNorm1d,
-    BatchNorm3d,
-    Dropout,
     Softmax,
     Softplus,
     SiLU,
     ELU,
     Identity,
     Conv1d,
     Conv3d,
 )
 from torch.nn.init import calculate_gain, constant_, uniform_, xavier_uniform_
-from enum import Enum
-
 
 __all__ = ["fan_in_init", "xavier_init", "constant_init", "normal_init", "ortho_init"]
 
 
 def fan_in_init(model: Module) -> None:
     """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/initialisation/ortho_weight_init.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/initialisation/ortho_weight_init.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/regularisation/reg_loss_wrapper.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/regularisation/reg_loss_wrapper.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/parameters/trainable.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/parameters/trainable.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/learning_rate_utilities.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/learning_rate_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
            """
 
 __all__ = ["set_lr", "exponential_lr_decay", "average_learning_rate"]
 
 from statistics import mean
 
 import torch
-
 from torch.optim.optimizer import Optimizer
 
 
 def set_lr(optimizer: torch.optim.Optimizer, lr: float) -> None:
     """
 
     :param optimizer:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/lr_scheduler.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/scheduling/schedulers.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/scheduling/schedulers.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/stopping/overfitting.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/stopping/overfitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import contextlib
+from typing import Callable
 
 from warg import sink, Number
 
 __all__ = ["ImprovementDetector", "OverfitDetector"]
 
 
 class ImprovementDetector(contextlib.AbstractContextManager):
     """description"""
 
     def __init__(
         self,
         patience: int,
-        writer: callable = print,
+        writer: Callable = print,
         minimization: bool = True,
-        callback: callable = None,
+        callback: Callable = None,
     ):
         """
         NOTE: strictly greater or less than is considered as improvement
 
         :param patience:
         :type patience:
         :param writer:
@@ -76,17 +77,17 @@
 
 class OverfitDetector(contextlib.AbstractContextManager):
     """description"""
 
     def __init__(
         self,
         patience: int,
-        writer: callable = print,
+        writer: Callable = print,
         minimization: bool = True,
-        callback: callable = None,
+        callback: Callable = None,
         verbose: bool = False,
     ):
         """
         NOTE: equality, greater or less than
 
         :param patience:
         :type patience:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/updates/copying.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/updates/copying.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/optimisation/updates/soft_update.py` & `Draugr-1.0.9/draugr/torch_utilities/optimisation/updates/soft_update.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/persistence/checkpoint.py` & `Draugr-1.0.9/draugr/torch_utilities/persistence/checkpoint.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/persistence/config.py` & `Draugr-1.0.9/draugr/torch_utilities/persistence/config.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/persistence/model.py` & `Draugr-1.0.9/draugr/torch_utilities/persistence/model.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import datetime
 import sys
 from typing import Optional
 
 import torch
-from torch.nn.modules.module import Module
-
 from draugr.torch_utilities.persistence.config import (
     ensure_directory_exist,
     save_config,
 )
+from torch.nn.modules.module import Module
+
 from warg import latest_file
 from warg import passes_kws_to
 from warg.decorators.kw_passing import drop_unused_kws
 
 __author__ = "Christian Heider Nielsen"
 
 model_extension = ".model"
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/persistence/parameters.py` & `Draugr-1.0.9/draugr/torch_utilities/persistence/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 __all__ = [
     "load_model_parameters",
     "load_latest_model_parameters",
     "save_parameters_and_configuration",
     "save_model_parameters",
 ]
 
-from pathlib import Path
 import datetime
 import os
+from pathlib import Path
 from typing import Optional, Tuple, Union
-from torch import nn
-import torch
-from torch.nn.modules.module import Module
-from torch.optim import Optimizer
 
+import torch
 from draugr.torch_utilities.persistence.config import (
     ensure_directory_exist,
     save_config,
 )
-from warg.decorators.kw_passing import drop_unused_kws
+from torch import nn
+from torch.nn.modules.module import Module
+from torch.optim import Optimizer
+
+from warg import drop_unused_kws, passes_kws_to
 
 PARAMETER_EXTENSION = ".parameters"
 CONFIG_EXTENSION = ".py"
 OPTIMISER_EXTENSION = ".optimiser"
 
 
 @drop_unused_kws
@@ -85,15 +86,15 @@
         return (model, optimiser), (model_loaded, optimiser_loaded)
     return model, model_loaded
 
 
 load_model_parameters = load_latest_model_parameters
 
 
-# @passes_kws_to(save_config)
+@passes_kws_to(save_config)
 def save_parameters_and_configuration(
     *,
     model: Union[torch.nn.Module, nn.Parameter],
     model_save_path: Path,
     optimiser: Optional[Optimizer] = None,
     optimiser_save_path: Optional[Path] = None,
     config_save_path: Optional[Path] = None,
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/sessions/cache_sessions.py` & `Draugr-1.0.9/draugr/torch_utilities/sessions/cache_sessions.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/sessions/determinism_sessions.py` & `Draugr-1.0.9/draugr/torch_utilities/sessions/determinism_sessions.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/sessions/device_sessions.py` & `Draugr-1.0.9/draugr/torch_utilities/sessions/device_sessions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 11/05/2020
            """
 
 import torch
+from draugr.torch_utilities import global_torch_device
 from torch.nn import Module
 
-from draugr.torch_utilities import global_torch_device
 from warg import AlsoDecorator
 
 __all__ = ["TorchCpuSession", "TorchCudaSession", "TorchDeviceSession"]
 
 
 class TorchCudaSession(AlsoDecorator):
     """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/sessions/jit_sessions.py` & `Draugr-1.0.9/draugr/torch_utilities/sessions/jit_sessions.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/sessions/model_sessions.py` & `Draugr-1.0.9/draugr/torch_utilities/sessions/model_sessions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
            Created on 11/05/2020
            """
 
 from collections import OrderedDict
 from itertools import tee
 
 import torch
-
 from draugr.torch_utilities.optimisation.parameters.freezing import freeze_parameters
+
 from warg import AlsoDecorator
 
 __all__ = [
     "TorchEvalSession",
     "TorchTrainSession",
     "TorchFrozenModelSession",
     "TorchTrainingSession",
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/sessions/type_sessions.py` & `Draugr-1.0.9/draugr/torch_utilities/sessions/type_sessions.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/system/constants.py` & `Draugr-1.0.9/draugr/torch_utilities/system/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from typing import Union
 
 import numpy
 import torch
-
 from draugr.torch_utilities.tensors import to_tensor
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 09/10/2019
            """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/system/data_type.py` & `Draugr-1.0.9/draugr/torch_utilities/system/data_type.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/system/device.py` & `Draugr-1.0.9/draugr/torch_utilities/system/device.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/system/info.py` & `Draugr-1.0.9/draugr/torch_utilities/system/info.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/system/loading.py` & `Draugr-1.0.9/draugr/torch_utilities/system/loading.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 __all__ = ["default_worker_init_fn", "global_pin_memory"]
 
 import random
 from typing import Union
 
 import numpy
 import torch
-
 from draugr.torch_utilities.system.device import global_torch_device
 
 
 def default_worker_init_fn() -> None:
     """description"""
     worker_seed = torch.initial_seed()
     torch.random.seed(worker_seed)
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/system/seeding.py` & `Draugr-1.0.9/draugr/torch_utilities/system/seeding.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/__init__.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/dimension_order.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/dimension_order.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/info.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/info.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/normalise.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/normalise.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/reshaping.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/reshaping.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/space.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/space.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/tensor_container.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/tensor_container.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = ["NamedTensorTuple"]
 
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any
 
 
 class NamedTensorTuple:
     """
     Help class for manage boxes, labels, etc...
     Not inherit dict due to `default_collate` will change dict's subclass to dict."""
 
@@ -19,23 +19,23 @@
 
     def __iter__(self):
         return self._data_dict.__iter__()
 
     def __setitem__(self, key, value):
         self._data_dict[key] = value
 
-    def _call(self, name, *args: Sequence, **kwargs: MutableMapping):
+    def _call(self, name, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         keys = list(self._data_dict.keys())
         for key in keys:
             value = self._data_dict[key]
             if hasattr(value, name):
                 self._data_dict[key] = getattr(value, name)(*args, **kwargs)
         return self
 
-    def to(self, *args: Sequence, **kwargs: MutableMapping):
+    def to(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """
 
         :param args:
         :type args:
         :param kwargs:
         :type kwargs:
         :return:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/to_scalar.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/to_scalar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from typing import Iterable, Sequence, Union
+from typing import Iterable, Sequence, Union, Callable
 
 import numpy
 import torch
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = ""
 __all__ = ["to_scalar"]
@@ -12,15 +12,15 @@
 from draugr.torch_utilities.tensors.to_tensor import to_tensor
 from warg import Number
 
 
 def to_scalar(
     obj: Union[torch.Tensor, numpy.ndarray, Iterable, Sequence, int, float],
     device: Union[str, torch.device] = "cpu",
-    aggregation: callable = torch.mean,
+    aggregation: Callable = torch.mean,
 ) -> Number:
     """
     Always detaches from computation graph
 
     default behaviour is obj.cpu().mean().item()
 
     :param aggregation:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/to_tensor.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/to_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = ""
 __all__ = ["to_tensor"]
 
 from draugr.torch_utilities.tensors.types import numpy_to_torch_dtype
 
 
+# from warg import passes_kws_to
+
+
 # @passes_kws_to(torch.Tensor.to)
 def to_tensor(
     obj: Union[torch.Tensor, numpy.ndarray, Iterable, Sequence, int, float],
     dtype: Union[
         torch.dtype, object
     ] = None,  # if None, torch.float or equivalent numpy.dtype is used, can be used to force dtype
     device: Union[str, torch.device] = "cpu",
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/tensors/types.py` & `Draugr-1.0.9/draugr/torch_utilities/tensors/types.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/mixins/graph_writer_mixin.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/mixins/graph_writer_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from abc import ABC, abstractmethod
 from typing import Union, Sequence
+
 import torch
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 09/10/2019
            """
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/tensorboard/__init__.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/tensorboard/launcher.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/tensorboard/launcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = ""
 __all__ = ["launch_tensorboard"]
 
 from pathlib import Path
 
-from tensorboard import program  # IMPORT OUT HERE; POSSIBLE RAISE CONDITIONS
-
 from draugr.python_utilities.sockets import is_port_in_use
+from tensorboard import program  # IMPORT OUT HERE; POSSIBLE RAISE CONDITIONS
 
 
 def launch_tensorboard(log_dir: Path, port: int = 6006) -> str:
     """
 
     launch tensorboard
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/tensorboard/tensorboard_pytorch_writer.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/tensorboard/tensorboard_pytorch_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from draugr.writers.mixins.precision_recall_writer_mixin import (
     PrecisionRecallCurveWriterMixin,
 )
 from draugr.writers.mixins.spectrogram_writer_mixin import SpectrogramWriterMixin
 from draugr.writers.writer import Writer
 from matplotlib import pyplot
 from matplotlib.figure import Figure
+
 from warg import drop_unused_kws, passes_kws_to, sprint
 
 with suppress(FutureWarning):
     from torch.utils.tensorboard import SummaryWriter
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = """
@@ -216,15 +217,15 @@
 
         if summary_writer_kws is None:
             summary_writer_kws = {}
 
         self._log_dir = path
         self._summary_writer_kws = summary_writer_kws
 
-    # @passes_kws_to(SummaryWriter.add_hparams)
+    @passes_kws_to(SummaryWriter.add_hparams)
     def instance(self, instance: dict, metrics: dict, **kwargs) -> None:
         """
 
         TODO: Not finished!
 
         :param instance:
         :param metrics:
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/torch_module_writer/module_parameter_writer_mixin.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/torch_module_writer/module_parameter_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/torch_module_writer/module_writer_parameters.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/torch_module_writer/module_writer_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import torch
 
 from draugr import PROJECT_APP_PATH
 
 # from draugr.torch_utilities.writers.tensorboard import TensorBoardPytorchWriter # Self reference issue
 from draugr.writers import HistogramWriterMixin
 
+# from warg import passes_kws_to
+
 __all__ = ["weight_bias_histograms"]
 
 
 # @passes_kws_to(TensorBoardPytorchWriter.histogram) # Self reference issue
 def weight_bias_histograms(
     writer: HistogramWriterMixin,
     model: torch.nn.Module,
```

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/visdom/episode_visual.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/visdom/episode_visual.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/visdom/plotting.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/visdom/plotting.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/torch_utilities/writers/visdom/visdom_writer.py` & `Draugr-1.0.9/draugr/torch_utilities/writers/visdom/visdom_writer.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/__init__.py` & `Draugr-1.0.9/draugr/visualisation/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/annotate.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/annotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 04-03-2021
            """
 
-from typing import Tuple, MutableMapping
+from typing import Tuple, MutableMapping, Callable
 
 from draugr.scipy_utilities import mag_decimation_subsample
 
 __all__ = [
     "annotate_lines",
     "default_index_decimator",
 ]
@@ -25,15 +25,15 @@
 )  # finds interesting features?
 
 
 @passes_kws_to(Axes.annotate)
 def annotate_lines(
     ax_: Axes,
     num_lines: int = 1,  # None for all
-    index_decimator: callable = default_index_decimator,
+    index_decimator: Callable = default_index_decimator,
     color: str = "k",  # None for auto color
     xycoords: Tuple[str, str] = (
         "data",
         # 'axes fraction',
         "data",
     ),  # TODO: NOT DONE! Where to place annotation, use 'axes fraction' for along axes'
     ha: str = "left",
```

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/figure_sessions.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/figure_sessions.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/display_3d_depth_image.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/display_3d_depth_image.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/display_depth_image.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/display_depth_image.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/multiple.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/multiple.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/image_data/replay_frames.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/image_data/replay_frames.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/matplotlib_utilities.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/matplotlib_utilities.py`

 * *Files identical despite different names*

```diff
@@ -10,28 +10,27 @@
 import subprocess
 from enum import Enum
 from pathlib import Path
 from typing import Any, Sequence, Union
 
 import numpy
 from cycler import Cycler
-from matplotlib import patches, pyplot, rcParams
-from matplotlib.legend_handler import HandlerErrorbar
-from sorcery import assigned_names
-
 from draugr.visualisation.matplotlib_utilities.quirks import auto_post_hatch
 from draugr.visualisation.matplotlib_utilities.styles.annotation import (
     rt_ann_transform,
     semi_opaque_round_tight_bbox,
 )
 from draugr.visualisation.matplotlib_utilities.styles.cyclers import (
     monochrome_hatch_cycler,
     monochrome_line_cycler,
     simple_hatch_cycler,
 )
+from matplotlib import patches, pyplot, rcParams
+from matplotlib.legend_handler import HandlerErrorbar
+from sorcery import assigned_names
 
 __all__ = [
     "denormalise_minusoneone",
     "matplotlib_bounding_box",
     "remove_decoration",
     "use_monochrome_style",
     "decolorise_plot",
```

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/matplotlib_writer.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/matplotlib_writer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 __all__ = []
 
 from pathlib import Path
 from typing import Sequence, Mapping, Union, MutableMapping
 
 import numpy
 from PIL import Image
-from matplotlib import pyplot
-from matplotlib.figure import Figure
-
 from draugr.writers import (
     Writer,
     ImageWriterMixin,
     HistogramWriterMixin,
     BarWriterMixin,
     LineWriterMixin,
     SpectrogramWriterMixin,
     FigureWriterMixin,
 )
+from matplotlib import pyplot
+from matplotlib.figure import Figure
+
 from warg import passes_kws_to
 
 
 class MatPlotLibWriter(
     Writer,
     ImageWriterMixin,
     HistogramWriterMixin,
```

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/metric_overview_plot.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/metric_overview_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import math
-from typing import Iterable, Iterator, Sequence, Tuple
+from typing import Iterable, Iterator, Sequence, Tuple, Any
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = """
 Created on 27/04/2019
 
 @author: cnheider
 """
@@ -124,15 +124,15 @@
         ax.imshow(image, **kwargs)
     return fig
 
 
 def biplot(
     scores: Sequence,
     coefficients: numpy.ndarray,
-    categories: Iterable = None,
+    categories: Iterable[Any] = None,
     labels: Sequence = None,
     label_multiplier: float = 1.06,
 ) -> pyplot.Figure:
     """
        Use only the 2 Principal components.
 
       :rtype: object
```

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/quirks.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/quirks.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 
            Created on 17-02-2021
            """
 
 from enum import Enum
 from typing import Sequence, Optional
 
+from draugr.visualisation.matplotlib_utilities.styles.cyclers import simple_hatch_cycler
 from matplotlib import cycler, pyplot, rcParams
 from matplotlib.axes import Axes
 
-from draugr.visualisation.matplotlib_utilities.styles.cyclers import simple_hatch_cycler
-
 __all__ = [
     "fix_edge_gridlines",
     "auto_post_print_dpi",
     "auto_post_hatch",
     "scatter_auto_mark",
 ]
```

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/3d_gradients.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/3d_gradients.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/3d_spectrum.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/3d_spectrum.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/display_sampler.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/display_sampler.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/signal_plotting.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/signal_plotting.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/signal_data/spectral_plotting.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/signal_data/spectral_plotting.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/annotation.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/annotation.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/cyclers.py` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/cyclers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 __all__ = [
     "monochrome_hatch_cycler",
     "simple_hatch_cycler",
     "monochrome_line_no_marker_cycler",
     "monochrome_line_cycler",
 ]
 
-from matplotlib import cycler
-
 from draugr.visualisation.matplotlib_utilities.styles.hatching import (
     four_times_denser_hatch,
 )
 from draugr.visualisation.matplotlib_utilities.styles.lines import (
     line_styles,
     marker_styles,
 )
+from matplotlib import cycler
 
 color_cycler = cycler("color", ["E24A33", "348ABD", "988ED5", "FBC15E", "8EBA42"])
 marker_cycler = cycler("marker", marker_styles)
 line_cycler = cycler("linestyle", line_styles)
 simple_hatch_cycler = cycler("hatch", four_times_denser_hatch)
 
 monochrome_hatch_cycler = (
```

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/monochrome.mplstyle` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/monochrome.mplstyle`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/matplotlib_utilities/styles/publish_color.mplstyle` & `Draugr-1.0.9/draugr/visualisation/matplotlib_utilities/styles/publish_color.mplstyle`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/pillow_utilities.py` & `Draugr-1.0.9/draugr/visualisation/pillow_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/progress/__init__.py` & `Draugr-1.0.9/draugr/writers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Christian Heider Nielsen"
-__doc__ = r"""
+__doc__ = """
+Created on 27/04/2019
 
-           Created on 08-12-2020
-           """
+@author: cnheider
+"""
 
 from pathlib import Path
 
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 # del Path
-try:
-    from .progress_bar import *
-    from .pooled_progress_bar import *
 
-    # from .eta_bar import # IT is super shit
-    from .pick import *
+try:
+    from .csv_writer import *
+    from .log_writer import *
+    from .mixins import *
+    from .mock_writer import *
+    from .terminal import *
+    from .writer import *
+    from .standard_tags import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = (
         Path(__file__).parent.parent.parent
         / "requirements"
         / f"requirements_{this_package_name}.txt"
     )
```

### Comparing `Draugr-1.0.8/draugr/visualisation/progress/eta_bar.py` & `Draugr-1.0.9/draugr/visualisation/progress/eta_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,17 @@
            Created on 8/24/22
            """
 
 __all__ = ["ETABar"]
 
 from typing import Iterator
 
-from progress.colors import color  # shit
-
 from draugr.python_utilities import in_ipynb
 from progress.bar import Bar  # IT is shit
+from progress.colors import color  # shit
 
 from warg import passes_kws_to, drop_unused_kws
 
 
 class ETABar(Bar, Iterator):
     """Progress bar that displays the estimated time of completion.
     TODO: REMOVE THIS PIECE OF SHIT!
```

### Comparing `Draugr-1.0.8/draugr/visualisation/progress/pick.py` & `Draugr-1.0.9/draugr/visualisation/progress/pick.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 __all__ = ["choose_progress_bar"]
 
 from itertools import count
 from typing import Iterator
 
 from draugr.python_utilities.platform_context import in_ipynb
-
 from draugr.visualisation.progress.eta_bar import ETABar
 from draugr.visualisation.progress.progress_bar import progress_bar
+
 from warg import LambdaContext
 
 
 class IteratorWrapper(Iterator):
     """
     #TO be removed
     """
```

### Comparing `Draugr-1.0.8/draugr/visualisation/progress/pooled_progress_bar.py` & `Draugr-1.0.9/draugr/visualisation/progress/pooled_progress_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Iterable,
     List,
     Mapping,
     Optional,
     Sized,
     MutableMapping,
 )
+
 from pathos.helpers import cpu_count
 from pathos.multiprocessing import ProcessPool as Pool
 from tqdm.auto import tqdm
 
 __author__ = "Christian Heider Nielsen"
 __all__ = [
     "parallel_map",
```

### Comparing `Draugr-1.0.8/draugr/visualisation/progress/progress_bar.py` & `Draugr-1.0.9/draugr/visualisation/progress/progress_bar.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 import time
 from enum import Enum
 from itertools import tee
 from typing import Any, Generator, Iterable
 
 import tqdm
+from notus.notification import JobNotificationSession
 from sorcery import assigned_names
 
-from notus.notification import JobNotificationSession
 from warg import drop_unused_kws, passes_kws_to, empty_str
 
 __all__ = ["progress_bar"]
 
 
 class TimestampModeEnum(Enum):
     none, prefix, postfix = assigned_names()
```

### Comparing `Draugr-1.0.8/draugr/visualisation/seaborn_utilities/seaborn_enums.py` & `Draugr-1.0.9/draugr/visualisation/seaborn_utilities/seaborn_enums.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/visualisation/seaborn_utilities/seaborn_utilities.py` & `Draugr-1.0.9/draugr/visualisation/seaborn_utilities/seaborn_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/__init__.py` & `Draugr-1.0.9/draugr/os_utilities/linux_utilities/gtk_utilities/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Christian Heider Nielsen"
-__doc__ = """
-Created on 27/04/2019
+__doc__ = r"""
 
-@author: cnheider
-"""
+           Created on 03/08/2020
+           """
 
 from pathlib import Path
 
-with open(Path(__file__).parent / "README.md", "r") as this_init_file:
-    __doc__ += this_init_file.read()
-# del Path
+from draugr import INCLUDE_PROJECT_READMES
+
+if INCLUDE_PROJECT_READMES:
+    with open(Path(__file__).parent / "README.md", "r") as this_init_file:
+        __doc__ += this_init_file.read()
 
 try:
-    from .csv_writer import *
-    from .log_writer import *
-    from .mixins import *
-    from .mock_writer import *
-    from .terminal import *
-    from .writer import *
-    from .standard_tags import *
+    from .gtk_settings import *
+    from .theme_preferences import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = (
         Path(__file__).parent.parent.parent
         / "requirements"
         / f"requirements_{this_package_name}.txt"
     )
```

### Comparing `Draugr-1.0.8/draugr/writers/csv_writer.py` & `Draugr-1.0.9/draugr/writers/csv_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import csv
 from typing import Any, TextIO, Tuple
 
-from warg import ensure_existence
 from draugr import PROJECT_APP_PATH
 from draugr.writers.writer import Writer
 
+from warg import ensure_existence
+
 __author__ = "Christian Heider Nielsen"
 __doc__ = """
 Created on 27/04/2019
 
 @author: cnheider
 """
```

### Comparing `Draugr-1.0.8/draugr/writers/log_writer.py` & `Draugr-1.0.9/draugr/writers/log_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import logging
 import sys
 from typing import Any, MutableMapping
 
-from warg import ensure_existence
 from draugr import PROJECT_APP_PATH
 from draugr.writers.writer import Writer
 
+from warg import ensure_existence
+
 __author__ = "Christian Heider Nielsen"
 __doc__ = """
 Created on 27/04/2019
 
 @author: cnheider
 """
 __all__ = ["LogWriter"]
```

### Comparing `Draugr-1.0.8/draugr/writers/mixins/__init__.py` & `Draugr-1.0.9/draugr/writers/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/audio_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/audio_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/bar_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/bar_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/embed_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/embed_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/figure_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/figure_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/histogram_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/histogram_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/image_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/image_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/instantiation_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/instantiation_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/line_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/line_writer_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 09/10/2019
            """
 __all__ = ["LineWriterMixin"]
+
 from abc import ABC, abstractmethod
 from typing import Mapping, Sequence, MutableMapping
 
 
 class LineWriterMixin(ABC):
     """
     Writer mixin that provides an interface for 'writing' line charts"""
```

### Comparing `Draugr-1.0.8/draugr/writers/mixins/mesh_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/mesh_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/precision_recall_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/precision_recall_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/scalar_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/scalar_writer_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 from itertools import cycle
 from typing import MutableMapping
-from warg import Number, passes_kws_to, drop_unused_kws
+
 from draugr.python_utilities import CounterFilter
 
+from warg import Number, passes_kws_to, drop_unused_kws
 
 __all__ = ["ScalarWriterMixin"]
 
 
 class ScalarWriterMixin(CounterFilter, ABC):
     """description"""
```

### Comparing `Draugr-1.0.8/draugr/writers/mixins/spectrogram_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/spectrogram_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mixins/video_writer_mixin.py` & `Draugr-1.0.9/draugr/writers/mixins/video_writer_mixin.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/mock_writer.py` & `Draugr-1.0.9/draugr/writers/mock_writer.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/standard_tags.py` & `Draugr-1.0.9/draugr/writers/standard_tags.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/terminal/console_writer.py` & `Draugr-1.0.9/draugr/writers/terminal/console_writer.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/draugr/writers/terminal/terminal_plot_writer.py` & `Draugr-1.0.9/draugr/writers/terminal/terminal_plot_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from typing import Union, MutableMapping
 
 import numpy
 import torch
 from PIL import Image
-from tqdm import tqdm
-
-from draugr.metrics import MetricCollection
-from draugr.writers.mixins import ImageWriterMixin
 from draugr.drawers.terminal import (
     terminal_render_image,
     terminalise_image,
     styled_terminal_plot_stats_shared_x,
     terminal_plot,
 )
+from draugr.metrics import MetricCollection
+from draugr.writers.mixins import ImageWriterMixin
 from draugr.writers.writer import Writer
+from tqdm import tqdm
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = """
 Created on 27/04/2019
 
 @author: cnheider
 """
```

### Comparing `Draugr-1.0.8/draugr/writers/writer.py` & `Draugr-1.0.9/draugr/writers/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 @author: cnheider
 """
 
 from abc import ABCMeta, abstractmethod
 from collections import deque
 
-from draugr.python_utilities.counter_filter import CounterFilter
 from draugr.writers.mixins.scalar_writer_mixin import ScalarWriterMixin
 
 __all__ = ["Writer", "global_writer", "set_global_writer"]
 
 from typing import Any, Optional, Sequence, MutableMapping
 
 
@@ -52,15 +51,15 @@
     def _close(self, exc_type=None, exc_val=None, exc_tb=None):
         raise NotImplementedError
 
     @abstractmethod
     def _open(self):
         return self
 
-    def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         self.scalar(*args, *kwargs)
 
 
 GLOBAL_WRITER_STACK = deque()
 GLOBAL_WRITER = None
```

### Comparing `Draugr-1.0.8/draugr/writers/writer_utilities.py` & `Draugr-1.0.9/draugr/writers/writer_utilities.py`

 * *Files identical despite different names*

### Comparing `Draugr-1.0.8/setup.py` & `Draugr-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from typing import TextIO, List, Sequence, Union
 
 
-def python_version_check(major: int = 3, minor: int = 7):
+def python_version_check(major: int = 3, minor: int = 8):
     """description"""
     import sys
 
     assert sys.version_info.major == major and sys.version_info.minor >= minor, (
         f"This project is utilises language features only present Python {major}.{minor} and greater. "
         f"You are running {sys.version_info}."
     )
```

### Comparing `Draugr-1.0.8/tests/test_imports.py` & `Draugr-1.0.9/tests/test_imports.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 01/08/2020
            """
 
 __all__ = []
-import pytest
 
+import pytest
 
 from warg import ensure_in_sys_path, find_nearest_ancestral_relative
 
 ensure_in_sys_path(find_nearest_ancestral_relative("draugr").parent)
 
 
 def test_import():
```

### Comparing `Draugr-1.0.8/tests/test_statistics.py` & `Draugr-1.0.9/tests/test_statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # -*- coding: utf-8 -*-
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 17-12-2020
            """
-from pathlib import Path
-
 
 from warg import ensure_in_sys_path, find_nearest_ancestral_relative
 
 ensure_in_sys_path(find_nearest_ancestral_relative("draugr").parent)
 from draugr.numpy_utilities import root_mean_square
```

