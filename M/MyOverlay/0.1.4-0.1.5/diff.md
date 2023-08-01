# Comparing `tmp/MyOverlay-0.1.4.tar.gz` & `tmp/MyOverlay-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.1.4.tar", last modified: Tue Aug  1 09:18:02 2023, max compression
+gzip compressed data, was "MyOverlay-0.1.5.tar", last modified: Tue Aug  1 09:47:02 2023, max compression
```

## Comparing `MyOverlay-0.1.4.tar` & `MyOverlay-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 09:18:02.150242 MyOverlay-0.1.4/
--rw-rw-rw-   0        0        0        0 2023-08-01 07:59:52.000000 MyOverlay-0.1.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-08-01 09:18:02.148249 MyOverlay-0.1.4/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      735 2023-08-01 09:18:02.000000 MyOverlay-0.1.4/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-08-01 09:18:02.000000 MyOverlay-0.1.4/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:18:02.000000 MyOverlay-0.1.4/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-08-01 09:18:02.000000 MyOverlay-0.1.4/MyOverlay.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:18:02.000000 MyOverlay-0.1.4/MyOverlay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      735 2023-08-01 09:18:02.149242 MyOverlay-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-01 08:00:03.000000 MyOverlay-0.1.4/README.rst
--rw-rw-rw-   0        0        0       86 2023-08-01 09:15:15.000000 MyOverlay-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 09:18:02.150242 MyOverlay-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-08-01 09:17:46.000000 MyOverlay-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.558841 MyOverlay-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-08-01 09:47:02.557840 MyOverlay-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.1.5/README.md
+-rw-rw-rw-   0        0        0      649 2023-08-01 09:43:00.000000 MyOverlay-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:47:02.558841 MyOverlay-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.541840 MyOverlay-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.545841 MyOverlay-0.1.5/src/MyOverlay/
+-rw-rw-rw-   0        0        0      332 2023-08-01 07:54:17.000000 MyOverlay-0.1.5/src/MyOverlay/Overlay.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 14:05:46.000000 MyOverlay-0.1.5/src/MyOverlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.556840 MyOverlay-0.1.5/src/MyOverlay/funcs/
+-rw-rw-rw-   0        0        0     3293 2023-08-01 07:53:45.000000 MyOverlay-0.1.5/src/MyOverlay/funcs/myfunctions.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:47:02.555841 MyOverlay-0.1.5/src/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-01 09:47:02.000000 MyOverlay-0.1.5/src/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-08-01 09:47:02.000000 MyOverlay-0.1.5/src/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:47:02.000000 MyOverlay-0.1.5/src/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 09:47:02.000000 MyOverlay-0.1.5/src/MyOverlay.egg-info/top_level.txt
```

