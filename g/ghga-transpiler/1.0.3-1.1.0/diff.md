# Comparing `tmp/ghga_transpiler-1.0.3.tar.gz` & `tmp/ghga_transpiler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_transpiler-1.0.3.tar", last modified: Tue Jun 20 20:13:18 2023, max compression
+gzip compressed data, was "ghga_transpiler-1.1.0.tar", last modified: Tue Aug  1 12:11:41 2023, max compression
```

## Comparing `ghga_transpiler-1.0.3.tar` & `ghga_transpiler-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/ghga_transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/ghga_transpiler/config/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/config/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/ghga_transpiler/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/configs/0.10.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/ghga_transpiler/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/ghga_transpiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-20 20:13:18.000000 ghga_transpiler-1.0.3/ghga_transpiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-20 20:13:18.000000 ghga_transpiler-1.0.3/ghga_transpiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:13:18.000000 ghga_transpiler-1.0.3/ghga_transpiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 20:13:18.000000 ghga_transpiler-1.0.3/ghga_transpiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:13:17.000000 ghga_transpiler-1.0.3/ghga_transpiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 20:13:18.000000 ghga_transpiler-1.0.3/ghga_transpiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 20:13:18.000000 ghga_transpiler-1.0.3/ghga_transpiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 20:13:18.150952 ghga_transpiler-1.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/tests/fixtures/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/fixtures/configs/0.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/fixtures/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:13:18.146952 ghga_transpiler-1.0.3/tests/fixtures/test_data_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/fixtures/test_data_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/fixtures/test_data_objects/conversion_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/test_convert_workbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/test_create_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-20 20:13:04.000000 ghga_transpiler-1.0.3/tests/test_process_workbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.411802 ghga_transpiler-1.1.0/ghga_transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.411802 ghga_transpiler-1.1.0/ghga_transpiler/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/config/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.411802 ghga_transpiler-1.1.0/ghga_transpiler/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/configs/0.10.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/configs/1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/ghga_transpiler/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.411802 ghga_transpiler-1.1.0/ghga_transpiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-08-01 12:11:41.000000 ghga_transpiler-1.1.0/ghga_transpiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-01 12:11:41.000000 ghga_transpiler-1.1.0/ghga_transpiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:11:41.000000 ghga_transpiler-1.1.0/ghga_transpiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 12:11:41.000000 ghga_transpiler-1.1.0/ghga_transpiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:11:41.000000 ghga_transpiler-1.1.0/ghga_transpiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 12:11:41.000000 ghga_transpiler-1.1.0/ghga_transpiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 12:11:41.000000 ghga_transpiler-1.1.0/ghga_transpiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/get_package_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/license_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/scripts/script_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/script_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/script_utils/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1461 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/update_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/update_config_docs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6789 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/update_readme.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/scripts/update_template_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/tests/fixtures/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/fixtures/configs/0.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/fixtures/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:11:41.415802 ghga_transpiler-1.1.0/tests/fixtures/test_data_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/fixtures/test_data_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/fixtures/test_data_objects/conversion_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/test_convert_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/test_create_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-01 12:11:31.000000 ghga_transpiler-1.1.0/tests/test_process_workbook.py
```

### Comparing `ghga_transpiler-1.0.3/LICENSE` & `ghga_transpiler-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/PKG-INFO` & `ghga_transpiler-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_transpiler
-Version: 1.0.3
+Version: 1.1.0
 Summary: GHGA-Transpiler - GHGA metadata XLSX to JSON transpilation
 Home-page: https://github.com/ghga-de/ghga-transpiler
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_transpiler-1.0.3/README.md` & `ghga_transpiler-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/__init__.py` & `ghga_transpiler-1.1.0/ghga_transpiler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Short description of package"""  # Please adapt to package
 
-__version__ = "1.0.3"
+__version__ = "1.1.0"
```

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/__main__.py` & `ghga_transpiler-1.1.0/ghga_transpiler/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/cli.py` & `ghga_transpiler-1.1.0/ghga_transpiler/cli.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/config/__init__.py` & `ghga_transpiler-1.1.0/ghga_transpiler/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/config/config.py` & `ghga_transpiler-1.1.0/ghga_transpiler/config/config.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/config/exceptions.py` & `ghga_transpiler-1.1.0/ghga_transpiler/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/configs/0.10.0.yaml` & `ghga_transpiler-1.1.0/ghga_transpiler/configs/0.10.0.yaml`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/configs/__init__.py` & `ghga_transpiler-1.1.0/ghga_transpiler/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/core.py` & `ghga_transpiler-1.1.0/ghga_transpiler/core.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/io.py` & `ghga_transpiler-1.1.0/ghga_transpiler/io.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler/transformations.py` & `ghga_transpiler-1.1.0/ghga_transpiler/transformations.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/ghga_transpiler.egg-info/PKG-INFO` & `ghga_transpiler-1.1.0/ghga_transpiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-transpiler
-Version: 1.0.3
+Version: 1.1.0
 Summary: GHGA-Transpiler - GHGA metadata XLSX to JSON transpilation
 Home-page: https://github.com/ghga-de/ghga-transpiler
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_transpiler-1.0.3/setup.cfg` & `ghga_transpiler-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/setup.py` & `ghga_transpiler-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/fixtures/__init__.py` & `ghga_transpiler-1.1.0/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/fixtures/configs/__init__.py` & `ghga_transpiler-1.1.0/tests/fixtures/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/fixtures/test_data_objects/__init__.py` & `ghga_transpiler-1.1.0/tests/fixtures/test_data_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/fixtures/test_data_objects/conversion_data.py` & `ghga_transpiler-1.1.0/tests/fixtures/test_data_objects/conversion_data.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/fixtures/utils.py` & `ghga_transpiler-1.1.0/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/test_convert_workbook.py` & `ghga_transpiler-1.1.0/tests/test_convert_workbook.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/test_create_config.py` & `ghga_transpiler-1.1.0/tests/test_create_config.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/test_io.py` & `ghga_transpiler-1.1.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.3/tests/test_process_workbook.py` & `ghga_transpiler-1.1.0/tests/test_process_workbook.py`

 * *Files identical despite different names*

