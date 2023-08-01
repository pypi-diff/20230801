# Comparing `tmp/convert_jupyter-1.0.2.tar.gz` & `tmp/convert_jupyter-1.0.3.tar.gz`

## Comparing `convert_jupyter-1.0.2.tar` & `convert_jupyter-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/.flake8
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/.pylintrc
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/Makefile
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/lint.sh
--rw-r--r--   0        0        0    46737 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/poetry.lock
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/upload.sh
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/__init__.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/__main__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/clean.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/code.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/convert_jupyter/constans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/test_clean.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/test_code.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/test_main.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/convert.py
--rw-r--r--   0        0        0    84335 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/test_jupyter.ipynb
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/test_jupyter_clean.ipynb
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/tmp.ipynb
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/tmp.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/try.ipynb
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/try.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/try3.ipynb
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/tests/code/try3.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/README.md
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 convert_jupyter-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/.flake8
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/.pylintrc
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/Makefile
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/lint.sh
+-rw-r--r--   0        0        0    47193 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/poetry.lock
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/upload.sh
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/convert_jupyter/__init__.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/convert_jupyter/__main__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/convert_jupyter/clean.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/convert_jupyter/code.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/convert_jupyter/constans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/test_clean.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/test_code.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/test_main.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/convert.py
+-rw-r--r--   0        0        0    84335 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/test_jupyter.ipynb
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/test_jupyter_clean.ipynb
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/tmp.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/tmp.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/try.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/try.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/try3.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/tests/code/try3.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/README.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 convert_jupyter-1.0.3/PKG-INFO
```

### Comparing `convert_jupyter-1.0.2/.pylintrc` & `convert_jupyter-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/lint.sh` & `convert_jupyter-1.0.3/lint.sh`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/poetry.lock` & `convert_jupyter-1.0.3/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -470,14 +470,22 @@
 python-versions = ">=3.7"
 
 [package.extras]
 docs = ["myst-parser", "pydata-sphinx-theme", "sphinx"]
 test = ["argcomplete (>=2.0)", "pre-commit", "pytest", "pytest-mock"]
 
 [[package]]
+name = "types-setuptools"
+version = "68.0.0.3"
+description = "Typing stubs for setuptools"
+category = "main"
+optional = false
+python-versions = "*"
+
+[[package]]
 name = "typing-extensions"
 version = "4.7.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 
@@ -496,15 +504,15 @@
 category = "main"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7"
 
 [metadata]
 lock-version = "1.1"
 python-versions = "^3.8"
-content-hash = "7e269c4ae2bc8659d6e6014637d8a96988ca0d066bf2ddc35f16bbfdff494f8c"
+content-hash = "2c56353bcb557dcc28d83bf1c23fe22bfb08b9165566da0132da2549cf19586a"
 
 [metadata.files]
 appnope = [
     {file = "appnope-0.1.3-py2.py3-none-any.whl", hash = "sha256:265a455292d0bd8a72453494fa24df5a11eb18373a60c7c0430889f22548605e"},
     {file = "appnope-0.1.3.tar.gz", hash = "sha256:02bd91c4de869fbb1e1c50aafc4098827a7a54ab2f39d9dcba6c9547ed920e24"},
 ]
 astroid = [
@@ -723,14 +731,18 @@
     {file = "tomlkit-0.12.1-py3-none-any.whl", hash = "sha256:712cbd236609acc6a3e2e97253dfc52d4c2082982a88f61b640ecf0817eab899"},
     {file = "tomlkit-0.12.1.tar.gz", hash = "sha256:38e1ff8edb991273ec9f6181244a6a391ac30e9f5098e7535640ea6be97a7c86"},
 ]
 traitlets = [
     {file = "traitlets-5.9.0-py3-none-any.whl", hash = "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8"},
     {file = "traitlets-5.9.0.tar.gz", hash = "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"},
 ]
+types-setuptools = [
+    {file = "types-setuptools-68.0.0.3.tar.gz", hash = "sha256:d57ae6076100b5704b3cc869fdefc671e1baf4c2cd6643f84265dfc0b955bf05"},
+    {file = "types_setuptools-68.0.0.3-py3-none-any.whl", hash = "sha256:fec09e5c18264c5c09351c00be01a34456fb7a88e457abe97401325f84ad9d36"},
+]
 typing-extensions = [
     {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
     {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 wcwidth = [
     {file = "wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
```

### Comparing `convert_jupyter-1.0.2/convert_jupyter/__main__.py` & `convert_jupyter-1.0.3/convert_jupyter/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,28 @@
 import getopt
-import os
 import sys
 
+import pkg_resources
+
 from . import clean, clean_all, jupyter2py, py2jupyter
 
 
 def get_project_version() -> str:
-    """Get project version from pyproject.toml [project] statment.
-
-    Raises:
-        EOFError: If pyproject.toml have not valid field.
-
-    Returns:
-        str: project version.
-    """
-    main_folder = sys.argv[0].split(os.sep)[:-2]
-    with open(
-        os.sep.join([*main_folder, "pyproject.toml"]), "r", encoding="utf-8"
-    ) as toml:
-        for line in toml:
-            if line.strip() == "[project]":
-                break
-        for line in toml:
-            if line.strip()[:7] == "version":
-                return line.split("=", 1)[1].strip().replace("'", "").replace('"', "")
-    raise EOFError("End of file.")
-
-
-def safety_get_project_version() -> str:
-    """Get project version, but if something work bad return empty string.
+    """Get version number safely.
 
     Returns:
-        str: project version or empty string.
+        str: version number, if pkg_resources.DistributionNotFound then "Unknown"
     """
     try:
-        version = get_project_version()
-        return f" version {version}"
-    except:  # pylint: disable=W0702 # noqa
-        return ""
+        return pkg_resources.get_distribution("convert_jupyter").version
+    except pkg_resources.DistributionNotFound:
+        return "Unknown"
 
 
-help_info = f"""convert_jupyter package{safety_get_project_version()}.
+help_info = f"""convert_jupyter package{get_project_version()}.
 Usage:
   python3 -m convert_jupyter [options] <command> <input_file>
 
 commands:
   jupyter2py                Convert jupyter file to python file.
   py2jupyter                Convert python file to jupyter file.
   clean                     Clean set jupyter file outputs.
```

### Comparing `convert_jupyter-1.0.2/convert_jupyter/clean.py` & `convert_jupyter-1.0.3/convert_jupyter/clean.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/convert_jupyter/code.py` & `convert_jupyter-1.0.3/convert_jupyter/code.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/test_clean.py` & `convert_jupyter-1.0.3/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/test_code.py` & `convert_jupyter-1.0.3/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/test_main.py` & `convert_jupyter-1.0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/code/convert.py` & `convert_jupyter-1.0.3/tests/code/convert.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/code/test_jupyter.ipynb` & `convert_jupyter-1.0.3/tests/code/test_jupyter.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/code/test_jupyter_clean.ipynb` & `convert_jupyter-1.0.3/tests/code/test_jupyter_clean.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/code/tmp.ipynb` & `convert_jupyter-1.0.3/tests/code/tmp.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/code/try.ipynb` & `convert_jupyter-1.0.3/tests/code/try.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/tests/code/try3.ipynb` & `convert_jupyter-1.0.3/tests/code/try3.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/LICENSE.md` & `convert_jupyter-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert_jupyter-1.0.2/README.md` & `convert_jupyter-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 # Convert jupyter 
 This project help convert jupyter flie.
 It let:
-    - convert .ipynb to .py file
-    - convert .py to .ipynb file
-    - clean output jupyter
+- convert .ipynb to .py file
+- convert .py to .ipynb file
+- clean output jupyter
 
 
 ## autors
 Bartłomiej Chwiłkowski (github: chwilko)
 
 
 # Usage:
 python3 -m convert_jupyter [options] <command> <input_file>
 
 commands:
-  jupyter2py                Convert jupyter file to python file.
-  py2jupyter                Convert python file to jupyter file.
-  clean                     Clean set jupyter file outputs.
-  clean_all                 Clean all jupyter files outputs from the set folder and child folders
+  - jupyter2py                Convert jupyter file to python file.
+  - py2jupyter                Convert python file to jupyter file.
+  - clean                     Clean set jupyter file outputs.
+  - clean_all                 Clean all jupyter files outputs from the set folder and child folders
 
 input_file -- name of input file to convert or clean.
 
 General options:
-  -o, --output              Set the output file name. By default, it is the input file name with a valid extension.
-  -i, --input               Set input file directly.
-  -c, --command             Set command directly.
-  -f, --force               If file with output name exists overwrite them. By default raise error.
-  -h, --help                Show help and exit.
-  -V, --version             Show version and exit.
+  - -o, --output              Set the output file name. By default, it is the input file name with a valid extension.
+  - -i, --input               Set input file directly.
+  - -c, --command             Set command directly.
+  - -f, --force               If file with output name exists overwrite them. By default raise error.
+  - -h, --help                Show help and exit.
+  - -V, --version             Show version and exit.
 
 
 # Structure
 convert_jupyter:
     - file with functions
 
 tests:
     - tests
 
 
 ## Functions 
 
-jupyter2py(
-    f_in_name: str,
-    f_out_name: Union[str, None] = None,
-    force: bool = False
-)
-    Convert jupyter file f_in_name to python file f_out_name.
+jupyter2py(f_in_name: str, f_out_name: Union[str, None] = None, force: bool = False)
+ - Convert jupyter file f_in_name to python file f_out_name.
 
-py2jupyter(f_in_name: str, f_out_name: str = None)
-    Convert python file f_in_name to jupyter file f_out_name.
+py2jupyter(f_in_name: str, f_out_name: Union[str, None] = None, force: bool = False)
+ - Convert python file f_in_name to jupyter file f_out_name.
 
 clean(path: str)
-    Function clean jupyter file output.
+ - Function clean jupyter file output.
 
 clean_all(path: str)
-    The function recursively finds all jupyter files and clears their output.
+ - The function recursively finds all jupyter files and clears their output.
 
 
 ## Licence
 MIT
```

### Comparing `convert_jupyter-1.0.2/pyproject.toml` & `convert_jupyter-1.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convert-jupyter"
-version = "1.0.2"
+version = "1.0.3"
 description = "Package help convert jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts"
 
 authors = ["Bartłomiej Chwiłkowski <bartekchwilkowski@gmail.com>"]
 packages = [{include = "convert_jupyter"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -14,25 +14,26 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 black = {extras = ["jupyter"], version = "^22.10.0"}
 pylint = "^2.17.5"
 isort = "^5.12.0"
 mypy = "^1.4.1"
+types-setuptools = "^68.0.0.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "convert-jupyter"
-version = "1.0.2"
+version = "1.0.3"
 authors = [    
   { name="Bartłomiej Chwiłkowski", email="bartekchwilkowski@gmail.com" },
   ]
 description = "Package help convert jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `convert_jupyter-1.0.2/PKG-INFO` & `convert_jupyter-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 Metadata-Version: 2.1
 Name: convert-jupyter
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package help convert jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts
 Project-URL: Homepage, https://github.com/chwilko/convert_jupyter
 Author-email: Bartłomiej Chwiłkowski <bartekchwilkowski@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Convert jupyter 
 This project help convert jupyter flie.
 It let:
-    - convert .ipynb to .py file
-    - convert .py to .ipynb file
-    - clean output jupyter
+- convert .ipynb to .py file
+- convert .py to .ipynb file
+- clean output jupyter
 
 
 ## autors
 Bartłomiej Chwiłkowski (github: chwilko)
 
 
 # Usage:
 python3 -m convert_jupyter [options] <command> <input_file>
 
 commands:
-  jupyter2py                Convert jupyter file to python file.
-  py2jupyter                Convert python file to jupyter file.
-  clean                     Clean set jupyter file outputs.
-  clean_all                 Clean all jupyter files outputs from the set folder and child folders
+  - jupyter2py                Convert jupyter file to python file.
+  - py2jupyter                Convert python file to jupyter file.
+  - clean                     Clean set jupyter file outputs.
+  - clean_all                 Clean all jupyter files outputs from the set folder and child folders
 
 input_file -- name of input file to convert or clean.
 
 General options:
-  -o, --output              Set the output file name. By default, it is the input file name with a valid extension.
-  -i, --input               Set input file directly.
-  -c, --command             Set command directly.
-  -f, --force               If file with output name exists overwrite them. By default raise error.
-  -h, --help                Show help and exit.
-  -V, --version             Show version and exit.
+  - -o, --output              Set the output file name. By default, it is the input file name with a valid extension.
+  - -i, --input               Set input file directly.
+  - -c, --command             Set command directly.
+  - -f, --force               If file with output name exists overwrite them. By default raise error.
+  - -h, --help                Show help and exit.
+  - -V, --version             Show version and exit.
 
 
 # Structure
 convert_jupyter:
     - file with functions
 
 tests:
     - tests
 
 
 ## Functions 
 
-jupyter2py(
-    f_in_name: str,
-    f_out_name: Union[str, None] = None,
-    force: bool = False
-)
-    Convert jupyter file f_in_name to python file f_out_name.
+jupyter2py(f_in_name: str, f_out_name: Union[str, None] = None, force: bool = False)
+ - Convert jupyter file f_in_name to python file f_out_name.
 
-py2jupyter(f_in_name: str, f_out_name: str = None)
-    Convert python file f_in_name to jupyter file f_out_name.
+py2jupyter(f_in_name: str, f_out_name: Union[str, None] = None, force: bool = False)
+ - Convert python file f_in_name to jupyter file f_out_name.
 
 clean(path: str)
-    Function clean jupyter file output.
+ - Function clean jupyter file output.
 
 clean_all(path: str)
-    The function recursively finds all jupyter files and clears their output.
+ - The function recursively finds all jupyter files and clears their output.
 
 
 ## Licence
 MIT
```

