# Comparing `tmp/katsdpsigproc-1.7.0.tar.gz` & `tmp/katsdpsigproc-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katsdpsigproc-1.7.0.tar", last modified: Thu Jun  1 10:49:34 2023, max compression
+gzip compressed data, was "katsdpsigproc-1.8.0.tar", last modified: Tue Aug  1 14:32:14 2023, max compression
```

## Comparing `katsdpsigproc-1.7.0.tar` & `katsdpsigproc-1.8.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      248 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/.flake8
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      109 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/.gitignore
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      425 2023-06-01 05:51:40.000000 katsdpsigproc-1.7.0/.pre-commit-config.yaml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       81 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/.pydocstyle
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      127 2021-03-23 08:09:24.000000 katsdpsigproc-1.7.0/.readthedocs.yml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      213 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/Jenkinsfile
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1527 2023-05-18 09:40:34.000000 katsdpsigproc-1.7.0/LICENSE
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      746 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/PKG-INFO
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      166 2022-11-03 10:07:08.000000 katsdpsigproc-1.7.0/README.md
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.474352 katsdpsigproc-1.7.0/doc/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        7 2015-12-01 10:48:07.000000 katsdpsigproc-1.7.0/doc/.gitignore
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6790 2020-05-13 08:54:56.000000 katsdpsigproc-1.7.0/doc/Makefile
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.474352 katsdpsigproc-1.7.0/doc/_static/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2014-11-27 07:59:41.000000 katsdpsigproc-1.7.0/doc/_static/.keep
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.474352 katsdpsigproc-1.7.0/doc/_templates/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2014-11-27 07:59:41.000000 katsdpsigproc-1.7.0/doc/_templates/.keep
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2796 2023-06-01 10:49:00.000000 katsdpsigproc-1.7.0/doc/changelog.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    12220 2022-11-08 09:40:15.000000 katsdpsigproc-1.7.0/doc/conf.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      504 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/index.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2636 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/installation.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      388 2021-09-23 14:40:29.000000 katsdpsigproc-1.7.0/doc/katsdpsigproc.asyncio.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      680 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/doc/katsdpsigproc.rfi.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2266 2022-09-14 13:17:57.000000 katsdpsigproc-1.7.0/doc/katsdpsigproc.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      378 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/doc/katsdpsigproc.test.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6715 2014-11-27 07:59:41.000000 katsdpsigproc-1.7.0/doc/make.bat
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.478352 katsdpsigproc-1.7.0/doc/user/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     9721 2022-11-01 10:36:53.000000 katsdpsigproc-1.7.0/doc/user/autotune.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4369 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/buffers.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1491 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/builtin-ops.rst
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.478352 katsdpsigproc-1.7.0/doc/user/examples/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      849 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/fill_reduce.dot
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1294 2020-06-12 09:09:15.000000 katsdpsigproc-1.7.0/doc/user/examples/fill_reduce.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)      203 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/hello_accel.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      249 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/set_ones.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      497 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/sum.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1676 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/sum.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1554 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/doc/user/examples/test_triple.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      673 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/triple.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1171 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/triple_op.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1452 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/triple_op_template.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      693 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/triple_templ.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2131 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/examples/triple_tune.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      658 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/index.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1766 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/init.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1442 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/intro.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4966 2023-06-01 05:51:40.000000 katsdpsigproc-1.7.0/doc/user/kernels.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     8516 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/macros.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    12438 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/operations.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5327 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/resource.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2823 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/sync.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5881 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/doc/user/testing.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1561 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/threads.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      433 2020-05-26 10:30:52.000000 katsdpsigproc-1.7.0/doc/user/undocumented.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      160 2021-11-25 10:54:14.000000 katsdpsigproc-1.7.0/doc-requirements.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      219 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/mypy.ini
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       82 2022-09-19 11:57:04.000000 katsdpsigproc-1.7.0/pyproject.toml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      317 2022-11-18 06:52:35.000000 katsdpsigproc-1.7.0/pytest.ini
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      211 2023-06-01 05:51:40.000000 katsdpsigproc-1.7.0/requirements.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      385 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/rtd-requirements.txt
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.478352 katsdpsigproc-1.7.0/scripts/
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     1679 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/scripts/maskedsumabstest.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     1638 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/scripts/maskedsumtest.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     1594 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/scripts/percentiletest.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     7738 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/scripts/rfiflagtest.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)      539 2020-02-25 09:42:58.000000 katsdpsigproc-1.7.0/scripts/transposetest.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1088 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/setup.cfg
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      842 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/setup.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.474352 katsdpsigproc-1.7.0/src/
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.482352 katsdpsigproc-1.7.0/src/katsdpsigproc/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      125 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/src/katsdpsigproc/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14361 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/abc.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    68521 2023-06-01 05:51:40.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/accel.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.482352 katsdpsigproc-1.7.0/src/katsdpsigproc/asyncio/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      869 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/src/katsdpsigproc/asyncio/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1023 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/asyncio/resource.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    17303 2023-05-19 08:35:41.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/cuda.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    16294 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/fft.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1195 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/fill.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4633 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/fill.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2802 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/hreduce.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2495 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/maskedsum.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5440 2023-05-19 08:11:58.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/maskedsum.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    20365 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/opencl.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4692 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/percentile.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7603 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/percentile.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3214 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/port.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/py.typed
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5005 2022-09-19 11:57:04.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/pytest_plugin.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     8562 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rank.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6248 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/reduce.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     9047 2022-11-28 09:25:10.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/resource.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.482352 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1636 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7238 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/background_median_filter.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    43105 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/device.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     9254 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/host.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4069 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/madnz.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2940 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/madnz_t.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1478 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/threshold_simple.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1528 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/threshold_simple_t.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4286 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/threshold_sum.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    43676 2023-05-19 11:32:19.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/twodflag.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.482352 katsdpsigproc-1.7.0/src/katsdpsigproc/test/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       59 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/src/katsdpsigproc/test/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4093 2022-09-19 11:57:04.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/test/test_accel.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2872 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/transpose.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5625 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/transpose.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4602 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/transpose_base.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    15752 2023-05-18 09:40:39.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/tune.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7389 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/src/katsdpsigproc/wg_reduce.mako
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.482352 katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      746 2023-06-01 10:49:34.000000 katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/PKG-INFO
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3244 2023-06-01 10:49:34.000000 katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/SOURCES.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2023-06-01 10:49:34.000000 katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/dependency_links.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2022-09-13 13:43:42.000000 katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/not-zip-safe
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      275 2023-06-01 10:49:34.000000 katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/requires.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       14 2023-06-01 10:49:34.000000 katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/top_level.txt
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/test/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1400 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      810 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/conftest.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-06-01 10:49:34.486352 katsdpsigproc-1.7.0/test/rfi/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      808 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/rfi/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3919 2022-11-18 06:52:35.000000 katsdpsigproc-1.7.0/test/rfi/test_background.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5311 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/rfi/test_flagger.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2357 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/rfi/test_median_non_zero.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2985 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/rfi/test_noise_est.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3482 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/rfi/test_threshold.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    26433 2022-11-18 06:52:35.000000 katsdpsigproc-1.7.0/test/rfi/test_twodflag.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    30223 2022-11-18 06:52:35.000000 katsdpsigproc-1.7.0/test/test_accel.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     9282 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/test_fft.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2221 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/test_fill.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2980 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/test_maskedsum.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3678 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/test_percentile.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3230 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/test/test_rank.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6846 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/test_rank.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1060 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/test/test_reduce.mako
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3984 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/test_reduce.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7749 2022-11-18 06:52:35.000000 katsdpsigproc-1.7.0/test/test_resource.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2559 2022-09-19 11:17:05.000000 katsdpsigproc-1.7.0/test/test_transpose.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7795 2023-05-18 09:40:39.000000 katsdpsigproc-1.7.0/test/test_tune.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      174 2022-09-15 14:02:50.000000 katsdpsigproc-1.7.0/test-requirements.txt
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      248 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/.flake8
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      109 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/.gitignore
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      425 2023-06-01 05:51:40.000000 katsdpsigproc-1.8.0/.pre-commit-config.yaml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       81 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/.pydocstyle
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      127 2021-03-23 08:09:24.000000 katsdpsigproc-1.8.0/.readthedocs.yml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      213 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/Jenkinsfile
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1527 2023-05-18 09:40:34.000000 katsdpsigproc-1.8.0/LICENSE
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      746 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/PKG-INFO
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      166 2022-11-03 10:07:08.000000 katsdpsigproc-1.8.0/README.md
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.004507 katsdpsigproc-1.8.0/doc/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        7 2015-12-01 10:48:07.000000 katsdpsigproc-1.8.0/doc/.gitignore
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6790 2020-05-13 08:54:56.000000 katsdpsigproc-1.8.0/doc/Makefile
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.004507 katsdpsigproc-1.8.0/doc/_static/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2014-11-27 07:59:41.000000 katsdpsigproc-1.8.0/doc/_static/.keep
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.004507 katsdpsigproc-1.8.0/doc/_templates/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2014-11-27 07:59:41.000000 katsdpsigproc-1.8.0/doc/_templates/.keep
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2992 2023-08-01 14:30:31.000000 katsdpsigproc-1.8.0/doc/changelog.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    12220 2022-11-08 09:40:15.000000 katsdpsigproc-1.8.0/doc/conf.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      504 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/index.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2636 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/installation.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      388 2021-09-23 14:40:29.000000 katsdpsigproc-1.8.0/doc/katsdpsigproc.asyncio.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      680 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/doc/katsdpsigproc.rfi.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2266 2022-09-14 13:17:57.000000 katsdpsigproc-1.8.0/doc/katsdpsigproc.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      378 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/doc/katsdpsigproc.test.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6715 2014-11-27 07:59:41.000000 katsdpsigproc-1.8.0/doc/make.bat
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.004507 katsdpsigproc-1.8.0/doc/user/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     9859 2023-08-01 14:25:25.000000 katsdpsigproc-1.8.0/doc/user/autotune.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4369 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/buffers.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1491 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/builtin-ops.rst
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.004507 katsdpsigproc-1.8.0/doc/user/examples/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      849 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/fill_reduce.dot
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1294 2020-06-12 09:09:15.000000 katsdpsigproc-1.8.0/doc/user/examples/fill_reduce.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)      203 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/hello_accel.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      249 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/set_ones.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      497 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/sum.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1676 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/sum.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1554 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/doc/user/examples/test_triple.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      673 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/triple.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1171 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/triple_op.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1452 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/triple_op_template.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      693 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/triple_templ.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2131 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/examples/triple_tune.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      658 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/index.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1766 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/init.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1442 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/intro.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4966 2023-06-01 05:51:40.000000 katsdpsigproc-1.8.0/doc/user/kernels.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     8516 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/macros.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    12438 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/operations.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5327 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/resource.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2823 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/sync.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5881 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/doc/user/testing.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1561 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/threads.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      433 2020-05-26 10:30:52.000000 katsdpsigproc-1.8.0/doc/user/undocumented.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      160 2021-11-25 10:54:14.000000 katsdpsigproc-1.8.0/doc-requirements.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      219 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/mypy.ini
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       82 2022-09-19 11:57:04.000000 katsdpsigproc-1.8.0/pyproject.toml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      317 2022-11-18 06:52:35.000000 katsdpsigproc-1.8.0/pytest.ini
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      211 2023-08-01 11:27:04.000000 katsdpsigproc-1.8.0/requirements.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      405 2023-08-01 11:27:04.000000 katsdpsigproc-1.8.0/rtd-requirements.txt
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.004507 katsdpsigproc-1.8.0/scripts/
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     1679 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/scripts/maskedsumabstest.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     1638 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/scripts/maskedsumtest.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     1594 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/scripts/percentiletest.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     7738 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/scripts/rfiflagtest.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)      539 2020-02-25 09:42:58.000000 katsdpsigproc-1.8.0/scripts/transposetest.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1088 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/setup.cfg
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      842 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/setup.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.000507 katsdpsigproc-1.8.0/src/
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.008507 katsdpsigproc-1.8.0/src/katsdpsigproc/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      125 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/src/katsdpsigproc/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14361 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/abc.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    68521 2023-08-01 11:27:04.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/accel.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.008507 katsdpsigproc-1.8.0/src/katsdpsigproc/asyncio/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      869 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/src/katsdpsigproc/asyncio/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1023 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/asyncio/resource.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    17303 2023-05-19 08:35:41.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/cuda.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    16294 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/fft.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1195 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/fill.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4633 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/fill.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2802 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/hreduce.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2495 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/maskedsum.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5440 2023-05-19 08:11:58.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/maskedsum.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    20365 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/opencl.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4692 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/percentile.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7603 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/percentile.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3214 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/port.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/py.typed
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5005 2022-09-19 11:57:04.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/pytest_plugin.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     8562 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rank.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6248 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/reduce.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     9047 2022-11-28 09:25:10.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/resource.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1636 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7238 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/background_median_filter.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    43105 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/device.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     9254 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/host.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4069 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/madnz.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2940 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/madnz_t.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1478 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/threshold_simple.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1528 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/threshold_simple_t.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4286 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/threshold_sum.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    43596 2023-08-01 14:25:25.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/twodflag.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/src/katsdpsigproc/test/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       59 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/src/katsdpsigproc/test/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4093 2022-09-19 11:57:04.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/test/test_accel.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2872 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/transpose.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5625 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/transpose.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4602 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/transpose_base.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    15673 2023-08-01 14:25:25.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/tune.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7389 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/src/katsdpsigproc/wg_reduce.mako
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.008507 katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      746 2023-08-01 14:32:13.000000 katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/PKG-INFO
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3244 2023-08-01 14:32:13.000000 katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/SOURCES.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2023-08-01 14:32:13.000000 katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/dependency_links.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2022-09-13 13:43:42.000000 katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/not-zip-safe
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      275 2023-08-01 14:32:13.000000 katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/requires.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       14 2023-08-01 14:32:13.000000 katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/top_level.txt
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/test/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1400 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      810 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/conftest.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-08-01 14:32:14.012507 katsdpsigproc-1.8.0/test/rfi/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      808 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/rfi/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3919 2022-11-18 06:52:35.000000 katsdpsigproc-1.8.0/test/rfi/test_background.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5311 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/rfi/test_flagger.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2357 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/rfi/test_median_non_zero.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2985 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/rfi/test_noise_est.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3482 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/rfi/test_threshold.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    26433 2022-11-18 06:52:35.000000 katsdpsigproc-1.8.0/test/rfi/test_twodflag.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    30223 2022-11-18 06:52:35.000000 katsdpsigproc-1.8.0/test/test_accel.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     9282 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/test_fft.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2221 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/test_fill.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2980 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/test_maskedsum.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3678 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/test_percentile.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3230 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/test/test_rank.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6846 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/test_rank.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1060 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/test/test_reduce.mako
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3984 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/test_reduce.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7749 2022-11-18 06:52:35.000000 katsdpsigproc-1.8.0/test/test_resource.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2559 2022-09-19 11:17:05.000000 katsdpsigproc-1.8.0/test/test_transpose.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     7795 2023-05-18 09:40:39.000000 katsdpsigproc-1.8.0/test/test_tune.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      174 2022-09-15 14:02:50.000000 katsdpsigproc-1.8.0/test-requirements.txt
```

### Comparing `katsdpsigproc-1.7.0/LICENSE` & `katsdpsigproc-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/PKG-INFO` & `katsdpsigproc-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katsdpsigproc
-Version: 1.7.0
+Version: 1.8.0
 Summary: Karoo Array Telescope accelerated signal processing tools
 Home-page: https://katsdpsigproc.readthedocs.io/
 Author: MeerKAT SDP team
 Author-email: sdpdev+katsdpsigproc@sarao.ac.za
 License: Modified BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `katsdpsigproc-1.7.0/doc/Makefile` & `katsdpsigproc-1.8.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/changelog.rst` & `katsdpsigproc-1.8.0/doc/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+.. rubric:: 1.8.0
+
+- Add :envvar:`KATSDPSIGPROC_TUNE_DB` environment variable to override the
+  location of the tuning database.
+- Remove use of deprecated :func:`numba.generated_jit` decorator.
+
 .. rubric:: 1.7.0
 
 - Add :meth:`.Operation.ensure_bound`.
 - Remove dependency on deprecated :mod:`pkg_resources` and use
   :mod:`importlib.resources` instead.
 - Fix :func:`.autotuner` decorator for autotune functions with no parameters.
 - Update type annotations to allow :class:`os.PathLike` in the `extra_dirs`
```

### Comparing `katsdpsigproc-1.7.0/doc/conf.py` & `katsdpsigproc-1.8.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/installation.rst` & `katsdpsigproc-1.8.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/katsdpsigproc.rfi.rst` & `katsdpsigproc-1.8.0/doc/katsdpsigproc.rfi.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/katsdpsigproc.rst` & `katsdpsigproc-1.8.0/doc/katsdpsigproc.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/make.bat` & `katsdpsigproc-1.8.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/autotune.rst` & `katsdpsigproc-1.8.0/doc/user/autotune.rst`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,17 @@
 setting an environment variable, :envvar:`KATSDPSIGPROC_TUNE_MATCH`. If
 :envvar:`KATSDPSIGPROC_TUNE_MATCH` is set to "nearest", the nearest match to the
 current GPU in the autotuning SQL table will be returned, by ignoring in turn
 the device driver, then platform, then device name. If no match is found,
 autotuning will proceed. If `KATSDPSIGPROC_TUNE_MATCH` is set to "exact" (or
 anything else), default behaviour will proceed.
 
+It is also possible to override the location of the tuning database by
+setting the environment variable :envvar:`KATSDPSIGPROC_TUNE_DB`.
+
 .. _autotune-testing:
 
 Testing
 -------
 The testing in general is addressed in :doc:`testing`, but it is worth noting
 that autotuning causes some additional challenges in testing:
```

### Comparing `katsdpsigproc-1.7.0/doc/user/buffers.rst` & `katsdpsigproc-1.8.0/doc/user/buffers.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/builtin-ops.rst` & `katsdpsigproc-1.8.0/doc/user/builtin-ops.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/fill_reduce.dot` & `katsdpsigproc-1.8.0/doc/user/examples/fill_reduce.dot`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/fill_reduce.py` & `katsdpsigproc-1.8.0/doc/user/examples/fill_reduce.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/sum.py` & `katsdpsigproc-1.8.0/doc/user/examples/sum.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/test_triple.py` & `katsdpsigproc-1.8.0/doc/user/examples/test_triple.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/triple.py` & `katsdpsigproc-1.8.0/doc/user/examples/triple.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/triple_op.py` & `katsdpsigproc-1.8.0/doc/user/examples/triple_op.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/triple_op_template.py` & `katsdpsigproc-1.8.0/doc/user/examples/triple_op_template.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/triple_templ.py` & `katsdpsigproc-1.8.0/doc/user/examples/triple_templ.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/examples/triple_tune.py` & `katsdpsigproc-1.8.0/doc/user/examples/triple_tune.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/index.rst` & `katsdpsigproc-1.8.0/doc/user/index.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/init.rst` & `katsdpsigproc-1.8.0/doc/user/init.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/intro.rst` & `katsdpsigproc-1.8.0/doc/user/intro.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/kernels.rst` & `katsdpsigproc-1.8.0/doc/user/kernels.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/macros.rst` & `katsdpsigproc-1.8.0/doc/user/macros.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/operations.rst` & `katsdpsigproc-1.8.0/doc/user/operations.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/resource.rst` & `katsdpsigproc-1.8.0/doc/user/resource.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/sync.rst` & `katsdpsigproc-1.8.0/doc/user/sync.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/testing.rst` & `katsdpsigproc-1.8.0/doc/user/testing.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/doc/user/threads.rst` & `katsdpsigproc-1.8.0/doc/user/threads.rst`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/scripts/maskedsumabstest.py` & `katsdpsigproc-1.8.0/scripts/maskedsumabstest.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/scripts/maskedsumtest.py` & `katsdpsigproc-1.8.0/scripts/maskedsumtest.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/scripts/percentiletest.py` & `katsdpsigproc-1.8.0/scripts/percentiletest.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/scripts/rfiflagtest.py` & `katsdpsigproc-1.8.0/scripts/rfiflagtest.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/scripts/transposetest.py` & `katsdpsigproc-1.8.0/scripts/transposetest.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/setup.cfg` & `katsdpsigproc-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/setup.py` & `katsdpsigproc-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/abc.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/abc.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/accel.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/accel.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/asyncio/__init__.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/asyncio/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ################################################################################
 
 """Utilities for working with :mod:`asyncio`."""
 
 # Automatically added by katversion
-__version__ = '1.7.0'
+__version__ = '1.8.0'
```

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/asyncio/resource.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/asyncio/resource.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/cuda.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/cuda.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/fft.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/fft.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/fill.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/fill.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/fill.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/fill.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/hreduce.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/hreduce.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/maskedsum.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/maskedsum.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/maskedsum.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/maskedsum.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/opencl.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/opencl.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/percentile.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/percentile.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/percentile.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/percentile.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/port.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/port.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/pytest_plugin.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rank.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rank.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/reduce.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/reduce.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/resource.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/resource.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/__init__.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 MAD_NORMAL = 1.4826
 """Ratio between `median absolute deviation`_ and standard deviation of a Gaussian distribution.
 
 .. _median absolute deviation: https://en.wikipedia.org/wiki/Median_absolute_deviation
 """
 
 # Automatically added by katversion
-__version__ = '1.7.0'
+__version__ = '1.8.0'
```

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/background_median_filter.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/background_median_filter.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/device.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/device.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/host.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/host.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/madnz.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/madnz.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/madnz_t.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/madnz_t.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/threshold_simple.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/threshold_simple.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/threshold_simple_t.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/threshold_simple_t.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/threshold_sum.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/threshold_sum.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/rfi/twodflag.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/rfi/twodflag.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,29 @@
     elif value >= 0 and value < 2**32:
         dtype = np.uint32
     else:
         dtype = np.int64
     return np.array(value, dtype)
 
 
-@numba.generated_jit(nopython=True, nogil=True)
 def _asbool(data):
     """Create a boolean array with the same values as `data`.
 
-    The `data` contain only 0's and 1's. If possible, a view is returned,
+    The `data` must contain only 0's and 1's. If possible, a view is returned,
     otherwise a copy.
     """
-    if isinstance(data, np.ndarray):
-        # We're being called as a regular function due to NUMBA_DISABLE_JIT.
-        if data.dtype.itemsize == 1:
-            return data.view(np.bool_)
-        else:
-            return data.astype(np.bool_)
-    elif (isinstance(data.dtype, numba.types.Boolean)
+    if data.dtype.itemsize == 1:
+        return data.view(np.bool_)
+    else:
+        return data.astype(np.bool_)
+
+
+@numba.extending.overload(_asbool, jit_options=dict(nogil=True))
+def _overload_asbool(data):
+    if (isinstance(data.dtype, numba.types.Boolean)
             or (isinstance(data.dtype, numba.types.Integer) and data.dtype.bitwidth == 8)):
         return lambda data: data.view(np.bool_)
     else:
         return lambda data: data.astype(np.bool_)
 
 
 @numba.jit(nopython=True, nogil=True)
```

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/test/test_accel.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/test/test_accel.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/transpose.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/transpose.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/transpose.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/transpose.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/transpose_base.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/transpose_base.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/tune.py` & `katsdpsigproc-1.8.0/src/katsdpsigproc/tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,25 +230,20 @@
     # Start transaction
     with conn:
         cursor = conn.cursor()
         cursor.execute(command, list(entries.values()))
 
 
 def _open_db() -> sqlite3.Connection:
-    cache_dir = appdirs.user_cache_dir("katsdpsigproc", "ska-sa")
-    try:
-        os.makedirs(cache_dir)
-    except OSError:
-        # This happens if the directory already exists. If we failed
-        # to create it, the database open will fail.
-        pass
-
-    cache_file = os.path.join(cache_dir, "tuning.db")
-    conn = sqlite3.connect(cache_file)
-    return conn
+    cache_file = os.getenv("KATSDPSIGPROC_TUNE_DB")
+    if cache_file is None:
+        cache_dir = appdirs.user_cache_dir("katsdpsigproc", "ska-sa")
+        os.makedirs(cache_dir, exist_ok=True)
+        cache_file = os.path.join(cache_dir, "tuning.db")
+    return sqlite3.connect(cache_file)
 
 
 def _close_db(conn: sqlite3.Connection) -> None:
     """Close a database.
 
     This is split into a separate function for the benefit of testing, because
     the close member of the object itself is read-only and hence cannot be
```

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc/wg_reduce.mako` & `katsdpsigproc-1.8.0/src/katsdpsigproc/wg_reduce.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/PKG-INFO` & `katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katsdpsigproc
-Version: 1.7.0
+Version: 1.8.0
 Summary: Karoo Array Telescope accelerated signal processing tools
 Home-page: https://katsdpsigproc.readthedocs.io/
 Author: MeerKAT SDP team
 Author-email: sdpdev+katsdpsigproc@sarao.ac.za
 License: Modified BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `katsdpsigproc-1.7.0/src/katsdpsigproc.egg-info/SOURCES.txt` & `katsdpsigproc-1.8.0/src/katsdpsigproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/__init__.py` & `katsdpsigproc-1.8.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/conftest.py` & `katsdpsigproc-1.8.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/rfi/__init__.py` & `katsdpsigproc-1.8.0/test/rfi/__init__.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/rfi/test_background.py` & `katsdpsigproc-1.8.0/test/rfi/test_background.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/rfi/test_flagger.py` & `katsdpsigproc-1.8.0/test/rfi/test_flagger.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/rfi/test_median_non_zero.mako` & `katsdpsigproc-1.8.0/test/rfi/test_median_non_zero.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/rfi/test_noise_est.py` & `katsdpsigproc-1.8.0/test/rfi/test_noise_est.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/rfi/test_threshold.py` & `katsdpsigproc-1.8.0/test/rfi/test_threshold.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/rfi/test_twodflag.py` & `katsdpsigproc-1.8.0/test/rfi/test_twodflag.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_accel.py` & `katsdpsigproc-1.8.0/test/test_accel.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_fft.py` & `katsdpsigproc-1.8.0/test/test_fft.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_fill.py` & `katsdpsigproc-1.8.0/test/test_fill.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_maskedsum.py` & `katsdpsigproc-1.8.0/test/test_maskedsum.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_percentile.py` & `katsdpsigproc-1.8.0/test/test_percentile.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_rank.mako` & `katsdpsigproc-1.8.0/test/test_rank.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_rank.py` & `katsdpsigproc-1.8.0/test/test_rank.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_reduce.mako` & `katsdpsigproc-1.8.0/test/test_reduce.mako`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_reduce.py` & `katsdpsigproc-1.8.0/test/test_reduce.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_resource.py` & `katsdpsigproc-1.8.0/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_transpose.py` & `katsdpsigproc-1.8.0/test/test_transpose.py`

 * *Files identical despite different names*

### Comparing `katsdpsigproc-1.7.0/test/test_tune.py` & `katsdpsigproc-1.8.0/test/test_tune.py`

 * *Files identical despite different names*

