# Comparing `tmp/hciplot-0.2.4.tar.gz` & `tmp/hciplot-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hciplot-0.2.4.tar", last modified: Wed Jun 28 10:10:48 2023, max compression
+gzip compressed data, was "hciplot-0.2.5.tar", last modified: Tue Aug  1 16:21:26 2023, max compression
```

## Comparing `hciplot-0.2.4.tar` & `hciplot-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-06-28 10:10:48.681573 hciplot-0.2.4/
--rw-r--r--   0 valentin   (501) staff       (20)     6148 2022-02-15 18:32:34.000000 hciplot-0.2.4/.DS_Store
--rw-r--r--   0 valentin   (501) staff       (20)     1221 2021-12-01 15:26:15.000000 hciplot-0.2.4/.gitignore
--rw-r--r--   0 valentin   (501) staff       (20)     1086 2021-12-01 15:26:15.000000 hciplot-0.2.4/LICENSE
--rw-r--r--   0 valentin   (501) staff       (20)     2743 2023-06-28 10:10:48.681391 hciplot-0.2.4/PKG-INFO
--rw-r--r--   0 valentin   (501) staff       (20)     1841 2021-12-01 15:26:15.000000 hciplot-0.2.4/README.md
-drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-06-28 10:10:48.674675 hciplot-0.2.4/hciplot/
--rw-r--r--   0 valentin   (501) staff       (20)       68 2023-06-28 10:10:22.000000 hciplot-0.2.4/hciplot/__init__.py
--rw-r--r--   0 valentin   (501) staff       (20)    50776 2023-05-23 15:18:50.000000 hciplot-0.2.4/hciplot/hciplot.py
-drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-06-28 10:10:48.681178 hciplot-0.2.4/hciplot.egg-info/
--rw-r--r--   0 valentin   (501) staff       (20)     2743 2023-06-28 10:10:48.000000 hciplot-0.2.4/hciplot.egg-info/PKG-INFO
--rw-r--r--   0 valentin   (501) staff       (20)      257 2023-06-28 10:10:48.000000 hciplot-0.2.4/hciplot.egg-info/SOURCES.txt
--rw-r--r--   0 valentin   (501) staff       (20)        1 2023-06-28 10:10:48.000000 hciplot-0.2.4/hciplot.egg-info/dependency_links.txt
--rw-r--r--   0 valentin   (501) staff       (20)       67 2023-06-28 10:10:48.000000 hciplot-0.2.4/hciplot.egg-info/requires.txt
--rw-r--r--   0 valentin   (501) staff       (20)        8 2023-06-28 10:10:48.000000 hciplot-0.2.4/hciplot.egg-info/top_level.txt
--rw-r--r--   0 valentin   (501) staff       (20)       66 2023-06-28 08:22:08.000000 hciplot-0.2.4/requirements.txt
--rw-r--r--   0 valentin   (501) staff       (20)       38 2023-06-28 10:10:48.681619 hciplot-0.2.4/setup.cfg
--rw-r--r--   0 valentin   (501) staff       (20)     2213 2022-05-16 15:51:24.000000 hciplot-0.2.4/setup.py
+drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-08-01 16:21:26.298123 hciplot-0.2.5/
+-rw-r--r--   0 valentin   (501) staff       (20)     6148 2022-02-15 18:32:34.000000 hciplot-0.2.5/.DS_Store
+-rw-r--r--   0 valentin   (501) staff       (20)     1246 2023-08-01 16:19:06.000000 hciplot-0.2.5/.gitignore
+-rw-r--r--   0 valentin   (501) staff       (20)     1086 2021-12-01 15:26:15.000000 hciplot-0.2.5/LICENSE
+-rw-r--r--   0 valentin   (501) staff       (20)     2743 2023-08-01 16:21:26.297910 hciplot-0.2.5/PKG-INFO
+-rw-r--r--   0 valentin   (501) staff       (20)     1841 2021-12-01 15:26:15.000000 hciplot-0.2.5/README.md
+drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-08-01 16:21:26.296288 hciplot-0.2.5/hciplot/
+-rw-r--r--   0 valentin   (501) staff       (20)       68 2023-08-01 16:19:06.000000 hciplot-0.2.5/hciplot/__init__.py
+-rw-r--r--   0 valentin   (501) staff       (20)    51163 2023-08-01 16:19:52.000000 hciplot-0.2.5/hciplot/hciplot.py
+drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-08-01 16:21:26.297686 hciplot-0.2.5/hciplot.egg-info/
+-rw-r--r--   0 valentin   (501) staff       (20)     2743 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/PKG-INFO
+-rw-r--r--   0 valentin   (501) staff       (20)      257 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/SOURCES.txt
+-rw-r--r--   0 valentin   (501) staff       (20)        1 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/dependency_links.txt
+-rw-r--r--   0 valentin   (501) staff       (20)       53 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/requires.txt
+-rw-r--r--   0 valentin   (501) staff       (20)        8 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/top_level.txt
+-rw-r--r--   0 valentin   (501) staff       (20)       52 2023-08-01 16:19:24.000000 hciplot-0.2.5/requirements.txt
+-rw-r--r--   0 valentin   (501) staff       (20)       38 2023-08-01 16:21:26.298174 hciplot-0.2.5/setup.cfg
+-rw-r--r--   0 valentin   (501) staff       (20)     2213 2022-05-16 15:51:24.000000 hciplot-0.2.5/setup.py
```

### Comparing `hciplot-0.2.4/.DS_Store` & `hciplot-0.2.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `hciplot-0.2.4/.gitignore` & `hciplot-0.2.5/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 .idea/*
 
+# macOS stuff
+.DS_Store
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `hciplot-0.2.4/LICENSE` & `hciplot-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hciplot-0.2.4/PKG-INFO` & `hciplot-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hciplot
-Version: 0.2.4
+Version: 0.2.5
 Summary: High-contrast Imaging Plotting library
 Home-page: https://github.com/carlgogo/hciplot
 Download-URL: https://github.com/carlgogo/hciplot/archive/refs/tags/v0.1.8.tar.gz
 Author: Carlos Alberto Gomez Gonzalez, Valentin Christiaens
 Author-email: valentinchrist@hotmail.com
 License: MIT
 Keywords: plotting,hci,package
```

### Comparing `hciplot-0.2.4/README.md` & `hciplot-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `hciplot-0.2.4/hciplot/hciplot.py` & `hciplot-0.2.5/hciplot/hciplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-__author__ = 'Carlos Alberto Gomez Gonzalez, Valentin Christiaens'
+__author__ = 'Carlos Alberto Gomez Gonzalez, Valentin Christiaens, Iain Hammond'
 __all__ = ['plot_frames',
            'plot_cubes']
 
-from decimal import *
-import os
-import shutil
-import numpy as np
-import holoviews as hv
-from holoviews import opts
+from decimal import Decimal
+from os import mkdir
+from os.path import exists
+from shutil import rmtree
 from subprocess import call
-from matplotlib.pyplot import (figure, subplot, show, savefig, close, hlines,
-                               annotate)
+from warnings import filterwarnings
+
+import numpy as np
+from holoviews import extension, Dataset, Image, Layout, output, opts
+from matplotlib.cm import register_cmap
+from matplotlib.colors import LinearSegmentedColormap, LogNorm, ListedColormap, Normalize
 from matplotlib.patches import Circle, Ellipse
 from matplotlib.pyplot import colorbar as plt_colorbar
+from matplotlib.pyplot import (figure, subplot, show, savefig, close, hlines,
+                               annotate)
 from mpl_toolkits.axes_grid1 import make_axes_locatable
-from matplotlib.cm import register_cmap
-import matplotlib.colors as colors
-from matplotlib.colors import LinearSegmentedColormap
-import warnings
-warnings.filterwarnings("ignore", module="matplotlib")
+
+filterwarnings("ignore", module="matplotlib")
 
 # Registering heat and cool colormaps from SaoImage DS9
 # borrowed from: https://gist.github.com/adonath/c9a97d2f2d964ae7b9eb
 ds9cool = {'red': lambda v: 2 * v - 1,
            'green': lambda v: 2 * v - 0.5,
            'blue': lambda v: 2 * v}
 ds9heat = {'red': lambda v: np.interp(v, [0, 0.34, 1], [0, 1, 1]),
            'green': lambda v: np.interp(v, [0, 1], [0, 1]),
            'blue': lambda v: np.interp(v, [0, 0.65, 0.98, 1], [0, 0, 1, 1])}
 register_cmap(cmap=LinearSegmentedColormap('ds9cool', ds9cool))
 register_cmap(cmap=LinearSegmentedColormap('ds9heat', ds9heat))
-cmap_binary = colors.ListedColormap(['black', 'white'])
+cmap_binary = ListedColormap(['black', 'white'])
 default_cmap = 'viridis'
 
 
 def plot_frames(data, backend='matplotlib', mode='mosaic', rows=1, vmax=None,
                 vmin=None, circle=None, circle_alpha=0.8, circle_color='white',
                 circle_linestyle='-', circle_radius=6, circle_label=False,
                 circle_label_color='white', ellipse=None, ellipse_alpha=0.8,
@@ -89,15 +90,15 @@
         [backend='matplotlib'] Alpha transparency for each circle.
     circle_color : str, optional
         [backend='matplotlib'] Color of the circles. White by default.
     circle_radius : int, optional
         [backend='matplotlib'] Radius of the circles, 6 px by default.
     circle_label : bool or string, optional
         [backend='matplotlib'] Whether to show the coordinates next to each
-        circle. If a string: the string to be printed. If a tuple, should be 
+        circle. If a string: the string to be printed. If a tuple, should be
         a tuple of strings with same length as 'circle'.
     circle_label_color : str, optional
         [backend='matplotlib'] Default 'white'. Sets the color of the circle
         label
     ellipse : None, tuple or tuple of tuples, optional
         [backend='matplotlib'] To show a circle at the given px coordinates. The
         circles are shown on all subplots.
@@ -106,19 +107,19 @@
     ellipse_color : str, optional
         [backend='matplotlib'] Color of the circles. White by default.
     ellipse_a : int, optional
         [backend='matplotlib'] Major axis of the ellipses, 6 px by default.
     ellipse_b : int, optional
         [backend='matplotlib'] Minor axis of the ellipses, 4 px by default.
     ellipse_angle : float, optional
-        [backend='matplotlib'] Position angle of the major axis in deg, 0 by 
+        [backend='matplotlib'] Position angle of the major axis in deg, 0 by
         default.
     ellipse_label : bool or string, optional
         [backend='matplotlib'] Whether to show the coordinates next to each
-        circle. If a string: the string to be printed. If a tuple, should be 
+        circle. If a string: the string to be printed. If a tuple, should be
         a tuple of strings with same length as 'circle'.
     ellipse_label_color : str, optional
         [backend='matplotlib'] Default 'white'. Sets the color of the circle
         label
     arrow : None or tuple of floats, optional
         [backend='matplotlib'] To show an arrow pointing to the given pixel
         coordinates.
@@ -157,15 +158,15 @@
         [backend='matplotlib'] Alpha transparency of the crosshair.
     cross_color : string, optional
         [backend='matplotlib'] Color of the crosshair.
     ang_scale : bool or tuple of bools, optional
         [backend='matplotlib'] If True, the axes are displayed in angular scale
         (arcsecs).
     ang_ticksep : int, optional
-        [backend='matplotlib'] Separation for the ticks in pixels, when using 
+        [backend='matplotlib'] Separation for the ticks in pixels, when using
         axis in angular scale.
     tick_direction : str, optional
         [backend='matplotlib'] Outward or inward facing axis ticks.
         'in' for inward, 'out' for outwards.
     tick_color : str, optional
         [backend='matplotlib'] Color of the axis ticks.
     ndec : int, optional
@@ -175,15 +176,15 @@
         (Keck/NIRC2, SPHERE-IRDIS).
     auscale : float, optional
         [backend='matplotlib'] Pixel scale in au/px. Default 1.
     ang_legend : bool or tuple of bools, optional
         [backend='matplotlib'] If True a scaling bar (1 arcsec or 500 mas) will
         be added in the bottom-right corner of the subplots.
     au_legend : bool or tuple of bools, optional
-        [backend='matplotlib'] If True (and ang_legend is False) a scaling bar 
+        [backend='matplotlib'] If True (and ang_legend is False) a scaling bar
         (10 au, 20 au or 50 au) will be added in the top-right corner of the
         subplots.
     axis : bool, optional
         [backend='matplotlib'] Show the axis, on by default.
     show_center : bool or tuple of bools, optional
         [backend='matplotlib'] To show a cross at the center of the frame.
     cmap : None, str or tuple of str, optional
@@ -263,40 +264,39 @@
         return param
 
     def check_numeric_param(param, name):
         msg_type = '`' + name + '` must be a None, float/int or tuple of ' + \
                    'None/float/ints'
         if param is None:
             param = [None] * num_plots
-        elif isinstance(param, (int, float)):
+        elif np.isscalar(param):
             param = [param] * num_plots
-        elif isinstance(param, tuple):
+        elif len(param) == num_plots:
             if not num_plots == len(param):
-                msg = 'The len of `' + name + '` ({}) does not match the ' + \
-                      'number of plots ({})'
+                msg = 'The len of `' + name + \
+                    '` ({}) does not match the ' + 'number of plots ({})'
                 raise ValueError(msg.format(len(param), num_plots))
             else:
                 for elem in param:
                     if elem and not isinstance(elem, (float, int)):
                         raise TypeError(msg_type)
         else:
             raise TypeError(msg_type)
         return param
 
     def check_str_param(param, name, default_value=None):
-        msg_type = '`' + name + '` must be a None, str or tuple of ' + \
-                   'None/str'
+        msg_type = '`' + name + '` must be a None, str or tuple of ' + 'None/str'
         if param is None:
             param = [default_value] * num_plots
         elif isinstance(param, str):
             param = [param] * num_plots
         elif isinstance(param, tuple):
             if not num_plots == len(param):
-                msg = 'The len of `' + name + '` ({}) does not match the ' + \
-                      'number of plots ({})'
+                msg = 'The len of `' + name + \
+                    '` ({}) does not match the ' + 'number of plots ({})'
                 raise ValueError(msg.format(len(param), num_plots))
             else:
                 for elem in param:
                     if elem and not isinstance(elem, str):
                         raise TypeError(msg_type)
         else:
             raise TypeError(msg_type)
@@ -305,16 +305,18 @@
 
     # Checking inputs: a frame (1 or 3 channels) or tuple of them
     msg_data_type = "`data` must be a frame (2d array) or tuple of frames"
     if isinstance(data, np.ndarray):
         if data.ndim == 2:
             data = [data]
         elif data.ndim == 3:
+            data = [data[i] for i in range(data.shape[0])]
+        else:
             raise TypeError(msg_data_type)
-    elif isinstance(data, tuple):
+    elif isinstance(data, (list, tuple)):
         for i in range(len(data)):
             # checking the elements are 2d (excepting the case of 3 channels)
             if not data[i].ndim == 2:  # and data[i].shape[2] != 3:
                 raise ValueError(msg_data_type)
     else:
         raise ValueError(msg_data_type)
 
@@ -521,64 +523,63 @@
             plot_mosaic = False
         elif mode == 'mosaic':
             plot_mosaic = True
         else:
             raise ValueError("`mode` value was not recognized")
 
         for i, v in enumerate(range(num_plots)):
-            image = data[i].copy()
+            image = np.copy(data[i])
             frame_size = image.shape[0]  # assuming square frames
             cy = image.shape[0] / 2 - 0.5
             cx = image.shape[1] / 2 - 0.5
             v += 1
 
             if plot_mosaic:
                 ax = subplot(rows, cols, v)
                 ax.set_aspect('auto')
 
                 if logscale[i]:
-                    image += np.abs(np.nanmin(image))
-                    if vmin[i] is None:
-                        linthresh = 1e-2
-                    else:
-                        linthresh = vmin[i]
-                    norm = colors.SymLogNorm(linthresh, base=10)
+                    # image += np.abs(np.nanmin(image))  # old code to avoid negatives in image
+                    if vmax[i] is None:
+                        vmax[i] = np.nanmax(image)
+                    if vmin[i] is None or vmin[i] <= 0:
+                        vmin[i] = vmax[i] * 1e-2
+                    norm = LogNorm(vmin=vmin[i], vmax=vmax[i], clip=True)
                 else:
-                    norm = None
+                    norm = Normalize(vmin=vmin[i], vmax=vmax[i], clip=True)
 
                 if image.dtype == bool:
                     image = image.astype(int)
 
                 if custom_cmap[i] == 'binary' and image.max() == 1 and \
                    image.min() == 0:
                     cucmap = cmap_binary
                     cbticks = (0, 0.5, 1)
 
                 else:
                     cucmap = custom_cmap[i]
                     cbticks = cbar_ticks[i]
 
-                im = ax.imshow(image, cmap=cucmap, origin='lower', norm=norm,
-                               interpolation='nearest', vmin=vmin[i],
-                               vmax=vmax[i])
+                im = ax.imshow(image, cmap=cucmap, origin='lower',
+                               norm=norm, interpolation='nearest')
                 # if colorbar[i]:
                 #     divider = make_axes_locatable(ax)
                 #     # the width of cax is 5% of ax and the padding between cax
                 #     # and ax wis fixed at 0.05 inch
                 #     cax = divider.append_axes("right", size="5%", pad=0.05)
                 #     cb = plt_colorbar(im, ax=ax, cax=cax, drawedges=False,
                 #                       ticks=cbticks)
                 #     cb.outline.set_linewidth(0.1)
                 #     cb.ax.tick_params(labelsize=lab_fontsize)
                 #     cbw = frame_size/10
                 # else:
                 #     cbw = 0
 
             else:
-                # Leave the import to make porjection='3d' work
+                # Leave the import to make projection='3d' work
                 #from mpl_toolkits.mplot3d import Axes3D
                 x = np.outer(np.arange(0, frame_size, 1), np.ones(frame_size))
                 y = x.copy().T
                 ax = subplot(rows, cols, v, projection='3d')
                 ax.set_aspect('auto')
                 surf = ax.plot_surface(x, y, image, rstride=sampling,
                                        cstride=sampling, linewidth=2,
@@ -631,15 +632,15 @@
                          color='white', size=label_size)
 
             if show_circle and plot_mosaic:
                 if isinstance(circle_linestyle, tuple):
                     c_offset = circle_linestyle[0]
                     circle_linestyle = circle_linestyle[1]
                 else:
-                    c_offset = label_size+1  # vertical offset is equal to the font size + 1, was 2
+                    c_offset = 4  # vertical offset equal to 4px
                 for j in range(n_circ):
                     if isinstance(circle_color, (list, tuple)):
                         circle_color_tmp = circle_color[j]
                     else:
                         circle_color_tmp = circle_color
                     if isinstance(circle_linestyle, (list, tuple)):
                         circle_linestyle_tmp = circle_linestyle[j]
@@ -654,25 +655,27 @@
                         y = coor_circle[j][1]
                         if isinstance(circle_label, str):
                             cirlabel = circle_label
                         elif isinstance(circle_label, tuple):
                             cirlabel = circle_label[j]
                         else:
                             cirlabel = str(int(x))+','+str(int(y))
-                        ax.text(x, y + circle_radius[j] + c_offset, cirlabel,
+                        # added below - can otherwise lead to wide separations
+                        c_offset_j = min(c_offset, circle_radius[j])
+                        ax.text(x, y + circle_radius[j] + c_offset_j, cirlabel,
                                 fontsize=label_size, color=circle_label_color,
                                 family='monospace', ha='center', va='center',
                                 weight='bold', alpha=circle_alpha[j])
 
             if show_ellipse and plot_mosaic:
                 if isinstance(ellipse_linestyle, tuple):
                     e_offset = ellipse_linestyle[0]
                     ellipse_linestyle = ellipse_linestyle[1]
                 else:
-                    e_offset = label_size+1  # vertical offset is equal to the font size + 1, was 2
+                    e_offset = 4  # vertical offset equal to 4px
                 for j in range(n_ell):
                     if isinstance(ellipse_color, (list, tuple)):
                         ellipse_color_tmp = ellipse_color[j]
                     else:
                         ellipse_color_tmp = ellipse_color
                     if isinstance(ellipse_linestyle, (list, tuple)):
                         ellipse_linestyle_tmp = ellipse_linestyle[j]
@@ -689,15 +692,17 @@
                         y = coor_ellipse[j][1]
                         if isinstance(ellipse_label, str):
                             elllabel = ellipse_label
                         elif isinstance(ellipse_label, tuple):
                             elllabel = ellipse_label[j]
                         else:
                             elllabel = str(int(x))+','+str(int(y))
-                        ax.text(x, y + ellipse_a[j] + e_offset, elllabel,
+                        # added below - can otherwise lead to wide separations
+                        e_offset_j = min(e_offset, ellipse_a[j])
+                        ax.text(x, y + ellipse_a[j] + e_offset_j, elllabel,
                                 fontsize=label_size, color=ellipse_label_color,
                                 family='monospace', ha='center', va='center',
                                 weight='bold', alpha=ellipse_alpha[j])
 
             if show_cross and plot_mosaic:
                 ax.axhline(coor_cross[0], xmin=0, xmax=frame_size, alpha=cross_alpha, lw=0.6,
                            linestyle='dashed', color='white')
@@ -826,33 +831,33 @@
             close()
         elif return_fig_ax is False and save is None:
             show()
         elif return_fig_ax and save is None:
             return fig, ax
 
     elif backend == 'bokeh':
-        hv.extension(backend)
+        extension(backend)
         subplots = []
         # options = "Image (cmap='" + custom_cmap[0] + "')"  # taking first item
         # hv.opts(options)
 
         for i, v in enumerate(range(num_plots)):
-            image = data[i].copy()
+            image = np.copy(data[i])
             if vmin[i] is None:
                 vmin[i] = image.min()
             if vmax[i] is None:
                 vmax[i] = image.max()
-            im = hv.Image((range(image.shape[1]), range(image.shape[0]), image))
+            im = Image((range(image.shape[1]), range(image.shape[0]), image))
             subplots.append(im.opts(tools=['hover'], colorbar=colorbar[i],
                                     colorbar_opts={'width': 15},
                                     width=width, height=height,
                                     clim=(vmin[i], vmax[i]),
                                     cmap=custom_cmap[0]))
 
-        return hv.Layout(subplots).cols(cols)
+        return Layout(subplots).cols(cols)
 
     else:
         raise ValueError('`backend` not supported')
 
 
 def plot_cubes(cube, mode='slider', backend='matplotlib', dpi=100,
                figtype='png', vmin=None, vmax=None, size=100, width=360,
@@ -929,19 +934,19 @@
     **kwargs : dictionary, optional
         [mode='animation'] Arguments to be passed to ``plot_frames`` to
         customize each frame of the animation (adding markers, using a log
         scale, etc).
 
     Notes
     -----
-    http://holoviews.org/getting_started/Gridded_Datasets.html
-    http://holoviews.org/user_guide/Gridded_Datasets.html
-    http://holoviews.org/user_guide/Applying_Customizations.html
+    https://holoviews.org/getting_started/Gridded_Datasets.html
+    https://holoviews.org/user_guide/Gridded_Datasets.html
+    https://holoviews.org/user_guide/Applying_Customizations.html
     """
-    hv.extension(backend)
+    extension(backend)
 
     if not isinstance(cube, np.ndarray):
         raise TypeError('`cube` must be a numpy.ndarray')
 
     if cmap is None:
         cmap = default_cmap
 
@@ -952,54 +957,54 @@
 
         if cube.ndim == 3:
             # Dataset((X, Y, Z), Data), where
             # X is a 1D array of shape M ,
             # Y is a 1D array of shape N and
             # Z is a 1D array of shape O
             # Data is a ND array of shape NxMxO
-            ds = hv.Dataset((range(cube.shape[2]), range(cube.shape[1]),
-                             range(cube.shape[0]), cube), ['x', 'y', 'time'],
-                            'flux')
+            ds = Dataset((range(cube.shape[2]), range(cube.shape[1]),
+                         range(cube.shape[0]), cube), ['x', 'y', 'time'],
+                         'flux')
             max_frames = cube.shape[0]
         elif cube.ndim == 4:
             # adding a lambda dimension
-            ds = hv.Dataset((range(cube.shape[3]), range(cube.shape[2]),
-                             range(cube.shape[1]), range(cube.shape[0]), cube),
-                            ['x', 'y', 'time', 'lambda'], 'flux')
+            ds = Dataset((range(cube.shape[3]), range(cube.shape[2]),
+                          range(cube.shape[1]), range(cube.shape[0]), cube),
+                         ['x', 'y', 'time', 'lambda'], 'flux')
             max_frames = cube.shape[0] * cube.shape[1]
 
         # Matplotlib takes None but not Bokeh. We take global min & max instead
         if vmin is None:
             vmin = cube.min()
         if vmax is None:
             vmax = cube.max()
 
         print(ds)
         print(":Cube_shape\t{}".format(list(cube.shape[::-1])))
 
         # not working for bokeh: dpi
-        image_stack = ds.to(hv.Image, kdims=['x', 'y'], dynamic=dynamic)
-        hv.output(backend=backend, size=size, dpi=dpi, fig=figtype,
-                  max_frames=max_frames)
+        image_stack = ds.to(Image, kdims=['x', 'y'], dynamic=dynamic)
+        output(backend=backend, size=size, dpi=dpi, fig=figtype,
+               max_frames=max_frames)
 
         if backend == 'matplotlib':
             # keywords in the currently active 'matplotlib' renderer are:
             # 'alpha', 'clims', 'cmap', 'filterrad', 'interpolation', 'norm',
             # 'visible'
-            #options = "Image (cmap='" + cmap + "', interpolation='nearest',"
-            #options += " clims=("+str(vmin)+','+str(vmax)+")"+")"
-            #opts(options, image_stack)
+            # options = "Image (cmap='" + cmap + "', interpolation='nearest',"
+            # options += " clims=("+str(vmin)+','+str(vmax)+")"+")"
+            # opts(options, image_stack)
             return image_stack.opts(opts.Image(colorbar=colorbar,
                                                cmap=cmap,
                                                clim=(vmin, vmax)))
             # hv.save(image_stack, 'holomap.gif', fps=5)
 
         elif backend == 'bokeh':
-            #options = "Image (cmap='" + cmap + "')"
-            #opts(options, image_stack)
+            # options = "Image (cmap='" + cmap + "')"
+            # opts(options, image_stack)
             # Compensating the width to accommodate the colorbar
             if colorbar:
                 cb_wid = 15
                 cb_pad = 3
                 tick_len = len(str(int(cube.max())))
                 if tick_len < 4:
                     cb_tick = 25
@@ -1058,36 +1063,36 @@
                 label_step_range = range(label_step_range[0],
                                          label_step_range[1])
             elif len(label_step_range) == 3:
                 label_step_range = range(label_step_range[0],
                                          label_step_range[1],
                                          label_step_range[2])
 
-        if os.path.exists(dir_path):
-            shutil.rmtree(dir_path)
+        if exists(dir_path):
+            rmtree(dir_path)
             print('Replacing ' + dir_path)
-        os.mkdir(dir_path)
+        mkdir(dir_path)
 
         print('Producing each animation frame...')
         for i, labstep in zip(data_step_range, list(label_step_range)):
             if label is None:
                 label = 'frame '
             savelabel = dir_path + label + str(i + 100)
             plot_frames(cube[i], backend='matplotlib', mode='mosaic',
                         save=savelabel, dpi=dpi, vmin=vmin, vmax=vmax,
                         colorbar=colorbar, cmap=cmap,
-                        label=[label + str(labstep + 1)], **kwargs)
+                        label=tuple([label + str(labstep + 1)]), **kwargs)
         try:
             filename = anim_path + '.' + anim_format
             call(['convert', '-delay', str(delay), dir_path + '*.png',
                   filename])
-            if os.path.exists(filename):
+            if exists(filename):
                 print('Animation successfully saved to disk as ' + filename)
                 if delete_anim_cache:
-                    shutil.rmtree(dir_path)
+                    rmtree(dir_path)
                     print('Temp directory deleted ' + dir_path)
 
         except FileNotFoundError:
             print('ImageMagick `convert` command could not be found')
 
     else:
         raise ValueError("`mode` is not recognized")
```

### Comparing `hciplot-0.2.4/hciplot.egg-info/PKG-INFO` & `hciplot-0.2.5/hciplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hciplot
-Version: 0.2.4
+Version: 0.2.5
 Summary: High-contrast Imaging Plotting library
 Home-page: https://github.com/carlgogo/hciplot
 Download-URL: https://github.com/carlgogo/hciplot/archive/refs/tags/v0.1.8.tar.gz
 Author: Carlos Alberto Gomez Gonzalez, Valentin Christiaens
 Author-email: valentinchrist@hotmail.com
 License: MIT
 Keywords: plotting,hci,package
```

### Comparing `hciplot-0.2.4/setup.py` & `hciplot-0.2.5/setup.py`

 * *Files identical despite different names*

