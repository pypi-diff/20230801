# Comparing `tmp/score_models-0.4.7.tar.gz` & `tmp/score_models-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_models-0.4.7.tar", last modified: Tue Aug  1 01:52:57 2023, max compression
+gzip compressed data, was "score_models-0.4.8.tar", last modified: Tue Aug  1 05:47:21 2023, max compression
```

## Comparing `score_models-0.4.7.tar` & `score_models-0.4.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.238483 score_models-0.4.7/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.7/LICENSE.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-01 01:52:57.238483 score_models-0.4.7/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.7/README.md
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.7/pyproject.toml
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.230483 score_models-0.4.7/score_models/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.230483 score_models-0.4.7/score_models/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.7/score_models/architectures/ddpm.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/architectures/mlp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/architectures/ncsnpp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    21045 2023-08-01 01:51:56.000000 score_models-0.4.7/score_models/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/definitions.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      517 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/dsm.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.238483 score_models-0.4.7/score_models/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      688 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/attention_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/combine.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/conditional_batchnorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/conditional_instancenorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/conditional_instancenorm2d_plus.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2874 2023-07-31 23:56:34.000000 score_models-0.4.7/score_models/layers/conv1dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3090 2023-07-31 23:56:24.000000 score_models-0.4.7/score_models/layers/conv2dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3141 2023-08-01 00:07:03.000000 score_models-0.4.7/score_models/layers/conv3dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/conv_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/ddpm_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/downsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/ncsn_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/projection_embedding.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/resnet_block_biggan.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/spectral_normalization.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/squeeze_and_excitation.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/style_gan_conv.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/up_or_downsampling.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/up_or_downsampling1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/up_or_downsampling2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/up_or_downsampling3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/upfirdn1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/upfirdn2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/upfirdn3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/upsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2713 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/score_model.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.238483 score_models-0.4.7/score_models/sde/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/sde/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1520 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/sde/sde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2184 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/sde/vesde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1641 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/sde/vpsde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3102 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/sliced_score_matching.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4128 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/utils.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.230483 score_models-0.4.7/score_models.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1784 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/top_level.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-01 01:52:57.238483 score_models-0.4.7/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-31 23:38:29.000000 score_models-0.4.7/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.238483 score_models-0.4.7/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-22 02:58:16.000000 score_models-0.4.7/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7729 2023-07-31 23:38:29.000000 score_models-0.4.7/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.7/tests/test_score_models.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.7/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.482461 score_models-0.4.8/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.8/LICENSE.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-01 05:47:21.482461 score_models-0.4.8/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.8/README.md
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.8/pyproject.toml
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.474461 score_models-0.4.8/score_models/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.474461 score_models-0.4.8/score_models/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.8/score_models/architectures/ddpm.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/architectures/mlp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/architectures/ncsnpp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20889 2023-08-01 05:40:23.000000 score_models-0.4.8/score_models/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/definitions.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      517 2023-08-01 05:47:04.000000 score_models-0.4.8/score_models/dsm.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.482461 score_models-0.4.8/score_models/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      688 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/attention_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/combine.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/conditional_batchnorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/conditional_instancenorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/conditional_instancenorm2d_plus.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2874 2023-08-01 03:24:14.000000 score_models-0.4.8/score_models/layers/conv1dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3090 2023-08-01 03:24:14.000000 score_models-0.4.8/score_models/layers/conv2dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3141 2023-08-01 03:24:14.000000 score_models-0.4.8/score_models/layers/conv3dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/conv_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/ddpm_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/downsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/ncsn_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/projection_embedding.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/resnet_block_biggan.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/spectral_normalization.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/squeeze_and_excitation.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/style_gan_conv.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/up_or_downsampling.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/up_or_downsampling1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/up_or_downsampling2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/up_or_downsampling3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/upfirdn1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/upfirdn2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/upfirdn3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/upsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2713 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/score_model.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.482461 score_models-0.4.8/score_models/sde/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/sde/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1520 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/sde/sde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2184 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/sde/vesde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1641 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/sde/vpsde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3102 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/sliced_score_matching.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4128 2023-08-01 03:00:20.000000 score_models-0.4.8/score_models/utils.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.474461 score_models-0.4.8/score_models.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1784 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/top_level.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-01 05:47:21.486461 score_models-0.4.8/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-08-01 05:45:39.000000 score_models-0.4.8/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.482461 score_models-0.4.8/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-22 02:58:16.000000 score_models-0.4.8/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7729 2023-07-31 23:38:29.000000 score_models-0.4.8/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.8/tests/test_score_models.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.8/tests/test_training.py
```

### Comparing `score_models-0.4.7/LICENSE.txt` & `score_models-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/PKG-INFO` & `score_models-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score_models
-Version: 0.4.7
+Version: 0.4.8
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `score_models-0.4.7/README.md` & `score_models-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/architectures/ddpm.py` & `score_models-0.4.8/score_models/architectures/ddpm.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/architectures/mlp.py` & `score_models-0.4.8/score_models/architectures/mlp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/architectures/ncsnpp.py` & `score_models-0.4.8/score_models/architectures/ncsnpp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/base.py` & `score_models-0.4.8/score_models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,27 +165,33 @@
         """
         n: Number of samples to draw
         shape: Shape of the tensor to sample, except batch dimension.
         steps: Number of Euler-Maruyam steps to perform
         likelihood_score_fn: Add an additional drift to the sampling for posterior sampling. Must have the signature f(t, x)
         guidance_factor: Multiplicative factor for the likelihood drift
         """
+        sampling_from = "prior" if likelihood_score_fn is None else "posterior"
         if likelihood_score_fn is None:
             likelihood_score_fn = lambda t, x: 0.
         # A simple Euler-Maruyama integration of the model SDE
         x = self.sde.prior(shape).sample([n]).to(self.device)
         dt = -self.sde.T / steps
         t = torch.ones(n).to(self.device) * self.sde.T
-        for _ in tqdm(range(steps)):
+        for _ in (pbar := tqdm(range(steps))):
+            pbar.set_description(f"Sampling from the {sampling_from} | t = {t[0].item():.1f} | sigma = {self.sde.sigma(t)[0].item():.1e}"
+                                 f"| scale ~ {x.max().item():.1e}")
             g = self.sde.diffusion(t, x)
             f = self.sde.drift(t, x) - g**2 * (self.score(t, x) + guidance_factor * likelihood_score_fn(t, x))
             dw = torch.randn_like(x) * (-dt)**(1/2)
             x_mean = x + f * dt
             x = x_mean + g * dw 
             t += dt
+            if torch.any(torch.isnan(x)):
+                print("Diffusion is not stable, NaN were produced. Stopped sampling.")
+                break
         return x_mean
 
     def loss_fn(self, x, *args, **kwargs):
         B, *D = x.shape
         broadcast = [B, *[1] * len(D)]
         z = torch.randn_like(x)
         t = torch.rand(B).to(self.device) * (self.sde.T - self.sde.epsilon) + self.sde.epsilon
@@ -220,17 +226,14 @@
         verbose=0
     ):
         """
         Train the model on the provided dataset.
 
         Parameters:
             dataset (torch.utils.data.Dataset): The training dataset.
-            dataset_path (str, optional): The path to the dataset file. If not provided, the function will assume a default path. Default is None.
-            dataset_extension (str, optional): The extension of the dataset file. Default is "h5".
-            dataset_key (str, optional): The key or identifier for the specific dataset within the file. If not provided, the function will assume a default key. Defaul
             preprocessing_fn (function, optional): A function to preprocess the input data. Default is None.
             learning_rate (float, optional): The learning rate for optimizer. Default is 1e-4.
             ema_decay (float, optional): The decay rate for Exponential Moving Average. Default is 0.9999.
             batch_size (int, optional): The batch size for training. Default is 1.
             shuffle (bool, optional): Whether to shuffle the dataset during training. Default is False.
             epochs (int, optional): The number of epochs for training. Default is 100.
             patience (float, optional): The patience value for early stopping. Default is infinity.
@@ -288,17 +291,14 @@
         if checkpoints_directory is not None or logdir is not None:
             save_checkpoint = True
             if checkpoints_directory is None: # the way to create a new directory is using logdir
                 checkpoints_directory = os.path.join(logdir, logname)
                 with open(os.path.join(checkpoints_directory, "script_params.json"), "w") as f:
                     json.dump(
                         {
-                            "dataset_path": dataset_path,
-                            "dataset_extension": dataset_extension,
-                            "dataset_key": dataset_extension,
                             "preprocessing": preprocessing_name,
                             "learning_rate": learning_rate,
                             "ema_decay": ema_decay,
                             "batch_size": batch_size,
                             "shuffle": shuffle,
                             "epochs": epochs,
                             "patience": patience,
```

### Comparing `score_models-0.4.7/score_models/definitions.py` & `score_models-0.4.8/score_models/definitions.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/dsm.py` & `score_models-0.4.8/score_models/dsm.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/__init__.py` & `score_models-0.4.8/score_models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/attention_block.py` & `score_models-0.4.8/score_models/layers/attention_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/combine.py` & `score_models-0.4.8/score_models/layers/combine.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/conditional_batchnorm2d.py` & `score_models-0.4.8/score_models/layers/conditional_batchnorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/conditional_instancenorm2d.py` & `score_models-0.4.8/score_models/layers/conditional_instancenorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/conditional_instancenorm2d_plus.py` & `score_models-0.4.8/score_models/layers/conditional_instancenorm2d_plus.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/conv1dsame.py` & `score_models-0.4.8/score_models/layers/conv1dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/conv2dsame.py` & `score_models-0.4.8/score_models/layers/conv2dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/conv3dsame.py` & `score_models-0.4.8/score_models/layers/conv3dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/conv_layers.py` & `score_models-0.4.8/score_models/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/ddpm_resnet_block.py` & `score_models-0.4.8/score_models/layers/ddpm_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/downsample.py` & `score_models-0.4.8/score_models/layers/downsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/ncsn_resnet_block.py` & `score_models-0.4.8/score_models/layers/ncsn_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/projection_embedding.py` & `score_models-0.4.8/score_models/layers/projection_embedding.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/resnet_block_biggan.py` & `score_models-0.4.8/score_models/layers/resnet_block_biggan.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/spectral_normalization.py` & `score_models-0.4.8/score_models/layers/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/squeeze_and_excitation.py` & `score_models-0.4.8/score_models/layers/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/style_gan_conv.py` & `score_models-0.4.8/score_models/layers/style_gan_conv.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/up_or_downsampling.py` & `score_models-0.4.8/score_models/layers/up_or_downsampling.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/up_or_downsampling1d.py` & `score_models-0.4.8/score_models/layers/up_or_downsampling1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/up_or_downsampling2d.py` & `score_models-0.4.8/score_models/layers/up_or_downsampling2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/up_or_downsampling3d.py` & `score_models-0.4.8/score_models/layers/up_or_downsampling3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/upfirdn1d.py` & `score_models-0.4.8/score_models/layers/upfirdn1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/upfirdn2d.py` & `score_models-0.4.8/score_models/layers/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/upfirdn3d.py` & `score_models-0.4.8/score_models/layers/upfirdn3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/layers/upsample.py` & `score_models-0.4.8/score_models/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/score_model.py` & `score_models-0.4.8/score_models/score_model.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/sde/sde.py` & `score_models-0.4.8/score_models/sde/sde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/sde/vesde.py` & `score_models-0.4.8/score_models/sde/vesde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/sde/vpsde.py` & `score_models-0.4.8/score_models/sde/vpsde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/sliced_score_matching.py` & `score_models-0.4.8/score_models/sliced_score_matching.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models/utils.py` & `score_models-0.4.8/score_models/utils.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/score_models.egg-info/PKG-INFO` & `score_models-0.4.8/score_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score-models
-Version: 0.4.7
+Version: 0.4.8
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `score_models-0.4.7/score_models.egg-info/SOURCES.txt` & `score_models-0.4.8/score_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/setup.py` & `score_models-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name="score_models",
-	version="0.4.7",
+	version="0.4.8",
     description="A simple pytorch interface for score model and basic diffusion.",
     long_description=long_description,
     author="Alexandre Adam",
     author_email="alexandre.adam@umontreal.ca",
     url="https://github.com/AlexandreAdam/torch_score_models",
     packages=find_packages(),
     install_requires=[
```

### Comparing `score_models-0.4.7/tests/test_architectures.py` & `score_models-0.4.8/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/tests/test_layers.py` & `score_models-0.4.8/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/tests/test_score_models.py` & `score_models-0.4.8/tests/test_score_models.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.7/tests/test_training.py` & `score_models-0.4.8/tests/test_training.py`

 * *Files identical despite different names*

