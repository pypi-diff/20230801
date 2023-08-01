# Comparing `tmp/tflstatuscli-0.1.0.tar.gz` & `tmp/tflstatuscli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tflstatuscli-0.1.0.tar", max compression
+gzip compressed data, was "tflstatuscli-0.1.1.tar", max compression
```

## Comparing `tflstatuscli-0.1.0.tar` & `tflstatuscli-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        9 2023-08-01 18:08:27.459975 tflstatuscli-0.1.0/README.md
--rw-r--r--   0        0        0      445 2023-08-01 18:20:36.205527 tflstatuscli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 22:24:52.823601 tflstatuscli-0.1.0/tflstatuscli/__init__.py
--rwxr-xr-x   0        0        0     2363 2023-08-01 18:02:56.312839 tflstatuscli-0.1.0/tflstatuscli/tflstatuscli.py
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 tflstatuscli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      179 2023-08-01 18:28:17.345268 tflstatuscli-0.1.1/README.md
+-rw-r--r--   0        0        0      461 2023-08-01 18:32:06.598386 tflstatuscli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 22:24:52.823601 tflstatuscli-0.1.1/tflstatuscli/__init__.py
+-rwxr-xr-x   0        0        0     2363 2023-08-01 18:02:56.312839 tflstatuscli-0.1.1/tflstatuscli/tflstatuscli.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 tflstatuscli-0.1.1/PKG-INFO
```

### Comparing `tflstatuscli-0.1.0/tflstatuscli/tflstatuscli.py` & `tflstatuscli-0.1.1/tflstatuscli/tflstatuscli.py`

 * *Files identical despite different names*

