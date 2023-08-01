# Comparing `tmp/conda-package-handling-2.1.0.tar.gz` & `tmp/conda-package-handling-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-package-handling-2.1.0.tar", last modified: Fri Jul 14 13:38:01 2023, max compression
+gzip compressed data, was "conda-package-handling-2.2.0.tar", last modified: Tue Aug  1 17:57:40 2023, max compression
```

## Comparing `conda-package-handling-2.1.0.tar` & `conda-package-handling-2.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 dholth     (502) staff       (20)        0 2023-07-14 13:38:01.018216 conda-package-handling-2.1.0/
--rw-r--r--   0 dholth     (502) staff       (20)      460 2023-05-05 11:45:00.000000 conda-package-handling-2.1.0/AUTHORS.md
--rw-r--r--   0 dholth     (502) staff       (20)     1505 2022-10-07 19:55:38.000000 conda-package-handling-2.1.0/LICENSE
--rw-r--r--   0 dholth     (502) staff       (20)      126 2022-10-07 19:55:38.000000 conda-package-handling-2.1.0/MANIFEST.in
--rw-r--r--   0 dholth     (502) staff       (20)      436 2023-07-14 13:38:01.018302 conda-package-handling-2.1.0/PKG-INFO
--rw-r--r--   0 dholth     (502) staff       (20)      591 2023-01-27 16:42:52.000000 conda-package-handling-2.1.0/README.md
--rw-r--r--   0 dholth     (502) staff       (20)      124 2023-01-27 16:42:52.000000 conda-package-handling-2.1.0/pyproject.toml
--rw-r--r--   0 dholth     (502) staff       (20)      536 2023-07-14 13:38:01.018841 conda-package-handling-2.1.0/setup.cfg
--rw-r--r--   0 dholth     (502) staff       (20)     1125 2023-01-27 16:42:50.000000 conda-package-handling-2.1.0/setup.py
-drwxr-xr-x   0 dholth     (502) staff       (20)        0 2023-07-14 13:38:01.012632 conda-package-handling-2.1.0/src/
-drwxr-xr-x   0 dholth     (502) staff       (20)        0 2023-07-14 13:38:01.016926 conda-package-handling-2.1.0/src/conda_package_handling/
--rw-r--r--   0 dholth     (502) staff       (20)       22 2023-05-05 11:45:01.000000 conda-package-handling-2.1.0/src/conda_package_handling/__init__.py
--rw-r--r--   0 dholth     (502) staff       (20)       60 2022-11-17 19:45:13.000000 conda-package-handling-2.1.0/src/conda_package_handling/__main__.py
--rw-r--r--   0 dholth     (502) staff       (20)     7772 2022-12-05 13:57:09.000000 conda-package-handling-2.1.0/src/conda_package_handling/api.py
--rw-r--r--   0 dholth     (502) staff       (20)     5083 2023-01-27 16:42:50.000000 conda-package-handling-2.1.0/src/conda_package_handling/cli.py
--rw-r--r--   0 dholth     (502) staff       (20)     5187 2023-03-31 12:39:09.000000 conda-package-handling-2.1.0/src/conda_package_handling/conda_fmt.py
--rw-r--r--   0 dholth     (502) staff       (20)     1893 2023-01-27 16:42:52.000000 conda-package-handling-2.1.0/src/conda_package_handling/exceptions.py
--rw-r--r--   0 dholth     (502) staff       (20)      613 2022-11-17 19:45:13.000000 conda-package-handling-2.1.0/src/conda_package_handling/interface.py
--rw-r--r--   0 dholth     (502) staff       (20)     1412 2022-12-05 13:57:09.000000 conda-package-handling-2.1.0/src/conda_package_handling/streaming.py
--rw-r--r--   0 dholth     (502) staff       (20)     2895 2023-01-27 16:42:52.000000 conda-package-handling-2.1.0/src/conda_package_handling/tarball.py
--rw-r--r--   0 dholth     (502) staff       (20)    16707 2023-03-31 12:39:09.000000 conda-package-handling-2.1.0/src/conda_package_handling/utils.py
--rw-r--r--   0 dholth     (502) staff       (20)     3652 2023-03-31 12:39:09.000000 conda-package-handling-2.1.0/src/conda_package_handling/validate.py
-drwxr-xr-x   0 dholth     (502) staff       (20)        0 2023-07-14 13:38:01.018052 conda-package-handling-2.1.0/src/conda_package_handling.egg-info/
--rw-r--r--   0 dholth     (502) staff       (20)      436 2023-07-14 13:38:00.000000 conda-package-handling-2.1.0/src/conda_package_handling.egg-info/PKG-INFO
--rw-r--r--   0 dholth     (502) staff       (20)      796 2023-07-14 13:38:00.000000 conda-package-handling-2.1.0/src/conda_package_handling.egg-info/SOURCES.txt
--rw-r--r--   0 dholth     (502) staff       (20)        1 2023-07-14 13:38:00.000000 conda-package-handling-2.1.0/src/conda_package_handling.egg-info/dependency_links.txt
--rw-r--r--   0 dholth     (502) staff       (20)       56 2023-07-14 13:38:00.000000 conda-package-handling-2.1.0/src/conda_package_handling.egg-info/entry_points.txt
--rw-r--r--   0 dholth     (502) staff       (20)      145 2023-07-14 13:38:00.000000 conda-package-handling-2.1.0/src/conda_package_handling.egg-info/requires.txt
--rw-r--r--   0 dholth     (502) staff       (20)       23 2023-07-14 13:38:00.000000 conda-package-handling-2.1.0/src/conda_package_handling.egg-info/top_level.txt
+drwxr-xr-x   0 dholth     (502) wheel        (0)        0 2023-08-01 17:57:40.082779 conda-package-handling-2.2.0/
+-rw-r--r--   0 dholth     (502) wheel        (0)      460 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/AUTHORS.md
+-rw-r--r--   0 dholth     (502) wheel        (0)     1505 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/LICENSE
+-rw-r--r--   0 dholth     (502) wheel        (0)      126 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/MANIFEST.in
+-rw-r--r--   0 dholth     (502) wheel        (0)     1245 2023-08-01 17:57:40.082896 conda-package-handling-2.2.0/PKG-INFO
+-rw-r--r--   0 dholth     (502) wheel        (0)      767 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/README.md
+-rw-r--r--   0 dholth     (502) wheel        (0)      124 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/pyproject.toml
+-rw-r--r--   0 dholth     (502) wheel        (0)      536 2023-08-01 17:57:40.083211 conda-package-handling-2.2.0/setup.cfg
+-rw-r--r--   0 dholth     (502) wheel        (0)     1224 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/setup.py
+drwxr-xr-x   0 dholth     (502) wheel        (0)        0 2023-08-01 17:57:40.077704 conda-package-handling-2.2.0/src/
+drwxr-xr-x   0 dholth     (502) wheel        (0)        0 2023-08-01 17:57:40.081479 conda-package-handling-2.2.0/src/conda_package_handling/
+-rw-r--r--   0 dholth     (502) wheel        (0)       22 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/__init__.py
+-rw-r--r--   0 dholth     (502) wheel        (0)       60 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/__main__.py
+-rw-r--r--   0 dholth     (502) wheel        (0)     7772 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/api.py
+-rw-r--r--   0 dholth     (502) wheel        (0)     5083 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/cli.py
+-rw-r--r--   0 dholth     (502) wheel        (0)     5187 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/conda_fmt.py
+-rw-r--r--   0 dholth     (502) wheel        (0)     1893 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/exceptions.py
+-rw-r--r--   0 dholth     (502) wheel        (0)      613 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/interface.py
+-rw-r--r--   0 dholth     (502) wheel        (0)     1412 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/streaming.py
+-rw-r--r--   0 dholth     (502) wheel        (0)     2895 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/tarball.py
+-rw-r--r--   0 dholth     (502) wheel        (0)    16707 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/utils.py
+-rw-r--r--   0 dholth     (502) wheel        (0)     3652 2023-08-01 17:57:29.000000 conda-package-handling-2.2.0/src/conda_package_handling/validate.py
+drwxr-xr-x   0 dholth     (502) wheel        (0)        0 2023-08-01 17:57:40.082601 conda-package-handling-2.2.0/src/conda_package_handling.egg-info/
+-rw-r--r--   0 dholth     (502) wheel        (0)     1245 2023-08-01 17:57:40.000000 conda-package-handling-2.2.0/src/conda_package_handling.egg-info/PKG-INFO
+-rw-r--r--   0 dholth     (502) wheel        (0)      796 2023-08-01 17:57:40.000000 conda-package-handling-2.2.0/src/conda_package_handling.egg-info/SOURCES.txt
+-rw-r--r--   0 dholth     (502) wheel        (0)        1 2023-08-01 17:57:40.000000 conda-package-handling-2.2.0/src/conda_package_handling.egg-info/dependency_links.txt
+-rw-r--r--   0 dholth     (502) wheel        (0)       56 2023-08-01 17:57:40.000000 conda-package-handling-2.2.0/src/conda_package_handling.egg-info/entry_points.txt
+-rw-r--r--   0 dholth     (502) wheel        (0)      145 2023-08-01 17:57:40.000000 conda-package-handling-2.2.0/src/conda_package_handling.egg-info/requires.txt
+-rw-r--r--   0 dholth     (502) wheel        (0)       23 2023-08-01 17:57:40.000000 conda-package-handling-2.2.0/src/conda_package_handling.egg-info/top_level.txt
```

### Comparing `conda-package-handling-2.1.0/LICENSE` & `conda-package-handling-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/setup.cfg` & `conda-package-handling-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/setup.py` & `conda-package-handling-2.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 module = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(module)
 version = module.__version__
 
 setup(
     name="conda-package-handling",
     version=version,
-    description="Create and extract conda packages of various formats",
+    description="Create and extract conda packages of various formats.",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     author="Anaconda, Inc.",
     author_email="conda@anaconda.com",
     url="https://github.com/conda/conda-package-handling",
     packages=find_packages("src", exclude=["tests"]),
     package_dir={"": "src"},
     entry_points={"console_scripts": ["cph=conda_package_handling.cli:main"]},
     keywords="conda-package-handling",
     classifiers=["Programming Language :: Python :: 3"],
     python_requires=">=3.7",
-    install_requires=["conda-package-streaming >= 0.7.0"],
+    install_requires=["conda-package-streaming >= 0.9.0"],
     extras_require={
         "docs": ["furo", "sphinx", "sphinx-argparse", "myst-parser", "mdit-py-plugins>=0.3.0"],
         "test": ["mock", "pytest", "pytest-cov", "pytest-mock"],
     },
 )
```

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/api.py` & `conda-package-handling-2.2.0/src/conda_package_handling/api.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/cli.py` & `conda-package-handling-2.2.0/src/conda_package_handling/cli.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/conda_fmt.py` & `conda-package-handling-2.2.0/src/conda_package_handling/conda_fmt.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/exceptions.py` & `conda-package-handling-2.2.0/src/conda_package_handling/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/interface.py` & `conda-package-handling-2.2.0/src/conda_package_handling/interface.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/streaming.py` & `conda-package-handling-2.2.0/src/conda_package_handling/streaming.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/tarball.py` & `conda-package-handling-2.2.0/src/conda_package_handling/tarball.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/utils.py` & `conda-package-handling-2.2.0/src/conda_package_handling/utils.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling/validate.py` & `conda-package-handling-2.2.0/src/conda_package_handling/validate.py`

 * *Files identical despite different names*

### Comparing `conda-package-handling-2.1.0/src/conda_package_handling.egg-info/SOURCES.txt` & `conda-package-handling-2.2.0/src/conda_package_handling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

