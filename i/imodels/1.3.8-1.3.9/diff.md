# Comparing `tmp/imodels-1.3.8.tar.gz` & `tmp/imodels-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imodels-1.3.8.tar", last modified: Sat Dec 10 22:57:43 2022, max compression
+gzip compressed data, was "imodels-1.3.9.tar", last modified: Mon Dec 12 23:16:49 2022, max compression
```

## Comparing `imodels-1.3.8.tar` & `imodels-1.3.9.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.287915 imodels-1.3.8/
--rw-r--r--   0 chandan    (501) staff       (20)       37 2022-05-12 20:54:22.000000 imodels-1.3.8/MANIFEST.in
--rw-r--r--   0 chandan    (501) staff       (20)    27945 2022-12-10 22:57:43.287557 imodels-1.3.8/PKG-INFO
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.164736 imodels-1.3.8/imodels/
--rw-r--r--   0 chandan    (501) staff       (20)     2918 2022-07-03 16:58:24.000000 imodels-1.3.8/imodels/__init__.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.169993 imodels-1.3.8/imodels/algebraic/
--rw-r--r--   0 chandan    (501) staff       (20)       95 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/algebraic/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     5849 2022-07-03 16:27:56.000000 imodels-1.3.8/imodels/algebraic/slim.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.173476 imodels-1.3.8/imodels/discretization/
--rw-r--r--   0 chandan    (501) staff       (20)      151 2021-12-10 04:31:20.000000 imodels-1.3.8/imodels/discretization/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)    33647 2022-02-09 22:00:08.000000 imodels-1.3.8/imodels/discretization/discretizer.py
--rw-r--r--   0 chandan    (501) staff       (20)    18119 2022-02-21 17:39:27.000000 imodels-1.3.8/imodels/discretization/mdlp.py
--rw-r--r--   0 chandan    (501) staff       (20)     2153 2022-02-21 17:39:45.000000 imodels-1.3.8/imodels/discretization/simple.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.177823 imodels-1.3.8/imodels/experimental/
--rw-r--r--   0 chandan    (501) staff       (20)       64 2022-05-12 20:54:22.000000 imodels-1.3.8/imodels/experimental/__init__.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.192543 imodels-1.3.8/imodels/experimental/bartpy/
--rw-r--r--   0 chandan    (501) staff       (20)       56 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)    10997 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/data.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.200896 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     3624 2022-06-15 00:11:28.000000 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/diagnostics.py
--rw-r--r--   0 chandan    (501) staff       (20)     8255 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/features.py
--rw-r--r--   0 chandan    (501) staff       (20)     7293 2022-04-16 16:21:58.000000 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/motivation.py
--rw-r--r--   0 chandan    (501) staff       (20)      743 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/residuals.py
--rw-r--r--   0 chandan    (501) staff       (20)     1094 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/sampling.py
--rw-r--r--   0 chandan    (501) staff       (20)      406 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/sigma.py
--rw-r--r--   0 chandan    (501) staff       (20)     1132 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/diagnostics/trees.py
--rw-r--r--   0 chandan    (501) staff       (20)      111 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/errors.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.203907 imodels-1.3.8/imodels/experimental/bartpy/extensions/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/extensions/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     1084 2022-03-26 05:01:03.000000 imodels-1.3.8/imodels/experimental/bartpy/extensions/baseestimator.py
--rw-r--r--   0 chandan    (501) staff       (20)      770 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/extensions/ols.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.208191 imodels-1.3.8/imodels/experimental/bartpy/features/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/features/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     4797 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/features/featureimportance.py
--rw-r--r--   0 chandan    (501) staff       (20)     2791 2022-03-26 05:00:14.000000 imodels-1.3.8/imodels/experimental/bartpy/features/featureselection.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.216464 imodels-1.3.8/imodels/experimental/bartpy/initializers/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/initializers/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)      875 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/initializers/initializer.py
--rw-r--r--   0 chandan    (501) staff       (20)     6885 2022-04-16 16:21:58.000000 imodels-1.3.8/imodels/experimental/bartpy/initializers/sklearntreeinitializer.py
--rw-r--r--   0 chandan    (501) staff       (20)     4410 2022-04-16 16:21:58.000000 imodels-1.3.8/imodels/experimental/bartpy/model.py
--rw-r--r--   0 chandan    (501) staff       (20)     1251 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/mutation.py
--rw-r--r--   0 chandan    (501) staff       (20)     4460 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/node.py
--rw-r--r--   0 chandan    (501) staff       (20)      335 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/plotting.py
--rw-r--r--   0 chandan    (501) staff       (20)     1711 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/runner.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.229020 imodels-1.3.8/imodels/experimental/bartpy/samplers/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     1813 2022-04-16 16:21:58.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/leafnode.py
--rw-r--r--   0 chandan    (501) staff       (20)     3023 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/modelsampler.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.232095 imodels-1.3.8/imodels/experimental/bartpy/samplers/oblivioustrees/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/oblivioustrees/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     6888 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/oblivioustrees/likihoodratio.py
--rw-r--r--   0 chandan    (501) staff       (20)     2727 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/oblivioustrees/proposer.py
--rw-r--r--   0 chandan    (501) staff       (20)     2198 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/oblivioustrees/treemutation.py
--rw-r--r--   0 chandan    (501) staff       (20)      220 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/sampler.py
--rw-r--r--   0 chandan    (501) staff       (20)     1437 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/scalar.py
--rw-r--r--   0 chandan    (501) staff       (20)     1797 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/schedule.py
--rw-r--r--   0 chandan    (501) staff       (20)      642 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/sigma.py
--rw-r--r--   0 chandan    (501) staff       (20)     4778 2022-04-16 16:21:58.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/treemutation.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.235445 imodels-1.3.8/imodels/experimental/bartpy/samplers/unconstrainedtree/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/unconstrainedtree/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     9264 2022-04-16 16:21:58.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/unconstrainedtree/likihoodratio.py
--rw-r--r--   0 chandan    (501) staff       (20)     3920 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/unconstrainedtree/proposer.py
--rw-r--r--   0 chandan    (501) staff       (20)     2286 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/samplers/unconstrainedtree/treemutation.py
--rw-r--r--   0 chandan    (501) staff       (20)     1238 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/sigma.py
--rw-r--r--   0 chandan    (501) staff       (20)    26441 2022-07-03 16:42:12.000000 imodels-1.3.8/imodels/experimental/bartpy/sklearnmodel.py
--rw-r--r--   0 chandan    (501) staff       (20)     1651 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/split.py
--rw-r--r--   0 chandan    (501) staff       (20)     3342 2022-02-04 22:40:36.000000 imodels-1.3.8/imodels/experimental/bartpy/splitcondition.py
--rw-r--r--   0 chandan    (501) staff       (20)     1022 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/trace.py
--rw-r--r--   0 chandan    (501) staff       (20)     5430 2022-03-18 20:35:41.000000 imodels-1.3.8/imodels/experimental/bartpy/tree.py
--rw-r--r--   0 chandan    (501) staff       (20)    24605 2022-09-15 20:16:47.000000 imodels-1.3.8/imodels/experimental/figs_ensembles.py
--rw-r--r--   0 chandan    (501) staff       (20)     8446 2022-07-03 16:42:12.000000 imodels-1.3.8/imodels/experimental/figs_shrinkage.py
--rw-r--r--   0 chandan    (501) staff       (20)     3336 2021-11-22 05:12:24.000000 imodels-1.3.8/imodels/experimental/stablelinear.py
--rw-r--r--   0 chandan    (501) staff       (20)     2333 2021-11-22 05:12:24.000000 imodels-1.3.8/imodels/experimental/stableskope.py
--rw-r--r--   0 chandan    (501) staff       (20)     1485 2021-11-22 05:12:24.000000 imodels-1.3.8/imodels/experimental/util.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.237991 imodels-1.3.8/imodels/importance/
--rw-r--r--   0 chandan    (501) staff       (20)      121 2022-05-28 04:34:15.000000 imodels-1.3.8/imodels/importance/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     9188 2022-05-28 04:38:11.000000 imodels-1.3.8/imodels/importance/r2f.py
--rw-r--r--   0 chandan    (501) staff       (20)    17113 2022-05-28 04:34:15.000000 imodels-1.3.8/imodels/importance/representation.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.244319 imodels-1.3.8/imodels/rule_list/
--rw-r--r--   0 chandan    (501) staff       (20)       70 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/rule_list/__init__.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.246377 imodels-1.3.8/imodels/rule_list/bayesian_rule_list/
--rw-r--r--   0 chandan    (501) staff       (20)      166 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/rule_list/bayesian_rule_list/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)    12271 2022-02-09 22:00:08.000000 imodels-1.3.8/imodels/rule_list/bayesian_rule_list/bayesian_rule_list.py
--rw-r--r--   0 chandan    (501) staff       (20)    22494 2022-02-21 17:47:12.000000 imodels-1.3.8/imodels/rule_list/bayesian_rule_list/brl_util.py
--rw-r--r--   0 chandan    (501) staff       (20)    11499 2022-05-21 23:49:55.000000 imodels-1.3.8/imodels/rule_list/corels_wrapper.py
--rw-r--r--   0 chandan    (501) staff       (20)    11521 2022-12-10 22:51:18.000000 imodels-1.3.8/imodels/rule_list/greedy_rule_list.py
--rw-r--r--   0 chandan    (501) staff       (20)     2133 2022-12-10 22:53:29.000000 imodels-1.3.8/imodels/rule_list/one_r.py
--rw-r--r--   0 chandan    (501) staff       (20)      255 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/rule_list/rule_list.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.256875 imodels-1.3.8/imodels/rule_set/
--rw-r--r--   0 chandan    (501) staff       (20)       95 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/rule_set/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     3186 2022-12-10 22:25:29.000000 imodels-1.3.8/imodels/rule_set/boosted_rules.py
--rw-r--r--   0 chandan    (501) staff       (20)    23303 2022-12-10 22:47:59.000000 imodels-1.3.8/imodels/rule_set/brs.py
--rw-r--r--   0 chandan    (501) staff       (20)     2259 2022-05-21 23:53:10.000000 imodels-1.3.8/imodels/rule_set/fplasso.py
--rw-r--r--   0 chandan    (501) staff       (20)     2694 2022-02-09 22:00:08.000000 imodels-1.3.8/imodels/rule_set/fpskope.py
--rw-r--r--   0 chandan    (501) staff       (20)    12910 2022-12-10 22:41:08.000000 imodels-1.3.8/imodels/rule_set/rule_fit.py
--rw-r--r--   0 chandan    (501) staff       (20)     1299 2022-02-21 17:48:49.000000 imodels-1.3.8/imodels/rule_set/rule_set.py
--rw-r--r--   0 chandan    (501) staff       (20)    20793 2022-12-10 22:36:09.000000 imodels-1.3.8/imodels/rule_set/skope_rules.py
--rw-r--r--   0 chandan    (501) staff       (20)      596 2022-12-10 22:27:35.000000 imodels-1.3.8/imodels/rule_set/slipper.py
--rw-r--r--   0 chandan    (501) staff       (20)     9157 2022-12-10 22:11:01.000000 imodels-1.3.8/imodels/rule_set/slipper_util.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.263790 imodels-1.3.8/imodels/tree/
--rw-r--r--   0 chandan    (501) staff       (20)       70 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/tree/__init__.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.267066 imodels-1.3.8/imodels/tree/c45_tree/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/tree/c45_tree/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)    16447 2022-07-03 16:42:12.000000 imodels-1.3.8/imodels/tree/c45_tree/c45_tree.py
--rw-r--r--   0 chandan    (501) staff       (20)     4412 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/tree/c45_tree/c45_utils.py
--rw-r--r--   0 chandan    (501) staff       (20)     8855 2022-07-03 16:42:12.000000 imodels-1.3.8/imodels/tree/cart_ccp.py
--rw-r--r--   0 chandan    (501) staff       (20)     4710 2022-12-10 22:31:20.000000 imodels-1.3.8/imodels/tree/cart_wrapper.py
--rw-r--r--   0 chandan    (501) staff       (20)    22504 2022-12-10 22:07:46.000000 imodels-1.3.8/imodels/tree/figs.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.270971 imodels-1.3.8/imodels/tree/gosdt/
--rw-r--r--   0 chandan    (501) staff       (20)        0 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/tree/gosdt/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)    11030 2022-02-09 22:00:08.000000 imodels-1.3.8/imodels/tree/gosdt/pygosdt.py
--rw-r--r--   0 chandan    (501) staff       (20)    17199 2022-08-11 14:16:19.000000 imodels-1.3.8/imodels/tree/gosdt/pygosdt_helper.py
--rw-r--r--   0 chandan    (501) staff       (20)     6936 2022-07-03 16:42:12.000000 imodels-1.3.8/imodels/tree/gosdt/pygosdt_shrinkage.py
--rw-r--r--   0 chandan    (501) staff       (20)    13378 2022-12-10 22:30:26.000000 imodels-1.3.8/imodels/tree/hierarchical_shrinkage.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.272370 imodels-1.3.8/imodels/tree/iterative_random_forest/
--rw-r--r--   0 chandan    (501) staff       (20)      109 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/tree/iterative_random_forest/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     1104 2022-06-15 02:05:03.000000 imodels-1.3.8/imodels/tree/iterative_random_forest/iterative_random_forest.py
--rw-r--r--   0 chandan    (501) staff       (20)    18121 2022-12-10 22:34:49.000000 imodels-1.3.8/imodels/tree/tao.py
--rw-r--r--   0 chandan    (501) staff       (20)     5540 2022-12-06 16:39:15.000000 imodels-1.3.8/imodels/tree/viz_utils.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.284500 imodels-1.3.8/imodels/util/
--rw-r--r--   0 chandan    (501) staff       (20)       72 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/util/__init__.py
--rw-r--r--   0 chandan    (501) staff       (20)     1137 2022-12-10 22:51:58.000000 imodels-1.3.8/imodels/util/arguments.py
--rw-r--r--   0 chandan    (501) staff       (20)     2237 2022-07-03 16:42:12.000000 imodels-1.3.8/imodels/util/checks.py
--rw-r--r--   0 chandan    (501) staff       (20)     5014 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/util/convert.py
--rw-r--r--   0 chandan    (501) staff       (20)     6494 2022-03-26 03:37:28.000000 imodels-1.3.8/imodels/util/data_util.py
--rw-r--r--   0 chandan    (501) staff       (20)     2138 2022-03-04 22:59:49.000000 imodels-1.3.8/imodels/util/distillation.py
--rw-r--r--   0 chandan    (501) staff       (20)     2030 2021-12-10 04:31:20.000000 imodels-1.3.8/imodels/util/explain_errors.py
--rw-r--r--   0 chandan    (501) staff       (20)     6619 2022-05-21 15:35:43.000000 imodels-1.3.8/imodels/util/extract.py
--rw-r--r--   0 chandan    (501) staff       (20)     2077 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/util/metrics.py
--rw-r--r--   0 chandan    (501) staff       (20)     6633 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/util/neural_nets.py
--rw-r--r--   0 chandan    (501) staff       (20)     3753 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/util/prune.py
--rw-r--r--   0 chandan    (501) staff       (20)     3117 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/util/rule.py
--rw-r--r--   0 chandan    (501) staff       (20)     5692 2021-12-10 04:31:20.000000 imodels-1.3.8/imodels/util/score.py
--rw-r--r--   0 chandan    (501) staff       (20)     2188 2021-11-15 19:21:29.000000 imodels-1.3.8/imodels/util/transforms.py
--rw-r--r--   0 chandan    (501) staff       (20)     1414 2021-12-06 01:44:36.000000 imodels-1.3.8/imodels/util/tree.py
--rw-r--r--   0 chandan    (501) staff       (20)     3585 2022-06-14 23:13:44.000000 imodels-1.3.8/imodels/util/tree_interaction_utils.py
-drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-10 22:57:43.168387 imodels-1.3.8/imodels.egg-info/
--rw-r--r--   0 chandan    (501) staff       (20)    27945 2022-12-10 22:57:42.000000 imodels-1.3.8/imodels.egg-info/PKG-INFO
--rw-r--r--   0 chandan    (501) staff       (20)     4666 2022-12-10 22:57:43.000000 imodels-1.3.8/imodels.egg-info/SOURCES.txt
--rw-r--r--   0 chandan    (501) staff       (20)        1 2022-12-10 22:57:42.000000 imodels-1.3.8/imodels.egg-info/dependency_links.txt
--rw-r--r--   0 chandan    (501) staff       (20)      154 2022-12-10 22:57:42.000000 imodels-1.3.8/imodels.egg-info/requires.txt
--rw-r--r--   0 chandan    (501) staff       (20)        8 2022-12-10 22:57:42.000000 imodels-1.3.8/imodels.egg-info/top_level.txt
--rw-r--r--   0 chandan    (501) staff       (20)     1074 2021-11-15 19:21:29.000000 imodels-1.3.8/license.md
--rw-r--r--   0 chandan    (501) staff       (20)    27375 2022-12-10 22:14:45.000000 imodels-1.3.8/readme.md
--rw-r--r--   0 chandan    (501) staff       (20)       38 2022-12-10 22:57:43.288002 imodels-1.3.8/setup.cfg
--rw-r--r--   0 chandan    (501) staff       (20)     2063 2022-12-10 22:54:15.000000 imodels-1.3.8/setup.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.883796 imodels-1.3.9/
+-rw-r--r--   0 chandan    (501) staff       (20)       37 2022-05-12 20:54:22.000000 imodels-1.3.9/MANIFEST.in
+-rw-r--r--   0 chandan    (501) staff       (20)    27945 2022-12-12 23:16:49.883380 imodels-1.3.9/PKG-INFO
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.446443 imodels-1.3.9/imodels/
+-rw-r--r--   0 chandan    (501) staff       (20)     2918 2022-07-03 16:58:24.000000 imodels-1.3.9/imodels/__init__.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.467713 imodels-1.3.9/imodels/algebraic/
+-rw-r--r--   0 chandan    (501) staff       (20)       95 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/algebraic/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     5849 2022-07-03 16:27:56.000000 imodels-1.3.9/imodels/algebraic/slim.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.507519 imodels-1.3.9/imodels/discretization/
+-rw-r--r--   0 chandan    (501) staff       (20)      151 2021-12-10 04:31:20.000000 imodels-1.3.9/imodels/discretization/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)    33647 2022-02-09 22:00:08.000000 imodels-1.3.9/imodels/discretization/discretizer.py
+-rw-r--r--   0 chandan    (501) staff       (20)    18119 2022-02-21 17:39:27.000000 imodels-1.3.9/imodels/discretization/mdlp.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2153 2022-02-21 17:39:45.000000 imodels-1.3.9/imodels/discretization/simple.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.532742 imodels-1.3.9/imodels/experimental/
+-rw-r--r--   0 chandan    (501) staff       (20)       64 2022-05-12 20:54:22.000000 imodels-1.3.9/imodels/experimental/__init__.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.573626 imodels-1.3.9/imodels/experimental/bartpy/
+-rw-r--r--   0 chandan    (501) staff       (20)       56 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)    10997 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/data.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.598470 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3624 2022-06-15 00:11:28.000000 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/diagnostics.py
+-rw-r--r--   0 chandan    (501) staff       (20)     8255 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/features.py
+-rw-r--r--   0 chandan    (501) staff       (20)     7293 2022-04-16 16:21:58.000000 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/motivation.py
+-rw-r--r--   0 chandan    (501) staff       (20)      743 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/residuals.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1094 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/sampling.py
+-rw-r--r--   0 chandan    (501) staff       (20)      406 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/sigma.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1132 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/diagnostics/trees.py
+-rw-r--r--   0 chandan    (501) staff       (20)      111 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/errors.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.603658 imodels-1.3.9/imodels/experimental/bartpy/extensions/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/extensions/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1084 2022-03-26 05:01:03.000000 imodels-1.3.9/imodels/experimental/bartpy/extensions/baseestimator.py
+-rw-r--r--   0 chandan    (501) staff       (20)      770 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/extensions/ols.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.609773 imodels-1.3.9/imodels/experimental/bartpy/features/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/features/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     4797 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/features/featureimportance.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2791 2022-03-26 05:00:14.000000 imodels-1.3.9/imodels/experimental/bartpy/features/featureselection.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.618306 imodels-1.3.9/imodels/experimental/bartpy/initializers/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/initializers/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)      875 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/initializers/initializer.py
+-rw-r--r--   0 chandan    (501) staff       (20)     6885 2022-04-16 16:21:58.000000 imodels-1.3.9/imodels/experimental/bartpy/initializers/sklearntreeinitializer.py
+-rw-r--r--   0 chandan    (501) staff       (20)     4410 2022-04-16 16:21:58.000000 imodels-1.3.9/imodels/experimental/bartpy/model.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1251 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/mutation.py
+-rw-r--r--   0 chandan    (501) staff       (20)     4460 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/node.py
+-rw-r--r--   0 chandan    (501) staff       (20)      335 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/plotting.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1711 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/runner.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.637757 imodels-1.3.9/imodels/experimental/bartpy/samplers/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1813 2022-04-16 16:21:58.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/leafnode.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3023 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/modelsampler.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.648903 imodels-1.3.9/imodels/experimental/bartpy/samplers/oblivioustrees/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/oblivioustrees/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     6888 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/oblivioustrees/likihoodratio.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2727 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/oblivioustrees/proposer.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2198 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/oblivioustrees/treemutation.py
+-rw-r--r--   0 chandan    (501) staff       (20)      220 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/sampler.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1437 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/scalar.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1797 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/schedule.py
+-rw-r--r--   0 chandan    (501) staff       (20)      642 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/sigma.py
+-rw-r--r--   0 chandan    (501) staff       (20)     4778 2022-04-16 16:21:58.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/treemutation.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.697338 imodels-1.3.9/imodels/experimental/bartpy/samplers/unconstrainedtree/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/unconstrainedtree/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     9264 2022-04-16 16:21:58.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/unconstrainedtree/likihoodratio.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3920 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/unconstrainedtree/proposer.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2286 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/samplers/unconstrainedtree/treemutation.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1238 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/sigma.py
+-rw-r--r--   0 chandan    (501) staff       (20)    26441 2022-07-03 16:42:12.000000 imodels-1.3.9/imodels/experimental/bartpy/sklearnmodel.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1651 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/split.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3342 2022-02-04 22:40:36.000000 imodels-1.3.9/imodels/experimental/bartpy/splitcondition.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1022 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/trace.py
+-rw-r--r--   0 chandan    (501) staff       (20)     5430 2022-03-18 20:35:41.000000 imodels-1.3.9/imodels/experimental/bartpy/tree.py
+-rw-r--r--   0 chandan    (501) staff       (20)    24605 2022-09-15 20:16:47.000000 imodels-1.3.9/imodels/experimental/figs_ensembles.py
+-rw-r--r--   0 chandan    (501) staff       (20)     8446 2022-07-03 16:42:12.000000 imodels-1.3.9/imodels/experimental/figs_shrinkage.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3336 2021-11-22 05:12:24.000000 imodels-1.3.9/imodels/experimental/stablelinear.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2333 2021-11-22 05:12:24.000000 imodels-1.3.9/imodels/experimental/stableskope.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1485 2021-11-22 05:12:24.000000 imodels-1.3.9/imodels/experimental/util.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.705816 imodels-1.3.9/imodels/importance/
+-rw-r--r--   0 chandan    (501) staff       (20)      121 2022-05-28 04:34:15.000000 imodels-1.3.9/imodels/importance/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     9188 2022-05-28 04:38:11.000000 imodels-1.3.9/imodels/importance/r2f.py
+-rw-r--r--   0 chandan    (501) staff       (20)    17113 2022-05-28 04:34:15.000000 imodels-1.3.9/imodels/importance/representation.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.716689 imodels-1.3.9/imodels/rule_list/
+-rw-r--r--   0 chandan    (501) staff       (20)       70 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/rule_list/__init__.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.724718 imodels-1.3.9/imodels/rule_list/bayesian_rule_list/
+-rw-r--r--   0 chandan    (501) staff       (20)      166 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/rule_list/bayesian_rule_list/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)    12271 2022-02-09 22:00:08.000000 imodels-1.3.9/imodels/rule_list/bayesian_rule_list/bayesian_rule_list.py
+-rw-r--r--   0 chandan    (501) staff       (20)    22494 2022-02-21 17:47:12.000000 imodels-1.3.9/imodels/rule_list/bayesian_rule_list/brl_util.py
+-rw-r--r--   0 chandan    (501) staff       (20)    11499 2022-05-21 23:49:55.000000 imodels-1.3.9/imodels/rule_list/corels_wrapper.py
+-rw-r--r--   0 chandan    (501) staff       (20)    11521 2022-12-10 22:51:18.000000 imodels-1.3.9/imodels/rule_list/greedy_rule_list.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2133 2022-12-10 22:53:29.000000 imodels-1.3.9/imodels/rule_list/one_r.py
+-rw-r--r--   0 chandan    (501) staff       (20)      255 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/rule_list/rule_list.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.759369 imodels-1.3.9/imodels/rule_set/
+-rw-r--r--   0 chandan    (501) staff       (20)       95 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/rule_set/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3317 2022-12-12 23:16:00.000000 imodels-1.3.9/imodels/rule_set/boosted_rules.py
+-rw-r--r--   0 chandan    (501) staff       (20)    23303 2022-12-10 22:47:59.000000 imodels-1.3.9/imodels/rule_set/brs.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2259 2022-05-21 23:53:10.000000 imodels-1.3.9/imodels/rule_set/fplasso.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2694 2022-02-09 22:00:08.000000 imodels-1.3.9/imodels/rule_set/fpskope.py
+-rw-r--r--   0 chandan    (501) staff       (20)    12910 2022-12-10 22:41:08.000000 imodels-1.3.9/imodels/rule_set/rule_fit.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1299 2022-02-21 17:48:49.000000 imodels-1.3.9/imodels/rule_set/rule_set.py
+-rw-r--r--   0 chandan    (501) staff       (20)    20793 2022-12-10 22:36:09.000000 imodels-1.3.9/imodels/rule_set/skope_rules.py
+-rw-r--r--   0 chandan    (501) staff       (20)      596 2022-12-10 22:27:35.000000 imodels-1.3.9/imodels/rule_set/slipper.py
+-rw-r--r--   0 chandan    (501) staff       (20)     9157 2022-12-10 22:11:01.000000 imodels-1.3.9/imodels/rule_set/slipper_util.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.782869 imodels-1.3.9/imodels/tree/
+-rw-r--r--   0 chandan    (501) staff       (20)       70 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/tree/__init__.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.790081 imodels-1.3.9/imodels/tree/c45_tree/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/tree/c45_tree/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)    16447 2022-07-03 16:42:12.000000 imodels-1.3.9/imodels/tree/c45_tree/c45_tree.py
+-rw-r--r--   0 chandan    (501) staff       (20)     4412 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/tree/c45_tree/c45_utils.py
+-rw-r--r--   0 chandan    (501) staff       (20)     8855 2022-07-03 16:42:12.000000 imodels-1.3.9/imodels/tree/cart_ccp.py
+-rw-r--r--   0 chandan    (501) staff       (20)     4710 2022-12-10 22:31:20.000000 imodels-1.3.9/imodels/tree/cart_wrapper.py
+-rw-r--r--   0 chandan    (501) staff       (20)    22504 2022-12-10 22:07:46.000000 imodels-1.3.9/imodels/tree/figs.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.804490 imodels-1.3.9/imodels/tree/gosdt/
+-rw-r--r--   0 chandan    (501) staff       (20)        0 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/tree/gosdt/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)    11030 2022-02-09 22:00:08.000000 imodels-1.3.9/imodels/tree/gosdt/pygosdt.py
+-rw-r--r--   0 chandan    (501) staff       (20)    17199 2022-08-11 14:16:19.000000 imodels-1.3.9/imodels/tree/gosdt/pygosdt_helper.py
+-rw-r--r--   0 chandan    (501) staff       (20)     6936 2022-07-03 16:42:12.000000 imodels-1.3.9/imodels/tree/gosdt/pygosdt_shrinkage.py
+-rw-r--r--   0 chandan    (501) staff       (20)    13378 2022-12-10 22:30:26.000000 imodels-1.3.9/imodels/tree/hierarchical_shrinkage.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.809347 imodels-1.3.9/imodels/tree/iterative_random_forest/
+-rw-r--r--   0 chandan    (501) staff       (20)      109 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/tree/iterative_random_forest/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1104 2022-06-15 02:05:03.000000 imodels-1.3.9/imodels/tree/iterative_random_forest/iterative_random_forest.py
+-rw-r--r--   0 chandan    (501) staff       (20)    18121 2022-12-10 22:34:49.000000 imodels-1.3.9/imodels/tree/tao.py
+-rw-r--r--   0 chandan    (501) staff       (20)     5540 2022-12-06 16:39:15.000000 imodels-1.3.9/imodels/tree/viz_utils.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.881639 imodels-1.3.9/imodels/util/
+-rw-r--r--   0 chandan    (501) staff       (20)       72 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/util/__init__.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1137 2022-12-10 22:51:58.000000 imodels-1.3.9/imodels/util/arguments.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2237 2022-07-03 16:42:12.000000 imodels-1.3.9/imodels/util/checks.py
+-rw-r--r--   0 chandan    (501) staff       (20)     5014 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/util/convert.py
+-rw-r--r--   0 chandan    (501) staff       (20)     6494 2022-03-26 03:37:28.000000 imodels-1.3.9/imodels/util/data_util.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2138 2022-03-04 22:59:49.000000 imodels-1.3.9/imodels/util/distillation.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2030 2021-12-10 04:31:20.000000 imodels-1.3.9/imodels/util/explain_errors.py
+-rw-r--r--   0 chandan    (501) staff       (20)     6619 2022-05-21 15:35:43.000000 imodels-1.3.9/imodels/util/extract.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2077 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/util/metrics.py
+-rw-r--r--   0 chandan    (501) staff       (20)     6633 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/util/neural_nets.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3753 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/util/prune.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3117 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/util/rule.py
+-rw-r--r--   0 chandan    (501) staff       (20)     5692 2021-12-10 04:31:20.000000 imodels-1.3.9/imodels/util/score.py
+-rw-r--r--   0 chandan    (501) staff       (20)     2188 2021-11-15 19:21:29.000000 imodels-1.3.9/imodels/util/transforms.py
+-rw-r--r--   0 chandan    (501) staff       (20)     1414 2021-12-06 01:44:36.000000 imodels-1.3.9/imodels/util/tree.py
+-rw-r--r--   0 chandan    (501) staff       (20)     3585 2022-06-14 23:13:44.000000 imodels-1.3.9/imodels/util/tree_interaction_utils.py
+drwxr-xr-x   0 chandan    (501) staff       (20)        0 2022-12-12 23:16:49.462660 imodels-1.3.9/imodels.egg-info/
+-rw-r--r--   0 chandan    (501) staff       (20)    27945 2022-12-12 23:16:48.000000 imodels-1.3.9/imodels.egg-info/PKG-INFO
+-rw-r--r--   0 chandan    (501) staff       (20)     4666 2022-12-12 23:16:49.000000 imodels-1.3.9/imodels.egg-info/SOURCES.txt
+-rw-r--r--   0 chandan    (501) staff       (20)        1 2022-12-12 23:16:48.000000 imodels-1.3.9/imodels.egg-info/dependency_links.txt
+-rw-r--r--   0 chandan    (501) staff       (20)      154 2022-12-12 23:16:49.000000 imodels-1.3.9/imodels.egg-info/requires.txt
+-rw-r--r--   0 chandan    (501) staff       (20)        8 2022-12-12 23:16:49.000000 imodels-1.3.9/imodels.egg-info/top_level.txt
+-rw-r--r--   0 chandan    (501) staff       (20)     1074 2021-11-15 19:21:29.000000 imodels-1.3.9/license.md
+-rw-r--r--   0 chandan    (501) staff       (20)    27375 2022-12-10 22:14:45.000000 imodels-1.3.9/readme.md
+-rw-r--r--   0 chandan    (501) staff       (20)       38 2022-12-12 23:16:49.883866 imodels-1.3.9/setup.cfg
+-rw-r--r--   0 chandan    (501) staff       (20)     2063 2022-12-12 23:15:07.000000 imodels-1.3.9/setup.py
```

### Comparing `imodels-1.3.8/PKG-INFO` & `imodels-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodels
-Version: 1.3.8
+Version: 1.3.9
 Summary: Implementations of various interpretable models
 Home-page: https://github.com/csinva/imodels
 Author: Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen, Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others
 Author-email: chandan_singh@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodels Version: 1.3.8 Summary: Implementations of
+Metadata-Version: 2.1 Name: imodels Version: 1.3.9 Summary: Implementations of
 various interpretable models Home-page: https://github.com/csinva/imodels
 Author: Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen,
 Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others Author-email:
 chandan_singh@berkeley.edu Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev
```

### Comparing `imodels-1.3.8/imodels/__init__.py` & `imodels-1.3.9/imodels/__init__.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/algebraic/slim.py` & `imodels-1.3.9/imodels/algebraic/slim.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/discretization/discretizer.py` & `imodels-1.3.9/imodels/discretization/discretizer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/discretization/mdlp.py` & `imodels-1.3.9/imodels/discretization/mdlp.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/discretization/simple.py` & `imodels-1.3.9/imodels/discretization/simple.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/data.py` & `imodels-1.3.9/imodels/experimental/bartpy/data.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/diagnostics/diagnostics.py` & `imodels-1.3.9/imodels/experimental/bartpy/diagnostics/diagnostics.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/diagnostics/features.py` & `imodels-1.3.9/imodels/experimental/bartpy/diagnostics/features.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/diagnostics/motivation.py` & `imodels-1.3.9/imodels/experimental/bartpy/diagnostics/motivation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/diagnostics/residuals.py` & `imodels-1.3.9/imodels/experimental/bartpy/diagnostics/residuals.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/diagnostics/sampling.py` & `imodels-1.3.9/imodels/experimental/bartpy/diagnostics/sampling.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/diagnostics/trees.py` & `imodels-1.3.9/imodels/experimental/bartpy/diagnostics/trees.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/extensions/baseestimator.py` & `imodels-1.3.9/imodels/experimental/bartpy/extensions/baseestimator.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/extensions/ols.py` & `imodels-1.3.9/imodels/experimental/bartpy/extensions/ols.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/features/featureimportance.py` & `imodels-1.3.9/imodels/experimental/bartpy/features/featureimportance.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/features/featureselection.py` & `imodels-1.3.9/imodels/experimental/bartpy/features/featureselection.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/initializers/initializer.py` & `imodels-1.3.9/imodels/experimental/bartpy/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/initializers/sklearntreeinitializer.py` & `imodels-1.3.9/imodels/experimental/bartpy/initializers/sklearntreeinitializer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/model.py` & `imodels-1.3.9/imodels/experimental/bartpy/model.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/mutation.py` & `imodels-1.3.9/imodels/experimental/bartpy/mutation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/node.py` & `imodels-1.3.9/imodels/experimental/bartpy/node.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/runner.py` & `imodels-1.3.9/imodels/experimental/bartpy/runner.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/leafnode.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/leafnode.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/modelsampler.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/modelsampler.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/oblivioustrees/likihoodratio.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/oblivioustrees/likihoodratio.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/oblivioustrees/proposer.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/oblivioustrees/proposer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/oblivioustrees/treemutation.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/oblivioustrees/treemutation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/scalar.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/scalar.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/schedule.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/schedule.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/sigma.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/sigma.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/treemutation.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/treemutation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/unconstrainedtree/likihoodratio.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/unconstrainedtree/likihoodratio.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/unconstrainedtree/proposer.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/unconstrainedtree/proposer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/samplers/unconstrainedtree/treemutation.py` & `imodels-1.3.9/imodels/experimental/bartpy/samplers/unconstrainedtree/treemutation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/sigma.py` & `imodels-1.3.9/imodels/experimental/bartpy/sigma.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/sklearnmodel.py` & `imodels-1.3.9/imodels/experimental/bartpy/sklearnmodel.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/split.py` & `imodels-1.3.9/imodels/experimental/bartpy/split.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/splitcondition.py` & `imodels-1.3.9/imodels/experimental/bartpy/splitcondition.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/trace.py` & `imodels-1.3.9/imodels/experimental/bartpy/trace.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/bartpy/tree.py` & `imodels-1.3.9/imodels/experimental/bartpy/tree.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/figs_ensembles.py` & `imodels-1.3.9/imodels/experimental/figs_ensembles.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/figs_shrinkage.py` & `imodels-1.3.9/imodels/experimental/figs_shrinkage.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/stablelinear.py` & `imodels-1.3.9/imodels/experimental/stablelinear.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/stableskope.py` & `imodels-1.3.9/imodels/experimental/stableskope.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/experimental/util.py` & `imodels-1.3.9/imodels/experimental/util.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/importance/r2f.py` & `imodels-1.3.9/imodels/importance/r2f.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/importance/representation.py` & `imodels-1.3.9/imodels/importance/representation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_list/bayesian_rule_list/bayesian_rule_list.py` & `imodels-1.3.9/imodels/rule_list/bayesian_rule_list/bayesian_rule_list.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_list/bayesian_rule_list/brl_util.py` & `imodels-1.3.9/imodels/rule_list/bayesian_rule_list/brl_util.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_list/corels_wrapper.py` & `imodels-1.3.9/imodels/rule_list/corels_wrapper.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_list/greedy_rule_list.py` & `imodels-1.3.9/imodels/rule_list/greedy_rule_list.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_list/one_r.py` & `imodels-1.3.9/imodels/rule_list/one_r.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_set/boosted_rules.py` & `imodels-1.3.9/imodels/rule_set/boosted_rules.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             random_state=random_state,
         )
         # self.estimator = estimator
 
     def fit(self, X, y, feature_names=None, **kwargs):
         X, y, feature_names = check_fit_arguments(self, X, y, feature_names)
         super().fit(X, y, **kwargs)
+        self.complexity_ = len(self.estimators_)
 
 class BoostedRulesRegressor(AdaBoostRegressor):
     '''An easy-interpretable regressor optimizing simple logical rules.
 
     Params
     ------
     estimator: object with fit and predict methods
@@ -74,18 +75,19 @@
             random_state=random_state,
         )
         # self.estimator = estimator
 
     def fit(self, X, y, feature_names=None, **kwargs):
         X, y, feature_names = check_fit_arguments(self, X, y, feature_names)
         super().fit(X, y, **kwargs)
+        self.complexity_ = len(self.estimators_)
 
 
 if __name__ == '__main__':
     np.random.seed(13)
     X, Y = sklearn.datasets.load_breast_cancer(as_frame=True, return_X_y=True)
     model = BoostedRulesClassifier(estimator=SlipperBaseEstimator)
     X_train, X_test, y_train, y_test = train_test_split(X, Y, test_size = 0.3)
     model.fit(X_train, y_train, feature_names=X_train.columns)
     y_pred = model.predict(X_test)
     acc = model.score(X_test, y_test)
-    print('acc', acc)
+    print('acc', acc, 'complexity', model.complexity_)
```

### Comparing `imodels-1.3.8/imodels/rule_set/brs.py` & `imodels-1.3.9/imodels/rule_set/brs.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_set/fplasso.py` & `imodels-1.3.9/imodels/rule_set/fplasso.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_set/fpskope.py` & `imodels-1.3.9/imodels/rule_set/fpskope.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_set/rule_fit.py` & `imodels-1.3.9/imodels/rule_set/rule_fit.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_set/rule_set.py` & `imodels-1.3.9/imodels/rule_set/rule_set.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_set/skope_rules.py` & `imodels-1.3.9/imodels/rule_set/skope_rules.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_set/slipper.py` & `imodels-1.3.9/imodels/rule_set/slipper.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/rule_set/slipper_util.py` & `imodels-1.3.9/imodels/rule_set/slipper_util.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/c45_tree/c45_tree.py` & `imodels-1.3.9/imodels/tree/c45_tree/c45_tree.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/c45_tree/c45_utils.py` & `imodels-1.3.9/imodels/tree/c45_tree/c45_utils.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/cart_ccp.py` & `imodels-1.3.9/imodels/tree/cart_ccp.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/cart_wrapper.py` & `imodels-1.3.9/imodels/tree/cart_wrapper.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/figs.py` & `imodels-1.3.9/imodels/tree/figs.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/gosdt/pygosdt.py` & `imodels-1.3.9/imodels/tree/gosdt/pygosdt.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/gosdt/pygosdt_helper.py` & `imodels-1.3.9/imodels/tree/gosdt/pygosdt_helper.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/gosdt/pygosdt_shrinkage.py` & `imodels-1.3.9/imodels/tree/gosdt/pygosdt_shrinkage.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/hierarchical_shrinkage.py` & `imodels-1.3.9/imodels/tree/hierarchical_shrinkage.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/iterative_random_forest/iterative_random_forest.py` & `imodels-1.3.9/imodels/tree/iterative_random_forest/iterative_random_forest.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/tao.py` & `imodels-1.3.9/imodels/tree/tao.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/tree/viz_utils.py` & `imodels-1.3.9/imodels/tree/viz_utils.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/arguments.py` & `imodels-1.3.9/imodels/util/arguments.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/checks.py` & `imodels-1.3.9/imodels/util/checks.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/convert.py` & `imodels-1.3.9/imodels/util/convert.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/data_util.py` & `imodels-1.3.9/imodels/util/data_util.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/distillation.py` & `imodels-1.3.9/imodels/util/distillation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/explain_errors.py` & `imodels-1.3.9/imodels/util/explain_errors.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/extract.py` & `imodels-1.3.9/imodels/util/extract.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/metrics.py` & `imodels-1.3.9/imodels/util/metrics.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/neural_nets.py` & `imodels-1.3.9/imodels/util/neural_nets.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/prune.py` & `imodels-1.3.9/imodels/util/prune.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/rule.py` & `imodels-1.3.9/imodels/util/rule.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/score.py` & `imodels-1.3.9/imodels/util/score.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/transforms.py` & `imodels-1.3.9/imodels/util/transforms.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/tree.py` & `imodels-1.3.9/imodels/util/tree.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels/util/tree_interaction_utils.py` & `imodels-1.3.9/imodels/util/tree_interaction_utils.py`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/imodels.egg-info/PKG-INFO` & `imodels-1.3.9/imodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodels
-Version: 1.3.8
+Version: 1.3.9
 Summary: Implementations of various interpretable models
 Home-page: https://github.com/csinva/imodels
 Author: Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen, Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others
 Author-email: chandan_singh@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodels Version: 1.3.8 Summary: Implementations of
+Metadata-Version: 2.1 Name: imodels Version: 1.3.9 Summary: Implementations of
 various interpretable models Home-page: https://github.com/csinva/imodels
 Author: Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen,
 Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others Author-email:
 chandan_singh@berkeley.edu Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev
```

### Comparing `imodels-1.3.8/imodels.egg-info/SOURCES.txt` & `imodels-1.3.9/imodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/license.md` & `imodels-1.3.9/license.md`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/readme.md` & `imodels-1.3.9/readme.md`

 * *Files identical despite different names*

### Comparing `imodels-1.3.8/setup.py` & `imodels-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'corels',  # optinally requires corels for optimalrulelistclassifier
     'gosdt-deprecated',  # optionally requires gosdt for optimaltreeclassifier
     'irf',  # optionally require irf for iterativeRandomForestClassifier
 ]
 
 setuptools.setup(
     name="imodels",
-    version="1.3.8",
+    version="1.3.9",
     author="Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen, Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others",
     author_email="chandan_singh@berkeley.edu",
     description="Implementations of various interpretable models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/csinva/imodels",
     packages=setuptools.find_packages(
```

