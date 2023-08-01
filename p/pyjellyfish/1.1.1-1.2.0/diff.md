# Comparing `tmp/pyjellyfish-1.1.1.tar.gz` & `tmp/pyjellyfish-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyjellyfish-1.1.1.tar", last modified: Thu Nov  3 17:40:20 2022, max compression
+gzip compressed data, was "pyjellyfish-1.2.0.tar", last modified: Tue Aug  1 00:03:40 2023, max compression
```

## Comparing `pyjellyfish-1.1.1.tar` & `pyjellyfish-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/jf/
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/jf/pkgs/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)  1123173 2021-11-17 03:06:44.000000 pyjellyfish-1.1.1/jf/pkgs/jellyfish-2.2.10.tar.gz
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)  1151287 2021-11-17 03:06:44.000000 pyjellyfish-1.1.1/jf/pkgs/jellyfish-2.3.0.tar.gz
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      174 2021-11-17 03:06:44.000000 pyjellyfish-1.1.1/jf/pkgs/links
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/pyjellyfish/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1069 2021-11-17 03:06:44.000000 pyjellyfish-1.1.1/pyjellyfish/Jellyfish.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       44 2021-11-17 03:06:44.000000 pyjellyfish-1.1.1/pyjellyfish/__init__.py
-drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/pyjellyfish.egg-info/
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     2499 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/pyjellyfish.egg-info/PKG-INFO
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      313 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/pyjellyfish.egg-info/SOURCES.txt
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)        1 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/pyjellyfish.egg-info/dependency_links.txt
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       44 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/pyjellyfish.egg-info/top_level.txt
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      338 2021-11-17 03:06:44.000000 pyjellyfish-1.1.1/.gitignore
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1472 2021-11-17 03:06:44.000000 pyjellyfish-1.1.1/LICENSE
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1709 2022-11-03 17:37:19.000000 pyjellyfish-1.1.1/README.md
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       79 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/setup.cfg
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    14442 2022-11-03 17:37:32.000000 pyjellyfish-1.1.1/setup.py
--rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     2499 2022-11-03 17:40:20.000000 pyjellyfish-1.1.1/PKG-INFO
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 00:03:40.941179 pyjellyfish-1.2.0/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1472 2021-11-17 03:06:44.000000 pyjellyfish-1.2.0/LICENSE
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     2765 2023-08-01 00:03:40.942179 pyjellyfish-1.2.0/PKG-INFO
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1955 2023-07-31 23:56:26.000000 pyjellyfish-1.2.0/README.md
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 00:03:40.826178 pyjellyfish-1.2.0/jf/
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 00:03:40.883179 pyjellyfish-1.2.0/jf/pkgs/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)  1123173 2022-11-04 18:02:42.000000 pyjellyfish-1.2.0/jf/pkgs/jellyfish-2.2.10.tar.gz
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)  1151287 2022-11-04 18:02:42.000000 pyjellyfish-1.2.0/jf/pkgs/jellyfish-2.3.0.tar.gz
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      174 2023-07-31 23:52:36.000000 pyjellyfish-1.2.0/jf/pkgs/links.txt
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 00:03:40.891179 pyjellyfish-1.2.0/pyjellyfish/
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 00:03:40.914179 pyjellyfish-1.2.0/pyjellyfish/.libs/
+-rwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)  2284232 2023-07-31 23:43:25.000000 pyjellyfish-1.2.0/pyjellyfish/.libs/libjellyfish-2.0.so.2
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     1069 2021-11-17 03:06:44.000000 pyjellyfish-1.2.0/pyjellyfish/Jellyfish.py
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       44 2021-11-17 03:06:44.000000 pyjellyfish-1.2.0/pyjellyfish/__init__.py
+drwxr-xr-x   0 feghalya  (1164) bioinfo  (16001)        0 2023-08-01 00:03:40.909179 pyjellyfish-1.2.0/pyjellyfish.egg-info/
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)     2765 2023-08-01 00:03:40.000000 pyjellyfish-1.2.0/pyjellyfish.egg-info/PKG-INFO
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      346 2023-08-01 00:03:40.000000 pyjellyfish-1.2.0/pyjellyfish.egg-info/SOURCES.txt
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)        1 2023-08-01 00:03:40.000000 pyjellyfish-1.2.0/pyjellyfish.egg-info/dependency_links.txt
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)       44 2023-08-01 00:03:40.000000 pyjellyfish-1.2.0/pyjellyfish.egg-info/top_level.txt
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)      125 2023-08-01 00:03:40.945179 pyjellyfish-1.2.0/setup.cfg
+-rw-r--r--   0 feghalya  (1164) bioinfo  (16001)    15141 2023-08-01 00:00:34.000000 pyjellyfish-1.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyjellyfish-1.1.1/jf/pkgs/jellyfish-2.2.10.tar.gz` & `pyjellyfish-1.2.0/jf/pkgs/jellyfish-2.2.10.tar.gz`

 * *Files identical despite different names*

### Comparing `pyjellyfish-1.1.1/jf/pkgs/jellyfish-2.3.0.tar.gz` & `pyjellyfish-1.2.0/jf/pkgs/jellyfish-2.3.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pyjellyfish-1.1.1/pyjellyfish/Jellyfish.py` & `pyjellyfish-1.2.0/pyjellyfish/Jellyfish.py`

 * *Files identical despite different names*

### Comparing `pyjellyfish-1.1.1/pyjellyfish.egg-info/PKG-INFO` & `pyjellyfish-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 Metadata-Version: 2.1
 Name: pyjellyfish
-Version: 1.1.1
+Version: 1.2.0
 Summary: A python wrapper around DNA k-kmer counter Jellfish
 Home-page: https://github.com/iric-soft/pyJellyfish
 Author: Albert Feghaly
 Author-email: bioinformatique@iric.ca
 License: BSD
 Keywords: k-mer DNA
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyJellyfish : Python wrapper around Jellyfish (k-mer counter)
 =============================================================
 
 [![Python version][py-image]][py-link]
 [![PyPi version][pypi-image]][pypi-link]
 
+NOTE
+----
+
+This install script is not yet PEP517 compliant, which means the
+wheel and setuptools packages *need* to be in your environment.
+
+Do not forget this line when setting up your environment (see below):
+
+``` {.sourceCode .shell}
+pip install --upgrade setuptools wheel pip
+```
+
 Introduction
 ------------
 
 This tool essentially serves as an installer for Jellyfish for use with
-Python. A small bundle of utilities is also included as a bonus.
+Python. A small bundle of utilities is also included.
 
 Citing
 ------
 
 -   Guillaume Marcais and Carl Kingsford, A fast, lock-free approach for
     efficient parallel counting of occurrences of k-mers. Bioinformatics
     (2011) 27(6): 764-770; doi:
@@ -52,33 +64,30 @@
 pip install .
 ```
 
 ### Options
 
 Additionally, pyJellyfish contains an option to manually specify which
 Jellyfish version one wishes to build against. This can be done by
-running setup.py with the the custom build command `jellyfish`.
+running setup.py with the custom build command `jellyfish`.
 
 ``` {.sourceCode .shell}
 source $HOME/.virtualenvs/km/bin/activate
 python setup.py jellyfish --version 2.2.10
 ```
 
-Note that the setup script will automatically detect if jellyfish is
-installed on your system and build against it if found. After running
-the previous commands, installation will proceed as usual, skipping the
-jellyfish installation step.
+Note that the setup script will automatically detect if jellyfish has
+already been built and use that instead of re-running the jellyfish step.
+After running the previous command, installation will proceed as usual.
 
 ``` {.sourceCode .shell}
 pip install .
 ```
 
 #### Requirements
 
 -   Python 3.6.0 or later
 
 [py-image]: https://img.shields.io/badge/python-3.6-blue.svg
 [py-link]: https://www.python.org/download/releases/3.6.0
 [pypi-image]: https://img.shields.io/pypi/v/pyjellyfish.svg
 [pypi-link]: https://pypi.python.org/pypi/pyjellyfish
-
-
```

### Comparing `pyjellyfish-1.1.1/LICENSE` & `pyjellyfish-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjellyfish-1.1.1/README.md` & `pyjellyfish-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 pyJellyfish : Python wrapper around Jellyfish (k-mer counter)
 =============================================================
 
 [![Python version][py-image]][py-link]
 [![PyPi version][pypi-image]][pypi-link]
 
+NOTE
+----
+
+This install script is not yet PEP517 compliant, which means the
+wheel and setuptools packages *need* to be in your environment.
+
+Do not forget this line when setting up your environment (see below):
+
+``` {.sourceCode .shell}
+pip install --upgrade setuptools wheel pip
+```
+
 Introduction
 ------------
 
 This tool essentially serves as an installer for Jellyfish for use with
-Python. A small bundle of utilities is also included as a bonus.
+Python. A small bundle of utilities is also included.
 
 Citing
 ------
 
 -   Guillaume Marcais and Carl Kingsford, A fast, lock-free approach for
     efficient parallel counting of occurrences of k-mers. Bioinformatics
     (2011) 27(6): 764-770; doi:
@@ -30,25 +42,24 @@
 pip install .
 ```
 
 ### Options
 
 Additionally, pyJellyfish contains an option to manually specify which
 Jellyfish version one wishes to build against. This can be done by
-running setup.py with the the custom build command `jellyfish`.
+running setup.py with the custom build command `jellyfish`.
 
 ``` {.sourceCode .shell}
 source $HOME/.virtualenvs/km/bin/activate
 python setup.py jellyfish --version 2.2.10
 ```
 
-Note that the setup script will automatically detect if jellyfish is
-installed on your system and build against it if found. After running
-the previous commands, installation will proceed as usual, skipping the
-jellyfish installation step.
+Note that the setup script will automatically detect if jellyfish has
+already been built and use that instead of re-running the jellyfish step.
+After running the previous command, installation will proceed as usual.
 
 ``` {.sourceCode .shell}
 pip install .
 ```
 
 #### Requirements
```

### Comparing `pyjellyfish-1.1.1/setup.py` & `pyjellyfish-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #!/usr/bin/env python3
 
-from setuptools import setup, find_packages, Extension
-from setuptools.command.build_py import build_py
-from setuptools.command.develop import develop
-from setuptools.command.build_ext import build_ext
-from distutils.cmd import Command
-from distutils import log
+import os
+import subprocess
+import sys
+import tarfile
 from contextlib import contextmanager
+from distutils import log
+from distutils.cmd import Command
 from distutils.errors import DistutilsOptionError
 from glob import glob
-import tarfile
-import os
-import sys
-import subprocess
+from setuptools import setup, find_packages, Extension
+from setuptools.command.build_ext import build_ext
+from setuptools.command.build_py import build_py
+from setuptools.command.develop import develop
 
 
 @contextmanager
 def pushd(dirname, makedirs=False, mode=0o777, exist_ok=False):
-    """This function was shamelessly copied from
-    https://github.com/jimporter/patchelf-wrapper/blob/master/setup.py
-    with slight modifications
+    """From: https://github.com/jimporter/patchelf-wrapper/blob/master/setup.py
     """
     old = os.getcwd()
     if makedirs and dirname is not None:
         try:
             os.makedirs(dirname, mode)
         except OSError as e:
             if ( not exist_ok or e.errno != errno.EEXIST or
@@ -37,18 +35,17 @@
         yield
     finally:
         os.chdir(old)
 
 
 class SuperCommand(Command):
     def spawn(self, cmd, cwd=None):
-        """Override spawn because we want flexible to able
+        """Override spawn because we need the flexibility to be able
         to change cwd in subprocesses.
         """
-
         with pushd(cwd):
             super().spawn(cmd)
 
 
 class JellyfishCommand(SuperCommand):
     """ Custom Jellyfish commands for compiling jellyfish. """
 
@@ -137,32 +134,32 @@
                 lib = os.path.basename(libs[0].strip().split(' ')[0])
             return lib
 
         self.mkpath(build_dir)
 
         with tarfile.open(jf_tarball, 'r:gz') as tar:
             def is_within_directory(directory, target):
-                
+
                 abs_directory = os.path.abspath(directory)
                 abs_target = os.path.abspath(target)
-            
+
                 prefix = os.path.commonprefix([abs_directory, abs_target])
-                
+
                 return prefix == abs_directory
-            
+
             def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
-            
+
                 for member in tar.getmembers():
                     member_path = os.path.join(path, member.name)
                     if not is_within_directory(path, member_path):
                         raise Exception("Attempted Path Traversal in Tar File")
-            
-                tar.extractall(path, members, numeric_owner=numeric_owner) 
-                
-            
+
+                tar.extractall(path, members, numeric_owner=numeric_owner)
+
+
             safe_extract(tar, "./jf/build")
 
         self.spawn(
             ['./configure', '--prefix', prefix],
             #['./configure', '--prefix', prefix, '--enable-python-binding'],
             # --enable-python-binding will install jellyfish.py in addition
             # to dna_jellyfish module without passing through pip which
@@ -213,49 +210,56 @@
             self.copy_file(
                 os.path.join('./jf/lib', get_lib_name()),
                 os.path.join('./pyjellyfish/.libs', get_lib_name())
             )
 
             if found_patchelf:
                 pass
+
             elif sys.prefix == sys.base_prefix:
-                # not in a virtual environment
-                # a handy hack for install bin and lib in a costum
+                # not in a virtual environment;
+                # a handy hack for installing bin and lib in a custom
                 # environment when not using venv (not recommended):
                 # https://stackoverflow.com/a/29103053/16653409
+
                 self.spawn(
                     [
                         'env',
                         'PYTHONUSERBASE=%s' % os.path.abspath('./jf'),
                         sys.executable, '-m', 'pip',
                         'install',
                         'patchelf-wrapper',
                         '--user',
                         '--upgrade',
                         '--no-cache-dir',
                         '--force'
                     ]
                 )
+
             else:
-                # in a virtual environment
+                # in a virtual environment;
+                # looks like there is no native way for pip to specify a target
+                # build directory: https://github.com/pypa/pip/issues/3934,
+                # defaulting to a simple mv command (this is quite dirty and
+                # leaves artifcats such as $VIRTUAL_ENV/share/doc/patchelf and
+                # $VIRTUAL_ENV/share/man/man1/patchelf.1 which is not ideal)
+
                 self.spawn(
                     [
                         sys.executable, '-m', 'pip',
                         'install',
                         'patchelf-wrapper',
                         '--target', lib_path,
                         '--upgrade',
                         '--no-cache-dir',
                         '--force'
                     ]
                 )
 
-                # looks like there is no native way for pip to specify a target
-                # build directory: https://github.com/pypa/pip/issues/3934,
-                # defaulting to a simple mv command
+
                 self.move_file(
                     os.path.join(os.path.dirname(sys.executable), 'patchelf'),
                     './jf/bin/'
                 )
 
             self.spawn(
                 [
@@ -310,18 +314,22 @@
     def build_extension(self, ext):
         ext_dest = self.get_ext_fullpath(ext.name)
         self.mkpath(os.path.dirname(ext_dest))
         ext_loc = os.path.join(os.getcwd(), os.path.basename(ext_dest))
         if os.path.isfile(ext_loc):
             self.copy_file(ext_loc, ext_dest)
         else:
+            log.warn(
+                "file %s (for extension %s) not found",
+                os.path.basename(ext_loc),
+                ext.name
+            )
             raise DistutilsOptionError('Cannot find extension %s' % ext_loc)
 
 
-
 # Ideally, this class would be a Singleton, but that would be
 # unnecessary for our purposes here.  A great Singleton implementation
 # can be found here: https://stackoverflow.com/a/7346105/16653409
 #@Singleton
 class ClassFactory(object):
     def __init__(self):
         self.classes = {}
@@ -335,30 +343,44 @@
 
     def create(self, parents):
 
         class CustomCommand(*parents):
             """Custom setuptools.command command."""
 
             def run(self):
-                # this assert just makes sure that don't need to manually
-                # set binary distribution to True by following the same method
-                # as this answer: https://stackoverflow.com/a/24793171/16653409
+                # this assert verifies that we don't need to set binary
+                # distribution to True as per this stackoverflow answer:
+                # https://stackoverflow.com/a/24793171/16653409
                 assert self.distribution.has_ext_modules()
+
                 self.expand_sub_commands()
                 for cmd_name in self.get_sub_commands():
                     self.run_command(cmd_name)
                 super(CustomCommand, self).run()
 
             def has_absent_jellyfish(self):
-                """Returns true if jellyfish is not installed."""
+                """Returns true if jellyfish is not installed.
+
+                Also makes sure the imported jellyfish is the one
+                built in the installation repo and not a pre-installed
+                version in python's libraries folder making sure a
+                _dna_jellyfish extension module exists, otherwise a
+                DistutilsOptionError will be raised.
+                """
+
                 try:
                     import dna_jellyfish
-                    return False
-                except (ModuleNotFoundError, ImportError):
-                    return True
+                    jf_loc = os.path.abspath(dna_jellyfish.__file__)
+                    cur_loc = os.path.abspath(os.getcwd())
+                    if os.path.dirname(jf_loc) == cur_loc:
+                        return False
+                except ModuleNotFoundError:
+                    pass
+
+                return True
 
             def expand_sub_commands(self):
                 if self.add_sub_cmd not in self.sub_commands:
                     self.sub_commands.insert(0, self.add_sub_cmd)
 
             add_sub_cmd = ('jellyfish', has_absent_jellyfish)
 
@@ -402,15 +424,15 @@
     'Programming Language :: Python :: 3.6',
 
     'Natural Language :: English',
 ]
 
 metadata = dict(
     name='pyjellyfish',
-    version='1.1.1',
+    version='1.2.0',
     description='A python wrapper around DNA k-kmer counter Jellfish',
     long_description=long_description,
     url='https://github.com/iric-soft/pyJellyfish',
     author='Albert Feghaly',
     author_email='bioinformatique@iric.ca',
     license='BSD',
     classifiers=classifiers,
```

### Comparing `pyjellyfish-1.1.1/PKG-INFO` & `pyjellyfish-1.2.0/pyjellyfish.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 Metadata-Version: 2.1
 Name: pyjellyfish
-Version: 1.1.1
+Version: 1.2.0
 Summary: A python wrapper around DNA k-kmer counter Jellfish
 Home-page: https://github.com/iric-soft/pyJellyfish
 Author: Albert Feghaly
 Author-email: bioinformatique@iric.ca
 License: BSD
 Keywords: k-mer DNA
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyJellyfish : Python wrapper around Jellyfish (k-mer counter)
 =============================================================
 
 [![Python version][py-image]][py-link]
 [![PyPi version][pypi-image]][pypi-link]
 
+NOTE
+----
+
+This install script is not yet PEP517 compliant, which means the
+wheel and setuptools packages *need* to be in your environment.
+
+Do not forget this line when setting up your environment (see below):
+
+``` {.sourceCode .shell}
+pip install --upgrade setuptools wheel pip
+```
+
 Introduction
 ------------
 
 This tool essentially serves as an installer for Jellyfish for use with
-Python. A small bundle of utilities is also included as a bonus.
+Python. A small bundle of utilities is also included.
 
 Citing
 ------
 
 -   Guillaume Marcais and Carl Kingsford, A fast, lock-free approach for
     efficient parallel counting of occurrences of k-mers. Bioinformatics
     (2011) 27(6): 764-770; doi:
@@ -52,33 +64,30 @@
 pip install .
 ```
 
 ### Options
 
 Additionally, pyJellyfish contains an option to manually specify which
 Jellyfish version one wishes to build against. This can be done by
-running setup.py with the the custom build command `jellyfish`.
+running setup.py with the custom build command `jellyfish`.
 
 ``` {.sourceCode .shell}
 source $HOME/.virtualenvs/km/bin/activate
 python setup.py jellyfish --version 2.2.10
 ```
 
-Note that the setup script will automatically detect if jellyfish is
-installed on your system and build against it if found. After running
-the previous commands, installation will proceed as usual, skipping the
-jellyfish installation step.
+Note that the setup script will automatically detect if jellyfish has
+already been built and use that instead of re-running the jellyfish step.
+After running the previous command, installation will proceed as usual.
 
 ``` {.sourceCode .shell}
 pip install .
 ```
 
 #### Requirements
 
 -   Python 3.6.0 or later
 
 [py-image]: https://img.shields.io/badge/python-3.6-blue.svg
 [py-link]: https://www.python.org/download/releases/3.6.0
 [pypi-image]: https://img.shields.io/pypi/v/pyjellyfish.svg
 [pypi-link]: https://pypi.python.org/pypi/pyjellyfish
-
-
```

