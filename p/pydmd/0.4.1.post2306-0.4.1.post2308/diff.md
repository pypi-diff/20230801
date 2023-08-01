# Comparing `tmp/pydmd-0.4.1.post2306.tar.gz` & `tmp/pydmd-0.4.1.post2308.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmd-0.4.1.post2306.tar", last modified: Thu Jun  1 03:29:13 2023, max compression
+gzip compressed data, was "pydmd-0.4.1.post2308.tar", last modified: Tue Aug  1 03:04:08 2023, max compression
```

## Comparing `pydmd-0.4.1.post2306.tar` & `pydmd-0.4.1.post2308.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:29:13.065699 pydmd-0.4.1.post2306/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-01 03:29:13.065699 pydmd-0.4.1.post2306/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:29:13.061699 pydmd-0.4.1.post2306/pydmd/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42597 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/bopdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/cdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmd_modes_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmdbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmdc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/dmdoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/fbdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/hankeldmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/havok.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/hodmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/mrdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/optdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/paramdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/pidmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/pidmd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/rdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/spdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/subspacedmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pydmd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:29:13.061699 pydmd-0.4.1.post2306/pydmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:29:12.000000 pydmd-0.4.1.post2306/pydmd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 03:29:13.000000 pydmd-0.4.1.post2306/pydmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:29:13.065699 pydmd-0.4.1.post2306/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:29:13.065699 pydmd-0.4.1.post2306/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_bopdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_cdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmd_modes_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmdbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_dmdoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_fbdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_hankeldmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_havok.py
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_hodmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_mrdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_optdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_paramdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_pidmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_rdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_spdmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-01 03:28:58.000000 pydmd-0.4.1.post2306/tests/test_subspacedmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:04:08.151317 pydmd-0.4.1.post2308/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-01 03:04:08.151317 pydmd-0.4.1.post2308/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:04:08.147317 pydmd-0.4.1.post2308/pydmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47260 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/bopdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/cdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21794 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/dmd_modes_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26459 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/dmdbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/dmdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/dmdoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/fbdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/hankeldmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/havok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/hodmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/mrdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/optdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/paramdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/pidmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/pidmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/rdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/spdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/subspacedmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pydmd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:04:08.147317 pydmd-0.4.1.post2308/pydmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-01 03:04:08.000000 pydmd-0.4.1.post2308/pydmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-01 03:04:08.000000 pydmd-0.4.1.post2308/pydmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:04:08.000000 pydmd-0.4.1.post2308/pydmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:04:07.000000 pydmd-0.4.1.post2308/pydmd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 03:04:08.000000 pydmd-0.4.1.post2308/pydmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 03:04:08.000000 pydmd-0.4.1.post2308/pydmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:04:08.151317 pydmd-0.4.1.post2308/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:04:08.147317 pydmd-0.4.1.post2308/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_bopdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_cdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_dmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_dmd_modes_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_dmdbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_dmdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_dmdoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_fbdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_hankeldmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_havok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_hodmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_mrdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_optdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_paramdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_pidmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_rdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_spdmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-01 03:03:54.000000 pydmd-0.4.1.post2308/tests/test_subspacedmd.py
```

### Comparing `pydmd-0.4.1.post2306/LICENSE.rst` & `pydmd-0.4.1.post2308/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/PKG-INFO` & `pydmd-0.4.1.post2308/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmd
-Version: 0.4.1.post2306
+Version: 0.4.1.post2308
 Summary: Python Dynamic Mode Decomposition.
 Home-page: https://github.com/mathLab/PyDMD
 Author: Nicola Demo, Marco Tezzele, Francesco Andreuzzi, Sara Ichinaga
 Author-email: pydmd.info@gmail.com
 License: MIT
 Keywords: dynamic-mode-decomposition dmd
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydmd-0.4.1.post2306/pydmd/__init__.py` & `pydmd-0.4.1.post2308/pydmd/__init__.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/bopdmd.py` & `pydmd-0.4.1.post2308/pydmd/bopdmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,22 @@
         when performing BOP-DMD. Eigenvalues will be sorted by real part and
         then by imaginary part to break ties if `eig_sort="real"`, by imaginary
         part and then by real part to break ties if `eig_sort="imag"`, or by
         magnitude if `eig_sort="abs"`. If `eig_sort="auto"`, one of the
         previously-mentioned sorting methods is chosen depending on eigenvalue
         variance.
     :type eig_sort: {"real", "imag", "abs", "auto"}
+    :param eig_constraints: Set containing desired DMD operator eigenvalue
+        constraints. Currently available constraints are `"stable"`, which
+        constrains eigenvalues to the left half of the complex plane,
+        `"imag"`, which constrains eigenvalues to the imaginary axis, and
+        `"conjugate_pairs"`, which enforces that eigenvalues are always
+        present with their complex conjugate. Note that constraints may be
+        combined if valid.
+    :type eig_constraints: set(str)
     :param init_lambda: Initial value used for the regularization parameter in
         the Levenberg method. Default is 1.0.
         Note: Larger lambda values make the method more like gradient descent.
     :type init_lambda: float
     :param maxlam: Maximum number of of steps used in the inner Levenberg loop,
         i.e. the number of times you increase lambda before quitting. Default
         is 52.
@@ -103,14 +111,15 @@
         compute_A,
         use_proj,
         init_alpha,
         proj_basis,
         num_trials,
         trial_size,
         eig_sort,
+        eig_constraints,
         init_lambda=1.0,
         maxlam=52,
         lamup=2.0,
         use_levmarq=True,
         maxiter=30,
         tol=1e-6,
         eps_stall=1e-12,
@@ -120,14 +129,15 @@
         self._compute_A = compute_A
         self._use_proj = use_proj
         self._init_alpha = init_alpha
         self._proj_basis = proj_basis
         self._num_trials = num_trials
         self._trial_size = trial_size
         self._eig_sort = eig_sort
+        self._eig_constraints = eig_constraints
         self._varpro_opts = (
             init_lambda,
             maxlam,
             lamup,
             use_levmarq,
             maxiter,
             tol,
@@ -236,14 +246,56 @@
             elif opt_value > opt_max:
                 msg = (
                     "Option {} with value {} is greater than {}, "
                     "which is not recommended."
                 )
                 warnings.warn(msg.format(opt_name, opt_value, opt_max))
 
+    def _push_eigenvalues(self, eigenvalues):
+        """
+        Helper function that constrains the given eigenvalues according to
+        the arguments found in self._eig_constraints. If no constraints were
+        given, this function simply returns the given eigenvalues sorted
+        according to real part and then imaginary part to break ties.
+
+        :param eigenvalues: Vector of original eigenvalues.
+        :type eigenvalues: numpy.ndarray
+        :return: Vector of constrained eigenvalues.
+        :rtype: numpy.ndarray
+        """
+        if "conjugate_pairs" in self._eig_constraints:
+            eigenvalues_sorted = np.sort(eigenvalues)
+            num_eigs = len(eigenvalues)
+            num_pair = num_eigs // 2
+            new_eigs = []
+            # If given an odd number of eigenvalues, find the eigenvalue with
+            # the smallest imaginary part and take it to be a real eigenvalue.
+            if num_eigs % 2 == 1:
+                imag_magnitudes = np.abs(eigenvalues_sorted.imag)
+                ind_single = np.argmin(imag_magnitudes)
+                new_eigs.append(eigenvalues_sorted[ind_single].real)
+                eigenvalues_sorted = np.delete(eigenvalues_sorted, ind_single)
+            for i in range(num_pair):
+                eig1 = eigenvalues_sorted[2 * i]
+                eig2 = eigenvalues_sorted[2 * i + 1]
+                real_comp = (eig1.real + eig2.real) / 2
+                imag_comp = (abs(eig1.imag) + abs(eig2.imag)) / 2
+                new_eigs.append(real_comp + 1j * imag_comp)
+                new_eigs.append(real_comp - 1j * imag_comp)
+
+            eigenvalues = np.array(new_eigs)
+
+        if "stable" in self._eig_constraints:
+            right_half = eigenvalues.real > 0.0
+            eigenvalues[right_half] = 1j * eigenvalues[right_half].imag
+        elif "imag" in self._eig_constraints:
+            eigenvalues = 1j * eigenvalues.imag
+
+        return np.sort(eigenvalues)
+
     def _exp_function(self, alpha, t):
         """
         Matrix of exponentials.
 
         :param alpha: Vector of time scalings in the exponent.
         :type alpha: numpy.ndarray
         :param t: Vector of time values.
@@ -417,18 +469,22 @@
             use_fulljac,
             verbose,
         ) = self._varpro_opts
 
         # Initialize values.
         tolrank = M * np.finfo(float).eps
         _lambda = init_lambda
-        alpha = np.copy(init_alpha)
+        alpha = self._push_eigenvalues(init_alpha)
         B, residual, error = compute_residual(alpha)
         U, S, Vh = self._compute_irank_svd(Phi(alpha, t), tolrank)
 
+        # Initialize termination flags.
+        converged = False
+        stalled = False
+
         # Initialize storage.
         all_error = np.zeros(maxiter)
         djac_matrix = np.zeros((M * IS, IA), dtype="complex")
         rjac = np.zeros((2 * IA, IA), dtype="complex")
         scales = np.zeros(IA)
 
         for itr in range(maxiter):
@@ -479,27 +535,28 @@
                 """
                 # Compute the step delta.
                 rjac[IA:] = _lambda * np.diag(scales_pvt)
                 delta = np.linalg.lstsq(rjac, rhs, rcond=None)[0]
                 delta = delta[ij_pvt]
                 # Compute the updated alpha vector.
                 alpha_updated = alpha.ravel() + delta.ravel()
+                alpha_updated = self._push_eigenvalues(alpha_updated)
                 return delta, alpha_updated
 
             # Take a step using our initial step size init_lambda.
             delta_0, alpha_0 = step(_lambda, rhs, scales_pvt, ij_pvt)
             B_0, residual_0, error_0 = compute_residual(alpha_0)
 
             # Check actual improvement vs predicted improvement.
             actual_improvement = error - error_0
             pred_improvement = (
                 0.5
                 * np.linalg.multi_dot(
                     [delta_0.conj().T, djac_matrix.conj().T, rhs_temp]
-                ).real
+                )[0].real
             )
             improvement_ratio = actual_improvement / pred_improvement
 
             if error_0 < error:
                 # Rescale lambda based on the improvement ratio.
                 _lambda *= max(1 / 3, 1 - (2 * improvement_ratio - 1) ** 3)
                 alpha, B, residual, error = alpha_0, B_0, residual_0, error_0
@@ -507,64 +564,68 @@
                 # Increase lambda until something works.
                 for _ in range(maxlam):
                     _lambda *= lamup
                     delta_0, alpha_0 = step(_lambda, rhs, scales_pvt, ij_pvt)
                     B_0, residual_0, error_0 = compute_residual(alpha_0)
 
                     if error_0 < error:
-                        alpha, B = alpha_0, B_0
-                        residual, error = residual_0, error_0
                         break
 
-                # Terminate if no appropriate step length was found.
+                # Terminate if no appropriate step length was found...
                 if error_0 >= error:
                     if verbose:
                         msg = (
                             "Failed to find appropriate step length at "
                             "iteration {}. Current error {}."
                         )
-                        warnings.warn(msg.format(itr, error))
+                        print(msg.format(itr, error))
                     return B, alpha
 
+                # ...otherwise, update and proceed.
+                alpha, B, residual, error = alpha_0, B_0, residual_0, error_0
+
             # Record the current error.
             all_error[itr] = error
 
             # Print iterative progress if the verbose flag is turned on.
             if verbose:
                 update_msg = "Step {} Error {} Lambda {}"
                 print(update_msg.format(itr, error, _lambda))
 
-            # Terminate if the tolerance is met.
-            if error < tol:
+            # Update termination status and terminate if converged or stalled.
+            converged = error < tol
+            error_reduction = all_error[itr - 1] - all_error[itr]
+            stalled = (itr > 0) and (
+                error_reduction < eps_stall * all_error[itr - 1]
+            )
+
+            if converged:
+                if verbose:
+                    print("Convergence reached!")
                 return B, alpha
 
-            # Terminate if a stall is detected.
-            if (
-                itr > 0
-                and all_error[itr - 1] - all_error[itr]
-                < eps_stall * all_error[itr - 1]
-            ):
+            if stalled:
                 if verbose:
                     msg = (
                         "Stall detected: error reduced by less than {} "
                         "times the error at the previous step. "
                         "Iteration {}. Current error {}."
                     )
-                    warnings.warn(msg.format(eps_stall, itr, error))
+                    print(msg.format(eps_stall, itr, error))
                 return B, alpha
 
             U, S, Vh = self._compute_irank_svd(Phi(alpha, t), tolrank)
 
         # Failed to meet tolerance in maxiter steps.
         if verbose:
             msg = (
                 "Failed to reach tolerance after maxiter = {} iterations. "
                 "Current error {}."
             )
-            warnings.warn(msg.format(maxiter, error))
+            print(msg.format(maxiter, error))
 
         return B, alpha
 
     def _single_trial_compute_operator(self, H, t, init_alpha):
         """
         Helper function that computes the standard optimized dmd operator.
         Returns the resulting DMD modes, eigenvalues, amplitudes, reduced
@@ -756,14 +817,22 @@
         when performing BOP-DMD. Eigenvalues will be sorted by real part and
         then by imaginary part to break ties if `eig_sort="real"`, by imaginary
         part and then by real part to break ties if `eig_sort="imag"`, or by
         magnitude if `eig_sort="abs"`. If `eig_sort="auto"`, one of the
         previously-mentioned sorting methods is chosen depending on eigenvalue
         variance. Default is "auto".
     :type eig_sort: {"real", "imag", "abs", "auto"}
+    :param eig_constraints: Set containing desired DMD operator eigenvalue
+        constraints. Currently available constraints are `"stable"`, which
+        constrains eigenvalues to the left half of the complex plane,
+        `"imag"`, which constrains eigenvalues to the imaginary axis, and
+        `"conjugate_pairs"`, which enforces that eigenvalues are always
+        present with their complex conjugate. Note that constraints may be
+        combined if valid.
+    :type eig_constraints: set(str)
     :param varpro_opts_dict: Dictionary containing the desired parameter values
         for variable projection. The following parameters may be specified:
         `init_lambda`, `maxlam`, `lamup`, `use_levmarq`, `maxiter`, `tol`,
         `eps_stall`, `use_fulljac`, `verbose`. Default values will be used for
         any parameters not specified in `varpro_opts_dict`.
         See `BOPDMDOperator` documentation for default values and descriptions
         for each parameter.
@@ -776,14 +845,15 @@
         compute_A=False,
         use_proj=True,
         init_alpha=None,
         proj_basis=None,
         num_trials=0,
         trial_size=0.2,
         eig_sort="auto",
+        eig_constraints=None,
         varpro_opts_dict=None,
     ):
         self._svd_rank = svd_rank
         self._compute_A = compute_A
         self._use_proj = use_proj
         self._init_alpha = init_alpha
         self._proj_basis = proj_basis
@@ -794,14 +864,21 @@
         if varpro_opts_dict is None:
             self._varpro_opts_dict = {}
         elif not isinstance(varpro_opts_dict, dict):
             raise ValueError("varpro_opts_dict must be a dict.")
         else:
             self._varpro_opts_dict = varpro_opts_dict
 
+        if eig_constraints is None:
+            eig_constraints = set()
+        elif not isinstance(eig_constraints, set):
+            raise ValueError("eig_constraints must be a set.")
+        self._eig_constraints = eig_constraints
+        self._check_eig_constraints()
+
         self._snapshots_holder = None
         self._time = None
         self._Atilde = None
         self._modes_activation_bitmask_proxy = None
 
     @property
     def svd_rank(self):
@@ -940,14 +1017,24 @@
         Get the modes standard deviation.
 
         :return: modes standard deviation.
         :rtype: numpy.ndarray
         """
         return self.operator.modes_std
 
+    @property
+    def eig_constraints(self):
+        """
+        Get the eigenvalue constraints.
+
+        :return: eigenvalue constraints.
+        :rtype: set(str)
+        """
+        return self._eig_constraints
+
     def print_varpro_opts(self):
         """
         Prints a formatted information string that displays all chosen
         variable projection parameter values.
         """
         if self._Atilde is None:
             raise ValueError("You need to call fit before")
@@ -967,14 +1054,31 @@
         print("============================")
         for name, value in zip(opt_names, self.operator.varpro_opts):
             if len(name) < 7:
                 print(name + ":\t\t" + str(value))
             else:
                 print(name + ":\t" + str(value))
 
+    def _check_eig_constraints(self):
+        """
+        Function that verifies that the set self._eig_constraints (1) does
+        not contain an unsupported constraint class, and (2) does not contain
+        an invalid combination of eigenvalue constraints.
+        """
+        valid_constraints = {"stable", "imag", "conjugate_pairs"}
+        invalid_combos = [{"stable", "imag"}]
+
+        if len(self._eig_constraints.difference(valid_constraints)) != 0:
+            raise ValueError("Invalid eigenvalue constraint provided.")
+
+        for invalid_combo_set in invalid_combos:
+            if invalid_combo_set.issubset(self._eig_constraints):
+                msg = "Invalid eigenvalue constraint combination provided."
+                raise ValueError(msg)
+
     def _initialize_alpha(self):
         """
         Uses projected trapezoidal rule to approximate the eigenvalues of A in
             z' = Az.
         The computed eigenvalues will serve as our initial guess for alpha.
 
         :return: Approximated eigenvalues of the matrix A.
@@ -1062,14 +1166,15 @@
             self._compute_A,
             self._use_proj,
             self._init_alpha,
             self._proj_basis,
             self._num_trials,
             self._trial_size,
             self._eig_sort,
+            self._eig_constraints,
             **self._varpro_opts_dict
         )
 
         # Define the snapshots that will be used for fitting.
         if self._use_proj:
             snp = self._proj_basis.conj().T.dot(self.snapshots)
         else:
@@ -1079,15 +1184,15 @@
         self._b = self.operator.compute_operator(snp.T, self._time)
 
         return self
 
     def forecast(self, t):
         """
         Predict the output X given the input time t using the fitted DMD model.
-        If model has been fitted using multiple enssembles, an average
+        If model has been fitted using multiple ensembles, an average
         prediction and its variance is returned.
 
         :param t: the input time vector.
         :type t: numpy.ndarray or iterable
         :return: system prediction at times given by vector t.
         :rtype: numpy.ndarray or numpy.ndarray, numpy.ndarray
         """
```

### Comparing `pydmd-0.4.1.post2306/pydmd/cdmd.py` & `pydmd-0.4.1.post2308/pydmd/cdmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """
 Derived module from dmdbase.py for compressed dmd.
 As a reference consult this work by Erichson, Brunton and Kutz:
 https://doi.org/10.1007/s11554-016-0655-2
 """
-from __future__ import division
-
 import numpy as np
 import scipy.sparse
 from scipy.linalg import sqrtm
 
 from .dmdbase import DMDBase
 from .dmdoperator import DMDOperator
 from .snapshots import Snapshots
```

### Comparing `pydmd-0.4.1.post2306/pydmd/dmd.py` & `pydmd-0.4.1.post2308/pydmd/dmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/dmd_modes_tuner.py` & `pydmd-0.4.1.post2308/pydmd/dmd_modes_tuner.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/dmdbase.py` & `pydmd-0.4.1.post2308/pydmd/dmdbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """
 Base module for the DMD: `fit` method must be implemented in inherited classes
 """
-from __future__ import division
-
 import pickle
 from copy import copy, deepcopy
-from os.path import splitext
 
 import numpy as np
 
 from .dmdoperator import DMDOperator
 from .utils import compute_svd
```

### Comparing `pydmd-0.4.1.post2306/pydmd/dmdc.py` & `pydmd-0.4.1.post2308/pydmd/dmdc.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/dmdoperator.py` & `pydmd-0.4.1.post2308/pydmd/dmdoperator.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             atilde_back = self._least_square_operator(bU, bs, bV, X)
             atilde = sqrtm(atilde.dot(np.linalg.inv(atilde_back)))
             if hasattr(np, "complex256") and atilde.dtype == np.complex256:
                 atilde = atilde.astype(np.complex128)
                 msg = "Casting atilde from np.complex256 to np.complex128"
                 logging.info(msg)
 
-        if self._rescale_mode == "auto":
+        if isinstance(self._rescale_mode, str) and self._rescale_mode == "auto":
             self._rescale_mode = s
 
         self._Atilde = atilde
         self._compute_eigenquantities()
         self._compute_modes(Y, U, s, V)
 
         return U, s, V
```

### Comparing `pydmd-0.4.1.post2306/pydmd/fbdmd.py` & `pydmd-0.4.1.post2308/pydmd/fbdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/hankeldmd.py` & `pydmd-0.4.1.post2308/pydmd/hankeldmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/havok.py` & `pydmd-0.4.1.post2308/pydmd/havok.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/hodmd.py` & `pydmd-0.4.1.post2308/pydmd/hodmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/mrdmd.py` & `pydmd-0.4.1.post2308/pydmd/mrdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/optdmd.py` & `pydmd-0.4.1.post2308/pydmd/optdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/paramdmd.py` & `pydmd-0.4.1.post2308/pydmd/paramdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/pidmd.py` & `pydmd-0.4.1.post2308/pydmd/pidmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
     :param manifold: the matrix manifold to restrict the full operator A to.
         The following matrix manifolds are permissible:
         - "unitary"
         - "uppertriangular"
         - "lowertriangular"
         - "diagonal"
-        - "symmetric",
+        - "symmetric"
         - "skewsymmetric"
         - "toeplitz"
         - "hankel"
         - "circulant"
         - "circulant_unitary"
         - "circulant_symmetric"
         - "circulant_skewsymmetric"
```

### Comparing `pydmd-0.4.1.post2306/pydmd/pidmd_utils.py` & `pydmd-0.4.1.post2308/pydmd/pidmd_utils.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/plotter.py` & `pydmd-0.4.1.post2308/pydmd/plotter.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/rdmd.py` & `pydmd-0.4.1.post2308/pydmd/rdmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 from .utils import compute_rank
 
 
 class RDMD(CDMD):
     """
     Randomized Dynamic Mode Decomposition
 
-    :param rand_mat: The random test matrix that will be used when executing
+    :param test_matrix: The random test matrix that will be used when executing
         the Randomized QB Decomposition. If not provided, the `svd_rank` and
         `oversampling` parameters will be used to compute the random matrix.
-    :type rand_mat: numpy.ndarray
+    :type test_matrix: numpy.ndarray
     :param oversampling: Number of additional samples (beyond the desired rank)
         to use when computing the random test matrix. Note that values {5,10}
         tend to be sufficient.
     :type oversampling: int
     :param power_iters: Number of power iterations to perform when executing
         the Randomized QB Decomposition. Note that values {1,2} often lead to
         considerable improvements.
     :type power_iters: int
     """
 
     def __init__(
         self,
-        rand_mat=None,
+        test_matrix=None,
         oversampling=10,
         power_iters=2,
         svd_rank=0,
         tlsq_rank=0,
         opt=False,
         rescale_mode=None,
         forward_backward=False,
@@ -53,33 +53,33 @@
             forward_backward=forward_backward,
             sorted_eigs=sorted_eigs,
             tikhonov_regularization=tikhonov_regularization,
         )
         self._svd_rank = svd_rank
         self._oversampling = oversampling
         self._power_iters = power_iters
-        self._rand_mat = rand_mat
+        self._test_matrix = test_matrix
 
     def _compress_snapshots(self):
         """
         Private method that compresses the snapshot matrix X by projecting X
         onto a near-optimal orthonormal basis for the range of X computed via
         the Randomized QB Decomposition.
 
         :return: the compressed snapshots
         :rtype: numpy.ndarray
         """
         # Define the random test matrix if not provided.
-        if self._rand_mat is None:
+        if self._test_matrix is None:
             m = self.snapshots.shape[-1]
             r = compute_rank(self.snapshots, self._svd_rank)
-            self._rand_mat = np.random.randn(m, r + self._oversampling)
+            self._test_matrix = np.random.randn(m, r + self._oversampling)
 
         # Compute sampling matrix.
-        Y = self.snapshots.dot(self._rand_mat)
+        Y = self.snapshots.dot(self._test_matrix)
 
         # Perform power iterations.
         for _ in range(self._power_iters):
             Q = np.linalg.qr(Y)[0]
             Z = np.linalg.qr(self.snapshots.conj().T.dot(Q))[0]
             Y = self.snapshots.dot(Z)
```

### Comparing `pydmd-0.4.1.post2306/pydmd/snapshots.py` & `pydmd-0.4.1.post2308/pydmd/snapshots.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/spdmd.py` & `pydmd-0.4.1.post2308/pydmd/spdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/subspacedmd.py` & `pydmd-0.4.1.post2308/pydmd/subspacedmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd/utils.py` & `pydmd-0.4.1.post2308/pydmd/utils.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/pydmd.egg-info/PKG-INFO` & `pydmd-0.4.1.post2308/pydmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmd
-Version: 0.4.1.post2306
+Version: 0.4.1.post2308
 Summary: Python Dynamic Mode Decomposition.
 Home-page: https://github.com/mathLab/PyDMD
 Author: Nicola Demo, Marco Tezzele, Francesco Andreuzzi, Sara Ichinaga
 Author-email: pydmd.info@gmail.com
 License: MIT
 Keywords: dynamic-mode-decomposition dmd
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pydmd-0.4.1.post2306/pydmd.egg-info/SOURCES.txt` & `pydmd-0.4.1.post2308/pydmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/setup.py` & `pydmd-0.4.1.post2308/setup.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_bopdmd.py` & `pydmd-0.4.1.post2308/tests/test_bopdmd.py`

 * *Files 17% similar despite different names*

```diff
@@ -177,7 +177,67 @@
     np.testing.assert_allclose(bopdmd_with_A.A, expected_A)
     with raises(ValueError):
         print(bopdmd_no_A.A)
 
     np.testing.assert_array_equal(bopdmd_with_A.atilde, bopdmd_no_A.atilde)
     np.testing.assert_array_equal(bopdmd_with_A.modes, bopdmd_no_A.modes)
     np.testing.assert_array_equal(bopdmd_with_A.eigs, bopdmd_no_A.eigs)
+
+
+def test_eig_constraints_errors():
+    """
+    Tests that the BOPDMD module correctly throws an error upon initialization
+    in each of the following cases:
+    - eig_constraints is a string rather than a set of strings
+    - eig_constraints contains an invalid constraint argument
+        (either alone or along with another constraint argument)
+    - eig_constraints contains the invalid combination "stable"+"imag"
+        (either alone or along with the extra argument "conjugate_pairs")
+    """
+    with raises(ValueError):
+        BOPDMD(eig_constraints="stable")
+
+    with raises(ValueError):
+        BOPDMD(eig_constraints={"stablee"})
+
+    with raises(ValueError):
+        BOPDMD(eig_constraints={"stablee", "imag"})
+
+    with raises(ValueError):
+        BOPDMD(eig_constraints={"stable", "imag"})
+
+    with raises(ValueError):
+        BOPDMD(eig_constraints={"stable", "imag", "conjugate_pairs"})
+
+
+def test_eig_constraints():
+    """
+    Tests that the BOPDMD module correctly enforces that eigenvalues...
+    - lie in the left half plane when eig_constraints contains "stable".
+    - lie on the imaginary axis when eig_constraints contains "imag".
+    - are present with their complex conjugate when eig_constraints
+        contains "conjugate_pairs".
+    Eigenvalue constraint combinations are also tested.
+    """
+    bopdmd = BOPDMD(svd_rank=2, eig_constraints={"stable"})
+    bopdmd.fit(Z, t)
+    assert np.all(bopdmd.eigs.real <= 0.0)
+
+    bopdmd = BOPDMD(svd_rank=2, eig_constraints={"imag"})
+    bopdmd.fit(Z, t)
+    assert np.all(bopdmd.eigs.real == 0.0)
+
+    bopdmd = BOPDMD(svd_rank=2, eig_constraints={"conjugate_pairs"})
+    bopdmd.fit(Z, t)
+    assert bopdmd.eigs[0].real == bopdmd.eigs[1].real
+    assert bopdmd.eigs[0].imag == -bopdmd.eigs[1].imag
+
+    bopdmd = BOPDMD(svd_rank=2, eig_constraints={"stable", "conjugate_pairs"})
+    bopdmd.fit(Z, t)
+    assert np.all(bopdmd.eigs.real <= 0.0)
+    assert bopdmd.eigs[0].real == bopdmd.eigs[1].real
+    assert bopdmd.eigs[0].imag == -bopdmd.eigs[1].imag
+
+    bopdmd = BOPDMD(svd_rank=2, eig_constraints={"imag", "conjugate_pairs"})
+    bopdmd.fit(Z, t)
+    assert np.all(bopdmd.eigs.real == 0.0)
+    assert bopdmd.eigs[0].imag == -bopdmd.eigs[1].imag
```

### Comparing `pydmd-0.4.1.post2306/tests/test_cdmd.py` & `pydmd-0.4.1.post2308/tests/test_cdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_dmd.py` & `pydmd-0.4.1.post2308/tests/test_dmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,15 @@
             [-7.29383297e00 - 4.90248179e-14j],
             [-5.69109796e00 - 2.74068833e00j],
             [3.38410649e-83 + 3.75677740e-83j],
         ]
     )
     np.testing.assert_almost_equal(dmd.dynamics, expected_data, decimal=6)
 
+
 def test_dmd_time_5():
     """
     Let us check that the timestep is actually reduced and not rounded to
     the closest integer.
     """
     dmd = DMD(svd_rank=3)
     dmd.fit(X=sample_data)
```

### Comparing `pydmd-0.4.1.post2306/tests/test_dmd_modes_tuner.py` & `pydmd-0.4.1.post2308/tests/test_dmd_modes_tuner.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_dmdbase.py` & `pydmd-0.4.1.post2308/tests/test_dmdbase.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_dmdc.py` & `pydmd-0.4.1.post2308/tests/test_dmdc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import division
-
 import numpy as np
 import scipy
 from pytest import raises
 
 from pydmd import DMDc
```

### Comparing `pydmd-0.4.1.post2306/tests/test_dmdoperator.py` & `pydmd-0.4.1.post2308/tests/test_dmdoperator.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_fbdmd.py` & `pydmd-0.4.1.post2308/tests/test_fbdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_hankeldmd.py` & `pydmd-0.4.1.post2308/tests/test_hankeldmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_havok.py` & `pydmd-0.4.1.post2308/tests/test_havok.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_hodmd.py` & `pydmd-0.4.1.post2308/tests/test_hodmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_mrdmd.py` & `pydmd-0.4.1.post2308/tests/test_mrdmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import division
-
 import numpy as np
 from pytest import raises
 
 from pydmd import DMD, FbDMD
 from pydmd.mrdmd import MrDMD
```

### Comparing `pydmd-0.4.1.post2306/tests/test_optdmd.py` & `pydmd-0.4.1.post2308/tests/test_optdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_paramdmd.py` & `pydmd-0.4.1.post2308/tests/test_paramdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_pidmd.py` & `pydmd-0.4.1.post2308/tests/test_pidmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_plotter.py` & `pydmd-0.4.1.post2308/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_rdmd.py` & `pydmd-0.4.1.post2308/tests/test_rdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_snapshots.py` & `pydmd-0.4.1.post2308/tests/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_spdmd.py` & `pydmd-0.4.1.post2308/tests/test_spdmd.py`

 * *Files identical despite different names*

### Comparing `pydmd-0.4.1.post2306/tests/test_subspacedmd.py` & `pydmd-0.4.1.post2308/tests/test_subspacedmd.py`

 * *Files identical despite different names*

