# Comparing `tmp/linear_operator-0.5.0.tar.gz` & `tmp/linear_operator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear_operator-0.5.0.tar", last modified: Fri Jun  2 19:27:08 2023, max compression
+gzip compressed data, was "linear_operator-0.5.1.tar", last modified: Tue Aug  1 20:10:37 2023, max compression
```

## Comparing `linear_operator-0.5.0.tar` & `linear_operator-0.5.1.tar`

### file list

```diff
@@ -1,188 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.208408 linear_operator-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.184408 linear_operator-0.5.0/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.180408 linear_operator-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.184408 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/documentation_examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/refactor.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.184408 linear_operator-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/push_to_main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/run_linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/run_test_suite.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/run_type_checked_test_suite.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.184408 linear_operator-0.5.0/.hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.hooks/check_type_hints.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.hooks/propagate_type_hints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.hooks/propagate_type_hints.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-02 19:26:50.000000 linear_operator-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 19:26:50.000000 linear_operator-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-02 19:27:08.208408 linear_operator-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-06-02 19:26:50.000000 linear_operator-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/composition_decoration_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/converting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/custom_linear_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/data_sparse_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/linear_operator.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/namespace.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-02 19:26:50.000000 linear_operator-0.5.0/examples/LinearOperator_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/linear_operator/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.192408 linear_operator-0.5.0/linear_operator/functions/
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_dsmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_inv_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_inv_quad_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_root_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_sqrt_inv_matmul.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.196408 linear_operator-0.5.0/linear_operator/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129865 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/batch_repeat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/block_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/block_interleaved_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/block_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/cat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/chol_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/constant_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/dense_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/identity_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22567 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/interpolated_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/keops_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/kernel_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16274 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/kronecker_product_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/linear_operator_representation_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/low_rank_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/matmul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/permutation_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/psd_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/sum_batch_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/sum_kronecker_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/toeplitz_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/triangular_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/zero_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.196408 linear_operator-0.5.0/linear_operator/test/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    56208 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/linear_operator_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/type_checking_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.200408 linear_operator-0.5.0/linear_operator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/broadcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/contour_integral_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/lanczos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/minres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/permutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/pinverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/stochastic_lq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/toeplitz.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/linear_operator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-06-02 19:27:08.000000 linear_operator-0.5.0/linear_operator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-02 19:26:50.000000 linear_operator-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-02 19:27:08.208408 linear_operator-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-02 19:26:50.000000 linear_operator-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.200408 linear_operator-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.204408 linear_operator-0.5.0/test/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_dsmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_inv_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_inv_quad_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_root_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.208408 linear_operator-0.5.0/test/operators/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_batch_repeat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_block_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_block_interleaved_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_cat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_chol_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_constant_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_dense_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_identity_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_interpolated_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_kernel_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_kronecker_product_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_kronecker_product_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_low_rank_root_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_low_rank_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_matmul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_permutation_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_psd_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_sum_batch_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_sum_kronecker_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_toeplitz_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_triangular_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_zero_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.208408 linear_operator-0.5.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_lanczos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_minres.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_permutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_toeplitz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.634119 linear_operator-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.602118 linear_operator-0.5.1/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.602118 linear_operator-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.602118 linear_operator-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/ISSUE_TEMPLATE/documentation_examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/ISSUE_TEMPLATE/refactor.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.602118 linear_operator-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/workflows/push_to_main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/workflows/run_linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/workflows/run_test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.github/workflows/run_type_checked_test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.606119 linear_operator-0.5.1/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.hooks/check_type_hints.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.hooks/propagate_type_hints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.hooks/propagate_type_hints.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 20:10:26.000000 linear_operator-0.5.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-08-01 20:10:26.000000 linear_operator-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 20:10:26.000000 linear_operator-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-08-01 20:10:37.634119 linear_operator-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-08-01 20:10:26.000000 linear_operator-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.606119 linear_operator-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.606119 linear_operator-0.5.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/composition_decoration_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/converting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/custom_linear_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/data_sparse_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/linear_operator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/namespace.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 20:10:26.000000 linear_operator-0.5.1/docs/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.606119 linear_operator-0.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-08-01 20:10:26.000000 linear_operator-0.5.1/examples/LinearOperator_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.606119 linear_operator-0.5.1/linear_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.606119 linear_operator-0.5.1/linear_operator/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_dsmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_inv_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_inv_quad_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_root_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/functions/_sqrt_inv_matmul.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.618119 linear_operator-0.5.1/linear_operator/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130183 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/batch_repeat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/block_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/block_interleaved_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/block_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/cat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/chol_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/constant_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/dense_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/identity_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/interpolated_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/keops_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/kernel_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16274 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/kronecker_product_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/kronecker_product_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/linear_operator_representation_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/low_rank_root_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/low_rank_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/masked_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/matmul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/permutation_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/psd_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/sum_batch_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/sum_kronecker_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/toeplitz_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/triangular_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/operators/zero_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.618119 linear_operator-0.5.1/linear_operator/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/test/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56866 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/test/linear_operator_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/test/type_checking_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.626119 linear_operator-0.5.1/linear_operator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/broadcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/contour_integral_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/minres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/pinverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/stochastic_lq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/toeplitz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-01 20:10:26.000000 linear_operator-0.5.1/linear_operator/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 20:10:37.000000 linear_operator-0.5.1/linear_operator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.606119 linear_operator-0.5.1/linear_operator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-08-01 20:10:37.000000 linear_operator-0.5.1/linear_operator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-08-01 20:10:37.000000 linear_operator-0.5.1/linear_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:10:37.000000 linear_operator-0.5.1/linear_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 20:10:37.000000 linear_operator-0.5.1/linear_operator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 20:10:37.000000 linear_operator-0.5.1/linear_operator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-01 20:10:26.000000 linear_operator-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-01 20:10:37.634119 linear_operator-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-01 20:10:26.000000 linear_operator-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.626119 linear_operator-0.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.626119 linear_operator-0.5.1/test/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/test_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/test_dsmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/test_inv_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/test_inv_quad_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/test_root_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/functions/test_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.630119 linear_operator-0.5.1/test/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_batch_repeat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_block_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_block_interleaved_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_cat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_chol_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_constant_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_dense_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_identity_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_interpolated_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_kernel_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_kronecker_product_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_kronecker_product_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_low_rank_root_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_low_rank_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_masked_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_matmul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_permutation_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_psd_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_sum_batch_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_sum_kronecker_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_toeplitz_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_triangular_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/operators/test_zero_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:10:37.634119 linear_operator-0.5.1/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_minres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-01 20:10:26.000000 linear_operator-0.5.1/test/utils/test_toeplitz.py
```

### Comparing `linear_operator-0.5.0/.conda/meta.yaml` & `linear_operator-0.5.1/.conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `linear_operator-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.github/ISSUE_TEMPLATE/documentation_examples.md` & `linear_operator-0.5.1/.github/ISSUE_TEMPLATE/documentation_examples.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `linear_operator-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.github/workflows/deploy.yml` & `linear_operator-0.5.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.github/workflows/pull_request.yml` & `linear_operator-0.5.1/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.github/workflows/run_linter.yml` & `linear_operator-0.5.1/.github/workflows/run_linter.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.github/workflows/run_test_suite.yml` & `linear_operator-0.5.1/.github/workflows/run_test_suite.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.github/workflows/run_type_checked_test_suite.yml` & `linear_operator-0.5.1/.github/workflows/run_type_checked_test_suite.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.gitignore` & `linear_operator-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.hooks/propagate_type_hints.py` & `linear_operator-0.5.1/.hooks/propagate_type_hints.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.pre-commit-config.yaml` & `linear_operator-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/.readthedocs.yml` & `linear_operator-0.5.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/CONTRIBUTING.md` & `linear_operator-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/LICENSE` & `linear_operator-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/PKG-INFO` & `linear_operator-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear_operator
-Version: 0.5.0
+Version: 0.5.1
 Summary: A linear operator implementation, primarily designed for finite-dimensional positive definite operators (i.e. kernel matrices).
 Home-page: UNKNOWN
 Author: Geoff Pleiss
 Author-email: gpleiss@gmail.com
 License: MIT
 Project-URL: Documentation, https://linear_operator.readthedocs.io
 Project-URL: Source, https://github.com/cornellius-gp/linear_operator/
```

### Comparing `linear_operator-0.5.0/README.md` & `linear_operator-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/docs/Makefile` & `linear_operator-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/docs/make.bat` & `linear_operator-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/docs/source/composition_decoration_operators.rst` & `linear_operator-0.5.1/docs/source/composition_decoration_operators.rst`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 
 :hidden:`KroneckerProductDiagLinearOperator`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: linear_operator.operators.KroneckerProductDiagLinearOperator
    :members:
 
+:hidden:`MaskedLinearOperator`
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: linear_operator.operators.MaskedLinearOperator
+   :members:
+
 :hidden:`MatmulLinearOperator`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: linear_operator.operators.MatmulLinearOperator
    :members:
 
 :hidden:`MulLinearOperator`
```

### Comparing `linear_operator-0.5.0/docs/source/conf.py` & `linear_operator-0.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/docs/source/custom_linear_operators.rst` & `linear_operator-0.5.1/docs/source/custom_linear_operators.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/docs/source/data_sparse_operators.rst` & `linear_operator-0.5.1/docs/source/data_sparse_operators.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/docs/source/index.rst` & `linear_operator-0.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/docs/source/namespace.rst` & `linear_operator-0.5.1/docs/source/namespace.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/examples/LinearOperator_demo.ipynb` & `linear_operator-0.5.1/examples/LinearOperator_demo.ipynb`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/__init__.py` & `linear_operator-0.5.1/linear_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/beta_features.py` & `linear_operator-0.5.1/linear_operator/beta_features.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/__init__.py` & `linear_operator-0.5.1/linear_operator/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/_diagonalization.py` & `linear_operator-0.5.1/linear_operator/functions/_diagonalization.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/_inv_quad.py` & `linear_operator-0.5.1/linear_operator/functions/_inv_quad.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/_inv_quad_logdet.py` & `linear_operator-0.5.1/linear_operator/functions/_inv_quad_logdet.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/_matmul.py` & `linear_operator-0.5.1/linear_operator/functions/_matmul.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/_pivoted_cholesky.py` & `linear_operator-0.5.1/linear_operator/functions/_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/_root_decomposition.py` & `linear_operator-0.5.1/linear_operator/functions/_root_decomposition.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/_solve.py` & `linear_operator-0.5.1/linear_operator/functions/_solve.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/functions/_sqrt_inv_matmul.py` & `linear_operator-0.5.1/linear_operator/functions/_sqrt_inv_matmul.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/__init__.py` & `linear_operator-0.5.1/linear_operator/operators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .kronecker_product_linear_operator import (
     KroneckerProductDiagLinearOperator,
     KroneckerProductLinearOperator,
     KroneckerProductTriangularLinearOperator,
 )
 from .low_rank_root_added_diag_linear_operator import LowRankRootAddedDiagLinearOperator
 from .low_rank_root_linear_operator import LowRankRootLinearOperator
+from .masked_linear_operator import MaskedLinearOperator
 from .matmul_linear_operator import MatmulLinearOperator
 from .mul_linear_operator import MulLinearOperator
 from .permutation_linear_operator import PermutationLinearOperator, TransposePermutationLinearOperator
 from .psd_sum_linear_operator import PsdSumLinearOperator
 from .root_linear_operator import RootLinearOperator
 from .sum_batch_linear_operator import SumBatchLinearOperator
 from .sum_kronecker_linear_operator import SumKroneckerLinearOperator
@@ -58,14 +59,15 @@
     "KroneckerProductLinearOperator",
     "KroneckerProductAddedDiagLinearOperator",
     "KroneckerProductDiagLinearOperator",
     "KroneckerProductTriangularLinearOperator",
     "SumKroneckerLinearOperator",
     "LowRankRootAddedDiagLinearOperator",
     "LowRankRootLinearOperator",
+    "MaskedLinearOperator",
     "MatmulLinearOperator",
     "MulLinearOperator",
     "PermutationLinearOperator",
     "PsdSumLinearOperator",
     "RootLinearOperator",
     "SumLinearOperator",
     "SumBatchLinearOperator",
```

### Comparing `linear_operator-0.5.0/linear_operator/operators/_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/_linear_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -2019,14 +2019,18 @@
                      [0.5000, 1.0000, 4.0000]]])
 
         :param sizes: The number of times to repeat this tensor along each dimension.
         :return: A LinearOperator with repeated dimensions.
         """
         from .batch_repeat_linear_operator import BatchRepeatLinearOperator
 
+        # Short path if no repetition is necessary
+        if all(x == 1 for x in sizes) and len(sizes) == self.dim():
+            return self
+
         if len(sizes) < 3 or tuple(sizes[-2:]) != (1, 1):
             raise RuntimeError(
                 "Invalid repeat arguments {}. Currently, repeat only works to create repeated "
                 "batches of a 2D LinearOperator.".format(tuple(sizes))
             )
 
         return BatchRepeatLinearOperator(self, batch_repeat=torch.Size(sizes[:-2]))
@@ -2641,30 +2645,36 @@
         A device-agnostic method of moving the LienarOperator to the specified dtype.
         This method operates similarly to :func:`torch.Tensor.dtype`.
 
         :param dtype: Target dtype.
         """
         attr_flag = _TYPES_DICT[dtype]
 
+        def _type_helper(arg):
+            if arg.dtype.is_floating_point:
+                return arg.to(dtype)
+            else:
+                return arg
+
         new_args = []
         new_kwargs = {}
         for arg in self._args:
             if hasattr(arg, attr_flag):
                 try:
-                    new_args.append(arg.clone().to(dtype))
+                    new_args.append(_type_helper(arg.clone()))
                 except AttributeError:
-                    new_args.append(deepcopy(arg).to(dtype))
+                    new_args.append(_type_helper(deepcopy(arg)))
             else:
                 new_args.append(arg)
         for name, val in self._kwargs.items():
             if hasattr(val, attr_flag):
                 try:
-                    new_kwargs[name] = val.clone().to(dtype)
+                    new_kwargs[name] = _type_helper(val.clone())
                 except AttributeError:
-                    new_kwargs[name] = deepcopy(val).to(dtype)
+                    new_kwargs[name] = _type_helper(deepcopy(val))
             else:
                 new_kwargs[name] = val
         return self.__class__(*new_args, **new_kwargs)
 
     @_implements(torch.unsqueeze)
     def unsqueeze(self, dim: int) -> LinearOperator:
         """
```

### Comparing `linear_operator-0.5.0/linear_operator/operators/added_diag_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/batch_repeat_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/batch_repeat_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/block_diag_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/block_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/block_interleaved_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/block_interleaved_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/block_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/block_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/cat_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/cat_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/chol_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/chol_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/constant_mul_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/constant_mul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/dense_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/dense_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/diag_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/identity_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/identity_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/interpolated_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/interpolated_linear_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,23 +401,14 @@
         block_diag = BlockDiagLinearOperator(self.base_linear_op, block_dim=dim)
 
         # Finally! We have an interpolated lazy tensor again
         return InterpolatedLinearOperator(
             block_diag, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
         )
 
-    def double(
-        self: Float[LinearOperator, "*batch M N"], device_id: Optional[str] = None
-    ) -> Float[LinearOperator, "*batch M N"]:
-        # We need to ensure that the indices remain integers.
-        new_lt = super().double(device_id=device_id)
-        new_lt.left_interp_indices = new_lt.left_interp_indices.type(torch.int64)
-        new_lt.right_interp_indices = new_lt.right_interp_indices.type(torch.int64)
-        return new_lt
-
     def matmul(
         self: Float[LinearOperator, "*batch M N"],
         other: Union[Float[Tensor, "*batch2 N P"], Float[Tensor, "*batch2 N"], Float[LinearOperator, "*batch2 N P"]],
     ) -> Union[Float[Tensor, "... M P"], Float[Tensor, "... M"], Float[LinearOperator, "... M P"]]:
         # We're using a custom matmul here, because it is significantly faster than
         # what we get from the function factory.
         # The _matmul_closure is optimized for repeated calls, such as for _solve
```

### Comparing `linear_operator-0.5.0/linear_operator/operators/keops_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/keops_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/kernel_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/kernel_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/kronecker_product_added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/kronecker_product_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/kronecker_product_linear_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,18 @@
                 f"({', '.join([str(tuple(linear_op.shape)) for linear_op in linear_ops])}) "
                 "are incompatible for a Kronecker product."
             )
 
         if len(batch_broadcast_shape):  # Otherwise all linear_ops are non-batch, and we don't need to expand
             # NOTE: we must explicitly call requires_grad on each of these arguments
             # for the automatic _bilinear_derivative to work in torch.autograd.Functions
-            linear_ops = [
+            linear_ops = tuple(
                 linear_op._expand_batch(batch_broadcast_shape).requires_grad_(linear_op.requires_grad)
                 for linear_op in linear_ops
-            ]
+            )
 
         super().__init__(*linear_ops)
         self.linear_ops = linear_ops
 
     def __add__(
         self: Float[LinearOperator, "... #M #N"],
         other: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"], float],
```

### Comparing `linear_operator-0.5.0/linear_operator/operators/linear_operator_representation_tree.py` & `linear_operator-0.5.1/linear_operator/operators/linear_operator_representation_tree.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/low_rank_root_added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/low_rank_root_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/low_rank_root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/matmul_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/matmul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/mul_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/mul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/permutation_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/permutation_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/psd_sum_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/psd_sum_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/root_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/sum_batch_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/sum_batch_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/sum_kronecker_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/sum_kronecker_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/sum_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/sum_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/toeplitz_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/toeplitz_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/triangular_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/triangular_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/operators/zero_linear_operator.py` & `linear_operator-0.5.1/linear_operator/operators/zero_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/settings.py` & `linear_operator-0.5.1/linear_operator/settings.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/test/base_test_case.py` & `linear_operator-0.5.1/linear_operator/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/test/linear_operator_test_case.py` & `linear_operator-0.5.1/linear_operator/test/linear_operator_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,28 @@
         return self._test_rmatmul(lhs)
 
     def test_matmul_matrix(self):
         linear_op = self.create_linear_op()
         rhs = torch.randn(*linear_op.batch_shape, linear_op.size(-1), 4)
         return self._test_matmul(rhs)
 
+    def test_t_matmul_matrix(self):
+        with torch.no_grad():
+            linear_op = self.create_linear_op()
+            rhs = torch.randn(*linear_op.batch_shape, linear_op.size(-2), 4)
+            linear_op_copy = torch.clone(linear_op)
+            evaluated = self.evaluate_linear_op(linear_op_copy)
+            rhs_evaluated = to_dense(rhs)
+
+            # Test operator
+            res = linear_op._t_matmul(rhs)
+            actual = evaluated.mT.matmul(rhs_evaluated)
+            res_evaluated = to_dense(res)
+            self.assertAllClose(res_evaluated, actual)
+
     def test_rmatmul_matrix(self):
         linear_op = self.create_linear_op()
         lhs = torch.randn(*linear_op.batch_shape, 4, linear_op.size(-2))
         return self._test_rmatmul(lhs)
 
     def test_matmul_diag_matrix(self):
         linear_op = self.create_linear_op()
@@ -680,15 +694,18 @@
 
         deriv_custom = linear_op._bilinear_derivative(left_vecs, right_vecs)
         deriv_auto = linear_operator.operators.LinearOperator._bilinear_derivative(
             linear_op_clone, left_vecs, right_vecs
         )
 
         for dc, da in zip(deriv_custom, deriv_auto):
-            self.assertAllClose(dc, da)
+            if dc is None:
+                assert da is None
+            else:
+                self.assertAllClose(dc, da)
 
     def test_cat_rows(self):
         linear_op = self.create_linear_op()
         evaluated = self.evaluate_linear_op(linear_op)
 
         for batch_shape in (torch.Size(), torch.Size([2])):
             new_rows = 1e-4 * torch.randn(*batch_shape, *linear_op.shape[:-2], 1, linear_op.shape[-1])
```

### Comparing `linear_operator-0.5.0/linear_operator/test/type_checking_test_case.py` & `linear_operator-0.5.1/linear_operator/test/type_checking_test_case.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/test/utils.py` & `linear_operator-0.5.1/linear_operator/test/utils.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/__init__.py` & `linear_operator-0.5.1/linear_operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/broadcasting.py` & `linear_operator-0.5.1/linear_operator/utils/broadcasting.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/cholesky.py` & `linear_operator-0.5.1/linear_operator/utils/cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/contour_integral_quad.py` & `linear_operator-0.5.1/linear_operator/utils/contour_integral_quad.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/deprecation.py` & `linear_operator-0.5.1/linear_operator/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/generic.py` & `linear_operator-0.5.1/linear_operator/utils/generic.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/getitem.py` & `linear_operator-0.5.1/linear_operator/utils/getitem.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/interpolation.py` & `linear_operator-0.5.1/linear_operator/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/lanczos.py` & `linear_operator-0.5.1/linear_operator/utils/lanczos.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/linear_cg.py` & `linear_operator-0.5.1/linear_operator/utils/linear_cg.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     # But we'll store which norms were actually close to zero
     rhs_norm = rhs.norm(2, dim=-2, keepdim=True)
     rhs_is_zero = rhs_norm.lt(eps)
     rhs_norm = rhs_norm.masked_fill_(rhs_is_zero, 1)
 
     # Let's normalize. We'll un-normalize afterwards
     rhs = rhs.div(rhs_norm)
+    initial_guess = initial_guess.div(rhs_norm)
 
     # residual: residual_{0} = b_vec - lhs x_{0}
     residual = rhs - matmul_closure(initial_guess)
     batch_shape = residual.shape[:-2]
 
     # result <- x_{0}
     result = initial_guess.expand_as(residual).contiguous()
```

### Comparing `linear_operator-0.5.0/linear_operator/utils/memoize.py` & `linear_operator-0.5.1/linear_operator/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/minres.py` & `linear_operator-0.5.1/linear_operator/utils/minres.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/permutation.py` & `linear_operator-0.5.1/linear_operator/utils/permutation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/pinverse.py` & `linear_operator-0.5.1/linear_operator/utils/pinverse.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/qr.py` & `linear_operator-0.5.1/linear_operator/utils/qr.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/sparse.py` & `linear_operator-0.5.1/linear_operator/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/stochastic_lq.py` & `linear_operator-0.5.1/linear_operator/utils/stochastic_lq.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator/utils/toeplitz.py` & `linear_operator-0.5.1/linear_operator/utils/toeplitz.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/linear_operator.egg-info/PKG-INFO` & `linear_operator-0.5.1/linear_operator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-operator
-Version: 0.5.0
+Version: 0.5.1
 Summary: A linear operator implementation, primarily designed for finite-dimensional positive definite operators (i.e. kernel matrices).
 Home-page: UNKNOWN
 Author: Geoff Pleiss
 Author-email: gpleiss@gmail.com
 License: MIT
 Project-URL: Documentation, https://linear_operator.readthedocs.io
 Project-URL: Source, https://github.com/cornellius-gp/linear_operator/
```

### Comparing `linear_operator-0.5.0/linear_operator.egg-info/SOURCES.txt` & `linear_operator-0.5.1/linear_operator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 linear_operator/operators/keops_linear_operator.py
 linear_operator/operators/kernel_linear_operator.py
 linear_operator/operators/kronecker_product_added_diag_linear_operator.py
 linear_operator/operators/kronecker_product_linear_operator.py
 linear_operator/operators/linear_operator_representation_tree.py
 linear_operator/operators/low_rank_root_added_diag_linear_operator.py
 linear_operator/operators/low_rank_root_linear_operator.py
+linear_operator/operators/masked_linear_operator.py
 linear_operator/operators/matmul_linear_operator.py
 linear_operator/operators/mul_linear_operator.py
 linear_operator/operators/permutation_linear_operator.py
 linear_operator/operators/psd_sum_linear_operator.py
 linear_operator/operators/root_linear_operator.py
 linear_operator/operators/sum_batch_linear_operator.py
 linear_operator/operators/sum_kronecker_linear_operator.py
@@ -140,14 +141,15 @@
 test/operators/test_identity_linear_operator.py
 test/operators/test_interpolated_linear_operator.py
 test/operators/test_kernel_linear_operator.py
 test/operators/test_kronecker_product_added_diag_linear_operator.py
 test/operators/test_kronecker_product_linear_operator.py
 test/operators/test_low_rank_root_added_diag_linear_operator.py
 test/operators/test_low_rank_root_linear_operator.py
+test/operators/test_masked_linear_operator.py
 test/operators/test_matmul_linear_operator.py
 test/operators/test_mul_linear_operator.py
 test/operators/test_permutation_linear_operator.py
 test/operators/test_psd_sum_linear_operator.py
 test/operators/test_root_linear_operator.py
 test/operators/test_sum_batch_linear_operator.py
 test/operators/test_sum_kronecker_linear_operator.py
@@ -160,9 +162,10 @@
 test/utils/test_generic.py
 test/utils/test_getitem.py
 test/utils/test_interpolation.py
 test/utils/test_lanczos.py
 test/utils/test_linear_cg.py
 test/utils/test_minres.py
 test/utils/test_permutation.py
+test/utils/test_repeat.py
 test/utils/test_sparse.py
 test/utils/test_toeplitz.py
```

### Comparing `linear_operator-0.5.0/setup.py` & `linear_operator-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/functions/test_diagonalization.py` & `linear_operator-0.5.1/test/functions/test_diagonalization.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/functions/test_dsmm.py` & `linear_operator-0.5.1/test/functions/test_dsmm.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/functions/test_inv_quad.py` & `linear_operator-0.5.1/test/functions/test_inv_quad.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/functions/test_inv_quad_logdet.py` & `linear_operator-0.5.1/test/functions/test_inv_quad_logdet.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/functions/test_matmul.py` & `linear_operator-0.5.1/test/functions/test_matmul.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/functions/test_pivoted_cholesky.py` & `linear_operator-0.5.1/test/functions/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/functions/test_root_decomposition.py` & `linear_operator-0.5.1/test/functions/test_root_decomposition.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/functions/test_solve.py` & `linear_operator-0.5.1/test/functions/test_solve.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_added_diag_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_batch_repeat_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_batch_repeat_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_block_diag_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_block_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_block_interleaved_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_block_interleaved_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_cat_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_cat_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_chol_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_chol_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_constant_mul_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_constant_mul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_dense_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_dense_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_diag_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_identity_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_identity_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_interpolated_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_interpolated_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_kernel_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_kernel_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_kronecker_product_added_diag_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_kronecker_product_added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_kronecker_product_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_kronecker_product_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_low_rank_root_added_diag_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_low_rank_root_added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_low_rank_root_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_low_rank_root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_matmul_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_matmul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_mul_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_mul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_permutation_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_permutation_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_psd_sum_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_psd_sum_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_root_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_sum_batch_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_sum_batch_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_sum_kronecker_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_sum_kronecker_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_sum_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_sum_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_toeplitz_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_toeplitz_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_triangular_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_triangular_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/operators/test_zero_linear_operator.py` & `linear_operator-0.5.1/test/operators/test_zero_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/test_settings.py` & `linear_operator-0.5.1/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_cholesky.py` & `linear_operator-0.5.1/test/utils/test_cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_generic.py` & `linear_operator-0.5.1/test/utils/test_generic.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_getitem.py` & `linear_operator-0.5.1/test/utils/test_getitem.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_interpolation.py` & `linear_operator-0.5.1/test/utils/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_lanczos.py` & `linear_operator-0.5.1/test/utils/test_lanczos.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_linear_cg.py` & `linear_operator-0.5.1/test/utils/test_linear_cg.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,10 +139,30 @@
         # Check tridiag
         for i in range(5):
             eigs = torch.linalg.eigvalsh(matrix[i])
             for j in range(8):
                 approx_eigs = torch.linalg.eigvalsh(t_mats[j, i])
                 self.assertTrue(torch.allclose(eigs, approx_eigs, atol=1e-3, rtol=1e-4))
 
+    def test_batch_cg_init(self):
+        batch = 5
+        size = 100
+        matrix = torch.randn(batch, size, size, dtype=torch.float64)
+        matrix = matrix.matmul(matrix.mT)
+        matrix.div_(matrix.norm())
+        matrix.add_(torch.eye(matrix.size(-1), dtype=torch.float64).mul_(1e-1))
+
+        # Initial solve
+        rhs = torch.randn(batch, size, 50, dtype=torch.float64)
+        solves = linear_cg(matrix.matmul, rhs=rhs, max_iter=size, max_tridiag_iter=0)
+
+        # Initialize with solve
+        solves_with_init = linear_cg(matrix.matmul, rhs=rhs, max_iter=1, initial_guess=solves, max_tridiag_iter=0)
+
+        # Check cg
+        matrix_chol = torch.linalg.cholesky(matrix)
+        actual = torch.cholesky_solve(rhs, matrix_chol)
+        self.assertTrue(torch.allclose(solves_with_init, actual, atol=1e-3, rtol=1e-4))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `linear_operator-0.5.0/test/utils/test_minres.py` & `linear_operator-0.5.1/test/utils/test_minres.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_permutation.py` & `linear_operator-0.5.1/test/utils/test_permutation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_sparse.py` & `linear_operator-0.5.1/test/utils/test_sparse.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.5.0/test/utils/test_toeplitz.py` & `linear_operator-0.5.1/test/utils/test_toeplitz.py`

 * *Files identical despite different names*

