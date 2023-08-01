# Comparing `tmp/jrpyoop-0.1.7.tar.gz` & `tmp/jrpyoop-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jrpyoop-0.1.7.tar", last modified: Thu Sep  3 14:51:10 2020, max compression
+gzip compressed data, was "jrpyoop-0.3.0.tar", max compression
```

## Comparing `jrpyoop-0.1.7.tar` & `jrpyoop-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0      127 2020-09-03 14:50:20.000000 jrpyoop-0.1.7/jrpyoop/__init__.py
--rw-r--r--   0        0        0       22 2020-09-03 14:50:20.000000 jrpyoop-0.1.7/jrpyoop/__version__.py
--rw-r--r--   0        0        0        0 2020-09-03 14:50:20.000000 jrpyoop-0.1.7/jrpyoop/datasets/__init__.py
--rw-r--r--   0        0        0    24036 2020-09-03 14:50:20.000000 jrpyoop-0.1.7/jrpyoop/vignettes/practical1.pdf
--rw-r--r--   0        0        0    34489 2020-09-03 14:50:20.000000 jrpyoop-0.1.7/jrpyoop/vignettes/solutions1.pdf
--rw-r--r--   0        0        0     1066 2020-09-03 14:50:20.000000 jrpyoop-0.1.7/jrpyoop/vignettes.py
--rw-r--r--   0        0        0      280 2020-09-03 14:50:20.000000 jrpyoop-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      707 2020-09-03 14:51:10.648750 jrpyoop-0.1.7/setup.py
--rw-r--r--   0        0        0      472 2020-09-03 14:51:10.649091 jrpyoop-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       85 2023-07-31 12:13:01.554894 jrpyoop-0.3.0/jrpyoop/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-31 12:13:01.554894 jrpyoop-0.3.0/jrpyoop/__version__.py
+-rw-r--r--   0        0        0  2828818 2023-07-31 12:13:01.558894 jrpyoop-0.3.0/jrpyoop/data/chess_games.zip
+-rw-r--r--   0        0        0  1355247 2023-07-31 12:13:01.562894 jrpyoop-0.3.0/jrpyoop/data/movies.zip
+-rw-r--r--   0        0        0      784 2023-08-01 09:49:54.380324 jrpyoop-0.3.0/jrpyoop/data.py
+-rw-r--r--   0        0        0      446 2023-08-01 09:49:54.384325 jrpyoop-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 jrpyoop-0.3.0/PKG-INFO
```

