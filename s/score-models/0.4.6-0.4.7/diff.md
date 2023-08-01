# Comparing `tmp/score_models-0.4.6.tar.gz` & `tmp/score_models-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/score_models-0.4.6.tar", last modified: Sat Jul 22 03:22:26 2023, max compression
+gzip compressed data, was "score_models-0.4.7.tar", last modified: Tue Aug  1 01:52:57 2023, max compression
```

## Comparing `score_models-0.4.6.tar` & `score_models-0.4.7.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.6/LICENSE.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7415 2023-07-22 03:22:26.000000 score_models-0.4.6/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.6/README.md
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.6/pyproject.toml
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.6/score_models/architectures/ddpm.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/architectures/mlp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/architectures/ncsnpp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20765 2023-07-22 03:21:43.000000 score_models-0.4.6/score_models/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/definitions.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/attention_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/combine.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conditional_batchnorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conditional_instancenorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conditional_instancenorm2d_plus.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conv1dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/conv2dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/conv3dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/conv_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/ddpm_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/downsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/ncsn_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/projection_embedding.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/resnet_block_biggan.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/spectral_normalization.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.6/score_models/layers/squeeze_and_excitation.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/style_gan_conv.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/up_or_downsampling.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/up_or_downsampling1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/up_or_downsampling2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/up_or_downsampling3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/upfirdn1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/upfirdn2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/upfirdn3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/layers/upsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1647 2023-07-17 04:57:57.000000 score_models-0.4.6/score_models/score_model.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models/sde/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.6/score_models/sde/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1348 2023-07-13 23:11:59.000000 score_models-0.4.6/score_models/sde/sde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2110 2023-07-13 23:11:59.000000 score_models-0.4.6/score_models/sde/vesde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1577 2023-07-13 23:11:59.000000 score_models-0.4.6/score_models/sde/vpsde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3101 2023-07-18 01:20:38.000000 score_models-0.4.6/score_models/sliced_score_matching.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4128 2023-07-22 03:19:51.000000 score_models-0.4.6/score_models/utils.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7415 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1764 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-22 03:22:26.000000 score_models-0.4.6/score_models.egg-info/top_level.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-22 03:22:26.000000 score_models-0.4.6/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-22 03:22:04.000000 score_models-0.4.6/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-22 03:22:26.000000 score_models-0.4.6/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-22 02:58:16.000000 score_models-0.4.6/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 13:52:30.000000 score_models-0.4.6/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.6/tests/test_score_models.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.6/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.238483 score_models-0.4.7/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.7/LICENSE.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-01 01:52:57.238483 score_models-0.4.7/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.7/README.md
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.7/pyproject.toml
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.230483 score_models-0.4.7/score_models/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.230483 score_models-0.4.7/score_models/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.7/score_models/architectures/ddpm.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/architectures/mlp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/architectures/ncsnpp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    21045 2023-08-01 01:51:56.000000 score_models-0.4.7/score_models/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/definitions.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      517 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/dsm.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.238483 score_models-0.4.7/score_models/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      688 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/attention_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/combine.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/conditional_batchnorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/conditional_instancenorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/conditional_instancenorm2d_plus.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2874 2023-07-31 23:56:34.000000 score_models-0.4.7/score_models/layers/conv1dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3090 2023-07-31 23:56:24.000000 score_models-0.4.7/score_models/layers/conv2dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3141 2023-08-01 00:07:03.000000 score_models-0.4.7/score_models/layers/conv3dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/conv_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/ddpm_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/downsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/ncsn_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/projection_embedding.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/resnet_block_biggan.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/spectral_normalization.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.7/score_models/layers/squeeze_and_excitation.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/style_gan_conv.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/up_or_downsampling.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/up_or_downsampling1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/up_or_downsampling2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/up_or_downsampling3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/upfirdn1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/upfirdn2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/upfirdn3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/layers/upsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2713 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/score_model.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.238483 score_models-0.4.7/score_models/sde/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.7/score_models/sde/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1520 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/sde/sde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2184 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/sde/vesde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1641 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/sde/vpsde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3102 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/sliced_score_matching.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4128 2023-07-31 23:38:29.000000 score_models-0.4.7/score_models/utils.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.230483 score_models-0.4.7/score_models.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1784 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-08-01 01:52:57.000000 score_models-0.4.7/score_models.egg-info/top_level.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-01 01:52:57.238483 score_models-0.4.7/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-31 23:38:29.000000 score_models-0.4.7/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 01:52:57.238483 score_models-0.4.7/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-22 02:58:16.000000 score_models-0.4.7/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7729 2023-07-31 23:38:29.000000 score_models-0.4.7/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.7/tests/test_score_models.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.7/tests/test_training.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `score_models-0.4.6/LICENSE.txt` & `score_models-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/PKG-INFO` & `score_models-0.4.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,160 +1,159 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: score_models
-Version: 0.4.6
+Version: 0.4.7
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
-License: UNKNOWN
-Description: =========================
-        Score Models for Pytorch
-        =========================
-        
-        .. image:: https://badge.fury.io/py/score_models.svg
-           :target: https://badge.fury.io/py/score_models
-        .. image:: https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg
-           :target: https://codecov.io/gh/AlexandreAdam/torch_score_models
-        
-        A storage for score-based models. The `ScoreModel` interface gives access to the following utilities:
-        
-        - Simple initialization of MLP, NCSN++ and DDPM neural network architectures
-        - A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
-        - A sampling method based on an Euler-Maruyama discretization of an SDE.
-        - A simple interface to train an energy model using DSM
-        
-        This repository is mainly intended for personal use.
-        You might also want to refer to the original implementation at `https://github.com/yang-song/score_sde <https://github.com/yang-song/score_sde>`_.
-        
-        Installation
-        ------------
-        
-        To install the package, you can use pip:
-        
-        .. code-block:: bash
-        
-           pip install torch-score-models
-        
-        Usage
-        -----
-        
-        ScoreModel
-        ~~~~~~~~~~
-        
-        The `ScoreModel` class is the main interface for training and using score models, defined as
-        
-        .. math::
-        
-           \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
-        
-        where :math:`\sigma(t)` is the standard deviation of the perturbation kernel :math:`p_t(\mathbf{x} \mid \mathbf{x}_0)`
-        of an SDE.
-        
-        The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
-        
-        .. code-block:: python
-        
-           from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
-        
-           # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
-           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
-           model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
-           # ... or the VPSDE
-           model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
-        
-           # NN Architectures support a Unet with 1D convolutions for time series input data
-           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
-           # ... or 3D convolutions for videos/voxels
-           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
-           # You can also use a simpler MLP architecture
-           net = MLP(dimensions=dim, layers=4, units=100)
-           # ... or Jonathan Ho's DDPM architecture
-           net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
-        
-           # Train the model
-           model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
-        
-           # Generate samples from the trained model
-           samples = model.sample(size=[batch_size, *dimensions], N=1000)
-        
-           # Compute the score for a given input
-           score = model.score(t, x)
-        
-           # Initialize the score model and its neural network from a path to a checkpoint directory
-           score = ScoreModel(checkpoint_directory)
-        
-        EnergyModel
-        ~~~~~~~~~~~
-        
-        The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the
-        automatic differentiation of an energy model
-        
-        .. math::
-        
-           E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^2
-        
-        This is to say that the score is defined as
-        
-        .. math::
-        
-           \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
-        
-        **Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
-        neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network
-        architecture to be a function :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}` instead of :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}^d`. An `output_activation` like `relu`
-        can also be specified to make the energy positive or bounded from below.
-        
-        Training Parameters
-        ~~~~~~~~~~~~~~~~~~~
-        
-        When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
-        
-        - `dataset`: The training dataset (`torch.utils.data.Dataset`).
-        - `epochs`: The number of training epochs.
-        - `learning_rate`: The learning rate for the ADAM optimizer.
-        - `batch_size`: The batch size for training.
-        - `checkpoints_directory`: The directory to save model checkpoints (default: None).
-        - `seed`: The random seed for numpy and torch.
-        
-        Refer to the method's docstring or the class definition for more details on available parameters.
-        
-        Citations
-        ---------
-        
-        If you use this package in your research, please consider citing the following papers:
-        
-        .. code-block:: bibtex
-        
-           @inproceedings{NEURIPS2020_4c5bcfec,
-               author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
-               booktitle   = {Advances in Neural Information Processing Systems},
-               editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
-               pages       = {6840--6851},
-               publisher   = {Curran Associates, Inc.},
-               title       = {Denoising Diffusion Probabilistic Models},
-               url         = {https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf},
-               volume      = {33},
-               year        = {2020}
-           }
-        
-           @inproceedings{song2021scorebased,
-             title={Score-Based Generative Modeling through Stochastic Differential Equations},
-             author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
-             booktitle={International Conference on Learning Representations},
-             year={2021},
-             url={https://openreview.net/forum?id=PxTIG12RRHS}
-           }
-        
-        License
-        -------
-        
-        This package is licensed under the MIT License.
-        
-        You can save the above content in an `.rst` file, such as `README.rst`, and include it in your project's root directory.
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
+License-File: LICENSE.txt
+
+=========================
+Score Models for Pytorch
+=========================
+
+.. image:: https://badge.fury.io/py/score_models.svg
+   :target: https://badge.fury.io/py/score_models
+.. image:: https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg
+   :target: https://codecov.io/gh/AlexandreAdam/torch_score_models
+
+A storage for score-based models. The `ScoreModel` interface gives access to the following utilities:
+
+- Simple initialization of MLP, NCSN++ and DDPM neural network architectures
+- A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
+- A sampling method based on an Euler-Maruyama discretization of an SDE.
+- A simple interface to train an energy model using DSM
+
+This repository is mainly intended for personal use.
+You might also want to refer to the original implementation at `https://github.com/yang-song/score_sde <https://github.com/yang-song/score_sde>`_.
+
+Installation
+------------
+
+To install the package, you can use pip:
+
+.. code-block:: bash
+
+   pip install torch-score-models
+
+Usage
+-----
+
+ScoreModel
+~~~~~~~~~~
+
+The `ScoreModel` class is the main interface for training and using score models, defined as
+
+.. math::
+
+   \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
+
+where :math:`\sigma(t)` is the standard deviation of the perturbation kernel :math:`p_t(\mathbf{x} \mid \mathbf{x}_0)`
+of an SDE.
+
+The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
+
+.. code-block:: python
+
+   from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
+
+   # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
+   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
+   model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
+   # ... or the VPSDE
+   model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
+
+   # NN Architectures support a Unet with 1D convolutions for time series input data
+   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
+   # ... or 3D convolutions for videos/voxels
+   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
+   # You can also use a simpler MLP architecture
+   net = MLP(dimensions=dim, layers=4, units=100)
+   # ... or Jonathan Ho's DDPM architecture
+   net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
+
+   # Train the model
+   model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
+
+   # Generate samples from the trained model
+   samples = model.sample(size=[batch_size, *dimensions], N=1000)
+
+   # Compute the score for a given input
+   score = model.score(t, x)
+
+   # Initialize the score model and its neural network from a path to a checkpoint directory
+   score = ScoreModel(checkpoint_directory)
+
+EnergyModel
+~~~~~~~~~~~
+
+The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the
+automatic differentiation of an energy model
+
+.. math::
+
+   E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^2
+
+This is to say that the score is defined as
+
+.. math::
+
+   \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
+
+**Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
+neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network
+architecture to be a function :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}` instead of :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}^d`. An `output_activation` like `relu`
+can also be specified to make the energy positive or bounded from below.
+
+Training Parameters
+~~~~~~~~~~~~~~~~~~~
+
+When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
+
+- `dataset`: The training dataset (`torch.utils.data.Dataset`).
+- `epochs`: The number of training epochs.
+- `learning_rate`: The learning rate for the ADAM optimizer.
+- `batch_size`: The batch size for training.
+- `checkpoints_directory`: The directory to save model checkpoints (default: None).
+- `seed`: The random seed for numpy and torch.
+
+Refer to the method's docstring or the class definition for more details on available parameters.
+
+Citations
+---------
+
+If you use this package in your research, please consider citing the following papers:
+
+.. code-block:: bibtex
+
+   @inproceedings{NEURIPS2020_4c5bcfec,
+       author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
+       booktitle   = {Advances in Neural Information Processing Systems},
+       editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
+       pages       = {6840--6851},
+       publisher   = {Curran Associates, Inc.},
+       title       = {Denoising Diffusion Probabilistic Models},
+       url         = {https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf},
+       volume      = {33},
+       year        = {2020}
+   }
+
+   @inproceedings{song2021scorebased,
+     title={Score-Based Generative Modeling through Stochastic Differential Equations},
+     author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
+     booktitle={International Conference on Learning Representations},
+     year={2021},
+     url={https://openreview.net/forum?id=PxTIG12RRHS}
+   }
+
+License
+-------
+
+This package is licensed under the MIT License.
+
+You can save the above content in an `.rst` file, such as `README.rst`, and include it in your project's root directory.
+
```

### Comparing `score_models-0.4.6/README.md` & `score_models-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/architectures/ddpm.py` & `score_models-0.4.7/score_models/architectures/ddpm.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/architectures/mlp.py` & `score_models-0.4.7/score_models/architectures/mlp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/architectures/ncsnpp.py` & `score_models-0.4.7/score_models/architectures/ncsnpp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/base.py` & `score_models-0.4.7/score_models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Callable
+
 import torch
 from torch import Tensor
 from torch.nn import Module
 from torch.func import vjp
 from .utils import DEVICE, DTYPE
 from score_models.sde import VESDE, VPSDE, SDE
 from typing import Union
@@ -10,34 +12,16 @@
 from torch_ema import ExponentialMovingAverage
 from tqdm import tqdm
 import h5py
 import time
 import os, glob, re, json
 import numpy as np
 from datetime import datetime
-from torch.utils.data import DataLoader
-
-
-class Dataset(torch.utils.data.Dataset):
-    def __init__(self, path, key, extension="h5", device=DEVICE):
-        self.device = device
-        self.key = key
-        if extension in ["h5", "hdf5"]:
-            self._data = h5py.File(self.filepath, "r")
-            self.data = lambda index: self._data[self.key][index]
-            self.size = self._data[self.key].shape[0]
-        elif extension == "npy":
-            self.data = np.load(path)
-            self.size = self.data.shape[0]
+from torch.utils.data import DataLoader, Dataset
 
-    def __len__(self):
-        return self.size
-
-    def __getitem__(self, index):
-        return torch.tensor(self.data[[index]], dtype=DTYPE).to(self.device)
 
 # TODO support data parallel
 class ScoreModelBase(Module, ABC):
     def __init__(self, model: Union[str, Module]=None, sde:SDE=None, checkpoints_directory=None, device=DEVICE, **hyperparameters):
         super().__init__()
         if model is None and checkpoints_directory is None:
             raise ValueError("Must provide one of 'model'i or 'checkpoints_directory'")
@@ -50,18 +34,28 @@
             if "sigma_min" in hyperparameters.keys():
                 hyperparameters["sde"] = "vesde"
             elif "beta_min" in hyperparameters.keys():
                 hyperparameters["sde"] = "vpsde"
             else:
                 raise KeyError("SDE parameters are missing, please specify `sigma_min` and `sigma_max`"
                                "or `beta_min` and `beta_max`. Alternatively, you may provide your own SDE")
+            if "T" not in hyperparameters.keys():
+                hyperparameters["T"] = 1.
             if hyperparameters["sde"].lower() == "vesde":
-                sde = VESDE(sigma_min=hyperparameters["sigma_min"], sigma_max=hyperparameters["sigma_max"])
+                sde = VESDE(sigma_min=hyperparameters["sigma_min"], sigma_max=hyperparameters["sigma_max"], T=hyperparameters["T"])
             elif hyperparameters["sde"].lower() == "vpsde":
-                sde = VPSDE(beta_min=hyperparameters["beta_min"], beta_max=hyperparameters["beta_max"])
+                if "epsilon" not in hyperparameters.keys():
+                    hyperparameters["epsilon"] = 1e-5
+                sde = VPSDE(
+                        beta_min=hyperparameters["beta_min"], 
+                        beta_max=hyperparameters["beta_max"], 
+                        T=hyperparameters["T"],
+                        epsilon=hyperparameters["epsilon"]
+                        )
+        self.hyperparameters = hyperparameters
         self.checkpoints_directory = checkpoints_directory
         self.model = model
         self.model.to(device)
         self.sde = sde
         self.device = device
 
     def forward(self, t, x) -> Tensor:
@@ -154,46 +148,58 @@
                   }
         wrapped_ll = lambda x: self.log_likelihood(x, **kwargs)
         ll, vjp_func = vjp(wrapped_ll, x)
         score = vjp_func(torch.ones_like(ll))
         if return_ll:
             return score, ll
         return score
-        
-
     
     @torch.no_grad()
-    def sample(self, n, shape, steps):
+    def sample(
+            self, 
+            n, 
+            shape, 
+            steps, 
+            likelihood_score_fn:Callable=None,
+            guidance_factor=1.
+            ):
         """
         n: Number of samples to draw
         shape: Shape of the tensor to sample, except batch dimension.
         steps: Number of Euler-Maruyam steps to perform
+        likelihood_score_fn: Add an additional drift to the sampling for posterior sampling. Must have the signature f(t, x)
+        guidance_factor: Multiplicative factor for the likelihood drift
         """
+        if likelihood_score_fn is None:
+            likelihood_score_fn = lambda t, x: 0.
         # A simple Euler-Maruyama integration of the model SDE
         x = self.sde.prior(shape).sample([n]).to(self.device)
-        dt = -1.0 / steps
-        t = torch.ones(n).to(self.device)
+        dt = -self.sde.T / steps
+        t = torch.ones(n).to(self.device) * self.sde.T
         for _ in tqdm(range(steps)):
+            g = self.sde.diffusion(t, x)
+            f = self.sde.drift(t, x) - g**2 * (self.score(t, x) + guidance_factor * likelihood_score_fn(t, x))
+            dw = torch.randn_like(x) * (-dt)**(1/2)
+            x_mean = x + f * dt
+            x = x_mean + g * dw 
             t += dt
-            drift = self.sde.drift(t, x)
-            diffusion = self.sde.diffusion(t, x)
-            score = self.score(t, x)
-            drift = drift - diffusion**2 * score
-            z = torch.randn_like(x)
-            x_mean = x + drift * dt
-            x = x_mean + diffusion * (-dt)**(1/2) * z
         return x_mean
 
+    def loss_fn(self, x, *args, **kwargs):
+        B, *D = x.shape
+        broadcast = [B, *[1] * len(D)]
+        z = torch.randn_like(x)
+        t = torch.rand(B).to(self.device) * (self.sde.T - self.sde.epsilon) + self.sde.epsilon
+        mean, sigma = self.sde.marginal_prob(t=t, x=x)
+        sigma_ = sigma.view(*broadcast)
+        return torch.sum((z + sigma_ * self.score(t=t, x=mean + sigma_ * z)) ** 2) / B
     
     def fit(
         self,
-        dataset=None,
-        dataset_path=None,
-        dataset_extension="h5",
-        dataset_key=None,
+        dataset: Dataset,
         preprocessing_fn=None,
         epochs=100,
         learning_rate=1e-4,
         ema_decay=0.9999,
         batch_size=1,
         shuffle=False,
         patience=float('inf'),
@@ -203,18 +209,18 @@
         warmup=0,
         clip=0.,
         checkpoints_directory=None,
         model_checkpoint=None,
         checkpoints=10,
         models_to_keep=2,
         seed=None,
-        model_id=None,
         logname=None,
+        logdir=None,
         n_iterations_in_epoch=None,
-        logname_prefixe="score_model",
+        logname_prefix="score_model",
         verbose=0
     ):
         """
         Train the model on the provided dataset.
 
         Parameters:
             dataset (torch.utils.data.Dataset): The training dataset.
@@ -234,25 +240,23 @@
             warmup (int, optional): The number of warmup iterations for learning rate. Default is 0.
             clip (float, optional): The gradient clipping value. Default is 0.
             model_checkpoint (float, optional): If checkpoints_directory is provided, this can be used to restart training from checkpoint.
             checkpoints_directory (str, optional): The directory to save model checkpoints. Default is None.
             checkpoints (int, optional): The interval for saving model checkpoints. Default is 10 epochs.
             models_to_keep (int, optional): The number of best models to keep. Default is 3.
             seed (int, optional): The random seed for numpy and torch. Default is None.
-            model_id (str, optional): The ID for the model. Default is None.
             logname (str, optional): The logname for saving checkpoints. Default is None.
-            logname_prefixe (str, optional): The prefix for the logname. Default is "score_model".
+            logdir (str, optional): The path to the directory in which to create the new checkpoint_directory with logname.
+            logname_prefix (str, optional): The prefix for the logname. Default is "score_model".
 
         Returns:
             list: List of loss values during training.
         """
-        optimizer = torch.optim.Adam(self.parameters(), lr=learning_rate)
-        ema = ExponentialMovingAverage(self.parameters(), decay=ema_decay)
-        if dataset is None:
-            dataset = Dataset(dataset_path, dataset_key, dataset_extension, device=self.device)
+        optimizer = torch.optim.Adam(self.model.parameters(), lr=learning_rate)
+        ema = ExponentialMovingAverage(self.model.parameters(), decay=ema_decay)
         dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, drop_last=False)
         if n_iterations_in_epoch is None:
             n_iterations_in_epoch = len(dataloader)
         if checkpoints_directory is None:
             checkpoints_directory = self.checkpoints_directory
         
         if preprocessing_fn is not None:
@@ -266,28 +270,29 @@
             hyperparameters["sde"] = "vpsde"
             hyperparameters["beta_min"] = self.sde.beta_min
             hyperparameters["beta_max"] = self.sde.beta_max
         elif isinstance(self.sde, VESDE):
             hyperparameters["sde"] = "vesde"
             hyperparameters["sigma_min"] = self.sde.sigma_min
             hyperparameters["sigma_max"] = self.sde.sigma_max
+        hyperparameters["epsilon"] = self.sde.epsilon
+        hyperparameters["T"] = self.sde.T
 
        # ==== Take care of where to write checkpoints and stuff =================================================================
-        if model_id is not None:
-            logname = model_id
-        elif logname is not None:
-            logname = logname
-        else:
-            logname = logname_prefixe + "_" + datetime.now().strftime("%y%m%d%H%M%S")
+        if checkpoints_directory is not None:
+            if os.path.isdir(checkpoints_directory):
+                logname = os.path.split(checkpoints_directory)[-1]
+        elif logname is None:
+            logname = logname_prefix + "_" + datetime.now().strftime("%y%m%d%H%M%S")
 
         save_checkpoint = False
-        if checkpoints_directory is not None:
+        if checkpoints_directory is not None or logdir is not None:
             save_checkpoint = True
-            if not os.path.isdir(checkpoints_directory):
-                os.mkdir(checkpoints_directory)
+            if checkpoints_directory is None: # the way to create a new directory is using logdir
+                checkpoints_directory = os.path.join(logdir, logname)
                 with open(os.path.join(checkpoints_directory, "script_params.json"), "w") as f:
                     json.dump(
                         {
                             "dataset_path": dataset_path,
                             "dataset_extension": dataset_extension,
                             "dataset_key": dataset_extension,
                             "preprocessing": preprocessing_name,
@@ -302,57 +307,48 @@
                             "epsilon": epsilon,
                             "warmup": warmup,
                             "clip": clip,
                             "checkpoint_directory": checkpoints_directory,
                             "checkpoints": checkpoints,
                             "models_to_keep": models_to_keep,
                             "seed": seed,
-                            "model_id": model_id,
                             "logname": logname,
-                            "logname_prefixe": logname_prefixe,
+                            "logname_prefix": logname_prefix,
                         },
                         f,
                         indent=4
                     )
                 with open(os.path.join(checkpoints_directory, "model_hparams.json"), "w") as f:
                     json.dump(hyperparameters, f, indent=4)
 
             # ======= Load model if model_id is provided ===============================================================
             paths = glob.glob(os.path.join(checkpoints_directory, "checkpoint*.pt"))
             opt_paths = glob.glob(os.path.join(checkpoints_directory, "optimizer*.pt"))
             checkpoint_indices = [int(re.findall('[0-9]+', os.path.split(path)[-1])[-1]) for path in paths]
             scores = [float(re.findall('([0-9]{1}.[0-9]+e[+-][0-9]{2})', os.path.split(path)[-1])[-1]) for path in paths]
-            if model_id is not None and checkpoint_indices:
+            if checkpoint_indices:
                 if model_checkpoint is not None:
                     checkpoint_path = paths[checkpoint_indices.index(model_checkpoint)]
                     self.model.load_state_dict(torch.load(checkpoint_path, map_location=self.model.device))
                     optimizer.load_state_dict(torch.load(opt_paths[checkpoints == model_checkpoint], map_location=self.device))
-                    print(f"Loaded checkpoint {model_checkpoint} of {model_id}")
+                    print(f"Loaded checkpoint {model_checkpoint} of {logname}")
                     latest_checkpoint = model_checkpoint
                 else:
                     max_checkpoint_index = np.argmax(checkpoint_indices)
                     checkpoint_path = paths[max_checkpoint_index]
+                    opt_path = opt_paths[max_checkpoint_index]
                     self.model.load_state_dict(torch.load(checkpoint_path, map_location=self.device))
-                    optimizer.load_state_dict(torch.load(checkpoint_path, map_location=self.device))
-                    print(f"Loaded checkpoint {checkpoint_indices[max_checkpoint_index]} of {model_id}")
+                    optimizer.load_state_dict(torch.load(opt_path, map_location=self.device))
+                    print(f"Loaded checkpoint {checkpoint_indices[max_checkpoint_index]} of {logname}")
                     latest_checkpoint = checkpoint_indices[max_checkpoint_index]
-            else:
                 latest_checkpoint = 0
 
         if seed is not None:
             torch.manual_seed(seed)
 
-        def loss_fn(x):
-            B, *D = x.shape
-            broadcast = [B, *[1] * len(D)]
-            z = torch.randn_like(x)
-            t = torch.rand(B).to(self.device) * (1. - epsilon) + epsilon
-            mean, sigma = self.sde.marginal_prob(t=t, x=x)
-            sigma_ = sigma.view(*broadcast)
-            return torch.sum((z + sigma_ * self(t=t, x=mean + sigma_ * z)) ** 2) / B
 
         best_loss = float('inf')
         losses = []
         step = 0
         global_start = time.time()
         estimated_time_for_epoch = 0
         out_of_time = False
@@ -364,31 +360,30 @@
             time_per_step_epoch_mean = 0
             cost = 0
             data_iter = iter(dataloader)
             for _ in range(n_iterations_in_epoch):
                 start = time.time()
                 try:
                     x = next(data_iter)
+                    x, *args = next(data_iter)
                 except StopIteration:
                     data_iter = iter(dataloader)
-                    x = next(data_iter)
-                if isinstance(x, tuple) or isinstance(x, list): # wrapper for tensor dataset
-                    x = x[0]
+                    x, *args = next(data_iter)
                 if preprocessing_fn is not None:
                     x = preprocessing_fn(x)
                 optimizer.zero_grad()
-                loss = loss_fn(x)
+                loss = self.loss_fn(x, *args)
                 loss.backward()
 
                 if step < warmup:
                     for g in optimizer.param_groups:
                         g['lr'] = learning_rate * np.minimum(step / warmup, 1.0)
 
                 if clip > 0:
-                    torch.nn.utils.clip_grad_norm_(self.parameters(), max_norm=clip)
+                    torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=clip)
 
                 optimizer.step()
                 ema.update()
 
                 _time = time.time() - start
                 time_per_step_epoch_mean += _time
                 cost += float(loss)
@@ -419,15 +414,15 @@
 
             if save_checkpoint:
                 if (epoch + 1) % checkpoints == 0 or patience == 0 or epoch == epochs - 1 or out_of_time:
                     latest_checkpoint += 1
                     with open(os.path.join(checkpoints_directory, "score_sheet.txt"), mode="a") as f:
                         f.write(f"{latest_checkpoint} {cost}\n")
                     with ema.average_parameters():
-                        torch.save(self.state_dict(), os.path.join(checkpoints_directory, f"checkpoint_{cost:.4e}_{latest_checkpoint:03d}.pt"))
+                        torch.save(self.model.state_dict(), os.path.join(checkpoints_directory, f"checkpoint_{cost:.4e}_{latest_checkpoint:03d}.pt"))
                     torch.save(optimizer.state_dict(), os.path.join(checkpoints_directory, f"optimizer_{cost:.4e}_{latest_checkpoint:03d}.pt"))
                     paths = glob.glob(os.path.join(checkpoints_directory, "*.pt"))
                     checkpoint_indices = [int(re.findall('[0-9]+', os.path.split(path)[-1])[-1]) for path in paths]
                     scores = [float(re.findall('([0-9]{1}.[0-9]+e[+-][0-9]{2})', os.path.split(path)[-1])[-1]) for path in paths]
                     if len(checkpoint_indices) > 2*models_to_keep: # has to be twice since we also save optimizer states
                         index_to_delete = np.argmin(checkpoint_indices)
                         os.remove(os.path.join(checkpoints_directory, f"checkpoint_{scores[index_to_delete]:.4e}_{checkpoint_indices[index_to_delete]:03d}.pt"))
```

### Comparing `score_models-0.4.6/score_models/definitions.py` & `score_models-0.4.7/score_models/definitions.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/__init__.py` & `score_models-0.4.7/score_models/layers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from .conv_layers import conv3x3, conv1x1
 from .resnet_block_biggan import ResnetBlockBigGANpp
 from .spectral_normalization import SpectralNorm
 from .ddpm_resnet_block import DDPMResnetBlock
 from .ncsn_resnet_block import NCSNResidualBlock
 from .attention_block import SelfAttentionBlock, ScaledAttentionLayer
 from .projection_embedding import GaussianFourierProjection
-from .conv2dsame import Conv2dSame, ConvTranspose2dSame
-from .conv1dsame import Conv1dSame, ConvTranspose1dSame
+from .conv1dsame import Conv1dSame, ConvTransposed1dSame
+from .conv2dsame import Conv2dSame, ConvTransposed2dSame
 from .conv3dsame import Conv3dSame, ConvTransposed3dSame
 from .combine import Combine
 from .upsample import UpsampleLayer
 from .downsample import DownsampleLayer
```

### Comparing `score_models-0.4.6/score_models/layers/attention_block.py` & `score_models-0.4.7/score_models/layers/attention_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/combine.py` & `score_models-0.4.7/score_models/layers/combine.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/conditional_batchnorm2d.py` & `score_models-0.4.7/score_models/layers/conditional_batchnorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/conditional_instancenorm2d.py` & `score_models-0.4.7/score_models/layers/conditional_instancenorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/conditional_instancenorm2d_plus.py` & `score_models-0.4.7/score_models/layers/conditional_instancenorm2d_plus.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/conv1dsame.py` & `score_models-0.4.7/score_models/layers/conv1dsame.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             groups: int = 1,
             bias: bool = True,
             padding_mode: str = 'zeros',
             spectral_norm: bool = False,
             device=None,
             dtype=None
     ):
-        super(Conv1dSame, self).__init__()
+        super().__init__()
         if spectral_norm:
             sp_norm = SpectralNorm
         else:
             sp_norm = lambda x: x
         self.conv = sp_norm(nn.Conv1d(
             in_channels=in_channels,
             out_channels=out_channels,
@@ -53,15 +53,15 @@
             h_o = h // self.stride
             p0 = ((h_o - 1) * self.stride + 1 + self.dilation * (self.kernel_size -1) - h) // 2
             x = F.pad(x, (p0, p0+1))
         x = self.conv(x)
         return x
 
 
-class ConvTranspose1dSame(nn.Module):
+class ConvTransposed1dSame(nn.Module):
     def __init__(
             self,
             in_channels: int,
             out_channels: int,
             kernel_size: int,
             stride: int = 1,
             padding: Union[str, int] = 0,
@@ -69,33 +69,33 @@
             groups: int = 1,
             bias: bool = True,
             padding_mode: str = 'zeros',
             spectral_norm: bool = False,
             device=None,
             dtype=None
     ):
-        super(ConvTranspose1dSame, self).__init__()
+        super().__init__()
         if spectral_norm:
             sp_norm = SpectralNorm
         else:
             sp_norm = lambda x: x
         self.conv = sp_norm(nn.ConvTranspose1d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
             stride=stride,
             dilation=dilation,
             groups=groups,
             bias=bias,
-            padding=dilation * (kernel_size - 1) // 2,
+            padding=dilation * (kernel_size - 1) // 2 + padding,
             output_padding=stride - 1,
             padding_mode=padding_mode,
             device=device,
             dtype=dtype
         ))
         self.stride = stride
         self.dilation = dilation
         self.kernel_size = kernel_size
 
     def forward(self, x):
         x = self.conv(x)
-        return x
+        return x
```

### Comparing `score_models-0.4.6/score_models/layers/conv2dsame.py` & `score_models-0.4.7/score_models/layers/conv2dsame.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             groups: int = 1,
             bias: bool = True,
             padding_mode: str = 'zeros',
             spectral_norm: bool = False,
             device=None,
             dtype=None
     ):
-        super(Conv2dSame, self).__init__()
+        super().__init__()
         if spectral_norm:
             sp_norm = SpectralNorm
         else:
             sp_norm = lambda x: x
         self.conv = sp_norm(nn.Conv2d(
             in_channels=in_channels,
             out_channels=out_channels,
@@ -54,15 +54,15 @@
             p0 = ((h_o - 1) * self.stride + 1 + self.dilation * (self.kernel_size -1) - h) // 2
             p1 = ((w_o - 1) * self.stride + 1 + self.dilation * (self.kernel_size -1) - w) // 2
             x = F.pad(x, (p0, p0+1, p1, p1+1)) # It might be controversial to do this, but this is how it is done in Tensorflow...
         x = self.conv(x)
         return x
 
 
-class ConvTranspose2dSame(nn.Module):
+class ConvTransposed2dSame(nn.Module):
     def __init__(
             self,
             in_channels: int,
             out_channels: int,
             kernel_size: int,
             stride: int = 1,
             padding: Union[str, int] = 0,
@@ -70,28 +70,28 @@
             groups: int = 1,
             bias: bool = True,
             padding_mode: str = 'zeros',
             spectral_norm: bool = False,
             device=None,
             dtype=None
     ):
-        super(ConvTranspose2dSame, self).__init__()
+        super().__init__()
         if spectral_norm:
             sp_norm = SpectralNorm
         else:
             sp_norm = lambda x: x
         self.conv = sp_norm(nn.ConvTranspose2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
             stride=stride,
             dilation=dilation,
             groups=groups,
             bias=bias,
-            padding=dilation * (kernel_size - 1) // 2,
+            padding=dilation * (kernel_size - 1) // 2 + padding,
             output_padding=stride - 1,
             padding_mode=padding_mode,
             device=device,
             dtype=dtype
         ))
         self.stride = stride
         self.dilation = dilation
```

### Comparing `score_models-0.4.6/score_models/layers/conv3dsame.py` & `score_models-0.4.7/score_models/layers/conv3dsame.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             groups: int = 1,
             bias: bool = True,
             padding_mode: str = 'zeros',
             spectral_norm: bool = False,
             device=None,
             dtype=None
     ):
-        super(Conv3dSame, self).__init__()
+        super().__init__()
         if spectral_norm:
             sp_norm = SpectralNorm
         else:
             sp_norm = lambda x: x
         self.conv = sp_norm(nn.Conv3d(
             in_channels=in_channels,
             out_channels=out_channels,
@@ -49,15 +49,15 @@
     def forward(self, x):
         if self.stride > 1:
             # compute some padding
             b, c, h, w, d = x.shape
             h_o, w_o, d_o = h // self.stride, w // self.stride, d // self.stride
             p0 = ((h_o - 1) * self.stride + 1 + self.dilation * (self.kernel_size - 1) - h) // 2
             p1 = ((w_o - 1) * self.stride + 1 + self.dilation * (self.kernel_size - 1) - w) // 2
-            p2 = ((d_o - 1) * self.stride + 1 + self.dilation * (self.kernel_size - 1) - c) // 2
+            p2 = ((d_o - 1) * self.stride + 1 + self.dilation * (self.kernel_size - 1) - d) // 2
             x = F.pad(x, (p0, p0+1, p1, p1+1, p2, p2+1))
         x = self.conv(x)
         return x
 
 
 class ConvTransposed3dSame(nn.Module):
     def __init__(
@@ -71,25 +71,26 @@
             groups: int = 1,
             bias: bool = True,
             padding_mode: str = 'zeros',
             spectral_norm: bool = False,
             device=None,
             dtype=None
     ):
-        super(ConvTransposed3dSame, self).__init__()
+        super().__init__()
         if spectral_norm:
             sp_norm = SpectralNorm
         else:
             sp_norm = lambda x: x
         self.conv = sp_norm(nn.ConvTranspose3d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
             stride=stride,
-            padding=dilation * (kernel_size - 1) // 2,
+            padding=dilation * (kernel_size - 1) // 2 + padding,
+            output_padding=stride - 1,
             dilation=dilation,
             groups=groups,
             bias=bias,
             padding_mode=padding_mode,
             device=device,
             dtype=dtype
         ))
```

### Comparing `score_models-0.4.6/score_models/layers/conv_layers.py` & `score_models-0.4.7/score_models/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/ddpm_resnet_block.py` & `score_models-0.4.7/score_models/layers/ddpm_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/downsample.py` & `score_models-0.4.7/score_models/layers/downsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/ncsn_resnet_block.py` & `score_models-0.4.7/score_models/layers/ncsn_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/projection_embedding.py` & `score_models-0.4.7/score_models/layers/projection_embedding.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/resnet_block_biggan.py` & `score_models-0.4.7/score_models/layers/resnet_block_biggan.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/spectral_normalization.py` & `score_models-0.4.7/score_models/layers/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/squeeze_and_excitation.py` & `score_models-0.4.7/score_models/layers/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/style_gan_conv.py` & `score_models-0.4.7/score_models/layers/style_gan_conv.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/up_or_downsampling.py` & `score_models-0.4.7/score_models/layers/up_or_downsampling.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/up_or_downsampling1d.py` & `score_models-0.4.7/score_models/layers/up_or_downsampling1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/up_or_downsampling2d.py` & `score_models-0.4.7/score_models/layers/up_or_downsampling2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/up_or_downsampling3d.py` & `score_models-0.4.7/score_models/layers/up_or_downsampling3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/upfirdn1d.py` & `score_models-0.4.7/score_models/layers/upfirdn1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/upfirdn2d.py` & `score_models-0.4.7/score_models/layers/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/upfirdn3d.py` & `score_models-0.4.7/score_models/layers/upfirdn3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/layers/upsample.py` & `score_models-0.4.7/score_models/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models/sde/sde.py` & `score_models-0.4.7/score_models/sde/sde.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 from torch.distributions import Distribution
 from torch import Tensor
 
 class SDE(ABC):
     """
     Abstract class for some SDE info important for the score models
     """
-    def __init__(self):
+    def __init__(self, T=1.0, epsilon=0.):
+        """
+        The time index in the diffusion is defined in the range [epsilon, T]. 
+        """
         super().__init__()
+        self.T = T
+        self.epsilon = epsilon
     
     @abstractmethod
     def sigma(self, t) -> Tensor:
         ...
     
     @abstractmethod
     def prior(self, shape) -> Distribution:
```

### Comparing `score_models-0.4.6/score_models/sde/vesde.py` & `score_models-0.4.7/score_models/sde/vesde.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,32 @@
 
 
 class VESDE(SDE):
     def __init__(
             self,
             sigma_min: float,
             sigma_max: float,
+            T:float=1.0,
+            epsilon:float=0.0
     ):
         """
         Variance Exploding stochastic differential equation 
         
         Args:
             sigma_min (float): The minimum value of the standard deviation of the noise term.
             sigma_max (float): The maximum value of the standard deviation of the noise term.
             T (float, optional): The time horizon for the VESDE. Defaults to 1.0.
             device (str, optional): The device to use for computation. Defaults to DEVICE.
         """
-        super().__init__()
+        super().__init__(T, epsilon)
         self.sigma_min = sigma_min
         self.sigma_max = sigma_max
 
     def sigma(self, t: Tensor) -> Tensor:
-        return self.sigma_min * (self.sigma_max / self.sigma_min) ** t
+        return self.sigma_min * (self.sigma_max / self.sigma_min) ** (t/self.T)
     
     def prior(self, shape, mu=None):
         """
         Technically, VESDE does not change the mean of the 0 temperature distribution, 
         so I give the option to provide for more accuracy. In practice, 
         sigma_max is chosen large enough to make this choice irrelevant
         """
```

### Comparing `score_models-0.4.6/score_models/sde/vpsde.py` & `score_models-0.4.7/score_models/sde/vpsde.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 
 class VPSDE(SDE):
     def __init__(
         self,
         beta_min: float = 0.1,
         beta_max: float = 20,
+        T: float = 1.0,
+        epsilon: float = 1e-5
     ):
-        super().__init__()
+        super().__init__(T, epsilon)
         self.beta_min = beta_min
         self.beta_max = beta_max
     
     def beta(self, t: Tensor):
         return self.beta_min + t * (self.beta_max - self.beta_min)
 
     def sigma(self, t: Tensor) -> Tensor:
```

### Comparing `score_models-0.4.6/score_models/sliced_score_matching.py` & `score_models-0.4.7/score_models/sliced_score_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,7 +54,8 @@
     vectors = torch.randn_like(samples)
     if noise_type == 'rademacher':
         vectors = vectors.sign()
     score, vjp_func = vjp(model, samples)
     trace_estimate = (vectors * vjp_func(vectors)[0]).flatten(1).sum(dim=1)
     loss = (0.5 * torch.sum(score.flatten(1)**2, dim=1) + trace_estimate).mean()
     return loss
+
```

### Comparing `score_models-0.4.6/score_models/utils.py` & `score_models-0.4.7/score_models/utils.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/score_models.egg-info/PKG-INFO` & `score_models-0.4.7/score_models.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,160 +1,159 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: score-models
-Version: 0.4.6
+Version: 0.4.7
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
-License: UNKNOWN
-Description: =========================
-        Score Models for Pytorch
-        =========================
-        
-        .. image:: https://badge.fury.io/py/score_models.svg
-           :target: https://badge.fury.io/py/score_models
-        .. image:: https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg
-           :target: https://codecov.io/gh/AlexandreAdam/torch_score_models
-        
-        A storage for score-based models. The `ScoreModel` interface gives access to the following utilities:
-        
-        - Simple initialization of MLP, NCSN++ and DDPM neural network architectures
-        - A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
-        - A sampling method based on an Euler-Maruyama discretization of an SDE.
-        - A simple interface to train an energy model using DSM
-        
-        This repository is mainly intended for personal use.
-        You might also want to refer to the original implementation at `https://github.com/yang-song/score_sde <https://github.com/yang-song/score_sde>`_.
-        
-        Installation
-        ------------
-        
-        To install the package, you can use pip:
-        
-        .. code-block:: bash
-        
-           pip install torch-score-models
-        
-        Usage
-        -----
-        
-        ScoreModel
-        ~~~~~~~~~~
-        
-        The `ScoreModel` class is the main interface for training and using score models, defined as
-        
-        .. math::
-        
-           \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
-        
-        where :math:`\sigma(t)` is the standard deviation of the perturbation kernel :math:`p_t(\mathbf{x} \mid \mathbf{x}_0)`
-        of an SDE.
-        
-        The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
-        
-        .. code-block:: python
-        
-           from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
-        
-           # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
-           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
-           model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
-           # ... or the VPSDE
-           model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
-        
-           # NN Architectures support a Unet with 1D convolutions for time series input data
-           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
-           # ... or 3D convolutions for videos/voxels
-           net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
-           # You can also use a simpler MLP architecture
-           net = MLP(dimensions=dim, layers=4, units=100)
-           # ... or Jonathan Ho's DDPM architecture
-           net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
-        
-           # Train the model
-           model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
-        
-           # Generate samples from the trained model
-           samples = model.sample(size=[batch_size, *dimensions], N=1000)
-        
-           # Compute the score for a given input
-           score = model.score(t, x)
-        
-           # Initialize the score model and its neural network from a path to a checkpoint directory
-           score = ScoreModel(checkpoint_directory)
-        
-        EnergyModel
-        ~~~~~~~~~~~
-        
-        The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the
-        automatic differentiation of an energy model
-        
-        .. math::
-        
-           E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^2
-        
-        This is to say that the score is defined as
-        
-        .. math::
-        
-           \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
-        
-        **Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
-        neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network
-        architecture to be a function :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}` instead of :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}^d`. An `output_activation` like `relu`
-        can also be specified to make the energy positive or bounded from below.
-        
-        Training Parameters
-        ~~~~~~~~~~~~~~~~~~~
-        
-        When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
-        
-        - `dataset`: The training dataset (`torch.utils.data.Dataset`).
-        - `epochs`: The number of training epochs.
-        - `learning_rate`: The learning rate for the ADAM optimizer.
-        - `batch_size`: The batch size for training.
-        - `checkpoints_directory`: The directory to save model checkpoints (default: None).
-        - `seed`: The random seed for numpy and torch.
-        
-        Refer to the method's docstring or the class definition for more details on available parameters.
-        
-        Citations
-        ---------
-        
-        If you use this package in your research, please consider citing the following papers:
-        
-        .. code-block:: bibtex
-        
-           @inproceedings{NEURIPS2020_4c5bcfec,
-               author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
-               booktitle   = {Advances in Neural Information Processing Systems},
-               editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
-               pages       = {6840--6851},
-               publisher   = {Curran Associates, Inc.},
-               title       = {Denoising Diffusion Probabilistic Models},
-               url         = {https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf},
-               volume      = {33},
-               year        = {2020}
-           }
-        
-           @inproceedings{song2021scorebased,
-             title={Score-Based Generative Modeling through Stochastic Differential Equations},
-             author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
-             booktitle={International Conference on Learning Representations},
-             year={2021},
-             url={https://openreview.net/forum?id=PxTIG12RRHS}
-           }
-        
-        License
-        -------
-        
-        This package is licensed under the MIT License.
-        
-        You can save the above content in an `.rst` file, such as `README.rst`, and include it in your project's root directory.
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
+License-File: LICENSE.txt
+
+=========================
+Score Models for Pytorch
+=========================
+
+.. image:: https://badge.fury.io/py/score_models.svg
+   :target: https://badge.fury.io/py/score_models
+.. image:: https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg
+   :target: https://codecov.io/gh/AlexandreAdam/torch_score_models
+
+A storage for score-based models. The `ScoreModel` interface gives access to the following utilities:
+
+- Simple initialization of MLP, NCSN++ and DDPM neural network architectures
+- A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
+- A sampling method based on an Euler-Maruyama discretization of an SDE.
+- A simple interface to train an energy model using DSM
+
+This repository is mainly intended for personal use.
+You might also want to refer to the original implementation at `https://github.com/yang-song/score_sde <https://github.com/yang-song/score_sde>`_.
+
+Installation
+------------
+
+To install the package, you can use pip:
+
+.. code-block:: bash
+
+   pip install torch-score-models
+
+Usage
+-----
+
+ScoreModel
+~~~~~~~~~~
+
+The `ScoreModel` class is the main interface for training and using score models, defined as
+
+.. math::
+
+   \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
+
+where :math:`\sigma(t)` is the standard deviation of the perturbation kernel :math:`p_t(\mathbf{x} \mid \mathbf{x}_0)`
+of an SDE.
+
+The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
+
+.. code-block:: python
+
+   from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
+
+   # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
+   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
+   model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
+   # ... or the VPSDE
+   model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
+
+   # NN Architectures support a Unet with 1D convolutions for time series input data
+   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
+   # ... or 3D convolutions for videos/voxels
+   net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
+   # You can also use a simpler MLP architecture
+   net = MLP(dimensions=dim, layers=4, units=100)
+   # ... or Jonathan Ho's DDPM architecture
+   net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
+
+   # Train the model
+   model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
+
+   # Generate samples from the trained model
+   samples = model.sample(size=[batch_size, *dimensions], N=1000)
+
+   # Compute the score for a given input
+   score = model.score(t, x)
+
+   # Initialize the score model and its neural network from a path to a checkpoint directory
+   score = ScoreModel(checkpoint_directory)
+
+EnergyModel
+~~~~~~~~~~~
+
+The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the
+automatic differentiation of an energy model
+
+.. math::
+
+   E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^2
+
+This is to say that the score is defined as
+
+.. math::
+
+   \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
+
+**Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
+neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network
+architecture to be a function :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}` instead of :math:`f_\theta: \mathbb{R}^d \to \mathbb{R}^d`. An `output_activation` like `relu`
+can also be specified to make the energy positive or bounded from below.
+
+Training Parameters
+~~~~~~~~~~~~~~~~~~~
+
+When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
+
+- `dataset`: The training dataset (`torch.utils.data.Dataset`).
+- `epochs`: The number of training epochs.
+- `learning_rate`: The learning rate for the ADAM optimizer.
+- `batch_size`: The batch size for training.
+- `checkpoints_directory`: The directory to save model checkpoints (default: None).
+- `seed`: The random seed for numpy and torch.
+
+Refer to the method's docstring or the class definition for more details on available parameters.
+
+Citations
+---------
+
+If you use this package in your research, please consider citing the following papers:
+
+.. code-block:: bibtex
+
+   @inproceedings{NEURIPS2020_4c5bcfec,
+       author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
+       booktitle   = {Advances in Neural Information Processing Systems},
+       editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
+       pages       = {6840--6851},
+       publisher   = {Curran Associates, Inc.},
+       title       = {Denoising Diffusion Probabilistic Models},
+       url         = {https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf},
+       volume      = {33},
+       year        = {2020}
+   }
+
+   @inproceedings{song2021scorebased,
+     title={Score-Based Generative Modeling through Stochastic Differential Equations},
+     author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
+     booktitle={International Conference on Learning Representations},
+     year={2021},
+     url={https://openreview.net/forum?id=PxTIG12RRHS}
+   }
+
+License
+-------
+
+This package is licensed under the MIT License.
+
+You can save the above content in an `.rst` file, such as `README.rst`, and include it in your project's root directory.
+
```

### Comparing `score_models-0.4.6/score_models.egg-info/SOURCES.txt` & `score_models-0.4.7/score_models.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 score_models/__init__.py
 score_models/base.py
 score_models/definitions.py
+score_models/dsm.py
 score_models/score_model.py
 score_models/sliced_score_matching.py
 score_models/utils.py
 score_models.egg-info/PKG-INFO
 score_models.egg-info/SOURCES.txt
 score_models.egg-info/dependency_links.txt
 score_models.egg-info/requires.txt
```

### Comparing `score_models-0.4.6/setup.py` & `score_models-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name="score_models",
-	version="0.4.6",
+	version="0.4.7",
     description="A simple pytorch interface for score model and basic diffusion.",
     long_description=long_description,
     author="Alexandre Adam",
     author_email="alexandre.adam@umontreal.ca",
     url="https://github.com/AlexandreAdam/torch_score_models",
     packages=find_packages(),
     install_requires=[
```

### Comparing `score_models-0.4.6/tests/test_architectures.py` & `score_models-0.4.7/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/tests/test_layers.py` & `score_models-0.4.7/tests/test_layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -171,7 +171,30 @@
     assert np.all(out.detach().numpy()[..., 2:-2, 2:-2] == 9.)
 
     conv = StyleGANConv(in_ch=1, out_ch=3, kernel=3, up=False, down=True, use_bias=True, kernel_init=init_test_fn, dimensions=2)
     out = conv(x)
     print(out)
     assert np.all(out.detach().numpy()[..., 1:-1, 1:-1] == 9.)
 
+def test_transposed_conv():
+    # Test that we can downsample and upsample odd numbered images with correct padding
+    from score_models.layers import ConvTransposed1dSame, ConvTransposed2dSame, ConvTransposed3dSame
+    from score_models.layers import Conv1dSame, Conv2dSame, Conv3dSame
+    
+    B = 10
+    D = 15
+    C = 16
+    K = 3
+    for dim in [1, 2, 3]:
+        x = torch.randn(B, C, *[D]*dim)
+        layer_ = [Conv1dSame, Conv2dSame, Conv3dSame][dim-1]
+        layer = layer_(C, C, K, stride=2)
+        x_down= layer(x)
+        print("Down", x_down.shape)
+        assert x_down.shape == torch.Size([B, C, *[D//2]*dim])
+        
+        layer_ = [ConvTransposed1dSame, ConvTransposed2dSame, ConvTransposed3dSame][dim-1]
+        layer = layer_(C, C, K, stride=2)
+        y = layer(x_down)
+        print("Up", x.shape)
+        assert x.shape == torch.Size([B, C, *[D]*dim])
+
```

### Comparing `score_models-0.4.6/tests/test_score_models.py` & `score_models-0.4.7/tests/test_score_models.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.6/tests/test_training.py` & `score_models-0.4.7/tests/test_training.py`

 * *Files identical despite different names*

