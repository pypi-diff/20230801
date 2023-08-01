# Comparing `tmp/m-abac-1.0.5.tar.gz` & `tmp/m-abac-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-1.0.5.tar", last modified: Mon Jul 31 04:21:26 2023, max compression
+gzip compressed data, was "m-abac-1.0.6.tar", last modified: Tue Aug  1 06:04:49 2023, max compression
```

## Comparing `m-abac-1.0.5.tar` & `m-abac-1.0.6.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.521657 m-abac-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     1683 2023-07-31 04:21:26.520657 m-abac-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-31 04:19:17.000000 m-abac-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.450655 m-abac-1.0.5/m_abac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1683 2023-07-31 04:21:26.000000 m-abac-1.0.5/m_abac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4522 2023-07-31 04:21:26.000000 m-abac-1.0.5/m_abac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:21:26.000000 m-abac-1.0.5/m_abac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      115 2023-07-31 04:21:26.000000 m-abac-1.0.5/m_abac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-31 04:21:26.000000 m-abac-1.0.5/m_abac.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.440655 m-abac-1.0.5/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.441655 m-abac-1.0.5/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.453655 m-abac-1.0.5/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.455655 m-abac-1.0.5/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    21622 2023-07-20 01:33:02.000000 m-abac-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7706 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-07-20 01:33:02.000000 m-abac-1.0.5/mobio/libs/abac/config.py
--rw-r--r--   0 root         (0) root         (0)    22064 2023-07-20 01:33:02.000000 m-abac-1.0.5/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.458655 m-abac-1.0.5/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.460656 m-abac-1.0.5/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.462656 m-abac-1.0.5/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.471656 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      418 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/any_contains.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.477656 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2649 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.484656 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.487656 m-abac-1.0.5/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.492657 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/
--rw-r--r--   0 root         (0) root         (0)      228 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/base.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      971 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.503657 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      328 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/base_list.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/list_gt.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/list_gte.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/list_lt.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/list_lte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.506657 m-abac-1.0.5/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      702 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2746 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:21:26.519657 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7273 2023-07-31 04:19:17.000000 m-abac-1.0.5/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     6433 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-07-17 15:45:49.000000 m-abac-1.0.5/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-17 15:45:49.000000 m-abac-1.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 04:21:26.521657 m-abac-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9805 2023-07-31 04:21:25.000000 m-abac-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.474953 m-abac-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-08-01 06:04:49.473953 m-abac-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2023-08-01 06:02:45.000000 m-abac-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.347949 m-abac-1.0.6/m_abac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-08-01 06:04:49.000000 m-abac-1.0.6/m_abac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4522 2023-08-01 06:04:49.000000 m-abac-1.0.6/m_abac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 06:04:49.000000 m-abac-1.0.6/m_abac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-08-01 06:04:49.000000 m-abac-1.0.6/m_abac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-08-01 06:04:49.000000 m-abac-1.0.6/m_abac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.334949 m-abac-1.0.6/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.334949 m-abac-1.0.6/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.355949 m-abac-1.0.6/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.357950 m-abac-1.0.6/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    21622 2023-07-20 01:33:02.000000 m-abac-1.0.6/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7706 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-07-20 01:33:02.000000 m-abac-1.0.6/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    22064 2023-07-20 01:33:02.000000 m-abac-1.0.6/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.361950 m-abac-1.0.6/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.363950 m-abac-1.0.6/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.366950 m-abac-1.0.6/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.376950 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      418 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/any_contains.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.391950 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.399951 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.408951 m-abac-1.0.6/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.415951 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/base.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.442952 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/base_list.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/list_gt.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/list_gte.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/list_lt.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/list_lte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.461953 m-abac-1.0.6/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      702 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-07-31 04:19:17.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 06:04:49.472953 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7498 2023-08-01 06:02:45.000000 m-abac-1.0.6/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-17 15:45:49.000000 m-abac-1.0.6/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-17 15:45:49.000000 m-abac-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 06:04:49.474953 m-abac-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9805 2023-08-01 06:04:48.000000 m-abac-1.0.6/setup.py
```

### Comparing `m-abac-1.0.5/PKG-INFO` & `m-abac-1.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac
-Version: 1.0.5
+Version: 1.0.6
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
@@ -51,9 +51,10 @@
 #### Log - 1.0.3
     - update cache
 #### Log - 1.0.4
     - update cache
 #### Log - 1.0.5
     - mm-dd operator
     - update if exists
-    
+#### Log - 1.0.6
+    - update operator exists
```

### Comparing `m-abac-1.0.5/README.md` & `m-abac-1.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,9 +28,10 @@
 #### Log - 1.0.3
     - update cache
 #### Log - 1.0.4
     - update cache
 #### Log - 1.0.5
     - mm-dd operator
     - update if exists
-    
+#### Log - 1.0.6
+    - update operator exists
```

### Comparing `m-abac-1.0.5/m_abac.egg-info/PKG-INFO` & `m-abac-1.0.6/m_abac.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac
-Version: 1.0.5
+Version: 1.0.6
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
@@ -51,9 +51,10 @@
 #### Log - 1.0.3
     - update cache
 #### Log - 1.0.4
     - update cache
 #### Log - 1.0.5
     - mm-dd operator
     - update if exists
-    
+#### Log - 1.0.6
+    - update operator exists
```

### Comparing `m-abac-1.0.5/m_abac.egg-info/SOURCES.txt` & `m-abac-1.0.6/m_abac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-1.0.6/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/call_api.py` & `m-abac-1.0.6/mobio/libs/abac/call_api.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/config.py` & `m-abac-1.0.6/mobio/libs/abac/config.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/pdp.py` & `m-abac-1.0.6/mobio/libs/abac/pdp.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/any_contains.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/any_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_contains.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_eq.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_gt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_gte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_lt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_lte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/monthday/day_neq.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/monthday/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/base_list.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/base_list.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/list_gt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/list_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/list_gte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/list_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/list_lt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/list_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/list_lte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/list_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-1.0.6/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/exceptions.py` & `m-abac-1.0.6/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/policy.py` & `m-abac-1.0.6/mobio/libs/abac/policy/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,24 @@
         have_condition_exclude = False
         for item in self.condition:
             cond_schema = self.validate_item_condition(item)
             # print("abac_sdk cond_schema: {}".format(json.dumps(cond_schema)))
             if cond_schema.get("operator") == "Null":
                 list_condition.append({**item})
             elif cond_schema.get("operator") in ["Exists", "NotExists"]:
+                if_exists = cond_schema.get("if_exists")
+                what_check = self.get_value_from_field(cond_schema.get("field"))
+                if if_exists:
+                    if not what_check and what_check not in [0, False]:
+                        continue
                 resource_name, resource_key = Utils.split_delemiter_resource(cond_schema.get("field"))
                 data_resource = {}
                 if resource_name:
-                    if self.request_access.get(resource_name) and isinstance(self.request_access.get(resource_name),
-                                                                             dict):
+                    if self.request_access.get(resource_name) and isinstance(
+                            self.request_access.get(resource_name), dict):
                         data_resource = self.request_access.get(resource_name)
                 list_condition.append({
                     **item,
                     "values": data_resource,
                     "what": resource_key,
                 })
             else:
```

### Comparing `m-abac-1.0.5/mobio/libs/abac/policy/utils.py` & `m-abac-1.0.6/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/mobio/libs/abac/result_access.py` & `m-abac-1.0.6/mobio/libs/abac/result_access.py`

 * *Files identical despite different names*

### Comparing `m-abac-1.0.5/setup.py` & `m-abac-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
 version_dev='1.0.34'
-version_prod='1.0.5'
+version_prod='1.0.6'
 
 run_mode=''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -71,15 +71,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.5',  # Required
+    version='1.0.6',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

