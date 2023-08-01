# Comparing `tmp/WignerSymbol-0.0.5.tar.gz` & `tmp/WignerSymbol-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WignerSymbol-0.0.5.tar", last modified: Sat Jun 10 13:28:56 2023, max compression
+gzip compressed data, was "WignerSymbol-0.0.6.tar", last modified: Tue Aug  1 12:56:59 2023, max compression
```

## Comparing `WignerSymbol-0.0.5.tar` & `WignerSymbol-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 13:28:56.171567 WignerSymbol-0.0.5/
--rw-rw-rw-   0        0        0     1080 2023-06-10 12:36:47.000000 WignerSymbol-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      523 2023-06-10 13:28:56.170566 WignerSymbol-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-10 13:25:00.000000 WignerSymbol-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 13:28:56.155566 WignerSymbol-0.0.5/WignerSymbol/
--rw-rw-rw-   0        0        0    36389 2023-06-10 08:59:57.000000 WignerSymbol-0.0.5/WignerSymbol/WignerSymbol.hpp
-drwxrwxrwx   0        0        0        0 2023-06-10 13:28:56.169567 WignerSymbol-0.0.5/WignerSymbol.egg-info/
--rw-rw-rw-   0        0        0      523 2023-06-10 13:28:56.000000 WignerSymbol-0.0.5/WignerSymbol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-10 13:28:56.000000 WignerSymbol-0.0.5/WignerSymbol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 13:28:56.000000 WignerSymbol-0.0.5/WignerSymbol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-10 10:06:42.000000 WignerSymbol-0.0.5/WignerSymbol.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-10 13:28:56.000000 WignerSymbol-0.0.5/WignerSymbol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3403 2023-06-10 12:52:17.000000 WignerSymbol-0.0.5/lib.cpp
--rw-rw-rw-   0        0        0      108 2023-06-10 13:15:34.000000 WignerSymbol-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 13:28:56.171567 WignerSymbol-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-06-10 13:28:45.000000 WignerSymbol-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 12:56:59.677274 WignerSymbol-0.0.6/
+-rw-rw-rw-   0        0        0     1080 2023-06-10 12:36:47.000000 WignerSymbol-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      523 2023-08-01 12:56:59.677274 WignerSymbol-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-10 13:25:00.000000 WignerSymbol-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 12:56:59.676274 WignerSymbol-0.0.6/WignerSymbol.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-08-01 12:56:59.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-08-01 12:56:59.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 12:56:59.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-01 12:56:58.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-08-01 12:56:59.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3403 2023-06-10 12:52:17.000000 WignerSymbol-0.0.6/lib.cpp
+-rw-rw-rw-   0        0        0      108 2023-06-10 13:15:34.000000 WignerSymbol-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 12:56:59.678277 WignerSymbol-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      925 2023-08-01 12:49:53.000000 WignerSymbol-0.0.6/setup.py
```

### Comparing `WignerSymbol-0.0.5/LICENSE` & `WignerSymbol-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `WignerSymbol-0.0.5/PKG-INFO` & `WignerSymbol-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WignerSymbol
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python port of 0382/WignerSymbol
 Home-page: https://github.com/0382/WignerSymbol-pybind11
 Author: 0382
 Author-email: 18322825326@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `WignerSymbol-0.0.5/WignerSymbol.egg-info/PKG-INFO` & `WignerSymbol-0.0.6/WignerSymbol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WignerSymbol
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python port of 0382/WignerSymbol
 Home-page: https://github.com/0382/WignerSymbol-pybind11
 Author: 0382
 Author-email: 18322825326@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `WignerSymbol-0.0.5/lib.cpp` & `WignerSymbol-0.0.6/lib.cpp`

 * *Files identical despite different names*

### Comparing `WignerSymbol-0.0.5/setup.py` & `WignerSymbol-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 from pathlib import Path
 
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 ext_modules = [
     Pybind11Extension("WignerSymbol",
                       ["lib.cpp"],
-                      define_macros=[("VERSION", __version__)]
+                      define_macros=[("VERSION", __version__)],
+                      include_dirs=[this_dir],
                       ),
 ]
 
 setup(
     name='WignerSymbol',
     version=__version__,
     author="0382",
```

