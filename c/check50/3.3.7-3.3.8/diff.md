# Comparing `tmp/check50-3.3.7.tar.gz` & `tmp/check50-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/check50/check50/dist/tmpo_upbw3d/check50-3.3.7.tar", last modified: Wed Sep 21 03:15:14 2022, max compression
+gzip compressed data, was "check50-3.3.8.tar", last modified: Tue Aug  1 12:35:17 2023, max compression
```

## Comparing `check50-3.3.7.tar` & `check50-3.3.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:15:14.000000 check50-3.3.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-09-21 03:13:45.000000 check50-3.3.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-09-21 03:13:45.000000 check50-3.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-09-21 03:15:14.000000 check50-3.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:15:14.000000 check50-3.3.7/check50/
--rw-r--r--   0 runner    (1001) docker     (121)     5031 2022-09-21 03:13:45.000000 check50-3.3.7/check50/c.py
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-09-21 03:13:45.000000 check50-3.3.7/check50/_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-09-21 03:13:45.000000 check50-3.3.7/check50/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)    16275 2022-09-21 03:13:45.000000 check50-3.3.7/check50/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5790 2022-09-21 03:13:45.000000 check50-3.3.7/check50/internal.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-09-21 03:13:45.000000 check50-3.3.7/check50/regex.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-09-21 03:13:45.000000 check50-3.3.7/check50/py.py
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-09-21 03:13:45.000000 check50-3.3.7/check50/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    16950 2022-09-21 03:13:45.000000 check50-3.3.7/check50/_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6479 2022-09-21 03:13:45.000000 check50-3.3.7/check50/flask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-09-21 03:13:45.000000 check50-3.3.7/check50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:15:14.000000 check50-3.3.7/check50/renderer/
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-09-21 03:13:45.000000 check50-3.3.7/check50/renderer/_renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:15:14.000000 check50-3.3.7/check50/renderer/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     8003 2022-09-21 03:13:45.000000 check50-3.3.7/check50/renderer/templates/results.html
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-21 03:13:45.000000 check50-3.3.7/check50/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15556 2022-09-21 03:13:45.000000 check50-3.3.7/check50/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:15:14.000000 check50-3.3.7/check50.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-09-21 03:15:14.000000 check50-3.3.7/check50.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-21 03:15:14.000000 check50-3.3.7/check50.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-21 03:15:14.000000 check50-3.3.7/check50.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 03:15:14.000000 check50-3.3.7/check50.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-09-21 03:15:14.000000 check50-3.3.7/check50.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-09-21 03:15:14.000000 check50-3.3.7/check50.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-21 03:13:45.000000 check50-3.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-09-21 03:13:45.000000 check50-3.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-09-21 03:15:14.000000 check50-3.3.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:35:17.627583 check50-3.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 12:34:07.000000 check50-3.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 12:34:07.000000 check50-3.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 12:35:17.627583 check50-3.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-01 12:34:07.000000 check50-3.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:35:17.627583 check50-3.3.8/check50/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-01 12:34:07.000000 check50-3.3.8/check50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-08-01 12:34:07.000000 check50-3.3.8/check50/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-08-01 12:34:07.000000 check50-3.3.8/check50/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-01 12:34:07.000000 check50-3.3.8/check50/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-08-01 12:34:07.000000 check50-3.3.8/check50/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-08-01 12:34:07.000000 check50-3.3.8/check50/c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-01 12:34:07.000000 check50-3.3.8/check50/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-08-01 12:34:07.000000 check50-3.3.8/check50/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-08-01 12:34:07.000000 check50-3.3.8/check50/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-01 12:34:07.000000 check50-3.3.8/check50/py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-01 12:34:07.000000 check50-3.3.8/check50/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:35:17.627583 check50-3.3.8/check50/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 12:34:07.000000 check50-3.3.8/check50/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-01 12:34:07.000000 check50-3.3.8/check50/renderer/_renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:35:17.627583 check50-3.3.8/check50/renderer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-08-01 12:34:07.000000 check50-3.3.8/check50/renderer/templates/results.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-08-01 12:34:07.000000 check50-3.3.8/check50/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:35:17.627583 check50-3.3.8/check50.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 12:35:17.000000 check50-3.3.8/check50.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-01 12:35:17.000000 check50-3.3.8/check50.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:35:17.000000 check50-3.3.8/check50.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 12:35:17.000000 check50-3.3.8/check50.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 12:35:17.000000 check50-3.3.8/check50.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 12:35:17.000000 check50-3.3.8/check50.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 12:35:17.627583 check50-3.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-01 12:34:07.000000 check50-3.3.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `check50-3.3.7/setup.py` & `check50-3.3.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,26 +9,27 @@
     classifiers=[
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
         "Topic :: Education",
         "Topic :: Utilities"
     ],
     description="This is check50, with which you can check solutions to problems for CS50.",
+    long_description=open("README.md").read(),
     license="GPLv3",
     message_extractors = {
         'check50': [('**.py', 'python', None),],
     },
-    install_requires=["attrs>=18", "beautifulsoup4>=0", "pexpect>=4.6", "lib50>=3,<4", "pyyaml>=3.10", "requests>=2.19", "termcolor>=1.1", "jinja2>=2.10"],
+    install_requires=["attrs>=18", "beautifulsoup4>=0", "pexpect>=4.6", "lib50>=3,<4", "pyyaml>6,<7", "requests>=2.19", "termcolor>=1.1", "jinja2>=2.10"],
     extras_require = {
         "develop": ["sphinx", "sphinx-autobuild", "sphinx_rtd_theme"]
     },
     keywords=["check", "check50"],
     name="check50",
     packages=["check50", "check50.renderer"],
     python_requires=">= 3.6",
     entry_points={
         "console_scripts": ["check50=check50.__main__:main"]
     },
     url="https://github.com/cs50/check50",
-    version="3.3.7",
+    version="3.3.8",
     include_package_data=True
 )
```

### Comparing `check50-3.3.7/check50/c.py` & `check50-3.3.8/check50/c.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/_simple.py` & `check50-3.3.8/check50/_simple.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/__main__.py` & `check50-3.3.8/check50/__main__.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/internal.py` & `check50-3.3.8/check50/internal.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/regex.py` & `check50-3.3.8/check50/regex.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/py.py` & `check50-3.3.8/check50/py.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/_exceptions.py` & `check50-3.3.8/check50/_exceptions.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/_api.py` & `check50-3.3.8/check50/_api.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/flask.py` & `check50-3.3.8/check50/flask.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/__init__.py` & `check50-3.3.8/check50/__init__.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/renderer/_renderers.py` & `check50-3.3.8/check50/renderer/_renderers.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/renderer/templates/results.html` & `check50-3.3.8/check50/renderer/templates/results.html`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50/runner.py` & `check50-3.3.8/check50/runner.py`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/check50.egg-info/SOURCES.txt` & `check50-3.3.8/check50.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `check50-3.3.7/LICENSE` & `check50-3.3.8/LICENSE`

 * *Files identical despite different names*

