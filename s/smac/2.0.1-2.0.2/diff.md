# Comparing `tmp/smac-2.0.1.tar.gz` & `tmp/smac-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smac-2.0.1.tar", last modified: Tue May 23 12:28:37 2023, max compression
+gzip compressed data, was "smac-2.0.2.tar", last modified: Tue Aug  1 13:20:09 2023, max compression
```

## Comparing `smac-2.0.1.tar` & `smac-2.0.2.tar`

### file list

```diff
@@ -1,148 +1,147 @@
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3377 2023-03-03 09:52:31.000000 smac-2.0.1/LICENSE.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      127 2023-03-03 09:52:31.000000 smac-2.0.1/MANIFEST.in
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7272 2023-05-23 12:28:37.844321 smac-2.0.1/PKG-INFO
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6116 2023-05-22 12:55:22.000000 smac-2.0.1/README.md
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2887 2023-03-03 09:52:31.000000 smac-2.0.1/pyproject.toml
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       38 2023-05-23 12:28:37.844321 smac-2.0.1/setup.cfg
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2303 2023-05-22 12:55:22.000000 smac-2.0.1/setup.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1555 2023-05-22 12:55:22.000000 smac-2.0.1/smac/__init__.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/acquisition/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/__init__.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/acquisition/function/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      717 2023-05-16 11:11:34.000000 smac-2.0.1/smac/acquisition/function/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3552 2023-05-16 11:11:34.000000 smac-2.0.1/smac/acquisition/function/abstract_acquisition_function.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3086 2023-05-16 11:11:34.000000 smac-2.0.1/smac/acquisition/function/confidence_bound.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9061 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/expected_improvement.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4002 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/integrated_acquisition_function.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9380 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/prior_acqusition_function.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2692 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/probability_improvement.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1930 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/function/thompson.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/acquisition/maximizer/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      649 2023-03-03 09:52:31.000000 smac-2.0.1/smac/acquisition/maximizer/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6213 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/abstract_acqusition_maximizer.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2344 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/differential_evolution.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4165 2023-05-22 12:55:22.000000 smac-2.0.1/smac/acquisition/maximizer/helpers.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10116 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/local_and_random_search.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    19915 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/local_search.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1828 2023-03-03 10:08:13.000000 smac-2.0.1/smac/acquisition/maximizer/random_search.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/callback/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      160 2023-05-22 12:55:22.000000 smac-2.0.1/smac/callback/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2519 2023-05-22 12:55:22.000000 smac-2.0.1/smac/callback/callback.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1013 2023-05-22 12:55:22.000000 smac-2.0.1/smac/callback/metadata_callback.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      270 2023-03-03 09:52:31.000000 smac-2.0.1/smac/constants.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/facade/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      674 2023-03-03 09:52:31.000000 smac-2.0.1/smac/facade/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    20537 2023-05-22 12:55:22.000000 smac-2.0.1/smac/facade/abstract_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6199 2023-03-03 09:52:31.000000 smac-2.0.1/smac/facade/algorithm_configuration_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11605 2023-04-11 12:42:46.000000 smac-2.0.1/smac/facade/blackbox_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2394 2023-05-16 11:11:34.000000 smac-2.0.1/smac/facade/hyperband_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7578 2023-05-16 11:11:34.000000 smac-2.0.1/smac/facade/hyperparameter_optimization_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4387 2023-05-16 11:11:34.000000 smac-2.0.1/smac/facade/multi_fidelity_facade.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5976 2023-03-03 09:52:31.000000 smac-2.0.1/smac/facade/random_facade.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/initial_design/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      621 2023-03-03 09:52:31.000000 smac-2.0.1/smac/initial_design/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8211 2023-05-22 12:55:22.000000 smac-2.0.1/smac/initial_design/abstract_initial_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      552 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/default_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2202 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/factorial_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1084 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/latin_hypercube_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      656 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/random_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1671 2023-03-03 10:08:13.000000 smac-2.0.1/smac/initial_design/sobol_design.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/intensifier/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      341 2023-03-03 09:52:31.000000 smac-2.0.1/smac/intensifier/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    33241 2023-05-22 12:55:22.000000 smac-2.0.1/smac/intensifier/abstract_intensifier.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2159 2023-05-22 12:55:22.000000 smac-2.0.1/smac/intensifier/hyperband.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17357 2023-05-22 12:55:22.000000 smac-2.0.1/smac/intensifier/intensifier.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    24457 2023-05-22 12:55:22.000000 smac-2.0.1/smac/intensifier/successive_halving.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      553 2023-03-03 09:52:31.000000 smac-2.0.1/smac/logging.yml
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/main/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-05-05 11:32:22.000000 smac-2.0.1/smac/main/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14833 2023-05-22 12:55:22.000000 smac-2.0.1/smac/main/config_selector.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    24432 2023-05-22 12:55:22.000000 smac-2.0.1/smac/main/smbo.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/model/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      247 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11457 2023-05-16 11:11:34.000000 smac-2.0.1/smac/model/abstract_model.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac/model/gaussian_process/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      350 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6523 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/abstract_gaussian_process.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10482 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/gaussian_process.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    35950 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/gpytorch_gaussian_process.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/model/gaussian_process/kernels/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      607 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    23169 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/_boing.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17034 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/base_kernels.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3648 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/hamming_kernel.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4121 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/matern_kernel.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2738 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/rbf_kernel.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1881 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/kernels/white_kernel.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    16808 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/mcmc_gaussian_process.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/model/gaussian_process/priors/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      435 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4306 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/abstract_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2013 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/gamma_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2402 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/horseshoe_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1900 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/log_normal_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5338 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/gaussian_process/priors/tophat_prior.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3002 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/multi_objective_model.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/model/random_forest/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      208 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/random_forest/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1741 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/random_forest/abstract_random_forest.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10805 2023-03-03 10:08:13.000000 smac-2.0.1/smac/model/random_forest/random_forest.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1206 2023-03-03 09:52:31.000000 smac-2.0.1/smac/model/random_model.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/multi_objective/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      333 2023-03-03 09:52:31.000000 smac-2.0.1/smac/multi_objective/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1038 2023-03-03 09:52:31.000000 smac-2.0.1/smac/multi_objective/abstract_multi_objective_algorithm.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1399 2023-03-03 09:52:31.000000 smac-2.0.1/smac/multi_objective/aggregation_strategy.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1902 2023-03-03 09:52:31.000000 smac-2.0.1/smac/multi_objective/parego.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.1/smac/py.typed
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/random_design/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      585 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1362 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/abstract_random_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2691 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/annealing_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3489 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/modulus_design.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2439 2023-03-03 09:52:31.000000 smac-2.0.1/smac/random_design/probability_design.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/runhistory/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      393 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4337 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/dataclasses.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/runhistory/encoder/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1076 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/encoder/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10551 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/abstract_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2443 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/encoder/boing_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2878 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/eips_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2540 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1372 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/encoder/inverse_scaled_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      867 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/log_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1180 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/log_scaled_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      978 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/scaled_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1354 2023-05-16 11:11:34.000000 smac-2.0.1/smac/runhistory/encoder/sqrt_scaled_encoder.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      356 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/enumerations.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       48 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runhistory/errors.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    41541 2023-05-22 12:55:22.000000 smac-2.0.1/smac/runhistory/runhistory.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/runner/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      472 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runner/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9402 2023-05-22 12:55:22.000000 smac-2.0.1/smac/runner/abstract_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1787 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runner/abstract_serial_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9153 2023-05-22 12:55:22.000000 smac-2.0.1/smac/runner/dask_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      419 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runner/exceptions.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8927 2023-05-22 12:55:22.000000 smac-2.0.1/smac/runner/target_function_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7486 2023-03-03 09:52:31.000000 smac-2.0.1/smac/runner/target_function_script_runner.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10868 2023-05-22 12:55:22.000000 smac-2.0.1/smac/scenario.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/utils/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9225 2023-05-16 11:11:34.000000 smac-2.0.1/smac/utils/configspace.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2276 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/data_structures.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1252 2023-05-22 12:55:22.000000 smac-2.0.1/smac/utils/logging.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1159 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/multi_objective.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6018 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/pareto_front.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.844321 smac-2.0.1/smac/utils/subspaces/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    29592 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/subspaces/__init__.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8717 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/subspaces/boing_subspace.py
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    13823 2023-03-03 09:52:31.000000 smac-2.0.1/smac/utils/subspaces/turbo_subspace.py
-drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-05-23 12:28:37.840321 smac-2.0.1/smac.egg-info/
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7272 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/PKG-INFO
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4544 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/SOURCES.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        1 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/dependency_links.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       53 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/entry_points.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      456 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/requires.txt
--rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       11 2023-05-23 12:28:37.000000 smac-2.0.1/smac.egg-info/top_level.txt
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3377 2023-03-03 09:52:31.000000 smac-2.0.2/LICENSE.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      127 2023-07-31 15:47:05.000000 smac-2.0.2/MANIFEST.in
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7245 2023-08-01 13:20:09.885776 smac-2.0.2/PKG-INFO
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6116 2023-07-31 15:47:05.000000 smac-2.0.2/README.md
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2887 2023-07-31 15:47:05.000000 smac-2.0.2/pyproject.toml
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       38 2023-08-01 13:20:09.885776 smac-2.0.2/setup.cfg
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2051 2023-08-01 13:05:49.000000 smac-2.0.2/setup.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1555 2023-08-01 13:05:49.000000 smac-2.0.2/smac/__init__.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/acquisition/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/__init__.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/acquisition/function/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      717 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3552 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/abstract_acquisition_function.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3086 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/confidence_bound.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9061 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/expected_improvement.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4002 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/integrated_acquisition_function.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9380 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/prior_acqusition_function.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2692 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/probability_improvement.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1930 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/function/thompson.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/acquisition/maximizer/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      649 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6213 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/abstract_acqusition_maximizer.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2344 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/differential_evolution.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4165 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/helpers.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10116 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/local_and_random_search.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    19915 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/local_search.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1828 2023-07-31 15:47:05.000000 smac-2.0.2/smac/acquisition/maximizer/random_search.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/callback/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      160 2023-07-31 15:47:05.000000 smac-2.0.2/smac/callback/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2519 2023-07-31 15:47:05.000000 smac-2.0.2/smac/callback/callback.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1013 2023-07-31 15:47:05.000000 smac-2.0.2/smac/callback/metadata_callback.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      270 2023-07-31 15:47:05.000000 smac-2.0.2/smac/constants.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/facade/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      674 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    21480 2023-08-01 13:05:49.000000 smac-2.0.2/smac/facade/abstract_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6199 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/algorithm_configuration_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11605 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/blackbox_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2394 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/hyperband_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7578 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/hyperparameter_optimization_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4387 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/multi_fidelity_facade.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5976 2023-07-31 15:47:05.000000 smac-2.0.2/smac/facade/random_facade.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/initial_design/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      621 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8211 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/abstract_initial_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      552 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/default_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2202 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/factorial_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1084 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/latin_hypercube_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      656 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/random_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1671 2023-07-31 15:47:05.000000 smac-2.0.2/smac/initial_design/sobol_design.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/intensifier/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      341 2023-07-31 15:47:05.000000 smac-2.0.2/smac/intensifier/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    33241 2023-07-31 15:47:05.000000 smac-2.0.2/smac/intensifier/abstract_intensifier.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2159 2023-07-31 15:47:05.000000 smac-2.0.2/smac/intensifier/hyperband.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17357 2023-07-31 15:47:05.000000 smac-2.0.2/smac/intensifier/intensifier.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    24527 2023-08-01 13:05:49.000000 smac-2.0.2/smac/intensifier/successive_halving.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      553 2023-07-31 15:47:05.000000 smac-2.0.2/smac/logging.yml
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/main/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-07-31 15:47:05.000000 smac-2.0.2/smac/main/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    14855 2023-08-01 13:05:49.000000 smac-2.0.2/smac/main/config_selector.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    24653 2023-08-01 13:05:49.000000 smac-2.0.2/smac/main/smbo.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac/model/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      247 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    11457 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/abstract_model.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/model/gaussian_process/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      350 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6523 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/abstract_gaussian_process.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10482 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/gaussian_process.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    35950 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/gpytorch_gaussian_process.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/model/gaussian_process/kernels/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      607 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    23169 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/_boing.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    17056 2023-08-01 13:05:49.000000 smac-2.0.2/smac/model/gaussian_process/kernels/base_kernels.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3648 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/hamming_kernel.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4121 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/matern_kernel.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2738 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/rbf_kernel.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1881 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/kernels/white_kernel.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    16808 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/mcmc_gaussian_process.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/model/gaussian_process/priors/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      435 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4306 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/abstract_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2013 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/gamma_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2402 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/horseshoe_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1900 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/log_normal_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     5338 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/gaussian_process/priors/tophat_prior.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3002 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/multi_objective_model.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/model/random_forest/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      208 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/random_forest/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1741 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/random_forest/abstract_random_forest.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10805 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/random_forest/random_forest.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1206 2023-07-31 15:47:05.000000 smac-2.0.2/smac/model/random_model.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/multi_objective/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      333 2023-07-31 15:47:05.000000 smac-2.0.2/smac/multi_objective/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1038 2023-07-31 15:47:05.000000 smac-2.0.2/smac/multi_objective/abstract_multi_objective_algorithm.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1399 2023-07-31 15:47:05.000000 smac-2.0.2/smac/multi_objective/aggregation_strategy.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1902 2023-07-31 15:47:05.000000 smac-2.0.2/smac/multi_objective/parego.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.2/smac/py.typed
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/random_design/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      585 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1362 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/abstract_random_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2691 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/annealing_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     3489 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/modulus_design.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2439 2023-07-31 15:47:05.000000 smac-2.0.2/smac/random_design/probability_design.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/runhistory/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      393 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4337 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/dataclasses.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/runhistory/encoder/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1076 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10551 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/abstract_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2443 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/boing_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2878 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/eips_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2540 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1372 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/inverse_scaled_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      867 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/log_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1180 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/log_scaled_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      978 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/scaled_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1354 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/encoder/sqrt_scaled_encoder.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      356 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/enumerations.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       48 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runhistory/errors.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    41527 2023-08-01 13:05:49.000000 smac-2.0.2/smac/runhistory/runhistory.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/runner/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      472 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9402 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/abstract_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1787 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/abstract_serial_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9153 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/dask_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      419 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/exceptions.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9356 2023-08-01 13:05:49.000000 smac-2.0.2/smac/runner/target_function_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7486 2023-07-31 15:47:05.000000 smac-2.0.2/smac/runner/target_function_script_runner.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    10868 2023-07-31 15:47:05.000000 smac-2.0.2/smac/scenario.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/utils/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        0 2023-03-03 09:52:31.000000 smac-2.0.2/smac/utils/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     9299 2023-08-01 13:05:49.000000 smac-2.0.2/smac/utils/configspace.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     2276 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/data_structures.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1252 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/logging.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     1167 2023-08-01 13:05:49.000000 smac-2.0.2/smac/utils/multi_objective.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     6018 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/pareto_front.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.885776 smac-2.0.2/smac/utils/subspaces/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    29592 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/subspaces/__init__.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     8717 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/subspaces/boing_subspace.py
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)    13823 2023-07-31 15:47:05.000000 smac-2.0.2/smac/utils/subspaces/turbo_subspace.py
+drwxrwxr-x   0 skrebs    (1000) skrebs    (1000)        0 2023-08-01 13:20:09.881776 smac-2.0.2/smac.egg-info/
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     7245 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/PKG-INFO
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)     4513 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/SOURCES.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)        1 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/dependency_links.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)      324 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/requires.txt
+-rw-rw-r--   0 skrebs    (1000) skrebs    (1000)       11 2023-08-01 13:20:09.000000 smac-2.0.2/smac.egg-info/top_level.txt
```

### Comparing `smac-2.0.1/LICENSE.txt` & `smac-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/PKG-INFO` & `smac-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smac
-Version: 2.0.1
+Version: 2.0.2
 Summary: SMAC3, a Python implementation of 'Sequential Model-based Algorithm Configuration'.
 Home-page: https://www.automl.org/
 Author: 	Marius Lindauer, Katharina Eggensperger, Matthias Feurer, André Biedenkapp, Difan Deng,
 	Carolin Benjamins, Tim Ruhkopf, René Sass and Frank Hutter
 Author-email: fh@cs.uni-freiburg.de
 License: BSD 3-Clause License
 Project-URL: Documentation, https://https://github.com/automl.github.io/SMAC3/main
@@ -17,15 +17,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: gpytorch
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # SMAC3: A Versatile Bayesian Optimization Package for Hyperparameter Optimization
 
 
 [![Tests](https://github.com/automl/SMAC3/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/automl/SMAC3/actions/workflows/pytest.yml)
@@ -168,9 +167,7 @@
   number  = {54},
   pages   = {1--9},
   url     = {http://jmlr.org/papers/v23/21-0888.html}
 }
 ```
 
 Copyright (C) 2016-2022  [AutoML Group](http://www.automl.org).
-
-
```

### Comparing `smac-2.0.1/README.md` & `smac-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/pyproject.toml` & `smac-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/setup.py` & `smac-2.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
 
 def read_file(filepath: str) -> str:
     with open(filepath, "r", encoding="utf-8") as fh:
         return fh.read()
 
 
-torch_requirements = ["torch>=1.9.0", "gpytorch>=1.5.0", "pyro-ppl>=1.7.0", "botorch>=0.5.0"]
 extras_require = {
-    "gpytorch": torch_requirements,
     "dev": [
         "setuptools",
         "types-setuptools",
         # Test
         "pytest>=4.6",
         "pytest-cov",
         "pytest-xdist",
@@ -36,15 +34,14 @@
         # Others
         "mypy",
         "isort",
         "black",
         "pydocstyle",
         "flake8",
         "pre-commit",
-        *torch_requirements,
     ],
 }
 
 setuptools.setup(
     name=package_name,
     author=author,
     author_email=author_email,
@@ -72,17 +69,14 @@
         "emcee>=3.0.0",
         "regex",
         "pyyaml",
     ],
     extras_require=extras_require,
     test_suite="pytest",
     platforms=["Linux"],
-    entry_points={
-        "console_scripts": ["smac = smac.smac_cli:cmd_line_call"],
-    },
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Natural Language :: English",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
```

### Comparing `smac-2.0.1/smac/__init__.py` & `smac-2.0.2/smac/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Documentation": "https://https://github.com/automl.github.io/SMAC3/main",
     "Source Code": "https://github.com/https://github.com/automl/smac",
 }
 copyright = f"""
     Copyright {datetime.date.today().strftime('%Y')}, Marius Lindauer, Katharina Eggensperger,
     Matthias Feurer, André Biedenkapp, Difan Deng, Carolin Benjamins, Tim Ruhkopf, René Sass
     and Frank Hutter"""
-version = "2.0.1"
+version = "2.0.2"
 
 
 try:
     from smac.callback.callback import Callback
     from smac.facade import (
         AlgorithmConfigurationFacade,
         BlackBoxFacade,
```

### Comparing `smac-2.0.1/smac/acquisition/function/__init__.py` & `smac-2.0.2/smac/acquisition/function/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/function/abstract_acquisition_function.py` & `smac-2.0.2/smac/acquisition/function/abstract_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/function/confidence_bound.py` & `smac-2.0.2/smac/acquisition/function/confidence_bound.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/function/expected_improvement.py` & `smac-2.0.2/smac/acquisition/function/expected_improvement.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/function/integrated_acquisition_function.py` & `smac-2.0.2/smac/acquisition/function/integrated_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/function/prior_acqusition_function.py` & `smac-2.0.2/smac/acquisition/function/prior_acqusition_function.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/function/probability_improvement.py` & `smac-2.0.2/smac/acquisition/function/probability_improvement.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/function/thompson.py` & `smac-2.0.2/smac/acquisition/function/thompson.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/maximizer/__init__.py` & `smac-2.0.2/smac/acquisition/maximizer/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/maximizer/abstract_acqusition_maximizer.py` & `smac-2.0.2/smac/acquisition/maximizer/abstract_acqusition_maximizer.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/maximizer/differential_evolution.py` & `smac-2.0.2/smac/acquisition/maximizer/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/maximizer/helpers.py` & `smac-2.0.2/smac/acquisition/maximizer/helpers.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/maximizer/local_and_random_search.py` & `smac-2.0.2/smac/acquisition/maximizer/local_and_random_search.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/maximizer/local_search.py` & `smac-2.0.2/smac/acquisition/maximizer/local_search.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/acquisition/maximizer/random_search.py` & `smac-2.0.2/smac/acquisition/maximizer/random_search.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/callback/callback.py` & `smac-2.0.2/smac/callback/callback.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/callback/metadata_callback.py` & `smac-2.0.2/smac/callback/metadata_callback.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/facade/__init__.py` & `smac-2.0.2/smac/facade/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/facade/abstract_facade.py` & `smac-2.0.2/smac/facade/abstract_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,16 +88,18 @@
         expected with the logging configuration. If nothing is passed, the default logging.yml from SMAC is used.
         If False is passed, SMAC will not do any customization of the logging setup and the responsibility is left
         to the user.
     callbacks: list[Callback], defaults to []
         Callbacks, which are incorporated into the optimization loop.
     overwrite: bool, defaults to False
         When True, overwrites the run results if a previous run is found that is
-        inconsistent in the meta data with the current setup. If ``overwrite`` is set to False, the user is asked
-        for the exact behaviour (overwrite completely, save old run, or use old results).
+        consistent in the meta data with the current setup. When False and a previous run is found that is
+        consistent in the meta data, the run is continued. When False and a previous run is found that is
+        not consistent in the meta data, the the user is asked for the exact behaviour (overwrite completely
+        or rename old run first).
     dask_client: Client | None, defaults to None
         User-created dask client, which can be used to start a dask cluster and then attach SMAC to it. This will not
         be closed automatically and will have to be closed manually if provided explicitly. If none is provided
         (default), a local one will be created for you and closed upon completion.
     """
 
     def __init__(
@@ -306,14 +308,17 @@
 
         Returns
         -------
         incumbent : Configuration
             Best found configuration.
         """
         incumbents = None
+        if isinstance(data_to_scatter, dict) and len(data_to_scatter) == 0:
+            raise ValueError("data_to_scatter must be None or dict with some elements, but got an empty dict.")
+
         try:
             incumbents = self._optimizer.optimize(data_to_scatter=data_to_scatter)
         finally:
             self._optimizer.save()
 
         return incumbents
 
@@ -451,14 +456,26 @@
         self._intensifier.runhistory = self._runhistory
 
     def _validate(self) -> None:
         """Checks if the composition is correct if there are dependencies."""
         # Make sure the same acquisition function is used
         assert self._acquisition_function == self._acquisition_maximizer._acquisition_function
 
+        if isinstance(self._runner, DaskParallelRunner) and (
+            self.scenario.trial_walltime_limit is not None or self.scenario.trial_memory_limit is not None
+        ):
+            # This is probably due to pickling dask jobs
+            raise ValueError(
+                "Parallelization via Dask cannot be used in combination with limiting "
+                "the resources "
+                "of the target function via `scenario.trial_walltime_limit` or "
+                "`scenario.trial_memory_limit`. Set those to `None` if you want "
+                "parallelization. "
+            )
+
     def _get_signature_arguments(self) -> list[str]:
         """Returns signature arguments, which are required by the intensifier."""
         arguments = []
 
         if self._intensifier.uses_seeds:
             arguments += ["seed"]
```

### Comparing `smac-2.0.1/smac/facade/algorithm_configuration_facade.py` & `smac-2.0.2/smac/facade/algorithm_configuration_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/facade/blackbox_facade.py` & `smac-2.0.2/smac/facade/blackbox_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/facade/hyperband_facade.py` & `smac-2.0.2/smac/facade/hyperband_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/facade/hyperparameter_optimization_facade.py` & `smac-2.0.2/smac/facade/hyperparameter_optimization_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/facade/multi_fidelity_facade.py` & `smac-2.0.2/smac/facade/multi_fidelity_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/facade/random_facade.py` & `smac-2.0.2/smac/facade/random_facade.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/initial_design/__init__.py` & `smac-2.0.2/smac/initial_design/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/initial_design/abstract_initial_design.py` & `smac-2.0.2/smac/initial_design/abstract_initial_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/initial_design/default_design.py` & `smac-2.0.2/smac/initial_design/default_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/initial_design/factorial_design.py` & `smac-2.0.2/smac/initial_design/factorial_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/initial_design/latin_hypercube_design.py` & `smac-2.0.2/smac/initial_design/latin_hypercube_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/initial_design/random_design.py` & `smac-2.0.2/smac/initial_design/random_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/initial_design/sobol_design.py` & `smac-2.0.2/smac/initial_design/sobol_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/intensifier/abstract_intensifier.py` & `smac-2.0.2/smac/intensifier/abstract_intensifier.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/intensifier/hyperband.py` & `smac-2.0.2/smac/intensifier/hyperband.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/intensifier/intensifier.py` & `smac-2.0.2/smac/intensifier/intensifier.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/intensifier/successive_halving.py` & `smac-2.0.2/smac/intensifier/successive_halving.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,15 +554,16 @@
             # Idea: We recursively calculate the pareto front in every iteration
             for incumbent in incumbents:
                 configs.remove(incumbent)
                 selected_configs.append(incumbent)
 
         # If we have more selected configs, we remove the ones with the smallest crowding distance
         if len(selected_configs) > n_configs:
-            selected_configs = sort_by_crowding_distance(rh, configs, all_keys)[:n_configs]
+            all_keys = [from_keys for _ in selected_configs]
+            selected_configs = sort_by_crowding_distance(rh, selected_configs, all_keys)[:n_configs]
             logger.debug("Found more configs than required. Removed configs with smallest crowding distance.")
 
         return selected_configs
 
     def _get_next_order_seed(self) -> int | None:
         """Next instances shuffle seed to use."""
         # Here we have the option to shuffle the trials when specified by the user
```

### Comparing `smac-2.0.1/smac/logging.yml` & `smac-2.0.2/smac/logging.yml`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/main/config_selector.py` & `smac-2.0.2/smac/main/config_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,22 +262,22 @@
 
         If no budgets are used, this is equivalent to returning all observations.
         """
         assert self._runhistory is not None
         assert self._runhistory_encoder is not None
 
         # If we use a float value as a budget, we want to train the model only on the highest budget
-        available_budgets = []
-        for run_key in self._runhistory:
-            budget = run_key.budget
-            if budget not in available_budgets:
-                available_budgets.append(run_key.budget)
+        unique_budgets: set[float] = {run_key.budget for run_key in self._runhistory if run_key.budget is not None}
 
-        # Sort available budgets from highest to lowest budget
-        available_budgets = sorted(list(set(available_budgets)), reverse=True)  # type: ignore
+        available_budgets: list[float] | list[None]
+        if len(unique_budgets) > 0:
+            # Sort available budgets from highest to lowest budget
+            available_budgets = sorted(unique_budgets, reverse=True)
+        else:
+            available_budgets = [None]
 
         # Get #points per budget and if there are enough samples, then build a model
         for b in available_budgets:
             X, Y = self._runhistory_encoder.transform(budget_subset=[b])
 
             if X.shape[0] >= self._min_trials:
                 self._considered_budgets = [b]
```

### Comparing `smac-2.0.1/smac/main/smbo.py` & `smac-2.0.2/smac/main/smbo.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,26 +457,30 @@
                 if len(cost) != len(cost_threshold):
                     raise RuntimeError("You must specify a termination cost threshold for each objective.")
 
                 if all(cost[i] < cost_threshold[i] for i in range(len(cost))):
                     logger.info("Cost threshold was reached. Abort is requested.")
                     self._stop = True
 
-    def register_callback(self, callback: Callback, index: int = -1) -> None:
+    def register_callback(self, callback: Callback, index: int | None = None) -> None:
         """
         Registers a callback to be called before, in between, and after the Bayesian optimization loop.
 
+        Callback is appended to the list by default.
 
         Parameters
         ----------
         callback : Callback
             The callback to be registered.
-        index : int
-            The index at which the callback should be registered.
+        index : int, optional
+            The index at which the callback should be registered. The default is None.
+            If it is None, append the callback to the list.
         """
+        if index is None:
+            index = len(self._callbacks)
         self._callbacks.insert(index, callback)
 
     def _initialize_state(self) -> None:
         """Detects whether the optimization is restored from a previous state."""
         # Here we actually check whether the run should be continued or not.
         # More precisely, we update our smbo/runhistory/intensifier object if all component arguments
         # and scenario object are the same. For doing so, we create a specific hash.
@@ -497,15 +501,15 @@
                     self.load()
 
                     # If the last run was not successful, we reset everything again
                     if self._runhistory.submitted <= 1 and self._runhistory.finished == 0:
                         logger.info("Since the previous run was not successful, SMAC will start from scratch again.")
                         self.reset()
                 else:
-                    # Here, we run into differen scenarios
+                    # Here, we run into different scenarios
                     diff = recursively_compare_dicts(
                         Scenario.make_serializable(self._scenario),
                         Scenario.make_serializable(old_scenario),
                         level="scenario",
                     )
                     logger.info(
                         f"Found old run in `{self._scenario.output_directory}` but it is not the same as the current "
```

### Comparing `smac-2.0.1/smac/model/abstract_model.py` & `smac-2.0.2/smac/model/abstract_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/abstract_gaussian_process.py` & `smac-2.0.2/smac/model/gaussian_process/abstract_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/gaussian_process.py` & `smac-2.0.2/smac/model/gaussian_process/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/gpytorch_gaussian_process.py` & `smac-2.0.2/smac/model/gaussian_process/gpytorch_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/kernels/__init__.py` & `smac-2.0.2/smac/model/gaussian_process/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/kernels/_boing.py` & `smac-2.0.2/smac/model/gaussian_process/kernels/_boing.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/kernels/base_kernels.py` & `smac-2.0.2/smac/model/gaussian_process/kernels/base_kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,20 +246,20 @@
 
             return sig
         else:
             return sig_
 
     def _set_active_dims(self, operate_on: np.ndarray | None = None) -> None:
         """Sets dimensions this kernel should work on."""
-        if operate_on is not None and type(operate_on) in (list, np.ndarray):
+        if operate_on is not None and isinstance(operate_on, (list, np.ndarray)):
             if not isinstance(operate_on, np.ndarray):
-                raise TypeError("The argument `operate_on` needs to be of type np.ndarray but is %s" % type(operate_on))
+                raise TypeError(f"The argument `operate_on` needs to be of type np.ndarray but is {type(operate_on)}")
 
-            if operate_on.dtype != int:
-                raise ValueError("The dtype of argument `operate_on` needs to be int, but is %s" % operate_on.dtype)
+            if not np.issubdtype(operate_on.dtype, np.integer):
+                raise ValueError(f"The dtype of `operate_on` needs to be np.integer, but is {operate_on.dtype}")
 
             self.operate_on = operate_on
             self._len_active = len(operate_on)
         else:
             self.operate_on = None
             self._len_active = None
```

### Comparing `smac-2.0.1/smac/model/gaussian_process/kernels/hamming_kernel.py` & `smac-2.0.2/smac/model/gaussian_process/kernels/hamming_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/kernels/matern_kernel.py` & `smac-2.0.2/smac/model/gaussian_process/kernels/matern_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/kernels/rbf_kernel.py` & `smac-2.0.2/smac/model/gaussian_process/kernels/rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/kernels/white_kernel.py` & `smac-2.0.2/smac/model/gaussian_process/kernels/white_kernel.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/mcmc_gaussian_process.py` & `smac-2.0.2/smac/model/gaussian_process/mcmc_gaussian_process.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/priors/abstract_prior.py` & `smac-2.0.2/smac/model/gaussian_process/priors/abstract_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/priors/gamma_prior.py` & `smac-2.0.2/smac/model/gaussian_process/priors/gamma_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/priors/horseshoe_prior.py` & `smac-2.0.2/smac/model/gaussian_process/priors/horseshoe_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/priors/log_normal_prior.py` & `smac-2.0.2/smac/model/gaussian_process/priors/log_normal_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/gaussian_process/priors/tophat_prior.py` & `smac-2.0.2/smac/model/gaussian_process/priors/tophat_prior.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/multi_objective_model.py` & `smac-2.0.2/smac/model/multi_objective_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/random_forest/abstract_random_forest.py` & `smac-2.0.2/smac/model/random_forest/abstract_random_forest.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/random_forest/random_forest.py` & `smac-2.0.2/smac/model/random_forest/random_forest.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/model/random_model.py` & `smac-2.0.2/smac/model/random_model.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/multi_objective/abstract_multi_objective_algorithm.py` & `smac-2.0.2/smac/multi_objective/abstract_multi_objective_algorithm.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/multi_objective/aggregation_strategy.py` & `smac-2.0.2/smac/multi_objective/aggregation_strategy.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/multi_objective/parego.py` & `smac-2.0.2/smac/multi_objective/parego.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/random_design/__init__.py` & `smac-2.0.2/smac/random_design/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/random_design/abstract_random_design.py` & `smac-2.0.2/smac/random_design/abstract_random_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/random_design/annealing_design.py` & `smac-2.0.2/smac/random_design/annealing_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/random_design/modulus_design.py` & `smac-2.0.2/smac/random_design/modulus_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/random_design/probability_design.py` & `smac-2.0.2/smac/random_design/probability_design.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/dataclasses.py` & `smac-2.0.2/smac/runhistory/dataclasses.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/__init__.py` & `smac-2.0.2/smac/runhistory/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/abstract_encoder.py` & `smac-2.0.2/smac/runhistory/encoder/abstract_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/boing_encoder.py` & `smac-2.0.2/smac/runhistory/encoder/boing_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/eips_encoder.py` & `smac-2.0.2/smac/runhistory/encoder/eips_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/encoder.py` & `smac-2.0.2/smac/runhistory/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/inverse_scaled_encoder.py` & `smac-2.0.2/smac/runhistory/encoder/inverse_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/log_encoder.py` & `smac-2.0.2/smac/runhistory/encoder/log_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/log_scaled_encoder.py` & `smac-2.0.2/smac/runhistory/encoder/log_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/scaled_encoder.py` & `smac-2.0.2/smac/runhistory/encoder/scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/encoder/sqrt_scaled_encoder.py` & `smac-2.0.2/smac/runhistory/encoder/sqrt_scaled_encoder.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runhistory/runhistory.py` & `smac-2.0.2/smac/runhistory/runhistory.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,23 +431,23 @@
         min_cost: float
             Computed cost for configuration
         """
         config_id = self._config_ids.get(config)
         cost = self._min_cost_per_config.get(config_id, np.nan)  # type: ignore
 
         if self._n_objectives > 1:
-            assert type(cost) == list
+            assert isinstance(cost, list)
             assert self.multi_objective_algorithm is not None
 
             costs = normalize_costs(cost, self._objective_bounds)
 
             # Note: We have to mean here because we already got the min cost
             return self.multi_objective_algorithm(costs)
 
-        assert type(cost) == float
+        assert isinstance(cost, float)
         return float(cost)
 
     def average_cost(
         self,
         config: Configuration,
         instance_seed_budget_keys: list[InstanceSeedBudgetKey] | None = None,
         normalize: bool = False,
@@ -843,15 +843,15 @@
         self._config_ids = {config: id_ for id_, config in self._ids_config.items()}
         self._n_id = len(self._config_ids)
 
         # Important to use add method to use all data structure correctly
         for entry in data["data"]:
             # Set n_objectives first
             if self._n_objectives == -1:
-                if isinstance(entry[4], float) or isinstance(entry[4], int):
+                if isinstance(entry[4], (float, int)):
                     self._n_objectives = 1
                 else:
                     self._n_objectives = len(entry[4])
 
             cost: list[float] | float
             if self._n_objectives == 1:
                 cost = float(entry[4])
```

### Comparing `smac-2.0.1/smac/runner/abstract_runner.py` & `smac-2.0.2/smac/runner/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runner/abstract_serial_runner.py` & `smac-2.0.2/smac/runner/abstract_serial_runner.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runner/dask_runner.py` & `smac-2.0.2/smac/runner/dask_runner.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/runner/target_function_runner.py` & `smac-2.0.2/smac/runner/target_function_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Callable
 
 import copy
 import inspect
 import math
 import time
 import traceback
+from functools import partial
 
 import numpy as np
 from ConfigSpace import Configuration
 from pynisher import MemoryLimitException, WallTimeoutException, limit
 
 from smac.runner.abstract_runner import StatusType
 from smac.runner.abstract_serial_runner import AbstractSerialRunner
@@ -84,15 +85,25 @@
 
         self._memory_limit = memory
         self._algorithm_walltime_limit = time
 
     @property
     def meta(self) -> dict[str, Any]:  # noqa: D102
         meta = super().meta
-        meta.update({"code": str(self._target_function.__code__.co_code)})
+
+        # Partial's don't have a __code__ attribute but are a convenient
+        # way a user might want to pass a function to SMAC, specifying
+        # keyword arguments.
+        f = self._target_function
+        if isinstance(f, partial):
+            f = f.func
+            meta.update({"code": str(f.__code__.co_code)})
+            meta.update({"code-partial-args": repr(f)})
+        else:
+            meta.update({"code": str(self._target_function.__code__.co_code)})
 
         return meta
 
     def run(
         self,
         config: Configuration,
         instance: str | None = None,
```

### Comparing `smac-2.0.1/smac/runner/target_function_script_runner.py` & `smac-2.0.2/smac/runner/target_function_script_runner.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/scenario.py` & `smac-2.0.2/smac/scenario.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/utils/configspace.py` & `smac-2.0.2/smac/utils/configspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,20 +165,25 @@
     challenger: Configuration | None,
     logger: logging.Logger,
 ) -> None:
     """Compares two configurations and prints the differences."""
     if incumbent is None or challenger is None:
         return
 
-    params = sorted([(param, incumbent[param], challenger[param]) for param in challenger.keys()])
-    for param in params:
-        if param[1] != param[2]:
-            logger.info("--- %s: %r -> %r" % param)
-        else:
-            logger.debug("--- %s Remains unchanged: %r", param[0], param[1])
+    inc_keys = set(incumbent.keys())
+    all_keys = inc_keys.union(challenger.keys())
+
+    lines = []
+    for k in sorted(all_keys):
+        inc_k = incumbent.get(k, "-inactive-")
+        cha_k = challenger.get(k, "-inactive-")
+        lines.append(f"--- {k}: {inc_k} -> {cha_k}" + " (unchanged)" if inc_k == cha_k else "")
+
+    msg = "\n".join(lines)
+    logger.debug(msg)
 
 
 # def check_subspace_points(
 #     X: np.ndarray,
 #     cont_dims: np.ndarray | list = [],
 #     cat_dims: np.ndarray | list = [],
 #     bounds_cont: np.ndarray | None = None,
```

### Comparing `smac-2.0.1/smac/utils/data_structures.py` & `smac-2.0.2/smac/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/utils/logging.py` & `smac-2.0.2/smac/utils/logging.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/utils/multi_objective.py` & `smac-2.0.2/smac/utils/multi_objective.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return values
 
     if len(values) != len(bounds):
         raise ValueError("Number of values and bounds must be equal.")
 
     costs = []
     for v, b in zip(values, bounds):
-        assert type(v) != list
+        assert not isinstance(v, list)
         p = v - b[0]
         q = b[1] - b[0]
 
         if q < 1e-10:
             cost = 1.0
         else:
             cost = p / q
```

### Comparing `smac-2.0.1/smac/utils/pareto_front.py` & `smac-2.0.2/smac/utils/pareto_front.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/utils/subspaces/__init__.py` & `smac-2.0.2/smac/utils/subspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/utils/subspaces/boing_subspace.py` & `smac-2.0.2/smac/utils/subspaces/boing_subspace.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac/utils/subspaces/turbo_subspace.py` & `smac-2.0.2/smac/utils/subspaces/turbo_subspace.py`

 * *Files identical despite different names*

### Comparing `smac-2.0.1/smac.egg-info/PKG-INFO` & `smac-2.0.2/smac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smac
-Version: 2.0.1
+Version: 2.0.2
 Summary: SMAC3, a Python implementation of 'Sequential Model-based Algorithm Configuration'.
 Home-page: https://www.automl.org/
 Author: 	Marius Lindauer, Katharina Eggensperger, Matthias Feurer, André Biedenkapp, Difan Deng,
 	Carolin Benjamins, Tim Ruhkopf, René Sass and Frank Hutter
 Author-email: fh@cs.uni-freiburg.de
 License: BSD 3-Clause License
 Project-URL: Documentation, https://https://github.com/automl.github.io/SMAC3/main
@@ -17,15 +17,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: gpytorch
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # SMAC3: A Versatile Bayesian Optimization Package for Hyperparameter Optimization
 
 
 [![Tests](https://github.com/automl/SMAC3/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/automl/SMAC3/actions/workflows/pytest.yml)
@@ -168,9 +167,7 @@
   number  = {54},
   pages   = {1--9},
   url     = {http://jmlr.org/papers/v23/21-0888.html}
 }
 ```
 
 Copyright (C) 2016-2022  [AutoML Group](http://www.automl.org).
-
-
```

### Comparing `smac-2.0.1/smac.egg-info/SOURCES.txt` & `smac-2.0.2/smac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 smac/constants.py
 smac/logging.yml
 smac/py.typed
 smac/scenario.py
 smac.egg-info/PKG-INFO
 smac.egg-info/SOURCES.txt
 smac.egg-info/dependency_links.txt
-smac.egg-info/entry_points.txt
 smac.egg-info/requires.txt
 smac.egg-info/top_level.txt
 smac/acquisition/__init__.py
 smac/acquisition/function/__init__.py
 smac/acquisition/function/abstract_acquisition_function.py
 smac/acquisition/function/confidence_bound.py
 smac/acquisition/function/expected_improvement.py
```

