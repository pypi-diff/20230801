# Comparing `tmp/fmriprep_docker-23.1.3.tar.gz` & `tmp/fmriprep_docker-23.1.4.tar.gz`

## Comparing `fmriprep_docker-23.1.3.tar` & `fmriprep_docker-23.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/.flake8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/src/fmriprep_docker/__init__.py
--rwxr-xr-x   0        0        0    18982 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/src/fmriprep_docker/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/src/fmriprep_docker/_version.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/LICENSE
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/README.rst
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/pyproject.toml
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/.flake8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/src/fmriprep_docker/__init__.py
+-rwxr-xr-x   0        0        0    18982 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/src/fmriprep_docker/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/src/fmriprep_docker/_version.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/LICENSE
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/README.rst
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 fmriprep_docker-23.1.4/PKG-INFO
```

### Comparing `fmriprep_docker-23.1.3/src/fmriprep_docker/__main__.py` & `fmriprep_docker-23.1.4/src/fmriprep_docker/__main__.py`

 * *Files identical despite different names*

### Comparing `fmriprep_docker-23.1.3/.gitignore` & `fmriprep_docker-23.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fmriprep_docker-23.1.3/LICENSE` & `fmriprep_docker-23.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fmriprep_docker-23.1.3/README.rst` & `fmriprep_docker-23.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `fmriprep_docker-23.1.3/pyproject.toml` & `fmriprep_docker-23.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fmriprep_docker-23.1.3/PKG-INFO` & `fmriprep_docker-23.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmriprep-docker
-Version: 23.1.3
+Version: 23.1.4
 Summary: A wrapper for generating Docker commands using regular fMRIPrep syntax
 Project-URL: Homepage, https://github.com/nipreps/fmriprep
 Project-URL: Documentation, https://fmriprep.org
 Project-URL: Paper, https://doi.org/10.1038/s41592-018-0235-4
 Project-URL: Docker Images, https://hub.docker.com/r/nipreps/fmriprep/tags/
 Project-URL: NiPreps, https://www.nipreps.org/
 Author-email: The NiPreps Developers <nipreps@gmail.com>
```

