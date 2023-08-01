# Comparing `tmp/prismstudio-1.1.7.tar.gz` & `tmp/prismstudio-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismstudio-1.1.7.tar", last modified: Mon Jul 31 15:18:35 2023, max compression
+gzip compressed data, was "prismstudio-1.1.8.tar", last modified: Tue Aug  1 00:50:32 2023, max compression
```

## Comparing `prismstudio-1.1.7.tar` & `prismstudio-1.1.8.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.091288 prismstudio-1.1.7/
--rw-r--r--   0 prism      (501) staff       (20)    23016 2023-07-19 13:45:53.000000 prismstudio-1.1.7/LICENSE.txt
--rw-r--r--   0 prism      (501) staff       (20)      440 2023-07-31 15:18:35.091109 prismstudio-1.1.7/PKG-INFO
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.078651 prismstudio-1.1.7/prism/
--rw-r--r--   0 prism      (501) staff       (20)     1290 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/__init__.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.079162 prismstudio-1.1.7/prism/_common/
--rw-r--r--   0 prism      (501) staff       (20)       35 2023-07-31 15:18:30.000000 prismstudio-1.1.7/prism/_common/.env
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_common/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     3472 2023-07-31 05:54:47.000000 prismstudio-1.1.7/prism/_common/config.py
--rw-r--r--   0 prism      (501) staff       (20)    11029 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_common/const.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.079569 prismstudio-1.1.7/prism/_core/
--rw-r--r--   0 prism      (501) staff       (20)      288 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/__init__.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.081374 prismstudio-1.1.7/prism/_core/_data/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_data/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)    17869 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_data/esg.py
--rw-r--r--   0 prism      (501) staff       (20)    41180 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_data/estimate.py
--rw-r--r--   0 prism      (501) staff       (20)     7950 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_data/event.py
--rw-r--r--   0 prism      (501) staff       (20)    70894 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_data/financial.py
--rw-r--r--   0 prism      (501) staff       (20)    12927 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_data/index.py
--rw-r--r--   0 prism      (501) staff       (20)   121051 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_data/industry.py
--rw-r--r--   0 prism      (501) staff       (20)    43804 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_data/market.py
--rw-r--r--   0 prism      (501) staff       (20)     6446 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_data/precalculated.py
--rw-r--r--   0 prism      (501) staff       (20)     3840 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_data/securitymaster.py
--rw-r--r--   0 prism      (501) staff       (20)    15625 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_fn.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.081716 prismstudio-1.1.7/prism/_core/_model/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_model/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     5246 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_model/tcmodel.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.083869 prismstudio-1.1.7/prism/_core/_req_builder/
--rw-r--r--   0 prism      (501) staff       (20)     1458 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     2074 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_req_builder/_auth.py
--rw-r--r--   0 prism      (501) staff       (20)    22677 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_req_builder/_dataquery.py
--rw-r--r--   0 prism      (501) staff       (20)     2058 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/_dbinfo.py
--rw-r--r--   0 prism      (501) staff       (20)     7633 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/_exportdata.py
--rw-r--r--   0 prism      (501) staff       (20)     3633 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/_gui.py
--rw-r--r--   0 prism      (501) staff       (20)    15003 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/_job.py
--rw-r--r--   0 prism      (501) staff       (20)     4828 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_core/_req_builder/_list.py
--rw-r--r--   0 prism      (501) staff       (20)    15321 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/_portfolio.py
--rw-r--r--   0 prism      (501) staff       (20)     4295 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/_securitymaster.py
--rw-r--r--   0 prism      (501) staff       (20)    25699 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/_task.py
--rw-r--r--   0 prism      (501) staff       (20)    10877 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/_taskquery.py
--rw-r--r--   0 prism      (501) staff       (20)    24533 2023-07-24 00:59:28.000000 prismstudio-1.1.7/prism/_core/_req_builder/_universe.py
--rw-r--r--   0 prism      (501) staff       (20)     8696 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/_req_builder/preference.py
--rw-r--r--   0 prism      (501) staff       (20)     9606 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_core/ols.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.084704 prismstudio-1.1.7/prism/_prismcomponent/
--rw-r--r--   0 prism      (501) staff       (20)      353 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_prismcomponent/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     7644 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_prismcomponent/abstract_prismcomponent.py
--rw-r--r--   0 prism      (501) staff       (20)    12663 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_prismcomponent/datacomponent.py
--rw-r--r--   0 prism      (501) staff       (20)   186982 2023-07-31 15:18:16.000000 prismstudio-1.1.7/prism/_prismcomponent/prismcomponent.py
--rw-r--r--   0 prism      (501) staff       (20)    21567 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_prismcomponent/taskcomponent.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.085800 prismstudio-1.1.7/prism/_utils/
--rw-r--r--   0 prism      (501) staff       (20)      480 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_utils/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     2248 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_utils/auth_utils.py
--rw-r--r--   0 prism      (501) staff       (20)     3629 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_utils/exceptions.py
--rw-r--r--   0 prism      (501) staff       (20)     2028 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_utils/loader.py
--rw-r--r--   0 prism      (501) staff       (20)     3706 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_utils/prismcomponent_utils.py
--rw-r--r--   0 prism      (501) staff       (20)     5532 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_utils/req_builder_utils.py
--rw-r--r--   0 prism      (501) staff       (20)    14289 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_utils/validate_utils.py
--rw-r--r--   0 prism      (501) staff       (20)     7232 2023-07-19 13:45:53.000000 prismstudio-1.1.7/prism/_utils/validate_utils_refactored.py
--rw-r--r--   0 prism      (501) staff       (20)     1438 2023-07-24 00:59:23.000000 prismstudio-1.1.7/prism/_utils/version.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.086376 prismstudio-1.1.7/prismstudio.egg-info/
--rw-r--r--   0 prism      (501) staff       (20)      440 2023-07-31 15:18:35.000000 prismstudio-1.1.7/prismstudio.egg-info/PKG-INFO
--rw-r--r--   0 prism      (501) staff       (20)     3138 2023-07-31 15:18:35.000000 prismstudio-1.1.7/prismstudio.egg-info/SOURCES.txt
--rw-r--r--   0 prism      (501) staff       (20)        1 2023-07-31 15:18:35.000000 prismstudio-1.1.7/prismstudio.egg-info/dependency_links.txt
--rw-r--r--   0 prism      (501) staff       (20)      242 2023-07-31 15:18:35.000000 prismstudio-1.1.7/prismstudio.egg-info/requires.txt
--rw-r--r--   0 prism      (501) staff       (20)       12 2023-07-31 15:18:35.000000 prismstudio-1.1.7/prismstudio.egg-info/top_level.txt
--rw-r--r--   0 prism      (501) staff       (20)      137 2023-07-31 15:18:16.000000 prismstudio-1.1.7/pyproject.toml
--rw-r--r--   0 prism      (501) staff       (20)       38 2023-07-31 15:18:35.091333 prismstudio-1.1.7/setup.cfg
--rw-r--r--   0 prism      (501) staff       (20)     1316 2023-07-31 15:18:16.000000 prismstudio-1.1.7/setup.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.086891 prismstudio-1.1.7/tests/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-1.1.7/tests/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)       94 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/conftest.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.087282 prismstudio-1.1.7/tests/test__validate_args/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     2200 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_common_functions.py
--rw-r--r--   0 prism      (501) staff       (20)     1539 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_fillna.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.089898 prismstudio-1.1.7/tests/test__validate_args/test_params/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     5990 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_01_frequency.py
--rw-r--r--   0 prism      (501) staff       (20)     2004 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_02_datetype.py
--rw-r--r--   0 prism      (501) staff       (20)     2719 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_03_periodtype.py
--rw-r--r--   0 prism      (501) staff       (20)     1615 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_04_adjustment.py
--rw-r--r--   0 prism      (501) staff       (20)     2304 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_05_shownid.py
--rw-r--r--   0 prism      (501) staff       (20)     1946 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_06_rank_method.py
--rw-r--r--   0 prism      (501) staff       (20)     2302 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_07_method.py
--rw-r--r--   0 prism      (501) staff       (20)     6448 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
--rw-r--r--   0 prism      (501) staff       (20)     3854 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_09_contains_universename.py
--rw-r--r--   0 prism      (501) staff       (20)     1717 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
--rw-r--r--   0 prism      (501) staff       (20)     1118 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_11_base.py
--rw-r--r--   0 prism      (501) staff       (20)     1792 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_12_preliminary.py
--rw-r--r--   0 prism      (501) staff       (20)      889 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_13_setting.py
--rw-r--r--   0 prism      (501) staff       (20)      956 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_14_settings.py
--rw-r--r--   0 prism      (501) staff       (20)     2441 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test_factors.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 15:18:35.090876 prismstudio-1.1.7/tests/test_util/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-1.1.7/tests/test_util/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)      603 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test_util/db_fixtures.py
--rw-r--r--   0 prism      (501) staff       (20)     1264 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test_util/dq_model.py
--rw-r--r--   0 prism      (501) staff       (20)     1753 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test_util/dq_table.py
--rw-r--r--   0 prism      (501) staff       (20)    15617 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test_util/factor_fixtures.py
--rw-r--r--   0 prism      (501) staff       (20)     2738 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test_util/update_factor.py
--rw-r--r--   0 prism      (501) staff       (20)     1259 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test_util/utils.py
--rw-r--r--   0 prism      (501) staff       (20)     1770 2023-07-31 15:18:16.000000 prismstudio-1.1.7/tests/test_version.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.731706 prismstudio-1.1.8/
+-rw-r--r--   0 prism      (501) staff       (20)    23016 2023-07-19 13:45:53.000000 prismstudio-1.1.8/LICENSE.txt
+-rw-r--r--   0 prism      (501) staff       (20)      440 2023-08-01 00:50:32.731567 prismstudio-1.1.8/PKG-INFO
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.720054 prismstudio-1.1.8/prism/
+-rw-r--r--   0 prism      (501) staff       (20)     1290 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/__init__.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.720486 prismstudio-1.1.8/prism/_common/
+-rw-r--r--   0 prism      (501) staff       (20)       35 2023-08-01 00:50:28.000000 prismstudio-1.1.8/prism/_common/.env
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_common/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     3472 2023-08-01 00:50:13.000000 prismstudio-1.1.8/prism/_common/config.py
+-rw-r--r--   0 prism      (501) staff       (20)    11067 2023-08-01 00:50:00.000000 prismstudio-1.1.8/prism/_common/const.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.720838 prismstudio-1.1.8/prism/_core/
+-rw-r--r--   0 prism      (501) staff       (20)      288 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_core/__init__.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.722279 prismstudio-1.1.8/prism/_core/_data/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_data/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)    17869 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_core/_data/esg.py
+-rw-r--r--   0 prism      (501) staff       (20)    46813 2023-08-01 00:50:00.000000 prismstudio-1.1.8/prism/_core/_data/estimate.py
+-rw-r--r--   0 prism      (501) staff       (20)     7950 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_data/event.py
+-rw-r--r--   0 prism      (501) staff       (20)    70894 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_data/financial.py
+-rw-r--r--   0 prism      (501) staff       (20)    12927 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_core/_data/index.py
+-rw-r--r--   0 prism      (501) staff       (20)   121051 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_data/industry.py
+-rw-r--r--   0 prism      (501) staff       (20)    43935 2023-07-31 16:42:12.000000 prismstudio-1.1.8/prism/_core/_data/market.py
+-rw-r--r--   0 prism      (501) staff       (20)     6446 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_data/precalculated.py
+-rw-r--r--   0 prism      (501) staff       (20)     3840 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_data/securitymaster.py
+-rw-r--r--   0 prism      (501) staff       (20)    15625 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_fn.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.722529 prismstudio-1.1.8/prism/_core/_model/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_core/_model/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     5272 2023-07-31 16:46:39.000000 prismstudio-1.1.8/prism/_core/_model/tcmodel.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.724479 prismstudio-1.1.8/prism/_core/_req_builder/
+-rw-r--r--   0 prism      (501) staff       (20)     1458 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2074 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_core/_req_builder/_auth.py
+-rw-r--r--   0 prism      (501) staff       (20)    22677 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_core/_req_builder/_dataquery.py
+-rw-r--r--   0 prism      (501) staff       (20)     2058 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/_dbinfo.py
+-rw-r--r--   0 prism      (501) staff       (20)     7633 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/_exportdata.py
+-rw-r--r--   0 prism      (501) staff       (20)     3633 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/_gui.py
+-rw-r--r--   0 prism      (501) staff       (20)    15003 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/_job.py
+-rw-r--r--   0 prism      (501) staff       (20)     4828 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_core/_req_builder/_list.py
+-rw-r--r--   0 prism      (501) staff       (20)    15321 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/_portfolio.py
+-rw-r--r--   0 prism      (501) staff       (20)     4295 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/_securitymaster.py
+-rw-r--r--   0 prism      (501) staff       (20)    25699 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/_task.py
+-rw-r--r--   0 prism      (501) staff       (20)    10877 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/_taskquery.py
+-rw-r--r--   0 prism      (501) staff       (20)    24533 2023-07-24 00:59:28.000000 prismstudio-1.1.8/prism/_core/_req_builder/_universe.py
+-rw-r--r--   0 prism      (501) staff       (20)     8696 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/_req_builder/preference.py
+-rw-r--r--   0 prism      (501) staff       (20)     9606 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_core/ols.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.725200 prismstudio-1.1.8/prism/_prismcomponent/
+-rw-r--r--   0 prism      (501) staff       (20)      353 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_prismcomponent/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     7644 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_prismcomponent/abstract_prismcomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)    12776 2023-08-01 00:50:00.000000 prismstudio-1.1.8/prism/_prismcomponent/datacomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)   186982 2023-07-31 15:18:16.000000 prismstudio-1.1.8/prism/_prismcomponent/prismcomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)    21567 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_prismcomponent/taskcomponent.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.726885 prismstudio-1.1.8/prism/_utils/
+-rw-r--r--   0 prism      (501) staff       (20)      480 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_utils/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2248 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_utils/auth_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     3629 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_utils/exceptions.py
+-rw-r--r--   0 prism      (501) staff       (20)     2028 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_utils/loader.py
+-rw-r--r--   0 prism      (501) staff       (20)     3706 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_utils/prismcomponent_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     5532 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_utils/req_builder_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)    14289 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_utils/validate_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     7232 2023-07-19 13:45:53.000000 prismstudio-1.1.8/prism/_utils/validate_utils_refactored.py
+-rw-r--r--   0 prism      (501) staff       (20)     1438 2023-07-24 00:59:23.000000 prismstudio-1.1.8/prism/_utils/version.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.727629 prismstudio-1.1.8/prismstudio.egg-info/
+-rw-r--r--   0 prism      (501) staff       (20)      440 2023-08-01 00:50:32.000000 prismstudio-1.1.8/prismstudio.egg-info/PKG-INFO
+-rw-r--r--   0 prism      (501) staff       (20)     3138 2023-08-01 00:50:32.000000 prismstudio-1.1.8/prismstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 prism      (501) staff       (20)        1 2023-08-01 00:50:32.000000 prismstudio-1.1.8/prismstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 prism      (501) staff       (20)      242 2023-08-01 00:50:32.000000 prismstudio-1.1.8/prismstudio.egg-info/requires.txt
+-rw-r--r--   0 prism      (501) staff       (20)       12 2023-08-01 00:50:32.000000 prismstudio-1.1.8/prismstudio.egg-info/top_level.txt
+-rw-r--r--   0 prism      (501) staff       (20)      137 2023-07-31 15:18:16.000000 prismstudio-1.1.8/pyproject.toml
+-rw-r--r--   0 prism      (501) staff       (20)       38 2023-08-01 00:50:32.731751 prismstudio-1.1.8/setup.cfg
+-rw-r--r--   0 prism      (501) staff       (20)     1316 2023-07-31 15:18:16.000000 prismstudio-1.1.8/setup.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.728110 prismstudio-1.1.8/tests/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-1.1.8/tests/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)       94 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/conftest.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.728460 prismstudio-1.1.8/tests/test__validate_args/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2200 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_common_functions.py
+-rw-r--r--   0 prism      (501) staff       (20)     1539 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_fillna.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.730489 prismstudio-1.1.8/tests/test__validate_args/test_params/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     5990 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_01_frequency.py
+-rw-r--r--   0 prism      (501) staff       (20)     2004 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_02_datetype.py
+-rw-r--r--   0 prism      (501) staff       (20)     2719 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_03_periodtype.py
+-rw-r--r--   0 prism      (501) staff       (20)     1615 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_04_adjustment.py
+-rw-r--r--   0 prism      (501) staff       (20)     2304 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_05_shownid.py
+-rw-r--r--   0 prism      (501) staff       (20)     1946 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_06_rank_method.py
+-rw-r--r--   0 prism      (501) staff       (20)     2302 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_07_method.py
+-rw-r--r--   0 prism      (501) staff       (20)     6448 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+-rw-r--r--   0 prism      (501) staff       (20)     3854 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_09_contains_universename.py
+-rw-r--r--   0 prism      (501) staff       (20)     1717 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
+-rw-r--r--   0 prism      (501) staff       (20)     1118 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_11_base.py
+-rw-r--r--   0 prism      (501) staff       (20)     1792 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_12_preliminary.py
+-rw-r--r--   0 prism      (501) staff       (20)      889 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_13_setting.py
+-rw-r--r--   0 prism      (501) staff       (20)      956 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_14_settings.py
+-rw-r--r--   0 prism      (501) staff       (20)     2441 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test_factors.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-08-01 00:50:32.731350 prismstudio-1.1.8/tests/test_util/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-1.1.8/tests/test_util/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)      603 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test_util/db_fixtures.py
+-rw-r--r--   0 prism      (501) staff       (20)     1264 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test_util/dq_model.py
+-rw-r--r--   0 prism      (501) staff       (20)     1753 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test_util/dq_table.py
+-rw-r--r--   0 prism      (501) staff       (20)    15617 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test_util/factor_fixtures.py
+-rw-r--r--   0 prism      (501) staff       (20)     2738 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test_util/update_factor.py
+-rw-r--r--   0 prism      (501) staff       (20)     1259 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test_util/utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     1770 2023-07-31 15:18:16.000000 prismstudio-1.1.8/tests/test_version.py
```

### Comparing `prismstudio-1.1.7/LICENSE.txt` & `prismstudio-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/__init__.py` & `prismstudio-1.1.8/prism/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_common/config.py` & `prismstudio-1.1.8/prism/_common/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     STAGING = "stg"
     PRODUCTION = "production"
     DEMO = "demo"
 
 
 class StateSettings(BaseSettings):
     ENV_STATE: EnvironmentState = 'production'
-    VERSION: str = '1.1.7'
+    VERSION: str = '1.1.8'
     URL_STABLE: str = 'https://api.prism39.com'
     URL_DEV: str = 'https://ops.prism39.com'
     dev: str = ':30495'
     stg: str = ':30496'
     demo: str = ':40452'
 
     class Config:
```

### Comparing `prismstudio-1.1.7/prism/_common/const.py` & `prismstudio-1.1.8/prism/_common/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 class EstimateDataComponentType(str, Enum):
     CONSENSUS = 'Consensus'
     GROWTH = 'Growth'
     GUIDANCE = 'Guidance'
     REVISION = 'Revision'
     ACTUAL = 'Actual'
     SURPRISE = 'Surprise'
+    RECOMMENDATION = 'Recommendation'
 
 
 class MarketDataComponentType(str, Enum):
     CLOSE = 'Close'
     OPEN = 'Open'
     HIGH = 'High'
     LOW = 'Low'
```

### Comparing `prismstudio-1.1.7/prism/_core/_data/esg.py` & `prismstudio-1.1.8/prism/_core/_data/esg.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_data/estimate.py` & `prismstudio-1.1.8/prism/_core/_data/estimate.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 from ..._prismcomponent.datacomponent import (
     _Actual,
     _Consensus,
     _Growth,
     _Guidance,
     _Revision,
     _Surprise,
+    _Recommendation,
 )
 from ..._utils.validate_utils import _validate_args
 
 
 __all__ = [
     'actual',
     'consensus',
     'growth',
     'guidance',
     'revision',
     'surprise',
+    'recommendation',
     'dataitems',
     'actual_dataitems',
     'consensus_dataitems',
     'growth_dataitems',
     'guidance_dataitems',
     'revision_dataitems',
     'surprise_dataitems',
@@ -488,26 +490,26 @@
         29      200493    EPS Normalized - Revision, Unfiltered No Change
         30      200494           EPS Normalized - Revision, Unfiltered Up
         31      200495                      EPS Normalized - Revision, Up
 
         >>> eps = prism.estimate.revision(dataitemid=200495, periodtype='Q')
         >>> eps_df = eps.get_data(universe='S&P 500', startdate='2010-01-01', enddate='2015-12-31', shownid=['ticker'])
         >>> eps_df
-                listingid        date  EPS Normalized - Revision, Up  Ticker
-        0         2586086  2010-04-20                              1     AFL
-        1         2586086  2010-04-21	                             1     AFL
-        2         2586086  2010-04-22	                             1     AFL
-        3         2586086  2010-04-29	                             2     AFL
-        4         2586086  2010-05-01	                             1     AFL
-        ...           ...         ...	                           ...     ...
-        126320  306093931  2015-12-05	                             1    PYPL
-        126321  313064514  2015-11-24	                             0     HPE
-        126322  313064514  2015-11-26	                             3     HPE
-        126323  313064514  2015-11-27	                             0     HPE
-        126324  313064514  2015-12-11	                             0     HPE
+                listingid        date   EPS Normalized - Revision, Up  Ticker
+        0         2586086  2010-04-20                               1     AFL
+        1         2586086  2010-04-21                               1     AFL
+        2         2586086  2010-04-22                               1     AFL
+        3         2586086  2010-04-29                               2     AFL
+        4         2586086  2010-05-01                               1     AFL
+        ...           ...         ...                             ...     ...
+        126320  306093931  2015-12-05                               1    PYPL
+        126321  313064514  2015-11-24                               0     HPE
+        126322  313064514  2015-11-26                               3     HPE
+        126323  313064514  2015-11-27                               0     HPE
+        126324  313064514  2015-12-11                               0     HPE
     """
     if periodtype in ["LTM"]:
         raise PrismValueError(
             f"Revision cannot take {periodtype} as periodtype.",
             valid_list=PeriodType,
             invalids=["LTM"],
         )
@@ -598,14 +600,82 @@
         dataitemid=dataitemid,
         periodtype=periodtype,
         currency=currency,
         package=package,
     )
 
 
+def recommendation(
+    dataitemid: int,
+    periodtype: str,
+    package: str = None,
+):
+    """
+    | TODO: Recommnedation Data Component description
+    | Default frequency is quarterly.
+
+    Parameters
+    ----------
+        dataitemid : int
+            | Unique identifier for the different data item. This identifies the type of the value (Score, Buy, etc.)
+
+        periodtype : str, {'A', 'Annual', 'SA', 'Semi-Annual', 'Quarterly', 'Q',  'NTM', 'YTD', 'Non-Periodic', 'Q-SA'}
+            | Estimate Period in which the financial statement results are estimated.
+            | An Estimate Period can be of one of the following Period Types:
+
+            - Annual period (A)
+            - Quarterly period (Q)
+            - Next twelve months (NTM)
+            - Year-to-date (YTD)
+            - Semi-Annual (SA)
+            - Non-Periodic
+            - Quarterly and Semi-Annual period (Q-SA) in quarterly standard
+
+    Returns
+    -------
+        prism._PrismComponent
+
+    Examples
+    --------
+        >>> df = prism.estimate.recommendation_dataitems('Score')
+        >>> df[['dataitemid', 'dataitemname']]
+           dataitemid                     dataitemname
+        0      200631           Recommendation - Score
+        1      200637  Industry Recommendation - Score
+        2      601998           Recommendation - Score
+        >>> rec = prism.estimate.recommendation(dataitemid=200631, periodtype='LTM')
+        >>> rec.get_data("LSE", "2022-01-01", shownid=['companyname'])
+               listingid                 date  Recommendation - Score                     Company Name
+        0       22033716  2022-01-01 00:30:00                 2.42105  The Berkeley Group Holdings plc
+        1       20131190  2022-01-01 03:29:13                 1.42105         Barratt Developments plc
+        2       20175571  2022-01-01 03:29:13                 2.09091                    Elementis plc
+        3       25117249  2022-01-01 03:29:13                 2.06250      Lancashire Holdings Limited
+        4       29847692  2022-01-01 03:29:13                 2.50000                       Hiscox Ltd
+        ...          ...                  ...                     ...                              ...
+        63519   20157229  2023-07-31 13:59:44                 2.00000                     RS Group plc
+        63520  224316065  2023-07-31 14:31:00                 1.77778                          WPP plc
+        63521   20176224  2023-07-31 14:40:11                 2.14286                     Spectris plc
+        63522   20157229  2023-07-31 15:11:00                 2.00000                     RS Group plc
+        63523   20182531  2023-07-31 17:04:13                 1.76923                      Pearson plc
+
+    """
+    if periodtype in ["LTM"]:
+        raise PrismValueError(
+            f"Consensus cannot take {periodtype} as periodtype.",
+            valid_list=PeriodType,
+            invalids=["LTM"],
+        )
+    return _estimate_builder(
+        _Recommendation,
+        dataitemid=dataitemid,
+        periodtype=periodtype,
+        package=package
+    )
+
+
 @_validate_args
 def dataitems(search: str = None, package: str = None):
     """
     Usable data items for the estimate data category.
 
     Parameters
     ----------
@@ -926,7 +996,62 @@
         1      200613  Net Income (Excl. Extraordinary Items & Good W...
         2      200614            Net Income (GAAP) - Surpise, Difference
         3      200615               Net Income (GAAP) - Surpise, Percent
         4      200616        Net Income Normalized - Surpise, Difference
         5      200617           Net Income Normalized - Surpise, Percent
     """
     return _list_dataitem_estimate(_EstimateDataComponentType.SURPRISE, search, package)
+
+
+
+@_validate_args
+def recommendation_dataitems(search: str = None, package: str = None):
+    """
+    Usable data items for the recommendation data component.
+
+    Parameters
+    ----------
+        search : str, default None
+            | Search word for dataitems name, the search is case-insensitive.
+
+        package : str, default None
+            | Search word for package name, the search is case-insensitive.
+
+    Returns
+    -------
+        pandas.DataFrame
+            Data items that belong to cash flow statement data component.
+
+        Columns:
+            - *datamodule*
+            - *datacomponent*
+            - *dataitemid*
+            - *datadescription*
+
+    Examples
+    --------
+        >>> di = prism.estimate.recommendation_dataitems()
+        >>> di[['dataitemid', 'dataitemname']]
+           dataitemid                                         dataitemname
+        0      200625    Recommendation - # of Analysts Buy Recommendation
+        1      200626    Recommendation - # of Analysts Hold Recommenda...
+        2      200627    Recommendation - # of Analysts No Opinion Reco...
+        3      200628    Recommendation - # of Analysts Outperform Reco...
+        4      200629    Recommendation - # of Analysts Sell Recommenda...
+        5      200630    Recommendation - # of Analysts Underperform Re...
+        6      200631    Recommendation - Score
+        7      200632    Industry Recommendation - # of Analysts Buy Re...
+        8      200633    Industry Recommendation - # of Analysts Hold R...
+        9      200634    Industry Recommendation - # of Analysts Outper...
+        10     200635    Industry Recommendation - # of Analysts Sell R...
+        11     200636    Industry Recommendation - # of Analysts Underp...
+        12     200637    Industry Recommendation - Score
+        13     601991    Recommendation - # of Analysts Buy Recommendation
+        14     601993    Recommendation - # of Analysts Hold Recommenda...
+        15     601995    Recommendation - # of Analysts Sell Recommenda...
+        16     601996    Recommendation - # of Analysts No Opinion Reco...
+        17     601997    Recommendation - # of Analysts Total Recommend...
+        18     601998    Recommendation - Score
+        19     602197    Recommendation - # of Analysts Overweight Reco...
+        20     602198    Recommendation - # of Analysts Underweight Rec...
+    """
+    return _list_dataitem_estimate(_EstimateDataComponentType.RECOMMENDATION, search, package)
```

### Comparing `prismstudio-1.1.7/prism/_core/_data/event.py` & `prismstudio-1.1.8/prism/_core/_data/event.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_data/financial.py` & `prismstudio-1.1.8/prism/_core/_data/financial.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_data/index.py` & `prismstudio-1.1.8/prism/_core/_data/index.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_data/industry.py` & `prismstudio-1.1.8/prism/_core/_data/industry.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_data/market.py` & `prismstudio-1.1.8/prism/_core/_data/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -944,14 +944,16 @@
 
     Returns
     -------
         prism._PrismComponent
 
     Examples
     --------
+        >>> immcap = prism.market.implied_market_cap()
+        >>> immcap.get_data("Semi", "2020-01-01", shownid=['Company Name'])
              listingid        date    implieddilutedmarketcapout  currency               Company Name
         0    707934944  2021-06-24                  1.317918e+09       USD  indie Semiconductor, Inc.
         1    707934944  2021-06-25                  1.335508e+09       USD  indie Semiconductor, Inc.
         2    707934944  2021-06-26                  1.335508e+09       USD  indie Semiconductor, Inc.
         3    707934944  2021-06-27                  1.335508e+09       USD  indie Semiconductor, Inc.
         4    707934944  2021-06-28                  1.332802e+09       USD  indie Semiconductor, Inc.
         ...        ...         ...                           ...       ...                        ...
```

### Comparing `prismstudio-1.1.7/prism/_core/_data/precalculated.py` & `prismstudio-1.1.8/prism/_core/_data/precalculated.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_data/securitymaster.py` & `prismstudio-1.1.8/prism/_core/_data/securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_fn.py` & `prismstudio-1.1.8/prism/_core/_fn.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_model/tcmodel.py` & `prismstudio-1.1.8/prism/_core/_model/tcmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 
 class almgren(_PrismTCModelComponent):
     r"""
     | Estimates and manage the trading costs associated with executing large orders in financial markets for a given trade.
     | The model was created/calibrated based on the data from Citi's trading desk. It uses 3/5 power laws instead of conventional square-root law.
     |
     .. math:: C = \frac 1 2 + \eta\sigma|\frac X {VT}|^\frac 3 5
-    |
     .. math:: I = \sigma\gamma \frac X V(\frac \theta V)^\frac 1 4
     |
-    | :math:`X \equiv` Transactions in shares
-    | :math:`T \equiv` Trade Duration
-    | :math:`V \equiv` Average Daily Volume
-    | :math:`\theta \equiv` Shares Outstanding
-    | :math:`\gamma = 0.314`
-    | :math:`\eta = 0.142`
+    .. math:: X \equiv \text {Transactions in shares}
+    .. math:: T \equiv \text {Trade Duration}
+    .. math:: V \equiv \text {Average Daily Volume}
+    .. math:: \theta \equiv \text {Shares Outstanding}
+    .. math:: \gamma = 0.314
+    .. math:: \eta = 0.142
 
 
     Parameters
     ----------
 
         transaction : prism._PrismComponent
             | Desired currency for the pricing data.
```

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/__init__.py` & `prismstudio-1.1.8/prism/_core/_req_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_auth.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_auth.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_dataquery.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_dataquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_dbinfo.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_dbinfo.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_exportdata.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_exportdata.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_gui.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_gui.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_job.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_job.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_list.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_list.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_portfolio.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_portfolio.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_securitymaster.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_task.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_task.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_taskquery.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_taskquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/_universe.py` & `prismstudio-1.1.8/prism/_core/_req_builder/_universe.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/_req_builder/preference.py` & `prismstudio-1.1.8/prism/_core/_req_builder/preference.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_core/ols.py` & `prismstudio-1.1.8/prism/_core/ols.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_prismcomponent/abstract_prismcomponent.py` & `prismstudio-1.1.8/prism/_prismcomponent/abstract_prismcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_prismcomponent/datacomponent.py` & `prismstudio-1.1.8/prism/_prismcomponent/datacomponent.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,18 @@
     _component_name = EstimateDataComponentType.ACTUAL
 
 
 class _Surprise(_PrismEstimateComponent):
     _component_name = EstimateDataComponentType.SURPRISE
 
 
+class _Recommendation(_PrismEstimateComponent):
+    _component_name = EstimateDataComponentType.RECOMMENDATION
+
+
 # ------------------------------------------------------------------------------------------------------------------- #
 #                                                          SM                                                         #
 # ------------------------------------------------------------------------------------------------------------------- #
 class _SecurityMasterAttribute(_PrismDataComponent, _PrismComponent):
     _component_category = DataCategoryType.SM
     _component_name = OtherDataComponentType.SM
```

### Comparing `prismstudio-1.1.7/prism/_prismcomponent/prismcomponent.py` & `prismstudio-1.1.8/prism/_prismcomponent/prismcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_prismcomponent/taskcomponent.py` & `prismstudio-1.1.8/prism/_prismcomponent/taskcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_utils/auth_utils.py` & `prismstudio-1.1.8/prism/_utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_utils/exceptions.py` & `prismstudio-1.1.8/prism/_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_utils/loader.py` & `prismstudio-1.1.8/prism/_utils/loader.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_utils/prismcomponent_utils.py` & `prismstudio-1.1.8/prism/_utils/prismcomponent_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_utils/req_builder_utils.py` & `prismstudio-1.1.8/prism/_utils/req_builder_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_utils/validate_utils.py` & `prismstudio-1.1.8/prism/_utils/validate_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_utils/validate_utils_refactored.py` & `prismstudio-1.1.8/prism/_utils/validate_utils_refactored.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prism/_utils/version.py` & `prismstudio-1.1.8/prism/_utils/version.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/prismstudio.egg-info/SOURCES.txt` & `prismstudio-1.1.8/prismstudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/setup.py` & `prismstudio-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_common_functions.py` & `prismstudio-1.1.8/tests/test__validate_args/test_common_functions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_fillna.py` & `prismstudio-1.1.8/tests/test__validate_args/test_fillna.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_01_frequency.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_01_frequency.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_02_datetype.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_02_datetype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_03_periodtype.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_03_periodtype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_04_adjustment.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_04_adjustment.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_05_shownid.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_05_shownid.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_06_rank_method.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_06_rank_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_07_method.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_07_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_09_contains_universename.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_09_contains_universename.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_11_base.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_11_base.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_12_preliminary.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_12_preliminary.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_13_setting.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_13_setting.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test__validate_args/test_params/test_param_14_settings.py` & `prismstudio-1.1.8/tests/test__validate_args/test_params/test_param_14_settings.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test_factors.py` & `prismstudio-1.1.8/tests/test_factors.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test_util/db_fixtures.py` & `prismstudio-1.1.8/tests/test_util/db_fixtures.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test_util/dq_model.py` & `prismstudio-1.1.8/tests/test_util/dq_model.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test_util/dq_table.py` & `prismstudio-1.1.8/tests/test_util/dq_table.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test_util/factor_fixtures.py` & `prismstudio-1.1.8/tests/test_util/factor_fixtures.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test_util/update_factor.py` & `prismstudio-1.1.8/tests/test_util/update_factor.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test_util/utils.py` & `prismstudio-1.1.8/tests/test_util/utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-1.1.7/tests/test_version.py` & `prismstudio-1.1.8/tests/test_version.py`

 * *Files identical despite different names*

