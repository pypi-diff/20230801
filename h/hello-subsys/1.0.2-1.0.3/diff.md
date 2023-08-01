# Comparing `tmp/hello-subsys-1.0.2.tar.gz` & `tmp/hello-subsys-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello-subsys-1.0.2.tar", last modified: Tue Aug  1 10:35:15 2023, max compression
+gzip compressed data, was "hello-subsys-1.0.3.tar", last modified: Tue Aug  1 10:39:22 2023, max compression
```

## Comparing `hello-subsys-1.0.2.tar` & `hello-subsys-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:35:15.962571 hello-subsys-1.0.2/
--rw-rw-r--   0 root         (0) root         (0)     1075 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      498 2023-08-01 10:35:15.958571 hello-subsys-1.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1527 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:35:15.954571 hello-subsys-1.0.2/app/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 16:54:57.000000 hello-subsys-1.0.2/app/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      314 2023-07-31 16:55:16.000000 hello-subsys-1.0.2/app/subsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:35:15.954571 hello-subsys-1.0.2/commands/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1219 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/commands/config.py
--rw-rw-r--   0 root         (0) root         (0)      316 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/commands/init.py
--rw-rw-r--   0 root         (0) root         (0)      999 2023-07-31 15:49:59.000000 hello-subsys-1.0.2/commands/snap.py
--rw-rw-r--   0 root         (0) root         (0)     1427 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/commands/submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:35:15.958571 hello-subsys-1.0.2/hello_subsys.egg-info/
--rw-r--r--   0 root         (0) root         (0)      498 2023-08-01 10:35:15.000000 hello-subsys-1.0.2/hello_subsys.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      505 2023-08-01 10:35:15.000000 hello-subsys-1.0.2/hello_subsys.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 10:35:15.000000 hello-subsys-1.0.2/hello_subsys.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-08-01 10:35:15.000000 hello-subsys-1.0.2/hello_subsys.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-08-01 10:35:15.000000 hello-subsys-1.0.2/hello_subsys.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-08-01 10:35:15.000000 hello-subsys-1.0.2/hello_subsys.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:35:15.958571 hello-subsys-1.0.2/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1384 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/services/auth.py
--rw-rw-r--   0 root         (0) root         (0)     2348 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/services/submit.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 10:35:15.962571 hello-subsys-1.0.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      668 2023-08-01 10:34:18.000000 hello-subsys-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:35:15.958571 hello-subsys-1.0.2/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3348 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/utils/misc.py
--rw-rw-r--   0 root         (0) root         (0)      982 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/utils/repository.py
--rw-rw-r--   0 root         (0) root         (0)     6876 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/utils/snap.py
--rw-rw-r--   0 root         (0) root         (0)     4842 2023-07-31 15:23:57.000000 hello-subsys-1.0.2/utils/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:39:22.117652 hello-subsys-1.0.3/
+-rw-rw-r--   0 root         (0) root         (0)     1075 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      498 2023-08-01 10:39:22.117652 hello-subsys-1.0.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1527 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:39:22.109651 hello-subsys-1.0.3/app/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 16:54:57.000000 hello-subsys-1.0.3/app/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      314 2023-07-31 16:55:16.000000 hello-subsys-1.0.3/app/subsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:39:22.109651 hello-subsys-1.0.3/commands/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1219 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/commands/config.py
+-rw-rw-r--   0 root         (0) root         (0)      316 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/commands/init.py
+-rw-rw-r--   0 root         (0) root         (0)      999 2023-07-31 15:49:59.000000 hello-subsys-1.0.3/commands/snap.py
+-rw-rw-r--   0 root         (0) root         (0)     1427 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/commands/submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:39:22.113652 hello-subsys-1.0.3/hello_subsys.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      498 2023-08-01 10:39:22.000000 hello-subsys-1.0.3/hello_subsys.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      505 2023-08-01 10:39:22.000000 hello-subsys-1.0.3/hello_subsys.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 10:39:22.000000 hello-subsys-1.0.3/hello_subsys.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-08-01 10:39:22.000000 hello-subsys-1.0.3/hello_subsys.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-08-01 10:39:22.000000 hello-subsys-1.0.3/hello_subsys.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-01 10:39:22.000000 hello-subsys-1.0.3/hello_subsys.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:39:22.113652 hello-subsys-1.0.3/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1384 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/services/auth.py
+-rw-rw-r--   0 root         (0) root         (0)     2348 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/services/submit.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 10:39:22.117652 hello-subsys-1.0.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      668 2023-08-01 10:37:21.000000 hello-subsys-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:39:22.117652 hello-subsys-1.0.3/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3348 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/utils/misc.py
+-rw-rw-r--   0 root         (0) root         (0)      982 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/utils/repository.py
+-rw-rw-r--   0 root         (0) root         (0)     6876 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/utils/snap.py
+-rw-rw-r--   0 root         (0) root         (0)     4842 2023-07-31 15:23:57.000000 hello-subsys-1.0.3/utils/stage.py
```

### Comparing `hello-subsys-1.0.2/LICENSE` & `hello-subsys-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/README.md` & `hello-subsys-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/commands/config.py` & `hello-subsys-1.0.3/commands/config.py`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/commands/snap.py` & `hello-subsys-1.0.3/commands/snap.py`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/commands/submit.py` & `hello-subsys-1.0.3/commands/submit.py`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/services/auth.py` & `hello-subsys-1.0.3/services/auth.py`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/services/submit.py` & `hello-subsys-1.0.3/services/submit.py`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/setup.py` & `hello-subsys-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="hello-subsys",
-    version="1.0.2 ",
+    version="1.0.3 ",
     packages=find_packages(),
     entry_points={"console_scripts": ["subsys = app.subsys:cli"]},
     install_requires=["click", "requests", "tqdm", "python-slugify"],
     author="Charles Biney, Eric Kodzi, Donal-Miles Gyasi",
     author_email="charles.biney@amalitech.org, eric.kodzi@amalitech.org, donal-miles.gyasi@amalitech.org",
     description="A git inspired assignment submission system.",
     classifiers=[
```

### Comparing `hello-subsys-1.0.2/utils/misc.py` & `hello-subsys-1.0.3/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/utils/repository.py` & `hello-subsys-1.0.3/utils/repository.py`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/utils/snap.py` & `hello-subsys-1.0.3/utils/snap.py`

 * *Files identical despite different names*

### Comparing `hello-subsys-1.0.2/utils/stage.py` & `hello-subsys-1.0.3/utils/stage.py`

 * *Files identical despite different names*

