# Comparing `tmp/wagtail-review-0.3.1.tar.gz` & `tmp/wagtail-review-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-review-0.3.1.tar", last modified: Wed Jan  4 13:23:24 2023, max compression
+gzip compressed data, was "wagtail-review-0.4.tar", last modified: Tue Aug  1 15:38:28 2023, max compression
```

## Comparing `wagtail-review-0.3.1.tar` & `wagtail-review-0.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.984569 wagtail-review-0.3.1/
--rw-r--r--   0 matthew    (501) staff       (20)     2007 2023-01-04 13:22:22.000000 wagtail-review-0.3.1/CHANGELOG.txt
--rw-r--r--   0 matthew    (501) staff       (20)     1508 2018-10-10 08:37:32.000000 wagtail-review-0.3.1/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)      144 2018-10-10 09:57:41.000000 wagtail-review-0.3.1/MANIFEST.in
--rw-r--r--   0 matthew    (501) staff       (20)     1224 2023-01-04 13:23:24.984233 wagtail-review-0.3.1/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)     4385 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/README.md
--rw-r--r--   0 matthew    (501) staff       (20)       38 2023-01-04 13:23:24.984668 wagtail-review-0.3.1/setup.cfg
--rw-r--r--   0 matthew    (501) staff       (20)     1446 2023-01-04 13:22:35.000000 wagtail-review-0.3.1/setup.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.958685 wagtail-review-0.3.1/tests/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2018-09-19 13:49:54.000000 wagtail-review-0.3.1/tests/__init__.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.960134 wagtail-review-0.3.1/tests/migrations/
--rw-r--r--   0 matthew    (501) staff       (20)      769 2018-09-26 19:01:17.000000 wagtail-review-0.3.1/tests/migrations/0001_initial.py
--rw-r--r--   0 matthew    (501) staff       (20)        0 2018-09-26 19:01:17.000000 wagtail-review-0.3.1/tests/migrations/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)       72 2018-09-26 18:56:46.000000 wagtail-review-0.3.1/tests/models.py
--rw-r--r--   0 matthew    (501) staff       (20)     2416 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/tests/settings.py
--rw-r--r--   0 matthew    (501) staff       (20)     7582 2023-01-04 13:13:16.000000 wagtail-review-0.3.1/tests/test_admin.py
--rw-r--r--   0 matthew    (501) staff       (20)     3937 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/tests/test_frontend.py
--rw-r--r--   0 matthew    (501) staff       (20)     2327 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/tests/test_models.py
--rw-r--r--   0 matthew    (501) staff       (20)      559 2022-08-26 15:10:09.000000 wagtail-review-0.3.1/tests/urls.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.964205 wagtail-review-0.3.1/wagtail_review/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2021-03-01 16:23:28.000000 wagtail-review-0.3.1/wagtail_review/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)     1121 2022-08-26 15:10:09.000000 wagtail-review-0.3.1/wagtail_review/admin_urls.py
--rw-r--r--   0 matthew    (501) staff       (20)     2217 2022-08-26 15:10:09.000000 wagtail-review-0.3.1/wagtail_review/forms.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.968678 wagtail-review-0.3.1/wagtail_review/migrations/
--rw-r--r--   0 matthew    (501) staff       (20)     4706 2023-01-04 13:13:16.000000 wagtail-review-0.3.1/wagtail_review/migrations/0001_initial.py
--rw-r--r--   0 matthew    (501) staff       (20)     1545 2018-10-02 09:37:35.000000 wagtail-review-0.3.1/wagtail_review/migrations/0002_annotation_annotationrange.py
--rw-r--r--   0 matthew    (501) staff       (20)      976 2018-10-02 14:44:58.000000 wagtail-review-0.3.1/wagtail_review/migrations/0003_response.py
--rw-r--r--   0 matthew    (501) staff       (20)        0 2018-09-19 15:22:02.000000 wagtail-review-0.3.1/wagtail_review/migrations/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)     8563 2023-01-04 13:13:16.000000 wagtail-review-0.3.1/wagtail_review/models.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.950491 wagtail-review-0.3.1/wagtail_review/static/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.950803 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.970827 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/css/
--rw-r--r--   0 matthew    (501) staff       (20)     3679 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/css/annotator.css
--rw-r--r--   0 matthew    (501) staff       (20)      220 2018-10-09 10:11:59.000000 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/css/audit_trail.css
--rw-r--r--   0 matthew    (501) staff       (20)      627 2021-03-01 16:23:28.000000 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/css/create_review.css
--rw-r--r--   0 matthew    (501) staff       (20)     2562 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/css/respond.css
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.974078 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/js/
--rw-r--r--   0 matthew    (501) staff       (20)   257028 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/js/annotator-2.0.0a3.min.js
--rw-r--r--   0 matthew    (501) staff       (20)     1680 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/js/annotator-extensions.js
--rw-r--r--   0 matthew    (501) staff       (20)     5282 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/static/wagtail_review/js/submit.js
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.951041 wagtail-review-0.3.1/wagtail_review/templates/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.977064 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.978121 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/admin/
--rw-r--r--   0 matthew    (501) staff       (20)     4209 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/admin/audit_trail.html
--rw-r--r--   0 matthew    (501) staff       (20)     1836 2021-03-01 16:23:28.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/admin/dashboard.html
--rw-r--r--   0 matthew    (501) staff       (20)     3463 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/annotate.html
--rw-r--r--   0 matthew    (501) staff       (20)     2506 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/create_review.html
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.980406 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/email/
--rw-r--r--   0 matthew    (501) staff       (20)      841 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/email/request_review.txt
--rw-r--r--   0 matthew    (501) staff       (20)      117 2018-09-27 10:56:08.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/email/request_review_subject.txt
--rw-r--r--   0 matthew    (501) staff       (20)      612 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/email/response_received.txt
--rw-r--r--   0 matthew    (501) staff       (20)      175 2018-10-17 14:22:10.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/email/response_received_subject.txt
--rw-r--r--   0 matthew    (501) staff       (20)      496 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/response_form_fields.html
--rw-r--r--   0 matthew    (501) staff       (20)      237 2021-03-01 16:23:28.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/submit_for_review_menu_item.html
--rw-r--r--   0 matthew    (501) staff       (20)      154 2021-03-01 16:23:28.000000 wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/submit_for_review_menu_item_pre_2_10.html
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.981398 wagtail-review-0.3.1/wagtail_review/templatetags/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2018-09-27 23:52:42.000000 wagtail-review-0.3.1/wagtail_review/templatetags/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)      355 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/templatetags/wagtailreview_admin_tags.py
--rw-r--r--   0 matthew    (501) staff       (20)     1172 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/templatetags/wagtailreview_tags.py
--rw-r--r--   0 matthew    (501) staff       (20)      644 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/text.py
--rw-r--r--   0 matthew    (501) staff       (20)      679 2022-08-26 15:10:09.000000 wagtail-review-0.3.1/wagtail_review/urls.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.983383 wagtail-review-0.3.1/wagtail_review/views/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2021-03-01 16:23:28.000000 wagtail-review-0.3.1/wagtail_review/views/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)     7089 2022-08-26 15:10:09.000000 wagtail-review-0.3.1/wagtail_review/views/admin.py
--rw-r--r--   0 matthew    (501) staff       (20)     2922 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/views/annotations_api.py
--rw-r--r--   0 matthew    (501) staff       (20)     2969 2021-03-01 16:47:13.000000 wagtail-review-0.3.1/wagtail_review/views/frontend.py
--rw-r--r--   0 matthew    (501) staff       (20)     3933 2022-10-19 15:41:49.000000 wagtail-review-0.3.1/wagtail_review/wagtail_hooks.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-04 13:23:24.965999 wagtail-review-0.3.1/wagtail_review.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)     1224 2023-01-04 13:23:24.000000 wagtail-review-0.3.1/wagtail_review.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)     2225 2023-01-04 13:23:24.000000 wagtail-review-0.3.1/wagtail_review.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2023-01-04 13:23:24.000000 wagtail-review-0.3.1/wagtail_review.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)       18 2023-01-04 13:23:24.000000 wagtail-review-0.3.1/wagtail_review.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)       21 2023-01-04 13:23:24.000000 wagtail-review-0.3.1/wagtail_review.egg-info/top_level.txt
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.988189 wagtail-review-0.4/
+-rw-r--r--   0 matthew    (501) staff       (20)     2145 2023-08-01 15:36:57.000000 wagtail-review-0.4/CHANGELOG.txt
+-rw-r--r--   0 matthew    (501) staff       (20)     1508 2018-10-10 08:37:32.000000 wagtail-review-0.4/LICENSE
+-rw-r--r--   0 matthew    (501) staff       (20)      144 2018-10-10 09:57:41.000000 wagtail-review-0.4/MANIFEST.in
+-rw-r--r--   0 matthew    (501) staff       (20)     1170 2023-08-01 15:38:28.987814 wagtail-review-0.4/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)     4384 2023-08-01 15:35:11.000000 wagtail-review-0.4/README.md
+-rw-r--r--   0 matthew    (501) staff       (20)       38 2023-08-01 15:38:28.988311 wagtail-review-0.4/setup.cfg
+-rw-r--r--   0 matthew    (501) staff       (20)     1399 2023-08-01 15:37:19.000000 wagtail-review-0.4/setup.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.961119 wagtail-review-0.4/tests/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2018-09-19 13:49:54.000000 wagtail-review-0.4/tests/__init__.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.962137 wagtail-review-0.4/tests/migrations/
+-rw-r--r--   0 matthew    (501) staff       (20)      769 2018-09-26 19:01:17.000000 wagtail-review-0.4/tests/migrations/0001_initial.py
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2018-09-26 19:01:17.000000 wagtail-review-0.4/tests/migrations/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)       67 2023-08-01 15:35:11.000000 wagtail-review-0.4/tests/models.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2312 2023-08-01 15:35:11.000000 wagtail-review-0.4/tests/settings.py
+-rw-r--r--   0 matthew    (501) staff       (20)     9658 2023-08-01 15:35:11.000000 wagtail-review-0.4/tests/test_admin.py
+-rw-r--r--   0 matthew    (501) staff       (20)     3932 2023-08-01 15:35:11.000000 wagtail-review-0.4/tests/test_frontend.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2322 2023-08-01 15:35:11.000000 wagtail-review-0.4/tests/test_models.py
+-rw-r--r--   0 matthew    (501) staff       (20)      539 2023-08-01 15:35:11.000000 wagtail-review-0.4/tests/urls.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.965629 wagtail-review-0.4/wagtail_review/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2021-03-01 16:23:28.000000 wagtail-review-0.4/wagtail_review/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1049 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/admin_urls.py
+-rw-r--r--   0 matthew    (501) staff       (20)      224 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/apps.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2217 2022-08-26 15:10:09.000000 wagtail-review-0.4/wagtail_review/forms.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.968828 wagtail-review-0.4/wagtail_review/migrations/
+-rw-r--r--   0 matthew    (501) staff       (20)     4474 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/migrations/0001_initial.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1545 2018-10-02 09:37:35.000000 wagtail-review-0.4/wagtail_review/migrations/0002_annotation_annotationrange.py
+-rw-r--r--   0 matthew    (501) staff       (20)      976 2018-10-02 14:44:58.000000 wagtail-review-0.4/wagtail_review/migrations/0003_response.py
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2018-09-19 15:22:02.000000 wagtail-review-0.4/wagtail_review/migrations/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)     8273 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/models.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.950025 wagtail-review-0.4/wagtail_review/static/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.950413 wagtail-review-0.4/wagtail_review/static/wagtail_review/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.971601 wagtail-review-0.4/wagtail_review/static/wagtail_review/css/
+-rw-r--r--   0 matthew    (501) staff       (20)     3679 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/static/wagtail_review/css/annotator.css
+-rw-r--r--   0 matthew    (501) staff       (20)      220 2018-10-09 10:11:59.000000 wagtail-review-0.4/wagtail_review/static/wagtail_review/css/audit_trail.css
+-rw-r--r--   0 matthew    (501) staff       (20)      627 2021-03-01 16:23:28.000000 wagtail-review-0.4/wagtail_review/static/wagtail_review/css/create_review.css
+-rw-r--r--   0 matthew    (501) staff       (20)     2562 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/static/wagtail_review/css/respond.css
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.977555 wagtail-review-0.4/wagtail_review/static/wagtail_review/js/
+-rw-r--r--   0 matthew    (501) staff       (20)   257028 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/static/wagtail_review/js/annotator-2.0.0a3.min.js
+-rw-r--r--   0 matthew    (501) staff       (20)     1680 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/static/wagtail_review/js/annotator-extensions.js
+-rw-r--r--   0 matthew    (501) staff       (20)     5282 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/static/wagtail_review/js/submit.js
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.950713 wagtail-review-0.4/wagtail_review/templates/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.980453 wagtail-review-0.4/wagtail_review/templates/wagtail_review/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.981529 wagtail-review-0.4/wagtail_review/templates/wagtail_review/admin/
+-rw-r--r--   0 matthew    (501) staff       (20)     4211 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/admin/audit_trail.html
+-rw-r--r--   0 matthew    (501) staff       (20)     1836 2021-03-01 16:23:28.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/admin/dashboard.html
+-rw-r--r--   0 matthew    (501) staff       (20)     3463 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/annotate.html
+-rw-r--r--   0 matthew    (501) staff       (20)     2506 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/create_review.html
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.983701 wagtail-review-0.4/wagtail_review/templates/wagtail_review/email/
+-rw-r--r--   0 matthew    (501) staff       (20)      841 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/email/request_review.txt
+-rw-r--r--   0 matthew    (501) staff       (20)      117 2018-09-27 10:56:08.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/email/request_review_subject.txt
+-rw-r--r--   0 matthew    (501) staff       (20)      612 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/email/response_received.txt
+-rw-r--r--   0 matthew    (501) staff       (20)      175 2018-10-17 14:22:10.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/email/response_received_subject.txt
+-rw-r--r--   0 matthew    (501) staff       (20)      496 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/response_form_fields.html
+-rw-r--r--   0 matthew    (501) staff       (20)      237 2021-03-01 16:23:28.000000 wagtail-review-0.4/wagtail_review/templates/wagtail_review/submit_for_review_menu_item.html
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.984981 wagtail-review-0.4/wagtail_review/templatetags/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2018-09-27 23:52:42.000000 wagtail-review-0.4/wagtail_review/templatetags/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)      547 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/templatetags/wagtailreview_admin_tags.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1172 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/templatetags/wagtailreview_tags.py
+-rw-r--r--   0 matthew    (501) staff       (20)      644 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/text.py
+-rw-r--r--   0 matthew    (501) staff       (20)      681 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/urls.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.987077 wagtail-review-0.4/wagtail_review/views/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2021-03-01 16:23:28.000000 wagtail-review-0.4/wagtail_review/views/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)     6897 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/views/admin.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2922 2021-03-01 16:47:13.000000 wagtail-review-0.4/wagtail_review/views/annotations_api.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2199 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/views/frontend.py
+-rw-r--r--   0 matthew    (501) staff       (20)     3525 2023-08-01 15:35:11.000000 wagtail-review-0.4/wagtail_review/wagtail_hooks.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-08-01 15:38:28.967270 wagtail-review-0.4/wagtail_review.egg-info/
+-rw-r--r--   0 matthew    (501) staff       (20)     1170 2023-08-01 15:38:28.000000 wagtail-review-0.4/wagtail_review.egg-info/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)     2166 2023-08-01 15:38:28.000000 wagtail-review-0.4/wagtail_review.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2023-08-01 15:38:28.000000 wagtail-review-0.4/wagtail_review.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       18 2023-08-01 15:38:28.000000 wagtail-review-0.4/wagtail_review.egg-info/requires.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       21 2023-08-01 15:38:28.000000 wagtail-review-0.4/wagtail_review.egg-info/top_level.txt
```

### Comparing `wagtail-review-0.3.1/CHANGELOG.txt` & `wagtail-review-0.4/CHANGELOG.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.4 (2023-08-01)
+----------------
+
+* Fixes for Wagtail 5.x (Matt Westcott)
+* Dropped support for Wagtail <4.1, Django <3.2, Python <3.8
+
+
 0.3.1 (2022-01-04)
 ------------------
 
 * Fixes for Django 4.x (Adrien Lemaire)
 * Fixes for Wagtail 3.x and 4.x (Matt Westcott, Dan Braghis, Sage Abdullah)
```

### Comparing `wagtail-review-0.3.1/LICENSE` & `wagtail-review-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/README.md` & `wagtail-review-0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 An extension for Wagtail allowing pages to be submitted for review (including to non-Wagtail users) prior to publication
 
 ![Screencast demo](https://tom.s3.amazonaws.com/wagtail-review.gif)
 
 ## Requirements
 
-Wagtail 2.4 or higher
+Wagtail 4.1 or higher
 
 ## Installation
 
 Install the package from PyPI:
 
     pip install wagtail-review
 
@@ -19,15 +19,15 @@
     'wagtail_review',
 
 Add to your project's URL config:
 
     from wagtail_review import urls as wagtailreview_urls
 
     # Somewhere above the include(wagtail_urls) line:
-        url(r'^review/', include(wagtailreview_urls)),
+        path("review/", include(wagtailreview_urls)),
 
 Add a `{% wagtailreview %}` tag to your project's base template(s), towards the bottom of the document `<body>`:
 
     {% load wagtailreview_tags %}
 
     {% wagtailreview %}
```

### Comparing `wagtail-review-0.3.1/setup.py` & `wagtail-review-0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='wagtail-review',
-    version='0.3.1',
+    version='0.4',
     description="Review workflow for Wagtail",
     author='Matthew Westcott',
     author_email='matthew.westcott@torchbox.com',
     url='https://github.com/wagtail/wagtail-review',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'swapper>=1.1,<1.2',
     ],
+    python_requires=">=3.8",
     license='BSD',
     long_description="An extension for Wagtail allowing pages to be submitted for review (including to non-Wagtail users) prior to publication",
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django',
+        'Framework :: Django :: 3',
+        'Framework :: Django :: 4',
         'Framework :: Wagtail',
-        'Framework :: Wagtail :: 2',
         'Framework :: Wagtail :: 3',
         'Framework :: Wagtail :: 4',
+        'Framework :: Wagtail :: 5',
     ],
 )
```

### Comparing `wagtail-review-0.3.1/tests/migrations/0001_initial.py` & `wagtail-review-0.4/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/tests/settings.py` & `wagtail-review-0.4/tests/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from __future__ import absolute_import, unicode_literals
 
 import os
-import django
-
-from wagtail import VERSION as WAGTAIL_VERSION
 
 DATABASES = {
     'default': {
         'ENGINE': os.environ.get('DATABASE_ENGINE', 'django.db.backends.sqlite3'),
         'NAME': os.environ.get('DATABASE_NAME', 'wagtail_review'),
         'USER': os.environ.get('DATABASE_USER', None),
         'PASSWORD': os.environ.get('DATABASE_PASS', None),
@@ -55,28 +52,25 @@
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
 ]
 
-if WAGTAIL_VERSION < (2, 9):
-    MIDDLEWARE.append('wagtail.core.middleware.SiteMiddleware')
-
 INSTALLED_APPS = (
     'wagtail_review',
     'tests',
 
     'wagtail.search',
     'wagtail.sites',
     'wagtail.users',
     'wagtail.images',
     'wagtail.documents',
     'wagtail.admin',
-    'wagtail.core',
+    'wagtail',
 
     'taggit',
 
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
@@ -85,8 +79,9 @@
 )
 
 PASSWORD_HASHERS = (
     'django.contrib.auth.hashers.MD5PasswordHasher',  # don't use the intentionally slow default password hasher
 )
 
 WAGTAIL_SITE_NAME = 'wagtail-review test'
-BASE_URL = 'http://test.local'
+WAGTAILADMIN_BASE_URL = 'http://test.local'
+ALLOWED_HOSTS = ['localhost', 'testserver']
```

### Comparing `wagtail-review-0.3.1/tests/test_admin.py` & `wagtail-review-0.4/tests/test_admin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 import json
 
 from django.contrib.auth.models import User
 from django.core import mail
 from django.test import TestCase
 
-from wagtail.core.models import Page
+from wagtail.models import Page
 
 from wagtail_review.models import Review
 
 
 class TestAdminViews(TestCase):
     fixtures = ['test.json']
 
     def setUp(self):
-        User.objects.create_superuser(username='admin', email='admin@example.com', password='password')
+        self.admin_user = User.objects.create_superuser(
+            username='admin', email='admin@example.com', password='password'
+        )
         self.assertTrue(
             self.client.login(username='admin', password='password')
         )
         self.homepage = Page.objects.get(url_path='/home/').specific
 
     def test_submit_for_review_action(self):
         """Test that 'submit for review' appears in the page action menu"""
         response = self.client.get('/admin/pages/%d/edit/' % self.homepage.pk)
         self.assertEqual(response.status_code, 200)
 
         self.assertContains(response, "Submit for review")
+        # check that the action button has a data-url attribute
+        self.assertContains(response, 'data-url="/admin/wagtail_review/create_review/"')
         # check that JS is imported
         self.assertContains(response, "wagtail_review/js/submit.js")
 
     def test_submit_for_review_action_on_create(self):
         """Test that 'submit for review' appears in the page action menu"""
         response = self.client.get('/admin/pages/add/tests/simplepage/%d/' % self.homepage.pk)
         self.assertEqual(response.status_code, 200)
 
         self.assertContains(response, "Submit for review")
+        # check that the action button has a data-url attribute
+        self.assertContains(response, 'data-url="/admin/wagtail_review/create_review/"')
         # check that JS is imported
         self.assertContains(response, "wagtail_review/js/submit.js")
 
     def test_create_review(self):
         response = self.client.get('/admin/wagtail_review/create_review/')
         self.assertEqual(response.status_code, 200)
         response_json = json.loads(response.content)
@@ -166,7 +172,36 @@
 
         reviewer_emails = set(reviewer.get_email_address() for reviewer in review.reviewers.all())
         self.assertEqual(reviewer_emails, {'admin@example.com', 'someone@example.com', 'spongebob@example.com'})
 
         self.assertEqual(len(mail.outbox), 2)
         email_recipients = set(email.to[0] for email in mail.outbox)
         self.assertEqual(email_recipients, {'someone@example.com', 'spongebob@example.com'})
+
+    def test_reviews_index(self):
+        revision = self.homepage.save_revision()
+        review = Review.objects.create(page_revision=revision, submitter=self.admin_user)
+        review.reviewers.create(user=self.admin_user)
+        review.reviewers.create(user=User.objects.get(username='spongebob'))
+        response = self.client.get('/admin/wagtail_review/reviews/')
+        self.assertEqual(response.status_code, 200)
+        self.assertContains(response, '<a href="/admin/wagtail_review/reviews/%d/">Home</a>' % self.homepage.pk, html=True)
+        self.assertContains(response, '<td class="status">Open</td>', html=True)
+
+    def test_review_audit_trail(self):
+        revision = self.homepage.save_revision()
+        review = Review.objects.create(page_revision=revision, submitter=self.admin_user)
+        review.reviewers.create(user=self.admin_user)
+        review.reviewers.create(user=User.objects.get(username='spongebob'))
+        response = self.client.get('/admin/wagtail_review/reviews/%d/' % self.homepage.pk)
+        self.assertEqual(response.status_code, 200)
+        self.assertContains(response, 'Review requested by admin')
+        self.assertContains(response, '<td>Spongebob Squarepants</td>')
+        self.assertContains(response, '<td>Awaiting response</td>')
+
+    def test_view_review(self):
+        revision = self.homepage.save_revision()
+        review = Review.objects.create(page_revision=revision, submitter=self.admin_user)
+        review.reviewers.create(user=self.admin_user)
+        review.reviewers.create(user=User.objects.get(username='spongebob'))
+        response = self.client.get('/admin/wagtail_review/reviews/%d/view/' % review.pk)
+        self.assertEqual(response.status_code, 200)
```

### Comparing `wagtail-review-0.3.1/tests/test_frontend.py` & `wagtail-review-0.4/tests/test_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.contrib.auth.models import User
 from django.test import TestCase
 
-from wagtail.core.models import Page, Site
+from wagtail.models import Page, Site
 
 from wagtail_review.models import Review, Reviewer
 from tests.models import SimplePage
 
 
 class TestFrontendViews(TestCase):
     fixtures = ['test.json']
```

### Comparing `wagtail-review-0.3.1/tests/test_models.py` & `wagtail-review-0.4/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.auth.models import User
 from django.core.exceptions import ValidationError
 from django.test import TestCase
 
-from wagtail.core.models import Page
+from wagtail.models import Page
 
 from wagtail_review.models import Review, Reviewer
 
 
 class TestReviewerModel(TestCase):
     fixtures = ['test.json']
```

### Comparing `wagtail-review-0.3.1/tests/urls.py` & `wagtail-review-0.4/tests/urls.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import absolute_import, unicode_literals
 
 from django.conf.urls import include
-from django.urls import re_path
+from django.urls import path
 
 from wagtail.admin import urls as wagtailadmin_urls
-from wagtail.core import urls as wagtail_urls
+from wagtail import urls as wagtail_urls
 
 from wagtail_review import urls as wagtailreview_urls
 
 
 urlpatterns = [
-    re_path(r'^admin/', include(wagtailadmin_urls)),
-    re_path(r'^review/', include(wagtailreview_urls)),
+    path(r'admin/', include(wagtailadmin_urls)),
+    path(r'review/', include(wagtailreview_urls)),
 
     # For anything not caught by a more specific rule above, hand over to
     # Wagtail's serving mechanism
-    re_path(r'', include(wagtail_urls)),
+    path('', include(wagtail_urls)),
 ]
```

### Comparing `wagtail-review-0.3.1/wagtail_review/forms.py` & `wagtail-review-0.4/wagtail_review/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/migrations/0001_initial.py` & `wagtail-review-0.4/wagtail_review/migrations/0001_initial.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,55 +6,52 @@
 from django.db import migrations, models
 from django.db.migrations.recorder import MigrationRecorder
 import django.db.models.deletion
 from wagtail import VERSION as WAGTAIL_VERSION
 
 
 def get_run_before_and_revision_model():
-    # Keep the existing behaviour for Wagtail pre-4.0.
-    run_before = []
+    # The return value of this function is used in the Migration class
+    # definition, so everything in this check happens at module load time
+    # (i.e. at the start of the `migrate` command).
+
+    # Changing the core migration dependency potentially breaks existing
+    # users as it can cause an InconsistentMigrationHistory error.
+
+    # Based on the dependencies, this migration can be run both before or
+    # after the PageRevision model is renamed to Revision. As a result,
+    # we cannot accurately determine the revision_model to use.
+
+    # What we can do instead is keep pointing to the old PageRevision name,
+    # but use run_before to make sure that this migration is run before the
+    # core migration that renames the PageRevision model.
+    run_before = [("wagtailcore", "0070_rename_pagerevision_revision")]
     revision_model = "wagtailcore.PageRevision"
-    if WAGTAIL_VERSION >= (4, 0, 0):
-        # The return value of this function is used in the Migration class
-        # definition, so everything in this check happens at module load time
-        # (i.e. at the start of the `migrate` command).
-
-        # Changing the core migration dependency potentially breaks existing
-        # users as it can cause an InconsistentMigrationHistory error.
-
-        # Based on the dependencies, this migration can be run both before or
-        # after the PageRevision model is renamed to Revision. As a result,
-        # we cannot accurately determine the revision_model to use.
-
-        # What we can do instead is keep pointing to the old PageRevision name,
-        # but use run_before to make sure that this migration is run before the
-        # core migration that renames the PageRevision model.
-        run_before = [("wagtailcore", "0070_rename_pagerevision_revision")]
-
-        try:
-            if MigrationRecorder.Migration.objects.filter(
-                app="wagtailcore", name="0070_rename_pagerevision_revision"
-            ).exists():
-                # However, if the core migration has already been applied in a
-                # previous `migrate` run, we should unset run_before to avoid an
-                # InconsistentMigrationHistory error.
-
-                # This might be the case if the core migration was run
-                # separately and an earlier version of wagtail-localize were
-                # already installed where we did not ensure this migration was
-                # run before the core migration.
-                run_before = []
-
-                # In any case, it should be safe to point to the new Revision
-                # model name as the core migration has already been applied.
-                revision_model = "wagtailcore.Revision"
-
-        except (django.db.utils.OperationalError, django.db.utils.ProgrammingError):
-            # Normally happens when running tests
-            pass
+
+    try:
+        if MigrationRecorder.Migration.objects.filter(
+            app="wagtailcore", name="0070_rename_pagerevision_revision"
+        ).exists():
+            # However, if the core migration has already been applied in a
+            # previous `migrate` run, we should unset run_before to avoid an
+            # InconsistentMigrationHistory error.
+
+            # This might be the case if the core migration was run
+            # separately and an earlier version of wagtail-localize were
+            # already installed where we did not ensure this migration was
+            # run before the core migration.
+            run_before = []
+
+            # In any case, it should be safe to point to the new Revision
+            # model name as the core migration has already been applied.
+            revision_model = "wagtailcore.Revision"
+
+    except (django.db.utils.OperationalError, django.db.utils.ProgrammingError):
+        # Normally happens when running tests
+        pass
 
     return run_before, revision_model
 
 
 class Migration(migrations.Migration):
 
     initial = True
```

### Comparing `wagtail-review-0.3.1/wagtail_review/migrations/0002_annotation_annotationrange.py` & `wagtail-review-0.4/wagtail_review/migrations/0002_annotation_annotationrange.py`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/migrations/0003_response.py` & `wagtail-review-0.4/wagtail_review/migrations/0003_response.py`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/models.py` & `wagtail-review-0.4/wagtail_review/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,41 +8,33 @@
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 
 import swapper
 
-try:
-    from wagtail.admin.mail import send_mail  # Wagtail >= 2.7
-except ImportError:
-    from wagtail.admin.utils import send_mail  # Wagtail < 2.7
+from wagtail.admin.mail import send_mail
 
-from wagtail import VERSION as WAGTAIL_VERSION
-from wagtail.core.models import UserPagePermissionsProxy
+from wagtail.models import UserPagePermissionsProxy
 
 from wagtail_review.text import user_display_name
 
 
 # make the setting name WAGTAILREVIEW_REVIEW_MODEL rather than WAGTAIL_REVIEW_REVIEW_MODEL
 swapper.set_app_prefix('wagtail_review', 'wagtailreview')
 
 
 REVIEW_STATUS_CHOICES = [
     ('open', _("Open")),
     ('closed', _("Closed")),
 ]
 
 
-if WAGTAIL_VERSION >= (4, 0):
-    revision_model = "wagtailcore.Revision"
-    revision_page_fk_relation = "page_revision__object_id"
-else:
-    revision_model = "wagtailcore.PageRevision"
-    revision_page_fk_relation = "page_revision__page_id"
+revision_model = "wagtailcore.Revision"
+revision_page_fk_relation = "page_revision__object_id"
 
 class BaseReview(models.Model):
     """
     Abstract base class for Review models. Can be subclassed to specify application-specific fields, e.g. review type
     """
     page_revision = models.ForeignKey(revision_model, related_name='+', on_delete=models.CASCADE, editable=False)
     status = models.CharField(max_length=30, default='open', choices=REVIEW_STATUS_CHOICES, editable=False)
@@ -52,15 +44,15 @@
     def send_request_emails(self):
         # send request emails to all reviewers except the reviewer record for the user submitting the request
         for reviewer in self.reviewers.exclude(user=self.submitter):
             reviewer.send_request_email()
 
     @cached_property
     def revision_as_page(self):
-        return self.page_revision.as_page_object()
+        return self.page_revision.as_object()
 
     def get_annotations(self):
         return Annotation.objects.filter(reviewer__review=self).prefetch_related('ranges')
 
     def get_responses(self):
         return Response.objects.filter(reviewer__review=self).order_by('created_at').select_related('reviewer')
 
@@ -136,21 +128,21 @@
             self.view_token = generate_token()
 
         super().save(**kwargs)
 
     def get_respond_url(self, absolute=False):
         url = reverse('wagtail_review:respond', args=[self.id, self.response_token])
         if absolute:
-            url = settings.BASE_URL + url
+            url = settings.WAGTAILADMIN_BASE_URL + url
         return url
 
     def get_view_url(self, absolute=False):
         url = reverse('wagtail_review:view', args=[self.id, self.view_token])
         if absolute:
-            url = settings.BASE_URL + url
+            url = settings.WAGTAILADMIN_BASE_URL + url
         return url
 
     def send_request_email(self):
         email_address = self.get_email_address()
 
         context = {
             'email': email_address,
```

### Comparing `wagtail-review-0.3.1/wagtail_review/static/wagtail_review/css/annotator.css` & `wagtail-review-0.4/wagtail_review/static/wagtail_review/css/annotator.css`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/static/wagtail_review/css/create_review.css` & `wagtail-review-0.4/wagtail_review/static/wagtail_review/css/create_review.css`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/static/wagtail_review/css/respond.css` & `wagtail-review-0.4/wagtail_review/static/wagtail_review/css/respond.css`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/static/wagtail_review/js/annotator-2.0.0a3.min.js` & `wagtail-review-0.4/wagtail_review/static/wagtail_review/js/annotator-2.0.0a3.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/static/wagtail_review/js/annotator-extensions.js` & `wagtail-review-0.4/wagtail_review/static/wagtail_review/js/annotator-extensions.js`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/static/wagtail_review/js/submit.js` & `wagtail-review-0.4/wagtail_review/static/wagtail_review/js/submit.js`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/admin/audit_trail.html` & `wagtail-review-0.4/wagtail_review/templates/wagtail_review/admin/audit_trail.html`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 </table>
 
                 <ul class="actions">
                     <li>
                         <a class="button button-secondary button-small" href="{% url 'wagtail_review_admin:view_review_page' review_id=review.id %}">{% trans "View page" %}</a>
                     </li>
                     <li>
-                        <a class="button button-secondary button-small" href="{% url 'wagtailadmin_pages:edit' review.page_revision.page.id %}">{% trans "Edit page" %}</a>
+                        <a class="button button-secondary button-small" href="{% url 'wagtailadmin_pages:edit' review.page_revision.object_id %}">{% trans "Edit page" %}</a>
                     </li>
                     {% if review.status == 'closed' %}
                         <li>
                             <form action="{% url 'wagtail_review_admin:reopen_review' review_id=review.id %}" method="POST">
                                 {% csrf_token %}
                                 <button class="button button-secondary button-small">{% trans "Reopen" %}</button>
                             </form>
```

### Comparing `wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/admin/dashboard.html` & `wagtail-review-0.4/wagtail_review/templates/wagtail_review/admin/dashboard.html`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/annotate.html` & `wagtail-review-0.4/wagtail_review/templates/wagtail_review/annotate.html`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/create_review.html` & `wagtail-review-0.4/wagtail_review/templates/wagtail_review/create_review.html`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/email/request_review.txt` & `wagtail-review-0.4/wagtail_review/templates/wagtail_review/email/request_review.txt`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/templates/wagtail_review/email/response_received.txt` & `wagtail-review-0.4/wagtail_review/templates/wagtail_review/email/response_received.txt`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/templatetags/wagtailreview_tags.py` & `wagtail-review-0.4/wagtail_review/templatetags/wagtailreview_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/text.py` & `wagtail-review-0.4/wagtail_review/text.py`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/views/admin.py` & `wagtail-review-0.4/wagtail_review/views/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from django.contrib.auth import get_user_model
+from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import PermissionDenied
 from django.db.models import Q
 from django.http import JsonResponse
 from django.shortcuts import get_object_or_404, redirect
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.http import require_POST
 from django.views.generic.detail import DetailView
 
 import swapper
 
-from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail.admin import messages
 from wagtail.admin.modal_workflow import render_modal_workflow
 from wagtail.admin.views import generic
+from wagtail.models import Page
 
 from wagtail_review.forms import get_review_form_class, ReviewerFormSet
 from wagtail_review.models import Reviewer
 from wagtail_review.text import user_display_name
 
 
 Review = swapper.load_model('wagtail_review', 'Review')
@@ -115,15 +116,16 @@
     def get_object(self):
         return super().get_object().specific
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
 
         context['reviews'] = Review.objects.filter(
-            page_revision__page=self.object
+            page_revision__object_id=str(self.object.pk),
+            page_revision__base_content_type=ContentType.objects.get_for_model(Page)
         ).order_by('created_at').select_related('submitter').prefetch_related('reviewers__responses')
         context['page_permissions'] = self.object.permissions_for_user(self.request.user)
 
         return context
 
 
 def view_review_page(request, review_id=None):
@@ -134,50 +136,44 @@
     try:
         reviewer = review.reviewers.get(user=request.user)
     except Reviewer.DoesNotExist:
         # current user is not participating in the review;
         # if they have edit access to the page, give them the submitter's
         # read-only credentials so that they can see annotations
 
-        page = review.page_revision.as_page_object()
+        page = review.page_revision.as_object()
         perms = page.permissions_for_user(request.user)
 
         if not (perms.can_edit() or perms.can_publish()):
             raise PermissionDenied
 
         try:
             reviewer = review.reviewers.get(user=review.submitter)
         except Reviewer.DoesNotExist:
             raise PermissionDenied
 
-    page = review.page_revision.as_page_object()
+    page = review.page_revision.as_object()
     if reviewer.user == request.user:
         review_mode = 'comment'
     else:
         review_mode = 'view'
 
-    if WAGTAIL_VERSION < (2, 7):
-        dummy_request = page.dummy_request(request)
-        dummy_request.wagtailreview_reviewer = reviewer
-        dummy_request.wagtailreview_mode = review_mode
-        return page.serve_preview(dummy_request, page.default_preview_mode)
-    else:
-        return page.make_preview_request(
-            original_request=request,
-            extra_request_attrs={
-                'wagtailreview_reviewer': reviewer,
-                'wagtailreview_mode': review_mode,
-            }
-        )
+    return page.make_preview_request(
+        original_request=request,
+        extra_request_attrs={
+            'wagtailreview_reviewer': reviewer,
+            'wagtailreview_mode': review_mode,
+        }
+    )
 
 
 @require_POST
 def close_review(request, review_id=None):
     review = get_object_or_404(Review, id=review_id)
-    page = review.page_revision.as_page_object()
+    page = review.page_revision.as_object()
     perms = page.permissions_for_user(request.user)
 
     if not (perms.can_edit() or perms.can_publish()):
         raise PermissionDenied
 
     review.status = 'closed'
     review.save()
@@ -186,15 +182,15 @@
 
     return redirect('wagtail_review_admin:audit_trail', page.id)
 
 
 @require_POST
 def close_and_publish(request, review_id=None):
     review = get_object_or_404(Review, id=review_id)
-    page = review.page_revision.as_page_object()
+    page = review.page_revision.as_object()
     perms = page.permissions_for_user(request.user)
     if not perms.can_publish():
         raise PermissionDenied
 
     review.status = 'closed'
     review.save()
     review.page_revision.publish()
@@ -203,15 +199,15 @@
 
     return redirect('wagtail_review_admin:audit_trail', page.id)
 
 
 @require_POST
 def reopen_review(request, review_id=None):
     review = get_object_or_404(Review, id=review_id)
-    page = review.page_revision.as_page_object()
+    page = review.page_revision.as_object()
     perms = page.permissions_for_user(request.user)
 
     if not (perms.can_edit() or perms.can_publish()):
         raise PermissionDenied
 
     review.status = 'open'
     review.save()
```

### Comparing `wagtail-review-0.3.1/wagtail_review/views/annotations_api.py` & `wagtail-review-0.4/wagtail_review/views/annotations_api.py`

 * *Files identical despite different names*

### Comparing `wagtail-review-0.3.1/wagtail_review/views/frontend.py` & `wagtail-review-0.4/wagtail_review/views/frontend.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 from django.contrib import messages
 from django.core.exceptions import PermissionDenied
 from django.http import HttpResponse
 from django.middleware.csrf import get_token as get_csrf_token
 from django.shortcuts import get_object_or_404, redirect
 from django.urls import reverse
 
-from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail_review.forms import ResponseForm
 from wagtail_review.models import Response, Reviewer
 
 SUCCESS_RESPONSE_MESSAGE = "Thank you, your review has been received."
 
 
 def view(request, reviewer_id, token):
     reviewer = get_object_or_404(Reviewer, id=reviewer_id)
     if token != reviewer.view_token:
         raise PermissionDenied
 
-    page = reviewer.review.page_revision.as_page_object()
-    if WAGTAIL_VERSION < (2, 7):
-        dummy_request = page.dummy_request(request)
-        dummy_request.wagtailreview_mode = 'view'
-        dummy_request.wagtailreview_reviewer = reviewer
-        return page.serve_preview(dummy_request, page.default_preview_mode)
-    else:
-        return page.make_preview_request(
-            original_request=request,
-            extra_request_attrs={
-                'wagtailreview_mode': 'view',
-                'wagtailreview_reviewer': reviewer,
-            }
-        )
+    page = reviewer.review.page_revision.as_object()
+    return page.make_preview_request(
+        original_request=request,
+        extra_request_attrs={
+            'wagtailreview_mode': 'view',
+            'wagtailreview_reviewer': reviewer,
+        }
+    )
 
 
 def respond(request, reviewer_id, token):
     reviewer = get_object_or_404(Reviewer, id=reviewer_id)
     if token != reviewer.response_token:
         raise PermissionDenied
 
@@ -46,28 +39,20 @@
             response.send_notification_to_submitter()
             if request.user.has_perm('wagtailadmin.access_admin'):
                 messages.success(request, SUCCESS_RESPONSE_MESSAGE)
                 return redirect(reverse('wagtail_review_admin:dashboard'))
             return HttpResponse(SUCCESS_RESPONSE_MESSAGE)
 
     else:
-        page = reviewer.review.page_revision.as_page_object()
+        page = reviewer.review.page_revision.as_object()
         # Fetch the CSRF token so that Django will return a set-cookie header in the case that this is
         # the user's first request, and ensure that the dummy request (where the submit-review form is
         # rendered) is using the same token
         get_csrf_token(request)
 
-        if WAGTAIL_VERSION < (2, 7):
-            dummy_request = page.dummy_request(request)
-            dummy_request.META["CSRF_COOKIE"] = request.META["CSRF_COOKIE"]
-
-            dummy_request.wagtailreview_mode = 'respond'
-            dummy_request.wagtailreview_reviewer = reviewer
-            return page.serve_preview(dummy_request, page.default_preview_mode)
-        else:
-            return page.make_preview_request(
-                original_request=request,
-                extra_request_attrs={
-                    'wagtailreview_mode': 'respond',
-                    'wagtailreview_reviewer': reviewer,
-                }
-            )
+        return page.make_preview_request(
+            original_request=request,
+            extra_request_attrs={
+                'wagtailreview_mode': 'respond',
+                'wagtailreview_reviewer': reviewer,
+            }
+        )
```

### Comparing `wagtail-review-0.3.1/wagtail_review/wagtail_hooks.py` & `wagtail-review-0.4/wagtail_review/wagtail_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from django.shortcuts import redirect
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
 
 import swapper
 
-from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail.admin import messages
 from wagtail.admin.action_menu import ActionMenuItem
 from wagtail.admin.menu import MenuItem
-from wagtail.core import hooks
+from wagtail import hooks
 
 from wagtail_review import admin_urls
 from wagtail_review.forms import get_review_form_class, ReviewerFormSet
 
 Review = swapper.load_model('wagtail_review', 'Review')
 
 
@@ -29,25 +28,16 @@
 
 
 # Replace 'submit for moderation' action with 'submit for review'
 
 class SubmitForReviewMenuItem(ActionMenuItem):
     label = _("Submit for review")
     name = 'action-submit-for-review'
-    if WAGTAIL_VERSION >= (2, 10):
-        template = 'wagtail_review/submit_for_review_menu_item.html'
-        icon_name = 'resubmit'
-    else:
-        template = 'wagtail_review/submit_for_review_menu_item_pre_2_10.html'
-
-    if WAGTAIL_VERSION < (2, 7):
-        def render_html(self, request, parent_context):
-            html = super().render_html(request, parent_context)
-            html = format_html('<li>{}</li>', html)
-            return html
+    template_name = 'wagtail_review/submit_for_review_menu_item.html'
+    icon_name = 'resubmit'
 
     class Media:
         js = ['wagtail_review/js/submit.js']
         css = {
             'all': ['wagtail_review/css/create_review.css']
         }
```

### Comparing `wagtail-review-0.3.1/wagtail_review.egg-info/SOURCES.txt` & `wagtail-review-0.4/wagtail_review.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 tests/test_frontend.py
 tests/test_models.py
 tests/urls.py
 tests/migrations/0001_initial.py
 tests/migrations/__init__.py
 wagtail_review/__init__.py
 wagtail_review/admin_urls.py
+wagtail_review/apps.py
 wagtail_review/forms.py
 wagtail_review/models.py
 wagtail_review/text.py
 wagtail_review/urls.py
 wagtail_review/wagtail_hooks.py
 wagtail_review.egg-info/PKG-INFO
 wagtail_review.egg-info/SOURCES.txt
@@ -35,15 +36,14 @@
 wagtail_review/static/wagtail_review/js/annotator-2.0.0a3.min.js
 wagtail_review/static/wagtail_review/js/annotator-extensions.js
 wagtail_review/static/wagtail_review/js/submit.js
 wagtail_review/templates/wagtail_review/annotate.html
 wagtail_review/templates/wagtail_review/create_review.html
 wagtail_review/templates/wagtail_review/response_form_fields.html
 wagtail_review/templates/wagtail_review/submit_for_review_menu_item.html
-wagtail_review/templates/wagtail_review/submit_for_review_menu_item_pre_2_10.html
 wagtail_review/templates/wagtail_review/admin/audit_trail.html
 wagtail_review/templates/wagtail_review/admin/dashboard.html
 wagtail_review/templates/wagtail_review/email/request_review.txt
 wagtail_review/templates/wagtail_review/email/request_review_subject.txt
 wagtail_review/templates/wagtail_review/email/response_received.txt
 wagtail_review/templates/wagtail_review/email/response_received_subject.txt
 wagtail_review/templatetags/__init__.py
```

