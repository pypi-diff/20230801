# Comparing `tmp/pina-mathlab-0.0.3.tar.gz` & `tmp/pina-mathlab-0.0.3.post2308.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PINA/PINA/dist/.tmp-xxd368s9/pina-mathlab-0.0.3.tar", last modified: Tue Jul  4 11:39:51 2023, max compression
+gzip compressed data, was "/home/runner/work/PINA/PINA/dist/.tmp-1ehqqzhu/pina-mathlab-0.0.3.post2308.tar", last modified: Tue Aug  1 02:52:29 2023, max compression
```

## Comparing `pina-mathlab-0.0.3.tar` & `pina-mathlab-0.0.3.post2308.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/adaptive_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_cos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_sin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_softplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_square.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/chebyshev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/label_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/location.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/model/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/deeponet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/feed_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/model/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/convolution_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/integral.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/stride.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/layers/utils_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/multi_feed_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/model/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/pinn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina/problem/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/parametric_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/spatial_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/problem/timedep_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/span.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/pina/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/pina_mathlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:39:51.000000 pina-mathlab-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_deeponet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_fnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_label_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_pinn.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-04 11:39:39.000000 pina-mathlab-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_cos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_sin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_softplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_square.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/label_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/deeponet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/feed_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina/model/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/layers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/layers/convolution_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/layers/integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/layers/stride.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/layers/utils_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/multi_feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/model/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/pinn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/problem/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/problem/parametric_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/problem/spatial_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/problem/timedep_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/pina/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:52:29.000000 pina-mathlab-0.0.3.post2308/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_deeponet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_fnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_label_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_pinn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-01 02:52:19.000000 pina-mathlab-0.0.3.post2308/tests/test_utils.py
```

### Comparing `pina-mathlab-0.0.3/LICENSE.rst` & `pina-mathlab-0.0.3.post2308/LICENSE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021-2021 PINA contributors
+Copyright (c) 2021-current PINA contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pina-mathlab-0.0.3/PKG-INFO` & `pina-mathlab-0.0.3.post2308/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pina-mathlab
-Version: 0.0.3
+Version: 0.0.3.post2308
 Summary: Physic Informed Neural networks for Advance modeling.
 Home-page: https://github.com/mathLab/PINA
 Author: Nicola Demo, Maria Strazzullo
 Author-email: demo.nicola@gmail.com, 
 License: MIT
 Keywords: physics-informed neural-network
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pina-mathlab-0.0.3/README.md` & `pina-mathlab-0.0.3.post2308/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,175 @@
-<p align="center">
-    <a href="http://mathlab.github.io/PINA/" target="_blank" >
-    <img alt="Physics-Informed Neural networks for Advanced modeling" src="readme/pina_logo.png" width="200" />
-    </a>
-</p>
-<p align="center">
-    <a href="https://github.com/mathLab/PINA/blob/master/LICENSE" target="_blank">
-        <img alt="Software License" src="https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square">
-    </a>
-    <a href="https://badge.fury.io/py/pina-mathlab">
-	<img src="https://badge.fury.io/py/pina-mathlab.svg" alt="PyPI version" height="18">
-    </a>
-    <a href="https://github.com/mathLab/PINA/actions/workflows/ci.yml" target="_blank">
-        <img alt="Build Status" src="https://github.com/mathLab/PINA/actions/workflows/ci.yml/badge.svg">
-    </a>
-    <a href="https://www.codacy.com/gh/mathLab/PINA/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mathLab/PINA&amp;utm_campaign=Badge_Grade">
-	<img src="https://app.codacy.com/project/badge/Grade/1ed0b0279cbe44cc8207575fe6e55f91"/>
+<!-- PROJECT SHIELDS -->
+<!--
+*** I'm using markdown "reference style" links for readability.
+*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
+*** See the bottom of this document for the declaration of the reference variables
+*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
+*** https://www.markdownguide.org/basic-syntax/#reference-style-links
+-->
+
+<div align="center">
+
+[![PyPi][pypi-shield]][pypi-url]
+[![PyPi][pypiversion-shield]][pypi-url]
+[![PyPi][downloads-shield]][downloads-url]
+[![License][license-shield]][license-url]
+
+</div>
+<!-- [![Contributors][contributors-shield]][contributors-url] -->
+<!-- [![Build][build-shield]][build-url] -->
+<!-- [![CodeCov][codecov-shield]][codecov-url] -->
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+
+[pypi-shield]: https://img.shields.io/pypi/pyversions/pina-mathlab?style=for-the-badge
+
+[pypi-url]: https://pypi.org/project/pina-mathlab/
+
+[pypiversion-shield]: https://img.shields.io/pypi/v/pina-mathlab?style=for-the-badge
+
+[downloads-shield]: https://img.shields.io/pypi/dm/pina-mathlab?style=for-the-badge
+
+[downloads-url]: https://pypi.org/project/pina-mathlab/
+
+[codecov-shield]: https://img.shields.io/codecov/c/gh/zenml-io/zenml?style=for-the-badge
+
+[codecov-url]: https://codecov.io/gh/zenml-io/zenml
+
+[contributors-shield]: https://img.shields.io/github/contributors/zenml-io/zenml?style=for-the-badge
+
+[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
+
+[license-shield]: https://img.shields.io/github/license/mathLab/pina?style=for-the-badge
+
+[license-url]: https://github.com/mathLab/PINA/blob/main/LICENSE.rst
+
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+
+<!-- [linkedin-url]: https://www.linkedin.com/company/zenml/
+
+[twitter-shield]: https://img.shields.io/twitter/follow/zenml_io?style=for-the-badge
+
+[twitter-url]: https://twitter.com/zenml_io -->
+
+[slack-shield]: https://img.shields.io/badge/-Slack-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+
+[slack-url]: https://zenml.io/slack-invite
+
+[build-shield]: https://img.shields.io/github/workflow/status/zenml-io/zenml/Build,%20Lint,%20Unit%20&%20Integration%20Test/develop?logo=github&style=for-the-badge
+
+[build-url]: https://github.com/zenml-io/zenml/actions/workflows/ci.yml
+
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://zenml.io">
+    <img alt="ZenML Logo" src="https://github.com/mathLab/PINA/raw/master/readme/pina_logo.png" alt="Logo" width="200">
+  </a>
+
+<h3 align="center">Solve equations, intuitively.</h3>
+
+  <p align="center">
+    A simple framework to solve difficult problems with neural networks.
+    <br />
+    <a href="https://mathlab.github.io/PINA/"><strong>Explore the docs »</strong></a>
+    <br />
+    <!-- <div align="center">
+      Join our <a href="https://zenml.io/slack-invite" target="_blank">
+      <img width="25" src="https://cdn3.iconfinder.com/data/icons/logos-and-brands-adobe/512/306_Slack-512.png" alt="Slack"/>
+    <b>Slack Community</b> </a> and be part of the ZenML family.
+    </div> -->
+    <br />
+    <!-- <a href="https://zenml.io/features">Features</a>
+    ·
+    <a href="https://zenml.io/roadmap">Roadmap</a>
+    ·
+    <a href="https://github.com/zenml-io/zenml/issues">Report Bug</a>
+    ·
+    <a href="https://zenml.io/discussion">Vote New Features</a>
+    ·
+    <a href="https://blog.zenml.io/">Read Blog</a>
+    ·
+    <a href="#-meet-the-team">Meet the Team</a> -->
+    <!-- <br />
+    🎉 Version 0.41.0 is out. Check out the release notes
+    <a href="https://github.com/zenml-io/zenml/releases">here</a>.
+    <br />
+    <br />
+    <a href="https://www.linkedin.com/company/zenml/">
+    <img src="https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555" alt="Logo">
     </a>
-    <a href="https://www.codacy.com/gh/mathLab/PINA/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mathLab/PINA&amp;utm_campaign=Badge_Coverage">
-	<img src="https://app.codacy.com/project/badge/Coverage/1ed0b0279cbe44cc8207575fe6e55f91"/>
+    <a href="https://twitter.com/zenml_io">
+    <img src="https://img.shields.io/badge/-Twitter-black.svg?style=for-the-badge&logo=twitter&colorB=555" alt="Logo">
     </a>
-</p>
+    <a href="https://www.youtube.com/c/ZenML">
+    <img src="https://img.shields.io/badge/-YouTube-black.svg?style=for-the-badge&logo=youtube&colorB=555" alt="Logo">
+    </a> -->
+  </p>
+</div>
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>🏁 Table of Contents</summary>
+  <ol>
+    <li><a href="#-introduction">Introduction</a></li>
+    <li><a href="#-quickstart">Quickstart</a></li>
+    <li>
+      <a href="#%EF%B8%8F-solve-your-differential-problem">Solve Your Differential Problem</a>
+      <ul>
+        <li><a href="#-1-formulate-the-problem">Formulate the Problem</a></li>
+        <li><a href="#-2-solve-the-problem">Solve the Problem</a></li>
+      </ul>
+    </li>
+    <!-- <li><a href="#-roadmap">Roadmap</a></li> -->
+    <li><a href="#-contributing-and-community">Contributing and Community</a></li>
+    <!-- <li><a href="#-getting-help">Getting Help</a></li> -->
+    <li><a href="#-license">License</a></li>
+  </ol>
+</details>
+
+<br />
+
+# 🤖 Introduction
+
+🤹 PINA is a Python package providing an easy interface to deal with *physics-informed neural networks* (PINN) for the approximation of (differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a simple and intuitive way to formalize a specific problem and solve it using PINN.
+
+- 👨‍💻 Formulate your differential problem in few lines of code, just translating the mathematical equations into Python
+
+- 📄 Training your neural network in order to solve the problem
+
+- 🚀  Use the model to visualize and analyze the solution!
 
 
-**PINA**: Physics-Informed Neural networks for Advanced modeling
+<br>
 
-## Table of contents
-* [Description](#description)
-     * [Problem definition](#problem-definition)
-     * [Problem solution](#problem-solution)
-* [Dependencies and installation](#dependencies-and-installation)
-	* [Installing via PIP](#installing-via-pip)
-	* [Installing from source](#installing-from-source)
-<!-- * [Documentation](#documentation) -->
-<!-- * [Testing](#testing) -->
-* [Examples and Tutorials](#examples-and-tutorials)
-* [References](#references)
-	<!-- * [Recent works with PyDMD](#recent-works-with-pydmd) -->
-* [Authors and contributors](#authors-and-contributors)
-* [How to contribute](#how-to-contribute)
-	* [Submitting a patch](#submitting-a-patch)
-* [License](#license)
+# 🤸 Quickstart
 
-## Description
-**PINA** is a Python package providing an easy interface to deal with *physics-informed neural networks* (PINN) for the approximation of (differential, nonlinear, ...) functions. Based on Pytorch, PINA offers a simple and intuitive way to formalize a specific problem and solve it using PINN. The approximated solution of a differential equation can be implemented using PINA in a few lines of code thanks to the intuitive and user-friendly interface.
+[Install PINA](https://mathlab.github.io/PINA/_rst/installation.html) via
+[PyPI](https://pypi.org/project/pina-mathlab/). Python 3 is required:
 
-<p align="center">
-    <a href="http://mathlab.github.io/PINA/" target="_blank" >
-    <img alt="PINA interface for solving problems." src="readme/API_color.png" width="400" />
-    </a>
-</p>
+```bash
+pip install "pina-mathlab"
+```
+<br>
+
+# 🖼️ Solve Your Differential Problem
 
+PINN is a novel approach that involves neural networks to solve supervised learning tasks while respecting any given law of physics described by general nonlinear differential equations. Proposed in [Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations](https://www.sciencedirect.com/science/article/pii/S0021999118307125?casa_token=p0BAG8SoAbEAAAAA:3H3r1G0SJ7IdXWm-FYGRJZ0RAb_T1qynSdfn-2VxqQubiSWnot5yyKli9UiH82rqQWY_Wzfq0HVV), such framework aims to solve problems in a continuous and nonlinear settings. 
 
-#### Physics-informed neural network
-PINN is a novel approach that involves neural networks to solve supervised learning tasks while respecting any given law of physics described by general nonlinear differential equations. Proposed in *"Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations"*, such framework aims to solve problems in a continuous and nonlinear settings.
+## 🔋 1. Formulate the Problem
 
-#### Problem definition
 First step is formalization of the problem in the PINA framework. We take as example here a simple Poisson problem, but PINA is already able to deal with **multi-dimensional**, **parametric**, **time-dependent** problems.
 Consider:
 
-$$\begin{cases} \Delta u = \sin(\pi x)\sin(\pi y)\quad& \text{in} \\ D \\\\ u = 0& \text{on} \\ \partial D \end{cases}$$
+$$
+\begin{cases}
+\Delta u = \sin(\pi x)\sin(\pi y)\quad& \text{in}\, D \\
+u = 0& \text{on}\, \partial D \end{cases}$$
 
 where $D = [0, 1]^2$ is a square domain, $u$ the unknown field, and $\partial D  = \Gamma_1 \cup \Gamma_2 \cup \Gamma_3 \cup \Gamma_4$, where $\Gamma_i$ are the boundaries of the square for $i=1,\cdots,4$. The translation in PINA code becomes a new class containing all the information about the domain, about the `conditions` and nothing more:
 
 ```python
 class Poisson(SpatialProblem):
     output_variables = ['u']
     spatial_domain = Span({'x': [0, 1], 'y': [0, 1]})
@@ -82,15 +189,15 @@
         'gamma2': Condition(Span({'x': [-1, 1], 'y': -1}), nil_dirichlet),
         'gamma3': Condition(Span({'x':  1, 'y': [-1, 1]}), nil_dirichlet),
         'gamma4': Condition(Span({'x': -1, 'y': [-1, 1]}), nil_dirichlet),
         'D': Condition(Span({'x': [-1, 1], 'y': [-1, 1]}), laplace_equation),
     }
 ```
 
-#### Problem solution
+## 👨‍🍳 2. Solve the Problem
 After defining it, we want of course to solve such a problem. The only things we need is a `model`, in this case a feed forward network, and some samples of the domain and boundaries, here using a Cartesian grid. In these points we are going to evaluate the residuals, which is nothing but the loss of the network.
 
 ```python
 poisson_problem = Poisson()
 
 model = FeedForward(layers=[10, 10],
                     output_variables=poisson_problem.output_variables,
@@ -104,122 +211,59 @@
 plotter = Plotter()
 plotter.plot(pinn)
 ```
 After the training we can infer our model, save it or just plot the PINN approximation. Below the graphical representation of the PINN approximation, the analytical solution of the problem and the absolute error, from left to right.
 <p align="center">
   <img alt="Poisson approximation" src="readme/poisson_plot.png" width="100%" />
 </p>
+<br>
 
+<!-- # 🗺 Roadmap
 
-## Dependencies and installation
-**PINA** requires `numpy`, `scipy`, `matplotlib`, `future`, `torch`, `sphinx` (for the documentation) and `pytest` (for local test). The code is tested for Python 3, while compatibility of Python 2 is not guaranteed anymore. It can be installed using `pip` or directly from the source code.
-
-### Installing via PIP
-Mac and Linux users can install pre-built binary packages using pip.
-To install the package just type:
-```bash
-> pip install git+https://github.com/mathLab/PINA.git
-```
-To uninstall the package:
-```bash
-> pip uninstall pina
-```
-
-### Installing from source
-The official distribution is on GitHub, and you can clone the repository using
-```bash
-> git clone https://github.com/mathLab/PINA
-```
-
-To install the package just type:
-```bash
-> pip install -e .
-```
-
-<!-- ## Documentation -->
-<!-- **PyDMD** uses [Sphinx](http://www.sphinx-doc.org/en/stable/) for code documentation. You can view the documentation online [here](http://mathlab.github.io/PyDMD/). To build the html version of the docs locally simply: -->
-
-<!-- ```bash -->
-<!-- > cd docs -->
-<!-- > make html -->
-<!-- ``` -->
-
-<!-- The generated html can be found in `docs/build/html`. Open up the `index.html` you find there to browse. -->
-
-
-<!-- ## Testing -->
+ZenML is being built in public. The [roadmap](https://zenml.io/roadmap) is a
+regularly updated source of truth for the ZenML community to understand where
+the product is going in the short, medium, and long term.
+
+ZenML is managed by a [core team](https://zenml.io/company#CompanyTeam) of
+developers that are responsible for making key decisions and incorporating
+feedback from the community. The team oversees feedback via various channels,
+and you can directly influence the roadmap as follows:
+
+- Vote on your most wanted feature on our [Discussion
+  board](https://zenml.io/discussion).
+- Start a thread in our [Slack channel](https://zenml.io/slack-invite).
+- [Create an issue](https://github.com/zenml-io/zenml/issues/new/choose) on our
+  Github repo.
+  -->
+
+# 🙌 Contributing and Community
+
+We would love to develop PINA together with our community! Best way to get
+started is to select any issue from the [`good-first-issue`
+label](https://github.com/mathLab/PINA/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22). If you
+would like to contribute, please review our [Contributing
+Guide](CONTRIBUTING.md) for all relevant details.
 
-<!-- We are using Travis CI for continuous intergration testing. You can check out the current status [here](https://travis-ci.org/mathLab/PyDMD). -->
-
-<!-- To run tests locally (`pytest` is required): -->
-
-<!-- ```bash -->
-<!-- > pytest -->
-<!-- ``` -->
-
-## Examples and Tutorials
-The directory `Examples` contains some examples showing Poisson and Burgers problems solved in the PINN context.
-
-### References
-To implement the package we follow these works:
-
-* Raissi, Maziar, Paris Perdikaris, and George E. Karniadakis.
-  *Physics-informed neural networks: A deep learning framework for solving
-  forward and inverse problems involving nonlinear partial differential
-  equations.* Journal of Computational Physics 378 (2019): 686-707.
-
-
-## Authors and contributors
-We warmly thank all the contributors that have supported PINA!
+We warmly thank all the contributors that have supported PINA so far:
 
 <a href="https://github.com/mathLab/PINA/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=mathLab/PINA" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 
-## How to contribute
-We'd love to accept your patches and contributions to this project. There are just a few small guidelines you need to follow.
-
-### Submitting a patch
+<!-- # 🆘 Getting Help
 
-  1. It's generally best to start by opening a new issue describing the bug or
-     feature you're intending to fix.  Even if you think it's relatively minor,
-     it's helpful to know what people are working on.  Mention in the initial
-     issue that you are planning to work on that bug or feature so that it can
-     be assigned to you.
-
-  2. Follow the normal process of [forking][] the project, and setup a new
-     branch to work in.  It's important that each group of changes be done in
-     separate branches in order to ensure that a pull request only includes the
-     commits related to that bug or feature.
-
-  3. To ensure properly formatted code, please make sure to use 4
-     spaces to indent the code. The easy way is to run on your bash the provided
-     script: ./code_formatter.sh. You should also run [pylint][] over your code.
-     It's not strictly necessary that your code be completely "lint-free",
-     but this will help you find common style issues.
-
-  4. Any significant changes should almost always be accompanied by tests.  The
-     project already has good test coverage, so look at some of the existing
-     tests if you're unsure how to go about it. We're using [coveralls][] that
-     is an invaluable tools for seeing which parts of your code aren't being
-     exercised by your tests.
-
-  5. Do your best to have [well-formed commit messages][] for each change.
-     This provides consistency throughout the project, and ensures that commit
-     messages are able to be formatted properly by various git tools.
-
-  6. Finally, push the commits to your fork and submit a [pull request][]. Please,
-     remember to rebase properly in order to maintain a clean, linear git history.
-
-[forking]: https://help.github.com/articles/fork-a-repo
-[pylint]: https://www.pylint.org/
-[coveralls]: https://coveralls.io
-[well-formed commit messages]: http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html
-[pull request]: https://help.github.com/articles/creating-a-pull-request
+The first point of call should
+be [our Slack group](https://zenml.io/slack-invite/).
+Ask your questions about bugs or specific use cases, and someone from
+the [core team](https://zenml.io/company#CompanyTeam) will respond.
+Or, if you
+prefer, [open an issue](https://github.com/zenml-io/zenml/issues/new/choose) on
+our GitHub repo. -->
 
 
-## License
+# 📜 License
 
-See the [LICENSE](LICENSE.rst) file for license rights and limitations (MIT).
+PINA is distributed under the terms of the MIT License. 
+A complete version of the license is available in the [LICENSE.rst](LICENSE.rst) file in this repository. Any contribution made to this project will be licensed under the MIT License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_cos.py` & `pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_cos.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_exp.py` & `pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_exp.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_linear.py` & `pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_linear.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_relu.py` & `pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_relu.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_sin.py` & `pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_sin.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_softplus.py` & `pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_softplus.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_square.py` & `pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_square.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/adaptive_functions/adaptive_tanh.py` & `pina-mathlab-0.0.3.post2308/pina/adaptive_functions/adaptive_tanh.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/condition.py` & `pina-mathlab-0.0.3.post2308/pina/condition.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/label_tensor.py` & `pina-mathlab-0.0.3.post2308/pina/label_tensor.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/deeponet.py` & `pina-mathlab-0.0.3.post2308/pina/model/deeponet.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/feed_forward.py` & `pina-mathlab-0.0.3.post2308/pina/model/feed_forward.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/layers/convolution.py` & `pina-mathlab-0.0.3.post2308/pina/model/layers/convolution.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/layers/convolution_2d.py` & `pina-mathlab-0.0.3.post2308/pina/model/layers/convolution_2d.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/layers/integral.py` & `pina-mathlab-0.0.3.post2308/pina/model/layers/integral.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/layers/stride.py` & `pina-mathlab-0.0.3.post2308/pina/model/layers/stride.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/layers/utils_convolution.py` & `pina-mathlab-0.0.3.post2308/pina/model/layers/utils_convolution.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/multi_feed_forward.py` & `pina-mathlab-0.0.3.post2308/pina/model/multi_feed_forward.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/model/network.py` & `pina-mathlab-0.0.3.post2308/pina/model/network.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/operators.py` & `pina-mathlab-0.0.3.post2308/pina/operators.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/pinn.py` & `pina-mathlab-0.0.3.post2308/pina/pinn.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/plotter.py` & `pina-mathlab-0.0.3.post2308/pina/plotter.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/problem/abstract_problem.py` & `pina-mathlab-0.0.3.post2308/pina/problem/abstract_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/problem/parametric_problem.py` & `pina-mathlab-0.0.3.post2308/pina/problem/parametric_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/problem/spatial_problem.py` & `pina-mathlab-0.0.3.post2308/pina/problem/spatial_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/problem/timedep_problem.py` & `pina-mathlab-0.0.3.post2308/pina/problem/timedep_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/span.py` & `pina-mathlab-0.0.3.post2308/pina/span.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina/utils.py` & `pina-mathlab-0.0.3.post2308/pina/utils.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/pina_mathlab.egg-info/PKG-INFO` & `pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pina-mathlab
-Version: 0.0.3
+Version: 0.0.3.post2308
 Summary: Physic Informed Neural networks for Advance modeling.
 Home-page: https://github.com/mathLab/PINA
 Author: Nicola Demo, Maria Strazzullo
 Author-email: demo.nicola@gmail.com, 
 License: MIT
 Keywords: physics-informed neural-network
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pina-mathlab-0.0.3/pina_mathlab.egg-info/SOURCES.txt` & `pina-mathlab-0.0.3.post2308/pina_mathlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/setup.py` & `pina-mathlab-0.0.3.post2308/setup.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_condition.py` & `pina-mathlab-0.0.3.post2308/tests/test_condition.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_conv.py` & `pina-mathlab-0.0.3.post2308/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_deeponet.py` & `pina-mathlab-0.0.3.post2308/tests/test_deeponet.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_fnn.py` & `pina-mathlab-0.0.3.post2308/tests/test_fnn.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_label_tensor.py` & `pina-mathlab-0.0.3.post2308/tests/test_label_tensor.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_network.py` & `pina-mathlab-0.0.3.post2308/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_operators.py` & `pina-mathlab-0.0.3.post2308/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_pinn.py` & `pina-mathlab-0.0.3.post2308/tests/test_pinn.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.0.3/tests/test_utils.py` & `pina-mathlab-0.0.3.post2308/tests/test_utils.py`

 * *Files identical despite different names*

