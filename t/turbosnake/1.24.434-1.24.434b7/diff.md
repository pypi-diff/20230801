# Comparing `tmp/turbosnake-1.24.434.tar.gz` & `tmp/turbosnake-1.24.434b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbosnake-1.24.434.tar", last modified: Tue Aug  1 08:15:43 2023, max compression
+gzip compressed data, was "turbosnake-1.24.434b7.tar", last modified: Tue Aug  1 08:12:07 2023, max compression
```

## Comparing `turbosnake-1.24.434.tar` & `turbosnake-1.24.434b7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:15:43.941263 turbosnake-1.24.434/
--rw-rw-rw-   0        0        0     1095 2021-09-10 12:31:06.000000 turbosnake-1.24.434/LICENCE
--rw-rw-rw-   0        0        0     5450 2023-08-01 08:15:43.913684 turbosnake-1.24.434/PKG-INFO
--rw-rw-rw-   0        0        0     4682 2021-10-29 11:28:47.000000 turbosnake-1.24.434/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 08:15:43.941263 turbosnake-1.24.434/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-08-01 08:14:35.000000 turbosnake-1.24.434/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:15:43.895751 turbosnake-1.24.434/turbosnake/
--rw-rw-rw-   0        0        0      850 2022-02-19 13:27:01.000000 turbosnake-1.24.434/turbosnake/__init__.py
--rw-rw-rw-   0        0        0     5655 2022-02-20 15:47:40.000000 turbosnake-1.24.434/turbosnake/_async.py
--rw-rw-rw-   0        0        0    18341 2023-08-01 05:59:14.000000 turbosnake-1.24.434/turbosnake/_components.py
--rw-rw-rw-   0        0        0     3496 2021-10-21 12:54:45.000000 turbosnake-1.24.434/turbosnake/_context.py
--rw-rw-rw-   0        0        0     3159 2023-08-01 05:59:30.000000 turbosnake-1.24.434/turbosnake/_functional_component.py
--rw-rw-rw-   0        0        0    11875 2021-11-02 13:29:06.000000 turbosnake-1.24.434/turbosnake/_hooks.py
--rw-rw-rw-   0        0        0     1021 2021-09-09 20:18:41.000000 turbosnake-1.24.434/turbosnake/_render_context.py
--rw-rw-rw-   0        0        0     3717 2021-11-02 13:53:18.000000 turbosnake-1.24.434/turbosnake/_slotted_component.py
--rw-rw-rw-   0        0        0     2910 2021-11-01 12:00:37.000000 turbosnake-1.24.434/turbosnake/_utils.py
--rw-rw-rw-   0        0        0     1529 2022-02-20 15:24:42.000000 turbosnake-1.24.434/turbosnake/_utils0.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:15:43.906703 turbosnake-1.24.434/turbosnake/test_helpers/
--rw-rw-rw-   0        0        0       51 2021-09-09 20:11:59.000000 turbosnake-1.24.434/turbosnake/test_helpers/__init__.py
--rw-rw-rw-   0        0        0     3589 2021-10-21 11:54:08.000000 turbosnake-1.24.434/turbosnake/test_helpers/_selectors.py
--rw-rw-rw-   0        0        0     3015 2022-02-20 15:27:46.000000 turbosnake-1.24.434/turbosnake/test_helpers/_test_helpers.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:15:43.912687 turbosnake-1.24.434/turbosnake/ttk/
--rw-rw-rw-   0        0        0      517 2022-01-27 16:27:11.000000 turbosnake-1.24.434/turbosnake/ttk/__init__.py
--rw-rw-rw-   0        0        0     7521 2022-01-27 15:48:04.000000 turbosnake-1.24.434/turbosnake/ttk/_adapters.py
--rw-rw-rw-   0        0        0     3670 2022-01-27 16:27:11.000000 turbosnake-1.24.434/turbosnake/ttk/_composite.py
--rw-rw-rw-   0        0        0     6748 2023-08-01 06:03:31.000000 turbosnake-1.24.434/turbosnake/ttk/_core.py
--rw-rw-rw-   0        0        0     7925 2021-11-02 13:54:25.000000 turbosnake-1.24.434/turbosnake/ttk/_layout.py
--rw-rw-rw-   0        0        0     6841 2023-08-01 06:00:17.000000 turbosnake-1.24.434/turbosnake/ttk/_menu.py
--rw-rw-rw-   0        0        0    12386 2022-02-12 14:46:51.000000 turbosnake-1.24.434/turbosnake/ttk/_style.py
--rw-rw-rw-   0        0        0     1618 2023-08-01 06:06:46.000000 turbosnake-1.24.434/turbosnake/ttk/_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:15:43.903709 turbosnake-1.24.434/turbosnake.egg-info/
--rw-rw-rw-   0        0        0     5450 2023-08-01 08:15:43.000000 turbosnake-1.24.434/turbosnake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-08-01 08:15:43.000000 turbosnake-1.24.434/turbosnake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:15:43.000000 turbosnake-1.24.434/turbosnake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 08:15:43.000000 turbosnake-1.24.434/turbosnake.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.229843 turbosnake-1.24.434b7/
+-rw-rw-rw-   0        0        0     1095 2021-09-10 12:31:06.000000 turbosnake-1.24.434b7/LICENCE
+-rw-rw-rw-   0        0        0     5452 2023-08-01 08:12:07.228843 turbosnake-1.24.434b7/PKG-INFO
+-rw-rw-rw-   0        0        0     4682 2021-10-29 11:28:47.000000 turbosnake-1.24.434b7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:12:07.229843 turbosnake-1.24.434b7/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-08-01 08:07:06.000000 turbosnake-1.24.434b7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.204293 turbosnake-1.24.434b7/turbosnake/
+-rw-rw-rw-   0        0        0      850 2022-02-19 13:27:01.000000 turbosnake-1.24.434b7/turbosnake/__init__.py
+-rw-rw-rw-   0        0        0     5655 2022-02-20 15:47:40.000000 turbosnake-1.24.434b7/turbosnake/_async.py
+-rw-rw-rw-   0        0        0    18341 2023-08-01 05:59:14.000000 turbosnake-1.24.434b7/turbosnake/_components.py
+-rw-rw-rw-   0        0        0     3496 2021-10-21 12:54:45.000000 turbosnake-1.24.434b7/turbosnake/_context.py
+-rw-rw-rw-   0        0        0     3159 2023-08-01 05:59:30.000000 turbosnake-1.24.434b7/turbosnake/_functional_component.py
+-rw-rw-rw-   0        0        0    11875 2021-11-02 13:29:06.000000 turbosnake-1.24.434b7/turbosnake/_hooks.py
+-rw-rw-rw-   0        0        0     1021 2021-09-09 20:18:41.000000 turbosnake-1.24.434b7/turbosnake/_render_context.py
+-rw-rw-rw-   0        0        0     3717 2021-11-02 13:53:18.000000 turbosnake-1.24.434b7/turbosnake/_slotted_component.py
+-rw-rw-rw-   0        0        0     2910 2021-11-01 12:00:37.000000 turbosnake-1.24.434b7/turbosnake/_utils.py
+-rw-rw-rw-   0        0        0     1529 2022-02-20 15:24:42.000000 turbosnake-1.24.434b7/turbosnake/_utils0.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.217873 turbosnake-1.24.434b7/turbosnake/test_helpers/
+-rw-rw-rw-   0        0        0       51 2021-09-09 20:11:59.000000 turbosnake-1.24.434b7/turbosnake/test_helpers/__init__.py
+-rw-rw-rw-   0        0        0     3589 2021-10-21 11:54:08.000000 turbosnake-1.24.434b7/turbosnake/test_helpers/_selectors.py
+-rw-rw-rw-   0        0        0     3015 2022-02-20 15:27:46.000000 turbosnake-1.24.434b7/turbosnake/test_helpers/_test_helpers.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.227847 turbosnake-1.24.434b7/turbosnake/ttk/
+-rw-rw-rw-   0        0        0      517 2022-01-27 16:27:11.000000 turbosnake-1.24.434b7/turbosnake/ttk/__init__.py
+-rw-rw-rw-   0        0        0     7521 2022-01-27 15:48:04.000000 turbosnake-1.24.434b7/turbosnake/ttk/_adapters.py
+-rw-rw-rw-   0        0        0     3670 2022-01-27 16:27:11.000000 turbosnake-1.24.434b7/turbosnake/ttk/_composite.py
+-rw-rw-rw-   0        0        0     6748 2023-08-01 06:03:31.000000 turbosnake-1.24.434b7/turbosnake/ttk/_core.py
+-rw-rw-rw-   0        0        0     7925 2021-11-02 13:54:25.000000 turbosnake-1.24.434b7/turbosnake/ttk/_layout.py
+-rw-rw-rw-   0        0        0     6841 2023-08-01 06:00:17.000000 turbosnake-1.24.434b7/turbosnake/ttk/_menu.py
+-rw-rw-rw-   0        0        0    12386 2022-02-12 14:46:51.000000 turbosnake-1.24.434b7/turbosnake/ttk/_style.py
+-rw-rw-rw-   0        0        0     1618 2023-08-01 06:06:46.000000 turbosnake-1.24.434b7/turbosnake/ttk/_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:12:07.214913 turbosnake-1.24.434b7/turbosnake.egg-info/
+-rw-rw-rw-   0        0        0     5452 2023-08-01 08:12:07.000000 turbosnake-1.24.434b7/turbosnake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-08-01 08:12:07.000000 turbosnake-1.24.434b7/turbosnake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:12:07.000000 turbosnake-1.24.434b7/turbosnake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 08:12:07.000000 turbosnake-1.24.434b7/turbosnake.egg-info/top_level.txt
```

### Comparing `turbosnake-1.24.434/LICENCE` & `turbosnake-1.24.434b7/LICENCE`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/PKG-INFO` & `turbosnake-1.24.434b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbosnake
-Version: 1.24.434
+Version: 1.24.434b7
 Summary: React.js-like framework with components for native user interfaces
 Home-page: https://github.com/AlexeyBond/turbosnake
 Author: Alexey Bondarenko
 Author-email: alexey.bond.94.55+turbosnake@gmail.com
 License: MIT
 Keywords: ui,reactive,tkinter
 Classifier: Development Status :: 4 - Beta
```

### Comparing `turbosnake-1.24.434/README.md` & `turbosnake-1.24.434b7/README.md`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/setup.py` & `turbosnake-1.24.434b7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open("README.md", encoding="utf-8") as fp:
     long_description = fp.read()
 
 setup(
     name='turbosnake',
-    version='1.24.434',
+    version='1.24.434-beta7',
     packages=['turbosnake', 'turbosnake.ttk', 'turbosnake.test_helpers'],
     url='https://github.com/AlexeyBond/turbosnake',
     author='Alexey Bondarenko',
     author_email='alexey.bond.94.55+turbosnake@gmail.com',
     description='React.js-like framework with components for native user interfaces',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `turbosnake-1.24.434/turbosnake/__init__.py` & `turbosnake-1.24.434b7/turbosnake/__init__.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_async.py` & `turbosnake-1.24.434b7/turbosnake/_async.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_components.py` & `turbosnake-1.24.434b7/turbosnake/_components.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_context.py` & `turbosnake-1.24.434b7/turbosnake/_context.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_functional_component.py` & `turbosnake-1.24.434b7/turbosnake/_functional_component.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_hooks.py` & `turbosnake-1.24.434b7/turbosnake/_hooks.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_render_context.py` & `turbosnake-1.24.434b7/turbosnake/_render_context.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_slotted_component.py` & `turbosnake-1.24.434b7/turbosnake/_slotted_component.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_utils.py` & `turbosnake-1.24.434b7/turbosnake/_utils.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/_utils0.py` & `turbosnake-1.24.434b7/turbosnake/_utils0.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/test_helpers/_selectors.py` & `turbosnake-1.24.434b7/turbosnake/test_helpers/_selectors.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/test_helpers/_test_helpers.py` & `turbosnake-1.24.434b7/turbosnake/test_helpers/_test_helpers.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/ttk/__init__.py` & `turbosnake-1.24.434b7/turbosnake/ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/ttk/_adapters.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_adapters.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/ttk/_composite.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_composite.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/ttk/_core.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_core.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/ttk/_layout.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_layout.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/ttk/_menu.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_menu.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/ttk/_style.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_style.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake/ttk/_utils.py` & `turbosnake-1.24.434b7/turbosnake/ttk/_utils.py`

 * *Files identical despite different names*

### Comparing `turbosnake-1.24.434/turbosnake.egg-info/PKG-INFO` & `turbosnake-1.24.434b7/turbosnake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbosnake
-Version: 1.24.434
+Version: 1.24.434b7
 Summary: React.js-like framework with components for native user interfaces
 Home-page: https://github.com/AlexeyBond/turbosnake
 Author: Alexey Bondarenko
 Author-email: alexey.bond.94.55+turbosnake@gmail.com
 License: MIT
 Keywords: ui,reactive,tkinter
 Classifier: Development Status :: 4 - Beta
```

### Comparing `turbosnake-1.24.434/turbosnake.egg-info/SOURCES.txt` & `turbosnake-1.24.434b7/turbosnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

