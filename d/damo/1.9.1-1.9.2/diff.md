# Comparing `tmp/damo-1.9.1.tar.gz` & `tmp/damo-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.9.1.tar", last modified: Mon Jul 24 17:11:40 2023, max compression
+gzip compressed data, was "damo-1.9.2.tar", last modified: Tue Aug  1 00:43:31 2023, max compression
```

## Comparing `damo-1.9.1.tar` & `damo-1.9.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:40.033988 damo-1.9.1/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-24 17:11:40.033988 damo-1.9.1/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-07-24 17:11:35.000000 damo-1.9.1/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.9.1/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-07-24 17:11:40.033988 damo-1.9.1/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.9.1/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:40.017989 damo-1.9.1/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:40.033988 damo-1.9.1/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:35.000000 damo-1.9.1/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.9.1/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9825 2023-07-15 19:33:44.000000 damo-1.9.1/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35836 2023-07-23 18:27:42.000000 damo-1.9.1/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11838 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.9.1/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    28979 2023-07-22 17:33:00.000000 damo-1.9.1/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19958 2023-07-22 18:51:01.000000 damo-1.9.1/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3853 2023-07-23 17:09:22.000000 damo-1.9.1/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.9.1/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.9.1/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13384 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.9.1/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.9.1/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_record_info.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3723 2023-07-15 19:33:44.000000 damo-1.9.1/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.9.1/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17392 2023-07-23 18:59:48.000000 damo-1.9.1/src/damo/damo_show.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.9.1/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3609 2023-07-23 17:24:02.000000 damo-1.9.1/src/damo/damo_status.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.9.1/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.9.1/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.9.1/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.9.1/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-07-24 17:10:30.000000 damo-1.9.1/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5537 2023-07-15 19:33:44.000000 damo-1.9.1/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-24 17:11:40.033988 damo-1.9.1/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1136 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-07-24 17:11:40.000000 damo-1.9.1/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:31.461842 damo-1.9.2/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-08-01 00:43:31.461842 damo-1.9.2/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-08-01 00:43:27.000000 damo-1.9.2/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.9.2/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-08-01 00:43:31.461842 damo-1.9.2/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.9.2/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:31.445843 damo-1.9.2/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:31.461842 damo-1.9.2/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:27.000000 damo-1.9.2/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.9.2/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9825 2023-07-15 19:33:44.000000 damo-1.9.2/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    36884 2023-07-30 19:06:29.000000 damo-1.9.2/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    15397 2023-07-30 18:25:59.000000 damo-1.9.2/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.9.2/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    28979 2023-07-30 17:37:07.000000 damo-1.9.2/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    20236 2023-07-29 21:28:06.000000 damo-1.9.2/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3853 2023-07-23 17:09:22.000000 damo-1.9.2/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.9.2/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.9.2/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13384 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.9.2/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.9.2/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3723 2023-07-15 19:33:44.000000 damo-1.9.2/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.9.2/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    18632 2023-07-30 19:06:29.000000 damo-1.9.2/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.9.2/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3447 2023-07-30 17:59:22.000000 damo-1.9.2/src/damo/damo_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.9.2/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.9.2/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-08-01 00:42:15.000000 damo-1.9.2/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5537 2023-07-15 19:33:44.000000 damo-1.9.2/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:31.461842 damo-1.9.2/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1136 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.9.1/PKG-INFO` & `damo-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.9.1
+Version: 1.9.2
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.1/README.md` & `damo-1.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -47,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,19 +75,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.1/setup.py` & `damo-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damo_deprecated.py` & `damo-1.9.2/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damo_deprecation_notice.py` & `damo-1.9.2/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damo_dist.py` & `damo-1.9.2/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damo_fmt_str.py` & `damo-1.9.2/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damo_fs.py` & `damo-1.9.2/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damo_paddr_layout.py` & `damo-1.9.2/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damo_subcmds.py` & `damo-1.9.2/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damon.py` & `damo-1.9.2/src/damo/_damon.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,15 +440,15 @@
                 [kv['weights']['sz_permil'],
                     kv['weights']['nr_accesses_permil'],
                     kv['weights']['age_permil'],])
 
     def to_str(self, raw):
         return '\n'.join([
             '%s / %s per %s' % (
-                _damo_fmt_str.format_sz(self.time_ms * 1000000, raw),
+                _damo_fmt_str.format_time_ns(self.time_ms * 1000000, raw),
                 _damo_fmt_str.format_time_ns(self.sz_bytes, raw),
                 _damo_fmt_str.format_time_ms(self.reset_interval_ms, raw)),
             'priority: sz %s, nr_accesses %s, age %s' % (
                 _damo_fmt_str.format_permil(self.weight_sz_permil, raw),
                 _damo_fmt_str.format_permil(
                     self.weight_nr_accesses_permil, raw),
                 _damo_fmt_str.format_permil(self.weight_age_permil, raw)),
@@ -479,28 +479,31 @@
     mid_permil = None
     low_permil = None
 
     # no limit by default
     def __init__(self, metric=damos_wmarks_metric_none, interval_us=0,
             high='0 %', mid='0 %', low='0 %'):
         # 'none' or 'free_mem_rate'
+        if not metric in [damos_wmarks_metric_none,
+                damos_wmarks_metric_free_mem_rate]:
+            raise Exception('wrong watermark metric (%s)' % metric)
         self.metric = metric
         self.interval_us = _damo_fmt_str.text_to_us(interval_us)
         self.high_permil = _damo_fmt_str.text_to_permil(high)
         self.mid_permil = _damo_fmt_str.text_to_permil(mid)
         self.low_permil = _damo_fmt_str.text_to_permil(low)
 
     def to_str(self, raw):
         return '\n'.join([
-            '%s/%s/%s' % (
+            'metric %s, interval %s' % (self.metric,
+                _damo_fmt_str.format_time_us(self.interval_us, raw)),
+            '%s, %s, %s' % (
                 _damo_fmt_str.format_permil(self.high_permil, raw),
                 _damo_fmt_str.format_permil(self.mid_permil, raw),
                 _damo_fmt_str.format_permil(self.low_permil, raw)),
-            'metric %s, interval %s' % (self.metric,
-                _damo_fmt_str.format_time_us(self.interval_us, raw))
             ])
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
         return (type(self) == type(other) and self.metric == other.metric and
@@ -525,55 +528,67 @@
                 ('mid_permil',
                     _damo_fmt_str.format_permil(self.mid_permil, raw)),
                 ('low_permil',
                     _damo_fmt_str.format_permil(self.low_permil, raw)),
                 ])
 
 class DamosFilter:
-    filter_type = None  # anon, memcg, or addr
+    filter_type = None  # anon, memcg, addr, or target
+    matching = None
     memcg_path = None
     address_range = None    # DamonRegion
-    matching = None
+    damon_target_idx = None
 
-    def __init__(self, filter_type, memcg_path, address_range, matching):
+    def __init__(self, filter_type, matching, memcg_path=None,
+            address_range=None, damon_target_idx=None):
         self.filter_type = filter_type
+        self.matching = _damo_fmt_str.text_to_bool(matching)
         self.memcg_path = memcg_path
         self.address_range = address_range
-        self.matching = _damo_fmt_str.text_to_bool(matching)
+        if damon_target_idx != None:
+            self.damon_target_idx = _damo_fmt_str.text_to_nr(damon_target_idx)
 
     def to_str(self, raw):
-        plus_str = ''
+        txt = '%s %s' % (self.filter_type,
+                'matching' if self.matching else 'nomatching')
+        if self.filter_type == 'anon':
+            return txt
         if self.filter_type == 'memcg':
-            plus_str = 'memcg_path %s, ' % self.memcg_path
+            return '%s %s' % (txt, self.memcg_path)
         if self.filter_type == 'addr':
-            plus_str = '%s, ' % self.address_range.to_str(raw)
-        return 'filter_type %s, %smatching %s' % (
-                self.filter_type, plus_str, self.matching)
+            return '%s %s' % (txt, self.address_range.to_str(raw))
+        if self.filter_type == 'target':
+            return '%s %s' % (txt, _damo_fmt_str.format_nr(
+                    self.damon_target_idx, raw))
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
         return type(self) == type(other) and '%s' % self == '%s' % other
 
     @classmethod
     def from_kvpairs(cls, kv):
-        return DamosFilter(kv['filter_type'],
+        return DamosFilter(kv['filter_type'], kv['matching'],
                 kv['memcg_path'] if kv['filter_type'] == 'memcg' else '',
                 DamonRegion.from_kvpairs(kv['address_range'])
                     if kv['filter_type'] == 'addr' else None,
-                kv['matching'])
+                kv['damon_target_idx']
+                    if kv['filter_type'] == 'target' else None)
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict([
             ('filter_type', self.filter_type),
+            ('matching', self.matching),
             ('memcg_path', self.memcg_path),
             ('address_range', self.address_range.to_kvpairs(raw) if
                 self.address_range != None else None),
-            ('matching', self.matching)])
+            ('damon_target_idx',
+                _damo_fmt_str.format_nr(self.damon_target_idx, raw)
+                if self.damon_target_idx != None else None)])
 
 class DamosStats:
     nr_tried = None
     sz_tried = None
     nr_applied = None
     sz_applied = None
     qt_exceeds = None
@@ -969,16 +984,23 @@
 
 def is_kdamond_running(kdamond_idx):
     return _damon_fs.is_kdamond_running(kdamond_idx)
 
 def current_kdamonds():
     return _damon_fs.current_kdamonds()
 
-def update_read_kdamonds():
-    err = update_schemes_status()
+def update_read_kdamonds(nr_retries=0):
+    err = 'assumed error'
+    nr_tries = 0
+    while True:
+        err = update_schemes_status()
+        nr_tries += 1
+        if err == None or nr_tries > nr_retries:
+            break
+        time.sleep(random.randrange(2**(nr_tries - 1), 2**nr_tries) / 100)
     if err:
         return None, err
     return current_kdamonds(), None
 
 def nr_kdamonds():
     return _damon_fs.nr_kdamonds()
```

### Comparing `damo-1.9.1/src/damo/_damon_args.py` & `damo-1.9.2/src/damo/_damon_args.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,21 +71,93 @@
 
     try:
         kvpairs = json.loads(schemes)
         return [_damon.Damos.from_kvpairs(kv) for kv in kvpairs], None
     except Exception as json_err:
         return None, '%s' % json_err
 
+def damos_options_to_filters(filters_args):
+    filters = []
+    if filters_args == None:
+        return filters, None
+
+    for fields in filters_args:
+        if len(fields) < 2:
+            return None, '<2 filter field legth (%s)' % fields
+        ftype = fields[0]
+        fmatching = fields[1]
+        fargs = fields[2:]
+        if not fmatching in ['matching', 'nomatching']:
+            return None, 'unsupported matching keyword (%s)' % fmatching
+        fmatching = fmatching == 'matching'
+        if ftype == 'anon':
+            if len(fargs):
+                return (None, 'anon filter receives no arguments but (%s)'
+                        % fargs)
+            filters.append(_damon.DamosFilter(ftype, fmatching))
+        elif ftype == 'memcg':
+            if len(fargs) != 1:
+                return None, 'wrong number of memcg arguments (%s)' % fargs
+            memcg_path = fargs[0]
+            filters.append(_damon.DamosFilter(ftype, fmatching, memcg_path))
+        elif ftype == 'addr':
+            if len(fargs) != 2:
+                return None, 'wrong number of addr arguments (%s)' % fargs
+            try:
+                addr_range = _damon.DamonRegion(fargs[0], fargs[1])
+            except Exception as e:
+                return None, 'wrong addr range (%s, %s)' % (fargs, e)
+            filters.append(
+                    _damon.DamosFilter(ftype, fmatching, None, addr_range))
+        elif ftype == 'target':
+            if len(fargs) != 1:
+                return None, 'wrong number of target argument (%s)' % fargs
+            try:
+                filters.append(
+                        _damon.DamosFilter(ftype, fmatching, None, None,
+                            fargs[0]))
+            except Exception as e:
+                return None, 'target filter creation failed (%s, %s)' % (
+                        fargs[0], e)
+        else:
+            return None, 'unsupported filter type'
+    return filters, None
+
 def damos_options_to_scheme(args):
+    if args.damos_quotas != None:
+        qargs = args.damos_quotas
+        try:
+            quotas = _damon.DamosQuotas(qargs[0], qargs[1], qargs[2],
+                    [qargs[3], qargs[4], qargs[5]])
+        except Exception as e:
+            return None, 'Wrong --damos_quotas (%s, %s)' % (qargs, e)
+    else:
+        quotas = None
+
+    if args.damos_wmarks != None:
+        wargs = args.damos_wmarks
+        try:
+            wmarks = _damon.DamosWatermarks(wargs[0], wargs[1], wargs[2],
+                    wargs[3], wargs[4])
+        except Exception as e:
+            return None, 'Wrong --damos_wmarks (%s, %s)' % (wargs, e)
+    else:
+        wmarks = None
+
+    filters, err = damos_options_to_filters(args.damos_filter)
+    if err != None:
+        return None, err
+
     try:
         return _damon.Damos(
                 access_pattern=_damon.DamosAccessPattern(
                     args.damos_sz_region, args.damos_access_rate,
                     _damon.unit_percent, args.damos_age, _damon.unit_usec),
-                action=args.damos_action), None
+                action=args.damos_action, quotas=quotas, watermarks=wmarks,
+                filters=filters), None
     except Exception as e:
         return None, 'Wrong \'--damos_*\' argument (%s)' % e
 
 def damos_for(args):
     if args.damos_action:
         damos, err = damos_options_to_scheme(args)
         if err != None:
@@ -301,14 +373,28 @@
             help='min/max access rate of damos target regions (percent)')
     parser.add_argument('--damos_age', metavar=('<min>', '<max>'), nargs=2,
             default=['min', 'max'],
             help='min/max age of damos target regions (microseconds)')
     parser.add_argument('--damos_action', metavar='<action>',
             choices=_damon.damos_actions,
             help='damos action to apply to the target regions')
+    parser.add_argument('--damos_quotas',
+            metavar=('<time (ms)>', '<size (bytes)>', '<reset interval (ms)>',
+                '<size priority weight (permil)>',
+                '<access rate priority weight> (permil)',
+                '<age priority weight> (permil)'), nargs=6,
+            help='damos quotas')
+    parser.add_argument('--damos_wmarks', nargs=5,
+            metavar=('<metric (none|free_mem_rate)>', '<interval (us)>',
+                '<high mark (permil)>', '<mid mark (permil)>',
+                '<low mark (permil)>'),
+            help='damos watermarks')
+    parser.add_argument('--damos_filter', nargs='+', action='append',
+            metavar='<filter argument>',
+            help='damos filter (type, matching, and optional arguments')
 
 def set_argparser(parser, add_record_options):
     if parser == None:
         parser = argparse.ArgumentParser()
     set_monitoring_argparser(parser)
     parser.add_argument('--ops', choices=['vaddr', 'paddr', 'fvaddr'],
             help='monitoring operations set')
```

### Comparing `damo-1.9.1/src/damo/_damon_dbgfs.py` & `damo-1.9.2/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damon_result.py` & `damo-1.9.2/src/damo/_damon_result.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/_damon_sysfs.py` & `damo-1.9.2/src/damo/_damon_sysfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,18 @@
     wops = {
         'type': '%s' % damos_filter.filter_type,
         'memcg_path': ('%s' % damos_filter.memcg_path
             if damos_filter.memcg_path != None else ''),
         'matching': 'Y' if damos_filter.matching else 'N',
         }
     if damos_filter.address_range != None:
-        wops['addr_start'] = damos_filter.address_range.start
-        wops['addr_end'] = damos_filter.address_range.end
+        wops['addr_start'] = '%d' % damos_filter.address_range.start
+        wops['addr_end'] = '%d' % damos_filter.address_range.end
+    if damos_filter.damon_target_idx != None:
+        wops['damon_target_idx'] = '%d' % damos_filter.damon_target_idx
     return wops
 
 def wops_for_scheme_filters(filters):
     wops = {}
     for idx, damos_filter in enumerate(filters):
         wops['%d' % idx] = wops_for_scheme_filter(damos_filter)
     return wops
@@ -356,19 +358,22 @@
             int(files_content['interval_us']),
             int(files_content['high']),
             int(files_content['mid']),
             int(files_content['low']))
 
 def files_content_to_damos_filters(files_content):
     return [_damon.DamosFilter(filter_kv['type'].strip(),
+            filter_kv['matching'].strip(),
             filter_kv['memcg_path'].strip(),
             _damon.DamonRegion(filter_kv['addr_start'].strip(),
                 filter_kv['addr_end'].strip())
-                if filter_kv['type'] == 'addr' else None,
-            filter_kv['matching'].strip())
+                if 'addr_start' in filter_kv and 'addr_end' in filter_kv
+                else None,
+            filter_kv['damon_target_idx']
+                if 'damon_target_idx' in filter_kv else None)
             for filter_kv in numbered_dirs_content(
                 files_content, 'nr_filters')]
 
 def files_content_to_damos_stats(files_content):
     return _damon.DamosStats(
             int(files_content['nr_tried']),
             int(files_content['sz_tried']),
```

### Comparing `damo-1.9.1/src/damo/damo.py` & `damo-1.9.2/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_adjust.py` & `damo-1.9.2/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_convert_record_format.py` & `damo-1.9.2/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_features.py` & `damo-1.9.2/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_fmt_json.py` & `damo-1.9.2/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_heats.py` & `damo-1.9.2/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_lru_sort.py` & `damo-1.9.2/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_monitor.py` & `damo-1.9.2/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_nr_regions.py` & `damo-1.9.2/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_reclaim.py` & `damo-1.9.2/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_record.py` & `damo-1.9.2/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_record_info.py` & `damo-1.9.2/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_report.py` & `damo-1.9.2/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_report_raw.py` & `damo-1.9.2/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_schemes.py` & `damo-1.9.2/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_show.py` & `damo-1.9.2/src/damo/damo_show.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,16 +58,21 @@
             _damo_fmt_str.format_sz(region.end, raw),
         '<region size>': lambda index, region, raw, mms:
             _damo_fmt_str.format_sz(region.size(), raw),
         '<access rate>': lambda index, region, raw, mms:
             _damo_fmt_str.format_percent(region.nr_accesses.percent, raw),
         '<age>': lambda index, region, raw, mms:
             _damo_fmt_str.format_time_us(region.age.usec, raw),
-        '<size_bar>': lambda index, region, raw, mms:
+        '<size bar>': lambda index, region, raw, mms:
            size_bar(region, mms, 0, 20),
+        '<size heat bar>': lambda index, region, raw, mms:
+           size_heat_bar(region, mms, 1, 20),
+        '<size heat age bar>': lambda index, region, raw, mms:
+           size_heat_age_bar(region, mms, 1, 20),
+
         }
 
 formatters = {
         'record': record_formatters,
         'snapshot': snapshot_formatters,
         'region': region_formatters
         }
@@ -132,23 +137,48 @@
     Returns
     -------
     float
         The rescaled value
     '''
     orig_length = orig_scale_minmax[1] - orig_scale_minmax[0]
     new_length = new_scale_minmax[1] - new_scale_minmax[0]
-    ratio = new_length / orig_length
+    ratio = new_length / orig_length if orig_length > 0 else 1
     return (val - orig_scale_minmax[0]) * ratio + new_scale_minmax[0]
 
 def size_bar(region, minmaxs, min_cols, max_cols):
+    print(region.size())
     nr_cols = int(rescale_val(region.size(),
             [minmaxs.min_sz_region, minmaxs.max_sz_region],
             [min_cols, max_cols]))
     return '<%s>' % ('-' * nr_cols)
 
+def size_heat_bar(region, minmaxs, min_cols, max_cols):
+    nr_cols = int(rescale_val(region.size(),
+            [minmaxs.min_sz_region, minmaxs.max_sz_region],
+            [min_cols, max_cols]))
+    heat_symbol = int(rescale_val(region.nr_accesses.percent,
+        [minmaxs.min_access_rate_percent, minmaxs.max_access_rate_percent],
+        [0, 9]))
+
+    return '<%s>' % ('%d' % heat_symbol * nr_cols)
+
+def size_heat_age_bar(region, minmaxs, min_cols, max_cols):
+    nr_cols = int(rescale_val(region.size(),
+            [minmaxs.min_sz_region, minmaxs.max_sz_region],
+            [min_cols, max_cols]))
+    heat_symbol = int(rescale_val(region.nr_accesses.percent,
+        [minmaxs.min_access_rate_percent, minmaxs.max_access_rate_percent],
+        [0, 9]))
+    nr_rows = int(rescale_val(region.age.usec,
+        [minmaxs.min_age_us, minmaxs.max_age_us],
+        [1, 5]))
+
+    row = '<%s>' % ('%d' % heat_symbol * nr_cols)
+    return '\n'.join([row] * nr_rows) + '\n'
+
 def apply_min_chars(min_chars, field_name, txt):
     # min_chars: [[<field name>, <number of min chars>]...]
     for name, nr in min_chars:
         try:
             nr = int(nr)
         except:
             print('wrong min_chars: %s' % min_chars)
```

### Comparing `damo-1.9.1/src/damo/damo_start.py` & `damo-1.9.2/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_status.py` & `damo-1.9.2/src/damo/damo_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,26 +61,15 @@
     kdamonds = _damon.current_kdamonds()
     summary = [k.summary_str() for k in kdamonds]
     if json_format:
         print(json.dumps(summary, indent=4))
         return
     print('\n'.join(summary))
 
-def update_pr_kdamonds(json_format, raw_nr):
-    err = 'assumed error'
-    nr_tries = 0
-    while err != None and nr_tries < 5:
-        nr_tries += 1
-        kdamonds, err = _damon.update_read_kdamonds()
-        if err != None:
-            time.sleep(random.randrange(
-                2**(nr_tries - 1), 2**nr_tries) / 100)
-    if err:
-        print(err)
-        return
+def pr_kdamonds(kdamonds, json_format, raw_nr):
     if json_format:
         print(json.dumps([k.to_kvpairs(raw_nr) for k in kdamonds], indent=4))
     else:
         for idx, k in enumerate(kdamonds):
             print('kdamond %d' % idx)
             print(_damo_fmt_str.indent_lines( k.to_str(raw_nr), 4))
 
@@ -96,11 +85,15 @@
 def main(args=None):
     if not args:
         parser = set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
 
-    update_pr_kdamonds(args.json, args.raw)
+    kdamonds, err = _damon.update_read_kdamonds(nr_retries=5)
+    if err != None:
+        print('cannot update and read kdamonds: %s' % err)
+        exit(1)
+    pr_kdamonds(kdamonds, args.json, args.raw)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.9.1/src/damo/damo_stop.py` & `damo-1.9.2/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_translate_damos.py` & `damo-1.9.2/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_tune.py` & `damo-1.9.2/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_validate.py` & `damo-1.9.2/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo/damo_wss.py` & `damo-1.9.2/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.1/src/damo.egg-info/PKG-INFO` & `damo-1.9.2/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.9.1
+Version: 1.9.2
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.1/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.1/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.1/src/damo.egg-info/SOURCES.txt` & `damo-1.9.2/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

