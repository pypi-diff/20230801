# Comparing `tmp/yvesCMD-0.1.4b0.tar.gz` & `tmp/yvesCMD-0.1.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.1.4b0.tar", last modified: Tue Aug  1 08:13:19 2023, max compression
+gzip compressed data, was "yvesCMD-0.1.4rc0.tar", last modified: Tue Aug  1 08:13:39 2023, max compression
```

## Comparing `yvesCMD-0.1.4b0.tar` & `yvesCMD-0.1.4rc0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:13:19.354094 yvesCMD-0.1.4b0/
--rw-rw-rw-   0        0        0      205 2023-08-01 08:13:19.352105 yvesCMD-0.1.4b0/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.4b0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 08:13:19.357085 yvesCMD-0.1.4b0/setup.cfg
--rw-rw-rw-   0        0        0      329 2023-08-01 08:11:59.000000 yvesCMD-0.1.4b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:13:19.345838 yvesCMD-0.1.4b0/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      205 2023-08-01 08:13:19.000000 yvesCMD-0.1.4b0/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-08-01 08:13:19.000000 yvesCMD-0.1.4b0/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:13:19.000000 yvesCMD-0.1.4b0/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-01 08:13:19.000000 yvesCMD-0.1.4b0/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:13:39.146553 yvesCMD-0.1.4rc0/
+-rw-rw-rw-   0        0        0      206 2023-08-01 08:13:39.141566 yvesCMD-0.1.4rc0/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.1.4rc0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:13:39.147552 yvesCMD-0.1.4rc0/setup.cfg
+-rw-rw-rw-   0        0        0      329 2023-08-01 08:13:31.000000 yvesCMD-0.1.4rc0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:13:39.139572 yvesCMD-0.1.4rc0/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      206 2023-08-01 08:13:38.000000 yvesCMD-0.1.4rc0/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-08-01 08:13:38.000000 yvesCMD-0.1.4rc0/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:13:38.000000 yvesCMD-0.1.4rc0/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 08:13:38.000000 yvesCMD-0.1.4rc0/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.1.4b0/README.md` & `yvesCMD-0.1.4rc0/README.md`

 * *Files identical despite different names*

