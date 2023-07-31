# Comparing `tmp/simpsom-2.0.2.tar.gz` & `tmp/simpsom-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/federico comitani/GitHub/simpsom/dist/tmp57v_k1fe/simpsom-2.0.2.tar", last modified: Wed Oct 12 01:08:25 2022, max compression
+gzip compressed data, was "simpsom-3.0.0b0.tar", last modified: Mon Jul 31 23:00:04 2023, max compression
```

## Comparing `simpsom-2.0.2.tar` & `simpsom-3.0.0b0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) 818713947        0 2022-10-12 01:08:25.000000 simpsom-2.0.2/
--rw-r--r--   0 root         (0) 818713947     1066 2022-10-12 00:45:32.000000 simpsom-2.0.2/LICENSE.txt
--rw-r--r--   0 root         (0) 818713947       38 2021-12-10 17:00:53.000000 simpsom-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) 818713947     8608 2022-10-12 01:08:25.000000 simpsom-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) 818713947     7888 2022-10-12 00:49:48.000000 simpsom-2.0.2/README.md
--rw-r--r--   0 root         (0) 818713947      145 2022-10-12 01:08:25.000000 simpsom-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) 818713947     1414 2022-10-12 00:59:49.000000 simpsom-2.0.2/setup.py
-drwxr-xr-x   0 root         (0) 818713947        0 2022-10-12 01:08:25.000000 simpsom-2.0.2/simpsom/
--rw-r--r--   0 root         (0) 818713947     2701 2022-10-12 00:45:33.000000 simpsom-2.0.2/simpsom/__init__.py
--rw-r--r--   0 root         (0) 818713947       50 2022-10-12 00:47:35.000000 simpsom-2.0.2/simpsom/_version.py
-drwxr-xr-x   0 root         (0) 818713947        0 2022-10-12 01:08:25.000000 simpsom-2.0.2/simpsom/cluster/
--rw-r--r--   0 root         (0) 818713947      176 2022-10-12 00:45:33.000000 simpsom-2.0.2/simpsom/cluster/__init__.py
--rw-r--r--   0 root         (0) 818713947    20688 2022-10-12 00:45:33.000000 simpsom-2.0.2/simpsom/cluster/density_peak.py
--rw-r--r--   0 root         (0) 818713947     5542 2022-10-12 00:45:33.000000 simpsom-2.0.2/simpsom/cluster/quality_threshold.py
--rw-r--r--   0 root         (0) 818713947     2265 2022-10-12 00:45:33.000000 simpsom-2.0.2/simpsom/hexagons.py
--rw-r--r--   0 root         (0) 818713947     2225 2022-10-12 00:45:33.000000 simpsom-2.0.2/simpsom/interface.py
--rw-r--r--   0 root         (0) 818713947    40230 2022-10-12 01:07:40.000000 simpsom-2.0.2/simpsom/network.py
-drwxr-xr-x   0 root         (0) 818713947        0 2022-10-12 01:08:25.000000 simpsom-2.0.2/simpsom.egg-info/
--rw-r--r--   0 root         (0) 818713947     8608 2022-10-12 01:08:25.000000 simpsom-2.0.2/simpsom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) 818713947      433 2022-10-12 01:08:25.000000 simpsom-2.0.2/simpsom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) 818713947        1 2022-10-12 01:08:25.000000 simpsom-2.0.2/simpsom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) 818713947        1 2021-12-10 17:49:17.000000 simpsom-2.0.2/simpsom.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) 818713947       88 2022-10-12 01:08:25.000000 simpsom-2.0.2/simpsom.egg-info/requires.txt
--rw-r--r--   0 root         (0) 818713947        8 2022-10-12 01:08:25.000000 simpsom-2.0.2/simpsom.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) 818713947        0 2023-07-31 23:00:04.557648 simpsom-3.0.0b0/
+-rw-r--r--   0 root         (0) 818713947    35150 2023-02-22 02:51:34.000000 simpsom-3.0.0b0/LICENSE.txt
+-rw-r--r--   0 root         (0) 818713947       38 2021-12-10 17:00:53.000000 simpsom-3.0.0b0/MANIFEST.in
+-rw-r--r--   0 root         (0) 818713947     4498 2023-07-31 23:00:04.557882 simpsom-3.0.0b0/PKG-INFO
+-rw-r--r--   0 root         (0) 818713947     3734 2022-11-17 02:40:44.000000 simpsom-3.0.0b0/README.md
+-rw-r--r--   0 root         (0) 818713947      145 2023-07-31 23:00:04.558797 simpsom-3.0.0b0/setup.cfg
+-rw-r--r--   0 root         (0) 818713947     1615 2023-07-31 22:59:53.000000 simpsom-3.0.0b0/setup.py
+drwxr-xr-x   0 root         (0) 818713947        0 2023-07-31 23:00:04.553272 simpsom-3.0.0b0/simpsom/
+-rw-r--r--   0 root         (0) 818713947      273 2023-02-22 02:51:34.000000 simpsom-3.0.0b0/simpsom/__init__.py
+-rw-r--r--   0 root         (0) 818713947       24 2023-07-31 22:57:12.000000 simpsom-3.0.0b0/simpsom/_version.py
+-rwxr-xr-x   0 root         (0) 818713947     6304 2023-07-31 22:39:58.000000 simpsom-3.0.0b0/simpsom/distances.py
+-rw-r--r--   0 root         (0) 818713947     2598 2022-10-28 01:16:51.000000 simpsom-3.0.0b0/simpsom/early_stop.py
+-rwxr-xr-x   0 root         (0) 818713947     3849 2023-07-31 22:39:58.000000 simpsom-3.0.0b0/simpsom/neighborhoods.py
+-rw-r--r--   0 root         (0) 818713947    42380 2023-07-31 22:39:58.000000 simpsom-3.0.0b0/simpsom/network.py
+-rw-r--r--   0 root         (0) 818713947     8745 2023-02-22 02:51:34.000000 simpsom-3.0.0b0/simpsom/plots.py
+-rw-r--r--   0 root         (0) 818713947    13329 2022-10-28 01:16:51.000000 simpsom-3.0.0b0/simpsom/polygons.py
+drwxr-xr-x   0 root         (0) 818713947        0 2023-07-31 23:00:04.556670 simpsom-3.0.0b0/simpsom.egg-info/
+-rw-r--r--   0 root         (0) 818713947     4498 2023-07-31 23:00:04.000000 simpsom-3.0.0b0/simpsom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) 818713947      422 2023-07-31 23:00:04.000000 simpsom-3.0.0b0/simpsom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) 818713947        1 2023-07-31 23:00:04.000000 simpsom-3.0.0b0/simpsom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) 818713947        1 2021-12-10 17:49:17.000000 simpsom-3.0.0b0/simpsom.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) 818713947      111 2023-07-31 23:00:04.000000 simpsom-3.0.0b0/simpsom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) 818713947        8 2023-07-31 23:00:04.000000 simpsom-3.0.0b0/simpsom.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) 818713947        0 2023-07-31 23:00:04.557206 simpsom-3.0.0b0/tests/
+-rw-r--r--   0 root         (0) 818713947     9260 2023-07-31 22:39:58.000000 simpsom-3.0.0b0/tests/test_network.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `simpsom-2.0.2/setup.py` & `simpsom-3.0.0b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,38 +15,41 @@
 
     name='simpsom',
 
     version=version,
 
     description='Simple Self-Organizing Maps in Python',
     long_description=long_description,
+    long_description_content_type='text/markdown',
 
     url='https://github.com/fcomitani/simpsom',
-	download_url = 'https://github.com/fcomitani/simpsom/archive/'+version+'.tar.gz', 
+    download_url = 'https://github.com/fcomitani/simpsom/archive/'+version+'.tar.gz', 
     author='Federico Comitani',
     author_email='federico.comitani@gmail.com',
 
     license='MIT',
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
-	'Programming Language :: Python :: 3'
-		],
+        'Programming Language :: Python :: 3'
+    ],
 
     keywords='kohonen self-organizing maps, self-organizing maps, clustering ,dimension-reduction, som',
 
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
 
-    install_requires=['numpy>=1.19.5',
-		'scikit-learn>=0.22.2.post1',
-		'matplotlib>=3.3.3'],
+    install_requires=['numpy>=1.23.4',
+                      'scikit-learn>=1.1.2',
+                      'matplotlib>=3.3.3',
+                      'loguru>=0.5.3',
+                      'pylettes>=0.2.0'],
 
     extras_require={ 'gpu': ['cupy==8.60',
-				'cuml==0.18']},
+                             'cuml==0.18']},
     zip_safe=False,
 
 )
```

### Comparing `simpsom-2.0.2/simpsom/network.py` & `simpsom-3.0.0b0/simpsom/network.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,934 +1,1000 @@
-"""
-SimpSOM (Simple Self-Organizing Maps) v2.0.2
-F. Comitani @2017-2022
- 
-A lightweight python library for Kohonen Self-Organizing Maps (SOM).
-"""
-
-from __future__ import print_function
-
+import multiprocessing
+import os
 import sys
-import os, errno
-
-import random 
-from math import sqrt, exp, log
+import random
+from functools import partial
+from types import ModuleType
+from typing import Union, List, Tuple
+
+import numpy as np
+from loguru import logger
+
+from simpsom.distances import Distance
+from simpsom.early_stop import EarlyStop
+from simpsom.neighborhoods import Neighborhoods
+from simpsom.plots import plot_map, line_plot, scatter_on_map
+from simpsom.polygons import Squares, Hexagons, Polygon
 
-import matplotlib.pyplot as plt
-from matplotlib import cm
-import matplotlib.patches as mpatches
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-
-import simpsom.interface as interface
-import simpsom.hexagons as hx
-from simpsom.cluster import density_peak as dp
-from simpsom.cluster import quality_threshold as qt
 
 class SOMNet:
     """ Kohonen SOM Network class. """
 
-    def __init__(self, net_height, net_width, data, load_file=None, metric='euclidean', metric_kwds={},
-                 init='PCA', PBC=False, GPU=False, random_seed=None):
-
-        """Initialise the SOM network.
+    __slots__ = ('output_path', 'cluster_algo', 'xp', 'nodes', 'data', 'metric',
+                 'polygons', 'distance', 'neighborhood_fun', 'neighborhoods',
+                 'convergence', 'height', 'width', 'init', 'PBC', 'GPU', 'CUML',
+                 'nodes_list', 'start_sigma', 'start_learning_rate', 'epochs',
+                 'tau', 'sigma', 'learning_rate')
+                 
+    def __init__(self, net_height: int, net_width: int, data: np.ndarray,
+                 load_file: str = None, metric: str = "euclidean",
+                 topology: str = "hexagonal", neighborhood_fun: str = "gaussian",
+                 init: str = "random", PBC: bool = False,
+                 GPU: bool = False, CUML: bool = False,
+                 random_seed: int = None, debug: bool = False, output_path: str = "./") -> None:
+        """ Initialize the SOM network.
 
         Args:
             net_height (int): Number of nodes along the first dimension.
             net_width (int): Numer of nodes along the second dimension.
-            data (self.interface.num.array or list): N-dimensional dataset.
-            load_file (str, optional): Name of file to load containing information 
+            data (array): N-dimensional dataset.
+            load_file (str): Name of file to load containing information
                 to initialize the network weights.
             metric (string): distance metric for the identification of best matching
-                units. Accepts metrics available in scikit-learn (default 'euclidean').
-            metric_kwds (dict): dictionary with optional keywords to pass to the chosen
-                metric (default {}).
-            init (str or list of self.interface.num.array): Nodes initialization method, to be chosen between 'random'
-                or 'PCA' (default 'PCA'). Alternatively a couple of vectors can be provided
-                whose values will be spanned uniformly.
+                units. Accepted metrics are euclidean, manhattan, and cosine (default "euclidean").
+            topology (str): topology of the map tiling.
+                Accepted shapes are hexagonal, and square (default "hexagonal").
+            neighborhood_fun (str): neighbours drop-off function for training, choose among gaussian,
+                mexican_hat and bubble (default "gaussian").
+            init (str or list[array, ...]): Nodes initialization method, choose between random
+                or PCA (default "random").
             PBC (boolean): Activate/deactivate periodic boundary conditions,
-                warning: only quality threshold clustering algorithm works with PBC (default 0).
-            GPU (boolean): Activate/deactivate GPU run with RAPIDS (requires CUDA).
+                warning: only quality threshold clustering algorithm works with PBC (default False).
+            GPU (boolean): Activate/deactivate GPU run with RAPIDS (requires CUDA, default False).
+            CUML (boolean): Use CUML for clustering. If deactivate, use scikit-learn instead
+                (requires CUDA, default False).
             random_seed (int): Seed for the random numbers generator (default None).
-                
+            debug (bool): Set logging level printed to screen as debug.
+            out_path (str): Path to the folder where all data and plots will be saved
+                (default, current folder).
         """
 
+        self.output_path = output_path
+
+        if not debug:
+            logger.remove()
+            logger.add(sys.stderr, level="INFO")
+
+        self.GPU = bool(GPU)
+        self.CUML = bool(CUML)
+
+        if self.GPU:
+            try:
+                import cupy
+                self.xp = cupy
+
+                if self.CUML:
+                    try:
+                        from cuml import cluster
+                    except:
+                        logger.warning(
+                            "CUML libraries not found. Scikit-learn will be used instead.")
+
+            except:
+                logger.warning(
+                    "CuPy libraries not found. Falling back to CPU.")
+                self.GPU = False
+
+        try:
+            self.xp
+        except:
+            self.xp = np
+
+        try:
+            cluster
+        except:
+            from sklearn import cluster
+        self.cluster_algo = cluster
+
         if random_seed is not None:
+            os.environ["PYTHONHASHSEED"] = str(random_seed)
+            np.random.seed(random_seed)
             random.seed(random_seed)
+            self.xp.random.seed(random_seed)
 
-        """ Set CPU/GPU libraries. """
+        self.PBC = bool(PBC)
+        if self.PBC:
+            logger.info("Periodic Boundary Conditions active.")
 
-        self.interface = interface.InterfaceGPU() if bool(GPU)\
-                            else interface.InterfaceCPU() 
+        self.nodes_list = []
+        self.data = self.xp.array(data, dtype=self.xp.float32)
 
-        """ Switch to activate special workflow if running the colors example. """
-        self.color_ex = False
+        self.metric = metric
 
-        """ Switch to activate periodic boundary conditions. """
-        self.PBC = bool(PBC)
+        if topology.lower() == "hexagonal":
+            self.polygons = Hexagons
+            logger.info("Hexagonal topology.")
+        else:
+            self.polygons = Squares
+            logger.info("Square topology.")
 
-        if self.PBC:
-            print("Periodic Boundary Conditions active.")
+        self.distance = Distance(self.xp)
+
+        self.neighborhood_fun = neighborhood_fun.lower()
+        if self.neighborhood_fun not in ['gaussian', 'mexican_hat', 'bubble']:
+            logger.error("{} neighborhood function not recognized.".format(self.neighborhood_fun) +
+                         "Choose among 'gaussian', 'mexican_hat' or 'bubble'.")
+            raise ValueError
+
+        self.convergence = []
+
+        self.height = net_height
+        self.width = net_width
+
+        self.init = init
+        if isinstance(self.init, str):
+            self.init = self.init.lower()
         else:
-            print("Periodic Boundary Conditions inactive.")
+            self.init = self.xp.array(self.init)
+        self._set_weights(load_file)
+
+    def _get(self, data: np.ndarray) -> np.ndarray:
+        """ Moves data from GPU to CPU.
+        If already on CPU, it will be left as it is.
+
+        Args:
+            data (array): data to move from GPU to CPU.
+
+        Returns:
+            (array): the same data on CPU.
+        """
 
-        self.node_list = []
-        self.data = self.interface.num.array(data)\
-                         .astype(self.interface.num.float32)
-        
-        self.metric      = metric
-        self.metric_kwds = metric_kwds
-        
-        self.convergence   = []
-
-        """ Load the weights from file, generate them randomly or from PCA. """
-
-        init_vec     = None
-        init_bounds  = None
-        wei_array    = None
+        if self.xp.__name__ == "cupy":
+            if isinstance(data, list):
+                return [d.get() for d in data]
+            elif isinstance(data, np.ndarray):
+                return data
+            return data.get()
+
+        return data
+
+    def _set_weights(self, load_file: str = None) -> None:
+        """ Set initial map weights values, either by loading them from file or with random/PCA.
+
+        Args:
+            load_file (str): Name of file to load containing information
+                to initialize the network weights.
+        """
+
+        init_vec = None
+        weights_array = None
+        this_weight = None
+
+        # When loaded from file, element 0 contains information on the network shape
+        count_weight = 3
 
         if load_file is None:
-            self.net_height = net_height
-            self.net_width  = net_width
 
-            if init == 'PCA':
-                print("The weights will be initialized with PCA.")
-            
-                pca     = self.interface.PCA(n_components = 2)
-                pca.fit(self.data)
-                init_vec = pca.components_
-            
-            elif init == 'random':
-                print("The weights will be initialized randomly.")
-
-                for i in range(self.data.shape[1]):
-                    init_bounds = [self.interface.num.min(self.data,axis=0),
-                                   self.interface.num.max(self.data,axis=0)]
-            
-            else: 
-                print("Custom weights provided.")
-
-                init_vec = init
-
-        else:   
-            print('The weights will be loaded from file.')
-
-            if load_file.endswith('.npy')==False:
-                load_file = load_file+'.npy'
-            wei_array = self.interface.num.load(load_file)
-            #add something to check that data and array have the same dimensions,
-            #or that they are mutually exclusive
-            self.net_height = int(wei_array[0][0])
-            self.net_width  = int(wei_array[0][1])
-            self.PBC        = bool(wei_array[0][2])
-
-        """ When loaded from file, element 0 contains information on the network shape."""
-        count_wei = 1
-
-        """ Set the weights. """
-
-        for x in range(self.net_width):
-            for y in range(self.net_height):
-
-                #if weights were loaded from file
-                this_wei = wei_array[count_wei] if wei_array is not None\
-                                                else None
-                count_wei += 1
-
-                self.node_list.append(SOMNode(x, y, self.data.shape[1], \
-                    self.net_height, self.net_width, self.PBC, self.interface,\
-                    wei_bounds=init_bounds, init_vec=init_vec, wei_array=this_wei))
+            if isinstance(self.init, str) and self.init == "pca":
+                logger.warning(
+                    "Please make sure that the data have been standardized before using PCA.")
+                logger.info("The weights will be initialized with PCA.")
+
+                if self.GPU:
+                    matrix = self.data.get()
+                    init_vec = self.pca(matrix, n_pca=2)
+                    init_vec = self.xp.array(init_vec)
+                else:
+                    matrix = self.data
+                    init_vec = self.pca(matrix, n_pca=2)
 
-    def save(self, fileName='SOMNet_trained', out_path='./'):
-    
+            else:
+                logger.info("The weights will be initialized randomly.")
+                init_vec = [self.xp.min(self.data, axis=0),
+                            self.xp.max(self.data, axis=0)]
+
+        else:
+            logger.info("The weights will be loaded from file.\n" +
+                        "The map shape will be overwritten and no weights" +
+                        "initialization will be applied.")
+            if not load_file.endswith(".npy"):
+                load_file += ".npy"
+            weights_array = np.load(load_file, allow_pickle=True)
+            self.height = int(weights_array[0][0])
+            self.width = int(weights_array[1][0])
+            self.PBC = bool(weights_array[2][0])
+
+        for x in range(self.width):
+            for y in range(self.height):
+
+                if weights_array is not None:
+                    this_weight = weights_array[count_weight]
+                    count_weight += 1
+
+                self.nodes_list.append(SOMNode(x, y, self.data.shape[1],
+                                               self.height, self.width,
+                                               self.PBC, self.polygons,
+                                               self.xp,
+                                               init_vec=init_vec,
+                                               weights_array=this_weight))
+
+    def pca(self, matrix: np.ndarray, n_pca: int) -> np.ndarray:
+        """Get principal components to initialize network weights.
+
+        Args:
+            matrix (array): N-dimensional dataset.
+            n_pca (int): number of components to keep.
+
+        Returns:
+            (array): Principal axes in feature space,
+                representing the directions of maximum variance in the data.
+        """
+
+        mean_vector = np.mean(matrix.T, axis=1)
+        center_mat = matrix - mean_vector
+        cov_mat = np.cov(center_mat.T).astype(self.xp.float32)
+
+        return np.linalg.eig(cov_mat)[-1].T[:n_pca]
+
+    def _get_n_process(self) -> int:
+        """ Count number of GPU or CPU processors.
+
+        Returns:
+            (int): the number of processors.
+        """
+
+        if self.xp.__name__ == "cupy":
+            try:
+                dev = self.xp.cuda.Device()
+                n_smp = dev.attributes["MultiProcessorCount"]
+                max_thread_per_smp = dev.attributes["MaxThreadsPerMultiProcessor"]
+                return n_smp * max_thread_per_smp
+            except:
+                logger.error("Something went wrong when trying to count the number\n" +
+                             "of GPU processors from CuPy.")
+                return -1
+
+        else:
+            try:
+                return multiprocessing.cpu_count()
+            except:
+                logger.error("Something went wrong when trying to count the number\n" +
+                             "of CPU processors.")
+                return -1
+
+    def _randomize_dataset(self, data: np.ndarray, epochs: int) -> np.ndarray:
+        """Generates a random list of datapoints indices for online training.
+
+        Args:
+            data (array or list): N-dimensional dataset.
+            epochs (int): Number of training iterations.
+
+        Returns:
+            entries (array): array with randomized indices
+        """
+
+        if epochs < data.shape[0]:
+            logger.warning(
+                "Epochs for online training are less than the input datapoints.")
+            epochs = data.shape[0]
+
+        iterations = int(np.ceil(epochs / data.shape[0]))
+
+        return [ix
+                for shuffled in [np.random.permutation(data.shape[0])
+                                 for it in np.arange(iterations)]
+                for ix in shuffled]
+
+    def save_map(self, file_name: str = "trained_som.npy") -> None:
         """Saves the network dimensions, the pbc and nodes weights to a file.
 
         Args:
-            fileName (str, optional): Name of file where the data will be saved.
-            out_path (str, optional): Path to the folder where data will be saved.
+            file_name (str): Name of the file where the data will be saved.
         """
-        
-        wei_array = [self.interface.num.zeros(len(self.node_list[0].weights))]
-        wei_array[0][0], wei_array[0][1], wei_array[0][2] = self.net_height, self.net_width, int(self.PBC)
-        for node in self.node_list:
-            wei_array.append(node.weights)
-        self.interface.num.save(os.path.join(out_path,fileName), self.interface.num.asarray(wei_array))
-    
 
-    def update_sigma(self, n_iter):
-    
+        weights_array = [[float(self.height)] * self.nodes_list[0].weights.shape[0],
+                         [float(self.width)] *
+                         self.nodes_list[0].weights.shape[0],
+                         [float(self.PBC)] * self.nodes_list[0].weights.shape[0]] + \
+                        [self._get(node.weights) for node in self.nodes_list]
+
+        if not file_name.endswith((".npy")):
+            file_name += ".npy"
+        logger.info("Map shape and weights will be saved to:\n" +
+                    os.path.join(self.output_path, file_name))
+        np.save(os.path.join(self.output_path, file_name),
+                np.array(weights_array))
+
+    def _update_sigma(self, n_iter: int) -> None:
         """Update the gaussian sigma.
 
-        Args:           
+        Args:
             n_iter (int): Iteration number.
-            
         """
-    
-        self.sigma = self.start_sigma * exp(-n_iter/self.tau)
-    
 
-    def update_learning_rate(self, n_iter):
-    
+        self.sigma = self.start_sigma * self.xp.exp(-n_iter / self.tau)
+
+    def _update_learning_rate(self, n_iter: int) -> None:
         """Update the learning rate.
 
-        Args:           
+        Args:
             n_iter (int): Iteration number.
-            
         """
-        
-        self.learning_rate =  self.start_learning_rate * exp(n_iter/self.epochs)
-    
 
-    def find_bmu_ix(self, vecs):
-    
+        self.learning_rate = self.start_learning_rate * \
+                             self.xp.exp(-n_iter / self.epochs)
+
+    def find_bmu_ix(self, vecs: np.array) -> 'SOMNode':
         """Find the index of the best matching unit (BMU) for a given list of vectors.
 
-        Args:           
-            vec (2d self.interface.num.array or list of lists): vectors whose distance from the network
+        Args:
+            vec (array or list[lists, ..]): vectors whose distance from the network
                 nodes will be calculated.
-            
-        Returns:            
+
+        Returns:
             bmu (SOMNode): The best matching unit node index.
-            
         """
-        
-        dists = self.interface.pairdist(vecs,
-                        self.interface.num.array([n.weights for n in self.node_list]), 
-                        metric=self.metric, **self.metric_kwds)
-
-        return self.interface.num.argmin(dists,axis=1)
-   
-    def train(self, train_algo='batch', epochs=-1, start_learning_rate=0.01,  
-                early_stop=None, early_stop_patience=3, early_stop_tolerance=1e-4,
-                batch_size=-1):
-    
+
+        dists = self.distance.pairdist(vecs,
+                                       self.xp.array(
+                                           [n.weights for n in self.nodes_list]),
+                                       metric=self.metric)
+
+        return self.xp.argmin(dists, axis=1)
+
+    def train(self, train_algo: str = "batch", epochs: int = -1,
+              start_learning_rate: float = 0.01, early_stop: str = None,
+              early_stop_patience: int = 3, early_stop_tolerance: float = 1e-4, batch_size: int = -1) -> None:
         """Train the SOM.
 
         Args:
-            train_algo (str): training algorithm, choose between 'online' or 'batch' 
-                (default 'online'). Beware that the online algorithm will run one datapoint
+            train_algo (str): training algorithm, choose between "online" or "batch"
+                (default "online"). Beware that the online algorithm will run one datapoint
                 per epoch, while the batch algorithm runs all points at one for each epoch.
             epochs (int): Number of training iterations. If not selected (or -1)
-                automatically set epochs as 10 times the number of datapoints. 
+                automatically set epochs as 10 times the number of datapoints.
+                Warning: for online training each epoch corresponds to 1 sample in the
+                input dataset, for batch training it corresponds to one full dataset
+                training.
             start_learning_rate (float): Initial learning rate, used only in online
                 learning.
-            early_stop (str): Early stopping method, for now only 'mapdiff' (checks if the
-                weights of nodes don't change) and 'bmudiff' (checks if the assigned bmu to each sample
-                don't change) are available. If None, don't use early stopping (default None).
-            early_stop_patience (int): Number of iterations without improvement before stopping the 
+            early_stop (str): Early stopping method, for now only "mapdiff" (checks if the
+                weights of nodes don"t change) is available. If None, don"t use early stopping (default None).
+            early_stop_patience (int): Number of iterations without improvement before stopping the
                 training, only available for batch training (default 3).
             early_stop_tolerance (float): Improvement tolerance, if the map does not improve beyond
                 this threshold, the early stopping counter will be activated (it needs to be set
                 appropriately depending on the used distance metric). Ignored if early stopping
                 is off (default 1e-4).
-            batch_size (int): Split the dataset in batches of this size when calculating the 
-                new weights, works only when train_algo is 'batch' and helps keeping down the 
+            batch_size (int): Split the dataset in batches of this size when calculating the
+                new weights, works only when train_algo is "batch" and helps keeping down the
                 memory requirements when working with large datasets, if -1 run the whole dataset
-                at once. 
-
+                at once.
         """
 
-        print("The map will be trained with the "+train_algo+" algorithm.")
-        self.start_sigma = max(self.net_height, self.net_width)/2
+        logger.info("The map will be trained with the " +
+                    train_algo + " algorithm.")
+        self.start_sigma = max(self.height, self.width) / 2
         self.start_learning_rate = start_learning_rate
 
+        self.data = self.xp.array(self.data)
+
         if epochs == -1:
-            epochs  = self.data.shape[0]*10
-            
+            if train_algo == 'online':
+                epochs = self.data.shape[0] * 10
+            else:
+                epochs = 10
+
         self.epochs = epochs
-        self.tau    = self.epochs/log(self.start_sigma)
+        self.tau = self.epochs / self.xp.log(self.start_sigma)
+
+        if early_stop not in ["mapdiff", None]:
+            logger.warning("Convergence method not recognized, early stopping will be deactivated. " +
+                           "Currently only \"mapdiff\" is available.")
+            early_stop = None
+
+        if early_stop is not None:
+            logger.info("Early stop active.")
+            logger.warning("Early stop is an experimental feature, " +
+                           "make sure to know what you are doing!")
+
+        early_stopper = EarlyStop(tolerance=early_stop_tolerance,
+                                  patience=early_stop_patience)
 
         if batch_size == -1 or batch_size > self.data.shape[0]:
-            batch_size = self.data.shape[0]
+            _n_parallel = self._get_n_process()
+        else:
+            _n_parallel = batch_size
 
-        if train_algo == 'online':
+        if train_algo == "online":
             """ Online training.
-                Bootstrap: one datapoint is extracted randomly with replacement at each epoch 
-                and used to update the weights.
+            Bootstrap: one datapoint is extracted randomly with replacement at each epoch
+            and used to update the weights.
             """
 
+            datapoints_ix = self._randomize_dataset(self.data, self.epochs)
+
             for n_iter in range(self.epochs):
 
-                if n_iter%10==0:
-                    print("\rTraining SOM... {:d}%".format(int(n_iter*100.0/self.epochs)), end=' ')
+                if early_stopper.stop_training:
+                    logger.info(
+                        "\rEarly stop tolerance reached at epoch {:d}, training will be stopped.".format(n_iter - 1))
+                    self.convergence = early_stopper.convergence
+                    break
 
-                self.update_sigma(n_iter)
-                self.update_learning_rate(n_iter)
+                if n_iter % 10 == 0:
+                    logger.debug("\rTraining SOM... {:d}%".format(
+                        int(n_iter * 100.0 / self.epochs)))
 
-                input_vec = self.data[random.randint(0, self.data.shape[0]-1), :].reshape(1,self.data.shape[1])
-                
-                bmu = self.node_list[int(self.find_bmu_ix(input_vec)[0])]
+                self._update_sigma(n_iter)
+                self._update_learning_rate(n_iter)
 
-                for node in self.node_list:
-                    node.update_weights(input_vec[0], self.sigma, self.learning_rate, bmu)
+                datapoint_ix = datapoints_ix.pop()
+                input_vec = self.data[datapoint_ix, :].reshape(
+                    1, self.data.shape[1])
 
-        elif train_algo == 'batch':
+                bmu = self.nodes_list[int(self.find_bmu_ix(input_vec)[0])]
+
+                for node in self.nodes_list:
+                    node._update_weights(
+                        input_vec[0], self.sigma, self.learning_rate, bmu)
+
+                if n_iter % self.data.shape[0] == 0 and early_stop is not None:
+                    early_stopper.check_convergence(
+                        early_stopper.calc_loss(self))
+
+        elif train_algo == "batch":
             """ Batch training.
-                All datapoints are used at once for each epoch, 
-                the weights are updated with the sum of contributions from all these points.
-                No learning rate needed.
+            All datapoints are used at once for each epoch,
+            the weights are updated with the sum of contributions from all these points.
+            No learning rate needed.
 
-                Kinouchi, M. et al. "Quick Learning for Batch-Learning Self-Organizing Map" (2002).
+            Kinouchi, M. et al. "Quick Learning for Batch-Learning Self-Organizing Map" (2002).
             """
-    
-            #Storing the distances and weight matrices defeats the purpose of having
-            #nodes as instances of a class, but it helps with the optimization
-            #and parallelization at the cost of memory.
-            #The object-oriented structure is kept to simplify code reading. 
-
-            """ Calculate the square euclidean distance matrix to speed up batch training. """
 
+            # Storing the distances and weight matrices defeats the purpose of having
+            # nodes as instances of a class, but it helps with the optimization
+            # and parallelization at the cost of memory.
+            # The object-oriented structure is kept to simplify code reading.
 
-            dist_matrix_sq = self.interface.num.zeros((self.net_width*self.net_height, 
-                                        self.net_width*self.net_height)) 
+            all_weights = self.xp.array([n.weights for n in self.nodes_list], dtype=self.xp.float32)
+            all_weights = all_weights.reshape(self.width, self.height, self.data.shape[1])
 
-            for i in range(self.net_width*self.net_height):
-                for j in range(i + 1, self.net_width*self.net_height):
-                    dist_matrix_sq[i,j] = self.interface.num.linalg.norm(self.node_list[i].pos-self.node_list[j].pos)
-            
-            dist_matrix_sq += dist_matrix_sq.T
-            dist_matrix_sq *= dist_matrix_sq
+            numerator = self.xp.zeros(all_weights.shape, dtype=self.xp.float32)
+            denominator = self.xp.zeros(
+                (all_weights.shape[0], all_weights.shape[1], 1), dtype=self.xp.float32)
 
-            """ Store all weights as matrix. """
+            unravel_precomputed = self.xp.unravel_index(self.xp.arange(self.width * self.height, dtype=self.xp.int64), (self.width, self.height))
 
-            all_weights = self.interface.num.array([n.weights for n in self.node_list])
+            _xx, _yy = self.xp.meshgrid(self.xp.arange(self.width), self.xp.arange(self.height))
 
-            early_stop_counter = 0
+            if self.PBC:
+                pbc_func_params = self.polygons.neighborhood_pbc
+            else:
+                pbc_func_params = None
 
-            for n_iter in range(self.epochs):
+            neighborhoods = Neighborhoods(self.xp, _xx, _yy, pbc_func_params)
 
-                """ Early stop check. """
+            sq_weights = None
 
-                if early_stop_counter == early_stop_patience:
+            for n_iter in range(self.epochs):
 
-                    print("\rTolerance reached at epoch {:d}, stopping training.".format(n_iter-1))
+                if self.metric in ["euclidean", "cosine"]:
+                    sq_weights = (self.xp.power(all_weights.reshape(-1, all_weights.shape[2]), 2).sum(axis=1, keepdims=True))
 
+                if early_stopper.stop_training:
+                    logger.info(
+                        "\rEarly stop tolerance reached at epoch {:d}, training will be stopped.".format(n_iter - 1))
+                    self.convergence = early_stopper.convergence
                     break
 
-                self.update_sigma(n_iter)
-                
-                """ Matrix of gaussian effects. """
+                self._update_sigma(n_iter)
+                self._update_learning_rate(n_iter)
 
-                gauss = self.interface.num.exp(-dist_matrix_sq/(2*self.sigma*self.sigma))
+                if n_iter % 10 == 0:
+                    logger.debug("Training SOM... {:.2f}%".format(
+                        n_iter * 100.0 / self.epochs))
 
-                if n_iter%10==0:
-                    print("\rTraining SOM... {:d}%".format(int(n_iter*100.0/self.epochs)), end=' ')
-                        
-                """ Run through mini batches to ease the memory burden. """
+                try:
+                    numerator.fill(0)
+                    denominator.fill(0)
+                except AttributeError:
+                    numerator = self.xp.zeros(all_weights.shape, dtype=self.xp.float32)
+                    denominator = self.xp.zeros((all_weights.shape[0], all_weights.shape[1], 1), dtype=self.xp.float32)
 
-                numerator   = self.interface.num.zeros((self.net_width*self.net_height, 
-                                        self.data.shape[1])) 
-                denominator =  self.interface.num.zeros((self.net_width*self.net_height, 
-                                        self.data.shape[1]))
+                for i in range(0, len(self.data), _n_parallel):
+                    start = i
+                    end = start + _n_parallel
+                    if end > len(self.data):
+                        end = len(self.data)
 
-                for b in range(int((self.data.shape[0]+batch_size-1)/batch_size)):
-                    
-                    batchdata = self.data[b*batch_size : min((b+1)*batch_size,self.data.shape[0])]
+                    batchdata = self.data[start:end]
 
-                    """ Find BMUs for all points and subselect gaussian matrix. """
+                    # Find BMUs for all points and subselect gaussian matrix.
+                    dists = self.distance.batchpairdist(batchdata, all_weights, sq_weights, self.metric)
 
-                    dists = self.interface.pairdist(batchdata, all_weights,  
-                                    metric=self.metric, **self.metric_kwds)
-                    bmus = self.interface.num.argmin(dists, axis=1)
+                    raveled_idxs = dists.argmin(axis=1)
+                    wins = (unravel_precomputed[0][raveled_idxs], unravel_precomputed[1][raveled_idxs])
 
-                    batchgauss = gauss[bmus]
-                    denominator += self.interface.num.repeat(batchgauss.sum(axis=0)[:, self.interface.num.newaxis], self.data.shape[1], axis=1)
+                    g_gpu = neighborhoods.neighborhood_caller(self.neighborhood_fun, wins, self.sigma) * self.learning_rate
 
-                    batchgauss = self.interface.num.repeat(batchgauss[:, :, self.interface.num.newaxis], self.data.shape[1], axis=2)
-                    batchdata = self.interface.num.repeat(batchdata[:, self.interface.num.newaxis, :], gauss.shape[1], axis=1)
+                    sum_g_gpu = self.xp.sum(g_gpu, axis=0)
+                    g_flat_gpu = g_gpu.reshape(g_gpu.shape[0], -1)
+                    gT_dot_x_flat_gpu = self.xp.dot(g_flat_gpu.T, batchdata)
 
-                    numerator  += self.interface.num.multiply(batchgauss,batchdata).sum(axis=0)
+                    numerator += gT_dot_x_flat_gpu.reshape(numerator.shape)
+                    denominator += sum_g_gpu[:, :, self.xp.newaxis]
 
-                new_weights = self.interface.num.divide(numerator,denominator)
-                new_weights[self.interface.num.isnan(new_weights)] = all_weights[self.interface.num.isnan(new_weights)] 
-
-                """ Early stopping, active if patience is not None """
+                new_weights = self.xp.where(
+                    denominator != 0, numerator / denominator, all_weights)
 
                 if early_stop is not None:
+                    loss = self.xp.abs(self.xp.subtract(
+                        new_weights, all_weights)).mean()
+                    early_stopper.check_convergence(loss)
 
-                    #These are pretty ruough convergence tests
-                    #To do: add more
-
-                    if early_stop == 'mapdiff':      
-
-                        """ Checks if the map weights are not moving. """
+                all_weights = new_weights
 
-                        self.convergence.append(self.interface.pairdist(new_weights,all_weights,  
-                                metric=self.metric, **self.metric_kwds).mean())
-                    
-                    elif early_stop == 'bmudiff':
+            # Revert to object oriented
+            all_weights = all_weights.reshape(self.width * self.height, self.data.shape[1])
+            for n_node, node in enumerate(self.nodes_list):
+                node.weights = all_weights[n_node]
 
-                        """ Checks if the bmus mean distance from the samples has stopped improving. """
+        else:
+            logger.error(
+                "Training algorithm not recognized. Choose between \"online\" and \"batch\".")
+            sys.exit(1)
+
+        if self.GPU:
+            for node in self.nodes_list:
+                node.weights = node.weights.get()
+        if early_stop is not None:
+            self.convergence = [arr.get(
+            ) for arr in early_stopper.convergence] if self.GPU else early_stopper.convergence
+
+    def get_nodes_difference(self) -> None:
+        """ Extracts the neighbouring nodes difference in weights and assigns it
+        to each node object.
+        """
+
+        weights = self.xp.array([node.weights for node in self.nodes_list])
+        pos = self.xp.array([node.pos for node in self.nodes_list])
+        weights_dist = self.distance.pairdist(
+            weights, weights, metric=self.metric)
+
+        # if self.PBC:
+        # TODO: a precision issue with the PBC nodes position creates an ugly line
+        # at the top and bottom of the map.
+        #    pos_dist = self.polygons.distance_pbc(pos, pos,
+        #        net_shape=(self.width,self.height),
+        #        distance_func=lambda x, y: self.distance.pairdist(x, y, metric='euclidean'),
+        #        xp=self.xp,
+        #        axis=0)
+        # else:
+        pos_dist = self.distance.pairdist(pos, pos, metric='euclidean')
+
+        weights_dist[(pos_dist > 1.01) | (pos_dist == 0.)] = np.nan
+        [node._set_difference(value)
+         for node, value in zip(self.nodes_list, self.xp.nanmean(weights_dist, axis=0))]
+
+        logger.info('Weights difference among neighboring nodes calculated.')
+
+    def project_onto_map(self, array: np.ndarray,
+                         file_name: str = "./som_projected.npy") -> list:
+        """Project the datapoints of a given array to the 2D space of the
+        SOM by calculating the bmus.
+
+        Args:
+            array (array): An array containing datapoints to be mapped.
+            file_name (str): Name of the file to which the data will be saved
+                if not None.
 
-                        self.convergence.append(self.interface.num.min(dists,axis=1).mean())
+        Returns:
+            (list): bmu x,y position for each input array datapoint.
+        """
 
-                    else:
-                        sys.exit('Error: convergence method not recognized. Choose between \'mapdiff\' and \'bmudiff\'.')
+        if not isinstance(array, self.xp.ndarray):
+            array = self.xp.array(array)
 
-                    if n_iter > 0 and self.convergence[-2]-self.convergence[-1] < early_stop_tolerance:
-                        early_stop_counter += 1
-                    else:
-                        early_stop_counter  = 0
+        bmu_list = [
+            self.nodes_list[int(mu)].pos for mu in self.find_bmu_ix(array)]
 
-                all_weights = new_weights
+        if file_name is not None:
+            if not file_name.endswith((".npy")):
+                file_name += ".npy"
+            logger.info("Projected coordinates will be saved to:\n" +
+                        os.path.join(self.output_path, file_name))
+            np.save(os.path.join(self.output_path,
+                                 file_name), self._get(bmu_list))
 
-            """ Store final weights in the nodes objects. """
-            #Revert back to object oriented
-            
-            for n_iter, node in enumerate(self.node_list):
-                node.weights = all_weights[n_iter] # * self.learning_rate
-
-            if early_stop is not None:
-
-                """ Plot convergence if it was tracked. """
-                
-                self.plot_convergence(logax=False)
+        return self.xp.array(bmu_list)
 
-        else:
-            sys.exit('Error: training algorithm not recognized. Choose between \'online\' and \'batch\'.')
-                        
-        print("\rTraining SOM... done!")
-
-    def plot_convergence(self, logax=False, show=False, print_out=False, out_path='./'):
-
-        """ Plot the the map training progress according to the 
-            chosen convergence criterion.
-            
-        Args: 
-            logax (bool, optional): if True, plot convergence on logarithmic y axis.
-            show (bool, optional): Choose to display the plot.
-            print_out (bool, optional): Choose to save the plot to a file.
-            out_path (str, optional): Path to the folder where data will be saved.
-        """
-
-
-        fig=plt.figure(figsize=(30,10))
-        fig, ax = plt.subplots()
-        
-        ax.set_facecolor('white')
-        plt.grid(color='#aaaaaa')
-        
-        plt.plot(self.convergence, color='#444444')
-        plt.xticks(fontsize=15)
-        plt.yticks(fontsize=15)
-
-        if logax:
-            ax.set_yscale('log')
-        
-        ax.spines['right'].set_visible(False)
-        ax.spines['top'].set_visible(False)
-
-        plt.xlabel('Iteration', fontsize=15)
-        plt.ylabel('Convergence score', fontsize=15)
-
-        print_name = os.path.join(out_path,'convergence.png')
-        
-        if print_out == True:
-            plt.savefig(print_name, bbox_inches='tight', dpi=300)
-        if show == True:
-            plt.show()
-        if show != False and print_out != False:
-            plt.clf()
-
-
-    def nodes_graph(self, colnum=0, show=False, print_out=True, out_path='./', colname=None):
-    
-        """Plot a 2D map with hexagonal nodes and weights values
-
-        Args:
-            colnum (int): The index of the weight that will be shown as colormap.
-            show (bool, optional): Choose to display the plot.
-            print_out (bool, optional): Choose to save the plot to a file.
-            colname (str, optional): Name of the column to be shown on the map.
-            out_path (str, optional): Path to the folder where data will be saved.
-        """
-
-        if not colname:
-            colname = str(colnum)
-
-        centers = [[node.pos[0],node.pos[1]] for node in self.node_list]
-        
-        side    = sqrt(self.net_width*self.net_height)
-        width_p = 100
-        dpi     = 72
-        xInch   = self.net_width*width_p/dpi 
-        yInch   = self.net_height*width_p/dpi 
-        fig     = plt.figure(figsize=(xInch, yInch), dpi=dpi)
-
-        cols = [self.interface.get_value(node.weights) for node in self.node_list]
-        
-        if self.color_ex==True:
-            ax = hx.plot_hex(fig, centers, cols, color_ex=self.color_ex)
-            ax.set_title('Node Grid w Color Features', size=4*side)
-            print_name=os.path.join(out_path,'nodes_colors.png')
+    def cluster(self, coor: np.ndarray, project: bool = True, algorithm: str = "DBSCAN",
+                file_name: str = "./som_clusters.npy", **kwargs: str) -> List[int]:
+        """Project data onto the map and find clusters with scikit-learn clustering algorithms.
 
-        else:
-            cols = [c[colnum] for c in cols]
-            ax = hx.plot_hex(fig, centers, cols)
-            ax.set_title('Node Grid w Feature ' +  colname, size=4*side)
-            divider = make_axes_locatable(ax)
-            cax = divider.append_axes("right", size="5%", pad=0.0)
-            cbar=plt.colorbar(ax.collections[0], cax=cax)
-            cbar.set_label(colname, size=4*side, labelpad=2.5*side)
-            cbar.ax.tick_params(labelsize=2*side)
-            cbar.outline.set_visible(False)
-
-            plt.sca(ax)
-            print_name=os.path.join(out_path,'nodes_feature_'+str(colnum)+'.png')
-            
-        if print_out==True:
-            plt.savefig(print_name, bbox_inches='tight', dpi=dpi)
-        if show==True:
-            plt.show()
-        if show!=False and print_out!=False:
-            plt.clf()
-
-    def diff_graph(self, show=False, print_out=True, returns=False, out_path='./'):
-    
-        """Plot a 2D map with nodes and weights difference among neighboring nodes.
-
-        Args:
-            show (bool, optional): Choose to display the plot.
-            print_out (bool, optional): Choose to save the plot to a file.
-            returns (bool, optional): Choose to return the difference value.
-            out_path (str, optional): Path to the folder where data will be saved.
+        Args:
+            coor (array): An array containing datapoints to be mapped or
+                pre-mapped if project False.
+            project (bool): if True, project the points in coor onto the map.
+            algorithm (clustering obj or str): The clusters identification algorithm. A scikit-like
+                class can be provided (must have a fit method), or a string indicating one of the algorithms
+                provided by the scikit library
+            file_name (str): Name of the file to which the data will be saved
+                if not None.
+            kwargs (dict): Keyword arguments to the clustering algorithm:
 
-        Returns:
-            (list): difference value for each node.             
-        """
-        
-        """ Find adjacent nodes in the grid. """
-        
-        #print(type(self.node_list[0].weights))
-        #print(type(self.node_list[0].get_node_distance(self.node_list[1])))
-        #print(self.node_list[0].get_node_distance(self.node_list[1])<= 1.001)
-        #pippo=[[node2.weights for node2 in self.node_list \
-        #                            if node != node2 and node.get_node_distance(node2) <= 1.001]
-        #                             for node in self.node_list]
-        #print(pippo, len(pippo), len(pippo[0]))
-        #print(self.interface.num.array)
-        #print(self.interface.num.array(pippo))
-        
-
-        neighbors = [self.interface.num.array([node2.weights for node2 in self.node_list \
-                    if node != node2 and node.get_node_distance(node2) <= 1.001])
-                    for node in self.node_list]
-
-        """ Calculate the summed weight difference. """
-
-        diffs = [self.interface.get_value(
-                 self.interface.pairdist(n.weights.reshape(1,n.weights.shape[0]),
-                                         neighbors[i], 
-                                         metric='euclidean', **self.metric_kwds).mean())\
-                 for i,n in enumerate(self.node_list)]
-
-        """ Define plotting hexagon centers. """
-
-        centers = [[node.pos[0],node.pos[1]] for node in self.node_list]
-
-        """ Set up and plot. """
-
-        if show == True or print_out==True:
-        
-            side    = sqrt(self.net_width*self.net_height)
-            width_p = 100
-            dpi     = 72
-            x_inch  = self.net_width*width_p/dpi 
-            y_inch  = self.net_height*width_p/dpi 
-            fig     = plt.figure(figsize=(x_inch, y_inch), dpi=dpi)
-
-            ax = hx.plot_hex(fig, centers, diffs)
-            ax.set_title('Nodes Grid w Weights Difference', size=4*side)
-            divider = make_axes_locatable(ax)
-            cax     = divider.append_axes("right", size="5%", pad=0.0)
-            cbar    = plt.colorbar(ax.collections[0], cax=cax)
-            cbar.set_label('Weights Difference', size=4*side, labelpad=2.5*side)
-            cbar.ax.tick_params(labelsize=2*side)
-            cbar.outline.set_visible(False)
-
-            plt.sca(ax)
-            print_name = os.path.join(out_path,'nodes_difference.png')
-            
-            if print_out == True:
-                plt.savefig(print_name, bbox_inches='tight', dpi=dpi)
-            if show == True:
-                plt.show()
-            if show != False and print_out != False:
-                plt.clf()
-
-        if returns == True:
-            return diffs 
-
-    def project(self, array, colnum=-1, labels=[], show=False, print_out=True, out_path='./', colname = None):
-
-        """Project the datapoints of a given array to the 2D space of the 
-            SOM by calculating the bmus. If requested plot a 2D map with as 
-            implemented in nodes_graph and adds circles to the bmu
-            of each datapoint in a given array.
-
-        Args:
-            array (self.interface.num.array): An array containing datapoints to be mapped.
-            colnum (int): The index of the weight that will be shown as colormap. 
-                If not chosen, the difference map will be used instead.
-            show (bool, optional): Choose to display the plot.
-            print_out (bool, optional): Choose to save the plot to a file.
-            out_path (str, optional): Path to the folder where data will be saved.
-            colname (str, optional): Name of the column to be shown on the map.
-            
-        Returns:
-            (list): bmu x,y position for each input array datapoint. 
-            
+            Returns:
+            (list of int): A list containing the clusters of the input array datapoints.
         """
-        
-        if not colname:
-            colname = str(colnum)
-
-        if labels != []:
-            colors  = ['#a6cee3','#1f78b4','#b2df8a','#33a02c','#fb9a99','#e31a1c',
-                       '#fdbf6f','#ff7f00','#cab2d6','#6a3d9a','#ffff99','#b15928']
-            counter = 0
-            class_assignment = {}
-            for i in range(len(labels)):
-                if labels[i] not in class_assignment:
-                    class_assignment[labels[i]] = colors[counter]
-                    counter = (counter + 1)%len(colors)
-        
-        if not isinstance(array, self.interface.num.ndarray):
-            array = self.interface.num.array(array)\
-                    .astype(self.interface.num.float64)
-
-        bmu_list, cls = [], []
-        bmu_list = [self.node_list[int(mu)].pos for mu in self.find_bmu_ix(array)]
-        
-        if self.color_ex:
-            cls = self.interface.get_value(array)
-        else: 
-            if labels != []:   
-                cls = [class_assignment[labels[i]] for i in range(array.shape[0])]
-            elif colnum == -1:
-                cls = ['#ffffff']*array.shape[0]
-            else: 
-                cls = self.interface.get_value(array[:,colnum])
-
-        if show == True or print_out == True:
-        
-            """ Call nodes_graph/diff_graph to first build the 2D map of the nodes. """
-            
-            side = sqrt(self.net_width*self.net_height)
-
-            if self.color_ex == True:
-                print_name = os.path.join(out_path,'color_projection.png')
-                self.nodes_graph(colnum, False, False)
-                plt.scatter([pos[0] for pos in bmu_list],[pos[1] for pos in bmu_list], color=cls,  
-                        s=500, edgecolor='#ffffff', linewidth=5, zorder=10)
-                plt.title('Datapoints Projection', size=4*side)
-            else:
-                #a random perturbation is added to the points positions so that data 
-                #belonging plotted to the same bmu will be visible in the plot      
-                if colnum == -1:
-                    print_name = os.path.join(out_path,'projection_difference.png')
-                    self.diff_graph(False, False, False)
-                    plt.scatter([pos[0]-0.125+random.random()*0.25 for pos in bmu_list],
-                                [pos[1]-0.125+random.random()*0.25 for pos in bmu_list], c=cls, cmap=cm.viridis,
-                                 s=200, linewidth=0, zorder=10)
-                    plt.title('Datapoints Projection on Nodes Difference', size=4*side)
-                else:   
-                    print_name = os.path.join(out_path,'projection_'+ colname +'.png')
-                    self.nodes_graph(colnum, False, False, colname=colname)
-                    plt.scatter([pos[0]-0.125+random.random()*0.25 for pos in bmu_list],
-                                [pos[1]-0.125+random.random()*0.25 for pos in bmu_list], c=cls, cmap=cm.viridis,
-                                 s=200, edgecolor='#ffffff', linewidth=4, zorder=10)
-                    plt.title('Datapoints Projection #' +  str(colnum), size=4*side)
-                
-            if labels != [ ] and not self.color_ex:
-                recs = []
-                for i in class_assignment:
-                    recs.append(mpatches.Rectangle((0,0),1,1,fc=class_assignment[i]))
-
-                plt.legend(recs, class_assignment.keys(), loc=(1.25,0), frameon=False, fontsize=2*side)
-
-            if print_out == True:
-                plt.savefig(print_name, bbox_inches='tight', dpi=72)
-            if show == True:
-                plt.show()
-            plt.clf()
-        
-        """ Print the x,y coordinates of bmus, useful for the clustering function. """
-        
-        return [[pos[0],pos[1]] for pos in bmu_list] 
-        
-        
-    def cluster(self, array, clus_type='qthresh', cutoff=5, quant=0.2, percent=0.02, num_cl=8,\
-                    save_file=True, file_type='dat', show=False, print_out=True, out_path='./'):
-    
-        """Clusters the data in a given array according to the SOM trained map.
-            The clusters can also be plotted.
-
-        Args:
-            array (self.interface.num.array): An array containing datapoints to be clustered.
-            clus_type (str, optional): The type of clustering to be applied, so far only quality threshold (qthresh) 
-                algorithm is directly implemented, other algorithms require sklearn.
-            cutoff (float, optional): Cutoff for the quality threshold algorithm. This also doubles as
-                maximum distance of two points to be considered in the same cluster with DBSCAN.
-            percent (float, optional): The percentile that defines the reference distance in density peak clustering (dpeak).
-            num_cl (int, optional): The number of clusters for K-Means clustering
-            quant (float, optional): Quantile used to calculate the bandwidth of the mean shift algorithm.
-            save_file (bool, optional): Choose to save the resulting clusters in a text file.
-            file_type (string, optional): Format of the file where the clusters will be saved (csv or dat)
-            show (bool, optional): Choose to display the plot.
-            print_out (bool, optional): Choose to save the plot to a file.
-            out_path (str, optional): Path to the folder where data will be saved.
-            
-        Returns:
-            (list of int): A nested list containing the clusters with indexes of the input array points.
-            
-        """
-
-        """ Call project to first find the bmu for each array datapoint, but without producing any graph. """
 
-        bmu_list = self.project(array, show=False, print_out=False)
-        clusters = []
+        bmu_coor = self.project_onto_map(coor, file_name="som_projected_" + algorithm + ".npy") \
+            if project else coor
+        if self.xp.__name__ == "cupy" and self.cluster_algo.__name__.startswith('sklearn'):
+            bmu_coor = self._get(bmu_coor)
 
-        if clus_type == 'qthresh':
-            
-            """ Cluster according to the quality threshold algorithm (slow!). """
-    
-            clusters = qt.quality_threshold(bmu_list, cutoff, self.PBC, self.net_height, self.net_width)
-
-        elif clus_type == 'dpeak':
+        if self.PBC:
+            # Implementing the distance_pbc as a wrapper automatically applied to the provided metric
+            # is not possible as many sklearn clustering functions don't allow for custom metric.
+            logger.warning("PBC are active. Make sure to provide a PBC-compatible custom metric if possible, " +
+                           "or use `polygons.distance_pbc`. See the documentation for more detail.")
+
+        if type(algorithm) is str:
+
+            import inspect
+            modules = [module[0] for module in inspect.getmembers(
+                self.cluster_algo, inspect.isclass)]
+
+            if algorithm not in modules:
+                logger.error("The desired algorithm is not among the algorithms provided by the scikit library,\n" +
+                             "please provide one of the algorithms provided by the scikit library:\n" +
+                             "|".join(modules))
+                return None, None
 
-            """ Cluster according to the density peak algorithm. """
+            clu_algo = eval("self.cluster_algo." + algorithm)
 
-            clusters = dp.density_peak(bmu_list, PBC=self.PBC, net_height=self.net_height, net_width=self.net_width)
+        else:
+            clu_algo = algorithm
 
-        elif clus_type in ['MeanShift', 'DBSCAN', 'KMeans']:
-        
-            """ Cluster according to algorithms implemented in sklearn. """
-        
-            if self.PBC == True:
-                print("Warning: Only Quality Threshold and Density Peak clustering work with PBC")
+            if not callable(getattr(clu_algo, "fit", None)):
+                logger.error(
+                    "There was a problem with the clustering, make sure to provide a scikit-like clustering\n" +
+                    "class or use one of the algorithms provided by the scikit library,\n" +
+                    "Custom classes must have a 'fit' method.")
+                return None, None
+
+        clu_algo = clu_algo(**kwargs)
+
+        try:
+            clu_labs = clu_algo.fit(bmu_coor).labels_
+        except:
+            logger.error("There was a problem with the clustering, make sure to provide a scikit-like clustering\n" +
+                         "class or use one of the algorithms provided by the scikit library,\n" +
+                         "Custom classes must have a 'fit' method.")
+            return None
+
+        if file_name is not None:
+            if not file_name.endswith((".npy")):
+                file_name += ".npy"
+            logger.info("Clustering results will be saved to:\n" +
+                        os.path.join(self.output_path, file_name))
+            np.save(os.path.join(self.output_path,
+                                 file_name), self._get(clu_labs))
+
+        return clu_labs, bmu_coor
+
+    def plot_map_by_feature(self, feature_ix: int, show: bool = False, print_out: bool = True,
+                            **kwargs: Tuple[int]) -> None:
+        """ Wrapper function to plot a trained 2D SOM map
+        color-coded according to a given feature.
+
+        Args:
+            feature_ix (int): The feature index number to use as color map.
+            show (bool): Choose to display the plot.
+            print_out (bool): Choose to save the plot to a file.
+            kwargs (dict): Keyword arguments to format the plot, such as 
+                - figsize (tuple(int, int)), the figure size;
+                - title (str), figure title;
+                - cbar_label (str), colorbar label;
+                - labelsize (int), font size of label, the title 15% larger, ticks 15% smaller;
+                - cmap (ListedColormap), a custom cmap.
+        """
+
+        if "file_name" not in kwargs.keys():
+            kwargs["file_name"] = os.path.join(self.output_path,
+                                               "./som_feature_{}.png".format(str(feature_ix)))
+
+        _, _ = plot_map([[node.pos[0], node.pos[1]] for node in self.nodes_list],
+                        [node.weights[feature_ix] for node in self.nodes_list],
+                        self.polygons,
+                        show=show, print_out=print_out,
+                        **kwargs)
+
+        if print_out:
+            logger.info("Feature map will be saved to:\n" +
+                        kwargs["file_name"])
+
+    def plot_map_by_difference(self, show: bool = False, print_out: bool = True,
+                               **kwargs: Tuple[int]) -> None:
+        """ Wrapper function to plot a trained 2D SOM map
+        color-coded according neighbours weights difference.
+        It will automatically calculate the difference values
+        if not already computed.
+
+        Args:
+            show (bool): Choose to display the plot.
+            print_out (bool): Choose to save the plot to a file.
+            kwargs (dict): Keyword arguments to format the plot, such as
+                - figsize (tuple(int, int)), the figure size;
+                - title (str), figure title;
+                - cbar_label (str), colorbar label;
+                - labelsize (int), font size of label, the title 15% larger, ticks 15% smaller;
+                - cmap (ListedColormap), a custom cmap.
+        """
+
+        if "file_name" not in kwargs.keys():
+            kwargs["file_name"] = os.path.join(
+                self.output_path, "./som_difference.png")
+
+        if self.nodes_list[0].difference is None:
+            self.get_nodes_difference()
+
+        if "cbar_label" not in kwargs.keys():
+            kwargs["cbar_label"] = "Nodes difference value"
+
+        _, _ = plot_map([[node.pos[0], node.pos[1]] for node in self.nodes_list],
+                        [node.difference for node in self.nodes_list],
+                        self.polygons,
+                        show=show, print_out=print_out,
+                        **kwargs)
+
+        if print_out:
+            logger.info("Node difference map will be saved to:\n" +
+                        kwargs["file_name"])
+
+    def plot_convergence(self, show: bool = False, print_out: bool = True,
+                         **kwargs: Tuple[int]) -> None:
+        """ Plot the the map training progress according to the
+        chosen convergence criterion, when train_algo is batch.
+
+        Args:
+            show (bool): Choose to display the plot.
+            print_out (bool): Choose to save the plot to a file.
+            kwargs (dict): Keyword arguments to format the plot, such as
+                - figsize (tuple(int, int)), the figure size;
+                - title (str), figure title;
+                - xlabel (str), x-axis label;
+                - ylabel (str), y-axis label;
+                - logx (bool), if True set x-axis to logarithmic scale;
+                - logy (bool), if True set y-axis to logarithmic scale;
+                - labelsize (int), font size of label, the title 15% larger, ticks 15% smaller;
+        """
+
+        if len(self.convergence) == 0:
+            logger.warning(
+                "The current parameters yelded no convergence. The plot will not be produced.")
 
-            try:
-                
-                if clus_type == 'MeanShift':
-                    bandwidth = self.interface.cluster_algo.estimate_bandwidth(self.interface.num.asarray(bmu_list), quantile=quant, n_samples=500)
-                    cl =  self.interface.cluster_algo.MeanShift(bandwidth=bandwidth, bin_seeding=True).fit(bmu_list)
-                
-                if clus_type == 'DBSCAN':
-                    cl = self.interface.cluster_algo.DBSCAN(eps=cutoff, min_samples=5).fit(bmu_list)     
-                
-                if clus_type == 'KMeans':
-                    cl = self.interface.cluster_algo.KMeans(n_clusters=num_cl).fit(bmu_list)
-
-                cl_labs = cl.labels_                 
-                    
-                for i in self.interface.num.unique(cl_labs):
-                    cl_list = []
-                    tmp_list = range(len(bmu_list))
-                    for j,k in zip(tmp_list,cl_labs):
-                        if i == k:
-                            cl_list.append(j)
-                    clusters.append(cl_list)     
-            except:
-                print(('Unexpected error: ', sys.exc_info()[0]))
-                raise
         else:
-            sys.exit("Error: unkown clustering algorithm " + clus_type)
 
-        
-        if save_file == True:
-            with open(os.path.join(out_path,clus_type+'_clusters.'+file_type),
-                      'w') as file:
-                if file_type == 'csv':
-                    separator = ','
-                else: 
-                    separator = ' '
-                for line in clusters:
-                    for id in line: file.write(str(id)+separator)
-                    file.write('\n')
-        
-        if print_out==True or show==True:
-            
-            print_name = os.path.join(out_path,clus_type+'_clusters.png')
-            
-            fig, ax = plt.subplots()
-            
-            for i in range(len(clusters)):
-                randCl = "#%06x" % random.randint(0, 0xFFFFFF)
-                xc,yc  = [],[]
-                for c in clusters[i]:
-                    #again, invert y and x to be consistent with the previous maps
-                    xc.append(bmu_list[int(c)][0])
-                    yc.append(self.net_height-bmu_list[int(c)][1])    
-                ax.scatter(xc, yc, color=randCl, label='cluster'+str(i))
-
-            plt.gca().invert_yaxis()
-            plt.legend(bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)           
-            ax.set_title('Clusters')
-            ax.axis('off')
-
-            if print_out == True:
-                plt.savefig(print_name, bbox_inches='tight', dpi=600)
-            if show == True:
-                plt.show()
-            plt.clf()   
-            
-        return clusters
+            if "file_name" not in kwargs.keys():
+                kwargs["file_name"] = os.path.join(
+                    self.output_path, "./som_convergence.png")
+
+            conv_values = np.nan_to_num(self.convergence)
+
+            if "title" not in kwargs.keys():
+                kwargs["title"] = "Convergence"
+            if "xlabel" not in kwargs.keys():
+                kwargs["xlabel"] = "Iteration"
+            if "ylabel" not in kwargs.keys():
+                kwargs["ylabel"] = "Score"
+
+            _, _ = line_plot(conv_values,
+                             show=show, print_out=print_out,
+                             **kwargs)
+
+            if print_out:
+                logger.info("Convergence results will be saved to:\n" +
+                            kwargs["file_name"])
+
+    def plot_projected_points(self, coor: np.ndarray, color_val: Union[np.ndarray, None] = None,
+                              project: bool = True, jitter: bool = True,
+                              show: bool = False, print_out: bool = True,
+                              **kwargs: Tuple[int]) -> None:
+        """Project points onto the trained 2D map and plot the result.
+
+        Args:
+            coor (array): An array containing datapoints to be mapped or
+                pre-mapped if project False.
+            color_val (array): The feature value to use as color map, if None
+                the map will be plotted as white.
+            project (bool): if True, project the points in coor onto the map.
+            jitter (bool): if True, add jitter to points coordinates to help
+                with overlapping points.
+            show (bool): Choose to display the plot.
+            print_out (bool): Choose to save the plot to a file.
+            kwargs (dict): Keyword arguments to format the plot, such as
+                - figsize (tuple(int, int)), the figure size;
+                - title (str), figure title;
+                - cbar_label (str), colorbar label;
+                - labelsize (int), font size of label, the title 15% larger, ticks 15% smaller;
+                - cmap (ListedColormap), a custom cmap.
+        """
+
+        if "file_name" not in kwargs.keys():
+            kwargs["file_name"] = os.path.join(
+                self.output_path, "./som_projected.png")
+
+        bmu_coor = self.project_onto_map(coor) if project else coor
+        bmu_coor = self._get(bmu_coor)
+
+        if jitter:
+            bmu_coor = np.array(bmu_coor).astype(float)
+            bmu_coor += np.random.uniform(low=-.15,
+                                          high=.15, size=(bmu_coor.shape[0], 2))
+
+        _, _ = scatter_on_map([bmu_coor],
+                              [[node.pos[0], node.pos[1]]
+                               for node in self.nodes_list],
+                              self.polygons,
+                              color_val=color_val,
+                              show=show, print_out=print_out,
+                              **kwargs)
+
+        if print_out:
+            logger.info("Projected data scatter plot will be saved to:\n" +
+                        kwargs["file_name"])
+
+    def plot_clusters(self, coor: np.ndarray, clusters: list,
+                      color_val: np.ndarray = None,
+                      project: bool = False, jitter: bool = False,
+                      show: bool = False, print_out: bool = True,
+                      **kwargs: Tuple[int]) -> None:
+        """Project points onto the trained 2D map and plot the result.
+
+        Args:
+            coor (array): An array containing datapoints to be mapped or
+                pre-mapped if project False.
+            clusters (list): Cluster assignment list.
+            color_val (array): The feature value to use as color map, if None
+                the map will be plotted as white.
+            project (bool): if True, project the points in coor onto the map.
+            jitter (bool): if True, add jitter to points coordinates to help
+                with overlapping points.
+            show (bool): Choose to display the plot.
+            print_out (bool): Choose to save the plot to a file.
+            kwargs (dict): Keyword arguments to format the plot, such as
+                - figsize (tuple(int, int)), the figure size;
+                - title (str), figure title;
+                - cbar_label (str), colorbar label;
+                - labelsize (int), font size of label, the title 15% larger, ticks 15% smaller;
+                - cmap (ListedColormap), a custom cmap.
+        """
+
+        if "file_name" not in kwargs.keys():
+            kwargs["file_name"] = os.path.join(
+                self.output_path, "./som_clusters.png")
+
+        bmu_coor = self.project_onto_map(coor) if project else coor
+        bmu_coor = self._get(bmu_coor)
+
+        if jitter:
+            bmu_coor += np.random.uniform(low=-.15,
+                                          high=.15, size=(bmu_coor.shape[0], 2))
+
+        _, _ = scatter_on_map([bmu_coor[clusters == clu] for clu in set(clusters)],
+                              [[node.pos[0], node.pos[1]]
+                               for node in self.nodes_list],
+                              self.polygons,
+                              color_val=color_val,
+                              show=show, print_out=print_out,
+                              **kwargs)
+
+        if print_out:
+            logger.info("Clustering plot will be saved to:\n" +
+                        kwargs["file_name"])
+
 
-        
 class SOMNode:
+    """ Single Kohonen SOM node class. """
 
-    """ Single Kohonen SOM Node class. """
-    
-    def __init__(self, x, y, num_weights, net_height, net_width, PBC, interface,
-                wei_bounds=None, init_vec=None, wei_array=None,):
-    
-        """Initialise the SOM node.
+    __slots__ = ('xp' , 'polygons', 'PBC', 'pos', 'weights', 'difference',
+                 'height', 'width')
+
+    def __init__(self, x: int, y: int, num_weights: int, net_height: int, net_width: int,
+                 PBC: bool, polygons: Polygon, xp: ModuleType = np,
+                 init_vec: Union[np.ndarray, None] = None,
+                 weights_array: Union[np.ndarray, None] = None) -> None:
+        """Initialize the SOM node.
 
         Args:
             x (int): Position along the first network dimension.
             y (int): Position along the second network dimension
             num_weights (int): Length of the weights vector.
             net_height (int): Network height, needed for periodic boundary conditions (PBC)
             net_width (int): Network width, needed for periodic boundary conditions (PBC)
             PBC (bool): Activate/deactivate periodic boundary conditions.
-            interface (Interface obj): CPU/GPU interface.
-            wei_bounds(self.interface.num.array, optional): boundary values for the random initialization
-                of the weights. Must be in the format [min_val, max_val]. 
-                They are overwritten by 'init_vec'.
-            init_vec (self.interface.num.array, optional): Array containing the two custom vectors (e.g. PCA)
+            polygons (Polygon obj): a polygon object with information on the map topology.
+            xp (numpy or cupy): the numeric library to be used.
+            weight_bounds(array): boundary values for the random initialization
+                of the weights. Must be in the format [min_val, max_val].
+                They are overwritten by "init_vec".
+            init_vec (array): Array containing the two custom vectors (e.g. PCA)
                 for the weights initalization.
-            wei_array (self.interface.num.array, optional): Array containing the weights to give
+            weights_array (array): Array containing the weights to give
                 to the node if loaded from a file.
-
-                
         """
-    
-        self.interface = interface
-        
-        self.PBC       = PBC
-        self.pos       = self.interface.num.array(hx.coor_to_hex(x,y))
-        self.weights   = []
-
-        self.net_height = net_height
-        self.net_width  = net_width
-
-        if wei_array is not None:
-            """ Load nodes's weights from file. """
-            
-            self.weights = wei_array
 
-        elif init_vec is not None:
-            """ Select uniformly in the space spanned by the custom vectors. """
+        self.xp = xp
+        self.polygons = polygons
+        self.PBC = PBC
+
+        self.pos = self.xp.array(polygons.to_tiles((x, y)))
+
+        self.weights = []
+        self.difference = None
 
-            self.weights = (x-self.net_width/2)*2.0/self.net_width*init_vec[0] + \
-                           (y-self.net_height/2)*2.0/self.net_height*init_vec[1]
+        self.height = net_height
+        self.width = net_width
+
+        if weights_array is not None:
+            self.weights = weights_array
+
+        elif init_vec is not None:
+            # Sample uniformly in the space spanned by the custom vectors.
+            self.weights = (init_vec[1] - init_vec[0]) * self.xp.array(
+                np.random.rand(len(init_vec[0])).astype(np.float32)) + init_vec[0]
 
-        elif wei_bounds is not None:
-            """ Select randomly in the space spanned by the data. """
-            
-            for i in range(num_weights):
-                self.weights.append(random.random()*(wei_bounds[1][i]-wei_bounds[0][i])+wei_bounds[0][i])
-       
-        else: 
-            """ Else return error. """
-
-            sys.exit(('Error in the network weights initialization, make sure to provide random initalization boundaries,\
-                        custom vectors, or load the weights from file.'))
-   
-        self.weights = self.interface.num.array(self.weights)
-
-    def get_distance(self, vec):
-    
-        """Calculate the distance between the weights vector of the node and a given vector.
-           DEPRECATED: this function will be removed in future versions, use SOMNet.get_bmu instead.
-
-        Args:
-            vec (self.interface.num.array): The vector from which the distance is calculated.
-            
-        Returns: 
-            (float): The distance between the two weight vectors.
-        """
-    
-        sum = 0
-        if len(self.weights) == len(vec):
-            for i in range(len(vec)):
-                sum += (self.weights[i]-vec[i])*(self.weights[i]-vec[i])
-            return sqrt(sum)
         else:
-            sys.exit("Error: dimension of nodes != input data dimension!")
+            logger.error(
+                "Error in the network weights initialization, make sure to provide random initalization boundaries,\n" +
+                "custom vectors, or load the weights from file.")
+            sys.exit(1)
+
+        self.weights = self.xp.array(self.weights)
 
-    def get_node_distance(self, node):
-    
-        """Calculate the distance within the network between the node and another node.
+    def get_node_distance(self, node: 'SOMNode') -> float:
+        """ Calculate the distance within the network between the current node and second node.
 
         Args:
             node (SOMNode): The node from which the distance is calculated.
-            
+
         Returns:
             (float): The distance between the two nodes.
-            
         """
 
-        #to clean up
-
-        if self.PBC == True:
-
-            """ Hexagonal Periodic Boundary Conditions """
-
-            offset = 0 if self.net_height % 2 == 0 else 0.5
-
-            return  min([sqrt((self.pos[0]-node.pos[0])*(self.pos[0]-node.pos[0])\
-                                +(self.pos[1]-node.pos[1])*(self.pos[1]-node.pos[1])),
-                            #right
-                            sqrt((self.pos[0]-node.pos[0]+self.net_width)*(self.pos[0]-node.pos[0]+self.net_width)\
-                                +(self.pos[1]-node.pos[1])*(self.pos[1]-node.pos[1])),
-                            #bottom 
-                            sqrt((self.pos[0]-node.pos[0]+offset)*(self.pos[0]-node.pos[0]+offset)\
-                                +(self.pos[1]-node.pos[1]+self.net_height*2/sqrt(3)*3/4)*(self.pos[1]-node.pos[1]+self.net_height*2/sqrt(3)*3/4)),
-                            #left
-                            sqrt((self.pos[0]-node.pos[0]-self.net_width)*(self.pos[0]-node.pos[0]-self.net_width)\
-                                +(self.pos[1]-node.pos[1])*(self.pos[1]-node.pos[1])),
-                            #top 
-                            sqrt((self.pos[0]-node.pos[0]-offset)*(self.pos[0]-node.pos[0]-offset)\
-                                +(self.pos[1]-node.pos[1]-self.net_height*2/sqrt(3)*3/4)*(self.pos[1]-node.pos[1]-self.net_height*2/sqrt(3)*3/4)),
-                            #bottom right
-                            sqrt((self.pos[0]-node.pos[0]+self.net_width+offset)*(self.pos[0]-node.pos[0]+self.net_width+offset)\
-                                +(self.pos[1]-node.pos[1]+self.net_height*2/sqrt(3)*3/4)*(self.pos[1]-node.pos[1]+self.net_height*2/sqrt(3)*3/4)),
-                            #bottom left
-                            sqrt((self.pos[0]-node.pos[0]-self.net_width+offset)*(self.pos[0]-node.pos[0]-self.net_width+offset)\
-                                +(self.pos[1]-node.pos[1]+self.net_height*2/sqrt(3)*3/4)*(self.pos[1]-node.pos[1]+self.net_height*2/sqrt(3)*3/4)),
-                            #top right
-                            sqrt((self.pos[0]-node.pos[0]+self.net_width-offset)*(self.pos[0]-node.pos[0]+self.net_width-offset)\
-                                +(self.pos[1]-node.pos[1]-self.net_height*2/sqrt(3)*3/4)*(self.pos[1]-node.pos[1]-self.net_height*2/sqrt(3)*3/4)),
-                            #top left
-                            sqrt((self.pos[0]-node.pos[0]-self.net_width-offset)*(self.pos[0]-node.pos[0]-self.net_width-offset)\
-                                +(self.pos[1]-node.pos[1]-self.net_height*2/sqrt(3)*3/4)*(self.pos[1]-node.pos[1]-self.net_height*2/sqrt(3)*3/4))])
-                        
+        if self.PBC:
+            return self.polygons.distance_pbc(self.pos, node.pos,
+                                              (self.width, self.height),
+                                              lambda x, y: self.xp.sqrt(
+                                                  self.xp.sum(self.xp.square(x - y))),
+                                              xp=self.xp)
         else:
-            return sqrt((self.pos[0]-node.pos[0])*(self.pos[0]-node.pos[0])\
-                +(self.pos[1]-node.pos[1])*(self.pos[1]-node.pos[1]))
+            return self.xp.sqrt(self.xp.sum(self.xp.square(self.pos - node.pos)))
 
-
-
-    def update_weights(self, input_vec, sigma, learning_rate, bmu):
-    
-        """Update the node weights.
+    def _update_weights(self, input_vec: np.ndarray, sigma: float, learning_rate: float, bmu: 'SOMNode') -> None:
+        """ Update the node weights.
 
         Args:
-            input_vec (self.interface.num.array): A weights vector whose distance drives the direction of the update.
+            input_vec (array): A weights vector whose distance drives the direction of the update.
             sigma (float): The updated gaussian sigma.
             learning_rate (float): The updated learning rate.
             bmu (SOMNode): The best matching unit.
         """
-    
-        dist  = self.get_node_distance(bmu)
-        gauss = exp(-dist*dist/(2*sigma*sigma))
-
-        i=0
-        
-        for i in range(len(self.weights)):
-            self.weights[i] = self.weights[i] - gauss*learning_rate*(self.weights[i]-input_vec[i])
-        
-        
-if __name__ == "__main__":
 
+        dist = self.get_node_distance(bmu)
+        gauss = self.xp.exp(-dist ** 2 / (2 * sigma ** 2))
+
+        self.weights -= gauss * learning_rate * (self.weights - input_vec)
+
+    def _set_difference(self, diff_value: Union[float, int]) -> None:
+        """ Set the neighbouring nodes weights difference.
+
+        Args:
+            diff_value (float or int), the difference value to set.
+        """
+
+        self.difference = float(diff_value)
+
+
+if __name__ == "__main__":
     pass
```

