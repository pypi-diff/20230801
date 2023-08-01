# Comparing `tmp/pydeseq2-0.3.5.tar.gz` & `tmp/pydeseq2-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bmuzellec/Documents/Projects/FL_genomics/PyDESeq2/dist/.tmp-p8wr8_61/pydeseq2-0.3.5.tar", last modified: Wed Jun 14 13:13:48 2023, max compression
+gzip compressed data, was "/Users/bmuzellec/Documents/Projects/FL_genomics/PyDESeq2/dist/.tmp-iij11kvm/pydeseq2-0.3.6.tar", last modified: Tue Aug  1 09:20:19 2023, max compression
```

## Comparing `pydeseq2-0.3.5.tar` & `pydeseq2-0.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1062 2022-12-03 17:11:22.000000 pydeseq2-0.3.5/LICENSE
--rw-r--r--   0 bmuzellec   (501) staff       (20)     6217 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/PKG-INFO
--rw-r--r--   0 bmuzellec   (501) staff       (20)     5884 2023-06-14 12:31:48.000000 pydeseq2-0.3.5/README.md
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/pydeseq2/
--rw-r--r--   0 bmuzellec   (501) staff       (20)       53 2022-12-28 09:54:14.000000 pydeseq2-0.3.5/pydeseq2/__init__.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)       22 2023-06-14 13:12:11.000000 pydeseq2-0.3.5/pydeseq2/__version__.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    40038 2023-06-14 13:07:34.000000 pydeseq2-0.3.5/pydeseq2/dds.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    23930 2023-06-01 08:36:10.000000 pydeseq2-0.3.5/pydeseq2/ds.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     8480 2023-03-24 14:45:04.000000 pydeseq2-0.3.5/pydeseq2/grid_search.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1587 2023-06-01 08:36:08.000000 pydeseq2-0.3.5/pydeseq2/preprocessing.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    39607 2023-06-12 08:27:45.000000 pydeseq2-0.3.5/pydeseq2/utils.py
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/pydeseq2.egg-info/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     6217 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/pydeseq2.egg-info/PKG-INFO
--rw-r--r--   0 bmuzellec   (501) staff       (20)      436 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/pydeseq2.egg-info/SOURCES.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)        1 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/pydeseq2.egg-info/dependency_links.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)      190 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/pydeseq2.egg-info/requires.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)        9 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/pydeseq2.egg-info/top_level.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)      408 2023-04-05 09:20:58.000000 pydeseq2-0.3.5/pyproject.toml
--rw-r--r--   0 bmuzellec   (501) staff       (20)       38 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/setup.cfg
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1362 2023-05-02 08:07:48.000000 pydeseq2-0.3.5/setup.py
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-06-14 13:13:48.000000 pydeseq2-0.3.5/tests/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     5654 2023-02-16 10:34:42.000000 pydeseq2-0.3.5/tests/test_docstring.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    11990 2023-06-12 08:27:50.000000 pydeseq2-0.3.5/tests/test_edge_cases.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    15867 2023-06-01 08:36:08.000000 pydeseq2-0.3.5/tests/test_pydeseq2.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1951 2023-02-21 15:32:02.000000 pydeseq2-0.3.5/tests/test_utils.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1062 2022-12-03 17:11:22.000000 pydeseq2-0.3.6/LICENSE
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6563 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/PKG-INFO
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6230 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/README.md
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       53 2022-12-28 09:54:14.000000 pydeseq2-0.3.6/pydeseq2/__init__.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       22 2023-08-01 09:16:03.000000 pydeseq2-0.3.6/pydeseq2/__version__.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    41325 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/pydeseq2/dds.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    25791 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/pydeseq2/ds.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     8480 2023-03-24 14:45:04.000000 pydeseq2-0.3.6/pydeseq2/grid_search.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1587 2023-06-01 08:36:08.000000 pydeseq2-0.3.6/pydeseq2/preprocessing.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    41248 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/pydeseq2/utils.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6563 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/PKG-INFO
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      436 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/SOURCES.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)        1 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/dependency_links.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      190 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/requires.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)        9 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/top_level.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      408 2023-04-05 09:20:58.000000 pydeseq2-0.3.6/pyproject.toml
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       38 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/setup.cfg
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1362 2023-05-02 08:07:48.000000 pydeseq2-0.3.6/setup.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/tests/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     5654 2023-02-16 10:34:42.000000 pydeseq2-0.3.6/tests/test_docstring.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    12647 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/tests/test_edge_cases.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    15705 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/tests/test_pydeseq2.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1951 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/tests/test_utils.py
```

### Comparing `pydeseq2-0.3.5/LICENSE` & `pydeseq2-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.5/PKG-INFO` & `pydeseq2-0.3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 Metadata-Version: 2.1
 Name: pydeseq2
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python implementation of DESeq2.
 Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
 Author-email: boris.muzellec@owkin.com
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="docs/source/_static/pydeseq2_logo_green.png" width="600">
 
+#
+[![pypi version](https://img.shields.io/pypi/v/pydeseq2)](https://pypi.org/project/pydeseq2)
+[![pypiDownloads](https://pepy.tech/badge/pydeseq2)](https://pepy.tech/project/pydeseq2)
+[![condaDownloads](https://img.shields.io/conda/dn/bioconda/pydeseq2?logo=Anaconda)](https://anaconda.org/bioconda/pydeseq2)
+[![license](https://img.shields.io/pypi/l/pydeseq2)](LICENSE)
+
+PyDESeq2 is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
+method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
+It aims to facilitate DEA experiments for python users.
+
+As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
+scratch, you may experience some differences in terms of retrieved values or available features.
+
+Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
+and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
+In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Table of Contents
 - [PyDESeq2](#pydeseq2)
   - [Table of Contents](#table-of-contents)
-  - [Overview](#overview)
   - [Installation](#installation)
     - [Requirements](#requirements)
   - [Getting started](#getting-started)
     - [Documentation](#documentation)
     - [Data](#data)
   - [Contributing](#contributing)
     - [1 - Download the repository](#1---download-the-repository)
     - [2 - Create a conda environment](#2---create-a-conda-environment)
   - [Development roadmap](#development-roadmap)
   - [Citing this work](#citing-this-work)
   - [References](#references)
   - [License](#license)
 
-## Overview
-
-This package is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
-method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
-It aims to facilitate DEA experiments for python users.
-
-As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
-scratch, you may experience some differences in terms of retrieved values or available features.
-
-Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
-and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
-In case there is a feature you would particularly like to be implemented, feel free to open an issue.
-
 ## Installation
 
 ### PyPI
 
 `PyDESeq2` can be installed from PyPI using `pip`:
 
 `pip install pydeseq2`
@@ -134,16 +136,17 @@
 Here are some of the features and improvements we plan to implement in the future:
 
 - [x] Integration to the [scverse](https://scverse.org/) ecosystem:
   * [x] Refactoring to use the [AnnData](https://anndata.readthedocs.io/) data structure
   * [x] Submitting a PR to be listed as an [scverse ecosystem](https://github.com/scverse/ecosystem-packages/) package
 - [x] Variance-stabilizing transformation
 - [ ] Improving multi-factor analysis:
-  * [x] Allowing n-level factors (only bi-level for now)
+  * [x] Allowing n-level factors
   * [ ] Implementing interaction terms
+  * [ ] Support for continuous covariates
 
 ## Citing this work
 
 ```
 @article{muzellec2022pydeseq2,
   title={PyDESeq2: a python package for bulk RNA-seq differential expression analysis},
   author={Muzellec, Boris and Telenczuk, Maria and Cabeli, Vincent and Andreux, Mathieu},
```

### Comparing `pydeseq2-0.3.5/README.md` & `pydeseq2-0.3.6/pydeseq2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,54 @@
+Metadata-Version: 2.1
+Name: pydeseq2
+Version: 0.3.6
+Summary: A python implementation of DESeq2.
+Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
+Author-email: boris.muzellec@owkin.com
+License: MIT
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 <img src="docs/source/_static/pydeseq2_logo_green.png" width="600">
 
+#
+[![pypi version](https://img.shields.io/pypi/v/pydeseq2)](https://pypi.org/project/pydeseq2)
+[![pypiDownloads](https://pepy.tech/badge/pydeseq2)](https://pepy.tech/project/pydeseq2)
+[![condaDownloads](https://img.shields.io/conda/dn/bioconda/pydeseq2?logo=Anaconda)](https://anaconda.org/bioconda/pydeseq2)
+[![license](https://img.shields.io/pypi/l/pydeseq2)](LICENSE)
+
+PyDESeq2 is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
+method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
+It aims to facilitate DEA experiments for python users.
+
+As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
+scratch, you may experience some differences in terms of retrieved values or available features.
+
+Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
+and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
+In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Table of Contents
 - [PyDESeq2](#pydeseq2)
   - [Table of Contents](#table-of-contents)
-  - [Overview](#overview)
   - [Installation](#installation)
     - [Requirements](#requirements)
   - [Getting started](#getting-started)
     - [Documentation](#documentation)
     - [Data](#data)
   - [Contributing](#contributing)
     - [1 - Download the repository](#1---download-the-repository)
     - [2 - Create a conda environment](#2---create-a-conda-environment)
   - [Development roadmap](#development-roadmap)
   - [Citing this work](#citing-this-work)
   - [References](#references)
   - [License](#license)
 
-## Overview
-
-This package is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
-method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
-It aims to facilitate DEA experiments for python users.
-
-As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
-scratch, you may experience some differences in terms of retrieved values or available features.
-
-Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
-and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
-In case there is a feature you would particularly like to be implemented, feel free to open an issue.
-
 ## Installation
 
 ### PyPI
 
 `PyDESeq2` can be installed from PyPI using `pip`:
 
 `pip install pydeseq2`
@@ -122,16 +136,17 @@
 Here are some of the features and improvements we plan to implement in the future:
 
 - [x] Integration to the [scverse](https://scverse.org/) ecosystem:
   * [x] Refactoring to use the [AnnData](https://anndata.readthedocs.io/) data structure
   * [x] Submitting a PR to be listed as an [scverse ecosystem](https://github.com/scverse/ecosystem-packages/) package
 - [x] Variance-stabilizing transformation
 - [ ] Improving multi-factor analysis:
-  * [x] Allowing n-level factors (only bi-level for now)
+  * [x] Allowing n-level factors
   * [ ] Implementing interaction terms
+  * [ ] Support for continuous covariates
 
 ## Citing this work
 
 ```
 @article{muzellec2022pydeseq2,
   title={PyDESeq2: a python package for bulk RNA-seq differential expression analysis},
   author={Muzellec, Boris and Telenczuk, Maria and Cabeli, Vincent and Andreux, Mathieu},
```

### Comparing `pydeseq2-0.3.5/pydeseq2/dds.py` & `pydeseq2-0.3.6/pydeseq2/dds.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import time
 import warnings
 from typing import List
 from typing import Literal
 from typing import Optional
 from typing import Union
 from typing import cast
@@ -36,16 +37,14 @@
 from pydeseq2.utils import trimmed_mean
 
 # Ignore DomainWarning raised by statsmodels when fitting a Gamma GLM with identity link.
 warnings.simplefilter("ignore", DomainWarning)
 # Ignore AnnData's FutureWarning about implicit data conversion.
 warnings.simplefilter("ignore", FutureWarning)
 
-# TODO: implement a quiet (non-verbose) mode ?
-
 
 class DeseqDataSet(ad.AnnData):
     r"""A class to implement dispersion and log fold-change (LFC) estimation.
 
     The DeseqDataSet extends the `AnnData class
     <https://anndata.readthedocs.io/en/latest/generated/anndata.AnnData.html#anndata.AnnData>`_.
     As such, it implements the same methods and attributes, in addition to those that are
@@ -53,42 +52,42 @@
     Dispersions and LFCs are estimated following the DESeq2 pipeline
     :cite:p:`DeseqDataSet-love2014moderated`.
 
     Parameters
     ----------
     adata : anndata.AnnData
         AnnData from which to initialize the DeseqDataSet. Must have counts ('X') and
-        clinical metadata ('obs') fields. If ``None``, both ``counts`` and ``clinical``
+        sample metadata ('obs') fields. If ``None``, both ``counts`` and ``metadata``
         arguments must be provided.
 
     counts : pandas.DataFrame
         Raw counts. One column per gene, rows are indexed by sample barcodes.
 
-    clinical : pandas.DataFrame
-        DataFrame containing clinical information.
+    metadata : pandas.DataFrame
+        DataFrame containing sample metadata.
         Must be indexed by sample barcodes.
 
     design_factors : str or list
-        Name of the columns of clinical to be used as design variables.
-        Only bi-level factors are supported. (default: ``'condition'``).
+        Name of the columns of metadata to be used as design variables.
+        Only categorial factors are supported. (default: ``'condition'``).
 
     ref_level : list or None
         An optional list of two strings of the form ``["factor", "test_level"]``
         specifying the factor of interest and the reference (control) level against which
         we're testing, e.g. ``["condition", "A"]``. (default: ``None``).
 
     min_mu : float
         Threshold for mean estimates. (default: ``0.5``).
 
     min_disp : float
         Lower threshold for dispersion parameters. (default: ``1e-8``).
 
     max_disp : float
         Upper threshold for dispersion parameters.
-        NB: The threshold that is actually enforced is max(max_disp, len(counts)).
+        Note: The threshold that is actually enforced is max(max_disp, len(counts)).
         (default: ``10``).
 
     refit_cooks : bool
         Whether to refit cooks outliers. (default: ``True``).
 
     min_replicates : int
         Minimum number of replicates a condition should have
@@ -106,14 +105,17 @@
     batch_size : int
         Number of tasks to allocate to each joblib parallel worker. (default: ``128``).
 
     joblib_verbosity : int
         The verbosity level for joblib tasks. The higher the value, the more updates
         are reported. (default: ``0``).
 
+    quiet : bool
+        Suppress deseq2 status updates during fit.
+
     Attributes
     ----------
     X
         A ‘number of samples’ x ‘number of genes’ count data matrix.
 
     obs
         Key-indexed one-dimensional observations annotation of length 'number of
@@ -148,74 +150,77 @@
     counts_to_refit : anndata.AnnData
         Read counts after replacement, containing only genes
         for which dispersions and LFCs must be fitted again.
 
     new_all_zeroes_genes : pandas.Index
         Genes which have only zero counts after outlier replacement.
 
+    quiet : bool
+        Suppress deseq2 status updates during fit.
+
     References
     ----------
     .. bibliography::
         :keyprefix: DeseqDataSet-
     """
 
     def __init__(
         self,
         *,
         adata: Optional[ad.AnnData] = None,
         counts: Optional[pd.DataFrame] = None,
-        clinical: Optional[pd.DataFrame] = None,
+        metadata: Optional[pd.DataFrame] = None,
         design_factors: Union[str, List[str]] = "condition",
         ref_level: Optional[List[str]] = None,
         min_mu: float = 0.5,
         min_disp: float = 1e-8,
         max_disp: float = 10.0,
         refit_cooks: bool = True,
         min_replicates: int = 7,
         beta_tol: float = 1e-8,
         n_cpus: Optional[int] = None,
         batch_size: int = 128,
         joblib_verbosity: int = 0,
+        quiet: bool = False,
     ) -> None:
-
         # Initialize the AnnData part
         if adata is not None:
             if counts is not None:
                 warnings.warn(
                     "adata was provided; ignoring counts.", UserWarning, stacklevel=2
                 )
-            if clinical is not None:
+            if metadata is not None:
                 warnings.warn(
-                    "adata was provided; ignoring clinical.", UserWarning, stacklevel=2
+                    "adata was provided; ignoring metadata.", UserWarning, stacklevel=2
                 )
             # Test counts before going further
             test_valid_counts(adata.X)
             # Copy fields from original AnnData
             self.__dict__.update(adata.__dict__)
-        elif counts is not None and clinical is not None:
+        elif counts is not None and metadata is not None:
             # Test counts before going further
             test_valid_counts(counts)
-            super().__init__(X=counts.astype(int), obs=clinical)
+            super().__init__(X=counts.astype(int), obs=metadata)
         else:
             raise ValueError(
-                "Either adata or both counts and clinical arguments must be provided."
+                "Either adata or both counts and metadata arguments must be provided."
             )
 
         # Convert design_factors to list if a single string was provided.
         self.design_factors = (
             [design_factors] if isinstance(design_factors, str) else design_factors
         )
         if self.obs[self.design_factors].isna().any().any():
             raise ValueError("NaNs are not allowed in the design factors.")
         self.obs[self.design_factors] = self.obs[self.design_factors].astype(str)
 
         # Build the design matrix
         # Stored in the obsm attribute of the dataset
         self.obsm["design_matrix"] = build_design_matrix(
-            clinical_df=self.obs,
+            metadata=self.obs,
             design_factors=self.design_factors,
             ref_level=ref_level,
             expanded=False,
             intercept=True,
         )
 
         # Check that the design matrix has full rank
@@ -227,14 +232,15 @@
         self.refit_cooks = refit_cooks
         self.ref_level = ref_level
         self.min_replicates = min_replicates
         self.beta_tol = beta_tol
         self.n_processes = get_num_processes(n_cpus)
         self.batch_size = batch_size
         self.joblib_verbosity = joblib_verbosity
+        self.quiet = quiet
 
     def vst(
         self,
         use_design: bool = False,
         fit_type: Literal["parametric", "mean"] = "parametric",
     ) -> None:
         """
@@ -337,15 +343,16 @@
         switches to the ``iterative`` method.
 
         Parameters
         ----------
         fit_type : str
             The normalization method to use (default: ``"ratio"``).
         """
-        print("Fitting size factors...")
+        if not self.quiet:
+            print("Fitting size factors...", file=sys.stderr)
         start = time.time()
         if fit_type == "iterative":
             self._fit_iterate_size_factors()
         # Test whether it is possible to use median-of-ratios.
         elif (self.X == 0).any(0).all():
             # There is at least a zero for each gene
             warnings.warn(
@@ -354,15 +361,17 @@
                 RuntimeWarning,
                 stacklevel=2,
             )
             self._fit_iterate_size_factors()
         else:
             self.layers["normed_counts"], self.obsm["size_factors"] = deseq2_norm(self.X)
         end = time.time()
-        print(f"... done in {end - start:.2f} seconds.\n")
+
+        if not self.quiet:
+            print(f"... done in {end - start:.2f} seconds.\n", file=sys.stderr)
 
     def fit_genewise_dispersions(self) -> None:
         """Fit gene-wise dispersion estimates.
 
         Fits a negative binomial per gene, independently.
         """
         # Check that size factors are available. If not, compute them.
@@ -427,15 +436,16 @@
 
                 _, mu_hat_, _, _ = zip(*res)
                 mu_hat_ = np.array(mu_hat_)
 
         self.layers["_mu_hat"] = np.full((self.n_obs, self.n_vars), np.NaN)
         self.layers["_mu_hat"][:, self.varm["non_zero"]] = mu_hat_.T
 
-        print("Fitting dispersions...")
+        if not self.quiet:
+            print("Fitting dispersions...", file=sys.stderr)
         start = time.time()
         with parallel_backend("loky", inner_max_num_threads=1):
             res = Parallel(
                 n_jobs=self.n_processes,
                 verbose=self.joblib_verbosity,
                 batch_size=self.batch_size,
             )(
@@ -447,15 +457,17 @@
                     min_disp=self.min_disp,
                     max_disp=self.max_disp,
                 )
                 # for i in range(num_genes)
                 for i in self.non_zero_idx
             )
         end = time.time()
-        print(f"... done in {end - start:.2f} seconds.\n")
+
+        if not self.quiet:
+            print(f"... done in {end - start:.2f} seconds.\n", file=sys.stderr)
 
         dispersions_, l_bfgs_b_converged_ = zip(*res)
 
         self.varm["genewise_dispersions"] = np.full(self.n_vars, np.NaN)
         self.varm["genewise_dispersions"][self.varm["non_zero"]] = np.clip(
             dispersions_, self.min_disp, self.max_disp
         )
@@ -469,15 +481,16 @@
         :math:`f(\mu) = \alpha_1/\mu + a_0`.
         """
 
         # Check that genewise dispersions are available. If not, compute them.
         if "genewise_dispersions" not in self.varm:
             self.fit_genewise_dispersions()
 
-        print("Fitting dispersion trend curve...")
+        if not self.quiet:
+            print("Fitting dispersion trend curve...", file=sys.stderr)
         start = time.time()
         self.varm["_normed_means"] = self.layers["normed_counts"].mean(0)
 
         # Exclude all-zero counts
         targets = pd.Series(
             self[:, self.non_zero_genes].varm["genewise_dispersions"].copy(),
             index=self.non_zero_genes,
@@ -524,52 +537,68 @@
             )
             covariates.drop(
                 covariates[(pred_ratios < 1e-4) | (pred_ratios >= 15)].index,
                 inplace=True,
             )
 
         end = time.time()
-        print(f"... done in {end - start:.2f} seconds.\n")
+
+        if not self.quiet:
+            print(f"... done in {end - start:.2f} seconds.\n", file=sys.stderr)
 
         self.uns["trend_coeffs"] = pd.Series(coeffs, index=["a0", "a1"])
 
         self.varm["fitted_dispersions"] = np.full(self.n_vars, np.NaN)
         self.varm["fitted_dispersions"][self.varm["non_zero"]] = dispersion_trend(
             self.varm["_normed_means"][self.varm["non_zero"]],
             self.uns["trend_coeffs"],
         )
 
     def fit_dispersion_prior(self) -> None:
         """Fit dispersion variance priors and standard deviation of log-residuals.
 
         The computation is based on genes whose dispersions are above 100 * min_disp.
+
+        Note: when the design matrix has fewer than 3 degrees of freedom, the
+        estimate of log dispersions is likely to be imprecise.
         """
 
         # Check that the dispersion trend curve was fitted. If not, fit it.
         if "fitted_dispersions" not in self.varm:
             self.fit_dispersion_trend()
 
         # Exclude genes with all zeroes
         num_samples = self.n_obs
         num_vars = self.obsm["design_matrix"].shape[-1]
 
+        # Check the degrees of freedom
+        if (num_samples - num_vars) <= 3:
+            warnings.warn(
+                "As the residual degrees of freedom is less than 3, the distribution "
+                "of log dispersions is especially asymmetric and likely to be poorly "
+                "estimated by the MAD.",
+                UserWarning,
+                stacklevel=2,
+            )
+
         # Fit dispersions to the curve, and compute log residuals
         disp_residuals = np.log(
             self[:, self.non_zero_genes].varm["genewise_dispersions"]
         ) - np.log(self[:, self.non_zero_genes].varm["fitted_dispersions"])
 
         # Compute squared log-residuals and prior variance based on genes whose
         # dispersions are above 100 * min_disp. This is to reproduce DESeq2's behaviour.
         above_min_disp = self[:, self.non_zero_genes].varm["genewise_dispersions"] >= (
             100 * self.min_disp
         )
 
         self.uns["_squared_logres"] = (
             mean_absolute_deviation(disp_residuals[above_min_disp]) ** 2
         )
+
         self.uns["prior_disp_var"] = np.maximum(
             self.uns["_squared_logres"] - polygamma(1, (num_samples - num_vars) / 2),
             0.25,
         )
 
     def fit_MAP_dispersions(self) -> None:
         """Fit Maximum a Posteriori dispersion estimates.
@@ -580,15 +609,16 @@
         # Check that the dispersion prior variance is available. If not, compute it.
         if "prior_disp_var" not in self.uns:
             self.fit_dispersion_prior()
 
         # Convert design matrix to numpy for speed
         design_matrix = self.obsm["design_matrix"].values
 
-        print("Fitting MAP dispersions...")
+        if not self.quiet:
+            print("Fitting MAP dispersions...", file=sys.stderr)
         start = time.time()
         with parallel_backend("loky", inner_max_num_threads=1):
             res = Parallel(
                 n_jobs=self.n_processes,
                 verbose=self.joblib_verbosity,
                 batch_size=self.batch_size,
             )(
@@ -602,15 +632,17 @@
                     prior_disp_var=self.uns["prior_disp_var"].item(),
                     cr_reg=True,
                     prior_reg=True,
                 )
                 for i in self.non_zero_idx
             )
         end = time.time()
-        print(f"... done in {end-start:.2f} seconds.\n")
+
+        if not self.quiet:
+            print(f"... done in {end-start:.2f} seconds.\n", file=sys.stderr)
 
         dispersions_, l_bfgs_b_converged_ = zip(*res)
 
         self.varm["MAP_dispersions"] = np.full(self.n_vars, np.NaN)
         self.varm["MAP_dispersions"][self.varm["non_zero"]] = np.clip(
             dispersions_, self.min_disp, self.max_disp
         )
@@ -637,15 +669,16 @@
         # Check that MAP dispersions are available. If not, compute them.
         if "dispersions" not in self.varm:
             self.fit_MAP_dispersions()
 
         # Convert design matrix to numpy for speed
         design_matrix = self.obsm["design_matrix"].values
 
-        print("Fitting LFCs...")
+        if not self.quiet:
+            print("Fitting LFCs...", file=sys.stderr)
         start = time.time()
         with parallel_backend("loky", inner_max_num_threads=1):
             res = Parallel(
                 n_jobs=self.n_processes,
                 verbose=self.joblib_verbosity,
                 batch_size=self.batch_size,
             )(
@@ -656,15 +689,17 @@
                     disp=self.varm["dispersions"][i],
                     min_mu=self.min_mu,
                     beta_tol=self.beta_tol,
                 )
                 for i in self.non_zero_idx
             )
         end = time.time()
-        print(f"... done in {end-start:.2f} seconds.\n")
+
+        if not self.quiet:
+            print(f"... done in {end-start:.2f} seconds.\n", file=sys.stderr)
 
         MLE_lfcs_, mu_, hat_diagonals_, converged_ = zip(*res)
         mu_ = np.array(mu_).T
         hat_diagonals_ = np.array(hat_diagonals_).T
 
         self.varm["LFC"] = pd.DataFrame(
             np.NaN,
@@ -732,15 +767,18 @@
         """Refit Cook outliers.
 
         Replace values that are filtered out based on the Cooks distance with imputed
         values, and then re-run the whole DESeq2 pipeline on replaced values.
         """
         # Replace outlier counts
         self._replace_outliers()
-        print(f"Refitting {sum(self.varm['replaced']) } outliers.\n")
+        if not self.quiet:
+            print(
+                f"Refitting {sum(self.varm['replaced']) } outliers.\n", file=sys.stderr
+            )
 
         if sum(self.varm["replaced"]) > 0:
             # Refit dispersions and LFCs for genes that had outliers replaced
             self._refit_without_outliers()
 
     def _fit_MoM_dispersions(self) -> None:
         """ "Rough method of moments" initial dispersions fit.
@@ -892,15 +930,15 @@
 
         sub_dds = DeseqDataSet(
             counts=pd.DataFrame(
                 self.counts_to_refit.X,
                 index=self.counts_to_refit.obs_names,
                 columns=self.counts_to_refit.var_names,
             ),
-            clinical=self.obs,
+            metadata=self.obs,
             design_factors=self.design_factors,
             ref_level=self.ref_level,
             min_mu=self.min_mu,
             min_disp=self.min_disp,
             max_disp=self.max_disp,
             refit_cooks=self.refit_cooks,
             min_replicates=self.min_replicates,
@@ -1016,23 +1054,23 @@
 
             # Fit size factors using MLE
             res = minimize(objective, np.log(old_sf), method="Powell")
 
             self.obsm["size_factors"] = np.exp(res.x - np.mean(res.x))
 
             if not res.success:
-                print("A size factor fitting iteration failed.")
+                print("A size factor fitting iteration failed.", file=sys.stderr)
                 break
 
             if (i > 1) and np.sum(
                 (np.log(old_sf) - np.log(self.obsm["size_factors"])) ** 2
             ) < 1e-4:
                 break
             elif i == niter - 1:
-                print("Iterative size factor fitting did not converge.")
+                print("Iterative size factor fitting did not converge.", file=sys.stderr)
 
         # Restore the design matrix and free buffer
         self.obsm["design_matrix"] = self.obsm["design_matrix_buffer"].copy()
         del self.obsm["design_matrix_buffer"]
 
         # Store normalized counts
         self.layers["normed_counts"] = self.X / self.obsm["size_factors"][:, None]
```

### Comparing `pydeseq2-0.3.5/pydeseq2/ds.py` & `pydeseq2-0.3.6/pydeseq2/ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import time
 from typing import List
 from typing import Optional
 
 # import anndata as ad
 import numpy as np
 import pandas as pd
@@ -12,14 +13,15 @@
 from joblib import parallel_backend  # type: ignore
 from scipy.optimize import root_scalar  # type: ignore
 from scipy.stats import f  # type: ignore
 from statsmodels.stats.multitest import multipletests  # type: ignore
 
 from pydeseq2.dds import DeseqDataSet
 from pydeseq2.utils import get_num_processes
+from pydeseq2.utils import make_MA_plot
 from pydeseq2.utils import nbinomGLM
 from pydeseq2.utils import wald_test
 
 
 class DeseqStats:
     """PyDESeq2 statistical tests for differential expression.
 
@@ -32,15 +34,15 @@
     ----------
     dds : DeseqDataSet
         DeseqDataSet for which dispersion and LFCs were already estimated.
 
     contrast : list or None
         A list of three strings, in the following format:
         ``['variable_of_interest', 'tested_level', 'ref_level']``.
-        Names must correspond to the clinical data passed to the DeseqDataSet.
+        Names must correspond to the metadata data passed to the DeseqDataSet.
         E.g., ``['condition', 'B', 'A']`` will measure the LFC of 'condition B' compared
         to 'condition A'. If None, the last variable from the design matrix is chosen
         as the variable of interest, and the reference level is picked alphabetically.
         (default: ``None``).
 
     alpha : float
         P-value and adjusted p-value significance threshold (usually 0.05).
@@ -63,14 +65,17 @@
     batch_size : int
         Number of tasks to allocate to each joblib parallel worker. (default: ``128``).
 
     joblib_verbosity : int
         The verbosity level for joblib tasks. The higher the value, the more updates
         are reported. (default: ``0``).
 
+    quiet : bool
+        Suppress deseq2 status updates during fit.
+
     Attributes
     ----------
     base_mean : pandas.Series
         Genewise means of normalized counts.
 
     contrast_vector : ndarray
         Vector encoding the contrast (variable being tested).
@@ -104,14 +109,17 @@
 
     shrunk_LFCs : bool
         Whether LFCs are shrunk.
 
     n_processes : int
         Number of threads to use for multiprocessing.
 
+    quiet : bool
+        Suppress deseq2 status updates during fit.
+
     References
     ----------
     .. bibliography::
         :keyprefix: DeseqStats-
     """
 
     def __init__(
@@ -121,14 +129,15 @@
         alpha: float = 0.05,
         cooks_filter: bool = True,
         independent_filter: bool = True,
         n_cpus: Optional[int] = None,
         prior_LFC_var: Optional[np.ndarray] = None,
         batch_size: int = 128,
         joblib_verbosity: int = 0,
+        quiet: bool = False,
     ) -> None:
         assert (
             "LFC" in dds.varm
         ), "Please provide a fitted DeseqDataSet by first running the `deseq2` method."
 
         self.dds = dds
 
@@ -150,14 +159,15 @@
         self._build_contrast_vector()
 
         # Set a flag to indicate that LFCs are unshrunk
         self.shrunk_LFCs = False
         self.n_processes = get_num_processes(n_cpus)
         self.batch_size = batch_size
         self.joblib_verbosity = joblib_verbosity
+        self.quiet = quiet
 
         # If the `refit_cooks` attribute of the dds object is True, check that outliers
         # were actually refitted.
         if self.dds.refit_cooks and "replaced" not in self.dds.varm:
             raise AttributeError(
                 "dds has 'refit_cooks' set to True but Cooks outliers have not been "
                 "refitted. Please run 'dds.refit()' first or set 'dds.refit_cooks' "
@@ -192,36 +202,40 @@
         self.results_df["baseMean"] = self.base_mean
         self.results_df["log2FoldChange"] = self.LFC @ self.contrast_vector / np.log(2)
         self.results_df["lfcSE"] = self.SE / np.log(2)
         self.results_df["stat"] = self.statistics
         self.results_df["pvalue"] = self.p_values
         self.results_df["padj"] = self.padj
 
-        print(
-            f"Log2 fold change & Wald test p-value: "
-            f"{self.contrast[0]} {self.contrast[1]} vs {self.contrast[2]}"
-        )
+        if not self.quiet:
+            print(
+                f"Log2 fold change & Wald test p-value: "
+                f"{self.contrast[0]} {self.contrast[1]} vs {self.contrast[2]}",
+                file=sys.stderr,
+            )
         display(self.results_df)
 
     def run_wald_test(self) -> None:
         """Perform a Wald test.
 
         Get gene-wise p-values for gene over/under-expression.`
         """
 
         num_genes = self.dds.n_vars
         num_vars = self.design_matrix.shape[1]
 
         # Raise a warning if LFCs are shrunk.
         if self.shrunk_LFCs:
-            print(
-                "Note: running Wald test on shrunk LFCs. "
-                "Some sequencing datasets show better performance with the testing "
-                "separated from the use of the LFC prior."
-            )
+            if not self.quiet:
+                print(
+                    "Note: running Wald test on shrunk LFCs. "
+                    "Some sequencing datasets show better performance with the testing "
+                    "separated from the use of the LFC prior.",
+                    file=sys.stderr,
+                )
 
         mu = (
             np.exp(self.design_matrix @ self.LFC.T)
             .multiply(self.dds.obsm["size_factors"], 0)
             .values
         )
 
@@ -230,15 +244,16 @@
             ridge_factor = np.diag(1 / self.prior_LFC_var**2)
         else:
             ridge_factor = np.diag(np.repeat(1e-6, num_vars))
 
         design_matrix = self.design_matrix.values
         LFCs = self.LFC.values
 
-        print("Running Wald tests...")
+        if not self.quiet:
+            print("Running Wald tests...", file=sys.stderr)
         start = time.time()
         with parallel_backend("loky", inner_max_num_threads=1):
             res = Parallel(
                 n_jobs=self.n_processes,
                 verbose=self.joblib_verbosity,
                 batch_size=self.batch_size,
             )(
@@ -249,15 +264,16 @@
                     mu=mu[:, i],
                     ridge_factor=ridge_factor,
                     contrast=self.contrast_vector,
                 )
                 for i in range(num_genes)
             )
         end = time.time()
-        print(f"... done in {end-start:.2f} seconds.\n")
+        if not self.quiet:
+            print(f"... done in {end-start:.2f} seconds.\n", file=sys.stderr)
 
         pvals, stats, se = zip(*res)
 
         self.p_values: pd.Series = pd.Series(pvals, index=self.dds.var_names)
         self.statistics: pd.Series = pd.Series(stats, index=self.dds.var_names)
         self.SE: pd.Series = pd.Series(se, index=self.dds.var_names)
 
@@ -322,15 +338,16 @@
         # Set priors
         prior_no_shrink_scale = 15
         prior_var = self._fit_prior_var(coeff_idx=coeff_idx)
         prior_scale = np.minimum(np.sqrt(prior_var), 1)
 
         design_matrix = self.design_matrix.values
 
-        print("Fitting MAP LFCs...")
+        if not self.quiet:
+            print("Fitting MAP LFCs...", file=sys.stderr)
         start = time.time()
         with parallel_backend("loky", inner_max_num_threads=1):
             res = Parallel(
                 n_jobs=self.n_processes,
                 verbose=self.joblib_verbosity,
                 batch_size=self.batch_size,
             )(
@@ -343,15 +360,16 @@
                     prior_scale=prior_scale,
                     optimizer="L-BFGS-B",
                     shrink_index=coeff_idx,
                 )
                 for i in self.dds.non_zero_idx
             )
         end = time.time()
-        print(f"... done in {end-start:.2f} seconds.\n")
+        if not self.quiet:
+            print(f"... done in {end-start:.2f} seconds.\n", file=sys.stderr)
 
         lfcs, inv_hessians, l_bfgs_b_converged_ = zip(*res)
 
         self.LFC.iloc[:, coeff_idx].update(
             pd.Series(
                 np.array(lfcs)[:, coeff_idx],
                 index=self.dds.non_zero_genes,
@@ -384,21 +402,60 @@
             self.results_df["lfcSE"] = self.SE / np.log(2)
 
             # Get the corrresponding factor, tested and reference levels of the shrunk
             # coefficient
             split_coeff = coeff.split("_")
             # coeffs are of the form "factor_A_vs_B", hence "factor" is split_coeff[0],
             # "A" is split_coeff[1] and "B" split_coeff[3]
-            print(
-                f"Shrunk Log2 fold change & Wald test p-value: "
-                f"{split_coeff[0]} {split_coeff[1]} vs {split_coeff[3]}"
-            )
+            if not self.quiet:
+                print(
+                    f"Shrunk Log2 fold change & Wald test p-value: "
+                    f"{split_coeff[0]} {split_coeff[1]} vs {split_coeff[3]}",
+                    file=sys.stderr,
+                )
 
             display(self.results_df)
 
+    def plot_MA(self, log: bool = True, save_path: Optional[str] = None, **kwargs):
+        """
+        Create an log ratio (M)-average (A) plot using matplotlib.
+
+        Useful for looking at log fold-change versus mean expression
+        between two groups/samples/etc.
+        Uses matplotlib to emulate make_MA() function in DESeq2 in R.
+
+        Parameters
+        ----------
+
+        log : bool
+            Whether or not to log scale x and y axes (``default=True``).
+
+        save_path : str or None
+            The path where to save the plot. If left None, the plot won't be saved
+            (``default=None``).
+
+        **kwargs
+            Matplotlib keyword arguments for the scatter plot.
+        """
+
+        # Raise an error if results_df are missing
+        if not hasattr(self, "results_df"):
+            raise AttributeError(
+                "Trying to make an MA plot but p-values were not computed yet. "
+                "Please run the summary() method first."
+            )
+
+        make_MA_plot(
+            self.results_df,
+            padj_thresh=self.alpha,
+            log=log,
+            save_path=save_path,
+            **kwargs,
+        )
+
     def _independent_filtering(self) -> None:
         """Compute adjusted p-values using independent filtering.
 
         Corrects p-value trend (see :cite:p:`DeseqStats-love2014moderated`)
         """
 
         # Check that p-values are available. If not, compute them.
@@ -550,15 +607,15 @@
     def _build_contrast(self, contrast: Optional[List[str]] = None) -> None:
         """
         Check the validity of the contrast (if provided). If not, build a default
         contrast, corresponding to the last column of the design matrix.
 
         A contrast should be a list of three strings, in the following format:
         ``['variable_of_interest', 'tested_level', 'reference_level']``.
-        Names must correspond to the clinical data passed to the DeseqDataSet.
+        Names must correspond to the metadata data passed to the DeseqDataSet.
         E.g., ``['condition', 'B', 'A']`` will measure the LFC of 'condition B'
         compared to 'condition A'. If None, the last variable from the design matrix
         is chosen as the variable of interest, and the reference level is picked
         alphabetically.
 
         Parameters
         ----------
```

### Comparing `pydeseq2-0.3.5/pydeseq2/grid_search.py` & `pydeseq2-0.3.6/pydeseq2/grid_search.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.5/pydeseq2/preprocessing.py` & `pydeseq2-0.3.6/pydeseq2/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.5/pydeseq2/utils.py` & `pydeseq2-0.3.6/pydeseq2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 import pydeseq2
 from pydeseq2.grid_search import grid_fit_alpha
 from pydeseq2.grid_search import grid_fit_beta
 from pydeseq2.grid_search import grid_fit_shrink_beta
 
 
 def load_example_data(
-    modality: Literal["raw_counts", "clinical"] = "raw_counts",
+    modality: Literal["raw_counts", "metadata"] = "raw_counts",
     dataset: Literal["synthetic"] = "synthetic",
     debug: bool = False,
     debug_seed: int = 42,
 ) -> pd.DataFrame:
     """Load synthetic example data.
 
-    May load either clinical or rna-seq data. For now, this function may only return the
+    May load either metadata or rna-seq data. For now, this function may only return the
     synthetic data provided as part of this repo, but new datasets might be added in the
     future.
 
     Parameters
     ----------
     modality : str
-        Data modality. "raw_counts" or "clinical".
+        Data modality. "raw_counts" or "metadata".
 
     dataset : str
         The dataset for which to return gene expression data.
         If "synthetic", will return the synthetic data that is used for CI unit tests.
         (default: ``"synthetic"``).
 
     debug : bool
@@ -55,16 +55,16 @@
 
     Returns
     -------
     pandas.DataFrame
         Requested data modality.
     """
 
-    assert modality in ["raw_counts", "clinical"], (
-        "The modality argument must be one of the following: " "raw_counts, clinical"
+    assert modality in ["raw_counts", "metadata"], (
+        "The modality argument must be one of the following: " "raw_counts, metadata"
     )
 
     assert dataset in [
         "synthetic"
     ], "The dataset argument must be one of the following: synthetic."
 
     # Load data
@@ -72,33 +72,33 @@
 
     if dataset == "synthetic":
         path_to_data = datasets_path / "synthetic"
         if Path(path_to_data).is_dir():
             # Cast the Paths to strings to have coherent types wrt to the url case (that
             # does not handle Paths), else mypy throws an error.
             path_to_data_counts = str(path_to_data / "test_counts.csv")
-            path_to_data_clinical = str(path_to_data / "test_clinical.csv")
+            path_to_data_metadata = str(path_to_data / "test_metadata.csv")
         else:
             # if the path does not exist (as is the case in RDT) load it from github
             url_to_data = (
                 "https://raw.githubusercontent.com/owkin/"
                 "PyDESeq2/main/datasets/synthetic/"
             )
             path_to_data_counts = url_to_data + "/test_counts.csv"
-            path_to_data_clinical = url_to_data + "/test_clinical.csv"
+            path_to_data_metadata = url_to_data + "/test_metadata.csv"
 
         if modality == "raw_counts":
             df = pd.read_csv(
                 path_to_data_counts,
                 sep=",",
                 index_col=0,
             ).T
-        elif modality == "clinical":
+        elif modality == "metadata":
             df = pd.read_csv(
-                path_to_data_clinical,
+                path_to_data_metadata,
                 sep=",",
                 index_col=0,
             )
 
     if debug:
         # TODO: until we provide a larger dataset, this option is useless
         # subsample 10 samples and 100 genes
@@ -134,34 +134,34 @@
     if (counts % 1 != 0).any().any():
         raise ValueError("The count matrix should only contain integers.")
     if (counts < 0).any().any():
         raise ValueError("The count matrix should only contain non-negative values.")
 
 
 def build_design_matrix(
-    clinical_df: pd.DataFrame,
+    metadata: pd.DataFrame,
     design_factors: Union[str, List[str]] = "condition",
     ref_level: Optional[List[str]] = None,
     expanded: bool = False,
     intercept: bool = True,
 ) -> pd.DataFrame:
     """Build design_matrix matrix for DEA.
 
     Only single factor, 2-level designs are currently supported.
     Unless specified, the reference factor is chosen alphabetically.
     NOTE: For now, each factor should have exactly two levels.
 
     Parameters
     ----------
-    clinical_df : pandas.DataFrame
-        DataFrame containing clinical information.
+    metadata : pandas.DataFrame
+        DataFrame containing metadata information.
         Must be indexed by sample barcodes.
 
     design_factors : str or list
-        Name of the columns of clinical_df to be used as design_matrix variables.
+        Name of the columns of metadata to be used as design_matrix variables.
         (default: ``"condition"``).
 
     ref_level : list or None
         An optional list of two strings of the form ``["factor", "ref_level"]``
         specifying the factor of interest and the desired reference level, e.g.
         ``["condition", "A"]``. (default: ``None``).
 
@@ -182,56 +182,56 @@
     if isinstance(
         design_factors, str
     ):  # if there is a single factor, convert to singleton list
         design_factors = [design_factors]
 
     for factor in design_factors:
         # Check that each factor has at least 2 levels
-        if len(np.unique(clinical_df[factor])) < 2:
+        if len(np.unique(metadata[factor])) < 2:
             raise ValueError(
                 f"Factors should take at least two values, but {factor} "
-                f"takes the single value '{np.unique(clinical_df[factor])}'."
+                f"takes the single value '{np.unique(metadata[factor])}'."
             )
 
-    design_matrix = pd.get_dummies(clinical_df[design_factors], drop_first=not expanded)
+    design_matrix = pd.get_dummies(metadata[design_factors], drop_first=not expanded)
 
     if ref_level is not None:
         if len(ref_level) != 2:
             raise KeyError("The reference level should contain 2 strings.")
-        if ref_level[1] not in clinical_df[ref_level[0]].values:
+        if ref_level[1] not in metadata[ref_level[0]].values:
             raise KeyError(
-                f"The clinical data should contain a '{ref_level[0]}' column"
+                f"The metadata data should contain a '{ref_level[0]}' column"
                 f" with a '{ref_level[1]}' level."
             )
 
         # Check that the reference level is not in the matrix (if unexpanded design)
         ref_level_name = "_".join(ref_level)
         if (not expanded) and ref_level_name in design_matrix.columns:
             # Remove the reference level and add one
             factor_cols = [
                 col for col in design_matrix.columns if col.startswith(ref_level[0])
             ]
             missing_level = next(
                 level
-                for level in np.unique(clinical_df[ref_level[0]])
+                for level in np.unique(metadata[ref_level[0]])
                 if f"{ref_level[0]}_{level}" not in design_matrix.columns
             )
             design_matrix[f"{ref_level[0]}_{missing_level}"] = 1 - design_matrix[
                 factor_cols
             ].sum(1)
             design_matrix.drop(ref_level_name, axis="columns", inplace=True)
 
     if not expanded:
         # Add reference level as column name suffix
         for factor in design_factors:
             if ref_level is None or factor != ref_level[0]:
                 # The reference is the unique level that is no longer there
                 ref = next(
                     level
-                    for level in np.unique(clinical_df[factor])
+                    for level in np.unique(metadata[factor])
                     if f"{factor}_{level}" not in design_matrix.columns
                 )
             else:
                 # The reference level is given as an argument
                 ref = ref_level[1]
             design_matrix.columns = [
                 f"{col}_vs_{ref}" if col.startswith(factor) else col
@@ -1286,15 +1286,15 @@
         Whether or not to log scale x and y axes (``default=True``).
 
     save_path : str or None
         The path where to save the plot. If left None, the plot won't be saved
         (``default=None``).
 
     **kwargs
-        Keyword arguments for the scatter plot.
+        Matplotlib keyword arguments for the scatter plot.
     """
 
     # Adding more colors if plotting more than 3 traces
     if len(disps) == 3:
         colors = "kbr"
     else:
         colors = "kbrcmyg"
@@ -1323,7 +1323,70 @@
     plt.legend(legend_labels, loc="best")
     plt.xlabel("mean of normalized counts")
     plt.ylabel("dispersion")
     plt.tight_layout()
     if save_path is not None:
         plt.savefig(save_path, bbox_inches="tight")
     plt.show()
+
+
+def make_MA_plot(
+    results_df: pd.DataFrame,
+    padj_thresh: float = 0.05,
+    log: bool = True,
+    save_path: Optional[str] = None,
+    **kwargs,
+) -> None:
+    """
+    Create an log ratio (M)-average (A) plot using matplotlib.
+
+    Useful for looking at log fold-change versus mean expression
+    between two groups/samples/etc.
+    Uses matplotlib to emulate make_MA() function in DESeq2 in R.
+
+    Parameters
+    ----------
+    results_df : pd.DataFrame
+        Resultant dataframe after running DeseqStats() and .summary().
+
+    padj_thresh : float
+        P-value threshold to subset scatterplot colors on.
+
+    log : bool
+        Whether or not to log scale x and y axes (``default=True``).
+
+    save_path : str or None
+        The path where to save the plot. If left None, the plot won't be saved
+        (``default=None``).
+
+    **kwargs
+        Matplotlib keyword arguments for the scatter plot.
+    """
+
+    colors = results_df["padj"].apply(lambda x: "darkred" if x < padj_thresh else "gray")
+
+    fig, ax = plt.subplots(dpi=600)
+
+    # Set default alpha and s parameters, if not already specified
+    kwargs.setdefault("alpha", 0.5)
+    kwargs.setdefault("s", 0.2)
+
+    plt.scatter(
+        x=results_df["baseMean"],
+        y=results_df["log2FoldChange"],
+        c=colors,
+        **kwargs,
+    )
+
+    ax.set_adjustable("datalim")
+
+    if log is True:
+        plt.xscale("log")
+
+    plt.xlabel("mean of normalized counts")
+    plt.ylabel("log2 fold change")
+
+    plt.axhline(0, color="red", alpha=0.5, linestyle="--", zorder=3)
+    plt.tight_layout()
+
+    if save_path is not None:
+        plt.savefig(save_path, bbox_inches="tight")
```

### Comparing `pydeseq2-0.3.5/pydeseq2.egg-info/PKG-INFO` & `pydeseq2-0.3.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,42 @@
-Metadata-Version: 2.1
-Name: pydeseq2
-Version: 0.3.5
-Summary: A python implementation of DESeq2.
-Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
-Author-email: boris.muzellec@owkin.com
-License: MIT
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <img src="docs/source/_static/pydeseq2_logo_green.png" width="600">
 
+#
+[![pypi version](https://img.shields.io/pypi/v/pydeseq2)](https://pypi.org/project/pydeseq2)
+[![pypiDownloads](https://pepy.tech/badge/pydeseq2)](https://pepy.tech/project/pydeseq2)
+[![condaDownloads](https://img.shields.io/conda/dn/bioconda/pydeseq2?logo=Anaconda)](https://anaconda.org/bioconda/pydeseq2)
+[![license](https://img.shields.io/pypi/l/pydeseq2)](LICENSE)
+
+PyDESeq2 is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
+method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
+It aims to facilitate DEA experiments for python users.
+
+As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
+scratch, you may experience some differences in terms of retrieved values or available features.
+
+Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
+and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
+In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Table of Contents
 - [PyDESeq2](#pydeseq2)
   - [Table of Contents](#table-of-contents)
-  - [Overview](#overview)
   - [Installation](#installation)
     - [Requirements](#requirements)
   - [Getting started](#getting-started)
     - [Documentation](#documentation)
     - [Data](#data)
   - [Contributing](#contributing)
     - [1 - Download the repository](#1---download-the-repository)
     - [2 - Create a conda environment](#2---create-a-conda-environment)
   - [Development roadmap](#development-roadmap)
   - [Citing this work](#citing-this-work)
   - [References](#references)
   - [License](#license)
 
-## Overview
-
-This package is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
-method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
-It aims to facilitate DEA experiments for python users.
-
-As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
-scratch, you may experience some differences in terms of retrieved values or available features.
-
-Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
-and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
-In case there is a feature you would particularly like to be implemented, feel free to open an issue.
-
 ## Installation
 
 ### PyPI
 
 `PyDESeq2` can be installed from PyPI using `pip`:
 
 `pip install pydeseq2`
@@ -134,16 +124,17 @@
 Here are some of the features and improvements we plan to implement in the future:
 
 - [x] Integration to the [scverse](https://scverse.org/) ecosystem:
   * [x] Refactoring to use the [AnnData](https://anndata.readthedocs.io/) data structure
   * [x] Submitting a PR to be listed as an [scverse ecosystem](https://github.com/scverse/ecosystem-packages/) package
 - [x] Variance-stabilizing transformation
 - [ ] Improving multi-factor analysis:
-  * [x] Allowing n-level factors (only bi-level for now)
+  * [x] Allowing n-level factors
   * [ ] Implementing interaction terms
+  * [ ] Support for continuous covariates
 
 ## Citing this work
 
 ```
 @article{muzellec2022pydeseq2,
   title={PyDESeq2: a python package for bulk RNA-seq differential expression analysis},
   author={Muzellec, Boris and Telenczuk, Maria and Cabeli, Vincent and Andreux, Mathieu},
```

### Comparing `pydeseq2-0.3.5/setup.py` & `pydeseq2-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.5/tests/test_docstring.py` & `pydeseq2-0.3.6/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.5/tests/test_edge_cases.py` & `pydeseq2-0.3.6/tests/test_edge_cases.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,31 +14,29 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     n, m = counts_df.shape
 
     # Introduce a few genes with fully 0 counts
     np.random.seed(42)
     zero_genes = counts_df.columns[np.random.choice(m, size=m // 3, replace=False)]
     counts_df[zero_genes] = 0
 
     # Run analysis
-    dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors="condition"
-    )
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
     dds.deseq2()
 
     # check that the corresponding parameters are NaN
     assert np.isnan(dds[:, zero_genes].varm["dispersions"]).all()
     assert np.isnan(dds[:, zero_genes].varm["LFC"]).all().all()
 
     res = DeseqStats(dds)
@@ -56,108 +54,108 @@
 
 # Tests on the count matrix
 def test_nan_counts():
     """Test that a ValueError is thrown when the count matrix contains NaNs."""
     counts_df = pd.DataFrame(
         {"gene1": [0, np.nan], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
+    metadata = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
-        DeseqDataSet(counts=counts_df, clinical=clinical_df, design_factors="condition")
+        DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
 
 
 def test_numeric_counts():
     """Test that a ValueError is thrown when the count matrix contains
     non-numeric values.
     """
     counts_df = pd.DataFrame(
         {"gene1": [0, "a"], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
+    metadata = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
-        DeseqDataSet(counts=counts_df, clinical=clinical_df, design_factors="condition")
+        DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
 
 
 def test_integer_counts():
     """Test that a ValueError is thrown when the count matrix contains
     non-integer values."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1.5], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
+    metadata = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
-        DeseqDataSet(counts=counts_df, clinical=clinical_df, design_factors="condition")
+        DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
 
 
 def test_non_negative_counts():
     """Test that a ValueError is thrown when the count matrix contains
     negative values."""
     counts_df = pd.DataFrame(
         {"gene1": [0, -1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
+    metadata = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
-        DeseqDataSet(counts=counts_df, clinical=clinical_df, design_factors="condition")
+        DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
 
 
-# Tests on the clinical data (design factors)
+# Tests on the metadata data (design factors)
 def test_nan_factors():
     """Test that a ValueError is thrown when the design factor contains NaNs."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame({"condition": [0, np.NaN]}, index=["sample1", "sample2"])
+    metadata = pd.DataFrame({"condition": [0, np.NaN]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
-        DeseqDataSet(counts=counts_df, clinical=clinical_df, design_factors="condition")
+        DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
 
 
 def test_one_factor():
     """Test that a ValueError is thrown when the design factor takes only one value."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame({"condition": [0, 0]}, index=["sample1", "sample2"])
+    metadata = pd.DataFrame({"condition": [0, 0]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
-        DeseqDataSet(counts=counts_df, clinical=clinical_df, design_factors="condition")
+        DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
 
 
 def test_rank_deficient_design():
     """Test that a ValueError is thrown when the design matrix does not have full column
     rank."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame(
+    metadata = pd.DataFrame(
         {"condition": [0, 1], "batch": ["A", "B"]}, index=["sample1", "sample2"]
     )
 
     with pytest.warns(UserWarning):
         DeseqDataSet(
-            counts=counts_df, clinical=clinical_df, design_factors=["condition", "batch"]
+            counts=counts_df, metadata=metadata, design_factors=["condition", "batch"]
         )
 
 
 def test_reference_level():
     """Test that a ValueError is thrown when the reference level is not one of the
     design factor values."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
+    metadata = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
 
     with pytest.raises(KeyError):
         DeseqDataSet(
             counts=counts_df,
-            clinical=clinical_df,
+            metadata=metadata,
             design_factors="condition",
             ref_level="control",
         )
 
 
 def test_lfc_shrinkage_coeff():
     """Test that a KeyError is thrown when attempting to shrink an unexisting LFC
@@ -166,23 +164,21 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
-    dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors="condition"
-    )
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
     dds.deseq2()
 
     # Check that coeff=None gives the same results as the default
     # coefficient condition_B_vs_A
     res_1 = DeseqStats(dds)
     res_1.summary()
     res_1.lfc_shrink(coeff=None)
@@ -196,49 +192,49 @@
     assert (shrunk_lfcs_1 == shrunk_lfcs_2).all()
 
     with pytest.raises(KeyError):
         res_1.lfc_shrink(coeff="this_coeff_does_not_exist")
 
 
 def test_indexes():
-    """Test that a ValueError is thrown when the count matrix and the clinical data
+    """Test that a ValueError is thrown when the count matrix and the metadata data
     don't have the same index."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
-    clinical_df = pd.DataFrame({"condition": [0, 1]}, index=["sample01", "sample02"])
+    metadata = pd.DataFrame({"condition": [0, 1]}, index=["sample01", "sample02"])
 
     with pytest.raises(ValueError):  # Should be raised by AnnData
         DeseqDataSet(
             counts=counts_df,
-            clinical=clinical_df,
+            metadata=metadata,
             design_factors="condition",
         )
 
 
 def test_contrast():
     """Test that KeyErrors/ValueErrors are thrown when invalid contrasts are passed to a
     DeseqStats."""
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Run analysis
     dds = DeseqDataSet(
         counts=counts_df,
-        clinical=clinical_df,
+        metadata=metadata,
         refit_cooks=False,
         design_factors=["condition", "group"],
     )
     dds.deseq2()
 
     # Too short
     with pytest.raises(ValueError):
@@ -264,24 +260,24 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Run analysis
     dds = DeseqDataSet(
         counts=counts_df,
-        clinical=clinical_df,
+        metadata=metadata,
         refit_cooks=False,
         design_factors="condition",
     )
     dds.deseq2()
 
     # Set refit_cooks to True even though outliers were not refitted
     dds.refit_cooks = True
@@ -299,36 +295,38 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Subsample two samples for each condition
     samples_to_keep = ["sample1", "sample2", "sample99", "sample100"]
     counts_df = counts_df.loc[samples_to_keep]
-    clinical_df = clinical_df.loc[samples_to_keep]
+    metadata = metadata.loc[samples_to_keep]
 
     # Introduce an outlier
     counts_df.iloc[0, 0] = 1000
 
-    # Run analysis. Should not throw an error.
+    # Run analysis. Should not throw degrees of freedom warning.
     dds = DeseqDataSet(
         counts=counts_df,
-        clinical=clinical_df,
+        metadata=metadata,
         refit_cooks=True,
         design_factors="condition",
     )
-    dds.deseq2()
+
+    with pytest.warns(UserWarning):
+        dds.deseq2()
 
     res = DeseqStats(dds)
     res.summary()
 
     # Check that no gene was refit, as there are not enough samples.
     assert dds.varm["replaced"].sum() == 0
 
@@ -341,16 +339,16 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Subsample two samples for each condition
     samples_to_keep = [
         "sample1",
@@ -363,24 +361,24 @@
         "sample97",
         "sample98",
         "sample99",
         "sample100",
     ]
 
     counts_df = counts_df.loc[samples_to_keep]
-    clinical_df = clinical_df.loc[samples_to_keep]
+    metadata = metadata.loc[samples_to_keep]
 
     # Introduce outliers
     counts_df.iloc[0, 0] = 1000
     counts_df.iloc[-1, -1] = 1000
 
     # Run analysis. Should not throw an error.
     dds = DeseqDataSet(
         counts=counts_df,
-        clinical=clinical_df,
+        metadata=metadata,
         refit_cooks=True,
         design_factors="condition",
     )
     dds.deseq2()
 
     res = DeseqStats(dds)
     res.summary()
@@ -393,22 +391,55 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Artificially zero-inflate the data
     # Each gene will have at least one sample with zero counts
     np.random.seed(42)
     idx = np.random.choice(len(counts_df), counts_df.shape[-1])
     counts_df.iloc[idx, :] = 0
 
-    dds = DeseqDataSet(counts=counts_df, clinical=clinical_df)
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata)
     with pytest.warns(RuntimeWarning):
         dds.deseq2()
+
+
+def test_plot_MA():
+    """
+    Test that a KeyError is thrown when attempting to run plot_MA without running the
+    statistical analysis first.
+    """
+
+    counts_df = load_example_data(
+        modality="raw_counts",
+        dataset="synthetic",
+        debug=False,
+    )
+
+    metadata = load_example_data(
+        modality="metadata",
+        dataset="synthetic",
+        debug=False,
+    )
+
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata)
+    dds.deseq2()
+
+    # Initialize a DeseqStats object without runnning the analysis
+    res = DeseqStats(dds)
+
+    with pytest.raises(AttributeError):
+        res.plot_MA()
+
+    # Run the analysis
+    res.summary()
+    # Now this shouldn't throw an error
+    res.plot_MA()
```

### Comparing `pydeseq2-0.3.5/tests/test_pydeseq2.py` & `pydeseq2-0.3.6/tests/test_pydeseq2.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,25 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     r_res = pd.read_csv(
         os.path.join(test_path, "data/single_factor/r_test_res.csv"), index_col=0
     )
 
-    dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors="condition"
-    )
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
     dds.deseq2()
 
     res = DeseqStats(dds)
     res.summary()
     res_df = res.results_df
 
     # check that the same p-values are NaN
@@ -69,27 +67,27 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     r_res = pd.read_csv(
         os.path.join(test_path, "data/single_factor/r_test_res.csv"), index_col=0
     )
 
     dds = DeseqDataSet(
         counts=counts_df,
-        clinical=clinical_df,
+        metadata=metadata,
         design_factors="condition",
         refit_cooks=False,
     )
     dds.deseq2()
 
     res = DeseqStats(dds)
     res.summary()
@@ -123,32 +121,30 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     r_size_factors = pd.read_csv(
         os.path.join(test_path, "data/single_factor/r_test_size_factors.csv"),
         index_col=0,
     ).squeeze()
 
     r_dispersions = pd.read_csv(
         os.path.join(test_path, "data/single_factor/r_test_dispersions.csv"), index_col=0
     ).squeeze()
 
-    dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors="condition"
-    )
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
     dds.deseq2()
     dds.obsm["size_factors"] = r_size_factors.values
     dds.varm["dispersions"] = r_dispersions.values
     dds.varm["LFC"].iloc[:, 1] = r_res.log2FoldChange.values * np.log(2)
 
     res = DeseqStats(dds)
     res.summary()
@@ -172,28 +168,26 @@
     test_path = str(Path(os.path.realpath(tests.__file__)).parent.resolve())
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     r_size_factors = pd.read_csv(
         os.path.join(test_path, "data/single_factor/r_iterative_size_factors.csv"),
         index_col=0,
     ).squeeze()
 
-    dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors="condition"
-    )
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
     dds._fit_iterate_size_factors()
 
     # Check that the same LFC are found (up to tol)
     assert (
         abs(r_size_factors - dds.obsm["size_factors"]) / abs(r_size_factors)
     ).max() < tol
 
@@ -208,26 +202,26 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     r_res = pd.read_csv(
         os.path.join(test_path, "data/multi_factor/r_test_res.csv"), index_col=0
     )
 
     dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors=["group", "condition"]
+        counts=counts_df, metadata=metadata, design_factors=["group", "condition"]
     )
     dds.deseq2()
 
     res = DeseqStats(dds)
     res.summary()
     res_df = res.results_df
 
@@ -259,31 +253,31 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     r_size_factors = pd.read_csv(
         os.path.join(test_path, "data/multi_factor/r_test_size_factors.csv"),
         index_col=0,
     ).squeeze()
 
     r_dispersions = pd.read_csv(
         os.path.join(test_path, "data/multi_factor/r_test_dispersions.csv"), index_col=0
     ).squeeze()
 
     dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors=["group", "condition"]
+        counts=counts_df, metadata=metadata, design_factors=["group", "condition"]
     )
     dds.deseq2()
     dds.obsm["size_factors"] = r_size_factors.values
     dds.varm["dispersions"] = r_dispersions.values
     dds.varm["LFC"].iloc[:, 1] = r_res.log2FoldChange.values * np.log(2)
 
     res = DeseqStats(dds)
@@ -307,22 +301,22 @@
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors=["group", "condition"]
+        counts=counts_df, metadata=metadata, design_factors=["group", "condition"]
     )
     dds.deseq2()
 
     res_B_vs_A = DeseqStats(dds, contrast=["condition", "B", "A"])
     res_A_vs_B = DeseqStats(dds, contrast=["condition", "A", "B"])
     res_B_vs_A.summary()
     res_A_vs_B.summary()
@@ -356,22 +350,22 @@
     # Load data
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Make an anndata object
-    adata = ad.AnnData(X=counts_df.astype(int), obs=clinical_df)
+    adata = ad.AnnData(X=counts_df.astype(int), obs=metadata)
 
     # Put some dummy data in unused fields
     adata.obsm["dummy_metadata"] = np.random.choice(2, adata.n_obs)
     adata.varm["dummy_param"] = np.random.randn(adata.n_vars)
 
     # Put values in the dispersions field
     adata.varm["dispersions"] = np.random.randn(adata.n_vars) ** 2
@@ -411,16 +405,16 @@
     # Load data
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Load R data
     test_path = str(Path(os.path.realpath(tests.__file__)).parent.resolve())
 
@@ -429,24 +423,20 @@
     ).T
 
     r_vst_with_design = pd.read_csv(
         os.path.join(test_path, "data/single_factor/r_vst_with_design.csv"), index_col=0
     ).T
 
     # Test blind design
-    dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors=["condition"]
-    )
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors=["condition"])
     dds.vst(use_design=False)
     assert (np.abs(r_vst - dds.layers["vst_counts"]) / r_vst).max().max() < tol
 
     # Test full design
-    dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors=["condition"]
-    )
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors=["condition"])
     dds.vst(use_design=True)
     assert (
         np.abs(r_vst_with_design - dds.layers["vst_counts"]) / r_vst_with_design
     ).max().max() < tol
 
 
 def test_mean_vst(tol=0.02):
@@ -457,64 +447,62 @@
     # Load data
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Load R data
     test_path = str(Path(os.path.realpath(tests.__file__)).parent.resolve())
 
     r_vst = pd.read_csv(
         os.path.join(test_path, "data/single_factor/r_mean_vst.csv"), index_col=0
     ).T
 
     # Test blind design
-    dds = DeseqDataSet(
-        counts=counts_df, clinical=clinical_df, design_factors=["condition"]
-    )
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata, design_factors=["condition"])
     dds.vst(use_design=False, fit_type="mean")
     assert (np.abs(r_vst - dds.layers["vst_counts"]) / r_vst).max().max() < tol
 
 
 def test_ref_level():
     """Test that DeseqDataSet columns are created according to the passed reference
     level, if any.
     """
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     dds = DeseqDataSet(
         counts=counts_df,
-        clinical=clinical_df,
+        metadata=metadata,
         design_factors=["group", "condition"],
         ref_level=["group", "Y"],
     )
 
     # Check that the column exists
     assert "group_X_vs_Y" in dds.obsm["design_matrix"].columns
     # Check that its content is correct
     assert (
         dds.obsm["design_matrix"]["group_X_vs_Y"]
-        == clinical_df["group"].apply(
+        == metadata["group"].apply(
             lambda x: 1 if x == "X" else 0 if x == "Y" else np.NaN
         )
     ).all()
 
 
 def test_deseq2_norm():
     """Test that deseq2_norm() called on a pandas dataframe outputs the same results as
@@ -522,22 +510,22 @@
     """
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
 
-    clinical_df = load_example_data(
-        modality="clinical",
+    metadata = load_example_data(
+        modality="metadata",
         dataset="synthetic",
         debug=False,
     )
 
     # Fit size factors from DeseqDataSet
-    dds = DeseqDataSet(counts=counts_df, clinical=clinical_df)
+    dds = DeseqDataSet(counts=counts_df, metadata=metadata)
     dds.fit_size_factors()
     s1 = dds.obsm["size_factors"]
 
     # Fit size factors from counts directly
     s2 = deseq2_norm(counts_df)[1]
 
     np.testing.assert_almost_equal(
```

### Comparing `pydeseq2-0.3.5/tests/test_utils.py` & `pydeseq2-0.3.6/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     deviation = var_th / np.sqrt(n_montecarlo)
     assert np.abs(diff) < 0.2 * deviation
     error_var = np.abs(sample.var() - var_th) / var_th
     assert error_var < 1 / np.sqrt(n_montecarlo)
 
 
 # Test data loading from outside the package (e.g. on RTF)
-@pytest.mark.parametrize("modality", ["raw_counts", "clinical"])
+@pytest.mark.parametrize("modality", ["raw_counts", "metadata"])
 @pytest.mark.parametrize("mocked_dir_flag", [True, False])
 @mock.patch("pathlib.Path.is_dir")
 def test_rtd_example_data_loading(mocked_function, modality, mocked_dir_flag):
     """
     Test that load_example_data still works when run from a place where the ``datasets``
     directory is not accessible, as is when the documentation is built on readthedocs.
     """
```

