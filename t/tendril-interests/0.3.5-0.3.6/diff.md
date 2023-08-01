# Comparing `tmp/tendril-interests-0.3.5.tar.gz` & `tmp/tendril-interests-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-interests-0.3.5.tar", last modified: Mon Jul 31 07:13:50 2023, max compression
+gzip compressed data, was "tendril-interests-0.3.6.tar", last modified: Tue Aug  1 21:49:12 2023, max compression
```

## Comparing `tendril-interests-0.3.5.tar` & `tendril-interests-0.3.6.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.925600 tendril-interests-0.3.5/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-07-31 07:13:50.925600 tendril-interests-0.3.5/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.905603 tendril-interests-0.3.5/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.909602 tendril-interests-0.3.5/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.909602 tendril-interests-0.3.5/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.3.5/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.909602 tendril-interests-0.3.5/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.909602 tendril-interests-0.3.5/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-31 07:13:50.925600 tendril-interests-0.3.5/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3288 2023-07-29 05:48:32.000000 tendril-interests-0.3.5/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.905603 tendril-interests-0.3.5/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.909602 tendril-interests-0.3.5/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.5/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.909602 tendril-interests-0.3.5/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.5/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.909602 tendril-interests-0.3.5/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.5/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3703 2023-07-20 18:33:13.000000 tendril-interests-0.3.5/src/tendril/apiserver/routers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.913601 tendril-interests-0.3.5/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.3.5/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      102 2023-02-18 22:08:54.000000 tendril-interests-0.3.5/src/tendril/apiserver/templates/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    21379 2023-07-25 18:59:57.000000 tendril-interests-0.3.5/src/tendril/apiserver/templates/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7395 2023-07-26 09:37:44.000000 tendril-interests-0.3.5/src/tendril/apiserver/templates/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.913601 tendril-interests-0.3.5/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.3.5/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.913601 tendril-interests-0.3.5/src/tendril/authz/approvals/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.3.5/src/tendril/authz/approvals/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.3.5/src/tendril/authz/approvals/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-07-19 05:11:01.000000 tendril-interests-0.3.5/src/tendril/authz/approvals/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.913601 tendril-interests-0.3.5/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.3.5/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13869 2023-07-21 18:06:15.000000 tendril-interests-0.3.5/src/tendril/authz/roles/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.3.5/src/tendril/authz/roles/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.913601 tendril-interests-0.3.5/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.3.5/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.3.5/src/tendril/authz/scopes/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.913601 tendril-interests-0.3.5/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.5/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.917601 tendril-interests-0.3.5/src/tendril/common/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.5/src/tendril/common/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.3.5/src/tendril/common/interests/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.3.5/src/tendril/common/interests/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.3.5/src/tendril/common/interests/memberships.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      347 2023-07-20 16:55:21.000000 tendril-interests-0.3.5/src/tendril/common/interests/representations.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.3.5/src/tendril/common/states.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.917601 tendril-interests-0.3.5/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.3.5/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.3.5/src/tendril/config/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.917601 tendril-interests-0.3.5/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.5/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.917601 tendril-interests-0.3.5/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.3.5/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9944 2023-07-20 16:04:26.000000 tendril-interests-0.3.5/src/tendril/db/controllers/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4684 2023-07-20 16:05:06.000000 tendril-interests-0.3.5/src/tendril/db/controllers/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.917601 tendril-interests-0.3.5/src/tendril/db/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.3.5/src/tendril/db/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.3.5/src/tendril/db/mixins/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.917601 tendril-interests-0.3.5/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.3.5/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4751 2023-07-18 17:03:54.000000 tendril-interests-0.3.5/src/tendril/db/models/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.3.5/src/tendril/db/models/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.921600 tendril-interests-0.3.5/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.3.5/src/tendril/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    19122 2023-07-31 07:13:16.000000 tendril-interests-0.3.5/src/tendril/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7344 2023-07-19 05:16:07.000000 tendril-interests-0.3.5/src/tendril/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.921600 tendril-interests-0.3.5/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.3.5/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17517 2023-07-29 04:40:45.000000 tendril-interests-0.3.5/src/tendril/interests/mixins/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      284 2023-07-29 03:58:12.000000 tendril-interests-0.3.5/src/tendril/interests/mixins/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6240 2023-07-29 13:52:16.000000 tendril-interests-0.3.5/src/tendril/interests/mixins/monitors.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.921600 tendril-interests-0.3.5/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.3.5/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.921600 tendril-interests-0.3.5/src/tendril/libraries/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.3.5/src/tendril/libraries/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6009 2023-07-16 08:29:12.000000 tendril-interests-0.3.5/src/tendril/libraries/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2644 2023-04-09 05:14:23.000000 tendril-interests-0.3.5/src/tendril/libraries/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.921600 tendril-interests-0.3.5/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.3.5/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.3.5/src/tendril/libraries/mixins/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.921600 tendril-interests-0.3.5/src/tendril/monitors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril-interests-0.3.5/src/tendril/monitors/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1062 2023-07-29 12:20:20.000000 tendril-interests-0.3.5/src/tendril/monitors/spec.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.925600 tendril-interests-0.3.5/src/tendril_interests.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-07-31 07:13:50.000000 tendril-interests-0.3.5/src/tendril_interests.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2557 2023-07-31 07:13:50.000000 tendril-interests-0.3.5/src/tendril_interests.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-31 07:13:50.000000 tendril-interests-0.3.5/src/tendril_interests.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      586 2023-07-31 07:13:50.000000 tendril-interests-0.3.5/src/tendril_interests.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-31 07:13:50.000000 tendril-interests-0.3.5/src/tendril_interests.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-31 07:13:50.925600 tendril-interests-0.3.5/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.3.5/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.321773 tendril-interests-0.3.6/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-08-01 21:49:12.321773 tendril-interests-0.3.6/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.305773 tendril-interests-0.3.6/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.3.6/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-01 21:49:12.321773 tendril-interests-0.3.6/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3288 2023-07-29 05:48:32.000000 tendril-interests-0.3.6/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.305773 tendril-interests-0.3.6/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.6/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.6/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.6/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3703 2023-07-20 18:33:13.000000 tendril-interests-0.3.6/src/tendril/apiserver/routers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.3.6/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      812 2023-08-01 11:41:37.000000 tendril-interests-0.3.6/src/tendril/apiserver/templates/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    21775 2023-08-01 21:47:57.000000 tendril-interests-0.3.6/src/tendril/apiserver/templates/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7395 2023-07-26 09:37:44.000000 tendril-interests-0.3.6/src/tendril/apiserver/templates/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.3.6/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/authz/approvals/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.3.6/src/tendril/authz/approvals/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.3.6/src/tendril/authz/approvals/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-07-19 05:11:01.000000 tendril-interests-0.3.6/src/tendril/authz/approvals/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.3.6/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13869 2023-07-21 18:06:15.000000 tendril-interests-0.3.6/src/tendril/authz/roles/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.3.6/src/tendril/authz/roles/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.3.6/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.3.6/src/tendril/authz/scopes/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.6/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/common/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.6/src/tendril/common/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.3.6/src/tendril/common/interests/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.3.6/src/tendril/common/interests/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.3.6/src/tendril/common/interests/memberships.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      347 2023-07-20 16:55:21.000000 tendril-interests-0.3.6/src/tendril/common/interests/representations.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.3.6/src/tendril/common/states.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.3.6/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.3.6/src/tendril/config/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.6/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.3.6/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9944 2023-07-20 16:04:26.000000 tendril-interests-0.3.6/src/tendril/db/controllers/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4684 2023-07-20 16:05:06.000000 tendril-interests-0.3.6/src/tendril/db/controllers/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/db/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.3.6/src/tendril/db/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.3.6/src/tendril/db/mixins/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.3.6/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4751 2023-07-18 17:03:54.000000 tendril-interests-0.3.6/src/tendril/db/models/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.3.6/src/tendril/db/models/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.3.6/src/tendril/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    19717 2023-08-01 21:37:28.000000 tendril-interests-0.3.6/src/tendril/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7344 2023-07-19 05:16:07.000000 tendril-interests-0.3.6/src/tendril/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.3.6/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17517 2023-07-29 04:40:45.000000 tendril-interests-0.3.6/src/tendril/interests/mixins/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      284 2023-07-29 03:58:12.000000 tendril-interests-0.3.6/src/tendril/interests/mixins/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6240 2023-07-29 13:52:16.000000 tendril-interests-0.3.6/src/tendril/interests/mixins/monitors.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.3.6/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/libraries/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.3.6/src/tendril/libraries/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6009 2023-07-16 08:29:12.000000 tendril-interests-0.3.6/src/tendril/libraries/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2644 2023-04-09 05:14:23.000000 tendril-interests-0.3.6/src/tendril/libraries/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.3.6/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.3.6/src/tendril/libraries/mixins/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/monitors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril-interests-0.3.6/src/tendril/monitors/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1062 2023-07-29 12:20:20.000000 tendril-interests-0.3.6/src/tendril/monitors/spec.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril_interests.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2557 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      586 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.321773 tendril-interests-0.3.6/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/tox.ini
```

### Comparing `tendril-interests-0.3.5/.gitignore` & `tendril-interests-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/.readthedocs.yml` & `tendril-interests-0.3.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/.travis.yml` & `tendril-interests-0.3.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/LICENSE` & `tendril-interests-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/PKG-INFO` & `tendril-interests-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.3.5
+Version: 0.3.6
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril-interests-0.3.5/README.rst` & `tendril-interests-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/Makefile` & `tendril-interests-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/_static/custom.css` & `tendril-interests-0.3.6/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/_static/favicon.ico` & `tendril-interests-0.3.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/_static/logo.png` & `tendril-interests-0.3.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/_static/logo_packed.png` & `tendril-interests-0.3.6/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/_templates/about.html` & `tendril-interests-0.3.6/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/conf.py` & `tendril-interests-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/index.rst` & `tendril-interests-0.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/docs/installation.rst` & `tendril-interests-0.3.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/setup.py` & `tendril-interests-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/apiserver/routers/interests.py` & `tendril-interests-0.3.6/src/tendril/apiserver/routers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/apiserver/templates/interests.py` & `tendril-interests-0.3.6/src/tendril/apiserver/templates/interests.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,24 +128,16 @@
         """
         with get_session() as session:
             result = self._actual.possible_parents(user=user, session=session)
             return [x.export(auth_user=user, session=session,
                              include_roles=False,
                              include_permissions=False) for x in result]
 
-    def _inject_create_model(self, ep, param='item'):
-        orig_sig = signature(ep)
-        params = list(orig_sig.parameters.values())
-        orig_param = next(p for p in params if p.name == param)
-        index = params.index(orig_param)
-        new_param = orig_param.replace(name=orig_param.name, default=orig_param.default, kind=orig_param.kind,
-                                       annotation=self._actual.interest_class.tmodel_create)
-        params[index] = new_param
-        new_sig = orig_sig.replace(parameters=params)
-        return create_function(func_signature=new_sig, func_impl=ep)
+    def _inject_create_model(self, ep):
+        return self._inject_model(ep, param='item', model=self._actual.interest_class.tmodel_create)
 
     def create_item(self, item,
                     user: AuthUserModel = auth_spec()):
         """
         Create an Interest.
 
         This endpoint does not enforce interest access controls, and allows
@@ -166,14 +158,25 @@
 
         """
         with get_session() as session:
             item = self._actual.add_item(item, session=session)
             rv = item.export(session=session)
         return rv
 
+    def _inject_edit_model(self, ep):
+        return self._inject_model(ep, param='changes', model=self._actual.interest_class.tmodel_edit)
+
+    async def edit_item(self, id:int, changes,
+                        user: AuthUserModel = auth_spec()):
+        with get_session() as session:
+            item = self._actual.item(id, session=session)
+            result = item.edit(changes, auth_user=user, session=session)
+            rv = item.export(auth_user=user, session=session)
+        return rv
+
     async def activate_item(self, request: Request, id: int,
                             background_tasks: BackgroundTasks,
                             user: AuthUserModel = auth_spec()):
         """
         Activate a specified interest.
 
         This endpoint enforces interest access control, and executes only if
@@ -408,14 +411,20 @@
                                  dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
 
         router.add_api_route("/{id:int}", self.item, methods=["GET"],
                              response_model=self._actual.interest_class.tmodel,
                              response_model_exclude_none=True,
                              dependencies=[auth_spec(scopes=[f'{prefix}:read'])])
 
+        router.add_api_route("/{id:int}/edit", self._inject_edit_model(self.edit_item),
+                             methods=["POST"],
+                             response_model=self._actual.interest_class.tmodel,
+                             response_model_exclude_none=True,
+                             dependencies=[auth_spec(scopes=[f'{prefix}:read'])])
+
         if self._actual.enable_membership_api:
             router.add_api_route("/{id:int}/members", self.item_members, methods=["GET"],
                                  response_model=Dict[str, List[MembershipInfoTModel]],
                                  response_model_exclude_none=True,
                                  dependencies=[auth_spec(scopes=[f'{prefix}:read'])], )
             router.add_api_route("/{id:int}/members/{role}", self.item_role_members, methods=["GET"],
                                  response_model=List[MembershipInfoTModel],
```

### Comparing `tendril-interests-0.3.5/src/tendril/apiserver/templates/interests_approvals.py` & `tendril-interests-0.3.6/src/tendril/apiserver/templates/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/authz/approvals/interests.py` & `tendril-interests-0.3.6/src/tendril/authz/approvals/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/authz/approvals/manager.py` & `tendril-interests-0.3.6/src/tendril/authz/approvals/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/authz/roles/interests.py` & `tendril-interests-0.3.6/src/tendril/authz/roles/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/authz/roles/interests_approvals.py` & `tendril-interests-0.3.6/src/tendril/authz/roles/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/common/interests/approvals.py` & `tendril-interests-0.3.6/src/tendril/common/interests/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/common/interests/exceptions.py` & `tendril-interests-0.3.6/src/tendril/common/interests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/common/interests/memberships.py` & `tendril-interests-0.3.6/src/tendril/common/interests/memberships.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/config/__init__.py` & `tendril-interests-0.3.6/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/config/interests.py` & `tendril-interests-0.3.6/src/tendril/config/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/db/controllers/interests.py` & `tendril-interests-0.3.6/src/tendril/db/controllers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/db/controllers/interests_approvals.py` & `tendril-interests-0.3.6/src/tendril/db/controllers/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/db/models/interests.py` & `tendril-interests-0.3.6/src/tendril/db/models/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/db/models/interests_approvals.py` & `tendril-interests-0.3.6/src/tendril/db/models/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/interests/base.py` & `tendril-interests-0.3.6/src/tendril/interests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,30 +41,36 @@
 class InterestBaseCreateTModel(TendrilTBaseModel):
     name: str = Field(..., max_length=255)
     descriptive_name: Optional[str] = Field(..., max_length=255)
     type: Literal['interest']
     info: dict
 
 
+class InterestBaseEditTModel(TendrilTBaseModel):
+    descriptive_name: Optional[str] = Field(default="", max_length=255)
+    info: Optional[dict]
+
+
 class InterestBaseReadTMixin(TendrilTBaseModel):
     id: int
     roles: Optional[List[str]]
     permissions: Optional[List[str]]
     status: LifecycleStatus
 
 
 class InterestBaseTModel(InterestBaseCreateTModel,
                          InterestBaseReadTMixin):
     ...
 
 
 class InterestBase(object):
     model = InterestModel
-    tmodel_create = InterestBaseCreateTModel
     tmodel = InterestBaseTModel
+    tmodel_create = InterestBaseCreateTModel
+    tmodel_edit = InterestBaseEditTModel
     additional_fields = []
     additional_creation_fields = []
     additional_export_fields = []
     additional_activation_checks = []
 
     def __init__(self, name, info=None, must_create=False,
                  can_create=True, session=None):
@@ -103,14 +109,23 @@
             return self._model_instance.descriptive_name
 
     @with_db
     def set_descriptive_name(self, value, session=None):
         self._descriptive_name = value
         self._commit_to_db(session=session)
 
+    @with_db
+    @require_permission('edit', strip_auth=False, required=False)
+    def edit(self, changes, auth_user=None, session=None):
+        for field_name in changes.__fields__:
+            value = getattr(changes, field_name)
+            if value and hasattr(self.model_instance, field_name):
+                setattr(self.model_instance, field_name, value)
+        session.add(self.model_instance)
+
     @property
     def ident(self):
         return f"{self.__class__.__name__} {self.name}"
 
     @property
     def info(self):
         if self._info is not None:
```

### Comparing `tendril-interests-0.3.5/src/tendril/interests/manager.py` & `tendril-interests-0.3.6/src/tendril/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/interests/mixins/approvals.py` & `tendril-interests-0.3.6/src/tendril/interests/mixins/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/interests/mixins/monitors.py` & `tendril-interests-0.3.6/src/tendril/interests/mixins/monitors.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/libraries/interests/base.py` & `tendril-interests-0.3.6/src/tendril/libraries/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/libraries/interests/manager.py` & `tendril-interests-0.3.6/src/tendril/libraries/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril/monitors/spec.py` & `tendril-interests-0.3.6/src/tendril/monitors/spec.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril_interests.egg-info/PKG-INFO` & `tendril-interests-0.3.6/src/tendril_interests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.3.5
+Version: 0.3.6
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril-interests-0.3.5/src/tendril_interests.egg-info/SOURCES.txt` & `tendril-interests-0.3.6/src/tendril_interests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/src/tendril_interests.egg-info/requires.txt` & `tendril-interests-0.3.6/src/tendril_interests.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/tests/coveralls.py` & `tendril-interests-0.3.6/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.5/tox.ini` & `tendril-interests-0.3.6/tox.ini`

 * *Files identical despite different names*

