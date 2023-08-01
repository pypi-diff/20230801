# Comparing `tmp/yvesCMD-0.1.2.tar.gz` & `tmp/yvesCMD-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.1.2.tar", last modified: Tue Aug  1 07:06:17 2023, max compression
+gzip compressed data, was "yvesCMD-0.1.3.tar", last modified: Tue Aug  1 07:13:38 2023, max compression
```

## Comparing `yvesCMD-0.1.2.tar` & `yvesCMD-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 07:06:17.092139 yvesCMD-0.1.2/
--rw-rw-rw-   0        0        0      203 2023-08-01 07:06:17.090142 yvesCMD-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 07:06:17.092139 yvesCMD-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-08-01 07:05:59.000000 yvesCMD-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 07:06:17.052244 yvesCMD-0.1.2/src/
--rw-rw-rw-   0        0        0       77 2023-08-01 07:04:42.000000 yvesCMD-0.1.2/src/__init__.py
--rw-rw-rw-   0        0        0     1427 2023-07-31 13:41:19.000000 yvesCMD-0.1.2/src/register.py
--rw-rw-rw-   0        0        0     5891 2023-08-01 07:01:36.000000 yvesCMD-0.1.2/src/yvescmd.py
-drwxrwxrwx   0        0        0        0 2023-08-01 07:06:17.087150 yvesCMD-0.1.2/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      203 2023-08-01 07:06:16.000000 yvesCMD-0.1.2/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-01 07:06:16.000000 yvesCMD-0.1.2/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:06:16.000000 yvesCMD-0.1.2/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 07:06:16.000000 yvesCMD-0.1.2/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 07:13:38.787307 yvesCMD-0.1.3/
+-rw-rw-rw-   0        0        0      203 2023-08-01 07:13:38.785313 yvesCMD-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:13:38.788305 yvesCMD-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-08-01 07:13:36.000000 yvesCMD-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:13:38.782320 yvesCMD-0.1.3/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-08-01 07:13:38.000000 yvesCMD-0.1.3/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-08-01 07:13:38.000000 yvesCMD-0.1.3/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:13:38.000000 yvesCMD-0.1.3/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:13:38.000000 yvesCMD-0.1.3/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.1.2/README.md` & `yvesCMD-0.1.3/README.md`

 * *Files identical despite different names*

