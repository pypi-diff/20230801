# Comparing `tmp/xlab-util-0.3.tar.gz` & `tmp/xlab-util-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlab-util-0.3.tar", last modified: Tue Aug  1 07:57:08 2023, max compression
+gzip compressed data, was "xlab-util-0.4.tar", last modified: Tue Aug  1 07:58:17 2023, max compression
```

## Comparing `xlab-util-0.3.tar` & `xlab-util-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-01 07:57:08.211413 xlab-util-0.3/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      182 2023-08-01 07:57:08.211413 xlab-util-0.3/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.3/README.md
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-01 07:57:08.211413 xlab-util-0.3/setup.cfg
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-01 07:57:06.000000 xlab-util-0.3/setup.py
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-01 07:57:08.211413 xlab-util-0.3/xlab_util.egg-info/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      182 2023-08-01 07:57:08.000000 xlab-util-0.3/xlab_util.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      224 2023-08-01 07:57:08.000000 xlab-util-0.3/xlab_util.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-01 07:57:08.000000 xlab-util-0.3/xlab_util.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-01 07:57:08.000000 xlab-util-0.3/xlab_util.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-01 07:57:08.211413 xlab-util-0.3/xlabutil/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      130 2023-08-01 07:56:51.000000 xlab-util-0.3/xlabutil/__init__.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.3/xlabutil/base.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1475 2023-08-01 07:32:58.000000 xlab-util-0.3/xlabutil/result.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      749 2023-08-01 07:33:04.000000 xlab-util-0.3/xlabutil/util.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-01 07:58:17.784002 xlab-util-0.4/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      182 2023-08-01 07:58:17.784002 xlab-util-0.4/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.4/README.md
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-01 07:58:17.784002 xlab-util-0.4/setup.cfg
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-01 07:58:16.000000 xlab-util-0.4/setup.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-01 07:58:17.780002 xlab-util-0.4/xlab_util.egg-info/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      182 2023-08-01 07:58:17.000000 xlab-util-0.4/xlab_util.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      224 2023-08-01 07:58:17.000000 xlab-util-0.4/xlab_util.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-01 07:58:17.000000 xlab-util-0.4/xlab_util.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-01 07:58:17.000000 xlab-util-0.4/xlab_util.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-01 07:58:17.784002 xlab-util-0.4/xlabutil/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      132 2023-08-01 07:58:06.000000 xlab-util-0.4/xlabutil/__init__.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.4/xlabutil/base.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1475 2023-08-01 07:32:58.000000 xlab-util-0.4/xlabutil/result.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      749 2023-08-01 07:33:04.000000 xlab-util-0.4/xlabutil/util.py
```

### Comparing `xlab-util-0.3/xlabutil/result.py` & `xlab-util-0.4/xlabutil/result.py`

 * *Files identical despite different names*

### Comparing `xlab-util-0.3/xlabutil/util.py` & `xlab-util-0.4/xlabutil/util.py`

 * *Files identical despite different names*

