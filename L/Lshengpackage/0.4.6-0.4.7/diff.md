# Comparing `tmp/Lshengpackage-0.4.6.tar.gz` & `tmp/Lshengpackage-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.4.6.tar", last modified: Mon Jul 31 09:28:40 2023, max compression
+gzip compressed data, was "Lshengpackage-0.4.7.tar", last modified: Tue Aug  1 07:58:18 2023, max compression
```

## Comparing `Lshengpackage-0.4.6.tar` & `Lshengpackage-0.4.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.042842 Lshengpackage-0.4.6/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.6/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.6/License.md
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.928592 Lshengpackage-0.4.6/Lshengpackage/
--rw-rw-rw-   0        0        0      550 2023-05-18 16:33:59.000000 Lshengpackage-0.4.6/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.940081 Lshengpackage-0.4.6/Lshengpackage/network/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:41:45.000000 Lshengpackage-0.4.6/Lshengpackage/network/__init__.py
--rw-rw-rw-   0        0        0     2495 2023-07-31 09:22:35.000000 Lshengpackage-0.4.6/Lshengpackage/network/scan.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.945082 Lshengpackage-0.4.6/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2023-05-18 15:10:46.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.950080 Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/
--rw-rw-rw-   0        0        0      162 2023-05-19 03:15:17.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      428 2023-05-19 03:15:17.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/mock_findFr.cpython-39.pyc
--rw-rw-rw-   0        0        0     1717 2023-05-19 03:26:52.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.972629 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     3313 2023-05-19 03:03:37.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0       49 2023-05-18 15:10:46.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.990141 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0     3855 2023-05-19 03:15:18.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
--rw-rw-rw-   0        0        0      166 2023-05-19 03:15:18.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2290 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.001640 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.004680 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__pycache__/
--rw-rw-rw-   0        0        0      175 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6503 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc
--rw-rw-rw-   0        0        0     8853 2023-05-19 05:56:20.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
--rw-rw-rw-   0        0        0     3059 2023-05-19 03:37:17.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/re_Pic.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.011681 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4683 2023-05-18 16:25:46.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.019688 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4828 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      160 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/mock_findFr.py
--rw-rw-rw-   0        0        0     2554 2023-05-19 03:34:10.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/mock_findPic.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.029650 Lshengpackage-0.4.6/Lshengpackage/tools/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.6/Lshengpackage/tools/ChaoJiYing.py
--rw-rw-rw-   0        0        0      757 2023-05-18 15:10:46.000000 Lshengpackage-0.4.6/Lshengpackage/tools/General.py
--rw-rw-rw-   0        0        0     2019 2023-05-19 03:47:29.000000 Lshengpackage-0.4.6/Lshengpackage/tools/Loading.py
--rw-rw-rw-   0        0        0     3311 2023-05-18 14:57:22.000000 Lshengpackage-0.4.6/Lshengpackage/tools/OperateFile.py
--rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.6/Lshengpackage/tools/SearchFile.py
--rw-rw-rw-   0        0        0       49 2023-05-18 16:20:17.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.040853 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/
--rw-rw-rw-   0        0        0     1982 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc
--rw-rw-rw-   0        0        0     1167 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/General.cpython-39.pyc
--rw-rw-rw-   0        0        0     1431 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc
--rw-rw-rw-   0        0        0     2530 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc
--rw-rw-rw-   0        0        0     1282 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc
--rw-rw-rw-   0        0        0      159 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.936560 Lshengpackage-0.4.6/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      969 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2122 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      342 2023-07-31 07:42:41.000000 Lshengpackage-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0      969 2023-07-31 09:28:40.042842 Lshengpackage-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.6/README.md
--rw-rw-rw-   0        0        0      422 2023-07-31 08:17:55.000000 Lshengpackage-0.4.6/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-07-31 09:28:40.043842 Lshengpackage-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     2098 2023-07-31 09:24:09.000000 Lshengpackage-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.122340 Lshengpackage-0.4.7/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.7/License.md
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:17.931859 Lshengpackage-0.4.7/Lshengpackage/
+-rw-rw-rw-   0        0        0      550 2023-05-18 16:33:59.000000 Lshengpackage-0.4.7/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:17.943445 Lshengpackage-0.4.7/Lshengpackage/network/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:41:45.000000 Lshengpackage-0.4.7/Lshengpackage/network/__init__.py
+-rw-rw-rw-   0        0        0     3316 2023-08-01 07:57:20.000000 Lshengpackage-0.4.7/Lshengpackage/network/scan.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:17.948481 Lshengpackage-0.4.7/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2023-05-18 15:10:46.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:17.986512 Lshengpackage-0.4.7/Lshengpackage/simulate/__pycache__/
+-rw-rw-rw-   0        0        0      162 2023-05-19 03:15:17.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      428 2023-05-19 03:15:17.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/__pycache__/mock_findFr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1717 2023-05-19 03:26:52.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.030275 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     3313 2023-05-19 03:03:37.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       49 2023-05-18 15:10:46.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.045660 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0     3855 2023-05-19 03:15:18.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
+-rw-rw-rw-   0        0        0      166 2023-05-19 03:15:18.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2290 2023-05-19 03:16:36.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.049702 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/dingtalk/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/dingtalk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.053669 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/dingtalk/__pycache__/
+-rw-rw-rw-   0        0        0      175 2023-05-19 03:16:36.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/dingtalk/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6503 2023-05-19 03:16:36.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8853 2023-05-19 05:56:20.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
+-rw-rw-rw-   0        0        0     3059 2023-05-19 03:37:17.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/adb/re_Pic.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.061670 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4683 2023-05-18 16:25:46.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.069185 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4828 2023-05-19 03:16:36.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      160 2023-05-19 03:16:36.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2554 2023-05-19 03:34:10.000000 Lshengpackage-0.4.7/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.096189 Lshengpackage-0.4.7/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.7/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      757 2023-05-18 15:10:46.000000 Lshengpackage-0.4.7/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0     2019 2023-05-19 03:47:29.000000 Lshengpackage-0.4.7/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3311 2023-05-18 14:57:22.000000 Lshengpackage-0.4.7/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.7/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       49 2023-05-18 16:20:17.000000 Lshengpackage-0.4.7/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:18.121337 Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/
+-rw-rw-rw-   0        0        0     1982 2023-05-19 03:16:35.000000 Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1167 2023-05-19 03:16:35.000000 Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/General.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1431 2023-05-19 03:16:35.000000 Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2530 2023-05-19 03:16:35.000000 Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1282 2023-05-19 03:16:36.000000 Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc
+-rw-rw-rw-   0        0        0      159 2023-05-19 03:16:35.000000 Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-08-01 07:58:17.940482 Lshengpackage-0.4.7/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      969 2023-08-01 07:58:17.000000 Lshengpackage-0.4.7/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2122 2023-08-01 07:58:17.000000 Lshengpackage-0.4.7/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:58:17.000000 Lshengpackage-0.4.7/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-08-01 07:58:17.000000 Lshengpackage-0.4.7/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-01 07:58:17.000000 Lshengpackage-0.4.7/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      342 2023-07-31 07:42:41.000000 Lshengpackage-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      969 2023-08-01 07:58:18.122340 Lshengpackage-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.7/README.md
+-rw-rw-rw-   0        0        0      422 2023-07-31 08:17:55.000000 Lshengpackage-0.4.7/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-08-01 07:58:18.123845 Lshengpackage-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     2098 2023-08-01 07:58:04.000000 Lshengpackage-0.4.7/setup.py
```

### Comparing `Lshengpackage-0.4.6/LICENSE` & `Lshengpackage-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/License.md` & `Lshengpackage-0.4.7/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/__init__.py` & `Lshengpackage-0.4.7/Lshengpackage/__init__.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/network/scan.py` & `Lshengpackage-0.4.7/Lshengpackage/network/scan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # -*- coding: utf-8 -*-
 import os
 import re
 import socket
+import threading
+import time
 from collections import defaultdict
 
+ip_Mac = defaultdict(list)
+
 
 # 获取指定IP地址的MAC地址
 def getMac(target_IP):
     # 初始化 用正则表达式're'编译出匹配MAC地址的正则表达式对象
     patt_mac = re.compile('([a-f0-9]{2}[-:]){5}[a-f0-9]{2}', re.I)
     # ping
     os.popen('ping -n 1 -w 500 {} > nul'.format(target_IP))
@@ -15,52 +19,80 @@
     arp_file = os.popen('arp -a {}'.format(target_IP))
     # 使用正则表达式'self.patt_mac'在输出结果中查找符合 MAC 地址格式的字符串 并返回找到的第一个匹配项 即 IP 对应的 MAC 地址
     mac_addr = patt_mac.search(arp_file.read())
 
     # 根据正则表达式对象匹配MAC地址 如果匹配到了就返回MAC地址 否则返回None
     if mac_addr:
         mac_addr = mac_addr.group()
+        ip_Mac[target_IP].append(mac_addr)
         return mac_addr
     else:
+        # print(target_IP)
         return '00-00-00-00-00-00'
 
 
-# 获取与本机在同一局域网下的设备 IP与MAC的映射
-def getLANIpMac():
+def threadsMac(gate_way, ip_addr, _mix, _max):
+    threads = []
+    for i in range(_mix, _max):
+        target_IP = gate_way + str(i)
+        if target_IP != ip_addr:
+            threads.append(threading.Thread(target=getMac, args={target_IP, }))
+        else:
+            threads.append(threading.Thread(target=getMac, args={target_IP, }))
+
+    for i in threads:
+        i.start()
+    for i in threads:
+        i.join()
+
+
+def common_LAN_WAN(gate_way, ip_addr, _mix, _max):
+    threadsMac(gate_way, ip_addr, _mix, _max)
+    # 打印方法
+    for i in ip_Mac:
+        print(i + ':[' + ip_Mac[i][0] + ']')
+    print("end time %s" % time.ctime())
+    print('本次扫描共检测到本网络存在%s台设备' % len(ip_Mac))
+
+
+# 获取与本机在同一局域网下的设备 IP与MAC的映射(多线程)除本机
+def getLANIpMac(_mix=0, _max=255):
+    ip_Mac.clear()
     """
     # 返回默认网卡对应的IP地址
     ip_addr = socket.gethostbyname(socket.gethostname())
     """
     # 创建一个UDP套接字
     sockets = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     # 连接到一个公共ip地址
     sockets.connect(('www.baidu.com', 80))
     # 获取本地套接字的地址信息 这个地址信息就是本机在局域网中的IP地址
     ip_addr = sockets.getsockname()[0]
     # 关闭套接字
     sockets.close()
-
-    print("当前本机局域网ip地址为:" + ip_addr + '\n')
+    print("start time %s" % time.ctime())
+    print("当前本机局域网ip地址为:" + ip_addr)
     # 获取网关
     idx = 0
     cnt = 0
     for i in ip_addr:
         idx = idx + 1
         if i == '.':
             cnt = cnt + 1
             if cnt == 3:
                 break
     gate_way = ip_addr[0:idx]
-    # 循环发送arp请求及获取对应ip的mac地址
-    ip_Mac = defaultdict(list)
-    for i in range(0, 255):
-        target_IP = gate_way + str(i)
-        if target_IP != ip_addr:
-            target_Mac = getMac(target_IP)
-            if target_Mac == "00-00-00-00-00-00":
-                # print("{:>15}".format(target_IP) + ":\t\tTimeout!")
-                pass
-            else:
-                # print("{:>15}".format(target_IP) + ":\t\t" + target_Mac)
-                ip_Mac[target_IP].append(target_Mac)
-    for i in ip_Mac:
-        print(i+':['+ip_Mac[i][0]+']')
+    common_LAN_WAN(gate_way, ip_addr, _mix, _max)
+    return ip_Mac
+
+# 获取内网可达的设备 IP与MAC的映射(多线程)除本机
+def getWANIpMac(cmd_args, _mix=0, _max=255):
+    ip_Mac.clear()
+    print("start time %s" % time.ctime())
+    # cmd_args = sys.argv[1:]
+    args = "".join(cmd_args)
+    gate_way = '.'.join(args.split('.')[:-1]) + '.'
+
+    ip_addr = '0'
+    common_LAN_WAN(gate_way, ip_addr, _mix, _max)
+
+
```

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/Command_adb.py` & `Lshengpackage-0.4.7/Lshengpackage/simulate/adb/Command_adb.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py` & `Lshengpackage-0.4.7/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/re_Pic.py` & `Lshengpackage-0.4.7/Lshengpackage/simulate/adb/re_Pic.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.4.7/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.4.7/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/simulate/mock_findPic.py` & `Lshengpackage-0.4.7/Lshengpackage/simulate/mock_findPic.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/ChaoJiYing.py` & `Lshengpackage-0.4.7/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/General.py` & `Lshengpackage-0.4.7/Lshengpackage/tools/General.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/Loading.py` & `Lshengpackage-0.4.7/Lshengpackage/tools/Loading.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/OperateFile.py` & `Lshengpackage-0.4.7/Lshengpackage/tools/OperateFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/SearchFile.py` & `Lshengpackage-0.4.7/Lshengpackage/tools/SearchFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/General.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/General.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc` & `Lshengpackage-0.4.7/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.4.7/Lshengpackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.6
+Version: 0.4.7
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫,网络
```

### Comparing `Lshengpackage-0.4.6/Lshengpackage.egg-info/SOURCES.txt` & `Lshengpackage-0.4.7/Lshengpackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/PKG-INFO` & `Lshengpackage-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.6
+Version: 0.4.7
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫,网络
```

### Comparing `Lshengpackage-0.4.6/README.md` & `Lshengpackage-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.6/setup.py` & `Lshengpackage-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.4.6',  # Start with a small number and increase it with every change you make
+    version='0.4.7',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
     url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
```

