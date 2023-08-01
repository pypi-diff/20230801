# Comparing `tmp/huhk-1.9.1.tar.gz` & `tmp/huhk-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.9.1.tar", last modified: Tue Aug  1 01:44:39 2023, max compression
+gzip compressed data, was "huhk-1.9.2.tar", last modified: Tue Aug  1 01:48:15 2023, max compression
```

## Comparing `huhk-1.9.1.tar` & `huhk-1.9.2.tar`

### file list

```diff
@@ -1,481 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.852923 huhk-1.9.1/
--rw-rw-rw-   0        0        0      223 2023-08-01 01:44:39.850899 huhk-1.9.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:37.794568 huhk-1.9.1/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.1/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:37.891250 huhk-1.9.1/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.9.1/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    21531 2023-07-31 07:13:40.000000 huhk-1.9.1/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     1332 2023-07-31 08:21:56.000000 huhk-1.9.1/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    18567 2023-07-31 08:18:51.000000 huhk-1.9.1/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.9.1/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-08-01 01:44:36.000000 huhk-1.9.1/huhk/case_project/version.py
--rw-rw-rw-   0        0        0     9925 2023-07-31 05:34:49.000000 huhk-1.9.1/huhk/init_project.py
--rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.9.1/huhk/main.py
--rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.9.1/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:37.896468 huhk-1.9.1/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.005378 huhk-1.9.1/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.1/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.9.1/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.9.1/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.1/huhk/unit_data.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    29027 2023-08-01 01:43:21.000000 huhk-1.9.1/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.9.1/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.9.1/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:37.828604 huhk-1.9.1/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19653 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.013357 huhk-1.9.1/service/
--rw-rw-rw-   0        0        0        0 2023-07-28 06:59:30.000000 huhk-1.9.1/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.028108 huhk-1.9.1/service/app_a/
--rw-rw-rw-   0        0        0      420 2023-07-31 05:25:05.000000 huhk-1.9.1/service/app_a/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.080965 huhk-1.9.1/service/app_a/apis/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.126843 huhk-1.9.1/service/app_a/apis/admin/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/admin/__init__.py
--rw-rw-rw-   0        0        0     1603 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/admin/apis_admin_guc.py
--rw-rw-rw-   0        0        0      784 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/admin/apis_admin_spa.py
--rw-rw-rw-   0        0        0     1105 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/apis_activitymanager.py
--rw-rw-rw-   0        0        0     2049 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/apis_app_a.py
--rw-rw-rw-   0        0        0     1072 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/apis_area.py
--rw-rw-rw-   0        0        0      914 2023-07-31 06:00:57.000000 huhk-1.9.1/service/app_a/apis/apis_content.py
--rw-rw-rw-   0        0        0     2511 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/apis_essay.py
--rw-rw-rw-   0        0        0     2187 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/apis_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.197114 huhk-1.9.1/service/app_a/apis/common/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_clue.py
--rw-rw-rw-   0        0        0     1071 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_common.py
--rw-rw-rw-   0        0        0     1945 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     2922 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_systemversion.py
--rw-rw-rw-   0        0        0      867 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_user.py
--rw-rw-rw-   0        0        0    25061 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_user4c.py
--rw-rw-rw-   0        0        0     5938 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.360952 huhk-1.9.1/service/app_a/apis/content/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/content/__init__.py
--rw-rw-rw-   0        0        0    26441 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_activitymanager.py
--rw-rw-rw-   0        0        0    13587 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_adv.py
--rw-rw-rw-   0        0        0     1184 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_advplace.py
--rw-rw-rw-   0        0        0    10283 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_agreement.py
--rw-rw-rw-   0        0        0     8389 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_campmanager.py
--rw-rw-rw-   0        0        0     7639 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_comment.py
--rw-rw-rw-   0        0        0     8748 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_commonquestion.py
--rw-rw-rw-   0        0        0     1419 2023-07-31 06:00:58.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_contentmanager.py
--rw-rw-rw-   0        0        0    14248 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_essay.py
--rw-rw-rw-   0        0        0     1317 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_essaycomment.py
--rw-rw-rw-   0        0        0     4566 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_essayweb.py
--rw-rw-rw-   0        0        0      859 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_hotcity.py
--rw-rw-rw-   0        0        0     2952 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_hotsearch.py
--rw-rw-rw-   0        0        0     6682 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_material.py
--rw-rw-rw-   0        0        0     9450 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_messagemanager.py
--rw-rw-rw-   0        0        0     3576 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_noticemanager.py
--rw-rw-rw-   0        0        0     5813 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_question.py
--rw-rw-rw-   0        0        0     2008 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_recruit.py
--rw-rw-rw-   0        0        0     5100 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_safecode.py
--rw-rw-rw-   0        0        0     9825 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_subject.py
--rw-rw-rw-   0        0        0     9388 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_subjectweb.py
--rw-rw-rw-   0        0        0     6365 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.372918 huhk-1.9.1/service/app_a/apis/content/material/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/material/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/material/apis_content_material_getmateriallist.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.413810 huhk-1.9.1/service/app_a/apis/goods/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/goods/__init__.py
--rw-rw-rw-   0        0        0     9854 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_area.py
--rw-rw-rw-   0        0        0    12191 2023-07-31 06:00:57.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_carmodel.py
--rw-rw-rw-   0        0        0    10643 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_configure.py
--rw-rw-rw-   0        0        0     6170 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_ordermain.py
--rw-rw-rw-   0        0        0     3147 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.419794 huhk-1.9.1/service/app_a/apis/manageapi/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.432761 huhk-1.9.1/service/app_a/apis/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     8140 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/manageapi/order/apis_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.437747 huhk-1.9.1/service/app_a/apis/open/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.459687 huhk-1.9.1/service/app_a/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      816 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0      849 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.503827 huhk-1.9.1/service/app_a/apis/order/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/order/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_freeorder.py
--rw-rw-rw-   0        0        0    23046 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_mainorder.py
--rw-rw-rw-   0        0        0     3724 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_order.py
--rw-rw-rw-   0        0        0    11987 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_rightsorder.py
--rw-rw-rw-   0        0        0     2582 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.518788 huhk-1.9.1/service/app_a/apis/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0     1125 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/mainorder/apis_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.541725 huhk-1.9.1/service/app_a/apis/order/rights/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/rights/__init__.py
--rw-rw-rw-   0        0        0    10735 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/rights/apis_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.566660 huhk-1.9.1/service/app_a/apis/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/rightsorder/apis_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.578626 huhk-1.9.1/service/app_a/apis/pay/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/pay/__init__.py
--rw-rw-rw-   0        0        0      865 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/pay/apis_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.613535 huhk-1.9.1/service/app_a/apis/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.620515 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.642457 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     3883 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0     1699 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     6180 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     7225 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     3763 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     2247 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     6270 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.665398 huhk-1.9.1/service/app_a/apis/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0     1871 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0     2061 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_pointsinfo.py
--rw-rw-rw-   0        0        0      752 2023-07-31 05:25:05.000000 huhk-1.9.1/service/app_a/app_a_fun.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.702555 huhk-1.9.1/service/app_a/asserts/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.719510 huhk-1.9.1/service/app_a/asserts/admin/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/admin/__init__.py
--rw-rw-rw-   0        0        0      941 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/admin/asserts_admin_guc.py
--rw-rw-rw-   0        0        0      552 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/admin/asserts_admin_spa.py
--rw-rw-rw-   0        0        0      626 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/asserts_activitymanager.py
--rw-rw-rw-   0        0        0      653 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/asserts_app_a.py
--rw-rw-rw-   0        0        0      525 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/asserts_area.py
--rw-rw-rw-   0        0        0      536 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/asserts_content.py
--rw-rw-rw-   0        0        0     1009 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/asserts_essay.py
--rw-rw-rw-   0        0        0      707 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/asserts_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.758403 huhk-1.9.1/service/app_a/asserts/common/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/common/__init__.py
--rw-rw-rw-   0        0        0      587 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_clue.py
--rw-rw-rw-   0        0        0      581 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_common.py
--rw-rw-rw-   0        0        0      712 2023-07-31 06:09:08.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     1116 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_systemversion.py
--rw-rw-rw-   0        0        0      579 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_user.py
--rw-rw-rw-   0        0        0     6848 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_user4c.py
--rw-rw-rw-   0        0        0     2174 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.871862 huhk-1.9.1/service/app_a/asserts/content/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/content/__init__.py
--rw-rw-rw-   0        0        0     7782 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_activitymanager.py
--rw-rw-rw-   0        0        0     5226 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_adv.py
--rw-rw-rw-   0        0        0      653 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_advplace.py
--rw-rw-rw-   0        0        0     3600 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_agreement.py
--rw-rw-rw-   0        0        0     2959 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_campmanager.py
--rw-rw-rw-   0        0        0     2532 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_comment.py
--rw-rw-rw-   0        0        0     4032 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_commonquestion.py
--rw-rw-rw-   0        0        0      649 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_contentmanager.py
--rw-rw-rw-   0        0        0     4302 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_essay.py
--rw-rw-rw-   0        0        0      664 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_essaycomment.py
--rw-rw-rw-   0        0        0     1937 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_essayweb.py
--rw-rw-rw-   0        0        0      582 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_hotcity.py
--rw-rw-rw-   0        0        0     1432 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_hotsearch.py
--rw-rw-rw-   0        0        0     3121 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_material.py
--rw-rw-rw-   0        0        0     3611 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_messagemanager.py
--rw-rw-rw-   0        0        0     1560 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_noticemanager.py
--rw-rw-rw-   0        0        0     1960 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_question.py
--rw-rw-rw-   0        0        0      998 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_recruit.py
--rw-rw-rw-   0        0        0     2216 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_safecode.py
--rw-rw-rw-   0        0        0     3677 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_subject.py
--rw-rw-rw-   0        0        0     3368 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_subjectweb.py
--rw-rw-rw-   0        0        0     2290 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.884828 huhk-1.9.1/service/app_a/asserts/content/material/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/material/__init__.py
--rw-rw-rw-   0        0        0      717 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/material/asserts_content_material_getmateriallist.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.918492 huhk-1.9.1/service/app_a/asserts/goods/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/goods/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_area.py
--rw-rw-rw-   0        0        0     3208 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_carmodel.py
--rw-rw-rw-   0        0        0     2408 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_configure.py
--rw-rw-rw-   0        0        0     2048 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_ordermain.py
--rw-rw-rw-   0        0        0     1164 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.923480 huhk-1.9.1/service/app_a/asserts/manageapi/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.936444 huhk-1.9.1/service/app_a/asserts/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     1277 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/manageapi/order/asserts_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.940433 huhk-1.9.1/service/app_a/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.957388 huhk-1.9.1/service/app_a/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      625 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      613 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.985313 huhk-1.9.1/service/app_a/asserts/order/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/order/__init__.py
--rw-rw-rw-   0        0        0      824 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_freeorder.py
--rw-rw-rw-   0        0        0     7067 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_mainorder.py
--rw-rw-rw-   0        0        0     1428 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_order.py
--rw-rw-rw-   0        0        0     3268 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_rightsorder.py
--rw-rw-rw-   0        0        0     1108 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.994289 huhk-1.9.1/service/app_a/asserts/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0      704 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/mainorder/asserts_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.003920 huhk-1.9.1/service/app_a/asserts/order/rights/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/rights/__init__.py
--rw-rw-rw-   0        0        0     3944 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/order/rights/asserts_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.012895 huhk-1.9.1/service/app_a/asserts/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0      890 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/order/rightsorder/asserts_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.020873 huhk-1.9.1/service/app_a/asserts/pay/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/pay/__init__.py
--rw-rw-rw-   0        0        0      611 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/pay/asserts_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.046319 huhk-1.9.1/service/app_a/asserts/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.051305 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.067262 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0      817 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     2203 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     2272 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     1275 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     1163 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     1660 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.084221 huhk-1.9.1/service/app_a/asserts/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0      807 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0      783 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_pointsinfo.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.151282 huhk-1.9.1/service/app_a/funs/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:13:45.000000 huhk-1.9.1/service/app_a/funs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.163396 huhk-1.9.1/service/app_a/funs/admin/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/admin/__init__.py
--rw-rw-rw-   0        0        0     1065 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/admin/funs_admin_guc.py
--rw-rw-rw-   0        0        0      647 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/admin/funs_admin_spa.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.195342 huhk-1.9.1/service/app_a/funs/common/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/__init__.py
--rw-rw-rw-   0        0        0      928 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_clue.py
--rw-rw-rw-   0        0        0      709 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_common.py
--rw-rw-rw-   0        0        0     1795 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     2804 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_systemversion.py
--rw-rw-rw-   0        0        0      729 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_user.py
--rw-rw-rw-   0        0        0    21622 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_user4c.py
--rw-rw-rw-   0        0        0     6180 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.292315 huhk-1.9.1/service/app_a/funs/content/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/__init__.py
--rw-rw-rw-   0        0        0    26429 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_activitymanager.py
--rw-rw-rw-   0        0        0    11631 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_adv.py
--rw-rw-rw-   0        0        0     1482 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_advplace.py
--rw-rw-rw-   0        0        0     7550 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_agreement.py
--rw-rw-rw-   0        0        0     8084 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_campmanager.py
--rw-rw-rw-   0        0        0     7904 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_comment.py
--rw-rw-rw-   0        0        0     7209 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_commonquestion.py
--rw-rw-rw-   0        0        0     1082 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_contentmanager.py
--rw-rw-rw-   0        0        0    13476 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_essay.py
--rw-rw-rw-   0        0        0     1526 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_essaycomment.py
--rw-rw-rw-   0        0        0     4715 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_essayweb.py
--rw-rw-rw-   0        0        0      694 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_hotcity.py
--rw-rw-rw-   0        0        0     2656 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_hotsearch.py
--rw-rw-rw-   0        0        0     5431 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_material.py
--rw-rw-rw-   0        0        0    10631 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_messagemanager.py
--rw-rw-rw-   0        0        0     2868 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_noticemanager.py
--rw-rw-rw-   0        0        0     4376 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_question.py
--rw-rw-rw-   0        0        0     1529 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_recruit.py
--rw-rw-rw-   0        0        0     3317 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_safecode.py
--rw-rw-rw-   0        0        0     8951 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_subject.py
--rw-rw-rw-   0        0        0     9433 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_subjectweb.py
--rw-rw-rw-   0        0        0     4900 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.302564 huhk-1.9.1/service/app_a/funs/content/material/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/material/__init__.py
--rw-rw-rw-   0        0        0     1219 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/material/funs_content_material_getmateriallist.py
--rw-rw-rw-   0        0        0     1130 2023-07-31 07:13:45.000000 huhk-1.9.1/service/app_a/funs/funs_activitymanager.py
--rw-rw-rw-   0        0        0      194 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_admin.py
--rw-rw-rw-   0        0        0     3167 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/funs_app_a.py
--rw-rw-rw-   0        0        0      599 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_area.py
--rw-rw-rw-   0        0        0      761 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_common.py
--rw-rw-rw-   0        0        0     3101 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/funs_content.py
--rw-rw-rw-   0        0        0     2527 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_essay.py
--rw-rw-rw-   0        0        0      506 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_goods.py
--rw-rw-rw-   0        0        0      140 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_manageapi.py
--rw-rw-rw-   0        0        0      118 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_open.py
--rw-rw-rw-   0        0        0      607 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_order.py
--rw-rw-rw-   0        0        0      131 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_pay.py
--rw-rw-rw-   0        0        0      698 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/funs_radarpoints.py
--rw-rw-rw-   0        0        0     2813 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.329491 huhk-1.9.1/service/app_a/funs/goods/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/goods/__init__.py
--rw-rw-rw-   0        0        0     6559 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_area.py
--rw-rw-rw-   0        0        0    11252 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_carmodel.py
--rw-rw-rw-   0        0        0    10293 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_configure.py
--rw-rw-rw-   0        0        0     5322 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_ordermain.py
--rw-rw-rw-   0        0        0     3626 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.339469 huhk-1.9.1/service/app_a/funs/manageapi/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/manageapi/__init__.py
--rw-rw-rw-   0        0        0      179 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/manageapi/funs_manageapi_order.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.348448 huhk-1.9.1/service/app_a/funs/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     4282 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/manageapi/order/funs_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.356421 huhk-1.9.1/service/app_a/funs/open/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/__init__.py
--rw-rw-rw-   0        0        0      267 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/funs_open_haohan.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.368389 huhk-1.9.1/service/app_a/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      869 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/haohan/funs_open_haohan_relation.py
--rw-rw-rw-   0        0        0      959 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/haohan/funs_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.395313 huhk-1.9.1/service/app_a/funs/order/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/__init__.py
--rw-rw-rw-   0        0        0     3970 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_freeorder.py
--rw-rw-rw-   0        0        0    19335 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_mainorder.py
--rw-rw-rw-   0        0        0     2770 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_order.py
--rw-rw-rw-   0        0        0      176 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_rights.py
--rw-rw-rw-   0        0        0    12237 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_rightsorder.py
--rw-rw-rw-   0        0        0     2884 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.403292 huhk-1.9.1/service/app_a/funs/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0     1373 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/mainorder/funs_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.412884 huhk-1.9.1/service/app_a/funs/order/rights/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/rights/__init__.py
--rw-rw-rw-   0        0        0     9168 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/rights/funs_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.421088 huhk-1.9.1/service/app_a/funs/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0     3959 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/rightsorder/funs_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.430071 huhk-1.9.1/service/app_a/funs/pay/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/pay/__init__.py
--rw-rw-rw-   0        0        0      900 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/pay/funs_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.457744 huhk-1.9.1/service/app_a/funs/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.467715 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.482678 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     4080 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0     2099 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0      433 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/funs_radarpoints_adjustpoints_adjust.py
--rw-rw-rw-   0        0        0     5930 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     8017 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     4126 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     2339 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     7883 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.501624 huhk-1.9.1/service/app_a/funs/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0     2169 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_pointsinfo.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.536537 huhk-1.9.1/service/app_a/sqls/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.551214 huhk-1.9.1/service/app_a/sqls/admin/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/admin/__init__.py
--rw-rw-rw-   0        0        0     1026 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/admin/sqls_admin_guc.py
--rw-rw-rw-   0        0        0      552 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/admin/sqls_admin_spa.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.582131 huhk-1.9.1/service/app_a/sqls/common/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/__init__.py
--rw-rw-rw-   0        0        0      563 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_clue.py
--rw-rw-rw-   0        0        0      562 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_common.py
--rw-rw-rw-   0        0        0      586 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     1050 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_systemversion.py
--rw-rw-rw-   0        0        0      563 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_user.py
--rw-rw-rw-   0        0        0     6794 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_user4c.py
--rw-rw-rw-   0        0        0     2069 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.663639 huhk-1.9.1/service/app_a/sqls/content/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/content/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.672615 huhk-1.9.1/service/app_a/sqls/content/material/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/material/__init__.py
--rw-rw-rw-   0        0        0      602 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/material/sqls_content_material_getmateriallist.py
--rw-rw-rw-   0        0        0     7456 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_activitymanager.py
--rw-rw-rw-   0        0        0     5815 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_adv.py
--rw-rw-rw-   0        0        0      568 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_advplace.py
--rw-rw-rw-   0        0        0     3943 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_agreement.py
--rw-rw-rw-   0        0        0     2981 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_campmanager.py
--rw-rw-rw-   0        0        0     2480 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_comment.py
--rw-rw-rw-   0        0        0     4458 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_commonquestion.py
--rw-rw-rw-   0        0        0      581 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_contentmanager.py
--rw-rw-rw-   0        0        0     4379 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_essay.py
--rw-rw-rw-   0        0        0      575 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_essaycomment.py
--rw-rw-rw-   0        0        0     2002 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_essayweb.py
--rw-rw-rw-   0        0        0      560 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_hotcity.py
--rw-rw-rw-   0        0        0     1520 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_hotsearch.py
--rw-rw-rw-   0        0        0     3466 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_material.py
--rw-rw-rw-   0        0        0     3504 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_messagemanager.py
--rw-rw-rw-   0        0        0     1564 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_noticemanager.py
--rw-rw-rw-   0        0        0     2022 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_question.py
--rw-rw-rw-   0        0        0     1037 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_recruit.py
--rw-rw-rw-   0        0        0     2474 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_safecode.py
--rw-rw-rw-   0        0        0     3917 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_subject.py
--rw-rw-rw-   0        0        0     3455 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_subjectweb.py
--rw-rw-rw-   0        0        0     2470 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.697550 huhk-1.9.1/service/app_a/sqls/goods/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/goods/__init__.py
--rw-rw-rw-   0        0        0     3904 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_area.py
--rw-rw-rw-   0        0        0     3000 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_carmodel.py
--rw-rw-rw-   0        0        0     2521 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_configure.py
--rw-rw-rw-   0        0        0     2016 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_ordermain.py
--rw-rw-rw-   0        0        0     1043 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.702538 huhk-1.9.1/service/app_a/sqls/manageapi/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.711513 huhk-1.9.1/service/app_a/sqls/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/manageapi/order/sqls_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.716498 huhk-1.9.1/service/app_a/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.729856 huhk-1.9.1/service/app_a/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.754771 huhk-1.9.1/service/app_a/sqls/order/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/order/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.764748 huhk-1.9.1/service/app_a/sqls/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0      590 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/mainorder/sqls_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.772724 huhk-1.9.1/service/app_a/sqls/order/rights/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/rights/__init__.py
--rw-rw-rw-   0        0        0     4025 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/order/rights/sqls_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.779504 huhk-1.9.1/service/app_a/sqls/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0      581 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/order/rightsorder/sqls_order_rightsorder_receive.py
--rw-rw-rw-   0        0        0      564 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_freeorder.py
--rw-rw-rw-   0        0        0     7363 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_mainorder.py
--rw-rw-rw-   0        0        0     1511 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_order.py
--rw-rw-rw-   0        0        0     2972 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_rightsorder.py
--rw-rw-rw-   0        0        0     1045 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.786515 huhk-1.9.1/service/app_a/sqls/pay/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/pay/__init__.py
--rw-rw-rw-   0        0        0      569 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/pay/sqls_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.806530 huhk-1.9.1/service/app_a/sqls/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.809522 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.822515 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0      604 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     2076 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     2046 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     1062 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     1083 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     1062 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.831978 huhk-1.9.1/service/app_a/sqls/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0      603 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0      599 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_pointsinfo.py
--rw-rw-rw-   0        0        0      574 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/sqls_activitymanager.py
--rw-rw-rw-   0        0        0      534 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/sqls_app_a.py
--rw-rw-rw-   0        0        0      546 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/sqls_area.py
--rw-rw-rw-   0        0        0      545 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/sqls_content.py
--rw-rw-rw-   0        0        0     1017 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/sqls_essay.py
--rw-rw-rw-   0        0        0      554 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/sqls_testdrive.py
--rw-rw-rw-   0        0        0       42 2023-08-01 01:44:39.852923 huhk-1.9.1/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.834970 huhk-1.9.1/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:02:47.000000 huhk-1.9.1/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.846910 huhk-1.9.1/testcase/app_a/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:02:47.000000 huhk-1.9.1/testcase/app_a/__init__.py
--rw-rw-rw-   0        0        0      361 2023-07-31 06:02:47.000000 huhk-1.9.1/testcase/app_a/conftest.py
--rw-rw-rw-   0        0        0     3184 2023-07-31 07:18:01.000000 huhk-1.9.1/testcase/app_a/test_page.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.396827 huhk-1.9.2/
+-rw-rw-rw-   0        0        0      223 2023-08-01 01:48:15.395812 huhk-1.9.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.324786 huhk-1.9.2/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.2/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.355665 huhk-1.9.2/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.9.2/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    21531 2023-07-31 07:13:40.000000 huhk-1.9.2/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     1337 2023-08-01 01:47:29.000000 huhk-1.9.2/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    18567 2023-07-31 08:18:51.000000 huhk-1.9.2/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.9.2/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-08-01 01:48:13.000000 huhk-1.9.2/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0     9925 2023-07-31 05:34:49.000000 huhk-1.9.2/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.9.2/huhk/main.py
+-rw-rw-rw-   0        0        0      338 2023-08-01 01:48:08.000000 huhk-1.9.2/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.356664 huhk-1.9.2/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.392820 huhk-1.9.2/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.2/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.9.2/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.9.2/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.2/huhk/unit_data.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    28964 2023-08-01 01:47:59.000000 huhk-1.9.2/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.9.2/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.9.2/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.336715 huhk-1.9.2/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 01:48:15.396827 huhk-1.9.2/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.9.2/setup.py
```

### Comparing `huhk-1.9.1/huhk/__init__.py` & `huhk-1.9.2/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/case_project/json_coder.py` & `huhk-1.9.2/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/case_project/main_fun.py` & `huhk-1.9.2/huhk/case_project/main_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/case_project/project_base.py` & `huhk-1.9.2/huhk/case_project/project_base.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/case_project/project_init.py` & `huhk-1.9.2/huhk/case_project/project_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from huhk import projects_path, admin_host
 from huhk.unit_dict import Dict
-from unit_data import size_names, page_names, before_names, end_names, page_and_size
+from huhk.unit_data import size_names, page_names, before_names, end_names, page_and_size
 
 
 class ProjectInIt:
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         """api_type: 0时，value是swagger的api，json的url
                      1时，value值为yapi项目token,
                      2时，value是yapi下载的json文件名，文件放在file目录下,
```

### Comparing `huhk-1.9.1/huhk/case_project/project_string.py` & `huhk-1.9.2/huhk/case_project/project_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/case_project/setup_set.py` & `huhk-1.9.2/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/init_project.py` & `huhk-1.9.2/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/main.py` & `huhk-1.9.2/huhk/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/beam_class.py` & `huhk-1.9.2/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/data.py` & `huhk-1.9.2/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/par_do.py` & `huhk-1.9.2/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.9.2/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/test_fiter.py` & `huhk-1.9.2/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/test_flatmap.py` & `huhk-1.9.2/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/test_map.py` & `huhk-1.9.2/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/test_par_do.py` & `huhk-1.9.2/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/test_regex.py` & `huhk-1.9.2/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/testcase/apache/test_time.py` & `huhk-1.9.2/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/unit_apache_beam.py` & `huhk-1.9.2/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/unit_dict.py` & `huhk-1.9.2/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/unit_encryption.py` & `huhk-1.9.2/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/unit_fun.py` & `huhk-1.9.2/huhk/unit_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import inspect
 import os
 import re
 import random
 import time
-from operator import methodcaller
-
 import requests
 import datetime
-# import pymysql
 from pandas import DataFrame, ExcelWriter
 from typing import List
 from faker import Faker
 
 from huhk.unit_dict import Dict
 from huhk.unit_logger import logger
-from unit_data import page_and_size, before_and_end, before_and_end_re_str
+from huhk.unit_data import page_and_size, before_and_end_re_str
 
 
 class FunBase:
     def __init__(self):
         self._time2 = 0
         self._time1 = 0
         self.sql_str = ""
```

### Comparing `huhk-1.9.1/huhk/unit_logger.py` & `huhk-1.9.2/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/unit_request.py` & `huhk-1.9.2/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/unit_tasks.py` & `huhk-1.9.2/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.1/huhk/常用命令.py` & `huhk-1.9.2/huhk/常用命令.py`

 * *Files identical despite different names*

