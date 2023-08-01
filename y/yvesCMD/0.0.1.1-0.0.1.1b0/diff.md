# Comparing `tmp/yvesCMD-0.0.1.1.tar.gz` & `tmp/yvesCMD-0.0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.1.1.tar", last modified: Tue Aug  1 08:41:56 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.1.1b0.tar", last modified: Tue Aug  1 08:44:40 2023, max compression
```

## Comparing `yvesCMD-0.0.1.1.tar` & `yvesCMD-0.0.1.1b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:41:56.667310 yvesCMD-0.0.1.1/
--rw-rw-rw-   0        0        0      205 2023-08-01 08:41:56.666313 yvesCMD-0.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:41:56.628414 yvesCMD-0.0.1.1/YvesCMD/
--rw-rw-rw-   0        0        0       19 2023-08-01 08:40:17.000000 yvesCMD-0.0.1.1/YvesCMD/__init__.py
--rw-rw-rw-   0        0        0       42 2023-08-01 08:41:56.668307 yvesCMD-0.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-08-01 08:41:48.000000 yvesCMD-0.0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:41:56.662323 yvesCMD-0.0.1.1/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      205 2023-08-01 08:41:56.000000 yvesCMD-0.0.1.1/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-08-01 08:41:56.000000 yvesCMD-0.0.1.1/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:41:56.000000 yvesCMD-0.0.1.1/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 08:41:56.000000 yvesCMD-0.0.1.1/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:44:40.221078 yvesCMD-0.0.1.1b0/
+-rw-rw-rw-   0        0        0      207 2023-08-01 08:44:40.217089 yvesCMD-0.0.1.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.1.1b0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:44:40.181185 yvesCMD-0.0.1.1b0/YvesCMD/
+-rw-rw-rw-   0        0        0       25 2023-08-01 08:44:25.000000 yvesCMD-0.0.1.1b0/YvesCMD/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:44:40.222076 yvesCMD-0.0.1.1b0/setup.cfg
+-rw-rw-rw-   0        0        0      332 2023-08-01 08:44:33.000000 yvesCMD-0.0.1.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:44:40.212102 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-08-01 08:44:39.000000 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-08-01 08:44:40.000000 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:44:39.000000 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 08:44:39.000000 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.1.1/README.md` & `yvesCMD-0.0.1.1b0/README.md`

 * *Files identical despite different names*

