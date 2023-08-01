# Comparing `tmp/chrislab-0.5.7.tar.gz` & `tmp/chrislab-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.7.tar", last modified: Fri Jul 21 02:14:46 2023, max compression
+gzip compressed data, was "chrislab-0.5.8.tar", last modified: Tue Aug  1 01:56:57 2023, max compression
```

## Comparing `chrislab-0.5.7.tar` & `chrislab-0.5.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.121773 chrislab-0.5.7/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-07-21 00:41:08.000000 chrislab-0.5.7/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-07-21 02:14:46.121773 chrislab-0.5.7/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-07-21 00:41:08.000000 chrislab-0.5.7/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-07-21 00:41:08.000000 chrislab-0.5.7/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1005 2023-07-21 02:14:46.121773 chrislab-0.5.7/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.113773 chrislab-0.5.7/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/chrislab/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/chrislab/common/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/common/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/common/downloader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/common/tokenizer_korbert.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11372 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/common/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/chrislab/language/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1319 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/converter.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/evaluater.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    39568 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/finetuner.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/modeling.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/predictor.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/chrislab.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1541 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      132 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       97 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/zip-safe
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/nlpbook/
--rw-rw-r--   0 chris     (1000) chris     (1000)       70 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13222 2023-07-21 01:58:50.000000 chrislab-0.5.7/src/nlpbook/arguments.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/nlpbook/cls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/cls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8835 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/cls/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5177 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/cls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2646 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/cls/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/data_utils.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/nlpbook/dp/
--rw-rw-r--   0 chris     (1000) chris     (1000)      142 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12276 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    18570 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10936 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/model.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8265 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2057 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/factory.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/nlpbook/generation/
--rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5354 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8966 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.121773 chrislab-0.5.7/src/nlpbook/ner/
--rw-rw-r--   0 chris     (1000) chris     (1000)       87 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/ner/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    18044 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/ner/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14181 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/ner/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11601 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/ner/task.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.121773 chrislab-0.5.7/src/nlpbook/paircls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/paircls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2654 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/paircls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/paircls/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.121773 chrislab-0.5.7/src/nlpbook/qa/
--rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17080 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9761 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.481448 chrislab-0.5.8/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-07-21 02:24:04.000000 chrislab-0.5.8/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-08-01 01:56:57.481448 chrislab-0.5.8/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-07-21 02:24:04.000000 chrislab-0.5.8/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-07-21 02:24:04.000000 chrislab-0.5.8/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1005 2023-08-01 01:56:57.481448 chrislab-0.5.8/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.465448 chrislab-0.5.8/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.465448 chrislab-0.5.8/src/chrislab/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.469448 chrislab-0.5.8/src/chrislab/common/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/common/__init__.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/common/downloader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/common/tokenizer_korbert.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9254 2023-07-26 23:58:04.000000 chrislab-0.5.8/src/chrislab/common/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.469448 chrislab-0.5.8/src/chrislab/language/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/language/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1319 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/language/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/language/converter.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/language/evaluater.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    39568 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/language/finetuner.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/language/modeling.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/chrislab/language/predictor.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.465448 chrislab-0.5.8/src/chrislab.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-08-01 01:56:57.000000 chrislab-0.5.8/src/chrislab.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1541 2023-08-01 01:56:57.000000 chrislab-0.5.8/src/chrislab.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-08-01 01:56:57.000000 chrislab-0.5.8/src/chrislab.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      132 2023-08-01 01:56:57.000000 chrislab-0.5.8/src/chrislab.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       97 2023-08-01 01:56:57.000000 chrislab-0.5.8/src/chrislab.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-08-01 01:56:57.000000 chrislab-0.5.8/src/chrislab.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-08-01 01:56:57.000000 chrislab-0.5.8/src/chrislab.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.473448 chrislab-0.5.8/src/nlpbook/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       70 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10518 2023-07-28 06:35:53.000000 chrislab-0.5.8/src/nlpbook/arguments.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.473448 chrislab-0.5.8/src/nlpbook/cls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/cls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8882 2023-07-25 07:59:15.000000 chrislab-0.5.8/src/nlpbook/cls/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5177 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/cls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2646 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/cls/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/data_utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.473448 chrislab-0.5.8/src/nlpbook/dp/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      142 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/dp/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12310 2023-07-25 07:59:15.000000 chrislab-0.5.8/src/nlpbook/dp/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18570 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/dp/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10936 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/dp/model.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8265 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/dp/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2059 2023-07-24 08:30:37.000000 chrislab-0.5.8/src/nlpbook/factory.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.477448 chrislab-0.5.8/src/nlpbook/generation/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/generation/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/generation/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5354 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/generation/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/generation/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/generation/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8966 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/metrics.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.477448 chrislab-0.5.8/src/nlpbook/ner/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       87 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/ner/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18130 2023-07-25 07:59:15.000000 chrislab-0.5.8/src/nlpbook/ner/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14181 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/ner/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11601 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/ner/task.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.477448 chrislab-0.5.8/src/nlpbook/paircls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/paircls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2654 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/paircls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/paircls/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-08-01 01:56:57.481448 chrislab-0.5.8/src/nlpbook/qa/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/qa/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/qa/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17080 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/qa/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/qa/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/qa/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9761 2023-07-21 02:24:04.000000 chrislab-0.5.8/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.7/LICENSE` & `chrislab-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/PKG-INFO` & `chrislab-0.5.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.7
+Version: 0.5.8
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.7/setup.cfg` & `chrislab-0.5.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.7
+version = 0.5.8
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `chrislab-0.5.7/src/chrislab/common/downloader.py` & `chrislab-0.5.8/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.8/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/chrislab/common/util.py` & `chrislab-0.5.8/src/chrislab/common/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -110,81 +110,14 @@
     elif len(_opt.rsplit('-')) >= 2:
         splits = _opt.rsplit('-', maxsplit=2)
         final['strategy'] = splits[-2] if splits[-2] in valid_strategies else default['strategy']
         final['run'] = int(number_only(splits[-1]))
     return final
 
 
-class EmptyTqdm:
-    """Dummy tqdm which doesn't do anything."""
-
-    def __init__(self, *args, **kwargs):
-        self._iterator = args[0] if args else None
-
-    def __iter__(self):
-        return iter(self._iterator)
-
-    def __getattr__(self, _):
-        def empty_fn(*args, **kwargs):
-            return
-
-        return empty_fn
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, type_, value, traceback_):
-        return
-
-
-class mute_tqdm_cls:
-    def __init__(self, *args, **kwargs):
-        pass
-
-    def __call__(self, *args, **kwargs):
-        return EmptyTqdm(*args, **kwargs)
-
-    def set_lock(self, *args, **kwargs):
-        self._lock = None
-
-    def get_lock(self):
-        pass
-
-
-class time_tqdm_cls:
-    def to_desc(self, desc, pre=None):
-        return f"- {now(prefix=self.prefix)}{f' {pre}' if pre else ''} {desc:{self.aline}{self.desc_size}s}"
-
-    def __init__(self, bar_size, desc_size, prefix=None, file=stdout, aline='right'):
-        self.desc_size = desc_size
-        self.bar_size = bar_size
-        self.prefix = prefix
-        self.file = file
-        self.aline = '<' if str(aline).strip().lower() == 'left' else '>'
-
-    def __call__(self, *args, **kwargs):
-        if 'desc' not in kwargs or not kwargs['desc'] or ('position' in kwargs and kwargs['position'] and kwargs['position'] > 0):
-            return EmptyTqdm(*args, **kwargs)
-        else:
-            if kwargs['desc'].endswith(' #0'):
-                kwargs['desc'] = kwargs['desc'][:-3]
-            kwargs['desc'] = self.to_desc(desc=kwargs['desc'],
-                                          pre=kwargs.pop('pre') if 'pre' in kwargs else None)
-            kwargs.pop('file', None)
-            kwargs.pop('bar_format', None)
-            return tqdm_std.tqdm(*args, bar_format=f"{{l_bar}}{{bar:{self.bar_size}}}{{r_bar}}", file=self.file, **kwargs)
-
-    def set_lock(self, *args, **kwargs):
-        self._lock = None
-        return tqdm_std.tqdm.set_lock(*args, **kwargs)
-
-    def get_lock(self):
-        return tqdm_std.tqdm.get_lock()
-
-
 def limit_num_samples(num, num_max, num_min=1):
     if isinstance(num, int):
         return min(max(num_min, num), num_max)
     elif isinstance(num, float):
         return min(max(num_min, int(num * num_max)), num_max)
     else:
         raise ValueError(f"Given number should be int or float: given_num={num}")
@@ -201,15 +134,15 @@
     def __init__(self, mute=True):
         self.mute = mute
 
     def __enter__(self):
         if self.mute:
             datasets.utils.logging.disable_progress_bar()
 
-    def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
+    def __exit__(self, *exc_info):
         if self.mute:
             datasets.utils.logging.enable_progress_bar()
 
 
 class StageMarker:
     time_fmt = '[%m.%d %H:%M:%S]'
 
@@ -229,17 +162,16 @@
         self.log_file = log_file
 
     def __enter__(self) -> "StageMarker":
         self.mongo = MongoClient(host=self.host, port=self.port)
         self.table = self.mongo[self.db_name][self.tab_name]
         return self
 
-    def __exit__(self, type_, value, traceback_) -> None:
+    def __exit__(self, *exc_info):
         self.mongo.close()
-        return
 
     @classmethod
     def _at_func(cls):
         return lambda: now(fmt=StageMarker.time_fmt)
 
     def _by_func(self):
         return lambda: f'#{self.node_idx + 1:01d}'
```

### Comparing `chrislab-0.5.7/src/chrislab/language/cli.py` & `chrislab-0.5.8/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/chrislab/language/converter.py` & `chrislab-0.5.8/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/chrislab/language/evaluater.py` & `chrislab-0.5.8/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/chrislab/language/finetuner.py` & `chrislab-0.5.8/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/chrislab/language/modeling.py` & `chrislab-0.5.8/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/chrislab/language/predictor.py` & `chrislab-0.5.8/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.8/src/chrislab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.7
+Version: 0.5.8
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.7/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.8/src/chrislab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/arguments.py` & `chrislab-0.5.8/src/nlpbook/arguments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,31 @@
 import logging
 import math
 import os
 from dataclasses import dataclass, field
-from datetime import datetime
 from pathlib import Path
 from typing import List
 
 import pandas as pd
 import pytorch_lightning
 import transformers
-import typer
 from dataclasses_json import DataClassJsonMixin
 from pytorch_lightning.accelerators import Accelerator
 from pytorch_lightning.loggers import CSVLogger
 from pytorch_lightning.strategies import Strategy
 
-from chrisbase.data import TypedData, ProjectEnv
-from chrisbase.io import files, make_parent_dir, hr, str_table, out_hr, out_table, configure_dual_logger, LoggingFormat
-from chrisbase.time import now, str_delta
+from chrisbase.data import ProjectEnv, OptionData, ResultData, CommonArguments
+from chrisbase.io import files, configure_dual_logger, LoggingFormat
+from chrisbase.time import now
 from chrisbase.util import to_dataframe
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
-class OptionData(TypedData):
-    def __post_init__(self):
-        super().__post_init__()
-
-
-@dataclass
-class ResultData(TypedData):
-    def __post_init__(self):
-        super().__post_init__()
-
-
-@dataclass
-class ArgumentGroupData(TypedData):
-    tag = None
-
-    def __post_init__(self):
-        super().__post_init__()
-
-
-@dataclass
 class DataFiles(DataClassJsonMixin):
     train: str | Path | None = field(default=None)
     valid: str | Path | None = field(default=None)
     test: str | Path | None = field(default=None)
 
 
 @dataclass
@@ -73,15 +51,14 @@
 
     def __post_init__(self):
         self.home = Path(self.home)
 
 
 @dataclass
 class HardwareOption(OptionData):
-    # cpu_workers: int = field(default=0)
     cpu_workers: int = field(default=os.cpu_count())
     accelerator: str | Accelerator = field(default="auto")  # possbile value: "cpu", "gpu", "tpu", "ipu", "hpu", "mps", "auto"
     batch_size: int = field(default=32)
     precision: int | str = field(default=32)  # floating-point precision type
     strategy: str | Strategy = field(default="auto")  # multi-device strategies
     devices: List[int] | int | str = field(default="auto")  # devices to use
 
@@ -104,48 +81,25 @@
     seed: int | None = field(default=None)  # random seed
 
     def __post_init__(self):
         self.validate_on = math.fabs(self.validate_on)
 
 
 @dataclass
-class TimeChecker(ResultData):
-    t1 = datetime.now()
-    t2 = datetime.now()
-    started: str | None = field(default=None)
-    settled: str | None = field(default=None)
-    elapsed: str | None = field(default=None)
-
-    def set_started(self):
-        self.started = now()
-        self.settled = None
-        self.elapsed = None
-        self.t1 = datetime.now()
-        return self
-
-    def set_settled(self):
-        self.t2 = datetime.now()
-        self.settled = now()
-        self.elapsed = str_delta(self.t2 - self.t1)
-        return self
-
-
-@dataclass
 class ProgressChecker(ResultData):
     result: dict = field(init=False, default_factory=dict)
+    csv_logger: CSVLogger = field(init=False, default=None)
     global_step: int = field(init=False, default=0)
     global_epoch: float = field(init=False, default=0.0)
     epoch_per_step: float = field(init=False, default=0.0)
 
 
 @dataclass
-class CommonArguments(ArgumentGroupData):
-    tag = "common"
-    env: ProjectEnv = field()
-    time: TimeChecker = field(default=TimeChecker())
+class MLArguments(CommonArguments):
+    tag = None
     prog: ProgressChecker = field(default=ProgressChecker())
     data: DataOption | None = field(default=None)
     model: ModelOption | None = field(default=None)
 
     def __post_init__(self):
         super().__post_init__()
         if not self.env.logging_file.stem.endswith(self.tag):
@@ -157,62 +111,42 @@
         if self.data and self.model:
             self.env.output_home = self.model.home / self.data.name
         elif self.data:
             self.env.output_home = self.env.output_home / self.data.home
         configure_dual_logger(level=self.env.msg_level, fmt=self.env.msg_format, datefmt=self.env.date_format,
                               filename=self.env.output_home / self.env.logging_file)
 
-    def reconfigure_output(self, version=None):
+    def configure_csv_logger(self, version=None):
         if not version:
             version = now('%m%d.%H%M%S')
-        self.env.csv_logger = CSVLogger(self.model.home, name=self.data.name,
-                                        version=f'{self.tag}-{self.env.job_name}-{version}',
-                                        flush_logs_every_n_steps=1)
+        self.prog.csv_logger = CSVLogger(self.model.home, name=self.data.name,
+                                         version=f'{self.tag}-{self.env.job_name}-{version}',
+                                         flush_logs_every_n_steps=1)
         existing_file = self.env.output_home / self.env.logging_file
         existing_content = existing_file.read_text() if existing_file.exists() else None
-        self.env.output_home = Path(self.env.csv_logger.log_dir)
+        existing_file.unlink(missing_ok=True)
+        self.env.output_home = Path(self.prog.csv_logger.log_dir)
         configure_dual_logger(level=self.env.msg_level, fmt=self.env.msg_format, datefmt=self.env.date_format,
                               filename=self.env.output_home / self.env.logging_file, existing_content=existing_content)
-        existing_file.unlink(missing_ok=True)
-        return self
-
-    def save_arguments(self, to: Path | str = None) -> Path | None:
-        if not self.env.output_home:
-            return None
-        args_file = to if to else self.env.output_home / self.env.argument_file
-        args_json = self.to_json(default=str, ensure_ascii=False, indent=2)
-        make_parent_dir(args_file).write_text(args_json, encoding="utf-8")
-        return args_file
-
-    def info_arguments(self):
-        table = str_table(self.dataframe(), tablefmt="presto")  # "plain", "presto"
-        for line in table.splitlines() + [hr(c='-')]:
-            logger.info(line)
         return self
 
     def dataframe(self, columns=None) -> pd.DataFrame:
         if not columns:
             columns = [self.data_type, "value"]
         return pd.concat([
             to_dataframe(columns=columns, raw=self.env, data_prefix="env"),
             to_dataframe(columns=columns, raw=self.time, data_prefix="time"),
             to_dataframe(columns=columns, raw=self.prog, data_prefix="prog"),
-            to_dataframe(columns=columns, raw=self.data, data_prefix="data"),
-            to_dataframe(columns=columns, raw=self.model, data_prefix="model"),
+            to_dataframe(columns=columns, raw=self.data, data_prefix="data") if self.data else None,
+            to_dataframe(columns=columns, raw=self.model, data_prefix="model") if self.model else None,
         ]).reset_index(drop=True)
 
-    def show(self):  # TODO: Remove someday
-        out_hr(c='-')
-        out_table(self.dataframe())
-        out_hr(c='-')
-        return self
-
 
 @dataclass
-class ServerArguments(CommonArguments):
+class ServerArguments(MLArguments):
     tag = "serve"
 
     def __post_init__(self):
         super().__post_init__()
         if self.tag in ("serve", "test"):
             assert self.model.home.exists() and self.model.home.is_dir(), \
                 f"No finetuning home: {self.model.home}"
@@ -295,15 +229,15 @@
         pretrained = Path(pretrained)
         return TrainerArguments(
             env=ProjectEnv(
                 project=project,
                 job_name=job_name if job_name else pretrained.name,
                 debugging=debugging,
                 msg_level=logging.DEBUG if debugging else logging.INFO,
-                msg_format=LoggingFormat.DEBUG if debugging else LoggingFormat.CHECK,
+                msg_format=LoggingFormat.DEBUG_48 if debugging else LoggingFormat.CHECK_48,
             ),
             data=DataOption(
                 home=data_home,
                 name=data_name,
                 files=DataFiles(
                     train=train_file,
                     valid=valid_file,
@@ -330,41 +264,7 @@
                 num_save=num_save,
                 save_by=save_by,
                 epochs=epochs,
                 lr=lr,
                 seed=seed,
             ),
         )
-
-
-class AppTyper(typer.Typer):
-    def __init__(self):
-        super().__init__(
-            add_completion=False,
-            pretty_exceptions_enable=False,
-        )
-
-
-class ArgumentsUsing:
-    def __init__(self, args: CommonArguments, delete_on_exit: bool = True):
-        self.args: CommonArguments = args
-        self.delete_on_exit: bool = delete_on_exit
-
-    def __enter__(self) -> Path:
-        self.args_file: Path | None = self.args.save_arguments()
-        return self.args_file
-
-    def __exit__(self, *exc_info):
-        if self.delete_on_exit and self.args_file:
-            self.args_file.unlink(missing_ok=True)
-
-
-class RuntimeChecking:
-    def __init__(self, args: CommonArguments):
-        self.args: CommonArguments = args
-
-    def __enter__(self):
-        self.args.time.set_started()
-
-    def __exit__(self, *exc_info):
-        self.args.time.set_settled()
-        self.args.save_arguments(self.args.env.output_home / self.args.env.argument_file)
```

### Comparing `chrislab-0.5.7/src/nlpbook/cls/cli.py` & `chrislab-0.5.8/src/nlpbook/cls/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 from torch.utils.data import DataLoader, RandomSampler
 from torch.utils.data import SequentialSampler
 from transformers import BertConfig, BertForSequenceClassification, BertTokenizer
 from transformers.modeling_outputs import SequenceClassifierOutput
 from typer import Typer
 
 import nlpbook
+from chrisbase.data import RuntimeChecking
 from chrisbase.io import JobTimer, err_hr
-from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
+from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments
 from nlpbook.cls.corpus import NsmcCorpus, ClassificationDataset
 from nlpbook.cls.task import ClassificationTask
 
 app = Typer()
 logger = logging.getLogger(__name__)
 
 
 @app.command()
 def train(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
-    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
+    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).info_args()
     nlpbook.set_seed(args)
 
     with JobTimer(f"chrialab.nlpbook.cls train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         if not (args.data.home / args.data.name).exists() or not (args.data.home / args.data.name).is_dir():
             Korpora.fetch(
                 corpus_name=args.data.name,
                 root_dir=args.data.home,
@@ -65,28 +66,28 @@
         )
         model = BertForSequenceClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config,
         )
         err_hr(c='-')
 
-        with RuntimeChecking(args.reconfigure_output()):
+        with RuntimeChecking(args.configure_csv_logger()):
             torch.set_float32_matmul_precision('high')
             trainer: Trainer = nlpbook.make_trainer(args)
             trainer.fit(ClassificationTask(model, args, trainer),
                         train_dataloaders=train_dataloader,
                         val_dataloaders=val_dataloader)
 
 
 @app.command()
 def test(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
-    args: TesterArguments = TesterArguments.from_json(args_file.read_text()).show()
+    args: TesterArguments = TesterArguments.from_json(args_file.read_text()).info_args()
 
     with JobTimer(f"chrialab.nlpbook.cls test {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         checkpoint_path = args.env.output_home / args.model.name
         assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
         logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
         err_hr(c='-')
 
@@ -116,28 +117,28 @@
         )
         model = BertForSequenceClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config,
         )
         err_hr(c='-')
 
-        with RuntimeChecking(args.reconfigure_output()):
+        with RuntimeChecking(args.configure_csv_logger()):
             torch.set_float32_matmul_precision('high')
             tester: Trainer = nlpbook.make_tester(args)
             tester.test(ClassificationTask(model, args, tester),
                         dataloaders=test_dataloader,
                         ckpt_path=checkpoint_path)
 
 
 @app.command()
 def serve(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file file: {args_file}"
-    args: ServerArguments = ServerArguments.from_json(args_file.read_text()).show()
+    args: ServerArguments = ServerArguments.from_json(args_file.read_text()).info_args()
 
     with JobTimer(f"chrialab.nlpbook serve_cls {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         checkpoint_path = args.env.output_home / args.model.name
         assert checkpoint_path.exists(), f"No downstream model file: {checkpoint_path}"
         checkpoint: dict = torch.load(checkpoint_path, map_location=torch.device("cpu"))
         logger.info(f"Using finetuned model file at {checkpoint_path}")
         err_hr(c='-')
@@ -173,12 +174,12 @@
                 'prediction': pred,
                 'positive_data': f"긍정 {positive_prob:.4f}",
                 'negative_data': f"부정 {negative_prob:.4f}",
                 'positive_width': f"{positive_prob * 100}%",
                 'negative_width': f"{negative_prob * 100}%",
             }
 
-        with RuntimeChecking(args.reconfigure_output()):
+        with RuntimeChecking(args.configure_csv_logger()):
             server: Flask = nlpbook.make_server(inference_fn,
                                                 template_file="serve_cls.html",
                                                 ngrok_home=args.env.working_path)
             server.run()
```

### Comparing `chrislab-0.5.7/src/nlpbook/cls/corpus.py` & `chrislab-0.5.8/src/nlpbook/cls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/cls/task.py` & `chrislab-0.5.8/src/nlpbook/cls/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/data_utils.py` & `chrislab-0.5.8/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/dp/cli.py` & `chrislab-0.5.8/src/nlpbook/dp/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 import lightning as L
 import torch
 import torch.nn.functional as F
 from torch.utils.data import DataLoader, RandomSampler, SequentialSampler
 from transformers import PreTrainedTokenizerFast, AutoTokenizer, AutoConfig, AutoModel, BertConfig, BertModel, RobertaConfig, RobertaModel, PreTrainedModel, PretrainedConfig
 from typer import Typer
 
+from chrisbase.data import RuntimeChecking
 from chrisbase.io import JobTimer, pop_keys, err_hr
 from chrislab.common.util import time_tqdm_cls, mute_tqdm_cls
 from nlpbook import save_checkpoint
-from nlpbook.arguments import TrainerArguments, RuntimeChecking
+from nlpbook.arguments import TrainerArguments
 from nlpbook.dp.corpus import DPCorpus, DPDataset
 from nlpbook.dp.model import ModelForDependencyParsing
 from nlpbook.metrics import DPResult
 
 app = Typer()
 logger = logging.getLogger(__name__)
 term_pattern = re.compile(re.escape("{") + "(.+?)(:.+?)?" + re.escape("}"))
 
 
 @app.command()
 def fabric_train(args_file: Path | str):
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
-    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
+    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).info_args()
     L.seed_everything(args.learning.seed)
 
     with JobTimer(f"chrialab.nlpbook.dp fabric_train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         # Data
         tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, use_fast=True)
         assert isinstance(tokenizer, PreTrainedTokenizerFast), f"Our code support only PreTrainedTokenizerFast, but used {type(tokenizer)}"
         corpus = DPCorpus(args)
@@ -76,22 +77,22 @@
         err_hr(c='-')
 
         # Optimizer
         optimizer = torch.optim.AdamW(model.parameters(), lr=args.learning.lr)
         scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer, gamma=0.9)
 
         # Fabric
-        with RuntimeChecking(args.reconfigure_output()):
+        with RuntimeChecking(args.configure_csv_logger()):
             torch.set_float32_matmul_precision('high')
             fabric = L.Fabric(
                 accelerator=args.hardware.accelerator,
                 precision=args.hardware.precision,
                 strategy=args.hardware.strategy,
                 devices=args.hardware.devices,
-                loggers=args.env.csv_logger,
+                loggers=args.prog.csv_logger,
             )
             fabric.setup(model, optimizer)
             train_dataloader, valid_dataloader = fabric.setup_dataloaders(train_dataloader, valid_dataloader)
             train_with_fabric(fabric, args, model, optimizer, scheduler, train_dataloader, valid_dataloader, valid_dataset)
 
 
 def train_with_fabric(fabric: L.Fabric, args: TrainerArguments, model: ModelForDependencyParsing,
```

### Comparing `chrislab-0.5.7/src/nlpbook/dp/corpus.py` & `chrislab-0.5.8/src/nlpbook/dp/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/dp/model.py` & `chrislab-0.5.8/src/nlpbook/dp/model.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/dp/task.py` & `chrislab-0.5.8/src/nlpbook/dp/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/factory.py` & `chrislab-0.5.8/src/nlpbook/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         dirpath=args.env.output_home,
         filename=args.model.name,
         save_top_k=args.learning.num_save,
         monitor=args.learning.save_by.split()[1],
         mode=args.learning.save_by.split()[0],
     )
     trainer = Trainer(
-        logger=args.env.csv_logger,
+        logger=args.prog.csv_logger,
         devices=args.hardware.devices,
         strategy=args.hardware.strategy,
         precision=args.hardware.precision,
         accelerator=args.hardware.accelerator,
         deterministic=torch.cuda.is_available() and args.learning.seed is not None,
         log_every_n_steps=1,
         # enable_progress_bar=False,
@@ -29,15 +29,15 @@
         callbacks=[checkpoint_callback],
     )
     return trainer
 
 
 def make_tester(args: TesterArguments) -> Trainer:
     tester = Trainer(
-        logger=args.env.csv_logger,
+        logger=args.prog.csv_logger,
         devices=args.hardware.devices,
         strategy=args.hardware.strategy,
         precision=args.hardware.precision,
         accelerator=args.hardware.accelerator,
         # enable_progress_bar=False,
     )
     return tester
```

### Comparing `chrislab-0.5.7/src/nlpbook/generation/arguments.py` & `chrislab-0.5.8/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/generation/corpus.py` & `chrislab-0.5.8/src/nlpbook/generation/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/generation/deploy.py` & `chrislab-0.5.8/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/generation/task.py` & `chrislab-0.5.8/src/nlpbook/generation/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/metrics.py` & `chrislab-0.5.8/src/nlpbook/metrics.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/ner/cli.py` & `chrislab-0.5.8/src/nlpbook/ner/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import logging
 import sys
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
 import lightning as L
+import pytorch_lightning as pl
 import torch
 from flask import Flask
 from torch import Tensor
 from torch.utils.data import DataLoader, RandomSampler, SequentialSampler
 from transformers import PreTrainedTokenizerFast, AutoTokenizer, AutoConfig, AutoModelForTokenClassification, BertForTokenClassification, CharSpan
 from transformers.modeling_outputs import TokenClassifierOutput
 from typer import Typer
 
 import nlpbook
+from chrisbase.data import RuntimeChecking
 from chrisbase.io import JobTimer, pop_keys, err_hr, out_hr
 from chrislab.common.util import time_tqdm_cls, mute_tqdm_cls
 from nlpbook import save_checkpoint, TERM_IN_NAME_FORMAT
-from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
+from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments
 from nlpbook.metrics import accuracy, klue_ner_char_macro_f1, klue_ner_entity_macro_f1
 from nlpbook.ner.corpus import NERCorpus, NERDataset, NEREncodedExample
 from nlpbook.ner.task import NERTask
 
 app = Typer()
 logger = logging.getLogger(__name__)
 
 
 @app.command()
 def fabric_train(args_file: Path | str):
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
-    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
+    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).info_args()
     L.seed_everything(args.learning.seed)
 
     with JobTimer(f"chrialab.nlpbook.ner fabric_train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         # Data
         tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, use_fast=True)
         assert isinstance(tokenizer, PreTrainedTokenizerFast), f"Our code support only PreTrainedTokenizerFast, but used {type(tokenizer)}"
         corpus = NERCorpus(args=args)
@@ -71,17 +73,17 @@
         err_hr(c='-')
 
         # Optimizer
         optimizer = torch.optim.AdamW(model.parameters(), lr=args.learning.lr)
         scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer, gamma=0.9)
 
         # Fabric
-        with RuntimeChecking(args.reconfigure_output()):
+        with RuntimeChecking(args.configure_csv_logger()):
             torch.set_float32_matmul_precision('high')
-            fabric = L.Fabric(loggers=args.env.csv_logger)
+            fabric = L.Fabric(loggers=args.prog.csv_logger)
             fabric.setup(model, optimizer)
             train_dataloader, valid_dataloader = fabric.setup_dataloaders(train_dataloader, valid_dataloader)
             train_with_fabric(fabric, args, model, optimizer, scheduler, train_dataloader, valid_dataloader, valid_dataset)
 
 
 def train_with_fabric(fabric: L.Fabric, args: TrainerArguments, model: torch.nn.Module,
                       optimizer: torch.optim.Optimizer, scheduler: torch.optim.lr_scheduler._LRScheduler,
@@ -180,15 +182,15 @@
 
 
 @app.command()
 def train(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
-    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
+    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).info_args()
     nlpbook.set_seed(args)
 
     with JobTimer(f"chrialab.nlpbook.ner train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         if args.data.redownload:
             nlpbook.download_downstream_dataset(args)
             err_hr(c='-')
 
@@ -217,29 +219,29 @@
         )
         model = AutoModelForTokenClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config
         )
         err_hr(c='-')
 
-        with RuntimeChecking(args.reconfigure_output()):
+        with RuntimeChecking(args.configure_csv_logger()):
             torch.set_float32_matmul_precision('high')
             trainer: pl.Trainer = nlpbook.make_trainer(args)
             trainer.fit(NERTask(model=model, args=args, trainer=trainer, valid_dataset=val_dataset,
                                 total_steps=len(train_dataloader) * args.learning.epochs),
                         train_dataloaders=train_dataloader,
                         val_dataloaders=val_dataloader)
 
 
 @app.command()
 def test(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
-    args = TesterArguments.from_json(args_file.read_text()).show()
+    args = TesterArguments.from_json(args_file.read_text()).info_args()
 
     with JobTimer(f"chrialab.nlpbook.ner test {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         checkpoint_path = args.env.output_home / args.model.name
         assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
         logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
         err_hr(c='-')
 
@@ -263,28 +265,28 @@
             num_labels=corpus.num_labels
         )
         model = AutoModelForTokenClassification.from_pretrained(
             args.model.pretrained,
             config=pretrained_model_config
         )
         err_hr(c='-')
-    with RuntimeChecking(args.reconfigure_output()):
+    with RuntimeChecking(args.configure_csv_logger()):
         torch.set_float32_matmul_precision('high')
         tester: pl.Trainer = nlpbook.make_tester(args)
         tester.test(NERTask(model, args, tester),
                     dataloaders=test_dataloader,
                     ckpt_path=checkpoint_path)
 
 
 @app.command()
 def serve(args_file: Path | str):
     nlpbook.set_logger()
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file file: {args_file}"
-    args: ServerArguments = ServerArguments.from_json(args_file.read_text()).show()
+    args: ServerArguments = ServerArguments.from_json(args_file.read_text()).info_args()
 
     with JobTimer(f"chrialab.nlpbook serve_ner {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         checkpoint_path = args.env.output_home / args.model.name
         assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
         checkpoint: dict = torch.load(checkpoint_path, map_location=torch.device("cpu"))
         logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
         err_hr(c='-')
@@ -328,12 +330,12 @@
                         "prob": f"{round(top_prob[0].item(), 4):.4f}",
                     })
             return {
                 'sentence': sentence,
                 'result': result,
             }
 
-        with RuntimeChecking(args.reconfigure_output()):
+        with RuntimeChecking(args.configure_csv_logger()):
             server: Flask = nlpbook.make_server(inference_fn,
                                                 template_file="serve_ner.html",
                                                 ngrok_home=args.env.working_path)
             server.run()
```

### Comparing `chrislab-0.5.7/src/nlpbook/ner/corpus.py` & `chrislab-0.5.8/src/nlpbook/ner/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/ner/task.py` & `chrislab-0.5.8/src/nlpbook/ner/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/paircls/corpus.py` & `chrislab-0.5.8/src/nlpbook/paircls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/paircls/deploy.py` & `chrislab-0.5.8/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/qa/arguments.py` & `chrislab-0.5.8/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/qa/corpus.py` & `chrislab-0.5.8/src/nlpbook/qa/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/qa/deploy.py` & `chrislab-0.5.8/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/qa/task.py` & `chrislab-0.5.8/src/nlpbook/qa/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.7/src/nlpbook/utils.py` & `chrislab-0.5.8/src/nlpbook/utils.py`

 * *Files identical despite different names*

