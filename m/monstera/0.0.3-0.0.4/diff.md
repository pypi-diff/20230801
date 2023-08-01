# Comparing `tmp/monstera-0.0.3.tar.gz` & `tmp/monstera-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstera-0.0.3.tar", last modified: Mon Jul 31 22:02:37 2023, max compression
+gzip compressed data, was "monstera-0.0.4.tar", last modified: Tue Aug  1 02:31:08 2023, max compression
```

## Comparing `monstera-0.0.3.tar` & `monstera-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.755302 monstera-0.0.3/
--rw-r--r--   0 dishb      (502) staff       (20)     1099 2023-07-31 17:18:53.000000 monstera-0.0.3/LICENSE.md
--rw-r--r--   0 dishb      (502) staff       (20)     5713 2023-07-31 22:02:37.751141 monstera-0.0.3/PKG-INFO
--rw-r--r--   0 dishb      (502) staff       (20)     4424 2023-07-31 20:58:11.000000 monstera-0.0.3/README.md
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.714182 monstera-0.0.3/monstera/
--rw-r--r--   0 dishb      (502) staff       (20)     2871 2023-07-31 21:31:13.000000 monstera-0.0.3/monstera/__init__.py
--rw-r--r--   0 dishb      (502) staff       (20)     1402 2023-07-31 20:23:46.000000 monstera-0.0.3/monstera/__main__.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.739007 monstera-0.0.3/monstera/_core/
--rw-r--r--   0 dishb      (502) staff       (20)     1272 2023-07-31 20:20:59.000000 monstera-0.0.3/monstera/_core/__init__.py
--rw-r--r--   0 dishb      (502) staff       (20)     4200 2023-07-31 20:24:20.000000 monstera-0.0.3/monstera/_core/_entry_points.py
--rw-r--r--   0 dishb      (502) staff       (20)     5509 2023-07-31 21:24:46.000000 monstera-0.0.3/monstera/_core/_main.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.727622 monstera-0.0.3/monstera.egg-info/
--rw-r--r--   0 dishb      (502) staff       (20)     5713 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/PKG-INFO
--rw-r--r--   0 dishb      (502) staff       (20)      394 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/SOURCES.txt
--rw-r--r--   0 dishb      (502) staff       (20)        1 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/dependency_links.txt
--rw-r--r--   0 dishb      (502) staff       (20)       53 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/entry_points.txt
--rw-r--r--   0 dishb      (502) staff       (20)       16 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/requires.txt
--rw-r--r--   0 dishb      (502) staff       (20)        9 2023-07-31 22:02:37.000000 monstera-0.0.3/monstera.egg-info/top_level.txt
--rw-r--r--   0 dishb      (502) staff       (20)       38 2023-07-31 22:02:37.755612 monstera-0.0.3/setup.cfg
--rw-r--r--   0 dishb      (502) staff       (20)     3602 2023-07-31 21:31:09.000000 monstera-0.0.3/setup.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-07-31 22:02:37.746614 monstera-0.0.3/tests/
--rw-r--r--   0 dishb      (502) staff       (20)     3774 2023-07-31 17:18:53.000000 monstera-0.0.3/tests/test_monstera.py
--rw-r--r--   0 dishb      (502) staff       (20)     3858 2023-07-31 17:18:53.000000 monstera-0.0.3/tests/test_python_m.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.552963 monstera-0.0.4/
+-rw-r--r--   0 dishb      (502) staff       (20)     1099 2023-07-31 17:18:53.000000 monstera-0.0.4/LICENSE.md
+-rw-r--r--   0 dishb      (502) staff       (20)     5713 2023-08-01 02:31:08.548981 monstera-0.0.4/PKG-INFO
+-rw-r--r--   0 dishb      (502) staff       (20)     4424 2023-07-31 20:58:11.000000 monstera-0.0.4/README.md
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.453819 monstera-0.0.4/monstera/
+-rw-r--r--   0 dishb      (502) staff       (20)     2871 2023-08-01 02:28:58.000000 monstera-0.0.4/monstera/__init__.py
+-rw-r--r--   0 dishb      (502) staff       (20)     1402 2023-07-31 20:23:46.000000 monstera-0.0.4/monstera/__main__.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.496712 monstera-0.0.4/monstera/_core/
+-rw-r--r--   0 dishb      (502) staff       (20)     1272 2023-07-31 20:20:59.000000 monstera-0.0.4/monstera/_core/__init__.py
+-rw-r--r--   0 dishb      (502) staff       (20)     4200 2023-07-31 20:24:20.000000 monstera-0.0.4/monstera/_core/_entry_points.py
+-rw-r--r--   0 dishb      (502) staff       (20)     5509 2023-07-31 21:24:46.000000 monstera-0.0.4/monstera/_core/_main.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.482531 monstera-0.0.4/monstera.egg-info/
+-rw-r--r--   0 dishb      (502) staff       (20)     5713 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/PKG-INFO
+-rw-r--r--   0 dishb      (502) staff       (20)      394 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/SOURCES.txt
+-rw-r--r--   0 dishb      (502) staff       (20)        1 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/dependency_links.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       67 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/entry_points.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       16 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/requires.txt
+-rw-r--r--   0 dishb      (502) staff       (20)        9 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/top_level.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       38 2023-08-01 02:31:08.553494 monstera-0.0.4/setup.cfg
+-rw-r--r--   0 dishb      (502) staff       (20)     3635 2023-08-01 02:28:32.000000 monstera-0.0.4/setup.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.546457 monstera-0.0.4/tests/
+-rw-r--r--   0 dishb      (502) staff       (20)     3774 2023-08-01 02:20:02.000000 monstera-0.0.4/tests/test_monstera.py
+-rw-r--r--   0 dishb      (502) staff       (20)     3858 2023-07-31 17:18:53.000000 monstera-0.0.4/tests/test_python_m.py
```

### Comparing `monstera-0.0.3/LICENSE.md` & `monstera-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monstera-0.0.3/PKG-INFO` & `monstera-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstera
-Version: 0.0.3
+Version: 0.0.4
 Summary: A cross-platform CLI to quickly retrieve system information to make issue management easier.
 Home-page: https://github.com/dishb/monstera
 Author: Dishant B. (@dishb)
 Author-email: code.dishb@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/dishb/monstera/tree/main/docs
 Project-URL: Source, https://github.com/dishb/monstera/
```

### Comparing `monstera-0.0.3/README.md` & `monstera-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `monstera-0.0.3/monstera/__init__.py` & `monstera-0.0.4/monstera/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Source: https://github.com/dishb/monstera
 """
 
 from ._core._main import run
 
 __source__ = "https://github.com/dishb/monstera"
 __license__ = "MIT License"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Dishant B. (@dishb) <code.dishb@gmail.com>"
 __copyright__ = """
                 MIT License
 
                 Copyright (c) 2023 Dishant B. (@dishb) <code.dishb@gmail.com>
 
                 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `monstera-0.0.3/monstera/__main__.py` & `monstera-0.0.4/monstera/__main__.py`

 * *Files identical despite different names*

### Comparing `monstera-0.0.3/monstera/_core/__init__.py` & `monstera-0.0.4/monstera/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `monstera-0.0.3/monstera/_core/_entry_points.py` & `monstera-0.0.4/monstera/_core/_entry_points.py`

 * *Files identical despite different names*

### Comparing `monstera-0.0.3/monstera/_core/_main.py` & `monstera-0.0.4/monstera/_core/_main.py`

 * *Files identical despite different names*

### Comparing `monstera-0.0.3/monstera.egg-info/PKG-INFO` & `monstera-0.0.4/monstera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstera
-Version: 0.0.3
+Version: 0.0.4
 Summary: A cross-platform CLI to quickly retrieve system information to make issue management easier.
 Home-page: https://github.com/dishb/monstera
 Author: Dishant B. (@dishb)
 Author-email: code.dishb@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/dishb/monstera/tree/main/docs
 Project-URL: Source, https://github.com/dishb/monstera/
```

### Comparing `monstera-0.0.3/setup.py` & `monstera-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 from setuptools import setup
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = """A cross-platform CLI to quickly retrieve system information to make issue management easier."""
 
 with open("README.md", "r", encoding = "utf-8") as file:
     LONG_DESCRIPTION = file.read()
     file.close()
 
 with open("requirements.txt", "r", encoding = "utf-8") as file:
@@ -40,16 +40,17 @@
       version = VERSION,
       author = "Dishant B. (@dishb)",
       author_email = "code.dishb@gmail.com",
       description = DESCRIPTION,
       long_description = LONG_DESCRIPTION,
       long_description_content_type = "text/markdown",
       packages = ["monstera",
-                  "monstera._core"],
-      entry_points = {"console_scripts": ["monstera = monstera.__main__:_main"]},
+                  "monstera._core"
+                  ],
+      entry_points = {"console_scripts": ["monstera = monstera._core._entry_points:_console"]},
       install_requires = REQUIREMENTS,
       python_requires = ">=3.9",
       keywords = ["monstera",
                   "bug tracker",
                   "bug tracking",
                   "issue tracker",
                   "issue tracking",
```

### Comparing `monstera-0.0.3/tests/test_monstera.py` & `monstera-0.0.4/tests/test_monstera.py`

 * *Files identical despite different names*

### Comparing `monstera-0.0.3/tests/test_python_m.py` & `monstera-0.0.4/tests/test_python_m.py`

 * *Files identical despite different names*

