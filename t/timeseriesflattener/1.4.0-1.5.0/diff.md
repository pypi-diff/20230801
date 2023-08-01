# Comparing `tmp/timeseriesflattener-1.4.0.tar.gz` & `tmp/timeseriesflattener-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-1.4.0.tar", last modified: Wed Jul 12 10:44:44 2023, max compression
+gzip compressed data, was "timeseriesflattener-1.5.0.tar", last modified: Tue Aug  1 09:11:36 2023, max compression
```

## Comparing `timeseriesflattener-1.4.0.tar` & `timeseriesflattener-1.5.0.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/
--rw-r--r--   0 root         (0) root         (0)      489 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      738 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.514534 timeseriesflattener-1.4.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.510533 timeseriesflattener-1.4.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.514534 timeseriesflattener-1.4.0/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      892 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.514534 timeseriesflattener-1.4.0/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      948 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.514534 timeseriesflattener-1.4.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)      849 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      868 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3056 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2871 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    56956 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    11550 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9122 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.518534 timeseriesflattener-1.4.0/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.518534 timeseriesflattener-1.4.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4173 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.518534 timeseriesflattener-1.4.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   118804 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    50220 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    72388 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4290 2023-07-12 10:44:34.000000 timeseriesflattener-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/src/
--rw-r--r--   0 root         (0) root         (0)     1996 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      309 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     5559 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     7090 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     8765 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    36395 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3008 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8082 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.510533 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.510533 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1505 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.526534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.538534 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      812 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     1392 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.538534 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.538534 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3425 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18309 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2688 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     8190 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/text_embedding_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.542534 timeseriesflattener-1.4.0/src/timeseriesflattener/utils/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/src/timeseriesflattener/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:44:44.522534 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11550 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5042 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      685 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 10:44:44.000000 timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9390 2023-07-12 10:44:33.000000 timeseriesflattener-1.4.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.588750 timeseriesflattener-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.552749 timeseriesflattener-1.5.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.544749 timeseriesflattener-1.5.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.552749 timeseriesflattener-1.5.0/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.552749 timeseriesflattener-1.5.0/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.556749 timeseriesflattener-1.5.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      868 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    57710 2023-08-01 09:11:25.000000 timeseriesflattener-1.5.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-08-01 09:11:36.588750 timeseriesflattener-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9122 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.556749 timeseriesflattener-1.5.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.560750 timeseriesflattener-1.5.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      332 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.560750 timeseriesflattener-1.5.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   118804 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50220 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)   111479 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.560750 timeseriesflattener-1.5.0/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.564750 timeseriesflattener-1.5.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-08-01 09:11:25.000000 timeseriesflattener-1.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 09:11:36.592750 timeseriesflattener-1.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.564750 timeseriesflattener-1.5.0/src/
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.564750 timeseriesflattener-1.5.0/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      309 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/column_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/df_transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.568750 timeseriesflattener-1.5.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.568750 timeseriesflattener-1.5.0/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     8765 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    36395 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.568750 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.572750 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.548749 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.548749 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.572750 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.572750 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.588750 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      812 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.588750 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.588750 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.588750 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_df_transforms.py
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.588750 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18309 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/text_embedding_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.588750 timeseriesflattener-1.5.0/src/timeseriesflattener/utils/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/src/timeseriesflattener/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:11:36.568750 timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11550 2023-08-01 09:11:36.000000 timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5160 2023-08-01 09:11:36.000000 timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 09:11:36.000000 timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      685 2023-08-01 09:11:36.000000 timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-01 09:11:36.000000 timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9390 2023-08-01 09:11:24.000000 timeseriesflattener-1.5.0/tasks.py
```

### Comparing `timeseriesflattener-1.4.0/.cruft.json` & `timeseriesflattener-1.5.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/actions/test/action.yml` & `timeseriesflattener-1.5.0/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-1.5.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/dependabot.yml` & `timeseriesflattener-1.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/recommended_repo_setup.md` & `timeseriesflattener-1.5.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/check_for_rej.yml` & `timeseriesflattener-1.5.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/cruft.yml` & `timeseriesflattener-1.5.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-1.5.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/documentation.yml` & `timeseriesflattener-1.5.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-1.5.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-1.5.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/pre-commit.yml` & `timeseriesflattener-1.5.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/stalebot.yml` & `timeseriesflattener-1.5.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.github/workflows/static_type_checks.yml` & `timeseriesflattener-1.5.0/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.gitignore` & `timeseriesflattener-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.pre-commit-config.yaml` & `timeseriesflattener-1.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/.zenodo.json` & `timeseriesflattener-1.5.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/CHANGELOG.md` & `timeseriesflattener-1.5.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.0 (2023-08-01)
+
+### Feature
+
+* Convert df with multiple values to named dataframes ([`ca797e6`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/ca797e66288eb011d58579814b84c858243f71f8))
+
+### Fix
+
+* Update name of column in synth text ([`bd58c4d`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/bd58c4dce341d1acddd59ee958027ce755c1b934))
+* Handle int column names ([`00c6a91`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/00c6a91696aa3e0258e9cdf591556b4d0c2941df))
+
+### Documentation
+
+* Add how to use pre-embedded text to text tutorial ([`c0f994c`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/c0f994c34c6c2623d719116cebe35761ffdf6782))
+
 ## v1.4.0 (2023-07-12)
 
 ### Feature
 
 * Change int detection for new version of pydantic ([`752d3bf`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/752d3bfd1702525bb30f285e4f3b8b0f4edf9a6d))
 
 ### Fix
```

### Comparing `timeseriesflattener-1.4.0/CODE_OF_CONDUCT.md` & `timeseriesflattener-1.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/CONTRIBUTING.md` & `timeseriesflattener-1.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/LICENSE` & `timeseriesflattener-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/PKG-INFO` & `timeseriesflattener-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.4.0
+Version: 1.5.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.4.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.5.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.4.0/README.md` & `timeseriesflattener-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/citation.cff` & `timeseriesflattener-1.5.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/Makefile` & `timeseriesflattener-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/_static/favicon.ico` & `timeseriesflattener-1.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/_static/icon.png` & `timeseriesflattener-1.5.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/_static/icon_dark.png` & `timeseriesflattener-1.5.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/_static/terminology_figure.png` & `timeseriesflattener-1.5.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/conf.py` & `timeseriesflattener-1.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/faq.rst` & `timeseriesflattener-1.5.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/index.rst` & `timeseriesflattener-1.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-1.5.0/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-1.5.0/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/tutorials/03_text.ipynb` & `timeseriesflattener-1.5.0/docs/tutorials/03_text.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.952931853491483%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(6, '1. How to generate flattened predictors from already "*

 * *            "embedded text.\\n'), (7, '2. How to featurize text using Huggingface or sci-kit learn "*

 * *            "models.\\n'), (8, '3. How to use write your own text embedding function in "*

 * *            "`timeseriesflattener`.\\n')], delete: [7, 6]}}, 2: {'execution_count': 1}, 15: "*

 * *            "{'outputs': {2: {'output_type': 'stream', 'name': 'stderr', 'text': "*

 * *            "['100%|██████████| 768/768 [00:23 […]*

```diff
@@ -7,16 +7,17 @@
             "source": [
                 "# Adding text features\n",
                 "\n",
                 "So far, the tutorials have dealt with _tabular_ data only. This tutorial will show you to make predictors out of text features, such as clinical notes, within `timeseriesflattener`.\n",
                 "\n",
                 "Specifically, this tutorial will cover:\n",
                 "\n",
-                "1. How to featurize text using Huggingface or sci-kit learn models.\n",
-                "2. How to use write your own text embedding function in `timeseriesflattener`.\n",
+                "1. How to generate flattened predictors from already embedded text.\n",
+                "2. How to featurize text using Huggingface or sci-kit learn models.\n",
+                "3. How to use write your own text embedding function in `timeseriesflattener`.\n",
                 "\n",
                 "To use the features in this tutorial you'll need to install some extra dependencies. These can be installed by running:\n",
                 "```\n",
                 "pip install pytorch transformers sentence-transformer\n",
                 "```\n",
                 "or by installing `timeseriesflattener` with the text dependencies.\n",
                 "```\n",
@@ -32,24 +33,24 @@
                 "## The dataset\n",
                 "\n",
                 "To start out, let's load a synthetic dataset containing text. As with all other features, each row in the dataset needs an ID, a timestamp, and the feature value. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from timeseriesflattener.testing.load_synth_data import load_synth_text\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -67,98 +68,901 @@
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>entity_id</th>\n",
                             "      <th>timestamp</th>\n",
-                            "      <th>text</th>\n",
                             "      <th>value</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>4647</td>\n",
                             "      <td>1967-07-19 00:22:00</td>\n",
                             "      <td>The patient went into a medically induced coma...</td>\n",
-                            "      <td>The patient went into a medically induced coma...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>2007</td>\n",
                             "      <td>1966-11-25 02:02:00</td>\n",
                             "      <td>The patient is taken to the emergency departme...</td>\n",
-                            "      <td>The patient is taken to the emergency departme...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>5799</td>\n",
                             "      <td>1967-09-19 12:31:00</td>\n",
                             "      <td>The patient, described as a 7-month old son wh...</td>\n",
-                            "      <td>The patient, described as a 7-month old son wh...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>1319</td>\n",
                             "      <td>1969-07-21 23:16:00</td>\n",
                             "      <td>The patient had been left on a bed for 20 minu...</td>\n",
-                            "      <td>The patient had been left on a bed for 20 minu...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>4234</td>\n",
                             "      <td>1966-04-14 22:04:00</td>\n",
                             "      <td>The patient had had some severe allergies but ...</td>\n",
-                            "      <td>The patient had had some severe allergies but ...</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "   entity_id           timestamp  \\\n",
                             "0       4647 1967-07-19 00:22:00   \n",
                             "1       2007 1966-11-25 02:02:00   \n",
                             "2       5799 1967-09-19 12:31:00   \n",
                             "3       1319 1969-07-21 23:16:00   \n",
                             "4       4234 1966-04-14 22:04:00   \n",
                             "\n",
-                            "                                                text  \\\n",
-                            "0  The patient went into a medically induced coma...   \n",
-                            "1  The patient is taken to the emergency departme...   \n",
-                            "2  The patient, described as a 7-month old son wh...   \n",
-                            "3  The patient had been left on a bed for 20 minu...   \n",
-                            "4  The patient had had some severe allergies but ...   \n",
-                            "\n",
                             "                                               value  \n",
                             "0  The patient went into a medically induced coma...  \n",
                             "1  The patient is taken to the emergency departme...  \n",
                             "2  The patient, described as a 7-month old son wh...  \n",
                             "3  The patient had been left on a bed for 20 minu...  \n",
                             "4  The patient had had some severe allergies but ...  "
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 2,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "synth_text = load_synth_text()\n",
+                "synth_text.head()\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Generating predictors from embedded text\n",
+                "\n",
+                "As generating text embeddings can often take a while, it can be an advantageous to embed the text before using `timeseriesflattener` to speed up the computation if you're generating multiple datasets. This first block will show how to convert a dataframe with embeddings into a format that can be passed to `timeseriesflattener`. Skip to [TextPredictorSpec](#textpredictorspec) if you want to perform the embedding step directly in `timeseriesflattener`.\n",
+                "\n",
+                "To start, let's embed the synthetic text data using a sentence-transformer. You can use any form of text-embedding you want - the only constraint is that the result of the embedding function should be a dataframe with an `entitiy_id_col`, `timestamp_col` and any number of `value_cols`. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%%capture\n",
+                "from sentence_transformers import SentenceTransformer\n",
+                "import pandas as pd\n",
+                "\n",
+                "# load fast model\n",
+                "model = SentenceTransformer(\"all-MiniLM-L6-v2\")\n",
+                "\n",
+                "# define function to embed text and return a dataframe\n",
+                "def embed_text_to_df(model: SentenceTransformer, text: list[str]) -> pd.DataFrame:\n",
+                "    embeddings = model.encode(text, batch_size=256)\n",
+                "    return pd.DataFrame(embeddings)\n",
+                "\n",
+                "# embed text\n",
+                "embedded_text = embed_text_to_df(model=model, text=synth_text[\"value\"].tolist())\n",
+                "# drop the text column from the original dataframe\n",
+                "metadata_only = synth_text.drop(columns=[\"value\"])\n",
+                "# concatenate the metadata and the embedded text\n",
+                "embedded_text_with_metadata = pd.concat([metadata_only, embedded_text], axis=1)\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>entity_id</th>\n",
+                            "      <th>timestamp</th>\n",
+                            "      <th>0</th>\n",
+                            "      <th>1</th>\n",
+                            "      <th>2</th>\n",
+                            "      <th>3</th>\n",
+                            "      <th>4</th>\n",
+                            "      <th>5</th>\n",
+                            "      <th>6</th>\n",
+                            "      <th>7</th>\n",
+                            "      <th>...</th>\n",
+                            "      <th>374</th>\n",
+                            "      <th>375</th>\n",
+                            "      <th>376</th>\n",
+                            "      <th>377</th>\n",
+                            "      <th>378</th>\n",
+                            "      <th>379</th>\n",
+                            "      <th>380</th>\n",
+                            "      <th>381</th>\n",
+                            "      <th>382</th>\n",
+                            "      <th>383</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>4647</td>\n",
+                            "      <td>1967-07-19 00:22:00</td>\n",
+                            "      <td>-0.020159</td>\n",
+                            "      <td>0.006134</td>\n",
+                            "      <td>-0.006455</td>\n",
+                            "      <td>0.005938</td>\n",
+                            "      <td>0.038562</td>\n",
+                            "      <td>0.005949</td>\n",
+                            "      <td>-0.056681</td>\n",
+                            "      <td>0.029464</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>0.021432</td>\n",
+                            "      <td>0.061494</td>\n",
+                            "      <td>0.011665</td>\n",
+                            "      <td>0.018157</td>\n",
+                            "      <td>-0.035946</td>\n",
+                            "      <td>0.101041</td>\n",
+                            "      <td>-0.002912</td>\n",
+                            "      <td>0.014489</td>\n",
+                            "      <td>-0.033684</td>\n",
+                            "      <td>-0.085988</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>2007</td>\n",
+                            "      <td>1966-11-25 02:02:00</td>\n",
+                            "      <td>-0.065502</td>\n",
+                            "      <td>0.026975</td>\n",
+                            "      <td>-0.042235</td>\n",
+                            "      <td>-0.012499</td>\n",
+                            "      <td>-0.012820</td>\n",
+                            "      <td>-0.003107</td>\n",
+                            "      <td>0.025823</td>\n",
+                            "      <td>0.115787</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.013681</td>\n",
+                            "      <td>-0.008509</td>\n",
+                            "      <td>-0.005801</td>\n",
+                            "      <td>-0.019228</td>\n",
+                            "      <td>-0.029137</td>\n",
+                            "      <td>0.107618</td>\n",
+                            "      <td>0.027575</td>\n",
+                            "      <td>0.061189</td>\n",
+                            "      <td>-0.036197</td>\n",
+                            "      <td>-0.023715</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>5799</td>\n",
+                            "      <td>1967-09-19 12:31:00</td>\n",
+                            "      <td>-0.015965</td>\n",
+                            "      <td>0.030239</td>\n",
+                            "      <td>-0.025726</td>\n",
+                            "      <td>0.011575</td>\n",
+                            "      <td>-0.056353</td>\n",
+                            "      <td>0.024950</td>\n",
+                            "      <td>0.005075</td>\n",
+                            "      <td>0.158615</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>0.021345</td>\n",
+                            "      <td>0.019185</td>\n",
+                            "      <td>0.046376</td>\n",
+                            "      <td>0.008546</td>\n",
+                            "      <td>-0.017712</td>\n",
+                            "      <td>0.014252</td>\n",
+                            "      <td>-0.090198</td>\n",
+                            "      <td>0.036281</td>\n",
+                            "      <td>0.119648</td>\n",
+                            "      <td>-0.031743</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>1319</td>\n",
+                            "      <td>1969-07-21 23:16:00</td>\n",
+                            "      <td>0.049595</td>\n",
+                            "      <td>0.124481</td>\n",
+                            "      <td>-0.050134</td>\n",
+                            "      <td>0.036343</td>\n",
+                            "      <td>0.040793</td>\n",
+                            "      <td>0.067932</td>\n",
+                            "      <td>0.108808</td>\n",
+                            "      <td>0.068143</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>0.041999</td>\n",
+                            "      <td>-0.011297</td>\n",
+                            "      <td>0.013209</td>\n",
+                            "      <td>0.002157</td>\n",
+                            "      <td>-0.032716</td>\n",
+                            "      <td>-0.001036</td>\n",
+                            "      <td>-0.013383</td>\n",
+                            "      <td>-0.025948</td>\n",
+                            "      <td>-0.033742</td>\n",
+                            "      <td>-0.013560</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>4234</td>\n",
+                            "      <td>1966-04-14 22:04:00</td>\n",
+                            "      <td>-0.062923</td>\n",
+                            "      <td>0.062385</td>\n",
+                            "      <td>-0.048646</td>\n",
+                            "      <td>0.081368</td>\n",
+                            "      <td>0.115612</td>\n",
+                            "      <td>-0.036585</td>\n",
+                            "      <td>0.105179</td>\n",
+                            "      <td>0.034068</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>0.015677</td>\n",
+                            "      <td>-0.009112</td>\n",
+                            "      <td>-0.032549</td>\n",
+                            "      <td>0.021608</td>\n",
+                            "      <td>-0.043334</td>\n",
+                            "      <td>0.057872</td>\n",
+                            "      <td>-0.044645</td>\n",
+                            "      <td>0.024808</td>\n",
+                            "      <td>0.002562</td>\n",
+                            "      <td>0.030407</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "<p>5 rows \u00d7 386 columns</p>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "   entity_id           timestamp         0         1         2         3  \\\n",
+                            "0       4647 1967-07-19 00:22:00 -0.020159  0.006134 -0.006455  0.005938   \n",
+                            "1       2007 1966-11-25 02:02:00 -0.065502  0.026975 -0.042235 -0.012499   \n",
+                            "2       5799 1967-09-19 12:31:00 -0.015965  0.030239 -0.025726  0.011575   \n",
+                            "3       1319 1969-07-21 23:16:00  0.049595  0.124481 -0.050134  0.036343   \n",
+                            "4       4234 1966-04-14 22:04:00 -0.062923  0.062385 -0.048646  0.081368   \n",
+                            "\n",
+                            "          4         5         6         7  ...       374       375       376  \\\n",
+                            "0  0.038562  0.005949 -0.056681  0.029464  ...  0.021432  0.061494  0.011665   \n",
+                            "1 -0.012820 -0.003107  0.025823  0.115787  ... -0.013681 -0.008509 -0.005801   \n",
+                            "2 -0.056353  0.024950  0.005075  0.158615  ...  0.021345  0.019185  0.046376   \n",
+                            "3  0.040793  0.067932  0.108808  0.068143  ...  0.041999 -0.011297  0.013209   \n",
+                            "4  0.115612 -0.036585  0.105179  0.034068  ...  0.015677 -0.009112 -0.032549   \n",
+                            "\n",
+                            "        377       378       379       380       381       382       383  \n",
+                            "0  0.018157 -0.035946  0.101041 -0.002912  0.014489 -0.033684 -0.085988  \n",
+                            "1 -0.019228 -0.029137  0.107618  0.027575  0.061189 -0.036197 -0.023715  \n",
+                            "2  0.008546 -0.017712  0.014252 -0.090198  0.036281  0.119648 -0.031743  \n",
+                            "3  0.002157 -0.032716 -0.001036 -0.013383 -0.025948 -0.033742 -0.013560  \n",
+                            "4  0.021608 -0.043334  0.057872 -0.044645  0.024808  0.002562  0.030407  \n",
+                            "\n",
+                            "[5 rows x 386 columns]"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "embedded_text_with_metadata.head()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Now that we have our embeddings, we can use the `df_with_multiple_values_to_named_dataframes` function to turn the embeddings into a format that can be readily supplied to `PredictorGroupSpec`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>entity_id</th>\n",
+                            "      <th>timestamp</th>\n",
+                            "      <th>value</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>4647</td>\n",
+                            "      <td>1967-07-19 00:22:00</td>\n",
+                            "      <td>-0.020159</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>2007</td>\n",
+                            "      <td>1966-11-25 02:02:00</td>\n",
+                            "      <td>-0.065502</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>5799</td>\n",
+                            "      <td>1967-09-19 12:31:00</td>\n",
+                            "      <td>-0.015965</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>1319</td>\n",
+                            "      <td>1969-07-21 23:16:00</td>\n",
+                            "      <td>0.049595</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>4234</td>\n",
+                            "      <td>1966-04-14 22:04:00</td>\n",
+                            "      <td>-0.062923</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "   entity_id           timestamp     value\n",
+                            "0       4647 1967-07-19 00:22:00 -0.020159\n",
+                            "1       2007 1966-11-25 02:02:00 -0.065502\n",
+                            "2       5799 1967-09-19 12:31:00 -0.015965\n",
+                            "3       1319 1969-07-21 23:16:00  0.049595\n",
+                            "4       4234 1966-04-14 22:04:00 -0.062923"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from timeseriesflattener.df_transforms import (\n",
+                "    df_with_multiple_values_to_named_dataframes,\n",
+                ")\n",
+                "\n",
+                "# split the dataframe into a list of named dataframes with one value each\n",
+                "embedded_dfs = df_with_multiple_values_to_named_dataframes(\n",
+                "    df=embedded_text_with_metadata,\n",
+                "    entity_id_col_name=\"entity_id\",\n",
+                "    timestamp_col_name=\"timestamp\",\n",
+                "    name_prefix=\"sent_emb_\",\n",
+                ")\n",
+                "\n",
+                "# check the first dataframe\n",
+                "embedded_dfs[0].df.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "384"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# check the number of embeddings/dataframes\n",
+                "len(embedded_dfs)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Each dataframe has been named according to `name_prefix` and the column name. This means, that if your column names are informative (e.g. if they correspond to specific words in a BOW model) they will be kept. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'sent_emb_0'"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "embedded_dfs[0].name"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Let's make some features! "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "768\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from timeseriesflattener.aggregation_fns import mean\n",
+                "from timeseriesflattener.feature_specs.group_specs import PredictorGroupSpec\n",
+                "import numpy as np\n",
+                "\n",
+                "# create a group spec for the embedded text that will take the mean of each embedding on the column axis\n",
+                "# for the last 365 and 730 days\n",
+                "emb_spec_batch = PredictorGroupSpec(\n",
+                "    named_dataframes=embedded_dfs,\n",
+                "    lookbehind_days=[365, 730],\n",
+                "    fallback=[np.nan],\n",
+                "    aggregation_fns=[mean],\n",
+                ").create_combinations()\n",
+                "\n",
+                "# print the number of features we will create\n",
+                "print(len(emb_spec_batch))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We are creating 384*2=768 features: 1 for each embedding for each lookbehind (365 and 730 days)."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "2023-07-21 14:58:09 [INFO] There were unprocessed specs, computing...\n",
+                        "2023-07-21 14:58:09 [INFO] Processing 768 temporal features in parallel with 1 workers. Chunksize is 768. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "huggingface/tokenizers: The current process just got forked, after parallelism has already been used. Disabling parallelism to avoid deadlocks...\n",
+                        "To disable this warning, you can either:\n",
+                        "\t- Avoid using `tokenizers` before the fork if possible\n",
+                        "\t- Explicitly set the environment variable TOKENIZERS_PARALLELISM=(true | false)\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 768/768 [00:23<00:00, 33.28it/s]\n",
+                        "2023-07-21 14:58:32 [INFO] Checking alignment of dataframes - this might take a little while (~2 minutes for 1.000 dataframes with 2.000.000 rows).\n",
+                        "2023-07-21 14:58:33 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features and 2_000_000 prediction times. This is normal.\n",
+                        "2023-07-21 14:58:34 [INFO] Concatenation took 1.269 seconds\n",
+                        "2023-07-21 14:58:34 [INFO] Merging with original df\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# make features how you would normally\n",
+                "from timeseriesflattener import TimeseriesFlattener\n",
+                "from timeseriesflattener.testing.load_synth_data import load_synth_prediction_times\n",
+                "\n",
+                "ts_flattener = TimeseriesFlattener(\n",
+                "    prediction_times_df=load_synth_prediction_times(),\n",
+                "    entity_id_col_name=\"entity_id\",\n",
+                "    timestamp_col_name=\"timestamp\",\n",
+                "    n_workers=1,\n",
+                "    drop_pred_times_with_insufficient_look_distance=False,\n",
+                ")\n",
+                "ts_flattener.add_spec(emb_spec_batch)\n",
+                "df = ts_flattener.get_df()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Let's check the output."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>entity_id</th>\n",
+                            "      <th>timestamp</th>\n",
+                            "      <th>prediction_time_uuid</th>\n",
+                            "      <th>pred_sent_emb_4_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_91_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_106_within_730_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_376_within_730_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_333_within_730_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_51_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_316_within_730_days_mean_fallback_nan</th>\n",
+                            "      <th>...</th>\n",
+                            "      <th>pred_sent_emb_217_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_288_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_67_within_730_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_120_within_730_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_221_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_26_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_137_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_11_within_365_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_205_within_730_days_mean_fallback_nan</th>\n",
+                            "      <th>pred_sent_emb_357_within_730_days_mean_fallback_nan</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>1917</th>\n",
+                            "      <td>4977</td>\n",
+                            "      <td>1968-11-28 16:05:00</td>\n",
+                            "      <td>4977-1968-11-28-16-05-00</td>\n",
+                            "      <td>0.001232</td>\n",
+                            "      <td>-0.000302</td>\n",
+                            "      <td>0.040634</td>\n",
+                            "      <td>-0.002166</td>\n",
+                            "      <td>0.039541</td>\n",
+                            "      <td>0.107663</td>\n",
+                            "      <td>0.012334</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.036499</td>\n",
+                            "      <td>0.073914</td>\n",
+                            "      <td>-0.078592</td>\n",
+                            "      <td>0.052193</td>\n",
+                            "      <td>0.013373</td>\n",
+                            "      <td>-0.069261</td>\n",
+                            "      <td>-0.088767</td>\n",
+                            "      <td>0.004150</td>\n",
+                            "      <td>-0.081158</td>\n",
+                            "      <td>-0.007002</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2463</th>\n",
+                            "      <td>6840</td>\n",
+                            "      <td>1965-11-02 07:17:00</td>\n",
+                            "      <td>6840-1965-11-02-07-17-00</td>\n",
+                            "      <td>0.015495</td>\n",
+                            "      <td>0.010209</td>\n",
+                            "      <td>-0.006142</td>\n",
+                            "      <td>0.047095</td>\n",
+                            "      <td>0.062537</td>\n",
+                            "      <td>-0.047844</td>\n",
+                            "      <td>-0.117715</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>0.031768</td>\n",
+                            "      <td>-0.075292</td>\n",
+                            "      <td>-0.061927</td>\n",
+                            "      <td>-0.028022</td>\n",
+                            "      <td>0.046316</td>\n",
+                            "      <td>-0.026953</td>\n",
+                            "      <td>-0.095338</td>\n",
+                            "      <td>0.002313</td>\n",
+                            "      <td>0.056995</td>\n",
+                            "      <td>0.015441</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2580</th>\n",
+                            "      <td>18</td>\n",
+                            "      <td>1968-08-26 15:19:00</td>\n",
+                            "      <td>18-1968-08-26-15-19-00</td>\n",
+                            "      <td>-0.025853</td>\n",
+                            "      <td>0.049886</td>\n",
+                            "      <td>-0.060344</td>\n",
+                            "      <td>0.054533</td>\n",
+                            "      <td>0.013257</td>\n",
+                            "      <td>-0.022677</td>\n",
+                            "      <td>-0.021626</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.013668</td>\n",
+                            "      <td>-0.024832</td>\n",
+                            "      <td>-0.086064</td>\n",
+                            "      <td>0.004718</td>\n",
+                            "      <td>0.020128</td>\n",
+                            "      <td>0.004320</td>\n",
+                            "      <td>-0.078148</td>\n",
+                            "      <td>0.016352</td>\n",
+                            "      <td>-0.011881</td>\n",
+                            "      <td>-0.061026</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2741</th>\n",
+                            "      <td>9832</td>\n",
+                            "      <td>1969-06-03 04:36:00</td>\n",
+                            "      <td>9832-1969-06-03-04-36-00</td>\n",
+                            "      <td>-0.047658</td>\n",
+                            "      <td>0.103156</td>\n",
+                            "      <td>0.049586</td>\n",
+                            "      <td>0.012266</td>\n",
+                            "      <td>-0.051270</td>\n",
+                            "      <td>-0.056747</td>\n",
+                            "      <td>-0.047248</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.015452</td>\n",
+                            "      <td>0.011051</td>\n",
+                            "      <td>-0.108515</td>\n",
+                            "      <td>-0.033745</td>\n",
+                            "      <td>-0.037524</td>\n",
+                            "      <td>0.009744</td>\n",
+                            "      <td>-0.045512</td>\n",
+                            "      <td>0.091745</td>\n",
+                            "      <td>0.012856</td>\n",
+                            "      <td>-0.013721</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2931</th>\n",
+                            "      <td>7281</td>\n",
+                            "      <td>1967-06-05 00:41:00</td>\n",
+                            "      <td>7281-1967-06-05-00-41-00</td>\n",
+                            "      <td>-0.027302</td>\n",
+                            "      <td>-0.031607</td>\n",
+                            "      <td>0.009704</td>\n",
+                            "      <td>0.059126</td>\n",
+                            "      <td>-0.036862</td>\n",
+                            "      <td>-0.098369</td>\n",
+                            "      <td>-0.026895</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.038409</td>\n",
+                            "      <td>0.015281</td>\n",
+                            "      <td>-0.071394</td>\n",
+                            "      <td>0.010426</td>\n",
+                            "      <td>-0.055521</td>\n",
+                            "      <td>0.071217</td>\n",
+                            "      <td>-0.029075</td>\n",
+                            "      <td>-0.037698</td>\n",
+                            "      <td>-0.063065</td>\n",
+                            "      <td>0.068621</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "<p>5 rows \u00d7 771 columns</p>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "      entity_id           timestamp      prediction_time_uuid  \\\n",
+                            "1917       4977 1968-11-28 16:05:00  4977-1968-11-28-16-05-00   \n",
+                            "2463       6840 1965-11-02 07:17:00  6840-1965-11-02-07-17-00   \n",
+                            "2580         18 1968-08-26 15:19:00    18-1968-08-26-15-19-00   \n",
+                            "2741       9832 1969-06-03 04:36:00  9832-1969-06-03-04-36-00   \n",
+                            "2931       7281 1967-06-05 00:41:00  7281-1967-06-05-00-41-00   \n",
+                            "\n",
+                            "      pred_sent_emb_4_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                           0.001232   \n",
+                            "2463                                           0.015495   \n",
+                            "2580                                          -0.025853   \n",
+                            "2741                                          -0.047658   \n",
+                            "2931                                          -0.027302   \n",
+                            "\n",
+                            "      pred_sent_emb_91_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                          -0.000302    \n",
+                            "2463                                           0.010209    \n",
+                            "2580                                           0.049886    \n",
+                            "2741                                           0.103156    \n",
+                            "2931                                          -0.031607    \n",
+                            "\n",
+                            "      pred_sent_emb_106_within_730_days_mean_fallback_nan  \\\n",
+                            "1917                                           0.040634     \n",
+                            "2463                                          -0.006142     \n",
+                            "2580                                          -0.060344     \n",
+                            "2741                                           0.049586     \n",
+                            "2931                                           0.009704     \n",
+                            "\n",
+                            "      pred_sent_emb_376_within_730_days_mean_fallback_nan  \\\n",
+                            "1917                                          -0.002166     \n",
+                            "2463                                           0.047095     \n",
+                            "2580                                           0.054533     \n",
+                            "2741                                           0.012266     \n",
+                            "2931                                           0.059126     \n",
+                            "\n",
+                            "      pred_sent_emb_333_within_730_days_mean_fallback_nan  \\\n",
+                            "1917                                           0.039541     \n",
+                            "2463                                           0.062537     \n",
+                            "2580                                           0.013257     \n",
+                            "2741                                          -0.051270     \n",
+                            "2931                                          -0.036862     \n",
+                            "\n",
+                            "      pred_sent_emb_51_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                           0.107663    \n",
+                            "2463                                          -0.047844    \n",
+                            "2580                                          -0.022677    \n",
+                            "2741                                          -0.056747    \n",
+                            "2931                                          -0.098369    \n",
+                            "\n",
+                            "      pred_sent_emb_316_within_730_days_mean_fallback_nan  ...  \\\n",
+                            "1917                                           0.012334    ...   \n",
+                            "2463                                          -0.117715    ...   \n",
+                            "2580                                          -0.021626    ...   \n",
+                            "2741                                          -0.047248    ...   \n",
+                            "2931                                          -0.026895    ...   \n",
+                            "\n",
+                            "      pred_sent_emb_217_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                          -0.036499     \n",
+                            "2463                                           0.031768     \n",
+                            "2580                                          -0.013668     \n",
+                            "2741                                          -0.015452     \n",
+                            "2931                                          -0.038409     \n",
+                            "\n",
+                            "      pred_sent_emb_288_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                           0.073914     \n",
+                            "2463                                          -0.075292     \n",
+                            "2580                                          -0.024832     \n",
+                            "2741                                           0.011051     \n",
+                            "2931                                           0.015281     \n",
+                            "\n",
+                            "      pred_sent_emb_67_within_730_days_mean_fallback_nan  \\\n",
+                            "1917                                          -0.078592    \n",
+                            "2463                                          -0.061927    \n",
+                            "2580                                          -0.086064    \n",
+                            "2741                                          -0.108515    \n",
+                            "2931                                          -0.071394    \n",
+                            "\n",
+                            "      pred_sent_emb_120_within_730_days_mean_fallback_nan  \\\n",
+                            "1917                                           0.052193     \n",
+                            "2463                                          -0.028022     \n",
+                            "2580                                           0.004718     \n",
+                            "2741                                          -0.033745     \n",
+                            "2931                                           0.010426     \n",
+                            "\n",
+                            "      pred_sent_emb_221_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                           0.013373     \n",
+                            "2463                                           0.046316     \n",
+                            "2580                                           0.020128     \n",
+                            "2741                                          -0.037524     \n",
+                            "2931                                          -0.055521     \n",
+                            "\n",
+                            "      pred_sent_emb_26_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                          -0.069261    \n",
+                            "2463                                          -0.026953    \n",
+                            "2580                                           0.004320    \n",
+                            "2741                                           0.009744    \n",
+                            "2931                                           0.071217    \n",
+                            "\n",
+                            "      pred_sent_emb_137_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                          -0.088767     \n",
+                            "2463                                          -0.095338     \n",
+                            "2580                                          -0.078148     \n",
+                            "2741                                          -0.045512     \n",
+                            "2931                                          -0.029075     \n",
+                            "\n",
+                            "      pred_sent_emb_11_within_365_days_mean_fallback_nan  \\\n",
+                            "1917                                           0.004150    \n",
+                            "2463                                           0.002313    \n",
+                            "2580                                           0.016352    \n",
+                            "2741                                           0.091745    \n",
+                            "2931                                          -0.037698    \n",
+                            "\n",
+                            "      pred_sent_emb_205_within_730_days_mean_fallback_nan  \\\n",
+                            "1917                                          -0.081158     \n",
+                            "2463                                           0.056995     \n",
+                            "2580                                          -0.011881     \n",
+                            "2741                                           0.012856     \n",
+                            "2931                                          -0.063065     \n",
+                            "\n",
+                            "      pred_sent_emb_357_within_730_days_mean_fallback_nan  \n",
+                            "1917                                          -0.007002    \n",
+                            "2463                                           0.015441    \n",
+                            "2580                                          -0.061026    \n",
+                            "2741                                          -0.013721    \n",
+                            "2931                                           0.068621    \n",
+                            "\n",
+                            "[5 rows x 771 columns]"
+                        ]
+                    },
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "load_synth_text().head()\n"
+                "# dropping na values (no embeddings within the lookbehind period) for the sake of this example\n",
+                "df.dropna().head()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## TextPredictorSpec\n",
-                "\n",
-                "The main difference when specifying text predictors compared to tabular predictors is the `Spec` you define. For text, we need to specify a `TextPredictorSpec` which is entirely similar to the `PredictorSpec` except for two additional attributes: `embedding_fn` and `embedding_fn_kwargs`.\n",
+                "The main difference when specifying text predictors compared to tabular predictors is the `Spec` you define. When working directly with text, we need to specify a `TextPredictorSpec` which is entirely similar to the `PredictorSpec` except for two additional attributes: `embedding_fn` and `embedding_fn_kwargs`.\n",
                 "\n",
                 "`embedding_fn` should be a callable that takes a pandas Series containing text and converts it to a pandas DataFrame with a column for each feature. `embedding_fn_kwargs` are simply optional keyword arguments that will be passed to the embedding function, such as a Huggingface model name.\n",
                 "\n",
                 "Not all `resolve_multiple_fn` are meaningful for text, as we can't do numerical operations on text. Instead, `TextPredictorSpec` defaults to the \"concatenate\" option, which simply concatenates all texts within the lookbehind within. Other options that work for text are \"latest\" and \"earliest\". \n"
             ]
         },
         {
@@ -172,66 +976,56 @@
                 "The `sentence_transformers_embedding` function is recommended for sentence-transformers. If you want to another type of model from the Huggingface Hub we recommend using the `huggingface_embedding` function which has the same interface as `sentence_transformers_embedding`.\n",
                 "\n",
                 "Notice, both `huggingface_embedding` and `sentence_transformers_embedding` will truncate the input to the maximum sequence length allowed by the model. If you want to use Huggingface embeddings for larger blocks of text, either use the `sklearn_embedding` function or write your own embedding function (see below)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from timeseriesflattener.text_embedding_functions import (\n",
                 "    sentence_transformers_embedding,\n",
                 "    huggingface_embedding,\n",
                 ")\n",
                 "from timeseriesflattener import TextPredictorSpec\n",
                 "from timeseriesflattener.aggregation_fns import concatenate\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "text_spec = TextPredictorSpec(\n",
                 "    timeseries_df=load_synth_text(),\n",
                 "    lookbehind_days=730,\n",
                 "    fallback=np.nan,\n",
                 "    aggregation_fn=concatenate,\n",
                 "    feature_base_name=\"text-st\",\n",
                 "    embedding_fn=sentence_transformers_embedding,\n",
                 "    embedding_fn_kwargs={\n",
-                "        \"model_name\": \"sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2\"\n",
+                "        \"model_name\": \"sentence-transformers/all-MiniLM-L6-v2\"\n",
                 "    },\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "That's it. Let's make our features in the usual way."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from timeseriesflattener import TimeseriesFlattener\n",
-                "from timeseriesflattener.testing.load_synth_data import load_synth_prediction_times\n"
-            ]
-        },
-        {
-            "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ts_flattener = TimeseriesFlattener(\n",
                 "    prediction_times_df=load_synth_prediction_times(),\n",
                 "    entity_id_col_name=\"entity_id\",\n",
@@ -247,21 +1041,37 @@
             "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2023-06-14 16:20:20 [INFO] There were unprocessed specs, computing...\n",
-                        "2023-06-14 16:20:20 [INFO] Processing 1 temporal features in parallel with 1 workers. Chunksize is 1. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n",
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:05<00:00,  5.27s/it]\n",
-                        "2023-06-14 16:20:25 [INFO] Checking alignment of dataframes - this might take a little while (~2 minutes for 1.000 dataframes with 2.000.000 rows).\n",
-                        "2023-06-14 16:20:25 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features and 2_000_000 prediction times. This is normal.\n",
-                        "2023-06-14 16:20:25 [INFO] Concatenation took 0.006 seconds\n",
-                        "2023-06-14 16:20:25 [INFO] Merging with original df\n"
+                        "2023-07-21 14:58:34 [INFO] There were unprocessed specs, computing...\n",
+                        "2023-07-21 14:58:34 [INFO] Processing 1 temporal features in parallel with 1 workers. Chunksize is 1. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "huggingface/tokenizers: The current process just got forked, after parallelism has already been used. Disabling parallelism to avoid deadlocks...\n",
+                        "To disable this warning, you can either:\n",
+                        "\t- Avoid using `tokenizers` before the fork if possible\n",
+                        "\t- Explicitly set the environment variable TOKENIZERS_PARALLELISM=(true | false)\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:05<00:00,  5.12s/it]\n",
+                        "2023-07-21 14:58:39 [INFO] Checking alignment of dataframes - this might take a little while (~2 minutes for 1.000 dataframes with 2.000.000 rows).\n",
+                        "2023-07-21 14:58:39 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features and 2_000_000 prediction times. This is normal.\n",
+                        "2023-07-21 14:58:40 [INFO] Concatenation took 0.024 seconds\n",
+                        "2023-07-21 14:58:40 [INFO] Merging with original df\n"
                     ]
                 }
             ],
             "source": [
                 "df = ts_flattener.get_df()\n"
             ]
         },
@@ -646,128 +1456,128 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>244</th>\n",
                             "      <td>7337</td>\n",
                             "      <td>1966-06-28 10:34:00</td>\n",
                             "      <td>7337-1966-06-28-10-34-00</td>\n",
-                            "      <td>-0.020497</td>\n",
-                            "      <td>0.201255</td>\n",
-                            "      <td>-0.187649</td>\n",
-                            "      <td>-0.240372</td>\n",
-                            "      <td>0.105265</td>\n",
-                            "      <td>0.004314</td>\n",
-                            "      <td>-0.151738</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>0.121190</td>\n",
-                            "      <td>0.381909</td>\n",
-                            "      <td>0.144211</td>\n",
-                            "      <td>-0.038955</td>\n",
-                            "      <td>-0.000124</td>\n",
-                            "      <td>0.156520</td>\n",
-                            "      <td>-0.196082</td>\n",
-                            "      <td>0.080771</td>\n",
-                            "      <td>0.025773</td>\n",
-                            "      <td>0.193602</td>\n",
+                            "      <td>-0.032579</td>\n",
+                            "      <td>0.117177</td>\n",
+                            "      <td>-0.049458</td>\n",
+                            "      <td>0.009333</td>\n",
+                            "      <td>0.013606</td>\n",
+                            "      <td>0.021374</td>\n",
+                            "      <td>0.001354</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.017522</td>\n",
+                            "      <td>0.099060</td>\n",
+                            "      <td>0.049743</td>\n",
+                            "      <td>0.015571</td>\n",
+                            "      <td>-0.019073</td>\n",
+                            "      <td>0.109147</td>\n",
+                            "      <td>0.047269</td>\n",
+                            "      <td>-0.043760</td>\n",
+                            "      <td>0.020477</td>\n",
+                            "      <td>-0.007479</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>755</th>\n",
                             "      <td>8951</td>\n",
                             "      <td>1969-12-22 16:32:00</td>\n",
                             "      <td>8951-1969-12-22-16-32-00</td>\n",
-                            "      <td>0.069950</td>\n",
-                            "      <td>0.099192</td>\n",
-                            "      <td>-0.007804</td>\n",
-                            "      <td>0.033173</td>\n",
-                            "      <td>-0.044742</td>\n",
-                            "      <td>0.193883</td>\n",
-                            "      <td>-0.165403</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>-0.236144</td>\n",
-                            "      <td>0.051994</td>\n",
-                            "      <td>-0.029250</td>\n",
-                            "      <td>-0.080070</td>\n",
-                            "      <td>-0.105516</td>\n",
-                            "      <td>0.141162</td>\n",
-                            "      <td>0.008052</td>\n",
-                            "      <td>-0.315303</td>\n",
-                            "      <td>0.049577</td>\n",
-                            "      <td>-0.070045</td>\n",
+                            "      <td>-0.011282</td>\n",
+                            "      <td>0.002961</td>\n",
+                            "      <td>0.025957</td>\n",
+                            "      <td>-0.015063</td>\n",
+                            "      <td>-0.050311</td>\n",
+                            "      <td>0.048773</td>\n",
+                            "      <td>-0.002749</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.067139</td>\n",
+                            "      <td>0.049532</td>\n",
+                            "      <td>-0.030149</td>\n",
+                            "      <td>-0.009194</td>\n",
+                            "      <td>-0.051574</td>\n",
+                            "      <td>0.013600</td>\n",
+                            "      <td>-0.100028</td>\n",
+                            "      <td>-0.116557</td>\n",
+                            "      <td>0.033871</td>\n",
+                            "      <td>0.008424</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>896</th>\n",
                             "      <td>2007</td>\n",
                             "      <td>1968-10-15 14:12:00</td>\n",
                             "      <td>2007-1968-10-15-14-12-00</td>\n",
-                            "      <td>0.048036</td>\n",
-                            "      <td>-0.050683</td>\n",
-                            "      <td>0.039954</td>\n",
-                            "      <td>0.038270</td>\n",
-                            "      <td>-0.208975</td>\n",
-                            "      <td>-0.262620</td>\n",
-                            "      <td>0.084824</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>-0.064676</td>\n",
-                            "      <td>0.065383</td>\n",
-                            "      <td>-0.030430</td>\n",
-                            "      <td>-0.047385</td>\n",
-                            "      <td>-0.037471</td>\n",
-                            "      <td>0.031160</td>\n",
-                            "      <td>-0.191298</td>\n",
-                            "      <td>0.291992</td>\n",
-                            "      <td>-0.154983</td>\n",
-                            "      <td>-0.043705</td>\n",
+                            "      <td>-0.065502</td>\n",
+                            "      <td>0.026975</td>\n",
+                            "      <td>-0.042235</td>\n",
+                            "      <td>-0.012499</td>\n",
+                            "      <td>-0.012820</td>\n",
+                            "      <td>-0.003107</td>\n",
+                            "      <td>0.025823</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.013681</td>\n",
+                            "      <td>-0.008509</td>\n",
+                            "      <td>-0.005801</td>\n",
+                            "      <td>-0.019228</td>\n",
+                            "      <td>-0.029137</td>\n",
+                            "      <td>0.107618</td>\n",
+                            "      <td>0.027575</td>\n",
+                            "      <td>0.061189</td>\n",
+                            "      <td>-0.036197</td>\n",
+                            "      <td>-0.023715</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1517</th>\n",
                             "      <td>1728</td>\n",
                             "      <td>1968-05-29 12:27:00</td>\n",
                             "      <td>1728-1968-05-29-12-27-00</td>\n",
-                            "      <td>0.042505</td>\n",
-                            "      <td>-0.009908</td>\n",
-                            "      <td>-0.091326</td>\n",
-                            "      <td>-0.005621</td>\n",
-                            "      <td>-0.085136</td>\n",
-                            "      <td>0.168317</td>\n",
-                            "      <td>0.037416</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>0.027059</td>\n",
-                            "      <td>0.319632</td>\n",
-                            "      <td>-0.044289</td>\n",
-                            "      <td>-0.042798</td>\n",
-                            "      <td>-0.136277</td>\n",
-                            "      <td>-0.118022</td>\n",
-                            "      <td>0.169292</td>\n",
-                            "      <td>-0.029509</td>\n",
-                            "      <td>0.262050</td>\n",
-                            "      <td>0.103499</td>\n",
+                            "      <td>0.003414</td>\n",
+                            "      <td>-0.022889</td>\n",
+                            "      <td>0.003017</td>\n",
+                            "      <td>0.036401</td>\n",
+                            "      <td>0.021559</td>\n",
+                            "      <td>-0.004627</td>\n",
+                            "      <td>0.070992</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.010578</td>\n",
+                            "      <td>0.028139</td>\n",
+                            "      <td>-0.013348</td>\n",
+                            "      <td>-0.062894</td>\n",
+                            "      <td>-0.059819</td>\n",
+                            "      <td>-0.064517</td>\n",
+                            "      <td>0.013139</td>\n",
+                            "      <td>-0.030818</td>\n",
+                            "      <td>0.088636</td>\n",
+                            "      <td>0.012063</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1917</th>\n",
                             "      <td>4977</td>\n",
                             "      <td>1968-11-28 16:05:00</td>\n",
                             "      <td>4977-1968-11-28-16-05-00</td>\n",
-                            "      <td>0.135539</td>\n",
-                            "      <td>0.035848</td>\n",
-                            "      <td>0.089571</td>\n",
-                            "      <td>0.098358</td>\n",
-                            "      <td>-0.066512</td>\n",
-                            "      <td>-0.051096</td>\n",
-                            "      <td>0.027142</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>-0.039122</td>\n",
-                            "      <td>0.246103</td>\n",
-                            "      <td>0.102282</td>\n",
-                            "      <td>0.031486</td>\n",
-                            "      <td>-0.336561</td>\n",
-                            "      <td>-0.110646</td>\n",
-                            "      <td>0.089151</td>\n",
-                            "      <td>0.233425</td>\n",
-                            "      <td>-0.021751</td>\n",
-                            "      <td>-0.023900</td>\n",
+                            "      <td>0.029870</td>\n",
+                            "      <td>0.059029</td>\n",
+                            "      <td>0.025774</td>\n",
+                            "      <td>0.065304</td>\n",
+                            "      <td>0.001232</td>\n",
+                            "      <td>0.097216</td>\n",
+                            "      <td>0.005217</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>-0.078040</td>\n",
+                            "      <td>0.121744</td>\n",
+                            "      <td>-0.002166</td>\n",
+                            "      <td>0.040929</td>\n",
+                            "      <td>-0.075126</td>\n",
+                            "      <td>-0.069748</td>\n",
+                            "      <td>0.009481</td>\n",
+                            "      <td>0.039800</td>\n",
+                            "      <td>0.010281</td>\n",
+                            "      <td>0.028113</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>5 rows \u00d7 387 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
@@ -775,131 +1585,131 @@
                             "244        7337 1966-06-28 10:34:00  7337-1966-06-28-10-34-00   \n",
                             "755        8951 1969-12-22 16:32:00  8951-1969-12-22-16-32-00   \n",
                             "896        2007 1968-10-15 14:12:00  2007-1968-10-15-14-12-00   \n",
                             "1517       1728 1968-05-29 12:27:00  1728-1968-05-29-12-27-00   \n",
                             "1917       4977 1968-11-28 16:05:00  4977-1968-11-28-16-05-00   \n",
                             "\n",
                             "      pred_text-st-0_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.020497         \n",
-                            "755                                            0.069950         \n",
-                            "896                                            0.048036         \n",
-                            "1517                                           0.042505         \n",
-                            "1917                                           0.135539         \n",
+                            "244                                           -0.032579         \n",
+                            "755                                           -0.011282         \n",
+                            "896                                           -0.065502         \n",
+                            "1517                                           0.003414         \n",
+                            "1917                                           0.029870         \n",
                             "\n",
                             "      pred_text-st-1_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.201255         \n",
-                            "755                                            0.099192         \n",
-                            "896                                           -0.050683         \n",
-                            "1517                                          -0.009908         \n",
-                            "1917                                           0.035848         \n",
+                            "244                                            0.117177         \n",
+                            "755                                            0.002961         \n",
+                            "896                                            0.026975         \n",
+                            "1517                                          -0.022889         \n",
+                            "1917                                           0.059029         \n",
                             "\n",
                             "      pred_text-st-2_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.187649         \n",
-                            "755                                           -0.007804         \n",
-                            "896                                            0.039954         \n",
-                            "1517                                          -0.091326         \n",
-                            "1917                                           0.089571         \n",
+                            "244                                           -0.049458         \n",
+                            "755                                            0.025957         \n",
+                            "896                                           -0.042235         \n",
+                            "1517                                           0.003017         \n",
+                            "1917                                           0.025774         \n",
                             "\n",
                             "      pred_text-st-3_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.240372         \n",
-                            "755                                            0.033173         \n",
-                            "896                                            0.038270         \n",
-                            "1517                                          -0.005621         \n",
-                            "1917                                           0.098358         \n",
+                            "244                                            0.009333         \n",
+                            "755                                           -0.015063         \n",
+                            "896                                           -0.012499         \n",
+                            "1517                                           0.036401         \n",
+                            "1917                                           0.065304         \n",
                             "\n",
                             "      pred_text-st-4_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.105265         \n",
-                            "755                                           -0.044742         \n",
-                            "896                                           -0.208975         \n",
-                            "1517                                          -0.085136         \n",
-                            "1917                                          -0.066512         \n",
+                            "244                                            0.013606         \n",
+                            "755                                           -0.050311         \n",
+                            "896                                           -0.012820         \n",
+                            "1517                                           0.021559         \n",
+                            "1917                                           0.001232         \n",
                             "\n",
                             "      pred_text-st-5_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.004314         \n",
-                            "755                                            0.193883         \n",
-                            "896                                           -0.262620         \n",
-                            "1517                                           0.168317         \n",
-                            "1917                                          -0.051096         \n",
+                            "244                                            0.021374         \n",
+                            "755                                            0.048773         \n",
+                            "896                                           -0.003107         \n",
+                            "1517                                          -0.004627         \n",
+                            "1917                                           0.097216         \n",
                             "\n",
                             "      pred_text-st-6_within_730_days_concatenate_fallback_nan  ...  \\\n",
-                            "244                                           -0.151738        ...   \n",
-                            "755                                           -0.165403        ...   \n",
-                            "896                                            0.084824        ...   \n",
-                            "1517                                           0.037416        ...   \n",
-                            "1917                                           0.027142        ...   \n",
+                            "244                                            0.001354        ...   \n",
+                            "755                                           -0.002749        ...   \n",
+                            "896                                            0.025823        ...   \n",
+                            "1517                                           0.070992        ...   \n",
+                            "1917                                           0.005217        ...   \n",
                             "\n",
                             "      pred_text-st-374_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.121190           \n",
-                            "755                                           -0.236144           \n",
-                            "896                                           -0.064676           \n",
-                            "1517                                           0.027059           \n",
-                            "1917                                          -0.039122           \n",
+                            "244                                           -0.017522           \n",
+                            "755                                           -0.067139           \n",
+                            "896                                           -0.013681           \n",
+                            "1517                                          -0.010578           \n",
+                            "1917                                          -0.078040           \n",
                             "\n",
                             "      pred_text-st-375_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.381909           \n",
-                            "755                                            0.051994           \n",
-                            "896                                            0.065383           \n",
-                            "1517                                           0.319632           \n",
-                            "1917                                           0.246103           \n",
+                            "244                                            0.099060           \n",
+                            "755                                            0.049532           \n",
+                            "896                                           -0.008509           \n",
+                            "1517                                           0.028139           \n",
+                            "1917                                           0.121744           \n",
                             "\n",
                             "      pred_text-st-376_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.144211           \n",
-                            "755                                           -0.029250           \n",
-                            "896                                           -0.030430           \n",
-                            "1517                                          -0.044289           \n",
-                            "1917                                           0.102282           \n",
+                            "244                                            0.049743           \n",
+                            "755                                           -0.030149           \n",
+                            "896                                           -0.005801           \n",
+                            "1517                                          -0.013348           \n",
+                            "1917                                          -0.002166           \n",
                             "\n",
                             "      pred_text-st-377_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.038955           \n",
-                            "755                                           -0.080070           \n",
-                            "896                                           -0.047385           \n",
-                            "1517                                          -0.042798           \n",
-                            "1917                                           0.031486           \n",
+                            "244                                            0.015571           \n",
+                            "755                                           -0.009194           \n",
+                            "896                                           -0.019228           \n",
+                            "1517                                          -0.062894           \n",
+                            "1917                                           0.040929           \n",
                             "\n",
                             "      pred_text-st-378_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.000124           \n",
-                            "755                                           -0.105516           \n",
-                            "896                                           -0.037471           \n",
-                            "1517                                          -0.136277           \n",
-                            "1917                                          -0.336561           \n",
+                            "244                                           -0.019073           \n",
+                            "755                                           -0.051574           \n",
+                            "896                                           -0.029137           \n",
+                            "1517                                          -0.059819           \n",
+                            "1917                                          -0.075126           \n",
                             "\n",
                             "      pred_text-st-379_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.156520           \n",
-                            "755                                            0.141162           \n",
-                            "896                                            0.031160           \n",
-                            "1517                                          -0.118022           \n",
-                            "1917                                          -0.110646           \n",
+                            "244                                            0.109147           \n",
+                            "755                                            0.013600           \n",
+                            "896                                            0.107618           \n",
+                            "1517                                          -0.064517           \n",
+                            "1917                                          -0.069748           \n",
                             "\n",
                             "      pred_text-st-380_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.196082           \n",
-                            "755                                            0.008052           \n",
-                            "896                                           -0.191298           \n",
-                            "1517                                           0.169292           \n",
-                            "1917                                           0.089151           \n",
+                            "244                                            0.047269           \n",
+                            "755                                           -0.100028           \n",
+                            "896                                            0.027575           \n",
+                            "1517                                           0.013139           \n",
+                            "1917                                           0.009481           \n",
                             "\n",
                             "      pred_text-st-381_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.080771           \n",
-                            "755                                           -0.315303           \n",
-                            "896                                            0.291992           \n",
-                            "1517                                          -0.029509           \n",
-                            "1917                                           0.233425           \n",
+                            "244                                           -0.043760           \n",
+                            "755                                           -0.116557           \n",
+                            "896                                            0.061189           \n",
+                            "1517                                          -0.030818           \n",
+                            "1917                                           0.039800           \n",
                             "\n",
                             "      pred_text-st-382_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.025773           \n",
-                            "755                                            0.049577           \n",
-                            "896                                           -0.154983           \n",
-                            "1517                                           0.262050           \n",
-                            "1917                                          -0.021751           \n",
+                            "244                                            0.020477           \n",
+                            "755                                            0.033871           \n",
+                            "896                                           -0.036197           \n",
+                            "1517                                           0.088636           \n",
+                            "1917                                           0.010281           \n",
                             "\n",
                             "      pred_text-st-383_within_730_days_concatenate_fallback_nan  \n",
-                            "244                                            0.193602          \n",
-                            "755                                           -0.070045          \n",
-                            "896                                           -0.043705          \n",
-                            "1517                                           0.103499          \n",
-                            "1917                                          -0.023900          \n",
+                            "244                                           -0.007479          \n",
+                            "755                                            0.008424          \n",
+                            "896                                           -0.023715          \n",
+                            "1517                                           0.012063          \n",
+                            "1917                                           0.028113          \n",
                             "\n",
                             "[5 rows x 387 columns]"
                         ]
                     },
                     "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -931,15 +1741,15 @@
             "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/Users/au484925/Desktop/Git/timeseriesflattener/.venv39/lib/python3.9/site-packages/sklearn/base.py:318: UserWarning: Trying to unpickle estimator CountVectorizer from version 1.1.2 when using version 1.2.2. This might lead to breaking code or invalid results. Use at your own risk. For more info please refer to:\n",
+                        "/Users/au554730/Desktop/Projects/timeseriesflattener/.venv/lib/python3.10/site-packages/sklearn/base.py:299: UserWarning: Trying to unpickle estimator CountVectorizer from version 1.1.2 when using version 1.2.1. This might lead to breaking code or invalid results. Use at your own risk. For more info please refer to:\n",
                         "https://scikit-learn.org/stable/model_persistence.html#security-maintainability-limitations\n",
                         "  warnings.warn(\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
@@ -960,15 +1770,15 @@
                 "\n",
                 "tfidf_model = _load_bow_model()\n",
                 "tfidf_model\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [],
             "source": [
                 "count_vectorizer_text_spec = TextPredictorSpec(\n",
                 "    timeseries_df=load_synth_text(),\n",
                 "    lookbehind_days=730,\n",
                 "    fallback=np.nan,\n",
@@ -985,30 +1795,44 @@
             "metadata": {},
             "source": [
                 "Let's add the feature to the dataset:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2023-02-07 11:08:48 [INFO] There were unprocessed specs, computing...\n",
-                        "2023-02-07 11:08:48 [INFO] Processing 1 temporal features in parallel with 1 workers. Chunksize is 1. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n",
-                        "  0%|          | 0/1 [00:00<?, ?it/s]/Users/au554730/Desktop/Projects/timeseriesflattener/.venv/lib/python3.10/site-packages/sklearn/utils/deprecation.py:87: FutureWarning: Function get_feature_names is deprecated; get_feature_names is deprecated in 1.0 and will be removed in 1.2. Please use get_feature_names_out instead.\n",
-                        "  warnings.warn(msg, category=FutureWarning)\n",
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:03<00:00,  3.15s/it]\n",
-                        "2023-02-07 11:08:51 [INFO] Checking alignment of dataframes - this might take a little while (~2 minutes for 1.000 dataframes with 2.000.000 rows).\n",
-                        "2023-02-07 11:08:51 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features and 2_000_000 prediction times. This is normal.\n",
-                        "2023-02-07 11:08:51 [INFO] Concatenation took 0.004 seconds\n",
-                        "2023-02-07 11:08:51 [INFO] Merging with original df\n"
+                        "2023-07-21 14:58:40 [INFO] There were unprocessed specs, computing...\n",
+                        "2023-07-21 14:58:40 [INFO] Processing 1 temporal features in parallel with 1 workers. Chunksize is 1. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "huggingface/tokenizers: The current process just got forked, after parallelism has already been used. Disabling parallelism to avoid deadlocks...\n",
+                        "To disable this warning, you can either:\n",
+                        "\t- Avoid using `tokenizers` before the fork if possible\n",
+                        "\t- Explicitly set the environment variable TOKENIZERS_PARALLELISM=(true | false)\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:02<00:00,  2.89s/it]\n",
+                        "2023-07-21 14:58:43 [INFO] Checking alignment of dataframes - this might take a little while (~2 minutes for 1.000 dataframes with 2.000.000 rows).\n",
+                        "2023-07-21 14:58:43 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features and 2_000_000 prediction times. This is normal.\n",
+                        "2023-07-21 14:58:43 [INFO] Concatenation took 0.005 seconds\n",
+                        "2023-07-21 14:58:43 [INFO] Merging with original df\n"
                     ]
                 }
             ],
             "source": [
                 "ts_flattener.add_spec(count_vectorizer_text_spec)\n",
                 "df = ts_flattener.get_df()\n"
             ]
@@ -1019,15 +1843,15 @@
             "metadata": {},
             "source": [
                 "Let's subset to only see the prediction times that include text again."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1054,283 +1878,283 @@
                             "      <th>pred_text-st-1_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-2_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-3_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-4_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-5_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-6_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>...</th>\n",
-                            "      <th>pred_text-st-374_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-375_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-376_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-377_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-378_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-379_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-380_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-381_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-382_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-st-383_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-and_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-for_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-in_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-of_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-or_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-patient_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-that_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-the_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-to_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-was_within_730_days_concatenate_fallback_nan</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>244</th>\n",
                             "      <td>7337</td>\n",
                             "      <td>1966-06-28 10:34:00</td>\n",
                             "      <td>7337-1966-06-28-10-34-00</td>\n",
-                            "      <td>-0.020497</td>\n",
-                            "      <td>0.201255</td>\n",
-                            "      <td>-0.187649</td>\n",
-                            "      <td>-0.240372</td>\n",
-                            "      <td>0.105265</td>\n",
-                            "      <td>0.004314</td>\n",
-                            "      <td>-0.151738</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>0.121190</td>\n",
-                            "      <td>0.381909</td>\n",
-                            "      <td>0.144211</td>\n",
-                            "      <td>-0.038955</td>\n",
-                            "      <td>-0.000124</td>\n",
-                            "      <td>0.156520</td>\n",
-                            "      <td>-0.196082</td>\n",
-                            "      <td>0.080771</td>\n",
-                            "      <td>0.025773</td>\n",
-                            "      <td>0.193602</td>\n",
+                            "      <td>-0.032579</td>\n",
+                            "      <td>0.117177</td>\n",
+                            "      <td>-0.049458</td>\n",
+                            "      <td>0.009333</td>\n",
+                            "      <td>0.013606</td>\n",
+                            "      <td>0.021374</td>\n",
+                            "      <td>0.001354</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>16.0</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>755</th>\n",
                             "      <td>8951</td>\n",
                             "      <td>1969-12-22 16:32:00</td>\n",
                             "      <td>8951-1969-12-22-16-32-00</td>\n",
-                            "      <td>0.069950</td>\n",
-                            "      <td>0.099192</td>\n",
-                            "      <td>-0.007804</td>\n",
-                            "      <td>0.033173</td>\n",
-                            "      <td>-0.044742</td>\n",
-                            "      <td>0.193883</td>\n",
-                            "      <td>-0.165403</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>-0.236144</td>\n",
-                            "      <td>0.051994</td>\n",
-                            "      <td>-0.029250</td>\n",
-                            "      <td>-0.080070</td>\n",
-                            "      <td>-0.105516</td>\n",
-                            "      <td>0.141162</td>\n",
-                            "      <td>0.008052</td>\n",
-                            "      <td>-0.315303</td>\n",
-                            "      <td>0.049577</td>\n",
-                            "      <td>-0.070045</td>\n",
+                            "      <td>-0.011282</td>\n",
+                            "      <td>0.002961</td>\n",
+                            "      <td>0.025957</td>\n",
+                            "      <td>-0.015063</td>\n",
+                            "      <td>-0.050311</td>\n",
+                            "      <td>0.048773</td>\n",
+                            "      <td>-0.002749</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>8.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>896</th>\n",
                             "      <td>2007</td>\n",
                             "      <td>1968-10-15 14:12:00</td>\n",
                             "      <td>2007-1968-10-15-14-12-00</td>\n",
-                            "      <td>0.048036</td>\n",
-                            "      <td>-0.050683</td>\n",
-                            "      <td>0.039954</td>\n",
-                            "      <td>0.038270</td>\n",
-                            "      <td>-0.208975</td>\n",
-                            "      <td>-0.262620</td>\n",
-                            "      <td>0.084824</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>-0.064676</td>\n",
-                            "      <td>0.065383</td>\n",
-                            "      <td>-0.030430</td>\n",
-                            "      <td>-0.047385</td>\n",
-                            "      <td>-0.037471</td>\n",
-                            "      <td>0.031160</td>\n",
-                            "      <td>-0.191298</td>\n",
-                            "      <td>0.291992</td>\n",
-                            "      <td>-0.154983</td>\n",
-                            "      <td>-0.043705</td>\n",
+                            "      <td>-0.065502</td>\n",
+                            "      <td>0.026975</td>\n",
+                            "      <td>-0.042235</td>\n",
+                            "      <td>-0.012499</td>\n",
+                            "      <td>-0.012820</td>\n",
+                            "      <td>-0.003107</td>\n",
+                            "      <td>0.025823</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>6.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>13.0</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1517</th>\n",
                             "      <td>1728</td>\n",
                             "      <td>1968-05-29 12:27:00</td>\n",
                             "      <td>1728-1968-05-29-12-27-00</td>\n",
-                            "      <td>0.042505</td>\n",
-                            "      <td>-0.009908</td>\n",
-                            "      <td>-0.091326</td>\n",
-                            "      <td>-0.005621</td>\n",
-                            "      <td>-0.085136</td>\n",
-                            "      <td>0.168317</td>\n",
-                            "      <td>0.037416</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>0.027059</td>\n",
-                            "      <td>0.319632</td>\n",
-                            "      <td>-0.044289</td>\n",
-                            "      <td>-0.042798</td>\n",
-                            "      <td>-0.136277</td>\n",
-                            "      <td>-0.118022</td>\n",
-                            "      <td>0.169292</td>\n",
-                            "      <td>-0.029509</td>\n",
-                            "      <td>0.262050</td>\n",
-                            "      <td>0.103499</td>\n",
+                            "      <td>0.003414</td>\n",
+                            "      <td>-0.022889</td>\n",
+                            "      <td>0.003017</td>\n",
+                            "      <td>0.036401</td>\n",
+                            "      <td>0.021559</td>\n",
+                            "      <td>-0.004627</td>\n",
+                            "      <td>0.070992</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>8.0</td>\n",
+                            "      <td>11.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>11.0</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1917</th>\n",
                             "      <td>4977</td>\n",
                             "      <td>1968-11-28 16:05:00</td>\n",
                             "      <td>4977-1968-11-28-16-05-00</td>\n",
-                            "      <td>0.135539</td>\n",
-                            "      <td>0.035848</td>\n",
-                            "      <td>0.089571</td>\n",
-                            "      <td>0.098358</td>\n",
-                            "      <td>-0.066512</td>\n",
-                            "      <td>-0.051096</td>\n",
-                            "      <td>0.027142</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>-0.039122</td>\n",
-                            "      <td>0.246103</td>\n",
-                            "      <td>0.102282</td>\n",
-                            "      <td>0.031486</td>\n",
-                            "      <td>-0.336561</td>\n",
-                            "      <td>-0.110646</td>\n",
-                            "      <td>0.089151</td>\n",
-                            "      <td>0.233425</td>\n",
-                            "      <td>-0.021751</td>\n",
-                            "      <td>-0.023900</td>\n",
+                            "      <td>0.029870</td>\n",
+                            "      <td>0.059029</td>\n",
+                            "      <td>0.025774</td>\n",
+                            "      <td>0.065304</td>\n",
+                            "      <td>0.001232</td>\n",
+                            "      <td>0.097216</td>\n",
+                            "      <td>0.005217</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>6.0</td>\n",
+                            "      <td>7.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>8.0</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>5 rows \u00d7 387 columns</p>\n",
+                            "<p>5 rows \u00d7 397 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "      entity_id           timestamp      prediction_time_uuid  \\\n",
                             "244        7337 1966-06-28 10:34:00  7337-1966-06-28-10-34-00   \n",
                             "755        8951 1969-12-22 16:32:00  8951-1969-12-22-16-32-00   \n",
                             "896        2007 1968-10-15 14:12:00  2007-1968-10-15-14-12-00   \n",
                             "1517       1728 1968-05-29 12:27:00  1728-1968-05-29-12-27-00   \n",
                             "1917       4977 1968-11-28 16:05:00  4977-1968-11-28-16-05-00   \n",
                             "\n",
                             "      pred_text-st-0_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.020497         \n",
-                            "755                                            0.069950         \n",
-                            "896                                            0.048036         \n",
-                            "1517                                           0.042505         \n",
-                            "1917                                           0.135539         \n",
+                            "244                                           -0.032579         \n",
+                            "755                                           -0.011282         \n",
+                            "896                                           -0.065502         \n",
+                            "1517                                           0.003414         \n",
+                            "1917                                           0.029870         \n",
                             "\n",
                             "      pred_text-st-1_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.201255         \n",
-                            "755                                            0.099192         \n",
-                            "896                                           -0.050683         \n",
-                            "1517                                          -0.009908         \n",
-                            "1917                                           0.035848         \n",
+                            "244                                            0.117177         \n",
+                            "755                                            0.002961         \n",
+                            "896                                            0.026975         \n",
+                            "1517                                          -0.022889         \n",
+                            "1917                                           0.059029         \n",
                             "\n",
                             "      pred_text-st-2_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.187649         \n",
-                            "755                                           -0.007804         \n",
-                            "896                                            0.039954         \n",
-                            "1517                                          -0.091326         \n",
-                            "1917                                           0.089571         \n",
+                            "244                                           -0.049458         \n",
+                            "755                                            0.025957         \n",
+                            "896                                           -0.042235         \n",
+                            "1517                                           0.003017         \n",
+                            "1917                                           0.025774         \n",
                             "\n",
                             "      pred_text-st-3_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.240372         \n",
-                            "755                                            0.033173         \n",
-                            "896                                            0.038270         \n",
-                            "1517                                          -0.005621         \n",
-                            "1917                                           0.098358         \n",
+                            "244                                            0.009333         \n",
+                            "755                                           -0.015063         \n",
+                            "896                                           -0.012499         \n",
+                            "1517                                           0.036401         \n",
+                            "1917                                           0.065304         \n",
                             "\n",
                             "      pred_text-st-4_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.105265         \n",
-                            "755                                           -0.044742         \n",
-                            "896                                           -0.208975         \n",
-                            "1517                                          -0.085136         \n",
-                            "1917                                          -0.066512         \n",
+                            "244                                            0.013606         \n",
+                            "755                                           -0.050311         \n",
+                            "896                                           -0.012820         \n",
+                            "1517                                           0.021559         \n",
+                            "1917                                           0.001232         \n",
                             "\n",
                             "      pred_text-st-5_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.004314         \n",
-                            "755                                            0.193883         \n",
-                            "896                                           -0.262620         \n",
-                            "1517                                           0.168317         \n",
-                            "1917                                          -0.051096         \n",
+                            "244                                            0.021374         \n",
+                            "755                                            0.048773         \n",
+                            "896                                           -0.003107         \n",
+                            "1517                                          -0.004627         \n",
+                            "1917                                           0.097216         \n",
                             "\n",
                             "      pred_text-st-6_within_730_days_concatenate_fallback_nan  ...  \\\n",
-                            "244                                           -0.151738        ...   \n",
-                            "755                                           -0.165403        ...   \n",
-                            "896                                            0.084824        ...   \n",
-                            "1517                                           0.037416        ...   \n",
-                            "1917                                           0.027142        ...   \n",
-                            "\n",
-                            "      pred_text-st-374_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.121190           \n",
-                            "755                                           -0.236144           \n",
-                            "896                                           -0.064676           \n",
-                            "1517                                           0.027059           \n",
-                            "1917                                          -0.039122           \n",
+                            "244                                            0.001354        ...   \n",
+                            "755                                           -0.002749        ...   \n",
+                            "896                                            0.025823        ...   \n",
+                            "1517                                           0.070992        ...   \n",
+                            "1917                                           0.005217        ...   \n",
+                            "\n",
+                            "      pred_text-cv-and_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 4.0           \n",
+                            "755                                                 1.0           \n",
+                            "896                                                 4.0           \n",
+                            "1517                                                1.0           \n",
+                            "1917                                                2.0           \n",
+                            "\n",
+                            "      pred_text-cv-for_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 2.0           \n",
+                            "755                                                 5.0           \n",
+                            "896                                                 0.0           \n",
+                            "1517                                                1.0           \n",
+                            "1917                                                1.0           \n",
+                            "\n",
+                            "      pred_text-cv-in_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 2.0          \n",
+                            "755                                                 1.0          \n",
+                            "896                                                 2.0          \n",
+                            "1517                                                8.0          \n",
+                            "1917                                                6.0          \n",
+                            "\n",
+                            "      pred_text-cv-of_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 5.0          \n",
+                            "755                                                 1.0          \n",
+                            "896                                                 1.0          \n",
+                            "1517                                               11.0          \n",
+                            "1917                                                7.0          \n",
+                            "\n",
+                            "      pred_text-cv-or_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 0.0          \n",
+                            "755                                                 1.0          \n",
+                            "896                                                 5.0          \n",
+                            "1517                                                0.0          \n",
+                            "1917                                                2.0          \n",
+                            "\n",
+                            "      pred_text-cv-patient_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 3.0               \n",
+                            "755                                                 2.0               \n",
+                            "896                                                 6.0               \n",
+                            "1517                                                2.0               \n",
+                            "1917                                                2.0               \n",
+                            "\n",
+                            "      pred_text-cv-that_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 1.0            \n",
+                            "755                                                 2.0            \n",
+                            "896                                                 2.0            \n",
+                            "1517                                                1.0            \n",
+                            "1917                                                1.0            \n",
+                            "\n",
+                            "      pred_text-cv-the_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                16.0           \n",
+                            "755                                                 8.0           \n",
+                            "896                                                13.0           \n",
+                            "1517                                               11.0           \n",
+                            "1917                                                8.0           \n",
+                            "\n",
+                            "      pred_text-cv-to_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 4.0          \n",
+                            "755                                                 2.0          \n",
+                            "896                                                 3.0          \n",
+                            "1517                                                5.0          \n",
+                            "1917                                                4.0          \n",
+                            "\n",
+                            "      pred_text-cv-was_within_730_days_concatenate_fallback_nan  \n",
+                            "244                                                 2.0          \n",
+                            "755                                                 0.0          \n",
+                            "896                                                 0.0          \n",
+                            "1517                                                2.0          \n",
+                            "1917                                                1.0          \n",
                             "\n",
-                            "      pred_text-st-375_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.381909           \n",
-                            "755                                            0.051994           \n",
-                            "896                                            0.065383           \n",
-                            "1517                                           0.319632           \n",
-                            "1917                                           0.246103           \n",
-                            "\n",
-                            "      pred_text-st-376_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.144211           \n",
-                            "755                                           -0.029250           \n",
-                            "896                                           -0.030430           \n",
-                            "1517                                          -0.044289           \n",
-                            "1917                                           0.102282           \n",
-                            "\n",
-                            "      pred_text-st-377_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.038955           \n",
-                            "755                                           -0.080070           \n",
-                            "896                                           -0.047385           \n",
-                            "1517                                          -0.042798           \n",
-                            "1917                                           0.031486           \n",
-                            "\n",
-                            "      pred_text-st-378_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.000124           \n",
-                            "755                                           -0.105516           \n",
-                            "896                                           -0.037471           \n",
-                            "1517                                          -0.136277           \n",
-                            "1917                                          -0.336561           \n",
-                            "\n",
-                            "      pred_text-st-379_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.156520           \n",
-                            "755                                            0.141162           \n",
-                            "896                                            0.031160           \n",
-                            "1517                                          -0.118022           \n",
-                            "1917                                          -0.110646           \n",
-                            "\n",
-                            "      pred_text-st-380_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.196082           \n",
-                            "755                                            0.008052           \n",
-                            "896                                           -0.191298           \n",
-                            "1517                                           0.169292           \n",
-                            "1917                                           0.089151           \n",
-                            "\n",
-                            "      pred_text-st-381_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.080771           \n",
-                            "755                                           -0.315303           \n",
-                            "896                                            0.291992           \n",
-                            "1517                                          -0.029509           \n",
-                            "1917                                           0.233425           \n",
-                            "\n",
-                            "      pred_text-st-382_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.025773           \n",
-                            "755                                            0.049577           \n",
-                            "896                                           -0.154983           \n",
-                            "1517                                           0.262050           \n",
-                            "1917                                          -0.021751           \n",
-                            "\n",
-                            "      pred_text-st-383_within_730_days_concatenate_fallback_nan  \n",
-                            "244                                            0.193602          \n",
-                            "755                                           -0.070045          \n",
-                            "896                                           -0.043705          \n",
-                            "1517                                           0.103499          \n",
-                            "1917                                          -0.023900          \n",
-                            "\n",
-                            "[5 rows x 387 columns]"
+                            "[5 rows x 397 columns]"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df_pred_times_with_text = df[\n",
                 "    ~df[\"pred_text-st-1_within_730_days_concatenate_fallback_nan\"].isna()\n",
@@ -1344,15 +2168,15 @@
             "metadata": {},
             "source": [
                 "We can subset further to only include the features we created with the count vectorizer by subsetting to only include columns starting with the feature name (\"text-cv\")."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1368,43 +2192,169 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
+                            "      <th>pred_text-cv-and_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-for_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-in_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-of_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-or_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-patient_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-that_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-the_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-to_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-cv-was_within_730_days_concatenate_fallback_nan</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>244</th>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>16.0</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>755</th>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>8.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>896</th>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>6.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>13.0</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1517</th>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>8.0</td>\n",
+                            "      <td>11.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>11.0</td>\n",
+                            "      <td>5.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1917</th>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>6.0</td>\n",
+                            "      <td>7.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>8.0</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "Empty DataFrame\n",
-                            "Columns: []\n",
-                            "Index: [244, 755, 896, 1517, 1917]"
+                            "      pred_text-cv-and_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 4.0           \n",
+                            "755                                                 1.0           \n",
+                            "896                                                 4.0           \n",
+                            "1517                                                1.0           \n",
+                            "1917                                                2.0           \n",
+                            "\n",
+                            "      pred_text-cv-for_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 2.0           \n",
+                            "755                                                 5.0           \n",
+                            "896                                                 0.0           \n",
+                            "1517                                                1.0           \n",
+                            "1917                                                1.0           \n",
+                            "\n",
+                            "      pred_text-cv-in_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 2.0          \n",
+                            "755                                                 1.0          \n",
+                            "896                                                 2.0          \n",
+                            "1517                                                8.0          \n",
+                            "1917                                                6.0          \n",
+                            "\n",
+                            "      pred_text-cv-of_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 5.0          \n",
+                            "755                                                 1.0          \n",
+                            "896                                                 1.0          \n",
+                            "1517                                               11.0          \n",
+                            "1917                                                7.0          \n",
+                            "\n",
+                            "      pred_text-cv-or_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 0.0          \n",
+                            "755                                                 1.0          \n",
+                            "896                                                 5.0          \n",
+                            "1517                                                0.0          \n",
+                            "1917                                                2.0          \n",
+                            "\n",
+                            "      pred_text-cv-patient_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 3.0               \n",
+                            "755                                                 2.0               \n",
+                            "896                                                 6.0               \n",
+                            "1517                                                2.0               \n",
+                            "1917                                                2.0               \n",
+                            "\n",
+                            "      pred_text-cv-that_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 1.0            \n",
+                            "755                                                 2.0            \n",
+                            "896                                                 2.0            \n",
+                            "1517                                                1.0            \n",
+                            "1917                                                1.0            \n",
+                            "\n",
+                            "      pred_text-cv-the_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                16.0           \n",
+                            "755                                                 8.0           \n",
+                            "896                                                13.0           \n",
+                            "1517                                               11.0           \n",
+                            "1917                                                8.0           \n",
+                            "\n",
+                            "      pred_text-cv-to_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                                 4.0          \n",
+                            "755                                                 2.0          \n",
+                            "896                                                 3.0          \n",
+                            "1517                                                5.0          \n",
+                            "1917                                                4.0          \n",
+                            "\n",
+                            "      pred_text-cv-was_within_730_days_concatenate_fallback_nan  \n",
+                            "244                                                 2.0          \n",
+                            "755                                                 0.0          \n",
+                            "896                                                 0.0          \n",
+                            "1517                                                2.0          \n",
+                            "1917                                                1.0          "
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df_cv_pred_times_with_text = df_pred_times_with_text.loc[\n",
                 "    :, df_pred_times_with_text.columns.str.startswith(\"pred_text-cv\")\n",
@@ -1423,31 +2373,31 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Writing your own text embedding function\n",
                 "\n",
-                "If you want to write your own embedding function, you simply need to write a function that takes a pd.Series of text as the first input and any number of optional keyword arguments. Let's write a small function to embed long texts using a Huggingface model. Note that this implementation will likely be quite slow."
+                "If you want to write your own embedding function, you simply need to write a function that takes a pd.Series of text as the first input and any number of optional keyword arguments. Let's write a small function to embed long texts using a Huggingface model. Note that this implementation will likely be quite slow. In most cases, the best thing to do would be to embed your data before passing to `timeseriesflattener` and following the procedure outlined in [Generating predictors from embedded text](#generating-predictors-from-embedded-text)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from transformers import AutoTokenizer, AutoModel\n",
                 "import pandas as pd\n",
                 "import torch\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def huggingface_long_text_embedding(\n",
                 "    text_series: pd.Series, model_name: str, chunk_length: int\n",
                 ") -> pd.DataFrame:\n",
                 "    \"\"\"\n",
@@ -1486,15 +2436,15 @@
             "metadata": {},
             "source": [
                 "The function can now be used as an embedding function in a `TextPredictorSpec` and used in the same manner as usual."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [],
             "source": [
                 "huggingface_long_text_spec = TextPredictorSpec(\n",
                 "    timeseries_df=load_synth_text(),\n",
                 "    lookbehind_days=730,\n",
                 "    fallback=np.nan,\n",
@@ -1521,15 +2471,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.17"
+            "version": "3.10.10"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "9e85d6a49b1f06126f30ca9ae16ded22dd7c17d2dbfabea9098dc6424f12e12a"
             }
         }
```

### Comparing `timeseriesflattener-1.4.0/docs/tutorials/img/term_a.png` & `timeseriesflattener-1.5.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/tutorials/img/term_b.png` & `timeseriesflattener-1.5.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/tutorials/img/term_c.png` & `timeseriesflattener-1.5.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/docs/tutorials/img/term_d.png` & `timeseriesflattener-1.5.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/icon.png` & `timeseriesflattener-1.5.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/paper/paper.bib` & `timeseriesflattener-1.5.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/paper/paper.md` & `timeseriesflattener-1.5.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/pyproject.toml` & `timeseriesflattener-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "1.4.0"
+version = "1.5.0"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
@@ -34,33 +34,33 @@
 file = "LICENSE"
 name = "MIT"
 [project.optional-dependencies]
 dev = [
   "cruft",
   "pyright==1.1.305",  
   "pre-commit==3.3.3",
-  "ruff==0.0.272", # important that these match the pre-commit hooks
-  "black[jupyter]==22.8.0", # important that these match the pre-commit hooks
+  "ruff==0.0.280", # important that these match the pre-commit hooks
+  "black[jupyter]==23.7.0", # important that these match the pre-commit hooks
   "pandas-stubs", # type stubs for pandas
   "invoke==2.1.1",
   "tox",
 ]
 test = [
   "pytest>=7.1.3,<7.3.0",
   "pytest-cov>=3.0.0,<3.1.0",
   "pytest-xdist>=3.0.0,<3.2.0",
   "pytest-sugar>=0.9.4,<0.10.0",
 ]
 docs = [
-    "sphinx>=5.3.0,<7.1.0",
-    "furo==2023.3.27",
+    "sphinx>=5.3.0,<7.2.0",
+    "furo==2023.7.26",
     "sphinx-copybutton>=0.5.1,<0.5.3",
     "sphinxext-opengraph>=0.7.3,<0.8.3",
     "myst-nb>=0.6.0,<1.17.0",
-    "sphinx_design>=0.3.0,<0.3.1",
+    "sphinx_design>=0.3.0,<0.5.1",
 ]
 tutorials = [
     "jupyter>=1.0.0,<1.1.0",
     "skimpy>=0.0.7,<0.1.0",
 ]
 text = [
     "transformers>=4.26.0",
```

### Comparing `timeseriesflattener-1.4.0/src/conftest.py` & `timeseriesflattener-1.5.0/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/aggregation_fns.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/group_specs.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/feature_specs/single_specs.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/logger.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/misc_utils.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,8 +115,9 @@
         n_rows: Number of rows to return. Defaults to None which returns entire coercion data view.
 
     Returns:
         pd.DataFrame
     """
     df = load_raw_test_csv("synth_text_data.csv", n_rows=n_rows)
     df["value"] = df["text"]
+    df = df.drop(columns=["text"])
     return df
```

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,34 +7,34 @@
     huggingface_embedding,
     sentence_transformers_embedding,
 )
 
 
 def test_embedding_fn(synth_text_data: pd.DataFrame):
     """Test that synth embedding function works as expected"""
-    df = synth_text_data.dropna(subset="text")
-    embedding_df = bow_test_embedding(df["text"])
+    df = synth_text_data.dropna(subset="value")
+    embedding_df = bow_test_embedding(df["value"])
     assert embedding_df.shape == (df.shape[0], 10)
 
 
 @pytest.mark.huggingface()
 def test_huggingface_embedding(synth_text_data: pd.DataFrame):
     """Test that the huggingface embedding function works as expected"""
-    df = synth_text_data.dropna(subset="text")
+    df = synth_text_data.dropna(subset="value")
     df = df.head(5)
     embedding_df = huggingface_embedding(
-        df["text"],
+        df["value"],
         model_name="sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
     )
     assert embedding_df.shape == (df.shape[0], 384)
 
 
 @pytest.mark.huggingface()
 def test_sentence_transformer_embedding(synth_text_data: pd.DataFrame):
     """Test that the sentence-transformer embedding function works as expected"""
-    df = synth_text_data.dropna(subset="text")
+    df = synth_text_data.dropna(subset="value")
     df = df.head(5)
     embedding_df = sentence_transformers_embedding(
-        df["text"],
+        df["value"],
         model_name="sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
     )
     assert embedding_df.shape == (df.shape[0], 384)
```

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,14 @@
 ):
     # Create an instance of the class that contains the `add_spec` method
     dataset = TimeseriesFlattener(
         prediction_times_df=synth_prediction_times,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
-    synth_text_data["value"] = synth_text_data["text"]
-
     # Create sample specs
     outcome_spec = OutcomeSpec(
         timeseries_df=synth_outcome,
         feature_base_name="outcome",
         lookahead_days=1,
         aggregation_fn=mean,
         fallback=0,
```

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener/utils/pydantic_basemodel.py` & `timeseriesflattener-1.5.0/src/timeseriesflattener/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.4.0
+Version: 1.5.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.4.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.5.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 docs/tutorials/img/term_d.png
 paper/paper.bib
 paper/paper.md
 src/conftest.py
 src/timeseriesflattener/__init__.py
 src/timeseriesflattener/aggregation_fns.py
 src/timeseriesflattener/column_handler.py
+src/timeseriesflattener/df_transforms.py
 src/timeseriesflattener/flattened_dataset.py
 src/timeseriesflattener/flattened_ds_validator.py
 src/timeseriesflattener/logger.py
 src/timeseriesflattener/misc_utils.py
 src/timeseriesflattener/text_embedding_functions.py
 src/timeseriesflattener.egg-info/PKG-INFO
 src/timeseriesflattener.egg-info/SOURCES.txt
@@ -93,14 +94,15 @@
 src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
 src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
 src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
 src/timeseriesflattener/tests/__init__.py
 src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
 src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
 src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
+src/timeseriesflattener/tests/test_timeseriesflattener/test_df_transforms.py
 src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
 src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
 src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
 src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
 src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
 src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
 src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
```

### Comparing `timeseriesflattener-1.4.0/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-1.5.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 frozendict>=2.3.4
 coloredlogs>14.0.0
 
 [dev]
 cruft
 pyright==1.1.305
 pre-commit==3.3.3
-ruff==0.0.272
-black[jupyter]==22.8.0
+ruff==0.0.280
+black[jupyter]==23.7.0
 pandas-stubs
 invoke==2.1.1
 tox
 
 [docs]
-sphinx<7.1.0,>=5.3.0
-furo==2023.3.27
+sphinx<7.2.0,>=5.3.0
+furo==2023.7.26
 sphinx-copybutton<0.5.3,>=0.5.1
 sphinxext-opengraph<0.8.3,>=0.7.3
 myst-nb<1.17.0,>=0.6.0
-sphinx_design<0.3.1,>=0.3.0
+sphinx_design<0.5.1,>=0.3.0
 
 [test]
 pytest<7.3.0,>=7.1.3
 pytest-cov<3.1.0,>=3.0.0
 pytest-xdist<3.2.0,>=3.0.0
 pytest-sugar<0.10.0,>=0.9.4
```

### Comparing `timeseriesflattener-1.4.0/tasks.py` & `timeseriesflattener-1.5.0/tasks.py`

 * *Files identical despite different names*

