# Comparing `tmp/django-sphinx-hosting-1.2.0.tar.gz` & `tmp/django-sphinx-hosting-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sphinx-hosting-1.2.0.tar", last modified: Thu Jul 27 20:15:34 2023, max compression
+gzip compressed data, was "django-sphinx-hosting-1.2.1.tar", last modified: Mon Jul 31 23:15:50 2023, max compression
```

## Comparing `django-sphinx-hosting-1.2.0.tar` & `django-sphinx-hosting-1.2.1.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.233319 django-sphinx-hosting-1.2.0/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.2.0/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.2.0/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-07-27 20:15:34.233528 django-sphinx-hosting-1.2.0/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.2.0/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.181705 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     2913 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1281 2023-07-27 20:15:34.234727 django-sphinx-hosting-1.2.0/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-07-27 20:15:11.000000 django-sphinx-hosting-1.2.0/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.195402 django-sphinx-hosting-1.2.0/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-07-27 20:15:11.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.199204 django-sphinx-hosting-1.2.0/sphinx_hosting/api/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/apps.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5706 2023-07-27 18:03:47.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/serializers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1357 2023-07-27 20:06:34.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    13616 2023-07-27 17:25:04.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/views.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/exc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/fields.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.200055 django-sphinx-hosting-1.2.0/sphinx_hosting/fixtures/
--rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/fixtures/classifiers.json
--rw-rw-r--   0 cmalek     (501) admin       (80)      445 2023-07-26 17:59:23.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/form_fields.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8372 2023-07-27 17:56:55.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    23812 2023-07-26 23:12:09.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/importers.py
--rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/logging.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.200855 django-sphinx-hosting-1.2.0/sphinx_hosting/management/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.205343 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2649 2023-07-26 23:13:05.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/fix_broken_hrefs.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2566 2023-07-26 17:58:46.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/import_docs.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1624 2023-07-26 17:58:54.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/parse_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/print_classifier_tree.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2286 2023-07-26 17:59:35.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/print_doctree.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.216013 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/
--rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0001_initial.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0002_original_html.py
--rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0003_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0004_next_page_FK.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0005_orig_global_toc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0007_load_classifiers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0008_Version_archived.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0010_add_groups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0011_machinenamefield.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1838 2023-07-26 18:06:51.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0012_project_relatedlinks.py
--rw-r--r--   0 cmalek     (501) admin       (80)      521 2023-07-27 17:59:47.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    33617 2023-07-27 17:55:22.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/models.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/search_indexes.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      776 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/signals.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.175937 django-sphinx-hosting-1.2.0/sphinx_hosting/static/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.176285 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.220132 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
--rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
--rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.221139 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/images/
--rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.177017 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.176716 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/search/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.176833 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/search/indexes/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.222505 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
--rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.223152 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/sphinx_hosting/base.html
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.224383 django-sphinx-hosting-1.2.0/sphinx_hosting/templatetags/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/templatetags/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/templatetags/sphinx_hosting.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/types.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2205 2023-07-26 17:16:32.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1103 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/validators.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    26588 2023-07-27 17:58:45.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/views.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.230891 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/classifier.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.232936 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/core/
--rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/core/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/core/basic.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4701 2023-05-04 19:20:06.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/navigation.py
--rw-r--r--   0 cmalek     (501) admin       (80)    18051 2023-07-27 20:11:32.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/project.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/search.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8924 2023-07-27 18:29:50.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/sphinx_page.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/version.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.781903 django-sphinx-hosting-1.2.1/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.2.1/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.2.1/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-07-31 23:15:50.782094 django-sphinx-hosting-1.2.1/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.2.1/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.737920 django-sphinx-hosting-1.2.1/django_sphinx_hosting.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-07-31 23:15:50.000000 django-sphinx-hosting-1.2.1/django_sphinx_hosting.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2947 2023-07-31 23:15:50.000000 django-sphinx-hosting-1.2.1/django_sphinx_hosting.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-31 23:15:50.000000 django-sphinx-hosting-1.2.1/django_sphinx_hosting.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-07-31 23:15:50.000000 django-sphinx-hosting-1.2.1/django_sphinx_hosting.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-07-31 23:15:50.000000 django-sphinx-hosting-1.2.1/django_sphinx_hosting.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1281 2023-07-31 23:15:50.783284 django-sphinx-hosting-1.2.1/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-07-31 23:15:35.000000 django-sphinx-hosting-1.2.1/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.749320 django-sphinx-hosting-1.2.1/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-07-31 23:15:35.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.752828 django-sphinx-hosting-1.2.1/sphinx_hosting/api/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/api/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/api/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1122 2023-07-31 22:42:09.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/api/permissions.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5706 2023-07-27 18:03:47.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/api/serializers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1357 2023-07-27 20:06:34.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/api/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    13981 2023-07-31 19:04:28.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/api/views.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/exc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/fields.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.753416 django-sphinx-hosting-1.2.1/sphinx_hosting/fixtures/
+-rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/fixtures/classifiers.json
+-rw-rw-r--   0 cmalek     (501) admin       (80)      445 2023-07-26 17:59:23.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/form_fields.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8372 2023-07-27 17:56:55.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    24175 2023-07-31 22:51:10.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/importers.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/logging.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.754022 django-sphinx-hosting-1.2.1/sphinx_hosting/management/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/management/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.757746 django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2649 2023-07-26 23:13:05.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/fix_broken_hrefs.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2566 2023-07-26 17:58:46.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/import_docs.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1624 2023-07-26 17:58:54.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/parse_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/print_classifier_tree.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2286 2023-07-26 17:59:35.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/print_doctree.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.767463 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0001_initial.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0002_original_html.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0003_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0004_next_page_FK.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0005_orig_global_toc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0007_load_classifiers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0008_Version_archived.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0010_add_groups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0011_machinenamefield.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1838 2023-07-26 18:06:51.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0012_project_relatedlinks.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      521 2023-07-27 17:59:47.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    33617 2023-07-27 17:55:22.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/py.typed
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/search_indexes.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      776 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/signals.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.731655 django-sphinx-hosting-1.2.1/sphinx_hosting/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.731995 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.771281 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
+-rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.771893 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/images/
+-rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.732969 django-sphinx-hosting-1.2.1/sphinx_hosting/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.732495 django-sphinx-hosting-1.2.1/sphinx_hosting/templates/search/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.732726 django-sphinx-hosting-1.2.1/sphinx_hosting/templates/search/indexes/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.772900 django-sphinx-hosting-1.2.1/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.773388 django-sphinx-hosting-1.2.1/sphinx_hosting/templates/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/templates/sphinx_hosting/base.html
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.774380 django-sphinx-hosting-1.2.1/sphinx_hosting/templatetags/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/templatetags/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/templatetags/sphinx_hosting.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/types.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2205 2023-07-26 17:16:32.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1103 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/validators.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    26582 2023-07-31 19:00:50.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/views.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.779953 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/classifier.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-31 23:15:50.781563 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/core/
+-rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/core/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/core/basic.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4701 2023-05-04 19:20:06.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/navigation.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    18051 2023-07-27 20:11:32.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/project.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/search.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8924 2023-07-27 18:29:50.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/sphinx_page.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.2.0/LICENSE.txt` & `django-sphinx-hosting-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/PKG-INFO` & `django-sphinx-hosting-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.2.0
+Version: 1.2.1
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.2.0/README.md` & `django-sphinx-hosting-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/PKG-INFO` & `django-sphinx-hosting-1.2.1/django_sphinx_hosting.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.2.0
+Version: 1.2.1
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/SOURCES.txt` & `django-sphinx-hosting-1.2.1/django_sphinx_hosting.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 sphinx_hosting/signals.py
 sphinx_hosting/types.py
 sphinx_hosting/urls.py
 sphinx_hosting/validators.py
 sphinx_hosting/views.py
 sphinx_hosting/api/__init__.py
 sphinx_hosting/api/apps.py
+sphinx_hosting/api/permissions.py
 sphinx_hosting/api/serializers.py
 sphinx_hosting/api/urls.py
 sphinx_hosting/api/views.py
 sphinx_hosting/fixtures/classifiers.json
 sphinx_hosting/management/__init__.py
 sphinx_hosting/management/commands/__init__.py
 sphinx_hosting/management/commands/fix_broken_hrefs.py
```

### Comparing `django-sphinx-hosting-1.2.0/setup.cfg` & `django-sphinx-hosting-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/setup.py` & `django-sphinx-hosting-1.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-sphinx-hosting",
-    version="1.2.0",
+    version="1.2.1",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "django-braces >= 1.15.0",
         "django-crispy-forms>=1.14.0",
         "django-extensions >= 3.2.1",
         "django-filter >= 22.1",
@@ -18,15 +18,15 @@
         "django-theme-academy >= 0.3.5",
         "django-wildewidgets >= 0.16.7",
         "djangorestframework >= 3.14.0",
         "drf-spectacular >= 0.25.1",
         "crispy-bootstrap5",
         "humanize",
         "lxml >= 4.9.1",
-        "cssselect >= 1.2.0",
+        "cssselect >= 1.2.1",
         "rich"
     ],
     author="Caltech IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     url="https://github.com/caltechads/django-sphinx-hosting",
     description="Reusable Django app for hosting Sphinx documentation privately.",
     long_description=long_description,
```

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/api/serializers.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/api/urls.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/api/views.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     ProjectRelatedLink,
     Version,
     SphinxPage,
     SphinxImage,
 )
 from sphinx_hosting.importers import SphinxPackageImporter
 
+from .permissions import ChangeProjectPermission, AddVersionPermission
 from .serializers import (
     ClassifierSerializer,
     ProjectSerializer,
     ProjectRelatedLinkSerializer,
     VersionSerializer,
     VersionUploadSerializer,
     SphinxPageSerializer,
@@ -45,15 +46,18 @@
     class Meta:
         model: Type[Model] = Classifier
         fields: List[str] = ["name"]
 
 
 class ClassifierViewSet(viewsets.ModelViewSet):
 
-    permission_classes = [permissions.IsAuthenticated]
+    permission_classes = [
+        permissions.IsAuthenticated,
+        permissions.DjangoModelPermissions,
+    ]
     serializer_class = ClassifierSerializer
     queryset = Classifier.objects.all()
     filterset_class = ClassifierFilter
 
 
 class ProjectFilter(filters.FilterSet):
 
@@ -78,15 +82,18 @@
     class Meta:
         model: Type[Model] = Project
         fields: List[str] = ["title", "machine_name", "description", "classifier"]
 
 
 class ProjectViewSet(viewsets.ModelViewSet):
 
-    permission_classes = [permissions.IsAuthenticated]
+    permission_classes = [
+        permissions.IsAuthenticated,
+        permissions.DjangoModelPermissions,
+    ]
     serializer_class = ProjectSerializer
     queryset = Project.objects.all()
     filterset_class = ProjectFilter
 
     @action(detail=True)
     def latest_version(self, request: Request, pk: Optional[int] = None) -> Response:
         project = self.get_object()
@@ -145,15 +152,18 @@
     viewsets.GenericViewSet,
 ):
     """
     Users can get, list and delete :py:class:`sphinx_hosting.models.Version` objects,
     but they can't create or update them the normal Django way.
     """
 
-    permission_classes = [permissions.IsAuthenticated]
+    permission_classes = [
+        permissions.IsAuthenticated,
+        permissions.DjangoModelPermissions | ChangeProjectPermission,
+    ]
     serializer_class = VersionSerializer
     queryset = Version.objects.all()
     filterset_class = VersionFilter
 
 
 class VersionUploadView(APIView):
     """
@@ -176,15 +186,18 @@
                 -XPOST \\
                 -H "Authorization: Token __THE_API_TOKEN__" \\
                 -F 'file=@path/to/yourdocs.tar.gz' \\
                 https://sphinx-hosting.example.com/api/v1/version/import/
     """
 
     serializer_class = VersionUploadSerializer
-    permission_classes = [permissions.IsAuthenticated]
+    permission_classes = [
+        permissions.IsAuthenticated,
+        AddVersionPermission
+    ]
     parser_classes = (MultiPartParser,)
 
     def post(self, request: Request) -> Response:
         serializer = VersionUploadSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         with tempfile.TemporaryDirectory() as tmpdir:
             fs = FileSystemStorage(tmpdir)
@@ -389,11 +402,14 @@
             "project_description",
             "project_classifier"
         ]
 
 
 class ProjectRelatedLinkViewSet(viewsets.ModelViewSet):
 
-    permission_classes = [permissions.IsAuthenticated]
+    permission_classes = [
+        permissions.IsAuthenticated,
+        ChangeProjectPermission
+    ]
     serializer_class = ProjectRelatedLinkSerializer
     queryset = ProjectRelatedLink.objects.all()
     filterset_class = ProjectRelatedLinkFilter
```

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/fields.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/fields.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/fixtures/classifiers.json` & `django-sphinx-hosting-1.2.1/sphinx_hosting/fixtures/classifiers.json`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/forms.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/forms.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/importers.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/importers.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,28 +280,35 @@
                 data['title'] = data['indextitle']
             else:
                 data['title'] = SphinxPage.SPECIAL_PAGES[path]
 
     def _fix_link_hrefs(self, body: str) -> str:
         """
         Given an HTML body of a Sphinx page, update the ``<a href="path">``
-        references to be absolute.  If we don't do this, any links on the
-        index page the version will be relative to the index page, instead of
-        being relative to the root of the docs, and won't work.
+        references for "path" to be rendered at page render time.  If we don't
+        do this, a lot of links won't work, because they do
+        index page, instead of being relative to the root of the docs, and won't
+        work.
 
         Args:
             body: the HTML body of a Sphinx document
 
         Returns:
             ``body`` with its ``<a>`` urls and updated
         """
         if not body:
             return ''
+
+        # Parse the HTML body into an lxml tree
         html = lxml.html.fromstring(body)
+
+        # Find all internal references
         links = html.cssselect('a.reference.internal')
+
+        # For each link, update its URL to be rendered at page render time
         for link in links:
             href = link.attrib['href']
             anchor = None
             if '#' in href:
                 href, anchor = href.split('#')
             if href.endswith('/'):
                 href = href[:-1]
@@ -309,27 +316,32 @@
             link.attrib['href'] = "{{% url 'sphinx_hosting:sphinxpage--detail' project_slug='{}' version='{}' path='{}' %}}".format(
                 self.config['project'],
                 self.config['release'],
                 href
             )
             if anchor:
                 link.attrib['href'] += f'#{anchor}'
+
+        # Return the updated HTML body
         return lxml.html.tostring(html).decode('utf-8')
 
-    def _fix_page_body(self, path: str, data: Dict[str, Any]) -> None:
+    def _fix_page_body(self, data: Dict[str, Any]) -> None:
         """
         Do any work needed to prepare the page body before inserting into the
-        database.  This means
+        database.  This means:
 
         * Ensure the ``body`` key exists in ``data``
         * Update the ``img`` sources to point to our Django storage location.
           We uploaded them to our storage during :py:meth:`import_images`.
+        * Update the ``href``s for any ``<a>`` links to be rendered at page
+          render time.
+        * Update the ``<table>``s to have the CSS classes we need for them to
+          display nicely.
 
         Args:
-            path: the file path in the tarfile
             data: the JSON data from our file
         """
         if 'body' not in data or data['body'] is None:
             # Ensure we always have data['body'] defined as a string, for when
             # we create the SphinxPage, below
             data['body'] = ''
         data['orig_body'] = data['body']
@@ -472,15 +484,15 @@
             path: str = str(Path(*Path(member.name).parts[1:]))
             if path.endswith('.fjson'):
                 # files that contain page data will have a .fjson extension
                 path = path.replace('.fjson', '')
                 fd = cast(io.BufferedReader, package.extractfile(member))
                 data = json.loads(fd.read())
                 self._fix_page_title(path, data)
-                self._fix_page_body(path, data)
+                self._fix_page_body(data)
                 self._fix_toc(data)
                 page = SphinxPage(
                     version=version,
                     relative_path=path,
                     content=json.dumps(data),
                     title=data['title'],
                     orig_body=data['orig_body'],
```

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/fix_broken_hrefs.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/fix_broken_hrefs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/import_docs.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/import_docs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/parse_globaltoc.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/parse_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/print_classifier_tree.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/print_classifier_tree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/print_doctree.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/management/commands/print_doctree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0001_initial.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0002_original_html.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0002_original_html.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0003_globaltoc.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0003_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0004_next_page_FK.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0004_next_page_FK.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0005_orig_global_toc.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0005_orig_global_toc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0007_load_classifiers.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0007_load_classifiers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0009_SphinxPage_searchable.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0010_add_groups.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0010_add_groups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0011_machinenamefield.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0011_machinenamefield.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0012_project_relatedlinks.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0012_project_relatedlinks.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/models.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/models.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/search_indexes.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/settings.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/settings.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/signals.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/signals.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss` & `django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss` & `django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss` & `django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css` & `django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss` & `django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg` & `django-sphinx-hosting-1.2.1/sphinx_hosting/static/sphinx_hosting/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/templates/sphinx_hosting/base.html` & `django-sphinx-hosting-1.2.1/sphinx_hosting/templates/sphinx_hosting/base.html`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/urls.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/validators.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/validators.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/views.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,15 +289,15 @@
                         version.version,
                         version.head.relative_path
                     ]
                 ),
                 color='orange',
                 css_class='mb-3'
             )
-        if user.has_perm('sphinxhostingcore.change_project'):
+        if user.has_perm('sphinxhostingcore.add_version'):
             layout.add_sidebar_bare_widget(
                 VersionUploadBlock(form=VersionUploadForm(project=self.object))
             )
         if user.has_perm('sphinxhostingcore.delete_project'):
             layout.add_sidebar_form_button(
                 'Delete Project',
                 reverse('sphinx_hosting:project--delete', args=[self.object.machine_name]),
@@ -518,15 +518,15 @@
                         self.object.head.relative_path
                     ]
                 ),
                 color='primary',
                 css_class='mb-3'
             )
         user = cast(AbstractUser, self.request.user)
-        if user.has_perm('sphinxhostingcore.change_project'):
+        if user.has_perm('sphinxhostingcore.delete_version'):
             layout.add_sidebar_form_button(
                 'Delete Version',
                 reverse('sphinx_hosting:version--delete', args=[self.object.project.machine_name, self.object.version]),
                 color='outline-secondary',
                 confirm_text=_("Are you sure you want to delete this version?"),
             )
         return layout
@@ -541,15 +541,15 @@
 class VersionUploadView(
     LoginRequiredMixin,
     PermissionRequiredMixin,
     FormInvalidMessageMixin,
     FormValidMessageMixin,
     BaseFormView
 ):
-    permission_required: str = 'sphinxhostingcore.change_project'
+    permission_required: str = 'sphinxhostingcore.add_version'
     form_class = VersionUploadForm
 
     def get_form_valid_message(self) -> str:
         version = cast(Version, self.version)
         return f'Uploaded version "{version.version}" to project "{version.project.title}"'
 
     def form_valid(self, form: Form):
@@ -585,15 +585,15 @@
 
 
 class VersionDeleteView(
     LoginRequiredMixin,
     PermissionRequiredMixin,
     DeleteView
 ):
-    permission_required: str = 'sphinxhostingcore.change_project'
+    permission_required: str = 'sphinxhostingcore.delete_version'
     model: Type[Model] = Version
     slug_field: str = 'version'
     slug_url_kwarg: str = 'version'
 
     def get_queryset(self) -> QuerySet[Version]:
         """
         Pre-filter our default queryset so that we only are able to get
```

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/classifier.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/classifier.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/navigation.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/navigation.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/project.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/project.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/search.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/search.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/sphinx_page.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/sphinx_page.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/version.py` & `django-sphinx-hosting-1.2.1/sphinx_hosting/wildewidgets/version.py`

 * *Files identical despite different names*

