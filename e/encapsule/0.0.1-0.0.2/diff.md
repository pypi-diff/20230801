# Comparing `tmp/encapsule-0.0.1.tar.gz` & `tmp/encapsule-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsule-0.0.1.tar", last modified: Mon Jul 31 11:08:25 2023, max compression
+gzip compressed data, was "encapsule-0.0.2.tar", last modified: Tue Aug  1 15:32:32 2023, max compression
```

## Comparing `encapsule-0.0.1.tar` & `encapsule-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-07-31 11:08:25.811837 encapsule-0.0.1/
--rw-r--r--   0 Owner    (197610) None     (197121)      189 2023-07-31 11:08:25.811837 encapsule-0.0.1/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-07-31 11:05:27.000000 encapsule-0.0.1/README
-drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-07-31 11:08:25.811837 encapsule-0.0.1/encapsule.egg-info/
--rw-r--r--   0 Owner    (197610) None     (197121)      189 2023-07-31 11:08:25.000000 encapsule-0.0.1/encapsule.egg-info/PKG-INFO
--rw-r--r--   0 Owner    (197610) None     (197121)      157 2023-07-31 11:08:25.000000 encapsule-0.0.1/encapsule.egg-info/SOURCES.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-07-31 11:08:25.000000 encapsule-0.0.1/encapsule.egg-info/dependency_links.txt
--rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-07-31 11:08:25.000000 encapsule-0.0.1/encapsule.egg-info/top_level.txt
--rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-07-31 11:08:25.811837 encapsule-0.0.1/setup.cfg
--rw-r--r--   0 Owner    (197610) None     (197121)      597 2023-07-31 11:08:19.000000 encapsule-0.0.1/setup.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.158211 encapsule-0.0.2/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 15:32:32.158211 encapsule-0.0.2/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:08:51.000000 encapsule-0.0.2/README
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.126949 encapsule-0.0.2/encapsule/
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2023-08-01 14:51:10.000000 encapsule-0.0.2/encapsule/__init__.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)     3237 2023-08-01 14:58:34.000000 encapsule-0.0.2/encapsule/isolate_bin.py
+-rwxr-xr-x   0 Owner    (197610) None     (197121)      579 2023-08-01 14:50:28.000000 encapsule-0.0.2/encapsule/isolate_sys.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-08-01 15:32:32.158211 encapsule-0.0.2/encapsule.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)      783 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)      229 2023-08-01 15:32:31.000000 encapsule-0.0.2/encapsule.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       10 2023-08-01 15:32:30.000000 encapsule-0.0.2/encapsule.egg-info/top_level.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-08-01 15:32:32.158211 encapsule-0.0.2/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     1331 2023-08-01 15:31:12.000000 encapsule-0.0.2/setup.py
```

