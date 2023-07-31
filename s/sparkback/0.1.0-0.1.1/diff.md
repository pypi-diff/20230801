# Comparing `tmp/sparkback-0.1.0.tar.gz` & `tmp/sparkback-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkback-0.1.0.tar", max compression
+gzip compressed data, was "sparkback-0.1.1.tar", max compression
```

## Comparing `sparkback-0.1.0.tar` & `sparkback-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-07-31 21:56:20.500473 sparkback-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      520 2023-07-31 23:04:57.297074 sparkback-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-31 22:01:55.272321 sparkback-0.1.0/sparkback/__init__.py
--rw-r--r--   0        0        0     2059 2023-07-31 22:44:53.321985 sparkback-0.1.0/sparkback/spark.py
--rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 sparkback-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-31 21:56:20.500473 sparkback-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      920 2023-07-31 22:53:55.909578 sparkback-0.1.1/README.md
+-rw-r--r--   0        0        0      858 2023-07-31 23:20:02.016319 sparkback-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-31 22:01:55.272321 sparkback-0.1.1/sparkback/__init__.py
+-rw-r--r--   0        0        0     2059 2023-07-31 22:44:53.321985 sparkback-0.1.1/sparkback/spark.py
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 sparkback-0.1.1/PKG-INFO
```

### Comparing `sparkback-0.1.0/LICENSE.txt` & `sparkback-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparkback-0.1.0/sparkback/spark.py` & `sparkback-0.1.1/sparkback/spark.py`

 * *Files identical despite different names*

