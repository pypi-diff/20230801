# Comparing `tmp/pyglove-0.4.3.dev20230731.tar.gz` & `tmp/pyglove-0.4.3.dev20230801.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.4.3.dev20230731.tar", last modified: Mon Jul 31 08:07:36 2023, max compression
+gzip compressed data, was "pyglove-0.4.3.dev20230801.tar", last modified: Tue Aug  1 08:06:50 2023, max compression
```

## Comparing `pyglove-0.4.3.dev20230731.tar` & `pyglove-0.4.3.dev20230801.tar`

### file list

```diff
@@ -1,196 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.139619 pyglove-0.4.3.dev20230731/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-31 08:07:36.139619 pyglove-0.4.3.dev20230731/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-31 08:07:34.000000 pyglove-0.4.3.dev20230731/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.123618 pyglove-0.4.3.dev20230731/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.123618 pyglove-0.4.3.dev20230731/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.123618 pyglove-0.4.3.dev20230731/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.123618 pyglove-0.4.3.dev20230731/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.127619 pyglove-0.4.3.dev20230731/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.127619 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.131619 pyglove-0.4.3.dev20230731/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.131619 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73654 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    64587 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/inferred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/inferred_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57908 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    82689 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.135619 pyglove-0.4.3.dev20230731/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.135619 pyglove-0.4.3.dev20230731/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.135619 pyglove-0.4.3.dev20230731/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.135619 pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.139619 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.139619 pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.139619 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:07:36.123618 pyglove-0.4.3.dev20230731/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-31 08:07:36.000000 pyglove-0.4.3.dev20230731/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-31 08:07:36.000000 pyglove-0.4.3.dev20230731/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:07:36.000000 pyglove-0.4.3.dev20230731/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 08:07:36.000000 pyglove-0.4.3.dev20230731/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 08:07:36.000000 pyglove-0.4.3.dev20230731/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:07:36.139619 pyglove-0.4.3.dev20230731/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-31 08:07:24.000000 pyglove-0.4.3.dev20230731/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-01 08:06:48.000000 pyglove-0.4.3.dev20230801/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.024967 pyglove-0.4.3.dev20230801/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.024967 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.024967 pyglove-0.4.3.dev20230801/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.028967 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73654 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64587 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24126 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29164 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/inferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/inferred_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57908 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82689 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/ref_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.028967 pyglove-0.4.3.dev20230801/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.032967 pyglove-0.4.3.dev20230801/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.032967 pyglove-0.4.3.dev20230801/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.032967 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.032967 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/setup.py
```

### Comparing `pyglove-0.4.3.dev20230731/LICENSE` & `pyglove-0.4.3.dev20230801/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/PKG-INFO` & `pyglove-0.4.3.dev20230801/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.3.dev20230731
+Version: 0.4.3.dev20230801
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.3.dev20230731/README.md` & `pyglove-0.4.3.dev20230801/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,22 @@
 List = symbolic.List
 list = List   # pylint: disable=redefined-builtin
 
 Object = symbolic.Object
 ClassWrapper = symbolic.ClassWrapper
 Functor = symbolic.Functor
 
+# Inferentiable base classes.
+Inferentiable = symbolic.Inferential
+InferredValue = symbolic.InferredValue
+
+# Reference types.
+Ref = symbolic.Ref
+maybe_ref = symbolic.maybe_ref
+
 # Decorator for declaring symbolic. members for `pg.Object`.
 members = symbolic.members
 
 # Decorator for updating the __init__ signature of `pg.Object`.
 use_init_args = symbolic.use_init_args
 
 #
@@ -161,18 +169,14 @@
 
 # Auxiliary classes:
 Origin = symbolic.Origin
 FieldUpdate = symbolic.FieldUpdate
 Insertion = symbolic.Insertion
 WritePermissionError = symbolic.WritePermissionError
 
-# Inferentiable classes.
-Inferentiable = symbolic.Inferential
-InferredValue = symbolic.InferredValue
-
 #
 # Symbols from 'typing.py'
 #
 
 # NOTE(daiyip): we introduce 'typing' as an alias for 'schema' sub-module, since
 # it may be easier to comprehend when users use pytype.
 from pyglove.core import typing
```

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/detouring/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/detouring/class_detour.py` & `pyglove-0.4.3.dev20230801/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/base.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/base_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/categorical.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/categorical_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/custom.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/custom_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/deduping.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/deduping_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/dna_generator.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/numerical.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/numerical_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/random.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/random_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/space.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/space_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/sweeping.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/geno/sweeping_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/base.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/categorical.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/categorical_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/custom.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/custom_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/derived.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/derived_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/evolvable.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/iter.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/iter_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/numerical.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/numerical_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/object_template.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/hyper/object_template_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/logging.py` & `pyglove-0.4.3.dev20230801/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/logging_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/codegen.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/common_traits.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/formatting.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/missing.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/missing_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/thread_local.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/value_location.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/patching/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/patching/object_factory.py` & `pyglove-0.4.3.dev20230801/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/patching/object_factory_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/patching/pattern_based.py` & `pyglove-0.4.3.dev20230801/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/patching/rule_based.py` & `pyglove-0.4.3.dev20230801/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/patching/rule_based_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,14 @@
 
 from pyglove.core.symbolic.flags import notify_on_change
 from pyglove.core.symbolic.flags import is_change_notification_enabled
 
 from pyglove.core.symbolic.flags import auto_call_functors
 from pyglove.core.symbolic.flags import should_call_functors_during_init
 
-# Inferential values
-from pyglove.core.symbolic.base import Inferential
-
-from pyglove.core.symbolic.inferred import InferredValue
-from pyglove.core.symbolic.inferred import ValueFromParentChain
-
 # Symbolic types and their definition helpers.
 from pyglove.core.symbolic.base import Symbolic
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.dict import Dict
 
 from pyglove.core.symbolic.object import ObjectMeta
 from pyglove.core.symbolic.object import Object
@@ -88,14 +82,24 @@
 
 from pyglove.core.symbolic.symbolize import symbolize
 
 from pyglove.core.symbolic.compounding import compound
 from pyglove.core.symbolic.compounding import compound_class
 from pyglove.core.symbolic.boilerplate import boilerplate_class
 
+# Inferential types.
+from pyglove.core.symbolic.base import Inferential
+
+from pyglove.core.symbolic.inferred import InferredValue
+from pyglove.core.symbolic.inferred import ValueFromParentChain
+
+# Reference type.
+from pyglove.core.symbolic.ref import Ref
+from pyglove.core.symbolic.ref import maybe_ref
+
 # Symbolic operations.
 from pyglove.core.symbolic.base import traverse
 from pyglove.core.symbolic.base import query
 
 from pyglove.core.symbolic.base import eq
 from pyglove.core.symbolic.base import ne
 from pyglove.core.symbolic.base import lt
```

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/base.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/base_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/compounding.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/compounding.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/compounding_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/dict.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/dict_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/diff.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/diff_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/flags.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/flags_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/functor.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/functor.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,14 +577,16 @@
     KeyError: names of symbolic arguments are not compatible with
       function signature.
     TypeError: types of symbolic arguments are not compatible with
       function signature.
     ValueError: default values of symbolic arguments are not compatible
       with  function signature.
   """
+  if not inspect.isfunction(func):
+    raise TypeError(f'{func!r} is not a function.')
 
   class _Functor(base_class or Functor):
     """Functor wrapper for input function."""
 
     def _call(self, *args, **kwargs):
       return func(*args, **kwargs)
```

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/functor_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/functor_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,19 +195,19 @@
   def test_auto_doc(self):
     @pg_functor([
         ('a', pg_typing.Int()),
         ('b', pg_typing.Int()),
     ], returns=pg_typing.Int(), auto_doc=True)
     def f(a=1, b=2):
       """Compute the sum.
-      
+
       Args:
         a: an integer.
         b: another integer.
-      
+
       Returns:
         Sum of two integers.
       """
       return a + b
 
     self.assertEqual(f.schema.description, 'Compute the sum.')
     self.assertEqual(
@@ -354,15 +354,15 @@
     self.assertEqual(
         f.signature.args, [pg_typing.Argument('x', pg_typing.Any())])
     self.assertIsNone(f.signature.return_value)
     self.assertEqual(f(1), 1)
 
   def test_bad_definition(self):
     # `pg.functor` decorator is not applicable to class.
-    with self.assertRaisesRegex(TypeError, '.* is not a method.'):
+    with self.assertRaisesRegex(TypeError, '.* is not a function.'):
 
       @pg_functor([('a', pg_typing.Int())])
       class A:
         pass
 
       del A
```

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/inferred.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/inferred.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/inferred_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/inferred_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/list.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/list_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/object.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/object.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/object_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/object_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/origin.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/origin_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/symbolize.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/backend.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/backend_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/early_stopping.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/local_backend.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/protocols.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/protocols_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/sample.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/tuning/sample_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/callable_ext.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/callable_signature.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/class_schema.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/class_schema_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/custom_typing.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/generic.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/generic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/generic_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/generic_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     self.assertTrue(generic.has_generic_bases(C))
 
   def test_get_type(self):
     self.assertIs(generic.get_type(str), str)
     self.assertIs(generic.get_type(A), A)
     self.assertIs(generic.get_type(A[str, int]), A)
     with self.assertRaisesRegex(TypeError, '.* is not a type.'):
-      generic.get_type(Any)
+      generic.get_type(1)
 
   def test_get_type_args(self):
     self.assertEqual(generic.get_type_args(str), ())
     self.assertEqual(generic.get_type_args(A), ())
     self.assertEqual(generic.get_type_args(A[str, int]), (str, int))
     self.assertEqual(generic.get_type_args(B1, A), ())
     self.assertEqual(generic.get_type_args(B1[str], A), ())
```

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/key_specs.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/key_specs_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/pytype_support.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/type_conversion.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/typed_missing.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/value_specs.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/core/typing/value_specs_test.py` & `pyglove-0.4.3.dev20230801/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/base.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/base.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/base_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/mutators.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/neat.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/neat_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/nsga2.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/recombinators.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/selectors.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/where.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/evolution/where_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/base.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/base_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/__init__.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/base.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/base_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/maths.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/maths_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/randoms.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/step_wise.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230731/pyglove.egg-info/PKG-INFO` & `pyglove-0.4.3.dev20230801/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.3.dev20230731
+Version: 0.4.3.dev20230801
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.3.dev20230731/pyglove.egg-info/SOURCES.txt` & `pyglove-0.4.3.dev20230801/pyglove.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,16 @@
 pyglove/core/symbolic/list.py
 pyglove/core/symbolic/list_test.py
 pyglove/core/symbolic/object.py
 pyglove/core/symbolic/object_test.py
 pyglove/core/symbolic/origin.py
 pyglove/core/symbolic/origin_test.py
 pyglove/core/symbolic/pure_symbolic.py
+pyglove/core/symbolic/ref.py
+pyglove/core/symbolic/ref_test.py
 pyglove/core/symbolic/schema_utils.py
 pyglove/core/symbolic/schema_utils_test.py
 pyglove/core/symbolic/symbolize.py
 pyglove/core/symbolic/symbolize_test.py
 pyglove/core/tuning/__init__.py
 pyglove/core/tuning/backend.py
 pyglove/core/tuning/backend_test.py
```

### Comparing `pyglove-0.4.3.dev20230731/setup.py` & `pyglove-0.4.3.dev20230801/setup.py`

 * *Files identical despite different names*

