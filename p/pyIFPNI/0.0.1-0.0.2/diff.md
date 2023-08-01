# Comparing `tmp/pyIFPNI-0.0.1.tar.gz` & `tmp/pyIFPNI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyIFPNI-0.0.1.tar", last modified: Tue Aug  1 04:12:02 2023, max compression
+gzip compressed data, was "pyIFPNI-0.0.2.tar", last modified: Tue Aug  1 07:56:18 2023, max compression
```

## Comparing `pyIFPNI-0.0.1.tar` & `pyIFPNI-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 04:12:02.397009 pyIFPNI-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-08-01 04:06:37.000000 pyIFPNI-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      470 2023-08-01 04:12:02.377829 pyIFPNI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-08-01 04:07:30.000000 pyIFPNI-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 04:12:02.377829 pyIFPNI-0.0.1/pyIFPNI.egg-info/
--rw-rw-rw-   0        0        0      470 2023-08-01 04:12:02.000000 pyIFPNI-0.0.1/pyIFPNI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-01 04:12:02.000000 pyIFPNI-0.0.1/pyIFPNI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 04:12:02.000000 pyIFPNI-0.0.1/pyIFPNI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 04:12:02.000000 pyIFPNI-0.0.1/pyIFPNI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 04:12:02.377829 pyIFPNI-0.0.1/pyifpni/
--rw-rw-rw-   0        0        0       27 2023-08-01 04:08:14.000000 pyIFPNI-0.0.1/pyifpni/__init__.py
--rw-rw-rw-   0        0        0    25252 2023-08-01 03:16:53.000000 pyIFPNI-0.0.1/pyifpni/pyifpni.py
--rw-rw-rw-   0        0        0       42 2023-08-01 04:12:02.397009 pyIFPNI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-08-01 04:01:53.000000 pyIFPNI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:56:18.774368 pyIFPNI-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-08-01 04:06:37.000000 pyIFPNI-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-08-01 07:56:18.773369 pyIFPNI-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-08-01 04:07:30.000000 pyIFPNI-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 07:56:18.771369 pyIFPNI-0.0.2/pyIFPNI.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-08-01 07:56:18.000000 pyIFPNI-0.0.2/pyIFPNI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-01 07:56:18.000000 pyIFPNI-0.0.2/pyIFPNI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:56:18.000000 pyIFPNI-0.0.2/pyIFPNI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 07:56:18.000000 pyIFPNI-0.0.2/pyIFPNI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 07:56:18.772370 pyIFPNI-0.0.2/pyifpni/
+-rw-rw-rw-   0        0        0       47 2023-08-01 07:52:23.000000 pyIFPNI-0.0.2/pyifpni/__init__.py
+-rw-rw-rw-   0        0        0    25248 2023-08-01 07:51:09.000000 pyIFPNI-0.0.2/pyifpni/pyifpni.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:56:18.774368 pyIFPNI-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-08-01 07:52:34.000000 pyIFPNI-0.0.2/setup.py
```

### Comparing `pyIFPNI-0.0.1/LICENSE` & `pyIFPNI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyIFPNI-0.0.1/pyifpni/pyifpni.py` & `pyIFPNI-0.0.2/pyifpni/pyifpni.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 
 
-class pyIFPNI:
+class IFPNI:
     def __init__(self):
         self.url_base = "http://ifpni.org/"
         self.url_end = ".htm?formIndex=def&submitForm=Search&isExtended=1"
         self.lists_lists = {"name": "name",
                             "supragenus": "supragenus",
                             "genus": "genus",
                             "infragenus": "infragenus",
@@ -380,12 +380,12 @@
                 res = requests.get(url, headers=self.headers)
                 return res
             except:
                 time.sleep(5)
 
 
 if __name__ == "__main__":
-    pyifpni = pyIFPNI()
+    pyifpni = IFPNI()
     # pyifpni.supragenus("Orchidaceae", save_to_csv="orchiaceae")
     # pyifpni.genus("mahonia")
     # pyifpni.species("achlys")
     pyifpni.species("mahonia", save_to_csv="mahonia speices")
```

### Comparing `pyIFPNI-0.0.1/setup.py` & `pyIFPNI-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyIFPNI",
-    version="0.0.1",
+    version="0.0.2",
     author="Bailong Zhao",
     author_email="bailongzhao@163.com",
     description="A package accessing to IFPNI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WDragon101/pyIFPNI",
     packages=setuptools.find_packages(),
```

