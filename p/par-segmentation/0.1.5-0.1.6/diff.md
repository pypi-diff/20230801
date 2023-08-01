# Comparing `tmp/par_segmentation-0.1.5.tar.gz` & `tmp/par_segmentation-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "par_segmentation-0.1.5.tar", last modified: Wed Apr 26 14:28:37 2023, max compression
+gzip compressed data, was "/home/runner/work/par-segmentation/par-segmentation/dist/.tmp-yphhugs8/par_segmentation-0.1.6.tar", last modified: Tue Aug  1 16:14:54 2023, max compression
```

## Comparing `par_segmentation-0.1.5.tar` & `par_segmentation-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:28:37.631277 par_segmentation-0.1.5/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 par_segmentation-0.1.5/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     5380 2023-04-26 14:28:37.631569 par_segmentation-0.1.5/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     4352 2023-02-01 14:17:05.000000 par_segmentation-0.1.5/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:28:37.466907 par_segmentation-0.1.5/par_segmentation/
--rw-r--r--   0 blandt   (743162876) 1934034978      136 2023-01-18 17:11:30.000000 par_segmentation-0.1.5/par_segmentation/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978    18880 2023-01-25 15:05:51.000000 par_segmentation-0.1.5/par_segmentation/funcs.py
--rw-r--r--   0 blandt   (743162876) 1934034978    15490 2023-01-31 11:47:21.000000 par_segmentation-0.1.5/par_segmentation/interactive.py
--rw-r--r--   0 blandt   (743162876) 1934034978    15993 2023-01-18 17:11:30.000000 par_segmentation-0.1.5/par_segmentation/legacy.py
--rw-r--r--   0 blandt   (743162876) 1934034978    16693 2023-01-27 22:47:32.000000 par_segmentation-0.1.5/par_segmentation/model.py
--rw-r--r--   0 blandt   (743162876) 1934034978    10511 2023-01-31 12:14:21.000000 par_segmentation-0.1.5/par_segmentation/quantifier.py
--rw-r--r--   0 blandt   (743162876) 1934034978    14337 2023-01-18 17:11:30.000000 par_segmentation-0.1.5/par_segmentation/roi.py
--rw-r--r--   0 blandt   (743162876) 1934034978    16402 2023-01-18 17:11:30.000000 par_segmentation-0.1.5/par_segmentation/tgf_interpolate.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:28:37.480894 par_segmentation-0.1.5/par_segmentation.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     5380 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      590 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      114 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       23 2023-04-26 14:28:36.000000 par_segmentation-0.1.5/par_segmentation.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:28:37.634613 par_segmentation-0.1.5/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978     1032 2023-04-26 14:28:08.000000 par_segmentation-0.1.5/setup.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:28:37.630017 par_segmentation-0.1.5/tests/
--rw-r--r--   0 blandt   (743162876) 1934034978        0 2023-01-18 12:19:25.000000 par_segmentation-0.1.5/tests/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978      774 2023-01-31 12:24:18.000000 par_segmentation-0.1.5/tests/test_de_completion.py
--rw-r--r--   0 blandt   (743162876) 1934034978     1230 2023-01-27 15:24:33.000000 par_segmentation-0.1.5/tests/test_de_correct.py
--rw-r--r--   0 blandt   (743162876) 1934034978     2355 2023-01-27 22:07:48.000000 par_segmentation-0.1.5/tests/test_gd_completion.py
--rw-r--r--   0 blandt   (743162876) 1934034978     1147 2023-01-27 15:24:33.000000 par_segmentation-0.1.5/tests/test_gd_correct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/quantifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/tgf_interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/test_de_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/test_de_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/test_gd_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/test_gd_correct.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `par_segmentation-0.1.5/LICENSE` & `par_segmentation-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.5/README.md` & `par_segmentation-0.1.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,67 @@
 # PAR Segmentation
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
 [![PyPi version](https://badgen.net/pypi/v/par-segmentation/)](https://pypi.org/project/par-segmentation)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
+[![run with docker](https://img.shields.io/badge/run%20with-docker-0db7ed?logo=docker)](https://www.docker.com/)
+[![run with conda](http://img.shields.io/badge/run%20with-conda-3EB049?logo=anaconda)](https://docs.conda.io/en/latest/)
 
-Tools for segmenting and straightening the cortex of cells from midplane images using a gradient descent algorithm.
-Designed primarily for use on images of PAR proteins in C. elegans zygotes.
+Tools for segmenting, straightening and quantifying the cortex of cells.
+Works by combining spline-based segmentation with a custom quantification model, using a gradient descent optimisation procedure.
+Designed primarily for membrane-bound PAR proteins in C. elegans zygotes.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation.gif" width="100%" height="100%"/>
 </p>
 
+
+## Instructions
+
+As a first step, I would recommend checking out the [tutorial notebook](https://nbviewer.org/github/tsmbland/par-segmentation/blob/master/scripts/Tutorial.ipynb). To run the notebook interactively you have a few options:
+
+#### Option 1: Binder
+
+To run in the cloud using Binder, click here: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
+
+(Please note that it may take several minutes to open the notebook)
+
+#### Option 2: Docker
+
+Step 1: With [Docker](https://www.docker.com/products/docker-desktop/) open on your machine,  pull the image (copy and paste into the terminal)
+
+    docker pull tsmbland/par-segmentation
+
+Step 2: Run the docker container (copy and paste into the terminal)
+
+    docker run -p 8888:8888 tsmbland/par-segmentation
+
+This will print a URL at the bottom for you to copy and paste into your web browser to open up Jupyter
+
+Step 3: When finished, delete the container and image
+    
+    docker container prune -f
+    docker image rm tsmbland/par-segmentation
+
+#### Option 3: Conda
+
+You can use the environment.yml file to set up a [Conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html) environment on your machine from which the notebook can be run
+
+    conda env create -f environment.yml
+    conda activate par-segmentation
+    jupyter notebook
+
+
+## Installation
+
+To explore further and incorporate into your own analysis pipelines, you can install the package using pip:
+
+    pip install par-segmentation
+
 ## Methods
 
 Starting with an initial rough manual ROI of the cell edge, the cortex of the image is straightened (Step 1).
 The program then attempts to mimic this straightened image by differentiable simulation (Step 2).
 In doing so, it learns the position of the cortex, which enables the ROI to be adjusted (Step 3) and the cortex re-straightened.
 
 <p align="center">
@@ -38,26 +84,17 @@
 The program learns the amplitude of these two components at each position around the cortex, so can serve as a quantification tool as well as a segmentation tool:
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation2.gif" width="100%" height="100%"/>
 </p>
 
 The model is a slight simplification of reality, and doesn't account for the possibility of a non-Gaussian PSF and complex 3D light-scattering behaviours, but is a close enough approximation for many purposes. 
-Nevertheless, we can relax these assumptions if higher quantification accuracy is required. 
+Nevertheless, one can relax these assumptions if higher quantification accuracy is required. 
 See [here](https://github.com/tsmbland/discco) for an extension of the method designed for more accurate quantification.
 
-## Installation
-
-    pip install par-segmentation
-
-## Instructions
-
-See the tutorial notebook [here](scripts/Tutorial.ipynb)
-
-To run in the cloud click 'launch binder' at the top
 
 ## Publications
 
 Code in this repository has been used in the following publications for PAR protein segmentation and/or quantification: 
 
 Illukkumbura, R., Hirani, N., Borrego-Pinto, J., Bland, T., Ng, K., Hubatsch, L., McQuade, J., Endres, R.G., and Goehring, N.W. (2022). Design principles for selective polarization of PAR proteins by cortical flows. BioRxiv 2022.09.05.506621.
```

### Comparing `par_segmentation-0.1.5/par_segmentation/funcs.py` & `par_segmentation-0.1.6/par_segmentation/funcs.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.5/par_segmentation/interactive.py` & `par_segmentation-0.1.6/par_segmentation/interactive.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.5/par_segmentation/legacy.py` & `par_segmentation-0.1.6/par_segmentation/legacy.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.5/par_segmentation/model.py` & `par_segmentation-0.1.6/par_segmentation/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 from scipy.interpolate import interp1d
 from tqdm import tqdm
 import time
 from .tgf_interpolate import interpolate
 import matplotlib.pyplot as plt
 from typing import Union, Tuple
 
+"""
+To do:
+- use a spline based method for nfits
+
+"""
+
 
 class ImageQuantGradientDescent:
 
     def __init__(self,
                  img: Union[np.ndarray, list],
                  roi: Union[np.ndarray, list],
                  sigma: float = 3.5,
```

### Comparing `par_segmentation-0.1.5/par_segmentation/quantifier.py` & `par_segmentation-0.1.6/par_segmentation/quantifier.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.5/par_segmentation/roi.py` & `par_segmentation-0.1.6/par_segmentation/roi.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.5/par_segmentation/tgf_interpolate.py` & `par_segmentation-0.1.6/par_segmentation/tgf_interpolate.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.5/par_segmentation.egg-info/SOURCES.txt` & `par_segmentation-0.1.6/par_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.5/setup.py` & `par_segmentation-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='par_segmentation',
-    version='0.1.5',
+    version='0.1.6',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib',
                       'scipy',
```

### Comparing `par_segmentation-0.1.5/tests/test_gd_completion.py` & `par_segmentation-0.1.6/tests/test_gd_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,58 @@
-import unittest
 from par_segmentation import *
 
 
-class GdCompletionTests(unittest.TestCase):
+
+class TestGdCompletion:
     """
 
     GRADIENT DESCENT COMPLETION TESTS
 
     Testing that the gradient descent optimiser runs to completion
     NOT testing that any results are as expected
 
     """
 
-    @classmethod
-    def setUpClass(cls):
-        path = os.path.dirname(os.path.abspath(__file__)) + '/../data/dataset2_par2_neon'
-        paths = direcslist(path)[:2]
-        cls.imgs = [load_image(p + '/af_corrected.tif') for p in paths]
-        cls.rois = [np.loadtxt(p + '/ROI.txt') for p in paths]
+    path = os.path.dirname(os.path.abspath(__file__)) + '/../scripts'
+    imgs = [load_image(os.path.dirname(os.path.abspath(__file__)) + '/../scripts/nwg338_af_corrected.tif'),]
+    rois = [np.loadtxt(os.path.dirname(os.path.abspath(__file__)) + '/../scripts/nwg338_ROI_manual.txt'),]
 
-    def test1(self):
+    def test_1(self):
         # Testing that it runs to completion with default parameters
         iq = ImageQuant(img=self.imgs, roi=self.rois, method='GD', descent_steps=10, verbose=False)
         iq.run()
         res = iq.compile_res()
 
-    def test2(self):
+    def test_2(self):
         # Testing that it runs to completion with periodic False
         iq = ImageQuant(img=self.imgs, roi=self.rois, method='GD', descent_steps=10, verbose=False, periodic=False)
         iq.run()
 
-    def test3(self):
+    def test_3(self):
         # Testing that it runs to completion with rotate True
         iq = ImageQuant(img=self.imgs, roi=self.rois, method='GD', descent_steps=10, verbose=False, rotate=True)
         iq.run()
 
-    def test4(self):
+    def test_4(self):
         # Testing that it runs to completion with adaptive sigma True
         iq = ImageQuant(img=self.imgs, roi=self.rois, method='GD', descent_steps=10, verbose=False, adaptive_sigma=True)
         iq.run()
 
-    def test5(self):
+    def test_5(self):
         # Testing that it runs to completion with adaptive batch_norm True
         iq = ImageQuant(img=self.imgs, roi=self.rois, method='GD', descent_steps=10, verbose=False, batch_norm=True)
         iq.run()
 
-    def test6(self):
+    def test_6(self):
         # Testing that it runs to completion with fit_outer False
         iq = ImageQuant(img=self.imgs, roi=self.rois, method='GD', descent_steps=10, verbose=False, fit_outer=False)
         iq.run()
 
-    def test7(self):
+    def test_7(self):
         # Testing that it runs to completion with nfits None
         iq = ImageQuant(img=self.imgs, roi=self.rois, method='GD', descent_steps=10, verbose=False, nfits=None)
         iq.run()
 
-    def test8(self):
+    def test_8(self):
         # Testing that it runs to completion with zerocap True
         iq = ImageQuant(img=self.imgs, roi=self.rois, method='GD', descent_steps=10, verbose=False, zerocap=True)
         iq.run()
```

