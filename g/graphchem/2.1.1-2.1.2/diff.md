# Comparing `tmp/graphchem-2.1.1.tar.gz` & `tmp/graphchem-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphchem-2.1.1.tar", last modified: Fri Apr  7 23:50:15 2023, max compression
+gzip compressed data, was "graphchem-2.1.2.tar", last modified: Tue Aug  1 02:36:54 2023, max compression
```

## Comparing `graphchem-2.1.1.tar` & `graphchem-2.1.2.tar`

### file list

```diff
@@ -1,34 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 23:50:15.935133 graphchem-2.1.1/
--rw-rw-rw-   0        0        0     1071 2023-03-30 20:48:18.000000 graphchem-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     2956 2023-04-07 23:50:15.934133 graphchem-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2592 2023-04-07 23:29:40.000000 graphchem-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 23:50:15.868111 graphchem-2.1.1/graphchem/
--rw-rw-rw-   0        0        0       46 2023-04-01 01:45:07.000000 graphchem-2.1.1/graphchem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:50:15.897111 graphchem-2.1.1/graphchem/data/
--rw-rw-rw-   0        0        0       52 2023-03-30 20:48:18.000000 graphchem-2.1.1/graphchem/data/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-04-07 23:22:25.000000 graphchem-2.1.1/graphchem/data/structs.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:50:15.899223 graphchem-2.1.1/graphchem/datasets/
--rw-rw-rw-   0        0        0       66 2023-03-30 20:48:18.000000 graphchem-2.1.1/graphchem/datasets/__init__.py
--rw-rw-rw-   0        0        0     1935 2023-04-07 23:22:25.000000 graphchem-2.1.1/graphchem/datasets/sets.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:50:15.929138 graphchem-2.1.1/graphchem/datasets/static/
--rw-rw-rw-   0        0        0    10547 2023-03-30 20:48:18.000000 graphchem-2.1.1/graphchem/datasets/static/cn.csv
--rw-rw-rw-   0        0        0     5790 2023-03-30 20:48:18.000000 graphchem-2.1.1/graphchem/datasets/static/lhv.csv
--rw-rw-rw-   0        0        0     5496 2023-03-30 20:48:18.000000 graphchem-2.1.1/graphchem/datasets/static/mon.csv
--rw-rw-rw-   0        0        0     5573 2023-03-30 20:48:18.000000 graphchem-2.1.1/graphchem/datasets/static/ron.csv
--rw-rw-rw-   0        0        0    11054 2023-03-30 20:48:18.000000 graphchem-2.1.1/graphchem/datasets/static/ysi.csv
-drwxrwxrwx   0        0        0        0 2023-04-07 23:50:15.931133 graphchem-2.1.1/graphchem/nn/
--rw-rw-rw-   0        0        0       29 2023-03-30 20:48:18.000000 graphchem-2.1.1/graphchem/nn/__init__.py
--rw-rw-rw-   0        0        0     4726 2023-04-07 23:22:25.000000 graphchem-2.1.1/graphchem/nn/gcn.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:50:15.933134 graphchem-2.1.1/graphchem/preprocessing/
--rw-rw-rw-   0        0        0       95 2023-04-01 01:45:07.000000 graphchem-2.1.1/graphchem/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     6833 2023-04-07 23:22:25.000000 graphchem-2.1.1/graphchem/preprocessing/features.py
--rw-rw-rw-   0        0        0      113 2023-04-07 23:22:25.000000 graphchem-2.1.1/graphchem/version.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:50:15.895110 graphchem-2.1.1/graphchem.egg-info/
--rw-rw-rw-   0        0        0     2956 2023-04-07 23:50:15.000000 graphchem-2.1.1/graphchem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      662 2023-04-07 23:50:15.000000 graphchem-2.1.1/graphchem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 23:50:15.000000 graphchem-2.1.1/graphchem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 23:50:15.000000 graphchem-2.1.1/graphchem.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-04-07 23:50:15.000000 graphchem-2.1.1/graphchem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-07 23:50:15.000000 graphchem-2.1.1/graphchem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 23:50:15.935133 graphchem-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1026 2023-04-07 23:22:25.000000 graphchem-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:36:54.822536 graphchem-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 02:36:42.000000 graphchem-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-01 02:36:54.822536 graphchem-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-01 02:36:42.000000 graphchem-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:36:54.818535 graphchem-2.1.2/graphchem/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:36:54.822536 graphchem-2.1.2/graphchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/data/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:36:54.822536 graphchem-2.1.2/graphchem/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/datasets/sets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:36:54.822536 graphchem-2.1.2/graphchem/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/nn/gcn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:36:54.822536 graphchem-2.1.2/graphchem/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/preprocessing/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 02:36:42.000000 graphchem-2.1.2/graphchem/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:36:54.822536 graphchem-2.1.2/graphchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-01 02:36:54.000000 graphchem-2.1.2/graphchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-01 02:36:54.000000 graphchem-2.1.2/graphchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:36:54.000000 graphchem-2.1.2/graphchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 02:36:54.000000 graphchem-2.1.2/graphchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 02:36:54.000000 graphchem-2.1.2/graphchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-01 02:36:42.000000 graphchem-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:36:54.822536 graphchem-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:36:54.822536 graphchem-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-01 02:36:42.000000 graphchem-2.1.2/tests/test_all.py
```

### Comparing `graphchem-2.1.1/LICENSE` & `graphchem-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphchem-2.1.1/PKG-INFO` & `graphchem-2.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,46 @@
-Metadata-Version: 2.1
-Name: graphchem
-Version: 2.1.1
-Summary: Graph-based models for chemical property prediction
-Home-page: https://github.com/ecrl/graphchem
-Author: Travis Kessler
-Author-email: Travis_Kessler@student.uml.edu
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![UML Energy & Combustion Research Laboratory](https://sites.uml.edu/hunter-mack/files/2021/11/ECRL_final.png)](http://faculty.uml.edu/Hunter_Mack/)
-
-# GraphChem: Graph-based machine learning for chemical property prediction
-
-[![GitHub version](https://badge.fury.io/gh/ecrl%2FGraphChem.svg)](https://badge.fury.io/gh/ecrl%2FGraphChem)
-[![PyPI version](https://badge.fury.io/py/graphchem.svg)](https://badge.fury.io/py/graphchem)
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/ecrl/GraphChem/master/LICENSE.txt)
-[![Documentation Status](https://readthedocs.org/projects/graphchem/badge/?version=latest)](https://graphchem.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://dev.azure.com/uml-ecrl/package-management/_apis/build/status%2Fecrl.graphchem?branchName=master)](https://dev.azure.com/uml-ecrl/package-management/_build/latest?definitionId=6&branchName=master)
-
-**GraphChem** is an open source Python package for constructing graph-based machine learning models with a focus on fuel property prediction. 
-
-Future plans for GraphChem include:
-- Robust hyper-parameter and model architecture tuning runtimes
-- Molecule visualization via RDKit
-
-# Installation:
-
-### Prerequisites:
-- Have Python 3.11+ installed
-
-### Method 1: pip
-```
-$ pip install graphchem
-```
-
-### Method 2: From Source
-```
-$ git clone https://github.com/ecrl/graphchem
-$ cd graphchem
-$ python setup.py install
-```
-
-If any errors occur when installing dependencies, namely with RDKit, PyTorch, or torch-geometric, visit their installation pages and follow the installation instructions: [RDKit](https://www.rdkit.org/docs/Install.html), [PyTorch](https://pytorch.org/get-started/locally/), [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html)
-
-# Usage:
-
-For advanced usage, head over to our [API documentation page](https://graphchem.readthedocs.io/en/latest/).
-
-# Examples
-
-To view some examples of how GraphChem can be used, head over to our [examples](https://github.com/ecrl/graphchem/tree/master/examples) folder on GitHub.
-
-# Contributing, Reporting Issues and Other Support:
-
-To contribute to GraphChem, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
-
-To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
-
-For additional support/questions, contact Travis Kessler (Travis_Kessler@student.uml.edu).
+[![UML Energy & Combustion Research Laboratory](https://sites.uml.edu/hunter-mack/files/2021/11/ECRL_final.png)](http://faculty.uml.edu/Hunter_Mack/)
+
+# GraphChem: Graph-based machine learning for chemical property prediction
+
+[![GitHub version](https://badge.fury.io/gh/ecrl%2FGraphChem.svg)](https://badge.fury.io/gh/ecrl%2FGraphChem)
+[![PyPI version](https://badge.fury.io/py/graphchem.svg)](https://badge.fury.io/py/graphchem)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/ecrl/GraphChem/master/LICENSE.txt)
+[![Documentation Status](https://readthedocs.org/projects/graphchem/badge/?version=latest)](https://graphchem.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://dev.azure.com/uml-ecrl/package-management/_apis/build/status%2Fecrl.graphchem?branchName=master)](https://dev.azure.com/uml-ecrl/package-management/_build/latest?definitionId=6&branchName=master)
+
+**GraphChem** is an open source Python package for constructing graph-based machine learning models with a focus on fuel property prediction.
+
+# Installation:
+
+### Prerequisites:
+- Have Python 3.11+ installed
+
+### Method 1: pip
+```
+$ pip install graphchem
+```
+
+### Method 2: From Source
+```
+$ git clone https://github.com/ecrl/graphchem
+$ cd graphchem
+$ python -m pip install .
+```
+
+If any errors occur when installing dependencies, namely with RDKit, PyTorch, or torch-geometric, visit their installation pages and follow the installation instructions: [RDKit](https://www.rdkit.org/docs/Install.html), [PyTorch](https://pytorch.org/get-started/locally/), [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html)
+
+# Usage:
+
+For advanced usage, head over to our [API documentation page](https://graphchem.readthedocs.io/en/latest/).
+
+# Examples
+
+To view some examples of how GraphChem can be used, head over to our [examples](https://github.com/ecrl/graphchem/tree/master/examples) folder on GitHub.
+
+# Contributing, Reporting Issues and Other Support:
+
+To contribute to GraphChem, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
+
+To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
+
+For additional support/questions, contact Travis Kessler (Travis_Kessler@student.uml.edu).
```

### Comparing `graphchem-2.1.1/graphchem/data/structs.py` & `graphchem-2.1.2/graphchem/data/structs.py`

 * *Files identical despite different names*

### Comparing `graphchem-2.1.1/graphchem/datasets/sets.py` & `graphchem-2.1.2/graphchem/datasets/sets.py`

 * *Files identical despite different names*

### Comparing `graphchem-2.1.1/graphchem/nn/gcn.py` & `graphchem-2.1.2/graphchem/nn/gcn.py`

 * *Files identical despite different names*

### Comparing `graphchem-2.1.1/graphchem/preprocessing/features.py` & `graphchem-2.1.2/graphchem/preprocessing/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 r"""Encoding/tokenizing SMILES strings (preparing for graph construction)"""
 
+import pickle
 from typing import List, Tuple, Union
 import rdkit
 import numpy as np
 import torch
 
 
 def get_ring_size(obj: Union['rdkit.Chem.Atom', 'rdkit.Chem.Bond'],
@@ -219,7 +220,49 @@
                 else:
                     connectivity[0, bond_index] = bond.GetEndAtomIdx()
                     connectivity[1, bond_index] = bond.GetBeginAtomIdx()
                 bond_index += 1
         connectivity = torch.from_numpy(connectivity).type(torch.long)
 
         return (enc_atoms, enc_bonds, connectivity)
+
+    def save(self, filename: str) -> None:
+        """ save the encoder to a file
+
+        Args:
+            filename (str): new filename/path for model
+
+        Returns:
+            None
+        """
+
+        with open(filename, 'wb') as outp:
+            pickle.dump(self, outp, pickle.HIGHEST_PROTOCOL)
+
+    def load(self, filename: str) -> None:
+        """ load an encoder from file (current encoder attributes, including
+        pre-trained tokenizers, are overwritten)
+
+        Args:
+            filename (str): filename/path of model
+
+        Returns:
+            None
+        """
+
+        with open(filename, 'rb') as inp:
+            self.__dict__.update(pickle.loads(inp).__dict__)
+
+
+def load_encoder(filename: str) -> MoleculeEncoder:
+    """ loads a pre-saved `MoleculeEncoder` object
+
+    Args:
+        filename (str): filename/path of saved encoder
+
+    Returns:
+        MoleculeEncoder: loaded encoder object
+    """
+
+    with open(filename, 'rb') as inp:
+        encoder = pickle.loads(inp)
+    return encoder
```

### Comparing `graphchem-2.1.1/graphchem.egg-info/PKG-INFO` & `graphchem-2.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-Metadata-Version: 2.1
-Name: graphchem
-Version: 2.1.1
-Summary: Graph-based models for chemical property prediction
-Home-page: https://github.com/ecrl/graphchem
-Author: Travis Kessler
-Author-email: Travis_Kessler@student.uml.edu
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![UML Energy & Combustion Research Laboratory](https://sites.uml.edu/hunter-mack/files/2021/11/ECRL_final.png)](http://faculty.uml.edu/Hunter_Mack/)
-
-# GraphChem: Graph-based machine learning for chemical property prediction
-
-[![GitHub version](https://badge.fury.io/gh/ecrl%2FGraphChem.svg)](https://badge.fury.io/gh/ecrl%2FGraphChem)
-[![PyPI version](https://badge.fury.io/py/graphchem.svg)](https://badge.fury.io/py/graphchem)
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/ecrl/GraphChem/master/LICENSE.txt)
-[![Documentation Status](https://readthedocs.org/projects/graphchem/badge/?version=latest)](https://graphchem.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://dev.azure.com/uml-ecrl/package-management/_apis/build/status%2Fecrl.graphchem?branchName=master)](https://dev.azure.com/uml-ecrl/package-management/_build/latest?definitionId=6&branchName=master)
-
-**GraphChem** is an open source Python package for constructing graph-based machine learning models with a focus on fuel property prediction. 
-
-Future plans for GraphChem include:
-- Robust hyper-parameter and model architecture tuning runtimes
-- Molecule visualization via RDKit
-
-# Installation:
-
-### Prerequisites:
-- Have Python 3.11+ installed
-
-### Method 1: pip
-```
-$ pip install graphchem
-```
-
-### Method 2: From Source
-```
-$ git clone https://github.com/ecrl/graphchem
-$ cd graphchem
-$ python setup.py install
-```
-
-If any errors occur when installing dependencies, namely with RDKit, PyTorch, or torch-geometric, visit their installation pages and follow the installation instructions: [RDKit](https://www.rdkit.org/docs/Install.html), [PyTorch](https://pytorch.org/get-started/locally/), [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html)
-
-# Usage:
-
-For advanced usage, head over to our [API documentation page](https://graphchem.readthedocs.io/en/latest/).
-
-# Examples
-
-To view some examples of how GraphChem can be used, head over to our [examples](https://github.com/ecrl/graphchem/tree/master/examples) folder on GitHub.
-
-# Contributing, Reporting Issues and Other Support:
-
-To contribute to GraphChem, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
-
-To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
-
-For additional support/questions, contact Travis Kessler (Travis_Kessler@student.uml.edu).
+Metadata-Version: 2.1
+Name: graphchem
+Version: 2.1.2
+Summary: Graph-based machine learning for chemical property prediction
+Author-email: Travis Kessler <travis.j.kessler@gmail.com>
+Project-URL: Homepage, https://github.com/ecrl/graphchem
+Project-URL: Bug Tracker, https://github.com/ecrl/graphchem/issues
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![UML Energy & Combustion Research Laboratory](https://sites.uml.edu/hunter-mack/files/2021/11/ECRL_final.png)](http://faculty.uml.edu/Hunter_Mack/)
+
+# GraphChem: Graph-based machine learning for chemical property prediction
+
+[![GitHub version](https://badge.fury.io/gh/ecrl%2FGraphChem.svg)](https://badge.fury.io/gh/ecrl%2FGraphChem)
+[![PyPI version](https://badge.fury.io/py/graphchem.svg)](https://badge.fury.io/py/graphchem)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/ecrl/GraphChem/master/LICENSE.txt)
+[![Documentation Status](https://readthedocs.org/projects/graphchem/badge/?version=latest)](https://graphchem.readthedocs.io/en/latest/?badge=latest)
+[![Build Status](https://dev.azure.com/uml-ecrl/package-management/_apis/build/status%2Fecrl.graphchem?branchName=master)](https://dev.azure.com/uml-ecrl/package-management/_build/latest?definitionId=6&branchName=master)
+
+**GraphChem** is an open source Python package for constructing graph-based machine learning models with a focus on fuel property prediction.
+
+# Installation:
+
+### Prerequisites:
+- Have Python 3.11+ installed
+
+### Method 1: pip
+```
+$ pip install graphchem
+```
+
+### Method 2: From Source
+```
+$ git clone https://github.com/ecrl/graphchem
+$ cd graphchem
+$ python -m pip install .
+```
+
+If any errors occur when installing dependencies, namely with RDKit, PyTorch, or torch-geometric, visit their installation pages and follow the installation instructions: [RDKit](https://www.rdkit.org/docs/Install.html), [PyTorch](https://pytorch.org/get-started/locally/), [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html)
+
+# Usage:
+
+For advanced usage, head over to our [API documentation page](https://graphchem.readthedocs.io/en/latest/).
+
+# Examples
+
+To view some examples of how GraphChem can be used, head over to our [examples](https://github.com/ecrl/graphchem/tree/master/examples) folder on GitHub.
+
+# Contributing, Reporting Issues and Other Support:
+
+To contribute to GraphChem, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
+
+To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
+
+For additional support/questions, contact Travis Kessler (Travis_Kessler@student.uml.edu).
```

