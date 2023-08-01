# Comparing `tmp/ansys-motorcad-core-0.1.3.tar.gz` & `tmp/ansys_motorcad_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-motorcad-core-0.1.3.tar", last modified: Mon Mar 20 08:57:55 2023, max compression
+gzip compressed data, was "ansys_motorcad_core-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-motorcad-core-0.1.3.tar` & `ansys_motorcad_core-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1089 2023-03-20 08:57:42.129865 ansys-motorcad-core-0.1.3/LICENSE
--rw-r--r--   0        0        0     5917 2023-03-20 08:57:42.129865 ansys-motorcad-core-0.1.3/README.rst
--rw-r--r--   0        0        0     1758 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      342 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/__init__.py
--rw-r--r--   0        0        0     1103 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/geometry.py
--rw-r--r--   0        0        0       29 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/__init__.py
--rw-r--r--   0        0        0     3795 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_calculations.py
--rw-r--r--   0        0        0    20693 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_fea_geometry.py
--rw-r--r--   0        0        0    15967 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_general.py
--rw-r--r--   0        0        0     2776 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_geometry.py
--rw-r--r--   0        0        0     7123 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_graphs.py
--rw-r--r--   0        0        0     6775 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_internal.py
--rw-r--r--   0        0        0     1397 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_internal_scripting.py
--rw-r--r--   0        0        0     4189 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_lab.py
--rw-r--r--   0        0        0     4791 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_materials.py
--rw-r--r--   0        0        0     6718 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_thermal.py
--rw-r--r--   0        0        0     5301 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_ui.py
--rw-r--r--   0        0        0      860 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_utility.py
--rw-r--r--   0        0        0     3689 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_variables.py
--rw-r--r--   0        0        0     3471 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/motorcad_methods.py
--rw-r--r--   0        0        0    15076 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/rpc_client_core.py
--rw-r--r--   0        0        0     2078 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/rpc_methods_core.py
--rw-r--r--   0        0        0    55413 2023-03-20 08:57:42.133865 ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/rpc_methods_core_old.py
--rw-r--r--   0        0        0     7486 1970-01-01 00:00:00.000000 ansys-motorcad-core-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-08-01 10:50:04.570273 ansys_motorcad_core-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5920 2023-08-01 10:50:04.570273 ansys_motorcad_core-0.2.0/README.rst
+-rw-r--r--   0        0        0     1822 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      572 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/__init__.py
+-rw-r--r--   0        0        0     1103 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/geometry.py
+-rw-r--r--   0        0        0       29 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/__init__.py
+-rw-r--r--   0        0        0     3795 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_calculations.py
+-rw-r--r--   0        0        0    20693 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_fea_geometry.py
+-rw-r--r--   0        0        0    17666 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_general.py
+-rw-r--r--   0        0        0     2776 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_geometry.py
+-rw-r--r--   0        0        0     7123 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_graphs.py
+-rw-r--r--   0        0        0     6775 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_internal.py
+-rw-r--r--   0        0        0     1397 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_internal_scripting.py
+-rw-r--r--   0        0        0     4189 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_lab.py
+-rw-r--r--   0        0        0     4791 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_materials.py
+-rw-r--r--   0        0        0     6718 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_thermal.py
+-rw-r--r--   0        0        0     5308 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_ui.py
+-rw-r--r--   0        0        0      860 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_utility.py
+-rw-r--r--   0        0        0     3689 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_variables.py
+-rw-r--r--   0        0        0     3713 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/motorcad_methods.py
+-rw-r--r--   0        0        0    19787 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/rpc_client_core.py
+-rw-r--r--   0        0        0     2078 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/rpc_methods_core.py
+-rw-r--r--   0        0        0    55413 2023-08-01 10:50:04.574273 ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/rpc_methods_core_old.py
+-rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 ansys_motorcad_core-0.2.0/PKG-INFO
```

### Comparing `ansys-motorcad-core-0.1.3/LICENSE` & `ansys_motorcad_core-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/README.rst` & `ansys_motorcad_core-0.2.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.7-blue
-   :target: https://pypi.org/project/pymotorcad-core/
+   :target: https://pypi.org/project/ansys-motorcad-core/
    :alt: Python
 
-.. |pypi| image:: https://img.shields.io/pypi/v/pymotorcad-core.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/pymotorcad-core
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-motorcad-core.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-motorcad-core/
    :alt: PyPI
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/pymotorcad/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pymotorcad
+.. |codecov| image:: https://codecov.io/gh/ansys/pymotorcad/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/pymotorcad
    :alt: Codecov
 
-.. |GH-CI| image:: https://github.com/pyansys/pymotorcad/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pymotorcad/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pymotorcad/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pymotorcad/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
@@ -67,15 +67,15 @@
     
 To install in developer mode, complete these steps:
 
 #. Clone the ``pymotorcad`` repository with this command:
 
     .. code:: bash
 
-        git clone https://github.com/pyansys/pymotorcad
+        git clone https://github.com/ansys/pymotorcad
 
 #. Create a fresh-clean Python environment and activate it with
    these commands:
 
     .. code:: bash
 
         # Create a virtual environment
```

### Comparing `ansys-motorcad-core-0.1.3/pyproject.toml` & `ansys_motorcad_core-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name="ansys-motorcad-core"
-dynamic = ["version"]
+version = "0.2.0"
 description = "Pythonic interface to Ansys Motor-CAD."
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
-    {name = "Ansys, Inc.", email = "pyansys.support@ansys.com"},
+    {name = "Ansys, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
-    {name = "PyAnsys developers", email = "pyansys.support@ansys.com"},
+    {name = "PyAnsys developers", email = "pyansys.core@ansys.com"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
@@ -26,36 +26,38 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "psutil >= 5.9.0",
     "requests >= 2.27.1",
     "packaging >= 21.3",
+    "importlib-metadata>=4.0",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.2.1",
-    "pytest-cov==4.0.0",
+    "pytest==7.4.0",
+    "pytest-cov==4.1.0",
+    "ansys.platform.instancemanagement>=1.0.2"
 ]
 doc = [
-    "Sphinx==5.3.0",
+    "Sphinx==7.0.1",
     "numpydoc==1.5.0",
-    "ansys-sphinx-theme==0.9.5",
-    "sphinx-copybutton==0.5.1",
-    "sphinx-gallery==0.11.1",
+    "ansys-sphinx-theme==0.9.9",
+    "sphinx-copybutton==0.5.2",
+    "sphinx-gallery==0.13.0",
     "matplotlib",
     "scipy",
-    "pypandoc==1.10"
+    "pypandoc==1.11"
 ]
 
 [project.urls]
-Source = "https://github.com/pyansys/pymotorcad"
+Source = "https://github.com/ansys/pymotorcad"
 Documentation = "https://motorcad.docs.pyansys.com/"
-Tracker = "https://github.com/pyansys/pymotorcad/issues"
+Tracker = "https://github.com/ansys/pymotorcad/issues"
 
 [tool.flit.module]
 name = "ansys.motorcad.core"
 
 [tool.black]
 line-length = 100
```

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/geometry.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/geometry.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_calculations.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_calculations.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_fea_geometry.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_fea_geometry.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_general.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_general.py`

 * *Files 11% similar despite different names*

```diff
@@ -449,13 +449,54 @@
     def clear_message_log(self):
         """Clear the message log file for the model."""
         method = "ClearMessageLog"
         return self.connection.send_and_receive(method)
 
     def quit(self):
         """Quit Motor-CAD."""
-        method = "Quit"
-        return self.connection.send_and_receive(method)
+        self.connection._quit()
 
     def set_free(self):
         """Free the Motor-CAD instance."""
         return self.connection._set_free()
+
+    def download_mot_file(self, file_path):
+        """Download the current .mot file from Motor-CAD and write it to a local directory.
+
+        This allows users to download .mot files to a local directory from a Motor-CAD instance
+        on a remote machine. Equivalent of :func:`save_file` for remote machines.
+
+        Parameters
+        ----------
+        file_path : str
+            Full path to the mot file, including the file name and .mot extension.
+            Use the ``r'filepath'`` syntax to force Python to ignore special characters.
+        """
+        self.connection.ensure_version_at_least("2023.2")
+        method = "GetCurrentFileJSON"
+        file_contents = self.connection.send_and_receive(method)
+
+        with open(file_path, "w") as mot_file:
+            for line in file_contents:
+                mot_file.write(line + "\n")
+
+    def upload_mot_file(self, file_path):
+        """Upload a .mot file to Motor-CAD instance from local directory.
+
+        This allows users to send .mot files from a local directory to a Motor-CAD instance
+        on a remote machine. Equivalent of :func:`load_file` for remote machines.
+
+        Parameters
+        ----------
+        file_path : str
+            Full path to the mot file, including the file name and .mot extension.
+            Use the ``r'filepath'`` syntax to force Python to ignore special characters.
+        """
+        self.connection.ensure_version_at_least("2023.2")
+        file_contents = []
+        with open(file_path, "r") as mot_file:
+            for line in mot_file:
+                file_contents += [line.replace("\n", "")]
+
+        method = "SetCurrentFileJSON"
+        params = [file_contents]
+        self.connection.send_and_receive(method, params)
```

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_geometry.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_geometry.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_graphs.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_graphs.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_internal.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_internal.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_internal_scripting.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_internal_scripting.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_lab.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_lab.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_materials.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_materials.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_thermal.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_thermal.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_ui.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
         method = "DisableErrorMessages"
         params = [active]
         return self.connection.send_and_receive(method, params)
 
     def initialise_tab_names(self):
         """Initialize the available tabs in the Motor-CAD UI.
 
-        Call this method prior to using the ``SaveMotorCADScreenToFile`` or
-        ``DisplayScreen`` method. The Motor-CAD UI must be visible.
+        Call this method prior to using the ``save_motorcad_screen_to_file`` or
+        ``display_screen`` method. The Motor-CAD UI must be visible.
         """
         method = "InitialiseTabNames"
         return self.connection.send_and_receive(method)
 
     def save_motorcad_screen_to_file(self, screen_name, file_name):
         """Save the entire Motor-CAD screen of a tab to an image file.
 
-        Call the ``InitialiseTabNames`` method before called this method.l The
+        Call the ``initialise_tab_names`` method before called this method.l The
         Motor-CAD UI must be visible.
 
         Parameters
         ----------
         screen_name : str
             Path of the screen to save. The path must be in this format:
             ``"tabName;tabName;tabName"``. For example,
```

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_utility.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_utility.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/methods/rpc_methods_variables.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/methods/rpc_methods_variables.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/motorcad_methods.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/motorcad_methods.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,25 @@
     def __init__(
         self,
         port=-1,
         open_new_instance=True,
         enable_exceptions=True,
         enable_success_variable=False,
         reuse_parallel_instances=False,
+        url="",
+        timeout=2,
     ):
         self.connection = _MotorCADConnection(
             port,
             open_new_instance,
             enable_exceptions,
             enable_success_variable,
             reuse_parallel_instances,
+            url=url,
+            timeout=timeout,
         )
 
         _RpcMethodsCore.__init__(self, mc_connection=self.connection)
         _RpcMethodsUtility.__init__(self, mc_connection=self.connection)
 
 
 class MotorCAD(_MotorCADCore):
@@ -42,36 +46,39 @@
     enable_exceptions : Boolean, default: True
         Whether to show Motor-CAD communication errors as Python exceptions.
     enable_success_variable : Boolean, default: False
         Whether Motor-CAD methods return a success variable (first object in tuple).
     reuse_parallel_instances : Boolean, default: False
         Whether to reuse MotorCAD instances when running in parallel. You must
         free instances after use.
-
+    url: string, default = ""
+        Full url for Motor-CAD connection. Assumes we are connecting to existing instance.
     Returns
     -------
     MotorCAD object.
     """
 
     def __init__(
         self,
         port=-1,
         open_new_instance=True,
         enable_exceptions=True,
         enable_success_variable=False,
         reuse_parallel_instances=False,
+        url="",
     ):
         """Initiate MotorCAD object."""
         _MotorCADCore.__init__(
             self,
             port=port,
             open_new_instance=open_new_instance,
             enable_exceptions=enable_exceptions,
             enable_success_variable=enable_success_variable,
             reuse_parallel_instances=reuse_parallel_instances,
+            url=url,
         )
 
 
 class MotorCADCompatibility(_RpcMethodsCoreOld):
     """Create a MotorCAD object that behaves the same as old ActiveX methods.
 
     This class contains the old ``camelCase`` function names.
```

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/rpc_client_core.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/rpc_client_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,44 @@
 
 from os import environ, path
 import re
 import socket
 import subprocess
 import time
 
+from packaging import version
 import psutil
 import requests
 
+try:
+    import ansys.platform.instancemanagement as pypim
+
+    _HAS_PIM = True
+except ModuleNotFoundError:
+    _HAS_PIM = False
+
+
 DETACHED_PROCESS = 0x00000008
 CREATE_NEW_PROCESS_GROUP = 0x00000200
 
 DEFAULT_INSTANCE = -1
 
-SERVER_IP = "http://localhost"
+LOCALHOST_ADDRESS = "http://localhost"
+TRY_RESOLVE_LOCALHOST = True
+SERVER_IP = LOCALHOST_ADDRESS
 
 _METHOD_SUCCESS = 0
 
 MOTORCAD_EXE_GLOBAL = ""
 
 MOTORCAD_PROC_NAMES = ["MotorCAD", "Motor-CAD"]
 
+# Useful for debugging new functions when using debug Motor-CAD
+DONT_CHECK_MOTORCAD_VERSION = False
+
 
 def set_server_ip(ip):
     """IP address of the machine that Motor-CAD is running on."""
     global SERVER_IP
     SERVER_IP = ip
 
 
@@ -124,14 +138,16 @@
     def __init__(
         self,
         port,
         open_new_instance,
         enable_exceptions,
         enable_success_variable,
         reuse_parallel_instances,
+        url="",
+        timeout=2,
         compatibility_mode=False,
     ):
         """Create a MotorCAD object for communication.
 
         Parameters
         ----------
         port : int
@@ -143,14 +159,16 @@
         enable_success_variable: Boolean
             Whether Motor-CAD methods are to return a success variable (first object in tuple).
         reuse_parallel_instances: Boolean
             Whether to reuse MotorCAD instances when running in parallel. You must free
             instances after use.
         compatibility_mode: Boolean, default: False
             Whether to try to run an old script written for ActiveX.
+        url: string, default = ""
+            Full url for Motor-CAD connection. Assumes we are connecting to existing instance.
 
         Returns
         -------
         MotorCAD object.
         """
         self._port = -1
         self._connected = False
@@ -163,76 +181,172 @@
 
         self._open_new_instance = open_new_instance
 
         self.enable_success_variable = enable_success_variable
 
         self._compatibility_mode = compatibility_mode
 
+        self.pim_instance = None
+
+        self._url = url
+        self._timeout = timeout
+
         if DEFAULT_INSTANCE != -1:
             # Getting called from MotorCAD internal scripting so port is known
             port = DEFAULT_INSTANCE
             self._open_new_instance = False
 
         if self.reuse_parallel_instances is True:
             self._open_new_instance = False
 
-        if self._open_new_instance is True:
-            if port != -1:
-                self._port = int(port)
-
-            self._open_motor_cad_local()
-
-        else:  # (self._open_new_instance == False)
-            if port != -1:
-                self._port = int(port)
-
-            else:  # port is not defined
-                self._find_free_motor_cad()
-
-        self.pid = self.get_process_id()
+        if self._url != "":
+            # Don't want to start a Motor-CAD instance
+            # Already have full url in _get_url()
+            # Also don't want to exit Motor-CAD upon script ending
+            self._open_new_instance = False
+        elif _HAS_PIM and pypim.is_configured():
+            # Start with PyPIM if the environment is configured for it
+            self._launch_motorcad_remote()
+        else:
+            # run/connect to motor-cad on local machine
+            self._launch_motorcad_local(port)
 
         # Check for response
-        if self._wait_for_response(2) is True:
+        if self._wait_for_response(self._timeout) is True:
             self._connected = True
-            # Store Motor-CAD version number for any required backwards compatibility
 
+            # Store Motor-CAD version number for any required backwards compatibility
             self.program_version = self._get_program_version()
 
+            self.pid = self.get_process_id()
+
+            if (SERVER_IP == LOCALHOST_ADDRESS) and TRY_RESOLVE_LOCALHOST:
+                # Try to resolve localhost to speed up function calls
+                self._resolve_localhost()
+
         else:
             raise MotorCADError(
                 "Failed to connect to Motor-CAD instance: port="
                 + str(self._port)
                 + ", Url="
                 + str(self._get_url())
             )
 
+    def _resolve_localhost(self):
+        """Try to resolve localhost so that we don't have to do this for every api method.
+
+        Replace the address http://localhost with the corresponding IP address.
+        On some configurations this was increasing each api method time to 1/2 seconds.
+        """
+        global SERVER_IP
+
+        ipv6_localhost = "http://[::1]"
+        ipv4_localhost = "http://127.0.0.1"
+
+        if self._check_address_for_response(ipv6_localhost):
+            SERVER_IP = ipv6_localhost
+        elif self._check_address_for_response(ipv4_localhost):
+            SERVER_IP = ipv4_localhost
+        else:
+            SERVER_IP = LOCALHOST_ADDRESS
+
+    def _check_address_for_response(self, address):
+        """Try to communicate with Motor-CAD with specific url, returns True if response received.
+
+        Uses handshake method. Used to resolve localhost.
+        """
+        # This function is only called from _resolve_localhost so SERVER_IP will be localhost
+        # address
+        # If connecting to remote machine then SERVER_IP is deprecated - should use url class
+        # parameter instead
+        global SERVER_IP
+
+        save_SERVER_IP = SERVER_IP
+
+        try:
+            SERVER_IP = address
+            address_responds = self._wait_for_response(1)
+        finally:
+            # Reset global SERVER_IP to original
+            # Calling function can set SERVER_IP depending on address_responds return value
+            SERVER_IP = save_SERVER_IP
+
+        return address_responds
+
     def __del__(self):
         """Close Motor-CAD when MotorCAD object leaves memory."""
-        if self._connected is True:
-            if (
-                (self.reuse_parallel_instances is False)
-                and (self._open_new_instance is True)
-                and (self._compatibility_mode is False)
-            ):
-                # Close Motor-CAD if not asked to keep open
-                try:
-                    self.quit()
-                except Exception:
-                    # Don't raise exception at this point
-                    # Motor-CAD might already have been closed by user
-                    pass
+        if self._close_motorcad_on_exit():
+            try:
+                self._quit()
+            except Exception:
+                # Don't raise exception at this point
+                # Motor-CAD might already have been closed by user
+                pass
+
+    def _close_motorcad_on_exit(self):
+        """Check whether to close Motor-CAD when MotorCAD object __del__ is called."""
+        if (
+            (self.reuse_parallel_instances is False)
+            and (self._open_new_instance is True)
+            and (self._compatibility_mode is False)
+        ):
+            # Local Motor-CAD has been launched by Python
+            return True
+        elif _HAS_PIM and pypim.is_configured():
+            # Always try to close Ansys Lab instance
+            return True
+        else:
+            return False
+
+    # Close Motor-CAD if not asked to keep open
+    def _launch_motorcad_local(self, port):
+        """Launch local Motor-CAD instance."""
+        if self._open_new_instance is True:
+            if port != -1:
+                self._port = int(port)
+
+            self._open_motor_cad_local()
+
+        else:  # (self._open_new_instance == False)
+            if port != -1:
+                self._port = int(port)
+
+            else:  # port is not defined
+                self._find_free_motor_cad()
+
+    def _launch_motorcad_remote(self):
+        """Launch Motor-CAD in Ansys Lab."""
+        pim = pypim.connect()
+
+        self.pim_instance = pim.create_instance(product_name="motorcad")
+        self.pim_instance.wait_for_ready()
+        # get ip and port for motorcad
+        address = self.pim_instance.services["http"].uri
+
+        ip = address.split(":")[0] + ":" + address.split(":")[1]
+        set_server_ip(ip)
+
+        self._port = address.split(":")[2]
+
+        # Wait for Motor-CAD RPC server to start on remote machine - this might take a few minutes
+        if self._wait_for_response(300) is False:
+            raise MotorCADError("Failed to connect to Motor-CAD instance on: " + address)
 
     def _raise_if_allowed(self, error_message):
         if self.enable_exceptions is True:
             raise MotorCADError(error_message)
 
     def _get_url(self):
         """Get url for RPC communication."""
-        url = SERVER_IP + ":" + str(self._port) + "/jsonrpc"
-        return url
+        if self._url != "":
+            # Already have full url from launch params
+            return self._url + "/jsonrpc"
+        else:
+            # Create url from server ip and port
+            return SERVER_IP + ":" + str(self._port) + "/jsonrpc"
 
     def _open_motor_cad_local(self):
         self.__MotorExe = _find_motor_cad_exe()
 
         if self.__MotorExe == "":
             self._raise_if_allowed(
                 "Failed to find instance of Motor-CAD to open."
@@ -245,15 +359,15 @@
             [self.__MotorExe, "/PORT=" + str(self._port), "/SCRIPTING"]
         )
 
         pid = motor_process.pid
 
         motor_util = psutil.Process(pid)
 
-        self._wait_for_server_to_start(motor_util)
+        self._wait_for_server_to_start_local(motor_util)
 
     def _find_free_motor_cad(self):
         found_free_instance = False
         for proc in psutil.process_iter():
             proc_name = proc.name()
             if any(motor_proc_name in proc_name for motor_proc_name in MOTORCAD_PROC_NAMES):
                 port = _get_port_from_motorcad_process(proc)
@@ -283,15 +397,23 @@
                 self._open_motor_cad_local()
             else:
                 raise MotorCADError(
                     "Could not find a Motor-CAD instance to connect to."
                     + "\n Ensure that Motor-CAD RPC server is enabled."
                 )
 
-    def _wait_for_server_to_start(self, process):
+    def ensure_version_at_least(self, required_version):
+        """Check that the Motor-CAD version is later or equal to required version."""
+        if DONT_CHECK_MOTORCAD_VERSION is False:
+            if version.parse(self.program_version) < version.parse(required_version):
+                raise MotorCADError(
+                    "This function requires Motor-CAD version: " + required_version + " or later"
+                )
+
+    def _wait_for_server_to_start_local(self, process):
         number_of_tries = 0
         timeout = 300  # in seconds
         # Don't poll this too much
         pause_time = 0.5
 
         while pause_time * number_of_tries < timeout:
             port = _get_port_from_motorcad_process(process)
@@ -443,11 +565,15 @@
         Returns
         -------
         error_message : str
             Most recent error message.
         """
         return self._last_error_message
 
-    def quit(self):
+    def _quit(self):
         """Quit MotorCAD."""
-        method = "Quit"
-        return self.send_and_receive(method)
+        if self.pim_instance is not None:
+            self.pim_instance.delete()
+        else:
+            # local machine
+            method = "Quit"
+            return self.send_and_receive(method)
```

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/rpc_methods_core.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/rpc_methods_core.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/src/ansys/motorcad/core/rpc_methods_core_old.py` & `ansys_motorcad_core-0.2.0/src/ansys/motorcad/core/rpc_methods_core_old.py`

 * *Files identical despite different names*

### Comparing `ansys-motorcad-core-0.1.3/PKG-INFO` & `ansys_motorcad_core-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 Metadata-Version: 2.1
 Name: ansys-motorcad-core
-Version: 0.1.3
+Version: 0.2.0
 Summary: Pythonic interface to Ansys Motor-CAD.
-Author-email: "Ansys, Inc." <pyansys.support@ansys.com>
-Maintainer-email: PyAnsys developers <pyansys.support@ansys.com>
-Requires-Python: >=3.7
+Author-email: "Ansys, Inc." <pyansys.core@ansys.com>
+Maintainer-email: PyAnsys developers <pyansys.core@ansys.com>
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: psutil >= 5.9.0
 Requires-Dist: requests >= 2.27.1
 Requires-Dist: packaging >= 21.3
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
+Requires-Dist: importlib-metadata>=4.0
+Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.5 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.11.1 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: matplotlib ; extra == "doc"
 Requires-Dist: scipy ; extra == "doc"
-Requires-Dist: pypandoc==1.10 ; extra == "doc"
-Requires-Dist: pytest==7.2.1 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pypandoc==1.11 ; extra == "doc"
+Requires-Dist: pytest==7.4.0 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
+Requires-Dist: ansys.platform.instancemanagement>=1.0.2 ; extra == "tests"
 Project-URL: Documentation, https://motorcad.docs.pyansys.com/
-Project-URL: Source, https://github.com/pyansys/pymotorcad
-Project-URL: Tracker, https://github.com/pyansys/pymotorcad/issues
+Project-URL: Source, https://github.com/ansys/pymotorcad
+Project-URL: Tracker, https://github.com/ansys/pymotorcad/issues
 Provides-Extra: doc
 Provides-Extra: tests
 
 PyMotorCAD
 ==========
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.7-blue
-   :target: https://pypi.org/project/pymotorcad-core/
+   :target: https://pypi.org/project/ansys-motorcad-core/
    :alt: Python
 
-.. |pypi| image:: https://img.shields.io/pypi/v/pymotorcad-core.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/pymotorcad-core
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-motorcad-core.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-motorcad-core/
    :alt: PyPI
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/pymotorcad/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pymotorcad
+.. |codecov| image:: https://codecov.io/gh/ansys/pymotorcad/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/pymotorcad
    :alt: Codecov
 
-.. |GH-CI| image:: https://github.com/pyansys/pymotorcad/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pymotorcad/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pymotorcad/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pymotorcad/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
@@ -103,15 +105,15 @@
     
 To install in developer mode, complete these steps:
 
 #. Clone the ``pymotorcad`` repository with this command:
 
     .. code:: bash
 
-        git clone https://github.com/pyansys/pymotorcad
+        git clone https://github.com/ansys/pymotorcad
 
 #. Create a fresh-clean Python environment and activate it with
    these commands:
 
     .. code:: bash
 
         # Create a virtual environment
```

