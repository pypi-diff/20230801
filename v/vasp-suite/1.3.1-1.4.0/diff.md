# Comparing `tmp/vasp_suite-1.3.1.tar.gz` & `tmp/vasp_suite-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.3.1.tar", last modified: Mon Jun 12 20:38:30 2023, max compression
+gzip compressed data, was "vasp_suite-1.4.0.tar", last modified: Tue Aug  1 13:12:33 2023, max compression
```

## Comparing `vasp_suite-1.3.1.tar` & `vasp_suite-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 20:38:30.738881 vasp_suite-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 20:38:30.737967 vasp_suite-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 20:38:30.738881 vasp_suite-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-06-12 20:38:28.000000 vasp_suite-1.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 20:38:30.737052 vasp_suite-1.3.1/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-12 20:38:28.000000 vasp_suite-1.3.1/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    16153 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5158 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/vasp_suite/core.py
--rwxrwxrwx   0 root         (0) root         (0)    19084 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     3714 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)    20919 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-12 20:37:59.000000 vasp_suite-1.3.1/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 20:38:30.737967 vasp_suite-1.3.1/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 20:38:30.000000 vasp_suite-1.3.1/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-12 20:38:30.000000 vasp_suite-1.3.1/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 20:38:30.000000 vasp_suite-1.3.1/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-12 20:38:30.000000 vasp_suite-1.3.1/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-12 20:38:30.000000 vasp_suite-1.3.1/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 20:38:30.000000 vasp_suite-1.3.1/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:12:33.681620 vasp_suite-1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:12:33.681620 vasp_suite-1.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 13:12:33.681620 vasp_suite-1.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-08-01 13:12:31.000000 vasp_suite-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:12:33.679620 vasp_suite-1.4.0/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-01 13:12:31.000000 vasp_suite-1.4.0/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18206 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    19106 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     3850 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/phonon.py
+-rw-rw-rw-   0 root         (0) root         (0)    20919 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-08-01 13:12:01.000000 vasp_suite-1.4.0/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:12:33.680620 vasp_suite-1.4.0/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 13:12:33.000000 vasp_suite-1.4.0/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.3.1/LICENSE` & `vasp_suite-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.3.1/PKG-INFO` & `vasp_suite-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.3.1
+Version: 1.4.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.3.1/README.md` & `vasp_suite-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.3.1/setup.py` & `vasp_suite-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.3.1"
+__version__ = "1.4.0"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.3.1/vasp_suite/cli.py` & `vasp_suite-1.4.0/vasp_suite/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Import argparse
 import argparse
 from textwrap import dedent
 import numpy as np
 
 # Import Modules
 from . import core
+from . import phonon
 
 # Create the wrapper funstions 
 
 def generate_input_func(args):
     '''
     Wrapper function for the generate_input function
 
@@ -255,14 +256,56 @@
     POSCAR : file 
     '''
     core.qm_region(
             filename=args.filename,
             atom=args.atom,
             )
 
+def phonon_calc(args):
+    '''
+    wrapper function for phonon calculation
+
+    parameters
+    ----------
+    supercell : list
+    mesh : list
+    encut : int
+    cores : int
+
+    Returns
+    -------
+    None
+    '''
+    supercell = args.supercell
+    mesh = args.mesh
+    encut = args.encut
+    cores = args.cores
+
+# Check if the config file exists
+    if not phonon.check_config():
+        raise ValueError('No config file found, please run the start_up command')
+
+# Generate the input files
+    # core.generate_input('POSCAR', 'phonon')
+    core.generate_kpoints(mesh=mesh)
+
+    with open('INCAR', 'a') as f:
+        f.write('ENCUT = {}\n'.format(str(encut)))
+
+# Create displacements
+    phonon.create_displacements(supercell)
+
+# get the number of displacements
+    disp = phonon.disp_files()
+
+# Generate the job file
+    job = phonon.phonopy_submit(cores, mesh)
+    job.write_submit(disp)
+
+
 def read_args(arg_list=None):
     '''Reads the command line arguments'''
     parser = argparse.ArgumentParser(
             prog='vasp_suite',
             description=dedent(
                 '''
                 ---------------------------------------------------
@@ -278,17 +321,22 @@
                     vasp_suite generate_kpoints ...
                     vasp_suite generate_supercell ...
                     vasp_suite convert_cif ...
                     vasp_suite start_up ...
                     vasp_suite dope_structure ...
                     vasp_suite generate_defect ...
                     vasp_suite molecular_qm ...
-                    vasp_suite ewald ...
                     vasp_suite plot_potential ...
                     vasp_suite qm_region ...
+                    vasp_suite phonon_calc ...
+
+                ##############################
+                ## Ewald code now found in: ##
+                ##        env_suite         ##
+                ##############################
                 '''
                 ),
             epilog=dedent(
                 '''
                 To display options for a specific programme, use vasp_suite <programme> -h
                 '''
                 ),
@@ -634,14 +682,48 @@
             )
 
     qm.add_argument(
             'atom',
             help='The name of the spin centre in the crystal, <Dy1>',
             )
 
+    phonon = subparsers.add_parser(
+            'phonon_calc',
+            help='Generate a phonopy input files and submit files',
+            formatter_class=argparse.RawDescriptionHelpFormatter
+            )
+
+    phonon.set_defaults(func=phonon_calc)
+
+    phonon.add_argument(
+            '-mesh',
+            help='The mesh to use for the phonon calculation',
+            nargs=3,
+            type=int,
+            )
+
+    phonon.add_argument(
+            '-cores',
+            help='The number of cores to use for the phonon calculation',
+            type=int,
+            )
+
+    phonon.add_argument(
+            '-encut',
+            help='The energy cutoff for the phonon calculation',
+            type=int,
+            )
+
+    phonon.add_argument(
+            '--supercell', '-s',
+            help='The supercell to use for the phonon calculation',
+            nargs=3,
+            type=int,
+            default=[1, 1, 1],
+            )
 
     # Parse the ArgumentParser
     parser.set_defaults(func=lambda args: parser.print_help())
     args = parser.parse_known_args(arg_list)
 
     # Select programme 
     if args in ['generate_input, generate_job, calculate_kpoints, generate_kpoints, generate_supercell, start_up, dope_structure, generate_defect, asymmetric_unit, ewald, plot_potential, convert_cif']:
```

### Comparing `vasp_suite-1.3.1/vasp_suite/core.py` & `vasp_suite-1.4.0/vasp_suite/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,8 +205,24 @@
 potim = 0.5
 lwave = .FALSE.
 lcharg = .FALSE.
 lorbit = 11
 gga = PE
 ivdw = 11
 ''')
+    with open('phonon.ini', 'w') as f:
+        f.write('''[Phonon]
+ALGO = Normal
+EDIFF = 1E-8
+GGA = PE
+ISIF = 2
+ISMEAR = 0
+LASPH = .TRUE.
+LCHARG = .FALSE.
+LEPSILON = .TRUE.
+LREAL = .FLASE.
+LWAVE = .FALSE.
+NSW = 0
+PREC = Accurate
+SIGMA = 0.01
+''')
     os.chdir(cwd)
```

### Comparing `vasp_suite-1.3.1/vasp_suite/ewald.py` & `vasp_suite-1.4.0/vasp_suite/ewald.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,16 @@
         # initial checks 
         a1, a2, a3 = self._s.av
         n1, n2, n3 = self._exp
         a1, a2, a3 = a1 * n1, a2 * n2, a3 * n3
         a_v = np.array([a1, a2, a3])
         min = np.linalg.norm(np.min(a_v, axis=0))
         if self._r_cut > min:
-            raise ValueError("Cutoff radius is larger than the smallest lattice vector")
+            # raise ValueError("Cutoff radius is larger than the smallest lattice vector")
+            pass
 
         # check unit cell charge
         if np.sum(self._q) != 0:
             raise ValueError("Unit cell is not charge neutral")
 
     def read_charges(self) -> None:
         '''
@@ -393,17 +394,17 @@
 
      Driving Dipole Moment
            To Zero
 
 --------------------------------
 Beginning RMS trials...
 ''')
-        rms = 2.0
+        rms = 200.0
         run = 0
-        while rms > 1:
+        while rms > 20:
             rms = self._drive_dipole()
             run += 1
             if run > 100:
                 raise ValueError('Could not drive the dipole moment to zero')
 
     def _fit_params(self):
         verbose: int = self.verbose
```

### Comparing `vasp_suite-1.3.1/vasp_suite/input.py` & `vasp_suite-1.4.0/vasp_suite/input.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,19 +55,23 @@
                     key = key.upper()
                     f.write(f'''{key} = {config[section][key]}\n''')
 
     def _POTCAR(self):
         pseudo = self.pseudopotentials
         potpaw = ['H', 'He', 'Li_sv', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na_pv', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K_sv', 'Ca_sv', 'Sc_sv', 'Ti_sv', 'V_sv', 'Cr_pv', 'Mn_pv', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga_d', 'Ge_d', 'As', 'Se', 'Br', 'Kr', 'Rb_sv', 'Sr_sv', 'Y_sv', 'Zr_sv', 'Nb_sv', 'Mo_sv', 'Tc_pv', 'Ru_pv', 'Rh_pv', 'Pd', 'Ag', 'Cd', 'In_d', 'Sn_d', 'Sb', 'Te', 'I', 'Xe', 'Cs_sv', 'Ba_sv', 'La', 'Ce_3', 'Nd_3', 'Pm_3', 'Sm_3', 'Eu_2', 'Gd_3', 'Tb_3', 'Dy_3', 'Ho_3', 'Er_3', 'Tm_3', 'Yb_2', 'Lu_3', 'Hf_pv', 'Ta_pv', 'W_sv', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl_d', 'Pb_d', 'Bi_d', 'Po_d', 'At', 'Rn', 'Fr_sv', 'Ra_sv', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm']
         atoms = self._s.atoms
-        order = list(range(len(atoms)))
 
-        files = [(x, x.split('_')) for x in potpaw if x.split('_')[0] in atoms]
-        files.sort(key=lambda x: order.index(atoms.index(x[1])))
-        files = [x[0] for x in files]
+        files = [x.split('_') for x in potpaw if x.split('_')[0] in atoms]
+        for i in range(len(atoms)):
+            for j in range(len(files)):
+                if files[j][0] == atoms[i]:
+                    files[j].append(i)
+        files.sort(key=lambda x: x[-1])
+        files = [x[:-1] for x in files]
+        files = ['_'.join(x) for x in files]
         cwd = os.getcwd()
 
         with open('POTCAR', 'w') as f:
             os.system(f'''module load vasp''')
             os.chdir(pseudo)
             for file in files:
                 os.chdir(str(file))
```

### Comparing `vasp_suite-1.3.1/vasp_suite/structure.py` & `vasp_suite-1.4.0/vasp_suite/structure.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.3.1/vasp_suite/submission.py` & `vasp_suite-1.4.0/vasp_suite/submission.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 class SubmissionWriter():
     def __init__(self, title, cores, vasp_type):
         self.title = title
         self.cores = cores
         self.vasp_type = vasp_type
         hostname = socket.gethostname() 
         if 'csf3' in hostname:
-            self.hostname = 'csf3' 
+            self.hostname = 'csf3'
         elif 'csf4' in hostname:
-            self.hostname = 'csf4' 
+            self.hostname = 'csf4'
         else:
             raise Warning('Hostname not recognised. No submission script generated.')
 
     def submission_csf3(self):
         with open('submit.sh', 'w') as f:
             if self.cores < 32:
                 f.write(f'''#!/bin/bash --login
 #$ -cwd
 #$ -pe smp.pe {self.cores}
 ''')
             else:
-                f.write(f'''#!/bin/bash --login 
-#$ -cwd 
+                f.write(f'''#!/bin/bash --login
+#$ -cwd
 #$ -pe mpi-24-ib.pe {self.cores}
 ''')
-                f.write(f'''#$ -N {self.title}
+            f.write(f'''#$ -N {self.title}
 
-module load apps/intel-19.0/vasp/5.4.4
-module load apps/binapps/anaconda3/2022.10 
+module load apps/intel-19.1/vasp/5.4.4
+module load apps/binapps/anaconda3/2022.10
 
 echo "Started running at `date`"
 
 # Run Vasp
-mpirun -np {self.cores} {self.vasp_type}
+mpirun -np {self.cores} {self.vasp_type}_par
 
 #run VASP via python script
-#python3 Opt.py 
+#python3 Opt.py
 #python3 Conv.py
 
 echo "Finished running at `date`"
 ''')
  
     def submission_csf4(self):
         with open('submit.sh', 'w') as f:
@@ -52,23 +52,21 @@
             else:
                 f.write(f'''#!/bin/bash --login
 #SBATCH -p multinode
 ''')
             f.write(f'''#SBATCH -n {self.cores}
 #SBATCH --job-name={self.title}
 
-module load vasp/5.4.4-iomkl-2020.02 
+module load vasp/5.4.4-iomkl-2020.02
 module load anaconda3/2020.07
 
-echo "Started running at `date`" 
+echo "Started running at `date`"
 
 # Run Vasp 
-mpirun -np {self.cores} {self.vasp_type}
+mpirun -np {self.cores} {self.vasp_type}_par
 
 #run VASP via python script
-#python3 Opt.py 
-#python3 Conv.py 
+#python3 Opt.py
+#python3 Conv.py
 
 echo "Finished running at `date`"
 ''')
-
-
```

### Comparing `vasp_suite-1.3.1/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.4.0/vasp_suite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.3.1
+Version: 1.4.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

