# Comparing `tmp/yvesCMD-0.0.1.1b0.tar.gz` & `tmp/yvesCMD-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.1.1b0.tar", last modified: Tue Aug  1 08:44:40 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.1.2.tar", last modified: Tue Aug  1 08:48:19 2023, max compression
```

## Comparing `yvesCMD-0.0.1.1b0.tar` & `yvesCMD-0.0.1.2.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:44:40.221078 yvesCMD-0.0.1.1b0/
--rw-rw-rw-   0        0        0      207 2023-08-01 08:44:40.217089 yvesCMD-0.0.1.1b0/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.1.1b0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:44:40.181185 yvesCMD-0.0.1.1b0/YvesCMD/
--rw-rw-rw-   0        0        0       25 2023-08-01 08:44:25.000000 yvesCMD-0.0.1.1b0/YvesCMD/__init__.py
--rw-rw-rw-   0        0        0       42 2023-08-01 08:44:40.222076 yvesCMD-0.0.1.1b0/setup.cfg
--rw-rw-rw-   0        0        0      332 2023-08-01 08:44:33.000000 yvesCMD-0.0.1.1b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:44:40.212102 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      207 2023-08-01 08:44:39.000000 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-08-01 08:44:40.000000 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:44:39.000000 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 08:44:39.000000 yvesCMD-0.0.1.1b0/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:48:19.644543 yvesCMD-0.0.1.2/
+-rw-rw-rw-   0        0        0      205 2023-08-01 08:48:19.642548 yvesCMD-0.0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:48:19.645539 yvesCMD-0.0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-08-01 08:48:12.000000 yvesCMD-0.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:48:19.639556 yvesCMD-0.0.1.2/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      205 2023-08-01 08:48:19.000000 yvesCMD-0.0.1.2/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-08-01 08:48:19.000000 yvesCMD-0.0.1.2/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:48:19.000000 yvesCMD-0.0.1.2/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-01 08:48:19.000000 yvesCMD-0.0.1.2/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.1.1b0/README.md` & `yvesCMD-0.0.1.2/README.md`

 * *Files identical despite different names*

