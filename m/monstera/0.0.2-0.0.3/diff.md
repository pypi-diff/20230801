# Comparing `tmp/monstera-0.0.2.tar.gz` & `tmp/monstera-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstera-0.0.2.tar", last modified: Fri Jul 28 23:56:35 2023, max compression
+gzip compressed data, was "monstera-0.0.3.tar", last modified: Mon Jul 31 22:02:37 2023, max compression
```

## Comparing `monstera-0.0.2.tar` & `monstera-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-28 23:56:35.098635 monstera-0.0.2/
--rw-r--r--   0 dishb      (502) staff       (20)     1099 2023-07-28 01:34:18.000000 monstera-0.0.2/LICENSE.md
--rw-r--r--   0 dishb      (502) staff       (20)     5737 2023-07-28 23:56:35.097747 monstera-0.0.2/PKG-INFO
--rw-r--r--   0 dishb      (502) staff       (20)     4448 2023-07-28 23:11:49.000000 monstera-0.0.2/README.md
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-28 23:56:35.072533 monstera-0.0.2/monstera/
--rw-r--r--   0 dishb      (502) staff       (20)     6303 2023-07-28 23:37:45.000000 monstera-0.0.2/monstera/__init__.py
--rw-r--r--   0 dishb      (502) staff       (20)     4283 2023-07-28 02:31:08.000000 monstera-0.0.2/monstera/__main__.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-28 23:56:35.078935 monstera-0.0.2/monstera.egg-info/
--rw-r--r--   0 dishb      (502) staff       (20)     5737 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/PKG-INFO
--rw-r--r--   0 dishb      (502) staff       (20)      311 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/SOURCES.txt
--rw-r--r--   0 dishb      (502) staff       (20)        1 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/dependency_links.txt
--rw-r--r--   0 dishb      (502) staff       (20)       53 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/entry_points.txt
--rw-r--r--   0 dishb      (502) staff       (20)       16 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/requires.txt
--rw-r--r--   0 dishb      (502) staff       (20)        9 2023-07-28 23:56:35.000000 monstera-0.0.2/monstera.egg-info/top_level.txt
--rw-r--r--   0 dishb      (502) staff       (20)       38 2023-07-28 23:56:35.098886 monstera-0.0.2/setup.cfg
--rw-r--r--   0 dishb      (502) staff       (20)     3620 2023-07-28 23:52:08.000000 monstera-0.0.2/setup.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-28 23:56:35.091733 monstera-0.0.2/tests/
--rw-r--r--   0 dishb      (502) staff       (20)     3774 2023-07-28 19:32:17.000000 monstera-0.0.2/tests/test_monstera.py
--rw-r--r--   0 dishb      (502) staff       (20)     3858 2023-07-28 19:31:28.000000 monstera-0.0.2/tests/test_python_m.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.755302 monstera-0.0.3/
+-rw-r--r--   0 dishb      (502) staff       (20)     1099 2023-07-31 17:18:53.000000 monstera-0.0.3/LICENSE.md
+-rw-r--r--   0 dishb      (502) staff       (20)     5713 2023-07-31 22:02:37.751141 monstera-0.0.3/PKG-INFO
+-rw-r--r--   0 dishb      (502) staff       (20)     4424 2023-07-31 20:58:11.000000 monstera-0.0.3/README.md
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.714182 monstera-0.0.3/monstera/
+-rw-r--r--   0 dishb      (502) staff       (20)     2871 2023-07-31 21:31:13.000000 monstera-0.0.3/monstera/__init__.py
+-rw-r--r--   0 dishb      (502) staff       (20)     1402 2023-07-31 20:23:46.000000 monstera-0.0.3/monstera/__main__.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.739007 monstera-0.0.3/monstera/_core/
+-rw-r--r--   0 dishb      (502) staff       (20)     1272 2023-07-31 20:20:59.000000 monstera-0.0.3/monstera/_core/__init__.py
+-rw-r--r--   0 dishb      (502) staff       (20)     4200 2023-07-31 20:24:20.000000 monstera-0.0.3/monstera/_core/_entry_points.py
+-rw-r--r--   0 dishb      (502) staff       (20)     5509 2023-07-31 21:24:46.000000 monstera-0.0.3/monstera/_core/_main.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.727622 monstera-0.0.3/monstera.egg-info/
+-rw-r--r--   0 dishb      (502) staff       (20)     5713 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/PKG-INFO
+-rw-r--r--   0 dishb      (502) staff       (20)      394 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/SOURCES.txt
+-rw-r--r--   0 dishb      (502) staff       (20)        1 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/dependency_links.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       53 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/entry_points.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       16 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/requires.txt
+-rw-r--r--   0 dishb      (502) staff       (20)        9 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/top_level.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       38 2023-07-31 22:02:37.755612 monstera-0.0.3/setup.cfg
+-rw-r--r--   0 dishb      (502) staff       (20)     3602 2023-07-31 21:31:09.000000 monstera-0.0.3/setup.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.746614 monstera-0.0.3/tests/
+-rw-r--r--   0 dishb      (502) staff       (20)     3774 2023-07-31 17:18:53.000000 monstera-0.0.3/tests/test_monstera.py
+-rw-r--r--   0 dishb      (502) staff       (20)     3858 2023-07-31 17:18:53.000000 monstera-0.0.3/tests/test_python_m.py
```

### Comparing `monstera-0.0.2/LICENSE.md` & `monstera-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monstera-0.0.2/PKG-INFO` & `monstera-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstera
-Version: 0.0.2
+Version: 0.0.3
 Summary: A cross-platform CLI to quickly retrieve system information to make issue management easier.
 Home-page: https://github.com/dishb/monstera
 Author: Dishant B. (@dishb)
 Author-email: code.dishb@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/dishb/monstera/tree/main/docs
 Project-URL: Source, https://github.com/dishb/monstera/
@@ -45,15 +45,17 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 -->
 
-![monstera's banner image](https://github.com/dishb/monstera/blob/2517642244aac49d978ed6b779cedb8e4fbb4681/assets/banner.png)
+<div align = 'center'>
+    <img alt = 'banner image' src = './assets/banner.png' width = 300/>
+</div>
 
 # monstera
 
 A cross-platform CLI to quickly retrieve system information to make issue management easier.
 
 ## Features:
 A list of all the information collected:
@@ -78,15 +80,15 @@
 You can install the package with `pip`.
 
 | macOS/Linux | Windows |
 | --- | --- |
 | `pip3 install monstera` | `pip install monstera` |
 
 ## Usage:
-There are 2 options for how you can use 'monstera'.
+There are 2 options for how you can use `monstera`.
 
 1. Use the CLI:
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `python3 -m monstera` | `python -m monstera` |
```

### Comparing `monstera-0.0.2/README.md` & `monstera-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 -->
 
-![monstera's banner image](https://github.com/dishb/monstera/blob/2517642244aac49d978ed6b779cedb8e4fbb4681/assets/banner.png)
+<div align = 'center'>
+    <img alt = 'banner image' src = './assets/banner.png' width = 300/>
+</div>
 
 # monstera
 
 A cross-platform CLI to quickly retrieve system information to make issue management easier.
 
 ## Features:
 A list of all the information collected:
@@ -51,15 +53,15 @@
 You can install the package with `pip`.
 
 | macOS/Linux | Windows |
 | --- | --- |
 | `pip3 install monstera` | `pip install monstera` |
 
 ## Usage:
-There are 2 options for how you can use 'monstera'.
+There are 2 options for how you can use `monstera`.
 
 1. Use the CLI:
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `python3 -m monstera` | `python -m monstera` |
```

### Comparing `monstera-0.0.2/monstera/__init__.py` & `monstera-0.0.3/monstera/_core/_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,42 +34,14 @@
 import platform
 from os.path import dirname
 from subprocess import CalledProcessError, run as sp_run
 from typing import Dict, List, Union
 
 import distro
 
-__source__ = "https://github.com/dishb/monstera"
-__license__ = "MIT License"
-__version__ = "0.0.2"
-__author__ = "Dishant B. (@dishb) <code.dishb@gmail.com>"
-__copyright__ = """
-                MIT License
-
-                Copyright (c) 2023 Dishant B. (@dishb) <code.dishb@gmail.com>
-
-                Permission is hereby granted, free of charge, to any person obtaining a copy
-                of this software and associated documentation files (the "Software"), to deal
-                in the Software without restriction, including without limitation the rights
-                to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-                copies of the Software, and to permit persons to whom the Software is
-                furnished to do so, subject to the following conditions:
-
-                The above copyright notice and this permission notice shall be included in all
-                copies or substantial portions of the Software.
-
-                THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-                IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-                FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-                AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-                LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-                OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-                SOFTWARE.
-                """
-
 def run(packages: Union[List[str], str] = None) -> Dict[str, str]:
     """
     monstera's main function. Gets the following information about the user's machine:
     Meant for programming use. Do not use monstera._main().
 
     - Operating system
     - OS version
@@ -101,17 +73,35 @@
     else:
         pip_cmd = "pip"
 
     pkg_vers = []
     pkg_locs = []
 
     if packages is not None:
-        for pkg in packages:
+        if isinstance(packages, list):
+            for pkg in packages:
+                try:
+                    output1 = sp_run([pip_cmd, "show", pkg],
+                                     check = True,
+                                     capture_output = True
+                                     ).stdout
+                    output1 = output1.decode().split("\n")
+
+                    pkg_locs.append(output1[7].split()[1])
+                    pkg_vers.append(output1[1].split()[1])
+                except CalledProcessError:
+                    pkg_locs.append(f"{pkg} is not installed")
+                    pkg_vers.append(f"{pkg} is not installed.")
+
+        elif isinstance(packages, str):
             try:
-                output1 = sp_run([pip_cmd, "show", pkg], check = True, capture_output = True).stdout
+                output1 = sp_run([pip_cmd, "show", packages],
+                                 check = True,
+                                 capture_output = True
+                                 ).stdout
                 output1 = output1.decode().split("\n")
 
                 pkg_locs.append(output1[7].split()[1])
                 pkg_vers.append(output1[1].split()[1])
             except CalledProcessError:
                 pkg_locs.append(f"{pkg} is not installed")
                 pkg_vers.append(f"{pkg} is not installed.")
```

### Comparing `monstera-0.0.2/monstera/__main__.py` & `monstera-0.0.3/monstera/_core/_entry_points.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,22 +26,21 @@
 monstera
 
 Author: Dishant B. (@dishb) code.dishb@gmail.com
 License: MIT License
 Source: https://github.com/dishb/monstera
 """
 
-from sys import exit as sys_exit
 from argparse import ArgumentParser
 
 from colorama import Fore, Style, init, deinit
 
-from .__init__ import run
+from ._main import run
 
-def _main() -> int:
+def _console() -> int:
     """
     monstera's main entry point. Gets the following information about the user's machine:
     Not meant for programming usage. Please use monstera.run().
 
     - Operating system
     - OS version
     - Machine architecture
@@ -127,10 +126,7 @@
                 print(f"    Location: {info[f'{pkg}_location']}")
                 print(f"    Version: {info[f'{pkg}_version']}")
 
     print("")
 
     deinit()
     return 0
-
-if __name__ == "__main__":
-    sys_exit(_main())
```

### Comparing `monstera-0.0.2/monstera.egg-info/PKG-INFO` & `monstera-0.0.3/monstera.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstera
-Version: 0.0.2
+Version: 0.0.3
 Summary: A cross-platform CLI to quickly retrieve system information to make issue management easier.
 Home-page: https://github.com/dishb/monstera
 Author: Dishant B. (@dishb)
 Author-email: code.dishb@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/dishb/monstera/tree/main/docs
 Project-URL: Source, https://github.com/dishb/monstera/
@@ -45,15 +45,17 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 -->
 
-![monstera's banner image](https://github.com/dishb/monstera/blob/2517642244aac49d978ed6b779cedb8e4fbb4681/assets/banner.png)
+<div align = 'center'>
+    <img alt = 'banner image' src = './assets/banner.png' width = 300/>
+</div>
 
 # monstera
 
 A cross-platform CLI to quickly retrieve system information to make issue management easier.
 
 ## Features:
 A list of all the information collected:
@@ -78,15 +80,15 @@
 You can install the package with `pip`.
 
 | macOS/Linux | Windows |
 | --- | --- |
 | `pip3 install monstera` | `pip install monstera` |
 
 ## Usage:
-There are 2 options for how you can use 'monstera'.
+There are 2 options for how you can use `monstera`.
 
 1. Use the CLI:
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `python3 -m monstera` | `python -m monstera` |
```

### Comparing `monstera-0.0.2/setup.py` & `monstera-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-from setuptools import setup, find_packages
+from setuptools import setup
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = """A cross-platform CLI to quickly retrieve system information to make issue management easier."""
 
 with open("README.md", "r", encoding = "utf-8") as file:
     LONG_DESCRIPTION = file.read()
     file.close()
 
 with open("requirements.txt", "r", encoding = "utf-8") as file:
@@ -39,15 +39,16 @@
 setup(name = "monstera",
       version = VERSION,
       author = "Dishant B. (@dishb)",
       author_email = "code.dishb@gmail.com",
       description = DESCRIPTION,
       long_description = LONG_DESCRIPTION,
       long_description_content_type = "text/markdown",
-      packages = find_packages(include = ["monstera", "monstera.*"]),
+      packages = ["monstera",
+                  "monstera._core"],
       entry_points = {"console_scripts": ["monstera = monstera.__main__:_main"]},
       install_requires = REQUIREMENTS,
       python_requires = ">=3.9",
       keywords = ["monstera",
                   "bug tracker",
                   "bug tracking",
                   "issue tracker",
```

### Comparing `monstera-0.0.2/tests/test_monstera.py` & `monstera-0.0.3/tests/test_monstera.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     output = command.stdout.decode()
 
     expected_output = """
 Python: 3.11.4, final release
 
 Python Location: /Users/dishb/Coding/monstera/.venv/bin
 
-Operating System: macOS 12.6.7
+Operating System: macOS 12.6.8
 
 Architecture: 64bit
 
 Pip: 23.2.1
 
 Pip Location: /Users/dishb/Coding/monstera/.venv/lib/python3.11/site-packages
 
@@ -81,15 +81,15 @@
     output = command.stdout.decode()
 
     expected_output = """
 Python: 3.11.4, final release
 
 Python Location: /Users/dishb/Coding/monstera/.venv/bin
 
-Operating System: macOS 12.6.7
+Operating System: macOS 12.6.8
 
 Architecture: 64bit
 
 Pip: 23.2.1
 
 Pip Location: /Users/dishb/Coding/monstera/.venv/lib/python3.11/site-packages
 
@@ -117,15 +117,15 @@
     output = command.stdout.decode()
 
     expected_output = """
 Python: 3.11.4, final release
 
 Python Location: /Users/dishb/Coding/monstera/.venv/bin
 
-Operating System: macOS 12.6.7
+Operating System: macOS 12.6.8
 
 Architecture: 64bit
 
 Pip: 23.2.1
 
 Pip Location: /Users/dishb/Coding/monstera/.venv/lib/python3.11/site-packages
```

### Comparing `monstera-0.0.2/tests/test_python_m.py` & `monstera-0.0.3/tests/test_python_m.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     output = command.stdout.decode()
 
     expected_output = """
 Python: 3.11.4, final release
 
 Python Location: /Users/dishb/Coding/monstera/.venv/bin
 
-Operating System: macOS 12.6.7
+Operating System: macOS 12.6.8
 
 Architecture: 64bit
 
 Pip: 23.2.1
 
 Pip Location: /Users/dishb/Coding/monstera/.venv/lib/python3.11/site-packages
 
@@ -81,15 +81,15 @@
     output = command.stdout.decode()
 
     expected_output = """
 Python: 3.11.4, final release
 
 Python Location: /Users/dishb/Coding/monstera/.venv/bin
 
-Operating System: macOS 12.6.7
+Operating System: macOS 12.6.8
 
 Architecture: 64bit
 
 Pip: 23.2.1
 
 Pip Location: /Users/dishb/Coding/monstera/.venv/lib/python3.11/site-packages
 
@@ -117,15 +117,15 @@
     output = command.stdout.decode()
 
     expected_output = """
 Python: 3.11.4, final release
 
 Python Location: /Users/dishb/Coding/monstera/.venv/bin
 
-Operating System: macOS 12.6.7
+Operating System: macOS 12.6.8
 
 Architecture: 64bit
 
 Pip: 23.2.1
 
 Pip Location: /Users/dishb/Coding/monstera/.venv/lib/python3.11/site-packages
```

