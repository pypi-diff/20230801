# Comparing `tmp/gytoolkit-0.1.0.tar.gz` & `tmp/gytoolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytoolkit-0.1.0.tar", max compression
+gzip compressed data, was "gytoolkit-0.2.0.tar", max compression
```

## Comparing `gytoolkit-0.1.0.tar` & `gytoolkit-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-08-01 06:47:06.696508 gytoolkit-0.1.0/LICENSE
--rw-r--r--   0        0        0      937 2023-08-01 06:47:06.696508 gytoolkit-0.1.0/README.md
--rw-r--r--   0        0        0      332 2023-08-01 07:54:19.246504 gytoolkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-08-01 07:49:38.216504 gytoolkit-0.1.0/src/gytoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 07:43:33.456506 gytoolkit-0.1.0/src/gytoolkit/mailparser/__init__.py
--rw-r--r--   0        0        0     1093 2023-08-01 07:47:18.766505 gytoolkit-0.1.0/src/gytoolkit/mailparser/constant.py
--rw-r--r--   0        0        0    12754 2023-08-01 07:47:08.816505 gytoolkit-0.1.0/src/gytoolkit/mailparser/mailparser.py
--rw-r--r--   0        0        0      381 2023-08-01 07:46:51.076506 gytoolkit-0.1.0/src/gytoolkit/mailparser/utils.py
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 gytoolkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-01 06:47:06.696508 gytoolkit-0.2.0/LICENSE
+-rw-r--r--   0        0        0      445 2023-08-01 10:30:18.866506 gytoolkit-0.2.0/README.md
+-rw-r--r--   0        0        0      421 2023-08-01 10:43:21.706507 gytoolkit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-08-01 07:49:38.216504 gytoolkit-0.2.0/src/gytoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 07:43:33.456506 gytoolkit-0.2.0/src/gytoolkit/mailparser/__init__.py
+-rw-r--r--   0        0        0     1093 2023-08-01 07:47:18.766505 gytoolkit-0.2.0/src/gytoolkit/mailparser/constant.py
+-rw-r--r--   0        0        0    12754 2023-08-01 07:47:08.816505 gytoolkit-0.2.0/src/gytoolkit/mailparser/mailparser.py
+-rw-r--r--   0        0        0      381 2023-08-01 07:46:51.076506 gytoolkit-0.2.0/src/gytoolkit/mailparser/utils.py
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 gytoolkit-0.2.0/PKG-INFO
```

### Comparing `gytoolkit-0.1.0/LICENSE` & `gytoolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.1.0/src/gytoolkit/mailparser/constant.py` & `gytoolkit-0.2.0/src/gytoolkit/mailparser/constant.py`

 * *Files identical despite different names*

### Comparing `gytoolkit-0.1.0/src/gytoolkit/mailparser/mailparser.py` & `gytoolkit-0.2.0/src/gytoolkit/mailparser/mailparser.py`

 * *Files identical despite different names*

