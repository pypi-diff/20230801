# Comparing `tmp/YahooRequests-0.1.5.6.tar.gz` & `tmp/yahoorequests-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YahooRequests-0.1.5.6.tar", last modified: Mon Jul 31 15:04:25 2023, max compression
+gzip compressed data, was "yahoorequests-1.0.tar", max compression
```

## Comparing `YahooRequests-0.1.5.6.tar` & `yahoorequests-1.0.tar`

### file list

```diff
@@ -1,17 +1,7 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.6/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.6/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1879 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      827 2023-07-31 14:45:57.000000 YahooRequests-0.1.5.6/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/YahooRequests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       70 2023-07-31 14:43:58.000000 YahooRequests-0.1.5.6/YahooRequests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2023-07-31 14:43:56.000000 YahooRequests-0.1.5.6/YahooRequests/yahoorequests.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/YahooRequests.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1879 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      329 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1378 2023-07-31 15:04:09.000000 YahooRequests-0.1.5.6/setup.py
+-rw-r--r--   0        0        0      637 2023-08-01 19:34:52.670774 yahoorequests-1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-08-01 19:34:52.670774 yahoorequests-1.0/LICENSE
+-rw-r--r--   0        0        0      641 2023-08-01 19:34:52.670774 yahoorequests-1.0/README.md
+-rw-r--r--   0        0        0       70 2023-08-01 19:34:52.670774 yahoorequests-1.0/YahooRequests/__init__.py
+-rw-r--r--   0        0        0     1643 2023-08-01 19:34:52.670774 yahoorequests-1.0/YahooRequests/yahoorequests.py
+-rw-r--r--   0        0        0      756 2023-08-01 19:34:52.670774 yahoorequests-1.0/pyproject.toml
+-rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 yahoorequests-1.0/PKG-INFO
```

### Comparing `YahooRequests-0.1.5.6/LICENSE` & `yahoorequests-1.0/LICENSE`

 * *Files identical despite different names*

