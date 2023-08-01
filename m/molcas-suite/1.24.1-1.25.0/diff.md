# Comparing `tmp/molcas_suite-1.24.1.tar.gz` & `tmp/molcas_suite-1.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcas_suite-1.24.1.tar", last modified: Thu Jul  6 08:40:29 2023, max compression
+gzip compressed data, was "molcas_suite-1.25.0.tar", last modified: Tue Aug  1 14:15:08 2023, max compression
```

## Comparing `molcas_suite-1.24.1.tar` & `molcas_suite-1.25.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:40:29.601597 molcas_suite-1.24.1/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3618 2023-07-06 08:40:29.601597 molcas_suite-1.24.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2952 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:40:29.599597 molcas_suite-1.24.1/molcas_suite/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-06 08:40:27.000000 molcas_suite-1.24.1/molcas_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     6311 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/barrier.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/cfp.py
--rw-rw-rw-   0 root         (0) root         (0)    28336 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    31919 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    18799 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/generate_input.py
--rw-rw-rw-   0 root         (0) root         (0)    25262 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/generate_job.py
--rw-rw-rw-   0 root         (0) root         (0)     6356 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/h5tools.py
--rw-rw-rw-   0 root         (0) root         (0)    21698 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/molcas_suite/orbs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:40:29.601597 molcas_suite-1.24.1/molcas_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3618 2023-07-06 08:40:29.000000 molcas_suite-1.24.1/molcas_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-06 08:40:29.000000 molcas_suite-1.24.1/molcas_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 08:40:29.000000 molcas_suite-1.24.1/molcas_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-06 08:40:29.000000 molcas_suite-1.24.1/molcas_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-06 08:40:29.000000 molcas_suite-1.24.1/molcas_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 08:40:29.000000 molcas_suite-1.24.1/molcas_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-06 08:40:15.000000 molcas_suite-1.24.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 08:40:29.601597 molcas_suite-1.24.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2023-07-06 08:40:27.000000 molcas_suite-1.24.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:15:08.955541 molcas_suite-1.25.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-08-01 14:15:08.955541 molcas_suite-1.25.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:15:08.953541 molcas_suite-1.25.0/molcas_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-08-01 14:15:06.000000 molcas_suite-1.25.0/molcas_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/barrier.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/cfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    28559 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    34861 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    18445 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/generate_input.py
+-rw-rw-rw-   0 root         (0) root         (0)    25262 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/generate_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     6356 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/h5tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    21698 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/molcas_suite/orbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 14:15:08.954541 molcas_suite-1.25.0/molcas_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-08-01 14:15:08.000000 molcas_suite-1.25.0/molcas_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      507 2023-08-01 14:15:08.000000 molcas_suite-1.25.0/molcas_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 14:15:08.000000 molcas_suite-1.25.0/molcas_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-08-01 14:15:08.000000 molcas_suite-1.25.0/molcas_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-08-01 14:15:08.000000 molcas_suite-1.25.0/molcas_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 14:15:08.000000 molcas_suite-1.25.0/molcas_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-08-01 14:14:48.000000 molcas_suite-1.25.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 14:15:08.955541 molcas_suite-1.25.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2023-08-01 14:15:06.000000 molcas_suite-1.25.0/setup.py
```

### Comparing `molcas_suite-1.24.1/LICENSE` & `molcas_suite-1.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.24.1/PKG-INFO` & `molcas_suite-1.25.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.24.1
+Version: 1.25.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.24.1/README.md` & `molcas_suite-1.25.0/README.md`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.24.1/molcas_suite/barrier.py` & `molcas_suite-1.25.0/molcas_suite/barrier.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.24.1/molcas_suite/cfp.py` & `molcas_suite-1.25.0/molcas_suite/cfp.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.24.1/molcas_suite/cli.py` & `molcas_suite-1.25.0/molcas_suite/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,14 +780,22 @@
         '--timestamp',
         nargs='+',
         action=OrderedSelectionAction,
         choices=extractor.MOLCAS_PRGS,
         help=('extract timestamp of specified modules (by order)')
     )
 
+    extract.add_argument(
+        '--orbitals',
+        nargs='+',
+        action=OrderedSelectionAction,
+        choices=["ener", "occ", "coef"],
+        help='Extract orbital information from the RASSCF section.',
+    )
+
     # Barrier figure
 
     barrier = subparsers.add_parser(
         'barrier',
         description="""
         Creates barrier figure of lowest lying J multiplet.
         Transition probabilities are given by magnetic moment operator.
```

### Comparing `molcas_suite-1.24.1/molcas_suite/extractor.py` & `molcas_suite-1.25.0/molcas_suite/extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains functions for extracting data from molcas output and
 hdf5 files
 """
 import re
 from functools import reduce
+from itertools import count
 import mmap
 import h5py
 import numpy as np
 from hpc_suite.store import RegexExtractor, H5AttrExtractor, H5Extractor, \
         Int, Cmplx, is_hdf5
 # from scipy.optimize.optimize import _line_search_wolfe12
 
@@ -58,15 +59,18 @@
 
     # plain text output extractors
     txt_extractors = {
         ("gradients", None): (ExtractAlaska, {'item': "gradients"}),
         ("rasscf", "energies"): (ExtractRASSCF, {'item': "energies"}),
         ("rasscf", "epot"): (ExtractRASSCFProperty, {'item': "epot"}),
         ("rasscf", "efld"): (ExtractRASSCFProperty, {'item': "efld"}),
-        ("rasscf", "fldg"): (ExtractRASSCFProperty, {'item': "fldg"})
+        ("rasscf", "fldg"): (ExtractRASSCFProperty, {'item': "fldg"}),
+        ("orbitals", "ener"): (ExtractRASSCFOrbitals, {'item': "orb_ener"}),
+        ("orbitals", "occ"): (ExtractRASSCFOrbitals, {'item': "orb_occ"}),
+        ("orbitals", "coef"): (ExtractRASSCFOrbitals, {'item': "orb_coef"})
     }
 
     # SINGLE_ANISO extractors
     txt_extractors.update({
         **{("quax", basis): (ExtractQUAX, {'basis': basis})
            for basis in ['l', 'j', 'zeeman']},
         **{("cfp", basis): (ExtractCFPs, {'basis': basis})
@@ -852,15 +856,16 @@
         txt_file : str
             Molcas text output file
         item : {'energies'}
             Item name
         """
 
         args = {
-            "energies": ("energies", "RASSCF root energies")
+            "energies": ("energies", "RASSCF root energies"),
+            "orbital_coefficients": ("orbital_coefficients", "Orbital coefficient matrix")
         }
 
         fmt = {
             "energies": '% .8f'
         }
 
         super().__init__("rasscf", txt_file, *args[item], label=label,
@@ -973,7 +978,79 @@
                 data = self.format_data(
                     re.findall(self.row_pattern.encode(), named_root["array"]))
 
                 # generate label
                 label = self.format_label(**named, **named_root)
 
                 yield (label, data)
+
+
+class ExtractRASSCFOrbitals(MolcasExtractor):
+
+    def __init__(self, txt_file, item, label="occurrence", units='au', fmt='% .4f'):
+
+        """
+        Parameters
+        ----------
+        txt_file : str
+            Molcas text output file
+        item : {'energies'}
+            Item name
+        """
+
+        title, description = {
+            "orb_ener": ("orbital_energies", "Orbital energies"),
+            "orb_occ": ("orbital_occupations", "Orbital occupations"),
+            "orb_coef": ("orbital_coefficients", "Orbital coefficients")
+        }[item]
+
+        super().__init__("rasscf", txt_file, title, description, label=label,
+                         units=units, fmt=fmt)
+
+        # \s*- to deal with concatentated negative 4 digit energies
+        row_patterns = {
+            "orb_ener": r"(?:Energy((?:\s*-?\d+\.\d+)+))",
+            "orb_occ": r"(?:Occ\. No\.((?:\s+\d\.\d+)+))",
+            "orb_coef": r"(?:\d+ \w+\s+[A-Za-z0-9+-]+((?:\s+\-?\d\.\d+)+))"
+        }
+
+        self.item = item
+        self.row_pattern = row_patterns[item]
+
+        self.array_pattern = "\s+".join([
+            r"Orbital(?:\s+\d+\s+)+",
+            rf"{row_patterns['orb_ener']}",
+            rf"{row_patterns['orb_occ']}",
+            rf"(?:{row_patterns['orb_coef']}\s+)+"])
+
+    def __iter__(self):
+
+        counter = count(1)
+
+        header = "Molecular orbitals for symmetry species 1: a"
+        block_pattern = header + rf"\s+(?:{self.array_pattern})+"
+
+        with open(self.txt_file, 'rb') as f:
+            # use mmap to buffer file contents
+            # as a result, search pattern has to be encoded to byte string
+            content = mmap.mmap(f.fileno(), 0, prot=mmap.PROT_READ)
+            it = re.finditer(self.sec_pattern.encode(), content)
+
+        def array_iter(block):
+            for array in re.finditer(self.array_pattern.encode(), block):
+                lines = re.findall(self.row_pattern.encode(), array.group(0))
+                yield list(map(lambda x: re.findall(r"(-?\d+\.\d+)".encode(), x), lines))
+
+        def block_iter(m):
+            for block in re.finditer(block_pattern.encode(), m.group()):
+                data = [[elem for line in lines for elem in line]
+                        for lines in zip(*array_iter(block.group()))]
+                return data
+
+        for m in it:
+            yield self.format_label(counter=counter), self.format_data(block_iter(m))
+
+    def format_data(self, data):
+        if self.item in ["orb_occ", "orb_ener"]:
+            return np.array(data, dtype=float)[0, :]
+
+        return np.array(data, dtype=float)
```

### Comparing `molcas_suite-1.24.1/molcas_suite/generate_input.py` & `molcas_suite-1.25.0/molcas_suite/generate_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -377,34 +377,29 @@
         warnings.warn("Encountered large number of RasOrb files.")
 
     rasscf_sections = [[
         Casscf(n_active_elec, n_active_orb if i == 1 else None,
                None if i == 1 else "Typeindex",
                *rasscf_extra[0], Spin=spin, Charge=charge,
                FILEORB=initial_orb if i == 1 else f"{i-1:d}.RasOrb",
-               CiRoot=f"{root} {root} 1", ORBA="FULL", MAXORB=str(root),
+               CiRoot=f"{root} {root} 1", ORBA="FULL", MAXORB="1",
                **rasscf_extra[1]),
         Emil("Copy", "$Project.JobIph", f"{i:d}_IPH"),
         Emil("Copy", "$Project.RasOrb", f"{i:d}.RasOrb"),
         Emil("Copy", "$Project.rasscf.h5", f"{i:d}.rasscf.h5"),
-        *([Emil("FOREACH", "ROOT", "in", "(1..{:d})".format(
-            root if max_orb is None or root < max_orb else max_orb)),
-          Emil("Shell", "mv", "$Project.RasOrb.$ROOT", f"{i:d}.RasOrb.$ROOT"),
-          Emil("Shell", "mv", "$Project.SpdOrb.$ROOT", f"{i:d}.SpdOrb.$ROOT"),
-          Emil("ENDDO")] if extract_orbs else []),
         Emil("EXEC", "molcas_suite orbs", f"{i:d}.rasscf.h5 --out {i:d}_rasorb"),  # noqa
         *([Caspt2(roots=range(1, root+1), *caspt2_extra[0], **caspt2_extra[1]),
            Emil("Copy", "$Project.JobIph", f"{i:d}_PT2_IPH")]
           if caspt2 else [])]
         for i, (spin, root) in enumerate(zip(spin_list, root_list), start=1)]
 
     sections.extend([row for sec in rasscf_sections for row in sec])
 
     sections.append(Rassi(
-        "SPIN", "MEES", "EJob", *rassi_extra[0], EPRG="7.0D-1",
+        "SPIN", "MEES", *rassi_extra[0], EPRG="7.0D-1",
         properties=[f"'ANGMOM' {i}" for i in range(1, 4)],
         jobiph=trunc_root_list,
         **rassi_extra[1]))
 
     # Request CFPs for TM, Ln, Ac
     if 21 <= ctr_num <= 30 and n_active_orb == 5:
         crys = True
```

### Comparing `molcas_suite-1.24.1/molcas_suite/generate_job.py` & `molcas_suite-1.25.0/molcas_suite/generate_job.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.24.1/molcas_suite/h5tools.py` & `molcas_suite-1.25.0/molcas_suite/h5tools.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.24.1/molcas_suite/orbs.py` & `molcas_suite-1.25.0/molcas_suite/orbs.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.24.1/molcas_suite.egg-info/PKG-INFO` & `molcas_suite-1.25.0/molcas_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas-suite
-Version: 1.24.1
+Version: 1.25.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.24.1/setup.py` & `molcas_suite-1.25.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.24.1"
+__version__ = "1.25.0"
 
 setuptools.setup(
     name='molcas_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for dealing with OpenMOLCAS input and output files',
```

