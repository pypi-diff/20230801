# Comparing `tmp/huhk-1.9.5.tar.gz` & `tmp/huhk-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.9.5.tar", last modified: Tue Aug  1 02:07:27 2023, max compression
+gzip compressed data, was "huhk-1.9.6.tar", last modified: Tue Aug  1 02:51:39 2023, max compression
```

## Comparing `huhk-1.9.5.tar` & `huhk-1.9.6.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.637168 huhk-1.9.5/
--rw-rw-rw-   0        0        0      223 2023-08-01 02:07:27.635175 huhk-1.9.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.444543 huhk-1.9.5/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.5/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.488401 huhk-1.9.5/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.9.5/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    21538 2023-08-01 01:55:58.000000 huhk-1.9.5/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     1369 2023-08-01 02:06:27.000000 huhk-1.9.5/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    18567 2023-07-31 08:18:51.000000 huhk-1.9.5/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.9.5/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-08-01 02:07:25.000000 huhk-1.9.5/huhk/case_project/version.py
--rw-rw-rw-   0        0        0     9925 2023-07-31 05:34:49.000000 huhk-1.9.5/huhk/init_project.py
--rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.9.5/huhk/main.py
--rw-rw-rw-   0        0        0      338 2023-08-01 01:48:08.000000 huhk-1.9.5/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.491420 huhk-1.9.5/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.539337 huhk-1.9.5/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.5/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.9.5/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.9.5/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.9.5/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.9.5/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.9.5/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.9.5/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.9.5/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.9.5/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.9.5/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.5/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.5/huhk/unit_data.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28964 2023-08-01 01:47:59.000000 huhk-1.9.5/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.9.5/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.9.5/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.5/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.462503 huhk-1.9.5/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-08-01 02:07:26.000000 huhk-1.9.5/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19653 2023-08-01 02:07:26.000000 huhk-1.9.5/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:07:26.000000 huhk-1.9.5/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-01 02:07:26.000000 huhk-1.9.5/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-08-01 02:07:26.000000 huhk-1.9.5/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-08-01 02:07:26.000000 huhk-1.9.5/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.543359 huhk-1.9.5/service/
--rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.5/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.549315 huhk-1.9.5/service/app_a/
--rw-rw-rw-   0        0        0      420 2023-08-01 01:48:49.000000 huhk-1.9.5/service/app_a/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.572246 huhk-1.9.5/service/app_a/apis/
--rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.5/service/app_a/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.583218 huhk-1.9.5/service/app_a/apis/admin/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/admin/__init__.py
--rw-rw-rw-   0        0        0     1603 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/admin/apis_admin_guc.py
--rw-rw-rw-   0        0        0      784 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/admin/apis_admin_spa.py
--rw-rw-rw-   0        0        0     1105 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/apis_activitymanager.py
--rw-rw-rw-   0        0        0     2049 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/apis_app_a.py
--rw-rw-rw-   0        0        0     1072 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/apis_area.py
--rw-rw-rw-   0        0        0      914 2023-08-01 02:06:49.000000 huhk-1.9.5/service/app_a/apis/apis_content.py
--rw-rw-rw-   0        0        0     2511 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/apis_essay.py
--rw-rw-rw-   0        0        0     2187 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/apis_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.610991 huhk-1.9.5/service/app_a/apis/common/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/common/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-08-01 02:06:45.000000 huhk-1.9.5/service/app_a/apis/common/apis_common_clue.py
--rw-rw-rw-   0        0        0     1071 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/common/apis_common_common.py
--rw-rw-rw-   0        0        0     1945 2023-08-01 02:06:45.000000 huhk-1.9.5/service/app_a/apis/common/apis_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     2922 2023-08-01 02:06:45.000000 huhk-1.9.5/service/app_a/apis/common/apis_common_systemversion.py
--rw-rw-rw-   0        0        0      867 2023-08-01 02:06:45.000000 huhk-1.9.5/service/app_a/apis/common/apis_common_user.py
--rw-rw-rw-   0        0        0    25061 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/apis/common/apis_common_user4c.py
--rw-rw-rw-   0        0        0     5938 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/apis/common/apis_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.677258 huhk-1.9.5/service/app_a/apis/content/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/content/__init__.py
--rw-rw-rw-   0        0        0    26441 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_activitymanager.py
--rw-rw-rw-   0        0        0    13587 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_adv.py
--rw-rw-rw-   0        0        0     1184 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_advplace.py
--rw-rw-rw-   0        0        0    10283 2023-08-01 02:06:50.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_agreement.py
--rw-rw-rw-   0        0        0     8389 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_campmanager.py
--rw-rw-rw-   0        0        0     7639 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_comment.py
--rw-rw-rw-   0        0        0     8748 2023-08-01 02:06:50.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_commonquestion.py
--rw-rw-rw-   0        0        0     1419 2023-08-01 02:06:50.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_contentmanager.py
--rw-rw-rw-   0        0        0    14248 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_essay.py
--rw-rw-rw-   0        0        0     1317 2023-08-01 02:06:50.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_essaycomment.py
--rw-rw-rw-   0        0        0     4566 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_essayweb.py
--rw-rw-rw-   0        0        0      859 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_hotcity.py
--rw-rw-rw-   0        0        0     2952 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_hotsearch.py
--rw-rw-rw-   0        0        0     6682 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_material.py
--rw-rw-rw-   0        0        0     9450 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_messagemanager.py
--rw-rw-rw-   0        0        0     3576 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_noticemanager.py
--rw-rw-rw-   0        0        0     5813 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_question.py
--rw-rw-rw-   0        0        0     2008 2023-08-01 02:06:50.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_recruit.py
--rw-rw-rw-   0        0        0     5100 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_safecode.py
--rw-rw-rw-   0        0        0     9825 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_subject.py
--rw-rw-rw-   0        0        0     9388 2023-08-01 02:06:51.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_subjectweb.py
--rw-rw-rw-   0        0        0     6365 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/content/apis_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.684240 huhk-1.9.5/service/app_a/apis/content/material/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/apis/content/material/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/apis/content/material/apis_content_material_getmateriallist.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.701250 huhk-1.9.5/service/app_a/apis/goods/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/goods/__init__.py
--rw-rw-rw-   0        0        0     9854 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/goods/apis_goods_area.py
--rw-rw-rw-   0        0        0    12191 2023-08-01 02:06:49.000000 huhk-1.9.5/service/app_a/apis/goods/apis_goods_carmodel.py
--rw-rw-rw-   0        0        0    10643 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/goods/apis_goods_configure.py
--rw-rw-rw-   0        0        0     6170 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/goods/apis_goods_ordermain.py
--rw-rw-rw-   0        0        0     3147 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/goods/apis_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.703249 huhk-1.9.5/service/app_a/apis/manageapi/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.710262 huhk-1.9.5/service/app_a/apis/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     8140 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/manageapi/order/apis_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.713225 huhk-1.9.5/service/app_a/apis/open/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.722200 huhk-1.9.5/service/app_a/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      816 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0      849 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.738780 huhk-1.9.5/service/app_a/apis/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:44.000000 huhk-1.9.5/service/app_a/apis/order/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/order/apis_order_freeorder.py
--rw-rw-rw-   0        0        0    23046 2023-08-01 02:06:48.000000 huhk-1.9.5/service/app_a/apis/order/apis_order_mainorder.py
--rw-rw-rw-   0        0        0     3724 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/order/apis_order_order.py
--rw-rw-rw-   0        0        0    11987 2023-08-01 02:06:48.000000 huhk-1.9.5/service/app_a/apis/order/apis_order_rightsorder.py
--rw-rw-rw-   0        0        0     2582 2023-08-01 02:06:52.000000 huhk-1.9.5/service/app_a/apis/order/apis_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.745361 huhk-1.9.5/service/app_a/apis/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:48.000000 huhk-1.9.5/service/app_a/apis/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0     1125 2023-08-01 02:06:48.000000 huhk-1.9.5/service/app_a/apis/order/mainorder/apis_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.751342 huhk-1.9.5/service/app_a/apis/order/rights/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:48.000000 huhk-1.9.5/service/app_a/apis/order/rights/__init__.py
--rw-rw-rw-   0        0        0    10735 2023-08-01 02:06:48.000000 huhk-1.9.5/service/app_a/apis/order/rights/apis_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.758922 huhk-1.9.5/service/app_a/apis/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:48.000000 huhk-1.9.5/service/app_a/apis/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-08-01 02:06:48.000000 huhk-1.9.5/service/app_a/apis/order/rightsorder/apis_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.764897 huhk-1.9.5/service/app_a/apis/pay/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/pay/__init__.py
--rw-rw-rw-   0        0        0      865 2023-08-01 02:06:47.000000 huhk-1.9.5/service/app_a/apis/pay/apis_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.783846 huhk-1.9.5/service/app_a/apis/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.787836 huhk-1.9.5/service/app_a/apis/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.798806 huhk-1.9.5/service/app_a/apis/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     3883 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0     1699 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     6180 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     7225 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     3763 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     2247 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     6270 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.809780 huhk-1.9.5/service/app_a/apis/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0     1871 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0     2061 2023-08-01 02:06:46.000000 huhk-1.9.5/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_pointsinfo.py
--rw-rw-rw-   0        0        0      752 2023-08-01 01:48:49.000000 huhk-1.9.5/service/app_a/app_a_fun.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.830724 huhk-1.9.5/service/app_a/asserts/
--rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.5/service/app_a/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.842132 huhk-1.9.5/service/app_a/asserts/admin/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/admin/__init__.py
--rw-rw-rw-   0        0        0      941 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/admin/asserts_admin_guc.py
--rw-rw-rw-   0        0        0      552 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/admin/asserts_admin_spa.py
--rw-rw-rw-   0        0        0      626 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/asserts_activitymanager.py
--rw-rw-rw-   0        0        0      653 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/asserts_app_a.py
--rw-rw-rw-   0        0        0      525 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/asserts_area.py
--rw-rw-rw-   0        0        0      536 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/asserts/asserts_content.py
--rw-rw-rw-   0        0        0     1009 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/asserts/asserts_essay.py
--rw-rw-rw-   0        0        0      707 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/asserts_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.867642 huhk-1.9.5/service/app_a/asserts/common/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/common/__init__.py
--rw-rw-rw-   0        0        0      587 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/common/asserts_common_clue.py
--rw-rw-rw-   0        0        0      581 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/asserts/common/asserts_common_common.py
--rw-rw-rw-   0        0        0      714 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/common/asserts_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     1116 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/common/asserts_common_systemversion.py
--rw-rw-rw-   0        0        0      579 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/common/asserts_common_user.py
--rw-rw-rw-   0        0        0     6848 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/common/asserts_common_user4c.py
--rw-rw-rw-   0        0        0     2174 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/common/asserts_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.929397 huhk-1.9.5/service/app_a/asserts/content/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/content/__init__.py
--rw-rw-rw-   0        0        0     7782 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_activitymanager.py
--rw-rw-rw-   0        0        0     5226 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_adv.py
--rw-rw-rw-   0        0        0      653 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_advplace.py
--rw-rw-rw-   0        0        0     3600 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_agreement.py
--rw-rw-rw-   0        0        0     2959 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_campmanager.py
--rw-rw-rw-   0        0        0     2532 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_comment.py
--rw-rw-rw-   0        0        0     4032 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_commonquestion.py
--rw-rw-rw-   0        0        0      649 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_contentmanager.py
--rw-rw-rw-   0        0        0     4302 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_essay.py
--rw-rw-rw-   0        0        0      664 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_essaycomment.py
--rw-rw-rw-   0        0        0     1937 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_essayweb.py
--rw-rw-rw-   0        0        0      582 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_hotcity.py
--rw-rw-rw-   0        0        0     1432 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_hotsearch.py
--rw-rw-rw-   0        0        0     3121 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_material.py
--rw-rw-rw-   0        0        0     3611 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_messagemanager.py
--rw-rw-rw-   0        0        0     1560 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_noticemanager.py
--rw-rw-rw-   0        0        0     1960 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_question.py
--rw-rw-rw-   0        0        0      998 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_recruit.py
--rw-rw-rw-   0        0        0     2216 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_safecode.py
--rw-rw-rw-   0        0        0     3677 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_subject.py
--rw-rw-rw-   0        0        0     3368 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_subjectweb.py
--rw-rw-rw-   0        0        0     2290 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/content/asserts_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.934411 huhk-1.9.5/service/app_a/asserts/content/material/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/content/material/__init__.py
--rw-rw-rw-   0        0        0      717 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/content/material/asserts_content_material_getmateriallist.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.951932 huhk-1.9.5/service/app_a/asserts/goods/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/goods/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_area.py
--rw-rw-rw-   0        0        0     3208 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_carmodel.py
--rw-rw-rw-   0        0        0     2408 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_configure.py
--rw-rw-rw-   0        0        0     2048 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_ordermain.py
--rw-rw-rw-   0        0        0     1164 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.954923 huhk-1.9.5/service/app_a/asserts/manageapi/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.963516 huhk-1.9.5/service/app_a/asserts/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     1277 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/manageapi/order/asserts_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.966506 huhk-1.9.5/service/app_a/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.979470 huhk-1.9.5/service/app_a/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      625 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      613 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:26.999418 huhk-1.9.5/service/app_a/asserts/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/order/__init__.py
--rw-rw-rw-   0        0        0      824 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/order/asserts_order_freeorder.py
--rw-rw-rw-   0        0        0     7067 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/order/asserts_order_mainorder.py
--rw-rw-rw-   0        0        0     1428 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/order/asserts_order_order.py
--rw-rw-rw-   0        0        0     3268 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/asserts/order/asserts_order_rightsorder.py
--rw-rw-rw-   0        0        0     1108 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/asserts/order/asserts_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.006398 huhk-1.9.5/service/app_a/asserts/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0      704 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/order/mainorder/asserts_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.013381 huhk-1.9.5/service/app_a/asserts/order/rights/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/order/rights/__init__.py
--rw-rw-rw-   0        0        0     3944 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/asserts/order/rights/asserts_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.020362 huhk-1.9.5/service/app_a/asserts/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/asserts/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0      890 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/asserts/order/rightsorder/asserts_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.027342 huhk-1.9.5/service/app_a/asserts/pay/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/pay/__init__.py
--rw-rw-rw-   0        0        0      611 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/pay/asserts_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.047291 huhk-1.9.5/service/app_a/asserts/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.050309 huhk-1.9.5/service/app_a/asserts/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.061111 huhk-1.9.5/service/app_a/asserts/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0      817 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     2203 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     2272 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     1275 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     1163 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     1660 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.069752 huhk-1.9.5/service/app_a/asserts/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0      807 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0      783 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_pointsinfo.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.107671 huhk-1.9.5/service/app_a/funs/
--rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.5/service/app_a/funs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.116074 huhk-1.9.5/service/app_a/funs/admin/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/admin/__init__.py
--rw-rw-rw-   0        0        0     1065 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/admin/funs_admin_guc.py
--rw-rw-rw-   0        0        0      647 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/admin/funs_admin_spa.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.136018 huhk-1.9.5/service/app_a/funs/common/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/common/__init__.py
--rw-rw-rw-   0        0        0      928 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/common/funs_common_clue.py
--rw-rw-rw-   0        0        0      709 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/funs/common/funs_common_common.py
--rw-rw-rw-   0        0        0     1795 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/common/funs_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     2804 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/common/funs_common_systemversion.py
--rw-rw-rw-   0        0        0      729 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/common/funs_common_user.py
--rw-rw-rw-   0        0        0    21622 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/common/funs_common_user4c.py
--rw-rw-rw-   0        0        0     6180 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/common/funs_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.199617 huhk-1.9.5/service/app_a/funs/content/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/content/__init__.py
--rw-rw-rw-   0        0        0    26429 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_activitymanager.py
--rw-rw-rw-   0        0        0    11631 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_adv.py
--rw-rw-rw-   0        0        0     1482 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_advplace.py
--rw-rw-rw-   0        0        0     7550 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_agreement.py
--rw-rw-rw-   0        0        0     8084 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_campmanager.py
--rw-rw-rw-   0        0        0     7904 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_comment.py
--rw-rw-rw-   0        0        0     7209 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_commonquestion.py
--rw-rw-rw-   0        0        0     1082 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_contentmanager.py
--rw-rw-rw-   0        0        0    13476 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_essay.py
--rw-rw-rw-   0        0        0     1526 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_essaycomment.py
--rw-rw-rw-   0        0        0     4715 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_essayweb.py
--rw-rw-rw-   0        0        0      694 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_hotcity.py
--rw-rw-rw-   0        0        0     2656 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_hotsearch.py
--rw-rw-rw-   0        0        0     5431 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_material.py
--rw-rw-rw-   0        0        0    10631 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_messagemanager.py
--rw-rw-rw-   0        0        0     2868 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_noticemanager.py
--rw-rw-rw-   0        0        0     4376 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_question.py
--rw-rw-rw-   0        0        0     1529 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_recruit.py
--rw-rw-rw-   0        0        0     3317 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_safecode.py
--rw-rw-rw-   0        0        0     8951 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_subject.py
--rw-rw-rw-   0        0        0     9433 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_subjectweb.py
--rw-rw-rw-   0        0        0     4900 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/content/funs_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.205598 huhk-1.9.5/service/app_a/funs/content/material/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/content/material/__init__.py
--rw-rw-rw-   0        0        0     1219 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/content/material/funs_content_material_getmateriallist.py
--rw-rw-rw-   0        0        0     1130 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/funs_activitymanager.py
--rw-rw-rw-   0        0        0      194 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/funs_admin.py
--rw-rw-rw-   0        0        0     3167 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/funs_app_a.py
--rw-rw-rw-   0        0        0      599 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/funs_area.py
--rw-rw-rw-   0        0        0      761 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/funs_common.py
--rw-rw-rw-   0        0        0     3099 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/funs_content.py
--rw-rw-rw-   0        0        0     2527 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/funs/funs_essay.py
--rw-rw-rw-   0        0        0      506 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/funs_goods.py
--rw-rw-rw-   0        0        0      140 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/funs_manageapi.py
--rw-rw-rw-   0        0        0      118 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/funs_open.py
--rw-rw-rw-   0        0        0      607 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/funs_order.py
--rw-rw-rw-   0        0        0      131 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/funs_pay.py
--rw-rw-rw-   0        0        0      698 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/funs_radarpoints.py
--rw-rw-rw-   0        0        0     2813 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/funs_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.225546 huhk-1.9.5/service/app_a/funs/goods/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/goods/__init__.py
--rw-rw-rw-   0        0        0     6559 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/goods/funs_goods_area.py
--rw-rw-rw-   0        0        0    11252 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/funs/goods/funs_goods_carmodel.py
--rw-rw-rw-   0        0        0    10293 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/goods/funs_goods_configure.py
--rw-rw-rw-   0        0        0     5322 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/goods/funs_goods_ordermain.py
--rw-rw-rw-   0        0        0     3626 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/goods/funs_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.231529 huhk-1.9.5/service/app_a/funs/manageapi/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/manageapi/__init__.py
--rw-rw-rw-   0        0        0      179 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/manageapi/funs_manageapi_order.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.238547 huhk-1.9.5/service/app_a/funs/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     4282 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/manageapi/order/funs_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.245493 huhk-1.9.5/service/app_a/funs/open/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/open/__init__.py
--rw-rw-rw-   0        0        0      267 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/open/funs_open_haohan.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.255466 huhk-1.9.5/service/app_a/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      869 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/open/haohan/funs_open_haohan_relation.py
--rw-rw-rw-   0        0        0      959 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/open/haohan/funs_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.275012 huhk-1.9.5/service/app_a/funs/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/order/__init__.py
--rw-rw-rw-   0        0        0     3970 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/order/funs_order_freeorder.py
--rw-rw-rw-   0        0        0    19335 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/order/funs_order_mainorder.py
--rw-rw-rw-   0        0        0     2770 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/order/funs_order_order.py
--rw-rw-rw-   0        0        0      176 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/order/funs_order_rights.py
--rw-rw-rw-   0        0        0    12237 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/funs/order/funs_order_rightsorder.py
--rw-rw-rw-   0        0        0     2884 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/funs/order/funs_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.280995 huhk-1.9.5/service/app_a/funs/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0     1373 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/order/mainorder/funs_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.288643 huhk-1.9.5/service/app_a/funs/order/rights/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/order/rights/__init__.py
--rw-rw-rw-   0        0        0     9168 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/funs/order/rights/funs_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.294615 huhk-1.9.5/service/app_a/funs/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/funs/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0     3959 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/funs/order/rightsorder/funs_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.300599 huhk-1.9.5/service/app_a/funs/pay/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/pay/__init__.py
--rw-rw-rw-   0        0        0      900 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/pay/funs_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.317555 huhk-1.9.5/service/app_a/funs/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.323539 huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.332515 huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     4080 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0     2099 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0      433 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/funs_radarpoints_adjustpoints_adjust.py
--rw-rw-rw-   0        0        0     5930 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     8017 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     4126 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     2339 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     7881 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.342489 huhk-1.9.5/service/app_a/funs/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/funs/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0     2169 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_pointsinfo.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.364432 huhk-1.9.5/service/app_a/sqls/
--rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.5/service/app_a/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.374405 huhk-1.9.5/service/app_a/sqls/admin/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/admin/__init__.py
--rw-rw-rw-   0        0        0     1026 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/admin/sqls_admin_guc.py
--rw-rw-rw-   0        0        0      552 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/admin/sqls_admin_spa.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.400559 huhk-1.9.5/service/app_a/sqls/common/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/common/__init__.py
--rw-rw-rw-   0        0        0      563 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/common/sqls_common_clue.py
--rw-rw-rw-   0        0        0      562 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/sqls/common/sqls_common_common.py
--rw-rw-rw-   0        0        0      586 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/common/sqls_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     1050 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/common/sqls_common_systemversion.py
--rw-rw-rw-   0        0        0      563 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/common/sqls_common_user.py
--rw-rw-rw-   0        0        0     6794 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/common/sqls_common_user4c.py
--rw-rw-rw-   0        0        0     2069 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/common/sqls_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.480240 huhk-1.9.5/service/app_a/sqls/content/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/content/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.488219 huhk-1.9.5/service/app_a/sqls/content/material/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/content/material/__init__.py
--rw-rw-rw-   0        0        0      602 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/content/material/sqls_content_material_getmateriallist.py
--rw-rw-rw-   0        0        0     7456 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_activitymanager.py
--rw-rw-rw-   0        0        0     5815 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_adv.py
--rw-rw-rw-   0        0        0      568 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_advplace.py
--rw-rw-rw-   0        0        0     3943 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_agreement.py
--rw-rw-rw-   0        0        0     2981 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_campmanager.py
--rw-rw-rw-   0        0        0     2480 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_comment.py
--rw-rw-rw-   0        0        0     4458 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_commonquestion.py
--rw-rw-rw-   0        0        0      581 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_contentmanager.py
--rw-rw-rw-   0        0        0     4379 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_essay.py
--rw-rw-rw-   0        0        0      575 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_essaycomment.py
--rw-rw-rw-   0        0        0     2002 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_essayweb.py
--rw-rw-rw-   0        0        0      560 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_hotcity.py
--rw-rw-rw-   0        0        0     1520 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_hotsearch.py
--rw-rw-rw-   0        0        0     3466 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_material.py
--rw-rw-rw-   0        0        0     3504 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_messagemanager.py
--rw-rw-rw-   0        0        0     1564 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_noticemanager.py
--rw-rw-rw-   0        0        0     2022 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_question.py
--rw-rw-rw-   0        0        0     1037 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_recruit.py
--rw-rw-rw-   0        0        0     2474 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_safecode.py
--rw-rw-rw-   0        0        0     3917 2023-08-01 02:06:59.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_subject.py
--rw-rw-rw-   0        0        0     3455 2023-08-01 02:06:58.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_subjectweb.py
--rw-rw-rw-   0        0        0     2470 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/content/sqls_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.508218 huhk-1.9.5/service/app_a/sqls/goods/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/goods/__init__.py
--rw-rw-rw-   0        0        0     3904 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_area.py
--rw-rw-rw-   0        0        0     3000 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_carmodel.py
--rw-rw-rw-   0        0        0     2521 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_configure.py
--rw-rw-rw-   0        0        0     2016 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_ordermain.py
--rw-rw-rw-   0        0        0     1043 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.510215 huhk-1.9.5/service/app_a/sqls/manageapi/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.518037 huhk-1.9.5/service/app_a/sqls/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/manageapi/order/sqls_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.520995 huhk-1.9.5/service/app_a/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.530727 huhk-1.9.5/service/app_a/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.549811 huhk-1.9.5/service/app_a/sqls/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/order/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.556758 huhk-1.9.5/service/app_a/sqls/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0      590 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/order/mainorder/sqls_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.562741 huhk-1.9.5/service/app_a/sqls/order/rights/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/order/rights/__init__.py
--rw-rw-rw-   0        0        0     4025 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/sqls/order/rights/sqls_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.569724 huhk-1.9.5/service/app_a/sqls/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/sqls/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0      581 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/sqls/order/rightsorder/sqls_order_rightsorder_receive.py
--rw-rw-rw-   0        0        0      564 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/order/sqls_order_freeorder.py
--rw-rw-rw-   0        0        0     7363 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/order/sqls_order_mainorder.py
--rw-rw-rw-   0        0        0     1511 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/order/sqls_order_order.py
--rw-rw-rw-   0        0        0     2972 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/sqls/order/sqls_order_rightsorder.py
--rw-rw-rw-   0        0        0     1045 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/order/sqls_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.576740 huhk-1.9.5/service/app_a/sqls/pay/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/pay/__init__.py
--rw-rw-rw-   0        0        0      569 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/pay/sqls_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.595656 huhk-1.9.5/service/app_a/sqls/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.598647 huhk-1.9.5/service/app_a/sqls/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.609241 huhk-1.9.5/service/app_a/sqls/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0      604 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     2076 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     2046 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     1062 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     1083 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     1062 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.619218 huhk-1.9.5/service/app_a/sqls/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0      603 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0      599 2023-08-01 02:06:54.000000 huhk-1.9.5/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_pointsinfo.py
--rw-rw-rw-   0        0        0      574 2023-08-01 02:06:53.000000 huhk-1.9.5/service/app_a/sqls/sqls_activitymanager.py
--rw-rw-rw-   0        0        0      534 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/sqls_app_a.py
--rw-rw-rw-   0        0        0      546 2023-08-01 02:07:00.000000 huhk-1.9.5/service/app_a/sqls/sqls_area.py
--rw-rw-rw-   0        0        0      545 2023-08-01 02:06:56.000000 huhk-1.9.5/service/app_a/sqls/sqls_content.py
--rw-rw-rw-   0        0        0     1017 2023-08-01 02:06:57.000000 huhk-1.9.5/service/app_a/sqls/sqls_essay.py
--rw-rw-rw-   0        0        0      554 2023-08-01 02:06:55.000000 huhk-1.9.5/service/app_a/sqls/sqls_testdrive.py
--rw-rw-rw-   0        0        0       42 2023-08-01 02:07:27.637168 huhk-1.9.5/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.9.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.622208 huhk-1.9.5/testcase/
--rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.5/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:07:27.632180 huhk-1.9.5/testcase/app_a/
--rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.5/testcase/app_a/__init__.py
--rw-rw-rw-   0        0        0      361 2023-08-01 01:48:49.000000 huhk-1.9.5/testcase/app_a/conftest.py
--rw-rw-rw-   0        0        0     3184 2023-08-01 02:07:00.000000 huhk-1.9.5/testcase/app_a/test_page.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.957186 huhk-1.9.6/
+-rw-rw-rw-   0        0        0      223 2023-08-01 02:51:39.956323 huhk-1.9.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.004404 huhk-1.9.6/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.6/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.036353 huhk-1.9.6/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.9.6/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    21538 2023-08-01 01:55:58.000000 huhk-1.9.6/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     1369 2023-08-01 02:06:27.000000 huhk-1.9.6/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    18567 2023-07-31 08:18:51.000000 huhk-1.9.6/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.9.6/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0     9925 2023-07-31 05:34:49.000000 huhk-1.9.6/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.9.6/huhk/main.py
+-rw-rw-rw-   0        0        0      338 2023-08-01 01:48:08.000000 huhk-1.9.6/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.038376 huhk-1.9.6/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.078871 huhk-1.9.6/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.6/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.9.6/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.9.6/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.6/huhk/unit_data.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    29577 2023-08-01 02:47:41.000000 huhk-1.9.6/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.9.6/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.9.6/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.017436 huhk-1.9.6/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19653 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.081864 huhk-1.9.6/service/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.086814 huhk-1.9.6/service/app_a/
+-rw-rw-rw-   0        0        0      420 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.101076 huhk-1.9.6/service/app_a/apis/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.108058 huhk-1.9.6/service/app_a/apis/admin/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/admin/__init__.py
+-rw-rw-rw-   0        0        0     1603 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/admin/apis_admin_guc.py
+-rw-rw-rw-   0        0        0      784 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/admin/apis_admin_spa.py
+-rw-rw-rw-   0        0        0     1105 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/apis_activitymanager.py
+-rw-rw-rw-   0        0        0     2049 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/apis_app_a.py
+-rw-rw-rw-   0        0        0     1072 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/apis_area.py
+-rw-rw-rw-   0        0        0      914 2023-08-01 02:26:05.000000 huhk-1.9.6/service/app_a/apis/apis_content.py
+-rw-rw-rw-   0        0        0     2511 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/apis_essay.py
+-rw-rw-rw-   0        0        0     2187 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/apis_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.126036 huhk-1.9.6/service/app_a/apis/common/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/common/__init__.py
+-rw-rw-rw-   0        0        0     1422 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_clue.py
+-rw-rw-rw-   0        0        0     1071 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_common.py
+-rw-rw-rw-   0        0        0     1945 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_remoteinterfacelog.py
+-rw-rw-rw-   0        0        0     2922 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_systemversion.py
+-rw-rw-rw-   0        0        0      867 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_user.py
+-rw-rw-rw-   0        0        0    25061 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_user4c.py
+-rw-rw-rw-   0        0        0     5938 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_userpointsmanage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.175156 huhk-1.9.6/service/app_a/apis/content/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/content/__init__.py
+-rw-rw-rw-   0        0        0    26441 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_activitymanager.py
+-rw-rw-rw-   0        0        0    13587 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_adv.py
+-rw-rw-rw-   0        0        0     1184 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_advplace.py
+-rw-rw-rw-   0        0        0    10283 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_agreement.py
+-rw-rw-rw-   0        0        0     8389 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_campmanager.py
+-rw-rw-rw-   0        0        0     7639 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_comment.py
+-rw-rw-rw-   0        0        0     8748 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_commonquestion.py
+-rw-rw-rw-   0        0        0     1419 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_contentmanager.py
+-rw-rw-rw-   0        0        0    14248 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_essay.py
+-rw-rw-rw-   0        0        0     1317 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_essaycomment.py
+-rw-rw-rw-   0        0        0     4566 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_essayweb.py
+-rw-rw-rw-   0        0        0      859 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_hotcity.py
+-rw-rw-rw-   0        0        0     2952 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_hotsearch.py
+-rw-rw-rw-   0        0        0     6682 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_material.py
+-rw-rw-rw-   0        0        0     9450 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_messagemanager.py
+-rw-rw-rw-   0        0        0     3576 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_noticemanager.py
+-rw-rw-rw-   0        0        0     5813 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_question.py
+-rw-rw-rw-   0        0        0     2008 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_recruit.py
+-rw-rw-rw-   0        0        0     5100 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_safecode.py
+-rw-rw-rw-   0        0        0     9825 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_subject.py
+-rw-rw-rw-   0        0        0     9388 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_subjectweb.py
+-rw-rw-rw-   0        0        0     6365 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_topic4c.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.180116 huhk-1.9.6/service/app_a/apis/content/material/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/material/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/material/apis_content_material_getmateriallist.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.193117 huhk-1.9.6/service/app_a/apis/goods/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/goods/__init__.py
+-rw-rw-rw-   0        0        0     9854 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_area.py
+-rw-rw-rw-   0        0        0    12191 2023-08-01 02:26:05.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_carmodel.py
+-rw-rw-rw-   0        0        0    10643 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_configure.py
+-rw-rw-rw-   0        0        0     6170 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_ordermain.py
+-rw-rw-rw-   0        0        0     3147 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.195076 huhk-1.9.6/service/app_a/apis/manageapi/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/manageapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.200096 huhk-1.9.6/service/app_a/apis/manageapi/order/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/manageapi/order/__init__.py
+-rw-rw-rw-   0        0        0     8140 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/manageapi/order/apis_manageapi_order_mainorder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.202093 huhk-1.9.6/service/app_a/apis/open/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.210071 huhk-1.9.6/service/app_a/apis/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      816 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/open/haohan/apis_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      849 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/open/haohan/apis_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.223002 huhk-1.9.6/service/app_a/apis/order/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/order/__init__.py
+-rw-rw-rw-   0        0        0     2652 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_freeorder.py
+-rw-rw-rw-   0        0        0    23046 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_mainorder.py
+-rw-rw-rw-   0        0        0     3724 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_order.py
+-rw-rw-rw-   0        0        0    11987 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_rightsorder.py
+-rw-rw-rw-   0        0        0     2582 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.228016 huhk-1.9.6/service/app_a/apis/order/mainorder/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/mainorder/__init__.py
+-rw-rw-rw-   0        0        0     1125 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/mainorder/apis_order_mainorder_scrm2app.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.232976 huhk-1.9.6/service/app_a/apis/order/rights/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/rights/__init__.py
+-rw-rw-rw-   0        0        0    10735 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/rights/apis_order_rights_rightsmanager.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.237988 huhk-1.9.6/service/app_a/apis/order/rightsorder/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/rightsorder/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/rightsorder/apis_order_rightsorder_receive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.242976 huhk-1.9.6/service/app_a/apis/pay/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/pay/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/pay/apis_pay_orderpaybill.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.256456 huhk-1.9.6/service/app_a/apis/radarpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.258036 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.266044 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/__init__.py
+-rw-rw-rw-   0        0        0     3883 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_batch.py
+-rw-rw-rw-   0        0        0     1699 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_single.py
+-rw-rw-rw-   0        0        0     6180 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_adjustpoints.py
+-rw-rw-rw-   0        0        0     7225 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_pointsconfig.py
+-rw-rw-rw-   0        0        0     3763 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_pointstask.py
+-rw-rw-rw-   0        0        0     2247 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_summarystatistics.py
+-rw-rw-rw-   0        0        0     6270 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_userpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.273594 huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/__init__.py
+-rw-rw-rw-   0        0        0     1871 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_exchangeinfo.py
+-rw-rw-rw-   0        0        0     2061 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_pointsinfo.py
+-rw-rw-rw-   0        0        0      752 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/app_a_fun.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.288596 huhk-1.9.6/service/app_a/asserts/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.295539 huhk-1.9.6/service/app_a/asserts/admin/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/admin/__init__.py
+-rw-rw-rw-   0        0        0      941 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/admin/asserts_admin_guc.py
+-rw-rw-rw-   0        0        0      552 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/admin/asserts_admin_spa.py
+-rw-rw-rw-   0        0        0      626 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/asserts_activitymanager.py
+-rw-rw-rw-   0        0        0      653 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/asserts_app_a.py
+-rw-rw-rw-   0        0        0      525 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/asserts_area.py
+-rw-rw-rw-   0        0        0      536 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/asserts_content.py
+-rw-rw-rw-   0        0        0     1009 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/asserts_essay.py
+-rw-rw-rw-   0        0        0      707 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/asserts_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.320474 huhk-1.9.6/service/app_a/asserts/common/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/common/__init__.py
+-rw-rw-rw-   0        0        0      587 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_clue.py
+-rw-rw-rw-   0        0        0      581 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_common.py
+-rw-rw-rw-   0        0        0      714 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_remoteinterfacelog.py
+-rw-rw-rw-   0        0        0     1116 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_systemversion.py
+-rw-rw-rw-   0        0        0      579 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_user.py
+-rw-rw-rw-   0        0        0     6848 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_user4c.py
+-rw-rw-rw-   0        0        0     2174 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_userpointsmanage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.381025 huhk-1.9.6/service/app_a/asserts/content/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/content/__init__.py
+-rw-rw-rw-   0        0        0     7782 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_activitymanager.py
+-rw-rw-rw-   0        0        0     5226 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_adv.py
+-rw-rw-rw-   0        0        0      653 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_advplace.py
+-rw-rw-rw-   0        0        0     3600 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_agreement.py
+-rw-rw-rw-   0        0        0     2959 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_campmanager.py
+-rw-rw-rw-   0        0        0     2532 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_comment.py
+-rw-rw-rw-   0        0        0     4032 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_commonquestion.py
+-rw-rw-rw-   0        0        0      649 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_contentmanager.py
+-rw-rw-rw-   0        0        0     4302 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_essay.py
+-rw-rw-rw-   0        0        0      664 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_essaycomment.py
+-rw-rw-rw-   0        0        0     1937 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_essayweb.py
+-rw-rw-rw-   0        0        0      582 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_hotcity.py
+-rw-rw-rw-   0        0        0     1432 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_hotsearch.py
+-rw-rw-rw-   0        0        0     3121 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_material.py
+-rw-rw-rw-   0        0        0     3611 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_messagemanager.py
+-rw-rw-rw-   0        0        0     1560 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_noticemanager.py
+-rw-rw-rw-   0        0        0     1960 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_question.py
+-rw-rw-rw-   0        0        0      998 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_recruit.py
+-rw-rw-rw-   0        0        0     2216 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_safecode.py
+-rw-rw-rw-   0        0        0     3677 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_subject.py
+-rw-rw-rw-   0        0        0     3368 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_subjectweb.py
+-rw-rw-rw-   0        0        0     2290 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_topic4c.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.386551 huhk-1.9.6/service/app_a/asserts/content/material/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/material/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/material/asserts_content_material_getmateriallist.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.400514 huhk-1.9.6/service/app_a/asserts/goods/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/asserts/goods/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_area.py
+-rw-rw-rw-   0        0        0     3208 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_carmodel.py
+-rw-rw-rw-   0        0        0     2408 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_configure.py
+-rw-rw-rw-   0        0        0     2048 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_ordermain.py
+-rw-rw-rw-   0        0        0     1164 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.402508 huhk-1.9.6/service/app_a/asserts/manageapi/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/manageapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.408493 huhk-1.9.6/service/app_a/asserts/manageapi/order/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/manageapi/order/__init__.py
+-rw-rw-rw-   0        0        0     1277 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/manageapi/order/asserts_manageapi_order_mainorder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.410487 huhk-1.9.6/service/app_a/asserts/open/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.418466 huhk-1.9.6/service/app_a/asserts/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/open/haohan/asserts_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      613 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/open/haohan/asserts_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.432940 huhk-1.9.6/service/app_a/asserts/order/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/order/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_freeorder.py
+-rw-rw-rw-   0        0        0     7067 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_mainorder.py
+-rw-rw-rw-   0        0        0     1428 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_order.py
+-rw-rw-rw-   0        0        0     3268 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_rightsorder.py
+-rw-rw-rw-   0        0        0     1108 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.437927 huhk-1.9.6/service/app_a/asserts/order/mainorder/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/mainorder/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/mainorder/asserts_order_mainorder_scrm2app.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.443910 huhk-1.9.6/service/app_a/asserts/order/rights/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/rights/__init__.py
+-rw-rw-rw-   0        0        0     3944 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/rights/asserts_order_rights_rightsmanager.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.449898 huhk-1.9.6/service/app_a/asserts/order/rightsorder/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/rightsorder/__init__.py
+-rw-rw-rw-   0        0        0      890 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/rightsorder/asserts_order_rightsorder_receive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.456884 huhk-1.9.6/service/app_a/asserts/pay/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/pay/__init__.py
+-rw-rw-rw-   0        0        0      611 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/pay/asserts_pay_orderpaybill.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.472840 huhk-1.9.6/service/app_a/asserts/radarpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.475859 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.484462 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_batch.py
+-rw-rw-rw-   0        0        0      817 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_single.py
+-rw-rw-rw-   0        0        0     2203 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_adjustpoints.py
+-rw-rw-rw-   0        0        0     2272 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_pointsconfig.py
+-rw-rw-rw-   0        0        0     1275 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_pointstask.py
+-rw-rw-rw-   0        0        0     1163 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_summarystatistics.py
+-rw-rw-rw-   0        0        0     1660 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_userpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.492440 huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/__init__.py
+-rw-rw-rw-   0        0        0      807 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_exchangeinfo.py
+-rw-rw-rw-   0        0        0      783 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_pointsinfo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.529884 huhk-1.9.6/service/app_a/funs/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/funs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.537864 huhk-1.9.6/service/app_a/funs/admin/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/admin/__init__.py
+-rw-rw-rw-   0        0        0     1065 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/admin/funs_admin_guc.py
+-rw-rw-rw-   0        0        0      647 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/admin/funs_admin_spa.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.561359 huhk-1.9.6/service/app_a/funs/common/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/common/__init__.py
+-rw-rw-rw-   0        0        0      928 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_clue.py
+-rw-rw-rw-   0        0        0      709 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_common.py
+-rw-rw-rw-   0        0        0     1795 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_remoteinterfacelog.py
+-rw-rw-rw-   0        0        0     2804 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_systemversion.py
+-rw-rw-rw-   0        0        0      729 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_user.py
+-rw-rw-rw-   0        0        0    21622 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_user4c.py
+-rw-rw-rw-   0        0        0     6180 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_userpointsmanage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.615184 huhk-1.9.6/service/app_a/funs/content/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/content/__init__.py
+-rw-rw-rw-   0        0        0    26429 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_activitymanager.py
+-rw-rw-rw-   0        0        0    11631 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_adv.py
+-rw-rw-rw-   0        0        0     1482 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_advplace.py
+-rw-rw-rw-   0        0        0     7550 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_agreement.py
+-rw-rw-rw-   0        0        0     8084 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_campmanager.py
+-rw-rw-rw-   0        0        0     7904 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_comment.py
+-rw-rw-rw-   0        0        0     7209 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_commonquestion.py
+-rw-rw-rw-   0        0        0     1082 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_contentmanager.py
+-rw-rw-rw-   0        0        0    13476 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_essay.py
+-rw-rw-rw-   0        0        0     1526 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_essaycomment.py
+-rw-rw-rw-   0        0        0     4715 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_essayweb.py
+-rw-rw-rw-   0        0        0      694 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_hotcity.py
+-rw-rw-rw-   0        0        0     2656 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_hotsearch.py
+-rw-rw-rw-   0        0        0     5431 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_material.py
+-rw-rw-rw-   0        0        0    10631 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_messagemanager.py
+-rw-rw-rw-   0        0        0     2868 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_noticemanager.py
+-rw-rw-rw-   0        0        0     4376 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_question.py
+-rw-rw-rw-   0        0        0     1529 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_recruit.py
+-rw-rw-rw-   0        0        0     3317 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_safecode.py
+-rw-rw-rw-   0        0        0     8951 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_subject.py
+-rw-rw-rw-   0        0        0     9433 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_subjectweb.py
+-rw-rw-rw-   0        0        0     4900 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_topic4c.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.620173 huhk-1.9.6/service/app_a/funs/content/material/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/material/__init__.py
+-rw-rw-rw-   0        0        0     1219 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/material/funs_content_material_getmateriallist.py
+-rw-rw-rw-   0        0        0     1130 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/funs_activitymanager.py
+-rw-rw-rw-   0        0        0      194 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/funs_admin.py
+-rw-rw-rw-   0        0        0     3167 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_app_a.py
+-rw-rw-rw-   0        0        0      599 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_area.py
+-rw-rw-rw-   0        0        0      761 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_common.py
+-rw-rw-rw-   0        0        0     3099 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_content.py
+-rw-rw-rw-   0        0        0     2527 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_essay.py
+-rw-rw-rw-   0        0        0      506 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/funs_goods.py
+-rw-rw-rw-   0        0        0      140 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/funs_manageapi.py
+-rw-rw-rw-   0        0        0      118 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/funs_open.py
+-rw-rw-rw-   0        0        0      607 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_order.py
+-rw-rw-rw-   0        0        0      131 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/funs_pay.py
+-rw-rw-rw-   0        0        0      698 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/funs_radarpoints.py
+-rw-rw-rw-   0        0        0     2813 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/funs_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.637124 huhk-1.9.6/service/app_a/funs/goods/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/funs/goods/__init__.py
+-rw-rw-rw-   0        0        0     6559 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_area.py
+-rw-rw-rw-   0        0        0    11252 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_carmodel.py
+-rw-rw-rw-   0        0        0    10293 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_configure.py
+-rw-rw-rw-   0        0        0     5322 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_ordermain.py
+-rw-rw-rw-   0        0        0     3626 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.643109 huhk-1.9.6/service/app_a/funs/manageapi/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/manageapi/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/manageapi/funs_manageapi_order.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.648097 huhk-1.9.6/service/app_a/funs/manageapi/order/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/manageapi/order/__init__.py
+-rw-rw-rw-   0        0        0     4282 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/manageapi/order/funs_manageapi_order_mainorder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.654014 huhk-1.9.6/service/app_a/funs/open/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/funs_open_haohan.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.661992 huhk-1.9.6/service/app_a/funs/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      869 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/haohan/funs_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      959 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/haohan/funs_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.679945 huhk-1.9.6/service/app_a/funs/order/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/order/__init__.py
+-rw-rw-rw-   0        0        0     3970 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_freeorder.py
+-rw-rw-rw-   0        0        0    19335 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_mainorder.py
+-rw-rw-rw-   0        0        0     2770 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_order.py
+-rw-rw-rw-   0        0        0      176 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_rights.py
+-rw-rw-rw-   0        0        0    12237 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_rightsorder.py
+-rw-rw-rw-   0        0        0     2884 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.684930 huhk-1.9.6/service/app_a/funs/order/mainorder/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/mainorder/__init__.py
+-rw-rw-rw-   0        0        0     1373 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/mainorder/funs_order_mainorder_scrm2app.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.690915 huhk-1.9.6/service/app_a/funs/order/rights/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/rights/__init__.py
+-rw-rw-rw-   0        0        0     9168 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/rights/funs_order_rights_rightsmanager.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.695903 huhk-1.9.6/service/app_a/funs/order/rightsorder/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/rightsorder/__init__.py
+-rw-rw-rw-   0        0        0     3959 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/rightsorder/funs_order_rightsorder_receive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.701552 huhk-1.9.6/service/app_a/funs/pay/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/pay/__init__.py
+-rw-rw-rw-   0        0        0      900 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/pay/funs_pay_orderpaybill.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.717240 huhk-1.9.6/service/app_a/funs/radarpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.721950 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.730537 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/__init__.py
+-rw-rw-rw-   0        0        0     4080 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_batch.py
+-rw-rw-rw-   0        0        0     2099 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_single.py
+-rw-rw-rw-   0        0        0      433 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/funs_radarpoints_adjustpoints_adjust.py
+-rw-rw-rw-   0        0        0     5930 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_adjustpoints.py
+-rw-rw-rw-   0        0        0     8017 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_pointsconfig.py
+-rw-rw-rw-   0        0        0     4126 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_pointstask.py
+-rw-rw-rw-   0        0        0     2339 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_summarystatistics.py
+-rw-rw-rw-   0        0        0     7881 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_userpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.737517 huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_exchangeinfo.py
+-rw-rw-rw-   0        0        0     2169 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_pointsinfo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.754445 huhk-1.9.6/service/app_a/sqls/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/sqls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.762423 huhk-1.9.6/service/app_a/sqls/admin/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/admin/__init__.py
+-rw-rw-rw-   0        0        0     1026 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/admin/sqls_admin_guc.py
+-rw-rw-rw-   0        0        0      552 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/admin/sqls_admin_spa.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.781401 huhk-1.9.6/service/app_a/sqls/common/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/common/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_clue.py
+-rw-rw-rw-   0        0        0      562 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_common.py
+-rw-rw-rw-   0        0        0      586 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_remoteinterfacelog.py
+-rw-rw-rw-   0        0        0     1050 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_systemversion.py
+-rw-rw-rw-   0        0        0      563 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_user.py
+-rw-rw-rw-   0        0        0     6794 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_user4c.py
+-rw-rw-rw-   0        0        0     2069 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_userpointsmanage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.834628 huhk-1.9.6/service/app_a/sqls/content/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/content/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.841580 huhk-1.9.6/service/app_a/sqls/content/material/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/material/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/material/sqls_content_material_getmateriallist.py
+-rw-rw-rw-   0        0        0     7456 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_activitymanager.py
+-rw-rw-rw-   0        0        0     5815 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_adv.py
+-rw-rw-rw-   0        0        0      568 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_advplace.py
+-rw-rw-rw-   0        0        0     3943 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_agreement.py
+-rw-rw-rw-   0        0        0     2981 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_campmanager.py
+-rw-rw-rw-   0        0        0     2480 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_comment.py
+-rw-rw-rw-   0        0        0     4458 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_commonquestion.py
+-rw-rw-rw-   0        0        0      581 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_contentmanager.py
+-rw-rw-rw-   0        0        0     4379 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_essay.py
+-rw-rw-rw-   0        0        0      575 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_essaycomment.py
+-rw-rw-rw-   0        0        0     2002 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_essayweb.py
+-rw-rw-rw-   0        0        0      560 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_hotcity.py
+-rw-rw-rw-   0        0        0     1520 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_hotsearch.py
+-rw-rw-rw-   0        0        0     3466 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_material.py
+-rw-rw-rw-   0        0        0     3504 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_messagemanager.py
+-rw-rw-rw-   0        0        0     1564 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_noticemanager.py
+-rw-rw-rw-   0        0        0     2022 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_question.py
+-rw-rw-rw-   0        0        0     1037 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_recruit.py
+-rw-rw-rw-   0        0        0     2474 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_safecode.py
+-rw-rw-rw-   0        0        0     3917 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_subject.py
+-rw-rw-rw-   0        0        0     3455 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_subjectweb.py
+-rw-rw-rw-   0        0        0     2470 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_topic4c.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.856576 huhk-1.9.6/service/app_a/sqls/goods/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/sqls/goods/__init__.py
+-rw-rw-rw-   0        0        0     3904 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_area.py
+-rw-rw-rw-   0        0        0     3000 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_carmodel.py
+-rw-rw-rw-   0        0        0     2521 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_configure.py
+-rw-rw-rw-   0        0        0     2016 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_ordermain.py
+-rw-rw-rw-   0        0        0     1043 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.858536 huhk-1.9.6/service/app_a/sqls/manageapi/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/manageapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.865518 huhk-1.9.6/service/app_a/sqls/manageapi/order/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/manageapi/order/__init__.py
+-rw-rw-rw-   0        0        0     1070 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/manageapi/order/sqls_manageapi_order_mainorder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.868512 huhk-1.9.6/service/app_a/sqls/open/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.876523 huhk-1.9.6/service/app_a/sqls/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/open/haohan/sqls_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      567 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/open/haohan/sqls_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.891482 huhk-1.9.6/service/app_a/sqls/order/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/order/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.896435 huhk-1.9.6/service/app_a/sqls/order/mainorder/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/mainorder/__init__.py
+-rw-rw-rw-   0        0        0      590 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/mainorder/sqls_order_mainorder_scrm2app.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.901429 huhk-1.9.6/service/app_a/sqls/order/rights/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/rights/__init__.py
+-rw-rw-rw-   0        0        0     4025 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/rights/sqls_order_rights_rightsmanager.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.906411 huhk-1.9.6/service/app_a/sqls/order/rightsorder/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/rightsorder/__init__.py
+-rw-rw-rw-   0        0        0      581 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/rightsorder/sqls_order_rightsorder_receive.py
+-rw-rw-rw-   0        0        0      564 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_freeorder.py
+-rw-rw-rw-   0        0        0     7363 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_mainorder.py
+-rw-rw-rw-   0        0        0     1511 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_order.py
+-rw-rw-rw-   0        0        0     2972 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_rightsorder.py
+-rw-rw-rw-   0        0        0     1045 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.911399 huhk-1.9.6/service/app_a/sqls/pay/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/pay/__init__.py
+-rw-rw-rw-   0        0        0      569 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/pay/sqls_pay_orderpaybill.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.925985 huhk-1.9.6/service/app_a/sqls/radarpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.927979 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.936516 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_batch.py
+-rw-rw-rw-   0        0        0      604 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_single.py
+-rw-rw-rw-   0        0        0     2076 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_adjustpoints.py
+-rw-rw-rw-   0        0        0     2046 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_pointsconfig.py
+-rw-rw-rw-   0        0        0     1062 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_pointstask.py
+-rw-rw-rw-   0        0        0     1083 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_summarystatistics.py
+-rw-rw-rw-   0        0        0     1062 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_userpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.943498 huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/__init__.py
+-rw-rw-rw-   0        0        0      603 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_exchangeinfo.py
+-rw-rw-rw-   0        0        0      599 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_pointsinfo.py
+-rw-rw-rw-   0        0        0      574 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/sqls_activitymanager.py
+-rw-rw-rw-   0        0        0      534 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/sqls_app_a.py
+-rw-rw-rw-   0        0        0      546 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/sqls_area.py
+-rw-rw-rw-   0        0        0      545 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/sqls_content.py
+-rw-rw-rw-   0        0        0     1017 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/sqls_essay.py
+-rw-rw-rw-   0        0        0      554 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/sqls_testdrive.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 02:51:39.957186 huhk-1.9.6/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.945454 huhk-1.9.6/testcase/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.953365 huhk-1.9.6/testcase/app_a/
+-rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/testcase/app_a/__init__.py
+-rw-rw-rw-   0        0        0      361 2023-08-01 02:26:00.000000 huhk-1.9.6/testcase/app_a/conftest.py
+-rw-rw-rw-   0        0        0     3184 2023-08-01 02:26:13.000000 huhk-1.9.6/testcase/app_a/test_page.py
```

### Comparing `huhk-1.9.5/huhk/__init__.py` & `huhk-1.9.6/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/case_project/json_coder.py` & `huhk-1.9.6/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/case_project/main_fun.py` & `huhk-1.9.6/huhk/case_project/main_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/case_project/project_base.py` & `huhk-1.9.6/huhk/case_project/project_base.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/case_project/project_init.py` & `huhk-1.9.6/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/case_project/project_string.py` & `huhk-1.9.6/huhk/case_project/project_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/case_project/setup_set.py` & `huhk-1.9.6/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/init_project.py` & `huhk-1.9.6/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/main.py` & `huhk-1.9.6/huhk/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/beam_class.py` & `huhk-1.9.6/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/data.py` & `huhk-1.9.6/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/par_do.py` & `huhk-1.9.6/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.9.6/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/test_fiter.py` & `huhk-1.9.6/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/test_flatmap.py` & `huhk-1.9.6/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/test_map.py` & `huhk-1.9.6/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/test_par_do.py` & `huhk-1.9.6/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/test_regex.py` & `huhk-1.9.6/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/testcase/apache/test_time.py` & `huhk-1.9.6/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/unit_apache_beam.py` & `huhk-1.9.6/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/unit_dict.py` & `huhk-1.9.6/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/unit_encryption.py` & `huhk-1.9.6/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/unit_fun.py` & `huhk-1.9.6/huhk/unit_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,34 +457,37 @@
 
     @staticmethod
     def has_true(kwargs):
         _kwargs = {k: v for k, v in kwargs.items() if k not in ('self', 'kwargs') and k[0] != '_' and v is True}
         return _kwargs
 
     def get_res_value_list(self, name, property_path=''):
+        out = []
         if property_path:
             tmp = self.res.rsp
             for i in property_path.split('.'):
                 if not isinstance(tmp, dict):
                     return []
                 tmp = tmp.get(i)
             if isinstance(tmp, list) and tmp and isinstance(tmp[0], dict):
-                return [i.get(name) for i in tmp if i.get(name)]
-            return []
+                out = [i.get(name) for i in tmp if i.get(name)]
         else:
             if self.res.status_code == 200 and self.res.rsp and isinstance(self.res.rsp, dict):
                 for key, value in self.res.rsp.items():
-                    if isinstance(value, list):
-                        return [i.get(name) for i in value]
+                    if isinstance(value, list) and value and isinstance(value[0], dict):
+                        out = out or [i.get(name) or i.get(name.lower()) or i.get(name[0].lower()+name[1:])
+                                      for i in value if (i.get(name) or i.get(name.lower())
+                                                         or i.get(name[0].lower()+name[1:]))]
                     elif isinstance(value, dict):
                         for key2, value2 in value.items():
-                            if isinstance(value2, list):
-                                return [i.get(name) or i.get(name.lower()) or
-                                        i.get(name[0].lower()+name[1:]) for i in value2 if i.get(name)]
-            return []
+                            if isinstance(value2, list) and value2 and isinstance(value2[0], dict):
+                                out = out or [i.get(name) or i.get(name.lower()) or i.get(name[0].lower()+name[1:])
+                                              for i in value2 if (i.get(name) or i.get(name.lower())
+                                                                  or i.get(name[0].lower()+name[1:]))]
+        return out
 
     @staticmethod
     def _to_excel(f, data, sheet_name="sheet", set_column=[], header_format=None, column_header=[],
                   column_default=[], isdigitl=True):
         if data and isinstance(data[0], (list, tuple)):
             h = data[0]
             data1 = []
@@ -644,19 +647,23 @@
         else:
             return None
 
     def get_output_value(self, name):
         name_list = name.split('.')
         if len(name_list) == 1:
             caller = inspect.getframeinfo(inspect.currentframe().f_back)
-            return self.output_list[caller.function][name_list[-1]]
-        elif len(name_list) > 1:
-            return self.output_list[name_list[-2]][name_list[-1]]
+            key = caller.function
+        else:
+            key = name_list[-2]
+        values = self.output_list[key][name_list[-1]]
+        if (not values) and re.findall(before_and_end_re_str, name_list[-1]):
+            name2 = re.sub(before_and_end_re_str, "", name_list[-1])
+            return self.output_list[key][name2]
         else:
-            return []
+            return values
 
     def aa(self, a=None, b=None, c=None, d=None):
         print(a,b,c,d)
 
     def bb(self):
         getattr(self, 'aa')(c=3)
```

### Comparing `huhk-1.9.5/huhk/unit_logger.py` & `huhk-1.9.6/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/unit_request.py` & `huhk-1.9.6/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/unit_tasks.py` & `huhk-1.9.6/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk/常用命令.py` & `huhk-1.9.6/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/huhk.egg-info/SOURCES.txt` & `huhk-1.9.6/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/admin/apis_admin_guc.py` & `huhk-1.9.6/service/app_a/apis/admin/apis_admin_guc.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/admin/apis_admin_spa.py` & `huhk-1.9.6/service/app_a/apis/admin/apis_admin_spa.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/apis_activitymanager.py` & `huhk-1.9.6/service/app_a/apis/apis_activitymanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/apis_app_a.py` & `huhk-1.9.6/service/app_a/apis/apis_app_a.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/page")
-def page(district=None, province=None, provinceNameSort=None, cityNameSort=None, dealerName=None, shopBusinessType=None, districtNameSort=None, dealerCode=None, current=None, dealerAddress=None, city=None, size=None, headers=None, **kwargs):
+def page(current=None, dealerAddress=None, districtNameSort=None, cityNameSort=None, city=None, province=None, dealerName=None, shopBusinessType=None, district=None, size=None, dealerCode=None, provinceNameSort=None, headers=None, **kwargs):
     """
     网点列表-获取经销商
     up_time=1675233719
 
     params: current :  : 
     params: size :  : 
     params: province :  :
```

### Comparing `huhk-1.9.5/service/app_a/apis/apis_area.py` & `huhk-1.9.6/service/app_a/apis/apis_area.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/apis_content.py` & `huhk-1.9.6/service/app_a/apis/apis_content.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/apis_essay.py` & `huhk-1.9.6/service/app_a/apis/apis_essay.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/essay/queryListCount")
-def essay_querylistcount(status=None, keyWord=None, startTime=None, endTime=None, subjectId=None, author=None, essayId=None, headers=None, **kwargs):
+def essay_querylistcount(author=None, subjectId=None, essayId=None, keyWord=None, endTime=None, startTime=None, status=None, headers=None, **kwargs):
     """
     文章-获取列表状态数量-Y
     up_time=1675736107
 
     params: essayId :  : 文章主键
     params: keyWord :  : 搜索关键字
     params: author :  : 作者
```

### Comparing `huhk-1.9.5/service/app_a/apis/apis_testdrive.py` & `huhk-1.9.6/service/app_a/apis/apis_testdrive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/testDrive/subscribe")
-def testdrive_subscribe(shopId=None, appointmentTime=None, modelId=None, model=None, shopName=None, leadSourceCode=None, customerName=None, activityCode=None, phoneNumber=None, channel=None, leadSanSourceCode=None, headers=None, **kwargs):
+def testdrive_subscribe(leadSanSourceCode=None, phoneNumber=None, appointmentTime=None, channel=None, customerName=None, activityCode=None, shopName=None, shopId=None, leadSourceCode=None, model=None, modelId=None, headers=None, **kwargs):
     """
     预约试驾
     up_time=1689560965
 
     params: model : text : 试驾车型名称
     params: shopName : text : 门店名称
     params: customerName : text : 客户姓名、昵称
```

### Comparing `huhk-1.9.5/service/app_a/apis/common/apis_common_clue.py` & `huhk-1.9.6/service/app_a/apis/common/apis_common_clue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/common/clue/getClueUserPage")
-def common_clue_getclueuserpage(size=None, current=None, userId=None, headers=None, **kwargs):
+def common_clue_getclueuserpage(userId=None, size=None, current=None, headers=None, **kwargs):
     """
     用户列表-详情-查询线索-Y
     up_time=1675318572
 
     params: current :  : 页码
     params: size :  : 每页大小
     params: userId :  : 用户ID
```

### Comparing `huhk-1.9.5/service/app_a/apis/common/apis_common_common.py` & `huhk-1.9.6/service/app_a/apis/common/apis_common_common.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/common/apis_common_remoteinterfacelog.py` & `huhk-1.9.6/service/app_a/apis/common/apis_common_remoteinterfacelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/common/remoteinterfacelog/getLogPage")
-def common_remoteinterfacelog_getlogpage(interfaceType=None, startTime=None, endTime=None, userName=None, mobile=None, current=None, size=None, headers=None, **kwargs):
+def common_remoteinterfacelog_getlogpage(interfaceType=None, current=None, mobile=None, size=None, endTime=None, startTime=None, userName=None, headers=None, **kwargs):
     """
     查询三方日志接口-Y
     up_time=1675324564
 
     params: interfaceType :  : 日志类型（1.支付日志  2.退款日志  3.换电日志）
     params: startTime :  : 开始时间
     params: endTime :  : 结束时间
```

### Comparing `huhk-1.9.5/service/app_a/apis/common/apis_common_systemversion.py` & `huhk-1.9.6/service/app_a/apis/common/apis_common_systemversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/common/systemversion/save")
-def common_systemversion_save(remark=None, downloadUrl=None, classify=None, versionId=None, version=None, publishStatus=None, content=None, force=None, size=None, name=None, headers=None, **kwargs):
+def common_systemversion_save(classify=None, remark=None, name=None, publishStatus=None, force=None, downloadUrl=None, version=None, content=None, size=None, versionId=None, headers=None, **kwargs):
     """
     保存版本信息-Y
     up_time=1675326010
 
     params: version : string : 版本号
     params: name : string : 版本名称
     params: content : string : 更新内容
```

### Comparing `huhk-1.9.5/service/app_a/apis/common/apis_common_user.py` & `huhk-1.9.6/service/app_a/apis/common/apis_common_user.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/common/apis_common_user4c.py` & `huhk-1.9.6/service/app_a/apis/common/apis_common_user4c.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/page")
-def common_user4c_page(status=None, type=None, createTimeEnd=None, memberSystemSource=None, userId=None, regisTimeEnd=None, lastLoginTimeStart=None, lastLoginTimeEnd=None, activitySource=None, nickName=None, regisTimeBegin=None, mobile=None, ownerFlag=None, current=None, createTimeStart=None, userSystemSource=None, size=None, headers=None, **kwargs):
+def common_user4c_page(ownerFlag=None, userSystemSource=None, regisTimeBegin=None, type=None, lastLoginTimeEnd=None, current=None, activitySource=None, regisTimeEnd=None, mobile=None, status=None, createTimeEnd=None, lastLoginTimeStart=None, memberSystemSource=None, nickName=None, userId=None, size=None, createTimeStart=None, headers=None, **kwargs):
     """
     用户列表-查询-Y
     up_time=1675318775
 
     params: userId :  : 用户Id
     params: mobile :  : 用户手机号码
     params: nickName :  : 用户昵称
@@ -103,15 +103,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/vehicleInfo")
-def common_user4c_vehicleinfo(mobile=None, size=None, current=None, userId=None, headers=None, **kwargs):
+def common_user4c_vehicleinfo(userId=None, size=None, mobile=None, current=None, headers=None, **kwargs):
     """
     用户列表-详情-车辆信息-Y
     up_time=1675319192
 
     params: userId :  : 用户ID
     params: mobile :  : 用户手机号码
     params: current :  : 页码
@@ -242,15 +242,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/download")
-def common_user4c_download(status=None, type=None, createTimeEnd=None, memberSystemSource=None, userId=None, regisTimeEnd=None, lastLoginTimeStart=None, lastLoginTimeEnd=None, activitySource=None, nickName=None, regisTimeBegin=None, mobile=None, ownerFlag=None, createTimeStart=None, userSystemSource=None, downloadType=None, userIds=None, headers=None, **kwargs):
+def common_user4c_download(ownerFlag=None, userSystemSource=None, regisTimeBegin=None, userIds=None, type=None, lastLoginTimeEnd=None, activitySource=None, regisTimeEnd=None, mobile=None, downloadType=None, status=None, createTimeEnd=None, lastLoginTimeStart=None, memberSystemSource=None, nickName=None, userId=None, createTimeStart=None, headers=None, **kwargs):
     """
     用户列表-导出-Y
     up_time=1675148564
 
     params: userId :  : 用户Id
     params: mobile :  : 用户手机号
     params: nickName :  : 用户昵称
@@ -301,15 +301,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/beforePointsExport")
-def common_user4c_beforepointsexport(status=None, type=None, createTimeEnd=None, memberSystemSource=None, userId=None, regisTimeEnd=None, lastLoginTimeStart=None, lastLoginTimeEnd=None, activitySource=None, nickName=None, regisTimeBegin=None, mobile=None, ownerFlag=None, createTimeStart=None, userSystemSource=None, downloadType=None, userIds=None, headers=None, **kwargs):
+def common_user4c_beforepointsexport(ownerFlag=None, userSystemSource=None, regisTimeBegin=None, userIds=None, type=None, lastLoginTimeEnd=None, activitySource=None, regisTimeEnd=None, mobile=None, downloadType=None, status=None, createTimeEnd=None, lastLoginTimeStart=None, memberSystemSource=None, nickName=None, userId=None, createTimeStart=None, headers=None, **kwargs):
     """
     用户列表-导出前置判断-Y
     up_time=1675306476
 
     params: userId :  : 用户Id
     params: mobile :  : 用户手机号
     params: nickName :  : 用户昵称
@@ -363,15 +363,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/insert")
-def common_user4c_insert(explain=None, avatarUrl=None, nickName=None, headers=None, **kwargs):
+def common_user4c_insert(nickName=None, explain=None, avatarUrl=None, headers=None, **kwargs):
     """
     用户列表-新增-Y
     up_time=1675319481
 
     params: avatarUrl : text : String；图片地址
     params: explain : text : String；简介
     params: nickName : text : String；昵称
@@ -398,15 +398,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/editStatus")
-def common_user4c_editstatus(status=None, userId=None, headers=None, **kwargs):
+def common_user4c_editstatus(userId=None, status=None, headers=None, **kwargs):
     """
     用户中心-禁用/启用用户-Y
     up_time=1675320747
 
     params: userId : text : 
     params: status : number : 是否启用0：禁用 1：启用
     params: headers : 请求头
@@ -431,15 +431,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/auditExport")
-def common_user4c_auditexport(userLabel=None, registerType=None, userId=None, nickName=None, ownerFlag=None, userType=None, phone=None, downloadType=None, userIds=None, headers=None, **kwargs):
+def common_user4c_auditexport(ownerFlag=None, userLabel=None, userIds=None, phone=None, userType=None, downloadType=None, registerType=None, nickName=None, userId=None, headers=None, **kwargs):
     """
     导出用户审核列表-Y
     up_time=1675308559
 
     params: userId :  : 用户主键
     params: phone :  : 手机号
     params: nickName :  : 昵称
@@ -505,15 +505,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/updateAudit")
-def common_user4c_updateaudit(auditType=None, userId=None, headers=None, **kwargs):
+def common_user4c_updateaudit(userId=None, auditType=None, headers=None, **kwargs):
     """
     更新审核状态-Y
     up_time=1675319778
 
     params: userId : string : 用户ID
     params: auditType : integer : 认证类型（1：注销审核单据，2：车主认证审核单据）
     params: headers : 请求头
@@ -538,15 +538,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/user4C/auditList")
-def common_user4c_auditlist(registerType=None, pageNum=None, pageSize=None, userId=None, userName=None, nickName=None, mobile=None, checkStatus=None, headers=None, **kwargs):
+def common_user4c_auditlist(pageSize=None, mobile=None, registerType=None, checkStatus=None, nickName=None, userId=None, userName=None, pageNum=None, headers=None, **kwargs):
     """
     根据用户审核状态搜索列表-Y
     up_time=1675320694
 
     params: userId :  : 用户id
     params: mobile :  : 手机号
     params: nickName :  : 用户昵称
```

### Comparing `huhk-1.9.5/service/app_a/apis/common/apis_common_userpointsmanage.py` & `huhk-1.9.6/service/app_a/apis/common/apis_common_userpointsmanage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/common/userPointsManage/userPointsExport")
-def common_userpointsmanage_userpointsexport(logIds=None, endTime=None, beginTime=None, nickName=None, mobile=None, headers=None, **kwargs):
+def common_userpointsmanage_userpointsexport(beginTime=None, logIds=None, mobile=None, endTime=None, nickName=None, headers=None, **kwargs):
     """
     用户积分列表导出-历史接口
     up_time=1676338877
 
     params: nickName :  : 用户昵称
     params: mobile :  : 用户手机号
     params: beginTime :  : 注册时间查询范围--开始时间
@@ -36,15 +36,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/userPointsManage/page")
-def common_userpointsmanage_page(endTime=None, beginTime=None, mobile=None, nickName=None, headers=None, **kwargs):
+def common_userpointsmanage_page(nickName=None, endTime=None, beginTime=None, mobile=None, headers=None, **kwargs):
     """
     用户积分列表查询-历史接口
     up_time=1676338867
 
     params: nickName :  : 
     params: mobile :  : 
     params: beginTime :  : 前端日期后面必须要追加 00:00:00
@@ -77,15 +77,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/userPointsManage/manualChangeUserPoints")
-def common_userpointsmanage_manualchangeuserpoints(taskName=None, userId=None, operatePoint=None, operateMark=None, pointChangType=None, operateType=None, headers=None, **kwargs):
+def common_userpointsmanage_manualchangeuserpoints(operateType=None, operatePoint=None, pointChangType=None, operateMark=None, taskName=None, userId=None, headers=None, **kwargs):
     """
     用户积分手动调整-历史接口
     up_time=1676338835
 
     params: userId : number : 用户id
     params: operateType : string : 积分操作类型 目前只有 “增加” 一类
     params: operatePoint : integer : 操作的积分数量
@@ -118,15 +118,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/common/userPointsManage/beforePointsExport")
-def common_userpointsmanage_beforepointsexport(logIds=None, endTime=None, beginTime=None, nickName=None, mobile=None, headers=None, **kwargs):
+def common_userpointsmanage_beforepointsexport(beginTime=None, logIds=None, mobile=None, endTime=None, nickName=None, headers=None, **kwargs):
     """
     积分导出前置判断-历史接口
     up_time=1676338890
 
     params: nickName :  : 用户昵称
     params: mobile :  : 用户手机号
     params: beginTime :  : 注册时间查询范围--开始时间
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_activitymanager.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_activitymanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/activityManager/updatePerson")
-def content_activitymanager_updateperson(limitPeople=None, activityId=None, needLimitPeople=None, headers=None, **kwargs):
+def content_activitymanager_updateperson(activityId=None, needLimitPeople=None, limitPeople=None, headers=None, **kwargs):
     """
     活动 -修改报名人数(930)-Y
     up_time=1675238032
 
     params: activityId : string : 活动Id
     params: needLimitPeople : string : 是否限制 0 不限制 1限制
     params: limitPeople : number : 限制人数
@@ -36,15 +36,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/updateEnrollTime")
-def content_activitymanager_updateenrolltime(enrollStartTime=None, activityId=None, enrollTime=None, headers=None, **kwargs):
+def content_activitymanager_updateenrolltime(activityId=None, enrollStartTime=None, enrollTime=None, headers=None, **kwargs):
     """
     活动 -修改报名时间-Y
     up_time=1675238090
 
     params: activityId : string : 活动Id
     params: enrollStartTime : string : 报名开始时间
     params: enrollTime : string : 报名结束时间
@@ -71,15 +71,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/page")
-def content_activitymanager_page(status=None, title=None, activityId=None, province=None, pushTimeSort=None, endTime=None, beginTime=None, createTimeSort=None, target=None, city=None, activityTimeSort=None, headers=None, **kwargs):
+def content_activitymanager_page(beginTime=None, title=None, city=None, activityId=None, endTime=None, status=None, province=None, createTimeSort=None, pushTimeSort=None, activityTimeSort=None, target=None, headers=None, **kwargs):
     """
     活动列表查询（930版本）-Y
     up_time=1675147665
 
     params: activityId :  : 
     params: title :  : 
     params: beginTime :  : 2022-01-18 00:00:00 （一定要带上00:00:00）
@@ -131,15 +131,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/actInfoUpdate")
-def content_activitymanager_actinfoupdate(operationType=None, activityId=None, headers=None, **kwargs):
+def content_activitymanager_actinfoupdate(activityId=None, operationType=None, headers=None, **kwargs):
     """
     活动操作停止报名和结束活动-Y
     up_time=1675393449
 
     params: activityId : text : 活动ID
     params: operationType : text : 1停止报名 2活动结束
     params: headers : 请求头
@@ -164,15 +164,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/setActivitySort")
-def content_activitymanager_setactivitysort(sort=None, activityId=None, headers=None, **kwargs):
+def content_activitymanager_setactivitysort(activityId=None, sort=None, headers=None, **kwargs):
     """
     设置活动权重(930版本)-Y
     up_time=1675237750
 
     params: activityId : string : 活动Id
     params: sort : number : 权重
     params: headers : 请求头
@@ -327,15 +327,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/save")
-def content_activitymanager_save(activityPicUrl=None, activityPicURL=None, beginTime=None, coordinate=None, reason=None, status=None, activityId=None, enrollTime=None, needLimitPeople=None, endTime=None, customerGroup=None, limitPeople=None, province=None, county=None, authId=None, publishType=None, needArea=None, content=None, activityAddr=None, title=None, enrollStartTime=None, publishTime=None, agreementId=None, city=None, headers=None, **kwargs):
+def content_activitymanager_save(enrollStartTime=None, beginTime=None, activityPicURL=None, needArea=None, limitPeople=None, activityPicUrl=None, publishTime=None, status=None, enrollTime=None, customerGroup=None, publishType=None, activityAddr=None, county=None, title=None, reason=None, coordinate=None, activityId=None, authId=None, needLimitPeople=None, agreementId=None, city=None, endTime=None, province=None, content=None, headers=None, **kwargs):
     """
     活动新增-Y
     up_time=1678257957
 
     params: activityId : text : 
     params: title : text : 
     params: reason : text : 
@@ -404,15 +404,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/update")
-def content_activitymanager_update(activityPicUrl=None, activityPicURL=None, beginTime=None, coordinate=None, reason=None, status=None, activityId=None, enrollTime=None, needLimitPeople=None, endTime=None, customerGroup=None, limitPeople=None, province=None, county=None, authId=None, publishType=None, needArea=None, content=None, activityAddr=None, title=None, enrollStartTime=None, publishTime=None, city=None, headers=None, **kwargs):
+def content_activitymanager_update(enrollStartTime=None, beginTime=None, activityPicURL=None, needArea=None, limitPeople=None, activityPicUrl=None, publishTime=None, status=None, enrollTime=None, customerGroup=None, publishType=None, activityAddr=None, county=None, title=None, reason=None, coordinate=None, activityId=None, authId=None, needLimitPeople=None, city=None, endTime=None, province=None, content=None, headers=None, **kwargs):
     """
     活动编辑（930版本）-Y
     up_time=1675237616
 
     params: activityId : text : 
     params: title : text : 
     params: reason : text : 
@@ -488,15 +488,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/publishUpdate")
-def content_activitymanager_publishupdate(status=None, publishStatus=None, activityId=None, activityIds=None, headers=None, **kwargs):
+def content_activitymanager_publishupdate(activityId=None, publishStatus=None, status=None, activityIds=None, headers=None, **kwargs):
     """
     活动发布状态修改(930)-Y
     up_time=1675392693
 
     params: activityIds : text : 单个记录修改传["xxxxx"]
     params: publishStatus : text : 
     params: activityId : string : 活动Id
@@ -525,15 +525,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/statusUpdate")
-def content_activitymanager_statusupdate(activityIds=None, checkStatus=None, headers=None, **kwargs):
+def content_activitymanager_statusupdate(checkStatus=None, activityIds=None, headers=None, **kwargs):
     """
     活动审核状态修改-Y
     up_time=1675392843
 
     params: checkStatus : text : 
     params: activityIds : array : 活动IDs
               type : string : None
@@ -592,15 +592,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/activityManager/activityExport")
-def content_activitymanager_activityexport(status=None, title=None, activityId=None, province=None, pushTimeSort=None, endTime=None, beginTime=None, createTimeSort=None, target=None, city=None, activityTimeSort=None, headers=None, **kwargs):
+def content_activitymanager_activityexport(beginTime=None, title=None, city=None, activityId=None, endTime=None, status=None, province=None, createTimeSort=None, pushTimeSort=None, activityTimeSort=None, target=None, headers=None, **kwargs):
     """
     活动数据导出-Y
     up_time=1675149098
 
     params: activityId :  : 
     params: title :  : 
     params: beginTime :  : 2022-01-18 00:00:00 （一定要带上00:00:00）
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_adv.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_adv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/adv/save")
-def content_adv_save(advLinkUrl=None, version=None, pictureList=None, advPlaceId=None, advId=None, bindingFlag=None, advSerial=None, jumpType=None, advPicUrl=None, jumpContent=None, advText=None, headers=None, **kwargs):
+def content_adv_save(advPlaceId=None, bindingFlag=None, advSerial=None, advId=None, jumpContent=None, advPicUrl=None, advLinkUrl=None, jumpType=None, pictureList=None, version=None, advText=None, headers=None, **kwargs):
     """
     点位内容-保存运营端配置(更新、新增)（930）-Y
     up_time=1675674291
 
     params: advPlaceId : number : 左侧列表选中ID
     params: advPicUrl : string : 图片地址
     params: advText : string : 文字描述
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_advplace.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_advplace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/advplace/updateName")
-def content_advplace_updatename(advPlaceId=None, startFlag=None, advPlaceName=None, playTime=None, headers=None, **kwargs):
+def content_advplace_updatename(advPlaceName=None, advPlaceId=None, startFlag=None, playTime=None, headers=None, **kwargs):
     """
     点位-更新大点位内容
     up_time=1675133826
 
     params: advPlaceId : text : 
     params: advPlaceName : text : 
     params: startFlag : text : 广告页广告位必传
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_agreement.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_agreement.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/agreement/save")
-def content_agreement_save(content=None, version=None, code=None, name=None, headers=None, **kwargs):
+def content_agreement_save(name=None, content=None, code=None, version=None, headers=None, **kwargs):
     """
     协议-新增协议-Y
     up_time=1675675877
 
     params: name : string : 协议名
     params: content : string : 内容
     params: version : number : 版本号
@@ -243,15 +243,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/agreement/update")
-def content_agreement_update(name=None, content=None, agreementId=None, code=None, version=None, headers=None, **kwargs):
+def content_agreement_update(code=None, name=None, agreementId=None, version=None, content=None, headers=None, **kwargs):
     """
     协议-更新协议-Y
     up_time=1675680222
 
     params: name : string : 协议名
     params: content : string : 内容
     params: version : number : 版本号
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_campmanager.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_campmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/campManager/page")
-def content_campmanager_page(status=None, sortord=None, sortBody=None, id=None, createBy=None, name=None, headers=None, **kwargs):
+def content_campmanager_page(createBy=None, name=None, sortBody=None, status=None, sortord=None, id=None, headers=None, **kwargs):
     """
     营地服务列表 - 分页查询
     up_time=1681969132
 
     params: id :  : 
     params: name :  : 
     params: status :  : 
@@ -113,15 +113,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/campManager/insert")
-def content_campmanager_insert(province=None, county=None, discountExpEndTime=None, id=None, discountExpBeginTime=None, campTradeTime=None, url=None, ownerDiscount=None, content=None, city=None, address=None, name=None, campDetail=None, headers=None, **kwargs):
+def content_campmanager_insert(campDetail=None, county=None, ownerDiscount=None, name=None, discountExpBeginTime=None, address=None, url=None, city=None, province=None, campTradeTime=None, content=None, id=None, discountExpEndTime=None, headers=None, **kwargs):
     """
     新增营地
     up_time=1681967827
 
     params: id : text : 营地服务ID
     params: name : text : 营地名称
     params: content : text : 营地简介
@@ -212,15 +212,15 @@
         "id": id,  # 营地服务ID
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/campManager/update")
-def content_campmanager_update(discountExpEndTime=None, ownerDiscount=None, discountExpBeginTime=None, phone=None, areaCode=None, headers=None, **kwargs):
+def content_campmanager_update(ownerDiscount=None, discountExpBeginTime=None, phone=None, areaCode=None, discountExpEndTime=None, headers=None, **kwargs):
     """
     编辑营地
     up_time=1681969876
 
     params: ownerDiscount : text : 车主优惠
     params: discountExpBeginTime : text : 车主优惠有效期 - 开始时间
     params: discountExpEndTime : text : 车主优惠有效期 - 结束时间
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_comment.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/comment/updateStatus")
-def content_comment_updatestatus(fromStatus=None, commentType=None, toStatus=None, commentId=None, headers=None, **kwargs):
+def content_comment_updatestatus(commentId=None, fromStatus=None, toStatus=None, commentType=None, headers=None, **kwargs):
     """
     评论-状态扭转（通用）-Y
     up_time=1675394720
 
     params: commentId :  : 评论主键
     params: commentType :  : 评论类型1：文章评论2：动态评论	
     params: fromStatus :  : 当前状态
@@ -38,15 +38,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/comment/downLoad")
-def content_comment_download(status=None, contentCommentIds=None, keyWord=None, startTime=None, endTime=None, nickName=None, EssayCommentIds=None, mobile=None, downloadType=None, headers=None, **kwargs):
+def content_comment_download(contentCommentIds=None, EssayCommentIds=None, keyWord=None, mobile=None, downloadType=None, endTime=None, startTime=None, status=None, nickName=None, headers=None, **kwargs):
     """
     评论-评论导出-Y
     up_time=1675649477
 
     params: mobile :  : 评论用户手机号
     params: nickName :  : 评论昵称
     params: keyWord :  : 搜索关键字
@@ -81,15 +81,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/comment/commentTop")
-def content_comment_commenttop(commentType=None, topFlag=None, commentId=None, headers=None, **kwargs):
+def content_comment_commenttop(commentId=None, topFlag=None, commentType=None, headers=None, **kwargs):
     """
     评论-评论置顶（通用）-Y
     up_time=1675663979
 
     params: commentId : string : 评论主键
     params: commentType : number : 评论类型1：文章评论2：动态评论
     params: topFlag : number : 1：置顶0：取消置顶
@@ -116,15 +116,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/comment/list")
-def content_comment_list(keyWord=None, startTime=None, endTime=None, nickName=None, checkedStatus=None, mobile=None, essayId=None, current=None, commentType=None, size=None, headers=None, **kwargs):
+def content_comment_list(current=None, essayId=None, keyWord=None, mobile=None, commentType=None, endTime=None, startTime=None, checkedStatus=None, nickName=None, size=None, headers=None, **kwargs):
     """
     后台管理-评论管理列表1030-Y
     up_time=1675394167
 
     params: nickName :  : 用户昵称 String
     params: keyWord :  : 搜索内容关键字  String
     params: startTime :  : 搜索开始时间 yyyy-MM-dd HH:mm:ss
@@ -169,15 +169,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/comment/delete")
-def content_comment_delete(commentType=None, toStatus=None, commentId=None, headers=None, **kwargs):
+def content_comment_delete(commentId=None, toStatus=None, commentType=None, headers=None, **kwargs):
     """
     评论-屏蔽评论-Y
     up_time=1675394437
 
     params: commentId : string : 评论主键
     params: commentType : number : 1：文章评论2：动态评论
     params: toStatus : string :
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_commonquestion.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_commonquestion.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_contentmanager.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_contentmanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_essay.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_essay.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "essayId": essayId,  # 文章id
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/essay/searchByKey")
-def content_essay_searchbykey(Key=None, size=None, current=None, headers=None, **kwargs):
+def content_essay_searchbykey(size=None, Key=None, current=None, headers=None, **kwargs):
     """
     专题-后台App文章关键词搜索-Y
     up_time=1675736722
 
     params: Key :  : 关键词
     params: size :  : 条数
     params: current :  : 当前页
@@ -64,15 +64,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/essay/checkList")
-def content_essay_checklist(status=None, StatusSortType=None, keyWord=None, startTime=None, endTime=None, CreateTimeSortType=None, subjectId=None, author=None, essayId=None, PublishTimeSortType=None, current=None, recommend=None, size=None, headers=None, **kwargs):
+def content_essay_checklist(author=None, subjectId=None, StatusSortType=None, essayId=None, current=None, PublishTimeSortType=None, keyWord=None, endTime=None, startTime=None, status=None, CreateTimeSortType=None, recommend=None, size=None, headers=None, **kwargs):
     """
     后台管理-内容审核列表1030-Y
     up_time=1675736061
 
     params: essayId :  : 文章主键
     params: keyWord :  : 文章搜索关键字
     params: author :  : 作者
@@ -123,15 +123,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/essay/list")
-def content_essay_list(status=None, StatusSortType=None, keyWord=None, startTime=None, endTime=None, CreateTimeSortType=None, subjectId=None, author=None, essayId=None, PublishTimeSortType=None, current=None, recommend=None, size=None, headers=None, **kwargs):
+def content_essay_list(author=None, subjectId=None, StatusSortType=None, essayId=None, current=None, PublishTimeSortType=None, keyWord=None, endTime=None, startTime=None, status=None, CreateTimeSortType=None, recommend=None, size=None, headers=None, **kwargs):
     """
     后台管理-内容管理列表1030-Y
     up_time=1675736044
 
     params: essayId :  : 文章主键
     params: keyWord :  : 文章搜索关键字
     params: author :  : 作者
@@ -182,15 +182,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/essay/add")
-def content_essay_add(status=None, essPicUrl=None, title=None, videoUrl=None, publishTime=None, publishType=None, subjectId=None, author=None, essayId=None, recommend=None, content=None, essayType=None, headers=None, **kwargs):
+def content_essay_add(videoUrl=None, author=None, title=None, subjectId=None, essayId=None, publishTime=None, essPicUrl=None, status=None, content=None, publishType=None, recommend=None, essayType=None, headers=None, **kwargs):
     """
     后台管理-新建&修改内容1030-Y
     up_time=1675736497
 
     params: essayId : string : 文章主键
     params: title : string : 标题
     params: author : string : 作者
@@ -331,15 +331,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/essay/getCommentList")
-def content_essay_getcommentlist(parentId=None, keyWord=None, startTime=None, endTime=None, essayId=None, commentId=None, current=None, checkedStatus=None, size=None, headers=None, **kwargs):
+def content_essay_getcommentlist(essayId=None, commentId=None, parentId=None, current=None, keyWord=None, endTime=None, checkedStatus=None, startTime=None, size=None, headers=None, **kwargs):
     """
     后台管理-评论信息1030-Y
     up_time=1675736123
 
     params: essayId :  : 文章主键
     params: keyWord :  : 关键词
     params: checkedStatus :  : 审核状态 审核状态 0待审核 1.已上架 2.审核未通过3：已下架 5已删除
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_essaycomment.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_essaycomment.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_essayweb.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_essayweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/essayweb/add")
-def content_essayweb_add(essPicUrl=None, status=None, title=None, publishTime=None, publishType=None, publishChannel=None, author=None, essayId=None, content=None, headers=None, **kwargs):
+def content_essayweb_add(publishChannel=None, author=None, title=None, essayId=None, publishTime=None, essPicUrl=None, status=None, content=None, publishType=None, headers=None, **kwargs):
     """
     专题-后台官网专题新建文章-Y
     up_time=1675737086
 
     params: essayId : string : 文章主键
     params: title : string : 文章标题
     params: author : string : 作者
@@ -48,15 +48,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/essayweb/searchByKey")
-def content_essayweb_searchbykey(key=None, size=None, current=None, headers=None, **kwargs):
+def content_essayweb_searchbykey(size=None, key=None, current=None, headers=None, **kwargs):
     """
     专题-后台官网文章关键词搜索-Y
     up_time=1675737282
 
     params: current :  : 当前页
     params: size :  : 每页条数
     params: key :  : 关键词
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_hotcity.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_hotcity.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_hotsearch.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_hotsearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/hotSearch/rank")
-def content_hotsearch_rank(kId=None, rank=None, headers=None, **kwargs):
+def content_hotsearch_rank(rank=None, kId=None, headers=None, **kwargs):
     """
     热门搜索-修改权重-Y
     up_time=1675737497
 
     params: kId : string : 主键id
     params: rank : string : 权重
     params: headers : 请求头
@@ -34,15 +34,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/hotSearch/list")
-def content_hotsearch_list(kId=None, rank=None, headers=None, **kwargs):
+def content_hotsearch_list(rank=None, kId=None, headers=None, **kwargs):
     """
     热门搜索-列表-Y
     up_time=1675737340
 
     params: kId : string : 主键id
     params: rank : string : 权重
     params: headers : 请求头
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_material.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_material.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/material/getMaterialList")
-def content_material_getmateriallist(groupId=None, size=None, current=None, headers=None, **kwargs):
+def content_material_getmateriallist(size=None, groupId=None, current=None, headers=None, **kwargs):
     """
     素材-根据素材组获取素材列表
     up_time=1675133826
 
     params: groupId :  : 分组主键
     params: size :  : 每页数据数
     params: current :  : 当前页
@@ -169,15 +169,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/material/addMaterial")
-def content_material_addmaterial(groupId=None, file=None, headers=None, **kwargs):
+def content_material_addmaterial(file=None, groupId=None, headers=None, **kwargs):
     """
     素材-素材上传
     up_time=1675133827
 
     params: file : file : 上传文件
     params: groupId : text : 所属分组主键
     params: headers : 请求头
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_messagemanager.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_messagemanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/messageManager/page")
-def content_messagemanager_page(status=None, cEndTime=None, userId=None, authId=None, endTime=None, beginTime=None, pStartTime=None, messageId=None, cStartTime=None, pEndTime=None, content=None, headers=None, **kwargs):
+def content_messagemanager_page(beginTime=None, cStartTime=None, pEndTime=None, authId=None, endTime=None, messageId=None, status=None, pStartTime=None, content=None, userId=None, cEndTime=None, headers=None, **kwargs):
     """
     消息列表查询接口-Y
     up_time=1675651897
 
     params: messageId :  : 
     params: userId :  : 
     params: content :  : 
@@ -99,15 +99,15 @@
         "messageId": messageId,
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/messageManager/messageTop")
-def content_messagemanager_messagetop(topFlag=None, messageIds=None, headers=None, **kwargs):
+def content_messagemanager_messagetop(messageIds=None, topFlag=None, headers=None, **kwargs):
     """
     消息置顶/取消置顶-Y
     up_time=1675652320
 
     params: messageIds : text : 消息ids集合
     params: topFlag : text : 消息置顶标识 0-置顶 1-不置顶
     params: headers : 请求头
@@ -132,15 +132,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/messageManager/insert")
-def content_messagemanager_insert(type=None, publishTime=None, messageId=None, sourceType=None, publishType=None, sendScope=None, imageUrl=None, content=None, param=None, checkPublish=None, checkStatus=None, headers=None, **kwargs):
+def content_messagemanager_insert(sendScope=None, type=None, publishTime=None, imageUrl=None, checkPublish=None, sourceType=None, messageId=None, checkStatus=None, content=None, publishType=None, param=None, headers=None, **kwargs):
     """
     消息新增接口-Y
     up_time=1675652341
 
     params: messageId : text : 
     params: type : text : 此处传1
     params: content : text : 
@@ -180,15 +180,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/messageManager/update")
-def content_messagemanager_update(type=None, messageId=None, sourceType=None, sendScope=None, imageUrl=None, userMobiles=None, content=None, param=None, checkPublish=None, checkStatus=None, headers=None, **kwargs):
+def content_messagemanager_update(sendScope=None, type=None, userMobiles=None, imageUrl=None, checkPublish=None, sourceType=None, messageId=None, checkStatus=None, content=None, param=None, headers=None, **kwargs):
     """
     消息编辑接口-Y
     up_time=1675652502
 
     params: messageId :  : 
     params: type :  : 此处传1
     params: content :  : 
@@ -226,15 +226,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/messageManager/publishUpdate")
-def content_messagemanager_publishupdate(publishStatus=None, messageIds=None, headers=None, **kwargs):
+def content_messagemanager_publishupdate(messageIds=None, publishStatus=None, headers=None, **kwargs):
     """
     消息发布状态修改-Y
     up_time=1675652643
 
     params: messageIds : text : 
     params: publishStatus : text : 
     params: headers : 请求头
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_noticemanager.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_noticemanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/noticeManager/getNoticeParamsList/")
-def content_noticemanager_getnoticeparamslist_(templateType=None, messageId=None, headers=None, **kwargs):
+def content_noticemanager_getnoticeparamslist_(messageId=None, templateType=None, headers=None, **kwargs):
     """
     获取系统通知详情
     up_time=1675133819
 
     params: messageId :  : 
     params: templateType :  : 模板编码
     params: headers : 请求头
@@ -82,15 +82,15 @@
         "messageId": messageId,
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/noticeManager/noticeParamsUpdate")
-def content_noticemanager_noticeparamsupdate(templateType=None, templateName=None, templateContent=None, headers=None, **kwargs):
+def content_noticemanager_noticeparamsupdate(templateContent=None, templateName=None, templateType=None, headers=None, **kwargs):
     """
     系统通知变量编辑-Y
     up_time=1675652880
 
     params: templateType : string : 模板类型
     params: templateName : string : 模板名称（标题）
     params: templateContent : string : 模板内容
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_question.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_question.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/question/answerQuestion")
-def content_question_answerquestion(questionId=None, answerContent=None, author=None, headers=None, **kwargs):
+def content_question_answerquestion(answerContent=None, author=None, questionId=None, headers=None, **kwargs):
     """
     问答-回复问题-Y
     up_time=1675680341
 
     params: questionId : string : 问题主键
     params: answerContent : string : 回答内容
     params: author : number : 作者
@@ -66,15 +66,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/question/getManegeQuestionList")
-def content_question_getmanegequestionlist(status=None, keyWord=None, startTime=None, endTime=None, mobile=None, current=None, size=None, headers=None, **kwargs):
+def content_question_getmanegequestionlist(current=None, keyWord=None, mobile=None, endTime=None, startTime=None, status=None, size=None, headers=None, **kwargs):
     """
     问答-搜索问题列表-Y
     up_time=1675740163
 
     params: keyWord :  : 关键字
     params: mobile :  : 发布人手机号
     params: startTime :  : 搜索起始时间
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_recruit.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_recruit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/recruit/save")
-def content_recruit_save(fileName=None, fileUrl=None, headers=None, **kwargs):
+def content_recruit_save(fileUrl=None, fileName=None, headers=None, **kwargs):
     """
     招聘信息保存-Y
     up_time=1675740268
 
     params: fileName : string : 文件名
     params: fileUrl : string : 文件url
     params: headers : 请求头
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_safecode.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_safecode.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_subject.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/subject/detailEssay")
-def content_subject_detailessay(subjectId=None, size=None, current=None, subjectName=None, headers=None, **kwargs):
+def content_subject_detailessay(subjectName=None, size=None, subjectId=None, current=None, headers=None, **kwargs):
     """
     专题-后台App专题文章列表-Y
     up_time=1675752193
 
     params: current :  : 
     params: size :  : 
     params: subjectId :  : Long
@@ -41,15 +41,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/subject/add")
-def content_subject_add(status=None, type=None, parentId=None, explain=None, level=None, subPicUrl=None, subjectName=None, headers=None, **kwargs):
+def content_subject_add(explain=None, type=None, parentId=None, subPicUrl=None, level=None, subjectName=None, status=None, headers=None, **kwargs):
     """
     专题-后台App专题新增-Y
     up_time=1675749730
 
     params: subjectName : string : 专题名称
     params: parentId : string : 父级专题主键
     params: level : number : 专题等级
@@ -115,15 +115,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/subject/mobileSubject")
-def content_subject_mobilesubject(subjectId=None, serial=None, parentId=None, headers=None, **kwargs):
+def content_subject_mobilesubject(parentId=None, subjectId=None, serial=None, headers=None, **kwargs):
     """
     专题-后台App移动专题更新-Y
     up_time=1675750974
 
     params: subjectId : text : 移动的专题ID
     params: parentId : text : 移动到的一级专题ID
     params: serial : text : 排序
@@ -265,15 +265,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/subject/save")
-def content_subject_save(status=None, type=None, parentId=None, explain=None, siftFlag=None, delFlag=None, level=None, subjectId=None, subPicUrl=None, isSearch=None, isService=None, subjectName=None, headers=None, **kwargs):
+def content_subject_save(subjectId=None, delFlag=None, explain=None, type=None, parentId=None, subPicUrl=None, siftFlag=None, level=None, subjectName=None, status=None, isSearch=None, isService=None, headers=None, **kwargs):
     """
     专题-后台App保存/更新-Y
     up_time=1675749773
 
     params: subjectId : number : 
     params: subjectName : string : 
     params: level : number :
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_subjectweb.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_subjectweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/subjectweb/detailEssay")
-def content_subjectweb_detailessay(subjectId=None, size=None, current=None, headers=None, **kwargs):
+def content_subjectweb_detailessay(size=None, subjectId=None, current=None, headers=None, **kwargs):
     """
     专题-后台官网专题文章列表-Y
     up_time=1675754018
 
     params: current :  : 当前页
     params: size :  : 当前条数
     params: subjectId :  : 专题主键id
@@ -39,15 +39,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/subjectweb/add")
-def content_subjectweb_add(status=None, type=None, parentId=None, subjectRank=None, explain=None, siftFlag=None, siftPicUrl=None, web=None, level=None, subPicUrl=None, serial=None, isSearch=None, recommend=None, isService=None, subjectName=None, headers=None, **kwargs):
+def content_subjectweb_add(subjectRank=None, web=None, type=None, explain=None, serial=None, parentId=None, subPicUrl=None, siftFlag=None, level=None, subjectName=None, status=None, siftPicUrl=None, isSearch=None, isService=None, recommend=None, headers=None, **kwargs):
     """
     专题-后台官网专题新增-Y
     up_time=1675754357
 
     params: subjectName : string : 专题名称
     params: level : string : 专题等级
     params: status : string : 是否可用1：是 0：否
@@ -130,15 +130,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/subjectweb/save")
-def content_subjectweb_save(status=None, type=None, parentId=None, explain=None, siftFlag=None, delFlag=None, subjectId=None, subPicUrl=None, isSearch=None, isService=None, subjectName=None, headers=None, **kwargs):
+def content_subjectweb_save(subjectId=None, delFlag=None, explain=None, type=None, parentId=None, subPicUrl=None, siftFlag=None, subjectName=None, status=None, isSearch=None, isService=None, headers=None, **kwargs):
     """
     专题-后台官网保存/更新-Y
     up_time=1675754842
 
     params: subjectId : string : 
     params: subjectName : string : 
     params: delFlag : string : 
@@ -251,15 +251,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/subjectweb/detailEssayNew")
-def content_subjectweb_detailessaynew(subjectId=None, size=None, current=None, headers=None, **kwargs):
+def content_subjectweb_detailessaynew(size=None, subjectId=None, current=None, headers=None, **kwargs):
     """
     新闻中心文章列表-Y
     up_time=1675753591
 
     params: current :  : 
     params: size :  : 
     params: subjectId :  : 2 官方新闻 3 自媒体 4 媒体报道  null 全部
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/apis_content_topic4c.py` & `huhk-1.9.6/service/app_a/apis/content/apis_content_topic4c.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/topic4C/getContentList")
-def content_topic4c_getcontentlist(topicId=None, size=None, current=None, headers=None, **kwargs):
+def content_topic4c_getcontentlist(size=None, topicId=None, current=None, headers=None, **kwargs):
     """
     话题-获取动态关联列表-Y
     up_time=1675653387
 
     params: topicId :  : 话题主键
     params: size :  : 每页数据数
     params: current :  : 当前页
@@ -76,15 +76,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/topic4C/list")
-def content_topic4c_list(topicId=None, keyWord=None, startTime=None, endTime=None, current=None, createBy=None, size=None, headers=None, **kwargs):
+def content_topic4c_list(createBy=None, current=None, keyWord=None, endTime=None, startTime=None, topicId=None, size=None, headers=None, **kwargs):
     """
     话题-搜索话题列表
     up_time=1675133829
 
     params: topicId :  : 话题主键
     params: createBy :  : 发布人主键
     params: keyWord :  : 话题关键字
@@ -130,15 +130,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/topic4C/insert")
-def content_topic4c_insert(author=None, topicId=None, topicTitle=None, headers=None, **kwargs):
+def content_topic4c_insert(topicId=None, author=None, topicTitle=None, headers=None, **kwargs):
     """
     话题-新增话题
     up_time=1675133829
 
     params: topicId : string : 话题主键
     params: topicTitle : string : 话题
     params: author : number : 话题作者
@@ -165,15 +165,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/content/topic4C/top")
-def content_topic4c_top(type=None, topicId=None, headers=None, **kwargs):
+def content_topic4c_top(topicId=None, type=None, headers=None, **kwargs):
     """
     话题-置顶
     up_time=1675133829
 
     params: topicId : string : 话题主键
     params: type : string : 操作类型1：置顶2：取消置顶
     params: headers : 请求头
```

### Comparing `huhk-1.9.5/service/app_a/apis/content/material/apis_content_material_getmateriallist.py` & `huhk-1.9.6/service/app_a/apis/content/material/apis_content_material_getmateriallist.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/content/material/getMaterialList_1659319316474")
-def content_material_getmateriallist_1659319316474(groupId=None, size=None, current=None, headers=None, **kwargs):
+def content_material_getmateriallist_1659319316474(size=None, groupId=None, current=None, headers=None, **kwargs):
     """
     素材-根据素材组获取素材列表_copy
     up_time=1675755133
 
     params: groupId :  : 分组主键
     params: size :  : 每页数据数
     params: current :  : 当前页
```

### Comparing `huhk-1.9.5/service/app_a/apis/goods/apis_goods_area.py` & `huhk-1.9.6/service/app_a/apis/goods/apis_goods_area.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/goods/apis_goods_carmodel.py` & `huhk-1.9.6/service/app_a/apis/goods/apis_goods_carmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/goods/carmodel/saveManageCarModel")
-def goods_carmodel_savemanagecarmodel(modelId=None, promptDesc=None, prePricePosters=None, depositPrice=None, carName=None, carDetailUrl=None, depositEndTime=None, version=None, status=None, modelName=None, preToDepositEndTime=None, preToDepositStartTime=None, depositStartTime=None, carCode=None, prePrice=None, prePriceContent=None, posters=None, carDetailPics=None, price=None, sort=None, modelCode=None, preEndTime=None, carSimpleName=None, depositPriceContent=None, brandName=None, preStartTime=None, configCode=None, sharePosters=None, carDetailType=None, headers=None, **kwargs):
+def goods_carmodel_savemanagecarmodel(prePricePosters=None, carDetailPics=None, depositPrice=None, carCode=None, preToDepositEndTime=None, preStartTime=None, sharePosters=None, depositEndTime=None, modelId=None, carDetailUrl=None, price=None, depositStartTime=None, preEndTime=None, promptDesc=None, brandName=None, modelName=None, carSimpleName=None, prePriceContent=None, status=None, posters=None, carDetailType=None, sort=None, prePrice=None, preToDepositStartTime=None, carName=None, modelCode=None, configCode=None, version=None, depositPriceContent=None, headers=None, **kwargs):
     """
     保存车型详细信息 - Y
     up_time=1675664128
 
     params: carName : string : 车系名称
     params: brandName : string : 品牌名称
     params: version : string : 品牌代码
@@ -168,15 +168,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/goods/carmodel/getManageCarModel")
-def goods_carmodel_getmanagecarmodel(status=None, brandName=None, modelCode=None, modelName=None, operator=None, carName=None, current=None, carCode=None, size=None, version=None, headers=None, **kwargs):
+def goods_carmodel_getmanagecarmodel(carName=None, modelCode=None, current=None, operator=None, brandName=None, modelName=None, carCode=None, status=None, version=None, size=None, headers=None, **kwargs):
     """
     车型列表-Y
     up_time=1675661996
 
     params: current :  : 分页
     params: size :  : 分页
     params: modelName :  : 车型名称
```

### Comparing `huhk-1.9.5/service/app_a/apis/goods/apis_goods_configure.py` & `huhk-1.9.6/service/app_a/apis/goods/apis_goods_configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/goods/configure/saveCarConfigure")
-def goods_configure_savecarconfigure(processColorList=None, salesVersionList=None, interiorColorList=None, appearanceColorList=None, optionalList=None, headers=None, **kwargs):
+def goods_configure_savecarconfigure(salesVersionList=None, appearanceColorList=None, interiorColorList=None, processColorList=None, optionalList=None, headers=None, **kwargs):
     """
     保存车型配置信息-Y
     up_time=1675650535
 
     params: salesVersionList : array : 销售版本
               configureId : string : 配置ID
               modelId : string : 关联的车型基础信息ID
```

### Comparing `huhk-1.9.5/service/app_a/apis/goods/apis_goods_ordermain.py` & `huhk-1.9.6/service/app_a/apis/goods/apis_goods_ordermain.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/goods/orderMain/orderExports")
-def goods_ordermain_orderexports(userMobile=None, billStatus	=None, modelName=None, startTime=None, endTime=None, userName=None, shopName=None, testDriveIdStr=None, exportType=None, headers=None, **kwargs):
+def goods_ordermain_orderexports(exportType=None, testDriveIdStr=None, billStatus	=None, modelName=None, shopName=None, endTime=None, startTime=None, userMobile=None, userName=None, headers=None, **kwargs):
     """
     订单列表文件导出接口-Y
     up_time=1675660544
 
     params: userMobile :  : 手机号
     params: userName :  : 用户名
     params: shopName :  : 店名
@@ -72,15 +72,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/goods/orderMain/getOrderMainPage")
-def goods_ordermain_getordermainpage(userMobile=None, modelName=None, startTime=None, endTime=None, userName=None, shopName=None, orderStatus	=None, headers=None, **kwargs):
+def goods_ordermain_getordermainpage(orderStatus	=None, modelName=None, shopName=None, endTime=None, startTime=None, userMobile=None, userName=None, headers=None, **kwargs):
     """
     订单查询接口-Y
     up_time=1675660564
 
     params: userMobile :  : 手机号
     params: userName :  : 用户名
     params: modelName :  : 车型
```

### Comparing `huhk-1.9.5/service/app_a/apis/goods/apis_goods_testdrive.py` & `huhk-1.9.6/service/app_a/apis/goods/apis_goods_testdrive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/goods/testDrive/driveExports")
-def goods_testdrive_driveexports(startTime=None, endTime=None, userName=None, shopName=None, mobile=None, channel=None, testDriveIdStr=None, exportType=None, headers=None, **kwargs):
+def goods_testdrive_driveexports(exportType=None, testDriveIdStr=None, channel=None, mobile=None, shopName=None, endTime=None, startTime=None, userName=None, headers=None, **kwargs):
     """
     试驾列表文件导出接口-Y
     up_time=1675390810
 
     params: mobile :  : 手机号
     params: userName :  : 用户名
     params: shopName :  : 店名
@@ -42,15 +42,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/goods/testDrive/page")
-def goods_testdrive_page(pageNum=None, pageSize=None, startTime=None, endTime=None, userName=None, shopName=None, mobile=None, channel=None, headers=None, **kwargs):
+def goods_testdrive_page(pageSize=None, channel=None, mobile=None, shopName=None, endTime=None, startTime=None, userName=None, pageNum=None, headers=None, **kwargs):
     """
     试驾查询接口-Y
     up_time=1675390631
 
     params: mobile :  : 手机号
     params: userName :  : 客户名
     params: shopName :  : 店名
```

### Comparing `huhk-1.9.5/service/app_a/apis/manageapi/order/apis_manageapi_order_mainorder.py` & `huhk-1.9.6/service/app_a/apis/manageapi/order/apis_manageapi_order_mainorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/manageapi/order/mainOrder/pageList")
-def manageapi_order_mainorder_pagelist(modelId=None, mainOrderId=None, channel=None, cityId=None, userName=None, dealerCode=None, createEndTime=None, extNum=None, mobile=None, orderId=None, orderType=None, createStartTime=None, current=None, orderStatus=None, extOrderStatus=None, size=None, provinceId=None, headers=None, **kwargs):
+def manageapi_order_mainorder_pagelist(extNum=None, provinceId=None, current=None, extOrderStatus=None, channel=None, createStartTime=None, createEndTime=None, mobile=None, orderId=None, orderType=None, cityId=None, mainOrderId=None, size=None, userName=None, dealerCode=None, orderStatus=None, modelId=None, headers=None, **kwargs):
     """
     订单管理-后台查询订单列表-Y
     up_time=1675752735
 
     params: mobile :  : 购买人手机号
     params: userName :  : 购买人
     params: modelId :  : 车型ID
```

### Comparing `huhk-1.9.5/service/app_a/apis/open/haohan/apis_open_haohan_relation.py` & `huhk-1.9.6/service/app_a/apis/open/haohan/apis_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/open/haohan/apis_open_haohan_rights.py` & `huhk-1.9.6/service/app_a/apis/open/haohan/apis_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/order/apis_order_freeorder.py` & `huhk-1.9.6/service/app_a/apis/order/apis_order_freeorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/order/freeOrder/downLoad")
-def order_freeorder_download(avatarUrl=None, modelId=None, userPolicyCode=None, privacyPolicyCode=None, provinceName=None, cityId=None, userName=None, regisTimeEnd=None, nickName=None, freeOrderId=None, regisTimeBegin=None, mobile=None, cityName=None, createTime=None, channel=None, channelName=None, provinceId=None, headers=None, **kwargs):
+def order_freeorder_download(regisTimeBegin=None, freeOrderId=None, avatarUrl=None, provinceId=None, channelName=None, nickName=None, channel=None, regisTimeEnd=None, privacyPolicyCode=None, mobile=None, userPolicyCode=None, cityId=None, createTime=None, cityName=None, userName=None, provinceName=None, modelId=None, headers=None, **kwargs):
     """
     导出0元订购预定信息表-Y
     up_time=1675318920
 
     params: freeOrderId : integer : 订单号
     params: modelId : string : 车型编码
     params: userName : string : 用户姓名
```

### Comparing `huhk-1.9.5/service/app_a/apis/order/apis_order_mainorder.py` & `huhk-1.9.6/service/app_a/apis/order/apis_order_mainorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/order/mainOrder/pageList")
-def order_mainorder_pagelist(createEndTime=None, createStartTime=None, current=None, sortItems=None, size=None, headers=None, **kwargs):
+def order_mainorder_pagelist(sortItems=None, current=None, createEndTime=None, createStartTime=None, size=None, headers=None, **kwargs):
     """
     小订订单分页查询（后台）-Y
     up_time=1683860159
 
     params: current : string : 
     params: size : string : 
     params: sortItems : string : 排序字段（只能是【orderMain.orderType】、【orderMain.createTime】、【orderPay.createTime】）
@@ -59,15 +59,15 @@
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 
 @allure.step(title="调接口：/order/mainOrder/downLoad")
-def order_mainorder_download(createTimeToSort=None, orderTypeToSort=None, createEndTime=None, createStartTime=None, payTimeToSort=None, headers=None, **kwargs):
+def order_mainorder_download(payTimeToSort=None, orderTypeToSort=None, createTimeToSort=None, createEndTime=None, createStartTime=None, headers=None, **kwargs):
     """
     小订订单列表导出（后台）-Y
     up_time=1675326837
 
     params: orderTypeToSort : string : 订单类型排序 不排序不赋值 正序：asc 倒序：desc
     params: createTimeToSort : string : 订单创建时间 不排序不赋值 正序：asc 倒序：desc
     params: payTimeToSort : string : 订单创建时间 不排序不赋值 正序：asc 倒序：desc
@@ -491,15 +491,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/mainOrder/syncScrmExtOrder")
-def order_mainorder_syncscrmextorder(soStatus=None, scUid=None, isArrived=None, orderId=None, createTime=None, trimCode=None, deliveryData=None, VIN=None, customerCtCode=None, syncMsg=None, chargePointEquity=None, unitTaxNo=None, dealerCode=None, unitName=None, orderAllAmount=None, phone=None, soNo=None, colorCode=None, syncStatus=None, optionCode=None, orderNo=None, modelCode=None, isTestDrive=None, customerId=None, scUname=None, seriesCode=None, updateTime=None, customerType=None, isLifetimeWarranty=None, custCertNo=None, unitInvoiceTitle=None, lifetimeWarrantyPrice=None, ossId=None, configCode=None, potentialName=None, headers=None, **kwargs):
+def order_mainorder_syncscrmextorder(orderAllAmount=None, scUid=None, lifetimeWarrantyPrice=None, syncMsg=None, seriesCode=None, orderId=None, customerId=None, VIN=None, isTestDrive=None, orderNo=None, scUname=None, isLifetimeWarranty=None, customerType=None, syncStatus=None, chargePointEquity=None, unitTaxNo=None, phone=None, soStatus=None, trimCode=None, unitInvoiceTitle=None, createTime=None, ossId=None, potentialName=None, unitName=None, modelCode=None, custCertNo=None, customerCtCode=None, configCode=None, optionCode=None, updateTime=None, colorCode=None, isArrived=None, soNo=None, deliveryData=None, dealerCode=None, headers=None, **kwargs):
     """
     SCRM第三方订单同步信息-Y
     up_time=1675406887
 
     params: ossId : string : 主键
     params: dealerCode : string : 经销商代码
     params: customerId : number : 潜客 ID
```

### Comparing `huhk-1.9.5/service/app_a/apis/order/apis_order_order.py` & `huhk-1.9.6/service/app_a/apis/order/apis_order_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/order/order/orderDetail")
-def order_order_orderdetail(pageNum=None, pageSize=None, userId=None, orderId=None, orderStatus=None, total=None, headers=None, **kwargs):
+def order_order_orderdetail(pageSize=None, total=None, orderId=None, userId=None, orderStatus=None, pageNum=None, headers=None, **kwargs):
     """
     订单详情
     up_time=1675133817
 
     params: orderId :  : 订单主单Id
     params: userId :  : 用户ID
     params: orderStatus : string : 订单状态
```

### Comparing `huhk-1.9.5/service/app_a/apis/order/apis_order_rightsorder.py` & `huhk-1.9.6/service/app_a/apis/order/apis_order_rightsorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/order/rightsOrder/export")
-def order_rightsorder_export(rightsType=None, payDateBegin=None, userId=None, payDateEnd=None, useStatus=None, orderMainId=None, receiveDateBegin=None, receiveDateEnd=None, mobile=None, rightsOrderId=None, headers=None, **kwargs):
+def order_rightsorder_export(receiveDateBegin=None, receiveDateEnd=None, payDateBegin=None, mobile=None, payDateEnd=None, useStatus=None, rightsOrderId=None, userId=None, orderMainId=None, rightsType=None, headers=None, **kwargs):
     """
     权益订单导出接口-Y
     up_time=1675414281
 
     params: userId :  : 用户ID
     params: mobile :  : 手机号码
     params: rightsOrderId :  : 权益订单ID
@@ -46,15 +46,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/rightsOrder/insert")
-def order_rightsorder_insert(refundBillNo=None, rightsType=None, updateId=None, userId=None, payAmount=None, payDate=None, useStatus=None, createBy=None, rightsName=None, orderMainId=None, refundDate=None, mobile=None, receiveDate=None, payBillNo=None, createTime=None, rightsId=None, updateTime=None, rightsOrderId=None, headers=None, **kwargs):
+def order_rightsorder_insert(payBillNo=None, createBy=None, payDate=None, payAmount=None, rightsId=None, updateId=None, mobile=None, updateTime=None, refundDate=None, useStatus=None, refundBillNo=None, receiveDate=None, createTime=None, rightsOrderId=None, userId=None, orderMainId=None, rightsName=None, rightsType=None, headers=None, **kwargs):
     """
     权益订单 - 新增-Y
     up_time=1675413078
 
     params: rightsOrderId : number : 权益订单ID
     params: rightsId : number : 权益ID
     params: rightsType : integer : 权益类型
@@ -111,15 +111,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/rightsOrder/page")
-def order_rightsorder_page(rightsType=None, payDateBegin=None, userId=None, payDateEnd=None, useStatus=None, orderMainId=None, receiveDateBegin=None, receiveDateEnd=None, mobile=None, current=None, size=None, rightsOrderId=None, headers=None, **kwargs):
+def order_rightsorder_page(receiveDateBegin=None, current=None, receiveDateEnd=None, payDateBegin=None, mobile=None, payDateEnd=None, useStatus=None, rightsOrderId=None, userId=None, size=None, orderMainId=None, rightsType=None, headers=None, **kwargs):
     """
     权益订单 - 分页查询-Y
     up_time=1675412172
 
     params: size :  : 
     params: current :  : 
     params: userId :  : 用户ID
@@ -167,15 +167,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/rightsOrder/receive")
-def order_rightsorder_receive(rightsId=None, orderId=None, headers=None, **kwargs):
+def order_rightsorder_receive(orderId=None, rightsId=None, headers=None, **kwargs):
     """
     权益-领取权益-Y
     up_time=1675660702
 
     params: orderId : string : 子订单ID
     params: rightsId : number : 权益ID
     params: headers : 请求头
@@ -214,15 +214,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/rightsOrder/getOrderList")
-def order_rightsorder_getorderlist(rightsType=None, useStatusList=None, orderMainId=None, rightsNameList=None, mobile=None, receiveDate=None, headers=None, **kwargs):
+def order_rightsorder_getorderlist(mobile=None, useStatusList=None, receiveDate=None, rightsNameList=None, orderMainId=None, rightsType=None, headers=None, **kwargs):
     """
     权益订单 - 查询-Y
     up_time=1675413979
 
     params: orderMainId : number : 主订单ID
     params: rightsType : integer : 权益类型
     params: rightsNameList : array : 权益名称
```

### Comparing `huhk-1.9.5/service/app_a/apis/order/apis_order_testdrive.py` & `huhk-1.9.6/service/app_a/apis/order/apis_order_testdrive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/order/testDrive/exportList")
-def order_testdrive_exportlist(startTime=None, endTime=None, id=None, createByName=None, shopName=None, phoneNumber=None, createTime=None, channel=None, headers=None, **kwargs):
+def order_testdrive_exportlist(phoneNumber=None, createByName=None, channel=None, shopName=None, endTime=None, startTime=None, createTime=None, id=None, headers=None, **kwargs):
     """
     导出试驾表单-Y
     up_time=1675417182
 
     params: phoneNumber :  : 手机号
     params: createByName :  : 
     params: id :  : 主键
@@ -42,15 +42,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/testDrive/userList")
-def order_testdrive_userlist(createBy=None, modelId=None, size=None, current=None, headers=None, **kwargs):
+def order_testdrive_userlist(modelId=None, createBy=None, size=None, current=None, headers=None, **kwargs):
     """
     用户中心-预约信息
     up_time=1675417772
 
     params: current :  : 当前页数
     params: size :  : 每页数据数
     params: createBy :  :
```

### Comparing `huhk-1.9.5/service/app_a/apis/order/mainorder/apis_order_mainorder_scrm2app.py` & `huhk-1.9.6/service/app_a/apis/order/mainorder/apis_order_mainorder_scrm2app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/order/mainOrder/scrm2app/refundAuditNotice")
-def order_mainorder_scrm2app_refundauditnotice(orderMainId=None, status=None, orderSubId=None, headers=None, **kwargs):
+def order_mainorder_scrm2app_refundauditnotice(orderSubId=None, status=None, orderMainId=None, headers=None, **kwargs):
     """
     订单管理-订单退款-Y
     up_time=1675660605
 
     params: orderMainId : string : 
     params: orderSubId : string : 
     params: status : integer :
```

### Comparing `huhk-1.9.5/service/app_a/apis/order/rights/apis_order_rights_rightsmanager.py` & `huhk-1.9.6/service/app_a/apis/order/rights/apis_order_rights_rightsmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/rights/rightsManager/page")
-def order_rights_rightsmanager_page(status=None, modelCode=None, effectiveEndDate=None, rightsName=None, current=None, size=None, headers=None, **kwargs):
+def order_rights_rightsmanager_page(effectiveEndDate=None, modelCode=None, current=None, status=None, size=None, rightsName=None, headers=None, **kwargs):
     """
     权益 - 分页查询-Y
     up_time=1675409025
 
     params: size :  : 
     params: current :  : 
     params: rightsName :  : 
@@ -105,15 +105,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/rights/rightsManager/getRightsList")
-def order_rights_rightsmanager_getrightslist(rightsName=None, status=None, modelId=None, effectiveStartDate=None, headers=None, **kwargs):
+def order_rights_rightsmanager_getrightslist(effectiveStartDate=None, status=None, rightsName=None, modelId=None, headers=None, **kwargs):
     """
     权益订单 - 查询-Y
     up_time=1675669230
 
     params: rightsName : string : 权益名称
     params: status : integer : 权益状态(0未生效，1已生效)
     params: modelId : string : 车型代码
@@ -162,15 +162,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/rights/rightsManager/insert")
-def order_rights_rightsmanager_insert(modelCode=None, rightsType=None, rightsName=None, orderType=None, effectiveStartDate=None, rightsId=None, headers=None, **kwargs):
+def order_rights_rightsmanager_insert(modelCode=None, rightsId=None, effectiveStartDate=None, orderType=None, rightsName=None, rightsType=None, headers=None, **kwargs):
     """
     权益-新增权益-Y
     up_time=1675669334
 
     params: effectiveStartDate : text : 权益生效时间 -- 开始
     params: rightsId : text : 权益ID
     params: rightsName : text : 权益名称
@@ -203,15 +203,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/order/rights/rightsManager/update")
-def order_rights_rightsmanager_update(effectiveEndDate=None, rightsName=None, Relation=None, effectiveStartDate=None, rightsId=None, Content=None, headers=None, **kwargs):
+def order_rights_rightsmanager_update(effectiveEndDate=None, Relation=None, rightsId=None, effectiveStartDate=None, Content=None, rightsName=None, headers=None, **kwargs):
     """
     权益-修改权益-Y
     up_time=1675669374
 
     params: rightsName : string : 权益名称
     params: rightsId : string : 权益主键
     params: Content : string : 权益描述
```

### Comparing `huhk-1.9.5/service/app_a/apis/order/rightsorder/apis_order_rightsorder_receive.py` & `huhk-1.9.6/service/app_a/apis/order/rightsorder/apis_order_rightsorder_receive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/order/rightsOrder/receive/update")
-def order_rightsorder_receive_update(refundBillNo=None, rightsType=None, updateId=None, userId=None, payAmount=None, payDate=None, useStatus=None, createBy=None, rightsName=None, orderMainId=None, refundDate=None, mobile=None, receiveDate=None, payBillNo=None, createTime=None, rightsId=None, updateTime=None, rightsOrderId=None, headers=None, **kwargs):
+def order_rightsorder_receive_update(payBillNo=None, createBy=None, payDate=None, payAmount=None, rightsId=None, updateId=None, mobile=None, updateTime=None, refundDate=None, useStatus=None, refundBillNo=None, receiveDate=None, createTime=None, rightsOrderId=None, userId=None, orderMainId=None, rightsName=None, rightsType=None, headers=None, **kwargs):
     """
     权益-编辑权益订单-Y
     up_time=1675660709
 
     params: rightsOrderId : string : 
     params: rightsId : string : 
     params: rightsType : string :
```

### Comparing `huhk-1.9.5/service/app_a/apis/pay/apis_pay_orderpaybill.py` & `huhk-1.9.6/service/app_a/apis/pay/apis_pay_orderpaybill.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_batch.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/adjustPoints/adjust/batch/save")
-def radarpoints_adjustpoints_adjust_batch_save(optAbility=None, optAbilityName=None, adjustNotes=None, redisKey=None, clientNotes=None, file=None, headers=None, **kwargs):
+def radarpoints_adjustpoints_adjust_batch_save(clientNotes=None, file=None, optAbilityName=None, redisKey=None, adjustNotes=None, optAbility=None, headers=None, **kwargs):
     """
     积分调整 - 批量调整
     up_time=1677216489
 
     params: file : file : 导入excel文件
     params: optAbility : text : 调整方式
     params: adjustNotes : text : 调整原因说明
@@ -47,15 +47,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/radarpoints/adjustPoints/adjust/batch/import")
-def radarpoints_adjustpoints_adjust_batch_import(file=None, field_34=None, adjustNotes=None, list=None, clientNotes=None, field_35=None, headers=None, **kwargs):
+def radarpoints_adjustpoints_adjust_batch_import(list=None, field_35=None, field_34=None, clientNotes=None, file=None, adjustNotes=None, headers=None, **kwargs):
     """
     积分调整 - 批量调整 - 导入excel
     up_time=1677216494
 
     params: file : file : excel文件
     params: adjustNotes : string : 调整原因说明
     params: clientNotes : string : 客户端显示信息
```

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_single.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_single.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/adjustPoints/adjust/single/save")
-def radarpoints_adjustpoints_adjust_single_save(userId=None, optAbility=None, pointsExpiration=None, adjustNotes=None, clientNotes=None, qty=None, headers=None, **kwargs):
+def radarpoints_adjustpoints_adjust_single_save(pointsExpiration=None, qty=None, clientNotes=None, adjustNotes=None, userId=None, optAbility=None, headers=None, **kwargs):
     """
     积分调整 - 单次调整
     up_time=1677216484
 
     params: optAbility : number : 积分调整类型
     params: adjustNotes : string : 调整原因说明
     params: clientNotes : string : 户端展示信息
```

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_adjustpoints.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_adjustpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/adjustPoints/pageList")
-def radarpoints_adjustpoints_pagelist(adjustTimeEnd=None, userId=None, optAbility=None, optAbilityName=None, adjustTimeBefore=None, nickName=None, adjustNotes=None, mobile=None, current=None, size=None, headers=None, **kwargs):
+def radarpoints_adjustpoints_pagelist(adjustTimeBefore=None, current=None, adjustTimeEnd=None, mobile=None, optAbilityName=None, size=None, adjustNotes=None, userId=None, nickName=None, optAbility=None, headers=None, **kwargs):
     """
     积分调整 - 分页查询
     up_time=1677209059
 
     params: userId :  : 用户id
     params: nickName :  : 用户名
     params: mobile :  : 手机号
@@ -126,15 +126,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/radarpoints/adjustPoints/export")
-def radarpoints_adjustpoints_export(adjustTimeEnd=None, userId=None, optAbility=None, optAbilityName=None, adjustTimeBefore=None, nickName=None, adjustNotes=None, mobile=None, current=None, size=None, headers=None, **kwargs):
+def radarpoints_adjustpoints_export(adjustTimeBefore=None, current=None, adjustTimeEnd=None, mobile=None, optAbilityName=None, size=None, adjustNotes=None, userId=None, nickName=None, optAbility=None, headers=None, **kwargs):
     """
     积分调整 - 导出excel
     up_time=1677216479
 
     params: userId :  : 用户id
     params: nickName :  : 用户名
     params: mobile :  : 手机号
```

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_pointsconfig.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_pointsconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/PointsConfig/page")
-def radarpoints_pointsconfig_page(pointsBegin=None, status=None, size=None, pointsExpiration=None, businessSceneType=None, Current=None, pointsEnd=None, code=None, name=None, headers=None, **kwargs):
+def radarpoints_pointsconfig_page(pointsExpiration=None, code=None, name=None, businessSceneType=None, pointsEnd=None, status=None, Current=None, size=None, pointsBegin=None, headers=None, **kwargs):
     """
     积分配置 - 分页查询
     up_time=1680142594
 
     params: code :  : 积分项Code
     params: name :  : 积分项名称
     params: businessSceneType :  : 发放场景类型
@@ -60,15 +60,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/radarpoints/PointsConfig/insert")
-def radarpoints_pointsconfig_insert(remark=None, pointsExpiration=None, points=None, bpmId=None, businessSceneType=None, userPointsDayMax=None, rulesPointsDayMax=None, toast=None, name=None, headers=None, **kwargs):
+def radarpoints_pointsconfig_insert(pointsExpiration=None, remark=None, userPointsDayMax=None, name=None, toast=None, businessSceneType=None, bpmId=None, rulesPointsDayMax=None, points=None, headers=None, **kwargs):
     """
     积分配置 -新增积分配置
     up_time=1680142659
 
     params: pointsExpiration : string : 积分有效期
     params: remark : string : 备注
     params: points : integer : 积分值
@@ -107,15 +107,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/radarpoints/PointsConfig/update")
-def radarpoints_pointsconfig_update(remark=None, pointsExpiration=None, points=None, userPointsDayMax=None, businessSceneType=None, id=None, bpmId=None, rulesPointsDayMax=None, toast=None, code=None, name=None, headers=None, **kwargs):
+def radarpoints_pointsconfig_update(pointsExpiration=None, remark=None, userPointsDayMax=None, code=None, name=None, toast=None, businessSceneType=None, bpmId=None, rulesPointsDayMax=None, points=None, id=None, headers=None, **kwargs):
     """
     积分配置 -修改积分配置
     up_time=1680142897
 
     params: pointsExpiration : string : 积分有效期
     params: remark : string : 备注
     params: points : integer : 积分值
@@ -158,15 +158,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/radarpoints/PointsConfig/updateStatusById")
-def radarpoints_pointsconfig_updatestatusbyid(status=None, id=None, headers=None, **kwargs):
+def radarpoints_pointsconfig_updatestatusbyid(id=None, status=None, headers=None, **kwargs):
     """
     积分配置 -生效状态变更
     up_time=1676455564
 
     params: id :  : 积分id
     params: status :  : 生效状态（0未生效，1已生效）
     params: headers : 请求头
```

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_pointstask.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_pointstask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/pointsTask/pageList")
-def radarpoints_pointstask_pagelist(size=None, dateLast=None, pointsConfigCode=None, pointsTaskDateSort=None, pointsConfigName=None, dateBegin=None, mobile=None, current=None, getPointsQtySort=None, headers=None, **kwargs):
+def radarpoints_pointstask_pagelist(getPointsQtySort=None, pointsTaskDateSort=None, pointsConfigName=None, dateLast=None, current=None, mobile=None, dateBegin=None, pointsConfigCode=None, size=None, headers=None, **kwargs):
     """
     积分任务 - 分页查询
     up_time=1679971837
 
     params: dateBegin :  : 开始日期
     params: dateLast :  : 结束日期
     params: pointsConfigCode :  : 任务编码
@@ -52,15 +52,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/radarpoints/pointsTask/export")
-def radarpoints_pointstask_export(dateLast=None, pointsConfigCode=None, pointsTaskDateSort=None, pointsConfigName=None, dateBegin=None, mobile=None, getPointsQtySort=None, headers=None, **kwargs):
+def radarpoints_pointstask_export(getPointsQtySort=None, pointsTaskDateSort=None, pointsConfigName=None, dateLast=None, mobile=None, dateBegin=None, pointsConfigCode=None, headers=None, **kwargs):
     """
     积分任务 - 导出excel
     up_time=1679971864
 
     params: dateBegin :  : 开始日期
     params: dateLast :  : 结束日期
     params: pointsConfigCode :  : 任务编码
```

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_summarystatistics.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_summarystatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/summaryStatistics/pageList")
-def radarpoints_summarystatistics_pagelist(flowTimeEnd=None, flowTimeBefore=None, size=None, current=None, headers=None, **kwargs):
+def radarpoints_summarystatistics_pagelist(flowTimeEnd=None, size=None, flowTimeBefore=None, current=None, headers=None, **kwargs):
     """
     积分汇总统计-分页查询积分
     up_time=1676623470
 
     params: current :  : 
     params: size :  : 
     params: flowTimeBefore :  : 流水开始时间
```

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/apis_radarpoints_userpoints.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_userpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/userPoints/pageList")
-def radarpoints_userpoints_pagelist(cumulativeAcquisitionMost=None, freezeQtyMost=None, conversionFrequencyLeast=None, size=None, registrationTimeBegin=None, userId=None, physicalIntegralMost=None, cumulativeConsumptionLeast=None, cumulativeAcquisitionLeast=None, registrationTimeEnd=None, nickName=None, physicalIntegralLeast=None, mobile=None, conversionFrequencyMost=None, cumulativeConsumptionMost=None, current=None, freezeQtyLeast=None, headers=None, **kwargs):
+def radarpoints_userpoints_pagelist(cumulativeAcquisitionMost=None, registrationTimeEnd=None, physicalIntegralMost=None, cumulativeConsumptionLeast=None, current=None, freezeQtyMost=None, cumulativeAcquisitionLeast=None, mobile=None, physicalIntegralLeast=None, freezeQtyLeast=None, conversionFrequencyMost=None, nickName=None, conversionFrequencyLeast=None, userId=None, size=None, registrationTimeBegin=None, cumulativeConsumptionMost=None, headers=None, **kwargs):
     """
     用户积分 - 分页查询
     up_time=1677209132
 
     params: userId :  : 用户id
     params: mobile :  : 用户手机号
     params: nickName :  : 用户昵称
@@ -68,15 +68,15 @@
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
 @allure.step(title="调接口：/radarpoints/userPoints/export")
-def radarpoints_userpoints_export(cumulativeAcquisitionMost=None, conversionFrequencyLeast=None, pageSize=None, registrationTimeBegin=None, physicalIntegralMost=None, currentPage=None, cumulativeConsumptionLeast=None, cumulativeAcquisitionLeast=None, registrationTimeEnd=None, nickName=None, physicalIntegralLeast=None, conversionFrequencyMost=None, cumulativeConsumptionMost=None, headers=None, **kwargs):
+def radarpoints_userpoints_export(cumulativeAcquisitionMost=None, physicalIntegralMost=None, cumulativeConsumptionLeast=None, pageSize=None, cumulativeAcquisitionLeast=None, physicalIntegralLeast=None, conversionFrequencyMost=None, nickName=None, conversionFrequencyLeast=None, registrationTimeEnd=None, currentPage=None, registrationTimeBegin=None, cumulativeConsumptionMost=None, headers=None, **kwargs):
     """
     用户积分 - 导出excel
     up_time=1677216441
 
     params: nickName :  : 用户昵称
     params: registrationTimeBegin :  : 注册时间 - 开始
     params: registrationTimeEnd :  : 注册时间 - 结束
```

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_exchangeinfo.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_exchangeinfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/userPoints/exchangeInfo/pageList")
-def radarpoints_userpoints_exchangeinfo_pagelist(consigneeName=None, orderEndTime=None, goodsOrderId=None, userId=None, orderStartTime=None, mobile=None, current=None, size=None, headers=None, **kwargs):
+def radarpoints_userpoints_exchangeinfo_pagelist(orderEndTime=None, orderStartTime=None, current=None, consigneeName=None, mobile=None, goodsOrderId=None, userId=None, size=None, headers=None, **kwargs):
     """
     用户中心-兑换明细 - 分页查询
     up_time=1676903335
 
     params: size :  : 每页大小
     params: current :  : 当前页
     params: userId :  : 用户ID
```

### Comparing `huhk-1.9.5/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_pointsinfo.py` & `huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_pointsinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import allure
 
 from service.app_a import http_requester
 from huhk.unit_request import get_url
 
 
 @allure.step(title="调接口：/radarpoints/userPoints/pointsInfo/pageList")
-def radarpoints_userpoints_pointsinfo_pagelist(userId=None, changeTimeEnd=None, businessSceneType=None, changeTimeBegin=None, current=None, size=None, name=None, headers=None, **kwargs):
+def radarpoints_userpoints_pointsinfo_pagelist(current=None, name=None, businessSceneType=None, changeTimeEnd=None, changeTimeBegin=None, userId=None, size=None, headers=None, **kwargs):
     """
     用户中心-积分明细-分页查询
     up_time=1677054547
 
     params: userId :  : 用户ID
     params: size :  : 每页大小
     params: current :  : 当前页
```

### Comparing `huhk-1.9.5/service/app_a/app_a_fun.py` & `huhk-1.9.6/service/app_a/app_a_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/admin/asserts_admin_guc.py` & `huhk-1.9.6/service/app_a/asserts/admin/asserts_admin_guc.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/admin/asserts_admin_spa.py` & `huhk-1.9.6/service/app_a/asserts/admin/asserts_admin_spa.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/asserts_activitymanager.py` & `huhk-1.9.6/service/app_a/asserts/asserts_activitymanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/asserts_app_a.py` & `huhk-1.9.6/service/app_a/asserts/asserts_app_a.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsAppA(SqlsAppA):
     @allure.step(title="接口返回结果校验")
     def assert_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["district", "province", "provinceNameSort", "cityNameSort", "dealerName", "shopBusinessType", "districtNameSort", "dealerCode", "dealerAddress", "city"])
+        # flag = self.compare_json_list(self.res, out, ["dealerAddress", "districtNameSort", "cityNameSort", "city", "province", "dealerName", "shopBusinessType", "district", "dealerCode", "provinceNameSort"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/asserts_area.py` & `huhk-1.9.6/service/app_a/asserts/asserts_area.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/asserts_content.py` & `huhk-1.9.6/service/app_a/asserts/asserts_content.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/asserts_essay.py` & `huhk-1.9.6/service/app_a/asserts/asserts_essay.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,10 +12,10 @@
         # flag = self.compare_json_list(self.res, out, ["batchType", "essayId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_essay_querylistcount(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_essay_querylistcount(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "keyWord", "startTime", "endTime", "subjectId", "author", "essayId"])
+        # flag = self.compare_json_list(self.res, out, ["author", "subjectId", "essayId", "keyWord", "endTime", "startTime", "status"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/asserts_testdrive.py` & `huhk-1.9.6/service/app_a/asserts/asserts_testdrive.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsTestdrive(SqlsTestdrive):
     @allure.step(title="接口返回结果校验")
     def assert_testdrive_subscribe(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_testdrive_subscribe(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["shopId", "appointmentTime", "modelId", "model", "shopName", "leadSourceCode", "customerName", "activityCode", "phoneNumber", "channel", "leadSanSourceCode"])
+        # flag = self.compare_json_list(self.res, out, ["leadSanSourceCode", "phoneNumber", "appointmentTime", "channel", "customerName", "activityCode", "shopName", "shopId", "leadSourceCode", "model", "modelId"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/common/asserts_common_clue.py` & `huhk-1.9.6/service/app_a/asserts/common/asserts_common_clue.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/common/asserts_common_common.py` & `huhk-1.9.6/service/app_a/asserts/common/asserts_common_common.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/common/asserts_common_remoteinterfacelog.py` & `huhk-1.9.6/service/app_a/asserts/common/asserts_common_remoteinterfacelog.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsCommonRemoteinterfacelog(SqlsCommonRemoteinterfacelog):
     @allure.step(title="接口返回结果校验")
     def assert_common_remoteinterfacelog_getlogpage(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_remoteinterfacelog_getlogpage(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["interfaceType", "startTime", "endTime", "userName", "mobile"])
+        # flag = self.compare_json_list(self.res, out, ["interfaceType", "mobile", "endTime", "startTime", "userName"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/common/asserts_common_systemversion.py` & `huhk-1.9.6/service/app_a/asserts/common/asserts_common_systemversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsCommonSystemversion(SqlsCommonSystemversion):
     @allure.step(title="接口返回结果校验")
     def assert_common_systemversion_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_systemversion_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["remark", "downloadUrl", "classify", "versionId", "version", "publishStatus", "content", "force", "name"])
+        # flag = self.compare_json_list(self.res, out, ["classify", "remark", "name", "publishStatus", "force", "downloadUrl", "version", "content", "versionId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_systemversion_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_systemversion_page(**kwargs)
         # flag = self.compare_json_list(self.res, out, [])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/common/asserts_common_user.py` & `huhk-1.9.6/service/app_a/asserts/common/asserts_common_user.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/common/asserts_common_user4c.py` & `huhk-1.9.6/service/app_a/asserts/common/asserts_common_user4c.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,22 @@
         # flag = self.compare_json_list(self.res, out, [])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "type", "createTimeEnd", "memberSystemSource", "userId", "regisTimeEnd", "lastLoginTimeStart", "lastLoginTimeEnd", "activitySource", "nickName", "regisTimeBegin", "mobile", "ownerFlag", "createTimeStart", "userSystemSource"])
+        # flag = self.compare_json_list(self.res, out, ["ownerFlag", "userSystemSource", "regisTimeBegin", "type", "lastLoginTimeEnd", "activitySource", "regisTimeEnd", "mobile", "status", "createTimeEnd", "lastLoginTimeStart", "memberSystemSource", "nickName", "userId", "createTimeStart"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_vehicleinfo(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_vehicleinfo(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["mobile", "userId"])
+        # flag = self.compare_json_list(self.res, out, ["userId", "mobile"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_getbyid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_getbyid(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["userId"])
@@ -40,64 +40,64 @@
         # flag = self.compare_json_list(self.res, out, ["userId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_download(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_download(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "type", "createTimeEnd", "memberSystemSource", "userId", "regisTimeEnd", "lastLoginTimeStart", "lastLoginTimeEnd", "activitySource", "nickName", "regisTimeBegin", "mobile", "ownerFlag", "createTimeStart", "userSystemSource", "downloadType", "userIds"])
+        # flag = self.compare_json_list(self.res, out, ["ownerFlag", "userSystemSource", "regisTimeBegin", "userIds", "type", "lastLoginTimeEnd", "activitySource", "regisTimeEnd", "mobile", "downloadType", "status", "createTimeEnd", "lastLoginTimeStart", "memberSystemSource", "nickName", "userId", "createTimeStart"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_beforepointsexport(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_beforepointsexport(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "type", "createTimeEnd", "memberSystemSource", "userId", "regisTimeEnd", "lastLoginTimeStart", "lastLoginTimeEnd", "activitySource", "nickName", "regisTimeBegin", "mobile", "ownerFlag", "createTimeStart", "userSystemSource", "downloadType", "userIds"])
+        # flag = self.compare_json_list(self.res, out, ["ownerFlag", "userSystemSource", "regisTimeBegin", "userIds", "type", "lastLoginTimeEnd", "activitySource", "regisTimeEnd", "mobile", "downloadType", "status", "createTimeEnd", "lastLoginTimeStart", "memberSystemSource", "nickName", "userId", "createTimeStart"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_insert(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_insert(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["explain", "avatarUrl", "nickName"])
+        # flag = self.compare_json_list(self.res, out, ["nickName", "explain", "avatarUrl"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_editstatus(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_editstatus(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "userId"])
+        # flag = self.compare_json_list(self.res, out, ["userId", "status"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_auditexport(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_auditexport(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userLabel", "registerType", "userId", "nickName", "ownerFlag", "userType", "phone", "downloadType", "userIds"])
+        # flag = self.compare_json_list(self.res, out, ["ownerFlag", "userLabel", "userIds", "phone", "userType", "downloadType", "registerType", "nickName", "userId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_identity(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_identity(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["userId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_updateaudit(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_updateaudit(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["auditType", "userId"])
+        # flag = self.compare_json_list(self.res, out, ["userId", "auditType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_auditlist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_auditlist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["registerType", "pageNum", "userId", "userName", "nickName", "mobile", "checkStatus"])
+        # flag = self.compare_json_list(self.res, out, ["mobile", "registerType", "checkStatus", "nickName", "userId", "userName", "pageNum"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_user4c_getuserpoints(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_user4c_getuserpoints(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["userId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/common/asserts_common_userpointsmanage.py` & `huhk-1.9.6/service/app_a/asserts/common/asserts_common_userpointsmanage.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 
 
 class AssertsCommonUserpointsmanage(SqlsCommonUserpointsmanage):
     @allure.step(title="接口返回结果校验")
     def assert_common_userpointsmanage_userpointsexport(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_userpointsmanage_userpointsexport(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["logIds", "endTime", "beginTime", "nickName", "mobile"])
+        # flag = self.compare_json_list(self.res, out, ["beginTime", "logIds", "mobile", "endTime", "nickName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_userpointsmanage_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_userpointsmanage_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["endTime", "beginTime", "mobile", "nickName"])
+        # flag = self.compare_json_list(self.res, out, ["nickName", "endTime", "beginTime", "mobile"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_userpointsmanage_manualchangeuserpoints(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_userpointsmanage_manualchangeuserpoints(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["taskName", "userId", "operatePoint", "operateMark", "pointChangType", "operateType"])
+        # flag = self.compare_json_list(self.res, out, ["operateType", "operatePoint", "pointChangType", "operateMark", "taskName", "userId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_common_userpointsmanage_beforepointsexport(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_common_userpointsmanage_beforepointsexport(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["logIds", "endTime", "beginTime", "nickName", "mobile"])
+        # flag = self.compare_json_list(self.res, out, ["beginTime", "logIds", "mobile", "endTime", "nickName"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_activitymanager.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_activitymanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 
 
 class AssertsContentActivitymanager(SqlsContentActivitymanager):
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_updateperson(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_updateperson(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["limitPeople", "activityId", "needLimitPeople"])
+        # flag = self.compare_json_list(self.res, out, ["activityId", "needLimitPeople", "limitPeople"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_updateenrolltime(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_updateenrolltime(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["enrollStartTime", "activityId", "enrollTime"])
+        # flag = self.compare_json_list(self.res, out, ["activityId", "enrollStartTime", "enrollTime"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "title", "activityId", "province", "pushTimeSort", "endTime", "beginTime", "createTimeSort", "target", "city", "activityTimeSort"])
+        # flag = self.compare_json_list(self.res, out, ["beginTime", "title", "city", "activityId", "endTime", "status", "province", "createTimeSort", "pushTimeSort", "activityTimeSort", "target"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_actinfoupdate(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_actinfoupdate(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["operationType", "activityId"])
+        # flag = self.compare_json_list(self.res, out, ["activityId", "operationType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_setactivitysort(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_setactivitysort(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["sort", "activityId"])
+        # flag = self.compare_json_list(self.res, out, ["activityId", "sort"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_getactivityinfo_(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_getactivityinfo_(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["activityId"])
@@ -61,50 +61,50 @@
         # flag = self.compare_json_list(self.res, out, ["activityId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["activityPicUrl", "activityPicURL", "beginTime", "coordinate", "reason", "status", "activityId", "enrollTime", "needLimitPeople", "endTime", "customerGroup", "limitPeople", "province", "county", "authId", "publishType", "needArea", "content", "activityAddr", "title", "enrollStartTime", "publishTime", "agreementId", "city"])
+        # flag = self.compare_json_list(self.res, out, ["enrollStartTime", "beginTime", "activityPicURL", "needArea", "limitPeople", "activityPicUrl", "publishTime", "status", "enrollTime", "customerGroup", "publishType", "activityAddr", "county", "title", "reason", "coordinate", "activityId", "authId", "needLimitPeople", "agreementId", "city", "endTime", "province", "content"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_update(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["activityPicUrl", "activityPicURL", "beginTime", "coordinate", "reason", "status", "activityId", "enrollTime", "needLimitPeople", "endTime", "customerGroup", "limitPeople", "province", "county", "authId", "publishType", "needArea", "content", "activityAddr", "title", "enrollStartTime", "publishTime", "city"])
+        # flag = self.compare_json_list(self.res, out, ["enrollStartTime", "beginTime", "activityPicURL", "needArea", "limitPeople", "activityPicUrl", "publishTime", "status", "enrollTime", "customerGroup", "publishType", "activityAddr", "county", "title", "reason", "coordinate", "activityId", "authId", "needLimitPeople", "city", "endTime", "province", "content"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_publishupdate(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_publishupdate(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "publishStatus", "activityId", "activityIds"])
+        # flag = self.compare_json_list(self.res, out, ["activityId", "publishStatus", "status", "activityIds"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_statusupdate(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_statusupdate(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["activityIds", "checkStatus"])
+        # flag = self.compare_json_list(self.res, out, ["checkStatus", "activityIds"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_enrollupdate(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_enrollupdate(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["checkEnroll", "activityIds"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_activityexport(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_activityexport(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "title", "activityId", "province", "pushTimeSort", "endTime", "beginTime", "createTimeSort", "target", "city", "activityTimeSort"])
+        # flag = self.compare_json_list(self.res, out, ["beginTime", "title", "city", "activityId", "endTime", "status", "province", "createTimeSort", "pushTimeSort", "activityTimeSort", "target"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_activitymanager_listlog(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_activitymanager_listlog(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["activityId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_adv.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_adv.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsContentAdv(SqlsContentAdv):
     @allure.step(title="接口返回结果校验")
     def assert_content_adv_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_adv_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["advLinkUrl", "version", "pictureList", "advPlaceId", "advId", "bindingFlag", "advSerial", "jumpType", "advPicUrl", "jumpContent", "advText"])
+        # flag = self.compare_json_list(self.res, out, ["advPlaceId", "bindingFlag", "advSerial", "advId", "jumpContent", "advPicUrl", "advLinkUrl", "jumpType", "pictureList", "version", "advText"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_adv_updateessayadvlist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_adv_updateessayadvlist(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["essayId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_advplace.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_advplace.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsContentAdvplace(SqlsContentAdvplace):
     @allure.step(title="接口返回结果校验")
     def assert_content_advplace_updatename(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_advplace_updatename(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["advPlaceId", "startFlag", "advPlaceName", "playTime"])
+        # flag = self.compare_json_list(self.res, out, ["advPlaceName", "advPlaceId", "startFlag", "playTime"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_agreement.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_agreement.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,22 @@
         # flag = self.compare_json_list(self.res, out, [])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_agreement_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_agreement_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["content", "version", "code", "name"])
+        # flag = self.compare_json_list(self.res, out, ["name", "content", "code", "version"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_agreement_update(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_agreement_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["name", "content", "agreementId", "code", "version"])
+        # flag = self.compare_json_list(self.res, out, ["code", "name", "agreementId", "version", "content"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_agreement_getbyid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_agreement_getbyid(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["agreementId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_campmanager.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_campmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsContentCampmanager(SqlsContentCampmanager):
     @allure.step(title="接口返回结果校验")
     def assert_content_campmanager_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_campmanager_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "sortord", "sortBody", "id", "createBy", "name"])
+        # flag = self.compare_json_list(self.res, out, ["createBy", "name", "sortBody", "status", "sortord", "id"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_campmanager_soldout(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_campmanager_soldout(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["id", "campId"])
@@ -26,24 +26,24 @@
         # flag = self.compare_json_list(self.res, out, [])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_campmanager_insert(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_campmanager_insert(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["province", "county", "discountExpEndTime", "id", "discountExpBeginTime", "campTradeTime", "url", "ownerDiscount", "content", "city", "address", "name", "campDetail"])
+        # flag = self.compare_json_list(self.res, out, ["campDetail", "county", "ownerDiscount", "name", "discountExpBeginTime", "address", "url", "city", "province", "campTradeTime", "content", "id", "discountExpEndTime"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_campmanager_detail_(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_campmanager_detail_(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["id"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_campmanager_update(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_campmanager_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["discountExpEndTime", "ownerDiscount", "discountExpBeginTime", "phone", "areaCode"])
+        # flag = self.compare_json_list(self.res, out, ["ownerDiscount", "discountExpBeginTime", "phone", "areaCode", "discountExpEndTime"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_comment.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_comment.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 
 
 class AssertsContentComment(SqlsContentComment):
     @allure.step(title="接口返回结果校验")
     def assert_content_comment_updatestatus(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_comment_updatestatus(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["fromStatus", "commentType", "toStatus", "commentId"])
+        # flag = self.compare_json_list(self.res, out, ["commentId", "fromStatus", "toStatus", "commentType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_comment_download(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_comment_download(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "contentCommentIds", "keyWord", "startTime", "endTime", "nickName", "EssayCommentIds", "mobile", "downloadType"])
+        # flag = self.compare_json_list(self.res, out, ["contentCommentIds", "EssayCommentIds", "keyWord", "mobile", "downloadType", "endTime", "startTime", "status", "nickName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_comment_commenttop(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_comment_commenttop(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["commentType", "topFlag", "commentId"])
+        # flag = self.compare_json_list(self.res, out, ["commentId", "topFlag", "commentType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_comment_list(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_comment_list(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["keyWord", "startTime", "endTime", "nickName", "checkedStatus", "mobile", "essayId", "commentType"])
+        # flag = self.compare_json_list(self.res, out, ["essayId", "keyWord", "mobile", "commentType", "endTime", "startTime", "checkedStatus", "nickName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_comment_delete(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_comment_delete(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["commentType", "toStatus", "commentId"])
+        # flag = self.compare_json_list(self.res, out, ["commentId", "toStatus", "commentType"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_commonquestion.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_commonquestion.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_contentmanager.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_contentmanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_essay.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_essay.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,29 @@
         # flag = self.compare_json_list(self.res, out, ["Key"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_essay_checklist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_essay_checklist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "StatusSortType", "keyWord", "startTime", "endTime", "CreateTimeSortType", "subjectId", "author", "essayId", "PublishTimeSortType", "recommend"])
+        # flag = self.compare_json_list(self.res, out, ["author", "subjectId", "StatusSortType", "essayId", "PublishTimeSortType", "keyWord", "endTime", "startTime", "status", "CreateTimeSortType", "recommend"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_essay_list(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_essay_list(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "StatusSortType", "keyWord", "startTime", "endTime", "CreateTimeSortType", "subjectId", "author", "essayId", "PublishTimeSortType", "recommend"])
+        # flag = self.compare_json_list(self.res, out, ["author", "subjectId", "StatusSortType", "essayId", "PublishTimeSortType", "keyWord", "endTime", "startTime", "status", "CreateTimeSortType", "recommend"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_essay_add(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_essay_add(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "essPicUrl", "title", "videoUrl", "publishTime", "publishType", "subjectId", "author", "essayId", "recommend", "content", "essayType"])
+        # flag = self.compare_json_list(self.res, out, ["videoUrl", "author", "title", "subjectId", "essayId", "publishTime", "essPicUrl", "status", "content", "publishType", "recommend", "essayType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_essay_createid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_essay_createid(**kwargs)
         # flag = self.compare_json_list(self.res, out, [])
@@ -61,10 +61,10 @@
         # flag = self.compare_json_list(self.res, out, [])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_essay_getcommentlist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_essay_getcommentlist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["parentId", "keyWord", "startTime", "endTime", "essayId", "commentId", "checkedStatus"])
+        # flag = self.compare_json_list(self.res, out, ["essayId", "commentId", "parentId", "keyWord", "endTime", "checkedStatus", "startTime"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_essaycomment.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_essaycomment.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_essayweb.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_essayweb.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsContentEssayweb(SqlsContentEssayweb):
     @allure.step(title="接口返回结果校验")
     def assert_content_essayweb_add(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_essayweb_add(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["essPicUrl", "status", "title", "publishTime", "publishType", "publishChannel", "author", "essayId", "content"])
+        # flag = self.compare_json_list(self.res, out, ["publishChannel", "author", "title", "essayId", "publishTime", "essPicUrl", "status", "content", "publishType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_essayweb_searchbykey(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_essayweb_searchbykey(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["key"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_hotcity.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_hotcity.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_hotsearch.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_hotsearch.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 
 class AssertsContentHotsearch(SqlsContentHotsearch):
     @allure.step(title="接口返回结果校验")
     def assert_content_hotsearch_rank(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_hotsearch_rank(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["kId", "rank"])
+        # flag = self.compare_json_list(self.res, out, ["rank", "kId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_hotsearch_list(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_hotsearch_list(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["kId", "rank"])
+        # flag = self.compare_json_list(self.res, out, ["rank", "kId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_hotsearch_insert(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_hotsearch_insert(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["point", "keyWord"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_material.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_material.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         # flag = self.compare_json_list(self.res, out, ["groupName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_material_addmaterial(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_material_addmaterial(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["groupId", "file"])
+        # flag = self.compare_json_list(self.res, out, ["file", "groupId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_material_getgrouplist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_material_getgrouplist(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["groupName"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_messagemanager.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_messagemanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,50 +5,50 @@
 
 
 class AssertsContentMessagemanager(SqlsContentMessagemanager):
     @allure.step(title="接口返回结果校验")
     def assert_content_messagemanager_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_messagemanager_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "cEndTime", "userId", "authId", "endTime", "beginTime", "pStartTime", "messageId", "cStartTime", "pEndTime", "content"])
+        # flag = self.compare_json_list(self.res, out, ["beginTime", "cStartTime", "pEndTime", "authId", "endTime", "messageId", "status", "pStartTime", "content", "userId", "cEndTime"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_messagemanager_getmessageinfo_(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_messagemanager_getmessageinfo_(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["messageId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_messagemanager_messagetop(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_messagemanager_messagetop(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["topFlag", "messageIds"])
+        # flag = self.compare_json_list(self.res, out, ["messageIds", "topFlag"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_messagemanager_insert(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_messagemanager_insert(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["type", "publishTime", "messageId", "sourceType", "publishType", "sendScope", "imageUrl", "content", "param", "checkPublish", "checkStatus"])
+        # flag = self.compare_json_list(self.res, out, ["sendScope", "type", "publishTime", "imageUrl", "checkPublish", "sourceType", "messageId", "checkStatus", "content", "publishType", "param"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_messagemanager_update(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_messagemanager_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["type", "messageId", "sourceType", "sendScope", "imageUrl", "userMobiles", "content", "param", "checkPublish", "checkStatus"])
+        # flag = self.compare_json_list(self.res, out, ["sendScope", "type", "userMobiles", "imageUrl", "checkPublish", "sourceType", "messageId", "checkStatus", "content", "param"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_messagemanager_publishupdate(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_messagemanager_publishupdate(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["publishStatus", "messageIds"])
+        # flag = self.compare_json_list(self.res, out, ["messageIds", "publishStatus"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_messagemanager_statusupdate(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_messagemanager_statusupdate(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["messageIds", "checkStatus"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_noticemanager.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_noticemanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         # flag = self.compare_json_list(self.res, out, [])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_noticemanager_getnoticeparamslist_(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_noticemanager_getnoticeparamslist_(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["templateType", "messageId"])
+        # flag = self.compare_json_list(self.res, out, ["messageId", "templateType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_noticemanager_noticeparamsupdate(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_noticemanager_noticeparamsupdate(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["templateType", "templateName", "templateContent"])
+        # flag = self.compare_json_list(self.res, out, ["templateContent", "templateName", "templateType"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_question.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_question.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 class AssertsContentQuestion(SqlsContentQuestion):
     @allure.step(title="接口返回结果校验")
     def assert_content_question_answerquestion(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_question_answerquestion(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["questionId", "answerContent", "author"])
+        # flag = self.compare_json_list(self.res, out, ["answerContent", "author", "questionId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_question_revoke(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_question_revoke(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["operaType", "questionId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_question_getmanegequestionlist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_question_getmanegequestionlist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "keyWord", "startTime", "endTime", "mobile"])
+        # flag = self.compare_json_list(self.res, out, ["keyWord", "mobile", "endTime", "startTime", "status"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_question_getbyid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_question_getbyid(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["questionId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_recruit.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_recruit.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsContentRecruit(SqlsContentRecruit):
     @allure.step(title="接口返回结果校验")
     def assert_content_recruit_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_recruit_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["fileName", "fileUrl"])
+        # flag = self.compare_json_list(self.res, out, ["fileUrl", "fileName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_recruit_detail(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_recruit_detail(**kwargs)
         # flag = self.compare_json_list(self.res, out, [])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_safecode.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_safecode.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_subject.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 
 
 class AssertsContentSubject(SqlsContentSubject):
     @allure.step(title="接口返回结果校验")
     def assert_content_subject_detailessay(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subject_detailessay(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["subjectId", "subjectName"])
+        # flag = self.compare_json_list(self.res, out, ["subjectName", "subjectId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subject_add(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subject_add(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "type", "parentId", "explain", "level", "subPicUrl", "subjectName"])
+        # flag = self.compare_json_list(self.res, out, ["explain", "type", "parentId", "subPicUrl", "level", "subjectName", "status"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subject_del(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subject_del(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["subjectId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subject_mobilesubject(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subject_mobilesubject(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["subjectId", "serial", "parentId"])
+        # flag = self.compare_json_list(self.res, out, ["parentId", "subjectId", "serial"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subject_getessaysubjects(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subject_getessaysubjects(**kwargs)
         # flag = self.compare_json_list(self.res, out, [])
@@ -54,10 +54,10 @@
         # flag = self.compare_json_list(self.res, out, [])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subject_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subject_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "type", "parentId", "explain", "siftFlag", "delFlag", "level", "subjectId", "subPicUrl", "isSearch", "isService", "subjectName"])
+        # flag = self.compare_json_list(self.res, out, ["subjectId", "delFlag", "explain", "type", "parentId", "subPicUrl", "siftFlag", "level", "subjectName", "status", "isSearch", "isService"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_subjectweb.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_subjectweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,29 +12,29 @@
         # flag = self.compare_json_list(self.res, out, ["subjectId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subjectweb_add(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subjectweb_add(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "type", "parentId", "subjectRank", "explain", "siftFlag", "siftPicUrl", "web", "level", "subPicUrl", "serial", "isSearch", "recommend", "isService", "subjectName"])
+        # flag = self.compare_json_list(self.res, out, ["subjectRank", "web", "type", "explain", "serial", "parentId", "subPicUrl", "siftFlag", "level", "subjectName", "status", "siftPicUrl", "isSearch", "isService", "recommend"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subjectweb_treelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subjectweb_treelist(**kwargs)
         # flag = self.compare_json_list(self.res, out, [])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subjectweb_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subjectweb_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "type", "parentId", "explain", "siftFlag", "delFlag", "subjectId", "subPicUrl", "isSearch", "isService", "subjectName"])
+        # flag = self.compare_json_list(self.res, out, ["subjectId", "delFlag", "explain", "type", "parentId", "subPicUrl", "siftFlag", "subjectName", "status", "isSearch", "isService"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_subjectweb_del(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_subjectweb_del(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["subjectId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/asserts_content_topic4c.py` & `huhk-1.9.6/service/app_a/asserts/content/asserts_content_topic4c.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,24 +19,24 @@
         # flag = self.compare_json_list(self.res, out, ["topicId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_topic4c_list(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_topic4c_list(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["topicId", "keyWord", "startTime", "endTime", "createBy"])
+        # flag = self.compare_json_list(self.res, out, ["createBy", "keyWord", "endTime", "startTime", "topicId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_topic4c_insert(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_topic4c_insert(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["author", "topicId", "topicTitle"])
+        # flag = self.compare_json_list(self.res, out, ["topicId", "author", "topicTitle"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_content_topic4c_top(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_content_topic4c_top(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["type", "topicId"])
+        # flag = self.compare_json_list(self.res, out, ["topicId", "type"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/content/material/asserts_content_material_getmateriallist.py` & `huhk-1.9.6/service/app_a/asserts/content/material/asserts_content_material_getmateriallist.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_area.py` & `huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_area.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_carmodel.py` & `huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_carmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsGoodsCarmodel(SqlsGoodsCarmodel):
     @allure.step(title="接口返回结果校验")
     def assert_goods_carmodel_savemanagecarmodel(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_carmodel_savemanagecarmodel(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["modelId", "promptDesc", "prePricePosters", "depositPrice", "carName", "carDetailUrl", "depositEndTime", "version", "status", "modelName", "preToDepositEndTime", "preToDepositStartTime", "depositStartTime", "carCode", "prePrice", "prePriceContent", "posters", "carDetailPics", "price", "sort", "modelCode", "preEndTime", "carSimpleName", "depositPriceContent", "brandName", "preStartTime", "configCode", "sharePosters", "carDetailType"])
+        # flag = self.compare_json_list(self.res, out, ["prePricePosters", "carDetailPics", "depositPrice", "carCode", "preToDepositEndTime", "preStartTime", "sharePosters", "depositEndTime", "modelId", "carDetailUrl", "price", "depositStartTime", "preEndTime", "promptDesc", "brandName", "modelName", "carSimpleName", "prePriceContent", "status", "posters", "carDetailType", "sort", "prePrice", "preToDepositStartTime", "carName", "modelCode", "configCode", "version", "depositPriceContent"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_goods_carmodel_removebyid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_carmodel_removebyid(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["modelId"])
@@ -26,15 +26,15 @@
         # flag = self.compare_json_list(self.res, out, ["modelId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_goods_carmodel_getmanagecarmodel(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_carmodel_getmanagecarmodel(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "brandName", "modelCode", "modelName", "operator", "carName", "carCode", "version"])
+        # flag = self.compare_json_list(self.res, out, ["carName", "modelCode", "operator", "brandName", "modelName", "carCode", "status", "version"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_goods_carmodel_getmodelnamelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_carmodel_getmodelnamelist(**kwargs)
         # flag = self.compare_json_list(self.res, out, [])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_configure.py` & `huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsGoodsConfigure(SqlsGoodsConfigure):
     @allure.step(title="接口返回结果校验")
     def assert_goods_configure_savecarconfigure(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_configure_savecarconfigure(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["processColorList", "salesVersionList", "interiorColorList", "appearanceColorList", "optionalList"])
+        # flag = self.compare_json_list(self.res, out, ["salesVersionList", "appearanceColorList", "interiorColorList", "processColorList", "optionalList"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_goods_configure_getcarconfigurename(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_configure_getcarconfigurename(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["modelId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_ordermain.py` & `huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_ordermain.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,22 @@
         # flag = self.compare_json_list(self.res, out, ["orderMainId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_goods_ordermain_orderexports(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_ordermain_orderexports(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userMobile", "billStatus", "modelName", "startTime", "endTime", "userName", "shopName", "testDriveIdStr", "exportType"])
+        # flag = self.compare_json_list(self.res, out, ["exportType", "testDriveIdStr", "billStatus", "modelName", "shopName", "endTime", "startTime", "userMobile", "userName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_goods_ordermain_getordermainpage(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_ordermain_getordermainpage(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userMobile", "modelName", "startTime", "endTime", "userName", "shopName", "orderStatus"])
+        # flag = self.compare_json_list(self.res, out, ["orderStatus", "modelName", "shopName", "endTime", "startTime", "userMobile", "userName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_goods_ordermain_getordermainbyid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_ordermain_getordermainbyid(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["orderMainId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/goods/asserts_goods_testdrive.py` & `huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_testdrive.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 class AssertsGoodsTestdrive(SqlsGoodsTestdrive):
     @allure.step(title="接口返回结果校验")
     def assert_goods_testdrive_driveexports(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_testdrive_driveexports(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["startTime", "endTime", "userName", "shopName", "mobile", "channel", "testDriveIdStr", "exportType"])
+        # flag = self.compare_json_list(self.res, out, ["exportType", "testDriveIdStr", "channel", "mobile", "shopName", "endTime", "startTime", "userName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_goods_testdrive_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_goods_testdrive_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["pageNum", "startTime", "endTime", "userName", "shopName", "mobile", "channel"])
+        # flag = self.compare_json_list(self.res, out, ["channel", "mobile", "shopName", "endTime", "startTime", "userName", "pageNum"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/manageapi/order/asserts_manageapi_order_mainorder.py` & `huhk-1.9.6/service/app_a/asserts/manageapi/order/asserts_manageapi_order_mainorder.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsManageapiOrderMainorder(SqlsManageapiOrderMainorder):
     @allure.step(title="接口返回结果校验")
     def assert_manageapi_order_mainorder_pagelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_manageapi_order_mainorder_pagelist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["modelId", "mainOrderId", "channel", "cityId", "userName", "dealerCode", "createEndTime", "extNum", "mobile", "orderId", "orderType", "createStartTime", "orderStatus", "extOrderStatus", "provinceId"])
+        # flag = self.compare_json_list(self.res, out, ["extNum", "provinceId", "extOrderStatus", "channel", "createStartTime", "createEndTime", "mobile", "orderId", "orderType", "cityId", "mainOrderId", "userName", "dealerCode", "orderStatus", "modelId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_manageapi_order_mainorder_detail(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_manageapi_order_mainorder_detail(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["orderId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/open/haohan/asserts_open_haohan_relation.py` & `huhk-1.9.6/service/app_a/asserts/open/haohan/asserts_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/open/haohan/asserts_open_haohan_rights.py` & `huhk-1.9.6/service/app_a/asserts/open/haohan/asserts_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/order/asserts_order_freeorder.py` & `huhk-1.9.6/service/app_a/asserts/order/asserts_order_freeorder.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsOrderFreeorder(SqlsOrderFreeorder):
     @allure.step(title="接口返回结果校验")
     def assert_order_freeorder_download(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_freeorder_download(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["avatarUrl", "modelId", "userPolicyCode", "privacyPolicyCode", "provinceName", "cityId", "userName", "regisTimeEnd", "nickName", "freeOrderId", "regisTimeBegin", "mobile", "cityName", "createTime", "channel", "channelName", "provinceId"])
+        # flag = self.compare_json_list(self.res, out, ["regisTimeBegin", "freeOrderId", "avatarUrl", "provinceId", "channelName", "nickName", "channel", "regisTimeEnd", "privacyPolicyCode", "mobile", "userPolicyCode", "cityId", "createTime", "cityName", "userName", "provinceName", "modelId"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/order/asserts_order_mainorder.py` & `huhk-1.9.6/service/app_a/asserts/order/asserts_order_mainorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 
 class AssertsOrderMainorder(SqlsOrderMainorder):
     @allure.step(title="接口返回结果校验")
     def assert_order_mainorder_pagelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_mainorder_pagelist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["createEndTime", "createStartTime", "sortItems"])
+        # flag = self.compare_json_list(self.res, out, ["sortItems", "createEndTime", "createStartTime"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_mainorder_download(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_mainorder_download(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["createTimeToSort", "orderTypeToSort", "createEndTime", "createStartTime", "payTimeToSort"])
+        # flag = self.compare_json_list(self.res, out, ["payTimeToSort", "orderTypeToSort", "createTimeToSort", "createEndTime", "createStartTime"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_mainorder_detail(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_mainorder_detail(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["orderId"])
@@ -96,15 +96,15 @@
         # flag = self.compare_json_list(self.res, out, ["orderId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_mainorder_syncscrmextorder(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_mainorder_syncscrmextorder(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["soStatus", "scUid", "isArrived", "orderId", "createTime", "trimCode", "deliveryData", "VIN", "customerCtCode", "syncMsg", "chargePointEquity", "unitTaxNo", "dealerCode", "unitName", "orderAllAmount", "phone", "soNo", "colorCode", "syncStatus", "optionCode", "orderNo", "modelCode", "isTestDrive", "customerId", "scUname", "seriesCode", "updateTime", "customerType", "isLifetimeWarranty", "custCertNo", "unitInvoiceTitle", "lifetimeWarrantyPrice", "ossId", "configCode", "potentialName"])
+        # flag = self.compare_json_list(self.res, out, ["orderAllAmount", "scUid", "lifetimeWarrantyPrice", "syncMsg", "seriesCode", "orderId", "customerId", "VIN", "isTestDrive", "orderNo", "scUname", "isLifetimeWarranty", "customerType", "syncStatus", "chargePointEquity", "unitTaxNo", "phone", "soStatus", "trimCode", "unitInvoiceTitle", "createTime", "ossId", "potentialName", "unitName", "modelCode", "custCertNo", "customerCtCode", "configCode", "optionCode", "updateTime", "colorCode", "isArrived", "soNo", "deliveryData", "dealerCode"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_mainorder_informorder(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_mainorder_informorder(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["sourceInfo", "systemCode"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/order/asserts_order_order.py` & `huhk-1.9.6/service/app_a/asserts/order/asserts_order_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsOrderOrder(SqlsOrderOrder):
     @allure.step(title="接口返回结果校验")
     def assert_order_order_orderdetail(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_order_orderdetail(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["pageNum", "userId", "orderId", "orderStatus", "total"])
+        # flag = self.compare_json_list(self.res, out, ["total", "orderId", "userId", "orderStatus", "pageNum"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_order_finish(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_order_finish(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["orderId"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/order/asserts_order_rightsorder.py` & `huhk-1.9.6/service/app_a/asserts/order/asserts_order_rightsorder.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 
 
 class AssertsOrderRightsorder(SqlsOrderRightsorder):
     @allure.step(title="接口返回结果校验")
     def assert_order_rightsorder_export(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rightsorder_export(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["rightsType", "payDateBegin", "userId", "payDateEnd", "useStatus", "orderMainId", "receiveDateBegin", "receiveDateEnd", "mobile", "rightsOrderId"])
+        # flag = self.compare_json_list(self.res, out, ["receiveDateBegin", "receiveDateEnd", "payDateBegin", "mobile", "payDateEnd", "useStatus", "rightsOrderId", "userId", "orderMainId", "rightsType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rightsorder_insert(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rightsorder_insert(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["refundBillNo", "rightsType", "updateId", "userId", "payAmount", "payDate", "useStatus", "createBy", "rightsName", "orderMainId", "refundDate", "mobile", "receiveDate", "payBillNo", "createTime", "rightsId", "updateTime", "rightsOrderId"])
+        # flag = self.compare_json_list(self.res, out, ["payBillNo", "createBy", "payDate", "payAmount", "rightsId", "updateId", "mobile", "updateTime", "refundDate", "useStatus", "refundBillNo", "receiveDate", "createTime", "rightsOrderId", "userId", "orderMainId", "rightsName", "rightsType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rightsorder_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rightsorder_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["rightsType", "payDateBegin", "userId", "payDateEnd", "useStatus", "orderMainId", "receiveDateBegin", "receiveDateEnd", "mobile", "rightsOrderId"])
+        # flag = self.compare_json_list(self.res, out, ["receiveDateBegin", "receiveDateEnd", "payDateBegin", "mobile", "payDateEnd", "useStatus", "rightsOrderId", "userId", "orderMainId", "rightsType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rightsorder_receive(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rightsorder_receive(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["rightsId", "orderId"])
+        # flag = self.compare_json_list(self.res, out, ["orderId", "rightsId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rightsorder_getorderlist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rightsorder_getorderlist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["rightsType", "useStatusList", "orderMainId", "rightsNameList", "mobile", "receiveDate"])
+        # flag = self.compare_json_list(self.res, out, ["mobile", "useStatusList", "receiveDate", "rightsNameList", "orderMainId", "rightsType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rightsorder_statusupdate(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rightsorder_statusupdate(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["workStatus", "soNo"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/order/asserts_order_testdrive.py` & `huhk-1.9.6/service/app_a/asserts/order/asserts_order_testdrive.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 class AssertsOrderTestdrive(SqlsOrderTestdrive):
     @allure.step(title="接口返回结果校验")
     def assert_order_testdrive_exportlist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_testdrive_exportlist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["startTime", "endTime", "id", "createByName", "shopName", "phoneNumber", "createTime", "channel"])
+        # flag = self.compare_json_list(self.res, out, ["phoneNumber", "createByName", "channel", "shopName", "endTime", "startTime", "createTime", "id"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_testdrive_userlist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_testdrive_userlist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["createBy", "modelId"])
+        # flag = self.compare_json_list(self.res, out, ["modelId", "createBy"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/order/mainorder/asserts_order_mainorder_scrm2app.py` & `huhk-1.9.6/service/app_a/asserts/order/mainorder/asserts_order_mainorder_scrm2app.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsOrderMainorderScrm2App(SqlsOrderMainorderScrm2App):
     @allure.step(title="接口返回结果校验")
     def assert_order_mainorder_scrm2app_refundauditnotice(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_mainorder_scrm2app_refundauditnotice(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["orderMainId", "status", "orderSubId"])
+        # flag = self.compare_json_list(self.res, out, ["orderSubId", "status", "orderMainId"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/order/rights/asserts_order_rights_rightsmanager.py` & `huhk-1.9.6/service/app_a/asserts/order/rights/asserts_order_rights_rightsmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,36 +19,36 @@
         # flag = self.compare_json_list(self.res, out, ["rightsId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rights_rightsmanager_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rights_rightsmanager_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "modelCode", "effectiveEndDate", "rightsName"])
+        # flag = self.compare_json_list(self.res, out, ["effectiveEndDate", "modelCode", "status", "rightsName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rights_rightsmanager_getrightslist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rights_rightsmanager_getrightslist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["rightsName", "status", "modelId", "effectiveStartDate"])
+        # flag = self.compare_json_list(self.res, out, ["effectiveStartDate", "status", "rightsName", "modelId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rights_rightsmanager_insert(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rights_rightsmanager_insert(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["modelCode", "rightsType", "rightsName", "orderType", "effectiveStartDate", "rightsId"])
+        # flag = self.compare_json_list(self.res, out, ["modelCode", "rightsId", "effectiveStartDate", "orderType", "rightsName", "rightsType"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rights_rightsmanager_update(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rights_rightsmanager_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["effectiveEndDate", "rightsName", "Relation", "effectiveStartDate", "rightsId", "Content"])
+        # flag = self.compare_json_list(self.res, out, ["effectiveEndDate", "Relation", "rightsId", "effectiveStartDate", "Content", "rightsName"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_order_rights_rightsmanager_rightsbyid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rights_rightsmanager_rightsbyid(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["id"])
```

### Comparing `huhk-1.9.5/service/app_a/asserts/order/rightsorder/asserts_order_rightsorder_receive.py` & `huhk-1.9.6/service/app_a/asserts/order/rightsorder/asserts_order_rightsorder_receive.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsOrderRightsorderReceive(SqlsOrderRightsorderReceive):
     @allure.step(title="接口返回结果校验")
     def assert_order_rightsorder_receive_update(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_order_rightsorder_receive_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["refundBillNo", "rightsType", "updateId", "userId", "payAmount", "payDate", "useStatus", "createBy", "rightsName", "orderMainId", "refundDate", "mobile", "receiveDate", "payBillNo", "createTime", "rightsId", "updateTime", "rightsOrderId"])
+        # flag = self.compare_json_list(self.res, out, ["payBillNo", "createBy", "payDate", "payAmount", "rightsId", "updateId", "mobile", "updateTime", "refundDate", "useStatus", "refundBillNo", "receiveDate", "createTime", "rightsOrderId", "userId", "orderMainId", "rightsName", "rightsType"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/pay/asserts_pay_orderpaybill.py` & `huhk-1.9.6/service/app_a/asserts/pay/asserts_pay_orderpaybill.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_batch.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_batch.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 class AssertsRadarpointsAdjustpointsAdjustBatch(SqlsRadarpointsAdjustpointsAdjustBatch):
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_adjustpoints_adjust_batch_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_adjustpoints_adjust_batch_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["optAbility", "optAbilityName", "adjustNotes", "redisKey", "clientNotes", "file"])
+        # flag = self.compare_json_list(self.res, out, ["clientNotes", "file", "optAbilityName", "redisKey", "adjustNotes", "optAbility"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_adjustpoints_adjust_batch_import(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_adjustpoints_adjust_batch_import(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["file", "field_34", "adjustNotes", "list", "clientNotes", "field_35"])
+        # flag = self.compare_json_list(self.res, out, ["list", "field_35", "field_34", "clientNotes", "file", "adjustNotes"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_single.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_single.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsRadarpointsAdjustpointsAdjustSingle(SqlsRadarpointsAdjustpointsAdjustSingle):
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_adjustpoints_adjust_single_save(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_adjustpoints_adjust_single_save(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userId", "optAbility", "pointsExpiration", "adjustNotes", "clientNotes", "qty"])
+        # flag = self.compare_json_list(self.res, out, ["pointsExpiration", "qty", "clientNotes", "adjustNotes", "userId", "optAbility"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_adjustpoints.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_adjustpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class AssertsRadarpointsAdjustpoints(SqlsRadarpointsAdjustpoints):
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_adjustpoints_pagelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_adjustpoints_pagelist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["adjustTimeEnd", "userId", "optAbility", "optAbilityName", "adjustTimeBefore", "nickName", "adjustNotes", "mobile"])
+        # flag = self.compare_json_list(self.res, out, ["adjustTimeBefore", "adjustTimeEnd", "mobile", "optAbilityName", "adjustNotes", "userId", "nickName", "optAbility"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_adjustpoints_getuserpointsqtybyuserid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_adjustpoints_getuserpointsqtybyuserid(**kwargs)
         # flag = self.compare_json_list(self.res, out, ["userId"])
@@ -26,10 +26,10 @@
         # flag = self.compare_json_list(self.res, out, ["mobile"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_adjustpoints_export(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_adjustpoints_export(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["adjustTimeEnd", "userId", "optAbility", "optAbilityName", "adjustTimeBefore", "nickName", "adjustNotes", "mobile"])
+        # flag = self.compare_json_list(self.res, out, ["adjustTimeBefore", "adjustTimeEnd", "mobile", "optAbilityName", "adjustNotes", "userId", "nickName", "optAbility"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_pointsconfig.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_pointsconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 
 
 class AssertsRadarpointsPointsconfig(SqlsRadarpointsPointsconfig):
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_pointsconfig_page(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_pointsconfig_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["pointsBegin", "status", "pointsExpiration", "businessSceneType", "pointsEnd", "code", "name"])
+        # flag = self.compare_json_list(self.res, out, ["pointsExpiration", "code", "name", "businessSceneType", "pointsEnd", "status", "pointsBegin"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_pointsconfig_insert(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_pointsconfig_insert(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["remark", "pointsExpiration", "points", "bpmId", "businessSceneType", "userPointsDayMax", "rulesPointsDayMax", "toast", "name"])
+        # flag = self.compare_json_list(self.res, out, ["pointsExpiration", "remark", "userPointsDayMax", "name", "toast", "businessSceneType", "bpmId", "rulesPointsDayMax", "points"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_pointsconfig_update(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_pointsconfig_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["remark", "pointsExpiration", "points", "userPointsDayMax", "businessSceneType", "id", "bpmId", "rulesPointsDayMax", "toast", "code", "name"])
+        # flag = self.compare_json_list(self.res, out, ["pointsExpiration", "remark", "userPointsDayMax", "code", "name", "toast", "businessSceneType", "bpmId", "rulesPointsDayMax", "points", "id"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_pointsconfig_updatestatusbyid(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_pointsconfig_updatestatusbyid(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["status", "id"])
+        # flag = self.compare_json_list(self.res, out, ["id", "status"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_pointstask.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_pointstask.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 class AssertsRadarpointsPointstask(SqlsRadarpointsPointstask):
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_pointstask_pagelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_pointstask_pagelist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["dateLast", "pointsConfigCode", "pointsTaskDateSort", "pointsConfigName", "dateBegin", "mobile", "getPointsQtySort"])
+        # flag = self.compare_json_list(self.res, out, ["getPointsQtySort", "pointsTaskDateSort", "pointsConfigName", "dateLast", "mobile", "dateBegin", "pointsConfigCode"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_pointstask_export(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_pointstask_export(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["dateLast", "pointsConfigCode", "pointsTaskDateSort", "pointsConfigName", "dateBegin", "mobile", "getPointsQtySort"])
+        # flag = self.compare_json_list(self.res, out, ["getPointsQtySort", "pointsTaskDateSort", "pointsConfigName", "dateLast", "mobile", "dateBegin", "pointsConfigCode"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_summarystatistics.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_summarystatistics.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/asserts_radarpoints_userpoints.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_userpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 class AssertsRadarpointsUserpoints(SqlsRadarpointsUserpoints):
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_userpoints_pagelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_userpoints_pagelist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["cumulativeAcquisitionMost", "freezeQtyMost", "conversionFrequencyLeast", "registrationTimeBegin", "userId", "physicalIntegralMost", "cumulativeConsumptionLeast", "cumulativeAcquisitionLeast", "registrationTimeEnd", "nickName", "physicalIntegralLeast", "mobile", "conversionFrequencyMost", "cumulativeConsumptionMost", "freezeQtyLeast"])
+        # flag = self.compare_json_list(self.res, out, ["cumulativeAcquisitionMost", "registrationTimeEnd", "physicalIntegralMost", "cumulativeConsumptionLeast", "freezeQtyMost", "cumulativeAcquisitionLeast", "mobile", "physicalIntegralLeast", "freezeQtyLeast", "conversionFrequencyMost", "nickName", "conversionFrequencyLeast", "userId", "registrationTimeBegin", "cumulativeConsumptionMost"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_userpoints_export(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_userpoints_export(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["cumulativeAcquisitionMost", "conversionFrequencyLeast", "registrationTimeBegin", "physicalIntegralMost", "cumulativeConsumptionLeast", "cumulativeAcquisitionLeast", "registrationTimeEnd", "nickName", "physicalIntegralLeast", "conversionFrequencyMost", "cumulativeConsumptionMost"])
+        # flag = self.compare_json_list(self.res, out, ["cumulativeAcquisitionMost", "physicalIntegralMost", "cumulativeConsumptionLeast", "cumulativeAcquisitionLeast", "physicalIntegralLeast", "conversionFrequencyMost", "nickName", "conversionFrequencyLeast", "registrationTimeEnd", "registrationTimeBegin", "cumulativeConsumptionMost"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_exchangeinfo.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_exchangeinfo.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsRadarpointsUserpointsExchangeinfo(SqlsRadarpointsUserpointsExchangeinfo):
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_userpoints_exchangeinfo_pagelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_userpoints_exchangeinfo_pagelist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["consigneeName", "orderEndTime", "goodsOrderId", "userId", "orderStartTime", "mobile"])
+        # flag = self.compare_json_list(self.res, out, ["orderEndTime", "orderStartTime", "consigneeName", "mobile", "goodsOrderId", "userId"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_pointsinfo.py` & `huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_pointsinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 
 class AssertsRadarpointsUserpointsPointsinfo(SqlsRadarpointsUserpointsPointsinfo):
     @allure.step(title="接口返回结果校验")
     def assert_radarpoints_userpoints_pointsinfo_pagelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
         # out = self.sql_radarpoints_userpoints_pointsinfo_pagelist(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userId", "changeTimeEnd", "businessSceneType", "changeTimeBegin", "name"])
+        # flag = self.compare_json_list(self.res, out, ["name", "businessSceneType", "changeTimeEnd", "changeTimeBegin", "userId"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.9.5/service/app_a/funs/admin/funs_admin_guc.py` & `huhk-1.9.6/service/app_a/funs/admin/funs_admin_guc.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/admin/funs_admin_spa.py` & `huhk-1.9.6/service/app_a/funs/admin/funs_admin_spa.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/common/funs_common_clue.py` & `huhk-1.9.6/service/app_a/funs/common/funs_common_clue.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.common.asserts_common_clue import AssertsCommonClue
 from service.app_a.apis.common import apis_common_clue
 
 
 class FunsCommonClue(AssertsCommonClue):
     @allure.step(title="用户列表-详情-查询线索-Y")
-    def common_clue_getclueuserpage(self, size=10, current=1, userId="$None$", _assert=True,  **kwargs):
+    def common_clue_getclueuserpage(self, userId="$None$", size=10, current=1, _assert=True,  **kwargs):
         """
             url=/common/clue/getClueUserPage
                 params: current :  : 页码
                 params: size :  : 每页大小
                 params: headers : 请求头
         """
         userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
```

### Comparing `huhk-1.9.5/service/app_a/funs/common/funs_common_common.py` & `huhk-1.9.6/service/app_a/funs/common/funs_common_common.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/common/funs_common_remoteinterfacelog.py` & `huhk-1.9.6/service/app_a/funs/common/funs_common_remoteinterfacelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from service.app_a.asserts.common.asserts_common_remoteinterfacelog import AssertsCommonRemoteinterfacelog
 from service.app_a.apis.common import apis_common_remoteinterfacelog
 
 
 class FunsCommonRemoteinterfacelog(AssertsCommonRemoteinterfacelog):
     @allure.step(title="查询三方日志接口-Y")
-    def common_remoteinterfacelog_getlogpage(self, interfaceType="$None$", startTime="$None$", endTime="$None$", userName="$None$", mobile="$None$", current=1, size=10, _assert=True,  **kwargs):
+    def common_remoteinterfacelog_getlogpage(self, interfaceType="$None$", current=1, mobile="$None$", size=10, endTime="$None$", startTime="$None$", userName="$None$", _assert=True,  **kwargs):
         """
             url=/common/remoteinterfacelog/getLogPage
                 params: interfaceType :  : 日志类型（1.支付日志  2.退款日志  3.换电日志）
                 params: startTime :  : 开始时间
                 params: endTime :  : 结束时间
                 params: userName :  : 用户昵称
                 params: mobile :  : 手机号
                 params: size :  : 每页条数
                 params: current :  : 当前页
                 params: headers : 请求头
         """
         interfaceType = self.get_list_choice(interfaceType, list_or_dict=None, key="interfaceType")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
         userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
-        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_remoteinterfacelog.common_remoteinterfacelog_getlogpage(**_kwargs)
 
         self.assert_common_remoteinterfacelog_getlogpage(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/common/funs_common_systemversion.py` & `huhk-1.9.6/service/app_a/funs/common/funs_common_systemversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 
 from service.app_a.asserts.common.asserts_common_systemversion import AssertsCommonSystemversion
 from service.app_a.apis.common import apis_common_systemversion
 
 
 class FunsCommonSystemversion(AssertsCommonSystemversion):
     @allure.step(title="保存版本信息-Y")
-    def common_systemversion_save(self, remark="$None$", downloadUrl="$None$", classify="$None$", versionId="$None$", version="$None$", publishStatus="$None$", content="$None$", force="$None$", size=10, name="$None$", _assert=True,  **kwargs):
+    def common_systemversion_save(self, classify="$None$", remark="$None$", name="$None$", publishStatus="$None$", force="$None$", downloadUrl="$None$", version="$None$", content="$None$", size=10, versionId="$None$", _assert=True,  **kwargs):
         """
             url=/common/systemversion/save
                 params: version : string : 版本号
                 params: name : string : 版本名称
                 params: content : string : 更新内容
                 params: remark : string : 备注
                 params: classify : string :  Android或IOS
                 params: force : string : 强制更新0.否1.是
                 params: downloadUrl : string : 下载路径
                 params: size : string : 大小
                 params: versionId : number : 主键，更新传，新增不传
                 params: publishStatus : number : 0. 未发布 1.已发布
                 params: headers : 请求头
         """
+        classify = self.get_list_choice(classify, list_or_dict=None, key="classify")
         remark = self.get_list_choice(remark, list_or_dict=None, key="remark")
+        name = self.get_list_choice(name, list_or_dict=None, key="name")
+        publishStatus = self.get_list_choice(publishStatus, list_or_dict=None, key="publishStatus")
+        force = self.get_list_choice(force, list_or_dict=None, key="force")
         downloadUrl = self.get_list_choice(downloadUrl, list_or_dict=None, key="downloadUrl")
-        classify = self.get_list_choice(classify, list_or_dict=None, key="classify")
-        versionId = self.get_list_choice(versionId, list_or_dict=None, key="versionId")
         version = self.get_list_choice(version, list_or_dict=None, key="version")
-        publishStatus = self.get_list_choice(publishStatus, list_or_dict=None, key="publishStatus")
         content = self.get_list_choice(content, list_or_dict=None, key="content")
-        force = self.get_list_choice(force, list_or_dict=None, key="force")
-        name = self.get_list_choice(name, list_or_dict=None, key="name")
+        versionId = self.get_list_choice(versionId, list_or_dict=None, key="versionId")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_systemversion.common_systemversion_save(**_kwargs)
 
         self.assert_common_systemversion_save(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/common/funs_common_user.py` & `huhk-1.9.6/service/app_a/funs/common/funs_common_user.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/common/funs_common_user4c.py` & `huhk-1.9.6/service/app_a/funs/common/funs_common_user4c.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
         self.assert_common_user4c_queryactivitysource(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户列表-查询-Y")
-    def common_user4c_page(self, status="$None$", type="$None$", createTimeEnd="$None$", memberSystemSource="$None$", userId="$None$", regisTimeEnd="$None$", lastLoginTimeStart="$None$", lastLoginTimeEnd="$None$", activitySource="$None$", nickName="$None$", regisTimeBegin="$None$", mobile="$None$", ownerFlag="$None$", current=1, createTimeStart="$None$", userSystemSource="$None$", size=10, _assert=True,  **kwargs):
+    def common_user4c_page(self, ownerFlag="$None$", userSystemSource="$None$", regisTimeBegin="$None$", type="$None$", lastLoginTimeEnd="$None$", current=1, activitySource="$None$", regisTimeEnd="$None$", mobile="$None$", status="$None$", createTimeEnd="$None$", lastLoginTimeStart="$None$", memberSystemSource="$None$", nickName="$None$", userId="$None$", size=10, createTimeStart="$None$", _assert=True,  **kwargs):
         """
             url=/common/user4C/page
                 params: mobile :  : 用户手机号码
                 params: nickName :  : 用户昵称
                 params: status :  : 会员状态 0：禁用 1：启用
                 params: type :  : 用户类型 0：注册 1：非注册
                 params: memberSystemSource :  : 会员来源系统： 1：APP、2：微信小程序、3：官网、4：H5
@@ -37,49 +37,49 @@
                 params: createTimeEnd :  : 用户创建结束时间
                 params: regisTimeBegin :  : 会员注册开始时间
                 params: regisTimeEnd :  : 会员注册结束时间
                 params: lastLoginTimeStart :  : 用户最近登录开始时间
                 params: lastLoginTimeEnd :  : 用户最近登录结束时间
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        ownerFlag = self.get_list_choice(ownerFlag, list_or_dict=None, key="ownerFlag")
+        userSystemSource = self.get_list_choice(userSystemSource, list_or_dict=None, key="userSystemSource")
+        regisTimeBegin = self.get_list_choice(regisTimeBegin, list_or_dict=None, key="regisTimeBegin")
         type = self.get_list_choice(type, list_or_dict=None, key="type")
-        createTimeEnd = self.get_list_choice(createTimeEnd, list_or_dict=None, key="createTimeEnd")
-        memberSystemSource = self.get_list_choice(memberSystemSource, list_or_dict=None, key="memberSystemSource")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        regisTimeEnd = self.get_list_choice(regisTimeEnd, list_or_dict=None, key="regisTimeEnd")
-        lastLoginTimeStart = self.get_list_choice(lastLoginTimeStart, list_or_dict=None, key="lastLoginTimeStart")
         lastLoginTimeEnd = self.get_list_choice(lastLoginTimeEnd, list_or_dict=None, key="lastLoginTimeEnd")
         activitySource = self.get_list_choice(activitySource, list_or_dict=None, key="activitySource")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
-        regisTimeBegin = self.get_list_choice(regisTimeBegin, list_or_dict=None, key="regisTimeBegin")
+        regisTimeEnd = self.get_list_choice(regisTimeEnd, list_or_dict=None, key="regisTimeEnd")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        ownerFlag = self.get_list_choice(ownerFlag, list_or_dict=None, key="ownerFlag")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        createTimeEnd = self.get_list_choice(createTimeEnd, list_or_dict=None, key="createTimeEnd")
+        lastLoginTimeStart = self.get_list_choice(lastLoginTimeStart, list_or_dict=None, key="lastLoginTimeStart")
+        memberSystemSource = self.get_list_choice(memberSystemSource, list_or_dict=None, key="memberSystemSource")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
         createTimeStart = self.get_list_choice(createTimeStart, list_or_dict=None, key="createTimeStart")
-        userSystemSource = self.get_list_choice(userSystemSource, list_or_dict=None, key="userSystemSource")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_page(**_kwargs)
 
         self.assert_common_user4c_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户列表-详情-车辆信息-Y")
-    def common_user4c_vehicleinfo(self, mobile="$None$", size=10, current=1, userId="$None$", _assert=True,  **kwargs):
+    def common_user4c_vehicleinfo(self, userId="$None$", size=10, mobile="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/common/user4C/vehicleInfo
                 params: mobile :  : 用户手机号码
                 params: current :  : 页码
                 params: size :  : 每页大小
                 params: headers : 请求头
         """
-        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
         userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_vehicleinfo(**_kwargs)
 
         self.assert_common_user4c_vehicleinfo(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
@@ -113,15 +113,15 @@
         self.res = apis_common_user4c.common_user4c_updateuser(**_kwargs)
 
         self.assert_common_user4c_updateuser(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户列表-导出-Y")
-    def common_user4c_download(self, status="$None$", type="$None$", createTimeEnd="$None$", memberSystemSource="$None$", userId="$None$", regisTimeEnd="$None$", lastLoginTimeStart="$None$", lastLoginTimeEnd="$None$", activitySource="$None$", nickName="$None$", regisTimeBegin="$None$", mobile="$None$", ownerFlag="$None$", createTimeStart="$None$", userSystemSource="$None$", downloadType="$None$", userIds="$None$", _assert=True,  **kwargs):
+    def common_user4c_download(self, ownerFlag="$None$", userSystemSource="$None$", regisTimeBegin="$None$", userIds="$None$", type="$None$", lastLoginTimeEnd="$None$", activitySource="$None$", regisTimeEnd="$None$", mobile="$None$", downloadType="$None$", status="$None$", createTimeEnd="$None$", lastLoginTimeStart="$None$", memberSystemSource="$None$", nickName="$None$", userId="$None$", createTimeStart="$None$", _assert=True,  **kwargs):
         """
             url=/common/user4C/download
                 params: mobile :  : 用户手机号
                 params: nickName :  : 用户昵称
                 params: status :  : 会员状态 0：禁用 1：启用
                 params: type :  : 用户类型 0：注册 1：非注册
                 params: memberSystemSource :  : 会员来源系统： 1：APP、2：微信小程序、3：官网、4：H5
@@ -133,42 +133,42 @@
                 params: regisTimeBegin :  : 会员注册开始时间
                 params: regisTimeEnd :  : 会员注册结束时间
                 params: lastLoginTimeStart :  : 会员最近登录开始时间
                 params: lastLoginTimeEnd :  : 会员最近登录结束时间
                 params: downloadType :  : 导出类型 1: 条件导出 2: 批量导出
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        ownerFlag = self.get_list_choice(ownerFlag, list_or_dict=None, key="ownerFlag")
+        userSystemSource = self.get_list_choice(userSystemSource, list_or_dict=None, key="userSystemSource")
+        regisTimeBegin = self.get_list_choice(regisTimeBegin, list_or_dict=None, key="regisTimeBegin")
+        userIds = self.get_list_choice(userIds, list_or_dict=None, key="userIds")
         type = self.get_list_choice(type, list_or_dict=None, key="type")
-        createTimeEnd = self.get_list_choice(createTimeEnd, list_or_dict=None, key="createTimeEnd")
-        memberSystemSource = self.get_list_choice(memberSystemSource, list_or_dict=None, key="memberSystemSource")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        regisTimeEnd = self.get_list_choice(regisTimeEnd, list_or_dict=None, key="regisTimeEnd")
-        lastLoginTimeStart = self.get_list_choice(lastLoginTimeStart, list_or_dict=None, key="lastLoginTimeStart")
         lastLoginTimeEnd = self.get_list_choice(lastLoginTimeEnd, list_or_dict=None, key="lastLoginTimeEnd")
         activitySource = self.get_list_choice(activitySource, list_or_dict=None, key="activitySource")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
-        regisTimeBegin = self.get_list_choice(regisTimeBegin, list_or_dict=None, key="regisTimeBegin")
+        regisTimeEnd = self.get_list_choice(regisTimeEnd, list_or_dict=None, key="regisTimeEnd")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        ownerFlag = self.get_list_choice(ownerFlag, list_or_dict=None, key="ownerFlag")
-        createTimeStart = self.get_list_choice(createTimeStart, list_or_dict=None, key="createTimeStart")
-        userSystemSource = self.get_list_choice(userSystemSource, list_or_dict=None, key="userSystemSource")
         downloadType = self.get_list_choice(downloadType, list_or_dict=None, key="downloadType")
-        userIds = self.get_list_choice(userIds, list_or_dict=None, key="userIds")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        createTimeEnd = self.get_list_choice(createTimeEnd, list_or_dict=None, key="createTimeEnd")
+        lastLoginTimeStart = self.get_list_choice(lastLoginTimeStart, list_or_dict=None, key="lastLoginTimeStart")
+        memberSystemSource = self.get_list_choice(memberSystemSource, list_or_dict=None, key="memberSystemSource")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        createTimeStart = self.get_list_choice(createTimeStart, list_or_dict=None, key="createTimeStart")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_download(**_kwargs)
 
         self.assert_common_user4c_download(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户列表-导出前置判断-Y")
-    def common_user4c_beforepointsexport(self, status="$None$", type="$None$", createTimeEnd="$None$", memberSystemSource="$None$", userId="$None$", regisTimeEnd="$None$", lastLoginTimeStart="$None$", lastLoginTimeEnd="$None$", activitySource="$None$", nickName="$None$", regisTimeBegin="$None$", mobile="$None$", ownerFlag="$None$", createTimeStart="$None$", userSystemSource="$None$", downloadType="$None$", userIds="$None$", _assert=True,  **kwargs):
+    def common_user4c_beforepointsexport(self, ownerFlag="$None$", userSystemSource="$None$", regisTimeBegin="$None$", userIds="$None$", type="$None$", lastLoginTimeEnd="$None$", activitySource="$None$", regisTimeEnd="$None$", mobile="$None$", downloadType="$None$", status="$None$", createTimeEnd="$None$", lastLoginTimeStart="$None$", memberSystemSource="$None$", nickName="$None$", userId="$None$", createTimeStart="$None$", _assert=True,  **kwargs):
         """
             url=/common/user4C/beforePointsExport
                 params: mobile :  : 用户手机号
                 params: nickName :  : 用户昵称
                 params: status :  : 账号状态 0：禁用 1：启用
                 params: type :  : 用户类型 0：注册 1：非注册
                 params: memberSystemSource :  : 用户来源系统： 1：APP、2：微信小程序、3：官网、4：H5
@@ -180,99 +180,99 @@
                 params: regisTimeBegin :  : 会员注册开始时间
                 params: regisTimeEnd :  : 会员注册结束时间
                 params: lastLoginTimeStart :  : 会员最近登录开始时间
                 params: lastLoginTimeEnd :  : 会员最近登录结束时间
                 params: downloadType :  : 1：条件导出 2：批量导出
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        ownerFlag = self.get_list_choice(ownerFlag, list_or_dict=None, key="ownerFlag")
+        userSystemSource = self.get_list_choice(userSystemSource, list_or_dict=None, key="userSystemSource")
+        regisTimeBegin = self.get_list_choice(regisTimeBegin, list_or_dict=None, key="regisTimeBegin")
+        userIds = self.get_list_choice(userIds, list_or_dict=None, key="userIds")
         type = self.get_list_choice(type, list_or_dict=None, key="type")
-        createTimeEnd = self.get_list_choice(createTimeEnd, list_or_dict=None, key="createTimeEnd")
-        memberSystemSource = self.get_list_choice(memberSystemSource, list_or_dict=None, key="memberSystemSource")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        regisTimeEnd = self.get_list_choice(regisTimeEnd, list_or_dict=None, key="regisTimeEnd")
-        lastLoginTimeStart = self.get_list_choice(lastLoginTimeStart, list_or_dict=None, key="lastLoginTimeStart")
         lastLoginTimeEnd = self.get_list_choice(lastLoginTimeEnd, list_or_dict=None, key="lastLoginTimeEnd")
         activitySource = self.get_list_choice(activitySource, list_or_dict=None, key="activitySource")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
-        regisTimeBegin = self.get_list_choice(regisTimeBegin, list_or_dict=None, key="regisTimeBegin")
+        regisTimeEnd = self.get_list_choice(regisTimeEnd, list_or_dict=None, key="regisTimeEnd")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        ownerFlag = self.get_list_choice(ownerFlag, list_or_dict=None, key="ownerFlag")
-        createTimeStart = self.get_list_choice(createTimeStart, list_or_dict=None, key="createTimeStart")
-        userSystemSource = self.get_list_choice(userSystemSource, list_or_dict=None, key="userSystemSource")
         downloadType = self.get_list_choice(downloadType, list_or_dict=None, key="downloadType")
-        userIds = self.get_list_choice(userIds, list_or_dict=None, key="userIds")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        createTimeEnd = self.get_list_choice(createTimeEnd, list_or_dict=None, key="createTimeEnd")
+        lastLoginTimeStart = self.get_list_choice(lastLoginTimeStart, list_or_dict=None, key="lastLoginTimeStart")
+        memberSystemSource = self.get_list_choice(memberSystemSource, list_or_dict=None, key="memberSystemSource")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        createTimeStart = self.get_list_choice(createTimeStart, list_or_dict=None, key="createTimeStart")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_beforepointsexport(**_kwargs)
 
         self.assert_common_user4c_beforepointsexport(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户列表-新增-Y")
-    def common_user4c_insert(self, explain="$None$", avatarUrl="$None$", nickName="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def common_user4c_insert(self, nickName="$None$", explain="$None$", avatarUrl="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/common/user4C/insert
                 params: avatarUrl : text : String；图片地址
                 params: explain : text : String；简介
                 params: nickName : text : String；昵称
                 params: headers : 请求头
         """
+        nickName = self.get_value_choice(nickName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         explain = self.get_value_choice(explain, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         avatarUrl = self.get_value_choice(avatarUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        nickName = self.get_value_choice(nickName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_insert(**_kwargs)
 
         self.assert_common_user4c_insert(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户中心-禁用/启用用户-Y")
-    def common_user4c_editstatus(self, status="$None$", userId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def common_user4c_editstatus(self, userId="$None$", status="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/common/user4C/editStatus
                 params: status : number : 是否启用0：禁用 1：启用
                 params: headers : 请求头
         """
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_editstatus(**_kwargs)
 
         self.assert_common_user4c_editstatus(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="导出用户审核列表-Y")
-    def common_user4c_auditexport(self, userLabel="$None$", registerType="$None$", userId="$None$", nickName="$None$", ownerFlag="$None$", userType="$None$", phone="$None$", downloadType="$None$", userIds="$None$", _assert=True,  **kwargs):
+    def common_user4c_auditexport(self, ownerFlag="$None$", userLabel="$None$", userIds="$None$", phone="$None$", userType="$None$", downloadType="$None$", registerType="$None$", nickName="$None$", userId="$None$", _assert=True,  **kwargs):
         """
             url=/common/user4C/auditExport
                 params: phone :  : 手机号
                 params: nickName :  : 昵称
                 params: ownerFlag :  : 是否车主认证1：是0：否
                 params: userLabel :  : 用户标签
                 params: registerType :  : 用户来源
                 params: userType :  : 用户类型
                 params: downloadType :  : 下载类型1：根据搜索条件导出2：多选导出
                 params: headers : 请求头
         """
-        userLabel = self.get_list_choice(userLabel, list_or_dict=None, key="userLabel")
-        registerType = self.get_list_choice(registerType, list_or_dict=None, key="registerType")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
         ownerFlag = self.get_list_choice(ownerFlag, list_or_dict=None, key="ownerFlag")
-        userType = self.get_list_choice(userType, list_or_dict=None, key="userType")
+        userLabel = self.get_list_choice(userLabel, list_or_dict=None, key="userLabel")
+        userIds = self.get_list_choice(userIds, list_or_dict=None, key="userIds")
         phone = self.get_list_choice(phone, list_or_dict=None, key="phone")
+        userType = self.get_list_choice(userType, list_or_dict=None, key="userType")
         downloadType = self.get_list_choice(downloadType, list_or_dict=None, key="downloadType")
-        userIds = self.get_list_choice(userIds, list_or_dict=None, key="userIds")
+        registerType = self.get_list_choice(registerType, list_or_dict=None, key="registerType")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_auditexport(**_kwargs)
 
         self.assert_common_user4c_auditexport(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
@@ -291,50 +291,50 @@
 
         self.assert_common_user4c_identity(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="更新审核状态-Y")
-    def common_user4c_updateaudit(self, auditType="$None$", userId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def common_user4c_updateaudit(self, userId="$None$", auditType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/common/user4C/updateAudit
                 params: auditType : integer : 认证类型（1：注销审核单据，2：车主认证审核单据）
                 params: headers : 请求头
         """
-        auditType = self.get_value_choice(auditType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        auditType = self.get_value_choice(auditType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_updateaudit(**_kwargs)
 
         self.assert_common_user4c_updateaudit(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="根据用户审核状态搜索列表-Y")
-    def common_user4c_auditlist(self, registerType="$None$", pageNum=1, pageSize="$None$", userId="$None$", userName="$None$", nickName="$None$", mobile="$None$", checkStatus="$None$", _assert=True,  **kwargs):
+    def common_user4c_auditlist(self, pageSize="$None$", mobile="$None$", registerType="$None$", checkStatus="$None$", nickName="$None$", userId="$None$", userName="$None$", pageNum=1, _assert=True,  **kwargs):
         """
             url=/common/user4C/auditList
                 params: mobile :  : 手机号
                 params: nickName :  : 用户昵称
                 params: userName :  : 用户实名姓名
                 params: registerType :  : 用户来源
                 params: pageSize :  : 每页数量
                 params: pageNum :  : 当前页数
                 params: checkStatus :  : 状态 0-正常 1-审核中 2-通过3-审核不通过
                 params: headers : 请求头
         """
-        registerType = self.get_list_choice(registerType, list_or_dict=None, key="registerType")
         pageSize = self.get_list_choice(pageSize, list_or_dict=None, key="pageSize")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        registerType = self.get_list_choice(registerType, list_or_dict=None, key="registerType")
         checkStatus = self.get_list_choice(checkStatus, list_or_dict=None, key="checkStatus")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_user4c.common_user4c_auditlist(**_kwargs)
 
         self.assert_common_user4c_auditlist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/common/funs_common_userpointsmanage.py` & `huhk-1.9.6/service/app_a/funs/common/funs_common_userpointsmanage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,102 +2,102 @@
 
 from service.app_a.asserts.common.asserts_common_userpointsmanage import AssertsCommonUserpointsmanage
 from service.app_a.apis.common import apis_common_userpointsmanage
 
 
 class FunsCommonUserpointsmanage(AssertsCommonUserpointsmanage):
     @allure.step(title="用户积分列表导出-历史接口")
-    def common_userpointsmanage_userpointsexport(self, logIds="$None$", endTime="$None$", beginTime="$None$", nickName="$None$", mobile="$None$", _assert=True,  **kwargs):
+    def common_userpointsmanage_userpointsexport(self, beginTime="$None$", logIds="$None$", mobile="$None$", endTime="$None$", nickName="$None$", _assert=True,  **kwargs):
         """
             url=/common/userPointsManage/userPointsExport
                 params: nickName :  : 用户昵称
                 params: mobile :  : 用户手机号
                 params: beginTime :  : 注册时间查询范围--开始时间
                 params: endTime :  : 注册时间查询范围--结束时间
                 params: logIds :  : 积分明细Id，用于积分导出，如果传参表示勾选数据导出
                 params: headers : 请求头
         """
+        beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
         logIds = self.get_list_choice(logIds, list_or_dict=None, key="logIds")
+        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
         nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
-        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_userpointsmanage.common_userpointsmanage_userpointsexport(**_kwargs)
 
         self.assert_common_userpointsmanage_userpointsexport(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户积分列表查询-历史接口")
-    def common_userpointsmanage_page(self, endTime="$None$", beginTime="$None$", mobile="$None$", nickName="$None$", _assert=True,  **kwargs):
+    def common_userpointsmanage_page(self, nickName="$None$", endTime="$None$", beginTime="$None$", mobile="$None$", _assert=True,  **kwargs):
         """
             url=/common/userPointsManage/page
                 params: nickName :  :
                 params: mobile :  :
                 params: beginTime :  : 前端日期后面必须要追加 00:00:00
                 params: endTime :  : 前端日期后面必须要追加 23:59:59
                 params: headers : 请求头
         """
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
         beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_userpointsmanage.common_userpointsmanage_page(**_kwargs)
 
         self.assert_common_userpointsmanage_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户积分手动调整-历史接口")
-    def common_userpointsmanage_manualchangeuserpoints(self, taskName="$None$", userId="$None$", operatePoint="$None$", operateMark="$None$", pointChangType="$None$", operateType="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def common_userpointsmanage_manualchangeuserpoints(self, operateType="$None$", operatePoint="$None$", pointChangType="$None$", operateMark="$None$", taskName="$None$", userId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/common/userPointsManage/manualChangeUserPoints
                 params: operateType : string : 积分操作类型 目前只有 “增加” 一类
                 params: operatePoint : integer : 操作的积分数量
                 params: operateMark : string : 操作的积分备注
                 params: taskName : string : 任务名称 注册 签到 消费
                 params: pointChangType : number : 1--增加  2--消耗
                 params: headers : 请求头
         """
-        taskName = self.get_value_choice(taskName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        operateType = self.get_value_choice(operateType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         operatePoint = self.get_value_choice(operatePoint, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        operateMark = self.get_value_choice(operateMark, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         pointChangType = self.get_value_choice(pointChangType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        operateType = self.get_value_choice(operateType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        operateMark = self.get_value_choice(operateMark, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        taskName = self.get_value_choice(taskName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_userpointsmanage.common_userpointsmanage_manualchangeuserpoints(**_kwargs)
 
         self.assert_common_userpointsmanage_manualchangeuserpoints(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="积分导出前置判断-历史接口")
-    def common_userpointsmanage_beforepointsexport(self, logIds="$None$", endTime="$None$", beginTime="$None$", nickName="$None$", mobile="$None$", _assert=True,  **kwargs):
+    def common_userpointsmanage_beforepointsexport(self, beginTime="$None$", logIds="$None$", mobile="$None$", endTime="$None$", nickName="$None$", _assert=True,  **kwargs):
         """
             url=/common/userPointsManage/beforePointsExport
                 params: nickName :  : 用户昵称
                 params: mobile :  : 用户手机号
                 params: beginTime :  : 注册时间查询范围--开始时间
                 params: endTime :  : 注册时间查询范围--结束时间
                 params: logIds :  : 积分明细Id，用于积分导出，如果传参表示勾选数据导出
                 params: headers : 请求头
         """
+        beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
         logIds = self.get_list_choice(logIds, list_or_dict=None, key="logIds")
+        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
         nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
-        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_common_userpointsmanage.common_userpointsmanage_beforepointsexport(**_kwargs)
 
         self.assert_common_userpointsmanage_beforepointsexport(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_activitymanager.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_activitymanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,55 +2,55 @@
 
 from service.app_a.asserts.content.asserts_content_activitymanager import AssertsContentActivitymanager
 from service.app_a.apis.content import apis_content_activitymanager
 
 
 class FunsContentActivitymanager(AssertsContentActivitymanager):
     @allure.step(title="活动 -修改报名人数(930)-Y")
-    def content_activitymanager_updateperson(self, limitPeople="$None$", activityId="$None$", needLimitPeople="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_activitymanager_updateperson(self, activityId="$None$", needLimitPeople="$None$", limitPeople="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/activityManager/updatePerson
                 params: activityId : string : 活动Id
                 params: needLimitPeople : string : 是否限制 0 不限制 1限制
                 params: limitPeople : number : 限制人数
                 params: headers : 请求头
         """
-        limitPeople = self.get_value_choice(limitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         needLimitPeople = self.get_value_choice(needLimitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        limitPeople = self.get_value_choice(limitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_updateperson(**_kwargs)
 
         self.assert_content_activitymanager_updateperson(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="活动 -修改报名时间-Y")
-    def content_activitymanager_updateenrolltime(self, enrollStartTime="$None$", activityId="$None$", enrollTime="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_activitymanager_updateenrolltime(self, activityId="$None$", enrollStartTime="$None$", enrollTime="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/activityManager/updateEnrollTime
                 params: activityId : string : 活动Id
                 params: enrollStartTime : string : 报名开始时间
                 params: enrollTime : string : 报名结束时间
                 params: headers : 请求头
         """
-        enrollStartTime = self.get_value_choice(enrollStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        enrollStartTime = self.get_value_choice(enrollStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         enrollTime = self.get_value_choice(enrollTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_updateenrolltime(**_kwargs)
 
         self.assert_content_activitymanager_updateenrolltime(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="活动列表查询（930版本）-Y")
-    def content_activitymanager_page(self, status="$None$", title="$None$", activityId="$None$", province="$None$", pushTimeSort="$None$", endTime="$None$", beginTime="$None$", createTimeSort="$None$", target="$None$", city="$None$", activityTimeSort="$None$", _assert=True,  **kwargs):
+    def content_activitymanager_page(self, beginTime="$None$", title="$None$", city="$None$", activityId="$None$", endTime="$None$", status="$None$", province="$None$", createTimeSort="$None$", pushTimeSort="$None$", activityTimeSort="$None$", target="$None$", _assert=True,  **kwargs):
         """
             url=/content/activityManager/page
                 params: activityId :  :
                 params: title :  :
                 params: beginTime :  : 2022-01-18 00:00:00 （一定要带上00:00:00）
                 params: endTime :  : 2022-01-18 23:59:59 （一定要带上23:59:59）
                 params: target :  : 1：全部用户,2：车主用户,3：非车主用户,4:使用人,5：车主&使用人,6：非车主&非使用人
@@ -58,62 +58,62 @@
                 params: province :  : 省（编码 areaId）全国则不需要传值
                 params: city :  : 市（编码areaId）
                 params: createTimeSort :  : 创建时间排序（DESC（倒序））|ASC（正序））
                 params: activityTimeSort :  : 活动时间排序（DESC|ASC）
                 params: pushTimeSort :  : 发布时间排序（DESC|ASC）
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
         title = self.get_list_choice(title, list_or_dict=None, key="title")
+        city = self.get_list_choice(city, list_or_dict=None, key="city")
         activityId = self.get_list_choice(activityId, list_or_dict=None, key="activityId")
-        province = self.get_list_choice(province, list_or_dict=None, key="province")
-        pushTimeSort = self.get_list_choice(pushTimeSort, list_or_dict=None, key="pushTimeSort")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        province = self.get_list_choice(province, list_or_dict=None, key="province")
         createTimeSort = self.get_list_choice(createTimeSort, list_or_dict=None, key="createTimeSort")
-        target = self.get_list_choice(target, list_or_dict=None, key="target")
-        city = self.get_list_choice(city, list_or_dict=None, key="city")
+        pushTimeSort = self.get_list_choice(pushTimeSort, list_or_dict=None, key="pushTimeSort")
         activityTimeSort = self.get_list_choice(activityTimeSort, list_or_dict=None, key="activityTimeSort")
+        target = self.get_list_choice(target, list_or_dict=None, key="target")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_page(**_kwargs)
 
         self.assert_content_activitymanager_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="活动操作停止报名和结束活动-Y")
-    def content_activitymanager_actinfoupdate(self, operationType="$None$", activityId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_activitymanager_actinfoupdate(self, activityId="$None$", operationType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/activityManager/actInfoUpdate
                 params: activityId : text : 活动ID
                 params: operationType : text : 1停止报名 2活动结束
                 params: headers : 请求头
         """
-        operationType = self.get_value_choice(operationType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        operationType = self.get_value_choice(operationType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_actinfoupdate(**_kwargs)
 
         self.assert_content_activitymanager_actinfoupdate(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="设置活动权重(930版本)-Y")
-    def content_activitymanager_setactivitysort(self, sort="$None$", activityId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_activitymanager_setactivitysort(self, activityId="$None$", sort="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/activityManager/setActivitySort
                 params: activityId : string : 活动Id
                 params: sort : number : 权重
                 params: headers : 请求头
         """
-        sort = self.get_value_choice(sort, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        sort = self.get_value_choice(sort, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_setactivitysort(**_kwargs)
 
         self.assert_content_activitymanager_setactivitysort(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -167,15 +167,15 @@
 
         self.assert_content_activitymanager_activityjoinuserexport(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="活动新增-Y")
-    def content_activitymanager_save(self, activityPicUrl="$None$", activityPicURL="$None$", beginTime="$None$", coordinate="$None$", reason="$None$", status="$None$", activityId="$None$", enrollTime="$None$", needLimitPeople="$None$", endTime="$None$", customerGroup="$None$", limitPeople="$None$", province="$None$", county="$None$", authId="$None$", publishType="$None$", needArea="$None$", content="$None$", activityAddr="$None$", title="$None$", enrollStartTime="$None$", publishTime="$None$", agreementId="$None$", city="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_activitymanager_save(self, enrollStartTime="$None$", beginTime="$None$", activityPicURL="$None$", needArea="$None$", limitPeople="$None$", activityPicUrl="$None$", publishTime="$None$", status="$None$", enrollTime="$None$", customerGroup="$None$", publishType="$None$", activityAddr="$None$", county="$None$", title="$None$", reason="$None$", coordinate="$None$", activityId="$None$", authId="$None$", needLimitPeople="$None$", agreementId="$None$", city="$None$", endTime="$None$", province="$None$", content="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/activityManager/save
                 params: activityId : text :
                 params: title : text :
                 params: reason : text :
                 params: activityPicUrl : text :
                 params: beginTime : text :
@@ -196,48 +196,48 @@
                 params: status : text :
                 params: activityAddr : text :
                 params: customerGroup : text :
                 params: activityPicURL : string : 活动封面图
                 params: agreementId : number : 协议ID
                 params: headers : 请求头
         """
-        activityPicUrl = self.get_value_choice(activityPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        activityPicURL = self.get_value_choice(activityPicURL, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        enrollStartTime = self.get_value_choice(enrollStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         beginTime = self.get_value_choice(beginTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        coordinate = self.get_value_choice(coordinate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        reason = self.get_value_choice(reason, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        activityPicURL = self.get_value_choice(activityPicURL, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        needArea = self.get_value_choice(needArea, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        limitPeople = self.get_value_choice(limitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        activityPicUrl = self.get_value_choice(activityPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         enrollTime = self.get_value_choice(enrollTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        needLimitPeople = self.get_value_choice(needLimitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        endTime = self.get_value_choice(endTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         customerGroup = self.get_value_choice(customerGroup, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        limitPeople = self.get_value_choice(limitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        province = self.get_value_choice(province, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        county = self.get_value_choice(county, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        authId = self.get_value_choice(authId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         publishType = self.get_value_choice(publishType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        needArea = self.get_value_choice(needArea, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityAddr = self.get_value_choice(activityAddr, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        county = self.get_value_choice(county, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         title = self.get_value_choice(title, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        enrollStartTime = self.get_value_choice(enrollStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        reason = self.get_value_choice(reason, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        coordinate = self.get_value_choice(coordinate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        authId = self.get_value_choice(authId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        needLimitPeople = self.get_value_choice(needLimitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         agreementId = self.get_value_choice(agreementId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         city = self.get_value_choice(city, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        endTime = self.get_value_choice(endTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        province = self.get_value_choice(province, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_save(**_kwargs)
 
         self.assert_content_activitymanager_save(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="活动编辑（930版本）-Y")
-    def content_activitymanager_update(self, activityPicUrl="$None$", activityPicURL="$None$", beginTime="$None$", coordinate="$None$", reason="$None$", status="$None$", activityId="$None$", enrollTime="$None$", needLimitPeople="$None$", endTime="$None$", customerGroup="$None$", limitPeople="$None$", province="$None$", county="$None$", authId="$None$", publishType="$None$", needArea="$None$", content="$None$", activityAddr="$None$", title="$None$", enrollStartTime="$None$", publishTime="$None$", city="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_activitymanager_update(self, enrollStartTime="$None$", beginTime="$None$", activityPicURL="$None$", needArea="$None$", limitPeople="$None$", activityPicUrl="$None$", publishTime="$None$", status="$None$", enrollTime="$None$", customerGroup="$None$", publishType="$None$", activityAddr="$None$", county="$None$", title="$None$", reason="$None$", coordinate="$None$", activityId="$None$", authId="$None$", needLimitPeople="$None$", city="$None$", endTime="$None$", province="$None$", content="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/activityManager/update
                 params: activityId : text :
                 params: title : text :
                 params: reason : text :
                 params: activityPicUrl : text :
                 params: beginTime : text :
@@ -266,78 +266,78 @@
                 * 10:已结束
                 * 11:已下架
                 * 12:已删除
                 params: activityAddr : string : 活动地址
                 params: customerGroup : string : 参与对象（1：全部用户，2：车主用户，3：非车主用户）
                 params: headers : 请求头
         """
-        activityPicUrl = self.get_value_choice(activityPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        activityPicURL = self.get_value_choice(activityPicURL, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        enrollStartTime = self.get_value_choice(enrollStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         beginTime = self.get_value_choice(beginTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        coordinate = self.get_value_choice(coordinate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        reason = self.get_value_choice(reason, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        activityPicURL = self.get_value_choice(activityPicURL, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        needArea = self.get_value_choice(needArea, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        limitPeople = self.get_value_choice(limitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        activityPicUrl = self.get_value_choice(activityPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         enrollTime = self.get_value_choice(enrollTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        needLimitPeople = self.get_value_choice(needLimitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        endTime = self.get_value_choice(endTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         customerGroup = self.get_value_choice(customerGroup, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        limitPeople = self.get_value_choice(limitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        province = self.get_value_choice(province, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        county = self.get_value_choice(county, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        authId = self.get_value_choice(authId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         publishType = self.get_value_choice(publishType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        needArea = self.get_value_choice(needArea, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityAddr = self.get_value_choice(activityAddr, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        county = self.get_value_choice(county, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         title = self.get_value_choice(title, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        enrollStartTime = self.get_value_choice(enrollStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        reason = self.get_value_choice(reason, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        coordinate = self.get_value_choice(coordinate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        authId = self.get_value_choice(authId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        needLimitPeople = self.get_value_choice(needLimitPeople, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         city = self.get_value_choice(city, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        endTime = self.get_value_choice(endTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        province = self.get_value_choice(province, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_update(**_kwargs)
 
         self.assert_content_activitymanager_update(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="活动发布状态修改(930)-Y")
-    def content_activitymanager_publishupdate(self, status="$None$", publishStatus="$None$", activityId="$None$", activityIds="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_activitymanager_publishupdate(self, activityId="$None$", publishStatus="$None$", status="$None$", activityIds="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/activityManager/publishUpdate
                 params: activityIds : text : 单个记录修改传["xxxxx"]
                 params: publishStatus : text :
                 params: activityId : string : 活动Id
                 params: status : number : //状态: 1.新建 2.待审核 3.审核通过 4.待发布 5.已发布 6.审核不过 7.已撤回 8.已归档 9.停止报名 10.已结束 11.已下架；查询时候传的状态：12.已删除
                 params: headers : 请求头
         """
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        publishStatus = self.get_value_choice(publishStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityId = self.get_value_choice(activityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishStatus = self.get_value_choice(publishStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityIds = self.get_value_choice(activityIds, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_publishupdate(**_kwargs)
 
         self.assert_content_activitymanager_publishupdate(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="活动审核状态修改-Y")
-    def content_activitymanager_statusupdate(self, activityIds="$None$", checkStatus="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_activitymanager_statusupdate(self, checkStatus="$None$", activityIds="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/activityManager/statusUpdate
                 params: checkStatus : text :
                 params: activityIds : array : 活动IDs
                 type : string : None
                 params: headers : 请求头
         """
-        activityIds = self.get_value_choice(activityIds, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         checkStatus = self.get_value_choice(checkStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        activityIds = self.get_value_choice(activityIds, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_statusupdate(**_kwargs)
 
         self.assert_content_activitymanager_statusupdate(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -357,15 +357,15 @@
         self.res = apis_content_activitymanager.content_activitymanager_enrollupdate(**_kwargs)
 
         self.assert_content_activitymanager_enrollupdate(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="活动数据导出-Y")
-    def content_activitymanager_activityexport(self, status="$None$", title="$None$", activityId="$None$", province="$None$", pushTimeSort="$None$", endTime="$None$", beginTime="$None$", createTimeSort="$None$", target="$None$", city="$None$", activityTimeSort="$None$", _assert=True,  **kwargs):
+    def content_activitymanager_activityexport(self, beginTime="$None$", title="$None$", city="$None$", activityId="$None$", endTime="$None$", status="$None$", province="$None$", createTimeSort="$None$", pushTimeSort="$None$", activityTimeSort="$None$", target="$None$", _assert=True,  **kwargs):
         """
             url=/content/activityManager/activityExport
                 params: activityId :  :
                 params: title :  :
                 params: beginTime :  : 2022-01-18 00:00:00 （一定要带上00:00:00）
                 params: endTime :  : 2022-01-18 23:59:59 （一定要带上23:59:59）
                 params: target :  : 1：全部用户,2：车主用户,3：非车主用户,4:使用人,5：车主&使用人,6：非车主&非使用人
@@ -373,25 +373,25 @@
                 params: province :  : 省（编码 areaId）全国则不需要传值
                 params: city :  : 市（编码areaId）
                 params: createTimeSort :  : 创建时间排序（DESC（倒序））|ASC（正序））
                 params: activityTimeSort :  : 活动时间排序（DESC|ASC）
                 params: pushTimeSort :  : 发布时间排序（DESC|ASC）
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
         title = self.get_list_choice(title, list_or_dict=None, key="title")
+        city = self.get_list_choice(city, list_or_dict=None, key="city")
         activityId = self.get_list_choice(activityId, list_or_dict=None, key="activityId")
-        province = self.get_list_choice(province, list_or_dict=None, key="province")
-        pushTimeSort = self.get_list_choice(pushTimeSort, list_or_dict=None, key="pushTimeSort")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        province = self.get_list_choice(province, list_or_dict=None, key="province")
         createTimeSort = self.get_list_choice(createTimeSort, list_or_dict=None, key="createTimeSort")
-        target = self.get_list_choice(target, list_or_dict=None, key="target")
-        city = self.get_list_choice(city, list_or_dict=None, key="city")
+        pushTimeSort = self.get_list_choice(pushTimeSort, list_or_dict=None, key="pushTimeSort")
         activityTimeSort = self.get_list_choice(activityTimeSort, list_or_dict=None, key="activityTimeSort")
+        target = self.get_list_choice(target, list_or_dict=None, key="target")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_activitymanager.content_activitymanager_activityexport(**_kwargs)
 
         self.assert_content_activitymanager_activityexport(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_adv.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_adv.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.content.asserts_content_adv import AssertsContentAdv
 from service.app_a.apis.content import apis_content_adv
 
 
 class FunsContentAdv(AssertsContentAdv):
     @allure.step(title="点位内容-保存运营端配置(更新、新增)（930）-Y")
-    def content_adv_save(self, advLinkUrl="$None$", version="$None$", pictureList="$None$", advPlaceId="$None$", advId="$None$", bindingFlag="$None$", advSerial="$None$", jumpType="$None$", advPicUrl="$None$", jumpContent="$None$", advText="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_adv_save(self, advPlaceId="$None$", bindingFlag="$None$", advSerial="$None$", advId="$None$", jumpContent="$None$", advPicUrl="$None$", advLinkUrl="$None$", jumpType="$None$", pictureList="$None$", version="$None$", advText="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/adv/save
                 params: advPlaceId : number : 左侧列表选中ID
                 params: advPicUrl : string : 图片地址
                 params: advText : string : 文字描述
                 params: advSerial : string : 排序
                 params: jumpType : number : 跳转类型
@@ -19,24 +19,24 @@
                 params: version : string : 绑定的车系（60s,80v）
                 params: advLinkUrl : string : 爱车海报填写地址/url跳转地址
                 params: bindingFlag : number : 车辆绑定标识 1绑定 0未绑定
                 params: pictureList : array : 当跳转类型为16：图片新增字段
                 type : string : None
                 params: headers : 请求头
         """
-        advLinkUrl = self.get_value_choice(advLinkUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        version = self.get_value_choice(version, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        pictureList = self.get_value_choice(pictureList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         advPlaceId = self.get_value_choice(advPlaceId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        advId = self.get_value_choice(advId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         bindingFlag = self.get_value_choice(bindingFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         advSerial = self.get_value_choice(advSerial, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        jumpType = self.get_value_choice(jumpType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        advPicUrl = self.get_value_choice(advPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        advId = self.get_value_choice(advId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         jumpContent = self.get_value_choice(jumpContent, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        advPicUrl = self.get_value_choice(advPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        advLinkUrl = self.get_value_choice(advLinkUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        jumpType = self.get_value_choice(jumpType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        pictureList = self.get_value_choice(pictureList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        version = self.get_value_choice(version, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         advText = self.get_value_choice(advText, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_adv.content_adv_save(**_kwargs)
 
         self.assert_content_adv_save(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_advplace.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_advplace.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from service.app_a.asserts.content.asserts_content_advplace import AssertsContentAdvplace
 from service.app_a.apis.content import apis_content_advplace
 
 
 class FunsContentAdvplace(AssertsContentAdvplace):
     @allure.step(title="点位-更新大点位内容")
-    def content_advplace_updatename(self, advPlaceId="$None$", startFlag="$None$", advPlaceName="$None$", playTime="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_advplace_updatename(self, advPlaceName="$None$", advPlaceId="$None$", startFlag="$None$", playTime="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/advplace/updateName
                 params: advPlaceId : text :
                 params: advPlaceName : text :
                 params: startFlag : text : 广告页广告位必传
                 params: playTime : text : 广告页广告位必传
                 params: headers : 请求头
         """
+        advPlaceName = self.get_value_choice(advPlaceName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         advPlaceId = self.get_value_choice(advPlaceId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         startFlag = self.get_value_choice(startFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        advPlaceName = self.get_value_choice(advPlaceName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         playTime = self.get_value_choice(playTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_advplace.content_advplace_updatename(**_kwargs)
 
         self.assert_content_advplace_updatename(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_agreement.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_agreement.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,51 +92,51 @@
 
         self.assert_content_agreement_list(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="协议-新增协议-Y")
-    def content_agreement_save(self, content="$None$", version="$None$", code="$None$", name="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_agreement_save(self, name="$None$", content="$None$", code="$None$", version="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/agreement/save
                 params: name : string : 协议名
                 params: content : string : 内容
                 params: version : number : 版本号
                 params: code : string : 协议编码
                 params: headers : 请求头
         """
+        name = self.get_value_choice(name, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        version = self.get_value_choice(version, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         code = self.get_value_choice(code, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        name = self.get_value_choice(name, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        version = self.get_value_choice(version, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_agreement.content_agreement_save(**_kwargs)
 
         self.assert_content_agreement_save(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="协议-更新协议-Y")
-    def content_agreement_update(self, name="$None$", content="$None$", agreementId="$None$", code="$None$", version="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_agreement_update(self, code="$None$", name="$None$", agreementId="$None$", version="$None$", content="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/agreement/update
                 params: name : string : 协议名
                 params: content : string : 内容
                 params: version : number : 版本号
                 params: agreementId : string : 协议id
                 params: code : string : 协议编码
                 params: headers : 请求头
         """
+        code = self.get_value_choice(code, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         name = self.get_value_choice(name, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         agreementId = self.get_value_choice(agreementId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        code = self.get_value_choice(code, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         version = self.get_value_choice(version, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_agreement.content_agreement_update(**_kwargs)
 
         self.assert_content_agreement_update(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_campmanager.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_campmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from service.app_a.asserts.content.asserts_content_campmanager import AssertsContentCampmanager
 from service.app_a.apis.content import apis_content_campmanager
 
 
 class FunsContentCampmanager(AssertsContentCampmanager):
     @allure.step(title="营地服务列表 - 分页查询")
-    def content_campmanager_page(self, status="$None$", sortord="$None$", sortBody="$None$", id="$None$", createBy="$None$", name="$None$", _assert=True,  **kwargs):
+    def content_campmanager_page(self, createBy="$None$", name="$None$", sortBody="$None$", status="$None$", sortord="$None$", id="$None$", _assert=True,  **kwargs):
         """
             url=/content/campManager/page
                 params: id :  :
                 params: name :  :
                 params: status :  :
                 params: createBy :  :
                 params: sortBody :  :
                 params: sortord :  : ASC/DESC/asc/desc
                 params: headers : 请求头
         """
+        createBy = self.get_list_choice(createBy, list_or_dict=None, key="createBy")
+        name = self.get_list_choice(name, list_or_dict=None, key="name")
+        sortBody = self.get_list_choice(sortBody, list_or_dict=None, key="sortBody")
         status = self.get_list_choice(status, list_or_dict=None, key="status")
         sortord = self.get_list_choice(sortord, list_or_dict=None, key="sortord")
-        sortBody = self.get_list_choice(sortBody, list_or_dict=None, key="sortBody")
         id = self.get_list_choice(id, list_or_dict=None, key="id")
-        createBy = self.get_list_choice(createBy, list_or_dict=None, key="createBy")
-        name = self.get_list_choice(name, list_or_dict=None, key="name")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_campmanager.content_campmanager_page(**_kwargs)
 
         self.assert_content_campmanager_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
@@ -62,15 +62,15 @@
 
         self.assert_content_campmanager_insertcampid(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="新增营地")
-    def content_campmanager_insert(self, province="$None$", county="$None$", discountExpEndTime="$None$", id="$None$", discountExpBeginTime="$None$", campTradeTime="$None$", url="$None$", ownerDiscount="$None$", content="$None$", city="$None$", address="$None$", name="$None$", campDetail="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_campmanager_insert(self, campDetail="$None$", county="$None$", ownerDiscount="$None$", name="$None$", discountExpBeginTime="$None$", address="$None$", url="$None$", city="$None$", province="$None$", campTradeTime="$None$", content="$None$", id="$None$", discountExpEndTime="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/campManager/insert
                 params: id : text : 营地服务ID
                 params: name : text : 营地名称
                 params: content : text : 营地简介
                 params: url : text : 营地图片
                 params: campDetail : text : 营地详情
@@ -80,27 +80,27 @@
                 params: discountExpEndTime : text : 车主优惠有效期 - 结束时间
                 params: province : text : 省
                 params: city : text : 市
                 params: county : text : 区/县
                 params: address : text : 详细地址
                 params: headers : 请求头
         """
-        province = self.get_value_choice(province, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        campDetail = self.get_value_choice(campDetail, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         county = self.get_value_choice(county, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        discountExpEndTime = self.get_value_choice(discountExpEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        id = self.get_value_choice(id, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        ownerDiscount = self.get_value_choice(ownerDiscount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        name = self.get_value_choice(name, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         discountExpBeginTime = self.get_value_choice(discountExpBeginTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        campTradeTime = self.get_value_choice(campTradeTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        address = self.get_value_choice(address, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         url = self.get_value_choice(url, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        ownerDiscount = self.get_value_choice(ownerDiscount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         city = self.get_value_choice(city, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        address = self.get_value_choice(address, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        name = self.get_value_choice(name, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        campDetail = self.get_value_choice(campDetail, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        province = self.get_value_choice(province, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        campTradeTime = self.get_value_choice(campTradeTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        id = self.get_value_choice(id, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        discountExpEndTime = self.get_value_choice(discountExpEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_campmanager.content_campmanager_insert(**_kwargs)
 
         self.assert_content_campmanager_insert(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -119,29 +119,29 @@
 
         self.assert_content_campmanager_detail_(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="编辑营地")
-    def content_campmanager_update(self, discountExpEndTime="$None$", ownerDiscount="$None$", discountExpBeginTime="$None$", phone="$None$", areaCode="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_campmanager_update(self, ownerDiscount="$None$", discountExpBeginTime="$None$", phone="$None$", areaCode="$None$", discountExpEndTime="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/campManager/update
                 params: ownerDiscount : text : 车主优惠
                 params: discountExpBeginTime : text : 车主优惠有效期 - 开始时间
                 params: discountExpEndTime : text : 车主优惠有效期 - 结束时间
                 params: areaCode : text : 区号
                 params: phone : text : 手机号
                 params: headers : 请求头
         """
-        discountExpEndTime = self.get_value_choice(discountExpEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         ownerDiscount = self.get_value_choice(ownerDiscount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         discountExpBeginTime = self.get_value_choice(discountExpBeginTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         phone = self.get_value_choice(phone, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         areaCode = self.get_value_choice(areaCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        discountExpEndTime = self.get_value_choice(discountExpEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_campmanager.content_campmanager_update(**_kwargs)
 
         self.assert_content_campmanager_update(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_comment.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,133 +2,133 @@
 
 from service.app_a.asserts.content.asserts_content_comment import AssertsContentComment
 from service.app_a.apis.content import apis_content_comment
 
 
 class FunsContentComment(AssertsContentComment):
     @allure.step(title="评论-状态扭转（通用）-Y")
-    def content_comment_updatestatus(self, fromStatus="$None$", commentType="$None$", toStatus="$None$", commentId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_comment_updatestatus(self, commentId="$None$", fromStatus="$None$", toStatus="$None$", commentType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/comment/updateStatus
                 params: commentId :  : 评论主键
                 params: commentType :  : 评论类型1：文章评论2：动态评论
                 params: fromStatus :  : 当前状态
                 params: toStatus :  : 扭转状态
                 params: headers : 请求头
         """
+        commentId = self.get_value_choice(commentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         fromStatus = self.get_value_choice(fromStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        commentType = self.get_value_choice(commentType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         toStatus = self.get_value_choice(toStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        commentId = self.get_value_choice(commentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        commentType = self.get_value_choice(commentType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_comment.content_comment_updatestatus(**_kwargs)
 
         self.assert_content_comment_updatestatus(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="评论-评论导出-Y")
-    def content_comment_download(self, status="$None$", contentCommentIds="$None$", keyWord="$None$", startTime="$None$", endTime="$None$", nickName="$None$", EssayCommentIds="$None$", mobile="$None$", downloadType="$None$", _assert=True,  **kwargs):
+    def content_comment_download(self, contentCommentIds="$None$", EssayCommentIds="$None$", keyWord="$None$", mobile="$None$", downloadType="$None$", endTime="$None$", startTime="$None$", status="$None$", nickName="$None$", _assert=True,  **kwargs):
         """
             url=/content/comment/downLoad
                 params: mobile :  : 评论用户手机号
                 params: nickName :  : 评论昵称
                 params: keyWord :  : 搜索关键字
                 params: startTime :  : 搜索起始时间
                 params: endTime :  : 搜索结束时间
                 params: status :  : 状态0.待审核 1.已审核 2.审核未通过3：已发布4：已屏蔽
                 params: downloadType :  : 1：根据搜索条件导出2：多选导出
                 params: EssayCommentIds :  : 文章评论主键，用英文,隔开
                 params: contentCommentIds :  : 动态评论主键，用英文,隔开
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
         contentCommentIds = self.get_list_choice(contentCommentIds, list_or_dict=None, key="contentCommentIds")
-        keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
-        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
         EssayCommentIds = self.get_list_choice(EssayCommentIds, list_or_dict=None, key="EssayCommentIds")
+        keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
         downloadType = self.get_list_choice(downloadType, list_or_dict=None, key="downloadType")
+        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_comment.content_comment_download(**_kwargs)
 
         self.assert_content_comment_download(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="评论-评论置顶（通用）-Y")
-    def content_comment_commenttop(self, commentType="$None$", topFlag="$None$", commentId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_comment_commenttop(self, commentId="$None$", topFlag="$None$", commentType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/comment/commentTop
                 params: commentId : string : 评论主键
                 params: commentType : number : 评论类型1：文章评论2：动态评论
                 params: topFlag : number : 1：置顶0：取消置顶
                 params: headers : 请求头
         """
-        commentType = self.get_value_choice(commentType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        topFlag = self.get_value_choice(topFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         commentId = self.get_value_choice(commentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        topFlag = self.get_value_choice(topFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        commentType = self.get_value_choice(commentType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_comment.content_comment_commenttop(**_kwargs)
 
         self.assert_content_comment_commenttop(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="后台管理-评论管理列表1030-Y")
-    def content_comment_list(self, keyWord="$None$", startTime="$None$", endTime="$None$", nickName="$None$", checkedStatus="$None$", mobile="$None$", essayId="$None$", current=1, commentType="$None$", size=10, _assert=True,  **kwargs):
+    def content_comment_list(self, current=1, essayId="$None$", keyWord="$None$", mobile="$None$", commentType="$None$", endTime="$None$", startTime="$None$", checkedStatus="$None$", nickName="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/content/comment/list
                 params: nickName :  : 用户昵称 String
                 params: keyWord :  : 搜索内容关键字  String
                 params: startTime :  : 搜索开始时间 yyyy-MM-dd HH:mm:ss
                 params: endTime :  : 搜索结束时间 yyyy-MM-dd HH:mm:ss
                 params: size :  : 每页数量数
                 params: current :  : 当前页
                 params: commentType :  : 评论类型1：文章评论 2：动态 Integer
                 params: checkedStatus :  : 审核状态 0待审核 1.已上架 2.审核未通过3：已发布 5已删除 Integer
                 params: mobile :  : 电话 string
                 params: essayId :  : 文章(资讯)主键 string
                 params: headers : 请求头
         """
+        essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
         keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
-        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
-        checkedStatus = self.get_list_choice(checkedStatus, list_or_dict=None, key="checkedStatus")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
         commentType = self.get_list_choice(commentType, list_or_dict=None, key="commentType")
+        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        checkedStatus = self.get_list_choice(checkedStatus, list_or_dict=None, key="checkedStatus")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_comment.content_comment_list(**_kwargs)
 
         self.assert_content_comment_list(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="评论-屏蔽评论-Y")
-    def content_comment_delete(self, commentType="$None$", toStatus="$None$", commentId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_comment_delete(self, commentId="$None$", toStatus="$None$", commentType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/comment/delete
                 params: commentId : string : 评论主键
                 params: commentType : number : 1：文章评论2：动态评论
                 params: toStatus : string :
                 params: headers : 请求头
         """
-        commentType = self.get_value_choice(commentType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        toStatus = self.get_value_choice(toStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         commentId = self.get_value_choice(commentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        toStatus = self.get_value_choice(toStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        commentType = self.get_value_choice(commentType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_comment.content_comment_delete(**_kwargs)
 
         self.assert_content_comment_delete(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_commonquestion.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_commonquestion.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_contentmanager.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_contentmanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_essay.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_essay.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.res = apis_content_essay.content_essay_delete_(**_kwargs)
 
         self.assert_content_essay_delete_(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="专题-后台App文章关键词搜索-Y")
-    def content_essay_searchbykey(self, Key="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def content_essay_searchbykey(self, size=10, Key="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/content/essay/searchByKey
                 params: Key :  : 关键词
                 params: size :  : 条数
                 params: current :  : 当前页
                 params: headers : 请求头
         """
@@ -37,15 +37,15 @@
 
         self.assert_content_essay_searchbykey(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="后台管理-内容审核列表1030-Y")
-    def content_essay_checklist(self, status="$None$", StatusSortType="$None$", keyWord="$None$", startTime="$None$", endTime="$None$", CreateTimeSortType="$None$", subjectId="$None$", author="$None$", essayId="$None$", PublishTimeSortType="$None$", current=1, recommend="$None$", size=10, _assert=True,  **kwargs):
+    def content_essay_checklist(self, author="$None$", subjectId="$None$", StatusSortType="$None$", essayId="$None$", current=1, PublishTimeSortType="$None$", keyWord="$None$", endTime="$None$", startTime="$None$", status="$None$", CreateTimeSortType="$None$", recommend="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/content/essay/checkList
                 params: essayId :  : 文章主键
                 params: keyWord :  : 文章搜索关键字
                 params: author :  : 作者
                 params: startTime :  : 搜索开始时间
                 params: endTime :  : 搜索结束时间
@@ -55,36 +55,36 @@
                 params: current :  : 当前页数
                 params: recommend :  : 是否推荐 1：推荐页0：非推荐页
                 params: PublishTimeSortType :  : 发布时间排序方式 默认倒序，正序  ASC 倒序 DESC
                 params: CreateTimeSortType :  : 创建时间排序方式 默认倒序，  正序  ASC 倒序 DESC
                 params: StatusSortType :  : 状态排序方式 默认倒序，  正序  ASC 倒序 DESC
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        author = self.get_list_choice(author, list_or_dict=None, key="author")
+        subjectId = self.get_list_choice(subjectId, list_or_dict=None, key="subjectId")
         StatusSortType = self.get_list_choice(StatusSortType, list_or_dict=None, key="StatusSortType")
+        essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
+        PublishTimeSortType = self.get_list_choice(PublishTimeSortType, list_or_dict=None, key="PublishTimeSortType")
         keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
         CreateTimeSortType = self.get_list_choice(CreateTimeSortType, list_or_dict=None, key="CreateTimeSortType")
-        subjectId = self.get_list_choice(subjectId, list_or_dict=None, key="subjectId")
-        author = self.get_list_choice(author, list_or_dict=None, key="author")
-        essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
-        PublishTimeSortType = self.get_list_choice(PublishTimeSortType, list_or_dict=None, key="PublishTimeSortType")
         recommend = self.get_list_choice(recommend, list_or_dict=None, key="recommend")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_essay.content_essay_checklist(**_kwargs)
 
         self.assert_content_essay_checklist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="后台管理-内容管理列表1030-Y")
-    def content_essay_list(self, status="$None$", StatusSortType="$None$", keyWord="$None$", startTime="$None$", endTime="$None$", CreateTimeSortType="$None$", subjectId="$None$", author="$None$", essayId="$None$", PublishTimeSortType="$None$", current=1, recommend="$None$", size=10, _assert=True,  **kwargs):
+    def content_essay_list(self, author="$None$", subjectId="$None$", StatusSortType="$None$", essayId="$None$", current=1, PublishTimeSortType="$None$", keyWord="$None$", endTime="$None$", startTime="$None$", status="$None$", CreateTimeSortType="$None$", recommend="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/content/essay/list
                 params: essayId :  : 文章主键
                 params: keyWord :  : 文章搜索关键字
                 params: author :  : 作者
                 params: startTime :  : 搜索开始时间
                 params: endTime :  : 搜索结束时间
@@ -94,36 +94,36 @@
                 params: current :  : 当前页数
                 params: recommend :  : 是否推荐 1：推荐页0：非推荐页
                 params: PublishTimeSortType :  : 发布时间排序方式 默认倒序，正序  ASC 倒序 DESC
                 params: CreateTimeSortType :  : 创建时间排序方式 默认倒序，  正序  ASC 倒序 DESC
                 params: StatusSortType :  : 状态排序方式 默认倒序，  正序  ASC 倒序 DESC
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        author = self.get_list_choice(author, list_or_dict=None, key="author")
+        subjectId = self.get_list_choice(subjectId, list_or_dict=None, key="subjectId")
         StatusSortType = self.get_list_choice(StatusSortType, list_or_dict=None, key="StatusSortType")
+        essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
+        PublishTimeSortType = self.get_list_choice(PublishTimeSortType, list_or_dict=None, key="PublishTimeSortType")
         keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
         CreateTimeSortType = self.get_list_choice(CreateTimeSortType, list_or_dict=None, key="CreateTimeSortType")
-        subjectId = self.get_list_choice(subjectId, list_or_dict=None, key="subjectId")
-        author = self.get_list_choice(author, list_or_dict=None, key="author")
-        essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
-        PublishTimeSortType = self.get_list_choice(PublishTimeSortType, list_or_dict=None, key="PublishTimeSortType")
         recommend = self.get_list_choice(recommend, list_or_dict=None, key="recommend")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_essay.content_essay_list(**_kwargs)
 
         self.assert_content_essay_list(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="后台管理-新建&修改内容1030-Y")
-    def content_essay_add(self, status="$None$", essPicUrl="$None$", title="$None$", videoUrl="$None$", publishTime="$None$", publishType="$None$", subjectId="$None$", author="$None$", essayId="$None$", recommend="$None$", content="$None$", essayType="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_essay_add(self, videoUrl="$None$", author="$None$", title="$None$", subjectId="$None$", essayId="$None$", publishTime="$None$", essPicUrl="$None$", status="$None$", content="$None$", publishType="$None$", recommend="$None$", essayType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/essay/add
                 params: essayId : string : 文章主键
                 params: title : string : 标题
                 params: author : string : 作者
                 params: publishType : number : 发布类型1：立即发布2：定时发布
                 params: publishTime : string : 发布时间
@@ -133,25 +133,25 @@
                 params: subjectId : array : 专题主键
                 type : string : None
                 params: recommend : number : 是否推荐 1：推荐页0：非推荐页
                 params: essPicUrl : string : 封面
                 params: videoUrl : string : 视频路径
                 params: headers : 请求头
         """
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        essPicUrl = self.get_value_choice(essPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        title = self.get_value_choice(title, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         videoUrl = self.get_value_choice(videoUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        publishType = self.get_value_choice(publishType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        subjectId = self.get_value_choice(subjectId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         author = self.get_value_choice(author, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        title = self.get_value_choice(title, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        subjectId = self.get_value_choice(subjectId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         essayId = self.get_value_choice(essayId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        recommend = self.get_value_choice(recommend, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        essPicUrl = self.get_value_choice(essPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishType = self.get_value_choice(publishType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        recommend = self.get_value_choice(recommend, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         essayType = self.get_value_choice(essayType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_essay.content_essay_add(**_kwargs)
 
         self.assert_content_essay_add(_assert, **_kwargs)
         self.set_value(_kwargs)
@@ -198,35 +198,35 @@
         self.res = apis_content_essay.content_essay_updatestatus(**_kwargs)
 
         self.assert_content_essay_updatestatus(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="后台管理-评论信息1030-Y")
-    def content_essay_getcommentlist(self, parentId="$None$", keyWord="$None$", startTime="$None$", endTime="$None$", essayId="$None$", commentId="$None$", current=1, checkedStatus="$None$", size=10, _assert=True,  **kwargs):
+    def content_essay_getcommentlist(self, essayId="$None$", commentId="$None$", parentId="$None$", current=1, keyWord="$None$", endTime="$None$", checkedStatus="$None$", startTime="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/content/essay/getCommentList
                 params: essayId :  : 文章主键
                 params: keyWord :  : 关键词
                 params: checkedStatus :  : 审核状态 审核状态 0待审核 1.已上架 2.审核未通过3：已下架 5已删除
                 params: startTime :  : 开始时间
                 params: endTime :  : 结束时间
                 params: commentId :  : 评论id
                 params: parentId :  : 父级id
                 params: size :  : 每页数量
                 params: current :  : 当前页
                 params: headers : 请求头
         """
+        essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
+        commentId = self.get_list_choice(commentId, list_or_dict=None, key="commentId")
         parentId = self.get_list_choice(parentId, list_or_dict=None, key="parentId")
         keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
-        commentId = self.get_list_choice(commentId, list_or_dict=None, key="commentId")
         checkedStatus = self.get_list_choice(checkedStatus, list_or_dict=None, key="checkedStatus")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_essay.content_essay_getcommentlist(**_kwargs)
 
         self.assert_content_essay_getcommentlist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_essaycomment.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_essaycomment.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_essayweb.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_essayweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 
 from service.app_a.asserts.content.asserts_content_essayweb import AssertsContentEssayweb
 from service.app_a.apis.content import apis_content_essayweb
 
 
 class FunsContentEssayweb(AssertsContentEssayweb):
     @allure.step(title="专题-后台官网专题新建文章-Y")
-    def content_essayweb_add(self, essPicUrl="$None$", status="$None$", title="$None$", publishTime="$None$", publishType="$None$", publishChannel="$None$", author="$None$", essayId="$None$", content="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_essayweb_add(self, publishChannel="$None$", author="$None$", title="$None$", essayId="$None$", publishTime="$None$", essPicUrl="$None$", status="$None$", content="$None$", publishType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/essayweb/add
                 params: essayId : string : 文章主键
                 params: title : string : 文章标题
                 params: author : string : 作者
                 params: publishType : string : 发布类型1：立即发布2：定时发布
                 params: publishTime : string : 定时发布时间
                 params: essPicUrl : string : 文章封面
                 params: publishChannel : string : 发布渠道
                 params: content : string : 文章正文富文本
                 params: status : string : 保存时传1，提交审核时传2
                 params: headers : 请求头
         """
-        essPicUrl = self.get_value_choice(essPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        title = self.get_value_choice(title, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        publishType = self.get_value_choice(publishType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         publishChannel = self.get_value_choice(publishChannel, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         author = self.get_value_choice(author, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        title = self.get_value_choice(title, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         essayId = self.get_value_choice(essayId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        essPicUrl = self.get_value_choice(essPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishType = self.get_value_choice(publishType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_essayweb.content_essayweb_add(**_kwargs)
 
         self.assert_content_essayweb_add(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="专题-后台官网文章关键词搜索-Y")
-    def content_essayweb_searchbykey(self, key="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def content_essayweb_searchbykey(self, size=10, key="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/content/essayweb/searchByKey
                 params: current :  : 当前页
                 params: size :  : 每页条数
                 params: key :  : 关键词
                 params: headers : 请求头
         """
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_hotcity.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_hotcity.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_hotsearch.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_hotsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 
 from service.app_a.asserts.content.asserts_content_hotsearch import AssertsContentHotsearch
 from service.app_a.apis.content import apis_content_hotsearch
 
 
 class FunsContentHotsearch(AssertsContentHotsearch):
     @allure.step(title="热门搜索-修改权重-Y")
-    def content_hotsearch_rank(self, kId="$None$", rank="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_hotsearch_rank(self, rank="$None$", kId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/hotSearch/rank
                 params: kId : string : 主键id
                 params: rank : string : 权重
                 params: headers : 请求头
         """
-        kId = self.get_value_choice(kId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         rank = self.get_value_choice(rank, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        kId = self.get_value_choice(kId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_hotsearch.content_hotsearch_rank(**_kwargs)
 
         self.assert_content_hotsearch_rank(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="热门搜索-列表-Y")
-    def content_hotsearch_list(self, kId="$None$", rank="$None$", _assert=True,  **kwargs):
+    def content_hotsearch_list(self, rank="$None$", kId="$None$", _assert=True,  **kwargs):
         """
             url=/content/hotSearch/list
                 params: kId : string : 主键id
                 params: rank : string : 权重
                 params: headers : 请求头
         """
-        kId = self.get_list_choice(kId, list_or_dict=None, key="kId")
         rank = self.get_list_choice(rank, list_or_dict=None, key="rank")
+        kId = self.get_list_choice(kId, list_or_dict=None, key="kId")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_hotsearch.content_hotsearch_list(**_kwargs)
 
         self.assert_content_hotsearch_list(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_material.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_material.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.res = apis_content_material.content_material_updategroup(**_kwargs)
 
         self.assert_content_material_updategroup(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="素材-根据素材组获取素材列表")
-    def content_material_getmateriallist(self, groupId="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def content_material_getmateriallist(self, size=10, groupId="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/content/material/getMaterialList
                 params: groupId :  : 分组主键
                 params: size :  : 每页数据数
                 params: current :  : 当前页
                 params: headers : 请求头
         """
@@ -85,23 +85,23 @@
         self.res = apis_content_material.content_material_addgroup(**_kwargs)
 
         self.assert_content_material_addgroup(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="素材-素材上传")
-    def content_material_addmaterial(self, groupId="$None$", file="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_material_addmaterial(self, file="$None$", groupId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/material/addMaterial
                 params: file : file : 上传文件
                 params: groupId : text : 所属分组主键
                 params: headers : 请求头
         """
-        groupId = self.get_value_choice(groupId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         file = self.get_value_choice(file, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        groupId = self.get_value_choice(groupId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_material.content_material_addmaterial(**_kwargs)
 
         self.assert_content_material_addmaterial(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_messagemanager.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_messagemanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 
 from service.app_a.asserts.content.asserts_content_messagemanager import AssertsContentMessagemanager
 from service.app_a.apis.content import apis_content_messagemanager
 
 
 class FunsContentMessagemanager(AssertsContentMessagemanager):
     @allure.step(title="消息列表查询接口-Y")
-    def content_messagemanager_page(self, status="$None$", cEndTime="$None$", userId="$None$", authId="$None$", endTime="$None$", beginTime="$None$", pStartTime="$None$", messageId="$None$", cStartTime="$None$", pEndTime="$None$", content="$None$", _assert=True,  **kwargs):
+    def content_messagemanager_page(self, beginTime="$None$", cStartTime="$None$", pEndTime="$None$", authId="$None$", endTime="$None$", messageId="$None$", status="$None$", pStartTime="$None$", content="$None$", userId="$None$", cEndTime="$None$", _assert=True,  **kwargs):
         """
             url=/content/messageManager/page
                 params: messageId :  :
                 params: content :  :
                 params: beginTime :  : 前端日期后面必须要追加 00:00:00
                 params: endTime :  : 前端日期后面必须要追加 23:59:59
                 params: authId :  :
                 params: status :  : -1.结束 0.待审核 1.审核通过 2.审核未通过 3.草稿  4.未发布 5.已发布 6.已撤销 7.已归档
                 params: pStartTime :  :
                 params: pEndTime :  :
                 params: cStartTime :  :
                 params: cEndTime :  :
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
-        cEndTime = self.get_list_choice(cEndTime, list_or_dict=None, key="cEndTime")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        authId = self.get_list_choice(authId, list_or_dict=None, key="authId")
-        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
         beginTime = self.get_list_choice(beginTime, list_or_dict=None, key="beginTime")
-        pStartTime = self.get_list_choice(pStartTime, list_or_dict=None, key="pStartTime")
-        messageId = self.get_list_choice(messageId, list_or_dict=None, key="messageId")
         cStartTime = self.get_list_choice(cStartTime, list_or_dict=None, key="cStartTime")
         pEndTime = self.get_list_choice(pEndTime, list_or_dict=None, key="pEndTime")
+        authId = self.get_list_choice(authId, list_or_dict=None, key="authId")
+        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        messageId = self.get_list_choice(messageId, list_or_dict=None, key="messageId")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        pStartTime = self.get_list_choice(pStartTime, list_or_dict=None, key="pStartTime")
         content = self.get_list_choice(content, list_or_dict=None, key="content")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        cEndTime = self.get_list_choice(cEndTime, list_or_dict=None, key="cEndTime")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_messagemanager.content_messagemanager_page(**_kwargs)
 
         self.assert_content_messagemanager_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
@@ -55,33 +55,33 @@
 
         self.assert_content_messagemanager_getmessageinfo_(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="消息置顶/取消置顶-Y")
-    def content_messagemanager_messagetop(self, topFlag="$None$", messageIds="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_messagemanager_messagetop(self, messageIds="$None$", topFlag="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/messageManager/messageTop
                 params: messageIds : text : 消息ids集合
                 params: topFlag : text : 消息置顶标识 0-置顶 1-不置顶
                 params: headers : 请求头
         """
-        topFlag = self.get_value_choice(topFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         messageIds = self.get_value_choice(messageIds, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        topFlag = self.get_value_choice(topFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_messagemanager.content_messagemanager_messagetop(**_kwargs)
 
         self.assert_content_messagemanager_messagetop(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="消息新增接口-Y")
-    def content_messagemanager_insert(self, type="$None$", publishTime="$None$", messageId="$None$", sourceType="$None$", publishType="$None$", sendScope="$None$", imageUrl="$None$", content="$None$", param="$None$", checkPublish="$None$", checkStatus="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_messagemanager_insert(self, sendScope="$None$", type="$None$", publishTime="$None$", imageUrl="$None$", checkPublish="$None$", sourceType="$None$", messageId="$None$", checkStatus="$None$", content="$None$", publishType="$None$", param="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/messageManager/insert
                 params: messageId : text :
                 params: type : text : 此处传1
                 params: content : text :
                 params: imageUrl : text :
                 params: sourceType : text : 此处传1
@@ -89,77 +89,77 @@
                 params: sendScope : text :
                 params: checkStatus : text :
                 params: checkPublish : text :
                 params: publishType : text :
                 params: publishTime : text :
                 params: headers : 请求头
         """
+        sendScope = self.get_value_choice(sendScope, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         publishTime = self.get_value_choice(publishTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        messageId = self.get_value_choice(messageId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        sourceType = self.get_value_choice(sourceType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        publishType = self.get_value_choice(publishType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        sendScope = self.get_value_choice(sendScope, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         imageUrl = self.get_value_choice(imageUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        param = self.get_value_choice(param, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         checkPublish = self.get_value_choice(checkPublish, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        sourceType = self.get_value_choice(sourceType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        messageId = self.get_value_choice(messageId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         checkStatus = self.get_value_choice(checkStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishType = self.get_value_choice(publishType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        param = self.get_value_choice(param, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_messagemanager.content_messagemanager_insert(**_kwargs)
 
         self.assert_content_messagemanager_insert(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="消息编辑接口-Y")
-    def content_messagemanager_update(self, type="$None$", messageId="$None$", sourceType="$None$", sendScope="$None$", imageUrl="$None$", userMobiles="$None$", content="$None$", param="$None$", checkPublish="$None$", checkStatus="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_messagemanager_update(self, sendScope="$None$", type="$None$", userMobiles="$None$", imageUrl="$None$", checkPublish="$None$", sourceType="$None$", messageId="$None$", checkStatus="$None$", content="$None$", param="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/messageManager/update
                 params: messageId :  :
                 params: type :  : 此处传1
                 params: content :  :
                 params: imageUrl :  :
                 params: sourceType :  : 此处传1
                 params: param :  :
                 params: sendScope :  :
                 params: checkStatus :  :
                 params: checkPublish :  :
                 params: userMobiles :  : ["131xxxx1234","132xxxx1234"]
                 params: headers : 请求头
         """
-        type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        messageId = self.get_value_choice(messageId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        sourceType = self.get_value_choice(sourceType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         sendScope = self.get_value_choice(sendScope, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        imageUrl = self.get_value_choice(imageUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         userMobiles = self.get_value_choice(userMobiles, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        param = self.get_value_choice(param, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        imageUrl = self.get_value_choice(imageUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         checkPublish = self.get_value_choice(checkPublish, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        sourceType = self.get_value_choice(sourceType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        messageId = self.get_value_choice(messageId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         checkStatus = self.get_value_choice(checkStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        content = self.get_value_choice(content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        param = self.get_value_choice(param, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_messagemanager.content_messagemanager_update(**_kwargs)
 
         self.assert_content_messagemanager_update(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="消息发布状态修改-Y")
-    def content_messagemanager_publishupdate(self, publishStatus="$None$", messageIds="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_messagemanager_publishupdate(self, messageIds="$None$", publishStatus="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/messageManager/publishUpdate
                 params: messageIds : text :
                 params: publishStatus : text :
                 params: headers : 请求头
         """
-        publishStatus = self.get_value_choice(publishStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         messageIds = self.get_value_choice(messageIds, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        publishStatus = self.get_value_choice(publishStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_messagemanager.content_messagemanager_publishupdate(**_kwargs)
 
         self.assert_content_messagemanager_publishupdate(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_noticemanager.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_noticemanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,44 +16,44 @@
 
         self.assert_content_noticemanager_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="获取系统通知详情")
-    def content_noticemanager_getnoticeparamslist_(self, templateType="$None$", messageId="$None$", _assert=True,  **kwargs):
+    def content_noticemanager_getnoticeparamslist_(self, messageId="$None$", templateType="$None$", _assert=True,  **kwargs):
         """
             url=/content/noticeManager/getNoticeParamsList/{messageId}
                 params: messageId :  :
                 params: templateType :  : 模板编码
                 params: headers : 请求头
         """
-        templateType = self.get_list_choice(templateType, list_or_dict=None, key="templateType")
         messageId = self.get_list_choice(messageId, list_or_dict=None, key="messageId")
+        templateType = self.get_list_choice(templateType, list_or_dict=None, key="templateType")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_noticemanager.content_noticemanager_getnoticeparamslist_(**_kwargs)
 
         self.assert_content_noticemanager_getnoticeparamslist_(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="系统通知变量编辑-Y")
-    def content_noticemanager_noticeparamsupdate(self, templateType="$None$", templateName="$None$", templateContent="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_noticemanager_noticeparamsupdate(self, templateContent="$None$", templateName="$None$", templateType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/noticeManager/noticeParamsUpdate
                 params: templateType : string : 模板类型
                 params: templateName : string : 模板名称（标题）
                 params: templateContent : string : 模板内容
                 params: headers : 请求头
         """
-        templateType = self.get_value_choice(templateType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        templateName = self.get_value_choice(templateName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         templateContent = self.get_value_choice(templateContent, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        templateName = self.get_value_choice(templateName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        templateType = self.get_value_choice(templateType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_noticemanager.content_noticemanager_noticeparamsupdate(**_kwargs)
 
         self.assert_content_noticemanager_noticeparamsupdate(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_question.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_question.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from service.app_a.asserts.content.asserts_content_question import AssertsContentQuestion
 from service.app_a.apis.content import apis_content_question
 
 
 class FunsContentQuestion(AssertsContentQuestion):
     @allure.step(title="问答-回复问题-Y")
-    def content_question_answerquestion(self, questionId="$None$", answerContent="$None$", author="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_question_answerquestion(self, answerContent="$None$", author="$None$", questionId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/question/answerQuestion
                 params: questionId : string : 问题主键
                 params: answerContent : string : 回答内容
                 params: author : number : 作者
                 params: headers : 请求头
         """
-        questionId = self.get_value_choice(questionId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         answerContent = self.get_value_choice(answerContent, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         author = self.get_value_choice(author, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        questionId = self.get_value_choice(questionId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_question.content_question_answerquestion(**_kwargs)
 
         self.assert_content_question_answerquestion(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -40,31 +40,31 @@
         self.res = apis_content_question.content_question_revoke(**_kwargs)
 
         self.assert_content_question_revoke(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="问答-搜索问题列表-Y")
-    def content_question_getmanegequestionlist(self, status="$None$", keyWord="$None$", startTime="$None$", endTime="$None$", mobile="$None$", current=1, size=10, _assert=True,  **kwargs):
+    def content_question_getmanegequestionlist(self, current=1, keyWord="$None$", mobile="$None$", endTime="$None$", startTime="$None$", status="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/content/question/getManegeQuestionList
                 params: keyWord :  : 关键字
                 params: mobile :  : 发布人手机号
                 params: startTime :  : 搜索起始时间
                 params: endTime :  : 搜索结束时间
                 params: status :  : 问答状态1：已回复、0：待回复、3：已撤回、4：已归档
                 params: size :  : 每页数据量
                 params: current :  : 页数
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
         keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
-        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_question.content_question_getmanegequestionlist(**_kwargs)
 
         self.assert_content_question_getmanegequestionlist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_recruit.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_recruit.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from service.app_a.asserts.content.asserts_content_recruit import AssertsContentRecruit
 from service.app_a.apis.content import apis_content_recruit
 
 
 class FunsContentRecruit(AssertsContentRecruit):
     @allure.step(title="招聘信息保存-Y")
-    def content_recruit_save(self, fileName="$None$", fileUrl="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_recruit_save(self, fileUrl="$None$", fileName="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/recruit/save
                 params: fileName : string : 文件名
                 params: fileUrl : string : 文件url
                 params: headers : 请求头
         """
-        fileName = self.get_value_choice(fileName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         fileUrl = self.get_value_choice(fileUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        fileName = self.get_value_choice(fileName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_recruit.content_recruit_save(**_kwargs)
 
         self.assert_content_recruit_save(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_safecode.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_safecode.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_subject.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,54 +2,54 @@
 
 from service.app_a.asserts.content.asserts_content_subject import AssertsContentSubject
 from service.app_a.apis.content import apis_content_subject
 
 
 class FunsContentSubject(AssertsContentSubject):
     @allure.step(title="专题-后台App专题文章列表-Y")
-    def content_subject_detailessay(self, subjectId="$None$", size=10, current=1, subjectName="$None$", _assert=True,  **kwargs):
+    def content_subject_detailessay(self, subjectName="$None$", size=10, subjectId="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/content/subject/detailEssay
                 params: current :  :
                 params: size :  :
                 params: subjectId :  : Long
                 params: subjectName :  :  string
                 params: headers : 请求头
         """
-        subjectId = self.get_list_choice(subjectId, list_or_dict=None, key="subjectId")
         subjectName = self.get_list_choice(subjectName, list_or_dict=None, key="subjectName")
+        subjectId = self.get_list_choice(subjectId, list_or_dict=None, key="subjectId")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_subject.content_subject_detailessay(**_kwargs)
 
         self.assert_content_subject_detailessay(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="专题-后台App专题新增-Y")
-    def content_subject_add(self, status="$None$", type="$None$", parentId="$None$", explain="$None$", level="$None$", subPicUrl="$None$", subjectName="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_subject_add(self, explain="$None$", type="$None$", parentId="$None$", subPicUrl="$None$", level="$None$", subjectName="$None$", status="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/subject/add
                 params: subjectName : string : 专题名称
                 params: parentId : string : 父级专题主键
                 params: level : number : 专题等级
                 params: status : number : 是否可用1：是0：否
                 params: explain : string : 说明
                 params: type : number : 关联类型
                 params: subPicUrl : string : 专题图片
                 params: headers : 请求头
         """
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        explain = self.get_value_choice(explain, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         parentId = self.get_value_choice(parentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        explain = self.get_value_choice(explain, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        level = self.get_value_choice(level, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         subPicUrl = self.get_value_choice(subPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        level = self.get_value_choice(level, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         subjectName = self.get_value_choice(subjectName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_subject.content_subject_add(**_kwargs)
 
         self.assert_content_subject_add(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -67,25 +67,25 @@
         self.res = apis_content_subject.content_subject_del(**_kwargs)
 
         self.assert_content_subject_del(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="专题-后台App移动专题更新-Y")
-    def content_subject_mobilesubject(self, subjectId="$None$", serial="$None$", parentId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_subject_mobilesubject(self, parentId="$None$", subjectId="$None$", serial="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/subject/mobileSubject
                 params: subjectId : text : 移动的专题ID
                 params: parentId : text : 移动到的一级专题ID
                 params: serial : text : 排序
                 params: headers : 请求头
         """
+        parentId = self.get_value_choice(parentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         subjectId = self.get_value_choice(subjectId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         serial = self.get_value_choice(serial, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        parentId = self.get_value_choice(parentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_subject.content_subject_mobilesubject(**_kwargs)
 
         self.assert_content_subject_mobilesubject(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -132,15 +132,15 @@
 
         self.assert_content_subject_treelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="专题-后台App保存/更新-Y")
-    def content_subject_save(self, status="$None$", type="$None$", parentId="$None$", explain="$None$", siftFlag="$None$", delFlag="$None$", level="$None$", subjectId="$None$", subPicUrl="$None$", isSearch="$None$", isService="$None$", subjectName="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_subject_save(self, subjectId="$None$", delFlag="$None$", explain="$None$", type="$None$", parentId="$None$", subPicUrl="$None$", siftFlag="$None$", level="$None$", subjectName="$None$", status="$None$", isSearch="$None$", isService="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/subject/save
                 params: subjectId : number :
                 params: subjectName : string :
                 params: level : number :
                 params: delFlag : number :
                 params: subPicUrl : string :
@@ -149,26 +149,26 @@
                 params: type : number :
                 params: parentId : string : 父ID
                 params: siftFlag : number : 是否精选 1是 0否
                 params: isService : number : 是否设置客服入口 1是 0否
                 params: isSearch : number : 是否配置搜索 0否 1是
                 params: headers : 请求头
         """
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        subjectId = self.get_value_choice(subjectId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        delFlag = self.get_value_choice(delFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        explain = self.get_value_choice(explain, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         parentId = self.get_value_choice(parentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        explain = self.get_value_choice(explain, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        subPicUrl = self.get_value_choice(subPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         siftFlag = self.get_value_choice(siftFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        delFlag = self.get_value_choice(delFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         level = self.get_value_choice(level, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        subjectId = self.get_value_choice(subjectId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        subPicUrl = self.get_value_choice(subPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        subjectName = self.get_value_choice(subjectName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         isSearch = self.get_value_choice(isSearch, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         isService = self.get_value_choice(isService, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        subjectName = self.get_value_choice(subjectName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_subject.content_subject_save(**_kwargs)
 
         self.assert_content_subject_save(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_subjectweb.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_subjectweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.content.asserts_content_subjectweb import AssertsContentSubjectweb
 from service.app_a.apis.content import apis_content_subjectweb
 
 
 class FunsContentSubjectweb(AssertsContentSubjectweb):
     @allure.step(title="专题-后台官网专题文章列表-Y")
-    def content_subjectweb_detailessay(self, subjectId="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def content_subjectweb_detailessay(self, size=10, subjectId="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/content/subjectweb/detailEssay
                 params: current :  : 当前页
                 params: size :  : 当前条数
                 params: subjectId :  : 专题主键id
                 params: headers : 请求头
         """
@@ -21,15 +21,15 @@
 
         self.assert_content_subjectweb_detailessay(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="专题-后台官网专题新增-Y")
-    def content_subjectweb_add(self, status="$None$", type="$None$", parentId="$None$", subjectRank="$None$", explain="$None$", siftFlag="$None$", siftPicUrl="$None$", web="$None$", level="$None$", subPicUrl="$None$", serial="$None$", isSearch="$None$", recommend="$None$", isService="$None$", subjectName="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_subjectweb_add(self, subjectRank="$None$", web="$None$", type="$None$", explain="$None$", serial="$None$", parentId="$None$", subPicUrl="$None$", siftFlag="$None$", level="$None$", subjectName="$None$", status="$None$", siftPicUrl="$None$", isSearch="$None$", isService="$None$", recommend="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/subjectweb/add
                 params: subjectName : string : 专题名称
                 params: level : string : 专题等级
                 params: status : string : 是否可用1：是 0：否
                 params: explain : string : 说明
                 params: type : string : 关联类型
@@ -41,29 +41,29 @@
                 params: isSearch : integer : 是否配置搜索 0否 1是
                 params: siftPicUrl : string : 精选配图
                 params: web : string :
                 params: recommend : integer : 咨询页展示
                 params: subjectRank : integer : 精选权重
                 params: headers : 请求头
         """
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        parentId = self.get_value_choice(parentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         subjectRank = self.get_value_choice(subjectRank, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        web = self.get_value_choice(web, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         explain = self.get_value_choice(explain, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        serial = self.get_value_choice(serial, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        parentId = self.get_value_choice(parentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        subPicUrl = self.get_value_choice(subPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         siftFlag = self.get_value_choice(siftFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        siftPicUrl = self.get_value_choice(siftPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        web = self.get_value_choice(web, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         level = self.get_value_choice(level, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        subPicUrl = self.get_value_choice(subPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        serial = self.get_value_choice(serial, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        subjectName = self.get_value_choice(subjectName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        siftPicUrl = self.get_value_choice(siftPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         isSearch = self.get_value_choice(isSearch, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        recommend = self.get_value_choice(recommend, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         isService = self.get_value_choice(isService, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        subjectName = self.get_value_choice(subjectName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        recommend = self.get_value_choice(recommend, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_subjectweb.content_subjectweb_add(**_kwargs)
 
         self.assert_content_subjectweb_add(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -79,15 +79,15 @@
 
         self.assert_content_subjectweb_treelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="专题-后台官网保存/更新-Y")
-    def content_subjectweb_save(self, status="$None$", type="$None$", parentId="$None$", explain="$None$", siftFlag="$None$", delFlag="$None$", subjectId="$None$", subPicUrl="$None$", isSearch="$None$", isService="$None$", subjectName="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_subjectweb_save(self, subjectId="$None$", delFlag="$None$", explain="$None$", type="$None$", parentId="$None$", subPicUrl="$None$", siftFlag="$None$", subjectName="$None$", status="$None$", isSearch="$None$", isService="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/subjectweb/save
                 params: subjectId : string :
                 params: subjectName : string :
                 params: delFlag : string :
                 params: subPicUrl : string :
                 params: explain : string :
@@ -95,25 +95,25 @@
                 params: type : string :
                 params: parentId : string :
                 params: siftFlag : string :
                 params: isService : string :
                 params: isSearch : string :
                 params: headers : 请求头
         """
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        subjectId = self.get_value_choice(subjectId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        delFlag = self.get_value_choice(delFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        explain = self.get_value_choice(explain, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         parentId = self.get_value_choice(parentId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        explain = self.get_value_choice(explain, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        siftFlag = self.get_value_choice(siftFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        delFlag = self.get_value_choice(delFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        subjectId = self.get_value_choice(subjectId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         subPicUrl = self.get_value_choice(subPicUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        siftFlag = self.get_value_choice(siftFlag, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        subjectName = self.get_value_choice(subjectName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         isSearch = self.get_value_choice(isSearch, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         isService = self.get_value_choice(isService, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        subjectName = self.get_value_choice(subjectName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_subjectweb.content_subjectweb_save(**_kwargs)
 
         self.assert_content_subjectweb_save(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -148,15 +148,15 @@
 
         self.assert_content_subjectweb_detail(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="新闻中心文章列表-Y")
-    def content_subjectweb_detailessaynew(self, subjectId="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def content_subjectweb_detailessaynew(self, size=10, subjectId="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/content/subjectweb/detailEssayNew
                 params: current :  :
                 params: size :  :
                 params: subjectId :  : 2 官方新闻 3 自媒体 4 媒体报道  null 全部
                 params: headers : 请求头
         """
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/funs_content_topic4c.py` & `huhk-1.9.6/service/app_a/funs/content/funs_content_topic4c.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.res = apis_content_topic4c.content_topic4c_del(**_kwargs)
 
         self.assert_content_topic4c_del(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="话题-获取动态关联列表-Y")
-    def content_topic4c_getcontentlist(self, topicId="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def content_topic4c_getcontentlist(self, size=10, topicId="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/content/topic4C/getContentList
                 params: topicId :  : 话题主键
                 params: size :  : 每页数据数
                 params: current :  : 当前页
                 params: headers : 请求头
         """
@@ -37,70 +37,70 @@
 
         self.assert_content_topic4c_getcontentlist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="话题-搜索话题列表")
-    def content_topic4c_list(self, topicId="$None$", keyWord="$None$", startTime="$None$", endTime="$None$", current=1, createBy="$None$", size=10, _assert=True,  **kwargs):
+    def content_topic4c_list(self, createBy="$None$", current=1, keyWord="$None$", endTime="$None$", startTime="$None$", topicId="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/content/topic4C/list
                 params: topicId :  : 话题主键
                 params: createBy :  : 发布人主键
                 params: keyWord :  : 话题关键字
                 params: startTime :  : 搜索开始时间
                 params: endTime :  : 搜索结束时间
                 params: size :  : 每页数量数
                 params: current :  : 当前页
                 params: headers : 请求头
         """
-        topicId = self.get_list_choice(topicId, list_or_dict=None, key="topicId")
+        createBy = self.get_list_choice(createBy, list_or_dict=None, key="createBy")
         keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        createBy = self.get_list_choice(createBy, list_or_dict=None, key="createBy")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        topicId = self.get_list_choice(topicId, list_or_dict=None, key="topicId")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_topic4c.content_topic4c_list(**_kwargs)
 
         self.assert_content_topic4c_list(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="话题-新增话题")
-    def content_topic4c_insert(self, author="$None$", topicId="$None$", topicTitle="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_topic4c_insert(self, topicId="$None$", author="$None$", topicTitle="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/topic4C/insert
                 params: topicId : string : 话题主键
                 params: topicTitle : string : 话题
                 params: author : number : 话题作者
                 params: headers : 请求头
         """
-        author = self.get_value_choice(author, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         topicId = self.get_value_choice(topicId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        author = self.get_value_choice(author, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         topicTitle = self.get_value_choice(topicTitle, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_topic4c.content_topic4c_insert(**_kwargs)
 
         self.assert_content_topic4c_insert(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="话题-置顶")
-    def content_topic4c_top(self, type="$None$", topicId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def content_topic4c_top(self, topicId="$None$", type="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/content/topic4C/top
                 params: topicId : string : 话题主键
                 params: type : string : 操作类型1：置顶2：取消置顶
                 params: headers : 请求头
         """
-        type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         topicId = self.get_value_choice(topicId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        type = self.get_value_choice(type, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_content_topic4c.content_topic4c_top(**_kwargs)
 
         self.assert_content_topic4c_top(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/content/material/funs_content_material_getmateriallist.py` & `huhk-1.9.6/service/app_a/funs/content/material/funs_content_material_getmateriallist.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.content.material.asserts_content_material_getmateriallist import AssertsContentMaterialGetmateriallist
 from service.app_a.apis.content.material import apis_content_material_getmateriallist
 
 
 class FunsContentMaterialGetmateriallist(AssertsContentMaterialGetmateriallist):
     @allure.step(title="素材-根据素材组获取素材列表_copy")
-    def content_material_getmateriallist_1659319316474(self, groupId="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def content_material_getmateriallist_1659319316474(self, size=10, groupId="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/content/material/getMaterialList_1659319316474
                 params: groupId :  : 分组主键
                 params: size :  : 每页数据数
                 params: current :  : 当前页
                 params: headers : 请求头
         """
```

### Comparing `huhk-1.9.5/service/app_a/funs/funs_activitymanager.py` & `huhk-1.9.6/service/app_a/funs/funs_activitymanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/funs_app_a.py` & `huhk-1.9.6/service/app_a/funs/funs_app_a.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from service.app_a.funs.funs_manageapi import FunsManageapi
 from service.app_a.funs.funs_essay import FunsEssay
 from service.app_a.funs.funs_area import FunsArea
 
 
 class FunsAppA(FunsOrder, FunsOpen, FunsContent, FunsAdmin, FunsCommon, FunsGoods, FunsActivitymanager, FunsRadarpoints, FunsPay, FunsTestdrive, FunsManageapi, FunsEssay, AssertsAppA, FunsArea):
     @allure.step(title="网点列表-获取经销商")
-    def page(self, district="$None$", province="$None$", provinceNameSort="$None$", cityNameSort="$None$", dealerName="$None$", shopBusinessType="$None$", districtNameSort="$None$", dealerCode="$None$", current=1, dealerAddress="$None$", city="$None$", size=10, _assert=True,  **kwargs):
+    def page(self, current=1, dealerAddress="$None$", districtNameSort="$None$", cityNameSort="$None$", city="$None$", province="$None$", dealerName="$None$", shopBusinessType="$None$", district="$None$", size=10, dealerCode="$None$", provinceNameSort="$None$", _assert=True,  **kwargs):
         """
             url=/page
                 params: current :  :
                 params: size :  :
                 params: province :  :
                 params: city :  :
                 params: district :  :
@@ -31,24 +31,24 @@
                 params: dealerAddress :  :
                 params: shopBusinessType :  :
                 params: cityNameSort :  :
                 params: districtNameSort :  :
                 params: provinceNameSort :  :
                 params: headers : 请求头
         """
-        district = self.get_list_choice(district, list_or_dict=None, key="district")
-        province = self.get_list_choice(province, list_or_dict=None, key="province")
-        provinceNameSort = self.get_list_choice(provinceNameSort, list_or_dict=None, key="provinceNameSort")
+        dealerAddress = self.get_list_choice(dealerAddress, list_or_dict=None, key="dealerAddress")
+        districtNameSort = self.get_list_choice(districtNameSort, list_or_dict=None, key="districtNameSort")
         cityNameSort = self.get_list_choice(cityNameSort, list_or_dict=None, key="cityNameSort")
+        city = self.get_list_choice(city, list_or_dict=None, key="city")
+        province = self.get_list_choice(province, list_or_dict=None, key="province")
         dealerName = self.get_list_choice(dealerName, list_or_dict=None, key="dealerName")
         shopBusinessType = self.get_list_choice(shopBusinessType, list_or_dict=None, key="shopBusinessType")
-        districtNameSort = self.get_list_choice(districtNameSort, list_or_dict=None, key="districtNameSort")
+        district = self.get_list_choice(district, list_or_dict=None, key="district")
         dealerCode = self.get_list_choice(dealerCode, list_or_dict=None, key="dealerCode")
-        dealerAddress = self.get_list_choice(dealerAddress, list_or_dict=None, key="dealerAddress")
-        city = self.get_list_choice(city, list_or_dict=None, key="city")
+        provinceNameSort = self.get_list_choice(provinceNameSort, list_or_dict=None, key="provinceNameSort")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_app_a.page(**_kwargs)
 
         self.assert_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/funs_area.py` & `huhk-1.9.6/service/app_a/funs/funs_area.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/funs_common.py` & `huhk-1.9.6/service/app_a/funs/funs_common.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/funs_content.py` & `huhk-1.9.6/service/app_a/funs/funs_content.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/funs_essay.py` & `huhk-1.9.6/service/app_a/funs/funs_essay.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,33 +20,33 @@
         self.res = apis_essay.essay_batch(**_kwargs)
 
         self.assert_essay_batch(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="文章-获取列表状态数量-Y")
-    def essay_querylistcount(self, status="$None$", keyWord="$None$", startTime="$None$", endTime="$None$", subjectId="$None$", author="$None$", essayId="$None$", _assert=True,  **kwargs):
+    def essay_querylistcount(self, author="$None$", subjectId="$None$", essayId="$None$", keyWord="$None$", endTime="$None$", startTime="$None$", status="$None$", _assert=True,  **kwargs):
         """
             url=/essay/queryListCount
                 params: essayId :  : 文章主键
                 params: keyWord :  : 搜索关键字
                 params: author :  : 作者
                 params: startTime :  : 搜索起始时间
                 params: endTime :  : 搜索结束时间
                 params: subjectId :  : 专题主键
                 params: status :  : 状态
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
-        keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
-        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        subjectId = self.get_list_choice(subjectId, list_or_dict=None, key="subjectId")
         author = self.get_list_choice(author, list_or_dict=None, key="author")
+        subjectId = self.get_list_choice(subjectId, list_or_dict=None, key="subjectId")
         essayId = self.get_list_choice(essayId, list_or_dict=None, key="essayId")
+        keyWord = self.get_list_choice(keyWord, list_or_dict=None, key="keyWord")
+        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_essay.essay_querylistcount(**_kwargs)
 
         self.assert_essay_querylistcount(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/funs_order.py` & `huhk-1.9.6/service/app_a/funs/funs_order.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/funs_radarpoints.py` & `huhk-1.9.6/service/app_a/funs/funs_radarpoints.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/funs_testdrive.py` & `huhk-1.9.6/service/app_a/funs/funs_testdrive.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.asserts_testdrive import AssertsTestdrive
 from service.app_a.apis import apis_testdrive
 
 
 class FunsTestdrive(AssertsTestdrive):
     @allure.step(title="预约试驾")
-    def testdrive_subscribe(self, shopId="$None$", appointmentTime="$None$", modelId="$None$", model="$None$", shopName="$None$", leadSourceCode="$None$", customerName="$None$", activityCode="$None$", phoneNumber="$None$", channel="$None$", leadSanSourceCode="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def testdrive_subscribe(self, leadSanSourceCode="$None$", phoneNumber="$None$", appointmentTime="$None$", channel="$None$", customerName="$None$", activityCode="$None$", shopName="$None$", shopId="$None$", leadSourceCode="$None$", model="$None$", modelId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/testDrive/subscribe
                 params: model : text : 试驾车型名称
                 params: shopName : text : 门店名称
                 params: customerName : text : 客户姓名、昵称
                 params: phoneNumber : text : 预留手机号
                 params: channel : text : 1:移动应用 2:小程序 3:官方网站
@@ -18,25 +18,25 @@
                 params: shopId : text : 预约门店id
                 params: appointmentTime : text : 预约时间
                 params: activityCode : string : 活动代码
                 params: leadSourceCode : string : 线索来源小类
                 params: leadSanSourceCode : string : 线索来源三级小类
                 params: headers : 请求头
         """
-        shopId = self.get_value_choice(shopId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        leadSanSourceCode = self.get_value_choice(leadSanSourceCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        phoneNumber = self.get_value_choice(phoneNumber, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         appointmentTime = self.get_value_choice(appointmentTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        modelId = self.get_value_choice(modelId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        model = self.get_value_choice(model, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        shopName = self.get_value_choice(shopName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        leadSourceCode = self.get_value_choice(leadSourceCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        channel = self.get_value_choice(channel, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         customerName = self.get_value_choice(customerName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         activityCode = self.get_value_choice(activityCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        phoneNumber = self.get_value_choice(phoneNumber, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        channel = self.get_value_choice(channel, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        leadSanSourceCode = self.get_value_choice(leadSanSourceCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        shopName = self.get_value_choice(shopName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        shopId = self.get_value_choice(shopId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        leadSourceCode = self.get_value_choice(leadSourceCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        model = self.get_value_choice(model, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        modelId = self.get_value_choice(modelId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_testdrive.testdrive_subscribe(**_kwargs)
 
         self.assert_testdrive_subscribe(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/goods/funs_goods_area.py` & `huhk-1.9.6/service/app_a/funs/goods/funs_goods_area.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/goods/funs_goods_carmodel.py` & `huhk-1.9.6/service/app_a/funs/goods/funs_goods_carmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.goods.asserts_goods_carmodel import AssertsGoodsCarmodel
 from service.app_a.apis.goods import apis_goods_carmodel
 
 
 class FunsGoodsCarmodel(AssertsGoodsCarmodel):
     @allure.step(title="保存车型详细信息 - Y")
-    def goods_carmodel_savemanagecarmodel(self, modelId="$None$", promptDesc="$None$", prePricePosters="$None$", depositPrice="$None$", carName="$None$", carDetailUrl="$None$", depositEndTime="$None$", version="$None$", status="$None$", modelName="$None$", preToDepositEndTime="$None$", preToDepositStartTime="$None$", depositStartTime="$None$", carCode="$None$", prePrice="$None$", prePriceContent="$None$", posters="$None$", carDetailPics="$None$", price="$None$", sort="$None$", modelCode="$None$", preEndTime="$None$", carSimpleName="$None$", depositPriceContent="$None$", brandName="$None$", preStartTime="$None$", configCode="$None$", sharePosters="$None$", carDetailType="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def goods_carmodel_savemanagecarmodel(self, prePricePosters="$None$", carDetailPics="$None$", depositPrice="$None$", carCode="$None$", preToDepositEndTime="$None$", preStartTime="$None$", sharePosters="$None$", depositEndTime="$None$", modelId="$None$", carDetailUrl="$None$", price="$None$", depositStartTime="$None$", preEndTime="$None$", promptDesc="$None$", brandName="$None$", modelName="$None$", carSimpleName="$None$", prePriceContent="$None$", status="$None$", posters="$None$", carDetailType="$None$", sort="$None$", prePrice="$None$", preToDepositStartTime="$None$", carName="$None$", modelCode="$None$", configCode="$None$", version="$None$", depositPriceContent="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/goods/carmodel/saveManageCarModel
                 params: carName : string : 车系名称
                 params: brandName : string : 品牌名称
                 params: version : string : 品牌代码
                 params: carCode : string : 车系代码
                 params: modelName : string : 车型名称
@@ -44,43 +44,43 @@
                 imageUrl : string :
                 modelId : string :
                 params: promptDesc : string : 提示文案
                 params: modelId : string : 车型ID
                 params: status : number : 状态(0禁用1启用)
                 params: headers : 请求头
         """
-        modelId = self.get_value_choice(modelId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        promptDesc = self.get_value_choice(promptDesc, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         prePricePosters = self.get_value_choice(prePricePosters, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        carDetailPics = self.get_value_choice(carDetailPics, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         depositPrice = self.get_value_choice(depositPrice, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        carName = self.get_value_choice(carName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        carDetailUrl = self.get_value_choice(carDetailUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        depositEndTime = self.get_value_choice(depositEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        version = self.get_value_choice(version, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        modelName = self.get_value_choice(modelName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        carCode = self.get_value_choice(carCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         preToDepositEndTime = self.get_value_choice(preToDepositEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        preToDepositStartTime = self.get_value_choice(preToDepositStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        preStartTime = self.get_value_choice(preStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        sharePosters = self.get_value_choice(sharePosters, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        depositEndTime = self.get_value_choice(depositEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        modelId = self.get_value_choice(modelId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        carDetailUrl = self.get_value_choice(carDetailUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        price = self.get_value_choice(price, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         depositStartTime = self.get_value_choice(depositStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        carCode = self.get_value_choice(carCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        prePrice = self.get_value_choice(prePrice, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        preEndTime = self.get_value_choice(preEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        promptDesc = self.get_value_choice(promptDesc, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        brandName = self.get_value_choice(brandName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        modelName = self.get_value_choice(modelName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        carSimpleName = self.get_value_choice(carSimpleName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         prePriceContent = self.get_value_choice(prePriceContent, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         posters = self.get_value_choice(posters, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        carDetailPics = self.get_value_choice(carDetailPics, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        price = self.get_value_choice(price, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        carDetailType = self.get_value_choice(carDetailType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         sort = self.get_value_choice(sort, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        prePrice = self.get_value_choice(prePrice, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        preToDepositStartTime = self.get_value_choice(preToDepositStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        carName = self.get_value_choice(carName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         modelCode = self.get_value_choice(modelCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        preEndTime = self.get_value_choice(preEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        carSimpleName = self.get_value_choice(carSimpleName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        depositPriceContent = self.get_value_choice(depositPriceContent, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        brandName = self.get_value_choice(brandName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        preStartTime = self.get_value_choice(preStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         configCode = self.get_value_choice(configCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        sharePosters = self.get_value_choice(sharePosters, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        carDetailType = self.get_value_choice(carDetailType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        version = self.get_value_choice(version, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        depositPriceContent = self.get_value_choice(depositPriceContent, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_goods_carmodel.goods_carmodel_savemanagecarmodel(**_kwargs)
 
         self.assert_goods_carmodel_savemanagecarmodel(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -116,36 +116,36 @@
 
         self.assert_goods_carmodel_getcarmodelmanagebyid(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="车型列表-Y")
-    def goods_carmodel_getmanagecarmodel(self, status="$None$", brandName="$None$", modelCode="$None$", modelName="$None$", operator="$None$", carName="$None$", current=1, carCode="$None$", size=10, version="$None$", _assert=True,  **kwargs):
+    def goods_carmodel_getmanagecarmodel(self, carName="$None$", modelCode="$None$", current=1, operator="$None$", brandName="$None$", modelName="$None$", carCode="$None$", status="$None$", version="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/goods/carmodel/getManageCarModel
                 params: current :  : 分页
                 params: size :  : 分页
                 params: modelName :  : 车型名称
                 params: modelCode :  : 车型代号
                 params: status :  : 0:待启用，1:启用，2:禁用 车型新增默认状态待启用，全部则不传值
                 params: operator :  : 操作人
                 params: brandName :  : 品牌名称
                 params: version :  : 品牌编码
                 params: carName :  : 车系名称
                 params: carCode :  : 车型编码
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
-        brandName = self.get_list_choice(brandName, list_or_dict=None, key="brandName")
+        carName = self.get_list_choice(carName, list_or_dict=None, key="carName")
         modelCode = self.get_list_choice(modelCode, list_or_dict=None, key="modelCode")
-        modelName = self.get_list_choice(modelName, list_or_dict=None, key="modelName")
         operator = self.get_list_choice(operator, list_or_dict=None, key="operator")
-        carName = self.get_list_choice(carName, list_or_dict=None, key="carName")
+        brandName = self.get_list_choice(brandName, list_or_dict=None, key="brandName")
+        modelName = self.get_list_choice(modelName, list_or_dict=None, key="modelName")
         carCode = self.get_list_choice(carCode, list_or_dict=None, key="carCode")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
         version = self.get_list_choice(version, list_or_dict=None, key="version")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_goods_carmodel.goods_carmodel_getmanagecarmodel(**_kwargs)
 
         self.assert_goods_carmodel_getmanagecarmodel(_assert, **_kwargs)
         self.set_output_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/goods/funs_goods_configure.py` & `huhk-1.9.6/service/app_a/funs/goods/funs_goods_configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.goods.asserts_goods_configure import AssertsGoodsConfigure
 from service.app_a.apis.goods import apis_goods_configure
 
 
 class FunsGoodsConfigure(AssertsGoodsConfigure):
     @allure.step(title="保存车型配置信息-Y")
-    def goods_configure_savecarconfigure(self, processColorList="$None$", salesVersionList="$None$", interiorColorList="$None$", appearanceColorList="$None$", optionalList="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def goods_configure_savecarconfigure(self, salesVersionList="$None$", appearanceColorList="$None$", interiorColorList="$None$", processColorList="$None$", optionalList="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/goods/configure/saveCarConfigure
                 params: salesVersionList : array : 销售版本
                 configureId : string : 配置ID
                 modelId : string : 关联的车型基础信息ID
                 configureCode : string : 配置编码
                 configureName : string : 配置名称
@@ -99,18 +99,18 @@
                 sort : number : 排序
                 versionDesc : string :
                 partsDesc : string : 配件描述
                 status : number : 状态 默认启用 1
                 type : number : 1:销售版本,2:外观颜色,3:套色,4:内饰颜色,5:选装配置
                 params: headers : 请求头
         """
-        processColorList = self.get_value_choice(processColorList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         salesVersionList = self.get_value_choice(salesVersionList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        interiorColorList = self.get_value_choice(interiorColorList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         appearanceColorList = self.get_value_choice(appearanceColorList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        interiorColorList = self.get_value_choice(interiorColorList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        processColorList = self.get_value_choice(processColorList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         optionalList = self.get_value_choice(optionalList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_goods_configure.goods_configure_savecarconfigure(**_kwargs)
 
         self.assert_goods_configure_savecarconfigure(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/goods/funs_goods_ordermain.py` & `huhk-1.9.6/service/app_a/funs/goods/funs_goods_ordermain.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,67 +18,67 @@
         self.res = apis_goods_ordermain.goods_ordermain_pay(**_kwargs)
 
         self.assert_goods_ordermain_pay(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="订单列表文件导出接口-Y")
-    def goods_ordermain_orderexports(self, userMobile="$None$", billStatus="$None$", modelName="$None$", startTime="$None$", endTime="$None$", userName="$None$", shopName="$None$", testDriveIdStr="$None$", exportType="$None$", _assert=True,  **kwargs):
+    def goods_ordermain_orderexports(self, exportType="$None$", testDriveIdStr="$None$", billStatus="$None$", modelName="$None$", shopName="$None$", endTime="$None$", startTime="$None$", userMobile="$None$", userName="$None$", _assert=True,  **kwargs):
         """
             url=/goods/orderMain/orderExports
                 params: userMobile :  : 手机号
                 params: userName :  : 用户名
                 params: shopName :  : 店名
                 params: modelName :  : 车型
                 params: billStatus	 :  : 支付状态
                 params: startTime :  : 开始时间
                 params: endTime :  : 结束时间
                 params: exportType :  : 导出类型
                 params: testDriveIdStr :  : 订单集合字符串
                 params: headers : 请求头
         """
-        userMobile = self.get_list_choice(userMobile, list_or_dict=None, key="userMobile")
+        exportType = self.get_list_choice(exportType, list_or_dict=None, key="exportType")
+        testDriveIdStr = self.get_list_choice(testDriveIdStr, list_or_dict=None, key="testDriveIdStr")
         billStatus = self.get_list_choice(billStatus, list_or_dict=None, key="billStatus")
         modelName = self.get_list_choice(modelName, list_or_dict=None, key="modelName")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        userMobile = self.get_list_choice(userMobile, list_or_dict=None, key="userMobile")
         userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
-        shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
-        testDriveIdStr = self.get_list_choice(testDriveIdStr, list_or_dict=None, key="testDriveIdStr")
-        exportType = self.get_list_choice(exportType, list_or_dict=None, key="exportType")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_goods_ordermain.goods_ordermain_orderexports(**_kwargs)
 
         self.assert_goods_ordermain_orderexports(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="订单查询接口-Y")
-    def goods_ordermain_getordermainpage(self, userMobile="$None$", modelName="$None$", startTime="$None$", endTime="$None$", userName="$None$", shopName="$None$", orderStatus="$None$", _assert=True,  **kwargs):
+    def goods_ordermain_getordermainpage(self, orderStatus="$None$", modelName="$None$", shopName="$None$", endTime="$None$", startTime="$None$", userMobile="$None$", userName="$None$", _assert=True,  **kwargs):
         """
             url=/goods/orderMain/getOrderMainPage
                 params: userMobile :  : 手机号
                 params: userName :  : 用户名
                 params: modelName :  : 车型
                 params: orderStatus	 :  : 支付状态 1001待支付 1002已支付 1003已完成 1004待退款
                 1005已取消 1006已退款 1007已驳回
                 params: startTime :  : 开始时间
                 params: endTime :  : 结束时间
                 params: shopName :  : 门店名称
                 params: headers : 请求头
         """
-        userMobile = self.get_list_choice(userMobile, list_or_dict=None, key="userMobile")
+        orderStatus = self.get_list_choice(orderStatus, list_or_dict=None, key="orderStatus")
         modelName = self.get_list_choice(modelName, list_or_dict=None, key="modelName")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        userMobile = self.get_list_choice(userMobile, list_or_dict=None, key="userMobile")
         userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
-        shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
-        orderStatus = self.get_list_choice(orderStatus, list_or_dict=None, key="orderStatus")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_goods_ordermain.goods_ordermain_getordermainpage(**_kwargs)
 
         self.assert_goods_ordermain_getordermainpage(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/goods/funs_goods_testdrive.py` & `huhk-1.9.6/service/app_a/funs/goods/funs_goods_testdrive.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,65 +2,65 @@
 
 from service.app_a.asserts.goods.asserts_goods_testdrive import AssertsGoodsTestdrive
 from service.app_a.apis.goods import apis_goods_testdrive
 
 
 class FunsGoodsTestdrive(AssertsGoodsTestdrive):
     @allure.step(title="试驾列表文件导出接口-Y")
-    def goods_testdrive_driveexports(self, startTime="$None$", endTime="$None$", userName="$None$", shopName="$None$", mobile="$None$", channel="$None$", testDriveIdStr="$None$", exportType="$None$", _assert=True,  **kwargs):
+    def goods_testdrive_driveexports(self, exportType="$None$", testDriveIdStr="$None$", channel="$None$", mobile="$None$", shopName="$None$", endTime="$None$", startTime="$None$", userName="$None$", _assert=True,  **kwargs):
         """
             url=/goods/testDrive/driveExports
                 params: mobile :  : 手机号
                 params: userName :  : 用户名
                 params: shopName :  : 店名
                 params: channel :  : 渠道
                 params: startTime :  : 开始时间
                 params: endTime :  : 结束时间
                 params: exportType :  : 导出类型
                 params: testDriveIdStr :  : 订单集合字符串
                 params: headers : 请求头
         """
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        exportType = self.get_list_choice(exportType, list_or_dict=None, key="exportType")
+        testDriveIdStr = self.get_list_choice(testDriveIdStr, list_or_dict=None, key="testDriveIdStr")
+        channel = self.get_list_choice(channel, list_or_dict=None, key="channel")
+        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
         userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
-        shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
-        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        channel = self.get_list_choice(channel, list_or_dict=None, key="channel")
-        testDriveIdStr = self.get_list_choice(testDriveIdStr, list_or_dict=None, key="testDriveIdStr")
-        exportType = self.get_list_choice(exportType, list_or_dict=None, key="exportType")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_goods_testdrive.goods_testdrive_driveexports(**_kwargs)
 
         self.assert_goods_testdrive_driveexports(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="试驾查询接口-Y")
-    def goods_testdrive_page(self, pageNum=1, pageSize="$None$", startTime="$None$", endTime="$None$", userName="$None$", shopName="$None$", mobile="$None$", channel="$None$", _assert=True,  **kwargs):
+    def goods_testdrive_page(self, pageSize="$None$", channel="$None$", mobile="$None$", shopName="$None$", endTime="$None$", startTime="$None$", userName="$None$", pageNum=1, _assert=True,  **kwargs):
         """
             url=/goods/testDrive/page
                 params: mobile :  : 手机号
                 params: userName :  : 客户名
                 params: shopName :  : 店名
                 params: channel :  : 渠道
                 params: startTime :  : 开始时间
                 params: endTime :  : 结束时间
                 params: pageNum :  : 当前页数
                 params: pageSize :  : 每页数据数
                 params: headers : 请求头
         """
         pageSize = self.get_list_choice(pageSize, list_or_dict=None, key="pageSize")
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
+        channel = self.get_list_choice(channel, list_or_dict=None, key="channel")
+        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
         endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
         userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
-        shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
-        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        channel = self.get_list_choice(channel, list_or_dict=None, key="channel")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_goods_testdrive.goods_testdrive_page(**_kwargs)
 
         self.assert_goods_testdrive_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/manageapi/order/funs_manageapi_order_mainorder.py` & `huhk-1.9.6/service/app_a/funs/manageapi/order/funs_manageapi_order_mainorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.manageapi.order.asserts_manageapi_order_mainorder import AssertsManageapiOrderMainorder
 from service.app_a.apis.manageapi.order import apis_manageapi_order_mainorder
 
 
 class FunsManageapiOrderMainorder(AssertsManageapiOrderMainorder):
     @allure.step(title="订单管理-后台查询订单列表-Y")
-    def manageapi_order_mainorder_pagelist(self, modelId="$None$", mainOrderId="$None$", channel="$None$", cityId="$None$", userName="$None$", dealerCode="$None$", createEndTime="$None$", extNum="$None$", mobile="$None$", orderId="$None$", orderType="$None$", createStartTime="$None$", current=1, orderStatus="$None$", extOrderStatus="$None$", size=10, provinceId="$None$", _assert=True,  **kwargs):
+    def manageapi_order_mainorder_pagelist(self, extNum="$None$", provinceId="$None$", current=1, extOrderStatus="$None$", channel="$None$", createStartTime="$None$", createEndTime="$None$", mobile="$None$", orderId="$None$", orderType="$None$", cityId="$None$", mainOrderId="$None$", size=10, userName="$None$", dealerCode="$None$", orderStatus="$None$", modelId="$None$", _assert=True,  **kwargs):
         """
             url=/manageapi/order/mainOrder/pageList
                 params: mobile :  : 购买人手机号
                 params: userName :  : 购买人
                 params: modelId :  : 车型ID
                 params: provinceId :  : 省编码
                 params: cityId :  : 市编码
@@ -25,29 +25,29 @@
                 params: createStartTime :  : 订单创建开始日期
                 params: createEndTime :  : 订单创建结束日期
                 params: extNum :  : 三方订单号
                 params: current :  :
                 params: size :  :
                 params: headers : 请求头
         """
-        modelId = self.get_list_choice(modelId, list_or_dict=None, key="modelId")
-        mainOrderId = self.get_list_choice(mainOrderId, list_or_dict=None, key="mainOrderId")
+        extNum = self.get_list_choice(extNum, list_or_dict=None, key="extNum")
+        provinceId = self.get_list_choice(provinceId, list_or_dict=None, key="provinceId")
+        extOrderStatus = self.get_list_choice(extOrderStatus, list_or_dict=None, key="extOrderStatus")
         channel = self.get_list_choice(channel, list_or_dict=None, key="channel")
-        cityId = self.get_list_choice(cityId, list_or_dict=None, key="cityId")
-        userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
-        dealerCode = self.get_list_choice(dealerCode, list_or_dict=None, key="dealerCode")
+        createStartTime = self.get_list_choice(createStartTime, list_or_dict=None, key="createStartTime")
         createEndTime = self.get_list_choice(createEndTime, list_or_dict=None, key="createEndTime")
-        extNum = self.get_list_choice(extNum, list_or_dict=None, key="extNum")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
         orderId = self.get_list_choice(orderId, list_or_dict=None, key="orderId")
         orderType = self.get_list_choice(orderType, list_or_dict=None, key="orderType")
-        createStartTime = self.get_list_choice(createStartTime, list_or_dict=None, key="createStartTime")
+        cityId = self.get_list_choice(cityId, list_or_dict=None, key="cityId")
+        mainOrderId = self.get_list_choice(mainOrderId, list_or_dict=None, key="mainOrderId")
+        userName = self.get_list_choice(userName, list_or_dict=None, key="userName")
+        dealerCode = self.get_list_choice(dealerCode, list_or_dict=None, key="dealerCode")
         orderStatus = self.get_list_choice(orderStatus, list_or_dict=None, key="orderStatus")
-        extOrderStatus = self.get_list_choice(extOrderStatus, list_or_dict=None, key="extOrderStatus")
-        provinceId = self.get_list_choice(provinceId, list_or_dict=None, key="provinceId")
+        modelId = self.get_list_choice(modelId, list_or_dict=None, key="modelId")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_manageapi_order_mainorder.manageapi_order_mainorder_pagelist(**_kwargs)
 
         self.assert_manageapi_order_mainorder_pagelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/open/haohan/funs_open_haohan_relation.py` & `huhk-1.9.6/service/app_a/funs/open/haohan/funs_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/open/haohan/funs_open_haohan_rights.py` & `huhk-1.9.6/service/app_a/funs/open/haohan/funs_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/order/funs_order_freeorder.py` & `huhk-1.9.6/service/app_a/funs/order/funs_order_freeorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.order.asserts_order_freeorder import AssertsOrderFreeorder
 from service.app_a.apis.order import apis_order_freeorder
 
 
 class FunsOrderFreeorder(AssertsOrderFreeorder):
     @allure.step(title="导出0元订购预定信息表-Y")
-    def order_freeorder_download(self, avatarUrl="$None$", modelId="$None$", userPolicyCode="$None$", privacyPolicyCode="$None$", provinceName="$None$", cityId="$None$", userName="$None$", regisTimeEnd="$None$", nickName="$None$", freeOrderId="$None$", regisTimeBegin="$None$", mobile="$None$", cityName="$None$", createTime="$None$", channel="$None$", channelName="$None$", provinceId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_freeorder_download(self, regisTimeBegin="$None$", freeOrderId="$None$", avatarUrl="$None$", provinceId="$None$", channelName="$None$", nickName="$None$", channel="$None$", regisTimeEnd="$None$", privacyPolicyCode="$None$", mobile="$None$", userPolicyCode="$None$", cityId="$None$", createTime="$None$", cityName="$None$", userName="$None$", provinceName="$None$", modelId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/freeOrder/downLoad
                 params: freeOrderId : integer : 订单号
                 params: modelId : string : 车型编码
                 params: userName : string : 用户姓名
                 params: mobile : string : 用户号码
                 params: provinceId : string : 省编码
@@ -24,31 +24,31 @@
                 params: regisTimeEnd : string : 结束时间
                 params: nickName : string : 昵称
                 params: avatarUrl : string : 头像
                 params: userPolicyCode : string : 用户协议版本号
                 params: privacyPolicyCode : string : 隐私协议版本号
                 params: headers : 请求头
         """
+        regisTimeBegin = self.get_value_choice(regisTimeBegin, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        freeOrderId = self.get_value_choice(freeOrderId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         avatarUrl = self.get_value_choice(avatarUrl, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        modelId = self.get_value_choice(modelId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        userPolicyCode = self.get_value_choice(userPolicyCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        privacyPolicyCode = self.get_value_choice(privacyPolicyCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        provinceName = self.get_value_choice(provinceName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        cityId = self.get_value_choice(cityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        userName = self.get_value_choice(userName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        regisTimeEnd = self.get_value_choice(regisTimeEnd, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        provinceId = self.get_value_choice(provinceId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        channelName = self.get_value_choice(channelName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         nickName = self.get_value_choice(nickName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        freeOrderId = self.get_value_choice(freeOrderId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        regisTimeBegin = self.get_value_choice(regisTimeBegin, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        channel = self.get_value_choice(channel, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        regisTimeEnd = self.get_value_choice(regisTimeEnd, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        privacyPolicyCode = self.get_value_choice(privacyPolicyCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         mobile = self.get_value_choice(mobile, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        cityName = self.get_value_choice(cityName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        userPolicyCode = self.get_value_choice(userPolicyCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        cityId = self.get_value_choice(cityId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         createTime = self.get_value_choice(createTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        channel = self.get_value_choice(channel, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        channelName = self.get_value_choice(channelName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        provinceId = self.get_value_choice(provinceId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        cityName = self.get_value_choice(cityName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        userName = self.get_value_choice(userName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        provinceName = self.get_value_choice(provinceName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        modelId = self.get_value_choice(modelId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_freeorder.order_freeorder_download(**_kwargs)
 
         self.assert_order_freeorder_download(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/order/funs_order_mainorder.py` & `huhk-1.9.6/service/app_a/funs/order/funs_order_mainorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,52 +3,52 @@
 from service.app_a.asserts.order.asserts_order_mainorder import AssertsOrderMainorder
 from service.app_a.apis.order import apis_order_mainorder
 from service.app_a.funs.order.mainorder.funs_order_mainorder_scrm2app import FunsOrderMainorderScrm2App
 
 
 class FunsOrderMainorder(AssertsOrderMainorder, FunsOrderMainorderScrm2App):
     @allure.step(title="小订订单分页查询（后台）-Y")
-    def order_mainorder_pagelist(self, createEndTime="$None$", createStartTime="$None$", current=1, sortItems="$None$", size=10, _assert=True,  **kwargs):
+    def order_mainorder_pagelist(self, sortItems="$None$", current=1, createEndTime="$None$", createStartTime="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/order/mainOrder/pageList
                 params: current : string :
                 params: size : string :
                 params: sortItems : string : 排序字段（只能是【orderMain.orderType】、【orderMain.createTime】、【orderPay.createTime】）
                 params: createStartTime : string : 订单创建开始日期
                 params: createEndTime : string : 订单创建结束日期
                 params: headers : 请求头
         """
+        sortItems = self.get_list_choice(sortItems, list_or_dict=None, key="sortItems")
         createEndTime = self.get_list_choice(createEndTime, list_or_dict=None, key="createEndTime")
         createStartTime = self.get_list_choice(createStartTime, list_or_dict=None, key="createStartTime")
-        sortItems = self.get_list_choice(sortItems, list_or_dict=None, key="sortItems")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_mainorder.order_mainorder_pagelist(**_kwargs)
 
         self.assert_order_mainorder_pagelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="小订订单列表导出（后台）-Y")
-    def order_mainorder_download(self, createTimeToSort="$None$", orderTypeToSort="$None$", createEndTime="$None$", createStartTime="$None$", payTimeToSort="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_mainorder_download(self, payTimeToSort="$None$", orderTypeToSort="$None$", createTimeToSort="$None$", createEndTime="$None$", createStartTime="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/mainOrder/downLoad
                 params: orderTypeToSort : string : 订单类型排序 不排序不赋值 正序：asc 倒序：desc
                 params: createTimeToSort : string : 订单创建时间 不排序不赋值 正序：asc 倒序：desc
                 params: payTimeToSort : string : 订单创建时间 不排序不赋值 正序：asc 倒序：desc
                 params: createStartTime : string : 订单创建开始日期
                 params: createEndTime : string : 订单创建结束日期
                 params: headers : 请求头
         """
-        createTimeToSort = self.get_value_choice(createTimeToSort, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        payTimeToSort = self.get_value_choice(payTimeToSort, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         orderTypeToSort = self.get_value_choice(orderTypeToSort, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        createTimeToSort = self.get_value_choice(createTimeToSort, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         createEndTime = self.get_value_choice(createEndTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         createStartTime = self.get_value_choice(createStartTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        payTimeToSort = self.get_value_choice(payTimeToSort, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_mainorder.order_mainorder_download(**_kwargs)
 
         self.assert_order_mainorder_download(_assert, **_kwargs)
         self.set_value(_kwargs)
 
@@ -223,15 +223,15 @@
 
         self.assert_order_mainorder_getcarconfigbyorderid(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="SCRM第三方订单同步信息-Y")
-    def order_mainorder_syncscrmextorder(self, soStatus="$None$", scUid="$None$", isArrived="$None$", orderId="$None$", createTime="$None$", trimCode="$None$", deliveryData="$None$", VIN="$None$", customerCtCode="$None$", syncMsg="$None$", chargePointEquity="$None$", unitTaxNo="$None$", dealerCode="$None$", unitName="$None$", orderAllAmount="$None$", phone="$None$", soNo="$None$", colorCode="$None$", syncStatus="$None$", optionCode="$None$", orderNo="$None$", modelCode="$None$", isTestDrive="$None$", customerId="$None$", scUname="$None$", seriesCode="$None$", updateTime="$None$", customerType="$None$", isLifetimeWarranty="$None$", custCertNo="$None$", unitInvoiceTitle="$None$", lifetimeWarrantyPrice="$None$", ossId="$None$", configCode="$None$", potentialName="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_mainorder_syncscrmextorder(self, orderAllAmount="$None$", scUid="$None$", lifetimeWarrantyPrice="$None$", syncMsg="$None$", seriesCode="$None$", orderId="$None$", customerId="$None$", VIN="$None$", isTestDrive="$None$", orderNo="$None$", scUname="$None$", isLifetimeWarranty="$None$", customerType="$None$", syncStatus="$None$", chargePointEquity="$None$", unitTaxNo="$None$", phone="$None$", soStatus="$None$", trimCode="$None$", unitInvoiceTitle="$None$", createTime="$None$", ossId="$None$", potentialName="$None$", unitName="$None$", modelCode="$None$", custCertNo="$None$", customerCtCode="$None$", configCode="$None$", optionCode="$None$", updateTime="$None$", colorCode="$None$", isArrived="$None$", soNo="$None$", deliveryData="$None$", dealerCode="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/mainOrder/syncScrmExtOrder
                 params: ossId : string : 主键
                 params: dealerCode : string : 经销商代码
                 params: customerId : number : 潜客 ID
                 params: isArrived : string : 是否到店（true or false）
                 params: isTestDrive : string : 是否试乘试驾（true or false）
@@ -263,49 +263,49 @@
                 params: lifetimeWarrantyPrice : string : 终身质保价格(保留 2 位小数)
                 params: createTime : string : 创建订单时间
                 params: updateTime : string : 更新订单时间
                 params: syncStatus : integer : 0待同步，1同步成功，2同步失败
                 params: syncMsg : string : 同步结果
                 params: headers : 请求头
         """
-        soStatus = self.get_value_choice(soStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        orderAllAmount = self.get_value_choice(orderAllAmount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         scUid = self.get_value_choice(scUid, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        isArrived = self.get_value_choice(isArrived, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        lifetimeWarrantyPrice = self.get_value_choice(lifetimeWarrantyPrice, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        syncMsg = self.get_value_choice(syncMsg, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        seriesCode = self.get_value_choice(seriesCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         orderId = self.get_value_choice(orderId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        createTime = self.get_value_choice(createTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        trimCode = self.get_value_choice(trimCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        deliveryData = self.get_value_choice(deliveryData, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        customerId = self.get_value_choice(customerId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         VIN = self.get_value_choice(VIN, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        customerCtCode = self.get_value_choice(customerCtCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        syncMsg = self.get_value_choice(syncMsg, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        chargePointEquity = self.get_value_choice(chargePointEquity, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        unitTaxNo = self.get_value_choice(unitTaxNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        dealerCode = self.get_value_choice(dealerCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        unitName = self.get_value_choice(unitName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        orderAllAmount = self.get_value_choice(orderAllAmount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        phone = self.get_value_choice(phone, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        soNo = self.get_value_choice(soNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        colorCode = self.get_value_choice(colorCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        syncStatus = self.get_value_choice(syncStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        optionCode = self.get_value_choice(optionCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        orderNo = self.get_value_choice(orderNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        modelCode = self.get_value_choice(modelCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         isTestDrive = self.get_value_choice(isTestDrive, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        customerId = self.get_value_choice(customerId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        orderNo = self.get_value_choice(orderNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         scUname = self.get_value_choice(scUname, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        seriesCode = self.get_value_choice(seriesCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        updateTime = self.get_value_choice(updateTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        customerType = self.get_value_choice(customerType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         isLifetimeWarranty = self.get_value_choice(isLifetimeWarranty, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        custCertNo = self.get_value_choice(custCertNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        customerType = self.get_value_choice(customerType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        syncStatus = self.get_value_choice(syncStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        chargePointEquity = self.get_value_choice(chargePointEquity, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        unitTaxNo = self.get_value_choice(unitTaxNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        phone = self.get_value_choice(phone, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        soStatus = self.get_value_choice(soStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        trimCode = self.get_value_choice(trimCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         unitInvoiceTitle = self.get_value_choice(unitInvoiceTitle, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        lifetimeWarrantyPrice = self.get_value_choice(lifetimeWarrantyPrice, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        createTime = self.get_value_choice(createTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         ossId = self.get_value_choice(ossId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        configCode = self.get_value_choice(configCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         potentialName = self.get_value_choice(potentialName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        unitName = self.get_value_choice(unitName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        modelCode = self.get_value_choice(modelCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        custCertNo = self.get_value_choice(custCertNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        customerCtCode = self.get_value_choice(customerCtCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        configCode = self.get_value_choice(configCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        optionCode = self.get_value_choice(optionCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        updateTime = self.get_value_choice(updateTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        colorCode = self.get_value_choice(colorCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        isArrived = self.get_value_choice(isArrived, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        soNo = self.get_value_choice(soNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        deliveryData = self.get_value_choice(deliveryData, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        dealerCode = self.get_value_choice(dealerCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_mainorder.order_mainorder_syncscrmextorder(**_kwargs)
 
         self.assert_order_mainorder_syncscrmextorder(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/order/funs_order_order.py` & `huhk-1.9.6/service/app_a/funs/order/funs_order_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from service.app_a.asserts.order.asserts_order_order import AssertsOrderOrder
 from service.app_a.apis.order import apis_order_order
 
 
 class FunsOrderOrder(AssertsOrderOrder):
     @allure.step(title="订单详情")
-    def order_order_orderdetail(self, pageNum=1, pageSize="$None$", userId="$None$", orderId="$None$", orderStatus="$None$", total="$None$", _assert=True,  **kwargs):
+    def order_order_orderdetail(self, pageSize="$None$", total="$None$", orderId="$None$", userId="$None$", orderStatus="$None$", pageNum=1, _assert=True,  **kwargs):
         """
             url=/order/order/orderDetail{orderId}{userId}
                 params: orderId :  : 订单主单Id
                 params: orderStatus : string : 订单状态
                 params: pageSize : number : 每页大小
                 params: pageNum : number : 当前页
                 params: total : number : 总数
                 params: headers : 请求头
         """
         pageSize = self.get_list_choice(pageSize, list_or_dict=None, key="pageSize")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        total = self.get_list_choice(total, list_or_dict=None, key="total")
         orderId = self.get_list_choice(orderId, list_or_dict=None, key="orderId")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
         orderStatus = self.get_list_choice(orderStatus, list_or_dict=None, key="orderStatus")
-        total = self.get_list_choice(total, list_or_dict=None, key="total")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_order.order_order_orderdetail(**_kwargs)
 
         self.assert_order_order_orderdetail(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/order/funs_order_rightsorder.py` & `huhk-1.9.6/service/app_a/funs/order/funs_order_rightsorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,49 +3,49 @@
 from service.app_a.asserts.order.asserts_order_rightsorder import AssertsOrderRightsorder
 from service.app_a.apis.order import apis_order_rightsorder
 from service.app_a.funs.order.rightsorder.funs_order_rightsorder_receive import FunsOrderRightsorderReceive
 
 
 class FunsOrderRightsorder(AssertsOrderRightsorder, FunsOrderRightsorderReceive):
     @allure.step(title="权益订单导出接口-Y")
-    def order_rightsorder_export(self, rightsType="$None$", payDateBegin="$None$", userId="$None$", payDateEnd="$None$", useStatus="$None$", orderMainId="$None$", receiveDateBegin="$None$", receiveDateEnd="$None$", mobile="$None$", rightsOrderId="$None$", _assert=True,  **kwargs):
+    def order_rightsorder_export(self, receiveDateBegin="$None$", receiveDateEnd="$None$", payDateBegin="$None$", mobile="$None$", payDateEnd="$None$", useStatus="$None$", rightsOrderId="$None$", userId="$None$", orderMainId="$None$", rightsType="$None$", _assert=True,  **kwargs):
         """
             url=/order/rightsOrder/export
                 params: mobile :  : 手机号码
                 params: rightsOrderId :  : 权益订单ID
                 params: orderMainId :  : 主订单ID
                 params: useStatus :  : 权益使用状态
                 params: rightsType :  : 权益类型
                 params: receiveDateBegin :  : 权益领取时间 - 开始
                 params: receiveDateEnd :  : 权益领取时间 - 结束
                 params: payDateBegin :  : 权益支付时间 - 开始
                 params: payDateEnd :  : 权益支付时间 - 结束
                 params: headers : 请求头
         """
-        rightsType = self.get_list_choice(rightsType, list_or_dict=None, key="rightsType")
-        payDateBegin = self.get_list_choice(payDateBegin, list_or_dict=None, key="payDateBegin")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        payDateEnd = self.get_list_choice(payDateEnd, list_or_dict=None, key="payDateEnd")
-        useStatus = self.get_list_choice(useStatus, list_or_dict=None, key="useStatus")
-        orderMainId = self.get_list_choice(orderMainId, list_or_dict=None, key="orderMainId")
         receiveDateBegin = self.get_list_choice(receiveDateBegin, list_or_dict=None, key="receiveDateBegin")
         receiveDateEnd = self.get_list_choice(receiveDateEnd, list_or_dict=None, key="receiveDateEnd")
+        payDateBegin = self.get_list_choice(payDateBegin, list_or_dict=None, key="payDateBegin")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        payDateEnd = self.get_list_choice(payDateEnd, list_or_dict=None, key="payDateEnd")
+        useStatus = self.get_list_choice(useStatus, list_or_dict=None, key="useStatus")
         rightsOrderId = self.get_list_choice(rightsOrderId, list_or_dict=None, key="rightsOrderId")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        orderMainId = self.get_list_choice(orderMainId, list_or_dict=None, key="orderMainId")
+        rightsType = self.get_list_choice(rightsType, list_or_dict=None, key="rightsType")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rightsorder.order_rightsorder_export(**_kwargs)
 
         self.assert_order_rightsorder_export(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="权益订单 - 新增-Y")
-    def order_rightsorder_insert(self, refundBillNo="$None$", rightsType="$None$", updateId="$None$", userId="$None$", payAmount="$None$", payDate="$None$", useStatus="$None$", createBy="$None$", rightsName="$None$", orderMainId="$None$", refundDate="$None$", mobile="$None$", receiveDate="$None$", payBillNo="$None$", createTime="$None$", rightsId="$None$", updateTime="$None$", rightsOrderId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_rightsorder_insert(self, payBillNo="$None$", createBy="$None$", payDate="$None$", payAmount="$None$", rightsId="$None$", updateId="$None$", mobile="$None$", updateTime="$None$", refundDate="$None$", useStatus="$None$", refundBillNo="$None$", receiveDate="$None$", createTime="$None$", rightsOrderId="$None$", userId="$None$", orderMainId="$None$", rightsName="$None$", rightsType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/rightsOrder/insert
                 params: rightsOrderId : number : 权益订单ID
                 params: rightsId : number : 权益ID
                 params: rightsType : integer : 权益类型
                 params: rightsName : string : 权益名称
                 params: orderMainId : string : 主订单ID
@@ -59,42 +59,42 @@
                 params: refundBillNo : string : 退款流水
                 params: createTime : string : 创建时间
                 params: createBy : number : 创建人
                 params: updateTime : string : 更新时间
                 params: updateId : number : 更新人id
                 params: headers : 请求头
         """
-        refundBillNo = self.get_value_choice(refundBillNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsType = self.get_value_choice(rightsType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        updateId = self.get_value_choice(updateId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        payAmount = self.get_value_choice(payAmount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        payDate = self.get_value_choice(payDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        useStatus = self.get_value_choice(useStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        payBillNo = self.get_value_choice(payBillNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         createBy = self.get_value_choice(createBy, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        orderMainId = self.get_value_choice(orderMainId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        refundDate = self.get_value_choice(refundDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        payDate = self.get_value_choice(payDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        payAmount = self.get_value_choice(payAmount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsId = self.get_value_choice(rightsId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        updateId = self.get_value_choice(updateId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         mobile = self.get_value_choice(mobile, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        updateTime = self.get_value_choice(updateTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        refundDate = self.get_value_choice(refundDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        useStatus = self.get_value_choice(useStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        refundBillNo = self.get_value_choice(refundBillNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         receiveDate = self.get_value_choice(receiveDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        payBillNo = self.get_value_choice(payBillNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         createTime = self.get_value_choice(createTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsId = self.get_value_choice(rightsId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        updateTime = self.get_value_choice(updateTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         rightsOrderId = self.get_value_choice(rightsOrderId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        orderMainId = self.get_value_choice(orderMainId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsType = self.get_value_choice(rightsType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rightsorder.order_rightsorder_insert(**_kwargs)
 
         self.assert_order_rightsorder_insert(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="权益订单 - 分页查询-Y")
-    def order_rightsorder_page(self, rightsType="$None$", payDateBegin="$None$", userId="$None$", payDateEnd="$None$", useStatus="$None$", orderMainId="$None$", receiveDateBegin="$None$", receiveDateEnd="$None$", mobile="$None$", current=1, size=10, rightsOrderId="$None$", _assert=True,  **kwargs):
+    def order_rightsorder_page(self, receiveDateBegin="$None$", current=1, receiveDateEnd="$None$", payDateBegin="$None$", mobile="$None$", payDateEnd="$None$", useStatus="$None$", rightsOrderId="$None$", userId="$None$", size=10, orderMainId="$None$", rightsType="$None$", _assert=True,  **kwargs):
         """
             url=/order/rightsOrder/page
                 params: size :  :
                 params: current :  :
                 params: mobile :  : 手机号码
                 params: rightsOrderId :  : 权益订单ID
                 params: orderMainId :  : 主订单ID
@@ -102,71 +102,71 @@
                 params: rightsType :  : 权益类型
                 params: receiveDateBegin :  : 权益领取时间 开始
                 params: receiveDateEnd :  : 权益领取时间-结束
                 params: payDateBegin :  : 权益支付时间 - 开始
                 params: payDateEnd :  : 权益支付时间 - 结束
                 params: headers : 请求头
         """
-        rightsType = self.get_list_choice(rightsType, list_or_dict=None, key="rightsType")
-        payDateBegin = self.get_list_choice(payDateBegin, list_or_dict=None, key="payDateBegin")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        payDateEnd = self.get_list_choice(payDateEnd, list_or_dict=None, key="payDateEnd")
-        useStatus = self.get_list_choice(useStatus, list_or_dict=None, key="useStatus")
-        orderMainId = self.get_list_choice(orderMainId, list_or_dict=None, key="orderMainId")
         receiveDateBegin = self.get_list_choice(receiveDateBegin, list_or_dict=None, key="receiveDateBegin")
         receiveDateEnd = self.get_list_choice(receiveDateEnd, list_or_dict=None, key="receiveDateEnd")
+        payDateBegin = self.get_list_choice(payDateBegin, list_or_dict=None, key="payDateBegin")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        payDateEnd = self.get_list_choice(payDateEnd, list_or_dict=None, key="payDateEnd")
+        useStatus = self.get_list_choice(useStatus, list_or_dict=None, key="useStatus")
         rightsOrderId = self.get_list_choice(rightsOrderId, list_or_dict=None, key="rightsOrderId")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        orderMainId = self.get_list_choice(orderMainId, list_or_dict=None, key="orderMainId")
+        rightsType = self.get_list_choice(rightsType, list_or_dict=None, key="rightsType")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rightsorder.order_rightsorder_page(**_kwargs)
 
         self.assert_order_rightsorder_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="权益-领取权益-Y")
-    def order_rightsorder_receive(self, rightsId="$None$", orderId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_rightsorder_receive(self, orderId="$None$", rightsId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/rightsOrder/receive
                 params: orderId : string : 子订单ID
                 params: rightsId : number : 权益ID
                 params: headers : 请求头
         """
-        rightsId = self.get_value_choice(rightsId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         orderId = self.get_value_choice(orderId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsId = self.get_value_choice(rightsId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rightsorder.order_rightsorder_receive(**_kwargs)
 
         self.assert_order_rightsorder_receive(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="权益订单 - 查询-Y")
-    def order_rightsorder_getorderlist(self, rightsType="$None$", useStatusList="$None$", orderMainId="$None$", rightsNameList="$None$", mobile="$None$", receiveDate="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_rightsorder_getorderlist(self, mobile="$None$", useStatusList="$None$", receiveDate="$None$", rightsNameList="$None$", orderMainId="$None$", rightsType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/rightsOrder/getOrderList
                 params: orderMainId : number : 主订单ID
                 params: rightsType : integer : 权益类型
                 params: rightsNameList : array : 权益名称
                 type : string : None
                 params: useStatusList : array : 权益使用状态
                 type : integer : None
                 params: mobile : string : 用户手机号
                 params: receiveDate : string : 权益领取时间
                 params: headers : 请求头
         """
-        rightsType = self.get_value_choice(rightsType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        useStatusList = self.get_value_choice(useStatusList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        orderMainId = self.get_value_choice(orderMainId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsNameList = self.get_value_choice(rightsNameList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         mobile = self.get_value_choice(mobile, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        useStatusList = self.get_value_choice(useStatusList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         receiveDate = self.get_value_choice(receiveDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsNameList = self.get_value_choice(rightsNameList, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        orderMainId = self.get_value_choice(orderMainId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsType = self.get_value_choice(rightsType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rightsorder.order_rightsorder_getorderlist(**_kwargs)
 
         self.assert_order_rightsorder_getorderlist(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/order/funs_order_testdrive.py` & `huhk-1.9.6/service/app_a/funs/order/funs_order_testdrive.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,56 +2,56 @@
 
 from service.app_a.asserts.order.asserts_order_testdrive import AssertsOrderTestdrive
 from service.app_a.apis.order import apis_order_testdrive
 
 
 class FunsOrderTestdrive(AssertsOrderTestdrive):
     @allure.step(title="导出试驾表单-Y")
-    def order_testdrive_exportlist(self, startTime="$None$", endTime="$None$", id="$None$", createByName="$None$", shopName="$None$", phoneNumber="$None$", createTime="$None$", channel="$None$", _assert=True,  **kwargs):
+    def order_testdrive_exportlist(self, phoneNumber="$None$", createByName="$None$", channel="$None$", shopName="$None$", endTime="$None$", startTime="$None$", createTime="$None$", id="$None$", _assert=True,  **kwargs):
         """
             url=/order/testDrive/exportList
                 params: phoneNumber :  : 手机号
                 params: createByName :  :
                 params: id :  : 主键
                 params: channel :  : 渠道(1:移动应用 2:小程序 3:官方网站)
                 params: startTime :  :
                 params: endTime :  :
                 params: shopName :  : 门店名称
                 params: createTime :  : 创建时间
                 params: headers : 请求头
         """
-        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
-        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
-        id = self.get_list_choice(id, list_or_dict=None, key="id")
+        phoneNumber = self.get_list_choice(phoneNumber, list_or_dict=None, key="phoneNumber")
         createByName = self.get_list_choice(createByName, list_or_dict=None, key="createByName")
+        channel = self.get_list_choice(channel, list_or_dict=None, key="channel")
         shopName = self.get_list_choice(shopName, list_or_dict=None, key="shopName")
-        phoneNumber = self.get_list_choice(phoneNumber, list_or_dict=None, key="phoneNumber")
+        endTime = self.get_list_choice(endTime, list_or_dict=None, key="endTime")
+        startTime = self.get_list_choice(startTime, list_or_dict=None, key="startTime")
         createTime = self.get_list_choice(createTime, list_or_dict=None, key="createTime")
-        channel = self.get_list_choice(channel, list_or_dict=None, key="channel")
+        id = self.get_list_choice(id, list_or_dict=None, key="id")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_testdrive.order_testdrive_exportlist(**_kwargs)
 
         self.assert_order_testdrive_exportlist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户中心-预约信息")
-    def order_testdrive_userlist(self, createBy="$None$", modelId="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def order_testdrive_userlist(self, modelId="$None$", createBy="$None$", size=10, current=1, _assert=True,  **kwargs):
         """
             url=/order/testDrive/userList
                 params: current :  : 当前页数
                 params: size :  : 每页数据数
                 params: createBy :  :
                 params: modelId :  :
                 params: headers : 请求头
         """
-        createBy = self.get_list_choice(createBy, list_or_dict=None, key="createBy")
         modelId = self.get_list_choice(modelId, list_or_dict=None, key="modelId")
+        createBy = self.get_list_choice(createBy, list_or_dict=None, key="createBy")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_testdrive.order_testdrive_userlist(**_kwargs)
 
         self.assert_order_testdrive_userlist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/order/mainorder/funs_order_mainorder_scrm2app.py` & `huhk-1.9.6/service/app_a/funs/order/mainorder/funs_order_mainorder_scrm2app.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from service.app_a.asserts.order.mainorder.asserts_order_mainorder_scrm2app import AssertsOrderMainorderScrm2App
 from service.app_a.apis.order.mainorder import apis_order_mainorder_scrm2app
 
 
 class FunsOrderMainorderScrm2App(AssertsOrderMainorderScrm2App):
     @allure.step(title="订单管理-订单退款-Y")
-    def order_mainorder_scrm2app_refundauditnotice(self, orderMainId="$None$", status="$None$", orderSubId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_mainorder_scrm2app_refundauditnotice(self, orderSubId="$None$", status="$None$", orderMainId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/mainOrder/scrm2app/refundAuditNotice
                 params: orderMainId : string :
                 params: orderSubId : string :
                 params: status : integer :
                 params: headers : 请求头
         """
-        orderMainId = self.get_value_choice(orderMainId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         orderSubId = self.get_value_choice(orderSubId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        orderMainId = self.get_value_choice(orderMainId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_mainorder_scrm2app.order_mainorder_scrm2app_refundauditnotice(**_kwargs)
 
         self.assert_order_mainorder_scrm2app_refundauditnotice(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/order/rights/funs_order_rights_rightsmanager.py` & `huhk-1.9.6/service/app_a/funs/order/rights/funs_order_rights_rightsmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,104 +33,104 @@
 
         self.assert_order_rights_rightsmanager_getrelation(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="权益 - 分页查询-Y")
-    def order_rights_rightsmanager_page(self, status="$None$", modelCode="$None$", effectiveEndDate="$None$", rightsName="$None$", current=1, size=10, _assert=True,  **kwargs):
+    def order_rights_rightsmanager_page(self, effectiveEndDate="$None$", modelCode="$None$", current=1, status="$None$", size=10, rightsName="$None$", _assert=True,  **kwargs):
         """
             url=/order/rights/rightsManager/page
                 params: size :  :
                 params: current :  :
                 params: rightsName :  :
                 params: status :  :
                 params: modelCode :  :
                 params: effectiveEndDate :  :
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
-        modelCode = self.get_list_choice(modelCode, list_or_dict=None, key="modelCode")
         effectiveEndDate = self.get_list_choice(effectiveEndDate, list_or_dict=None, key="effectiveEndDate")
+        modelCode = self.get_list_choice(modelCode, list_or_dict=None, key="modelCode")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
         rightsName = self.get_list_choice(rightsName, list_or_dict=None, key="rightsName")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rights_rightsmanager.order_rights_rightsmanager_page(**_kwargs)
 
         self.assert_order_rights_rightsmanager_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="权益订单 - 查询-Y")
-    def order_rights_rightsmanager_getrightslist(self, rightsName="$None$", status="$None$", modelId="$None$", effectiveStartDate="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_rights_rightsmanager_getrightslist(self, effectiveStartDate="$None$", status="$None$", rightsName="$None$", modelId="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/rights/rightsManager/getRightsList
                 params: rightsName : string : 权益名称
                 params: status : integer : 权益状态(0未生效，1已生效)
                 params: modelId : string : 车型代码
                 params: effectiveStartDate : string : 权益生效时间
                 params: headers : 请求头
         """
-        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        effectiveStartDate = self.get_value_choice(effectiveStartDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         status = self.get_value_choice(status, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         modelId = self.get_value_choice(modelId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        effectiveStartDate = self.get_value_choice(effectiveStartDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rights_rightsmanager.order_rights_rightsmanager_getrightslist(**_kwargs)
 
         self.assert_order_rights_rightsmanager_getrightslist(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="权益-新增权益-Y")
-    def order_rights_rightsmanager_insert(self, modelCode="$None$", rightsType="$None$", rightsName="$None$", orderType="$None$", effectiveStartDate="$None$", rightsId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_rights_rightsmanager_insert(self, modelCode="$None$", rightsId="$None$", effectiveStartDate="$None$", orderType="$None$", rightsName="$None$", rightsType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/rights/rightsManager/insert
                 params: effectiveStartDate : text : 权益生效时间 -- 开始
                 params: rightsId : text : 权益ID
                 params: rightsName : text : 权益名称
                 params: rightsType : text : 权益类型
                 params: modelCode : text : 车型代码
                 params: orderType : text : 关联订单类型code
                 params: headers : 请求头
         """
         modelCode = self.get_value_choice(modelCode, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsType = self.get_value_choice(rightsType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        orderType = self.get_value_choice(orderType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        effectiveStartDate = self.get_value_choice(effectiveStartDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         rightsId = self.get_value_choice(rightsId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        effectiveStartDate = self.get_value_choice(effectiveStartDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        orderType = self.get_value_choice(orderType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsType = self.get_value_choice(rightsType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rights_rightsmanager.order_rights_rightsmanager_insert(**_kwargs)
 
         self.assert_order_rights_rightsmanager_insert(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="权益-修改权益-Y")
-    def order_rights_rightsmanager_update(self, effectiveEndDate="$None$", rightsName="$None$", Relation="$None$", effectiveStartDate="$None$", rightsId="$None$", Content="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_rights_rightsmanager_update(self, effectiveEndDate="$None$", Relation="$None$", rightsId="$None$", effectiveStartDate="$None$", Content="$None$", rightsName="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/rights/rightsManager/update
                 params: rightsName : string : 权益名称
                 params: rightsId : string : 权益主键
                 params: Content : string : 权益描述
                 params: effectiveStartDate : string : 权益生效时间
                 params: effectiveEndDate : string : 权益生效时间-结束
                 params: Relation : string : 互斥关系
                 params: headers : 请求头
         """
         effectiveEndDate = self.get_value_choice(effectiveEndDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         Relation = self.get_value_choice(Relation, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        effectiveStartDate = self.get_value_choice(effectiveStartDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         rightsId = self.get_value_choice(rightsId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        effectiveStartDate = self.get_value_choice(effectiveStartDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         Content = self.get_value_choice(Content, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rights_rightsmanager.order_rights_rightsmanager_update(**_kwargs)
 
         self.assert_order_rights_rightsmanager_update(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/order/rightsorder/funs_order_rightsorder_receive.py` & `huhk-1.9.6/service/app_a/funs/order/rightsorder/funs_order_rightsorder_receive.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.order.rightsorder.asserts_order_rightsorder_receive import AssertsOrderRightsorderReceive
 from service.app_a.apis.order.rightsorder import apis_order_rightsorder_receive
 
 
 class FunsOrderRightsorderReceive(AssertsOrderRightsorderReceive):
     @allure.step(title="权益-编辑权益订单-Y")
-    def order_rightsorder_receive_update(self, refundBillNo="$None$", rightsType="$None$", updateId="$None$", userId="$None$", payAmount="$None$", payDate="$None$", useStatus="$None$", createBy="$None$", rightsName="$None$", orderMainId="$None$", refundDate="$None$", mobile="$None$", receiveDate="$None$", payBillNo="$None$", createTime="$None$", rightsId="$None$", updateTime="$None$", rightsOrderId="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def order_rightsorder_receive_update(self, payBillNo="$None$", createBy="$None$", payDate="$None$", payAmount="$None$", rightsId="$None$", updateId="$None$", mobile="$None$", updateTime="$None$", refundDate="$None$", useStatus="$None$", refundBillNo="$None$", receiveDate="$None$", createTime="$None$", rightsOrderId="$None$", userId="$None$", orderMainId="$None$", rightsName="$None$", rightsType="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/order/rightsOrder/receive/update
                 params: rightsOrderId : string :
                 params: rightsId : string :
                 params: rightsType : string :
                 params: rightsName : string :
                 params: orderMainId : string :
@@ -24,32 +24,32 @@
                 params: refundBillNo : string :
                 params: createTime : string :
                 params: createBy : string :
                 params: updateTime : string :
                 params: updateId : string :
                 params: headers : 请求头
         """
-        refundBillNo = self.get_value_choice(refundBillNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsType = self.get_value_choice(rightsType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        updateId = self.get_value_choice(updateId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        payAmount = self.get_value_choice(payAmount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        payDate = self.get_value_choice(payDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        useStatus = self.get_value_choice(useStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        payBillNo = self.get_value_choice(payBillNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         createBy = self.get_value_choice(createBy, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        orderMainId = self.get_value_choice(orderMainId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        refundDate = self.get_value_choice(refundDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        payDate = self.get_value_choice(payDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        payAmount = self.get_value_choice(payAmount, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsId = self.get_value_choice(rightsId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        updateId = self.get_value_choice(updateId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         mobile = self.get_value_choice(mobile, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        updateTime = self.get_value_choice(updateTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        refundDate = self.get_value_choice(refundDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        useStatus = self.get_value_choice(useStatus, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        refundBillNo = self.get_value_choice(refundBillNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         receiveDate = self.get_value_choice(receiveDate, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        payBillNo = self.get_value_choice(payBillNo, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         createTime = self.get_value_choice(createTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rightsId = self.get_value_choice(rightsId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        updateTime = self.get_value_choice(updateTime, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         rightsOrderId = self.get_value_choice(rightsOrderId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        orderMainId = self.get_value_choice(orderMainId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsName = self.get_value_choice(rightsName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rightsType = self.get_value_choice(rightsType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_order_rightsorder_receive.order_rightsorder_receive_update(**_kwargs)
 
         self.assert_order_rightsorder_receive_update(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/pay/funs_pay_orderpaybill.py` & `huhk-1.9.6/service/app_a/funs/pay/funs_pay_orderpaybill.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_batch.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 
 from service.app_a.asserts.radarpoints.adjustpoints.adjust.asserts_radarpoints_adjustpoints_adjust_batch import AssertsRadarpointsAdjustpointsAdjustBatch
 from service.app_a.apis.radarpoints.adjustpoints.adjust import apis_radarpoints_adjustpoints_adjust_batch
 
 
 class FunsRadarpointsAdjustpointsAdjustBatch(AssertsRadarpointsAdjustpointsAdjustBatch):
     @allure.step(title="积分调整 - 批量调整")
-    def radarpoints_adjustpoints_adjust_batch_save(self, optAbility="$None$", optAbilityName="$None$", adjustNotes="$None$", redisKey="$None$", clientNotes="$None$", file="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def radarpoints_adjustpoints_adjust_batch_save(self, clientNotes="$None$", file="$None$", optAbilityName="$None$", redisKey="$None$", adjustNotes="$None$", optAbility="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/radarpoints/adjustPoints/adjust/batch/save
                 params: file : file : 导入excel文件
                 params: optAbility : text : 调整方式
                 params: adjustNotes : text : 调整原因说明
                 params: clientNotes : text : 用户端展示
                 params: optAbilityName : string : 调整方式枚举
                 params: redisKey : string : 缓存键
                 params: headers : 请求头
         """
-        optAbility = self.get_value_choice(optAbility, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        optAbilityName = self.get_value_choice(optAbilityName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        adjustNotes = self.get_value_choice(adjustNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        redisKey = self.get_value_choice(redisKey, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         clientNotes = self.get_value_choice(clientNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         file = self.get_value_choice(file, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        optAbilityName = self.get_value_choice(optAbilityName, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        redisKey = self.get_value_choice(redisKey, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        adjustNotes = self.get_value_choice(adjustNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        optAbility = self.get_value_choice(optAbility, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_adjustpoints_adjust_batch.radarpoints_adjustpoints_adjust_batch_save(**_kwargs)
 
         self.assert_radarpoints_adjustpoints_adjust_batch_save(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="积分调整 - 批量调整 - 导入excel")
-    def radarpoints_adjustpoints_adjust_batch_import(self, file="$None$", field_34="$None$", adjustNotes="$None$", list="$None$", clientNotes="$None$", field_35="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def radarpoints_adjustpoints_adjust_batch_import(self, list="$None$", field_35="$None$", field_34="$None$", clientNotes="$None$", file="$None$", adjustNotes="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/radarpoints/adjustPoints/adjust/batch/import
                 params: file : file : excel文件
                 params: adjustNotes : string : 调整原因说明
                 params: clientNotes : string : 客户端显示信息
                 params: list : array : 成功数据集
                 userId : number : 用户id
@@ -44,20 +44,20 @@
                 adjustNumber : number : 调整数值
                 pointsDepartment : number : 积分归属部门
                 DateType : number : 生效时间类型
                 params: field_35 : string :
                 params: field_34 : string :
                 params: headers : 请求头
         """
-        file = self.get_value_choice(file, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        field_34 = self.get_value_choice(field_34, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        adjustNotes = self.get_value_choice(adjustNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         list = self.get_value_choice(list, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        clientNotes = self.get_value_choice(clientNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         field_35 = self.get_value_choice(field_35, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        field_34 = self.get_value_choice(field_34, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        clientNotes = self.get_value_choice(clientNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        file = self.get_value_choice(file, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        adjustNotes = self.get_value_choice(adjustNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_adjustpoints_adjust_batch.radarpoints_adjustpoints_adjust_batch_import(**_kwargs)
 
         self.assert_radarpoints_adjustpoints_adjust_batch_import(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_single.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_single.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from service.app_a.asserts.radarpoints.adjustpoints.adjust.asserts_radarpoints_adjustpoints_adjust_single import AssertsRadarpointsAdjustpointsAdjustSingle
 from service.app_a.apis.radarpoints.adjustpoints.adjust import apis_radarpoints_adjustpoints_adjust_single
 
 
 class FunsRadarpointsAdjustpointsAdjustSingle(AssertsRadarpointsAdjustpointsAdjustSingle):
     @allure.step(title="积分调整 - 单次调整")
-    def radarpoints_adjustpoints_adjust_single_save(self, userId="$None$", optAbility="$None$", pointsExpiration="$None$", adjustNotes="$None$", clientNotes="$None$", qty="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def radarpoints_adjustpoints_adjust_single_save(self, pointsExpiration="$None$", qty="$None$", clientNotes="$None$", adjustNotes="$None$", userId="$None$", optAbility="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/radarpoints/adjustPoints/adjust/single/save
                 params: optAbility : number : 积分调整类型
                 params: adjustNotes : string : 调整原因说明
                 params: clientNotes : string : 户端展示信息
                 params: qty : number : 调整数值
                 params: pointsExpiration : number : 积分有效期类型（新增时赋值）
                 params: headers : 请求头
         """
-        userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        optAbility = self.get_value_choice(optAbility, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         pointsExpiration = self.get_value_choice(pointsExpiration, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        adjustNotes = self.get_value_choice(adjustNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        clientNotes = self.get_value_choice(clientNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         qty = self.get_value_choice(qty, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        clientNotes = self.get_value_choice(clientNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        adjustNotes = self.get_value_choice(adjustNotes, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        userId = self.get_value_choice(userId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        optAbility = self.get_value_choice(optAbility, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_adjustpoints_adjust_single.radarpoints_adjustpoints_adjust_single_save(**_kwargs)
 
         self.assert_radarpoints_adjustpoints_adjust_single_save(_assert, **_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_adjustpoints.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_adjustpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 from service.app_a.asserts.radarpoints.asserts_radarpoints_adjustpoints import AssertsRadarpointsAdjustpoints
 from service.app_a.apis.radarpoints import apis_radarpoints_adjustpoints
 from service.app_a.funs.radarpoints.adjustpoints.funs_radarpoints_adjustpoints_adjust import FunsRadarpointsAdjustpointsAdjust
 
 
 class FunsRadarpointsAdjustpoints(AssertsRadarpointsAdjustpoints, FunsRadarpointsAdjustpointsAdjust):
     @allure.step(title="积分调整 - 分页查询")
-    def radarpoints_adjustpoints_pagelist(self, adjustTimeEnd="$None$", userId="$None$", optAbility="$None$", optAbilityName="$None$", adjustTimeBefore="$None$", nickName="$None$", adjustNotes="$None$", mobile="$None$", current=1, size=10, _assert=True,  **kwargs):
+    def radarpoints_adjustpoints_pagelist(self, adjustTimeBefore="$None$", current=1, adjustTimeEnd="$None$", mobile="$None$", optAbilityName="$None$", size=10, adjustNotes="$None$", userId="$None$", nickName="$None$", optAbility="$None$", _assert=True,  **kwargs):
         """
             url=/radarpoints/adjustPoints/pageList
                 params: nickName :  : 用户名
                 params: mobile :  : 手机号
                 params: adjustNotes :  : 调整原因说明
                 params: optAbility :  : 调整积分方式
                 params: optAbilityName :  : 调整积分方式枚举
                 params: adjustTimeBefore :  : 调整时间 - 开始
                 params: adjustTimeEnd :  : 调整时间 - 结束
                 params: current :  : 页码
                 params: size :  : 每页大小
                 params: headers : 请求头
         """
+        adjustTimeBefore = self.get_list_choice(adjustTimeBefore, list_or_dict=None, key="adjustTimeBefore")
         adjustTimeEnd = self.get_list_choice(adjustTimeEnd, list_or_dict=None, key="adjustTimeEnd")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        optAbility = self.get_list_choice(optAbility, list_or_dict=None, key="optAbility")
+        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
         optAbilityName = self.get_list_choice(optAbilityName, list_or_dict=None, key="optAbilityName")
-        adjustTimeBefore = self.get_list_choice(adjustTimeBefore, list_or_dict=None, key="adjustTimeBefore")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
         adjustNotes = self.get_list_choice(adjustNotes, list_or_dict=None, key="adjustNotes")
-        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        optAbility = self.get_list_choice(optAbility, list_or_dict=None, key="optAbility")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_adjustpoints.radarpoints_adjustpoints_pagelist(**_kwargs)
 
         self.assert_radarpoints_adjustpoints_pagelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
@@ -68,36 +68,36 @@
 
         self.assert_radarpoints_adjustpoints_getuserpointsqtybymobile(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="积分调整 - 导出excel")
-    def radarpoints_adjustpoints_export(self, adjustTimeEnd="$None$", userId="$None$", optAbility="$None$", optAbilityName="$None$", adjustTimeBefore="$None$", nickName="$None$", adjustNotes="$None$", mobile="$None$", current=1, size=10, _assert=True,  **kwargs):
+    def radarpoints_adjustpoints_export(self, adjustTimeBefore="$None$", current=1, adjustTimeEnd="$None$", mobile="$None$", optAbilityName="$None$", size=10, adjustNotes="$None$", userId="$None$", nickName="$None$", optAbility="$None$", _assert=True,  **kwargs):
         """
             url=/radarpoints/adjustPoints/export
                 params: nickName :  : 用户名
                 params: mobile :  : 手机号
                 params: adjustNotes :  : 调整原因说明
                 params: optAbility :  : 调整积分方式
                 params: optAbilityName :  : 调整积分方式枚举
                 params: adjustTimeBefore :  : 调整时间 - 开始
                 params: adjustTimeEnd :  : 调整时间 - 结束
                 params: current :  : 页码
                 params: size :  : 每页大小
                 params: headers : 请求头
         """
+        adjustTimeBefore = self.get_list_choice(adjustTimeBefore, list_or_dict=None, key="adjustTimeBefore")
         adjustTimeEnd = self.get_list_choice(adjustTimeEnd, list_or_dict=None, key="adjustTimeEnd")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        optAbility = self.get_list_choice(optAbility, list_or_dict=None, key="optAbility")
+        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
         optAbilityName = self.get_list_choice(optAbilityName, list_or_dict=None, key="optAbilityName")
-        adjustTimeBefore = self.get_list_choice(adjustTimeBefore, list_or_dict=None, key="adjustTimeBefore")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
         adjustNotes = self.get_list_choice(adjustNotes, list_or_dict=None, key="adjustNotes")
-        mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        optAbility = self.get_list_choice(optAbility, list_or_dict=None, key="optAbility")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_adjustpoints.radarpoints_adjustpoints_export(**_kwargs)
 
         self.assert_radarpoints_adjustpoints_export(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_pointsconfig.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_pointsconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,79 +2,79 @@
 
 from service.app_a.asserts.radarpoints.asserts_radarpoints_pointsconfig import AssertsRadarpointsPointsconfig
 from service.app_a.apis.radarpoints import apis_radarpoints_pointsconfig
 
 
 class FunsRadarpointsPointsconfig(AssertsRadarpointsPointsconfig):
     @allure.step(title="积分配置 - 分页查询")
-    def radarpoints_pointsconfig_page(self, pointsBegin="$None$", status="$None$", size=10, pointsExpiration="$None$", businessSceneType="$None$", Current="$None$", pointsEnd="$None$", code="$None$", name="$None$", _assert=True,  **kwargs):
+    def radarpoints_pointsconfig_page(self, pointsExpiration="$None$", code="$None$", name="$None$", businessSceneType="$None$", pointsEnd="$None$", status="$None$", Current="$None$", size=10, pointsBegin="$None$", _assert=True,  **kwargs):
         """
             url=/radarpoints/PointsConfig/page
                 params: code :  : 积分项Code
                 params: name :  : 积分项名称
                 params: businessSceneType :  : 发放场景类型
                 params: pointsBegin :  : 积分值 - 开始区间
                 params: pointsEnd :  : 积分值 - 结束区间
                 params: pointsExpiration :  : 积分有效期
                 params: status :  : 生效状态（0未生效，1已生效）
                 params: Current :  : 当前页
                 params: size :  : 每页大小
                 params: headers : 请求头
         """
-        pointsBegin = self.get_list_choice(pointsBegin, list_or_dict=None, key="pointsBegin")
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
         pointsExpiration = self.get_list_choice(pointsExpiration, list_or_dict=None, key="pointsExpiration")
-        businessSceneType = self.get_list_choice(businessSceneType, list_or_dict=None, key="businessSceneType")
-        Current = self.get_list_choice(Current, list_or_dict=None, key="Current")
-        pointsEnd = self.get_list_choice(pointsEnd, list_or_dict=None, key="pointsEnd")
         code = self.get_list_choice(code, list_or_dict=None, key="code")
         name = self.get_list_choice(name, list_or_dict=None, key="name")
+        businessSceneType = self.get_list_choice(businessSceneType, list_or_dict=None, key="businessSceneType")
+        pointsEnd = self.get_list_choice(pointsEnd, list_or_dict=None, key="pointsEnd")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
+        Current = self.get_list_choice(Current, list_or_dict=None, key="Current")
+        pointsBegin = self.get_list_choice(pointsBegin, list_or_dict=None, key="pointsBegin")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_pointsconfig.radarpoints_pointsconfig_page(**_kwargs)
 
         self.assert_radarpoints_pointsconfig_page(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="积分配置 -新增积分配置")
-    def radarpoints_pointsconfig_insert(self, remark="$None$", pointsExpiration="$None$", points="$None$", bpmId="$None$", businessSceneType="$None$", userPointsDayMax="$None$", rulesPointsDayMax="$None$", toast="$None$", name="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def radarpoints_pointsconfig_insert(self, pointsExpiration="$None$", remark="$None$", userPointsDayMax="$None$", name="$None$", toast="$None$", businessSceneType="$None$", bpmId="$None$", rulesPointsDayMax="$None$", points="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/radarpoints/PointsConfig/insert
                 params: pointsExpiration : string : 积分有效期
                 params: remark : string : 备注
                 params: points : integer : 积分值
                 params: toast : string : toast内容
                 params: name : string : 积分项名称
                 params: businessSceneType : integer : 发放场景类型
                 params: bpmId : integer : bpm单号
                 params: userPointsDayMax : integer : 单用户单日上限
                 params: rulesPointsDayMax : integer : 单日上限
                 params: headers : 请求头
         """
-        remark = self.get_value_choice(remark, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         pointsExpiration = self.get_value_choice(pointsExpiration, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        points = self.get_value_choice(points, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        bpmId = self.get_value_choice(bpmId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        businessSceneType = self.get_value_choice(businessSceneType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        remark = self.get_value_choice(remark, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         userPointsDayMax = self.get_value_choice(userPointsDayMax, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        rulesPointsDayMax = self.get_value_choice(rulesPointsDayMax, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        toast = self.get_value_choice(toast, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         name = self.get_value_choice(name, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        toast = self.get_value_choice(toast, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        businessSceneType = self.get_value_choice(businessSceneType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        bpmId = self.get_value_choice(bpmId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        rulesPointsDayMax = self.get_value_choice(rulesPointsDayMax, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        points = self.get_value_choice(points, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_pointsconfig.radarpoints_pointsconfig_insert(**_kwargs)
 
         self.assert_radarpoints_pointsconfig_insert(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="积分配置 -修改积分配置")
-    def radarpoints_pointsconfig_update(self, remark="$None$", pointsExpiration="$None$", points="$None$", userPointsDayMax="$None$", businessSceneType="$None$", id="$None$", bpmId="$None$", rulesPointsDayMax="$None$", toast="$None$", code="$None$", name="$None$", _assert=True, _all_is_None=False,  **kwargs):
+    def radarpoints_pointsconfig_update(self, pointsExpiration="$None$", remark="$None$", userPointsDayMax="$None$", code="$None$", name="$None$", toast="$None$", businessSceneType="$None$", bpmId="$None$", rulesPointsDayMax="$None$", points="$None$", id="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/radarpoints/PointsConfig/update
                 params: pointsExpiration : string : 积分有效期
                 params: remark : string : 备注
                 params: points : integer : 积分值
                 params: toast : string : toast内容
                 params: name : string : 积分项名称
@@ -82,43 +82,43 @@
                 params: id : integer : 积分项id
                 params: code : string : 积分项code
                 params: rulesPointsDayMax : integer : 单日上限
                 params: userPointsDayMax : integer : 单用户单日上限
                 params: bpmId : integer : bpm单号
                 params: headers : 请求头
         """
-        remark = self.get_value_choice(remark, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         pointsExpiration = self.get_value_choice(pointsExpiration, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        points = self.get_value_choice(points, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        remark = self.get_value_choice(remark, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         userPointsDayMax = self.get_value_choice(userPointsDayMax, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        code = self.get_value_choice(code, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        name = self.get_value_choice(name, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        toast = self.get_value_choice(toast, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         businessSceneType = self.get_value_choice(businessSceneType, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        id = self.get_value_choice(id, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         bpmId = self.get_value_choice(bpmId, list_or_dict=None, key=None, _all_is_None=_all_is_None)
         rulesPointsDayMax = self.get_value_choice(rulesPointsDayMax, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        toast = self.get_value_choice(toast, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        code = self.get_value_choice(code, list_or_dict=None, key=None, _all_is_None=_all_is_None)
-        name = self.get_value_choice(name, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        points = self.get_value_choice(points, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+        id = self.get_value_choice(id, list_or_dict=None, key=None, _all_is_None=_all_is_None)
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_pointsconfig.radarpoints_pointsconfig_update(**_kwargs)
 
         self.assert_radarpoints_pointsconfig_update(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="积分配置 -生效状态变更")
-    def radarpoints_pointsconfig_updatestatusbyid(self, status="$None$", id="$None$", _assert=True,  **kwargs):
+    def radarpoints_pointsconfig_updatestatusbyid(self, id="$None$", status="$None$", _assert=True,  **kwargs):
         """
             url=/radarpoints/PointsConfig/updateStatusById
                 params: id :  : 积分id
                 params: status :  : 生效状态（0未生效，1已生效）
                 params: headers : 请求头
         """
-        status = self.get_list_choice(status, list_or_dict=None, key="status")
         id = self.get_list_choice(id, list_or_dict=None, key="id")
+        status = self.get_list_choice(status, list_or_dict=None, key="status")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_pointsconfig.radarpoints_pointsconfig_updatestatusbyid(**_kwargs)
 
         self.assert_radarpoints_pointsconfig_updatestatusbyid(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_pointstask.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_pointstask.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,64 +2,64 @@
 
 from service.app_a.asserts.radarpoints.asserts_radarpoints_pointstask import AssertsRadarpointsPointstask
 from service.app_a.apis.radarpoints import apis_radarpoints_pointstask
 
 
 class FunsRadarpointsPointstask(AssertsRadarpointsPointstask):
     @allure.step(title="积分任务 - 分页查询")
-    def radarpoints_pointstask_pagelist(self, size=10, dateLast="$None$", pointsConfigCode="$None$", pointsTaskDateSort="$None$", pointsConfigName="$None$", dateBegin="$None$", mobile="$None$", current=1, getPointsQtySort="$None$", _assert=True,  **kwargs):
+    def radarpoints_pointstask_pagelist(self, getPointsQtySort="$None$", pointsTaskDateSort="$None$", pointsConfigName="$None$", dateLast="$None$", current=1, mobile="$None$", dateBegin="$None$", pointsConfigCode="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/radarpoints/pointsTask/pageList
                 params: dateBegin :  : 开始日期
                 params: dateLast :  : 结束日期
                 params: pointsConfigCode :  : 任务编码
                 params: pointsConfigName :  : 任务名称
                 params: mobile :  : 用户手机号
                 params: pointsTaskDateSort :  : 日期排序字段，"ASC"升序，"DESC"降序
                 params: getPointsQtySort :  : 积分值排序字段，"ASC"升序，"DESC"降序
                 params: current :  : 页码
                 params: size :  : 每页大小
                 params: headers : 请求头
         """
-        dateLast = self.get_list_choice(dateLast, list_or_dict=None, key="dateLast")
-        pointsConfigCode = self.get_list_choice(pointsConfigCode, list_or_dict=None, key="pointsConfigCode")
+        getPointsQtySort = self.get_list_choice(getPointsQtySort, list_or_dict=None, key="getPointsQtySort")
         pointsTaskDateSort = self.get_list_choice(pointsTaskDateSort, list_or_dict=None, key="pointsTaskDateSort")
         pointsConfigName = self.get_list_choice(pointsConfigName, list_or_dict=None, key="pointsConfigName")
-        dateBegin = self.get_list_choice(dateBegin, list_or_dict=None, key="dateBegin")
+        dateLast = self.get_list_choice(dateLast, list_or_dict=None, key="dateLast")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        getPointsQtySort = self.get_list_choice(getPointsQtySort, list_or_dict=None, key="getPointsQtySort")
+        dateBegin = self.get_list_choice(dateBegin, list_or_dict=None, key="dateBegin")
+        pointsConfigCode = self.get_list_choice(pointsConfigCode, list_or_dict=None, key="pointsConfigCode")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_pointstask.radarpoints_pointstask_pagelist(**_kwargs)
 
         self.assert_radarpoints_pointstask_pagelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="积分任务 - 导出excel")
-    def radarpoints_pointstask_export(self, dateLast="$None$", pointsConfigCode="$None$", pointsTaskDateSort="$None$", pointsConfigName="$None$", dateBegin="$None$", mobile="$None$", getPointsQtySort="$None$", _assert=True,  **kwargs):
+    def radarpoints_pointstask_export(self, getPointsQtySort="$None$", pointsTaskDateSort="$None$", pointsConfigName="$None$", dateLast="$None$", mobile="$None$", dateBegin="$None$", pointsConfigCode="$None$", _assert=True,  **kwargs):
         """
             url=/radarpoints/pointsTask/export
                 params: dateBegin :  : 开始日期
                 params: dateLast :  : 结束日期
                 params: pointsConfigCode :  : 任务编码
                 params: pointsConfigName :  : 任务名称
                 params: mobile :  : 用户手机号
                 params: pointsTaskDateSort :  : 日期排序字段，"ASC"升序，"DESC"降序
                 params: getPointsQtySort :  : 积分值排序字段，"ASC"升序，"DESC"降序
                 params: headers : 请求头
         """
-        dateLast = self.get_list_choice(dateLast, list_or_dict=None, key="dateLast")
-        pointsConfigCode = self.get_list_choice(pointsConfigCode, list_or_dict=None, key="pointsConfigCode")
+        getPointsQtySort = self.get_list_choice(getPointsQtySort, list_or_dict=None, key="getPointsQtySort")
         pointsTaskDateSort = self.get_list_choice(pointsTaskDateSort, list_or_dict=None, key="pointsTaskDateSort")
         pointsConfigName = self.get_list_choice(pointsConfigName, list_or_dict=None, key="pointsConfigName")
-        dateBegin = self.get_list_choice(dateBegin, list_or_dict=None, key="dateBegin")
+        dateLast = self.get_list_choice(dateLast, list_or_dict=None, key="dateLast")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
-        getPointsQtySort = self.get_list_choice(getPointsQtySort, list_or_dict=None, key="getPointsQtySort")
+        dateBegin = self.get_list_choice(dateBegin, list_or_dict=None, key="dateBegin")
+        pointsConfigCode = self.get_list_choice(pointsConfigCode, list_or_dict=None, key="pointsConfigCode")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_pointstask.radarpoints_pointstask_export(**_kwargs)
 
         self.assert_radarpoints_pointstask_export(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_summarystatistics.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_summarystatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.radarpoints.asserts_radarpoints_summarystatistics import AssertsRadarpointsSummarystatistics
 from service.app_a.apis.radarpoints import apis_radarpoints_summarystatistics
 
 
 class FunsRadarpointsSummarystatistics(AssertsRadarpointsSummarystatistics):
     @allure.step(title="积分汇总统计-分页查询积分")
-    def radarpoints_summarystatistics_pagelist(self, flowTimeEnd="$None$", flowTimeBefore="$None$", size=10, current=1, _assert=True,  **kwargs):
+    def radarpoints_summarystatistics_pagelist(self, flowTimeEnd="$None$", size=10, flowTimeBefore="$None$", current=1, _assert=True,  **kwargs):
         """
             url=/radarpoints/summaryStatistics/pageList
                 params: current :  :
                 params: size :  :
                 params: flowTimeBefore :  : 流水开始时间
                 params: flowTimeEnd :  : 流水结束时间
                 params: headers : 请求头
```

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/funs_radarpoints_userpoints.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_userpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import allure
 from service.app_a.funs.radarpoints.userpoints.funs_radarpoints_userpoints_pointsinfo import FunsRadarpointsUserpointsPointsinfo
 from service.app_a.funs.radarpoints.userpoints.funs_radarpoints_userpoints_exchangeinfo import FunsRadarpointsUserpointsExchangeinfo
 
 
 class FunsRadarpointsUserpoints(FunsRadarpointsUserpointsPointsinfo, FunsRadarpointsUserpointsExchangeinfo, AssertsRadarpointsUserpoints):
     @allure.step(title="用户积分 - 分页查询")
-    def radarpoints_userpoints_pagelist(self, cumulativeAcquisitionMost="$None$", freezeQtyMost="$None$", conversionFrequencyLeast="$None$", size=10, registrationTimeBegin="$None$", userId="$None$", physicalIntegralMost="$None$", cumulativeConsumptionLeast="$None$", cumulativeAcquisitionLeast="$None$", registrationTimeEnd="$None$", nickName="$None$", physicalIntegralLeast="$None$", mobile="$None$", conversionFrequencyMost="$None$", cumulativeConsumptionMost="$None$", current=1, freezeQtyLeast="$None$", _assert=True,  **kwargs):
+    def radarpoints_userpoints_pagelist(self, cumulativeAcquisitionMost="$None$", registrationTimeEnd="$None$", physicalIntegralMost="$None$", cumulativeConsumptionLeast="$None$", current=1, freezeQtyMost="$None$", cumulativeAcquisitionLeast="$None$", mobile="$None$", physicalIntegralLeast="$None$", freezeQtyLeast="$None$", conversionFrequencyMost="$None$", nickName="$None$", conversionFrequencyLeast="$None$", userId="$None$", size=10, registrationTimeBegin="$None$", cumulativeConsumptionMost="$None$", _assert=True,  **kwargs):
         """
             url=/radarpoints/userPoints/pageList
                 params: mobile :  : 用户手机号
                 params: nickName :  : 用户昵称
                 params: registrationTimeBegin :  : 注册时间 - 开始
                 params: registrationTimeEnd :  : 注册时间 - 结束
                 params: physicalIntegralLeast :  : 持有积分 - 最少
@@ -25,39 +25,39 @@
                 params: freezeQtyLeast :  : 冻结积分 - 最少
                 params: freezeQtyMost :  : 冻结积分 - 最多
                 params: current :  : 页码
                 params: size :  : 每页大小
                 params: headers : 请求头
         """
         cumulativeAcquisitionMost = self.get_list_choice(cumulativeAcquisitionMost, list_or_dict=None, key="cumulativeAcquisitionMost")
-        freezeQtyMost = self.get_list_choice(freezeQtyMost, list_or_dict=None, key="freezeQtyMost")
-        conversionFrequencyLeast = self.get_list_choice(conversionFrequencyLeast, list_or_dict=None, key="conversionFrequencyLeast")
-        registrationTimeBegin = self.get_list_choice(registrationTimeBegin, list_or_dict=None, key="registrationTimeBegin")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        registrationTimeEnd = self.get_list_choice(registrationTimeEnd, list_or_dict=None, key="registrationTimeEnd")
         physicalIntegralMost = self.get_list_choice(physicalIntegralMost, list_or_dict=None, key="physicalIntegralMost")
         cumulativeConsumptionLeast = self.get_list_choice(cumulativeConsumptionLeast, list_or_dict=None, key="cumulativeConsumptionLeast")
+        freezeQtyMost = self.get_list_choice(freezeQtyMost, list_or_dict=None, key="freezeQtyMost")
         cumulativeAcquisitionLeast = self.get_list_choice(cumulativeAcquisitionLeast, list_or_dict=None, key="cumulativeAcquisitionLeast")
-        registrationTimeEnd = self.get_list_choice(registrationTimeEnd, list_or_dict=None, key="registrationTimeEnd")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
-        physicalIntegralLeast = self.get_list_choice(physicalIntegralLeast, list_or_dict=None, key="physicalIntegralLeast")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        physicalIntegralLeast = self.get_list_choice(physicalIntegralLeast, list_or_dict=None, key="physicalIntegralLeast")
+        freezeQtyLeast = self.get_list_choice(freezeQtyLeast, list_or_dict=None, key="freezeQtyLeast")
         conversionFrequencyMost = self.get_list_choice(conversionFrequencyMost, list_or_dict=None, key="conversionFrequencyMost")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        conversionFrequencyLeast = self.get_list_choice(conversionFrequencyLeast, list_or_dict=None, key="conversionFrequencyLeast")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
+        registrationTimeBegin = self.get_list_choice(registrationTimeBegin, list_or_dict=None, key="registrationTimeBegin")
         cumulativeConsumptionMost = self.get_list_choice(cumulativeConsumptionMost, list_or_dict=None, key="cumulativeConsumptionMost")
-        freezeQtyLeast = self.get_list_choice(freezeQtyLeast, list_or_dict=None, key="freezeQtyLeast")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_userpoints.radarpoints_userpoints_pagelist(**_kwargs)
 
         self.assert_radarpoints_userpoints_pagelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
     @allure.step(title="用户积分 - 导出excel")
-    def radarpoints_userpoints_export(self, cumulativeAcquisitionMost="$None$", conversionFrequencyLeast="$None$", pageSize="$None$", registrationTimeBegin="$None$", physicalIntegralMost="$None$", currentPage="$None$", cumulativeConsumptionLeast="$None$", cumulativeAcquisitionLeast="$None$", registrationTimeEnd="$None$", nickName="$None$", physicalIntegralLeast="$None$", conversionFrequencyMost="$None$", cumulativeConsumptionMost="$None$", _assert=True,  **kwargs):
+    def radarpoints_userpoints_export(self, cumulativeAcquisitionMost="$None$", physicalIntegralMost="$None$", cumulativeConsumptionLeast="$None$", pageSize="$None$", cumulativeAcquisitionLeast="$None$", physicalIntegralLeast="$None$", conversionFrequencyMost="$None$", nickName="$None$", conversionFrequencyLeast="$None$", registrationTimeEnd="$None$", currentPage="$None$", registrationTimeBegin="$None$", cumulativeConsumptionMost="$None$", _assert=True,  **kwargs):
         """
             url=/radarpoints/userPoints/export
                 params: nickName :  : 用户昵称
                 params: registrationTimeBegin :  : 注册时间 - 开始
                 params: registrationTimeEnd :  : 注册时间 - 结束
                 params: physicalIntegralLeast :  : 持有积分 - 最少
                 params: physicalIntegralMost :  : 持有积分 - 最多
@@ -68,25 +68,25 @@
                 params: conversionFrequencyLeast :  : 兑换次数 - 最少
                 params: conversionFrequencyMost :  : 兑换次数 - 最多
                 params: currentPage :  : 当前页码
                 params: pageSize :  : 每页大小
                 params: headers : 请求头
         """
         cumulativeAcquisitionMost = self.get_list_choice(cumulativeAcquisitionMost, list_or_dict=None, key="cumulativeAcquisitionMost")
-        conversionFrequencyLeast = self.get_list_choice(conversionFrequencyLeast, list_or_dict=None, key="conversionFrequencyLeast")
-        pageSize = self.get_list_choice(pageSize, list_or_dict=None, key="pageSize")
-        registrationTimeBegin = self.get_list_choice(registrationTimeBegin, list_or_dict=None, key="registrationTimeBegin")
         physicalIntegralMost = self.get_list_choice(physicalIntegralMost, list_or_dict=None, key="physicalIntegralMost")
-        currentPage = self.get_list_choice(currentPage, list_or_dict=None, key="currentPage")
         cumulativeConsumptionLeast = self.get_list_choice(cumulativeConsumptionLeast, list_or_dict=None, key="cumulativeConsumptionLeast")
+        pageSize = self.get_list_choice(pageSize, list_or_dict=None, key="pageSize")
         cumulativeAcquisitionLeast = self.get_list_choice(cumulativeAcquisitionLeast, list_or_dict=None, key="cumulativeAcquisitionLeast")
-        registrationTimeEnd = self.get_list_choice(registrationTimeEnd, list_or_dict=None, key="registrationTimeEnd")
-        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
         physicalIntegralLeast = self.get_list_choice(physicalIntegralLeast, list_or_dict=None, key="physicalIntegralLeast")
         conversionFrequencyMost = self.get_list_choice(conversionFrequencyMost, list_or_dict=None, key="conversionFrequencyMost")
+        nickName = self.get_list_choice(nickName, list_or_dict=None, key="nickName")
+        conversionFrequencyLeast = self.get_list_choice(conversionFrequencyLeast, list_or_dict=None, key="conversionFrequencyLeast")
+        registrationTimeEnd = self.get_list_choice(registrationTimeEnd, list_or_dict=None, key="registrationTimeEnd")
+        currentPage = self.get_list_choice(currentPage, list_or_dict=None, key="currentPage")
+        registrationTimeBegin = self.get_list_choice(registrationTimeBegin, list_or_dict=None, key="registrationTimeBegin")
         cumulativeConsumptionMost = self.get_list_choice(cumulativeConsumptionMost, list_or_dict=None, key="cumulativeConsumptionMost")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_userpoints.radarpoints_userpoints_export(**_kwargs)
 
         self.assert_radarpoints_userpoints_export(_assert, **_kwargs)
         self.set_output_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_exchangeinfo.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_exchangeinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 
 from service.app_a.asserts.radarpoints.userpoints.asserts_radarpoints_userpoints_exchangeinfo import AssertsRadarpointsUserpointsExchangeinfo
 from service.app_a.apis.radarpoints.userpoints import apis_radarpoints_userpoints_exchangeinfo
 
 
 class FunsRadarpointsUserpointsExchangeinfo(AssertsRadarpointsUserpointsExchangeinfo):
     @allure.step(title="用户中心-兑换明细 - 分页查询")
-    def radarpoints_userpoints_exchangeinfo_pagelist(self, consigneeName="$None$", orderEndTime="$None$", goodsOrderId="$None$", userId="$None$", orderStartTime="$None$", mobile="$None$", current=1, size=10, _assert=True,  **kwargs):
+    def radarpoints_userpoints_exchangeinfo_pagelist(self, orderEndTime="$None$", orderStartTime="$None$", current=1, consigneeName="$None$", mobile="$None$", goodsOrderId="$None$", userId="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/radarpoints/userPoints/exchangeInfo/pageList
                 params: size :  : 每页大小
                 params: current :  : 当前页
                 params: consigneeName :  : 收货人姓名
                 params: goodsOrderId :  : 商品订单
                 params: mobile :  : 收货人电话
                 params: orderStartTime :  : 下单开始时间
                 params: orderEndTime :  : 下单结束时间
                 params: headers : 请求头
         """
-        consigneeName = self.get_list_choice(consigneeName, list_or_dict=None, key="consigneeName")
         orderEndTime = self.get_list_choice(orderEndTime, list_or_dict=None, key="orderEndTime")
-        goodsOrderId = self.get_list_choice(goodsOrderId, list_or_dict=None, key="goodsOrderId")
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
         orderStartTime = self.get_list_choice(orderStartTime, list_or_dict=None, key="orderStartTime")
+        consigneeName = self.get_list_choice(consigneeName, list_or_dict=None, key="consigneeName")
         mobile = self.get_list_choice(mobile, list_or_dict=None, key="mobile")
+        goodsOrderId = self.get_list_choice(goodsOrderId, list_or_dict=None, key="goodsOrderId")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_userpoints_exchangeinfo.radarpoints_userpoints_exchangeinfo_pagelist(**_kwargs)
 
         self.assert_radarpoints_userpoints_exchangeinfo_pagelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_pointsinfo.py` & `huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_pointsinfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from service.app_a.asserts.radarpoints.userpoints.asserts_radarpoints_userpoints_pointsinfo import AssertsRadarpointsUserpointsPointsinfo
 from service.app_a.apis.radarpoints.userpoints import apis_radarpoints_userpoints_pointsinfo
 
 
 class FunsRadarpointsUserpointsPointsinfo(AssertsRadarpointsUserpointsPointsinfo):
     @allure.step(title="用户中心-积分明细-分页查询")
-    def radarpoints_userpoints_pointsinfo_pagelist(self, userId="$None$", changeTimeEnd="$None$", businessSceneType="$None$", changeTimeBegin="$None$", current=1, size=10, name="$None$", _assert=True,  **kwargs):
+    def radarpoints_userpoints_pointsinfo_pagelist(self, current=1, name="$None$", businessSceneType="$None$", changeTimeEnd="$None$", changeTimeBegin="$None$", userId="$None$", size=10, _assert=True,  **kwargs):
         """
             url=/radarpoints/userPoints/pointsInfo/pageList
                 params: size :  : 每页大小
                 params: current :  : 当前页
                 params: businessSceneType :  : 10001 转介裂变
                 10002 营销活动
                 10003 社区活跃
@@ -21,19 +21,19 @@
                 10008 后台管理手动操作
                 20000 其他
                 params: name :  : 名称
                 params: changeTimeBegin :  : 变动开始时间
                 params: changeTimeEnd :  : 变动结束时间
                 params: headers : 请求头
         """
-        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
-        changeTimeEnd = self.get_list_choice(changeTimeEnd, list_or_dict=None, key="changeTimeEnd")
+        name = self.get_list_choice(name, list_or_dict=None, key="name")
         businessSceneType = self.get_list_choice(businessSceneType, list_or_dict=None, key="businessSceneType")
+        changeTimeEnd = self.get_list_choice(changeTimeEnd, list_or_dict=None, key="changeTimeEnd")
         changeTimeBegin = self.get_list_choice(changeTimeBegin, list_or_dict=None, key="changeTimeBegin")
-        name = self.get_list_choice(name, list_or_dict=None, key="name")
+        userId = self.get_list_choice(userId, list_or_dict=None, key="userId")
 
         _kwargs = self.get_kwargs(locals())
         self.res = apis_radarpoints_userpoints_pointsinfo.radarpoints_userpoints_pointsinfo_pagelist(**_kwargs)
 
         self.assert_radarpoints_userpoints_pointsinfo_pagelist(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
```

### Comparing `huhk-1.9.5/service/app_a/sqls/admin/sqls_admin_guc.py` & `huhk-1.9.6/service/app_a/sqls/admin/sqls_admin_guc.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/admin/sqls_admin_spa.py` & `huhk-1.9.6/service/app_a/sqls/admin/sqls_admin_spa.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/common/sqls_common_clue.py` & `huhk-1.9.6/service/app_a/sqls/common/sqls_common_clue.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/common/sqls_common_common.py` & `huhk-1.9.6/service/app_a/sqls/common/sqls_common_common.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/common/sqls_common_remoteinterfacelog.py` & `huhk-1.9.6/service/app_a/sqls/common/sqls_common_remoteinterfacelog.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/common/sqls_common_systemversion.py` & `huhk-1.9.6/service/app_a/sqls/common/sqls_common_systemversion.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/common/sqls_common_user.py` & `huhk-1.9.6/service/app_a/sqls/common/sqls_common_user.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/common/sqls_common_user4c.py` & `huhk-1.9.6/service/app_a/sqls/common/sqls_common_user4c.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/common/sqls_common_userpointsmanage.py` & `huhk-1.9.6/service/app_a/sqls/common/sqls_common_userpointsmanage.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/material/sqls_content_material_getmateriallist.py` & `huhk-1.9.6/service/app_a/sqls/content/material/sqls_content_material_getmateriallist.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_activitymanager.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_activitymanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_adv.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_adv.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_advplace.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_advplace.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_agreement.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_agreement.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_campmanager.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_campmanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_comment.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_comment.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_commonquestion.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_commonquestion.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_contentmanager.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_contentmanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_essay.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_essay.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_essaycomment.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_essaycomment.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_essayweb.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_essayweb.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_hotcity.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_hotcity.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_hotsearch.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_hotsearch.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_material.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_material.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_messagemanager.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_messagemanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_noticemanager.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_noticemanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_question.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_question.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_recruit.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_recruit.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_safecode.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_safecode.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_subject.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_subject.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_subjectweb.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_subjectweb.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/content/sqls_content_topic4c.py` & `huhk-1.9.6/service/app_a/sqls/content/sqls_content_topic4c.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_area.py` & `huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_area.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_carmodel.py` & `huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_carmodel.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_configure.py` & `huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_configure.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_ordermain.py` & `huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_ordermain.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/goods/sqls_goods_testdrive.py` & `huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_testdrive.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/manageapi/order/sqls_manageapi_order_mainorder.py` & `huhk-1.9.6/service/app_a/sqls/manageapi/order/sqls_manageapi_order_mainorder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/open/haohan/sqls_open_haohan_relation.py` & `huhk-1.9.6/service/app_a/sqls/open/haohan/sqls_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/open/haohan/sqls_open_haohan_rights.py` & `huhk-1.9.6/service/app_a/sqls/open/haohan/sqls_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/order/mainorder/sqls_order_mainorder_scrm2app.py` & `huhk-1.9.6/service/app_a/sqls/order/mainorder/sqls_order_mainorder_scrm2app.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/order/rights/sqls_order_rights_rightsmanager.py` & `huhk-1.9.6/service/app_a/sqls/order/rights/sqls_order_rights_rightsmanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/order/rightsorder/sqls_order_rightsorder_receive.py` & `huhk-1.9.6/service/app_a/sqls/order/rightsorder/sqls_order_rightsorder_receive.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/order/sqls_order_freeorder.py` & `huhk-1.9.6/service/app_a/sqls/order/sqls_order_freeorder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/order/sqls_order_mainorder.py` & `huhk-1.9.6/service/app_a/sqls/order/sqls_order_mainorder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/order/sqls_order_order.py` & `huhk-1.9.6/service/app_a/sqls/order/sqls_order_order.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/order/sqls_order_rightsorder.py` & `huhk-1.9.6/service/app_a/sqls/order/sqls_order_rightsorder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/order/sqls_order_testdrive.py` & `huhk-1.9.6/service/app_a/sqls/order/sqls_order_testdrive.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/pay/sqls_pay_orderpaybill.py` & `huhk-1.9.6/service/app_a/sqls/pay/sqls_pay_orderpaybill.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_batch.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_batch.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_single.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_single.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_adjustpoints.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_adjustpoints.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_pointsconfig.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_pointsconfig.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_pointstask.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_pointstask.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_summarystatistics.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_summarystatistics.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/sqls_radarpoints_userpoints.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_userpoints.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_exchangeinfo.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_exchangeinfo.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_pointsinfo.py` & `huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_pointsinfo.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/sqls_activitymanager.py` & `huhk-1.9.6/service/app_a/sqls/sqls_activitymanager.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/sqls_app_a.py` & `huhk-1.9.6/service/app_a/sqls/sqls_app_a.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/sqls_area.py` & `huhk-1.9.6/service/app_a/sqls/sqls_area.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/sqls_content.py` & `huhk-1.9.6/service/app_a/sqls/sqls_content.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/sqls_essay.py` & `huhk-1.9.6/service/app_a/sqls/sqls_essay.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/service/app_a/sqls/sqls_testdrive.py` & `huhk-1.9.6/service/app_a/sqls/sqls_testdrive.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.5/testcase/app_a/test_page.py` & `huhk-1.9.6/testcase/app_a/test_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,61 +21,61 @@
 
     # @pytest.mark.skip("不执行")
     @allure.step(title="网点列表-获取经销商__每页条数")
     def test_page__size_003(self):
         self.f.page(size=20)
 
     # @pytest.mark.skip("不执行")
-    @allure.step(title="网点列表-获取经销商__单参数有值： district")
-    def test_page__district_004(self):
-        self.f.page(district=True)
-
-    # @pytest.mark.skip("不执行")
-    @allure.step(title="网点列表-获取经销商__单参数有值： province")
-    def test_page__province_005(self):
-        self.f.page(province=True)
+    @allure.step(title="网点列表-获取经销商__单参数有值： dealerAddress")
+    def test_page__dealerAddress_004(self):
+        self.f.page(dealerAddress=True)
 
     # @pytest.mark.skip("不执行")
-    @allure.step(title="网点列表-获取经销商__单参数有值： provinceNameSort")
-    def test_page__provinceNameSort_006(self):
-        self.f.page(provinceNameSort=True)
+    @allure.step(title="网点列表-获取经销商__单参数有值： districtNameSort")
+    def test_page__districtNameSort_005(self):
+        self.f.page(districtNameSort=True)
 
     # @pytest.mark.skip("不执行")
     @allure.step(title="网点列表-获取经销商__单参数有值： cityNameSort")
-    def test_page__cityNameSort_007(self):
+    def test_page__cityNameSort_006(self):
         self.f.page(cityNameSort=True)
 
     # @pytest.mark.skip("不执行")
+    @allure.step(title="网点列表-获取经销商__单参数有值： city")
+    def test_page__city_007(self):
+        self.f.page(city=True)
+
+    # @pytest.mark.skip("不执行")
+    @allure.step(title="网点列表-获取经销商__单参数有值： province")
+    def test_page__province_008(self):
+        self.f.page(province=True)
+
+    # @pytest.mark.skip("不执行")
     @allure.step(title="网点列表-获取经销商__单参数有值： dealerName")
-    def test_page__dealerName_008(self):
+    def test_page__dealerName_009(self):
         self.f.page(dealerName=True)
 
     # @pytest.mark.skip("不执行")
     @allure.step(title="网点列表-获取经销商__单参数有值： shopBusinessType")
-    def test_page__shopBusinessType_009(self):
+    def test_page__shopBusinessType_010(self):
         self.f.page(shopBusinessType=True)
 
     # @pytest.mark.skip("不执行")
-    @allure.step(title="网点列表-获取经销商__单参数有值： districtNameSort")
-    def test_page__districtNameSort_010(self):
-        self.f.page(districtNameSort=True)
+    @allure.step(title="网点列表-获取经销商__单参数有值： district")
+    def test_page__district_011(self):
+        self.f.page(district=True)
 
     # @pytest.mark.skip("不执行")
     @allure.step(title="网点列表-获取经销商__单参数有值： dealerCode")
-    def test_page__dealerCode_011(self):
+    def test_page__dealerCode_012(self):
         self.f.page(dealerCode=True)
 
     # @pytest.mark.skip("不执行")
-    @allure.step(title="网点列表-获取经销商__单参数有值： dealerAddress")
-    def test_page__dealerAddress_012(self):
-        self.f.page(dealerAddress=True)
-
-    # @pytest.mark.skip("不执行")
-    @allure.step(title="网点列表-获取经销商__单参数有值： city")
-    def test_page__city_013(self):
-        self.f.page(city=True)
+    @allure.step(title="网点列表-获取经销商__单参数有值： provinceNameSort")
+    def test_page__provinceNameSort_013(self):
+        self.f.page(provinceNameSort=True)
 
     # @pytest.mark.skip("不执行")
     @allure.step(title="网点列表-获取经销商__所有参数有值")
     def test_page__all_014(self):
-        self.f.page(district=True, province=True, provinceNameSort=True, cityNameSort=True, dealerName=True, shopBusinessType=True, districtNameSort=True, dealerCode=True, dealerAddress=True, city=True)
+        self.f.page(dealerAddress=True, districtNameSort=True, cityNameSort=True, city=True, province=True, dealerName=True, shopBusinessType=True, district=True, dealerCode=True, provinceNameSort=True)
```

