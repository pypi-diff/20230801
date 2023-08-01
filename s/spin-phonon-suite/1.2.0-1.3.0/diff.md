# Comparing `tmp/spin_phonon_suite-1.2.0.tar.gz` & `tmp/spin_phonon_suite-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin_phonon_suite-1.2.0.tar", last modified: Fri Jun  9 11:27:02 2023, max compression
+gzip compressed data, was "spin_phonon_suite-1.3.0.tar", last modified: Tue Aug  1 12:59:22 2023, max compression
```

## Comparing `spin_phonon_suite-1.2.0.tar` & `spin_phonon_suite-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:02.067175 spin_phonon_suite-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    35085 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3750 2023-06-09 11:27:02.066186 spin_phonon_suite-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3031 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 11:27:02.067175 spin_phonon_suite-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-06-09 11:26:59.000000 spin_phonon_suite-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:02.065197 spin_phonon_suite-1.2.0/spin_phonon_suite/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-09 11:26:59.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    10850 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/cells.py
--rw-rw-rw-   0 root         (0) root         (0)    34732 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/derivative.py
--rw-rw-rw-   0 root         (0) root         (0)    22303 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/lvc.py
--rw-rw-rw-   0 root         (0) root         (0)    18786 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/vibrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:02.066186 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3750 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      493 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:59:22.185824 spin_phonon_suite-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35085 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-08-01 12:59:22.185824 spin_phonon_suite-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 12:59:22.185824 spin_phonon_suite-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-08-01 12:59:19.000000 spin_phonon_suite-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:59:22.183990 spin_phonon_suite-1.3.0/spin_phonon_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 12:59:19.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10806 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/cells.py
+-rw-rw-rw-   0 root         (0) root         (0)    34976 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)    22303 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/lvc.py
+-rw-rw-rw-   0 root         (0) root         (0)    18786 2023-08-01 12:58:46.000000 spin_phonon_suite-1.3.0/spin_phonon_suite/vibrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:59:22.184907 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      159 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-01 12:59:22.000000 spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/top_level.txt
```

### Comparing `spin_phonon_suite-1.2.0/LICENSE` & `spin_phonon_suite-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.2.0/PKG-INFO` & `spin_phonon_suite-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin_phonon_suite
-Version: 1.2.0
+Version: 1.3.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-1.2.0/README.md` & `spin_phonon_suite-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.2.0/setup.py` & `spin_phonon_suite-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 setuptools.setup(
     name='spin_phonon_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian', # noqa
```

### Comparing `spin_phonon_suite-1.2.0/spin_phonon_suite/cells.py` & `spin_phonon_suite-1.3.0/spin_phonon_suite/cells.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,26 +110,26 @@
 
     mappings = [[equivalent_positions[idx] for idx in shift_dict]
                 for shift_dict in indices]
 
     return equivalent_positions, elements, mappings, molecules
 
 
-def build_cluster(poscar, central_index=None, distortion_expansion=None,
+def build_cluster(poscar, central_idc=None, distortion_expansion=None,
                   distortion_expansion_old=None, distortion_cutoff=None):
 
     if distortion_expansion is not None:
         cluster = DistortionSupercell.from_poscar(
-            poscar, distortion_expansion, central_index=central_index)
+            poscar, distortion_expansion, central_idc=central_idc)
     elif distortion_expansion_old is not None:
         cluster = DistortionSupercellOld.from_poscar(
-            poscar, distortion_expansion_old, central_index=central_index)
+            poscar, distortion_expansion_old, central_idc=central_idc)
     elif distortion_cutoff is not None:
         cluster = DistortionCluster.from_poscar(
-            poscar, distortion_cutoff, central_index=central_index)
+            poscar, distortion_cutoff, central_idc=central_idc)
     else:
         ValueError("Invalid cluster specification!")
 
     return cluster
 
 
 class DistortionExpansion:
@@ -150,36 +150,39 @@
     Attributes
     ----------
     expansion : list[int]
         Expansion used to generate supercell from cell e.g. [3, 3, 3]
     uc_sc_map : list
         Mapping of supercell atoms onto unit cell atoms
     """
-    def __init__(self, lat_vecs, coords, atom_numbers, *args, **kwargs):
+    def __init__(self, lat_vecs, coords, atom_numbers, center, *args, **kwargs):
 
         self.lat_vecs = lat_vecs
-        self.coords = self.recenter_unitcell(coords, *args)
+        self.coords = self.recenter_unitcell(coords, center, *args)
         self.atom_numbers = atom_numbers
 
         self.cart_coords = self.generate_cluster(*args)
         self.frac_coords = self.cart_coords @ la.inv(self.lat_vecs)
         self.n_atoms = len(atom_numbers)
         self.n_cell = self.frac_coords.shape[0] // self.coords.shape[0]
 
     @classmethod
-    def from_poscar(cls, poscar_name, *args, central_index=None):
+    def from_poscar(cls, poscar_name, *args, central_idc=None, center=None):
         atoms = read_vasp(poscar_name)
 
-        if central_index is None:
-            coords = atoms.scaled_positions
+        coords = atoms.scaled_positions
+
+        if center is not None:
+            center = center
+        elif central_idc is not None:
+            center = np.mean(coords[list(central_idc)], axis=0)
         else:
-            shift = atoms.scaled_positions[central_index - 1]
-            coords = (atoms.scaled_positions - shift) % 1.
+            center = None
 
-        return cls(atoms.cell, coords, atoms.numbers, *args)
+        return cls(atoms.cell, coords, atoms.numbers, center, *args)
 
     def generate_cluster(self, *args):
 
         def shift_coords(idc):
             return (self.coords + np.array(idc)) @ self.lat_vecs
 
         coords = np.array([coord for idc in self.generate_cell_idc(*args)
@@ -204,31 +207,28 @@
     def generate_cell_idc(self, expansion, central_index):
         for nvec in product(*map(range, reversed(expansion))):
             # reverse ordering of product
             yield tuple(reversed(nvec))
 
     def recenter_cluster(self, cart, expansion, central_index):
 
-        # _lat_vecs = self.lat_vecs * np.array(expansion)[:, np.newaxis]
-        center = np.array(expansion) @ self.lat_vecs / 2
-
         frac = cart @ la.inv(self.lat_vecs)
         frac += np.array(expansion) / 2 - frac[central_index]
         frac %= np.array(expansion)
 
         cart = frac @ self.lat_vecs
 
         return cart - cart[central_index]
 
     @classmethod
-    def from_poscar(cls, poscar_name, *args, central_index=None):
+    def from_poscar(cls, poscar_name, *args, central_indices=None):
         atoms = read_vasp(poscar_name)
         coords = atoms.scaled_positions
 
-        return cls(atoms.cell, coords, atoms.numbers, *args, central_index - 1)
+        return cls(atoms.cell, coords, atoms.numbers, *args, central_indices[0])
 
 
 class DistortionSupercell(DistortionExpansion):
 
     def generate_cell_idc(self, expansion):
 
         def expansion_range(num):
@@ -249,23 +249,23 @@
             if num % 2 == 0:  # even
                 return 0.0
             elif num % 2 == 1:  # odd
                 return vec / 2
 
         return cart - np.sum(list(map(shift, expansion, self.lat_vecs)), axis=0)
 
-    def recenter_unitcell(self, frac, expansion):
+    def recenter_unitcell(self, frac, center, expansion):
 
         def shift(num):
             if num % 2 == 0:  # even
                 return 0.0
             elif num % 2 == 1:  # odd
                 return 1 / 2
 
-        return (frac + np.array(list(map(shift, expansion)))) % 1.0
+        return (frac - center + np.array(list(map(shift, expansion)))) % 1.0
 
 
 class DistortionCluster(DistortionExpansion):
 
     def generate_cell_idc(self, cutoff):
 
         def expansion_range(vec):
@@ -278,16 +278,16 @@
 
             if np.linalg.norm(r) <= cutoff:
                 yield nvec
 
     def recenter_cluster(self, cart, *args):
         return cart - np.sum(self.lat_vecs, axis=0) / 2
 
-    def recenter_unitcell(self, frac, *args):
-        return (frac + 1 / 2) % 1.0
+    def recenter_unitcell(self, frac, center, *args):
+        return (frac - center + 1 / 2) % 1.0
 
 
 def write_molcas_basis(labels, charge_dict, name):
     """
     Writes dummy molcas basis file for environment charges to a textfile named
     according to the basis name.
```

### Comparing `spin_phonon_suite-1.2.0/spin_phonon_suite/cli.py` & `spin_phonon_suite-1.3.0/spin_phonon_suite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,18 @@
 def str_int(x):
     try:
         return int(x)
     except ValueError:
         return str(x)
 
 
+def parse_index(x):
+    return int(x) - 1
+
+
 def lvc_func(args):
 
     if args.add is not None:
         def join(a, b):
             return a.join(b, xyzp.load_xyz(args.reference_xyz)[1] * ANG2BOHR)
         lvc = reduce(join, (LVC.from_file(f_lvc) for f_lvc in args.add))
 
@@ -140,15 +144,15 @@
             args.poscar,
             args.force_sets,
             ext_masses=args.mass,
             trans=args.trans,
             distortion_expansion=args.distortion_expansion,
             distortion_expansion_old=args.distortion_expansion_old,
             distortion_cutoff=args.distortion_cutoff,
-            central_index=args.central_index,
+            central_idc=args.central_index,
             force_expansion=args.force_expansion,
             q_mesh=args.q_mesh
         )
 
     elif args.phonopy_hdf5:
 
         if args.mass:
@@ -408,31 +412,37 @@
     print("Molcas basis set file for environment written to:")
     print("     ENV (basis set specification)\033[0m")
 
 
 def cluster_func(args):
 
     structure = Structure.from_file(args.poscar)
-    central_index = args.central_index
-    central_index_unit = (central_index - 1) % structure.num_sites
-    central_site = structure.sites[central_index_unit]
+    central_idc = args.central_index
 
-    if args.from_central:
-        molecular_graph = cells.generate_molecular_graph(structure)
+    molecular_graph = cells.generate_molecular_graph(structure)
+
+    def generate_qm_region(idx):
         connected_graphs = cells.split_molecular_graph(molecular_graph, filter_unique=False)
-        central_graph = next(filter(lambda nodes: central_index_unit in nodes, connected_graphs))
-        _, qm_region = cells.extract_molecule(structure, central_graph, central_index=central_index_unit)
+        central_graph = next(filter(lambda nodes: idx in nodes, connected_graphs))
+        _, qm_region = cells.extract_molecule(structure, central_graph, central_index=idx)
+        central_site = structure.sites[idx]
         shift = np.array([central_site.x, central_site.y, central_site.z])
+        return qm_region, shift
+
+    if args.from_central:
+        qm_regions, shifts = zip(*map(generate_qm_region, central_idc))
+        qm_region = Molecule.from_sites([site for mol in qm_regions for site in mol.sites])
+        shift = np.mean(shifts, axis=0)
     elif args.qm_region is not None:
         qm_region = Molecule.from_file(args.qm_region)
         shift = np.zeros(3)
     else:
         raise NotImplementedError()
 
-    cluster = cells.build_cluster(args.poscar, central_index=central_index,
+    cluster = cells.build_cluster(args.poscar, central_idc=central_idc,
                                   distortion_expansion=args.distortion_expansion,
                                   distortion_expansion_old=args.distortion_expansion_old,
                                   distortion_cutoff=args.distortion_cutoff)
 
     def format_label(args):
         idx, specie = args
         return f"{specie.symbol}.ENV.{idx}"
@@ -655,16 +665,17 @@
     '--distortion_cutoff',
     type=float,
     help='Cut-off distance for unit cell cluster.'
 )
 
 cluster.add_argument(
     '--central_index',
-    type=int,
-    help='Index of the central spin center.'
+    type=parse_index,
+    nargs='+',
+    help='Index of the central spin center or list of atomic indices.'
 )
 
 
 def read_args(arg_list=None):
     description = '''
     A package for performing Spin-Phonon coupling calculations.
     '''
```

### Comparing `spin_phonon_suite-1.2.0/spin_phonon_suite/derivative.py` & `spin_phonon_suite-1.3.0/spin_phonon_suite/derivative.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.2.0/spin_phonon_suite/lvc.py` & `spin_phonon_suite-1.3.0/spin_phonon_suite/lvc.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.2.0/spin_phonon_suite/vibrations.py` & `spin_phonon_suite-1.3.0/spin_phonon_suite/vibrations.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/PKG-INFO` & `spin_phonon_suite-1.3.0/spin_phonon_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-phonon-suite
-Version: 1.2.0
+Version: 1.3.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

