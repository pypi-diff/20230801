# Comparing `tmp/shahidutils-0.1.0.tar.gz` & `tmp/shahidutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shahidutils-0.1.0.tar", max compression
+gzip compressed data, was "shahidutils-0.1.1.tar", max compression
```

## Comparing `shahidutils-0.1.0.tar` & `shahidutils-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-08-01 00:59:58.317280 shahidutils-0.1.0/README.md
--rw-r--r--   0        0        0      274 2023-08-01 00:59:58.317280 shahidutils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 00:59:58.317280 shahidutils-0.1.0/shahidutils/__init__.py
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 shahidutils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-01 00:59:58.317280 shahidutils-0.1.1/README.md
+-rw-r--r--   0        0        0      274 2023-08-01 01:03:56.676471 shahidutils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-08-01 01:02:33.758937 shahidutils-0.1.1/shahidutils/__init__.py
+-rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 shahidutils-0.1.1/PKG-INFO
```

