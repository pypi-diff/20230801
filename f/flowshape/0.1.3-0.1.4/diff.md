# Comparing `tmp/flowshape-0.1.3.tar.gz` & `tmp/flowshape-0.1.4.tar.gz`

## Comparing `flowshape-0.1.3.tar` & `flowshape-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/__init__.py
--rw-r--r--   0        0        0    13941 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/dirac.py
--rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/fit.py
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/flow.py
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/so3.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/stat.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/util.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/icosphere/ico1.obj
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/icosphere/ico2.obj
--rw-r--r--   0        0        0    28220 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/icosphere/ico3.obj
--rw-r--r--   0        0        0   115625 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/icosphere/ico4.obj
--rw-r--r--   0        0        0   490977 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/icosphere/ico5.obj
--rw-r--r--   0        0        0  2039883 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/icosphere/ico6.obj
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/LICENSE
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/__init__.py
--rw-r--r--   0        0        0 36732979 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/SO3/J_dense_0-150.npy
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/SO3/SO3FFT.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/SO3/__init__.py
--rw-r--r--   0        0        0    18016 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/SO3/irrep_bases.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/SO3/pinchon_hoggan_dense.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 flowshape-0.1.3/src/flowshape/lie_learn/SO3/wigner_d.py
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 flowshape-0.1.3/LICENSE
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 flowshape-0.1.3/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 flowshape-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 flowshape-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/__init__.py
+-rw-r--r--   0        0        0    13941 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/dirac.py
+-rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/fit.py
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/flow.py
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/so3.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/stat.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/util.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/icosphere/ico1.obj
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/icosphere/ico2.obj
+-rw-r--r--   0        0        0    28220 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/icosphere/ico3.obj
+-rw-r--r--   0        0        0   115625 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/icosphere/ico4.obj
+-rw-r--r--   0        0        0   490977 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/icosphere/ico5.obj
+-rw-r--r--   0        0        0  2039883 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/icosphere/ico6.obj
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/LICENSE
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/__init__.py
+-rw-r--r--   0        0        0 36732979 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/SO3/J_dense_0-150.npy
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/SO3/SO3FFT.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/SO3/__init__.py
+-rw-r--r--   0        0        0    18016 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/SO3/irrep_bases.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/SO3/pinchon_hoggan_dense.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 flowshape-0.1.4/src/flowshape/lie_learn/SO3/wigner_d.py
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 flowshape-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 flowshape-0.1.4/README.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 flowshape-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 flowshape-0.1.4/PKG-INFO
```

### Comparing `flowshape-0.1.3/src/flowshape/dirac.py` & `flowshape-0.1.4/src/flowshape/dirac.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/fit.py` & `flowshape-0.1.4/src/flowshape/fit.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/flow.py` & `flowshape-0.1.4/src/flowshape/flow.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/so3.py` & `flowshape-0.1.4/src/flowshape/so3.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/stat.py` & `flowshape-0.1.4/src/flowshape/stat.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/util.py` & `flowshape-0.1.4/src/flowshape/util.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/icosphere/ico1.obj` & `flowshape-0.1.4/src/flowshape/icosphere/ico1.obj`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/icosphere/ico2.obj` & `flowshape-0.1.4/src/flowshape/icosphere/ico2.obj`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/icosphere/ico3.obj` & `flowshape-0.1.4/src/flowshape/icosphere/ico3.obj`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/icosphere/ico4.obj` & `flowshape-0.1.4/src/flowshape/icosphere/ico4.obj`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/icosphere/ico5.obj` & `flowshape-0.1.4/src/flowshape/icosphere/ico5.obj`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/icosphere/ico6.obj` & `flowshape-0.1.4/src/flowshape/icosphere/ico6.obj`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/lie_learn/LICENSE` & `flowshape-0.1.4/src/flowshape/lie_learn/LICENSE`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/lie_learn/README.md` & `flowshape-0.1.4/src/flowshape/lie_learn/README.md`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/lie_learn/SO3/J_dense_0-150.npy` & `flowshape-0.1.4/src/flowshape/lie_learn/SO3/J_dense_0-150.npy`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/lie_learn/SO3/SO3FFT.py` & `flowshape-0.1.4/src/flowshape/lie_learn/SO3/SO3FFT.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/lie_learn/SO3/irrep_bases.py` & `flowshape-0.1.4/src/flowshape/lie_learn/SO3/irrep_bases.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/lie_learn/SO3/pinchon_hoggan_dense.py` & `flowshape-0.1.4/src/flowshape/lie_learn/SO3/pinchon_hoggan_dense.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/src/flowshape/lie_learn/SO3/wigner_d.py` & `flowshape-0.1.4/src/flowshape/lie_learn/SO3/wigner_d.py`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/LICENSE` & `flowshape-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flowshape-0.1.3/README.md` & `flowshape-0.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # FlowShape
 This package provides functionality for the analysis of cell shape using the spherical harmonics decomposition.
-Please refer to the [preprint](https://www.biorxiv.org/content/10.1101/2022.12.08.519700v1) for more information.
+Please refer to our paper ["Cell shape characterization, alignment, and comparison using FlowShape"](https://doi.org/10.1093/bioinformatics/btad383) for more information.
+
 A local branch of [lie_learn](https://github.com/AMLab-Amsterdam/lie_learn) that does not depend on cython is included (spheremesh/lie_learn). 
 
 ## Installation
 Currently the package is on pypi, but still requires conda to install libigl. We are working on an easier installation but in the meantime you can follow these steps:
 
 Recommended: create a seperate conda environment and activate it:
 
@@ -18,22 +19,47 @@
 
 Finally, install FlowShape from pip:
 
 `pip install flowshape`
 
 ## Demo
 
-For the [demo](./demo/), you will need [JupyterLab](https://jupyter.org/install), as well as [Meshplot](https://skoch9.github.io/meshplot/tutorial/) for plotting.
+For the [demos](./demo/), you will need [JupyterLab](https://jupyter.org/install), as well as [Meshplot](https://skoch9.github.io/meshplot/tutorial/) for plotting.
 
 To install both, run:
 
 `conda install -c conda-forge jupyterlab meshplot`
 
 Then, to open JupyterLab, run:
 
 `jupyter-lab`
 
 Download the demo folder from this repository and open the `demo.ipynb` notebook. 
 
+Further, `demo_alignment.ipynb` shows how to align meshes.
+`demo_from_img.ipynb` shows how to use marching cubes to make meshes from image stacks.
+There are some additional dependencies for this notebook.
 
 ## How to use
-See [demo.ipynb](./demo/) for a basic example. The API consists only of functions operating on NumPy ndarrays and there are no classes. Most functions have docstrings in the source. More documentation to follow.
+See the [demos](./demo/) for examples on how to use the package. 
+The API consists only of functions operating on NumPy ndarrays and there are no classes. 
+Most functions have docstrings in the source. 
+
+## Citation
+
+Bibtex:
+```bibtex
+@article{10.1093/bioinformatics/btad383,
+    author = {van Bavel, Casper and Thiels, Wim and Jelier, Rob},
+    title = "{Cell shape characterization, alignment, and comparison using FlowShape}",
+    journal = {Bioinformatics},
+    volume = {39},
+    number = {6},
+    pages = {btad383},
+    year = {2023},
+    month = {06},
+    issn = {1367-4811},
+    doi = {10.1093/bioinformatics/btad383},
+    url = {https://doi.org/10.1093/bioinformatics/btad383},
+    eprint = {https://academic.oup.com/bioinformatics/article-pdf/39/6/btad383/50738096/btad383.pdf},
+}
+```
```

### Comparing `flowshape-0.1.3/pyproject.toml` & `flowshape-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flowshape"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Casper van Bavel", email="casper.vanbavel@kuleuven.be" },
 ]
 description = "Cell shape analysis using the spherical harmonics decomposition"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Preprint" = "https://www.biorxiv.org/content/10.1101/2022.12.08.519700v1"
+"Paper" = "https://doi.org/10.1093/bioinformatics/btad383"
 "Homepage" = "https://bitbucket.org/pgmsembryogenesis/flowshape/"
 "Bug Tracker" = "https://bitbucket.org/pgmsembryogenesis/flowshape/issues"
```

### Comparing `flowshape-0.1.3/PKG-INFO` & `flowshape-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: flowshape
-Version: 0.1.3
+Version: 0.1.4
 Summary: Cell shape analysis using the spherical harmonics decomposition
-Project-URL: Preprint, https://www.biorxiv.org/content/10.1101/2022.12.08.519700v1
+Project-URL: Paper, https://doi.org/10.1093/bioinformatics/btad383
 Project-URL: Homepage, https://bitbucket.org/pgmsembryogenesis/flowshape/
 Project-URL: Bug Tracker, https://bitbucket.org/pgmsembryogenesis/flowshape/issues
 Author-email: Casper van Bavel <casper.vanbavel@kuleuven.be>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # FlowShape
 This package provides functionality for the analysis of cell shape using the spherical harmonics decomposition.
-Please refer to the [preprint](https://www.biorxiv.org/content/10.1101/2022.12.08.519700v1) for more information.
+Please refer to our paper ["Cell shape characterization, alignment, and comparison using FlowShape"](https://doi.org/10.1093/bioinformatics/btad383) for more information.
+
 A local branch of [lie_learn](https://github.com/AMLab-Amsterdam/lie_learn) that does not depend on cython is included (spheremesh/lie_learn). 
 
 ## Installation
 Currently the package is on pypi, but still requires conda to install libigl. We are working on an easier installation but in the meantime you can follow these steps:
 
 Recommended: create a seperate conda environment and activate it:
 
@@ -33,22 +34,47 @@
 
 Finally, install FlowShape from pip:
 
 `pip install flowshape`
 
 ## Demo
 
-For the [demo](./demo/), you will need [JupyterLab](https://jupyter.org/install), as well as [Meshplot](https://skoch9.github.io/meshplot/tutorial/) for plotting.
+For the [demos](./demo/), you will need [JupyterLab](https://jupyter.org/install), as well as [Meshplot](https://skoch9.github.io/meshplot/tutorial/) for plotting.
 
 To install both, run:
 
 `conda install -c conda-forge jupyterlab meshplot`
 
 Then, to open JupyterLab, run:
 
 `jupyter-lab`
 
 Download the demo folder from this repository and open the `demo.ipynb` notebook. 
 
+Further, `demo_alignment.ipynb` shows how to align meshes.
+`demo_from_img.ipynb` shows how to use marching cubes to make meshes from image stacks.
+There are some additional dependencies for this notebook.
 
 ## How to use
-See [demo.ipynb](./demo/) for a basic example. The API consists only of functions operating on NumPy ndarrays and there are no classes. Most functions have docstrings in the source. More documentation to follow.
+See the [demos](./demo/) for examples on how to use the package. 
+The API consists only of functions operating on NumPy ndarrays and there are no classes. 
+Most functions have docstrings in the source. 
+
+## Citation
+
+Bibtex:
+```bibtex
+@article{10.1093/bioinformatics/btad383,
+    author = {van Bavel, Casper and Thiels, Wim and Jelier, Rob},
+    title = "{Cell shape characterization, alignment, and comparison using FlowShape}",
+    journal = {Bioinformatics},
+    volume = {39},
+    number = {6},
+    pages = {btad383},
+    year = {2023},
+    month = {06},
+    issn = {1367-4811},
+    doi = {10.1093/bioinformatics/btad383},
+    url = {https://doi.org/10.1093/bioinformatics/btad383},
+    eprint = {https://academic.oup.com/bioinformatics/article-pdf/39/6/btad383/50738096/btad383.pdf},
+}
+```
```

