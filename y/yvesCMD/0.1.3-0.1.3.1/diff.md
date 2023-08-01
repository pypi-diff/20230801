# Comparing `tmp/yvesCMD-0.1.3.tar.gz` & `tmp/yvesCMD-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.1.3.tar", last modified: Tue Aug  1 07:13:38 2023, max compression
+gzip compressed data, was "yvesCMD-0.1.3.1.tar", last modified: Tue Aug  1 07:21:31 2023, max compression
```

## Comparing `yvesCMD-0.1.3.tar` & `yvesCMD-0.1.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 07:13:38.787307 yvesCMD-0.1.3/
--rw-rw-rw-   0        0        0      203 2023-08-01 07:13:38.785313 yvesCMD-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 07:13:38.788305 yvesCMD-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-08-01 07:13:36.000000 yvesCMD-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 07:13:38.782320 yvesCMD-0.1.3/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      203 2023-08-01 07:13:38.000000 yvesCMD-0.1.3/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-08-01 07:13:38.000000 yvesCMD-0.1.3/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:13:38.000000 yvesCMD-0.1.3/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:13:38.000000 yvesCMD-0.1.3/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 07:21:31.880975 yvesCMD-0.1.3.1/
+-rw-rw-rw-   0        0        0      205 2023-08-01 07:21:31.876985 yvesCMD-0.1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:21:31.881971 yvesCMD-0.1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      330 2023-08-01 07:17:49.000000 yvesCMD-0.1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:21:31.873992 yvesCMD-0.1.3.1/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      205 2023-08-01 07:21:31.000000 yvesCMD-0.1.3.1/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-08-01 07:21:31.000000 yvesCMD-0.1.3.1/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:21:31.000000 yvesCMD-0.1.3.1/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 07:21:31.000000 yvesCMD-0.1.3.1/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.1.3/README.md` & `yvesCMD-0.1.3.1/README.md`

 * *Files identical despite different names*

