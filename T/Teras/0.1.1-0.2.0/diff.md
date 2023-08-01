# Comparing `tmp/Teras-0.1.1.tar.gz` & `tmp/Teras-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Teras-0.1.1.tar", last modified: Fri Jul 14 19:44:00 2023, max compression
+gzip compressed data, was "Teras-0.2.0.tar", last modified: Tue Aug  1 18:09:08 2023, max compression
```

## Comparing `Teras-0.1.1.tar` & `Teras-0.2.0.tar`

### file list

```diff
@@ -1,150 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.869325 Teras-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-07-14 19:43:02.000000 Teras-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-14 19:44:00.869325 Teras-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-14 19:43:02.000000 Teras-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.853325 Teras-0.1.1/Teras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-14 19:43:02.000000 Teras-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:44:00.869325 Teras-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-14 19:43:02.000000 Teras-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.853325 Teras-0.1.1/teras/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/config/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/tabtransformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/ensemble/bagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/ensemble/stacking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/generative/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/generative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/impute/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/impute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/layerflow/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/layerflow/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/layerflow/layers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/common/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/node.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/tabtransformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.861325 Teras-0.1.1/teras/layerflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/dnfnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/ft_transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/rtdl_resnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/saint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    15754 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tabnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tabtransformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.865325 Teras-0.1.1/teras/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/activations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.865325 Teras-0.1.1/teras/layers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/ctgan_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/dnfnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/ft_transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/gain_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/oenf.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/oenf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/rtdl_resnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33470 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/saint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34959 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tabnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tabtransformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.865325 Teras-0.1.1/teras/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.865325 Teras-0.1.1/teras/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    23895 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.869325 Teras-0.1.1/teras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.869325 Teras-0.1.1/teras/preprocessing/base/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/base/base_data_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/oenf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.869325 Teras-0.1.1/teras/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.103215 Teras-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-01 18:07:59.000000 Teras-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-08-01 18:09:08.103215 Teras-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-08-01 18:07:59.000000 Teras-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.075214 Teras-0.2.0/Teras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 18:09:08.000000 Teras-0.2.0/Teras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-01 18:07:59.000000 Teras-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:09:08.103215 Teras-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 18:07:59.000000 Teras-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.075214 Teras-0.2.0/teras/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/activations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/config/tabtransformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/ensemble/bagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/ensemble/stacking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/generative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/impute/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/impute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/layerflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/layerflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/layerflow/layers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/common/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.079214 Teras-0.2.0/teras/layerflow/layers/saint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/saint_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/saint_projection_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/saint_reconstruction_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/layers/saint/saint_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.083215 Teras-0.2.0/teras/layerflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/dnfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/dnfnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/ft_transformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18548 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/rtdl_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/rtdl_resnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/saint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tabnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tabtransformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layerflow/models/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.083215 Teras-0.2.0/teras/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.083215 Teras-0.2.0/teras/layers/activation/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/activation/gumbel_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/activation/gumbel_softmax_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/categorical_feature_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/categorical_feature_embedding_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.083215 Teras-0.2.0/teras/layers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/common/transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/ctgan_discriminator_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/ctgan_discriminator_block_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/ctgan_generator_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ctgan/ctgan_generator_block_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/dnfnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnfnet_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnfnet_feature_selection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnfnet_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnfnet_localization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/dnfnet/dnnf_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/ft_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/ft_cls_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/ft_cls_token_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/ft_numerical_feature_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/ft_transformer/ft_numerical_feature_embedding_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/gain/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/gain_discriminator_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/gain_discriminator_block_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/gain_generator_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/gain/gain_generator_block_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/node_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/node_feature_selector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/odst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/node/odst_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/numerical_feature_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/numerical_feature_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/numerical_features_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/numerical_features_extractor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.087215 Teras-0.2.0/teras/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/label_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/label_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/periodic_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/preprocessing/periodic_embedding_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.091215 Teras-0.2.0/teras/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/cutmix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/regularization/mixup_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.091215 Teras-0.2.0/teras/layers/rtdl_resnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/rtdl_resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/rtdl_resnet/rtd_resnet_block_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/rtdl_resnet/rtdl_resnet_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.091215 Teras-0.2.0/teras/layers/saint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/multi_head_inter_sample_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/multi_head_inter_sample_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_numerical_feature_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_numerical_feature_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_projection_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_projection_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_reconstruction_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_reconstruction_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/saint/saint_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.091215 Teras-0.2.0/teras/layers/tabnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_attentive_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_attentive_transformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer_block_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabnet/tabnet_feature_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.095215 Teras-0.2.0/teras/layers/tabtransformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabtransformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabtransformer/tabtransformer_column_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/tabtransformer/tabtransformer_column_embedding_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.095215 Teras-0.2.0/teras/layers/vime/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_feature_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_feature_estimator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_mask_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_mask_estimator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_mask_generation_and_corruption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_mask_generation_and_corruption_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/layers/vime/vime_predictor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.095215 Teras-0.2.0/teras/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/losses/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.099215 Teras-0.2.0/teras/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/ctgan_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/dnfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/dnfnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/ft_transformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/gain_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/pcgain_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/rtdl_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/rtdl_resnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/saint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32249 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tabnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24544 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tabtransformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/models/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.099215 Teras-0.2.0/teras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.099215 Teras-0.2.0/teras/preprocessing/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/base/base_data_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/oenf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/preprocessing/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:09:08.103215 Teras-0.2.0/teras/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/dnfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-08-01 18:07:59.000000 Teras-0.2.0/teras/utils/vime.py
```

### Comparing `Teras-0.1.1/LICENSE` & `Teras-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/PKG-INFO` & `Teras-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: Teras
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Unified Deep Learning Library for Tabular Data
 Author: Khawaja Abaid
 Author-email: Khawaja Abaid <khawaja.abaid@gmail.com>
 Project-URL: Homepage, https://github.com/KhawajaAbaid/teras
 Project-URL: Bug Tracker, https://github.com/KhawajaAbaid/teras/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Teras — A Unified Deep Learning Library for Tabular Data
 
+![Teras logo banner](./data/imgs/Teras_logo_github_banner.jpg)
+
 Teras (short for Tabular Keras) is a unified deep learning library for Tabular Data that aims to be your one stop for everything related to deep learing with tabular data.
 
 It provides state of the art layers, models and arhitectures for all purposes, be it classification, regression or even data generation and imputation using state of the art deep learning architectures. 
 
 It also includes Preprocessing, Encoding and (Categorical and Numerical) Embedding layers. 
 
 While these state of the art architectures can be quite sophisticated, Teras, thanks to the incredible design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
@@ -27,46 +29,49 @@
 ## Installation:
 You can install Teras using pip as follows,
 ```
 pip install teras
 ```
 
 ## Getting Started
-Read our [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb) to...*drum roll* get started with Teras.
+Read our [Getting Started Guide](https://teras.readthedocs.io/en/latest/getting_started.html) to...*drum roll* get started with Teras.
 
 
 ## Documentation:
 You can access the documentation on ReadTheDocs.io: https://teras.readthedocs.io/en/latest/index.html
-Only the front page is a little messy but rest of the documentation should be good — though a lot of works needs to be done in this regard.
 
 ## Usage
 Teras provides two API for usage to satiate different levels of flexibility and accessibility needs:
 1. **Parametric API**: This is the default API, where user specifies values for parameters that are used in construction of any sub-layers or models within the architecture.
 ```
 from teras.models import TabNetClassifier
 
 model = TabNetClassifier(num_classes=2, features_metadata=features_metadata)
 ```
 2. **LayerFlow API**: It maximizes flexibility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
+Note that, there're no `<architecture>Classifier` or `<architecture>Regressor` model classes, but just one model class, which accepts a `head` layer that decides the model's final purpose.
 ```
-from teras.layerflow.models import TabNetClassifier
-from teras.layerflow.layers import TabNetEncoder, TabNetClassificationHead
+from teras.layerflow.models import TabNet
+from teras.layers import TabNetEncoder, CategoricalFeatureEmbedding, ClassificationHead
 
-encoder = TabNetEncoder()
-head = TabNetClassificationHead(num_classes=2)
-model = TabNetClassifier(features_metadata=features_metadata,
-                         encoder=encoder,
-                         head=head)
+embedding = CategoricalFeatureEmbedding(features_metadata, embedding_dim=1)     # TabNet requires embedding_dim to be 1
+encoder = TabNetEncoder(input_dim=input_dim)
+head = ClassificationHead(num_classes=2)
+model = TabNet(input_dim=input_dim,
+               features_metadata=features_metadata,
+               categorical_feature_embedding=embedding,
+               encoder=encoder,
+               head=head)
 ```
 You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 
 ## Main Teras Modules
 Teras offers following main modules:
 
-1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
+1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the **Teras APIs** section in the [Getting Started Guide](https://teras.readthedocs.io/en/latest/getting_started.html).
 2. `teras.layers`: It contains all the layers for all of the architectures offered by Teras.
 3. `teras.models`: It contains all of the models of all the architectures types, be it Classificaiton, Regresssion etc offered by Teras.
 4. `teras.generative`: It contains state of the art models for Data Generation. (Currently it offers `CTGAN` and `TVAE`).
 5. `teras.impute`: It contains state of the art models for Data Imputation. (Currently it offers `GAIN` and `PCGAIN`)
 6. `teras.preprocessing`: It offers preprocessing classes for data transformation and data sampling that are required by highly sophisticated models specifically the data generation and imputation models.
 7. `teras.ensemble`: It is a work in progress and aims to offers ensembling techniques making it easier than ever to ensemble your deep learning models, such as using Bagging or Stacking. (Currently it offers very basic version of these.)
 8. `teras.utils`: It contains useful utility functions making life easier for Teras users
```

### Comparing `Teras-0.1.1/README.md` & `Teras-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Teras — A Unified Deep Learning Library for Tabular Data
 
+![Teras logo banner](./data/imgs/Teras_logo_github_banner.jpg)
+
 Teras (short for Tabular Keras) is a unified deep learning library for Tabular Data that aims to be your one stop for everything related to deep learing with tabular data.
 
 It provides state of the art layers, models and arhitectures for all purposes, be it classification, regression or even data generation and imputation using state of the art deep learning architectures. 
 
 It also includes Preprocessing, Encoding and (Categorical and Numerical) Embedding layers. 
 
 While these state of the art architectures can be quite sophisticated, Teras, thanks to the incredible design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
@@ -13,46 +15,49 @@
 ## Installation:
 You can install Teras using pip as follows,
 ```
 pip install teras
 ```
 
 ## Getting Started
-Read our [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb) to...*drum roll* get started with Teras.
+Read our [Getting Started Guide](https://teras.readthedocs.io/en/latest/getting_started.html) to...*drum roll* get started with Teras.
 
 
 ## Documentation:
 You can access the documentation on ReadTheDocs.io: https://teras.readthedocs.io/en/latest/index.html
-Only the front page is a little messy but rest of the documentation should be good — though a lot of works needs to be done in this regard.
 
 ## Usage
 Teras provides two API for usage to satiate different levels of flexibility and accessibility needs:
 1. **Parametric API**: This is the default API, where user specifies values for parameters that are used in construction of any sub-layers or models within the architecture.
 ```
 from teras.models import TabNetClassifier
 
 model = TabNetClassifier(num_classes=2, features_metadata=features_metadata)
 ```
 2. **LayerFlow API**: It maximizes flexibility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
+Note that, there're no `<architecture>Classifier` or `<architecture>Regressor` model classes, but just one model class, which accepts a `head` layer that decides the model's final purpose.
 ```
-from teras.layerflow.models import TabNetClassifier
-from teras.layerflow.layers import TabNetEncoder, TabNetClassificationHead
+from teras.layerflow.models import TabNet
+from teras.layers import TabNetEncoder, CategoricalFeatureEmbedding, ClassificationHead
 
-encoder = TabNetEncoder()
-head = TabNetClassificationHead(num_classes=2)
-model = TabNetClassifier(features_metadata=features_metadata,
-                         encoder=encoder,
-                         head=head)
+embedding = CategoricalFeatureEmbedding(features_metadata, embedding_dim=1)     # TabNet requires embedding_dim to be 1
+encoder = TabNetEncoder(input_dim=input_dim)
+head = ClassificationHead(num_classes=2)
+model = TabNet(input_dim=input_dim,
+               features_metadata=features_metadata,
+               categorical_feature_embedding=embedding,
+               encoder=encoder,
+               head=head)
 ```
 You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 
 ## Main Teras Modules
 Teras offers following main modules:
 
-1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
+1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the **Teras APIs** section in the [Getting Started Guide](https://teras.readthedocs.io/en/latest/getting_started.html).
 2. `teras.layers`: It contains all the layers for all of the architectures offered by Teras.
 3. `teras.models`: It contains all of the models of all the architectures types, be it Classificaiton, Regresssion etc offered by Teras.
 4. `teras.generative`: It contains state of the art models for Data Generation. (Currently it offers `CTGAN` and `TVAE`).
 5. `teras.impute`: It contains state of the art models for Data Imputation. (Currently it offers `GAIN` and `PCGAIN`)
 6. `teras.preprocessing`: It offers preprocessing classes for data transformation and data sampling that are required by highly sophisticated models specifically the data generation and imputation models.
 7. `teras.ensemble`: It is a work in progress and aims to offers ensembling techniques making it easier than ever to ensemble your deep learning models, such as using Bagging or Stacking. (Currently it offers very basic version of these.)
 8. `teras.utils`: It contains useful utility functions making life easier for Teras users
```

### Comparing `Teras-0.1.1/Teras.egg-info/PKG-INFO` & `Teras-0.2.0/Teras.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: Teras
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Unified Deep Learning Library for Tabular Data
 Author: Khawaja Abaid
 Author-email: Khawaja Abaid <khawaja.abaid@gmail.com>
 Project-URL: Homepage, https://github.com/KhawajaAbaid/teras
 Project-URL: Bug Tracker, https://github.com/KhawajaAbaid/teras/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Teras — A Unified Deep Learning Library for Tabular Data
 
+![Teras logo banner](./data/imgs/Teras_logo_github_banner.jpg)
+
 Teras (short for Tabular Keras) is a unified deep learning library for Tabular Data that aims to be your one stop for everything related to deep learing with tabular data.
 
 It provides state of the art layers, models and arhitectures for all purposes, be it classification, regression or even data generation and imputation using state of the art deep learning architectures. 
 
 It also includes Preprocessing, Encoding and (Categorical and Numerical) Embedding layers. 
 
 While these state of the art architectures can be quite sophisticated, Teras, thanks to the incredible design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
@@ -27,46 +29,49 @@
 ## Installation:
 You can install Teras using pip as follows,
 ```
 pip install teras
 ```
 
 ## Getting Started
-Read our [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb) to...*drum roll* get started with Teras.
+Read our [Getting Started Guide](https://teras.readthedocs.io/en/latest/getting_started.html) to...*drum roll* get started with Teras.
 
 
 ## Documentation:
 You can access the documentation on ReadTheDocs.io: https://teras.readthedocs.io/en/latest/index.html
-Only the front page is a little messy but rest of the documentation should be good — though a lot of works needs to be done in this regard.
 
 ## Usage
 Teras provides two API for usage to satiate different levels of flexibility and accessibility needs:
 1. **Parametric API**: This is the default API, where user specifies values for parameters that are used in construction of any sub-layers or models within the architecture.
 ```
 from teras.models import TabNetClassifier
 
 model = TabNetClassifier(num_classes=2, features_metadata=features_metadata)
 ```
 2. **LayerFlow API**: It maximizes flexibility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
+Note that, there're no `<architecture>Classifier` or `<architecture>Regressor` model classes, but just one model class, which accepts a `head` layer that decides the model's final purpose.
 ```
-from teras.layerflow.models import TabNetClassifier
-from teras.layerflow.layers import TabNetEncoder, TabNetClassificationHead
+from teras.layerflow.models import TabNet
+from teras.layers import TabNetEncoder, CategoricalFeatureEmbedding, ClassificationHead
 
-encoder = TabNetEncoder()
-head = TabNetClassificationHead(num_classes=2)
-model = TabNetClassifier(features_metadata=features_metadata,
-                         encoder=encoder,
-                         head=head)
+embedding = CategoricalFeatureEmbedding(features_metadata, embedding_dim=1)     # TabNet requires embedding_dim to be 1
+encoder = TabNetEncoder(input_dim=input_dim)
+head = ClassificationHead(num_classes=2)
+model = TabNet(input_dim=input_dim,
+               features_metadata=features_metadata,
+               categorical_feature_embedding=embedding,
+               encoder=encoder,
+               head=head)
 ```
 You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 
 ## Main Teras Modules
 Teras offers following main modules:
 
-1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
+1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the **Teras APIs** section in the [Getting Started Guide](https://teras.readthedocs.io/en/latest/getting_started.html).
 2. `teras.layers`: It contains all the layers for all of the architectures offered by Teras.
 3. `teras.models`: It contains all of the models of all the architectures types, be it Classificaiton, Regresssion etc offered by Teras.
 4. `teras.generative`: It contains state of the art models for Data Generation. (Currently it offers `CTGAN` and `TVAE`).
 5. `teras.impute`: It contains state of the art models for Data Imputation. (Currently it offers `GAIN` and `PCGAIN`)
 6. `teras.preprocessing`: It offers preprocessing classes for data transformation and data sampling that are required by highly sophisticated models specifically the data generation and imputation models.
 7. `teras.ensemble`: It is a work in progress and aims to offers ensembling techniques making it easier than ever to ensemble your deep learning models, such as using Bagging or Stacking. (Currently it offers very basic version of these.)
 8. `teras.utils`: It contains useful utility functions making life easier for Teras users
```

### Comparing `Teras-0.1.1/pyproject.toml` & `Teras-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "tensorflow", "tensorflow-probability",
             "tensorflow-addons", "pandas", "numpy", "tqdm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Teras"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Khawaja Abaid", email="khawaja.abaid@gmail.com" },
 ]
 description = "A Unified Deep Learning Library for Tabular Data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `Teras-0.1.1/teras/__init__.py` & `Teras-0.2.0/teras/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/config/__init__.py` & `Teras-0.2.0/teras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/config/base.py` & `Teras-0.2.0/teras/config/base.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/config/saint.py` & `Teras-0.2.0/teras/config/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/config/tabnet.py` & `Teras-0.2.0/teras/config/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/ensemble/__init__.py` & `Teras-0.2.0/teras/preprocessing/base/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,12 +6,10 @@
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.5
+# limitations under the License.
 
-
-from .bagging import Bagging
-from .stacking import Stacking
+from .base_data_transformer import BaseDataTransformer
```

### Comparing `Teras-0.1.1/teras/ensemble/bagging.py` & `Teras-0.2.0/teras/ensemble/bagging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 from sklearn.model_selection import KFold, StratifiedKFold
-from typing import List
+from typing import List, Union
 import numpy as np
 
-INT_OR_FLOAT = List[int, float]
+INT_OR_FLOAT = Union[int, float]
 
 # NOTE: This is a very simple implementation of Bagging.
 # And mostly is for demonstration purpose.
 # Will make it efficient and better soon enough.
 # Also, currently there's just Bagging class, but my plan is to add
 # BaggingClassifier and BaggingRegressor like sklearn.
```

### Comparing `Teras-0.1.1/teras/ensemble/stacking.py` & `Teras-0.2.0/teras/ensemble/stacking.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/generative/__init__.py` & `Teras-0.2.0/teras/ensemble/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,13 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.5
 
 
-# CTGAN models
-from ..models.ctgan import CTGAN
-
-# TVAE models
-from ..models.tvae import TVAE
-
+from teras.ensemble.bagging import Bagging
+from teras.ensemble.stacking import Stacking
```

### Comparing `Teras-0.1.1/teras/impute/__init__.py` & `Teras-0.2.0/teras/impute/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.5
 
 
 # GAIN
-from ..models.gain import GAIN
+from teras.models.gain import GAIN
```

### Comparing `Teras-0.1.1/teras/layerflow/__init__.py` & `Teras-0.2.0/teras/layers/dnfnet/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,8 +6,13 @@
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitations under the License.
+
+
+from teras.layers.dnfnet.dnfnet_feature_selection import DNFNetFeatureSelection
+from teras.layers.dnfnet.dnfnet_localization import DNFNetLocalization
+from teras.layers.dnfnet.dnnf import DNNF
```

### Comparing `Teras-0.1.1/teras/layerflow/layers/common/__init__.py` & `Teras-0.2.0/teras/layers/node/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,7 +7,11 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+
+from teras.layers.node.odst import ObliviousDecisionTree
+from teras.layers.node.node_feature_selector import NodeFeatureSelector
```

### Comparing `Teras-0.1.1/teras/layerflow/layers/ft_transformer.py` & `Teras-0.2.0/teras/layerflow/models/rtdl_resnet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 from tensorflow import keras
-from tensorflow.keras import layers, models
-from teras.layers.ft_transformer import (NumericalFeatureEmbedding,
-                                         CLSToken,
-                                         ClassificationHead as _BaseClassificationHead,
-                                         RegressionHead as _BaseRegressionHead)
+from teras.utils.types import LayersCollection
+from typeguard import check_type
 
 
-class ClassificationHead(_BaseClassificationHead):
+@keras.saving.register_keras_serializable(package="teras.layerflow.models")
+class RTDLResNet(keras.Model):
     """
-    ClassificationHead with LayerFlow design for FTTransformer.
+    RTDLResNet model with LayerFlow desing.
+    It is based on the ResNet architecture proposed by Yury Gorishniy et al.
+    in the paper,
+    Revisiting Deep Learning Models for Tabular Data.
 
-    Args:
-        hidden_block: `layers.Layer | models.Model`,
-            An instance of anything that can serve as the hidden block in the
-            classification head.
-            It can be as simple as a single dense layer, or a custom layer that
-            uses a bunch of other dense and other fancy layers,
-            or may as well be a keras model -- as long as it satisfies the input
-            output constraints.
-            If None, a default hidden block specific to the current architecture
-            will be used.
-        output_layer: `layers.Layer`,
-            An instance of keras layer (Dense or a custom layer), with relevant
-            activation function for classification relevant to the task at hand.
-            If None, a default relevant output layer will be used.
-    """
-    def __init__(self,
-                 hidden_block: layers.Layer = None,
-                 output_layer: layers.Layer = None,
-                 **kwargs):
-        super().__init__(**kwargs)
-        if hidden_block is not None:
-            self.hidden_block = hidden_block
-
-        if output_layer is not None:
-            self.output_layer = output_layer
-
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'hidden_block': keras.layers.serialize(self.hidden_block),
-                      'output_layer': keras.layers.serialize(self.output_layer)
-                      }
-        config.update(new_config)
-        return config
-
-
-class RegressionHead(_BaseRegressionHead):
-    """
-    RegressionHead with LayerFlow design for FTTransformer.
+    Reference(s):
+        https://arxiv.org/abs/2106.11959
 
     Args:
-        hidden_block: `layers.Layer | models.Model`,
-            An instance of anything that can serve as the hidden block in the
-            regression head.
-            It can be as simple as a single dense layer, or a custom layer that
-            uses a bunch of other dense and other fancy layers,
-            or may as well be a keras model -- as long as it satisfies the input
-            output constraints.
-            If None, a default hidden block specific to the current architecture
-            will be used.
-        output_layer: `layers.Layer`,
-            An instance of keras layer (Dense or a custom layer),
-            for regression outputs relevant to the task at hand.
-            If None, a default relevant output layer will be used.
+        input_dim: ``int``,
+            The dimensionality of the input dataset,
+            or the number of features in the input dataset.
+
+        resnet_blocks: ``List[layers.Layer]`` or ``models.Model`` or ``keras.layers.Layer``,
+            List of ``RTDLResNetBlock`` layers to use in the ``RTDLResNet`` model.
+            You can pass either pass a list of instances of ``RTDLResNetBlock`` layers,
+            or pack them in a Keras model.
+            You can import the ``RTDLResNetBlock`` layer as follows,
+                >>> from teras.layers import RTDLResNetBlock
+
+        head: ``keras.layers.Layer``,
+            An instance of either ``ClassificationHead`` or ``RegressionHead`` layers,
+            depending on the task at hand.
+
+            You can import the ``ClassificationHead`` and ``RegressionHead`` layers as follows,
+                >>> from teras.layers import ClassificationHead
+                >>> from teras.layers import RegressionHead
     """
+
     def __init__(self,
-                 hidden_block: layers.Layer = None,
-                 output_layer: layers.Layer = None,
+                 input_dim: int,
+                 resnet_blocks: LayersCollection,
+                 head: keras.layers.Layer = None,
                  **kwargs):
-        super().__init__(**kwargs)
-        if hidden_block is not None:
-            self.hidden_block = hidden_block
-
-        if output_layer is not None:
-            self.output_layer = output_layer
+        # if not isinstance(resnet_blocks, LayersCollection):
+        try:
+            check_type("resnet_blocks", resnet_blocks, LayersCollection)
+        except TypeError:
+            raise TypeError("`resnet_blocks` can either be a list of `RTDLResNetBlock` layers "
+                            "or a Keras Layer or Model made up of `RTDLResNetBlock` layers. \n"
+                            f"But received type: {type(resnet_blocks)}.")
+        if isinstance(resnet_blocks, (list, tuple)):
+            resnet_blocks = keras.models.Sequential(resnet_blocks,
+                                                    name="resnet_blocks")
+
+        inputs = keras.layers.Input(shape=(input_dim,))
+        outputs = resnet_blocks(inputs)
+        if head is not None:
+            outputs = head(outputs)
+        super().__init__(inputs=inputs,
+                         outputs=outputs,
+                         **kwargs)
+        self.input_dim = input_dim
+        self.resnet_blocks = resnet_blocks
+        self.head = head
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'hidden_block': keras.layers.serialize(self.hidden_block),
-                      'output_layer': keras.layers.serialize(self.output_layer)
-                      }
-        config.update(new_config)
+        config.update({'input_dim': self.input_dim,
+                       'resnet_blocks': keras.layers.serialize(self.resnet_blocks),
+                       'head': keras.layers.serialize(self.head)
+                       })
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        resnet_blocks = keras.layers.deserialize(config.pop("resnet_blocks"))
+        head = keras.layers.deserialize(config.pop("head"))
+        return cls(input_dim=input_dim,
+                   resnet_blocks=resnet_blocks,
+                   head=head,
+                   **config)
```

### Comparing `Teras-0.1.1/teras/layerflow/layers/tabtransformer.py` & `Teras-0.2.0/teras/layerflow/models/dnfnet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,76 @@
 from tensorflow import keras
-from tensorflow.keras import layers, models
-from teras.layers.tabtransformer import (ClassificationHead as _BaseClassificationHead,
-                                         RegressionHead as _BaseRegressionHead)
+from teras.utils.types import LayersCollection
 
 
-class ClassificationHead(_BaseClassificationHead):
+@keras.saving.register_keras_serializable(package="teras.layerflow.models")
+class DNFNet(keras.Model):
     """
-    ClassificationHead with LayerFlow design for TabTransformerClassifier.
+    DNFNet model based on the DNFNet architecture with LayerFlow design.
+    DNFNet architecture is proposed by Liran Katzir et al.
+    in the paper,
+    "NET-DNF: Effective Deep Modeling Of Tabular Data."
 
-    Args:
-        hidden_block: `layers.Layer | models.Model`,
-            An instance of anything that can serve as the hidden block in the
-            classification head.
-            It can be as simple as a single dense layer, or a custom layer that
-            uses a bunch of other dense and other fancy layers,
-            or may as well be a keras model -- as long as it satisfies the input
-            output constraints.
-            If None, a default hidden block specific to the current architecture
-            will be used.
-        output_layer: `layers.Layer`,
-            An instance of keras layer (Dense or a custom layer), with relevant
-            activation function for classification relevant to the task at hand.
-            If None, a default relevant output layer will be used.
-    """
-    def __init__(self,
-                 hidden_block: layers.Layer = None,
-                 output_layer: layers.Layer = None,
-                 **kwargs):
-        super().__init__(**kwargs)
-        if hidden_block is not None:
-            self.hidden_block = hidden_block
-
-        if output_layer is not None:
-            self.output_layer = output_layer
-
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'hidden_block': keras.layers.serialize(self.hidden_block),
-                      'output_layer': keras.layers.serialize(self.output_layer)
-                      }
-        config.update(new_config)
-        return config
-
-
-class RegressionHead(_BaseRegressionHead):
-    """
-    RegressionHead with LayerFlow design for TabTransformerRegressor.
+    Reference(s):
+        https://openreview.net/forum?id=73WTGs96kho
 
     Args:
-        hidden_block: `layers.Layer | models.Model`,
-            An instance of anything that can serve as the hidden block in the
-            regression head.
-            It can be as simple as a single dense layer, or a custom layer that
-            uses a bunch of other dense and other fancy layers,
-            or may as well be a keras model -- as long as it satisfies the input
-            output constraints.
-            If None, a default hidden block specific to the current architecture
-            will be used.
-        output_layer: `layers.Layer`,
-            An instance of keras layer (Dense or a custom layer),
-            for regression outputs relevant to the task at hand.
-            If None, a default relevant output layer will be used.
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the input dataset.
+
+        dnnf_layers: ``List[layers.Layer]`` or ``keras.Model``,
+            A list of instances of ``DNNF`` layers or
+            a Keras layer or model made up of ``DNNF`` layers.
+            You can import the ``DNNF`` layer as follows,
+                >>> from teras.layers import DNNF
+
+        head: ``keras.layers.Layer``,
+            An instance of either ``ClassificationHead`` or ``RegressionHead`` layers,
+            depending on the task at hand.
+            You can import the ``ClassificationHead`` and ``RegressionHead`` layers as follows,
+                >>> from teras.layers import ClassificationHead
+                >>> from teras.layers import RegressionHead
     """
     def __init__(self,
-                 hidden_block: layers.Layer = None,
-                 output_layer: layers.Layer = None,
+                 input_dim: int,
+                 dnnf_layers: LayersCollection,
+                 head: keras.layers.Layer = None,
                  **kwargs):
-        super().__init__(**kwargs)
-        if hidden_block is not None:
-            self.hidden_block = hidden_block
-
-        if output_layer is not None:
-            self.output_layer = output_layer
+        if isinstance(dnnf_layers, (keras.layers.Layer, keras.models.Model)):
+            # keep it as is
+            dnnf_layers = dnnf_layers
+        elif isinstance(dnnf_layers, (list, tuple)):
+            dnnf_layers = keras.models.Sequential(dnnf_layers,
+                                                  name="dnnf_layers")
+        else:
+            raise ValueError("`dnnf_layers` can either be a list of `DNNF` layers, a Keras Layer, "
+                             f"or a Keras model model but received type: {type(dnnf_layers)}.")
+        inputs = keras.layers.Input(shape=(input_dim,))
+        outputs = dnnf_layers(inputs)
+        if head is not None:
+            outputs = head(outputs)
+        super().__init__(inputs=inputs,
+                         outputs=outputs,
+                         **kwargs)
+        self.input_dim = input_dim
+        self.dnnf_layers = dnnf_layers
+        self.head = head
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'hidden_block': keras.layers.serialize(self.hidden_block),
-                      'output_layer': keras.layers.serialize(self.output_layer)
-                      }
-        config.update(new_config)
+        config.update({'input_dim': self.input_dim,
+                       'dnnf_layers': keras.layers.serialize(self.dnnf_layers),
+                       'head': keras.layers.serialize(self.head)
+                       }
+                      )
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        dnnf_layers = keras.layers.deserialize(config.pop("dnnf_layers"))
+        head = keras.layers.deserialize(config.pop("head"))
+        return cls(input_dim=input_dim,
+                   dnnf_layers=dnnf_layers,
+                   head=head,
+                   **config)
```

### Comparing `Teras-0.1.1/teras/layerflow/models/__init__.py` & `Teras-0.2.0/teras/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,75 +9,72 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-# Simple Model
-from .simple import SimpleModel
-
-
-# TabTransfomer models
-from teras.layerflow.models.tabtransformer import (TabTransformer,
-                                                   TabTransformerClassifier,
-                                                   TabTransformerRegressor,
-                                                   TabTransformerPretrainer)
+# NODE models
+from teras.models.node import (NODE,
+                               NODEClassifier,
+                               NODERegressor)
 
 # TabNet models
-from teras.layerflow.models.tabnet import (TabNet,
-                                           TabNetRegressor,
-                                           TabNetClassifier)
-
-
-# SAINT models
-from teras.layerflow.models.saint import (SAINT,
-                                          SAINTClassifier,
-                                          SAINTRegressor,
-                                          SAINTPretrainer)
-
+from teras.models.tabnet import (TabNet,
+                                 TabNetClassifier,
+                                 TabNetRegressor,
+                                 TabNetPretrainer)
+
+# TabTransformer models
+from teras.models.tabtransformer import (TabTransformer,
+                                         TabTransformerClassifier,
+                                         TabTransformerRegressor)
 
-# FT Transformer models
-from teras.layerflow.models.ft_transformer import (FTTransformer,
-                                                   FTTransformerClassifier,
-                                                   FTTransformerRegressor)
 
 # DNFNet models
-from teras.layerflow.models.dnfnet import (DNFNet,
-                                           DNFNetClassifier,
-                                           DNFNetRegressor)
-
-
-# NODE models
-from teras.layerflow.models.node import (NODE,
-                                         NODEClassifier,
-                                         NODERegressor)
+from teras.models.dnfnet import (DNFNet,
+                                 DNFNetRegressor,
+                                 DNFNetClassifier)
 
+# SAINT models
+from teras.models.saint import (SAINT,
+                                SAINTClassifier,
+                                SAINTRegressor)
+
+
+# RTDL ResNet models
+from teras.models.rtdl_resnet import (RTDLResNetClassifier,
+                                      RTDLResNetRegressor)
+
+# RTDL FTTransformer models
+from teras.models.ft_transformer import (FTTransformer,
+                                         FTTransformerClassifier,
+                                         FTTransformerRegressor)
+
+# VIME models
+from teras.models.vime import (VimeSelf,
+                               VimeSemi)
 
-# RTDLResNet models
-from teras.layerflow.models.rtdl_resnet import (RTDLResNet,
-                                                RTDLResNetClassifier,
-                                                RTDLResNetRegressor)
 
+# CTGAN models
+from teras.models.ctgan import (CTGANGenerator,
+                                CTGANDiscriminator,
+                                CTGAN)
 
-# GAIN models
-from teras.layerflow.models.gain import (Generator as GAINGenerator,
-                                         Discriminator as GAINDiscriminator,
-                                         GAIN)
 
-# PCGAIN models
-from teras.layerflow.models.gain import (Generator as PCGAINGenerator,
-                                         Discriminator as PCGAINDiscriminator)
-from teras.layerflow.models.pcgain import (Classifier as PCGAINClassifier,
-                                           PCGAIN)
+# TVAE models
+from teras.models.tvae import (TVAEEncoder,
+                               TVAEDecoder,
+                               TVAE)
 
 
-# CTGAN models
-from teras.layerflow.models.ctgan import (Generator as CTGANGenerator,
-                                          Discriminator as CTGANDiscriminator,
-                                          CTGAN)
+# GAIN models
+from teras.models.gain import (GAINGenerator,
+                               GAINDiscriminator,
+                               GAIN)
 
 
-# TVAE models
-from teras.layerflow.models.tvae import (Encoder as TVAEEncoder,
-                                         Decoder as TVAEDecoder,
-                                         TVAE)
+# PCGAIN models
+from teras.models.pcgain import (PCGAINGenerator,
+                                 PCGAINDiscriminator,
+                                 PCGAINClassifier,
+                                 PCGAIN)
```

### Comparing `Teras-0.1.1/teras/layerflow/models/saint_test.py` & `Teras-0.2.0/teras/layers/saint/saint_reconstruction_head_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-from teras.layerflow.models.saint import SAINTClassifier, SAINTRegressor, SAINTPretrainer
+import tensorflow as tf
+from teras.layers.saint.saint_reconstruction_head import SAINTReconstructionHead
 from teras.utils import get_features_metadata_for_embedding
 import pandas as pd
 import numpy as np
-import pytest
 
 
-@pytest.fixture
-def setup_data():
-    data = {"length": np.ones(10),
-            "area": np.ones(10),
-            "color": ['green', 'yellow', 'green', 'orange', 'red',
-                      'orange', 'orange', 'green', 'red', 'red'],
-            "shape": ["circle", "square", "square", "rectangle", "circle",
-                      "square", "circle", "rectangle", "circle", "square"]}
-    categorical_feats = ["color", "shape"]
-    numerical_feats = ["length", "area"]
+def test_saint_reconstruction_head_output_shape():
+    data = pd.DataFrame({"income": np.ones(10),
+                         "goals": np.ones(10),
+                         'player_level': [5, 7, 9, 8, 9, 10, 9, 7, 8, 9],
+                         'shirt_number': [7, 10, 10, 7, 7, 10, 10, 10, 7, 10]})
+    categorical_feats = ["player_level", "shirt_number"]
+    numerical_feats = ["income", "goals"]
     features_metadata = get_features_metadata_for_embedding(pd.DataFrame(data),
                                                             categorical_features=categorical_feats,
                                                             numerical_features=numerical_feats)
-    return data, features_metadata
-
-
-def test_saint_classifier_works(setup_data):
-    data, features_metadata = setup_data
-    saint_classifier = SAINTClassifier(features_metadata=features_metadata)
-    saint_classifier(data)
-
-
-def test_saint_regressor_works(setup_data):
-    data, features_metadata = setup_data
-    saint_regressor = SAINTRegressor(features_metadata=features_metadata)
-    saint_regressor(data)
-
-
-# TODO add tests for pretrainer
+    sum_of_features_cardinalities = sum(map(lambda x: len(features_metadata["categorical"][x][1]),
+                                            features_metadata["categorical"])
+                                        ) + len(numerical_feats)
+
+    saint_reconstruction_head = SAINTReconstructionHead(features_metadata,
+                                                        embedding_dim=32)
+    inputs = tf.ones(shape=(16, 4, 32), dtype=tf.float32)
+    outputs = saint_reconstruction_head(inputs)
+    assert len(tf.shape(outputs)) == 2
+    assert tf.shape(outputs)[0] == 16
+    assert tf.shape(outputs)[1] == sum_of_features_cardinalities
```

### Comparing `Teras-0.1.1/teras/layerflow/models/tabtransformer.py` & `Teras-0.2.0/teras/layerflow/models/saint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,312 +1,368 @@
+import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers, models
-from teras.layers.tabtransformer import (ClassificationHead,
-                                         RegressionHead)
-from teras.models import (TabTransformer as BaseTabTransformer,
-                          TabTransformerPretrainer)
-from teras.layerflow.models import SimpleModel
+from teras.losses.saint import info_nce_loss, denoising_loss
 
 
-class TabTransformer(BaseTabTransformer):
+@keras.saving.register_keras_serializable(package="teras.layerflow.models.backbones")
+class SAINT(keras.Model):
     """
-    Base TabTransformer model class with LayerFlow design.
-
-    TabTransformer architecture is proposed by Xin Huang et al.
+    SAINT architecture with LayerFlow design.
+    It proposed by Gowthami Somepalli et al.
     in the paper,
-    TabTransformer: Tabular Data Modeling Using Contextual Embeddings.
+    SAINT: Improved Neural Networks for Tabular Data
+    via Row Attention and Contrastive Pre-Training.
 
-    TabTransformer is a novel deep tabular data modeling architecture for
-    supervised and semi-supervised learning.
-    The TabTransformer is built upon self-attention based Transformers.
-    The Transformer layers transform the embeddings of categorical features
-    into robust contextual embeddings to achieve higher prediction accuracy.
+    SAINT performs attention over both rows and columns.
 
     Reference(s):
-        https://arxiv.org/abs/2012.06678
+        https://arxiv.org/abs/2106.01342
 
     Args:
-        features_metadata: `dict`,
-            a nested dictionary of metadata for features where
-            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
-            feature indices and the lists of unique values (vocabulary) in them,
-            while numerical dictionary is a mapping of numerical feature names to their indices.
-            `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
-            `{feature_name: feature_idx}` for feature in numerical features.
-            You can get this dictionary from
-                >>> from teras.utils import get_features_metadata_for_embedding
-                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
-                                                                        numerical_features,
-                                                                        categorical_features)
-        categorical_feature_embedding: `layers.Layer`,
-            An instance of `CategoricalFeatureEmbedding` layer to embedd categorical features
-            or any layer that can work in place of `CategoricalFeatureEmbedding` for that purpose.
-            If None, a `CategoricalFeatureEmbedding` layer with default values will be used.
-            You can import the `CategoricalFeatureEmbedding` layer as follows,
-                >>> from teras.layerflow.layers import CategoricalFeatureEmbedding
-
-        column_embedding: `layers.Layer`,
-            An instance of `TabTransformerColumnEmbedding` layer to apply over categorical embeddings,
-            or any layer that can work in place of `TabTransformerColumnEmbedding` for that purpose.
-            If None, a `TabTransformerColumnEmbedding` layer with default values will be used.
-            You can import the `TabTransformerColumnEmbedding` layer as follows,
-                >>> from teras.layerflow.layers import TabTColumnEmbedding
-
-        encoder: `layers.Layer`,
-            An instance of Encoder layer to encode feature embeddings,
-            or any layer that can work in place of Encoder for that purpose.
-            If None, an Encoder layer with default values will be used.
-                >>> from teras.layerflow.layers import Encoder
-
-        head: `layers.Layer`,
-            An instance of ClassificationHead or RegressionHead layer for final outputs,
-            or any layer that can work in place of a Head layer for that purpose.
+        input_dim: ``int``,
+            Dimensionality of the input dataset.
+
+        encoder: ``keras.layers.Layer``,
+            An instance of `SAINTEncoder` layer to encode the features embeddings,
+            or any layer that can work in its place for that purpose.
+            If None, a ``SAINTEncoder`` layer with default values will be used.
+            You can import the ``SAINTEncoder`` layer as follows,
+                >>> from teras.layerflow.layers import SAINTEncoder
+
+        categorical_feature_embedding: ``keras.layers.Layer``,
+            An instance of ``CategoricalFeatureEmbedding`` layer to embedd categorical features
+            or any layer that can work in its palce for that purpose.
+            If None, a ``CategoricalFeatureEmbedding`` layer with default values will be used.
+            You can import the ``CategoricalFeatureEmbedding`` layer as follows,
+                >>> from teras.layers import CategoricalFeatureEmbedding
+
+        numerical_feature_embedding: ``keras.layers.Layer``,
+            An instance of ``SAINTNumericalFeatureEmbedding`` layer to embedd numerical features
+            or any layer that can work in its place for that purpose.
+            If None, a ``SAINTNumericalFeatureEmbedding`` layer with default values will be used.
+            You can import the ``SAINTNumericalFeatureEmbedding`` layer as follows,
+                >>> from teras.layers import SAINTNumericalFeatureEmbedding
+
+        head: ``keras.layers.Layer``,
+            An instance of either ``ClassificationHead`` or ``RegressionHead`` layers,
+            depending on the task at hand.
+
+            REMEMBER: In case you're using this model as a base model for pretraining, you MUST leave
+            this argument as None.
+
+            You can import the ``ClassificationHead`` and ``RegressionHead`` layers as follows,
+                >>> from teras.layers import ClassificationHead
+                >>> from teras.layers import RegressionHead
     """
     def __init__(self,
-                 features_metadata: dict,
-                 categorical_feature_embedding: layers.Layer = None,
-                 column_embedding: layers.Layer = None,
-                 encoder: layers.Layer = None,
-                 head: layers.Layer = None,
+                 input_dim: int,
+                 categorical_feature_embedding: keras.layers.Layer = None,
+                 numerical_feature_embedding: keras.layers.Layer = None,
+                 encoder: keras.layers.Layer = None,
+                 head: keras.layers.Layer = None,
                  **kwargs):
-        super().__init__(features_metadata=features_metadata,
-                         **kwargs)
-        if categorical_feature_embedding is not None:
-            self.categorical_feature_embedding = categorical_feature_embedding
+        if categorical_feature_embedding is None and numerical_feature_embedding is None:
+            raise ValueError("Both `categorical_feature_embedding` and `numerical_feature_embedding` "
+                             "cannot be None at the same time as a tabular dataset must contains "
+                             "features of at least one of the types if not both. ")
+
+        if encoder is None:
+            raise ValueError("`encoder` cannot be None. Please pass an instance of `SAINTEncoder` layer. "
+                             "You can import it as, `from teras.layerflow.layers import SAINTEncoder``")
+
+        inputs = keras.layers.Input(shape=(input_dim,))
+
+        if categorical_feature_embedding is None:
+            # then there's only numerical features because we already
+            # have a check above that both categorical and numerical embeddings
+            # cannot be None at the same time
+            feature_embeddings = numerical_feature_embedding(inputs)
+        else:
+            categorical_embeddings = categorical_feature_embedding(inputs)
+            numerical_embeddings = numerical_feature_embedding(inputs)
+            feature_embeddings = keras.layers.Concatenate(axis=1)([categorical_embeddings, numerical_embeddings])
 
-        if column_embedding is not None:
-            self.column_embedding = column_embedding
+        outputs = encoder(feature_embeddings)
 
-        if encoder is not None:
-            self.encoder = encoder
+        if head is not None:
+            outputs = head(outputs)
 
+        super().__init__(inputs=inputs,
+                         outputs=outputs,
+                         **kwargs)
+
+        self.input_dim = input_dim
+        self.encoder = encoder
+        self.categorical_feature_embedding = categorical_feature_embedding
+        self.numerical_feature_embedding = numerical_feature_embedding
         self.head = head
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'categorical_feature_embedding': keras.layers.serialize(self.categorical_feature_embedding),
-                      'column_embedding': keras.layers.serialize(self.column_embedding),
-                      'encoder': keras.layers.serialize(self.encoder),
-                      'head': keras.layers.serialize(self.head),
-                      }
-        config.update(new_config)
+        config.update({'input_dim': self.input_dim,
+                       'categorical_feature_embedding': keras.layers.serialize(self.categorical_feature_embedding),
+                       'numerical_feature_embedding': keras.layers.serialize(self.numerical_feature_embedding),
+                       'encoder': keras.layers.serialize(self.encoder),
+                       'head': keras.layers.serialize(self.head),
+                       })
         return config
 
-
-class TabTransformerClassifier(TabTransformer):
-    """
-    TabTransformerClassifier model class with LayerFlow design.
-
-    TabTransformer architecture is proposed by Xin Huang et al.
-    in the paper,
-    TabTransformer: Tabular Data Modeling Using Contextual Embeddings.
-
-    TabTransformer is a novel deep tabular data modeling architecture for
-    supervised and semi-supervised learning.
-    The TabTransformer is built upon self-attention based Transformers.
-    The Transformer layers transform the embeddings of categorical features
-    into robust contextual embeddings to achieve higher prediction accuracy.
-
-    Reference(s):
-        https://arxiv.org/abs/2012.06678
-
-    Args:
-        features_metadata: `dict`,
-            a nested dictionary of metadata for features where
-            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
-            feature indices and the lists of unique values (vocabulary) in them,
-            while numerical dictionary is a mapping of numerical feature names to their indices.
-            `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
-            `{feature_name: feature_idx}` for feature in numerical features.
-            You can get this dictionary from
-                >>> from teras.utils import get_features_metadata_for_embedding
-                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
-                                                                        numerical_features,
-                                                                        categorical_features)
-
-        categorical_feature_embedding: `layers.Layer`,
-            An instance of `CategoricalFeatureEmbedding` layer to embedd categorical features
-            or any layer that can work in place of `CategoricalFeatureEmbedding` for that purpose.
-            If None, a `CategoricalFeatureEmbedding` layer with default values will be used.
-            You can import the `CategoricalFeatureEmbedding` layer as follows,
-                >>> from teras.layerflow.layers import CategoricalFeatureEmbedding
-
-        column_embedding: `layers.Layer`,
-            An instance of `TabTransformerColumnEmbedding` layer to apply over categorical embeddings,
-            or any layer that can work in place of `TabTransformerColumnEmbedding` for that purpose.
-            If None, a `TabTransformerColumnEmbedding` layer with default values will be used.
-            You can import the `TabTransformerColumnEmbedding` layer as follows,
-                >>> from teras.layerflow.layers import TabTColumnEmbedding
-
-        encoder: `layers.Layer`,
-            An instance of Encoder layer to encode feature embeddings,
-            or any layer that can work in place of Encoder for that purpose.
-            If None, an Encoder layer with default values will be used.
-                >>> from teras.layerflow.layers import Encoder
-
-        head: `layers.Layer`,
-            An instance of `TabTClassificationHead` layer for the final outputs,
-            or any layer that can work in place of a `TabTClassificationHead` layer for that purpose.
-            If None, `TabTClassificationHead` layer with default values will be used.
-            You can import the `TabTClassificationHead` as follows,
-                >>> from teras.layerflow.layers import TabTClassificationHead
-    """
-
-    def __init__(self,
-                 features_metadata: dict,
-                 categorical_feature_embedding: layers.Layer = None,
-                 column_embedding: layers.Layer = None,
-                 encoder: layers.Layer = None,
-                 head: layers.Layer = None,
-                 **kwargs):
-        if head is None:
-            num_classes = 2
-            activation_out = None
-            if "num_classes" in kwargs:
-                num_classes = kwargs.pop("num_classes")
-            if "activation_out" in kwargs:
-                activation_out = kwargs.pop("activation_out")
-            head = ClassificationHead(num_classes=num_classes,
-                                      activation_out=activation_out,
-                                      name="tabtransformer_classification_head")
-        super().__init__(features_metadata=features_metadata,
-                         categorical_feature_embedding=categorical_feature_embedding,
-                         column_embedding=column_embedding,
-                         encoder=encoder,
-                         head=head,
-                         **kwargs)
-
     @classmethod
-    def from_pretrained(cls,
-                        pretrained_model: TabTransformer,
-                        head: layers.Layer = None
-                        ):
-        """
-        Class method to create a TabTransformer Classifier model instance from
-        a pretrained base TabTransformer model instance.
-
-        Args:
-            pretrained_model: `TabTransformer`,
-                A pretrained base TabTransformer model instance.
-           head: `layers.Layer`,
-                An instance of `TabTClassificationHead` layer for the final outputs,
-                or any layer that can work in place of a `TabTClassificationHead` layer for that purpose.
-                If None, `TabTClassificationHead` layer with default values will be used.
-                You can import `TabTClassificationHead` as follows,
-                    >>> from teras.layerflow.layers import TabTClassificationHead
-
-        Returns:
-            A TabTransformer Classifier instance based of the pretrained model.
-        """
-        if head is None:
-            head = ClassificationHead(name="tabtransformer_classification_head")
-        model = SimpleModel(body=pretrained_model,
-                            head=head,
-                            name="tabtransformer_classifier_pretrained")
-        return model
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        encoder = keras.layers.deserialize(config.pop("encoder"))
+        categorical_feature_embedding = keras.layers.deserialize(config.pop("categorical_feature_embedding"))
+        numerical_feature_embedding = keras.layers.deserialize(config.pop("numerical_feature_embedding"))
+        head = keras.layers.deserialize(config.pop("head"))
+        return cls(input_dim=input_dim,
+                   categorical_feature_embedding=categorical_feature_embedding,
+                   numerical_feature_embedding=numerical_feature_embedding,
+                   encoder=encoder,
+                   head=head,
+                   **config)
 
 
-class TabTransformerRegressor(TabTransformer):
+@keras.saving.register_keras_serializable(package="teras.layerflow.models")
+class SAINTPretrainer(keras.Model):
     """
-    TabTransformerRegressor model class with LayerFlow design.
-
-    TabTransformer architecture is proposed by Xin Huang et al.
+    SAINTPretrainer model with LayerFlow design.
+    It is based on the pretraining architecture of the SAINT model
+    proposed by Gowthami Somepalli et al.
     in the paper,
-    TabTransformer: Tabular Data Modeling Using Contextual Embeddings.
+    SAINT: Improved Neural Networks for Tabular Data
+    via Row Attention and Contrastive Pre-Training.
 
-    TabTransformer is a novel deep tabular data modeling architecture for
-    supervised and semi-supervised learning.
-    The TabTransformer is built upon self-attention based Transformers.
-    The Transformer layers transform the embeddings of categorical features
-    into robust contextual embeddings to achieve higher prediction accuracy.
+    SAINT performs attention over both rows and columns.
 
     Reference(s):
-        https://arxiv.org/abs/2012.06678
+        https://arxiv.org/abs/2106.01342
 
     Args:
-        features_metadata: `dict`,
+        model: ``keras.Model``,
+            An instance of the ``SAINT`` model that is to be pretrained.
+
+        features_metadata: ``dict``,
             a nested dictionary of metadata for features where
             categorical sub-dictionary is a mapping of categorical feature names to a tuple of
             feature indices and the lists of unique values (vocabulary) in them,
             while numerical dictionary is a mapping of numerical feature names to their indices.
             `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
             `{feature_name: feature_idx}` for feature in numerical features.
             You can get this dictionary from
                 >>> from teras.utils import get_features_metadata_for_embedding
                 >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
-                                                                        numerical_features,
-                                                                        categorical_features)
-        categorical_feature_embedding: `layers.Layer`,
-            An instance of `CategoricalFeatureEmbedding` layer to embedd categorical features
-            or any layer that can work in place of `CategoricalFeatureEmbedding` for that purpose.
-            If None, a `CategoricalFeatureEmbedding` layer with default values will be used.
-            You can import the `CategoricalFeatureEmbedding` layer as follows,
-                >>> from teras.layerflow.layers import CategoricalFeatureEmbedding
-
-        column_embedding: `layers.Layer`,
-            An instance of `TabTransformerColumnEmbedding` layer to apply over categorical embeddings,
-            or any layer that can work in place of `TabTransformerColumnEmbedding` for that purpose.
-            If None, a `TabTransformerColumnEmbedding` layer with default values will be used.
-            You can import the `TabTransformerColumnEmbedding` layer as follows,
-                >>> from teras.layerflow.layers import TabTColumnEmbedding
-
-        encoder: `layers.Layer`,
-            An instance of Encoder layer to encode feature embeddings,
-            or any layer that can work in place of Encoder for that purpose.
-            If None, an Encoder layer with default values will be used.
-                >>> from teras.layerflow.layers import Encoder
-
-        head: `layers.Layer`,
-            An instance of `TabTRegressionHead` layer for the final outputs,
-            or any layer that can work in place of a `TabTRegressionHead` layer for that purpose.
-            If None, `TabTRegressionHead` layer with default values will be used.
-            You can import `TabTRegressionHead` as follows,
-                >>> from teras.layerflow.layers import TabTRegressionHead
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        mixup: ``keras.layers.Layer``,
+            An instance of ``MixUp`` layer or any custom layer that can work
+            in its place.
+            You can import the ``MixUp`` layer as follows,
+                >>> from teras.layers import MixUp
+
+        cutmix: ``keras.layers.Layer``,
+            An instance of ``CutMix`` layer or any custom layer that can work
+            in its place.
+            You can import the `CutMix` layer as follows,
+                >>> from teras.layers import CutMix
+
+        projection_head_1: ``keras.layers.Layer``,
+            An instance of ``SAINTProjectionHead`` layer that is used to project embeddings
+            of *real* samples to a lower dimensionality before reconstructing the inputs.
+            You can import the ``SAINTProjectionHead`` layer as follows,
+                >>> from teras.layerflow.layers import SAINTProjectionHead
+
+        projection_head_2: ``keras.layers.Layer``,
+            An instance of ``SAINTProjectionHead`` layer that is used to project embeddings
+            of *augmented* samples to a lower dimensionality before reconstructing the inputs.
+            You can import the ``SAINTProjectionHead`` layer as follows,
+                >>> from teras.layerflow.layers import SAINTProjectionHead
+
+        reconstruction_head: ``keras.layers.Layer``,
+            An instance of ``SAINTReconstructionHead`` which applies a separate ``ReconstructionHeadBlock``
+            to reconstruct the input features.
+            You can import the ``SAINTReconstructionHead`` as follows,
+                >>> from teras.layerflow.layers import SAINTReconstructionHead
+
+        temperature: ``float``, default 0.7,
+            Temperature value used in the computation of the InfoNCE contrastive loss.
+
+        lambda_: ``float``, default 10,
+            Controls the weightage of denoising loss in the summation of denoising and
+            contrastive loss.
     """
     def __init__(self,
+                 model: keras.Model,
                  features_metadata: dict,
-                 categorical_feature_embedding: layers.Layer = None,
-                 column_embedding: layers.Layer = None,
-                 encoder: layers.Layer = None,
-                 head: layers.Layer = None,
+                 mixup: keras.layers.Layer = None,
+                 cutmix: keras.layers.Layer = None,
+                 projection_head_1: keras.layers.Layer = None,
+                 projection_head_2: keras.layers.Layer = None,
+                 reconstruction_head: keras.layers.Layer = None,
+                 temperature: float = 0.7,
+                 lambda_: float = 10.,
                  **kwargs):
-        if head is None:
-            num_outputs = 1
-            if "num_outputs" in kwargs:
-                num_outputs = kwargs.pop("num_outputs")
-            head = RegressionHead(num_outputs=num_outputs,
-                                  name="tatransformer_regression_head")
-        super().__init__(features_metadata=features_metadata,
-                         categorical_feature_embedding=categorical_feature_embedding,
-                         column_embedding=column_embedding,
-                         encoder=encoder,
-                         head=head,
-                         **kwargs)
+        super().__init__(**kwargs)
+        self.model = model
+        if mixup is None:
+            raise ValueError("`mixup` cannot be None. Please pass an instance of `MixUp` layer. "
+                             "You can import it as, `from teras.layers import MixUp`")
+
+        if cutmix is None:
+            raise ValueError("`cutmix` cannot be None. Please pass an instance of `CutMix` layer. "
+                             "You can import it as, `from teras.layers import CutMix``")
+
+        if projection_head_1 is None:
+            raise ValueError("`projection_head_1` cannot be None. "
+                             "Please pass an instance of `SAINTProjectionHead` layer. "
+                             "You can import it as, `from teras.layers import SAINTProjectionHead``")
+
+        if projection_head_2 is None:
+            raise ValueError("`projection_head_2` cannot be None. "
+                             "Please pass an instance of `SAINTProjectionHead` layer. "
+                             "You can import it as, `from teras.layers import SAINTProjectionHead`")
+
+        if reconstruction_head is None:
+            raise ValueError("`reconstruction_head` cannot be None. "
+                             "Please pass an instance of `SAINTReconstructionHead` layer. "
+                             "You can import it as, `from teras.layers import SAINTReconstructionHead`")
+
+        self.features_metadata = features_metadata
+        self._categorical_features_exist = len(self.features_metadata["categorical"]) > 0
+        self._numerical_features_exist = len(self.features_metadata["numerical"]) > 0
+
+        self.mixup = mixup
+        self.cutmix = cutmix
+        self.projection_head_1 = projection_head_1
+        self.projection_head_2 = projection_head_2
+        self.reconstruction_head = reconstruction_head
+        self.temperature = temperature
+        self.lambda_ = lambda_
+
+        self.contrastive_loss_tracker = keras.metrics.Mean(name="contrastive_loss")
+        self.denoising_loss_tracker = keras.metrics.Mean(name="denoising_loss")
+
+    def get_pretrained_model(self):
+        """Returns pretrained model"""
+        return self.model
+
+    @property
+    def pretrained_model(self):
+        """Returns pretrained model"""
+        return self.model
+
+    def compile(self,
+                contrastive_loss=info_nce_loss,
+                denoising_loss=denoising_loss,
+                **kwargs):
+        super().compile(**kwargs)
+        self.contrastive_loss = contrastive_loss
+        self.denoising_loss = denoising_loss
+
+    def call(self, inputs):
+        x = inputs
+
+        # Apply cutmix on the raw input space
+        x_prime = self.cutmix(x)
+
+        # Embed the raw inputs as well as cutmixed data
+        p = None
+        p_prime = None
+        if self._categorical_features_exist:
+            p = self.model.categorical_feature_embedding(x)
+            p_prime = self.model.categorical_feature_embedding(x_prime)
+
+        if self._numerical_features_exist:
+            numerical_features = self.model.numerical_feature_embedding(x)
+            numerical_features_prime = self.model.numerical_feature_embedding(x_prime)
+            if p is not None:
+                p = tf.concat([p, numerical_features],
+                              axis=1)
+                p_prime = tf.concat([p_prime, numerical_features_prime],
+                                    axis=1)
+            else:
+                p = numerical_features
+                p_prime = numerical_features_prime
+
+        # Apply mixup on the embedding space -- only to the augment data
+        p_prime = self.mixup(p_prime)
+
+        # Pass these embeddings through saint encoder
+        r = self.model.encoder(p)
+        r_prime = self.model.encoder(p_prime)
+
+        # Pass the encoded features through projection heads
+        z = self.projection_head_1(r)
+        z_prime = self.projection_head_2(r_prime)
+        # Normalize
+        z = z / tf.norm(z, axis=-1, keepdims=True)
+        z_prime = z_prime / tf.norm(z_prime, axis=-1, keepdims=True)
+        # Flatten last two dimensions
+        z = tf.reshape(z, shape=(tf.shape(z)[0], tf.reduce_prod(tf.shape(z)[1:])))
+        z_prime = tf.reshape(z_prime, shape=(tf.shape(z_prime)[0], tf.reduce_prod(tf.shape(z_prime)[1:])))
+
+        # To reconstruct the input data, we pass the encodings of augmented data
+        # i.e. the `r_prime` through a reconstruction head
+        reconstructed_samples = self.reconstruction_head(r_prime)
+
+        return z, z_prime, reconstructed_samples
+
+    def train_step(self, data):
+        if isinstance(data, tuple):
+            data = data[0]
+
+        with tf.GradientTape() as tape:
+            z, z_prime, reconstructed_samples = self(data)
+            c_loss = self.contrastive_loss(real_projection_outputs=z,
+                                           augmented_projection_outputs=z_prime,
+                                           temperature=self.temperature)
+            d_loss = self.denoising_loss(real_samples=data,
+                                         reconstructed_samples=reconstructed_samples,
+                                         categorical_features_metadata=self.features_metadata["categorical"])
+
+            loss = c_loss + self.lambda_ * d_loss
+        gradients = tape.gradient(loss, self.trainable_weights)
+        self.optimizer.apply_gradients(zip(gradients, self.trainable_weights))
+
+        self.contrastive_loss_tracker.update_state(c_loss)
+        self.denoising_loss_tracker.update_state(d_loss)
+        # If user has passed any additional metrics to compile, we should update their states
+        if len(self.compiled_metrics.metrics) > 0:
+            self.compiled_metrics.update_state(data, reconstructed_samples)
+        # If user has passed any additional losses to compile, we should call them
+        if self.compiled_loss._losses is not None:
+            self.compiled_loss(data, reconstructed_samples)
+        results = {m.name: m.result() for m in self.metrics}
+        return results
+
+    def get_config(self):
+        config = super().get_config()
+        new_config = {'model': keras.layers.serialize(self.model),
+                      'features_metadata': self.features_metadata,
+                      'mixup': keras.layers.serialize(self.mixup),
+                      'cutmix': keras.layers.serialize(self.cutmix),
+                      'projection_head_1': keras.layers.serialize(self.projection_head_1),
+                      'projection_head_2': keras.layers.serialize(self.projection_head_2),
+                      'reconstruction_head': keras.layers.serialize(self.reconstruction_head),
+                      'temperature': self.temperature,
+                      'lambda_': self.lambda_,
+                      }
+        config.update(new_config)
+        return config
 
     @classmethod
-    def from_pretrained(cls,
-                        pretrained_model: TabTransformer,
-                        head: layers.Layer = None,
-                        ):
-        """
-        Class method to create a TabTransformer Regressor model instance from
-        a pretrained base TabTransformer model instance.
-
-        Args:
-            pretrained_model: `TabTransformer`,
-                A pretrained base TabTransformer model instance.
-            head: `layers.Layer`,
-                An instance of RegressionHead layer for the final outputs,
-                or any layer that can work in place of a RegressionHead layer for that purpose.
-                If None, RegressionHead layer with default values will be used.
-                You can import `TabTRegressionHead` as follows,
-                    >>> from teras.layerflow.layers import TabTRegressionHead
-
-        Returns:
-            A TabTransformer Regressor instance based of the pretrained model.
-        """
-        if head is None:
-            head = RegressionHead(name="tabtransformer_regression_head")
-        model = SimpleModel(body=pretrained_model,
-                            head=head,
-                            name="tabtransformer_regressor_pretrained")
-        return model
+    def from_config(cls, config):
+        model = keras.layers.deserialize(config.pop("model"))
+        features_metadata = config.pop("features_metadata")
+        mixup = keras.layers.deserialize(config.pop("mixup"))
+        cutmix = keras.layers.deserialize(config.pop("cutmix"))
+        projection_head_1 = keras.layers.deserialize(config.pop("projection_head_1"))
+        projection_head_2 = keras.layers.deserialize(config.pop("projection_head_2"))
+        reconstruction_head = keras.layers.deserialize(config.pop("reconstruction_head"))
+        return cls(model=model,
+                   features_metadata=features_metadata,
+                   mixup=mixup,
+                   cutmix=cutmix,
+                   projection_head_1=projection_head_1,
+                   projection_head_2=projection_head_2,
+                   reconstruction_head=reconstruction_head,
+                   **config)
```

### Comparing `Teras-0.1.1/teras/layerflow/models/tvae.py` & `Teras-0.2.0/teras/models/tvae.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,223 @@
+import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers, models
-from teras.models.tvae import (Encoder as _BaseEncoder,
-                               Decoder as _BaseDecoder,
-                               TVAE as _BaseTVAE)
-from typing import Union
+from teras.layerflow.models.tvae import TVAE as _TVAE_LF
+from teras.utils.types import UnitsValuesType
 
-LAYER_OR_MODEL = Union[layers.Layer, models.Model]
 
-
-class Encoder(_BaseEncoder):
+@keras.saving.register_keras_serializable(package="teras.models")
+class TVAEEncoder(keras.Model):
     """
-    Encoder for the TVAE model with LayerFlow design.
-    TVAE is proposed by
+    Encoder for the TVAE model as proposed by
     Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        compression_block: `layers.Layer`, `List[layers.Layer]` or `models.Model`,
-            An instance of Keras Dense layer, list of layers or Keras model
-            that can work as the compression block for the Encoder model.
-            If None, a compression made up of two dense layers of 128 dimensionality
-            is used.
-        latent_dim: `int`, default 128.
+        latent_dim: ``int``, default 128.
             Dimensionality of the learned latent space
+
+        units_values: ``List[int]`` or ``Tuple[int]``, default (128, 128),
+            A list or tuple of integers.
+            For each value in the sequence, a dense layer of that
+            dimensions (units) is added to construct a compression block.
     """
     def __init__(self,
-                 compression_block: LAYER_OR_MODEL = None,
                  latent_dim: int = 128,
+                 units_values: UnitsValuesType = (128, 128),
                  **kwargs):
-        super().__init__(latent_dim=latent_dim,
-                         **kwargs)
+        super().__init__(**kwargs)
 
-        if compression_block is not None:
-            if isinstance(compression_block, (layers.Layer, models.Model)):
-                # leave it as is
-                compression_block = compression_block
-            elif isinstance(compression_block, (list, tuple)):
-                compression_block = models.Sequential(compression_block,
-                                                      name="encoder_compression_block")
-            else:
-                raise TypeError("`compression_block` can either be a Keras layer, list of layers or a keras model "
-                                f"but received type: {type(compression_block)} which is not supported.")
-            self.compression_block = compression_block
+        if not isinstance(units_values, (list, tuple)):
+            raise ValueError(f"""`units_values` must be a list or tuple of units which determines
+                        the number of compression layers and the dimensionality of those layers.
+                        Received: {units_values}""")
+
+        self.latent_dim = latent_dim
+        self.units_values = units_values
+
+        self.compression_block = keras.models.Sequential(name="compression_block")
+        for i, units in enumerate(self.units_values, start=1):
+            self.compression_block.add(keras.layers.Dense(units=units,
+                                                          activation="relu",
+                                                          name=f"compression_layer_{i}"))
+        self.dense_mean = keras.layers.Dense(units=self.latent_dim,
+                                             name="mean")
+        self.dense_log_var = keras.layers.Dense(units=self.latent_dim,
+                                                name="log_var")
+
+    def call(self, inputs):
+        h = self.compression_block(inputs)
+        mean = self.dense_mean(h)
+        log_var = self.dense_log_var(h)
+        std = tf.exp(0.5 * log_var)
+        return mean, std, log_var
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'compression_block': keras.layers.serialize(self.compression_block),
+        new_config = {'latent_dim': self.latent_dim,
+                      'units_values': self.units_values
                       }
         config.update(new_config)
         return config
 
 
-class Decoder(_BaseDecoder):
+@keras.saving.register_keras_serializable(package="teras.models")
+class TVAEDecoder(keras.Model):
     """
     Encoder for the TVAE model as proposed by
     Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
         data_dim: `int`,
-            Dimensionality of the input dataset.
-        decompression_block: `layers.Layer` or `models.Model`, decompresses the compressed
-            latent dimension data back to original data dimensions.
-            Note, the last layer of decompression_block must project the data back to
-            original dimensions i.e. `data_dim`.
+            Dimensionality of the input dataset. It is used to create the last layer for
+            the decompression_block that projects data back to the original dimensions.
+        units_values: `List[int]` or `Tuple[int]`,
+            A list or tuple of integers. For each value in the sequence,
+            a dense layer of that dimensionality is added to construct a decompression block.
+            Note that, a dense layer of `data_dim` is also appended at the of decompression
+            block to project data back to the original data dimensions.
     """
     def __init__(self,
                  data_dim: int = None,
-                 decompression_block: LAYER_OR_MODEL = None,
+                 units_values: UnitsValuesType = (128, 128),
                  **kwargs):
-        super().__init__(data_dim=data_dim,
-                         **kwargs)
+        super().__init__(**kwargs)
 
-        if decompression_block is not None:
-            if isinstance(decompression_block, (layers.Layer, models.Model)):
-                # leave it as is
-                decompression_block = decompression_block
-            elif isinstance(decompression_block, (list, tuple)):
-                decompression_block = models.Sequential(decompression_block,
-                                                        name="decoder_decompression_block")
-            else:
-                raise TypeError("`decompression_block` can either be a Keras layer, list of layers or a keras model "
-                                f"but received type: {type(decompression_block)} which is not supported.")
-            self.decompression_block = decompression_block
+        if data_dim is None:
+            raise ValueError("`data_dim` cannot be None, "
+                             "as `data_dim` value is required to project data back to original data dimensions.")
+
+        if not isinstance(units_values, (list, tuple)):
+            raise ValueError(f"""`units_values` must be a list or tuple of units which determines
+                        the number of decompression layers and the dimensionality of those layers.
+                        Received: {units_values}""")
+
+        self.data_dim = data_dim
+        self.units_values = units_values
+
+        self.decompression_block = keras.models.Sequential(name="decompression_block")
+        for i, units in enumerate(self.units_values, start=1):
+            self.decompression_block.add(keras.layers.Dense(units=units,
+                                                            activation="relu",
+                                                            name=f"decompression_layer_{i}"
+                                                            )
+                                         )
+        self.decompression_block.add(keras.layers.Dense(units=self.data_dim,
+                                                        name="projection_to_data_dim"))
+
+        self.sigmas = tf.Variable(initial_value=keras.initializers.ones()(shape=(self.data_dim,)) * 0.1,
+                                  trainable=True,
+                                  name="sigmas")
+
+    def call(self, inputs):
+        x_generated = self.decompression_block(inputs)
+        return x_generated, self.sigmas
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'decompression_block': keras.layers.serialize(self.decompression_block),
+        new_config = {'data_dim': self.data_dim,
+                      'units_values': self.units_values
                       }
         config.update(new_config)
         return config
 
 
-class TVAE(_BaseTVAE):
+@keras.saving.register_keras_serializable(package="teras.models")
+class TVAE(_TVAE_LF):
     """
-    TVAE model with LayerFlow design.
-    TVAE is a tabular data generation architecture proposed by the
+    TVAE model for tabular data generation
+    based on the architecture proposed by the
     Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        data_dim: `int`, dimensionality of the input dataset.
-            It should be the dimensionality of the dataset that is passed to the `fit`
-            method and not necessarily the dimensionality of the original input data
-            as sometimes data transformations can alter the dimensionality of the data.
-            Conveniently, if you're using DataSampler class, you can access `.data_dim`
-            attribute to get the dimensionality of data.
-        meta_data: `dict`,
+        input_dim: ``int``, dimensionality of the input dataset.
+            The dimensionality of the input dataset.
+
+            Note the dimensionality must be equal to the dimensionality of dataset
+            that is passed to the fit method and not necessarily the dimensionality
+            of the raw input dataset as sometimes data transformation alters the
+            dimensionality of the dataset.
+
+            You can access the dimensionality of the transformed dataset through the
+            ``.data_dim`` attribute of the ``TVAEDataSampler`` instance used in sampling
+            the dataset.
+
+        metadata: ``dict``,
             A dictionary containing metadata for all features in the input data.
             This metadata is computed during the data transformation step and can be accessed
-            from `.get_meta_data()` method of DataTransformer instance.
-        encoder: `layers.Layer` or `models.Model`.
-            An instance of `TVAEEncoder` or any custom keras layer/model that can work
-            in its place.
-            It encodes or compresses data to useful hidden dimensional representations.
-            If `None`, a default encoder is constructed with (128, 128)
-            dimensions is constructed.
-            You can import the `TVAEEncoder` as follows,
-                >>> from teras.layerflow.models import TVAEEncoder
-        decoder: `layers.Layer` or `models.Model`
-            An instance of `TVAEDecoder` or any custom keras model/layer that can work
-            in its palce.
-            It decodes or decompresses from latent dimensions to data dimensions.
-            If `None`, a default decoder is constructed with (128, 128) hidden
-            dimensions along with a dense output layer that projects the data
-            back to original dimensions.
-            You can import the `TVAEDecoder` as follows,
-                >>> from teras.layerflow.models import TVAEDecoder
+            from ``.get_metadata()`` method of ``TVAEDataTransformer`` instance.
+
+        units_values: ``List[int]`` or ``Tuple[int]``, default (128, 128),
+            A list or tuple of units to construct the compression block in ``TVAEEncoder``.
+            For each value in the sequence, a dense layer of that
+            dimensions (units) is added to construct a compression block.
+
+        decoder_units_values: ``List[int]`` or ``Tuple[int]``,
+            A list or tuple of units to construct the decompression block in ``TVAEDecoder``.
+            For each value in the sequence,
+            a dense layer of that dimensionality is added to construct a decompression block.
+            Note that, a dense layer of ``data_dim`` is also appended at the of decompression
+            block to project data back to the original data dimensions.
+
         latent_dim: `int`, default 128,
-            Dimensionality of the learned latent space
+            Dimensionality of the learned latent space.
+
         loss_factor: `float`, default 2,
             Hyperparameter used in the computation of ELBO loss for TVAE.
             It controls how much the cross entropy loss contributes to the overall loss.
             It is directly proportional to the cross entropy loss.
     """
     def __init__(self,
-                 data_dim: int = None,
-                 meta_data: dict = None,
-                 encoder: LAYER_OR_MODEL = None,
-                 decoder: LAYER_OR_MODEL = None,
+                 input_dim: int,
+                 metadata: dict = None,
+                 encoder_units_values: UnitsValuesType = (128, 128),
+                 decoder_units_values: UnitsValuesType = (128, 128),
                  latent_dim: int = 128,
-                 loss_factor=2,
+                 loss_factor: float = 2,
                  **kwargs):
-        super().__init__(data_dim=data_dim,
-                         meta_data=meta_data,
+        if metadata is None:
+            raise ValueError("`metadata` cannot be None. "
+                             "You can access it through `.get_metadata()` method of the `TVAEDataTransformer` instance.")
+        encoder = TVAEEncoder(latent_dim=latent_dim,
+                              units_values=encoder_units_values)
+        decoder = TVAEDecoder(data_dim=input_dim,
+                              units_values=decoder_units_values)
+        super().__init__(encoder=encoder,
+                         decoder=decoder,
                          latent_dim=latent_dim,
                          loss_factor=loss_factor,
                          **kwargs)
-
-        if encoder is not None:
-            self.encoder = encoder
-
-        if decoder is not None:
-            self.decoder = decoder
+        self.input_dim = input_dim
+        self.metadata = metadata
+        self.encoder_units_values = encoder_units_values
+        self.decoder_units_values = decoder_units_values
+        self.latent_dim = latent_dim
+        self.loss_factor = loss_factor
 
     def get_config(self):
-        config = super().get_config()
-        new_config = {'encoder': keras.layers.serialize(self.encoder),
-                      'decoder': keras.layers.serialize(self.decoder)
-                      }
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'input_dim': self.input_dim,
+                  'metadata': self.metadata,
+                  'encoder_units_values': self.encoder_units_values,
+                  'decoder_units_values': self.decoder_units_values,
+                  'latent_dim': self.latent_dim,
+                  'loss_factor': self.loss_factor,
+                  }
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        return cls(input_dim=input_dim,
+                   **config)
```

### Comparing `Teras-0.1.1/teras/layers/activations.py` & `Teras-0.2.0/teras/layers/activation/gumbel_softmax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,44 @@
 import tensorflow as tf
-from tensorflow.keras import layers
+from tensorflow import keras
+from teras.activations import gumbel_softmax
 
-class GLU(layers.Layer):
-    """Generalized linear unit nonlinear activation."""
-    def __init__(self,
-                units,
-                **kwagrs):
-        super().__init__(**kwagrs)
-        self.units = units
-    
-    def call(self, inputs):
-        return inputs[:, :self.units] * tf.nn.sigmoid(inputs[:, self.units:])
-
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'units': self.units}
-        config.update(new_config)
-        return config
-
-
-class GEGLU(layers.Layer):
-    """GeGLU is an activation function which is a variant of GLU"""
-    def __init__(self):
-        super().__init__()
-
-    def call(self, inputs):
-        x, gates = tf.split(inputs,
-                            num_or_size_splits=2,
-                            axis=-1)
-        return x * tf.nn.gelu(gates)
 
-
-class GumbelSoftmax(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers.activation")
+class GumbelSoftmax(keras.layers.Layer):
     """
     Implementation of the Gumbel Softmax activation
     proposed by Eric Jang et al. in the paper
     Categorical Reparameterization with Gumbel-Softmax
 
     Reference(s):
         https://arxiv.org/abs/1611.01144
 
     Args:
-        temperature: Controls the sharpness or smoothness of the resulting probability distribution.
+        temperature: ``float``, default 0.2,
+            Controls the sharpness or smoothness of the resulting probability distribution.
             A higher temperature value leads to a smoother and more uniform probability distribution.
             Conversely, a lower temperature value makes the distribution concentrated around
-            the category with the highest probability. Defaults to 0.2
-        hard: Whether to return soft probabilities or hard one hot vectors. Defaults to False.
+            the category with the highest probability.
+
+        hard: ``bool``, default False,
+            Whether to return soft probabilities or hard one hot vectors.
     """
     def __init__(self,
-                 temperature=0.2,
+                 temperature: float = 0.2,
                  hard: bool = False,
                  **kwargs):
         super().__init__(**kwargs)
         self.temperature = temperature
         self.hard = hard
 
-    def call(self, logits):
-        u = tf.random.uniform(tf.shape(logits),
-                                    minval=0,
-                                    maxval=1)
-        gumbels = -tf.math.log(-tf.math.log(u))
-        perturbed_logits = (logits + gumbels) / self.temperature
-        probabilities = tf.nn.softmax(perturbed_logits)
-        if self.hard:
-            one_hot_labels = tf.one_hot(tf.argmax(probabilities, axis=-1), tf.shape(logits)[-1])
-            return one_hot_labels
-        return probabilities
+    def call(self, logits: tf.Tensor):
+        return gumbel_softmax(logits,
+                              temperature=self.temperature,
+                              hard=self.hard)
 
     def get_config(self):
         config = super().get_config()
         new_config = {'temperature': self.temperature,
                       'hard': self.hard}
         config.update(new_config)
         return config
```

### Comparing `Teras-0.1.1/teras/layers/common/__init__.py` & `Teras-0.2.0/teras/layers/tabtransformer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,8 +6,11 @@
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.5
+# limitations under the License.
+
+
+from teras.layers.tabtransformer.tabtransformer_column_embedding import TabTransformerColumnEmbedding
```

### Comparing `Teras-0.1.1/teras/layers/common/head.py` & `Teras-0.2.0/teras/layers/common/head.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,121 @@
 from tensorflow import keras
-from tensorflow.keras import layers, models
 from teras.utils import get_normalization_layer
-from typing import List, Tuple, Union
+from teras.utils.types import (UnitsValuesType,
+                               NormalizationType,
+                               ActivationType)
 
 
-LIST_OR_TUPLE = Union[List[int], Tuple[int]]
-LAYER_OR_STR = Union[keras.layers.Layer, str]
-
-
-class RegressionHead(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers.common")
+class RegressionHead(keras.layers.Layer):
     """
-    Regression head to use on top of the architectures for regression.
+    Regression Head to use on top of the architectures for regression.
 
     Args:
-        num_outputs: `int`, default 1, Number of regression outputs to predict.
-        units_values: `List[int] | Tuple[int]`, default (64, 32), for each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the RegressionHead.
-        activation_hidden: default "relu", Activation function to use in hidden dense layers.
-        normalization: `Layer | str`, default "batch", Normalization layer to use.
+        num_outputs: ``int``, default 1,
+            Number of regression outputs to predict.
+
+        units_values: ``List[int]`` or ``Tuple[int]``, default (64, 32),
+            For each value in the sequence a hidden layer of that dimension
+            preceded by a normalization layer (if specified) is
+            added to the ``RegressionHead``.
+
+        activation_hidden: ``callable`` or ``str``, default "relu",
+            Activation function to use in hidden dense layers.
+
+        normalization: ``keras.layers.Layer`` or ``str``, default "batch",
+            Normalization layer to use.
             If specified a normalization layer is applied after each hidden layer.
             If None, no normalization layer is applied.
             You can either pass a keras normalization layer or name for a layer implemented by keras.
     """
     def __init__(self,
                  num_outputs: int = 1,
-                 units_values: LIST_OR_TUPLE = (64, 32),
-                 activation_hidden="relu",
-                 normalization: LAYER_OR_STR = "batch",
+                 units_values: UnitsValuesType = (64, 32),
+                 activation_hidden: ActivationType = "relu",
+                 normalization: NormalizationType = "batch",
                  **kwargs):
         super().__init__(**kwargs)
         self.num_outputs = num_outputs
         self.units_values = units_values
         self.activation_hidden = activation_hidden
         self.normalization = normalization
 
         self.hidden_block = None
         if self.units_values is not None:
             self.hidden_block = keras.models.Sequential(name="inner_head")
             for units in self.units_values:
                 if self.normalization is not None:
                     self.hidden_block.add(get_normalization_layer(self.normalization))
-                self.hidden_block.add(layers.Dense(units,
-                                                   activation=self.activation_hidden))
-        self.output_layer = layers.Dense(self.num_outputs)
-
-    # def build(self, input_shape):
-    #     self.hidden_block.build(input_shape)
+                self.hidden_block.add(keras.layers.Dense(units,
+                                                         activation=self.activation_hidden))
+        self.output_layer = keras.layers.Dense(self.num_outputs)
 
     def call(self, inputs):
         x = inputs
         if self.hidden_block is not None:
             x = self.hidden_block(x)
         outputs = self.output_layer(x)
         return outputs
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_outputs': self.num_outputs,
-                      'units_values': self.units_values,
-                      'activation_hidden': self.activation_hidden,
-                      'normalization': self.normalization}
-        config.update(new_config)
+
+        if isinstance(self.activation_hidden, str):
+            activation_hidden_serialized = self.activation_hidden
+        else:
+            activation_hidden_serialized = keras.layers.serialize(self.activation_hidden)
+
+        if isinstance(self.normalization, str):
+            normalization_serialized = self.normalization
+        else:
+            normalization_serialized = keras.layers.serialize(self.normalization)
+
+        config.update({'num_outputs': self.num_outputs,
+                       'units_values': self.units_values,
+                       'activation_hidden': activation_hidden_serialized,
+                       'normalization': normalization_serialized}
+                      )
         return config
 
 
-class ClassificationHead(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers.common")
+class ClassificationHead(keras.layers.Layer):
     """
     Classification head to use on top of the architectures for classification.
 
     Args:
-        num_classes: `int`, default 2, Number of classes to predict.
-        units_values: `List[int] | Tuple[int]`, default (64, 32), for each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the ClassificationHead.
-        activation_hidden: default "relu", Activation function to use in hidden dense layers.
-        activation_out: Activation function to use for the output layer.
+        num_classes: ``int``, default 2,
+            Number of classes to predict.
+
+        units_values: ``List[int]`` or ``Tuple[int]``, default (64, 32),
+            For each value in the sequence a hidden layer of that dimension
+            preceded by a normalization layer (if specified) is
+            added to the ``ClassificationHead``.
+
+        activation_hidden: ``callable``, ``keras.layers.Layer``, or ``str``, default "relu",
+            Activation function to use in hidden dense layers.
+
+        activation_out: ``callable``, ``keras.layers.Layer``, or ``str``,
+            Activation function to use for the output layer.
             If not specified, `sigmoid` is used for binary and `softmax` is used for
             multiclass classification.
-        normalization: `Layer | str`, default "batch", Normalization layer to use.
+
+        normalization: ``keras.layers.Layer`` or ``str``, default "batch",
+            Normalization layer to use.
             If specified a normalization layer is applied after each hidden layer.
             If None, no normalization layer is applied.
             You can either pass a keras normalization layer or name for a layer implemented by keras.
     """
     def __init__(self,
                  num_classes: int = 2,
-                 units_values: LIST_OR_TUPLE = (64, 32),
-                 activation_hidden="relu",
-                 activation_out=None,
-                 normalization: LAYER_OR_STR = "batch",
+                 units_values: UnitsValuesType = (64, 32),
+                 activation_hidden: ActivationType = "relu",
+                 activation_out: ActivationType = None,
+                 normalization: NormalizationType = "batch",
                  **kwargs):
         super().__init__(**kwargs)
         self.num_classes = 1 if num_classes <= 2 else num_classes
         self.units_values = units_values
         self.activation_hidden = activation_hidden
         self.activation_out = activation_out
         if self.activation_out is None:
@@ -101,28 +124,44 @@
 
         self.hidden_block = None
         if self.units_values is not None:
             self.hidden_block = keras.models.Sequential(name="inner_head")
             for units in self.units_values:
                 if self.normalization is not None:
                     self.hidden_block.add(get_normalization_layer(self.normalization))
-                self.hidden_block.add(layers.Dense(units,
-                                                   activation=self.activation_hidden))
-        self.output_layer = layers.Dense(self.num_classes,
-                                         activation=self.activation_out)
+                self.hidden_block.add(keras.layers.Dense(units,
+                                                         activation=self.activation_hidden))
+        self.output_layer = keras.layers.Dense(self.num_classes,
+                                               activation=self.activation_out)
 
     def call(self, inputs):
         x = inputs
         if self.hidden_block is not None:
             x = self.hidden_block(x)
         outputs = self.output_layer(x)
         return outputs
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_classes': self.num_outputs,
-                      'units_values': self.units_values,
-                      'activation_hidden': self.activation_hidden,
-                      'activation_out': self.activation_out,
-                      'normalization': self.normalization}
-        config.update(new_config)
+
+        if isinstance(self.activation_hidden, str):
+            activation_hidden_serialized = self.activation_hidden
+        else:
+            activation_hidden_serialized = keras.layers.serialize(self.activation_hidden)
+
+        if isinstance(self.activation_out, str):
+            activation_out_serialized = self.activation_out
+        else:
+            activation_out_serialized = keras.layers.serialize(self.activation_out)
+
+        if isinstance(self.normalization, str):
+            normalization_serialized = self.normalization
+        else:
+            normalization_serialized = keras.layers.serialize(self.normalization)
+
+        config.update({'num_classes': self.num_classes,
+                       'units_values': self.units_values,
+                       'activation_hidden': activation_hidden_serialized,
+                       'activation_out': activation_out_serialized,
+                       'normalization': normalization_serialized}
+                      )
         return config
```

### Comparing `Teras-0.1.1/teras/layers/common/head_test.py` & `Teras-0.2.0/teras/layers/common/head_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/layers/common/transformer.py` & `Teras-0.2.0/teras/layers/common/transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,206 +1,224 @@
-import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers, models
-from teras.layers.activations import GEGLU
-from typing import List, Tuple, Union
+from teras.utils import get_activation
+from teras.layerflow.layers.common.transformer import (FeedForward as _FeedForwardLF,
+                                                       Transformer as _TransformerLF,
+                                                       Encoder as _EncoderLF)
+from teras.utils.types import ActivationType
 
 
-LIST_OR_TUPLE = Union[List[int], Tuple[int]]
-LAYER_OR_STR = Union[keras.layers.Layer, str]
-
-
-class FeedForward(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers.common")
+class FeedForward(_FeedForwardLF):
     """
-    FeedForward layer that is used in the Transformer layer of the Encoder block
+    FeedForward layer that is used in the ``Transformer`` layer of the ``Encoder`` block
     of Transformer architecture.
     It is shared by all transformer based architectures for tabular data.
     The first layer expands the inputs to `embedding dimensions` times `multiplier`
     and the second layer projects them back to the embedding dimensions.
-    Usually, since the feed forward layer follows the MultiHeadAttention layer
+    Usually, since the feed forward layer follows the ``MultiHeadAttention`` layer
     whose outputs are of `embedding dimensions` so it essentially takes
     MultiHeadAttention layer's outputs as inputs, expands them to input dimensions
     times the multiplier and then projects them back to the input dimensions.
 
     Args:
-        embedding_dim: `int`, default 16, Embedding dimensions used in the given
+        embedding_dim: `int`, default 16,
+            Embedding dimensions used in the given
             architecture to usually embedded the numerical features but at times
             to also embedd the numerical features like in SAINT architecture.
-        multiplier: `int`, default 4, Multiplier that is multipled with embedding dims
+
+        multiplier: ``int``, default 4,
+            Multiplier that is multipled with embedding dims
             and the resultant value is used as hidden dimensions.
-        dropout: Dropout rate to use in the dropout layer that is applied after
+
+        dropout: ``float``, default 0.,
+            Dropout rate to use in the dropout layer that is applied after
             the hidden layer.
-        activation: Activation function to use in the hidden layer.
-            By default, GEGLU activation is used, which isn't offered by Keras by is offered by Teras.
-            You can import it using
-            `from teras.layers import GEGLU()`
+
+        activation: default "geglu",
+            Activation function to use in the hidden layer.
+            By default, ``geglu`` activation is used.
+            You can import it as,
+                >>> from teras.activations import geglu
     """
     def __init__(self,
-                 embedding_dim: int = 16,
+                 embedding_dim: int = 32,
                  multiplier: int = 4,
                  dropout: float = 0.,
-                 activation="geglu",
+                 activation: ActivationType = "geglu",
                  **kwargs):
-        super().__init__(**kwargs)
+        hidden_block = keras.models.Sequential(name="feed_forward_hidden_block")
+        hidden_block.add(keras.layers.Dense(embedding_dim * multiplier,
+                                            activation=get_activation(activation)))
+        hidden_block.add(keras.layers.Dropout(dropout))
+        output_layer = keras.layers.Dense(embedding_dim)
+
+        super().__init__(hidden_block=hidden_block,
+                         output_layer=output_layer,
+                         **kwargs)
+
         self.embedding_dim = embedding_dim
         self.multiplier = multiplier
         self.dropout = dropout
-        self.activation = GEGLU() if activation.lower() == "geglu" else activation
-        self.hidden_block = models.Sequential(name="feed_forward_hidden_block")
-        self.hidden_block.add(layers.Dense(self.embedding_dim * self.multiplier,
-                                           activation=self.activation))
-        self.hidden_block.add(layers.Dropout(self.dropout))
-        self.output_layer = layers.Dense(self.embedding_dim)
-
-    def call(self, inputs):
-        x = self.hidden_block(inputs)
-        outputs = self.output_layer(x)
-        return outputs
+        self.activation = activation
 
     def get_config(self):
-        config = super().get_config()
-        new_config = {'embedding_dim': self.embedding_dim,
-                      'multiplier': self.multiplier,
-                      'dropout': self.dropout,
-                      'activation': self.activation}
-        config.update(new_config)
+        activation_serialized = self.activation
+        if not isinstance(activation_serialized, str):
+            activation_serialized = keras.layers.serialize(activation_serialized)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'embedding_dim': self.embedding_dim,
+                  'multiplier': self.multiplier,
+                  'dropout': self.dropout,
+                  'activation': activation_serialized}
         return config
 
 
-class Transformer(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers.common")
+class Transformer(_TransformerLF):
     """
     Transformer layer that is used as a building block for
-    constructing the Encoder block of transformer based architectures.
-    It applies the MultiHeadAttention followed by the FeedForward layer
+    constructing the ``Encoder`` block of transformer based architectures.
+    It applies the ``MultiHeadAttention`` followed by the FeedForward layer
     and also employs residual connections.
 
     Args:
-        num_attention_heads: `int`, default 8, Number of heads to use
-            in the MultiHeadAttention layer.
-        embedding_dim: `int`, default 32, emebdding dimensions being
-            used in the overall architecture.
+        num_attention_heads: ``int``, default 8,
+            Number of heads to use in the ``MultiHeadAttention`` layer.
+
+        embedding_dim: ``int``, default 32,
+            Embedding dimensions being used in the overall architecture.
             These serve as the `key dimensions` in the
-            `MultiHeadAttention` layer and are multiplied by the
-            `mutliplier` in the `FeedForward` layer to compute the
+            ``MultiHeadAttention`` layer and are multiplied by the
+            ``mutliplier`` in the ``FeedForward`` layer to compute the
             hidden dimensions to project the inputs into.
-        attention_dropout: `float`, default 0., Dropout rate for
-            the MultiHeadAttention layer.
-        feedforward_dropout: `float`, default 0., Dropout rate to use
-            in for the dropout layer in the FeedForward layer.
-        norm_epsilon: `float`, default 1e-6, Normalization value to
-            use for LayerNormalization layer.
+
+        attention_dropout: ``float``, default 0.,
+            Dropout rate for the ``MultiHeadAttention`` layer.
+
+        feedforward_dropout: ``float``, default 0.,
+            Dropout rate to use in for the dropout layer in the ``FeedForward`` layer.
+
+        norm_epsilon: ``float``, default 1e-6,
+            Normalization value to use for ``LayerNormalization`` layer.
     """
     def __init__(self,
                  embedding_dim: int = 32,
                  num_attention_heads: int = 8,
                  attention_dropout: float = 0.,
                  feedforward_dropout: float = 0.,
                  feedforward_multiplier: int = 4,
                  norm_epsilon: float = 1e-6,
                  **kwagrs):
-        super().__init__(**kwagrs)
+        multi_head_attention = keras.layers.MultiHeadAttention(
+            num_heads=num_attention_heads,
+            key_dim=embedding_dim,
+            dropout=attention_dropout
+        )
+        layer_norm_1 = keras.layers.LayerNormalization(epsilon=norm_epsilon)
+        feed_forward = FeedForward(embedding_dim,
+                                   multiplier=feedforward_multiplier,
+                                   dropout=feedforward_dropout)
+        layer_norm_2 = keras.layers.LayerNormalization(epsilon=norm_epsilon)
+        super().__init__(multi_head_attention=multi_head_attention,
+                         feed_forward=feed_forward,
+                         layer_norm_1=layer_norm_1,
+                         layer_norm_2=layer_norm_2,
+                         **kwagrs)
         self.embedding_dim = embedding_dim
         self.num_attention_heads = num_attention_heads
         self.attention_dropout = attention_dropout
         self.feedforward_dropout = feedforward_dropout
         self.feedforward_multiplier = feedforward_multiplier
         self.norm_epsilon = norm_epsilon
 
-        self.multi_head_attention = layers.MultiHeadAttention(
-            num_heads=self.num_attention_heads,
-            key_dim=self.embedding_dim,
-            dropout=self.attention_dropout
-        )
-        self.skip_1 = layers.Add()
-        self.layer_norm_1 = layers.LayerNormalization(epsilon=self.norm_epsilon)
-        self.feed_forward = FeedForward(self.embedding_dim,
-                                        multiplier=self.feedforward_multiplier,
-                                        dropout=self.feedforward_dropout)
-        self.skip_2 = layers.Add()
-        self.layer_norm_2 = layers.LayerNormalization(epsilon=self.norm_epsilon)
-
-    def call(self, inputs):
-        attention_out = self.multi_head_attention(inputs, inputs)
-        x = self.skip_1([attention_out, inputs])
-        x = self.layer_norm_1(x)
-        feedforward_out = self.feed_forward(x)
-        x = self.skip_2([feedforward_out, x])
-        x = self.layer_norm_2(x)
-        return x
-
     def get_config(self):
-        config = super().get_config()
-        new_config = {'embedding_dim': self.embedding_dim,
-                      'num_attention_heads': self.num_attention_heads,
-                      'attention_dropout': self.attention_dropout,
-                      'feedforward_dropout': self.feedforward_dropout,
-                      'feedforward_multiplier': self.feedforward_multiplier,
-                      'norm_epsilon': self.norm_epsilon}
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'embedding_dim': self.embedding_dim,
+                  'num_attention_heads': self.num_attention_heads,
+                  'attention_dropout': self.attention_dropout,
+                  'feedforward_dropout': self.feedforward_dropout,
+                  'feedforward_multiplier': self.feedforward_multiplier,
+                  'norm_epsilon': self.norm_epsilon}
         return config
 
 
-class Encoder(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers.common")
+class Encoder(_EncoderLF):
     """
     Encoder for transformer based architectures.
     It is simply a stack of `num_transformer_layers`
     that is applied to the inputs.
 
     Args:
-        num_transformer_layer: `int`, default 6, Number of transformer layers
-            to use in the Encoder.
-        num_heads: `int`, default 8, Number of heads to use in the
-            MultiHeadAttention layer that is used to construct the Transformer layer.
-        embedding_dim: `int`, default 32, Embedding dimensions in the
-            MultiHeadAttention layer.
-        attention_dropout: `float`, default 0., Dropout rate to use in the
-            MultiHeadAttention layer.
-        feedforward_dropout: `float`, default 0., Dropout rate to use for
-            the dropout layer in the FeedForward layer.
-        norm_epsilon: `float`, default 1e-6, Value for epsilon parameter
-            of the `LayerNormalization` layer that is used to construct the
-            `Transformer` layer.
+        num_transformer_layer: ``int``, default 6,
+            Number of transformer layers to use in the Encoder.
+
+        num_attention_heads: ``int``, default 8,
+            Number of heads to use in the ``MultiHeadAttention`` layer
+            that is used to construct the ``Transformer`` layer.
+
+        embedding_dim: ``int``, default 32,
+            Embedding dimensions being used in the overall architecture.
+            These serve as the `key dimensions` in the
+            ``MultiHeadAttention`` layer and are multiplied by the
+            ``mutliplier`` in the ``FeedForward`` layer to compute the
+            hidden dimensions to project the inputs into.
+
+        attention_dropout: ``float``, default 0.,
+            Dropout rate for the ``MultiHeadAttention`` layer.
+
+        feedforward_dropout: ``float``, default 0.,
+            Dropout rate to use in for the dropout layer in the ``FeedForward`` layer.
+
+        norm_epsilon: ``float``, default 1e-6,
+            Normalization value to use for ``LayerNormalization`` layer.
     """
     def __init__(self,
                  num_transformer_layers: int = 6,
-                 num_heads: int = 8,
+                 num_attention_heads: int = 8,
                  embedding_dim: int = 32,
                  attention_dropout: float = 0.,
                  feedforward_dropout: float = 0.,
                  feedforward_multiplier: int = 4,
                  norm_epsilon: float = 1e-6,
                  **kwargs):
-        super().__init__(**kwargs)
+        transformer_layers = keras.models.Sequential(name="transformer_layers")
+        for i in range(num_transformer_layers):
+            transformer_layers.add(
+                Transformer(num_attention_heads=num_attention_heads,
+                            embedding_dim=embedding_dim,
+                            attention_dropout=attention_dropout,
+                            feedforward_dropout=feedforward_dropout,
+                            feedforward_multiplier=feedforward_multiplier,
+                            norm_epsilon=norm_epsilon,
+                            name=f"transformer_layer_{i+1}"))
+        super().__init__(transformer_layers,
+                         **kwargs)
         self.num_transformer_layers = num_transformer_layers
-        self.num_heads = num_heads
+        self.num_attention_heads = num_attention_heads
         self.embedding_dim = embedding_dim
         self.attention_dropout = attention_dropout
         self.feedforward_dropout = feedforward_dropout
         self.feedforward_multiplier = feedforward_multiplier
         self.norm_epsilon = norm_epsilon
 
-        self.transformer_layers = models.Sequential(name="transformer_layers")
-        for i in range(self.num_transformer_layers):
-            self.transformer_layers.add(
-                Transformer(num_attention_heads=self.num_heads,
-                            embedding_dim=self.embedding_dim,
-                            attention_dropout=self.attention_dropout,
-                            feedforward_dropout=self.feedforward_dropout,
-                            feedforward_multiplier=self.feedforward_multiplier,
-                            norm_epsilon=self.norm_epsilon,
-                            name=f"transformer_layer_{i+1}"))
-
-    def call(self, inputs):
-        outputs = self.transformer_layers(inputs)
-        return outputs
-
     def get_config(self):
-        config = super().get_config()
-        new_config = {'num_transformer_layers': self.num_transformer_layers,
-                      'num_heads': self.num_heads,
-                      'embedding_dim': self.embedding_dim,
-                      'attention_dropout': self.attention_dropout,
-                      'feedforward_dropout': self.feedforward_dropout,
-                      'feedforward_multiplier': self.feedforward_multiplier,
-                      'norm_epsilon': self.norm_epsilon}
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'num_transformer_layers': self.num_transformer_layers,
+                  'num_attention_heads': self.num_attention_heads,
+                  'embedding_dim': self.embedding_dim,
+                  'attention_dropout': self.attention_dropout,
+                  'feedforward_dropout': self.feedforward_dropout,
+                  'feedforward_multiplier': self.feedforward_multiplier,
+                  'norm_epsilon': self.norm_epsilon}
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        # we need to override the from_config method because the parent
+        # is layerflow version of Encoder which tried to extract
+        # the value against `transformer_layers` key to deserialize
+        # which causes KeyError
+        return cls(**config)
```

### Comparing `Teras-0.1.1/teras/layers/common/transformer_test.py` & `Teras-0.2.0/teras/layers/common/transformer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/layers/ctgan_test.py` & `Teras-0.2.0/teras/layers/ctgan/ctgan_discriminator_block_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import tensorflow as tf
-from teras.layers.ctgan import GeneratorBlock, DiscriminatorBlock
+from teras.layers.ctgan.ctgan_discriminator_block import CTGANDiscriminatorBlock
 
 
-def test_generator_block_output_shape():
-    gen_block = GeneratorBlock(units=32)
-    inputs = tf.ones((128, 16), dtype=tf.float32)
-    outputs = gen_block(inputs)
-    assert len(tf.shape(outputs)) == 2
-    assert tf.shape(outputs)[0] == 128
-    assert tf.shape(outputs)[1] == 32 + 16
+def test_ctgan_discriminator_block_valid_call():
+    disc_block = CTGANDiscriminatorBlock(units=32)
+    inputs = tf.ones((8, 5), dtype=tf.float32)
+    outputs = disc_block(inputs)
 
 
-def test_discriminator_block_output_shape():
-    gen_block = DiscriminatorBlock(units=32)
-    inputs = tf.ones((128, 16), dtype=tf.float32)
-    outputs = gen_block(inputs)
+def test_ctgan_discriminator_block_output_shape():
+    disc_block = CTGANDiscriminatorBlock(units=32)
+    inputs = tf.ones((8, 5), dtype=tf.float32)
+    outputs = disc_block(inputs)
     assert len(tf.shape(outputs)) == 2
-    assert tf.shape(outputs)[0] == 128
+    assert tf.shape(outputs)[0] == 8
     assert tf.shape(outputs)[1] == 32
```

### Comparing `Teras-0.1.1/teras/layers/dnfnet.py` & `Teras-0.2.0/teras/models/node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,374 +1,394 @@
-import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import initializers
-from teras.utils.dnfnet import (compute_total_number_of_literals,
-                                compute_total_number_of_conjunctions,
-                                compute_num_literals_per_formula,
-                                create_conjunctions_indicator_matrix,
-                                create_formulas_indicator_matrix,
-                                dense_ndim_array_to_sparse_tensor,
-                                tf_matmul_sparse_dense,
-                                and_operator,
-                                or_operator,
-                                generate_random_mask,
-                                extension_matrix,
-                                binary_threshold)
-from teras.layers.common.head import (ClassificationHead as _BaseClassificationHead,
-                                      RegressionHead as _BaseRegressionHead)
-from typing import List, Union
-
-LIST_OF_INT = List[int]
-LIST_OF_FLOAT = List[float]
-LIST_OR_TUPLE = Union[list, tuple]
-LAYER_OR_STR = Union[keras.layers.Layer, str]
+from teras.layers.node import ObliviousDecisionTree
+from teras.utils.node import sparsemoid
+from teras.activations import sparsemax
+from teras.layers.node.node_feature_selector import NodeFeatureSelector
+from teras.layerflow.models.node import NODE as _NodeLF
+from teras.layers.common.head import ClassificationHead, RegressionHead
+from teras.utils.types import UnitsValuesType
 
 
-class FeatureSelection(keras.layers.Layer):
+@keras.saving.register_keras_serializable("teras.models")
+class NODE(_NodeLF):
     """
-    Feature Selection layer based on the Feature Selection component proposed by Liran Katzir et al.
-    in the paper Net-DNF: Effective Deep Modeling of Tabular Data.
+    Neural Oblivious Decision Tree (NODE) model
+    based on the NODE architecture proposed by Sergei Popov et al.
+    in paper Neural Oblivious Decision Ensembles for Deep Learning on Tabular Data
 
     Reference(s):
-        https://openreview.net/forum?id=73WTGs96kho
+        https://arxiv.org/abs/1909.06312
 
     Args:
-        num_formulas: `int`, default 256,
-            Number of DNF formulas to use.
-            Each DNF formula is analogous to a tree in tree based ensembles.
-        keep_feature_prob_arr: `List[float]`, default [0.1, 0.3, 0.5, 0.7, 0.9],
-            Feature probability array.
-            It is used  to randomly select a probability value that is used
-            in the random selection of input features.
-        elastic_net_beta: `float`, default 0.4,
-            Used in the computation of Elastic Net Regularization.
-        binary_threshold_eps:   `float`, default 1.0,
-            Used in the computation of learnable mask.
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        num_layers: ``int``, default 8,
+            Number of ObliviousDecisionTree layers to use in model
+
+        num_trees: ``int``, default 128,
+            Number of trees to use in each `ObliviousDecisionTree` layer
+
+        depth: ``int``, default 6,
+            Number of splits in every tree
+
+        tree_dim: ``int``, default 1,
+            Number of response channels in the response of individual tree
+
+        max_features: ``int``,
+            Maximum number of features to use. If None, all features in the input dataset will be used.
+
+        input_dropout: ``float``, default 0.,
+            Dropout rate to apply to inputs.
+
+        choice_function:
+            Function that computes feature weights s.t. f(tensor, dim).sum(dim) == 1
+            By default, ``sparsemax`` is used.
+
+        bin_function:
+            Function that computes tree leaf weights.
+            By default, ``sparsemoid`` is used.
+
+        response_initializer: default "random_normal",
+            Initializer for tree output tensor. Any format that is acceptable by the keras initializers.
+
+        selection_logits_initializer: default "random_uniform",
+            Initializer for logits that select features for the tree
+            Both thresholds and scales are initialized with data-aware initialization function.
+
+        threshold_init_beta: ``float``, default 1.0,
+            Initializes threshold to a q-th quantile of data points
+            where q ~ Beta(:threshold_init_beta:, :threshold_init_beta:)
+            If this param is set to 1, initial thresholds will have the same distribution as data points
+            If greater than 1 (e.g. 10), thresholds will be closer to median data value
+            If less than 1 (e.g. 0.1), thresholds will approach min/max data values.
+
+        threshold_init_cutoff: ``float``, default 1.0,
+            Threshold log-temperatures initializer.
+            By default(1.0), log-temperatures are initialized in such a way that all bin selectors
+            end up in the linear region of sparse-sigmoid. The temperatures are then scaled by this parameter.
+            Setting this value > 1.0 will result in some margin between data points and sparse-sigmoid cutoff value
+            Setting this value < 1.0 will cause (1 - value) part of data points to end up in flat sparse-sigmoid region
+            For instance, threshold_init_cutoff = 0.9 will set 10% points equal to 0.0 or 1.0
+            Setting this value > 1.0 will result in a margin between data points and sparse-sigmoid cutoff value
+            All points will be between (0.5 - 0.5 / threshold_init_cutoff) and (0.5 + 0.5 / threshold_init_cutoff)
     """
     def __init__(self,
                  input_dim: int,
-                 num_formulas: int = 256,
-                 keep_feature_prob_arr: LIST_OF_FLOAT = [0.1, 0.3, 0.5, 0.7, 0.9],
-                 elastic_net_beta: float = 0.4,
-                 binary_threshold_eps: float = 1.0,
-                 **kwagrs):
-        super().__init__(**kwagrs)
+                 num_layers: int = 8,
+                 num_trees: int = 16,
+                 depth: int = 6,
+                 tree_dim: int = 1,
+                 max_features: int = None,
+                 input_dropout: float = 0.,
+                 choice_function=None,
+                 bin_function=None,
+                 response_initializer="random_normal",
+                 selection_logits_initializer="random_uniform",
+                 threshold_init_beta: float = 1.0,
+                 threshold_init_cutoff: float = 1.0,
+                 **kwargs):
+        choice_func = sparsemax if choice_function is None else choice_function
+        bin_func = sparsemoid if bin_function is None else bin_function
+
+        tree_layers = [ObliviousDecisionTree(num_trees=num_trees,
+                                             depth=depth,
+                                             tree_dim=tree_dim,
+                                             choice_function=choice_func,
+                                             bin_function=bin_func,
+                                             response_initializer=response_initializer,
+                                             selection_logits_initializer=selection_logits_initializer,
+                                             threshold_init_beta=threshold_init_beta,
+                                             threshold_init_cutoff=threshold_init_cutoff)
+                       for _ in range(num_layers)]
+        feature_selector = NodeFeatureSelector(data_dim=input_dim,
+                                               max_features=max_features,
+                                               name="feature_selector")
+        dropout = keras.layers.Dropout(input_dropout,
+                                       name="input_dropout")
+        super().__init__(input_dim=input_dim,
+                         tree_layers=tree_layers,
+                         feature_selector=feature_selector,
+                         dropout=dropout,
+                         **kwargs)
+
         self.input_dim = input_dim
-        self.num_formulas = num_formulas
-        self.keep_feature_prob_arr = keep_feature_prob_arr
-        self.elastic_net_beta = elastic_net_beta
-        self.binary_threshold_eps = binary_threshold_eps
-        self.v_temp = tf.Variable(tf.zeros(self.num_formulas), trainable=False)
-
-    def build(self, input_shape):
-        self.elastic_net_alpha = tf.Variable(initial_value=tf.constant(0.),
-                                             name='elastic_net_alpha')
-        self.learnable_mask = tf.Variable(initial_value=tf.fill(dims=(self.input_dim, self.num_formulas),
-                                                                value=self.binary_threshold_eps + 0.5),
-                                          shape=(self.input_dim, self.num_formulas),
-                                          name='learnable_mask')
-    def call(self,
-             num_literals_per_formula_arr=None,
-             ):
-        literals_random_mask, formulas_random_mask = generate_random_mask(self.input_dim,
-                                                                          self.keep_feature_prob_arr,
-                                                                          num_literals_per_formula_arr,
-                                                                          self.num_formulas)
-        num_effective_features = tf.reduce_sum(formulas_random_mask, axis=0)
-        formulas_random_mask = tf.reshape(formulas_random_mask, shape=tf.shape(self.learnable_mask))
-        ext_matrix = extension_matrix(self.v_temp,
-                                      self.num_formulas,
-                                      num_literals_per_formula_arr)
-        learnable_mask_01 = binary_threshold(self.learnable_mask, eps=self.binary_threshold_eps)
-
-        l2_square_norm_selected = tf.linalg.diag_part(tf.matmul(tf.transpose(tf.square(self.learnable_mask)),
-                                                                formulas_random_mask))
-        l1_norm_selected = tf.linalg.diag_part(tf.matmul(tf.transpose(tf.abs(self.learnable_mask)),
-                                                         formulas_random_mask))
-
-        l2 = tf.abs(
-            tf.divide(l2_square_norm_selected, num_effective_features) - self.elastic_net_beta * self.binary_threshold_eps ** 2)
-        l1 = tf.abs(tf.divide(l1_norm_selected, num_effective_features) - self.elastic_net_beta * self.binary_threshold_eps)
-        elastic_net_reg = tf.reduce_mean(
-            (l2 * ((1 - tf.nn.sigmoid(self.elastic_net_alpha)) / 2) + l1 * tf.nn.sigmoid(self.elastic_net_alpha)))
-        learnable_binary_mask = tf_matmul_sparse_dense(ext_matrix, learnable_mask_01)
-        return learnable_binary_mask, literals_random_mask, elastic_net_reg
+        self.num_layers = num_layers
+        self.num_trees = num_trees
+        self.depth = depth
+        self.tree_dim = tree_dim
+        self.max_features = max_features
+        self.input_dropout = input_dropout
+        self.choice_function = choice_function
+        self.bin_function = bin_function
+        self.choice_function = choice_function
+        self.response_initializer = response_initializer
+        self.selection_logits_initializer = selection_logits_initializer
+        self.threshold_init_beta = threshold_init_beta
+        self.threshold_init_cutoff = threshold_init_cutoff
 
     def get_config(self):
-        config = super().get_config()
-        new_config = {'input_dim': self.input_dim,
-                      'num_formulas': self.num_formulas,
-                      'keep_feature_prob_arr': self.keep_feature_prob_arr,
-                      'elastic_net_beta': self.elastic_net_beta,
-                      'binary_threshold_eps': self.binary_threshold_eps,
-                      'v_temp': self.v_temp}
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'input_dim': self.input_dim,
+                  'num_layers': self.num_layers,
+                  'num_trees': self.num_trees,
+                  'depth': self.depth,
+                  'tree_dim': self.tree_dim,
+                  'max_features': self.max_features,
+                  'input_dropout': self.input_dropout,
+                  'choice_function': self.choice_function,
+                  'bin_function': self.bin_function,
+                  'response_initializer': self.response_initializer,
+                  'selection_logits_initializer': self.selection_logits_initializer,
+                  'threshold_init_beta': self.threshold_init_beta,
+                  'threshold_init_cutoff': self.threshold_init_cutoff,
+                  }
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        return cls(input_dim=input_dim, **config)
 
-class Localization(keras.layers.Layer):
+
+@keras.saving.register_keras_serializable("teras.models")
+class NODERegressor(NODE):
     """
-    Localization layer based on the localization component proposed by Liran Katzir et al.
-    in the paper Net-DNF: Effective Deep Modeling of Tabular Data.
+    Neural Oblivious Decision Tree (NODE) Regressor model
+    based on the NODE architecture proposed by Sergei Popov et al.
+    in paper Neural Oblivious Decision Ensembles for Deep Learning on Tabular Data
 
     Reference(s):
-        https://openreview.net/forum?id=73WTGs96kho
+        https://arxiv.org/abs/1909.06312
 
     Args:
-        num_formulas: `int`, default 256,
-            Number of DNF formulas to use.
-            Each DNF formula is analogous to a tree in tree based ensembles.
-        temperature: `float`, default 2.0,
-            Temperature value to use.
-            According to the paper, The inclusion of an adaptive temperature in this localization mechanism
-            facilitates a data-dependent degree of exclusivity:
-            at high temperatures, only a few DNNFs will handle an input instance whereas
-            at low temperatures, more DNNFs will effectively participate in the ensemble.
+        num_outputs: `int`, default 1,
+            Number of regression outputs to predict.
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default None,
+            Units values to use in the hidden layers in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+            By default, no hidden layer is used.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        num_layers: ``int``, default 8,
+            Number of ObliviousDecisionTree layers to use in model
+
+        num_trees: ``int``, default 128,
+            Number of trees to use in each `ObliviousDecisionTree` layer
+
+        depth: ``int``, default 6,
+            Number of splits in every tree
+
+        tree_dim: ``int``, default 1,
+            Number of response channels in the response of individual tree
+
+        max_features: ``int``,
+            Maximum number of features to use. If None, all features in the input dataset will be used.
+
+        input_dropout: ``float``, default 0.,
+            Dropout rate to apply to inputs.
+
+        choice_function:
+            Function that computes feature weights s.t. f(tensor, dim).sum(dim) == 1
+            By default, ``sparsemax`` is used.
+
+        bin_function:
+            Function that computes tree leaf weights.
+            By default, ``sparsemoid`` is used.
+
+        response_initializer: default "random_normal",
+            Initializer for tree output tensor. Any format that is acceptable by the keras initializers.
+
+        selection_logits_initializer: default "random_uniform",
+            Initializer for logits that select features for the tree
+            Both thresholds and scales are initialized with data-aware initialization function.
+
+        threshold_init_beta: ``float``, default 1.0,
+            Initializes threshold to a q-th quantile of data points
+            where q ~ Beta(:threshold_init_beta:, :threshold_init_beta:)
+            If this param is set to 1, initial thresholds will have the same distribution as data points
+            If greater than 1 (e.g. 10), thresholds will be closer to median data value
+            If less than 1 (e.g. 0.1), thresholds will approach min/max data values.
+
+        threshold_init_cutoff: ``float``, default 1.0,
+            Threshold log-temperatures initializer.
+            By default(1.0), log-temperatures are initialized in such a way that all bin selectors
+            end up in the linear region of sparse-sigmoid. The temperatures are then scaled by this parameter.
+            Setting this value > 1.0 will result in some margin between data points and sparse-sigmoid cutoff value
+            Setting this value < 1.0 will cause (1 - value) part of data points to end up in flat sparse-sigmoid region
+            For instance, threshold_init_cutoff = 0.9 will set 10% points equal to 0.0 or 1.0
+            Setting this value > 1.0 will result in a margin between data points and sparse-sigmoid cutoff value
+            All points will be between (0.5 - 0.5 / threshold_init_cutoff) and (0.5 + 0.5 / threshold_init_cutoff)
     """
     def __init__(self,
-                 num_formulas: int = 256,
-                 temperature: float = 2.0,
+                 num_outputs: int = 1,
+                 head_units_values: UnitsValuesType = None,
+                 input_dim: int = None,
+                 num_layers: int = 8,
+                 num_trees: int = 16,
+                 depth: int = 6,
+                 tree_dim: int = 1,
+                 max_features: int = None,
+                 input_dropout: float = 0.,
+                 choice_function=None,
+                 bin_function=None,
+                 response_initializer="random_normal",
+                 selection_logits_initializer="random_uniform",
+                 threshold_init_beta: float = 1.0,
+                 threshold_init_cutoff: float = 1.0,
                  **kwargs):
-        super().__init__(**kwargs)
-        self.num_formulas = num_formulas
-        self.temperature = temperature
-        self.softmax = layers.Softmax()
-
-    def build(self, input_shape):
-        input_dim = input_shape[1]
-        mu_initializer = initializers.random_normal()
-        self.mu = tf.Variable(initial_value=mu_initializer(shape=(self.num_formulas, input_dim)),
-                              shape=(self.num_formulas, input_dim),
-                              name='exp_mu')
-        sigma_initializer = initializers.random_normal()
-        self.sigma = tf.Variable(initial_value=sigma_initializer(shape=(1, self.num_formulas, input_dim)),
-                                 shape=(1, self.num_formulas, input_dim),
-                                 name="exp_sigma")
-        self.temperature = tf.Variable(name='temperature',
-                                       initial_value=tf.constant(value=self.temperature),
-                                       dtype=tf.float32)
-
-    def call(self, inputs):
-        diff = tf.expand_dims(inputs, axis=1) - tf.expand_dims(self.mu, axis=0)
-        loc = tf.exp(-1 * tf.norm(tf.multiply(diff, self.sigma), axis=-1))
-        loc = self.softmax(tf.sigmoid(self.temperature) * loc)
-        return loc
+        head = RegressionHead(num_outputs=num_outputs,
+                              units_values=head_units_values,
+                              normalization=None)
+        super().__init__(input_dim=input_dim,
+                         num_layers=num_layers,
+                         num_trees=num_trees,
+                         depth=depth,
+                         tree_dim=tree_dim,
+                         max_features=max_features,
+                         input_dropout=input_dropout,
+                         choice_function=choice_function,
+                         bin_function=bin_function,
+                         response_initializer=response_initializer,
+                         selection_logits_initializer=selection_logits_initializer,
+                         threshold_init_beta=threshold_init_beta,
+                         threshold_init_cutoff=threshold_init_cutoff,
+                         head=head,
+                         **kwargs)
+        self.num_outputs = num_outputs
+        self.head_units_values = head_units_values
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_formulas': self.num_formulas,
-                      'temperature': self.temperature}
+        new_config = {'num_outputs': self.num_outputs,
+                      'head_units_values': self.head_units_values,
+                      }
         config.update(new_config)
         return config
 
 
-class DNNF(keras.layers.Layer):
+@keras.saving.register_keras_serializable("teras.models")
+class NODEClassifier(NODE):
     """
-    Disjunctive Normal Neural Form (DNNF) layer
-    is the  main building block of DNF-Net architecture.
-    Based on the paper Net-DNF: Effective Deep Modeling of Tabular Data by Liran Katzir et al.
+    Neural Oblivious Decision Tree (NODE) Classifier model
+    based on the NODE architecture proposed by Sergei Popov et al.
+    in paper Neural Oblivious Decision Ensembles for Deep Learning on Tabular Data
 
     Reference(s):
-        https://openreview.net/forum?id=73WTGs96kho
-
-    Args:
-        num_formulas: `int`, default 256,
-            Number of DNF formulas. Each DNF formula is analogous to a tree in tree based ensembles.
-        num_conjunctions_arr: `List[int]`, default [6, 9, 12, 15],
-            Conjunctions array.
-            It is used in the computation of total number of literals as well as
-            computation of number of literals per DNF formula.
-        conjunctions_depth_arr: `List[int]`, default [2, 4, 6],
-            Conjunctions depth array.
-            It is used in the computation of total number of literals as well as
-            computation of number of literals per DNF formula.
-        keep_feature_prob_arr: `List[float]`, default [0.1, 0.3, 0.5, 0.7, 0.9],
-            Feature probability array.
-            It is used by the Feature Selection layer to randomly select a probability
-            value that is used in the random selection of input features.
-        elastic_net_beta: `float`, default 0.4,
-            Used in the computation of Elastic Net Regularization.
-        binary_threshold_eps:   `float`, default 1.0,
-            Used in the computation of learnable mask.
-        temperature: `float`, default 2.0,
-            Temperature value to use in the Localization layer.
-            According to the paper, The inclusion of an adaptive temperature in this localization mechanism
-            facilitates a data-dependent degree of exclusivity:
-            at high temperatures, only a few DNNFs will handle an input instance whereas
-            at low temperatures, more DNNFs will effectively participate in the ensemble.
-    """
-    def __init__(self,
-                 num_formulas: int = 256,
-                 num_conjunctions_arr: LIST_OF_INT = [6, 9, 12, 15],
-                 conjunctions_depth_arr: LIST_OF_INT = [2, 4, 6],
-                 keep_feature_prob_arr: LIST_OF_FLOAT = [0.1, 0.3, 0.5, 0.7, 0.9],
-                 elastic_net_beta: float = 0.4,
-                 binary_threshold_eps: float = 1.0,
-                 temperature: float = 2.0,
-                 **kwargs
-                 ):
-        super().__init__(**kwargs)
-        self.num_formulas = num_formulas
-        self.num_conjunctions_arr = num_conjunctions_arr
-        self.conjunctions_depth_arr = conjunctions_depth_arr
-        self.keep_feature_prob_arr = keep_feature_prob_arr
-        self.elastic_net_beta = elastic_net_beta
-        self.binary_threshold_eps = binary_threshold_eps
-        self.temperature = temperature
-
-        self.localization = Localization(num_formulas=self.num_formulas,
-                                         temperature=self.temperature)
-
-        self.loaded_input_masks = None
-
-    def build(self, input_shape):
-        input_dim = input_shape[1]
-        self.feature_selection = FeatureSelection(input_dim=input_dim,
-                                                  num_formulas=self.num_formulas,
-                                                  keep_feature_prob_arr=self.keep_feature_prob_arr,
-                                                  elastic_net_beta=self.elastic_net_beta,
-                                                  binary_threshold_eps=self.binary_threshold_eps)
-
-        self.total_number_of_literals = compute_total_number_of_literals(self.num_formulas,
-                                                                         self.num_conjunctions_arr,
-                                                                         self.conjunctions_depth_arr)
-        num_literals_per_formula_arr = compute_num_literals_per_formula(self.num_conjunctions_arr,
-                                                                        self.conjunctions_depth_arr)
-        total_number_of_conjunctions = compute_total_number_of_conjunctions(self.num_formulas,
-                                                                            self.num_conjunctions_arr)
-
-        self.learnable_binary_mask, self.literals_random_mask, self.elastic_net_reg = self.feature_selection(
-                                                                                            num_literals_per_formula_arr)
-
-        self.bias = tf.Variable(name='literals_bias',
-                                shape=tf.shape(self.literals_random_mask)[1],
-                                initial_value=tf.fill(dims=(tf.shape(self.literals_random_mask)[1],), value=0.))
-        self.weight = self.add_weight(name='literals_weights',
-                                      shape=tf.shape(self.literals_random_mask),
-                                      initializer=initializers.glorot_normal())
-        self.weight = tf.multiply(self.weight, self.literals_random_mask)
-
-        # 'b' is just a prop to hold intermediate values since we can't assign values to a tensor,
-        # so we define a variable here with trainable argument set to False.
-        # same is the case with 'c' below.
-        b = tf.Variable(tf.cast(tf.zeros(tf.shape(self.literals_random_mask)[1]),
-                                dtype=tf.bool),
-                                trainable=False)
-        conjunctions_indicator_matrix = create_conjunctions_indicator_matrix(b,
-                                                                             total_number_of_conjunctions,
-                                                                             self.conjunctions_depth_arr,
-                                                                             )
-        conjunctions_indicator_matrix = tf.cast(conjunctions_indicator_matrix, dtype=tf.float32)
-        self.conjunctions_indicator_sparse_matrix = dense_ndim_array_to_sparse_tensor(conjunctions_indicator_matrix)
-        self.and_bias = tf.reduce_sum(conjunctions_indicator_matrix,
-                                      axis=0)
-
-        c = tf.Variable(tf.cast(tf.zeros(total_number_of_conjunctions),
-                                dtype=tf.bool))
-        formulas_indicator_matrix = create_formulas_indicator_matrix(c,
-                                                                     self.num_formulas,
-                                                                     self.num_conjunctions_arr)
-        formulas_indicator_matrix = tf.cast(formulas_indicator_matrix, dtype=tf.float32)
-        self.formulas_indicator_sparse_matrix = dense_ndim_array_to_sparse_tensor(formulas_indicator_matrix)
-        self.or_bias = tf.reduce_sum(formulas_indicator_matrix,
-                                     axis=0)
-
-    def call(self, inputs):
-        x = inputs
-        # Creating affine literals
-        out_literals = tf.tanh(tf.add(tf.matmul(x, tf.multiply(self.weight, self.learnable_binary_mask)), self.bias))
-        
-        # Soft Conjunctions
-        out_conjunctions = and_operator(tf_matmul_sparse_dense(self.conjunctions_indicator_sparse_matrix, out_literals),
-                                        d=self.and_bias)
-        out_DNNFs = or_operator(tf_matmul_sparse_dense(self.formulas_indicator_sparse_matrix, out_conjunctions),
-                                d=self.or_bias)
-        out_DNNFs = tf.reshape(out_DNNFs, shape=(-1, self.num_formulas))
-        
-        # Localization
-        loc = self.localization(x)
-        out_DNNFs = tf.multiply(out_DNNFs, loc)
-        return out_DNNFs
-
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'num_formulas': self.num_formulas,
-                      'num_conjunctions_arr': self.num_conjunctions_arr,
-                      'conjunctions_depth_arr': self.conjunctions_depth_arr,
-                      'keep_feature_prob_arr': self.keep_feature_prob_arr,
-                      'elastic_net_beta': self.elastic_net_beta,
-                      'binary_threshold_eps': self.binary_threshold_eps,
-                      'temperature': self.temperature}
-        config.update(new_config)
-        return config
-
-
-class ClassificationHead(_BaseClassificationHead):
-    """
-    Classification head for DNFNet Classifier model.
+        https://arxiv.org/abs/1909.06312
 
     Args:
         num_classes: `int`, default 2,
             Number of classes to predict.
-        units_values: `List[int] | Tuple[int]`, default `None`,
-            If specified, for each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the ClassificationHead.
-        activation_hidden: default `None`,
-            Activation function to use in hidden dense layers.
-        activation_out: default `None`,
-            Activation function to use for the output layer.
-            If not specified, `sigmoid` is used for binary and `softmax` is used for
-            multiclass classification.
-        normalization: `Layer | str`, default `None`,
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default None,
+            Units values to use in the hidden layers in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+            By default, no hidden layer is used.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        num_layers: ``int``, default 8,
+            Number of ObliviousDecisionTree layers to use in model
+
+        num_trees: ``int``, default 128,
+            Number of trees to use in each `ObliviousDecisionTree` layer
+
+        depth: ``int``, default 6,
+            Number of splits in every tree
+
+        tree_dim: ``int``, default 1,
+            Number of response channels in the response of individual tree
+
+        max_features: ``int``,
+            Maximum number of features to use. If None, all features in the input dataset will be used.
+
+        input_dropout: ``float``, default 0.,
+            Dropout rate to apply to inputs.
+
+        choice_function:
+            Function that computes feature weights s.t. f(tensor, dim).sum(dim) == 1
+            By default, ``sparsemax`` is used.
+
+        bin_function:
+            Function that computes tree leaf weights.
+            By default, ``sparsemoid`` is used.
+
+        response_initializer: default "random_normal",
+            Initializer for tree output tensor. Any format that is acceptable by the keras initializers.
+
+        selection_logits_initializer: default "random_uniform",
+            Initializer for logits that select features for the tree
+            Both thresholds and scales are initialized with data-aware initialization function.
+
+        threshold_init_beta: ``float``, default 1.0,
+            Initializes threshold to a q-th quantile of data points
+            where q ~ Beta(:threshold_init_beta:, :threshold_init_beta:)
+            If this param is set to 1, initial thresholds will have the same distribution as data points
+            If greater than 1 (e.g. 10), thresholds will be closer to median data value
+            If less than 1 (e.g. 0.1), thresholds will approach min/max data values.
+
+        threshold_init_cutoff: ``float``, default 1.0,
+            Threshold log-temperatures initializer.
+            By default(1.0), log-temperatures are initialized in such a way that all bin selectors
+            end up in the linear region of sparse-sigmoid. The temperatures are then scaled by this parameter.
+            Setting this value > 1.0 will result in some margin between data points and sparse-sigmoid cutoff value
+            Setting this value < 1.0 will cause (1 - value) part of data points to end up in flat sparse-sigmoid region
+            For instance, threshold_init_cutoff = 0.9 will set 10% points equal to 0.0 or 1.0
+            Setting this value > 1.0 will result in a margin between data points and sparse-sigmoid cutoff value
+            All points will be between (0.5 - 0.5 / threshold_init_cutoff) and (0.5 + 0.5 / threshold_init_cutoff)
     """
     def __init__(self,
                  num_classes: int = 2,
-                 units_values: LIST_OR_TUPLE = None,
-                 activation_hidden=None,
-                 activation_out=None,
-                 normalization: LAYER_OR_STR = None,
+                 head_units_values: UnitsValuesType = None,
+                 input_dim: int = None,
+                 num_layers: int = 8,
+                 num_trees: int = 16,
+                 depth: int = 6,
+                 tree_dim: int = 1,
+                 max_features: int = None,
+                 input_dropout: float = 0.,
+                 choice_function=None,
+                 bin_function=None,
+                 response_initializer="random_normal",
+                 selection_logits_initializer="random_uniform",
+                 threshold_init_beta: float = 1.0,
+                 threshold_init_cutoff: float = 1.0,
                  **kwargs):
-        super().__init__(num_classes=num_classes,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         activation_out=activation_out,
-                         normalization=normalization,
+        head = ClassificationHead(num_classes=num_classes,
+                                  units_values=head_units_values,
+                                  normalization=None)
+        super().__init__(input_dim=input_dim,
+                         num_layers=num_layers,
+                         num_trees=num_trees,
+                         depth=depth,
+                         tree_dim=tree_dim,
+                         max_features=max_features,
+                         input_dropout=input_dropout,
+                         choice_function=choice_function,
+                         bin_function=bin_function,
+                         response_initializer=response_initializer,
+                         selection_logits_initializer=selection_logits_initializer,
+                         threshold_init_beta=threshold_init_beta,
+                         threshold_init_cutoff=threshold_init_cutoff,
+                         head=head,
                          **kwargs)
+        self.num_classes = num_classes
+        self.head_units_values = head_units_values
 
-
-
-class RegressionHead(_BaseRegressionHead):
-    """
-    Regression head for the DNFNet Regressor model.
-
-    Args:
-        num_outputs: `int`, default 1,
-            Number of regression outputs to predict.
-        units_values: `List[int] | Tuple[int]`, default `None`,
-            If specified, for each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the RegressionHead.
-        activation_hidden: default `None`,
-            Activation function to use in hidden dense layers.
-        normalization: `Layer | str`, default `None`,
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
-    """
-    def __init__(self,
-                 num_outputs: int = 1,
-                 units_values: LIST_OR_TUPLE = None,
-                 activation_hidden=None,
-                 normalization: LAYER_OR_STR = None,
-                 **kwargs):
-        super().__init__(num_outputs=num_outputs,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         normalization=normalization,
-                         **kwargs)
+    def get_config(self):
+        config = super().get_config()
+        new_config = {'num_classes': self.num_classes,
+                      'head_units_values': self.head_units_values,
+                      }
+        config.update(new_config)
+        return config
```

### Comparing `Teras-0.1.1/teras/layers/dnfnet_test.py` & `Teras-0.2.0/teras/layers/dnfnet/dnfnet_feature_selection_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 import tensorflow as tf
-from teras.layers.dnfnet import FeatureSelection, Localization, DNNF
+from teras.layers.dnfnet.dnfnet_feature_selection import DNFNetFeatureSelection
 from teras.utils.dnfnet import compute_num_literals_per_formula
 
 
-def test_feature_selection_output_shape():
-    feature_selection = FeatureSelection(input_dim=16,
-                                         num_formulas=32)
-    inputs = tf.ones((128, 16), dtype=tf.float32)
+def test_dnfnet_feature_selection_valid_call():
+    feature_selection = DNFNetFeatureSelection(input_dim=10,
+                                               num_formulas=16)
+    inputs = tf.ones((8, 10), dtype=tf.float32)
+    num_conjunctions_arr = [6, 9, 12, 15]
+    conjunctions_depth_arr = [2, 4, 6]
+    num_literals_per_formula_arr = compute_num_literals_per_formula(num_conjunctions_arr,
+                                                                    conjunctions_depth_arr)
+
+    learnable_binary_mask, literals_random_mask, elastic_net_reg = feature_selection(num_literals_per_formula_arr)
+
+
+def test_dnfnet_feature_selection_output_shape():
+    feature_selection = DNFNetFeatureSelection(input_dim=10,
+                                               num_formulas=16)
+    inputs = tf.ones((8, 10), dtype=tf.float32)
     num_conjunctions_arr = [6, 9, 12, 15]
     conjunctions_depth_arr = [2, 4, 6]
     num_literals_per_formula_arr = compute_num_literals_per_formula(num_conjunctions_arr,
                                                                     conjunctions_depth_arr)
 
     learnable_binary_mask, literals_random_mask, elastic_net_reg = feature_selection(num_literals_per_formula_arr)
-    print(tf.shape(learnable_binary_mask))
-    print(tf.shape(literals_random_mask))
-    print(tf.shape(elastic_net_reg))
     assert len(tf.shape(learnable_binary_mask)) == 2
-    assert tf.shape(learnable_binary_mask)[0] == 16
+    assert tf.shape(learnable_binary_mask)[0] == 10
     assert tf.shape(learnable_binary_mask)[1] == 0
     assert len(tf.shape(literals_random_mask)) == 2
-    assert tf.shape(literals_random_mask)[0] == 16
+    assert tf.shape(literals_random_mask)[0] == 10
     assert tf.shape(literals_random_mask)[1] == 0
     assert len(tf.shape(elastic_net_reg)) == 0
-
-
-def test_localitzation_output_shape():
-    localization = Localization(num_formulas=32)
-    inputs = tf.ones((128, 16), dtype=tf.float32)
-    outputs = localization(inputs)
-    assert len(tf.shape(outputs)) == 2
-    assert tf.shape(outputs)[0] == 128
-    assert tf.shape(outputs)[1] == 32
-
-
-def test_dnnf_output_shape():
-    dnnf = DNNF(num_formulas=32)
-    inputs = tf.ones((128, 16), dtype=tf.float32)
-    outputs = dnnf(inputs)
-    assert len(tf.shape(outputs)) == 2
-    assert tf.shape(outputs)[0] == 128
-    assert tf.shape(outputs)[1] == 32
```

### Comparing `Teras-0.1.1/teras/layers/embedding.py` & `Teras-0.2.0/teras/layers/categorical_feature_embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,123 +1,126 @@
-import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from typing import List
-
-
-LIST_OF_STR = List[str]
+import numpy as np
+import tensorflow as tf
+from teras.utils.types import Number
 
 
-class CategoricalFeatureEmbedding(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers")
+class CategoricalFeatureEmbedding(keras.layers.Layer):
     """
     CategoricalFeatureEmbedding layer that encodes categorical features into
     categorical feature embeddings.
 
     Args:
-        categorical_features_metadata: `dict`, A dictionary of metadata of categorical features.
-            It is simply a mapping where for each categorical feature, the feature name maps
-            to a tuple of feature index and a list of unique values (a.k.a. Vocabulary) in the feature.
+        features_metadata: ``dict``,
+            a nested dictionary of metadata for features where
+            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
+            feature indices and the lists of unique values (vocabulary) in them,
+            while numerical dictionary is a mapping of numerical feature names to their indices.
+            `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
+            `{feature_name: feature_idx}` for feature in numerical features.
             You can get this metadata dictionary by calling
                 >>> from teras.utils import get_features_metadata_for_embedding
                 >>> features_metadata = get_features_metadata_for_embedding(dataset,
-                                                                            categorical_features,
-                                                                            numerical_features)
-            and then accessing its `categorical` key as follows:
-                >>> categorical_features_metadata = features_metadata["categorical"]
-        embedding_dim: `int`, default 32, Dimensionality of the embeddings
-            to which categorical features should be mapped.
-        encode: `bool`, default True, whether to (label) encode categorical values,
+                ..                                                          categorical_features,
+                ..                                                          numerical_features)
+        embedding_dim: ``int``, default 32,
+            Dimensionality of the embeddings to which categorical features should be mapped.
+
+        encode: ``bool``, default True,
+            Whether to (label) encode categorical values,
             If you've already encoded the categorical values using for instance
             Label/Ordinal encoding, you should set this to False,
             otherwise leave it as True.
             In the case of True, categorical values will be mapped to integer indices
-            using keras's string lookup layer.
+            using keras's ``IntegrerLookup`` layer.
     """
     def __init__(self,
-                 categorical_features_metadata: dict,
+                 features_metadata: dict,
                  embedding_dim: int = 32,
                  encode: bool = True,
                  **kwargs):
         super().__init__(**kwargs)
-        self.categorical_features_metadata = categorical_features_metadata
+        if not len(features_metadata["categorical"]) > 0:
+            raise ValueError("`features_metadata` does not contain any categorical features. "
+                             "Either you forgot to pass categorical features names list to the "
+                             "`get_features_metadata_for_embedding` or the dataset does not contain "
+                             "any categorical features to begin with. \n"
+                             "In either case, "
+                             "`CategoricalFeatureEmbedding` cannot be called on inputs with no categorical features. ")
+
+        self.features_metadata = features_metadata
         self.embedding_dim = embedding_dim
         self.encode = encode
 
+        self.categorical_features_metadata = features_metadata["categorical"]
         self.lookup_tables, self.embedding_layers = self._get_lookup_tables_and_embedding_layers()
-        self.concat = layers.Concatenate(axis=1)
-        self._is_data_in_dict_format = False
-        self._is_first_batch = True
-        self._num_categorical_features = len(categorical_features_metadata)
+        self._num_categorical_features = len(self.categorical_features_metadata)
 
     def _get_lookup_tables_and_embedding_layers(self):
         """Lookup tables and embedding layers for each categorical feature"""
         lookup_tables = []
         embedding_layers = []
         for feature_name, (feature_idx, vocabulary) in self.categorical_features_metadata.items():
             # If the categorical values in the dataset haven't been encoded in preprocessing step
             # then encode them first. The `encode` parameter lets user specify if we need to encode
             # the categorical values or not.
             if self.encode:
-                # Lookup Table to convert string values to integer indices
-                lookup = layers.StringLookup(vocabulary=vocabulary,
-                                             mask_token=None,
-                                             num_oov_indices=0,
-                                             output_mode="int"
-                                             )
+                if isinstance(vocabulary[0], Number):
+                    # Lookup Table to map integer values to integer indices
+                    lookup = keras.layers.IntegerLookup(vocabulary=vocabulary,
+                                                        mask_token=None,
+                                                        output_mode="int",
+                                                        )
+                else:
+                    raise TypeError("`CategoricalFeatureEmbedding` layer can only encode values of type int "
+                                    f"but received type: {type(vocabulary[0])} for feature {feature_name}.")
                 lookup_tables.append(lookup)
 
             # Embedding layers map the integer representations of categorical values
             # to dense vectors of `embedding_dim` dimensionality,
             # which in fancier lingo are called `embeddings`.
-            embedding = layers.Embedding(input_dim=len(vocabulary),
-                                         output_dim=self.embedding_dim)
+            embedding = keras.layers.Embedding(input_dim=len(vocabulary) + 1,
+                                               output_dim=self.embedding_dim)
             embedding_layers.append(embedding)
 
         return lookup_tables, embedding_layers
 
     def call(self, inputs):
-        # Find the dataset's format - is it either in dictionary format.
-        # If inputs is an instance of dict, it's in dictionary format
-        # If inputs is an instance of tuple, it's in array format
-        if self._is_first_batch:
-            if isinstance(inputs, dict):
-                self._is_data_in_dict_format = True
-            self._is_first_batch = False
-
         # Encode and embedd categorical features
         categorical_feature_embeddings = tf.TensorArray(size=self._num_categorical_features,
                                                         dtype=tf.float32)
         # feature_idx is the overall index of feature in the dataset
         # so it can't be used to retrieve lookup table and embedding layer from list
         # which are both of length equal to number of categorical features - not input dimensions
         # hence the need for current_idx
         current_idx = 0
         # We only embedd the categorical features
         for feature_name, (feature_idx, _) in self.categorical_features_metadata.items():
-            if self._is_data_in_dict_format:
-                feature = tf.expand_dims(inputs[feature_name], 1)
-            else:
-                feature = tf.expand_dims(inputs[:, feature_idx], 1)
+            feature = tf.expand_dims(inputs[:, feature_idx], 1)
             if self.encode:
                 # Convert string input values to integer indices
                 lookup = self.lookup_tables[current_idx]
                 feature = lookup(feature)
             # Convert index values to embedding representations
             embedding = self.embedding_layers[current_idx]
             feature = embedding(feature)
             categorical_feature_embeddings = categorical_feature_embeddings.write(current_idx, feature)
             current_idx += 1
         categorical_feature_embeddings = categorical_feature_embeddings.stack()
         categorical_feature_embeddings = tf.squeeze(categorical_feature_embeddings, axis=2)
-        if tf.rank(categorical_feature_embeddings) == 3:
-            categorical_feature_embeddings = tf.transpose(categorical_feature_embeddings, perm=[1, 0, 2])
-        else:
-            categorical_feature_embeddings = tf.transpose(categorical_feature_embeddings)
+        categorical_feature_embeddings = tf.transpose(categorical_feature_embeddings, perm=[1, 0, 2])
+        categorical_feature_embeddings.set_shape((None, self._num_categorical_features, self.embedding_dim))
         return categorical_feature_embeddings
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'categorical_features_metadata': self.categorical_features_metadata,
+        new_config = {'features_metadata': self.features_metadata,
                       'embedding_dim': self.embedding_dim,
                       'encode': self.encode}
         config.update(new_config)
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        features_metadata = config.pop("features_metadata")
+        return cls(features_metadata, **config)
```

### Comparing `Teras-0.1.1/teras/layers/encoding_test.py` & `Teras-0.2.0/teras/layers/preprocessing/label_encoding_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 import tensorflow as tf
-from teras.layers.encoding import LabelEncoding
+from teras.layers.preprocessing.label_encoding import LabelEncoding
 from teras.utils import get_features_metadata_for_embedding
 import pandas as pd
+import numpy as np
 import pytest
 
 
 @pytest.fixture
 def setup_data():
-    data = {'color': ['green', 'yellow', 'green', 'orange', 'red', 'orange', 'orange', 'green'],
-            'shape': ['square', 'square', 'circle', 'rectangle', 'circle', 'rectangle', 'rectangle', 'square'],
-            'area': [8., 10., 11., 7., 5., 1., 7., 9.]}
-    metadata = get_features_metadata_for_embedding(pd.DataFrame(data),
-                                                   categorical_features=['color', 'shape'],
-                                                   numerical_features=['area'])
-    return data, metadata
+    df = pd.DataFrame({'player_level': [70, 90, 80, 90, 100, 90, 70, 80],
+                       'income': [1000, 1270, 900, 1000, 1234, 5678, 9999, 0],
+                       'shirt_number': [10, 7, 7, 10, 10, 10, 7, 10],
+                       })
+    metadata = get_features_metadata_for_embedding(df,
+                                                   categorical_features=["player_level", "shirt_number"],
+                                                   numerical_features=["income"])
+    return df.values, metadata
 
 
 def test_label_encoding_output_shape_when_concatenate_numerical_features_is_false(setup_data):
     data, metadata = setup_data
-    label_encoding = LabelEncoding(categorical_features_metadata=metadata["categorical"],
+    label_encoding = LabelEncoding(features_metadata=metadata,
                                    concatenate_numerical_features=False)
     outputs = label_encoding(data)
     assert len(tf.shape(outputs)) == 2
     assert tf.shape(outputs)[0] == 8
     assert tf.shape(outputs)[1] == 2    # number of categorical features = 2
 
 
 def test_label_encoding_output_shape_when_concatenate_numerical_features_is_true(setup_data):
     data, metadata = setup_data
-    label_encoding = LabelEncoding(categorical_features_metadata=metadata["categorical"],
+    label_encoding = LabelEncoding(features_metadata=metadata,
                                    concatenate_numerical_features=True)
     outputs = label_encoding(data)
     assert len(tf.shape(outputs)) == 2
     assert tf.shape(outputs)[0] == 8
     assert tf.shape(outputs)[1] == 3    # total number of features = 3
 
+
+def test_label_encoding_keeps_features_order(setup_data):
+    data, metadata = setup_data
+    label_encoding = LabelEncoding(features_metadata=metadata,
+                                   concatenate_numerical_features=True,
+                                   keep_features_order=True)
+    outputs = label_encoding(data)
+    assert len(tf.shape(outputs)) == 2
+    assert tf.shape(outputs)[0] == 8
+    assert tf.shape(outputs)[1] == 3    # total number of features = 3
+    assert all(data[:, 1] == outputs[:, 1])
```

### Comparing `Teras-0.1.1/teras/layers/gain.py` & `Teras-0.2.0/teras/layers/gain/gain_discriminator_block.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,49 @@
-from tensorflow.keras import layers
+from tensorflow import keras
 
 
-class GeneratorBlock(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers.gain")
+class GAINDiscriminatorBlock(keras.layers.Layer):
     """
-    GeneratorBlock that is used in construction of hidden block
-    inside the Generator model of GAIN architecture.
+    GAINDiscriminatorBlock that is used in construction of hidden block
+    inside the ``GAINDiscriminator`` model of ``GAIN`` architecture.
 
     Args:
-        units: `int`,
-            Hidden dimensionality of the generator block
-        activation: default "relu",
-            Activation function to use in the generator block
-        kernel_initializer: default "glorot_normal",
-            Kernel initializer for the generator block
-    """
-    def __init__(self,
-                 units: int,
-                 activation="relu",
-                 kernel_initializer="glorot_normal",
-                 **kwargs):
-        super().__init__(**kwargs)
-        self.units = units
-        self.activation = activation
-        self.kernel_initializer = kernel_initializer
-        self.dense = layers.Dense(units,
-                                  activation=self.activation,
-                                  kernel_initializer=self.kernel_initializer)
-
-    def call(self, inputs):
-        return self.dense(inputs)
-
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'units': self.units,
-                      'activation': self.activation,
-                      'kernel_initializer': self.kernel_initializer,
-                      }
-
-        config.update(new_config)
-        return config
-
-
-class DiscriminatorBlock(layers.Layer):
-    """
-    DiscriminatorBlock that is used in construction of hidden block
-    inside the Discriminator model of GAIN architecture.
-
-    Args:
-        units: `int`,
+        units: ``int``,
             Hidden dimensionality of the discriminator block
+
         activation: default "relu",
             Activation function to use in the discriminator block
+
         kernel_initializer: default "glorot_normal",
             Kernel initializer for the discriminator block
     """
     def __init__(self,
                  units: int,
                  activation="relu",
                  kernel_initializer="glorot_normal",
                  **kwargs):
         super().__init__(**kwargs)
         self.units = units
         self.activation = activation
         self.kernel_initializer = kernel_initializer
-        self.dense = layers.Dense(units,
-                                  activation=self.activation,
-                                  kernel_initializer=self.kernel_initializer)
+        self.dense = keras.layers.Dense(units,
+                                        activation=self.activation,
+                                        kernel_initializer=self.kernel_initializer)
 
     def call(self, inputs):
         return self.dense(inputs)
 
     def get_config(self):
         config = super().get_config()
         new_config = {'units': self.units,
                       'activation': self.activation,
                       'kernel_initializer': self.kernel_initializer,
                       }
 
         config.update(new_config)
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        units = config.pop("units")
+        return cls(units, **config)
```

### Comparing `Teras-0.1.1/teras/layers/node.py` & `Teras-0.2.0/teras/layers/node/odst.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,93 @@
 from tensorflow import keras
 import tensorflow as tf
-from tensorflow.keras import layers
 from warnings import warn
 from teras.utils import sparsemoid
-import tensorflow_addons as tfa
+from teras.activations import sparsemax
 import tensorflow_probability as tfp
-from teras.layers.common.head import (ClassificationHead as _BaseClassificationHead,
-                                      RegressionHead as _BaseRegressionHead)
-from typing import List, Union
+from teras.utils import get_activation
 
-LIST_OR_TUPLE = Union[list, tuple]
-LAYER_OR_STR = Union[keras.layers.Layer, str]
 
-
-class ObliviousDecisionTree(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layers.node")
+class ObliviousDecisionTree(keras.layers.Layer):
     """
         Oblivious Decision Tree layer as proposed by Sergei Popov et al.
         in paper Neural Oblivious Decision Ensembles
         for Deep Learning on Tabular Data
 
         Reference(s):
             https://arxiv.org/abs/1909.06312
 
         Args:
-       num_trees: `int`, default 128,
+       num_trees: ``int``, default 128,
             Number of trees
-        depth: `int`, default 6,
-            Number of splits in every tree
-        tree_dim: `int`, default 1,
-            Number of response channels in the response of individual tree
-        max_features: `int`,
-            Maximum number of features to use. If None, all features in the input dataset will be used.
-        input_dropout: `float`, default 0.,
-            Dropout rate to apply to inputs.
-        choice_function:
-            f(tensor, dim) -> R_simplex computes feature weights s.t. f(tensor, dim).sum(dim) == 1
-            By default, sparsemax is used.
-        bin_function:
-            f(tensor) -> R[0, 1], computes tree leaf weights
-            By default, sparsemoid is used.
-        response_initializer: default "random_normal",
-            Initializer for tree output tensor. Any format that is acceptable by the keras initializers.
-        selection_logits_intializer: default "random_uniform",
-            Initializer for logits that select features for the tree
-            Both thresholds and scales are initialized with data-aware initialization function.
-        threshold_init_beta: `float`, default 1.0,
-            Initializes threshold to a q-th quantile of data points
-            where q ~ Beta(:threshold_init_beta:, :threshold_init_beta:)
-            If this param is set to 1, initial thresholds will have the same distribution as data points
-            If greater than 1 (e.g. 10), thresholds will be closer to median data value
-            If less than 1 (e.g. 0.1), thresholds will approach min/max data values.
-        threshold_init_cutoff: `float`, default 1.0,
-            Threshold log-temperatures initializer, \in (0, inf)
-            By default(1.0), log-remperatures are initialized in such a way that all bin selectors
-            end up in the linear region of sparse-sigmoid. The temperatures are then scaled by this parameter.
-            Setting this value > 1.0 will result in some margin between data points and sparse-sigmoid cutoff value
-            Setting this value < 1.0 will cause (1 - value) part of data points to end up in flat sparse-sigmoid region
-            For instance, threshold_init_cutoff = 0.9 will set 10% points equal to 0.0 or 1.0
-            Setting this value > 1.0 will result in a margin between data points and sparse-sigmoid cutoff value
-            All points will be between (0.5 - 0.5 / threshold_init_cutoff) and (0.5 + 0.5 / threshold_init_cutoff)
+
+       depth: ``int``, default 6,
+           Number of splits in every tree
+
+       tree_dim: ``int``, default 1,
+           Number of response channels in the response of individual tree
+
+       max_features: ``int``,
+           Maximum number of features to use. If None, all features in the input dataset will be used.
+
+       input_dropout: ``float``, default 0.,
+           Dropout rate to apply to inputs.
+
+       choice_function:
+           f(tensor, dim) -> R_simplex computes feature weights s.t. f(tensor, dim).sum(dim) == 1
+           By default, sparsemax is used.
+
+       bin_function:
+           f(tensor) -> R[0, 1], computes tree leaf weights
+           By default, `sparsemoid` is used.
+
+       response_initializer: default "random_normal",
+           Initializer for tree output tensor. Any format that is acceptable by the keras initializers.
+
+       selection_logits_initializer: default "random_uniform",
+           Initializer for logits that select features for the tree
+           Both thresholds and scales are initialized with data-aware initialization function.
+
+       threshold_init_beta: ``float``, default 1.0,
+           Initializes threshold to a q-th quantile of data points
+           where q ~ Beta(:threshold_init_beta:, :threshold_init_beta:)
+           If this param is set to 1, initial thresholds will have the same distribution as data points
+           If greater than 1 (e.g. 10), thresholds will be closer to median data value
+           If less than 1 (e.g. 0.1), thresholds will approach min/max data values.
+
+       threshold_init_cutoff: ``float``, default 1.0,
+           Threshold log-temperatures initializer, \in (0, inf)
+           By default(1.0), log-temperatures are initialized in such a way that all bin selectors
+           end up in the linear region of sparse-sigmoid. The temperatures are then scaled by this parameter.
+           Setting this value > 1.0 will result in some margin between data points and sparse-sigmoid cutoff value
+           Setting this value < 1.0 will cause (1 - value) part of data points to end up in flat sparse-sigmoid region
+           For instance, threshold_init_cutoff = 0.9 will set 10% points equal to 0.0 or 1.0
+           Setting this value > 1.0 will result in a margin between data points and sparse-sigmoid cutoff value
+           All points will be between (0.5 - 0.5 / threshold_init_cutoff) and (0.5 + 0.5 / threshold_init_cutoff)
     """
     def __init__(self,
                  num_trees: int = 128,
                  depth: int = 6,
                  tree_dim: int = 1,
                  choice_function=None,
                  bin_function=None,
                  response_initializer="random_normal",
-                 selection_logits_intializer="random_uniform",
+                 selection_logits_initializer="random_uniform",
                  threshold_init_beta: float = 1.0,
                  threshold_init_cutoff: float = 1.0,
                  **kwargs):
         super().__init__(**kwargs)
         self.num_trees = num_trees
         self.depth = depth
         self.tree_dim = tree_dim
-        self.choice_function = tfa.activations.sparsemax if choice_function is None else choice_function
-        self.bin_function = sparsemoid if bin_function is None else bin_function
+        self.choice_function = sparsemax if choice_function is None else get_activation(choice_function)
+        self.bin_function = sparsemoid if bin_function is None else get_activation(bin_function)
         self.response_initializer = response_initializer
-        self.selection_logits_initializer = selection_logits_intializer
+        self.selection_logits_initializer = selection_logits_initializer
         self.threshold_init_beta = threshold_init_beta
         self.threshold_init_cutoff = threshold_init_cutoff
         self.initialized = False
 
     def build(self, input_shape):
         input_dim = input_shape[-1]
         self.response = self.add_weight(initializer=self.response_initializer,
@@ -160,84 +165,14 @@
         config = super().get_config()
         new_config = {'num_trees': self.num_trees,
                       'depth': self.depth,
                       'tree_dim': self.tree_dim,
                       'choice_function': self.choice_function,
                       'bin_function': self.bin_function,
                       'response_initializer': self.response_initializer,
-                      'selection_logits_intializer': self.selection_logits_intializer,
+                      'selection_logits_initializer': self.selection_logits_initializer,
                       'threshold_init_beta': self.threshold_init_beta,
                       'threshold_init_cutoff': self.threshold_init_cutoff,
                       }
 
         config.update(new_config)
-        return config
-
-
-class ClassificationHead(_BaseClassificationHead):
-    """
-    Classification head for NODE Classifier model.
-
-    Args:
-        num_classes: `int`, default 2,
-            Number of classes to predict.
-        units_values: `List[int] | Tuple[int]`, default `None`,
-            If specified, for each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the ClassificationHead.
-        activation_hidden: default `None`,
-            Activation function to use in hidden dense layers.
-        activation_out: default `None`,
-            Activation function to use for the output layer.
-            If not specified, `sigmoid` is used for binary and `softmax` is used for
-            multiclass classification.
-        normalization: `Layer | str`, default `None`,
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
-    """
-    def __init__(self,
-                 num_classes: int = 2,
-                 units_values: LIST_OR_TUPLE = None,
-                 activation_hidden=None,
-                 activation_out=None,
-                 normalization: LAYER_OR_STR = None,
-                 **kwargs):
-        super().__init__(num_classes=num_classes,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         activation_out=activation_out,
-                         normalization=normalization,
-                         **kwargs)
-
-
-class RegressionHead(_BaseRegressionHead):
-    """
-    Regression head for the NODE Regressor model.
-
-    Args:
-        num_outputs: `int`, default 1,
-            Number of regression outputs to predict.
-        units_values: `List[int] | Tuple[int]`, default `None`,
-            If specified, for each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the RegressionHead.
-        activation_hidden: default `None`,
-            Activation function to use in hidden dense layers.
-        normalization: `Layer | str`, default `None`,
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
-    """
-    def __init__(self,
-                 num_outputs: int = 1,
-                 units_values: LIST_OR_TUPLE = None,
-                 activation_hidden=None,
-                 normalization: LAYER_OR_STR = None,
-                 **kwargs):
-        super().__init__(num_outputs=num_outputs,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         normalization=normalization,
-                         **kwargs)
+        return config
```

### Comparing `Teras-0.1.1/teras/layers/node_test.py` & `Teras-0.2.0/teras/layers/node/odst_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import tensorflow as tf
-from teras.layers.node import ObliviousDecisionTree
+from teras.layers.node.odst import ObliviousDecisionTree
+
+
+def test_node_oblivious_decision_tree_valid_call():
+    oblivious = ObliviousDecisionTree(num_trees=16,
+                                      depth=8,
+                                      tree_dim=4)
+    inputs = tf.ones((128, 16), dtype=tf.float32)
+    outputs = oblivious(inputs)
 
 
 def test_node_oblivious_decision_tree_output_shape():
     oblivious = ObliviousDecisionTree(num_trees=16,
                                       depth=8,
                                       tree_dim=4)
     inputs = tf.ones((128, 16), dtype=tf.float32)
     outputs = oblivious(inputs)
-    print("\n\nSHAPEEEEEEEEEE: ", tf.shape(outputs))
     assert len(tf.shape(outputs)) == 2
     assert tf.shape(outputs)[0] == 128
     assert tf.shape(outputs)[1] == 16 * 4   # num_tress * tree_dim
```

### Comparing `Teras-0.1.1/teras/layers/saint.py` & `Teras-0.2.0/teras/models/saint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,689 +1,636 @@
-import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import models
-from teras.layers.common.transformer import FeedForward, Transformer
-from teras.layers.common.head import (ClassificationHead as BaseClassificationHead,
-                                      RegressionHead as BaseRegressionHead)
-from typing import Union, List, Tuple
+from teras.layers.categorical_feature_embedding import CategoricalFeatureEmbedding
+from teras.layers.saint.saint_numerical_feature_embedding import SAINTNumericalFeatureEmbedding
+from teras.layers.saint.saint_encoder import SAINTEncoder
+from teras.layers.common.head import ClassificationHead, RegressionHead
+from teras.layerflow.models.saint import (SAINT as _SAINTLF,
+                                          SAINTPretrainer as _SAINTPretrainerLF)
+from teras.layers.saint.saint_reconstruction_head import SAINTReconstructionHead
+from teras.layers.saint.saint_projection_head import SAINTProjectionHead
+from teras.layers.regularization import MixUp, CutMix
+from teras.config.saint import SAINTConfig
+from teras.utils.types import UnitsValuesType
 
 
-LIST_OR_TUPLE = Union[List[int], Tuple[int]]
-LAYER_OR_STR = Union[keras.layers.Layer, str]
-
-
-class NumericalFeatureEmbedding(layers.Layer):
+@keras.saving.register_keras_serializable("teras.models")
+class SAINT(_SAINTLF):
     """
-    Numerical Feature Embedding layer based on the architecture proposed
-    by Gowthami Somepalli et al. in the paper
+    SAINT architecture proposed by Gowthami Somepalli et al.
+    in the paper,
     SAINT: Improved Neural Networks for Tabular Data
     via Row Attention and Contrastive Pre-Training.
 
+    SAINT performs attention over both rows and columns.
+
     Reference(s):
         https://arxiv.org/abs/2106.01342
 
     Args:
-        numerical_features_metadata: `dict`,
-            A dictionary where for each feature in numerical features
-            the feature name is mapped against its index in the dataset.
-        embedding_dim: `int`, default 32,
-            Embedding dimension is the dimensionality of the output layer or
-            the dimensionality of the embeddings produced.
-            (These embedding dimensions are the same used for the embedding categorical features)
-        hidden_dim: `int`, default 16,
-            Hidden dimension, used by the first dense layer i.e the hidden layer whose outputs
-            are later projected to the `emebedding_dim`
-    """
-    def __init__(self,
-                 numerical_features_metadata: dict,
-                 embedding_dim: int = 32,
-                 hidden_dim: int = 16
-                 ):
-        super().__init__()
-        self.numerical_features_metadata = numerical_features_metadata
-        self.hidden_dim = hidden_dim
-        self.embedding_dim = embedding_dim
-
-        self._num_numerical_features = len(self.numerical_features_metadata)
-        # Need to create as many embedding layers as there are numerical features
-        self.embedding_layers = []
-        for _ in range(self._num_numerical_features):
-            self.embedding_layers.append(
-                models.Sequential([
-                    layers.Dense(units=self.hidden_dim, activation="relu"),
-                    layers.Dense(units=self.embedding_dim)
-                    ]
-                )
-            )
-
-        self._is_first_batch = True
-        self._is_data_in_dict_format = False
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
 
-    def call(self, inputs):
-        # Find the dataset's format - is it either in dictionary format or array format.
-        # If inputs is an instance of dict, it's in dictionary format
-        # If inputs is an instance of tuple, it's in array format
-        if self._is_first_batch:
-            if isinstance(inputs, dict):
-                self._is_data_in_dict_format = True
-            self._is_first_batch = False
-
-        numerical_feature_embeddings = tf.TensorArray(size=self._num_numerical_features,
-                                                      dtype=tf.float32)
-
-        for i, (feature_name, feature_idx) in enumerate(self.numerical_features_metadata.items()):
-            if self._is_data_in_dict_format:
-                feature = tf.expand_dims(inputs[feature_name], 1)
-            else:
-                feature = tf.expand_dims(inputs[:, feature_idx], 1)
-            embedding = self.embedding_layers[i]
-            feature = embedding(feature)
-            numerical_feature_embeddings = numerical_feature_embeddings.write(i, feature)
-
-        numerical_feature_embeddings = tf.squeeze(numerical_feature_embeddings.stack())
-        if tf.rank(numerical_feature_embeddings) == 3:
-            numerical_feature_embeddings = tf.transpose(numerical_feature_embeddings, perm=[1, 0, 2])
-        else:
-            # else the rank must be 2
-            numerical_feature_embeddings = tf.transpose(numerical_feature_embeddings)
-        return numerical_feature_embeddings
-
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'numerical_features_metadata': self.numerical_features_metadata,
-                      'embedding_dim': self.embedding_dim,
-                      'hidden_dim': self.hidden_dim,
-                      }
-        config.update(new_config)
-        return config
+        features_metadata: ``dict``,
+            a nested dictionary of metadata for features where
+            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
+            feature indices and the lists of unique values (vocabulary) in them,
+            while numerical dictionary is a mapping of numerical feature names to their indices.
+            `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
+            `{feature_name: feature_idx}` for feature in numerical features.
+            You can get this dictionary from
+                >>> from teras.utils import get_features_metadata_for_embedding
+                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
 
+        embedding_dim: ``int``, default 32,
+            Embedding dimensions used in embedding numerical and categorical features.
 
-class MultiHeadInterSampleAttention(layers.Layer):
-    """
-    MultiHeadInterSampleAttention layer as proposed by Gowthami Somepalli et al.
-    in the paper SAINT: Improved Neural Networks for Tabular Data
-    via Row Attention and Contrastive Pre-Training.
-    Unlike the usual MultiHeadAttention layer, this MultiHeadInterSampleAttention layer,
-    as the name enunciates, applies attention over samples/rows instead of features/columns.
+        numerical_embedding_hidden_dim: ``int`` default 16,
+            Dimensionality of the hidden layer that precedes the output layer in the
+            ``SAINTNumericalFeatureEmebedding`` layer.
 
-    Reference(s):
-        https://arxiv.org/abs/2106.01342
+        num_transformer_layer: ``int``, default 6,
+            Number of (SAINT) transformer layers to use in the Encoder.
+            The encoder is used to contextualize the learned feature embeddings.
 
-    Args:
-        num_heads: `int`, default 8,
-            Number of Attention heads to use
-        key_dim: `int`, default 32,
-            Key dimensionality for attention.
-        dropout: `float`, default 0.1,
-            Dropout rate to use.
-    """
-    def __init__(self,
-                 num_heads: int = 8,
-                 key_dim: int = 32,
-                 dropout: float = 0.1,
-                 **kwargs):
-        super().__init__()
-        self.num_heads = num_heads
-        self.key_dim = key_dim
-        self.dropout = dropout
-        self.multi_head_attention = layers.MultiHeadAttention(num_heads=self.num_heads,
-                                                              key_dim=self.key_dim,
-                                                              dropout=dropout,
-                                                              **kwargs)
-
-    def call(self, inputs):
-        # Expected inputs shape: (b, n, d)
-        # b: batch_size, n: num_features, d: embedding_dim
-        x = inputs
-        x = tf.reshape(x, shape=(1,
-                                 tf.shape(x)[0],
-                                 tf.shape(x)[1] * tf.shape(x)[2]))
-        x = self.multi_head_attention(x, x)
-        x = tf.reshape(x, shape=tf.shape(inputs))
-        return x
+        num_attention_heads: ``int``, default 8,
+            Number of attention heads to use in the ``MultiHeadSelfAttention`` layer
+            that is part of the `Transformer` layer which in turn is part of the `Encoder`.
 
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'num_heads': self.num_heads,
-                      'key_dim': self.key_dim,
-                      'dropout': self.dropout,
-                      }
-        config.update(new_config)
-        return config
+        num_inter_sample_attention_heads: ``int``, default 8,
+            Number of heads to use in the ``MultiHeadInterSampleAttention`` that applies
+            attention over rows.
 
+        attention_dropout: ``float``, default 0.1, Dropout rate to use in the
+            ``MultiHeadSelfAttention`` layer in the transformer layer.
 
-class SAINTTransformer(layers.Layer):
-    """
-    SAINT Transformer layer as proposed by Gowthami Somepalli et al.
-    in the paper SAINT: Improved Neural Networks for Tabular Data
-    via Row Attention and Contrastive Pre-Training.
-    It differs from the usual Transformer (L) block in that it contains additional
-    multihead intersample attention layer in addition to the usual multihead attention layer
+        inter_sample_attention_dropout: `float`, default 0.1,
+            Dropout rate for ``MultiHeadInterSampleAttention`` layer that applies
+            attention over rows.
 
-    Reference(s):
-        https://arxiv.org/abs/2106.01342
+        feedforward_dropout: ``float``, default 0.1,
+            Dropout rate to use for the dropout layer in the ``FeedForward`` layer.
 
-    Args:
-        embedding_dim: `int`, default 32,
-            Embedding dimensions used to embedd numerical and
-            categorical features. These server as the key dimensions
-            in the MultiHeadAttention layer.
-        num_attention_heads: `default`, default 8, Number of heads
-            to use in the typical MultiHeadAttention that will be
-            applied over features.
-        num_inter_sample_attention_heads: `int`, default 8,
-            Number of heads to use in the MultiHeadInterSampleAttention
-            that will be applied over rows
-        embedding_dim: `int`, default 32, Embedding dimensions. These will
-            also serve as key dimensions for the MultiHeadAttention layers
-        attention_dropout: `float`, default 0.1, Dropout rate for
-            MultiHeadAttention which is applied over features.
-        inter_sample_attention_dropout: `float`, default 0.1, Dropout rate for
-            MultiHeadInterSampleAttention which is applied over rows.
-        feedforward_dropout: `float`, default 0.1, Dropout rate for the
-            dropout layer that is part of the FeedForward block.
-        feedforward_multiplier: `int`, default 4.
+        feedforward_multiplier: ``int``, default 4.
             Multiplier that is multiplied with the `embedding_dim`
             and the resultant value is used as hidden dimensions value for the
             hidden layer in the feedforward block.
-        apply_attention_to_features: `bool`, default True,
-            Whether to apply attention over features.
-            If True, the regular MultiHeadAttention layer will be applied
-            over features.
-        apply_attention_to_rows: `bool`, default True,
-            Whether to apply attention over rows.
-            If True, the MultiHeadInterSampleAttention will apply attention
-            over rows.
-            NOTE: It is strongly recommended to keep both as True, but you
-            can turn one off for experiment's sake.
-            Also, note that, both CANNOT be False at the same time!
-        num_embedded_features: `int`, Number of features that have been embedded.
-            If both categorical and numerical features are embedded, then
-            `num_features` is equal to the total number of features in the dataset,
-            otherwise if only categorical features are embedded, then `num_features`
-            is equal to the number of categorical features in the dataset.
+
+        norm_epsilon: ``float``, default 1e-6,
+            A very small number used for normalization in the ``LayerNormalization`` layer.
+
+        encode_categorical_values: ``bool``, default True,
+            Whether to (label) encode categorical values.
+            If you've already encoded the categorical values using for instance
+            Label/Ordinal encoding, you should set this to False,
+            otherwise leave it as True.
+            In the case of True, categorical values will be mapped to integer indices
+            using keras's string lookup layer.
+
+        apply_attention_to_features: ``bool``, default True,
+            Whether to apply attention over features using the regular ``MultiHeadAttenion`` layer.
+
+        apply_attention_to_rows: ``bool``, default True,
+            Whether to apply attention over rows using the SAINT ``MultiHeadInterSampleAttention``
+            layer.
+            Although it is strongly recommended to apply attention to both rows and features,
+            but for experimentation's sake you can disable one of them, but NOT both at the
+            same time!
     """
     def __init__(self,
-                 embedding_dim: int = 32,
-                 num_attention_heads: int = 8,
-                 num_inter_sample_attention_heads: int = 8,
-                 attention_dropout: float = 0.1,
-                 inter_sample_attention_dropout: float = 0.1,
-                 feedforward_dropout: float = 0.1,
-                 feedforward_multiplier: int = 4,
-                 norm_epsilon: float = 1e-6,
-                 apply_attention_to_features: bool = True,
-                 apply_attention_to_rows: bool = True,
-                 num_embedded_features: int = None,
-                 **kwagrs):
-        super().__init__(**kwagrs)
+                 input_dim: int,
+                 features_metadata: dict,
+                 embedding_dim: int = SAINTConfig.embedding_dim,
+                 numerical_embedding_hidden_dim: int = SAINTConfig.numerical_embedding_hidden_dim,
+                 num_transformer_layers: int = SAINTConfig.num_transformer_layers,
+                 num_attention_heads: int = SAINTConfig.num_attention_heads,
+                 num_inter_sample_attention_heads: int = SAINTConfig.num_inter_sample_attention_heads,
+                 attention_dropout: float = SAINTConfig.attention_dropout,
+                 inter_sample_attention_dropout: float = SAINTConfig.inter_sample_attention_dropout,
+                 feedforward_dropout: float = SAINTConfig.feedforward_dropout,
+                 feedforward_multiplier: int = SAINTConfig.feedforward_multiplier,
+                 norm_epsilon: float = SAINTConfig.norm_epsilon,
+                 encode_categorical_values: bool = SAINTConfig.encode_categorical_values,
+                 apply_attention_to_features: bool = SAINTConfig.apply_attention_to_features,
+                 apply_attention_to_rows: bool = SAINTConfig.apply_attention_to_rows,
+                 **kwargs
+                 ):
+        num_categorical_features = len(features_metadata["categorical"])
+        num_numerical_features = len(features_metadata["numerical"])
+        numerical_features_exist = num_numerical_features > 0
+        categorical_features_exist = num_categorical_features > 0
+
+        # Numerical/Continuous Features Embedding
+        numerical_feature_embedding = None
+        if numerical_features_exist:
+            # If numerical features exist, then they must be embedded
+            numerical_feature_embedding = SAINTNumericalFeatureEmbedding(
+                features_metadata=features_metadata,
+                embedding_dim=embedding_dim,
+                hidden_dim=numerical_embedding_hidden_dim
+            )
+
+        # Categorical Features Embedding
+        categorical_feature_embedding = None
+        if categorical_features_exist:
+            # If categorical features exist, then they must be embedded
+            categorical_feature_embedding = CategoricalFeatureEmbedding(
+                features_metadata=features_metadata,
+                embedding_dim=embedding_dim,
+                encode=encode_categorical_values)
+
+        encoder = SAINTEncoder(data_dim=input_dim,
+                               num_transformer_layers=num_transformer_layers,
+                               embedding_dim=embedding_dim,
+                               num_attention_heads=num_attention_heads,
+                               num_inter_sample_attention_heads=num_inter_sample_attention_heads,
+                               attention_dropout=attention_dropout,
+                               inter_sample_attention_dropout=inter_sample_attention_dropout,
+                               feedforward_dropout=feedforward_dropout,
+                               feedforward_multiplier=feedforward_multiplier,
+                               norm_epsilon=norm_epsilon,
+                               apply_attention_to_features=apply_attention_to_features,
+                               apply_attention_to_rows=apply_attention_to_rows,
+                               )
+
+        super().__init__(input_dim=input_dim,
+                         encoder=encoder,
+                         categorical_feature_embedding=categorical_feature_embedding,
+                         numerical_feature_embedding=numerical_feature_embedding,
+                         **kwargs)
+
+        self.features_metadata = features_metadata
         self.embedding_dim = embedding_dim
+        self.num_transformer_layers = num_transformer_layers
         self.num_attention_heads = num_attention_heads
         self.num_inter_sample_attention_heads = num_inter_sample_attention_heads
         self.attention_dropout = attention_dropout
         self.inter_sample_attention_dropout = inter_sample_attention_dropout
         self.feedforward_dropout = feedforward_dropout
         self.feedforward_multiplier = feedforward_multiplier
         self.norm_epsilon = norm_epsilon
+        self.encode_categorical_values = encode_categorical_values
+        self.numerical_embedding_hidden_dim = numerical_embedding_hidden_dim
         self.apply_attention_to_features = apply_attention_to_features
         self.apply_attention_to_rows = apply_attention_to_rows
-        self.num_embedded_features = num_embedded_features
-
-        # To make this layer compatible with the layerflow version of this layer,
-        # we instantiate some layers as self attributes
-        self.multihead_inter_sample_attention = MultiHeadInterSampleAttention(
-                                                    num_heads=self.num_inter_sample_attention_heads,
-                                                    key_dim=self.embedding_dim * self.num_embedded_features,
-                                                    dropout=self.inter_sample_attention_dropout,
-                                                    name="inter_sample_multihead_attention"
-                                                    )
-        self.feed_forward = FeedForward(embedding_dim=self.embedding_dim,
-                                        multiplier=self.feedforward_multiplier,
-                                        dropout=feedforward_dropout)
-        self.transformer = Transformer(embedding_dim=self.embedding_dim,
-                                       num_attention_heads=self.num_attention_heads,
-                                       attention_dropout=self.attention_dropout,
-                                       feedforward_dropout=self.feedforward_dropout,
-                                       feedforward_multiplier=self.feedforward_multiplier,
-                                       norm_epsilon=self.norm_epsilon,
-                                       name="inner_trasnformer_block_for_features")
-
-        # by default we make call to the _build_saint_inner_transformer_block function
-        # when the SAINTTransformer gets constructed but when this class is used as a
-        # parent to the layerflow version of this, we want to be able to reconstruct
-        # the functional model using the user passed layers for attention/transformer etc.
-        self._build_saint_inner_transformer_block()
-
-    def _build_saint_inner_transformer_block(self):
-        # We build the inner SAINT Transformer block using keras Functional API
-
-        # Inter Sample Attention Block: this attention is applied to rows.
-        inputs = layers.Input(shape=(self.num_embedded_features, self.embedding_dim))
-        intermediate_outputs = inputs
-
-        if self.apply_attention_to_rows:
-            residual = inputs
-            x = self.multihead_inter_sample_attention(inputs)
-            x = layers.Add()([x, residual])
-            x = layers.LayerNormalization(epsilon=self.norm_epsilon)(x)
-            residual = x
-            x = self.feed_forward(x)
-            x = layers.Add()([x, residual])
-            intermediate_outputs = layers.LayerNormalization(epsilon=self.norm_epsilon)(x)
-            final_outputs = intermediate_outputs
-
-        # MultiHeadAttention block: this attention is applied to columns
-        if self.apply_attention_to_features:
-            # If `apply_attention_to_features` is set to True,
-            # then attention will be applied to columns/features
-            # The MultiHeadInterSampleAttention applies attention over rows,
-            # but the regular MultiHeadAttention layer is used to apply attention over features.
-            # Since the common Transformer layer applies MutliHeadAttention over features
-            # as well as takes care of applying all the preceding and following layers,
-            # so we'll just use that here.
-            final_outputs = self.transformer(intermediate_outputs)
-
-        self.transformer_block = keras.Model(inputs=inputs,
-                                             outputs=final_outputs,
-                                             name="saint_inner_transformer_block")
-
-    def call(self, inputs):
-        out = self.transformer_block(inputs)
-        return out
 
     def get_config(self):
-        config = super().get_config()
-        new_config = {'embedding_dim': self.embedding_dim,
-                      'num_attention_heads': self.num_attention_heads,
-                      'num_inter_sample_attention_heads': self.num_inter_sample_attention_heads,
-                      'attention_dropout': self.attention_dropout,
-                      'inter_sample_attention_dropout': self.inter_sample_attention_dropout,
-                      'feedforward_dropout': self.feedforward_dropout,
-                      'feedforward_multiplier': self.feedforward_multiplier,
-                      'norm_epsilon': self.norm_epsilon,
-                      'apply_attention_to_features': self.apply_attention_to_features,
-                      'apply_attention_to_rows': self.apply_attention_to_rows,
-                      'num_embedded_features': self.num_embedded_features,
-                      }
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'input_dim': self.input_dim,
+                  'features_metadata': self.features_metadata,
+                  'embedding_dim': self.embedding_dim,
+                  'numerical_embedding_hidden_dim': self.numerical_embedding_hidden_dim,
+                  'num_transformer_layers': self.num_transformer_layers,
+                  'num_attention_heads': self.num_attention_heads,
+                  'num_inter_sample_attention_heads': self.num_inter_sample_attention_heads,
+                  'attention_dropout': self.attention_dropout,
+                  'inter_sample_attention_dropout': self.inter_sample_attention_dropout,
+                  'feedforward_dropout': self.feedforward_dropout,
+                  'feedforward_multiplier': self.feedforward_multiplier,
+                  'norm_epsilon': self.norm_epsilon,
+                  'encode_categorical_values': self.encode_categorical_values,
+                  'apply_attention_to_features': self.apply_attention_to_features,
+                  'apply_attention_to_rows': self.apply_attention_to_rows,
+                  }
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        features_metadata = config.pop("features_metadata")
+        return cls(input_dim=input_dim,
+                   features_metadata=features_metadata, **config)
 
-class Encoder(layers.Layer):
+
+@keras.saving.register_keras_serializable("teras.models")
+class SAINTClassifier(SAINT):
     """
-    Encoder for SAINT as proposed by Gowthami Somepalli et al. in the paper
+    SAINTClassifier model based on the SAINT architecture proposed by
+    Gowthami Somepalli et al. in the paper,
     SAINT: Improved Neural Networks for Tabular Data
     via Row Attention and Contrastive Pre-Training.
-    It simply stacks N transformer layers and applies them to the outputs
-    of the embedded features.
 
-    It differs from the typical Encoder block only in that the Transformer
-    layer is a bit different from the regular Transformer layer used in the
-    Transformer based architectures as it uses multi-head inter-sample attention,
-    in addition to the regular mutli-head attention for features.
+    SAINT performs attention over both rows and columns.
 
     Reference(s):
         https://arxiv.org/abs/2106.01342
 
     Args:
-        num_transformer_layer: `int`, default 6,
-            Number of transformer layers to use in the Encoder
-        embedding_dim: `int`, default 32,
-            Embedding dimensions used to embedd numerical and
-            categorical features. These server as the key dimensions
-            in the MultiHeadAttention layer.
-        num_attention_heads: `default`, default 8, Number of heads
-            to use in the typical MultiHeadAttention that will be
-            applied over features.
-        num_inter_sample_attention_heads: `int`, default 8,
-            Number of heads to use in the MultiHeadInterSampleAttention
-            that will be applied over rows
-        embedding_dim: `int`, default 32, Embedding dimensions. These will
-            also serve as key dimensions for the MultiHeadAttention layers
-        attention_dropout: `float`, default 0.1, Dropout rate for
-            MultiHeadAttention which is applied over features.
-        inter_sample_attention_dropout: `float`, default 0.1, Dropout rate for
-            MultiHeadInterSampleAttention which is applied over rows.
-        feedforward_dropout: `float`, default 0.1, Dropout rate for the
-            dropout layer that is part of the FeedForward block.
-        feedforward_multiplier: `int`, default 4.
+        num_classes: ``int``, default 2,
+            Number of classes to predict.
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default [64, 32],
+            Hidden units to use in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        features_metadata: ``dict``,
+            a nested dictionary of metadata for features where
+            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
+            feature indices and the lists of unique values (vocabulary) in them,
+            while numerical dictionary is a mapping of numerical feature names to their indices.
+            `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
+            `{feature_name: feature_idx}` for feature in numerical features.
+            You can get this dictionary from
+                >>> from teras.utils import get_features_metadata_for_embedding
+                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        embedding_dim: ``int``, default 32,
+            Embedding dimensions used in embedding numerical and categorical features.
+
+        numerical_embedding_hidden_dim: ``int`` default 16,
+            Dimensionality of the hidden layer that precedes the output layer in the
+            ``SAINTNumericalFeatureEmebedding`` layer.
+
+        num_transformer_layer: ``int``, default 6,
+            Number of (SAINT) transformer layers to use in the Encoder.
+            The encoder is used to contextualize the learned feature embeddings.
+
+        num_attention_heads: ``int``, default 8,
+            Number of attention heads to use in the ``MultiHeadSelfAttention`` layer
+            that is part of the `Transformer` layer which in turn is part of the `Encoder`.
+
+        num_inter_sample_attention_heads: ``int``, default 8,
+            Number of heads to use in the ``MultiHeadInterSampleAttention`` that applies
+            attention over rows.
+
+        attention_dropout: ``float``, default 0.1, Dropout rate to use in the
+            ``MultiHeadSelfAttention`` layer in the transformer layer.
+
+        inter_sample_attention_dropout: `float`, default 0.1,
+            Dropout rate for ``MultiHeadInterSampleAttention`` layer that applies
+            attention over rows.
+
+        feedforward_dropout: ``float``, default 0.1,
+            Dropout rate to use for the dropout layer in the ``FeedForward`` layer.
+
+        feedforward_multiplier: ``int``, default 4.
             Multiplier that is multiplied with the `embedding_dim`
             and the resultant value is used as hidden dimensions value for the
             hidden layer in the feedforward block.
-        apply_attention_to_features: `bool`, default True,
-            Whether to apply attention over features.
-            If True, the regular MultiHeadAttention layer will be applied
-            over features.
-        apply_attention_to_rows: `bool`, default True,
-            Whether to apply attention over rows.
-            If True, the MultiHeadInterSampleAttention will apply attention
-            over rows.
-            NOTE: It is strongly recommended to keep both as True, but you
-            can turn one off for experiment's sake.
-            Also, note that, both CANNOT be False at the same time!
-        num_embedded_features: `int`, Number of features that have been embedded.
-            If both categorical and numerical features are embedded, then
-            `num_features` is equal to the total number of features in the dataset,
-            otherwise if only categorical features are embedded, then `num_features`
-            is equal to the number of categorical features in the dataset.
-    """
-    def __init__(self,
-                 num_transformer_layers: int = 6,
-                 embedding_dim: int = 32,
-                 num_attention_heads: int = 8,
-                 num_inter_sample_attention_heads: int = 8,
-                 attention_dropout: float = 0.1,
-                 inter_sample_attention_dropout: float = 0.1,
-                 feedforward_dropout: float = 0.1,
-                 feedforward_multiplier: int = 4,
-                 norm_epsilon: float = 1e-6,
-                 apply_attention_to_features: bool = True,
-                 apply_attention_to_rows: bool = True,
-                 num_embedded_features: int = None,
-                 **kwargs):
-        super().__init__(**kwargs)
 
-        if not apply_attention_to_features and not apply_attention_to_rows:
-            raise ValueError("`apply_attention_to_features` and `apply_attention_to_rows` both cannot be False "
-                             "at the same time. You must set at least one to True if not both. "
-                             f"Received: `apply_attention_to_features`={apply_attention_to_features}, "
-                             f"`apply_attention_to_rows`={apply_attention_to_rows}")
+        norm_epsilon: ``float``, default 1e-6,
+            A very small number used for normalization in the ``LayerNormalization`` layer.
 
-        self.num_transformer_layers = num_transformer_layers
-        self.embedding_dim = embedding_dim
-        self.num_attention_heads = num_attention_heads
-        self.num_inter_sample_attention_heads = num_inter_sample_attention_heads
-        self.attention_dropout = attention_dropout
-        self.inter_sample_attention_dropout = inter_sample_attention_dropout
-        self.feedforward_dropout = feedforward_dropout
-        self.feedforward_multiplier = feedforward_multiplier
-        self.norm_epsilon = norm_epsilon
-        self.apply_attention_to_features = apply_attention_to_features
-        self.apply_attention_to_rows = apply_attention_to_rows
-        self.num_embedded_features = num_embedded_features
-
-        self.saint_transformer_layers = keras.models.Sequential(name="saint_transformer_layers")
-        for i in range(self.num_transformer_layers):
-            self.saint_transformer_layers.add(SAINTTransformer(
-                embedding_dim=self.embedding_dim,
-                num_attention_heads=self.num_attention_heads,
-                num_inter_sample_attention_heads=self.num_inter_sample_attention_heads,
-                attention_dropout=self.attention_dropout,
-                inter_sample_attention_dropout=self.inter_sample_attention_dropout,
-                feedforward_dropout=self.feedforward_dropout,
-                feedforward_multiplier=self.feedforward_multiplier,
-                apply_attention_to_features=self.apply_attention_to_features,
-                apply_attention_to_rows=self.apply_attention_to_rows,
-                num_embedded_features=self.num_embedded_features,
-                name=f"saint_transformer_layer_{i}"))
-
-    def call(self, inputs):
-        outputs = self.saint_transformer_layers(inputs)
-        return outputs
+        encode_categorical_values: ``bool``, default True,
+            Whether to (label) encode categorical values.
+            If you've already encoded the categorical values using for instance
+            Label/Ordinal encoding, you should set this to False,
+            otherwise leave it as True.
+            In the case of True, categorical values will be mapped to integer indices
+            using keras's string lookup layer.
+
+        apply_attention_to_features: ``bool``, default True,
+            Whether to apply attention over features using the regular ``MultiHeadAttenion`` layer.
+
+        apply_attention_to_rows: ``bool``, default True,
+            Whether to apply attention over rows using the SAINT ``MultiHeadInterSampleAttention``
+            layer.
+            Although it is strongly recommended to apply attention to both rows and features,
+            but for experimentation's sake you can disable one of them, but NOT both at the
+            same time!
+    """
+    def __init__(self,
+                 num_classes: int = 2,
+                 head_units_values: UnitsValuesType = (64, 32),
+                 input_dim: int = None,
+                 features_metadata: dict = None,
+                 embedding_dim: int = SAINTConfig.embedding_dim,
+                 numerical_embedding_hidden_dim: int = SAINTConfig.numerical_embedding_hidden_dim,
+                 num_transformer_layers: int = SAINTConfig.num_transformer_layers,
+                 num_attention_heads: int = SAINTConfig.num_attention_heads,
+                 num_inter_sample_attention_heads: int = SAINTConfig.num_inter_sample_attention_heads,
+                 attention_dropout: float = SAINTConfig.attention_dropout,
+                 inter_sample_attention_dropout: float = SAINTConfig.inter_sample_attention_dropout,
+                 feedforward_dropout: float = SAINTConfig.feedforward_dropout,
+                 feedforward_multiplier: int = SAINTConfig.feedforward_multiplier,
+                 norm_epsilon: float = SAINTConfig.norm_epsilon,
+                 encode_categorical_values: bool = SAINTConfig.encode_categorical_values,
+                 apply_attention_to_features: bool = SAINTConfig.apply_attention_to_features,
+                 apply_attention_to_rows: bool = SAINTConfig.apply_attention_to_rows,
+                 **kwargs
+                 ):
+        if features_metadata is None:
+            raise ValueError("`features_metadata` cannot be None. "
+                             "You can get features metadata dictionary using the `get_features_metadata_for_embedding` "
+                             "function from teras.utils.")
+        # Since the parent `SAINT` class subclasses its LayerFlow version
+        # which accepts layers as input and does expose a head argument to pass the layer.
+        # we can create a relevant head layer, in this case, the `ClassificationHead` layer
+        # and pass its instance to the parent who will pass it along to its parent as part of
+        # the **kwargs dict
+        head = ClassificationHead(num_classes=num_classes,
+                                  units_values=head_units_values,
+                                  activation_hidden="relu",
+                                  normalization="batch",
+                                  name="saint_classifier_head")
+        super().__init__(input_dim=input_dim,
+                         features_metadata=features_metadata,
+                         embedding_dim=embedding_dim,
+                         numerical_embedding_hidden_dim=numerical_embedding_hidden_dim,
+                         num_transformer_layers=num_transformer_layers,
+                         num_attention_heads=num_attention_heads,
+                         num_inter_sample_attention_heads=num_inter_sample_attention_heads,
+                         attention_dropout=attention_dropout,
+                         inter_sample_attention_dropout=inter_sample_attention_dropout,
+                         feedforward_dropout=feedforward_dropout,
+                         feedforward_multiplier=feedforward_multiplier,
+                         norm_epsilon=norm_epsilon,
+                         encode_categorical_values=encode_categorical_values,
+                         apply_attention_to_features=apply_attention_to_features,
+                         apply_attention_to_rows=apply_attention_to_rows,
+                         head=head,
+                         **kwargs)
+        self.num_classes = num_classes
+        self.head_units_values = head_units_values
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_transformer_layers': self.num_transformer_layers,
-                      'embedding_dim': self.embedding_dim,
-                      'num_attention_heads': self.num_attention_heads,
-                      'num_inter_sample_attention_heads': self.num_inter_sample_attention_heads,
-                      'attention_dropout': self.attention_dropout,
-                      'inter_sample_attention_dropout': self.inter_sample_attention_dropout,
-                      'feedforward_dropout': self.feedforward_dropout,
-                      'feedforward_multiplier': self.feedforward_multiplier,
-                      'norm_epsilon': self.norm_epsilon,
-                      'apply_attention_to_features': self.apply_attention_to_features,
-                      'apply_attention_to_rows': self.apply_attention_to_rows,
-                      'num_embedded_features': self.num_embedded_features,
-                      }
-        config.update(new_config)
+        config.update({'num_classes': self.num_classes,
+                       'head_units_values': self.head_units_values
+                       })
         return config
 
 
-class ProjectionHead(layers.Layer):
+@keras.saving.register_keras_serializable("teras.models")
+class SAINTRegressor(SAINT):
     """
-    ProjectionHead layer that is used in the contrastive learning phase of
-    the SAINTPretrainer to project embeddings to a lower dimension.
-    According to the SAINT paper,
-    "The use of a projection head to reduce dimensionality before computing
-    contrastive loss is common in vision and indeed also improves results
-    on tabular data."
+    SAINTRegressor model based on the SAINT architecture proposed by
+    Gowthami Somepalli et al. in the paper,
+    SAINT: Improved Neural Networks for Tabular Data
+    via Row Attention and Contrastive Pre-Training.
+
+    SAINT performs attention over both rows and columns.
 
     Reference(s):
-    https://arxiv.org/abs/2106.01342
+        https://arxiv.org/abs/2106.01342
 
     Args:
-        hidden_dim: `int`,
-            Dimensionality of the hidden layer.
-            In the official implementation, it is computed as follows,
-            `hidden_dim = 6 * embedding_dim * number_of_features // 5`
-        hidden_activation, default "relu":
-            Activation function to use in the hidden layer.
-        output_dim: `int`,
-            Dimensionality of the output layer.
-            In the official implementation, it is computed as follows,
-            `output_dim = embedding_dim * number_of_featuers // 5`
-    """
-    def __init__(self,
-                 hidden_dim: int = None,
-                 hidden_activation="relu",
-                 output_dim: int = None,
-                 **kwargs):
-        super().__init__(**kwargs)
-        self.hidden_dim = hidden_dim
-        self.hidden_activation = hidden_activation
-        self.output_dim = output_dim
-
-        self.hidden_block = layers.Dense(units=self.hidden_dim,
-                                         activation=self.hidden_activation)
-        self.output_layer = layers.Dense(units=self.output_dim)
-
-    def call(self, inputs):
-        x = self.hidden_block(inputs)
-        outputs = self.output_layer(x)
-        return outputs
+        num_outputs: ``int``, default 1,
+            Number of regression outputs to predict.
 
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default [64, 32],
+            Hidden units to use in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
 
-class ReconstructionBlock(layers.Layer):
-    """
-    ReconstructionBlock layer that is used in constructing ReconstructionHead.
-    One ReconstructionBlock is created for each feature in the dataset.
+        features_metadata: ``dict``,
+            a nested dictionary of metadata for features where
+            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
+            feature indices and the lists of unique values (vocabulary) in them,
+            while numerical dictionary is a mapping of numerical feature names to their indices.
+            `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
+            `{feature_name: feature_idx}` for feature in numerical features.
+            You can get this dictionary from
+                >>> from teras.utils import get_features_metadata_for_embedding
+                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
 
-    Args:
-        hidden_dim: `int`,
-            Dimensionality of the hidden layer.
-        hidden_activation:
-            Activation function to use in the hidden layer.
-        data_dim: `int`,
-            Dimensionality of the given input feature.
-            The inputs to this layer are first mapped to hidden dimensions
-            and then projected to the dimensionality of the feature.
-            For categorical features, it is equal to the number of classes
-            in the feature, and for numerical feautures, it is equal to 1.
+        embedding_dim: ``int``, default 32,
+            Embedding dimensions used in embedding numerical and categorical features.
+
+        numerical_embedding_hidden_dim: ``int`` default 16,
+            Dimensionality of the hidden layer that precedes the output layer in the
+            ``SAINTNumericalFeatureEmebedding`` layer.
+
+        num_transformer_layer: ``int``, default 6,
+            Number of (SAINT) transformer layers to use in the Encoder.
+            The encoder is used to contextualize the learned feature embeddings.
+
+        num_attention_heads: ``int``, default 8,
+            Number of attention heads to use in the ``MultiHeadSelfAttention`` layer
+            that is part of the `Transformer` layer which in turn is part of the `Encoder`.
+
+        num_inter_sample_attention_heads: ``int``, default 8,
+            Number of heads to use in the ``MultiHeadInterSampleAttention`` that applies
+            attention over rows.
+
+        attention_dropout: ``float``, default 0.1, Dropout rate to use in the
+            ``MultiHeadSelfAttention`` layer in the transformer layer.
+
+        inter_sample_attention_dropout: `float`, default 0.1,
+            Dropout rate for ``MultiHeadInterSampleAttention`` layer that applies
+            attention over rows.
+
+        feedforward_dropout: ``float``, default 0.1,
+            Dropout rate to use for the dropout layer in the ``FeedForward`` layer.
+
+        feedforward_multiplier: ``int``, default 4.
+            Multiplier that is multiplied with the `embedding_dim`
+            and the resultant value is used as hidden dimensions value for the
+            hidden layer in the feedforward block.
+
+        norm_epsilon: ``float``, default 1e-6,
+            A very small number used for normalization in the ``LayerNormalization`` layer.
+
+        encode_categorical_values: ``bool``, default True,
+            Whether to (label) encode categorical values.
+            If you've already encoded the categorical values using for instance
+            Label/Ordinal encoding, you should set this to False,
+            otherwise leave it as True.
+            In the case of True, categorical values will be mapped to integer indices
+            using keras's string lookup layer.
+
+        apply_attention_to_features: ``bool``, default True,
+            Whether to apply attention over features using the regular ``MultiHeadAttenion`` layer.
+
+        apply_attention_to_rows: ``bool``, default True,
+            Whether to apply attention over rows using the SAINT ``MultiHeadInterSampleAttention``
+            layer.
+            Although it is strongly recommended to apply attention to both rows and features,
+            but for experimentation's sake you can disable one of them, but NOT both at the
+            same time!
     """
+
     def __init__(self,
-                 hidden_dim: int = None,
-                 hidden_activation="relu",
-                 data_dim: int = None,
-                 **kwargs):
-        super().__init__(**kwargs)
-        self.hidden_block = layers.Dense(hidden_dim,
-                                         activation=hidden_activation)
-        self.output_layer = layers.Dense(data_dim)
-
-    def call(self, inputs):
-        x = self.hidden_block(inputs)
-        outputs = self.output_layer(x)
-        return outputs
+                 num_outputs: int = 1,
+                 head_units_values: UnitsValuesType = (64, 32),
+                 input_dim: int = None,
+                 features_metadata: dict = None,
+                 embedding_dim: int = SAINTConfig.embedding_dim,
+                 numerical_embedding_hidden_dim: int = SAINTConfig.numerical_embedding_hidden_dim,
+                 num_transformer_layers: int = SAINTConfig.num_transformer_layers,
+                 num_attention_heads: int = SAINTConfig.num_attention_heads,
+                 num_inter_sample_attention_heads: int = SAINTConfig.num_inter_sample_attention_heads,
+                 attention_dropout: float = SAINTConfig.attention_dropout,
+                 inter_sample_attention_dropout: float = SAINTConfig.inter_sample_attention_dropout,
+                 feedforward_dropout: float = SAINTConfig.feedforward_dropout,
+                 feedforward_multiplier: int = SAINTConfig.feedforward_multiplier,
+                 norm_epsilon: float = SAINTConfig.norm_epsilon,
+                 encode_categorical_values: bool = SAINTConfig.encode_categorical_values,
+                 apply_attention_to_features: bool = SAINTConfig.apply_attention_to_features,
+                 apply_attention_to_rows: bool = SAINTConfig.apply_attention_to_rows,
+                 **kwargs
+                 ):
+        if features_metadata is None:
+            raise ValueError("`features_metadata` cannot be None. "
+                             "You can get features metadata dictionary using the `get_features_metadata_for_embedding` "
+                             "function from teras.utils.")
+        head = RegressionHead(num_outputs=num_outputs,
+                              units_values=head_units_values,
+                              activation_hidden="relu",
+                              normalization="batch",
+                              name="saint_regressor_head")
+        super().__init__(input_dim=input_dim,
+                         features_metadata=features_metadata,
+                         embedding_dim=embedding_dim,
+                         numerical_embedding_hidden_dim=numerical_embedding_hidden_dim,
+                         num_transformer_layers=num_transformer_layers,
+                         num_attention_heads=num_attention_heads,
+                         num_inter_sample_attention_heads=num_inter_sample_attention_heads,
+                         attention_dropout=attention_dropout,
+                         inter_sample_attention_dropout=inter_sample_attention_dropout,
+                         feedforward_dropout=feedforward_dropout,
+                         feedforward_multiplier=feedforward_multiplier,
+                         norm_epsilon=norm_epsilon,
+                         encode_categorical_values=encode_categorical_values,
+                         apply_attention_to_features=apply_attention_to_features,
+                         apply_attention_to_rows=apply_attention_to_rows,
+                         head=head,
+                         **kwargs)
+        self.num_outputs = num_outputs
+        self.head_units_values = head_units_values
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'hidden_dim': self.hidden_dim,
-                      'hidden_activation': self.hidden_activation,
-                      'data_dim': self.data_dim,
-                      }
-        config.update(new_config)
+        config.update({'num_outputs': self.num_outputs,
+                       'head_units_values': self.head_units_values,
+                       })
         return config
 
 
-class ReconstructionHead(layers.Layer):
+@keras.saving.register_keras_serializable("teras.models")
+class SAINTPretrainer(_SAINTPretrainerLF):
     """
-    ReconstructionHead layer for SAINTPretrainer model.
-    SAINT applies a separate single hidden layer MLP block
-    (here we name it, the reconstruction block)
-    with an output layer where output dimensions are equal
-    to the number of categories in the case of categorical
-    features and 1 in the case of numerical features.
+    SAINTPretrainer model based on the pretraining architecture
+    for the SAINT model proposed by Gowthami Somepalli et al.
+    in the paper,
+    SAINT: Improved Neural Networks for Tabular Data
+    via Row Attention and Contrastive Pre-Training.
+
+    SAINT performs attention over both rows and columns.
+
+    Reference(s):
+        https://arxiv.org/abs/2106.01342
 
     Args:
-        features_metadata: `dict`,
+        model: ``SAINT``,
+            An instance of the ``SAINT`` model that you want to pretrain.
+            Note that, you should use the base ``SAINT`` model's instance,
+            not ``SAINTClassifier`` or ``SAINTRegressor``.
+            Using default API, you can import it as,
+                >>> from teras.models import SAINT
+            Using LayerFlow API, you can import it as,
+                >>> from teras.layerflow.models import SAINT
+                And REMEMBER to leave the ``head`` argment as None.
+
+        features_metadata: ``dict``,
             a nested dictionary of metadata for features where
             categorical sub-dictionary is a mapping of categorical feature names to a tuple of
             feature indices and the lists of unique values (vocabulary) in them,
             while numerical dictionary is a mapping of numerical feature names to their indices.
             `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
             `{feature_name: feature_idx}` for feature in numerical features.
             You can get this dictionary from
                 >>> from teras.utils import get_features_metadata_for_embedding
                 >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
-                                                                        numerical_features,
-                                                                        categorical_features)
-        embedding_dim: `int`, default 32,
-            Embedding dimensions being used in the pretraining model.
-            Used in the computation of the hidden dimensions for each
-            reconstruction (mlp) block for each feature.
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        embedding_dim: ``int``, default 32,
+            Embedding dimensions being used by the base model for embedding
+            numerical and categorical features.
+
+        cutmix_probs: ``float``, default 0.1,
+            ``CutMix`` probability which is used in generation of mask
+            that is used to mix samples together.
+
+        mixup_alpha: ``float``, default 1.0,
+            Alpha value for the ``MixUp`` layer, that is used for the
+            Beta distribution to sample `lambda_`
+            which is used to interpolate samples.
+
+        temperature: ``float``, default 0.7,
+            Temperature value used in the computation of the InfoNCE contrastive loss.
+
+        lambda_: ``float``, default 10,
+            Controls the weightage of denoising loss in the summation of denoising and
+            contrastive loss.
     """
     def __init__(self,
+                 model: SAINT,
                  features_metadata: dict,
                  embedding_dim: int = 32,
+                 cutmix_probs: float = 0.3,
+                 mixup_alpha: float = 1.0,
+                 temperature: float = 0.7,
+                 lambda_: float = 10.,
                  **kwargs):
-        super().__init__(**kwargs)
+        mixup = MixUp(alpha=mixup_alpha)
+        cutmix = CutMix(probs=cutmix_probs)
+        num_features = len(features_metadata["categorical"]) + len(features_metadata["numerical"])
+
+        # For the computation of contrastive loss, we use projection heads.
+        # Projection head hidden dimensions as calculated by the
+        # official implementation
+        projection_head_hidden_dim = 6 * embedding_dim * num_features // 5
+        projection_head_output_dim = embedding_dim * num_features // 2
+
+        projection_head_1 = SAINTProjectionHead(hidden_dim=projection_head_hidden_dim,
+                                                output_dim=projection_head_output_dim,
+                                                name="projection_head_for_original_data")
+
+        projection_head_2 = SAINTProjectionHead(hidden_dim=projection_head_hidden_dim,
+                                                output_dim=projection_head_output_dim,
+                                                name="projection_head_for_augmented_data")
+
+        reconstruction_head = SAINTReconstructionHead(features_metadata=model.features_metadata,
+                                                      embedding_dim=model.embedding_dim)
+
+        super().__init__(model=model,
+                         features_metadata=features_metadata,
+                         mixup=mixup,
+                         cutmix=cutmix,
+                         projection_head_1=projection_head_1,
+                         projection_head_2=projection_head_2,
+                         reconstruction_head=reconstruction_head,
+                         **kwargs)
+        self.model = model
         self.features_metadata = features_metadata
         self.embedding_dim = embedding_dim
-
-        categorical_features_metadata = self.features_metadata["categorical"]
-        numerical_features_metadata = self.features_metadata["numerical"]
-        num_categorical_features = len(categorical_features_metadata)
-        num_numerical_features = len(numerical_features_metadata)
-        self.num_features = num_categorical_features + num_numerical_features
-
-        # feature_dims: Dimensions of each feature in the input
-        # For a categorical feature, it is equal to the number of unique categories in the feature
-        # For a numerical features, it is equal to 1
-        feature_dims = []
-        # recall that categorical_features_metadata dict maps feature names to a tuple of
-        # feature id and unique values in the feature
-        if num_categorical_features > 0:
-            feature_dims = list(map(lambda x: len(x[1]), categorical_features_metadata.values()))
-        # for num in num_categories_per_feature:
-        #     feature_dims.append(num)
-        feature_dims.extend([1] * num_numerical_features)
-
-        # For the computation of denoising loss, we use a separate MLP block for each feature
-        # we call the combined blocks, reconstruction heads
-        self.reconstruction_blocks = [
-            ReconstructionBlock(hidden_dim=self.embedding_dim * 5,
-                                data_dim=dim)
-            for dim in feature_dims]
-
-    def call(self, inputs):
-        """
-        Args:
-            inputs: SAINT transformer outputs for the augmented data.
-                Since we apply categorical and numerical embedding layers
-                separately and then combine them into a new features matrix
-                this effectively makes the first k features in the outputs
-                categorical (since categorical embeddings are applied first)
-                and all other features numerical.
-                Here, k = num_categorical_features
-
-        Returns:
-            Reconstructed input features
-        """
-        reconstructed_inputs = []
-        for idx in range(self.num_features):
-            feature_encoding = inputs[:, idx]
-            reconstructed_feature = self.reconstruction_blocks[idx](feature_encoding)
-            reconstructed_inputs.append(reconstructed_feature)
-        # the reconstructed inputs will have features equal to
-        # `number of numerical features` + `number of categories in the categorical features`
-        reconstructed_inputs = tf.concat(reconstructed_inputs, axis=1)
-        return reconstructed_inputs
+        self.cutmix_probs = cutmix_probs
+        self.mixup_alpha = mixup_alpha
+        self.temperature = temperature
+        self.lambda_ = lambda_
 
     def get_config(self):
-        config = super().get_config()
-        new_config = {'features_metadata': self.features_metadata,
-                      'embedding_dim': self.embedding_dim,
-                      }
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'model': keras.layers.serialize(self.model),
+                  'features_metadata': self.features_metadata,
+                  'embedding_dim': self.embedding_dim,
+                  'cutmix_probs': self.cutmix_probs,
+                  'mixup_alpha': self.mixup_alpha,
+                  'temperature': self.temperature,
+                  'lambda_': self.lambda_,
+                  }
         return config
 
-
-class ClassificationHead(BaseClassificationHead):
-    """
-    Classification head for the SAINT Classifier architecture.
-
-    Args:
-        num_classes: `int`, default 2,
-            Number of classes to predict.
-        units_values: `List[int] | Tuple[int]`, default (64, 32),
-            For each value in the sequence,
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the ClassificationHead.
-        activation_hidden: default "relu",
-            Activation function to use in hidden dense layers.
-        activation_out:
-            Activation function to use for the output layer.
-            If not specified, `sigmoid` is used for binary and `softmax` is used for
-            multiclass classification.
-        normalization: `Layer | str`, default "batch",
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
-    """
-    def __init__(self,
-                 num_classes: int = 2,
-                 units_values: LIST_OR_TUPLE = (64, 32),
-                 activation_hidden="relu",
-                 activation_out=None,
-                 normalization: LAYER_OR_STR = "batch",
-                 **kwargs):
-        super().__init__(num_classes=num_classes,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         activation_out=activation_out,
-                         normalization=normalization,
-                         **kwargs)
-
-
-class RegressionHead(BaseRegressionHead):
-    """
-    Regression head for the SAINT Regressor architecture.
-
-    Args:
-        num_outputs: `int`, default 1,
-            Number of regression outputs to predict.
-        units_values: `List[int] | Tuple[int]`, default (64, 32),
-            For each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the RegressionHead.
-        activation_hidden: default "relu",
-            Activation function to use in hidden dense layers.
-        normalization: `Layer | str`, default "batch",
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
-    """
-    def __init__(self,
-                 num_outputs: int = 1,
-                 units_values: LIST_OR_TUPLE = (64, 32),
-                 activation_hidden="relu",
-                 normalization: LAYER_OR_STR = "batch",
-                 **kwargs):
-        super().__init__(num_outputs=num_outputs,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         normalization=normalization,
-                         **kwargs)
+    @classmethod
+    def from_config(cls, config):
+        model = keras.layers.deserialize(config.pop("model"))
+        features_metadata = config.pop("features_metadata")
+        return cls(model, features_metadata, **config)
```

### Comparing `Teras-0.1.1/teras/layers/tabnet.py` & `Teras-0.2.0/teras/models/tabnet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,667 +1,584 @@
-import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers, models
-import tensorflow_addons as tfa
-from teras.layers import GLU
-from teras.layers.common.head import (RegressionHead as BaseRegressionHead,
-                                      ClassificationHead as BaseClassificationHead)
-from typing import Union, List, Tuple
+from teras.layers.tabnet.tabnet_encoder import TabNetEncoder
+from teras.layers.tabnet.tabnet_decoder import TabNetDecoder
+from teras.layers.categorical_feature_embedding import CategoricalFeatureEmbedding
+from teras.layers.common.head import (ClassificationHead,
+                                      RegressionHead)
+from teras.config.tabnet import TabNetConfig
+from teras.layerflow.models.tabnet import (TabNet as _TabNetLF,
+                                           TabNetPretrainer as _TabNetPretrainerLF)
+from teras.utils.types import UnitsValuesType
 
-LIST_OR_TUPLE = Union[List[int], Tuple[int]]
-LAYER_OR_STR = Union[keras.layers.Layer, str]
 
-
-class AttentiveTransformer(layers.Layer):
+@keras.saving.register_keras_serializable(package="keras.models")
+class TabNet(_TabNetLF):
     """
-    Attentive Transformer layer for mask generation
-    as proposed by Sercan et al. in TabNet paper.
-    It applies a Dense layer followed by a BatchNormalization layer
-    followed by a GLU activation layer.
+    TabNet model as proposed by Sercan et al. in TabNet paper.
+    This purpose will serve as the parent class for the TabNetRegressor and TabNetClassifier.
 
     Reference(s):
         https://arxiv.org/abs/1908.07442
 
     Args:
-        num_features: `int`, Number of features in the input dataset.
-        batch_momentum: `float`, default 0.9, Momentum value to use for BatchNormalization layer.
-        virtual_batch_size: `int`, default 64, Batch size to use for `virtual_batch_size`
-            parameter in BatchNormalization layer.
-        relaxation_factor: `float`, default 1.5, Relaxation factor that promotes the reuse of each
-            feature at different decision steps. When it is 1, a feature is enforced
-            to be used only at one decision step and as it increases, more
-            flexibility is provided to use a feature at multiple decision steps.
-            An optimal value of relaxation_factor can have a major role on the performance.
-            Typically, a larger value for `num_decision_steps` favors for a larger `relaxation_factor`.
-
-    """
-    def __init__(self,
-                 num_features,
-                 batch_momentum: float = 0.9,
-                 virtual_batch_size: int = 64,
-                 relaxation_factor: float = 1.5,
-                 **kwargs):
-        super().__init__(**kwargs)
-        self.num_features = num_features
-        self.batch_momentum = batch_momentum
-        self.virtual_batch_size = virtual_batch_size
-        self.relaxation_factor = relaxation_factor
-
-        self.dense = layers.Dense(self.num_features, use_bias=False)
-        self.batch_norm = layers.BatchNormalization(momentum=batch_momentum,
-                                                    virtual_batch_size=self.virtual_batch_size)
-
-    def call(self, inputs, prior_scales=None):
-        # We need the batch_size and inputs_dimensions to initialize prior scale,
-        # we can get them when attentive transformer first gets called.
-        outputs = self.dense(inputs)
-        outputs = self.batch_norm(outputs)
-        outputs *= prior_scales
-        outputs = tfa.activations.sparsemax(outputs)
-        return outputs
-
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'num_features': self.num_features,
-                      'batch_momentum': self.batch_momentum,
-                      'virtual_batch_size': self.virtual_batch_size,
-                      'relaxation_factor': self.relaxation_factor,
-                      }
-        config.update(new_config)
-        return config
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the input dataset.
+
+        features_metadata: ``dict``,
+            A nested dictionary of metadata for features where
+            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
+            feature indices and the lists of unique values (vocabulary) in them,
+            while numerical dictionary is a mapping of numerical feature names to their indices.
+            ``{feature_name: (feature_idx, vocabulary)}`` for feature in categorical features.
+            ``{feature_name: feature_idx}`` for feature in numerical features.
+            You can get this dictionary from
+                >>> from teras.utils import get_features_metadata_for_embedding
+                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
 
-
-class FeatureTransformerBlock(layers.Layer):
-    """
-    Feature Transformer block layer is used in constructing the FeatureTransformer
-    as proposed by Sercan et al. in TabNet paper.
-    It applies a Dense layer followed by a BatchNormalization layer
-    followed by a GLU activation layer.
-
-    Reference(s):
-        https://arxiv.org/abs/1908.07442
-
-    Args:
-        units: `int`, default 32, the dimensionality of the hidden
-            representation in feature transformation block.
+        feature_transformer_dim: ``int``, default 32,
+            The dimensionality of the hidden representation in feature transformation block.
             Each layer first maps the representation to a `2 * feature_transformer_dim`
             output and half of it is used to determine the
             non-linearity of the GLU activation where the other half is used as an
             input to GLU, and eventually `feature_transformer_dim` output is
-            transferred to the next layer.        batch_momentum: Momentum value to use for BatchNormalization layer
-        batch_momentum: `float`, default 0.9, Momentum value to use for BatchNormalization layer.
-        virtual_batch_size: `int`, default 64, Batch size to use for `virtual_batch_size`
-            parameter in BatchNormalization layer.
-            This is typically much smaller than the `batch_size` used for training.
-        residual_normalization_factor: `float`, default 0.5, In the feature transformer, except for the
-            layer, every other layer utilizes normalized residuals, where `residual_normalization_factor`
-            determines the scale of normalization.
-        use_residual_normalization: `bool`, default True, Whether to use residual normalization.
-            According to the default architecture, every layer uses residual normalization EXCEPT
-            for the very first layer.
-    """
-    def __init__(self,
-                 units: int,
-                 batch_momentum: float = 0.9,
-                 virtual_batch_size: int = 64,
-                 residual_normalization_factor: float = 0.5,
-                 use_residual_normalization: bool = True,
-                 **kwargs):
-        super().__init__(**kwargs)
-        self.units = units
-        self.batch_momentum = batch_momentum
-        self.virtual_batch_size = virtual_batch_size
-        self.use_residual_normalization = use_residual_normalization
-        self.residual_normalization_factor = residual_normalization_factor
-        self.dense = layers.Dense(self.units * 2, use_bias=False)
-        self.norm = layers.BatchNormalization(momentum=self.batch_momentum,
-                                              virtual_batch_size=virtual_batch_size)
-
-        self.glu = GLU(self.units)
-        self.add = layers.Add()
-
-    def call(self, inputs):
-        x = self.dense(inputs)
-        x = self.norm(x)
-        x = self.glu(x)
-        if self.use_residual_normalization:
-            x = self.add([x, inputs]) * tf.math.sqrt(self.residual_normalization_factor)
-        return x
+            transferred to the next layer.
 
-    def get_config(self):
-        config = super().get_config()
-        new_config = {'units': self.units,
-                      'batch_momentum': self.batch_momentum,
-                      'virtual_batch_size': self.virtual_batch_size,
-                      'residual_normalization_factor': self.residual_normalization_factor,
-                      'use_residual_normalization': self.use_residual_normalization,
-                      }
-        config.update(new_config)
-        return config
+        decision_step_output_dim: ``int``, default 32,
+            The dimensionality of output at each decision step, which is later mapped to the
+            final classification or regression output.
+            It is recommended to keep ``decision_step_output_dim`` and ``feature_transformer_dim``
+            equal to each other.
+            Adjusting these two parameters values is a good way of obtaining a tradeoff between
+            performance and complexity.
 
+        num_decision_steps: ``int``, default 5,
+            The number of sequential decision steps.
+            For most datasets a value in the range [3, 10] is optimal.
+            If there are more informative features in the dataset, the value tends to
+            be higher. That said, a very high value of `num_decision_steps` may suffer
+            from overfitting.
 
-class FeatureTransformer(layers.Layer):
-    """
-    Feature Transformer as proposed by Sercan et al. in TabNet paper.
-    It is made up of FeatureTransformerBlock building blocks.
+        num_shared_layers: ``int``, default 2,
+            Number of shared layers to use in the ``TabNetFeatureTransformer``.
+            These shared layers are *shared* across decision steps.
+
+        num_decision_dependent_layers: ``int``, default 2,
+            Number of decision dependent layers to use in the ``TabNetFeatureTransformer``.
+            In simple words, ``num_decision_dependent_layers`` are created
+            for each decision step in the ``num_decision_steps``.
+            For instance, if ``num_decision_steps = `5` and  ``num_decision_dependent_layers = 2``
+            then 10 layers will be created, 2 for each decision step.
 
-    Reference(s):
-        https://arxiv.org/abs/1908.07442
+        relaxation_factor: ``float``, default 1.5,
+            Relaxation factor that promotes the reuse of each
+            feature at different decision steps. When it is 1, a feature is enforced
+            to be used only at one decision step and as it increases, more
+            flexibility is provided to use a feature at multiple decision steps.
+            An optimal value of relaxation_factor can have a major role on the performance.
+            Typically, a larger value for `num_decision_steps` favors for a larger ``relaxation_factor``.
 
-    Args:
-        units: `int`, default 32, the dimensionality of the hidden
-            representation in feature transformation block.
-            Each layer first maps the representation to a `2 * feature_transformer_dim`
-            output and half of it is used to determine the
-            non-linearity of the GLU activation where the other half is used as an
-            input to GLU, and eventually `feature_transformer_dim` output is
-            transferred to the next layer.
-        num_shared_layers: `int`, default 2. Number of shared layers to use in the Feature Transformer.
-            These shared layers are `shared` across decision steps.
-        num_decision_dependent_layers: `int`, default 2. Number of decision dependent layers to use in
-            the Feature Transformer. In simple words, `num_decision_dependent_layers` are created
-            for each decision step in the `num_decision_steps`.
-            For instance, if `num_decision_steps = 5` and  `num_decision_dependent_layers = 2`
-            then 10 layers will be created, 2 for each decision step.
-        batch_momentum: `float`, default 0.9, Momentum value to use for BatchNormalization layer.
-        virtual_batch_size: `int`, default 64, Batch size to use for `virtual_batch_size`
-            parameter in BatchNormalization layer.
-            This is typically much smaller than the `batch_size` used for training.
-        residual_normalization_factor: `float`, default 0.5, In the feature transformer, except for the
-            layer, every other layer utilizes normalized residuals, where `residual_normalization_factor`
+        batch_momentum: ``float``, default 0.9,
+            Momentum value to use for ``BatchNormalization`` layer.
+
+        virtual_batch_size: `int`, default 64,
+            Batch size to use for ``virtual_batch_size`` parameter in ``BatchNormalization`` layer.
+            This is typically much smaller than the ``batch_size`` used for training.
+
+        residual_normalization_factor: ``float``, default 0.5,
+            In the feature transformer, except for the first layer, every other layer utilizes
+            normalized residuals, where ``residual_normalization_factor``
             determines the scale of normalization.
-    """
-    shared_layers = None
 
+        epsilon: ``float``, default 0.00001,
+            Epsilon is a small number for numerical stability
+            during the computation of entropy loss.
+
+        encode_categorical_values: ``bool``, default True,
+            Whether to (label) encode categorical values,
+            If you've already encoded the categorical values using for instance
+            Label/Ordinal encoding, you should set this to False,
+            otherwise leave it as True.
+            In the case of True, categorical values will be mapped to integer indices
+            using keras's ``IntegerLookup`` layer.
+    """
     def __init__(self,
-                 units,
-                 num_shared_layers: int = 2,
-                 num_decision_dependent_layers: int = 2,
-                 batch_momentum: float = 0.9,
-                 virtual_batch_size: int = 64,
-                 residual_normalization_factor: float = 0.5,
+                 input_dim: int,
+                 features_metadata: dict,
+                 feature_transformer_dim: int = TabNetConfig.feature_transformer_dim,
+                 decision_step_output_dim: int = TabNetConfig.decision_step_output_dim,
+                 num_decision_steps: int = TabNetConfig.num_decision_steps,
+                 num_shared_layers: int = TabNetConfig.num_shared_layers,
+                 num_decision_dependent_layers: int = TabNetConfig.num_decision_dependent_layers,
+                 relaxation_factor: float = TabNetConfig.relaxation_factor,
+                 batch_momentum: float = TabNetConfig.batch_momentum,
+                 virtual_batch_size: int = TabNetConfig.virtual_batch_size,
+                 residual_normalization_factor: float = TabNetConfig.residual_normalization_factor,
+                 epsilon: float = TabNetConfig.epsilon,
+                 encode_categorical_values: bool = TabNetConfig.encode_categorical_features,
                  **kwargs):
-
-        if num_shared_layers == 0 and num_decision_dependent_layers == 0:
-            raise ValueError("Feature Transformer requires at least one of either shared or decision depenedent layers."
-                             " But both `num_shared_layers` and `num_decision_dependent_layers` were passed a 0 value.")
-
-        super().__init__(**kwargs)
-        self.units = units
+        categorical_feature_embedding = CategoricalFeatureEmbedding(features_metadata=features_metadata,
+                                                                     embedding_dim=1,
+                                                                     encode=encode_categorical_values)
+        encoder = TabNetEncoder(data_dim=input_dim,
+                                feature_transformer_dim=feature_transformer_dim,
+                                decision_step_output_dim=decision_step_output_dim,
+                                num_decision_steps=num_decision_steps,
+                                num_shared_layers=num_shared_layers,
+                                num_decision_dependent_layers=num_decision_dependent_layers,
+                                relaxation_factor=relaxation_factor,
+                                batch_momentum=batch_momentum,
+                                virtual_batch_size=virtual_batch_size,
+                                residual_normalization_factor=residual_normalization_factor,
+                                epsilon=epsilon)
+        super().__init__(input_dim=input_dim,
+                         features_metadata=features_metadata,
+                         categorical_feature_embedding=categorical_feature_embedding,
+                         encoder=encoder,
+                         **kwargs)
+        self.input_dim = input_dim
+        self.features_metadata = features_metadata
+        self.feature_transformer_dim = feature_transformer_dim
+        self.decision_step_output_dim = decision_step_output_dim
+        self.num_decision_steps = num_decision_steps
         self.num_shared_layers = num_shared_layers
         self.num_decision_dependent_layers = num_decision_dependent_layers
+        self.relaxation_factor = relaxation_factor
         self.batch_momentum = batch_momentum
         self.virtual_batch_size = virtual_batch_size
         self.residual_normalization_factor = residual_normalization_factor
-
-        # Since shared layers should be accessible across instances so we make them as class attributes
-        # and use class method to instantiate them, the first time an instance of this FeatureTransformer
-        # class is made.
-        if self.shared_layers is None and num_shared_layers > 0:
-            self._create_shared_layers(num_shared_layers,
-                                       units,
-                                       batch_momentum=batch_momentum,
-                                       virtual_batch_size=virtual_batch_size,
-                                       residual_normalization_factor=residual_normalization_factor)
-
-        self.inner_block = models.Sequential(name="inner_block")
-
-        self.inner_block.add(self.shared_layers)
-
-        if self.num_decision_dependent_layers > 0:
-            decision_dependent_layers = models.Sequential(name=f"decision_dependent_layers")
-            for j in range(self.num_decision_dependent_layers):
-                if j == 0 and self.num_shared_layers == 0:
-                    # then it means that this is the very first layer in the Feature Transformer
-                    # because no shard layers exist.
-                    # hence we shouldn't use residual normalization
-                    use_residual_normalization = False
-                else:
-                    use_residual_normalization = True
-                decision_dependent_layers.add(FeatureTransformerBlock(
-                    units=self.units,
-                    batch_momentum=self.batch_momentum,
-                    virtual_batch_size=self.virtual_batch_size,
-                    use_residual_normalization=use_residual_normalization,
-                    name=f"decision_dependent_layer_{j}")
-                )
-
-            self.inner_block.add(decision_dependent_layers)
-
-    @classmethod
-    def _create_shared_layers(cls, num_shared_layers, units, **kwargs):
-        # The outputs of first layer in feature transformer isn't residual normalized
-        # so we use a pointer to know which layer is first.
-        # Important to keep in mind that shared layers ALWAYS precede the decision dependent layers
-        # BUT we want to allow user to be able to use NO shared layers at all, i.e. 0.
-        # Hence, only if the `num_shared_layers` is 0, should the first dependent layer for each step
-        # be treated differently.
-        # Initialize the block of shared layers
-        cls.shared_layers = models.Sequential(name="shared_layers")
-        for i in range(num_shared_layers):
-            if i == 0:
-                # First layer should not use residual normalization
-                use_residual_normalization = False
-            else:
-                use_residual_normalization = True
-            cls.shared_layers.add(FeatureTransformerBlock(units=units,
-                                                          use_residual_normalization=use_residual_normalization,
-                                                          name=f"shared_layer_{i}",
-                                                          **kwargs))
-
-    def call(self, inputs):
-        outputs = self.inner_block(inputs)
-        return outputs
+        self.epsilon = epsilon
+        self.encode_categorical_values = encode_categorical_values
 
     def get_config(self):
-        config = super().get_config()
-        new_config = {'units': self.units,
-                      'num_shared_layers': self.num_shared_layers,
-                      'num_decision_dependent_layers': self.num_decision_dependent_layers,
-                      'batch_momentum': self.batch_momentum,
-                      'virtual_batch_size': self.virtual_batch_size,
-                      'residual_normalization_factor': self.residual_normalization_factor,
-                      }
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'input_dim': self.input_dim,
+                  'features_metadata': self.features_metadata,
+                  'feature_transformer_dim': self.feature_transformer_dim,
+                  'decision_step_output_dim': self.decision_step_output_dim,
+                  'num_decision_steps': self.num_decision_steps,
+                  'num_shared_layers': self.num_shared_layers,
+                  'num_decision_dependent_layers': self.num_decision_dependent_layers,
+                  'relaxation_factor': self.relaxation_factor,
+                  'batch_momentum': self.batch_momentum,
+                  'virtual_batch_size': self.virtual_batch_size,
+                  'residual_normalization_factor': self.residual_normalization_factor,
+                  'epsilon': self.epsilon,
+                  'encode_categorical_values': self.encode_categorical_values,
+                  }
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        features_metadata = config.pop("features_metadata")
+        return cls(input_dim=input_dim,
+                   features_metadata=features_metadata,
+                   **config)
+
 
-class Encoder(layers.Layer):
+@keras.saving.register_keras_serializable(package="keras.models")
+class TabNetClassifier(TabNet):
     """
-    Encoder as proposed by Sercan et al. in TabNet paper.
+    TabNet Classifier based on the TabNet architecture
+    as proposed by Sercan et al. in TabNet paper.
 
     Reference(s):
         https://arxiv.org/abs/1908.07442
 
     Args:
-        feature_transformer_dim: `int`, default 32, the dimensionality of the hidden
-            representation in feature transformation block.
+        num_classes: ``int``, default 2,
+            Number of classes to predict.
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default None,
+            Hidden units to use in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+            By default, no hidden layer is used.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the input dataset.
+
+        features_metadata: ``dict``,
+            A nested dictionary of metadata for features where
+            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
+            feature indices and the lists of unique values (vocabulary) in them,
+            while numerical dictionary is a mapping of numerical feature names to their indices.
+            ``{feature_name: (feature_idx, vocabulary)}`` for feature in categorical features.
+            ``{feature_name: feature_idx}`` for feature in numerical features.
+            You can get this dictionary from
+                >>> from teras.utils import get_features_metadata_for_embedding
+                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        feature_transformer_dim: ``int``, default 32,
+            The dimensionality of the hidden representation in feature transformation block.
             Each layer first maps the representation to a `2 * feature_transformer_dim`
             output and half of it is used to determine the
             non-linearity of the GLU activation where the other half is used as an
             input to GLU, and eventually `feature_transformer_dim` output is
             transferred to the next layer.
-        decision_step_output_dim: `int`, default 32, the dimensionality of output at each
-            decision step, which is later mapped to the final classification or regression output.
-            It is recommended to keep `decision_step_output_dim` and `feature_transformer_dim`
+
+        decision_step_output_dim: ``int``, default 32,
+            The dimensionality of output at each decision step, which is later mapped to the
+            final classification or regression output.
+            It is recommended to keep ``decision_step_output_dim`` and ``feature_transformer_dim``
             equal to each other.
             Adjusting these two parameters values is a good way of obtaining a tradeoff between
             performance and complexity.
-        num_decision_steps: `int`, default 5, the number of sequential decision steps.
+
+        num_decision_steps: ``int``, default 5,
+            The number of sequential decision steps.
             For most datasets a value in the range [3, 10] is optimal.
             If there are more informative features in the dataset, the value tends to
             be higher. That said, a very high value of `num_decision_steps` may suffer
             from overfitting.
-        num_shared_layers: `int`, default 2. Number of shared layers to use in the Feature Transformer.
-            These shared layers are `shared` across decision steps.
-        num_decision_dependent_layers: `int`, default 2. Number of decision dependent layers to use in
-            the Feature Transformer. In simple words, `num_decision_dependent_layers` are created
-            for each decision step in the `num_decision_steps`.
-            For instance, if `num_decision_steps = 5` and  `num_decision_dependent_layers = 2`
+
+        num_shared_layers: ``int``, default 2,
+            Number of shared layers to use in the ``TabNetFeatureTransformer``.
+            These shared layers are *shared* across decision steps.
+
+        num_decision_dependent_layers: ``int``, default 2,
+            Number of decision dependent layers to use in the ``TabNetFeatureTransformer``.
+            In simple words, ``num_decision_dependent_layers`` are created
+            for each decision step in the ``num_decision_steps``.
+            For instance, if ``num_decision_steps = `5` and  ``num_decision_dependent_layers = 2``
             then 10 layers will be created, 2 for each decision step.
-        relaxation_factor: `float`, default 1.5, Relaxation factor that promotes the reuse of each
+
+        relaxation_factor: ``float``, default 1.5,
+            Relaxation factor that promotes the reuse of each
             feature at different decision steps. When it is 1, a feature is enforced
             to be used only at one decision step and as it increases, more
             flexibility is provided to use a feature at multiple decision steps.
             An optimal value of relaxation_factor can have a major role on the performance.
-            Typically, a larger value for `num_decision_steps` favors for a larger `relaxation_factor`.
-        batch_momentum: `float`, default 0.9, Momentum value to use for BatchNormalization layer.
-        virtual_batch_size: `int`, default 64, Batch size to use for `virtual_batch_size`
-            parameter in BatchNormalization layer.
-            This is typically much smaller than the `batch_size` used for training.
-        residual_normalization_factor: `float`, default 0.5, In the feature transformer, except for the
-            layer, every other layer utilizes normalized residuals, where `residual_normalization_factor`
+            Typically, a larger value for `num_decision_steps` favors for a larger ``relaxation_factor``.
+
+        batch_momentum: ``float``, default 0.9,
+            Momentum value to use for ``BatchNormalization`` layer.
+
+        virtual_batch_size: `int`, default 64,
+            Batch size to use for ``virtual_batch_size`` parameter in ``BatchNormalization`` layer.
+            This is typically much smaller than the ``batch_size`` used for training.
+
+        residual_normalization_factor: ``float``, default 0.5,
+            In the feature transformer, except for the first layer, every other layer utilizes
+            normalized residuals, where ``residual_normalization_factor``
             determines the scale of normalization.
-        epsilon: `float`, default 0.00001, Epsilon is a small number for numerical stability
+
+        epsilon: ``float``, default 0.00001,
+            Epsilon is a small number for numerical stability
             during the computation of entropy loss.
-        num_features: `int`, Number of features in the dataset.
+
+        encode_categorical_values: ``bool``, default True,
+            Whether to (label) encode categorical values,
+            If you've already encoded the categorical values using for instance
+            Label/Ordinal encoding, you should set this to False,
+            otherwise leave it as True.
+            In the case of True, categorical values will be mapped to integer indices
+            using keras's ``IntegerLookup`` layer.
     """
     def __init__(self,
-                 feature_transformer_dim: int = 32,
-                 decision_step_output_dim: int = 32,
-                 num_decision_steps: int = 5,
-                 num_shared_layers: int = 2,
-                 num_decision_dependent_layers: int = 2,
-                 relaxation_factor: float = 1.5,
-                 batch_momentum: float = 0.9,
-                 virtual_batch_size: int = 64,
-                 residual_normalization_factor: float = 0.5,
-                 epsilon=1e-5,
-                 num_features: int = None,
+                 num_classes: int = 2,
+                 head_units_values: UnitsValuesType = None,
+                 input_dim: int = None,
+                 features_metadata: dict = None,
+                 feature_transformer_dim: int = TabNetConfig.feature_transformer_dim,
+                 decision_step_output_dim: int = TabNetConfig.decision_step_output_dim,
+                 num_decision_steps: int = TabNetConfig.num_decision_steps,
+                 num_shared_layers: int = TabNetConfig.num_shared_layers,
+                 num_decision_dependent_layers: int = TabNetConfig.num_decision_dependent_layers,
+                 relaxation_factor: float = TabNetConfig.relaxation_factor,
+                 batch_momentum: float = TabNetConfig.batch_momentum,
+                 virtual_batch_size: int = TabNetConfig.virtual_batch_size,
+                 residual_normalization_factor: float = TabNetConfig.residual_normalization_factor,
+                 epsilon: float = TabNetConfig.epsilon,
+                 encode_categorical_values: bool = TabNetConfig.encode_categorical_features,
                  **kwargs):
-        super().__init__(**kwargs)
-        self.feature_transformer_dim = feature_transformer_dim
-        self.decision_step_output_dim = decision_step_output_dim
-        self.num_shared_layers = num_shared_layers
-        self.num_decision_dependent_layers = num_decision_dependent_layers
-        self.num_decision_steps = num_decision_steps
-        self.relaxation_factor = relaxation_factor
-        self.batch_momentum = batch_momentum
-        self.virtual_batch_size = virtual_batch_size
-        self.residual_normalization_factor = residual_normalization_factor
-        self.epsilon = epsilon
-        self.num_features = num_features
-
-        self.inputs_norm = layers.BatchNormalization(momentum=batch_momentum)
-
-        self.features_transformers_per_step = [FeatureTransformer(
-            units=self.feature_transformer_dim,
-            num_shared_layers=self.num_shared_layers,
-            num_decision_dependent_layers=self.num_decision_dependent_layers,
-            batch_momentum=self.batch_momentum,
-            virtual_batch_size=self.virtual_batch_size,
-            residual_normalization_factor=self.residual_normalization_factor,
-            name=f"step_{i}_feature_transformer"
-        )
-            for i in range(self.num_decision_steps)
-        ]
-
-        # Attentive transformer -- used for creating mask
-        # We initialize this layer in the build method here
-        # since we need to know the num_features for its initialization
-        self.attentive_transformers_per_step = [AttentiveTransformer(num_features=self.num_features,
-                                                                     batch_momentum=self.batch_momentum,
-                                                                     virtual_batch_size=self.virtual_batch_size,
-                                                                     relaxation_factor=self.relaxation_factor,
-                                                                     name=f"step_{i}_attentive_transformer")
-                                                for i in range(self.num_decision_steps)
-                                                ]
-
-        self.feature_importances_per_sample = []
-        self.relu = layers.ReLU()
-
-    def call(self, inputs, mask=None):
-        batch_size = tf.shape(inputs)[0]
-        # Initializes decision-step dependent variables
-        outputs_aggregated = tf.zeros(shape=(batch_size, self.decision_step_output_dim))
-        # we only pass mask alongside inputs when we're pretaining
-        # As the paper says in the Self-Supervised section, we  initialize
-        # mask_values (P) to be 1-S during pretraining.
-        # we create this S in the TabNetPretrainer class and pass it from there
-        if mask is not None:
-            mask_values = mask
-        else:
-            mask_values = tf.zeros(shape=tf.shape(inputs))
-        # Aggregated mask values are used for explaining feature importance
-        # Here we'll refer to them as feature_importances_per_sample since
-        # that's a more descriptive name
-        # For more details, read the `Interpretability` section on page 5
-        # of the paper "TabNet: Attentive Interpretable Tabular Learning"
-        feature_importances_per_sample = tf.zeros(shape=tf.shape(inputs))
-        total_entropy = 0.
-
-        # Prior scales `P` indicate how much a particular feature has been used previously
-        # P[i] = ((Pi)j=1 to i)(gamma (gamma - M[j])
-        # where `Pi` is the Product Greek letter
-        # gamma is the relaxation factor, when gamma = 1, a feature is enforced,
-        # to be used only at one decision step and as gamma increases, more
-        # flexibility is provided to use a feature at multiple decision steps.
-        # P[0] is initialized as all ones, `1`B×D, without any prior
-        # on the masked features.
-        prior_scales = tf.ones(tf.shape(inputs))
-
-        normalized_inputs = self.inputs_norm(inputs)
-        masked_features = normalized_inputs
-
-        for step_num in range(self.num_decision_steps):
-            # Feature transformer with two shared and two decision step dependent
-            # blocks is used below
-            x = self.features_transformers_per_step[step_num](masked_features)
-
-            if step_num > 0 or self.num_decision_steps == 1:
-                decision_step_outputs = self.relu(x[:, :self.decision_step_output_dim])
-                # Decision aggregation.
-                outputs_aggregated += decision_step_outputs
-                # Aggregated masks are used for visualization of the
-                # feature importance attributes.
-                scale_agg = tf.reduce_sum(decision_step_outputs,
-                                          axis=1,
-                                          keepdims=True)
-
-                # To prevent division by zero, we introduce this conditional
-                # and only divide by (num_decision_steps - 1) if num_decision_steps > 1
-                if self.num_decision_steps > 1:
-                    scale_agg = scale_agg / tf.cast(self.num_decision_steps - 1, tf.float32)
-
-                feature_importances_per_sample += (mask_values * scale_agg)
-                self.feature_importances_per_sample.append(feature_importances_per_sample)
-
-            features_for_attentive_transformer = (x[:, self.decision_step_output_dim:])
-
-            if step_num < self.num_decision_steps - 1:
-                # Determines the feature masks via linear and nonlinear
-                # transformations, taking into account of aggregated feature use
-                mask_values = self.attentive_transformers_per_step[step_num](features_for_attentive_transformer,
-                                                                             prior_scales=prior_scales)
-                # Relaxation factor controls the amount of reuse of features between
-                # different decision blocks and updated with the values of coefficients
-                prior_scales *= (self.relaxation_factor - mask_values)
-
-                # Entropy is used to penalize the amount of sparsity in feature selection
-                total_entropy += tf.reduce_mean(
-                    tf.reduce_sum(-mask_values * tf.math.log(mask_values + self.epsilon), axis=1)
-                ) / (self.num_decision_steps - 1)
-                entropy_loss = total_entropy
-
-                # Feature Selection
-                masked_features = tf.multiply(mask_values, normalized_inputs)
-            else:
-                entropy_loss = 0.
-
-        # Add entropy loss
-        self.add_loss(entropy_loss)
-
-        return outputs_aggregated
+        head = ClassificationHead(num_classes=num_classes,
+                                  units_values=head_units_values,
+                                  name="tabnet_classification_head")
+        super().__init__(input_dim=input_dim,
+                         features_metadata=features_metadata,
+                         feature_transformer_dim=feature_transformer_dim,
+                         decision_step_output_dim=decision_step_output_dim,
+                         num_decision_steps=num_decision_steps,
+                         num_shared_layers=num_shared_layers,
+                         num_decision_dependent_layers=num_decision_dependent_layers,
+                         relaxation_factor=relaxation_factor,
+                         batch_momentum=batch_momentum,
+                         virtual_batch_size=virtual_batch_size,
+                         residual_normalization_factor=residual_normalization_factor,
+                         epsilon=epsilon,
+                         encode_categorical_values=encode_categorical_values,
+                         head=head,
+                         **kwargs)
+        self.num_classes = num_classes
+        self.head_units_values = head_units_values
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'feature_transformer_dim': self.feature_transformer_dim,
-                      'decision_step_output_dim': self.decision_step_output_dim,
-                      'num_decision_steps': self.num_decision_steps,
-                      'num_shared_layers': self.num_shared_layers,
-                      'num_decision_dependent_layers': self.num_decision_dependent_layers,
-                      'relaxation_factor': self.relaxation_factor,
-                      'batch_momentum': self.batch_momentum,
-                      'virtual_batch_size': self.virtual_batch_size,
-                      'residual_normalization_factor': self.residual_normalization_factor,
-                      'epsilon': self.epsilon,
-                      'num_features': self.num_features,
-                      }
-        config.update(new_config)
+        config.update({'num_classes': self.num_classes,
+                       'head_units_values': self.head_units_values
+                       })
         return config
 
 
-class Decoder(layers.Layer):
+@keras.saving.register_keras_serializable(package="keras.models")
+class TabNetRegressor(TabNet):
     """
-    Decoder as proposed by Sercan et al. in TabNet paper.
+    TabNet Regressor based on the TabNet architecture
+    as proposed by Sercan et al. in TabNet paper.
 
     Reference(s):
         https://arxiv.org/abs/1908.07442
 
     Args:
-        data_dim: Dimensionality of the original dataset - or the total number of
-            features in the original dataset.
-        feature_transformer_dim: `int`, default 32, the dimensionality of the hidden
-            representation in feature transformation block.
+        num_outputs: ``int``, default 1,
+            Number of regression outputs.
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default None,
+            Hidden units to use in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+            By default, no hidden layer is used.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the input dataset.
+
+        features_metadata: ``dict``,
+            A nested dictionary of metadata for features where
+            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
+            feature indices and the lists of unique values (vocabulary) in them,
+            while numerical dictionary is a mapping of numerical feature names to their indices.
+            ``{feature_name: (feature_idx, vocabulary)}`` for feature in categorical features.
+            ``{feature_name: feature_idx}`` for feature in numerical features.
+            You can get this dictionary from
+                >>> from teras.utils import get_features_metadata_for_embedding
+                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        feature_transformer_dim: ``int``, default 32,
+            The dimensionality of the hidden representation in feature transformation block.
             Each layer first maps the representation to a `2 * feature_transformer_dim`
             output and half of it is used to determine the
             non-linearity of the GLU activation where the other half is used as an
             input to GLU, and eventually `feature_transformer_dim` output is
             transferred to the next layer.
-        decision_step_output_dim: `int`, default 32, the dimensionality of output at each
-            decision step, which is later mapped to the final classification or regression output.
-            It is recommended to keep `decision_step_output_dim` and `feature_transformer_dim`
+
+        decision_step_output_dim: ``int``, default 32,
+            The dimensionality of output at each decision step, which is later mapped to the
+            final classification or regression output.
+            It is recommended to keep ``decision_step_output_dim`` and ``feature_transformer_dim``
             equal to each other.
             Adjusting these two parameters values is a good way of obtaining a tradeoff between
             performance and complexity.
-        num_decision_steps: `int`, default 5, the number of sequential decision steps.
+
+        num_decision_steps: ``int``, default 5,
+            The number of sequential decision steps.
             For most datasets a value in the range [3, 10] is optimal.
             If there are more informative features in the dataset, the value tends to
             be higher. That said, a very high value of `num_decision_steps` may suffer
             from overfitting.
-        num_shared_layers: `int`, default 2. Number of shared layers to use in the Feature Transformer.
-            These shared layers are `shared` across decision steps.
-        num_decision_dependent_layers: `int`, default 2. Number of decision dependent layers to use in
-            the Feature Transformer. In simple words, `num_decision_dependent_layers` are created
-            for each decision step in the `num_decision_steps`.
-            For instance, if `num_decision_steps = 5` and  `num_decision_dependent_layers = 2`
+
+        num_shared_layers: ``int``, default 2,
+            Number of shared layers to use in the ``TabNetFeatureTransformer``.
+            These shared layers are *shared* across decision steps.
+
+        num_decision_dependent_layers: ``int``, default 2,
+            Number of decision dependent layers to use in the ``TabNetFeatureTransformer``.
+            In simple words, ``num_decision_dependent_layers`` are created
+            for each decision step in the ``num_decision_steps``.
+            For instance, if ``num_decision_steps = `5` and  ``num_decision_dependent_layers = 2``
             then 10 layers will be created, 2 for each decision step.
-        batch_momentum: `float`, default 0.9, Momentum value to use for BatchNormalization layer.
-        virtual_batch_size: `int`, default 64, Batch size to use for `virtual_batch_size`
-            parameter in BatchNormalization layer.
-            This is typically much smaller than the `batch_size` used for training.
-        residual_normalization_factor: `float`, default 0.5, In the feature transformer, except for the
-            layer, every other layer utilizes normalized residuals, where `residual_normalization_factor`
+
+        relaxation_factor: ``float``, default 1.5,
+            Relaxation factor that promotes the reuse of each
+            feature at different decision steps. When it is 1, a feature is enforced
+            to be used only at one decision step and as it increases, more
+            flexibility is provided to use a feature at multiple decision steps.
+            An optimal value of relaxation_factor can have a major role on the performance.
+            Typically, a larger value for `num_decision_steps` favors for a larger ``relaxation_factor``.
+
+        batch_momentum: ``float``, default 0.9,
+            Momentum value to use for ``BatchNormalization`` layer.
+
+        virtual_batch_size: `int`, default 64,
+            Batch size to use for ``virtual_batch_size`` parameter in ``BatchNormalization`` layer.
+            This is typically much smaller than the ``batch_size`` used for training.
+
+        residual_normalization_factor: ``float``, default 0.5,
+            In the feature transformer, except for the first layer, every other layer utilizes
+            normalized residuals, where ``residual_normalization_factor``
             determines the scale of normalization.
+
+        epsilon: ``float``, default 0.00001,
+            Epsilon is a small number for numerical stability
+            during the computation of entropy loss.
+
+        encode_categorical_values: ``bool``, default True,
+            Whether to (label) encode categorical values,
+            If you've already encoded the categorical values using for instance
+            Label/Ordinal encoding, you should set this to False,
+            otherwise leave it as True.
+            In the case of True, categorical values will be mapped to integer indices
+            using keras's ``IntegerLookup`` layer.
     """
     def __init__(self,
-                 data_dim: int,
-                 feature_transformer_dim: int = 32,
-                 decision_step_output_dim: int = 32,
-                 num_decision_steps: int = 5,
-                 num_shared_layers: int = 2,
-                 num_decision_dependent_layers: int = 2,
-                 batch_momentum: float = 0.9,
-                 virtual_batch_size: int = 64,
-                 residual_normalization_factor: float = 0.5,
+                 num_outputs=1,
+                 head_units_values: UnitsValuesType = None,
+                 input_dim: int = None,
+                 features_metadata: dict = None,
+                 feature_transformer_dim: int = TabNetConfig.feature_transformer_dim,
+                 decision_step_output_dim: int = TabNetConfig.decision_step_output_dim,
+                 num_decision_steps: int = TabNetConfig.num_decision_steps,
+                 num_shared_layers: int = TabNetConfig.num_shared_layers,
+                 num_decision_dependent_layers: int = TabNetConfig.num_decision_dependent_layers,
+                 relaxation_factor: float = TabNetConfig.relaxation_factor,
+                 batch_momentum: float = TabNetConfig.batch_momentum,
+                 virtual_batch_size: int = TabNetConfig.virtual_batch_size,
+                 residual_normalization_factor: float = TabNetConfig.residual_normalization_factor,
+                 epsilon: float = TabNetConfig.epsilon,
+                 encode_categorical_values: bool = TabNetConfig.encode_categorical_features,
                  **kwargs):
-        super().__init__(**kwargs)
-        self.data_dim = data_dim
-        self.feature_transformer_dim = feature_transformer_dim
-        self.decision_step_output_dim = decision_step_output_dim
-        self.num_shared_layers = num_shared_layers
-        self.num_decision_dependent_layers = num_decision_dependent_layers
-        self.num_decision_steps = num_decision_steps
-        self.batch_momentum = batch_momentum
-        self.virtual_batch_size = virtual_batch_size
-        self.residual_normalization_factor = residual_normalization_factor
-
-        self.features_transformers_per_step = []
-        self.projection_layers_per_step = []
-
-        # OKAY LISTEN: To be able to share the `shared_layers` across instances, we introduced
-        # a class attribute called `shared_layers` in the FeatureTransformer class BUT here's the problem,
-        # even though we now want to create shared layers separately for our Decoder, it won't ... unless...
-        # we do this
-        FeatureTransformer.shared_layers = None
-        # Why? Because each time we create FeatureTransformer instance, it first checks if `shared_layers`
-        # attribute is None or not, if it's None it will create new shared layers, otherwise it won't.
-
-        for i in range(self.num_decision_steps):
-            self.features_transformers_per_step.append(FeatureTransformer(
-                                                        units=self.feature_transformer_dim,
-                                                        num_shared_layers=self.num_shared_layers,
-                                                        num_decision_dependent_layers=self.num_decision_dependent_layers,
-                                                        batch_momentum=self.batch_momentum,
-                                                        virtual_batch_size=self.virtual_batch_size,
-                                                        residual_normalization_factor=self.residual_normalization_factor,
-                                                        name=f"step_{i}_feature_transformer"
-                                                        ))
-            self.projection_layers_per_step.append(layers.Dense(self.data_dim))
-
-    def call(self, inputs, mask=None):
-        """
-        Args:
-            inputs: Encoded representations.
-
-        Returns:
-
-        """
-        batch_size = tf.shape(inputs)[0]
-        reconstructed_features = tf.zeros(shape=(batch_size, self.data_dim))
-
-        for i in range(self.num_decision_steps):
-            feat_output = self.features_transformers_per_step[i](inputs)
-            reconstructed_features += self.projection_layers_per_step[i](feat_output)
-
-        # The paper says,
-        # the decoder’s last FC (dense) layer is multiplied with S (binary mask indicating which features are missing)
-        # to output the unknown features.
-        if mask is not None:
-            reconstructed_features *= mask
-
-        return reconstructed_features
+        head = RegressionHead(num_outputs=num_outputs,
+                              units_values=head_units_values,
+                              name="tabnet_regression_head")
+        super().__init__(input_dim=input_dim,
+                         features_metadata=features_metadata,
+                         feature_transformer_dim=feature_transformer_dim,
+                         decision_step_output_dim=decision_step_output_dim,
+                         num_decision_steps=num_decision_steps,
+                         num_shared_layers=num_shared_layers,
+                         num_decision_dependent_layers=num_decision_dependent_layers,
+                         relaxation_factor=relaxation_factor,
+                         batch_momentum=batch_momentum,
+                         virtual_batch_size=virtual_batch_size,
+                         residual_normalization_factor=residual_normalization_factor,
+                         epsilon=epsilon,
+                         encode_categorical_values=encode_categorical_values,
+                         head=head,
+                         **kwargs)
+        self.num_outputs = num_outputs
+        self.head_units_values = head_units_values
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'data_dim': self.data_dim,
-                      'feature_transformer_dim': self.feature_transformer_dim,
-                      'decision_step_output_dim': self.decision_step_output_dim,
-                      'num_decision_steps': self.num_decision_steps,
-                      'num_shared_layers': self.num_shared_layers,
-                      'num_decision_dependent_layers': self.num_decision_dependent_layers,
-                      'batch_momentum': self.batch_momentum,
-                      'virtual_batch_size': self.virtual_batch_size,
-                      'residual_normalization_factor': self.residual_normalization_factor,
-                      }
-        config.update(new_config)
+        config.update({'num_outputs': self.num_outputs,
+                       'head_units_values': self.head_units_values
+                       })
         return config
 
 
-class RegressionHead(BaseRegressionHead):
+@keras.saving.register_keras_serializable(package="keras.models")
+class TabNetPretrainer(_TabNetPretrainerLF):
     """
-    Regression head for the TabNet Regressor architecture.
+    TabNetPretrainer model based on the architecture
+    proposed by Sercan et al. in TabNet paper.
+
+    TabNetPretrainer is an encoder-decoder model based on the TabNet architecture,
+    where the TabNet model acts as an encoder while a separate decoder
+    is used to reconstruct the input features.
+
+    Reference(s):
+        https://arxiv.org/abs/1908.07442
 
     Args:
-        num_outputs: `int`, default 1,
-            Number of regression outputs to predict.
-        units_values: `List[int] | Tuple[int]`, default `None`,
-            If specified, for each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the RegressionHead.
-        activation_hidden: default `None`,
-            Activation function to use in hidden dense layers.
-        normalization: `Layer | str`, default `None`,
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
-    """
-    def __init__(self,
-                 num_outputs: int = 1,
-                 units_values: LIST_OR_TUPLE = None,
-                 activation_hidden=None,
-                 normalization: LAYER_OR_STR = None,
-                 **kwargs):
-        super().__init__(num_outputs=num_outputs,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         normalization=normalization,
-                         **kwargs)
+        model: ``TabNet``,
+            An instance of `TabNet` class to pretrain.
 
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the input dataset.
+
+        features_metadata: ``dict``,
+            A nested dictionary of metadata for features where
+            categorical sub-dictionary is a mapping of categorical feature names to a tuple of
+            feature indices and the lists of unique values (vocabulary) in them,
+            while numerical dictionary is a mapping of numerical feature names to their indices.
+            ``{feature_name: (feature_idx, vocabulary)}`` for feature in categorical features.
+            ``{feature_name: feature_idx}`` for feature in numerical features.
+            You can get this dictionary from
+                >>> from teras.utils import get_features_metadata_for_embedding
+                >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        missing_feature_probability: ``float``, default 3,
+            Fraction of features to randomly mask i.e. make them missing.
+            Missing features are introduced in the pretraining dataset and
+            the probability of missing features is controlled by the parameter.
+            The pretraining objective is to predict values for these missing features,
+            (pre)training the ``TabNet`` model in the process.
+
+        decoder_feature_transformer_dim: ``int``, default 32,
+            Feature transformer dimensions for ``TabNetDecoder``.
+
+        decoder_decision_step_output_dim: ``int``, default 32,
+            Decision step output dimensions for ``TabNetDecoder``.
 
-class ClassificationHead(BaseClassificationHead):
-    """
-    Classification head for TabNet Classifier model.
+        decoder_num_decision_steps: ``int``, default 5,
+            Number of decision steps to use in ``TabNetDecoder``.
 
-    Args:
-        num_classes: `int`, default 2,
-            Number of classes to predict.
-        units_values: `List[int] | Tuple[int]`, default `None`,
-            If specified, for each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the ClassificationHead.
-        activation_hidden: default `None`,
-            Activation function to use in hidden dense layers.
-        activation_out: default `None`,
-            Activation function to use for the output layer.
-            If not specified, `sigmoid` is used for binary and `softmax` is used for
-            multiclass classification.
-        normalization: `Layer | str`, default `None`,
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
+        decoder_num_shared_layers: ``int``, default 2,
+            Number of shared layers in ``TabNetFeatureTransformer`` in ``TabNetDecoder``.
+
+        decoder_num_decision_dependent_layers: ``int``, default 2,
+            Number of decision dependent layers in ``TabNetFeatureTransformer`` layer in ``TabNetDecoder``.
     """
     def __init__(self,
-                 num_classes: int = 2,
-                 units_values: LIST_OR_TUPLE = None,
-                 activation_hidden=None,
-                 activation_out=None,
-                 normalization: LAYER_OR_STR = None,
+                 model: TabNet,
+                 input_dim: int = None,
+                 features_metadata: dict = None,
+                 missing_feature_probability: float = 0.3,
+                 decoder_feature_transformer_dim: int = TabNetConfig.feature_transformer_dim,
+                 decoder_decision_step_output_dim: int = TabNetConfig.decision_step_output_dim,
+                 decoder_num_decision_steps: int = TabNetConfig.num_decision_steps,
+                 decoder_num_shared_layers: int = TabNetConfig.num_shared_layers,
+                 decoder_num_decision_dependent_layers: int = TabNetConfig.num_decision_dependent_layers,
                  **kwargs):
-        super().__init__(num_classes=num_classes,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         activation_out=activation_out,
-                         normalization=normalization,
+        decoder = TabNetDecoder(data_dim=input_dim,
+                                feature_transformer_dim=decoder_feature_transformer_dim,
+                                decision_step_output_dim=decoder_decision_step_output_dim,
+                                num_decision_steps=decoder_num_decision_steps,
+                                num_shared_layers=decoder_num_shared_layers,
+                                num_decision_dependent_layers=decoder_num_shared_layers)
+        super().__init__(model=model,
+                         features_metadata=features_metadata,
+                         decoder=decoder,
+                         missing_feature_probability=missing_feature_probability,
                          **kwargs)
+        self.model = model
+        self.input_dim = input_dim
+        self.features_metadata = features_metadata
+        self.missing_feature_probability = missing_feature_probability
+        self.decoder_feature_transformer_dim = decoder_feature_transformer_dim
+        self.decoder_decision_step_output_dim = decoder_decision_step_output_dim
+        self.decoder_num_decision_steps = decoder_num_decision_steps
+        self.decoder_num_shared_layers = decoder_num_shared_layers
+        self.decoder_num_decision_dependent_layers = decoder_num_decision_dependent_layers
+
+    def get_config(self):
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'model': keras.layers.serialize(self.model),
+                  'input_dim': self.input_dim,
+                  'features_metadata': self.features_metadata,
+                  'missing_feature_probability': self.missing_feature_probability,
+                  'decoder_feature_transformer_dim': self.decoder_feature_transformer_dim,
+                  'decoder_decision_step_output_dim': self.decoder_decision_step_output_dim,
+                  'decoder_num_decision_steps': self.decoder_num_decision_steps,
+                  'decoder_num_shared_layers': self.decoder_num_shared_layers,
+                  'decoder_num_decision_dependent_layers': self.decoder_num_decision_dependent_layers,
+                  }
+        return config
+
+    @classmethod
+    def from_config(cls, config):
+        model = keras.layers.deserialize(config.pop("model"))
+        return cls(model=model, **config)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Teras-0.1.1/teras/layers/tabtransformer.py` & `Teras-0.2.0/teras/layerflow/layers/saint/saint_transformer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,102 @@
-import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from teras.layers.common.head import (ClassificationHead as BaseClassificationHead,
-                                      RegressionHead as BaseRegressionHead)
-from typing import Union, List, Tuple
 
 
-LIST_OR_TUPLE = Union[List[int], Tuple[int]]
-LAYER_OR_STR = Union[keras.layers.Layer, str]
-
-
-class ColumnEmbedding(layers.Layer):
+@keras.saving.register_keras_serializable(package="teras.layerflow.layers.saint")
+class SAINTTransformer(keras.layers.Layer):
     """
-    ColumnEmbedding layer as proposed by Xin Huang et al. in the paper
-    TabTransformer: Tabular Data Modeling Using Contextual Embeddings.
+    SAINT Transformer layer with LayerFlow design.
+    It is part of the SAINT architecture,
+    which is proposed by Gowthami Somepalli et al.
+    in the paper SAINT: Improved Neural Networks for Tabular Data
+    via Row Attention and Contrastive Pre-Training.
+    It differs from the usual Transformer (L) block in that it contains additional
+    ``MultiHeadInterSampleAttention`` layer in addition to the usual
+    ``MultiHeadAttention`` layer.
 
     Reference(s):
-        https://arxiv.org/abs/2012.06678
+        https://arxiv.org/abs/2106.01342
 
     Args:
-        num_categorical_features: `int`,
-            Number of categorical features in the dataset.
-        embedding_dim: `int`, default 32,
-            Dimensionality of the embedded features
+        multi_head_inter_sample_attention: ``keras.layers.Layer``,
+            An instance of ``MultiHeadInterSampleAttention`` layer or any other custom
+            layer that can work in its place.
+            You can import this layer as follows,
+                >>> from teras.layers import MultiHeadInterSampleAttention
+
+        feed_forward: ``keras.layers.Layer``,
+            An instance of ``FeedForward`` layer or any custom layer that can work
+            in its place.
+            You can import this layer as follows,
+                >>> from teras.layerflow.layers import FeedForward
+
+        transformer: ``keras.layers.Layer``,
+            An instance of the regular ``Transformer`` layer, or any custom layer
+            that can work in its place.
+            You can import this layer as follows,
+                >>> from teras.layerflow.layers import Transformer
     """
     def __init__(self,
-                 num_categorical_features: int,
-                 embedding_dim=32,
+                 multi_head_inter_sample_attention: keras.layers.Layer,
+                 feed_forward: keras.layers.Layer,
+                 transformer: keras.layers.Layer,
                  **kwargs):
         super().__init__(**kwargs)
-        self.embedding_dim = embedding_dim
-        self.num_categorical_features = num_categorical_features
-        self.column_embedding = keras.layers.Embedding(input_dim=self.num_categorical_features,
-                                                       output_dim=self.embedding_dim)
-        self.column_indices = tf.range(start=0,
-                                       limit=self.num_categorical_features,
-                                       delta=1)
-        self.column_indices = tf.cast(self.column_indices, dtype="float32")
+        self.multi_head_inter_sample_attention = multi_head_inter_sample_attention
+        self.feed_forward = feed_forward
+        self.transformer = transformer
+
+    def build(self, input_shape):
+        # We build the inner SAINT Transformer block using keras Functional API
+        # and since we need the input dimensions that's why we're building it in the build method.
+
+        # Inter Sample Attention Block: this attention is applied to rows.
+        inputs = keras.layers.Input(shape=tuple(input_shape[1:]))
+        intermediate_outputs = inputs
+        if self.apply_attention_to_rows:
+            residual = inputs
+            x = self.multi_head_inter_sample_attention(inputs)
+            x = keras.layers.Add()([x, residual])
+            x = keras.layers.LayerNormalization()(x)
+            residual = x
+            x = self.feed_forward(x)
+            x = keras.layers.Add()([x, residual])
+            intermediate_outputs = keras.layers.LayerNormalization()(x)
+            final_outputs = intermediate_outputs
+
+        # MultiHeadAttention block: this attention is applied to columns
+        if self.apply_attention_to_features:
+            # If `apply_attention_to_features` is set to True,
+            # then attention will be applied to columns/features
+            # The MultiHeadInterSampleAttention appollection)lies attention over rows,
+            # but the regular MultiHeadAttention layer is used to apply attention over features.
+            # Since the common Transformer layer applies MutliHeadAttention over features
+            # as well as takes care of applying all the preceding and following layers,
+            # so we'll just use that here.
+            final_outputs = self.transformer(intermediate_outputs)
+
+        self.transformer_block = keras.Model(inputs=inputs,
+                                             outputs=final_outputs,
+                                             name="saint_inner_transformer_block")
 
     def call(self, inputs):
-        """
-        Args:
-            inputs: Embeddings of categorical features encoded by CategoricalFeatureEmbedding layer
-        """
-        return inputs + self.column_embedding(self.column_indices)
+        outputs = self.transformer_block(inputs)
+        return outputs
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_categorical_features': self.num_categorical_features,
-                      'embedding_dim': self.embedding_dim,
+        new_config = {'multi_head_inter_sample_attention': keras.layers.serialize(self.multi_head_inter_sample_attention),
+                      'feed_forward': keras.layers.serialize(self.feed_forward),
+                      'transformer': keras.layers.serialize(self.transformer),
                       }
         config.update(new_config)
         return config
 
-
-class ClassificationHead(BaseClassificationHead):
-    """
-    Classification head for the TabTransformer Classifier architecture.
-
-    Args:
-        num_classes: `int`, default 2,
-            Number of classes to predict.
-        units_values: `List[int] | Tuple[int]`, default (64, 32),
-            For each value in the sequence,
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the ClassificationHead.
-        activation_hidden: default "relu",
-            Activation function to use in hidden dense layers.
-        activation_out:
-            Activation function to use for the output layer.
-            If not specified, `sigmoid` is used for binary and `softmax` is used for
-            multiclass classification.
-        normalization: `Layer | str`, default "batch",
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
-    """
-    def __init__(self,
-                 num_classes: int = 2,
-                 units_values: LIST_OR_TUPLE = (64, 32),
-                 activation_hidden="relu",
-                 activation_out=None,
-                 normalization: LAYER_OR_STR = "batch",
-                 **kwargs):
-        super().__init__(num_classes=num_classes,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         activation_out=activation_out,
-                         normalization=normalization,
-                         **kwargs)
-
-
-class RegressionHead(BaseRegressionHead):
-    """
-    Regression head for the TabTransformer Regressor architecture.
-
-    Args:
-        num_outputs: `int`, default 1,
-            Number of regression outputs to predict.
-        units_values: `List[int] | Tuple[int]`, default (64, 32),
-            For each value in the sequence
-            a hidden layer of that dimension preceded by a normalization layer (if specified) is
-            added to the RegressionHead.
-        activation_hidden: default "relu",
-            Activation function to use in hidden dense layers.
-        normalization: `Layer | str`, default "batch",
-            Normalization layer to use.
-            If specified a normalization layer is applied after each hidden layer.
-            If None, no normalization layer is applied.
-            You can either pass a keras normalization layer or name for a layer implemented by keras.
-    """
-    def __init__(self,
-                 num_outputs: int = 1,
-                 units_values: LIST_OR_TUPLE = (64, 32),
-                 activation_hidden="relu",
-                 normalization: LAYER_OR_STR = "batch",
-                 **kwargs):
-        super().__init__(num_outputs=num_outputs,
-                         units_values=units_values,
-                         activation_hidden=activation_hidden,
-                         normalization=normalization,
-                         **kwargs)
+    @classmethod
+    def from_config(cls, config):
+        multi_head_inter_sample_attention = keras.layers.deserialize(config.pop("multi_head_inter_sample_attention"))
+        feed_forward = keras.layers.deserialize(config.pop("feed_forward"))
+        transformer = keras.layers.deserialize(config.pop("transformer"))
+        return cls(multi_head_inter_sample_attention=multi_head_inter_sample_attention,
+                   feed_forward=feed_forward,
+                   transformer=transformer,
+                   **config)
```

### Comparing `Teras-0.1.1/teras/losses/__init__.py` & `Teras-0.2.0/teras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/losses/ctgan.py` & `Teras-0.2.0/teras/losses/ctgan.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tensorflow import keras
 
 
 def generator_loss(generated_samples,
                    y_generated,
                    cond_vectors=None,
                    mask=None,
-                   meta_data=None):
+                   metadata=None):
     """
     Loss for the Generator model in the CTGAN architecture.
 
     CTGAN is a state-of-the-art tabular data generation architecture
     proposed by Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
@@ -19,27 +19,27 @@
 
     Args:
         generated_samples: Samples drawn from the input dataset
         y_generated: Discriminator's output for the generated samples
         cond_vectors: Conditional vectors that are used for and with
             generated samples
         mask: Mask created during the conditional vectors generation step
-        meta_data: Namedtuple meta deta of features.
+        metadata: Namedtuple meta deta of features.
             That meta data contains miscellaneous information about features,
             which is calculated during data transformation step.
 
     Returns:
         Generator's loss.
     """
     loss = []
     cross_entropy_loss = keras.losses.SparseCategoricalCrossentropy(from_logits=True,
                                                                     reduction=keras.losses.Reduction.NONE)
-    numerical_features_relative_indices = meta_data.numerical.relative_indices_all
-    features_relative_indices_all = meta_data.relative_indices_all
-    num_categories_all = meta_data.categorical.num_categories_all
+    numerical_features_relative_indices = metadata["numerical"]["relative_indices_all"]
+    features_relative_indices_all = metadata["relative_indices_all"]
+    num_categories_all = metadata["categorical"]["num_categories_all"]
     # the first k features in the data are numerical which we'll ignore as we're only
     # concerned with the categorical features here
     offset = len(numerical_features_relative_indices)
     for i, index in enumerate(features_relative_indices_all[offset:]):
         logits = generated_samples[:, index: index + num_categories_all[i]]
         temp_cond_vector = cond_vectors[:, i: i + num_categories_all[i]]
         labels = tf.argmax(temp_cond_vector, axis=1)
```

### Comparing `Teras-0.1.1/teras/losses/gain.py` & `Teras-0.2.0/teras/losses/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/losses/pcgain.py` & `Teras-0.2.0/teras/losses/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/losses/saint.py` & `Teras-0.2.0/teras/losses/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/losses/tabnet.py` & `Teras-0.2.0/teras/losses/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/losses/tvae.py` & `Teras-0.2.0/teras/losses/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/losses/vime.py` & `Teras-0.2.0/teras/losses/vime.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/models/ctgan.py` & `Teras-0.2.0/teras/models/ctgan.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,106 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import models
-from tensorflow.keras import optimizers
-from teras.layers.ctgan import GeneratorBlock, DiscriminatorBlock
-from teras.layers.activations import GumbelSoftmax
-from teras.losses.ctgan import generator_loss, discriminator_loss
-from typing import List, Union, Tuple
-from tqdm import tqdm
+from teras.layers.ctgan.ctgan_generator_block import CTGANGeneratorBlock
+from teras.layers.ctgan.ctgan_discriminator_block import CTGANDiscriminatorBlock
+from teras.layerflow.models.ctgan import CTGAN as _CTGAN_LF
+from teras.layers.activation import GumbelSoftmax
+from teras.utils.types import UnitsValuesType
 
 
-LIST_OR_TUPLE = Union[List[int], Tuple[int]]
-HIDDEN_BLOCK_TYPE = Union[keras.layers.Layer, keras.models.Model]
-
-
-class Generator(keras.Model):
+@keras.saving.register_keras_serializable(package="teras.models")
+class CTGANGenerator(keras.Model):
     """
-    Generator for CTGAN architecture as proposed by
+    CTGANGenerator for CTGAN architecture as proposed by
     Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        units_values: default [256, 256],
-            A list or tuple of units.
-            For each value, a `GeneratorBlock`
-            (`from teras.layers.ctgan import GeneratorBlock`)
-            of that dimensionality (units) is added to the generator
-            to form the `hidden block` of the generator.
-        data_dim: `int`,
+        data_dim: ``int``,
             The dimensionality of the dataset.
             It will also be the dimensionality of the output produced
             by the generator.
+
             Note the dimensionality must be equal to the dimensionality of dataset
             that is passed to the fit method and not necessarily the dimensionality
             of the raw input dataset as sometimes data transformation alters the
             dimensionality of the dataset.
-        meta_data: `dict`,
-            The Generator in CTGAN architecture,
-            applies different activation functions to the output of Generator,
-            depending on the type of features.
-            And to determine the feature types and for other computation during
-            activation step, the `meta data` computed during the data transformation step,
+
+            You can access the dimensionailty of the transformed dataset throught the
+            ``.data_dim`` attribute of the ``CTGANDataSampler`` instance used in sampling
+            the dataset.
+
+        metadata: ``dict``,
+            The ``CTGANGeneratorBlock``, applies different activation functions
+            to its outputs depending on the type of features (categorical or numerical).
+            And to determine the feature types and for other computations during the
+            activation step, the ``metadata`` computed during the data transformation step,
             is required.
-            It can be accessed through the `.get_meta_data()` method of the DataTransformer
+
+            It can be accessed through the ``.get_metadata()`` method of the ``CTGANDataTransformer``
             instance which was used to transform the raw input data.
-            It must NOT be None.
+
+            Note that, this is NOT the same metadata as ``features_metadata``, which is computed
+            using the ``get_features_metadata_for_embedding`` utility function from ``teras.utils``.
+            You must use the ``.get_metadata()`` method of the ``CTGANDataTransformer`` to access it.
+
+            You can import the ``CTGANDataTransformer`` as follows,
+                >>> from teras.preprocessing import CTGANDataTransformer
+
+        units_values: ``List[int]`` or ``Tuple[int]``, default [256, 256],
+            A list or tuple of units.
+            For each value, a ```CTGANGeneratorBlock``` of that
+            dimensionality (units) is added to the ``CTGANGeneratorBlock``
+            to form its ``hidden block``.
+            You can access the ``CTGANGeneratorBlock`` as follows,
+                >>> from teras.layers import CTGANGeneratorBlock
     """
     def __init__(self,
-                 units_values: LIST_OR_TUPLE = (256, 256),
-                 data_dim: int = None,
-                 meta_data: dict = None,
+                 data_dim: int,
+                 metadata: dict = None,
+                 units_values: UnitsValuesType = (256, 256),
                  **kwargs):
         super().__init__(**kwargs)
 
         if not isinstance(units_values, (list, tuple)):
             raise ValueError(f"""`units_values` must be a list or tuple of units which determines
                         the number of Generator residual blocks and the dimensionality of those blocks.
-                        But {units_values} was passed.""")
-
-        if data_dim is None:
-            raise ValueError(f"""`data_dim` cannot be None.
-                    You must pass the value for `data_dim`, which can be accessed through `.data_dim`
-                    attribute of DataSampler instance if you don't know the data dimensions.""")
-
-        if meta_data is None:
-            raise ValueError(f"""`meta_data`, which is computed during the data transformation step,
-                    is required by the Generator to apply relevant activation functions to the 
-                    output of the Generator. But {meta_data} was passed.
-                    Please pass the meta data by accessing it through the `.get_meta_data()` method
-                    of the DataTransformer instance which was used to transform the raw input data.
-                    """)
+                        Received: {type(units_values)}""")
 
+        if metadata is None:
+            raise ValueError(f"""`metadata` cannot be None.
+                `metadata`, which is computed during the data transformation step,
+                is required by the `CTGANGenerator` to apply relevant activation functions to the 
+                output of the Generator. But received `None`.\n
+                Please pass the metadata by accessing it through the `.get_metadata()` method
+                of the `CTGANDataTransformer` instance which was used to transform the raw input data.
+                """)
         self.data_dim = data_dim
-        self.meta_data = meta_data
+        self.metadata = metadata
         self.units_values = units_values
 
-        self.hidden_block = models.Sequential(name="generator_hidden_block")
+        self.hidden_block = keras.models.Sequential(name="generator_hidden_block")
         for units in self.units_values:
-            self.hidden_block.add(GeneratorBlock(units))
-
-        self.output_layer = layers.Dense(self.data_dim, name="generator_output_layer")
-
+            self.hidden_block.add(CTGANGeneratorBlock(units))
+        self.output_layer = keras.layers.Dense(self.data_dim, name="generator_output_layer")
         self.gumbel_softmax = GumbelSoftmax()
 
     def apply_activations_by_feature_type(self, interim_outputs):
         """
         This function applies activation functions to the interim outputs of
         the Generator by feature type.
         As CTGAN architecture requires specific transformations on the raw input data,
         that decompose one feature in several features,
         and since each type of feature, i.e. numerical or categorical require
         different activation functions to be applied, the process of applying those
         activations becomes rather tricky as it requires knowledge of underlying
-        data transformation and features meta data.
+        data transformation and features metadata.
         To ease the user's burden, in case a user wants to subclass this
         Generator model and completely customize the inner workings of the generator
         but would want to use the activation method specific to the CTGAN architecture,
         so that the subclassed Generator can work seamlessly with the rest of the
         architecture and there won't be any discrepancies in outputs produced by
         the subclasses Generator and those expected by the architecture,
         this function is separated, so user can just call this function on the interim
@@ -108,20 +109,20 @@
         Args:
             interim_outputs: Outputs produced by the `output_layer` of the Generator.
 
         Returns:
             Final outputs activated by the relevant activation functions.
         """
         outputs = []
-        numerical_features_relative_indices = self.meta_data.numerical.relative_indices_all
-        features_relative_indices_all = self.meta_data.relative_indices_all
-        num_valid_clusters_all = self.meta_data.numerical.num_valid_clusters_all
+        numerical_features_relative_indices = self.metadata["numerical"]["relative_indices_all"]
+        features_relative_indices_all = self.metadata["relative_indices_all"]
+        num_valid_clusters_all = self.metadata["numerical"]["num_valid_clusters_all"]
         cont_i = 0
         cat_i = 0
-        num_categories_all = self.meta_data.categorical.num_categories_all
+        num_categories_all = self.metadata["categorical"]["num_categories_all"]
         for i, index in enumerate(features_relative_indices_all):
             # the first k = num_numerical_features are numerical in the data
             if i < len(numerical_features_relative_indices):
                 # each numerical features has been transformed into num_valid_clusters + 1 features
                 # where the first feature is alpha while the following features are beta components
                 alphas = tf.nn.tanh(interim_outputs[:, index])
                 alphas = tf.expand_dims(alphas, 1)
@@ -144,92 +145,103 @@
         # while the outputs will have the shape of equal to (batch_size, transformed_data_dims)
         interim_outputs = self.output_layer(self.hidden_block(inputs))
         outputs = self.apply_activations_by_feature_type(interim_outputs)
         return outputs
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'units_values': self.units_values,
-                      'data_dim': self.data_dim,
-                      'meta_data': self.meta_data}
-        config.update(new_config)
+        config.update({'data_dim': self.data_dim,
+                       'units_values': self.units_values,
+                       'metadata': self.metadata}
+                      )
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        data_dim = config.pop("data_dim")
+        return cls(data_dim=data_dim,
+                   **config)
 
-class Discriminator(keras.Model):
+
+@keras.saving.register_keras_serializable(package="teras.models")
+class CTGANDiscriminator(keras.Model):
     """
-    Discriminator for CTGAN architecture as proposed by
+    CTGANDiscriminator for CTGAN architecture as proposed by
     Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        units_values: default [256, 256],
+        units_values: ``List[int]`` or ``Tuple[int]``, default [256, 256],
             A list or tuple of units.
-            For each value, a `DiscriminatorBlock`
-            (`from teras.layers.ctgan import DiscriminatorBlock`)
+            For each value, a ```CTGANDiscriminatorBlock```
             of that dimensionality (units) is added to the discriminator
             to form the `hidden block` of the discriminator.
-        packing_degree: `int`, default 8,
+
+            You can import the ``CTGANDiscriminatorBlock`` as follows,
+                >>> from teras.layers import CTGANDiscriminatorBlock
+
+        packing_degree: ``int``, default 8,
             Packing degree - taken from the PacGAN paper.
             The number of samples concatenated or "packed" together.
             It must be a factor of the batch_size.
             Packing degree is borrowed from the PacGAN [Diederik P. Kingma et al.] architecture,
             which proposes passing `m` samples at once to discriminator instead of `1` to be
             jointly classified as real or fake by the discriminator in order to tackle the
             issue of mode collapse inherent in the GAN based architectures.
             The number of samples passed jointly `m`, is termed as the `packing degree`.
-        gradient_penalty_lambda: `float`, default 10,
+
+        gradient_penalty_lambda: ``float``, default 10,
                 Controls the strength of gradient penalty.
                 lambda value is directly proportional to the strength of gradient penalty.
                 Gradient penalty penalizes the discriminator for large weights in an attempt
                 to combat Discriminator becoming too confident and overfitting.
 
     Example:
         ```python
         # Instantiate Generator
-        generator = Generator(data_dim=data_dim,
-                              meta_data=meta_data)
+        generator = CTGANGenerator(data_dim=data_dim,
+                                   metadata=metadata)
 
         # Instantiate Discriminator
-        discriminator = Discriminator()
+        discriminator = CTGANDiscriminator()
 
         # Sample noise to generate samples from
         z = tf.random.normal([512, 18])
 
         # Generate samples
         generated_samples = generator(z)
 
         # Predict using discriminator
         y_pred = discriminator(generated_samples)
         ```
     """
     def __init__(self,
-                 units_values: LIST_OR_TUPLE = (256, 256),
+                 units_values: UnitsValuesType = (256, 256),
                  packing_degree: int = 8,
                  gradient_penalty_lambda: float = 10,
                  **kwargs):
         super().__init__(**kwargs)
 
         if not isinstance(units_values, (list, tuple)):
             raise ValueError(f"""`units_values` must be a list or tuple of units which determines
                         the number of Discriminator blocks and the dimensionality of those blocks.
                         But {units_values} was passed""")
 
         self.units_values = units_values
         self.packing_degree = packing_degree
         self.gradient_penalty_lambda = gradient_penalty_lambda
 
-        self.hidden_block = models.Sequential(name="discriminator_hidden_block")
+        self.hidden_block = keras.models.Sequential(name="discriminator_hidden_block")
         for units in self.units_values:
-            self.hidden_block.add(DiscriminatorBlock(units))
+            self.hidden_block.add(CTGANDiscriminatorBlock(units))
 
-        self.output_layer = layers.Dense(1, name="discriminator_output_layer")
+        self.output_layer = keras.layers.Dense(1, name="discriminator_output_layer")
 
     @tf.function
     def gradient_penalty(self,
                          real_samples,
                          generated_samples):
         """
         Calculates the gradient penalty as proposed
@@ -275,252 +287,135 @@
         new_config = {'units_values': self.units_values,
                       'packing_degree': self.packing_degree,
                       'gradient_penalty_lambda': self.gradient_penalty_lambda}
         config.update(new_config)
         return config
 
 
-class CTGAN(keras.Model):
+@keras.saving.register_keras_serializable(package="teras.models")
+class CTGAN(_CTGAN_LF):
     """
     CTGAN is a state-of-the-art tabular data generation architecture
     proposed by Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        data_dim: `int`,
+        input_dim: ``int``,
             The dimensionality of the input dataset.
+
             Note the dimensionality must be equal to the dimensionality of dataset
             that is passed to the fit method and not necessarily the dimensionality
             of the raw input dataset as sometimes data transformation alters the
             dimensionality of the dataset.
-        meta_data: `dict`,
-            Simply pass the result of `.get_meta_data()` method of the DataTransformer instance
+
+            You can access the dimensionailty of the transformed dataset throught the
+            ``.data_dim`` attribute of the ``CTGANDataSampler`` instance used in sampling
+            the dataset.
+
+        metadata: ``dict``,
+            A dictionary of metadata computed during the data transformation step.
+            Simply pass the result of ``.get_metadata()`` method of the ``CTGANDataTransformer`` instance
             which was used to transform the raw input data.
-            The Generator in CTGAN architecture applies different activation functions
+            The Generator in ``CTGAN`` architecture applies different activation functions
             to the output of Generator, depending on the type of features.
             And to determine the feature types and for other computation during
-            activation step, the `meta data` computed during the data transformation step,
+            activation step, the ``metadata`` computed during the data transformation step,
             is required.
             It is also required during the computation of generator loss.
             Hence, it cannot be None.
-            It can be accessed through the `.get_meta_data()` method of the DataTransformer
-            instance which was used to transform the raw input data.
-        generator_units_values: `List[int]` or `Tuple[int]`, default [256, 256],
+
+        generator_units_values: ``List[int]`` or ``Tuple[int]``, default [256, 256],
             A list or tuple of units.
-            For each value, a `CTGANGeneratorBlock`
-            (`from teras.layers import CTGANGeneratorBlock`)
+            For each value, a ``CTGANGeneratorBlock``
             of that dimensionality (units) is added to the generator
-            to form the `hidden block` of the generator.
-        discriminator_units_values: `List[int]` or `Tuple[int]`, default [256, 256],
+            to form the ``hidden block`` of the generator.
+            You can import the ``CTGANGeneratorBlock`` as follows,
+                >>> from teras.layers import CTGANGeneratorBlock
+
+        discriminator_units_values: ``List[int]`` or ``Tuple[int]``, default [256, 256],
             A list or tuple of units values.
-            For each value, a `CTGANDiscriminatorBlock`
-            (`from teras.layers import CTGANDiscriminatorBlock`)
+            For each value, a ``CTGANDiscriminatorBlock``
             of that dimensionality (units) is added to the discriminator
-            to form the `hidden block` of the discriminator.
-        num_discriminator_steps: `int`, default 1,
-            Number of discriminator training steps per CTGAN training step.
-        latent_dim: `int`, default 128,
+            to form the ``hidden block`` of the discriminator.
+            You can import the ``CTGANDiscriminatorBlock`` as follows,
+                >>> from teras.layers import CTGANDiscriminatorBlock
+
+        num_discriminator_steps: ``int``, default 1,
+            Number of discriminator training steps per ``CTGAN`` training step.
+
+        latent_dim: ``int``, default 128,
             Dimensionality of noise or `z` that serves as input to Generator
             to generate samples.
-        packing_degree: `int`, default 8,
+
+        packing_degree: ``int``, default 8,
             Packing degree - taken from the PacGAN paper.
             The number of samples concatenated or "packed" together.
             It must be a factor of the batch_size.
             Packing degree is borrowed from the PacGAN [Diederik P. Kingma et al.] architecture,
-            which proposes passing `m` samples at once to discriminator instead of `1` to be
+            which proposes passing ``m`` samples at once to discriminator instead of ``1`` to be
             jointly classified as real or fake by the discriminator in order to tackle the
             issue of mode collapse inherent in the GAN based architectures.
-            The number of samples passed jointly `m`, is termed as the `packing degree`.
-        gradient_penalty_lambda: `float`, default 10,
-            Controls the strength of gradient penalty in the Discriminator.
+            The number of samples passed jointly ``m``, is termed as the ``packing degree``.
+
+        gradient_penalty_lambda: ``float``, default 10,
+            Controls the strength of gradient penalty in the ``CTGANDiscriminator``.
             lambda value is directly proportional to the strength of gradient penalty.
             Gradient penalty penalizes the discriminator for large weights in an attempt
             to combat Discriminator becoming too confident and overfitting.
     """
     def __init__(self,
-                 data_dim: int = None,
-                 meta_data: dict = None,
-                 generator_units_values: LIST_OR_TUPLE = (256, 256),
-                 discriminator_units_values: LIST_OR_TUPLE = (256, 256),
+                 input_dim: int,
+                 metadata: dict = None,
+                 generator_units_values: UnitsValuesType = (256, 256),
+                 discriminator_units_values: UnitsValuesType = (256, 256),
                  num_discriminator_steps: int = 1,
                  latent_dim: int = 128,
-                 packing_degree: int =8,
+                 packing_degree: int = 8,
                  gradient_penalty_lambda: float = 10,
                  **kwargs):
-        super().__init__(**kwargs)
-
-        if data_dim is None:
-            raise ValueError(f"""`data_dim` is required to instantiate the Generator.
-                    But {data_dim} was passed.
-                    You must pass the value for `data_dim`, which can be accessed through `.data_dim`
-                    attribute of DataSampler instance if you don't know the data dimensions.""")
-        if meta_data is None:
-            raise ValueError("`meta_data` cannot be None. "
-                             "You can access the `meta_data` through `.get_meta_data()` method of DataTransformer "
+        if metadata is None:
+            raise ValueError("`metadata` cannot be None. "
+                             "You can access the `metadata` through `.get_metadata()` method of `CTGANDataTransformer` "
                              "instance.")
-        self.data_dim = data_dim
-        self.meta_data = meta_data
+        generator = CTGANGenerator(data_dim=input_dim,
+                                   metadata=metadata,
+                                   units_values=generator_units_values)
+
+        discriminator = CTGANDiscriminator(units_values=discriminator_units_values,
+                                           packing_degree=packing_degree,
+                                           gradient_penalty_lambda=gradient_penalty_lambda)
+        super().__init__(generator=generator,
+                         discriminator=discriminator,
+                         num_discriminator_steps=num_discriminator_steps,
+                         latent_dim=latent_dim,
+                         **kwargs)
+        self.input_dim = input_dim
+        self.metadata = metadata
         self.generator_units_values = generator_units_values
         self.discriminator_units_values = discriminator_units_values
         self.num_discriminator_steps = num_discriminator_steps
         self.latent_dim = latent_dim
         self.packing_degree = packing_degree
         self.gradient_penalty_lambda = gradient_penalty_lambda
 
-        self.generator = Generator(data_dim=self.data_dim,
-                                   meta_data=self.meta_data,
-                                   units_values=self.generator_units_values)
-
-        self.discriminator = Discriminator(units_values=self.discriminator_units_values,
-                                           packing_degree=self.packing_degree,
-                                           gradient_penalty_lambda=self.gradient_penalty_lambda)
-
-        # Loss trackers
-        self.generator_loss_tracker = keras.metrics.Mean(name="generator_loss")
-        self.discriminator_loss_tracker = keras.metrics.Mean(name="discriminator_loss")
-
-    def compile(self,
-                generator_optimizer=optimizers.Adam(learning_rate=1e-3,
-                                                    beta_1=0.5, beta_2=0.9),
-                discriminator_optimizer=optimizers.Adam(learning_rate=1e-3,
-                                                        beta_1=0.5, beta_2=0.9),
-                generator_loss=generator_loss,
-                discriminator_loss=discriminator_loss,
-                ):
-        super().compile()
-        self.generator_optimizer = generator_optimizer
-        self.discriminator_optimizer = discriminator_optimizer
-        self.generator_loss = generator_loss
-        self.discriminator_loss = discriminator_loss
-
-    def call(self, inputs):
-        generated_samples = self.generator(inputs)
-        return generated_samples
-
-    def train_step(self, data):
-        # real_samples, shuffled_idx, random_features_indices, random_values_indices = data
-        real_samples, cond_vectors_real, cond_vectors, mask = data
-        self.batch_size = tf.shape(real_samples)[0]
-
-        for _ in range(self.num_discriminator_steps):
-            z = tf.random.normal(shape=[self.batch_size, self.latent_dim])
-            # cond_vector, mask = self.data_sampler.sample_cond_vector_for_training(self.batch_size,
-            #                                                                       random_features_indices=random_features_indices,
-            #                                                                       random_values_indices=random_values_indices)
-            input_gen = tf.concat([z, cond_vectors], axis=1)
-            generated_samples = self.generator(input_gen, training=False)
-            # cond_vector_2 = tf.gather(cond_vector, indices=tf.cast(shuffled_idx, tf.int32))
-            generated_samples = tf.concat([generated_samples, cond_vectors], axis=1)
-            real_samples = tf.concat([real_samples, cond_vectors_real], axis=1)
-
-            with tf.GradientTape(persistent=True) as tape:
-                y_generated = self.discriminator(generated_samples)
-                y_real = self.discriminator(real_samples)
-                grad_pen = self.discriminator.gradient_penalty(real_samples, generated_samples)
-                loss_disc = self.discriminator_loss(y_real, y_generated)
-            gradients_pen = tape.gradient(grad_pen, self.discriminator.trainable_weights)
-            gradients_loss = tape.gradient(loss_disc, self.discriminator.trainable_weights)
-            self.discriminator_optimizer.apply_gradients(zip(gradients_pen, self.discriminator.trainable_weights))
-            self.discriminator_optimizer.apply_gradients(zip(gradients_loss, self.discriminator.trainable_weights))
-
-        z = tf.random.normal(shape=[self.batch_size, self.latent_dim])
-        # cond_vector, mask = self.data_sampler.sample_cond_vector_for_training(self.batch_size,
-        #                                                                       random_features_indices=random_features_indices,
-        #                                                                       random_values_indices=random_values_indices)
-        # Practically speaking, we don't really need the partial function,
-        # but it makes things look more neat
-        # generator_partial_loss_fn = partial(generator_loss, mask=mask, meta_data=self.meta_data)
-        input_gen = tf.concat([z, cond_vectors], axis=1)
-        with tf.GradientTape() as tape:
-            tape.watch(cond_vectors)
-            tape.watch(mask)
-            # generated_samples, y_generated = self(input_gen, cond_vector=cond_vector)
-            generated_samples = self(input_gen)
-            generated_samples = tf.concat([generated_samples, cond_vectors], axis=1)
-            y_generated = self.discriminator(generated_samples, training=False)
-            loss_gen = self.generator_loss(generated_samples, y_generated,
-                                           cond_vectors=cond_vectors, mask=mask,
-                                           meta_data=self.meta_data)
-            # dummy_targets = tf.zeros(shape=(self.batch_size,))
-            # loss_gen_dummy = self.generator.compiled_loss(dummy_targets, loss_gen)
-        gradients = tape.gradient(loss_gen, self.generator.trainable_weights)
-        self.generator_optimizer.apply_gradients(zip(gradients, self.generator.trainable_weights))
-
-        self.generator_loss_tracker.update_state(loss_gen)
-        self.discriminator_loss_tracker.update_state(loss_disc)
-
-        results = {m.name: m.result() for m in self.metrics}
-        generator_results = {'generator_' + m.name: m.result() for m in self.generator.metrics}
-        results.update(generator_results)
-        discriminator_results = {'discriminator_' + m.name: m.result() for m in self.discriminator.metrics}
-        results.update(discriminator_results)
-        return results
-
-    def generate(self,
-                 num_samples: int,
-                 data_sampler,
-                 data_transformer=None,
-                 reverse_transform: bool = True,
-                 batch_size: int = None):
-        """
-        Generates new samples using the trained generator.
-
-        Args:
-            num_samples: Number of new samples to generate
-            data_sampler: Instance of the DataSampler class used in preparing
-                the tensorflow dataset for training.
-            data_transformer: Instance of DataTransformer class used to preprocess
-                the raw data.
-                This is required only if the `reverse_transform` is set to True.
-            reverse_transform: bool, default True,
-                whether to reverse transform the generated data to the original data format.
-                If False, the raw generated data will be returned, which you can then manually
-                transform into original data format by utilizing DataTransformer instance's
-                `reverse_transform` method.
-            batch_size: int, default None.
-                If a value is passed, samples will be generated in batches
-                where `batch_size` determines the size of each batch.
-                If `None`, all `num_samples` will be generated at once.
-                Note that, if the number of samples to generate aren't huge
-                or you know your hardware can handle to generate all samples at once,
-                you can leave the value to None, otherwise it is recommended to specify
-                a value for batch size.
-        """
-        if batch_size is None:
-            batch_size = num_samples
-        num_steps = num_samples // batch_size
-        num_steps += 1 if num_samples % batch_size != 0 else 0
-        generated_samples = []
-        for _ in tqdm(range(num_steps), desc="Generating Data"):
-            z = tf.random.normal(shape=[batch_size, self.latent_dim])
-            cond_vector = data_sampler.sample_cond_vectors_for_generation(batch_size)
-            input_gen = tf.concat([z, cond_vector], axis=1)
-            generated_samples.append(self.generator(input_gen, training=False))
-        generated_samples = tf.concat(generated_samples, axis=0)
-        generated_samples = generated_samples[:num_samples]
-
-        if reverse_transform:
-            if data_transformer is None:
-                raise ValueError("""To reverse transform the raw generated data, `data_transformer` must not be None.
-                             Please pass the instance of DataTransformer class used to transform the input
-                             data. Or alternatively, you can set `reverse_transform` to False, and later
-                             manually reverse transform the generated raw data to original format.""")
-            generated_samples = data_transformer.reverse_transform(x_generated=generated_samples)
-
-        return generated_samples
-
     def get_config(self):
-        config = super().get_config()
-        new_config = {'data_dim': self.data_dim,
-                      'meta_data': self.meta_data,
-                      'generator_units_values': self.generator_units_values,
-                      'discriminator_units_values': self.discriminator_units_values,
-                      'num_discriminator_steps': self.num_discriminator_steps,
-                      'latent_dim': self.latent_dim,
-                      'packing_degree': self.packing_degree,
-                      'gradient_penalty_lambda': self.gradient_penalty_lambda,
-                      }
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'input_dim': self.input_dim,
+                  'metadata': self.metadata,
+                  'generator_units_values': self.generator_units_values,
+                  'discriminator_units_values': self.discriminator_units_values,
+                  'num_discriminator_steps': self.num_discriminator_steps,
+                  'latent_dim': self.latent_dim,
+                  'packing_degree': self.packing_degree,
+                  'gradient_penalty_lambda': self.gradient_penalty_lambda,
+                  }
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        return cls(input_dim=input_dim,
+                   **config)
```

### Comparing `Teras-0.1.1/teras/models/dnfnet.py` & `Teras-0.2.0/teras/models/dnfnet.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,242 +1,305 @@
-from tensorflow.keras import layers, models
-from teras.layers import DNNF, DNFNetClassificationHead, DNFNetRegressionHead
-from typing import List
+from tensorflow import keras
+from teras.layers.dnfnet.dnnf import DNNF
+from teras.utils.types import (IntegerSequence,
+                               FloatSequence,
+                               UnitsValuesType)
+from teras.layers.common.head import (ClassificationHead,
+                                      RegressionHead)
+from teras.layerflow.models.dnfnet import DNFNet as _DNFNetLF
 
-LIST_OF_INT = List[int]
-LIST_OF_FLOAT = List[float]
 
-
-class DNFNet(models.Model):
+@keras.saving.register_keras_serializable(package="teras.models")
+class DNFNet(_DNFNetLF):
     """
     DNFNet model based on the DNFNet architecture,
     proposed by Liran Katzir et al.
     in the paper,
     "NET-DNF: Effective Deep Modeling Of Tabular Data."
 
     Reference(s):
         https://openreview.net/forum?id=73WTGs96kho
 
     Args:
-        num_dnnf_layers: `int`, default 1,
-            Number of DNNF layers to use in the model
-        num_formulas: `int`, default 256,
-            Number of DNF formulas to use in each DNNF layer.
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        num_dnnf_layers: ``int``, default 1,
+            Number of ``DNNF`` layers to use in the model
+
+        num_formulas: ``int``, default 256,
+            Number of DNF formulas to use in each ``DNNF`` layer.
             Each DNF formula is analogous to a tree in tree based ensembles.
-        num_conjunctions_arr: `List[int]`, default [6, 9, 12, 15],
+
+        num_conjunctions_arr: ``List[int]`` or ``Tuple[int]``, default [6, 9, 12, 15],
             Conjunctions array to use in each DNNF layer.
             It is used in the computation of total number of literals as well as
             computation of number of literals per DNF formula.
-        conjunctions_depth_arr: `List[int]`, default [2, 4, 6],
-            Conjunctions depth array to use in each DNNF layer.
+
+        conjunctions_depth_arr: ``List[int]`` or ``Tuple[int]``, default [2, 4, 6],
+            Conjunctions depth array to use in each ``DNNF`` layer.
             It is used in the computation of total number of literals as well as
             computation of number of literals per DNF formula.
-        keep_feature_prob_arr: `List[float]`, default [0.1, 0.3, 0.5, 0.7, 0.9],
-            Feature probability array to use in each DNNF layer.
+
+        keep_feature_prob_arr: ``List[float]`` or ``Tuple[float]``, default [0.1, 0.3, 0.5, 0.7, 0.9],
+            Feature probability array to use in each ``DNNF`` layer.
             It is used by the Feature Selection layer to randomly select a probability
             value that is used in the random selection of input features.
-        elastic_net_beta: `float`, default 0.4,
-            Used in the computation of Elastic Net Regularization in the DNNF layer.
-        binary_threshold_eps:   `float`, default 1.0,
-            Used in the computation of learnable mask in the DNNF layer.
-        temperature: `float`, default 2.0,
-            Temperature value to use in the Localization layer.
+
+        elastic_net_beta: ``float``, default 0.4,
+            Used in the computation of Elastic Net Regularization in the ``DNNF`` layer.
+
+        binary_threshold_eps: ``float``, default 1.0,
+            Used in the computation of learnable mask in the ``DNNF`` layer.
+
+        temperature: ``float``, default 2.0,
+            Temperature value to use in the ``Localization`` layer.
             According to the paper, The inclusion of an adaptive temperature in this localization mechanism
             facilitates a data-dependent degree of exclusivity:
             at high temperatures, only a few DNNFs will handle an input instance whereas
             at low temperatures, more DNNFs will effectively participate in the ensemble.
     """
     def __init__(self,
+                 input_dim: int,
                  num_dnnf_layers: int = 1,
                  num_formulas: int = 2048,
-                 num_conjunctions_arr: LIST_OF_INT = [6, 9, 12, 15],
-                 conjunctions_depth_arr: LIST_OF_INT = [2, 4, 6],
-                 keep_feature_prob_arr: LIST_OF_FLOAT = [0.1, 0.3, 0.5, 0.7, 0.9],
+                 num_conjunctions_arr: IntegerSequence = [6, 9, 12, 15],
+                 conjunctions_depth_arr: IntegerSequence = [2, 4, 6],
+                 keep_feature_prob_arr: FloatSequence = [0.1, 0.3, 0.5, 0.7, 0.9],
                  elastic_net_beta: float = 0.4,
                  binary_threshold_eps: float = 1.0,
                  temperature: float = 2.0,
                  **kwargs):
-        super().__init__(**kwargs)
+        dnnf_layers = keras.models.Sequential(name="dnnf_layers")
+        for _ in range(num_dnnf_layers):
+            dnnf_layers.add(DNNF(num_formulas=num_formulas,
+                                 num_conjunctions_arr=num_conjunctions_arr,
+                                 conjunctions_depth_arr=conjunctions_depth_arr,
+                                 keep_feature_prob_arr=keep_feature_prob_arr,
+                                 elastic_net_beta=elastic_net_beta,
+                                 binary_threshold_eps=binary_threshold_eps,
+                                 temperature=temperature))
+        super().__init__(input_dim=input_dim,
+                         dnnf_layers=dnnf_layers,
+                         **kwargs)
+        self.input_dim = input_dim
         self.num_dnnf_layers = num_dnnf_layers
         self.num_formulas = num_formulas
         self.num_conjunctions_arr = num_conjunctions_arr
         self.conjunctions_depth_arr = conjunctions_depth_arr
         self.keep_feature_prob_arr = keep_feature_prob_arr
         self.elastic_net_beta = elastic_net_beta
         self.binary_threshold_eps = binary_threshold_eps
         self.temperature = temperature
-        self.dnnf_layers = models.Sequential(name="dnnf_layers")
-        for _ in range(self.num_dnnf_layers):
-            self.dnnf_layers.add(DNNF(num_formulas=self.num_formulas,
-                                      num_conjunctions_arr=self.num_conjunctions_arr,
-                                      conjunctions_depth_arr=self.conjunctions_depth_arr,
-                                      keep_feature_prob_arr=self.keep_feature_prob_arr,
-                                      elastic_net_beta=self.elastic_net_beta,
-                                      binary_threshold_eps=self.binary_threshold_eps))
-        self.head = None
-
-    def call(self, inputs):
-        outputs = self.dnnf_layers(inputs)
-        if self.head is not None:
-            outputs = self.head(outputs)
-        return outputs
 
     def get_config(self):
-        config = super().get_config()
-        new_config = {'num_dnnf_layers': self.num_dnnf_layers,
-                      'num_formulas': self.num_formulas,
-                      'num_conjunctions_arr': self.num_conjunctions_arr,
-                      'conjunctions_depth_arr': self.conjunctions_depth_arr,
-                      'keep_feature_prob_arr': self.keep_feature_prob_arr,
-                      'elastic_net_beta': self.elastic_net_beta,
-                      'binary_threshold_eps': self.binary_threshold_eps,
-                      'temperature': self.temperature}
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'input_dim': self.input_dim,
+                  'num_dnnf_layers': self.num_dnnf_layers,
+                  'num_formulas': self.num_formulas,
+                  'num_conjunctions_arr': self.num_conjunctions_arr,
+                  'conjunctions_depth_arr': self.conjunctions_depth_arr,
+                  'keep_feature_prob_arr': self.keep_feature_prob_arr,
+                  'elastic_net_beta': self.elastic_net_beta,
+                  'binary_threshold_eps': self.binary_threshold_eps,
+                  'temperature': self.temperature
+                  }
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        return cls(input_dim=input_dim,
+                   **config)
 
-class DNFNetRegressor(DNFNet):
+
+@keras.saving.register_keras_serializable(package="teras.models")
+class DNFNetClassifier(DNFNet):
     """
     DNFNetRegressor based on the DNFNet architecture proposed by Liran Katzir et al.
     in the paper NET-DNF: Effective Deep Modeling Of Tabular Data.
 
     Reference(s):
         https://openreview.net/forum?id=73WTGs96kho
 
     Args:
-        num_outputs: `int`, default 1,
-            Number of regression outputs.
-        num_dnnf_layers: `int`, default 1,
-            Number of DNNF layers to use in the model
-        num_formulas: `int`, default 256,
-            Number of DNF formulas to use in each DNNF layer.
+        num_classes: ``int``, default 2,
+            Number of classes to predict.
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default None,
+            Hidden units to use in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+            By default, no hidden layer is used.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        num_dnnf_layers: ``int``, default 1,
+            Number of ``DNNF`` layers to use in the model
+
+        num_formulas: ``int``, default 256,
+            Number of DNF formulas to use in each ``DNNF`` layer.
             Each DNF formula is analogous to a tree in tree based ensembles.
-        num_conjunctions_arr: `List[int]`, default [6, 9, 12, 15],
+
+        num_conjunctions_arr: ``List[int]`` or ``Tuple[int]``, default [6, 9, 12, 15],
             Conjunctions array to use in each DNNF layer.
             It is used in the computation of total number of literals as well as
             computation of number of literals per DNF formula.
-        conjunctions_depth_arr: `List[int]`, default [2, 4, 6],
-            Conjunctions depth array to use in each DNNF layer.
+
+        conjunctions_depth_arr: ``List[int]`` or ``Tuple[int]``, default [2, 4, 6],
+            Conjunctions depth array to use in each ``DNNF`` layer.
             It is used in the computation of total number of literals as well as
             computation of number of literals per DNF formula.
-        keep_feature_prob_arr: `List[float]`, default [0.1, 0.3, 0.5, 0.7, 0.9],
-            Feature probability array to use in each DNNF layer.
+
+        keep_feature_prob_arr: ``List[float]`` or ``Tuple[float]``, default [0.1, 0.3, 0.5, 0.7, 0.9],
+            Feature probability array to use in each ``DNNF`` layer.
             It is used by the Feature Selection layer to randomly select a probability
             value that is used in the random selection of input features.
-        elastic_net_beta: `float`, default 0.4,
-            Used in the computation of Elastic Net Regularization in the DNNF layer.
-        binary_threshold_eps:   `float`, default 1.0,
-            Used in the computation of learnable mask in the DNNF layer.
-        temperature: `float`, default 2.0,
-            Temperature value to use in the Localization layer.
+
+        elastic_net_beta: ``float``, default 0.4,
+            Used in the computation of Elastic Net Regularization in the ``DNNF`` layer.
+
+        binary_threshold_eps: ``float``, default 1.0,
+            Used in the computation of learnable mask in the ``DNNF`` layer.
+
+        temperature: ``float``, default 2.0,
+            Temperature value to use in the ``Localization`` layer.
             According to the paper, The inclusion of an adaptive temperature in this localization mechanism
             facilitates a data-dependent degree of exclusivity:
             at high temperatures, only a few DNNFs will handle an input instance whereas
             at low temperatures, more DNNFs will effectively participate in the ensemble.
     """
     def __init__(self,
-                 num_outputs: int = 1,
+                 num_classes: int = 2,
+                 head_units_values: UnitsValuesType = None,
+                 input_dim: int = None,
                  num_dnnf_layers: int = 1,
                  num_formulas: int = 2048,
-                 num_conjunctions_arr: LIST_OF_INT = [6, 9, 12, 15],
-                 conjunctions_depth_arr: LIST_OF_INT = [2, 4, 6],
-                 keep_feature_prob_arr: LIST_OF_FLOAT = [0.1, 0.3, 0.5, 0.7, 0.9],
+                 num_conjunctions_arr: IntegerSequence = [6, 9, 12, 15],
+                 conjunctions_depth_arr: IntegerSequence = [2, 4, 6],
+                 keep_feature_prob_arr: FloatSequence = [0.1, 0.3, 0.5, 0.7, 0.9],
                  elastic_net_beta: float = 0.4,
                  binary_threshold_eps: float = 1.0,
                  temperature: float = 2.0,
                  **kwargs):
-        super().__init__(num_dnnf_layers=num_dnnf_layers,
+        head = ClassificationHead(num_classes=num_classes,
+                                  units_values=head_units_values)
+        super().__init__(input_dim=input_dim,
+                         num_dnnf_layers=num_dnnf_layers,
                          num_conjunctions_arr=num_conjunctions_arr,
                          conjunctions_depth_arr=conjunctions_depth_arr,
                          keep_feature_prob_arr=keep_feature_prob_arr,
                          num_formulas=num_formulas,
                          elastic_net_beta=elastic_net_beta,
                          binary_threshold_eps=binary_threshold_eps,
                          temperature=temperature,
+                         head=head,
                          **kwargs)
-        self.num_outputs = num_outputs
-        self.head = DNFNetRegressionHead(num_outputs=self.num_outputs)
+        self.num_classes = num_classes
+        self.head_units_values = head_units_values
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_outputs': self.num_outputs,
-                      }
-        config.update(new_config)
+        config.update({'num_classes': self.num_classes,
+                       'head_units_values': self.head_units_values
+                       })
         return config
 
 
-class DNFNetClassifier(DNFNet):
+@keras.saving.register_keras_serializable(package="teras.models")
+class DNFNetRegressor(DNFNet):
     """
     DNFNetRegressor based on the DNFNet architecture proposed by Liran Katzir et al.
     in the paper NET-DNF: Effective Deep Modeling Of Tabular Data.
 
     Reference(s):
         https://openreview.net/forum?id=73WTGs96kho
 
     Args:
-        num_classes: `int`, default 2,
-            Number of classes to predict.
-        activation_out:
-            Activation function to use for the output layer.
-            By default, "sigmoid" is used for binary and "softmax" is used for
-            multiclass classification.
-        num_dnnf_layers: `int`, default 1,
-            Number of DNNF layers to use in the model
-        num_formulas: `int`, default 256,
-            Number of DNF formulas to use in each DNNF layer.
+        num_outputs: ``int``, default 1,
+            Number of regression outputs.
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, None,
+            Hidden units to use in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+            By default, no hidden layer is used.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        num_dnnf_layers: ``int``, default 1,
+            Number of ``DNNF`` layers to use in the model
+
+        num_formulas: ``int``, default 256,
+            Number of DNF formulas to use in each ``DNNF`` layer.
             Each DNF formula is analogous to a tree in tree based ensembles.
-        num_conjunctions_arr: `List[int]`, default [6, 9, 12, 15],
+
+        num_conjunctions_arr: ``List[int]`` or ``Tuple[int]``, default [6, 9, 12, 15],
             Conjunctions array to use in each DNNF layer.
             It is used in the computation of total number of literals as well as
             computation of number of literals per DNF formula.
-        conjunctions_depth_arr: `List[int]`, default [2, 4, 6],
-            Conjunctions depth array to use in each DNNF layer.
+
+        conjunctions_depth_arr: ``List[int]`` or ``Tuple[int]``, default [2, 4, 6],
+            Conjunctions depth array to use in each ``DNNF`` layer.
             It is used in the computation of total number of literals as well as
             computation of number of literals per DNF formula.
-        keep_feature_prob_arr: `List[float]`, default [0.1, 0.3, 0.5, 0.7, 0.9],
-            Feature probability array to use in each DNNF layer.
+
+        keep_feature_prob_arr: ``List[float]`` or ``Tuple[float]``, default [0.1, 0.3, 0.5, 0.7, 0.9],
+            Feature probability array to use in each ``DNNF`` layer.
             It is used by the Feature Selection layer to randomly select a probability
             value that is used in the random selection of input features.
-        elastic_net_beta: `float`, default 0.4,
-            Used in the computation of Elastic Net Regularization in the DNNF layer.
-        binary_threshold_eps:   `float`, default 1.0,
-            Used in the computation of learnable mask in the DNNF layer.
-        temperature: `float`, default 2.0,
-            Temperature value to use in the Localization layer.
+
+        elastic_net_beta: ``float``, default 0.4,
+            Used in the computation of Elastic Net Regularization in the ``DNNF`` layer.
+
+        binary_threshold_eps: ``float``, default 1.0,
+            Used in the computation of learnable mask in the ``DNNF`` layer.
+
+        temperature: ``float``, default 2.0,
+            Temperature value to use in the ``Localization`` layer.
             According to the paper, The inclusion of an adaptive temperature in this localization mechanism
             facilitates a data-dependent degree of exclusivity:
             at high temperatures, only a few DNNFs will handle an input instance whereas
             at low temperatures, more DNNFs will effectively participate in the ensemble.
     """
     def __init__(self,
-                 num_classes: int = 2,
-                 activation_out=None,
+                 num_outputs: int = 1,
+                 head_units_values: UnitsValuesType = None,
+                 input_dim: int = None,
                  num_dnnf_layers: int = 1,
                  num_formulas: int = 2048,
-                 num_conjunctions_arr: LIST_OF_INT = [6, 9, 12, 15],
-                 conjunctions_depth_arr: LIST_OF_INT = [2, 4, 6],
-                 keep_feature_prob_arr: LIST_OF_FLOAT = [0.1, 0.3, 0.5, 0.7, 0.9],
+                 num_conjunctions_arr: IntegerSequence = [6, 9, 12, 15],
+                 conjunctions_depth_arr: IntegerSequence = [2, 4, 6],
+                 keep_feature_prob_arr: FloatSequence = [0.1, 0.3, 0.5, 0.7, 0.9],
                  elastic_net_beta: float = 0.4,
                  binary_threshold_eps: float = 1.0,
                  temperature: float = 2.0,
                  **kwargs):
-        super().__init__(num_dnnf_layers=num_dnnf_layers,
+        head = RegressionHead(num_outputs=num_outputs,
+                              units_values=head_units_values)
+        super().__init__(input_dim=input_dim,
+                         num_dnnf_layers=num_dnnf_layers,
                          num_conjunctions_arr=num_conjunctions_arr,
                          conjunctions_depth_arr=conjunctions_depth_arr,
                          keep_feature_prob_arr=keep_feature_prob_arr,
                          num_formulas=num_formulas,
                          elastic_net_beta=elastic_net_beta,
                          binary_threshold_eps=binary_threshold_eps,
                          temperature=temperature,
+                         head=head,
                          **kwargs)
-        self.num_classes = num_classes
-        self.activation_out = activation_out
-        self.head = DNFNetClassificationHead(num_classes=self.num_classes,
-                                             activation_out=self.activation_out)
+        self.num_outputs = num_outputs
+        self.head_units_values = head_units_values
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_classes': self.num_outputs,
-                      'activation_out': self.activation_out
+        new_config = {'num_outputs': self.num_outputs,
+                      'head_units_values': self.head_units_values
                       }
         config.update(new_config)
         return config
```

### Comparing `Teras-0.1.1/teras/models/ft_transformer.py` & `Teras-0.2.0/teras/models/ft_transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,344 +1,367 @@
-import tensorflow as tf
 from tensorflow import keras
-from teras.layers import FTNumericalFeatureEmbedding, FTCLSToken
-from teras.layers.embedding import CategoricalFeatureEmbedding
+from teras.layers.ft_transformer.ft_numerical_feature_embedding import FTNumericalFeatureEmbedding
+from teras.layers.ft_transformer.ft_cls_token import FTCLSToken
+from teras.layers.categorical_feature_embedding import CategoricalFeatureEmbedding
 from teras.layers.common.transformer import Encoder
 from teras.layers.common.head import ClassificationHead, RegressionHead
-from typing import List, Union
+from teras.layerflow.models.ft_transformer import FTTransformer as _FTTransformerLF
+from teras.utils.types import UnitsValuesType
 
 
-LayerType = Union[str, keras.layers.Layer]
-
-
-class FTTransformer(keras.Model):
+@keras.saving.register_keras_serializable("teras.models")
+class FTTransformer(_FTTransformerLF):
     """
     FT Transformer architecture proposed by Yury Gorishniy et al.
     in the paper Revisiting Deep Learning Models for Tabular Data
     in their FTTransformer architecture.
 
     Reference(s):
         https://arxiv.org/abs/2106.11959
 
     Args:
-        features_metadata: `dict`,
-            a nested dictionary of metadata for features where
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        features_metadata: ``dict``,
+            A nested dictionary of metadata for features where
             categorical sub-dictionary is a mapping of categorical feature names to a tuple of
             feature indices and the lists of unique values (vocabulary) in them,
             while numerical dictionary is a mapping of numerical feature names to their indices.
             `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
             `{feature_name: feature_idx}` for feature in numerical features.
             You can get this dictionary from
                 >>> from teras.utils import get_features_metadata_for_embedding
                 >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
-                                                                        numerical_features,
-                                                                        categorical_features)
-        embedding_dim: `int`, default 32,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        embedding_dim: ``int``, default 32,
             Embedding dimensions used in embedding numerical and categorical features.
-        numerical_embedding_hidden_dim: `int` default 16,
+
+        numerical_embedding_hidden_dim: ``int`` default 16,
             Dimensionality of the hidden layer that precedes the output layer in the
             SAINT NumericalFeatureEmebedding layer.
-        num_transformer_layer: `int`, default 6,
-            Number of (SAINT) transformer layers to use in the Encoder.
+
+        num_transformer_layer: ``int``, default 6,
+            Number of ``Transformer`` layers to use in the ``Encoder``.
             The encoder is used to contextualize the learned feature embeddings.
-        num_attention_heads: `int`, default 8,
-            Number of attention heads to use in the MultiHeadSelfAttention layer
+
+        num_attention_heads: ``int``, default 8,
+            Number of attention heads to use in the ``MultiHeadSelfAttention`` layer
             that is part of the `Transformer` layer which in turn is part of the `Encoder`.
-        num_inter_sample_attention_heads: `int`, default 8,
-            Number of heads to use in the MultiHeadInterSampleAttention that applies
-            attention over rows.
-        attention_dropout: `float`, default 0.1, Dropout rate to use in the
-            MultiHeadSelfAttention layer in the transformer layer.
-        inter_sample_attention_dropout: `float`, default 0.1,
-            Dropout rate for MultiHeadInterSampleAttention layer that applies
-            attention over rows.
-        feedforward_dropout: `float`, default 0.1,
+
+        attention_dropout: ``float``, default 0.1,
+            Dropout rate to use in the ``MultiHeadSelfAttention`` layer in the transformer layer.
+
+        feedforward_dropout: ``float``, default 0.1,
             Dropout rate to use for the dropout layer in the FeedForward block.
-        feedforward_multiplier: `int`, default 4.
+
+        feedforward_multiplier: ``int``, default 4.
             Multiplier that is multipled with the `embedding_dim`
             and the resultant value is used as hidden dimensions value for the
             hidden layer in the feedforward block.
-        encode_categorical_values: `bool`, default True,
+
+        encode_categorical_values: ``bool``, default True,
             Whether to (label) encode categorical values.
             If you've already encoded the categorical values using for instance
             Label/Ordinal encoding, you should set this to False,
             otherwise leave it as True.
             In the case of True, categorical values will be mapped to integer indices
-            using keras's string lookup layer.
+            using keras's ``IntegerLookup`` layer.
     """
     def __init__(self,
+                 input_dim: int,
                  features_metadata: dict,
                  embedding_dim: int = 32,
                  num_transformer_layers: int = 8,
                  num_attention_heads: int = 8,
                  attention_dropout: float = 0.1,
                  feedforward_dropout:  float = 0.05,
                  feedforward_multiplier: int = 4,
                  encode_categorical_values: bool = True,
                  **kwargs):
-        super().__init__(**kwargs)
+        num_categorical_features = len(features_metadata["categorical"])
+        num_numerical_features = len(features_metadata["numerical"])
+        categorical_features_exist = num_categorical_features > 0
+        numerical_features_exist = num_numerical_features > 0
+
+        # Numerical/Continuous Features Embedding
+        numerical_feature_embedding = None
+        if numerical_features_exist:
+            numerical_feature_embedding = FTNumericalFeatureEmbedding(features_metadata=features_metadata,
+                                                                      embedding_dim=embedding_dim)
+
+        # Categorical Features Embedding
+        categorical_feature_embedding = None
+        if categorical_features_exist:
+            # If categorical features exist, then they must be embedded
+            categorical_feature_embedding = CategoricalFeatureEmbedding(
+                features_metadata=features_metadata,
+                embedding_dim=embedding_dim,
+                encode=encode_categorical_values)
+
+        cls_token = FTCLSToken(embedding_dim,
+                               initialization="normal")
+        encoder = Encoder(num_transformer_layers=num_transformer_layers,
+                          num_attention_heads=num_attention_heads,
+                          embedding_dim=embedding_dim,
+                          attention_dropout=attention_dropout,
+                          feedforward_dropout=feedforward_dropout,
+                          feedforward_multiplier=feedforward_multiplier)
+
+        super().__init__(input_dim=input_dim,
+                         categorical_feature_embedding=categorical_feature_embedding,
+                         numerical_feature_embedding=numerical_feature_embedding,
+                         cls_token=cls_token,
+                         encoder=encoder,
+                         **kwargs
+                         )
+        self.input_dim = input_dim
         self.features_metadata = features_metadata
         self.num_transformer_layers = num_transformer_layers
         self.embedding_dim = embedding_dim
         self.num_attention_heads = num_attention_heads
         self.attention_dropout = attention_dropout
         self.feedforward_dropout = feedforward_dropout
         self.feedforward_multiplier = feedforward_multiplier
         self.encode_categorical_values = encode_categorical_values
 
-        self._categorical_features_metadata = self.features_metadata["categorical"]
-        self._numerical_features_metadata = self.features_metadata["numerical"]
-        self._num_categorical_features = len(self._categorical_features_metadata)
-        self._num_numerical_features = len(self._numerical_features_metadata)
-
-        self._numerical_features_exist = self._num_numerical_features > 0
-        self._categorical_features_exist = self._num_categorical_features > 0
-
-        # Numerical/Continuous Features Embedding
-        self.numerical_feature_embedding = None
-        if self._numerical_features_exist:
-            self.numerical_feature_embedding = FTNumericalFeatureEmbedding(
-                                                    numerical_features_metadata=self._numerical_features_metadata,
-                                                    embedding_dim=self.embedding_dim)
-
-        # Categorical Features Embedding
-        self.categorical_feature_embedding = None
-        if self._categorical_features_exist:
-            # If categorical features exist, then they must be embedded
-            self.categorical_feature_embedding = CategoricalFeatureEmbedding(
-                                                    categorical_features_metadata=self._categorical_features_metadata,
-                                                    embedding_dim=self.embedding_dim,
-                                                    encode=self.encode_categorical_values)
-
-        self.cls_token = FTCLSToken(self.embedding_dim,
-                                    initialization="normal")
-        self.encoder = Encoder(num_transformer_layers=self.num_transformer_layers,
-                               num_heads=self.num_attention_heads,
-                               embedding_dim=self.embedding_dim,
-                               attention_dropout=self.attention_dropout,
-                               feedforward_dropout=self.feedforward_dropout,
-                               feedforward_multiplier=self.feedforward_multiplier)
-
-        self.head = None
-
-    def call(self, inputs):
-        features = None
-        if self._categorical_features_exist:
-            categorical_features = self.categorical_feature_embedding(inputs)
-            features = categorical_features
-        if self._numerical_features_exist:
-            numerical_features = self.numerical_feature_embedding(inputs)
-            if features is not None:
-                features = tf.concat([features, numerical_features],
-                                     axis=1)
-            else:
-                features = numerical_features
-
-        features_with_cls_token = self.cls_token(features)
-        outputs = self.encoder(features_with_cls_token)
-        if self.head is not None:
-            # Since FTTransformer employs BERT like CLS token.
-            # So, it makes its predictions
-            # using only the CLS token, not the entire dataset.
-            outputs = self.head(outputs[:, -1])
-        return outputs
-
     def get_config(self):
-        config = super().get_config()
-        new_config = {'features_metadata': self.features_metadata,
-                      'embedding_dim': self.embedding_dim,
-                      'num_transformer_layers': self.num_transformer_layers,
-                      'num_attention_heads': self.num_attention_heads,
-                      'attention_dropout': self.attention_dropout,
-                      'feedforward_dropout': self.feedforward_dropout,
-                      'feedforward_multiplier': self.feedforward_multiplier,
-                      'encode_categorical_values': self.encode_categorical_values}
-        config.update(new_config)
+        config = {'name': self.name,
+                  'trainable': self.trainable,
+                  'input_dim': self.input_dim,
+                  'features_metadata': self.features_metadata,
+                  'embedding_dim': self.embedding_dim,
+                  'num_transformer_layers': self.num_transformer_layers,
+                  'num_attention_heads': self.num_attention_heads,
+                  'attention_dropout': self.attention_dropout,
+                  'feedforward_dropout': self.feedforward_dropout,
+                  'feedforward_multiplier': self.feedforward_multiplier,
+                  'encode_categorical_values': self.encode_categorical_values}
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        features_metadata = config.pop("features_metadata")
+        return cls(input_dim=input_dim,
+                   features_metadata=features_metadata,
+                   **config)
+
 
+@keras.saving.register_keras_serializable("teras.models")
 class FTTransformerClassifier(FTTransformer):
     """
     FTTransformerClassifier based on the FTTransformer architecture proposed
     by Yury Gorishniy et al. in the paper,
     Revisiting Deep Learning Models for Tabular Data.
 
     Reference(s):
         https://arxiv.org/abs/2106.11959
 
     Args:
-        num_classes: `int`, default 2,
+        num_classes: ``int``, default 2,
             Number of classes to predict.
-        activation_out: Activation to use in the Classification head,
-            by default, `sigmoid` is used for binary and `softmax` is used
-            for multi-class classification.
-        features_metadata: `dict`,
-            a nested dictionary of metadata for features where
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default None,
+            Units values to use in the hidden layers in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+            By default, no hidden layer is used.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        features_metadata: ``dict``,
+            A nested dictionary of metadata for features where
             categorical sub-dictionary is a mapping of categorical feature names to a tuple of
             feature indices and the lists of unique values (vocabulary) in them,
             while numerical dictionary is a mapping of numerical feature names to their indices.
             `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
             `{feature_name: feature_idx}` for feature in numerical features.
             You can get this dictionary from
                 >>> from teras.utils import get_features_metadata_for_embedding
                 >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
-                                                                        numerical_features,
-                                                                        categorical_features)
-        embedding_dim: `int`, default 32,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        embedding_dim: ``int``, default 32,
             Embedding dimensions used in embedding numerical and categorical features.
-        numerical_embedding_hidden_dim: `int` default 16,
+
+        numerical_embedding_hidden_dim: ``int`` default 16,
             Dimensionality of the hidden layer that precedes the output layer in the
             SAINT NumericalFeatureEmebedding layer.
-        num_transformer_layer: `int`, default 6,
-            Number of (SAINT) transformer layers to use in the Encoder.
+
+        num_transformer_layer: ``int``, default 6,
+            Number of ``Transformer`` layers to use in the ``Encoder``.
             The encoder is used to contextualize the learned feature embeddings.
-        num_attention_heads: `int`, default 8,
-            Number of attention heads to use in the MultiHeadSelfAttention layer
+
+        num_attention_heads: ``int``, default 8,
+            Number of attention heads to use in the ``MultiHeadSelfAttention`` layer
             that is part of the `Transformer` layer which in turn is part of the `Encoder`.
-        num_inter_sample_attention_heads: `int`, default 8,
-            Number of heads to use in the MultiHeadInterSampleAttention that applies
-            attention over rows.
-        attention_dropout: `float`, default 0.1, Dropout rate to use in the
-            MultiHeadSelfAttention layer in the transformer layer.
-        inter_sample_attention_dropout: `float`, default 0.1,
-            Dropout rate for MultiHeadInterSampleAttention layer that applies
-            attention over rows.
-        feedforward_dropout: `float`, default 0.1,
+
+        attention_dropout: ``float``, default 0.1,
+            Dropout rate to use in the ``MultiHeadSelfAttention`` layer in the transformer layer.
+
+        feedforward_dropout: ``float``, default 0.1,
             Dropout rate to use for the dropout layer in the FeedForward block.
-        feedforward_multiplier: `int`, default 4.
+
+        feedforward_multiplier: ``int``, default 4.
             Multiplier that is multipled with the `embedding_dim`
             and the resultant value is used as hidden dimensions value for the
             hidden layer in the feedforward block.
-        encode_categorical_values: `bool`, default True,
+
+        encode_categorical_values: ``bool``, default True,
             Whether to (label) encode categorical values.
             If you've already encoded the categorical values using for instance
             Label/Ordinal encoding, you should set this to False,
             otherwise leave it as True.
             In the case of True, categorical values will be mapped to integer indices
-            using keras's string lookup layer.
+            using keras's ``IntegerLookup`` layer.
     """
     def __init__(self,
                  num_classes: int = 2,
-                 activation_out=None,
+                 head_units_value: UnitsValuesType = None,
                  features_metadata: dict = None,
+                 input_dim: int = None,
                  embedding_dim: int = 32,
                  num_transformer_layers: int = 8,
                  num_attention_heads: int = 8,
                  attention_dropout: float = 0.1,
                  feedforward_dropout:  float = 0.05,
                  feedforward_multiplier: int = 4,
                  encode_categorical_values: bool = True,
                  **kwargs):
-        super().__init__(features_metadata=features_metadata,
+        head = ClassificationHead(num_classes=num_classes,
+                                  units_values=head_units_value,
+                                  normalization="layer")
+        super().__init__(input_dim=input_dim,
+                         features_metadata=features_metadata,
                          embedding_dim=embedding_dim,
                          num_transformer_layers=num_transformer_layers,
                          num_attention_heads=num_attention_heads,
                          attention_dropout=attention_dropout,
                          feedforward_dropout=feedforward_dropout,
                          feedforward_multiplier=feedforward_multiplier,
                          encode_categorical_values=encode_categorical_values,
+                         head=head,
                          **kwargs)
         self.num_classes = num_classes
-        self.activation_out = activation_out
-        self.head = ClassificationHead(num_classes=self.num_classes,
-                                       units_values=None,
-                                       activation_out=self.activation_out,
-                                       normalization="layer")
+        self.head_units_value = head_units_value
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_classes': self.num_classes,
-                      'activation_out': self.activation_out
-                      }
-        config.update(new_config)
+        config.update({'num_classes': self.num_classes,
+                       'head_units_value': self.head_units_value})
         return config
 
 
+@keras.saving.register_keras_serializable("teras.models")
 class FTTransformerRegressor(FTTransformer):
     """
     FTTransformerRegressor based on the FTTransformer architecture proposed
     by Yury Gorishniy et al. in the paper,
     Revisiting Deep Learning Models for Tabular Data.
 
     Reference(s):
         https://arxiv.org/abs/2106.11959
 
     Args:
         num_outputs: `int`, default 1,
             Number of outputs to predict.
-        features_metadata: `dict`,
-            a nested dictionary of metadata for features where
+
+        head_units_values: ``List[int]`` or ``Tuple[int]``, default None,
+            Units values to use in the hidden layers in the Classification head.
+            For each value in the list/tuple,
+            a hidden layer of that dimensionality is added to the head.
+            By default, no hidden layer is used.
+
+        input_dim: ``int``,
+            Dimensionality of the input dataset,
+            or the number of features in the dataset.
+
+        features_metadata: ``dict``,
+            A nested dictionary of metadata for features where
             categorical sub-dictionary is a mapping of categorical feature names to a tuple of
             feature indices and the lists of unique values (vocabulary) in them,
             while numerical dictionary is a mapping of numerical feature names to their indices.
             `{feature_name: (feature_idx, vocabulary)}` for feature in categorical features.
             `{feature_name: feature_idx}` for feature in numerical features.
             You can get this dictionary from
                 >>> from teras.utils import get_features_metadata_for_embedding
                 >>> metadata_dict = get_features_metadata_for_embedding(dataframe,
-                                                                        numerical_features,
-                                                                        categorical_features)
-        embedding_dim: `int`, default 32,
+                ..                                                      categorical_features,
+                ..                                                      numerical_features)
+
+        embedding_dim: ``int``, default 32,
             Embedding dimensions used in embedding numerical and categorical features.
-        numerical_embedding_hidden_dim: `int` default 16,
+
+        numerical_embedding_hidden_dim: ``int`` default 16,
             Dimensionality of the hidden layer that precedes the output layer in the
             SAINT NumericalFeatureEmebedding layer.
-        num_transformer_layer: `int`, default 6,
-            Number of (SAINT) transformer layers to use in the Encoder.
+
+        num_transformer_layer: ``int``, default 6,
+            Number of ``Transformer`` layers to use in the ``Encoder``.
             The encoder is used to contextualize the learned feature embeddings.
-        num_attention_heads: `int`, default 8,
-            Number of attention heads to use in the MultiHeadSelfAttention layer
+
+        num_attention_heads: ``int``, default 8,
+            Number of attention heads to use in the ``MultiHeadSelfAttention`` layer
             that is part of the `Transformer` layer which in turn is part of the `Encoder`.
-        num_inter_sample_attention_heads: `int`, default 8,
-            Number of heads to use in the MultiHeadInterSampleAttention that applies
-            attention over rows.
-        attention_dropout: `float`, default 0.1, Dropout rate to use in the
-            MultiHeadSelfAttention layer in the transformer layer.
-        inter_sample_attention_dropout: `float`, default 0.1,
-            Dropout rate for MultiHeadInterSampleAttention layer that applies
-            attention over rows.
-        feedforward_dropout: `float`, default 0.1,
+
+        attention_dropout: ``float``, default 0.1,
+            Dropout rate to use in the ``MultiHeadSelfAttention`` layer in the transformer layer.
+
+        feedforward_dropout: ``float``, default 0.1,
             Dropout rate to use for the dropout layer in the FeedForward block.
-        feedforward_multiplier: `int`, default 4.
+
+        feedforward_multiplier: ``int``, default 4.
             Multiplier that is multipled with the `embedding_dim`
             and the resultant value is used as hidden dimensions value for the
             hidden layer in the feedforward block.
-        encode_categorical_values: `bool`, default True,
+
+        encode_categorical_values: ``bool``, default True,
             Whether to (label) encode categorical values.
             If you've already encoded the categorical values using for instance
             Label/Ordinal encoding, you should set this to False,
             otherwise leave it as True.
             In the case of True, categorical values will be mapped to integer indices
-            using keras's string lookup layer.
+            using keras's ``IntegerLookup`` layer.
     """
 
     def __init__(self,
                  num_outputs: int = 1,
+                 head_units_value: UnitsValuesType = None,
+                 input_dim: int = None,
                  features_metadata: dict = None,
                  embedding_dim: int = 32,
                  num_transformer_layers: int = 8,
                  num_attention_heads: int = 8,
                  attention_dropout: float = 0.1,
                  feedforward_dropout: float = 0.05,
                  feedforward_multiplier: int = 4,
                  encode_categorical_values: bool = True,
                  **kwargs):
-        super().__init__(features_metadata=features_metadata,
+        head = RegressionHead(num_outputs=num_outputs,
+                              units_values=head_units_value,
+                              normalization="layer")
+        super().__init__(input_dim=input_dim,
+                         features_metadata=features_metadata,
                          embedding_dim=embedding_dim,
                          num_transformer_layers=num_transformer_layers,
                          num_attention_heads=num_attention_heads,
                          attention_dropout=attention_dropout,
                          feedforward_dropout=feedforward_dropout,
                          feedforward_multiplier=feedforward_multiplier,
                          encode_categorical_values=encode_categorical_values,
+                         head=head,
                          **kwargs)
         self.num_outputs = num_outputs
-        self.head = RegressionHead(num_outputs=self.num_outputs,
-                                   units_values=None,
-                                   normalization="layer")
+        self.head_units_value = head_units_value
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'num_outputs': self.num_outputs,
-                      }
-        config.update(new_config)
+        config.update({'num_outputs': self.num_outputs,
+                       'head_units_value': self.head_units_value})
         return config
```

### Comparing `Teras-0.1.1/teras/models/gain.py` & `Teras-0.2.0/teras/models/gain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-import tensorflow as tf
-import tensorflow_probability as tfp
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import models
-from tensorflow.keras import optimizers
-from teras.losses.gain import generator_loss, discriminator_loss
-from teras.layers.gain import GeneratorBlock, DiscriminatorBlock
-from typing import List, Tuple, Union
+from teras.layers.gain import GAINGeneratorBlock, GAINDiscriminatorBlock
+from teras.layerflow.models.gain import GAIN as _GAIN_LF
+from teras.utils.types import UnitsValuesType, ActivationType
 
 
-LIST_OR_TUPLE = Union[List[int], Tuple[int]]
-
-
-class Generator(keras.Model):
+@keras.saving.register_keras_serializable(package="teras.models")
+class GAINGenerator(keras.Model):
     """
     Generator model for the GAIN architecture proposed by
     Jinsung Yoon et al. in the paper
     GAIN: Missing Data Imputation using Generative Adversarial Nets.
 
     Reference(s):
         https://arxiv.org/abs/1806.02920
 
     Args:
-        data_dim: `int`,
-            The dimensionality of the dataset.
-            It will also be the dimensionality of the output produced
-            by the generator.
+        data_dim: ``int``,
+            The dimensionality of the input dataset.
+
             Note the dimensionality must be equal to the dimensionality of dataset
-            that is passed to the `fit` method and not necessarily the dimensionality
+            that is passed to the fit method and not necessarily the dimensionality
             of the raw input dataset as sometimes data transformation alters the
             dimensionality of the dataset.
-        units_values: `List[int]` or `Tuple[int]`,
+
+            You can access the dimensionality of the transformed dataset through the
+            ``.data_dim`` attribute of the ``GAINDataSampler`` instance used in sampling
+            the dataset.
+
+        units_values: ``List[int]`` or ``Tuple[int]``,
             A list or tuple of units for constructing hidden block.
-            For each value, a `GeneratorBlock`
-            (`from teras.layers import GAINGeneratorBlock`)
+            For each value, a ``GAINGeneratorBlock``
+            (``from teras.layers import GAINGeneratorBlock``)
             of that dimensionality (units) is added to the generator
-            to form the `hidden block` of the generator.
-            By default, units_values = [data_dim, data_dim].
+            to form the ``hidden block`` of the generator.
+            By default, ``units_values`` = [``data_dim``, ``data_dim``].
+
         activation_hidden: default "relu",
             Activation function to use for the hidden layers in the hidden block.
+
         activation_out: default "sigmoid",
             Activation function to use for the output layer of the Generator.
 
     Example:
         ```python
         data_dim = 12
         # Instantiate Generator.
@@ -53,17 +52,17 @@
 
         # Generate samples
         generated_samples = generator(z)
         ```
     """
     def __init__(self,
                  data_dim: int,
-                 units_values: LIST_OR_TUPLE = None,
-                 activation_hidden="relu",
-                 activation_out="sigmoid",
+                 units_values: UnitsValuesType = None,
+                 activation_hidden: ActivationType = "relu",
+                 activation_out: ActivationType = "sigmoid",
                  **kwargs):
         super().__init__(**kwargs)
 
         if units_values is not None and not isinstance(units_values, (list, tuple)):
             raise ValueError(f"""`units_values` must be a list or tuple of units which determines
                         the number of Generator blocks and the dimensionality of those blocks.
                         But received type {type(units_values)} which is not supported.""")
@@ -71,73 +70,94 @@
         self.data_dim = data_dim
         self.units_values = units_values
         self.activation_hidden = activation_hidden
         self.activation_out = activation_out
 
         if self.units_values is None:
             self.units_values = [self.data_dim] * 2
-        self.hidden_block = models.Sequential(name="generator_hidden_block")
+        self.hidden_block = keras.models.Sequential(name="generator_hidden_block")
         for units in self.units_values:
-            self.hidden_block.add(GeneratorBlock(units,
-                                                 activation=self.activation_hidden))
+            self.hidden_block.add(GAINGeneratorBlock(units,
+                                                     activation=self.activation_hidden))
 
-        self.output_layer = layers.Dense(self.data_dim,
-                                         activation=self.activation_out,
-                                         name="generator_output_layer")
+        self.output_layer = keras.layers.Dense(self.data_dim,
+                                               activation=self.activation_out,
+                                               name="generator_output_layer")
 
     def call(self, inputs):
         # inputs is the concatenation of `mask` and `original data`
         # where `mask` has the same dimensions as data
         # so the inputs received are 2x the dimensions of `original data`
         outputs = self.hidden_block(inputs)
         outputs = self.output_layer(outputs)
         return outputs
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'data_dim': self.data_dim,
-                      "units_values": self.units_values,
-                      "activation_hidden": self.activation_hidden,
-                      "activation_out": self.activation_out,
-                      }
-        config.update(new_config)
+        activation_hidden_serialized = self.activation_hidden
+        if not isinstance(self.activation_hidden, str):
+            activation_hidden_serialized = keras.layers.serialize(self.activation_hidden)
+
+        activation_out_serialized = self.activation_out
+        if not isinstance(self.activation_out, str):
+            activation_out_serialized = keras.layers.serialize(self.activation_out)
+
+        config.update({'data_dim': self.data_dim,
+                       "units_values": self.units_values,
+                       "activation_hidden": activation_hidden_serialized,
+                       "activation_out": activation_out_serialized,
+                       }
+                      )
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        data_dim = config.pop("data_dim")
+        return cls(data_dim=data_dim,
+                   **config)
+
 
-class Discriminator(keras.Model):
+@keras.saving.register_keras_serializable(package="teras.models")
+class GAINDiscriminator(keras.Model):
     """
     Discriminator model for the GAIN architecture proposed by
     Jinsung Yoon et al. in the paper
     GAIN: Missing Data Imputation using Generative Adversarial Nets.
 
     Note that the Generator and Discriminator share the exact same
     architecture by default. They differ in the inputs they receive
     and their loss functions.
 
     Reference(s):
         https://arxiv.org/abs/1806.02920
 
     Args:
-        data_dim: `int`,
-            The dimensionality of the dataset.
-            It will also be the dimensionality of the output produced
-            by the generator.
+        data_dim: ``int``,
+            The dimensionality of the input dataset.
+
             Note the dimensionality must be equal to the dimensionality of dataset
-            that is passed to the `fit` method and not necessarily the dimensionality
+            that is passed to the fit method and not necessarily the dimensionality
             of the raw input dataset as sometimes data transformation alters the
             dimensionality of the dataset.
-        units_values: `List[int]` or `Tuple[int]`,
+
+            You can access the dimensionality of the transformed dataset through the
+            ``.data_dim`` attribute of the ``GAINDataSampler`` instance used in sampling
+            the dataset.
+
+        units_values: ``List[int]`` or ``Tuple[int]``,
             A list or tuple of units for constructing hidden block.
-            For each value, a `GAINDiscriminatorBlock`
-            (`from teras.layers import GAINDiscriminatorBlock`)
+            For each value, a ``GAINDiscriminatorBlock``
+            (``from teras.layers import GAINDiscriminatorBlock``)
             of that dimensionality (units) is added to the discriminator
-            to form the `hidden block` of the discriminator.
-            By default, units_values = [data_dim, data_dim].
+            to form the ``hidden block`` of the discriminator.
+            By default, ``units_values`` = [``data_dim``, ``data_dim``].
+
         activation_hidden: default "relu",
             Activation function to use for the hidden layers in the hidden block.
+
         activation_out: default "sigmoid",
             Activation function to use for the output layer of the Discriminator.
 
     Example:
         ```python
         data_dim = 12
         # Instantiate Generator
@@ -154,17 +174,17 @@
 
         # Predict using discriminator
         y_pred = discriminator(generated_samples)
         ```
     """
     def __init__(self,
                  data_dim: int,
-                 units_values: LIST_OR_TUPLE = None,
-                 activation_hidden="relu",
-                 activation_out="sigmoid",
+                 units_values: UnitsValuesType = None,
+                 activation_hidden: ActivationType = "relu",
+                 activation_out: ActivationType = "sigmoid",
                  **kwargs):
         super().__init__(**kwargs)
 
         if units_values is not None and not isinstance(units_values, (list, tuple)):
             raise ValueError(f"""`units_values` must be a list or tuple of units which determines
                         the number of Discriminator blocks and the dimensionality of those blocks.
                         But {units_values} was passed.""")
@@ -172,44 +192,59 @@
         self.data_dim = data_dim
         self.units_values = units_values
         self.activation_hidden = activation_hidden
         self.activation_out = activation_out
 
         if self.units_values is None:
             self.units_values = [self.data_dim] * 2
-        self.hidden_block = models.Sequential(name="discriminator_hidden_block")
+        self.hidden_block = keras.models.Sequential(name="discriminator_hidden_block")
         for units in self.units_values:
-            self.hidden_block.add(DiscriminatorBlock(units,
-                                                     activation=self.activation_hidden))
+            self.hidden_block.add(GAINDiscriminatorBlock(units,
+                                                         activation=self.activation_hidden))
 
-        self.output_layer = layers.Dense(self.data_dim,
-                                         activation=self.activation_out,
-                                         name="discriminator_output_layer")
+        self.output_layer = keras.layers.Dense(self.data_dim,
+                                               activation=self.activation_out,
+                                               name="discriminator_output_layer")
 
     def call(self, inputs):
         # inputs is the concatenation of `hint` and manipulated
         # Generator output (i.e. generated samples).
         # `hint` has the same dimensions as data
         # so the inputs received are 2x the dimensions of original data
         outputs = self.hidden_block(inputs)
         outputs = self.output_layer(outputs)
         return outputs
 
     def get_config(self):
         config = super().get_config()
-        new_config = {'data_dim': self.data_dim,
-                      "units_values": self.units_values,
-                      "activation_hidden": self.activation_hidden,
-                      "activation_out": self.activation_out,
-                      }
-        config.update(new_config)
+        activation_hidden_serialized = self.activation_hidden
+        if not isinstance(self.activation_hidden, str):
+            activation_hidden_serialized = keras.layers.serialize(self.activation_hidden)
+
+        activation_out_serialized = self.activation_out
+        if not isinstance(self.activation_out, str):
+            activation_out_serialized = keras.layers.serialize(self.activation_out)
+
+        config.update({'data_dim': self.data_dim,
+                       "units_values": self.units_values,
+                       "activation_hidden": activation_hidden_serialized,
+                       "activation_out": activation_out_serialized,
+                       }
+                      )
         return config
 
+    @classmethod
+    def from_config(cls, config):
+        data_dim = config.pop("data_dim")
+        return cls(data_dim=data_dim,
+                   **config)
+
 
-class GAIN(keras.Model):
+@keras.saving.register_keras_serializable(package="teras.models")
+class GAIN(_GAIN_LF):
     """
     GAIN is a missing data imputation model based on GANs.
     This is an implementation of the GAIN architecture
     proposed by Jinsung Yoon et al. in the paper
     GAIN: Missing Data Imputation using Generative Adversarial Nets.
 
     In GAIN, the generator observes some components of
@@ -223,53 +258,66 @@
     ensures that generator does in fact learn to generate
     samples according to the true data distribution.
 
     Reference(s):
         https://arxiv.org/abs/1806.02920
 
     Args:
-        data_dim: `int`, dimensionality of the input dataset.
+        input_dim: ``int``,
+            The dimensionality of the input dataset.
+
             Note the dimensionality must be equal to the dimensionality of dataset
             that is passed to the fit method and not necessarily the dimensionality
             of the raw input dataset as sometimes data transformation alters the
             dimensionality of the dataset.
-            This parameter can be left None if instances of Generator and Discriminator
-            are passed, otherwise it must be specified.
-        generator_units_values: `List[int]` or `Tuple[int]`,
+
+            You can access the dimensionality of the transformed dataset through the
+            ``.data_dim`` attribute of the ``GAINDataSampler`` instance used in sampling
+            the dataset.
+
+        generator_units_values: ``List[int]`` or ``Tuple[int]``,
             A list or tuple of units for constructing hidden block for the Generator.
-            For each value, a `GAINDiscriminatorBlock`
-            (`from teras.layers import GAINGeneratorBlock`)
+            For each value, a ``GAINGeneratorBlock``
+            (``from teras.layers import GAINGeneratorBlock``)
             of that dimensionality (units) is added to the generator to form the
             `hidden block` of the generator.
-            By default, generator_units_values = [data_dim, data_dim].
-        discriminator_units_values: `List[int]` or `Tuple[int]`,
+            By default, ``generator_units_values = [data_dim, data_dim]``.
+
+        discriminator_units_values: ``List[int]`` or ``Tuple[int]``,
             A list or tuple of units for constructing hidden block for the Discriminator.
-            For each value, a `GAINDiscriminatorBlock`
-            (`from teras.layers import GAINDiscriminatorBlock`)
+            For each value, a ``GAINDiscriminatorBlock``
+            (``from teras.layers import GAINDiscriminatorBlock``)
             of that dimensionality (units) is added to the discriminator
             to form the `hidden block` of the discriminator.
-            By default, discriminator_units_values = [data_dim, data_dim].
+            By default, ``discriminator_units_values = [data_dim, data_dim]``.
+
         generator_activation_hidden: default "relu",
             Activation function to use for the hidden layers in the hidden block
             for the Generator.
+
         discriminator_activation_hidden: default "relu",
             Activation function to use for the hidden layers in the hidden block
             for the Discriminator.
+
         generator_activation_out: default "sigmoid",
             Activation function to use for the output layer of the Generator.
+
         discriminator_activation_out: default "sigmoid",
             Activation function to use for the output layer of the Discriminator.
-        num_discriminator_steps: `int`, default 1,
+
+        num_discriminator_steps: ``int``, default 1,
             Number of discriminator training steps per GAIN training step.
-        hint_rate: `float`, default 0.9,
+
+        hint_rate: ``float``, default 0.9,
             Hint rate will be used to sample binary vectors for
             `hint vectors` generation. Must be between 0. and 1.
             Hint vectors ensure that generated samples follow the
             underlying data distribution.
-        alpha: `float`, default 100,
+
+        alpha: ``float``, default 100,
             Hyper parameter for the generator loss computation that
             controls how much weight should be given to the MSE loss.
             Precisely, `generator_loss` = `cross_entropy_loss` + `alpha` * `mse_loss`
             The higher the `alpha`, the more the mse_loss will affect the
             overall generator loss.
     Example:
         ```python
@@ -291,15 +339,15 @@
 
         transformed_data = data_transformer.transform(input_data, return_dataframe=True)
 
         data_sampler = DataSampler()
         dataset = data_sampler.get_dataset(transformed_data)
 
         # Instantiate GAIN
-        gain_imputer = GAIN()
+        gain_imputer = GAIN(input_dim=data_sampler.data_dim)
 
         # Compile it
         gain_imputer.compile()
 
         # Train it
         gain_imputer.fit(dataset)
 
@@ -313,219 +361,64 @@
         imputed_data = data_transformer.reverse_transform(imputed_data)
 
         # Imputation Method 2:
         imputed_data = gain_imputer.impute(test_data)
         ```
     """
     def __init__(self,
-                 data_dim: int,
-                 generator_units_values: LIST_OR_TUPLE = None,
-                 discriminator_units_values: LIST_OR_TUPLE = None,
-                 generator_activation_hidden="relu",
-                 discriminator_activation_hidden="relu",
-                 generator_activation_out="sigmoid",
-                 discriminator_activation_out="sigmoid",
+                 input_dim: int,
+                 generator_units_values: UnitsValuesType = None,
+                 discriminator_units_values: UnitsValuesType = None,
+                 generator_activation_hidden: ActivationType = "relu",
+                 discriminator_activation_hidden: ActivationType = "relu",
+                 generator_activation_out: ActivationType = "sigmoid",
+                 discriminator_activation_out: ActivationType = "sigmoid",
                  num_discriminator_steps: int = 1,
                  hint_rate: float = 0.9,
                  alpha: float = 100,
                  **kwargs):
-        super().__init__(**kwargs)
-        self.data_dim = data_dim
+        generator = GAINGenerator(data_dim=input_dim,
+                                  units_values=generator_units_values,
+                                  activation_hidden=generator_activation_hidden,
+                                  activation_out=generator_activation_out)
+        discriminator = GAINDiscriminator(data_dim=input_dim,
+                                          units_values=discriminator_units_values,
+                                          activation_hidden=discriminator_activation_hidden,
+                                          activation_out=discriminator_activation_out)
+        super().__init__(generator=generator,
+                         discriminator=discriminator,
+                         num_discriminator_steps=num_discriminator_steps,
+                         hint_rate=hint_rate,
+                         alpha=alpha,
+                         **kwargs)
+        self.input_dim = input_dim
         self.generator_units_values = generator_units_values
         self.discriminator_units_values = discriminator_units_values
         self.generator_activation_hidden = generator_activation_hidden
         self.discriminator_activation_hidden = discriminator_activation_hidden
         self.generator_activation_out = generator_activation_out
         self.discriminator_activation_out = discriminator_activation_out
         self.num_discriminator_steps = num_discriminator_steps
         self.hint_rate = hint_rate
         self.alpha = alpha
 
-        self.generator = Generator(data_dim=self.data_dim,
-                                   units_values=self.generator_units_values,
-                                   activation_hidden=self.generator_activation_hidden,
-                                   activation_out=self.generator_activation_out)
-        self.discriminator = Discriminator(data_dim=self.data_dim,
-                                           units_values=self.discriminator_units_values,
-                                           activation_hidden=self.discriminator_activation_hidden,
-                                           activation_out=self.discriminator_activation_out)
-        self.z_sampler = tfp.distributions.Uniform(low=0.,
-                                                   high=0.01,
-                                                   name="z_sampler")
-        self.hint_vectors_sampler = tfp.distributions.Binomial(total_count=1,
-                                                               probs=self.hint_rate,
-                                                               name="hint_vectors_generator")
-
-        # Loss trackers
-        self.generator_loss_tracker = keras.metrics.Mean(name="generator_loss")
-        self.discriminator_loss_tracker = keras.metrics.Mean(name="discriminator_loss")
-
-    def compile(self,
-                generator_optimizer=optimizers.Adam(),
-                discriminator_optimizer=optimizers.Adam(),
-                generator_loss=generator_loss,
-                discriminator_loss=discriminator_loss):
-        super().compile()
-        self.generator_optimizer = generator_optimizer
-        self.discriminator_optimizer = discriminator_optimizer
-        self.generator_loss = generator_loss
-        self.discriminator_loss = discriminator_loss
-
-    def get_generator(self):
-        return self.generator
-
-    def get_discriminator(self):
-        return self.discriminator
-
-    def call(self, inputs, mask=None, training=None):
-        if mask is not None:
-            inputs = tf.concat([inputs, mask], axis=1)
-        generated_samples = self.generator(inputs)
-        return generated_samples
-
-    def train_step(self, data):
-        # data is a tuple of x_generator and x_discriminator batches
-        # drawn from the dataset. The reason behind generating two separate
-        # batches of data at each step is that it's how GAIN's algorithm works
-        x_gen, x_disc = data
-
-        # =====> Train the discriminator <=====
-        for _ in range(self.num_discriminator_steps):
-            # Create mask
-            mask = tf.constant(1.) - tf.cast(tf.math.is_nan(x_disc), dtype=tf.float32)
-            # replace nans with 0.
-            x_disc = tf.where(tf.math.is_nan(x_disc), x=0., y=x_disc)
-            # Sample noise
-            z = self.z_sampler.sample(sample_shape=tf.shape(x_disc))
-            # Sample hint vectors
-            hint_vectors = self.hint_vectors_sampler.sample(sample_shape=(tf.shape(x_disc)))
-            hint_vectors *= mask
-            # Combine random vectors with original data
-            x_disc = x_disc * mask + (1 - mask) * z
-            # Keras model raises `gain`'s weights not created error if we don't implement the
-            # `call` method and call it from our code no matter if we compile it or not.
-            # so to work around that error we place the call to `Generator`'s `call` method
-            # in the `call` method of the `GAIN` model, this way the model's
-            # generated_samples = self.generator(tf.concat([x_disc, mask], axis=1))
-            generated_samples = self(x_disc, mask=mask)
-            # Combine generated samples with original data
-            x_hat_disc = (generated_samples * (1 - mask)) + (x_disc * mask)
-            with tf.GradientTape() as tape:
-                discriminator_pred = self.discriminator(tf.concat([x_hat_disc, hint_vectors], axis=1))
-                loss_disc = self.discriminator_loss(discriminator_pred, mask)
-            gradients = tape.gradient(loss_disc, self.discriminator.trainable_weights)
-            self.discriminator_optimizer.apply_gradients(zip(gradients, self.discriminator.trainable_weights))
-
-        # =====> Train the generator <=====
-        mask = tf.constant(1.) - tf.cast(tf.math.is_nan(x_gen), dtype=tf.float32)
-        x_gen = tf.where(tf.math.is_nan(x_gen), x=0., y=x_gen)
-        z = self.z_sampler.sample(sample_shape=tf.shape(x_gen))
-        hint_vectors = self.hint_vectors_sampler.sample(sample_shape=(tf.shape(x_gen)))
-        hint_vectors *= mask
-        x_gen = x_gen * mask + (1 - mask) * z
-
-        with tf.GradientTape() as tape:
-            # generated_samples = self.generator(tf.concat([x_gen, mask], axis=1))
-            generated_samples = self(x_gen, mask=mask)
-            # Combine generated samples with original/observed data
-            x_hat = (generated_samples * (1 - mask)) + (x_gen * mask)
-            discriminator_pred = self.discriminator(tf.concat([x_hat, hint_vectors], axis=1))
-            loss_gen = self.generator_loss(generated_samples=generated_samples,
-                                           real_samples=x_gen,
-                                           discriminator_pred=discriminator_pred,
-                                           mask=mask,
-                                           alpha=self.alpha)
-        gradients = tape.gradient(loss_gen, self.generator.trainable_weights)
-        self.generator_optimizer.apply_gradients(zip(gradients, self.generator.trainable_weights))
-
-        # Update custom tracking metrics
-        self.generator_loss_tracker.update_state(loss_gen)
-        self.discriminator_loss_tracker.update_state(loss_disc)
-
-        results = {m.name: m.result() for m in self.metrics}
-        results.update({"generator_" + m.name: m.result() for m in self.generator.metrics})
-        results.update({"discriminator_" + m.name: m.result() for m in self.discriminator.metrics})
-        return results
-
-    def predict_step(self, data):
-        """
-        Args:
-            Transformed data.
-        Returns:
-            Imputed data that should be reverse transformed
-            to its original form.
-        """
-        if isinstance(data, tuple):
-            data = data[0]
-        data = tf.cast(data, tf.float32)
-        # Create mask
-        mask = tf.constant(1.) - tf.cast(tf.math.is_nan(data), dtype=tf.float32)
-        data = tf.where(tf.math.is_nan(data), x=0., y=data)
-        # Sample noise
-        z = self.z_sampler.sample(sample_shape=tf.shape(data))
-        x = mask * data + (1 - mask) * z
-        # imputed_data = self.generator(tf.concat([x, mask], axis=1))
-        imputed_data = self(x, mask=mask)
-        imputed_data = mask * data + (1 - mask) * imputed_data
-        return imputed_data
-
-    def impute(self,
-               x,
-               data_transformer=None,
-               reverse_transform=True,
-               batch_size=None,
-               verbose="auto",
-               steps=None,
-               callbacks=None,
-               max_queue_size=10,
-               workers=1,
-               use_multiprocessing=False
-               ):
-        """
-        Impute function combines GAIN's `predict` method and
-        DataTransformer's `reverse_transform` method to fill
-        the missing data and transform into the original format.
-        It exposes all the arguments taken by the `predict` method.
-
-        Args:
-            x: `pd.DataFrame`, dataset with missing values.
-            data_transformer: An instance of DataTransformer class which
-                was used in transforming the raw input data
-            reverse_transform: `bool`, default True, whether to reverse
-                transformed the raw imputed data to original format.
-
-        Returns:
-            Imputed data in the original format.
-        """
-        x_imputed = self.predict(x,
-                                 batch_size=batch_size,
-                                 verbose=verbose,
-                                 steps=steps,
-                                 callbacks=callbacks,
-                                 max_queue_size=max_queue_size,
-                                 workers=workers,
-                                 use_multiprocessing=use_multiprocessing)
-        if reverse_transform:
-            if data_transformer is None:
-                raise ValueError("To reverse transform the raw imputed data, `data_transformer` must not be None. "
-                                 "Please pass the instance of DataTransformer class used to transform the input "
-                                 "data as argument to this `impute` method."
-                                 "Or alternatively, you can set `reverse_transform` parameter to False, "
-                                 "and manually reverse transform the generated raw data to original format "
-                                 "using the `reverse_transform` method of DataTransformer instance.")
-            x_imputed = data_transformer.reverse_transform(x_imputed)
-        return x_imputed
-
     def get_config(self):
-        config = super(GAIN, self).get_config()
-        config.update({'data_dim': self.data_dim,
-                       "generator_units_values": self.generator_units_values,
-                       "discriminator_units_values": self.discriminator_units_values,
-                       "generator_activation_hidden": self.generator_activation_hidden,
-                       "discriminator_activation_hidden": self.discriminator_activation_hidden,
-                       "generator_activation_out": self.generator_activation_out,
-                       "discriminator_activation_out":  self.discriminator_activation_out,
-                       'num_discriminator_steps': self.num_discriminator_steps,
-                       'hint_rate': self.hint_rate,
-                       'alpha': self.alpha,
-                       })
+        config = {"name": self.name,
+                  "trainable": self.trainable,
+                  "input_dim": self.input_dim,
+                  "generator_units_values": self.generator_units_values,
+                  "discriminator_units_values": self.discriminator_units_values,
+                  "generator_activation_hidden": self.generator_activation_hidden,
+                  "discriminator_activation_hidden": self.discriminator_activation_hidden,
+                  "generator_activation_out": self.generator_activation_out,
+                  "discriminator_activation_out":  self.discriminator_activation_out,
+                  "num_discriminator_steps": self.num_discriminator_steps,
+                  "hint_rate": self.hint_rate,
+                  "alpha": self.alpha,
+                  }
         return config
+
+    @classmethod
+    def from_config(cls, config):
+        input_dim = config.pop("input_dim")
+        return cls(input_dim=input_dim,
+                   **config)
```

### Comparing `Teras-0.1.1/teras/preprocessing/__init__.py` & `Teras-0.2.0/teras/layers/activation/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,10 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from .oenf import PiecewiseLinearEncoding
-
-from .ctgan import ModeSpecificNormalization
+from teras.layers.activation.gumbel_softmax import GumbelSoftmax
```

### Comparing `Teras-0.1.1/teras/preprocessing/base/__init__.py` & `Teras-0.2.0/teras/generative/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,10 +6,17 @@
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitations under the License.5
+
+
+# CTGAN models
+from teras.models.ctgan import CTGAN
+
+
+# TVAE models
+from teras.models.tvae import TVAE
 
-from .base_data_transformer import BaseDataTransformer
```

### Comparing `Teras-0.1.1/teras/preprocessing/ctgan.py` & `Teras-0.2.0/teras/preprocessing/ctgan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 from sklearn.preprocessing import OneHotEncoder
 import tensorflow as tf
 from sklearn.mixture import BayesianGaussianMixture
 from teras.utils import tf_random_choice
 import numpy as np
 import pandas as pd
-from collections import namedtuple
-from copy import deepcopy
 from teras.preprocessing.base import BaseDataTransformer
+from teras.utils.types import FeaturesNamesType
 
 
 class ModeSpecificNormalization:
     """
     Mode Specific Normalization as proposed by
     Lei Xu et al. in the paper,
     "Modeling Tabular data using Conditional GAN".
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
 
     Args:
-        numerical_features:
+        numerical_features: ``List[str]``
             List of numerical features names.
             In the case of ndarray, pass a list of numerical column indices.
-        max_clusters: Maximum clusters
-        std_multiplier:
+
+        max_clusters: ``int``, default 10,
+            Maximum clusters
+
+        std_multiplier: ``int``, default 4,
             Multiplies the standard deviation in the normalization.
             Defaults to 4 as proposed in the paper.
-        weight_threshold:
+
+        weight_threshold: ``int``, default 0.005,
             Taken from the official implementation.
             The minimum value a component weight can take to be considered a valid component.
             `weights_` under this value will be ignored.
-            Defaults to 0.005.
-        covariance_type: parameter for the GaussianMixtureModel class of sklearn
-        weight_concentration_prior_type: parameter for the GaussianMixtureModel class of sklearn
-        weight_concentration_prior: parameter for the GaussianMixtureModel class of sklearn
+
+        covariance_type: ``str``,
+            Parameter for the ``GaussianMixtureModel`` class of sklearn
+
+        weight_concentration_prior_type: ``str``, default "dirichlet_process",
+            Parameter for the ``GaussianMixtureModel`` class of sklearn
+
+        weight_concentration_prior: ``float``, default 0.01,
+            Parameter for the GaussianMixtureModel class of sklearn
     """
     def __init__(self,
-                 numerical_features=None,
-                 max_clusters=10,
-                 std_multiplier=4,
-                 weight_threshold=0.,
-                 covariance_type="full",
-                 weight_concentration_prior_type="dirichlet_process",
-                 weight_concentration_prior=0.001):
+                 numerical_features: FeaturesNamesType = None,
+                 max_clusters: int = 10,
+                 std_multiplier: int = 4,
+                 weight_threshold: float = 0.,
+                 covariance_type: str = "full",
+                 weight_concentration_prior_type: str = "dirichlet_process",
+                 weight_concentration_prior: float = 0.001):
         self.numerical_features = numerical_features
         self.max_clusters = max_clusters
         self.std_multiplier = std_multiplier
         self.weight_threshold = weight_threshold
         self.covariance_type = covariance_type
         self.weight_concentration_prior_type = weight_concentration_prior_type
         self.weight_concentration_prior = weight_concentration_prior
@@ -57,15 +65,15 @@
         # 1. `Clusters indices` will be used in the transform method
         #       to create the one hot vector B(i,j) where B stands for Beta, for each value c(i,j)
         #       where c(i,j) is the jth value in the ith numerical feature.
         #       as proposed in the paper in the steps to apply mode specific normalization method on page 3-4.
         # 2. `Number of valid clusters` will be used in the transform method when one-hotting
         # 3. `means` and `standard deviations` will be used in transform
         #       step to normalize the value c(i,j) to create a(i,j) where a stands for alpha.
-        self.meta_data = {}
+        self.metadata = {}
 
         self.bay_guass_mix = BayesianGaussianMixture(n_components=self.max_clusters,
                                                      covariance_type=self.covariance_type,
                                                      weight_concentration_prior_type=self.weight_concentration_prior_type,
                                                      weight_concentration_prior=self.weight_concentration_prior)
 
         self.fitted = False
@@ -83,15 +91,15 @@
                 feature = x[feature_name].values.reshape(-1, 1)
             elif isinstance(x, np.ndarray):
                 feature = x[:, feature_name].reshape(-1, 1)
             else:
                 raise ValueError(f"`x` must be either a pandas DataFrame or numpy ndarray. "
                                  f"{type(x)} was given.")
 
-            self.meta_data[feature_name] = {}
+            self.metadata[feature_name] = {}
             self.bay_guass_mix.fit(feature)
             # The authors use a weight threshold to filter out components in their implementation.
             # For consistency's sake, we're going to use this idea but with slight modification.
             # Reference to the official implementation: https://github.com/sdv-dev/CTGAN
             valid_clusters_indicator = self.bay_guass_mix.weights_ > self.weight_threshold
             # Compute probability of coming from each cluster for each value in the given (numerical) feature.
             clusters_probs = self.bay_guass_mix.predict_proba(feature)
@@ -111,57 +119,57 @@
                 random_choice,
                 axis=1,
                 arr=clusters_probs)
 
             # To create one-hot component, we'll store the selected clusters indices
             # and the number of valid clusters
             num_valid_clusters = sum(valid_clusters_indicator)
-            self.meta_data[feature_name]['selected_clusters_indices'] = selected_clusters_indices
-            self.meta_data[feature_name]['num_valid_clusters'] = num_valid_clusters
+            self.metadata[feature_name]['selected_clusters_indices'] = selected_clusters_indices
+            self.metadata[feature_name]['num_valid_clusters'] = num_valid_clusters
 
             relative_indices_all.append(relative_index)
             # The 1 is for the alpha feature, since each numerical feature
             # gets transformed into alpha + betas where,
             # |alpha| = 1 and |betas| = num_valid_clusters
             relative_index += (1 + num_valid_clusters)
             num_valid_clusters_all.append(num_valid_clusters)
 
             # Use the selected clusters to normalize the values.
             # To normalize, we need the means and standard deviations
             # Means
             clusters_means = self.bay_guass_mix.means_.squeeze()[valid_clusters_indicator]
-            self.meta_data[feature_name]['clusters_means'] = clusters_means
+            self.metadata[feature_name]['clusters_means'] = clusters_means
             # Standard Deviations
             clusters_stds = np.sqrt(self.bay_guass_mix.covariances_).squeeze()[valid_clusters_indicator]
-            self.meta_data[feature_name]['clusters_stds'] = clusters_stds
+            self.metadata[feature_name]['clusters_stds'] = clusters_stds
 
-        self.meta_data["relative_indices_all"] = np.array(relative_indices_all)
-        self.meta_data["num_valid_clusters_all"] = num_valid_clusters_all
+        self.metadata["relative_indices_all"] = np.array(relative_indices_all)
+        self.metadata["num_valid_clusters_all"] = num_valid_clusters_all
         self.fitted = True
 
     def transform(self, x):
         """
         Args:
             x: A pandas DataFrame
         Returns:
             A numpy ndarray of transformed numerical data
         """
         # Contain the normalized numerical features
         x_cont_normalized = []
         for feature_name in self.numerical_features:
-            selected_clusters_indices = self.meta_data[feature_name]['selected_clusters_indices']
-            num_valid_clusters = self.meta_data[feature_name]['num_valid_clusters']
+            selected_clusters_indices = self.metadata[feature_name]['selected_clusters_indices']
+            num_valid_clusters = self.metadata[feature_name]['num_valid_clusters']
             # One hot components for all values in the feature
             # we borrow the beta notation from the paper
             # for clarity and understanding's sake.
             betas = np.eye(num_valid_clusters)[selected_clusters_indices]
 
             # Normalizing
-            means = self.meta_data[feature_name]['clusters_means']
-            stds = self.meta_data[feature_name]['clusters_stds']
+            means = self.metadata[feature_name]['clusters_means']
+            stds = self.metadata[feature_name]['clusters_stds']
             if isinstance(x, pd.DataFrame):
                 feature = x[feature_name].values
             elif isinstance(x, np.ndarray):
                 feature = x[:, feature_name]
             else:
                 raise ValueError(f"`x` must be either a pandas DataFrame or numpy ndarray. "
                                  f"{type(x)} was given.")
@@ -206,52 +214,59 @@
                 x[:, feature_name] = normalized_feature * (self.std_multiplier * stds) + means
             else:
                 raise ValueError(f"`x_normalized` must be either a pandas DataFrame or numpy ndarray. "
                                  f"{type(x_normalized)} was given.")
         return x
 
 
-class DataTransformer(BaseDataTransformer):
+class CTGANDataTransformer(BaseDataTransformer):
     """
     Data Transformation class based on the data transformation
     in the official CTGAN paper and implementation.
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
         https://github.com/sdv-dev/CTGAN/
 
     Args:
-        numerical_features: List of numerical features names
-        categorical_features: List of categorical features names
-        max_clusters: Maximum Number of clusters to use in ModeSpecificNormalization
-            Defaults to 10
-        std_multiplier:
+        categorical_features: ``List[str]``,
+            List of categorical features names in the dataset.
+
+        numerical_features: ``List[str]``,
+            List of numerical features names in the dataset.
+
+        max_clusters: ``int``, default 10,
+            Maximum Number of clusters to use in ``ModeSpecificNormalization``
+
+        std_multiplier: ``int``, default 4,
             Multiplies the standard deviation in the normalization.
-            Defaults to 4 as proposed in the paper.
-        weight_threshold:
-            Taken from the official implementation.
+
+        weight_threshold: ``float``, default 0.005,
             The minimum value a component weight can take to be considered a valid component.
             `weights_` under this value will be ignored.
-            Defaults to 0.005
-        covariance_type: parameter for the GaussianMixtureModel class of sklearn
-            Defaults to 'full'
-        weight_concentration_prior_type: parameter for the GaussianMixtureModel class of sklearn
-            Defaults to 'dirichlet_process'
-        weight_concentration_prior: parameter for the GaussianMixtureModel class of sklearn.
-            Defaults to 0.001
+            (Taken from the official implementation.)
+
+        covariance_type: ``str``, default "full",
+            Parameter for the ``GaussianMixtureModel`` class of sklearn.
+
+        weight_concentration_prior_type: ``str``, default "dirichlet_process",
+            Parameter for the ``GaussianMixtureModel`` class of sklearn
+
+        weight_concentration_prior: ``float``, default 0.001,
+            Parameter for the ``GaussianMixtureModel`` class of sklearn.
     """
     def __init__(self,
-                 numerical_features=None,
-                 categorical_features=None,
-                 max_clusters=10,
-                 std_multiplier=4,
-                 weight_threshold=0.005,
-                 covariance_type="full",
-                 weight_concentration_prior_type="dirichlet_process",
-                 weight_concentration_prior=0.001
+                 numerical_features: FeaturesNamesType = None,
+                 categorical_features: FeaturesNamesType = None,
+                 max_clusters: int = 10,
+                 std_multiplier: int = 4,
+                 weight_threshold: float = 0.005,
+                 covariance_type: str = "full",
+                 weight_concentration_prior_type: str = "dirichlet_process",
+                 weight_concentration_prior: float = 0.001
                  ):
         self.numerical_features = numerical_features if numerical_features else []
         self.categorical_features = categorical_features if categorical_features else []
         self.max_clusters = max_clusters
         self.std_multiplier = std_multiplier
         self.weight_threshold = weight_threshold
         self.covariance_type = covariance_type
@@ -267,31 +282,33 @@
                 numerical_features=self.numerical_features,
                 max_clusters=self.max_clusters,
                 std_multiplier=self.std_multiplier,
                 weight_threshold=self.weight_threshold,
                 covariance_type=self.covariance_type,
                 weight_concentration_prior_type=self.weight_concentration_prior_type,
                 weight_concentration_prior=self.weight_concentration_prior)
-        self.meta_data = dict()
         self.categorical_values_probs = dict()
         self.one_hot_enc = OneHotEncoder()
+        self.metadata = dict()
+        self.metadata["categorical"] = dict()
+        self.metadata["numerical"] = dict()
 
     def transform_numerical_data(self, x):
         return self.mode_specific_normalizer.fit_transform(x)
 
     def transform_categorical_data(self, x):
         # To speedup computation of conditional vector down the road,
         # we assign a relative index to each feature. For instance,
         # Given three categorical columns Gender(2 categories), City (4 categories) and EconomicClass (5 categories)
         # Relative indexes will be calculated as below:
         #   gender_relative_index: 0
         #   city_relative_index: gender_relative_index + num_categories_in_gender => 0 + 2 = 2
         #   economic_class_relative_index: city_relative_index + num_categories_in_city => 2 + 4 = 6
 
-        categorical_meta_data = dict()
+        categorical_metadata = dict()
         # NOTE: The purpose of using these lists is that, this way we'll later be able to access
         # metadata for multiple features at once using their indices rather than names
         # which would've been required in case of a dict and would have been less efficient
         relative_indices_all = []
         num_categories_all = []
         # For every feature we'll compute the probabilities over the range of values based on their freqs
         # and then append that probabilities array to the following mother array
@@ -312,115 +329,94 @@
             # we round the probabilities to 7 decimal points
             probs = np.around(np.array(list(categories_probs_dict.values())), 7)
             # Normalizing so all probs sum up to 1
             probs = probs / np.sum(probs)
             categories, categories_probs = list(categories_probs_dict.keys()), probs
             categories_probs_all.append(categories_probs)
             categories_all.append(categories)
-        categorical_meta_data["total_num_categories"] = sum(num_categories_all)
-        categorical_meta_data["num_categories_all"] = num_categories_all
-        categorical_meta_data["relative_indices_all"] = np.array(relative_indices_all)
-        categorical_meta_data["categories_probs_all"] = categories_probs_all
-        categorical_meta_data["categories_all"] = categories_all
+        categorical_metadata["total_num_categories"] = sum(num_categories_all)
+        categorical_metadata["num_categories_all"] = num_categories_all
+        categorical_metadata["relative_indices_all"] = np.array(relative_indices_all)
+        categorical_metadata["categories_probs_all"] = categories_probs_all
+        categorical_metadata["categories_all"] = categories_all
 
-        self.meta_data["categorical"] = categorical_meta_data
+        self.metadata["categorical"] = categorical_metadata
 
         self.one_hot_enc.fit(x)
         return self.one_hot_enc.transform(x)
 
     def fit(self, x, **kwargs):
         # we've got nothing to fit in this case
         pass
 
     def transform(self, x, **kwargs):
         total_transformed_features = 0
         x_numerical, x_categorical = None, None
         if self.num_numerical_features > 0:
             x_numerical = self.transform_numerical_data(x[self.numerical_features])
-            self.meta_data["numerical"] = self.mode_specific_normalizer.meta_data
-            total_transformed_features += (self.meta_data["numerical"]["relative_indices_all"][-1] +
-                                           self.meta_data["numerical"]["num_valid_clusters_all"][-1])
+            self.metadata["numerical"] = self.mode_specific_normalizer.metadata
+            total_transformed_features += (self.metadata["numerical"]["relative_indices_all"][-1] +
+                                           self.metadata["numerical"]["num_valid_clusters_all"][-1])
         if self.num_categorical_features > 0:
             x_categorical = self.transform_categorical_data(x[self.categorical_features])
-            total_transformed_features += (self.meta_data["categorical"]["relative_indices_all"][-1] +
-                                           self.meta_data["categorical"]["num_categories_all"][-1] + 1)
+            total_transformed_features += (self.metadata["categorical"]["relative_indices_all"][-1] +
+                                           self.metadata["categorical"]["num_categories_all"][-1] + 1)
 
         # since we concatenate the categorical features AFTER the numerical alphas and betas
         # so we'll create an overall relative indices array where we offset the relative indices
         # of the categorical features by the total number of numerical features components
         relative_indices_all = []
         offset = 0
         if x_numerical is not None:
-            cont_relative_indices = self.meta_data["numerical"]["relative_indices_all"]
+            cont_relative_indices = self.metadata["numerical"]["relative_indices_all"]
             relative_indices_all.extend(cont_relative_indices)
-            offset = cont_relative_indices[-1] + self.meta_data["numerical"]["num_valid_clusters_all"][-1]
+            offset = cont_relative_indices[-1] + self.metadata["numerical"]["num_valid_clusters_all"][-1]
         if x_categorical is not None:
             # +1 since the categorical relative indices start at 0
-            relative_indices_all.extend(self.meta_data["categorical"]["relative_indices_all"] + 1 + offset)
-        self.meta_data["relative_indices_all"] = relative_indices_all
-        self.meta_data["total_transformed_features"] = total_transformed_features
+            relative_indices_all.extend(self.metadata["categorical"]["relative_indices_all"] + 1 + offset)
+        self.metadata["relative_indices_all"] = relative_indices_all
+        self.metadata["total_transformed_features"] = total_transformed_features
         x_transformed = np.concatenate([x_numerical, x_categorical.toarray()], axis=1)
         return x_transformed
 
-    def get_meta_data(self):
-        """
-        Returns:
-            named tuple of features meta data.
-        """
-        MetaData = namedtuple("MetaData", self.meta_data.keys())
-
-        CategoricalMetaData = namedtuple("CategoricalMetaData",
-                                         self.meta_data["categorical"].keys())
-        categorical_meta_data = CategoricalMetaData(**self.meta_data["categorical"])
-
-        NumericalMetaData = namedtuple("NumericalMetaData",
-                                       self.meta_data["numerical"].keys())
-        numerical_meta_data = NumericalMetaData(**self.meta_data["numerical"])
-
-        meta_data_copy = deepcopy(self.meta_data)
-        meta_data_copy["categorical"] = categorical_meta_data
-        meta_data_copy["numerical"] = numerical_meta_data
-        meta_data_tuple = MetaData(**meta_data_copy)
-        return meta_data_tuple
-
     def reverse_transform(self, x_generated):
         """
         Reverses transforms the generated data to the original data format.
 
         Args:
             x_generated: Generated dataset.
 
         Returns:
             Generated data in the original data format.
         """
         all_features = self.numerical_features + self.categorical_features
         if self.num_numerical_features > 0:
-            num_valid_clusters_all = self.meta_data["numerical"]["num_valid_clusters_all"]
+            num_valid_clusters_all = self.metadata["numerical"]["num_valid_clusters_all"]
         if self.num_categorical_features > 0:
-            num_categories_all = self.meta_data["categorical"]["num_categories_all"]
+            num_categories_all = self.metadata["categorical"]["num_categories_all"]
         data = {}
         cat_index = 0       # categorical index
         cont_index = 0      # numerical index
         for index, feature_name in enumerate(all_features):
             # the first n features are numerical
             if index < len(self.numerical_features):
                 alphas = x_generated[:, index]
                 betas = x_generated[:, index + 1 : index + 1 + num_valid_clusters_all[cont_index]]
                 # Recall that betas represent the one hot encoded form of the cluster number
                 cluster_indices = np.argmax(betas, axis=1)
                 # List of cluster means for a feature. contains one value per cluster
-                means = self.meta_data["numerical"][feature_name]["clusters_means"]
+                means = self.metadata["numerical"][feature_name]["clusters_means"]
 
                 # Since each individual element within the cluster is associated with
                 # one of the cluster's mean. We use the `cluster_indices` to get
                 # a list of size len(x) where each element is a mean for the corresponding
                 # element in the feature
                 means = means[cluster_indices]
                 # Do the same for stds
-                stds = self.meta_data["numerical"][feature_name]["clusters_stds"]
+                stds = self.metadata["numerical"][feature_name]["clusters_stds"]
                 stds = stds[cluster_indices]
                 feature = alphas * (self.std_multiplier * stds) + means
                 data[feature_name] = feature
                 cont_index += 1
             else:
                 # if the index is greater than or equal to len(numerical_features),
                 # then the column at hand is categorical
@@ -429,52 +425,59 @@
                 categories_indices = tf.argmax(raw_feature_parts, axis=1)
                 feature = categories[categories_indices]
                 data[feature_name] = feature
                 cat_index += 1
         return pd.DataFrame(data)
 
 
-class DataSampler:
+class CTGANDataSampler:
     """
-    Data Sampler class based on the data sampler class
+    CTGANDataSampler class based on the data sampler class
     in the official CTGAN implementation.
 
     Reference(s):
         https://arxiv.org/abs/1907.00503
         https://github.com/sdv-dev/CTGAN/
 
     Args:
-        batch_size: `int`, default 512, Batch size to use for the dataset.
-        categorical_features: List of categorical features names
-        numerical_features: List of numerical features names
-        meta_data: Namedtuple of features meta data computed during data transformation.
-            You can access it from the `.get_meta_data()` of DataTransformer instance.
+        batch_size: ``int``, default 512,
+            Batch size to use for the dataset.
+
+        categorical_features: ``List[str]``,
+            List of categorical features names
+
+        numerical_features: ```List[str]``,
+            List of numerical features names
+
+        metadata: ``dict``,
+            A dictionary of metadata computed during data transformation.
+            You can access it from the ``.get_metadata()`` of ``CTGANDataTransformer`` instance.
     """
     def __init__(self,
                  batch_size=512,
                  categorical_features=None,
                  numerical_features=None,
-                 meta_data=None):
+                 metadata=None):
         if categorical_features is None:
             raise ValueError("`categorical_features` must not be None. "
                              "CTGAN requires dataset to have atleast one categorical feature, "
                              "if your dataset doesn't contain any categorical features, "
                              "then you should use some other generative model. ")
 
-        if meta_data is None:
-            raise ValueError("`meta_data` must not be None. "
+        if metadata is None:
+            raise ValueError("`metadata` must not be None. "
                              "DataSampler requires meta data computed in the transformation step "
                              "to sample data. "
-                             "Use DataTransformer's `get_meta_data` method to "
+                             "Use DataTransformer's `get_metadata` method to "
                              "access meta data and pass it as argument to DataSampler.")
 
         self.batch_size = batch_size
         self.categorical_features = categorical_features
         self.numerical_features = numerical_features
-        self.meta_data = meta_data
+        self.metadata = metadata
 
         self.num_samples = None
         self.data_dim = None
         self.batch_size = batch_size
         self.row_idx_by_categories = list()
 
     def get_dataset(self,
@@ -485,52 +488,52 @@
             x_transformed: Dataset transformed using DataTransformer class
             x_original: Original Dataset - a pandas DataFrame.
                 It is used for computing categorical values' probabilities
                 for later sampling.
         Returns:
             Returns a tensorflow dataset that utilizes the sample_data method
             to create batches of data. This way user can just pass the dataset object to the fit
-            method of the model and each batch generated will satisfies all out requirements of sampling
+            method of the model and each batch generated will satisfy all out requirements of sampling
         """
         self.num_samples, self.data_dim = x_transformed.shape
         # adapting the approach from the official implementation
         # to sample evenly across the categories to combat imbalance
         row_idx_raw = [x_original.groupby(feature).groups for feature in self.categorical_features]
         self.row_idx_by_categories = tf.ragged.constant([[values.to_list()
                                                           for values in feat.values()]
                                                          for feat in row_idx_raw])
 
-        total_num_categories = self.meta_data.categorical.total_num_categories
+        total_num_categories = self.metadata["categorical"]["total_num_categories"]
 
         dataset = tf.data.Dataset.from_generator(
             self.generator,
             output_signature=(tf.TensorSpec(shape=(self.batch_size, tf.shape(x_transformed)[1]),
                                             name="real_samples"),
                               tf.TensorSpec(shape=(self.batch_size, total_num_categories),
                                             dtype=tf.float32, name="cond_vectors_real"),
                               tf.TensorSpec(shape=(self.batch_size, total_num_categories),
                                             dtype=tf.float32, name="cond_vectors"),
                               tf.TensorSpec(shape=(self.batch_size, len(self.categorical_features)),
                                             dtype=tf.float32, name="mask")),
             args=[x_transformed]
-            )
+        )
         return dataset
 
     def sample_cond_vectors_for_training(self,
-                                        random_features_idx=None,
-                                        random_values_idx=None):
+                                         random_features_idx=None,
+                                         random_values_idx=None):
         # 1. Create Nd zero-filled mask vectors mi = [mi(k)] where k=1...|Di| and for i = 1,...,Nd,
         # so the ith mask vector corresponds to the ith column,
         # and each component is associated to the category of that column.
         masks = tf.zeros([self.batch_size, len(self.categorical_features)])
-        cond_vectors = tf.zeros([self.batch_size, self.meta_data.categorical.total_num_categories])
+        cond_vectors = tf.zeros([self.batch_size, self.metadata["categorical"]["total_num_categories"]])
         # 2. Randomly select a discrete column Di out of all the Nd discrete columns, with equal probability.
         # >>> We select them in generator method
 
-        random_features_relative_indices = tf.gather(self.meta_data.categorical.relative_indices_all,
+        random_features_relative_indices = tf.gather(self.metadata["categorical"]["relative_indices_all"],
                                                      indices=random_features_idx)
 
         # 3. Construct a PMF across the range of values of the column selected in 2, Di* , such that the
         # probability mass of each value is the logarithm of its frequency in that column.
         # >>> Moved to the generator method, which calls this method
         # and passes the value of `random_features_idx`
 
@@ -556,16 +559,16 @@
 
     def sample_cond_vectors_for_generation(self, batch_size):
         """
         The difference between this method and the training one is that, here
         we sample indices purely randomly instead of based on the calculated
         probability as proposed in the paper.
         """
-        num_categories_all = self.meta_data.categorical.num_categories_all
-        cond_vectors = tf.zeros((batch_size, self.meta_data.categorical.total_num_categories))
+        num_categories_all = self.metadata["categorical"]["num_categories_all"]
+        cond_vectors = tf.zeros((batch_size, self.metadata["categorical"]["total_num_categories"]))
         random_features_idx = tf.random.uniform(shape=(batch_size,),
                                                 minval=0, maxval=len(self.categorical_features),
                                                 dtype=tf.int32)
 
         # For each randomly picked feature, we get it's corresponding num_categories
         random_num_categories_all = tf.gather(num_categories_all,
                                               indices=random_features_idx)
@@ -573,15 +576,15 @@
         random_values_idx = [tf.squeeze(tf.random.uniform(shape=(1,),
                                                           minval=0, maxval=num_categories, dtype=tf.int32))
                              for num_categories in random_num_categories_all]
         random_values_idx = tf.stack(random_values_idx)
         # Offset this index by relative index of the feature that it belongs to.
         # because the final cond vector is the concatenation of all features and
         # is just one vector that has the length equal to total_num_categories
-        random_features_relative_indices = tf.gather(self.meta_data.categorical.relative_indices_all,
+        random_features_relative_indices = tf.gather(self.metadata["categorical"]["relative_indices_all"],
                                                      indices=random_features_idx)
         random_values_idx_offsetted =  random_values_idx + tf.cast(random_features_relative_indices, dtype=tf.int32)
         # random_values_idx_offsetted = tf.cast(random_values_idx_offsetted, dtype=tf.int32)
         indices_cond = list(zip(tf.range(batch_size), random_values_idx_offsetted))
         ones = tf.ones(batch_size)
         cond_vectors = tf.tensor_scatter_nd_update(cond_vectors, indices_cond, ones)
         return cond_vectors
@@ -600,16 +603,17 @@
         num_steps_per_epoch = self.num_samples // self.batch_size
         for _ in range(num_steps_per_epoch):
             random_features_idx = tf.random.uniform([self.batch_size], minval=0,
                                                     maxval=len(self.categorical_features),
                                                     dtype=tf.int32)
             # NOTE: We've precomputed the probabilities in the DataTransformer class for each feature already
             # to speed things up.
-            random_features_categories_probs = tf.gather(tf.ragged.constant(self.meta_data.categorical.categories_probs_all),
-                                                         indices=random_features_idx)
+            random_features_categories_probs = tf.gather(
+                tf.ragged.constant(self.metadata["categorical"]["categories_probs_all"]),
+                indices=random_features_idx)
             random_values_idx = [tf_random_choice(np.arange(len(feature_probs)),
                                                   n_samples=1,
                                                   p=feature_probs)
                                  for feature_probs in random_features_categories_probs]
             random_values_idx = tf.cast(tf.squeeze(random_values_idx), dtype=tf.int32)
             # the official implementation uses actual indices during the sample_cond_vector method
             # but uses the shuffled version in sampling data, so we're gonna do just that.
@@ -630,13 +634,13 @@
             # transformed data and cond vector must have one to one feature correspondence.
             # yield x_transformed[sample_idx], shuffled_idx, random_features_idx, random_values_idx
 
             # `cond_vectors` will be first concatenated with the noise
             # vector `z` to create generator input and then will be concatenated
             # with the generated samples to serve as input for discriminator
             cond_vectors, mask = self.sample_cond_vectors_for_training(random_features_idx=random_features_idx,
-                                                                      random_values_idx=random_values_idx)
+                                                                       random_values_idx=random_values_idx)
             # `cond_vectors_real` will be concatenated with the real_samples
             # and passed to the discriminator
             cond_vectors_real = tf.gather(cond_vectors, indices=shuffled_idx)
             real_samples = x_transformed[sample_idx]
             yield real_samples, cond_vectors_real, cond_vectors, mask
```

### Comparing `Teras-0.1.1/teras/preprocessing/gain.py` & `Teras-0.2.0/teras/preprocessing/gain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import tensorflow as tf
 import pandas as pd
 import numpy as np
-from typing import List
 from sklearn.preprocessing import OrdinalEncoder
-from teras.preprocessing.base.base_data_transformer import BaseDataTransformer
+from teras.preprocessing.base.base_data_transformer import BaseDataTransformer as _BaseDataTransformer
+from teras.utils.types import FeaturesNamesType
 
 
-FEATURE_NAMES_TYPE = List[str]
-
-
-class DataTransformer(BaseDataTransformer):
+class GAINDataTransformer(_BaseDataTransformer):
     """
-    DataTransformer class that performs the required transformations
+    GAINDataTransformer class that performs the required transformations
     on the raw dataset required by the GAIN architecture proposed by
     Jinsung Yoon et al. in the paper
     GAIN: Missing Data Imputation using Generative Adversarial Nets.
 
     Reference(s):
         https://arxiv.org/abs/1806.02920
 
     Args:
-        categorical_features: A list of names of categorical features.
+        categorical_features: ``List[str]``,
+            List of categorical features names in the dataset.
             Categorical features are encoded by ordinal encoder method.
             And then MinMax normalization is applied.
-        numerical_features: A list of names of categorical/continuous features.
+
+        numerical_features: ``List[str]``,
+            List of numerical features names in the dataset.
             Numerical features are encoded using MinMax normalization.
 
     Example:
-        ```python
+        .. code-block:: python
+
             input_df = pd.DataFrame(np.arange(10, 3).reshape(20, 5),
-                                    columns=['A', 'B', 'C'])
+                                        columns=['A', 'B', 'C'])
             numerical_features = input_df.columns
             data_transformer = DataTransformer(categorical_features=None,
                                                numerical_features=numerical_features)
             transformed_df = data_transformer.transform(input_df)
-        ```
     """
     def __init__(self,
-                 categorical_features: FEATURE_NAMES_TYPE = None,
-                 numerical_features: FEATURE_NAMES_TYPE = None):
+                 categorical_features: FeaturesNamesType = None,
+                 numerical_features: FeaturesNamesType = None
+                 ):
         super().__init__()
         self.categorical_features = categorical_features
         self.numerical_features = numerical_features
         self.encoder = OrdinalEncoder()
         self.min_vals = None
         self.max_vals = None
 
@@ -68,15 +69,15 @@
 
     def transform(self,
                   x: pd.DataFrame,
                   **kwargs):
         """
         Transforms the data (applying normalization etc)
         and returns a tensorflow dataset.
-        It also stores the meta data of features
+        It also stores the metadata of features
         that is used in the reverse transformation step.
 
         Args:
             x: Data to transform. Must be a pandas DataFrame.
 
         Returns:
             Transformed data.
@@ -138,28 +139,33 @@
             x[self.categorical_features] = self.encoder.inverse_transform(x[self.categorical_features])
 
         # if not return_dataframe:
         #     x = x.values
         return x
 
 
-class DataSampler:
+class GAINDataSampler:
     """
-    DataSampler class that prepares the transformed data in the format
+    GAINDataSampler class that prepares the transformed data in the format
     that is expected and digestible by the GAIN architecture proposed by
     Jinsung Yoon et al. in the paper
     GAIN: Missing Data Imputation using Generative Adversarial Nets.
 
     Reference(s):
         https://arxiv.org/abs/1806.02920
 
     Args:
-        batch_size: default 512, Batch size to use for dataset.
-        shuffle: default True, Whether to shuffle the data.
-        random_seed: default None, Random seed to use when shuffling.
+        batch_size: ``int``, default 512,
+            Batch size to use for dataset.
+
+        shuffle: ``bool``, default True,
+            Whether to shuffle the data.
+
+        random_seed: ``int``, default None,
+            Random seed to use when shuffling.
 
     Example:
         ```python
         input_data = np.random.arange(100).reshape(20, 5)
         data_sampler = DataSampler()
         dataset = data_sampler.get_dataset(input_data)
         ```
@@ -176,15 +182,15 @@
 
         if self.random_seed:
             np.random.seed(self.random_seed)
 
     def get_dataset(self, x_transformed):
         """
         Args:
-            x_transformed: `np.ndarray` or `pd.DataFrame`,
+            x_transformed: ``np.ndarray`` or ``pd.DataFrame``,
                 Transformed dataset.
         Returns:
              A tensorflow dataset, that generates batches of
             size `batch_size` which is the argument passed during
             DataSampler instantiation. The dataset instance then can
             be readily passed to the GAIN fit method without requiring
             any further processing.
@@ -192,15 +198,15 @@
         self.num_samples, self.data_dim = x_transformed.shape
 
         dataset = (tf.data.Dataset
                    .from_generator(self.generator,
                                    output_signature=(
                                        tf.TensorSpec(shape=(None, self.data_dim), dtype=tf.float32, name="x_generator"),
                                        tf.TensorSpec(shape=(None, self.data_dim), dtype=tf.float32, name="x_discriminator"),
-                                        ),
+                                   ),
                                    args=[x_transformed]
                                    )
                    )
         return dataset
 
     def generator(self, x):
         """
```

### Comparing `Teras-0.1.1/teras/preprocessing/oenf.py` & `Teras-0.2.0/teras/preprocessing/oenf.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/preprocessing/pcgain.py` & `Teras-0.2.0/teras/preprocessing/pcgain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,94 @@
 import tensorflow as tf
 import numpy as np
 import pandas as pd
-from teras.preprocessing.gain import DataSampler as GainDataSampler, DataTransformer
+from teras.preprocessing.gain import (GAINDataTransformer as _GAINDataTransformer,
+                                      GAINDataSampler as _GAINDataSampler)
+from teras.utils.types import FeaturesNamesType
 
 
-class DataSampler(GainDataSampler):
+class PCGAINDataTransformer(_GAINDataTransformer):
+    """
+    PCGAINDataTransformer class that performs the required transformations
+    on the raw dataset required by the PCGAIN architecture.
+
+    It is simply a wrapper around the GAINDataTransformer class, as everything
+    is exactly the same.
+
+    Args:
+        categorical_features: ``List[str]``,
+            List of categorical features names in the dataset.
+            Categorical features are encoded by ordinal encoder method.
+            And then MinMax normalization is applied.
+
+        numerical_features: ``List[str]``,
+            List of numerical features names in the dataset.
+            Numerical features are encoded using MinMax normalization.
+    """
+    def __init__(self,
+                 categorical_features: FeaturesNamesType = None,
+                 numerical_features: FeaturesNamesType = None
+                 ):
+        super().__init__(categorical_features=categorical_features,
+                         numerical_features=numerical_features)
+
+
+class PCGAINDataSampler(_GAINDataSampler):
     """
     DataSampler class for PC-GAIN.
     It extends GAIN's DataSampler class because PC-GAIN
     in itself is an extension of GAIN architecture,
     so the data required by them is in similar format.
     But PC-GAIN requires one extra thing -- the pretraining dataset.
     Hence, the need to extend the GAIN Data Sampler class and
     implement that functionality here.
 
     Reference(s):
         https://arxiv.org/abs/2011.07770
 
     Args:
-        batch_size: Batch size to use for dataset.
-            Defaults to 512.
-        shuffle: Whether to shuffle the dataset.
-            Defaults to True.
-        random_seed: Random seed to make shuffling
+        batch_size: ``int``, default 512,
+            Batch size to use for dataset.
+
+        shuffle: ``bool``, default True,
+            Whether to shuffle the dataset.
+
+        random_seed: ``int``, default None,
+            Random seed to make shuffling
             and any other random operations consistent.
     """
     def __init__(self,
                  batch_size=512,
                  shuffle=True,
                  random_seed=None):
         super().__init__(batch_size=batch_size,
                          shuffle=shuffle,
                          random_seed=random_seed)
-        self.batch_size = batch_size
-        self.shuffle = shuffle
-        self.random_seed = random_seed
 
     def get_pretraining_dataset(self,
                                 x_transformed,
-                                pretraining_size=0.2,
-                                batch_size=None):
+                                pretraining_size: float = 0.2,
+                                batch_size: int = None):
         """
         Args:
-            x_transformed: Transformed dataset.
-            pretraining_size: Fraction of dataset that will be used for pretraining.
+            x_transformed:
+                Transformed dataset.
+
+            pretraining_size: ``float``, default 0.2,
+                Fraction of dataset that will be used for pretraining.
                 As a general rule of thumb (based on official implementation),
-                    - for datasets with `num_samples >= 20000`, use `pretraining_size=0.2`
-                    - for datasets with `num_samples < 20000`, use `pretraining_size = 0.4`
+                    - for datasets with ``num_samples >= 20000``, use ``pretraining_size=0.2``
+                    - for datasets with ``num_samples < 20000``, use ``pretraining_size = 0.4``
                 Please note that, this is NOT a hard and fast rule. You can specify
                 whatever fraction size you deem reasonable for your use case.
-            batch_size: In case you want to use a different batch size for your
-                pretraining than for actual training. If None, the batch_size
-                specified while DataSample instantiation will be used.
+
+            batch_size: ``int``,
+                In case you want to use a different batch size for your
+                pretraining than for actual training. If None, the ``batch_size``
+                specified while instantiating ``PCGAINDataSampler`` will be used.
         """
         if batch_size is None:
             batch_size = self.batch_size
 
         # Sort all the samples according to their missing rate and select the top
         # lambda a.k.a. `pretraining_size` samples to make the pretraining dataset.
         # Missing rate in simple terms means,
```

### Comparing `Teras-0.1.1/teras/utils/__init__.py` & `Teras-0.2.0/teras/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,35 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # General purpose utility functions
-from .utils import (tf_random_choice,
-                    get_normalization_layer,
-                    get_categorical_features_cardinalities,
-                    get_activation,
-                    get_initializer,
-                    get_features_metadata_for_embedding,
-                    dataframe_to_tf_dataset,
-                    convert_dict_to_array_tensor,
-                    serialize_layers_collection,
-                    inject_missing_values)
-
-
-# DNFNet utility function(s)
-# Since all the DNFNet utility functions are so specific to the architecture,
-# and some even contain generic names, so it's better not to import them here
-# and rather import them from the path .NetDNF
+from teras.utils.utils import (tf_random_choice,
+                               get_normalization_layer,
+                               get_categorical_features_cardinalities,
+                               get_activation,
+                               get_initializer,
+                               get_features_metadata_for_embedding,
+                               dataframe_to_tf_dataset,
+                               convert_dict_to_array_tensor,
+                               serialize_layers_collection,
+                               deserialize_layers_collection,
+                               inject_missing_values,
+                               generate_fake_gemstone_data)
 
 
 # NODE utility function(s)
-from .node import sparsemoid
+from teras.utils.node import sparsemoid
 
 
 # VIME utility function(s)
-from .vime import (mask_generator as vime_mask_generator,
-                   pretext_generator as vime_pretext_generator,
-                   preprocess_input_vime_self,
-                   preprocess_input_vime_semi)
-
+from teras.utils.vime import (vime_mask_generator,
+                              vime_pretext_generator,
+                              preprocess_input_vime_self,
+                              preprocess_input_vime_semi)
```

### Comparing `Teras-0.1.1/teras/utils/dnfnet.py` & `Teras-0.2.0/teras/utils/dnfnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/utils/pcgain.py` & `Teras-0.2.0/teras/utils/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.1/teras/utils/utils.py` & `Teras-0.2.0/teras/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from tensorflow import keras
 import tensorflow as tf
 from tensorflow.keras import layers, models
 from typing import List, Union, Tuple
 import pandas as pd
 import numpy as np
-
+from warnings import warn
+from teras.utils.types import ActivationType
+from teras import activations
 
 LayerType = Union[str, layers.Layer]
-FEATURE_NAMES_TYPE = Union[List[str], Tuple[str]]
 LAYERS_COLLECTION = Union[List[layers.Layer], layers.Layer, models.Model]
+LAYERS_CONFIGS_COLLECTION = Union[List[dict], dict]
 
 
 def tf_random_choice(inputs,
                      n_samples: int,
                      p: List[float] = None):
     """Tensorflow equivalent of np.random.choice
 
@@ -65,38 +67,56 @@
         normalization_layer = normalization
     else:
         raise ValueError(f"Invalid Normalization value type. Expected type str or keras.layers.Layer"
                          f" Received value {normalization} of type {type(normalization)}")
     return normalization_layer
 
 
-
-def get_activation(activation: LayerType,
-                   units=None):
+def get_activation(activation: ActivationType):
     """
     Retrieves and returns a keras activation function if not already.
 
     Args:
-        activation: default None.
+        activation:
             If type of activation is a keras function, it is returned as is.
             If it is of type, str, that is, it is a name,
-            then relevant activation function is returned
+            then relevant activation function is returned, if it is offered
+            by either ``Teras`` or ``Keras``, otherwise an error is raised.
 
     Returns:
         Keras Activation function
     """
     if isinstance(activation, str):
         activation = activation.lower()
+        # First check if Keras offers that function
         try:
             activation_func = keras.activations.get(activation)
         except ValueError:
-            raise ValueError(f"{activation} function's name is either wrong or this activation is not supported by Keras."
-                             f"Please contact Teras team, and we'll make sure to add this to Teras.")
-    else:
+            # Then check if Teras offers it
+            if activation == "glu":
+                activation_func = activations.glu
+            elif activation == "geglu":
+                activation_func = activations.geglu
+            elif activation == "gumblesoftmax":
+                activation_func = activations.gumbel_softmax
+            elif activation == "sparsemax":
+                activation_func = activations.sparsemax
+            elif activation == "sparsemoid":
+                from teras.utils.node import sparsemoid
+                activation_func = sparsemoid
+            else:
+                # Otherwise return error
+                raise ValueError(f"{activation} function's name is either incorrect "
+                                 f"or this activation is not offered by either Keras and Teras. ")
+    elif callable(activation):
         activation_func = activation
+
+    else:
+        TypeError("Unsupported type for `activation` argument. "
+                  f"Expected type(s): [`str`, `callable`]. Received: {type(activation)}")
     return activation_func
 
 
 def get_initializer(initializer: LayerType):
     """
     Retrieves and returns a keras initializer function if not already.
 
@@ -125,16 +145,14 @@
                                            categorical_features):
     cardinalities = []
     for feature in categorical_features:
         cardinalities.append(dataframe[feature].nunique())
     return cardinalities
 
 
-
-
 def get_features_metadata_for_embedding(dataframe: pd.DataFrame,
                                         categorical_features=None,
                                         numerical_features=None):
     """
     Utility function that create metadata for features in a given dataframe
     required by the Categorical and Numerical embedding layers in Teras.
     For numerical features, it maps each feature name to feature index.
@@ -181,69 +199,44 @@
 
 
 def dataframe_to_tf_dataset(
         dataframe: pd.DataFrame,
         target: Union[str, list] = None,
         shuffle: bool = True,
         batch_size: int = 1024,
-        as_dict: bool = False,
 ):
     """
     Builds a tf.data.Dataset from a given pandas dataframe
 
     Args:
         dataframe: `pd.DataFrame`,
             A pandas dataframe
         target: `str` or `list`,
             Name of the target column or list of names of the target columns.
         shuffle: `bool`, default True
             Whether to shuffle the dataset
         batch_size: `int`, default 1024,
             Batch size
-        as_dict: `bool`, default False,
-            Whether to make a tensorflow dataset in a dictionary format
-            where each record is a mapping of features names against their values.
-
-            SOME GUIDELINES on when to create dataset in dictionary format and when not:
-            1. If your dataset is composed of heterogeneous data formats, i.e. it contains
-                features where some features contain integers/floats AND others contain strings,
-                and you don't want to manually encode the string values into integers/floats,
-                then your dataset must be in dictionary format, which you can get by setting
-                the `as_dict` parameter to `True`.
-
 
     Returns:
          A tf.data.Dataset dataset
     """
     df = dataframe.copy()
     if target is not None:
         if isinstance(target, (list, tuple, set)):
-            if as_dict:
-                labels = dict()
-                for feat in target:
-                    labels[feat] = df.pop(feat).values
-            else:
-                labels = []
-                for feat in target:
-                    labels.append(df.pop(feat).values)
-                labels = tf.transpose(tf.constant(labels))
+            labels = []
+            for feat in target:
+                labels.append(df.pop(feat).values)
+            labels = tf.transpose(tf.constant(labels))
         else:
             labels = df.pop(target)
-            if not as_dict:
-                labels = labels.values
-        if as_dict:
-            dataset = tf.data.Dataset.from_tensor_slices((dict(df), labels))
-        else:
-            df = df.values
-            dataset = tf.data.Dataset.from_tensor_slices((df, labels))
+            labels = labels.values
+        dataset = tf.data.Dataset.from_tensor_slices((df.values, labels))
     else:
-        if as_dict:
-            dataset = tf.data.Dataset.from_tensor_slices(dict(df))
-        else:
-            dataset = tf.data.Dataset.from_tensor_slices(df.values)
+        dataset = tf.data.Dataset.from_tensor_slices(df.values)
     if shuffle:
         dataset = dataset.shuffle(buffer_size=len(dataframe))
     dataset = dataset.batch(batch_size)
     dataset = dataset.prefetch(batch_size)
     return dataset
 
 
@@ -254,27 +247,22 @@
     Args:
         dict_tensor: A batch of data taken from tensorflow dictionary format dataset.
 
     Returns:
         Array format data.
     """
     if not isinstance(dict_tensor, dict):
-        print("Given tensor is not in dictionary format. Hence no processing will be applied. \n"
-              f"Expected type: {dict}, Received type: {type(dict_tensor)}")
+        warn("Given tensor is not in dictionary format. Hence no processing will be applied. \n"
+             f"Expected type: {dict}, Received type: {type(dict_tensor)}")
         return
 
     feature_names = dict_tensor.keys()
-    array_tensor = tf.TensorArray(size=len(feature_names),
-                                  dtype=tf.float32)
-    for idx, feature_name in enumerate(feature_names):
-        feature = tf.expand_dims(tf.cast(dict_tensor[feature_name], dtype=tf.float32), 1)
-        array_tensor = array_tensor.write(idx, feature)
-
-    array_tensor = tf.transpose(tf.squeeze(array_tensor.stack()))
-    array_tensor.set_shape((None, len(feature_names)))
+    array_tensor = [tf.expand_dims(dict_tensor[feature_name], axis=1)
+                    for feature_name in feature_names]
+    array_tensor = tf.concat(array_tensor, axis=1)
     return array_tensor
 
 
 def serialize_layers_collection(layers_collection: LAYERS_COLLECTION):
     """
     Serializes a collection of keras layers/models.
 
@@ -282,20 +270,39 @@
         If layers_collection is an instance of list or tuple, it returns a list of serialized layers
         otherwise it simply returns the serialized layer or model.
     """
     if isinstance(layers_collection, (list, tuple)):
         layers_collection_serialized = [keras.layers.serialize(layer)
                                         for layer in layers_collection]
     else:
-        # We assume it's either of type Layer or Model
+        # We assume it's either of type Layer or Model, or None
         layers_collection_serialized = keras.layers.serialize(layers_collection)
 
     return layers_collection_serialized
 
 
+def deserialize_layers_collection(layers_configs_collection: LAYERS_CONFIGS_COLLECTION):
+    """
+    De-serializes a collection of keras layers/models configs.
+
+    Returns:
+        If layers_configs_collection is a list of layers config dictionaries, it returns a
+        list of de-serialized layers otherwise if it's a config dictionary, it returns the
+         de-serialized layer or model.
+    """
+    if isinstance(layers_configs_collection, list):
+        layers_collection_deserialized = [keras.layers.deserialize(layer)
+                                          for layer in layers_configs_collection]
+    else:
+        # We assume it's either a dict or None
+        layers_collection_deserialized = keras.layers.deserialize(layers_configs_collection)
+
+    return layers_collection_deserialized
+
+
 def inject_missing_values(x: pd.DataFrame,
                           miss_rate=0.1,
                           return_dataframe=True):
     """
     Injects missing (np.nan) values in the given dataset.
 
     Args:
@@ -323,8 +330,30 @@
 
     mask = np.random.binomial(1, 1-miss_rate, size=x.shape)
     x_with_missing_data[mask == 0] = np.nan
 
     if return_dataframe:
         x_with_missing_data = pd.DataFrame(x_with_missing_data,
                                            columns=x.columns if is_dataframe else None)
-    return x_with_missing_data
+    return x_with_missing_data
+
+
+def generate_fake_gemstone_data(num_samples: int = 16):
+    """
+    Generate fake gemstone like data of specified num_samples.
+
+    Args:
+        num_samples:
+            Number of samples to generate
+
+    Returns:
+        A pandas DataFrame of fake gemstone like data.
+    """
+    fake_gem_df = pd.DataFrame({
+        "cut": np.random.randint(low=0, high=3, size=(num_samples,)),
+        "color": np.random.randint(low=0, high=5, size=(num_samples,)),
+        "clarity": np.random.randint(low=0, high=4, size=(num_samples,)),
+        "depth": np.random.randint(low=0, high=100, size=(num_samples,)),
+        "table": np.random.randint(low=0, high=100, size=(num_samples,))
+    })
+    fake_gem_df = fake_gem_df.astype(np.float32)
+    return fake_gem_df
```

### Comparing `Teras-0.1.1/teras/utils/vime.py` & `Teras-0.2.0/teras/utils/vime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 import tensorflow as tf
 
 
 @tf.function
-def mask_generator(p_m, x):
+def vime_mask_generator(x,
+                        p_m: float = 0.3):
     """
     Generates mask vector for self and semi-supervised learning
     Args:
-        p_m: corruption probability
-        x: feature matrix
+        x:
+            Dataset.
+
+        p_m: ``float``, default 0.3,
+            Corruption probability
 
     Returns:
         mask: binary mask matrix
 
     """
     mask = tf.random.stateless_binomial(shape=tf.shape(x),
-                                           seed=(0, 0),
-                                           counts=1,
-                                           probs=p_m,
-                                           output_dtype=tf.float32)
+                                        seed=(0, 0),
+                                        counts=1,
+                                        probs=p_m,
+                                        output_dtype=tf.float32)
     return mask
 
+
 @tf.function
-def pretext_generator(m, x):
+def vime_pretext_generator(x, mask):
     """
     Generates corrupted samples for self and semi-supervised learning
 
     Args:
-        m: mask matrix
-        x: feature matrix
-        batch_size: When X is passed from within the keras model during training, its batch dimension is none, to handle
-        that particular case, pass batch_size explicity
+        x:
+            Dataset.
+
+        mask:
+            Mask matrix
 
     Returns:
-        m_new: final mask matrix after corruption
-        x_tilde: corrupted feature matrix
+        mask_corrupted: Final mask matrix after corruption
+        x_tilde: Corrupted feature matrix
     """
     x = tf.cast(x, dtype=tf.float32)
     num_samples = tf.shape(x)[0]
     dim = tf.shape(x)[1]
 
     x_bar = tf.TensorArray(size=dim, dtype=tf.float32)
     for i in range(dim):
         idx = tf.random.shuffle(tf.range(num_samples))
         x_bar = x_bar.write(i, tf.gather(x[:, i], idx))
     x_bar = tf.transpose(x_bar.stack())
 
     # Corrupt Samples
-    x_tilde = x * (1 - m) + x_bar * m
+    x_tilde = x * (1 - mask) + x_bar * mask
 
     m_new = (x != x_tilde)
     m_new = tf.cast(m_new, dtype="float32")
     return m_new, x_tilde
 
 
 def preprocess_input_vime_semi(x_labeled,
-                         y_labeled,
-                         x_unlabeled,
-                         batch_size=None):
+                               y_labeled,
+                               x_unlabeled,
+                               batch_size=None):
     """
     VIME's semi supervised training requires a labeled and an unlabeled training set.
     It also allows user to specify the unlabeled/labeled split.
     Hence, the labeled and unlabeled dataset sizes will almost always differ.
     And here's the issue, Keras's default fit method will raise incompatible input cardinalities error
     if we try to pass labeled and unlabeled datasets to `x` parameter as a dict and pass labeled targets to `y`
     To allow for varying sizes for labeled and unlabeled dataset, this function comes to clutch.
@@ -121,17 +127,17 @@
         batch_size: Batch size
 
     Returns:
         TensorFlow dataset
     """
 
     if m_labeled is None and x_tilde is None:
-        m_unlabeled = mask_generator(p_m,
-                                     x_unlabeled)
-        m_labeled, x_tilde = pretext_generator(m_unlabeled, x_unlabeled)
+        m_unlabeled = vime_mask_generator(p_m,
+                                          x_unlabeled)
+        m_labeled, x_tilde = vime_pretext_generator(m_unlabeled, x_unlabeled)
 
     dataset = tf.data.Dataset.from_tensor_slices((x_tilde,
                                                   {"mask_estimator": m_labeled, "feature_estimator": x_unlabeled}))
 
     if batch_size is not None:
         dataset = dataset.batch(batch_size=batch_size)
```

