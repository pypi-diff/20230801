# Comparing `tmp/ni_measurementlink_generator-1.1.0.dev2.tar.gz` & `tmp/ni_measurementlink_generator-1.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_generator-1.1.0.dev2.tar", max compression
+gzip compressed data, was "ni_measurementlink_generator-1.2.0.dev0.tar", max compression
```

## Comparing `ni_measurementlink_generator-1.1.0.dev2.tar` & `ni_measurementlink_generator-1.2.0.dev0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      593 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/README.md
--rw-r--r--   0        0        0      148 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/__main__.py
--rw-r--r--   0        0        0        0 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/py.typed
--rw-r--r--   0        0        0     5671 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/template.py
--rw-r--r--   0        0        0    10343 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/_helpers.py.mako
--rw-r--r--   0        0        0     1690 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.measproj.mako
--rw-r--r--   0        0        0     5143 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.measui.mako
--rw-r--r--   0        0        0     1472 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.py.mako
--rw-r--r--   0        0        0      341 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
--rw-r--r--   0        0        0      241 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/start.bat.mako
--rw-r--r--   0        0        0     1602 2023-06-26 21:36:36.225855 ni_measurementlink_generator-1.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev2/setup.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0      623 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/README.md
+-rw-r--r--   0        0        0      148 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/py.typed
+-rw-r--r--   0        0        0     6470 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/template.py
+-rw-r--r--   0        0        0    10343 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/_helpers.py.mako
+-rw-r--r--   0        0        0     1690 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/measurement.measproj.mako
+-rw-r--r--   0        0        0     5143 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/measurement.measui.mako
+-rw-r--r--   0        0        0     1472 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/measurement.py.mako
+-rw-r--r--   0        0        0      815 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
+-rw-r--r--   0        0        0      241 2023-08-01 19:42:01.266704 ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/start.bat.mako
+-rw-r--r--   0        0        0     1603 2023-08-01 19:43:03.615460 ni_measurementlink_generator-1.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.2.0.dev0/setup.py
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.2.0.dev0/PKG-INFO
```

### Comparing `ni_measurementlink_generator-1.1.0.dev2/README.md` & `ni_measurementlink_generator-1.2.0.dev0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # MeasurementLink™ Code Generator for Python
 
 ---
 
 ## Introduction
 
-MeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a tool for generating measurement plugins.
+MeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a
+tool for generating reusable measurement plug-ins using gRPC services.
 
 For installation and usage, see [MeasurementLink Support for Python (`ni-measurementlink-service`)](https://pypi.org/project/ni-measurementlink-service/).
 
 ---
 
 ## Dependencies
```

### Comparing `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/template.py` & `ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utilizes command line args to create a measurement using template files."""
 import logging
 import pathlib
 import re
-from typing import Optional
+from typing import Optional, Tuple
 
 import click
 from mako import exceptions
 from mako.template import Template
 
 _logger = logging.getLogger(__name__)
 
@@ -90,37 +90,62 @@
 )
 @click.option(
     "-s",
     "--service-class",
     help="Service Class that the measurement belongs to. Default: '<display_name>_Python'",
 )
 @click.option(
+    "-D",
+    "--description",
+    default="",
+    help="Short description of the measurement",
+)
+@click.option(
     "-d",
     "--description-url",
     default="",
     help="Description URL that links to a web page containing information about the measurement.",
 )
 @click.option(
     "-o",
     "--directory-out",
     help="Output directory for measurement files. Default: '<current_directory>/<display_name>'",
 )
 @click.option(
+    "-c",
+    "--collection",
+    default="",
+    help="\b\nThe collection that this measurement belongs to. Collection names are specified"
+    "using a period-delimited namespace hierarchy and are case-insensitive."
+    "\nExample: 'CurrentTests.Inrush'",
+)
+@click.option(
+    "-t",
+    "--tags",
+    default=[],
+    multiple=True,
+    help="\b\nTags describing the measurement. This option may be repeated to specify multiple tags. Tags are case-insensitive."
+    "\nExample: '-t test -t Internal'",
+)
+@click.option(
     "-v",
     "--verbose",
     count=True,
     help="Enable verbose logging. Repeat to increase verbosity.",
 )
 def create_measurement(
     display_name: str,
     measurement_version: str,
     ui_file: Optional[str],
     service_class: str,
     description_url: str,
     directory_out: Optional[str],
+    description: str,
+    collection: str,
+    tags: Tuple[str, ...],
     verbose: bool,
 ) -> None:
     """Generate a Python measurement service from a template.
 
     You can use this to get started writing your own MeasurementLink services.
 
     DISPLAY_NAME: The measurement display name for client to display to user.
@@ -162,14 +187,17 @@
         "measurement.serviceconfig.mako",
         serviceconfig_file,
         directory_out_path,
         display_name=display_name,
         service_class=service_class,
         description_url=description_url,
         ui_file_type=ui_file_type,
+        description=description,
+        collection=collection,
+        tags=list(tags),
     )
     if ui_file_type == "MeasurementUI":
         _create_file(
             "measurement.measui.mako",
             ui_file,
             directory_out_path,
             display_name=display_name,
```

### Comparing `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/_helpers.py.mako` & `ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/_helpers.py.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.measproj.mako` & `ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/measurement.measproj.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.measui.mako` & `ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/measurement.measui.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.py.mako` & `ni_measurementlink_generator-1.2.0.dev0/ni_measurementlink_generator/templates/measurement.py.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev2/pyproject.toml` & `ni_measurementlink_generator-1.2.0.dev0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ni_measurementlink_generator"
-version = "1.1.0-dev2"
+version = "1.2.0-dev0"
 description = "MeasurementLink Code Generator for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md"
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -49,8 +49,8 @@
 [[tool.mypy.overrides]]
 module = "mako.*"
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore tests/test_assets --strict-markers"
 filterwarnings = ["always::ImportWarning", "always::ResourceWarning"]
-testpaths = ["tests"]
+testpaths = ["tests"]
```

### Comparing `ni_measurementlink_generator-1.1.0.dev2/setup.py` & `ni_measurementlink_generator-1.2.0.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['ni-measurementlink-generator = '
                      'ni_measurementlink_generator.template:create_measurement']}
 
 setup_kwargs = {
     'name': 'ni-measurementlink-generator',
-    'version': '1.1.0.dev2',
+    'version': '1.2.0.dev0',
     'description': 'MeasurementLink Code Generator for Python',
-    'long_description': '# MeasurementLink™ Code Generator for Python\n\n---\n\n## Introduction\n\nMeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a tool for generating measurement plugins.\n\nFor installation and usage, see [MeasurementLink Support for Python (`ni-measurementlink-service`)](https://pypi.org/project/ni-measurementlink-service/).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [mako >= 1.2.1, < 2.x](https://pypi.org/project/Mako/1.2.1/)\n- [click >= 8.1.3, < 9.x](https://pypi.org/project/click/8.1.3/)\n\n---',
+    'long_description': '# MeasurementLink™ Code Generator for Python\n\n---\n\n## Introduction\n\nMeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a\ntool for generating reusable measurement plug-ins using gRPC services.\n\nFor installation and usage, see [MeasurementLink Support for Python (`ni-measurementlink-service`)](https://pypi.org/project/ni-measurementlink-service/).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [mako >= 1.2.1, < 2.x](https://pypi.org/project/Mako/1.2.1/)\n- [click >= 8.1.3, < 9.x](https://pypi.org/project/click/8.1.3/)\n\n---',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/measurementlink-python/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ni_measurementlink_generator-1.1.0.dev2/PKG-INFO` & `ni_measurementlink_generator-1.2.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ni-measurementlink-generator
-Version: 1.1.0.dev2
+Version: 1.2.0.dev0
 Summary: MeasurementLink Code Generator for Python
 Home-page: https://github.com/ni/measurementlink-python/
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,16 @@
 
 # MeasurementLink™ Code Generator for Python
 
 ---
 
 ## Introduction
 
-MeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a tool for generating measurement plugins.
+MeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a
+tool for generating reusable measurement plug-ins using gRPC services.
 
 For installation and usage, see [MeasurementLink Support for Python (`ni-measurementlink-service`)](https://pypi.org/project/ni-measurementlink-service/).
 
 ---
 
 ## Dependencies
```

