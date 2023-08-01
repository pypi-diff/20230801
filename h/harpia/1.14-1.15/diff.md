# Comparing `tmp/harpia-1.14.tar.gz` & `tmp/harpia-1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.14.tar", last modified: Tue Aug  1 05:59:34 2023, max compression
+gzip compressed data, was "harpia-1.15.tar", last modified: Tue Aug  1 06:58:50 2023, max compression
```

## Comparing `harpia-1.14.tar` & `harpia-1.15.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 05:59:34.010968 harpia-1.14/
--rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.14/LICENSE
--rw-rw-rw-   0        0        0      554 2023-08-01 05:59:34.009970 harpia-1.14/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.14/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 05:59:33.919677 harpia-1.14/harpia/
--rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.14/harpia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:59:33.939863 harpia-1.14/harpia/tropomi/
--rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.14/harpia/tropomi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:59:33.945278 harpia-1.14/harpia/tropomi/no2/
--rw-rw-rw-   0        0        0     1145 2023-07-31 04:21:05.000000 harpia-1.14/harpia/tropomi/no2/__init__.py
--rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.14/harpia/tropomi/no2/converter.py
--rw-rw-rw-   0        0        0     3189 2023-08-01 04:23:57.000000 harpia-1.14/harpia/tropomi/no2/cp_completion.py
--rw-rw-rw-   0        0        0     3155 2023-08-01 05:23:46.000000 harpia-1.14/harpia/tropomi/no2/kriging.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:59:33.915689 harpia-1.14/harpia/tropomi/no2/lib/
-drwxrwxrwx   0        0        0        0 2023-08-01 05:59:33.951262 harpia-1.14/harpia/tropomi/no2/lib/random_missing_indices/
--rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.14/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
-drwxrwxrwx   0        0        0        0 2023-08-01 05:59:34.008973 harpia-1.14/harpia/tropomi/no2/lib/raster_templates/
--rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
--rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
--rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
--rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
--rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
--rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.14/harpia/tropomi/no2/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:59:33.938868 harpia-1.14/harpia.egg-info/
--rw-rw-rw-   0        0        0      554 2023-08-01 05:59:33.000000 harpia-1.14/harpia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-08-01 05:59:33.000000 harpia-1.14/harpia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 05:59:33.000000 harpia-1.14/harpia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-01 05:59:33.000000 harpia-1.14/harpia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-01 05:59:33.000000 harpia-1.14/harpia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 05:59:34.010968 harpia-1.14/setup.cfg
--rw-rw-rw-   0        0        0     2226 2023-08-01 05:58:39.000000 harpia-1.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:58:50.394457 harpia-1.15/
+-rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.15/LICENSE
+-rw-rw-rw-   0        0        0      554 2023-08-01 06:58:50.394457 harpia-1.15/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.15/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 06:58:50.326611 harpia-1.15/harpia/
+-rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.15/harpia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:58:50.336016 harpia-1.15/harpia/tropomi/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.15/harpia/tropomi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:58:50.346518 harpia-1.15/harpia/tropomi/no2/
+-rw-rw-rw-   0        0        0     1216 2023-08-01 06:57:57.000000 harpia-1.15/harpia/tropomi/no2/__init__.py
+-rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.15/harpia/tropomi/no2/converter.py
+-rw-rw-rw-   0        0        0     3189 2023-08-01 04:23:57.000000 harpia-1.15/harpia/tropomi/no2/cp_completion.py
+-rw-rw-rw-   0        0        0     3155 2023-08-01 05:23:46.000000 harpia-1.15/harpia/tropomi/no2/kriging.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:58:50.323619 harpia-1.15/harpia/tropomi/no2/lib/
+drwxrwxrwx   0        0        0        0 2023-08-01 06:58:50.347514 harpia-1.15/harpia/tropomi/no2/lib/random_missing_indices/
+-rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.15/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
+drwxrwxrwx   0        0        0        0 2023-08-01 06:58:50.392955 harpia-1.15/harpia/tropomi/no2/lib/raster_templates/
+-rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
+-rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
+-rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
+-rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
+-rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
+-rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.15/harpia/tropomi/no2/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 06:58:50.335043 harpia-1.15/harpia.egg-info/
+-rw-rw-rw-   0        0        0      554 2023-08-01 06:58:50.000000 harpia-1.15/harpia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-08-01 06:58:50.000000 harpia-1.15/harpia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 06:58:50.000000 harpia-1.15/harpia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-01 06:58:50.000000 harpia-1.15/harpia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 06:58:50.000000 harpia-1.15/harpia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 06:58:50.395494 harpia-1.15/setup.cfg
+-rw-rw-rw-   0        0        0     2226 2023-08-01 06:58:18.000000 harpia-1.15/setup.py
```

### Comparing `harpia-1.14/LICENSE` & `harpia-1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.14/PKG-INFO` & `harpia-1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.14
+Version: 1.15
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.14/harpia/__init__.py` & `harpia-1.15/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/__init__.py` & `harpia-1.15/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/__init__.py` & `harpia-1.15/harpia/tropomi/no2/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
 SOFTWARE.
 '''
 
 from . import converter
-
+from . import utils
+from . import cp_completion
+from . import kriging
```

### Comparing `harpia-1.14/harpia/tropomi/no2/converter.py` & `harpia-1.15/harpia/tropomi/no2/converter.py`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/cp_completion.py` & `harpia-1.15/harpia/tropomi/no2/cp_completion.py`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/kriging.py` & `harpia-1.15/harpia/tropomi/no2/kriging.py`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy` & `harpia-1.15/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif` & `harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif` & `harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif` & `harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif` & `harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif` & `harpia-1.15/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia/tropomi/no2/utils.py` & `harpia-1.15/harpia/tropomi/no2/utils.py`

 * *Files identical despite different names*

### Comparing `harpia-1.14/harpia.egg-info/PKG-INFO` & `harpia-1.15/harpia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.14
+Version: 1.15
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.14/harpia.egg-info/SOURCES.txt` & `harpia-1.15/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.14/setup.py` & `harpia-1.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.14",
+    version="1.15",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```

